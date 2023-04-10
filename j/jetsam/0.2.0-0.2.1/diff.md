# Comparing `tmp/jetsam-0.2.0.tar.gz` & `tmp/jetsam-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jetsam-0.2.0.tar", last modified: Tue Apr  4 18:04:22 2023, max compression
+gzip compressed data, was "jetsam-0.2.1.tar", last modified: Mon Apr 10 04:39:53 2023, max compression
```

## Comparing `jetsam-0.2.0.tar` & `jetsam-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tony       (502) staff       (20)        0 2023-04-04 18:04:22.782406 jetsam-0.2.0/
--rw-r--r--   0 tony       (502) staff       (20)     1068 2023-03-17 19:06:19.000000 jetsam-0.2.0/LICENSE
--rw-r--r--   0 tony       (502) staff       (20)      146 2023-03-17 19:06:19.000000 jetsam-0.2.0/MANIFEST.in
--rw-r--r--   0 tony       (502) staff       (20)     1616 2023-04-04 18:04:22.782119 jetsam-0.2.0/PKG-INFO
--rw-r--r--   0 tony       (502) staff       (20)     1316 2023-04-04 17:55:45.000000 jetsam-0.2.0/README.md
--rw-r--r--   0 tony       (502) staff       (20)       38 2023-04-04 18:04:22.782479 jetsam-0.2.0/setup.cfg
--rw-r--r--   0 tony       (502) staff       (20)     1485 2023-04-04 18:03:19.000000 jetsam-0.2.0/setup.py
-drwxr-xr-x   0 tony       (502) staff       (20)        0 2023-04-04 18:04:22.780083 jetsam-0.2.0/src/
--rw-r--r--   0 tony       (502) staff       (20)     8125 2023-03-18 15:03:23.000000 jetsam-0.2.0/src/detach.c
-drwxr-xr-x   0 tony       (502) staff       (20)        0 2023-04-04 18:04:22.781789 jetsam-0.2.0/src/jetsam.egg-info/
--rw-r--r--   0 tony       (502) staff       (20)     1616 2023-04-04 18:04:22.000000 jetsam-0.2.0/src/jetsam.egg-info/PKG-INFO
--rw-r--r--   0 tony       (502) staff       (20)      221 2023-04-04 18:04:22.000000 jetsam-0.2.0/src/jetsam.egg-info/SOURCES.txt
--rw-r--r--   0 tony       (502) staff       (20)        1 2023-04-04 18:04:22.000000 jetsam-0.2.0/src/jetsam.egg-info/dependency_links.txt
--rw-r--r--   0 tony       (502) staff       (20)       16 2023-04-04 18:04:22.000000 jetsam-0.2.0/src/jetsam.egg-info/top_level.txt
--rw-r--r--   0 tony       (502) staff       (20)     1081 2023-03-18 15:07:46.000000 jetsam-0.2.0/src/jetsam.py
--rw-r--r--   0 tony       (502) staff       (20)     1517 2023-04-04 18:00:07.000000 jetsam-0.2.0/src/log.c
--rw-r--r--   0 tony       (502) staff       (20)      265 2023-03-18 15:03:23.000000 jetsam-0.2.0/src/log.h
+drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-04-10 04:39:53.952240 jetsam-0.2.1/
+-rw-r--r--   0 tony      (1000) tony      (1000)     1068 2023-03-16 19:49:52.000000 jetsam-0.2.1/LICENSE
+-rw-r--r--   0 tony      (1000) tony      (1000)      151 2023-04-10 04:36:36.000000 jetsam-0.2.1/MANIFEST.in
+-rw-r--r--   0 tony      (1000) tony      (1000)     1348 2023-04-10 04:39:53.952240 jetsam-0.2.1/PKG-INFO
+-rw-r--r--   0 tony      (1000) tony      (1000)     1048 2023-04-10 04:29:44.000000 jetsam-0.2.1/README.md
+-rw-r--r--   0 tony      (1000) tony      (1000)       38 2023-04-10 04:39:53.952240 jetsam-0.2.1/setup.cfg
+-rw-r--r--   0 tony      (1000) tony      (1000)     1485 2023-04-10 04:35:59.000000 jetsam-0.2.1/setup.py
+drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-04-10 04:39:53.952240 jetsam-0.2.1/src/
+-rw-r--r--   0 tony      (1000) tony      (1000)     8125 2023-03-18 00:03:57.000000 jetsam-0.2.1/src/detach.c
+drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-04-10 04:39:53.952240 jetsam-0.2.1/src/jetsam.egg-info/
+-rw-r--r--   0 tony      (1000) tony      (1000)     1348 2023-04-10 04:39:53.000000 jetsam-0.2.1/src/jetsam.egg-info/PKG-INFO
+-rw-r--r--   0 tony      (1000) tony      (1000)      221 2023-04-10 04:39:53.000000 jetsam-0.2.1/src/jetsam.egg-info/SOURCES.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)        1 2023-04-10 04:39:53.000000 jetsam-0.2.1/src/jetsam.egg-info/dependency_links.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)       16 2023-04-10 04:39:53.000000 jetsam-0.2.1/src/jetsam.egg-info/top_level.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)     1081 2023-03-24 05:27:16.000000 jetsam-0.2.1/src/jetsam.py
+-rw-r--r--   0 tony      (1000) tony      (1000)     1517 2023-04-10 04:27:58.000000 jetsam-0.2.1/src/log.c
+-rw-r--r--   0 tony      (1000) tony      (1000)      265 2023-03-17 23:31:46.000000 jetsam-0.2.1/src/log.h
```

### Comparing `jetsam-0.2.0/LICENSE` & `jetsam-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jetsam-0.2.0/PKG-INFO` & `jetsam-0.2.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetsam
-Version: 0.2.0
+Version: 0.2.1
 Summary: Jettison functions with jetsam!
 Author: Tony B
 Author-email: tony@ballast.dev
 License: MIT
 Project-URL: Source Code, https://gitlab.com/ballast-dev/jetsam
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -22,47 +22,33 @@
 ## Example 
 ```python
 import time
 import logging
 import jetsam
 from jetsam import daemon
 
-# jetsam will log pids and errors from daemons 
+# jetsam will log pids and errors from daemons
 # to a single log file. It will also update the file
-# with the current status of the daemon  
-#  
+# with the current status of the daemon
+#
 #   function_name:pid:status
 #
 jetsam.set_logfile("user_daemon.log")  # defaults to /tmp/jetsam.log
 
-@daemon
-def func1():
-    logging.basicConfig(
-        filename="func1.log", 
-        level=logging.DEBUG, 
-        filemode="w"
-    )
-    while True:
-        time.sleep(1)
-        logging.debug("Truly daemonized!")
 
-def func2():
-    logging.basicConfig(
-        filename="func2.log", 
-        level=logging.DEBUG, 
-        filemode="w"
-    )
+@daemon
+def func():
+    logging.basicConfig(filename="func.log", level=logging.DEBUG, filemode="w")
     while True:
         time.sleep(1)
-        logging.debug("I can do this all day...")
+        logging.debug("I am running in my own interpreter!")
 
 
-func1()  # detachs from current interpreter
-daemon(func2)  # each function immediately returns 
+func()  # detachs from current interpreter each function immediately returns 
 
-time.sleep(3)  # a long running process...
+print("simulate long running process...")
+time.sleep(3)
 
-jetsam.end_daemon(func1)
-jetsam.end_daemon(func2)
+jetsam.end_daemon(func)
 
-print("Jettison functions with jetsam!")
+print("Eject and forget with jetsam!")
 ```
