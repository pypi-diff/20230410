# Comparing `tmp/reacher-0.3.7-py2.py3-none-any.whl.zip` & `tmp/reacher-0.3.8-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 7938 bytes, number of entries: 6
+Zip file size: 7985 bytes, number of entries: 6
 -rw-rw-r--  2.0 unx       52 b- defN 23-Mar-26 10:19 reacher/__init__.py
--rw-rw-r--  2.0 unx    19620 b- defN 23-Apr-09 17:16 reacher/reacher.py
--rw-rw-r--  2.0 unx     6932 b- defN 23-Apr-09 17:55 reacher-0.3.7.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Apr-09 17:55 reacher-0.3.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-Apr-09 17:55 reacher-0.3.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      448 b- defN 23-Apr-09 17:55 reacher-0.3.7.dist-info/RECORD
-6 files, 27170 bytes uncompressed, 7130 bytes compressed:  73.8%
+-rw-rw-r--  2.0 unx    19231 b- defN 23-Apr-10 15:22 reacher/reacher.py
+-rw-rw-r--  2.0 unx     7010 b- defN 23-Apr-10 15:36 reacher-0.3.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Apr-10 15:36 reacher-0.3.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-Apr-10 15:36 reacher-0.3.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      448 b- defN 23-Apr-10 15:36 reacher-0.3.8.dist-info/RECORD
+6 files, 26859 bytes uncompressed, 7177 bytes compressed:  73.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: reacher/__init__.py
 Comment: 
 
 Filename: reacher/reacher.py
 Comment: 
 
-Filename: reacher-0.3.7.dist-info/METADATA
+Filename: reacher-0.3.8.dist-info/METADATA
 Comment: 
 
-Filename: reacher-0.3.7.dist-info/WHEEL
+Filename: reacher-0.3.8.dist-info/WHEEL
 Comment: 
 
-Filename: reacher-0.3.7.dist-info/top_level.txt
+Filename: reacher-0.3.8.dist-info/top_level.txt
 Comment: 
 
-Filename: reacher-0.3.7.dist-info/RECORD
+Filename: reacher-0.3.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## reacher/reacher.py

