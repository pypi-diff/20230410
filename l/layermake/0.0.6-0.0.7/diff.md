# Comparing `tmp/layermake-0.0.6.tar.gz` & `tmp/layermake-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layermake-0.0.6.tar", last modified: Sat Apr  1 23:45:06 2023, max compression
+gzip compressed data, was "layermake-0.0.7.tar", last modified: Mon Apr 10 18:26:46 2023, max compression
```

## Comparing `layermake-0.0.6.tar` & `layermake-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-01 23:45:06.695606 layermake-0.0.6/
--rw-rw-rw-   0        0        0     1061 2023-03-31 17:19:15.000000 layermake-0.0.6/LICENSE.md
--rw-rw-rw-   0        0        0     7937 2023-04-01 23:45:06.693605 layermake-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     7444 2023-04-01 23:44:07.000000 layermake-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-01 23:45:06.682092 layermake-0.0.6/layermake/
--rw-rw-rw-   0        0        0      370 2023-04-01 21:41:37.000000 layermake-0.0.6/layermake/__init__.py
--rw-rw-rw-   0        0        0     4318 2023-04-01 23:28:23.000000 layermake-0.0.6/layermake/binary.py
--rw-rw-rw-   0        0        0     3325 2023-04-01 23:39:19.000000 layermake-0.0.6/layermake/bundler.py
--rw-rw-rw-   0        0        0     7891 2023-04-01 23:44:07.000000 layermake-0.0.6/layermake/cli.py
--rw-rw-rw-   0        0        0     6460 2023-04-01 17:29:10.000000 layermake-0.0.6/layermake/cmd.py
--rw-rw-rw-   0        0        0     2143 2023-04-01 14:03:05.000000 layermake-0.0.6/layermake/logger.py
--rw-rw-rw-   0        0        0     2608 2023-04-01 23:31:11.000000 layermake-0.0.6/layermake/node.py
--rw-rw-rw-   0        0        0     3177 2023-04-01 23:28:23.000000 layermake-0.0.6/layermake/publisher.py
--rw-rw-rw-   0        0        0     2809 2023-04-01 23:36:34.000000 layermake-0.0.6/layermake/python.py
-drwxrwxrwx   0        0        0        0 2023-04-01 23:45:06.691604 layermake-0.0.6/layermake.egg-info/
--rw-rw-rw-   0        0        0     7937 2023-04-01 23:45:06.000000 layermake-0.0.6/layermake.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2023-04-01 23:45:06.000000 layermake-0.0.6/layermake.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-01 23:45:06.000000 layermake-0.0.6/layermake.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-01 23:45:06.000000 layermake-0.0.6/layermake.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-04-01 23:45:06.000000 layermake-0.0.6/layermake.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-01 23:45:06.000000 layermake-0.0.6/layermake.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-01 23:45:06.695606 layermake-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      868 2023-04-01 14:49:19.000000 layermake-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 18:26:46.771856 layermake-0.0.7/
+-rw-rw-rw-   0        0        0     1061 2023-03-31 17:19:15.000000 layermake-0.0.7/LICENSE.md
+-rw-rw-rw-   0        0        0     7937 2023-04-10 18:26:46.769859 layermake-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     7444 2023-04-01 23:44:07.000000 layermake-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 18:26:46.757850 layermake-0.0.7/layermake/
+-rw-rw-rw-   0        0        0      370 2023-04-10 17:31:32.000000 layermake-0.0.7/layermake/__init__.py
+-rw-rw-rw-   0        0        0     4367 2023-04-10 18:12:13.000000 layermake-0.0.7/layermake/binary.py
+-rw-rw-rw-   0        0        0     3827 2023-04-10 18:12:13.000000 layermake-0.0.7/layermake/bundler.py
+-rw-rw-rw-   0        0        0     7906 2023-04-10 18:12:13.000000 layermake-0.0.7/layermake/cli.py
+-rw-rw-rw-   0        0        0     6460 2023-04-01 17:29:10.000000 layermake-0.0.7/layermake/cmd.py
+-rw-rw-rw-   0        0        0     2143 2023-04-01 14:03:05.000000 layermake-0.0.7/layermake/logger.py
+-rw-rw-rw-   0        0        0     2665 2023-04-10 18:12:13.000000 layermake-0.0.7/layermake/node.py
+-rw-rw-rw-   0        0        0     2549 2023-04-10 18:12:13.000000 layermake-0.0.7/layermake/publisher.py
+-rw-rw-rw-   0        0        0     2866 2023-04-10 18:12:13.000000 layermake-0.0.7/layermake/python.py
+drwxrwxrwx   0        0        0        0 2023-04-10 18:26:46.768856 layermake-0.0.7/layermake.egg-info/
+-rw-rw-rw-   0        0        0     7937 2023-04-10 18:26:46.000000 layermake-0.0.7/layermake.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2023-04-10 18:26:46.000000 layermake-0.0.7/layermake.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 18:26:46.000000 layermake-0.0.7/layermake.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-10 18:26:46.000000 layermake-0.0.7/layermake.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-04-10 18:26:46.000000 layermake-0.0.7/layermake.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-10 18:26:46.000000 layermake-0.0.7/layermake.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 18:26:46.771856 layermake-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      868 2023-04-01 14:49:19.000000 layermake-0.0.7/setup.py
```

### Comparing `layermake-0.0.6/LICENSE.md` & `layermake-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `layermake-0.0.6/PKG-INFO` & `layermake-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layermake
-Version: 0.0.6
+Version: 0.0.7
 Summary: CLI toolkit for bundling AWS Lambda layers
 Home-page: https://github.com/ericmaustin/layermake
 Author: Eric Austin
 Author-email: eric.m.austin@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `layermake-0.0.6/README.md` & `layermake-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `layermake-0.0.6/layermake/binary.py` & `layermake-0.0.7/layermake/binary.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List
+from typing import List, Set
 from pathlib import Path
 import uuid
 from .cmd import docker_build
 from .bundler import Bundler
 from .logger import logger
 
 # list of filenames to look for when provided a directory instead of a file as a build artifact
@@ -24,19 +24,24 @@
         base_image: str = "amazonlinux:latest",
         dockerfile: str = None,
         local_dir: str = "./layer",
         build_cmd: str = None,
         yum_packages: List[str] = None,
         workdir: str = "/opt",
         container_output_dir: str = "/opt",
+        no_zip: bool = False,
     ):
         super(BinaryBundler, self).__init__(
-            workdir=workdir, local_dir=local_dir, build_artifact=build_artifact
+            workdir=workdir,
+            local_dir=local_dir,
+            build_artifact=build_artifact,
+            no_zip=no_zip,
         )
-        self.__yum_packages = yum_packages if yum_packages else []
+        self.__yum_packages = set(yum_packages)
+        self.__yum_packages.add("gzip")
         self.__dockerfile = dockerfile
         self.__base_image = base_image
         self.__container_output_dir = container_output_dir
         if build_cmd:
             self.__container_cmd = build_cmd
             return
 
@@ -90,19 +95,16 @@
             self._container = container_hash
             logger().success(f"container built successfully: {container_hash}")
 
     @staticmethod
     def compile_dockerfile(
         base_image: str = "amazonlinux:latest",
         workdir: str = "/opt",
-        packages: List[str] = None,
+        packages: Set[str] = None,
     ):
-        if not packages:
-            packages = ["gzip"]
-
         dockerfile = f"""FROM {base_image}
 ENV OUTPUT_BIN=/opt/bin
 ENV OUTPUT_LIB=/opt/lib
 RUN yum -y groupinstall 'Development Tools'
 """
         if packages:
             dockerfile += f"RUN yum -y install {' '.join(packages)}\n"
```

