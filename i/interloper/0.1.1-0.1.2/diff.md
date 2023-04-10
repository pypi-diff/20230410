# Comparing `tmp/interloper-0.1.1.tar.gz` & `tmp/interloper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interloper-0.1.1.tar", last modified: Mon Apr 10 13:23:16 2023, max compression
+gzip compressed data, was "interloper-0.1.2.tar", last modified: Mon Apr 10 15:43:12 2023, max compression
```

## Comparing `interloper-0.1.1.tar` & `interloper-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 h4s        (501) staff       (20)        0 2023-04-10 13:23:16.122970 interloper-0.1.1/
--rw-r--r--   0 h4s        (501) staff       (20)     1080 2022-10-18 21:18:37.000000 interloper-0.1.1/LICENSE
--rw-r--r--   0 h4s        (501) staff       (20)     3678 2023-04-10 13:23:16.123064 interloper-0.1.1/PKG-INFO
--rw-r--r--   0 h4s        (501) staff       (20)     3166 2023-04-10 10:51:19.000000 interloper-0.1.1/README.md
-drwxr-xr-x   0 h4s        (501) staff       (20)        0 2023-04-10 13:23:16.122168 interloper-0.1.1/interloper.egg-info/
--rw-r--r--   0 h4s        (501) staff       (20)     3678 2023-04-10 13:23:16.000000 interloper-0.1.1/interloper.egg-info/PKG-INFO
--rw-r--r--   0 h4s        (501) staff       (20)      250 2023-04-10 13:23:16.000000 interloper-0.1.1/interloper.egg-info/SOURCES.txt
--rw-r--r--   0 h4s        (501) staff       (20)        1 2023-04-10 13:23:16.000000 interloper-0.1.1/interloper.egg-info/dependency_links.txt
--rw-r--r--   0 h4s        (501) staff       (20)       33 2023-04-10 13:23:16.000000 interloper-0.1.1/interloper.egg-info/requires.txt
--rw-r--r--   0 h4s        (501) staff       (20)       11 2023-04-10 13:23:16.000000 interloper-0.1.1/interloper.egg-info/top_level.txt
--rw-r--r--   0 h4s        (501) staff       (20)     3689 2023-04-10 13:17:40.000000 interloper-0.1.1/interloper.py
--rw-r--r--   0 h4s        (501) staff       (20)       64 2022-10-18 21:18:37.000000 interloper-0.1.1/pyproject.toml
--rw-r--r--   0 h4s        (501) staff       (20)      641 2023-04-10 13:23:16.125134 interloper-0.1.1/setup.cfg
-drwxr-xr-x   0 h4s        (501) staff       (20)        0 2023-04-10 13:23:16.122659 interloper-0.1.1/tests/
--rw-r--r--   0 h4s        (501) staff       (20)      875 2022-10-18 21:18:37.000000 interloper-0.1.1/tests/test_interloper.py
+drwxr-xr-x   0 h4s        (501) staff       (20)        0 2023-04-10 15:43:12.085462 interloper-0.1.2/
+-rw-r--r--   0 h4s        (501) staff       (20)     1080 2022-10-18 21:18:37.000000 interloper-0.1.2/LICENSE
+-rw-r--r--   0 h4s        (501) staff       (20)     3678 2023-04-10 15:43:12.085546 interloper-0.1.2/PKG-INFO
+-rw-r--r--   0 h4s        (501) staff       (20)     3166 2023-04-10 10:51:19.000000 interloper-0.1.2/README.md
+drwxr-xr-x   0 h4s        (501) staff       (20)        0 2023-04-10 15:43:12.083052 interloper-0.1.2/interloper.egg-info/
+-rw-r--r--   0 h4s        (501) staff       (20)     3678 2023-04-10 15:43:12.000000 interloper-0.1.2/interloper.egg-info/PKG-INFO
+-rw-r--r--   0 h4s        (501) staff       (20)      250 2023-04-10 15:43:12.000000 interloper-0.1.2/interloper.egg-info/SOURCES.txt
+-rw-r--r--   0 h4s        (501) staff       (20)        1 2023-04-10 15:43:12.000000 interloper-0.1.2/interloper.egg-info/dependency_links.txt
+-rw-r--r--   0 h4s        (501) staff       (20)       33 2023-04-10 15:43:12.000000 interloper-0.1.2/interloper.egg-info/requires.txt
+-rw-r--r--   0 h4s        (501) staff       (20)       11 2023-04-10 15:43:12.000000 interloper-0.1.2/interloper.egg-info/top_level.txt
+-rw-r--r--   0 h4s        (501) staff       (20)     3945 2023-04-10 14:53:42.000000 interloper-0.1.2/interloper.py
+-rw-r--r--   0 h4s        (501) staff       (20)       64 2022-10-18 21:18:37.000000 interloper-0.1.2/pyproject.toml
+-rw-r--r--   0 h4s        (501) staff       (20)      641 2023-04-10 15:43:12.088224 interloper-0.1.2/setup.cfg
+drwxr-xr-x   0 h4s        (501) staff       (20)        0 2023-04-10 15:43:12.084991 interloper-0.1.2/tests/
+-rw-r--r--   0 h4s        (501) staff       (20)      875 2022-10-18 21:18:37.000000 interloper-0.1.2/tests/test_interloper.py
```

### Comparing `interloper-0.1.1/LICENSE` & `interloper-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `interloper-0.1.1/PKG-INFO` & `interloper-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interloper
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tool to run ecs execute command in lambda.
 Home-page: https://github.com/theherk/interloper
 Author: Adam Sherwood
 Author-email: theherk@gmail.com
 Project-URL: Bug Tracker, https://github.com/theherk/interloper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `interloper-0.1.1/README.md` & `interloper-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `interloper-0.1.1/interloper.egg-info/PKG-INFO` & `interloper-0.1.2/interloper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interloper
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tool to run ecs execute command in lambda.
 Home-page: https://github.com/theherk/interloper
 Author: Adam Sherwood
 Author-email: theherk@gmail.com
 Project-URL: Bug Tracker, https://github.com/theherk/interloper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `interloper-0.1.1/interloper.py` & `interloper-0.1.2/interloper.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,34 +50,41 @@
 
     def _exec(self, cmd: str) -> str:
         params = {
             "task": self.task,
             "interactive": True,
             "command": cmd,
         }