```diff
@@ -5,15 +5,14 @@
 from os import system
 from typing import List
 import os
 from paramiko import AutoAddPolicy, RSAKey, SSHClient
 from paramiko.auth_handler import AuthenticationException, SSHException
 from scp import SCPClient, SCPException
 import logging
-import shutil
 import socket
 import select
 import sys
 
 try:
     import SocketServer
 except ImportError:
@@ -178,15 +177,16 @@
         self,
         build_name: str,
         client: RemoteClient = None,
         host: str = None,
         port: int = 22,
         user: str = None,
         password: str = None,
-        ssh_key_filepath: str = None
+        ssh_key_filepath: str = None,
+        prefix_cmd: str = None,
     ):
 
         if client is None:
 
             assert (
                 host is not None
                 and user is not None
@@ -201,14 +201,16 @@
                 port=port,
             )
 
         self._client = client
     
         self._port_forwarding = PortForwarding(client=self._client)
 
+        self._prefix_cmd = prefix_cmd
+
         self._build_name = build_name
     
     @property
     def workspace_path(self):
 
         return os.path.join("/home", self._client.user, ".reacher")
     
@@ -241,32 +243,42 @@
 
     def setup(self):
 
         self._client.execute_command(
             f"mkdir -p {self.build_path} && mkdir -p {self.artifact_path} && mkdir -p {self.log_path}"
         )
 
-    def clear(self):
+    def cleanup(self, exclude: list = ["artifacts", "logs"]):
 
-        self._client.execute_command(
-            f"rm -rf {self.build_path}", suppress=True,
-        )
+        files = self.ls()
+        files_pruned = []
+
+        for x in files:
+            if any([f in x for f in exclude]):
+                continue
+            if x == "" or x == "." or x == "..":
+                continue
+            files_pruned.append(x)
+
+        if len(files_pruned) > 0:
+            cmd = f"rm -r {' '.join(files_pruned)}"
+            self.execute_command(cmd)
 
         self.setup()
 
-    def ls(self, folder: str = None, supress: bool = False):
+    def ls(self, folder: str = None):
 
         if folder is None:
             folder = self.build_path
         else:
             folder = os.path.join(self.build_path, folder)
 
         r = self.execute_command(
-            f"find {folder} -print",
-            suppress=supress,
+            f"find {folder} -mindepth 1 -print",
+            suppress=True,
             stream=False,
         ).replace("\n", "").split("\r")
 
         r = [x for x in r if x != "" and x != "."]
 
         return r
 
@@ -305,58 +317,61 @@
         self.put(artifact, self.artifact_path)
 
     def _wrap_command_in_screen(self, command: str, named_session: str = None):
 
         named_session = named_session if named_session is not None else uuid.uuid4()
 
         return f"screen -S {named_session} {command}"
+    
+    def _wrap_command_in_prefix(self, command: str):
+        
+        return f"{self._prefix_cmd};{command}"
 
     def execute_command(
         self,
         command,
         stream: bool = True,
         suppress: bool = False,
         named_session: str = None,
         wrap_in_screen: bool = False,
     ):  
 
         if wrap_in_screen:
             command = self._wrap_command_in_screen(command, named_session=named_session)
 
+        if self._prefix_cmd is not None:
+            command = self._wrap_command_in_prefix(command)
+
         command = f"cd {self.build_path} && {command}"
 
         return self._client.execute_command(
             command,
             stream=stream,
             suppress=suppress,
         )
 
     def execute(
         self,
         command: str,
-        file: str = None,
-        context_folder: str = None,
+        context: Union[str, List[str]] = None,
         named_session: str = None,
-    ):  
+        wrap_in_screen: bool = True,
+        cleanup_before: bool = True,
+    ):      
+        
+        if cleanup_before:
+            self.cleanup()
 
-        if file is not None:
-            self._client.upload_dir(file, self.build_path)
-        if context_folder is not None:
-            e = context_folder.split("/")[-1]
-            intermidiate = os.path.join(self.build_path, "trash0")
-            self._client.upload_dir(context_folder, intermidiate)
-            self.execute_command(
-                f"mv {intermidiate}/{e}/* {self.build_path} && rm -r {intermidiate}",
-                wrap_in_screen=False,
-            )
+        if context is not None:
+            self._client.upload_dir(context, self.build_path)
 
         self.execute_command(
             command,
             named_session=named_session,
-            wrap_in_screen=True,
+            wrap_in_screen=wrap_in_screen,
         )
 
     def list_named_sessions(self):
 
         self.execute_command(f"screen -list")
 
     def attach_named_session(self, named_session: str):
@@ -421,22 +436,22 @@
         if self.exists:
             self._client.execute_command(
                 f"docker rm {self._build_name}", suppress=True,
             )
 
         super().clear()
 
-    def ls(self, folder: str = None, supress: bool = False):
+    def ls(self, folder: str = None):
 
         if folder is None:
             folder = "."
 
         r = self.execute_command(
-            f"find {folder} -print",
-            suppress=supress,
+            f"find {folder} -mindepth 1 -print",
+            suppress=True,
             stream=False,
         ).replace("\n", "").split("\r")
 
         r = [x for x in r if x != "" and x != "."]
 
         return r
 
@@ -465,66 +480,42 @@
 
         return self._client.execute_command(
             command,
             stream=stream,
             suppress=suppress,
         )
 
-    def clear_container(self):
-
-        files = self.ls(supress=True)
-        files_pruned = []
-
-        for x in files:
-            if any([f in x for f in self.MOUNTED]):
-                continue
-            if x == "" or x == "." or x == "..":
-                continue
-            files_pruned.append(x)
-        
-        if len(files_pruned) > 0:
-            cmd = f"rm -r {' '.join(files_pruned)}"
-            self.execute_command(cmd)
-
     def execute(
         self,
         command: str,
-        file: str = None,
-        context_folder: str = None,
+        context: Union[str, List[str]] = None,
         named_session: str = None,
-        clear_container: bool = False,
+        cleanup_before: bool = False,
+        wrap_in_screen: bool = True,
     ):  
 
-        if clear_container:
-            self.clear_container()
+        if cleanup_before:
+            self.cleanup()
 
-        tmp_path = os.path.join(self.build_path, "src")
+        tmp_path = os.path.join(self.build_path, "tmp")
         self._client.execute_command(f"mkdir -p {tmp_path}")
 
-        if file is not None:
-            self._client.upload_dir(file, tmp_path)
-        
-        if context_folder is not None:
-            e = context_folder.split("/")[-1]
-            intermidiate = os.path.join(self.build_path, "trash0")
-            self._client.upload_dir(context_folder, intermidiate)
-            self._client.execute_command(
-                f"mv {intermidiate}/{e}/* {tmp_path} && rm -r {intermidiate}"
-            )
+        if context is not None:
+            self._client.upload_dir(context, tmp_path)
 
         self._client.execute_command(
             f"docker cp {tmp_path}/. {self._build_name}:/{ReacherDocker.CON_WORKSPACE_PATH}"
         )
 
         self._client.execute_command(f"rm -r {tmp_path}")
 
         self.execute_command(
             command,
             named_session=named_session,
-            wrap_in_screen=True
+            wrap_in_screen=wrap_in_screen
         )
 
     def setup(
         self,
         ports: List[int] = None,
         envs: Dict[str, str] = None,
         command: str = "sleep infinity",
@@ -646,17 +637,17 @@
     ForwardServer(("", local_port), SubHander).serve_forever()
     
 
 def forward_tunnel_system(
         local_port,
         remote_port,
         client,
-):
+):  
 
-    command = f"ssh -L {local_port}:localhost:{remote_port} -N {client.user}@{client.host} -p {client.port}"
+    command = f"ssh -o StrictHostKeyChecking=no -i {client.ssh_key_filepath} -L 0.0.0.0:{local_port}:localhost:{remote_port} -N {client.user}@{client.host} -p {client.port}"
     
     os.system(command)
     
 import threading
     
 class PortForwarding(object):
```

