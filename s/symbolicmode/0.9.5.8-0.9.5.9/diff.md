# Comparing `tmp/symbolicmode-0.9.5.8.tar.gz` & `tmp/symbolicmode-0.9.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbolicmode-0.9.5.8.tar", last modified: Mon Apr 10 00:29:04 2023, max compression
+gzip compressed data, was "symbolicmode-0.9.5.9.tar", last modified: Mon Apr 10 00:31:10 2023, max compression
```

## Comparing `symbolicmode-0.9.5.8.tar` & `symbolicmode-0.9.5.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:29:04.952035 symbolicmode-0.9.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-10 00:28:50.000000 symbolicmode-0.9.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-04-10 00:29:04.952035 symbolicmode-0.9.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-10 00:28:50.000000 symbolicmode-0.9.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-10 00:28:55.000000 symbolicmode-0.9.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 00:29:04.952035 symbolicmode-0.9.5.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:29:04.948035 symbolicmode-0.9.5.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:29:04.948035 symbolicmode-0.9.5.8/src/symbolicmode/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9017 2023-04-10 00:28:50.000000 symbolicmode-0.9.5.8/src/symbolicmode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:29:04.952035 symbolicmode-0.9.5.8/src/symbolicmode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-04-10 00:29:04.000000 symbolicmode-0.9.5.8/src/symbolicmode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-10 00:29:04.000000 symbolicmode-0.9.5.8/src/symbolicmode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 00:29:04.000000 symbolicmode-0.9.5.8/src/symbolicmode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-10 00:29:04.000000 symbolicmode-0.9.5.8/src/symbolicmode.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:29:04.952035 symbolicmode-0.9.5.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-10 00:28:50.000000 symbolicmode-0.9.5.8/tests/test_chmod.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-04-10 00:28:50.000000 symbolicmode-0.9.5.8/tests/test_modes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:31:10.160957 symbolicmode-0.9.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-10 00:30:47.000000 symbolicmode-0.9.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-04-10 00:31:10.160957 symbolicmode-0.9.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-10 00:30:47.000000 symbolicmode-0.9.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-10 00:31:01.000000 symbolicmode-0.9.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 00:31:10.160957 symbolicmode-0.9.5.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:31:10.160957 symbolicmode-0.9.5.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:31:10.160957 symbolicmode-0.9.5.9/src/symbolicmode/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9017 2023-04-10 00:30:47.000000 symbolicmode-0.9.5.9/src/symbolicmode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:31:10.160957 symbolicmode-0.9.5.9/src/symbolicmode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-04-10 00:31:10.000000 symbolicmode-0.9.5.9/src/symbolicmode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-10 00:31:10.000000 symbolicmode-0.9.5.9/src/symbolicmode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 00:31:10.000000 symbolicmode-0.9.5.9/src/symbolicmode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-10 00:31:10.000000 symbolicmode-0.9.5.9/src/symbolicmode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:31:10.160957 symbolicmode-0.9.5.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-10 00:30:47.000000 symbolicmode-0.9.5.9/tests/test_chmod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-04-10 00:30:47.000000 symbolicmode-0.9.5.9/tests/test_modes.py
```

### Comparing `symbolicmode-0.9.5.8/LICENSE` & `symbolicmode-0.9.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `symbolicmode-0.9.5.8/PKG-INFO` & `symbolicmode-0.9.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbolicmode
-Version: 0.9.5.8
+Version: 0.9.5.9
 Summary: Code to handle symbolic permissions like GNU chmod does ('a=rx,u+w')
 Author-email: Sean Reifschneider <jafo00@gmail.com>
 Project-URL: Homepage, https://github.com/linsomniac/symbolicmode
 Project-URL: Bug Tracker, https://github.com/linsomniac/symbolicmode/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
```

### Comparing `symbolicmode-0.9.5.8/README.md` & `symbolicmode-0.9.5.9/README.md`

 * *Files identical despite different names*

### Comparing `symbolicmode-0.9.5.8/pyproject.toml` & `symbolicmode-0.9.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 pythonpath = "src"
 
 [project]
 name = "symbolicmode"
-version = "0.9.5.8"
+version = "0.9.5.9"
 authors = [
   { name="Sean Reifschneider", email="jafo00@gmail.com" },
 ]
 description = "Code to handle symbolic permissions like GNU chmod does ('a=rx,u+w')"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `symbolicmode-0.9.5.8/src/symbolicmode/__init__.py` & `symbolicmode-0.9.5.9/src/symbolicmode/__init__.py`

 * *Files identical despite different names*

### Comparing `symbolicmode-0.9.5.8/src/symbolicmode.egg-info/PKG-INFO` & `symbolicmode-0.9.5.9/src/symbolicmode.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbolicmode
-Version: 0.9.5.8
+Version: 0.9.5.9
 Summary: Code to handle symbolic permissions like GNU chmod does ('a=rx,u+w')
 Author-email: Sean Reifschneider <jafo00@gmail.com>
 Project-URL: Homepage, https://github.com/linsomniac/symbolicmode
 Project-URL: Bug Tracker, https://github.com/linsomniac/symbolicmode/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
```

### Comparing `symbolicmode-0.9.5.8/tests/test_chmod.py` & `symbolicmode-0.9.5.9/tests/test_chmod.py`

 * *Files identical despite different names*

### Comparing `symbolicmode-0.9.5.8/tests/test_modes.py` & `symbolicmode-0.9.5.9/tests/test_modes.py`

 * *Files identical despite different names*