+        LOG.debug("exec params: %s", params)
         if self.cluster:
             params["cluster"] = self.cluster
         if self.container:
             params["container"] = self.container
         exec_resp = boto3.client("ecs").execute_command(**params)
+        LOG.debug("exec response: %s", exec_resp)
         return session_reader(exec_resp["session"])
 
     def cmd(self, cmd: str) -> str:
-        LOG.debug("interloping with simple command...")
+        LOG.info("interloping with simple command...")
+        LOG.info(cmd)
         return self._exec(cmd)
 
     @staticmethod
     def fmt_cmd(filename: str, args: List[str]) -> str:
         with open(filename, "rb") as f:
             script = f.read()
-        return CMD_TMPL.format(base64.b64encode(script).decode(), " ".join(args))
+        cmd = CMD_TMPL.format(base64.b64encode(script).decode(), " ".join(args))
+        LOG.debug("formatted script cmd: \n%s", cmd)
+        return cmd
 
     def script(self, filename: str, args: List[str] = None) -> str:
-        LOG.debug("interloping with script...")
+        LOG.info("interloping with script...")
+        LOG.info(filename)
         args = args or []
+        LOG.debug("script args: %s", args)
         return self._exec(self.fmt_cmd(filename, args))
 
 
 def session_reader(session: dict) -> str:
     AgentMessageHeader = c.Struct(
         "HeaderLength" / c.Int32ub,
         "MessageType" / c.PaddedString(32, "ascii"),
```

### Comparing `interloper-0.1.1/setup.cfg` & `interloper-0.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = interloper
-version = 0.1.1
+version = 0.1.2
 author = Adam Sherwood
 author_email = theherk@gmail.com
 description = Tool to run ecs execute command in lambda.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/theherk/interloper
 project_urls =
```

### Comparing `interloper-0.1.1/tests/test_interloper.py` & `interloper-0.1.2/tests/test_interloper.py`

 * *Files identical despite different names*

