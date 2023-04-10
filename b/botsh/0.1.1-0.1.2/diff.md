# Comparing `tmp/botsh-0.1.1.tar.gz` & `tmp/botsh-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botsh-0.1.1.tar", last modified: Mon Apr 10 14:30:02 2023, max compression
+gzip compressed data, was "botsh-0.1.2.tar", last modified: Mon Apr 10 14:41:40 2023, max compression
```

## Comparing `botsh-0.1.1.tar` & `botsh-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 14:30:02.147375 botsh-0.1.1/
--rw-r--r--   0 paulbutler   (501) staff       (20)       54 2023-04-10 14:28:50.000000 botsh-0.1.1/MANIFEST.in
--rw-r--r--   0 paulbutler   (501) staff       (20)     3527 2023-04-10 14:30:02.147196 botsh-0.1.1/PKG-INFO
--rw-r--r--   0 paulbutler   (501) staff       (20)      234 2023-04-10 14:12:58.000000 botsh-0.1.1/Pipfile
--rw-r--r--   0 paulbutler   (501) staff       (20)    64876 2023-04-10 14:13:02.000000 botsh-0.1.1/Pipfile.lock
--rw-r--r--   0 paulbutler   (501) staff       (20)     2888 2023-04-10 14:19:23.000000 botsh-0.1.1/README.md
--rw-r--r--   0 paulbutler   (501) staff       (20)       38 2023-04-10 14:30:02.147416 botsh-0.1.1/setup.cfg
--rw-r--r--   0 paulbutler   (501) staff       (20)     1597 2023-04-10 14:25:01.000000 botsh-0.1.1/setup.py
-drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 14:30:02.142576 botsh-0.1.1/src/
-drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 14:30:02.145370 botsh-0.1.1/src/botsh/
--rw-r--r--   0 paulbutler   (501) staff       (20)        0 2023-04-10 09:30:05.000000 botsh-0.1.1/src/botsh/__init__.py
--rw-r--r--   0 paulbutler   (501) staff       (20)     3056 2023-04-10 14:09:21.000000 botsh-0.1.1/src/botsh/docker_exec.py
--rw-r--r--   0 paulbutler   (501) staff       (20)      317 2023-04-10 11:28:56.000000 botsh-0.1.1/src/botsh/history.py
--rw-r--r--   0 paulbutler   (501) staff       (20)     1479 2023-04-10 13:40:08.000000 botsh-0.1.1/src/botsh/llm.py
--rw-r--r--   0 paulbutler   (501) staff       (20)       46 2023-04-10 12:14:03.000000 botsh-0.1.1/src/botsh/logging.py
--rw-r--r--   0 paulbutler   (501) staff       (20)     2539 2023-04-10 14:08:25.000000 botsh-0.1.1/src/botsh/main.py
--rw-r--r--   0 paulbutler   (501) staff       (20)      972 2023-04-10 12:28:06.000000 botsh-0.1.1/src/botsh/prompt.py
--rw-r--r--   0 paulbutler   (501) staff       (20)     2164 2023-04-10 13:51:16.000000 botsh-0.1.1/src/botsh/task_driver.py
-drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 14:30:02.146744 botsh-0.1.1/src/botsh/templates/
--rw-r--r--   0 paulbutler   (501) staff       (20)     1099 2023-04-10 13:51:54.000000 botsh-0.1.1/src/botsh/templates/prompt.jinja2
-drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 14:30:02.146615 botsh-0.1.1/src/botsh.egg-info/
--rw-r--r--   0 paulbutler   (501) staff       (20)     3527 2023-04-10 14:30:02.000000 botsh-0.1.1/src/botsh.egg-info/PKG-INFO
--rw-r--r--   0 paulbutler   (501) staff       (20)      454 2023-04-10 14:30:02.000000 botsh-0.1.1/src/botsh.egg-info/SOURCES.txt
--rw-r--r--   0 paulbutler   (501) staff       (20)        1 2023-04-10 14:30:02.000000 botsh-0.1.1/src/botsh.egg-info/dependency_links.txt
--rw-r--r--   0 paulbutler   (501) staff       (20)       42 2023-04-10 14:30:02.000000 botsh-0.1.1/src/botsh.egg-info/entry_points.txt
--rw-r--r--   0 paulbutler   (501) staff       (20)      881 2023-04-10 14:30:02.000000 botsh-0.1.1/src/botsh.egg-info/requires.txt
--rw-r--r--   0 paulbutler   (501) staff       (20)        6 2023-04-10 14:30:02.000000 botsh-0.1.1/src/botsh.egg-info/top_level.txt
+drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 14:41:40.946276 botsh-0.1.2/
+-rw-r--r--   0 paulbutler   (501) staff       (20)       54 2023-04-10 14:28:50.000000 botsh-0.1.2/MANIFEST.in
+-rw-r--r--   0 paulbutler   (501) staff       (20)     3527 2023-04-10 14:41:40.946043 botsh-0.1.2/PKG-INFO
+-rw-r--r--   0 paulbutler   (501) staff       (20)      234 2023-04-10 14:12:58.000000 botsh-0.1.2/Pipfile
+-rw-r--r--   0 paulbutler   (501) staff       (20)    64876 2023-04-10 14:13:02.000000 botsh-0.1.2/Pipfile.lock
+-rw-r--r--   0 paulbutler   (501) staff       (20)     2888 2023-04-10 14:19:23.000000 botsh-0.1.2/README.md
+-rw-r--r--   0 paulbutler   (501) staff       (20)       38 2023-04-10 14:41:40.946342 botsh-0.1.2/setup.cfg
+-rw-r--r--   0 paulbutler   (501) staff       (20)     1597 2023-04-10 14:40:26.000000 botsh-0.1.2/setup.py
+drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 14:41:40.941098 botsh-0.1.2/src/
+drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 14:41:40.944502 botsh-0.1.2/src/botsh/
+-rw-r--r--   0 paulbutler   (501) staff       (20)        0 2023-04-10 09:30:05.000000 botsh-0.1.2/src/botsh/__init__.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)     3264 2023-04-10 14:41:08.000000 botsh-0.1.2/src/botsh/docker_exec.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)      317 2023-04-10 11:28:56.000000 botsh-0.1.2/src/botsh/history.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)     1479 2023-04-10 13:40:08.000000 botsh-0.1.2/src/botsh/llm.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)       46 2023-04-10 12:14:03.000000 botsh-0.1.2/src/botsh/logging.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)     2718 2023-04-10 14:39:56.000000 botsh-0.1.2/src/botsh/main.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)      972 2023-04-10 12:28:06.000000 botsh-0.1.2/src/botsh/prompt.py
+-rw-r--r--   0 paulbutler   (501) staff       (20)     2164 2023-04-10 13:51:16.000000 botsh-0.1.2/src/botsh/task_driver.py
+drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 14:41:40.945718 botsh-0.1.2/src/botsh/templates/
+-rw-r--r--   0 paulbutler   (501) staff       (20)     1099 2023-04-10 13:51:54.000000 botsh-0.1.2/src/botsh/templates/prompt.jinja2
+drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 14:41:40.945596 botsh-0.1.2/src/botsh.egg-info/
+-rw-r--r--   0 paulbutler   (501) staff       (20)     3527 2023-04-10 14:41:40.000000 botsh-0.1.2/src/botsh.egg-info/PKG-INFO
+-rw-r--r--   0 paulbutler   (501) staff       (20)      454 2023-04-10 14:41:40.000000 botsh-0.1.2/src/botsh.egg-info/SOURCES.txt
+-rw-r--r--   0 paulbutler   (501) staff       (20)        1 2023-04-10 14:41:40.000000 botsh-0.1.2/src/botsh.egg-info/dependency_links.txt
+-rw-r--r--   0 paulbutler   (501) staff       (20)       42 2023-04-10 14:41:40.000000 botsh-0.1.2/src/botsh.egg-info/entry_points.txt
+-rw-r--r--   0 paulbutler   (501) staff       (20)      881 2023-04-10 14:41:40.000000 botsh-0.1.2/src/botsh.egg-info/requires.txt
+-rw-r--r--   0 paulbutler   (501) staff       (20)        6 2023-04-10 14:41:40.000000 botsh-0.1.2/src/botsh.egg-info/top_level.txt
```

### Comparing `botsh-0.1.1/PKG-INFO` & `botsh-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botsh
-Version: 0.1.1
+Version: 0.1.2
 Summary: A task runner powered by OpenAI and Docker.
 Home-page: https://github.com/drifting-in-space/botsh
 Author: Paul Butler
 Author-email: paul@driftingin.space
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `botsh-0.1.1/Pipfile.lock` & `botsh-0.1.2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `botsh-0.1.1/README.md` & `botsh-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `botsh-0.1.1/setup.py` & `botsh-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         f"{pkg_name}{pkg_info['version']}"
         for pkg_name, pkg_info in pipfile_lock[mode].items()
     ]
 
 
 setup(
     name="botsh",
-    version="0.1.1",
+    version="0.1.2",
     description="A task runner powered by OpenAI and Docker.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Paul Butler",
     author_email="paul@driftingin.space",
     url="https://github.com/drifting-in-space/botsh",
     packages=find_packages("src"),
```