### Comparing `layermake-0.0.6/layermake/bundler.py` & `layermake-0.0.7/layermake/bundler.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,17 @@
         self,
         workdir: str,
         local_dir: Path,
         container_cmd: str = None,
         container: str = None,
         build_artifact: str = None,
         container_output_dir: str = None,
+        no_zip: bool = False,
     ):
+        self.__no_zip = no_zip
         self._container = container
         self._container_cmd = container_cmd
         self.__cleanup_paths: List[Path] = []
         self.__workdir = workdir
         self._local_path = Path(local_dir)
         self.__build_artifact_path = Path(build_artifact) if build_artifact else None
         self.__prep_local(self._local_path, self.__build_artifact_path)
@@ -42,14 +44,16 @@
             self.__build_artifact_path = local_path / build_artifact_path.name
 
     def bundle(self) -> Path:
         try:
             self.pre_bundle()
             with logger().status("bundling layer with Docker..."):
                 cmd_str = self._container_cmd
+                if not self.__no_zip:
+                    cmd_str += " && zip -r layer.zip *"
                 if self.__container_output_dir != self.__workdir:
                     cmd_str = f"mkdir -p {self.__container_output_dir} && " + cmd_str
                 try:
                     logger().info(
                         f"starting bundling task with docker container {self._container}"
                     )
                     docker_run(
@@ -60,16 +64,25 @@
                     )
                 except Exception as e:
                     logger().fatal_error(
                         f"failed bundling layer with docker container {self._container}: {str(e)}"
                     )
                 logger().success("bundling complete!")
             self.post_bundle()
