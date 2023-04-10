# Comparing `tmp/py_madvr-1.2.4.tar.gz` & `tmp/py_madvr-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_madvr-1.2.4.tar", last modified: Mon Apr 10 02:33:16 2023, max compression
+gzip compressed data, was "py_madvr-1.2.5.tar", last modified: Mon Apr 10 02:44:05 2023, max compression
```

## Comparing `py_madvr-1.2.4.tar` & `py_madvr-1.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:33:16.946104 py_madvr-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-10 02:33:03.000000 py_madvr-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-10 02:33:16.946104 py_madvr-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-10 02:33:03.000000 py_madvr-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:33:16.946104 py_madvr-1.2.4/madvr/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-10 02:33:03.000000 py_madvr-1.2.4/madvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-10 02:33:03.000000 py_madvr-1.2.4/madvr/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-10 02:33:03.000000 py_madvr-1.2.4/madvr/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    19693 2023-04-10 02:33:03.000000 py_madvr-1.2.4/madvr/madvr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:33:16.946104 py_madvr-1.2.4/py_madvr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-10 02:33:16.000000 py_madvr-1.2.4/py_madvr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-10 02:33:16.000000 py_madvr-1.2.4/py_madvr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 02:33:16.000000 py_madvr-1.2.4/py_madvr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-10 02:33:16.000000 py_madvr-1.2.4/py_madvr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 02:33:16.946104 py_madvr-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-10 02:33:03.000000 py_madvr-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:33:16.946104 py_madvr-1.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 02:33:03.000000 py_madvr-1.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-10 02:33:03.000000 py_madvr-1.2.4/tests/testMadVR.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:44:05.630140 py_madvr-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-10 02:43:52.000000 py_madvr-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-10 02:44:05.630140 py_madvr-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-10 02:43:52.000000 py_madvr-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:44:05.626140 py_madvr-1.2.5/madvr/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-10 02:43:52.000000 py_madvr-1.2.5/madvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-10 02:43:52.000000 py_madvr-1.2.5/madvr/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-10 02:43:52.000000 py_madvr-1.2.5/madvr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19837 2023-04-10 02:43:52.000000 py_madvr-1.2.5/madvr/madvr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:44:05.630140 py_madvr-1.2.5/py_madvr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-10 02:44:05.000000 py_madvr-1.2.5/py_madvr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-10 02:44:05.000000 py_madvr-1.2.5/py_madvr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 02:44:05.000000 py_madvr-1.2.5/py_madvr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-10 02:44:05.000000 py_madvr-1.2.5/py_madvr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 02:44:05.630140 py_madvr-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-10 02:43:52.000000 py_madvr-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:44:05.630140 py_madvr-1.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 02:43:52.000000 py_madvr-1.2.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-10 02:43:52.000000 py_madvr-1.2.5/tests/testMadVR.py
```

### Comparing `py_madvr-1.2.4/LICENSE` & `py_madvr-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py_madvr-1.2.4/PKG-INFO` & `py_madvr-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_madvr
-Version: 1.2.4
+Version: 1.2.5
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.2.4/madvr/commands.py` & `py_madvr-1.2.5/madvr/commands.py`

 * *Files identical despite different names*

### Comparing `py_madvr-1.2.4/madvr/madvr.py` & `py_madvr-1.2.5/madvr/madvr.py`

 * *Files 2% similar despite different names*

```diff
@@ -395,15 +395,17 @@
         return ""
 
     def start_read_notifications(self, wait_forever: bool) -> None:
         """
         Listen for notifications. Meant to run as a background task
         wait_forever: bool -> if true, it will block forever. False useful for testing
         """
-        # Is there a way for HA to always poll in background?z
+        # reconnect if client is not init or its off
+        if self.client is None or self.is_on is False:
+            self._reconnect()
 
         # Receive data in a loop
         i = 0
         while wait_forever or i < 5:
             try:
                 self.notification_client.sendall(self.HEARTBEAT)
                 data = self.notification_client.recv(self.read_limit)
@@ -421,14 +423,16 @@
                 self.logger.debug("Connection timed out")
                 self.notification_client.sendall(self.HEARTBEAT)
                 continue
             except socket.error:
                 self.logger.debug("Connection error")
                 self.notification_client.sendall(self.HEARTBEAT)
                 continue
+            except AttributeError:
+                self._reconnect()
 
     def _process_notifications(self, input_data: Union[bytes, str]) -> None:
         """
         Process arbitrary stream of notifications and set them as instance attr
         """
         # This code constructs a dict for all values processed
         self.logger.debug("Processing data for %s", input_data)
```

### Comparing `py_madvr-1.2.4/py_madvr.egg-info/PKG-INFO` & `py_madvr-1.2.5/py_madvr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-madvr
-Version: 1.2.4
+Version: 1.2.5
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.2.4/setup.py` & `py_madvr-1.2.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_madvr",
-    version="1.2.4",
+    version="1.2.5",
     author="iloveicedgreentea",
     description="A package to control MadVR Envy over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/py-madvr",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `py_madvr-1.2.4/tests/testMadVR.py` & `py_madvr-1.2.5/tests/testMadVR.py`

 * *Files identical despite different names*