### Comparing `botsh-0.1.1/src/botsh/docker_exec.py` & `botsh-0.1.2/src/botsh/docker_exec.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,20 @@
 
 from botsh.logging import log
 
 
 class DockerContainer:
     current_directory: str
     shell_command: str
+    remove_on_exit: bool
 
-    def __init__(self, image: str, shell_command: str, wipe: bool):
+    def __init__(
+        self, image: str, shell_command: str, wipe: bool, remove_on_exit: bool
+    ):
+        self.remove_on_exit = remove_on_exit
         self.current_directory = os.getcwd()
         self.shell_command = shell_command
         dir_hash = hashlib.sha256(self.current_directory.encode("utf-8")).hexdigest()
         container_name = f"botsh-{dir_hash}"
 
         log.info("Connecting to Docker...")
         self.client = docker.from_env()
@@ -34,22 +38,22 @@
             log.info("Locating existing container...")
             container = self.client.containers.get(container_name)
             if not wipe:
                 log.info("Using existing container.")
                 if container.status != "running":
                     log.info("Starting container...")
                     container.start()
-                return container
+                self.container = container
+                return
             else:
                 log.info("Terminating existing container.")
                 container.stop(timeout=0)
                 container.remove(force=True)
         except docker.errors.NotFound:
             log.info("No container exists, creating one.")