+            if not self.__no_zip:
+                # delete all files in the output dir that are not the layer itself
+                for p in self._local_path.iterdir():
+                    if p.name != "layer.zip":
+                        self.add_cleanup_path(p)
         finally:
             self.__cleanup()
+
+        if not self.__no_zip:
+            return self._local_path / "layer.zip"
+
         return self._local_path
 
     def add_cleanup_path(self, p: Path):
         self.__cleanup_paths.append(p)
 
     def __cleanup(self):
         with logger().status("cleaning up..."):
```

### Comparing `layermake-0.0.6/layermake/cli.py` & `layermake-0.0.7/layermake/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,16 +167,17 @@
     bundler = NodeBundler(
         runtime=runtime,
         artifact_dir=dir,
         local_dir=output,
         container=container,
         manifest=manifest,
         packages=packages,
+        no_zip=publisher.no_zip,
     )
-    publisher.publish_layer(bundler.bundle(), Path(output) / "layer.zip", _runtime_name)
+    publisher.publish_layer(bundler.bundle(), _runtime_name)
 
 
 @cli.command()
 @click_common
 @click.option("-r", "--runtime", help="python runtime")
 @click.option("-m", "--manifest", help="python manifest file (requirements.txt)")
 @click.option(
@@ -209,16 +210,17 @@
     bundler = PythonBundler(
         runtime=runtime,
         artifact_dir=dir,
         local_dir=output,
         container=container,
         manifest=manifest,
         packages=packages,
+        no_zip=publisher.no_zip,
     )
-    publisher.publish_layer(bundler.bundle(), Path(output) / "layer.zip", _runtime_name)
+    publisher.publish_layer(bundler.bundle(), _runtime_name)
 
 
 @cli.command()
 @click_common
 @click.option("--dockerfile", help="use the provided dockerfile for bundling")
 @click.option(
     "-o",
@@ -279,14 +281,15 @@
         build_artifact=artifact[0],
         local_dir=output,
         base_image=base_image,
         yum_packages=packages,
         dockerfile=dockerfile,
         build_cmd=cmd,
         workdir=workdir,
+        no_zip=publisher.no_zip,
     )
-    publisher.publish_layer(bundler.bundle(), Path(output) / "layer.zip", "binary")
+    publisher.publish_layer(bundler.bundle(), "binary")
 
 
 if __name__ == "__main__":
     docker = BinaryBundler(build_artifact="static-gnupg-build.sh")
     docker.bundle()
```

### Comparing `layermake-0.0.6/layermake/cmd.py` & `layermake-0.0.7/layermake/cmd.py`

 * *Files identical despite different names*

### Comparing `layermake-0.0.6/layermake/logger.py` & `layermake-0.0.7/layermake/logger.py`

 * *Files identical despite different names*

### Comparing `layermake-0.0.6/layermake/node.py` & `layermake-0.0.7/layermake/node.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,28 +17,30 @@
         self,
         runtime: str,
         local_dir: Path,
         container: str = None,
         artifact_dir: str = None,
         packages: List[str] = None,
         manifest: str = None,
+        no_zip: bool = False,
     ):
         self.__manifest = manifest
         self.__packages = packages
         self.__artifact_dir = Path(artifact_dir) if artifact_dir else None
 
         if not container:
             container = NODE_ECR_TEMPLATE.substitute(runtime=runtime, version="latest")
 
         super(NodeBundler, self).__init__(
             workdir="/opt",
             container=container,
             container_cmd="",
             local_dir=local_dir,
             build_artifact=manifest,
+            no_zip=no_zip,
         )
 
     def pre_bundle(self):
         node_dir = self._local_path / "nodejs"
         try:
             node_dir.mkdir(parents=True)
         except Exception as e:
```

### Comparing `layermake-0.0.6/layermake/publisher.py` & `layermake-0.0.7/layermake/publisher.py`

 * *Files 27% similar despite different names*

```diff
@@ -49,46 +49,33 @@
         if self.__license_text:
             return self.__license_text
         if self.__license_text:
             with open(self.__license_text, "r") as f:
                 return f.read()
         return ""
 
-    def publish_layer(self, output_path: Path, zip_target: Path, layer_type: str):
+    def publish_layer(self, output_path: Path, layer_type: str):
+        if not output_path.exists():
+            raise FileNotFoundError(f"layer at: {output_path} is empty")
+
         if self.__no_zip:
-            logger().info('layer publishing and zipping skipped with "--no-zip"')
+            logger().info('layer publishing skipped because "--no-zip" was set')
             return
 
-        if not output_path.is_dir():
-            raise NotADirectoryError(f"layer output directory: {output_path} not found")
-
-        with logger().status("zipping layer"):
-            logger().info(f"zipping layer contents in: {output_path}")
-            shutil.make_archive(str(output_path), "zip", str(zip_target))
-            logger().success(f"zipped layer contents in: {output_path} to {zip_target}")
-
-        if not zip_target.exists():
-            raise FileNotFoundError(f"layer zip file: {zip_target} is empty")
-
-        # delete the output directory after zipping
-        with logger().status("removing layer source directory"):
-            logger().info(f"deleting dir: {output_path}")
-            rmtree(output_path)
-
         if self.__no_pub:
-            logger().info('layer publishing skipped with "--no-publish"')
+            logger().info('layer publishing skipped because "--no-publish" was set')
             return
 
         with logger().status("publishing layer"):
             try:
                 resp = self.__client.publish_layer_version(
                     LayerName=self.name,
                     Description=self.__description
                     or f"my {layer_type} layer built with layermake",
-                    Content={"ZipFile": zip_target},
+                    Content={"ZipFile": output_path},
                     LicenseInfo=self.get_license_info(),
                     CompatibleRuntimes=self.__runtimes,
                     CompatibleArchitectures=self.__arch or ["x86_64"],
                 )
                 logger().success(f'version: {resp["Version"]}', concat=True)
             except Exception as e:
                 logger().fatal_error(f"Failed to publish layer: {str(e)}")
```

### Comparing `layermake-0.0.6/layermake/python.py` & `layermake-0.0.7/layermake/python.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         self,
         runtime: str,
         local_dir: Path,
         container: str = None,
         artifact_dir: str = None,
         packages: List[str] = None,
         manifest: str = None,
+        no_zip: bool = False,
     ):
         self.__manifest = manifest
         self.__packages = packages
         self.__artifact_dir = Path(artifact_dir) if artifact_dir else None
 
         if not container:
             container = PYTHON_ECR_TEMPLATE.substitute(
@@ -40,14 +41,15 @@
 
         super(PythonBundler, self).__init__(
             workdir="/opt",
             container=container,
             container_cmd="",
             local_dir=local_dir,
             build_artifact=manifest,
+            no_zip=no_zip,
         )
 
     def pre_bundle(self):
         container_cmds = []
         local_src = self._local_path / "src"
         try:
             local_src.mkdir(parents=True, exist_ok=True)
```

### Comparing `layermake-0.0.6/layermake.egg-info/PKG-INFO` & `layermake-0.0.7/layermake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layermake
-Version: 0.0.6
+Version: 0.0.7
 Summary: CLI toolkit for bundling AWS Lambda layers
 Home-page: https://github.com/ericmaustin/layermake
 Author: Eric Austin
 Author-email: eric.m.austin@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `layermake-0.0.6/setup.py` & `layermake-0.0.7/setup.py`

 * *Files identical despite different names*