```

### Comparing `jetsam-0.2.0/setup.py` & `jetsam-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     define = "_DARWIN_C_SOURCE"
 elif system == "Linux":
     define = "__USE_MISC"
 
 
 setup(
     name="jetsam",
-    version="0.2.0",
+    version="0.2.1",
     description="Jettison functions with jetsam!",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     author="Tony B",
     author_email="tony@ballast.dev",
     license="MIT",
     license_files=["LICENSE"],
```

### Comparing `jetsam-0.2.0/src/detach.c` & `jetsam-0.2.1/src/detach.c`

 * *Files identical despite different names*

### Comparing `jetsam-0.2.0/src/jetsam.egg-info/PKG-INFO` & `jetsam-0.2.1/src/jetsam.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetsam
-Version: 0.2.0
+Version: 0.2.1
 Summary: Jettison functions with jetsam!
 Author: Tony B
 Author-email: tony@ballast.dev
 License: MIT
 Project-URL: Source Code, https://gitlab.com/ballast-dev/jetsam
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -22,47 +22,33 @@
 ## Example 
 ```python
 import time
 import logging
 import jetsam
 from jetsam import daemon
 
-# jetsam will log pids and errors from daemons 
+# jetsam will log pids and errors from daemons
 # to a single log file. It will also update the file
-# with the current status of the daemon  
-#  
+# with the current status of the daemon
+#
 #   function_name:pid:status
 #
 jetsam.set_logfile("user_daemon.log")  # defaults to /tmp/jetsam.log
 
-@daemon
-def func1():
-    logging.basicConfig(
-        filename="func1.log", 
-        level=logging.DEBUG, 
-        filemode="w"
-    )
-    while True:
-        time.sleep(1)
-        logging.debug("Truly daemonized!")
 
-def func2():
-    logging.basicConfig(
-        filename="func2.log", 
-        level=logging.DEBUG, 
-        filemode="w"
-    )
+@daemon
+def func():
+    logging.basicConfig(filename="func.log", level=logging.DEBUG, filemode="w")
     while True:
         time.sleep(1)
-        logging.debug("I can do this all day...")
+        logging.debug("I am running in my own interpreter!")
 
 
-func1()  # detachs from current interpreter
-daemon(func2)  # each function immediately returns 
+func()  # detachs from current interpreter each function immediately returns 
 
-time.sleep(3)  # a long running process...
+print("simulate long running process...")
+time.sleep(3)
 
-jetsam.end_daemon(func1)
-jetsam.end_daemon(func2)
+jetsam.end_daemon(func)
 
-print("Jettison functions with jetsam!")
+print("Eject and forget with jetsam!")
 ```
```

### Comparing `jetsam-0.2.0/src/jetsam.py` & `jetsam-0.2.1/src/jetsam.py`

 * *Files identical despite different names*

### Comparing `jetsam-0.2.0/src/log.c` & `jetsam-0.2.1/src/log.c`

 * *Files identical despite different names*