-            pass
 
         log.info("Pulling image...")
         self.client.images.pull(image)
 
         mounts = self._get_mounts()
 
         log.info("Creating container...")
@@ -90,8 +94,10 @@
 
         return exit_code, "".join(result)
 
     def __del__(self):
         if hasattr(self, "container"):
             log.info("Terminating container.")
             self.container.stop(timeout=0)
-            # self.container.remove()
+            if self.remove_on_exit:
+                log.info("Removing container.")
+                self.container.remove()
```

### Comparing `botsh-0.1.1/src/botsh/llm.py` & `botsh-0.1.2/src/botsh/llm.py`

 * *Files identical despite different names*

### Comparing `botsh-0.1.1/src/botsh/main.py` & `botsh-0.1.2/src/botsh/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,25 +41,32 @@
         "--save-transcript", action="store_true", help="Save transcript to file"
     )
     parser.add_argument(
         "--wipe",
         action="store_true",
         help="Start with a fresh container even if one exists for this directory.",
     )
+    parser.add_argument(
+        "--rm",
+        action="store_true",
+        help="Remove the container after the task is complete.",
+    )
     args = parser.parse_args()
 
     if "OPENAI_API_KEY" not in environ:
         log.error(
             "OpenAI API key not found."
             "Please set the OPENAI_API_KEY environment variable."
         )
         return
 
     llm = LLM(args.model, save_transcript=args.save_transcript)
-    container = DockerContainer(args.image, args.shell_command, wipe=args.wipe)
+    container = DockerContainer(
+        args.image, args.shell_command, wipe=args.wipe, remove_on_exit=args.rm
+    )
     task_runner = TaskDriver(args.prompt, container, llm)
 
     try:
         for _ in range(args.max_rounds):
             result = task_runner.step()
             if result:
                 break
```

### Comparing `botsh-0.1.1/src/botsh/prompt.py` & `botsh-0.1.2/src/botsh/prompt.py`

 * *Files identical despite different names*

### Comparing `botsh-0.1.1/src/botsh/task_driver.py` & `botsh-0.1.2/src/botsh/task_driver.py`

 * *Files identical despite different names*

### Comparing `botsh-0.1.1/src/botsh/templates/prompt.jinja2` & `botsh-0.1.2/src/botsh/templates/prompt.jinja2`

 * *Files identical despite different names*

### Comparing `botsh-0.1.1/src/botsh.egg-info/PKG-INFO` & `botsh-0.1.2/src/botsh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botsh
-Version: 0.1.1
+Version: 0.1.2
 Summary: A task runner powered by OpenAI and Docker.
 Home-page: https://github.com/drifting-in-space/botsh
 Author: Paul Butler
 Author-email: paul@driftingin.space
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `botsh-0.1.1/src/botsh.egg-info/requires.txt` & `botsh-0.1.2/src/botsh.egg-info/requires.txt`

 * *Files identical despite different names*