## Comparing `reacher-0.3.7.dist-info/METADATA` & `reacher-0.3.8.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reacher
-Version: 0.3.7
+Version: 0.3.8
 Summary: A tool for reaching out to remote machine - excecute code and collect artificats
 Home-page: https://github.com/johannes-skog/reacher
 Author: johannes skog
 Author-email: johannes.skog.unsec@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -52,15 +52,15 @@
 the connection is sent to ReacherDocker together with the name of the image that we want to build and the name of the container.
 
 ```python
 reacher = ReacherDocker(
     client=client,
     build_name="base",
     image_name="base",
-    build_context="dockercontext"
+    build_context="dockercontext",
 )
 ```
 
 or send in the aruments for RemoteClient direcly to Reacher
 
 ```python
 reacher = ReacherDocker(
@@ -108,18 +108,21 @@
 
 ```python
 reacher = Reacher(
     build_name="base",
     host=config["HOST"],
     user=config["USER"],
     password=config["PASSWORD"],
-    ssh_key_filepath=config["SSH_KEY_PATH"]
+    ssh_key_filepath=config["SSH_KEY_PATH"],
+    prefix_cmd="PATH=...."
 )
 ```
 
+```prefix_cmd``` is useful to set when we want to specify some PATH or when we want to source an venv before running a command. 
+
 # Port-forwarding between remote and local
 
 If you want to access some service on the remote, you can forward the traffic on the ports of the remote to the local machine.
 
 ```python
 reacher.add_port_forward(remote_port=6006, local_port=5998, paramiko=True)
 ```
@@ -148,14 +151,15 @@
 # Running commands on the remote 
 
 ```python
 reacher.execute_command("ls", wrap_in_screen=True, named_session="test")
 ```
 
 wrap the command in a screen if running something that you want make persistent. If named_session is not specified an unique id will be created for the sesssion.
+```reacher.list_named_sessions()``` will list current sessions and ```reacher.kill_named_sessions(<session_name>)``` will kill the selected session.
 
 # Running code on the remote 
 
 ## Running a code-snippet 
 
 Now we have built the docker image on the remote and have a container ready to execute whatever code that we want to run.
 
@@ -172,27 +176,22 @@
     time.sleep(1)
 ```
 
 and then we execute it on the remote inside our controlled docker enviroment.
 
 ```python
 reacher.execute(
-    file="simple_test.py",
     command="python simple_test.py",
+    context=["simple_test.py"],
     named_session="simple_test",
-    # Before sending the code to the remote, clean the container from previous runs.
-    clear_container=True, 
+    # clean the container from previous runs.
+    cleanup_before=True, 
+    wrap_in_screen=True,
 )
 
-Preparing to copy...
-
-Copying to container - 2.56kB
-
-Successfully copied 2.56kB to base://workspace
-
 Hello from remote
 Hello from remote
 ...
 ```
 
 simple_test will continue to run in the background (even if you kill the cell/script that you instantiated the reacher.execute from) until we explicitly have killed it.
 
@@ -200,18 +199,16 @@
 
 ```python
 reacher.list_named_sessions()
 There is a screen on:
 	22.simple_test	(03/19/23 18:20:07)	(Attached)
 1 Socket in /run/screen/S-root.
 ```
-
 we can always attach to a named session to continue to get printouts.
 
-
 ```python
 reacher.attach_named_session("simple_test")
 ```
 
 or kill it
 
 ```python
@@ -227,23 +224,16 @@
 %%writefile dependency_test.py
 from dependency import Dependency
 d = Dependency()
 ```
 
 ```python
 reacher.execute(
-    context_folder="src",
-    file="dependency_test.py",
     command="python dependency_test.py",
+    context=["src", "dependency_test.py"],
     named_session="dependency_test",
 )
 
-Preparing to copy...
-
-Copying to container - 3.584kB
-
-Successfully copied 3.584kB to base://workspace
-
 Hello from class Dependency
 [screen is terminating]
 ```
```

