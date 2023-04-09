# Comparing `tmp/symbolicmode-0.9.5.tar.gz` & `tmp/symbolicmode-0.9.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbolicmode-0.9.5.tar", last modified: Sun Apr  9 17:58:34 2023, max compression
+gzip compressed data, was "symbolicmode-0.9.5.1.tar", last modified: Sun Apr  9 23:36:51 2023, max compression
```

## Comparing `symbolicmode-0.9.5.tar` & `symbolicmode-0.9.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:58:34.877075 symbolicmode-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-09 17:58:23.000000 symbolicmode-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-04-09 17:58:34.877075 symbolicmode-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-09 17:58:23.000000 symbolicmode-0.9.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-09 17:58:27.000000 symbolicmode-0.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 17:58:34.877075 symbolicmode-0.9.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:58:34.873075 symbolicmode-0.9.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:58:34.873075 symbolicmode-0.9.5/src/symbolicmode/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9017 2023-04-09 17:58:23.000000 symbolicmode-0.9.5/src/symbolicmode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:58:34.873075 symbolicmode-0.9.5/src/symbolicmode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-04-09 17:58:34.000000 symbolicmode-0.9.5/src/symbolicmode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-09 17:58:34.000000 symbolicmode-0.9.5/src/symbolicmode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 17:58:34.000000 symbolicmode-0.9.5/src/symbolicmode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-09 17:58:34.000000 symbolicmode-0.9.5/src/symbolicmode.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:58:34.877075 symbolicmode-0.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-09 17:58:23.000000 symbolicmode-0.9.5/tests/test_chmod.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-04-09 17:58:23.000000 symbolicmode-0.9.5/tests/test_modes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:36:51.782004 symbolicmode-0.9.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-09 23:36:42.000000 symbolicmode-0.9.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-04-09 23:36:51.782004 symbolicmode-0.9.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-09 23:36:42.000000 symbolicmode-0.9.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-09 23:36:45.000000 symbolicmode-0.9.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 23:36:51.782004 symbolicmode-0.9.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:36:51.778004 symbolicmode-0.9.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:36:51.782004 symbolicmode-0.9.5.1/src/symbolicmode/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9017 2023-04-09 23:36:42.000000 symbolicmode-0.9.5.1/src/symbolicmode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:36:51.782004 symbolicmode-0.9.5.1/src/symbolicmode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-04-09 23:36:51.000000 symbolicmode-0.9.5.1/src/symbolicmode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-09 23:36:51.000000 symbolicmode-0.9.5.1/src/symbolicmode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 23:36:51.000000 symbolicmode-0.9.5.1/src/symbolicmode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-09 23:36:51.000000 symbolicmode-0.9.5.1/src/symbolicmode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:36:51.782004 symbolicmode-0.9.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-09 23:36:42.000000 symbolicmode-0.9.5.1/tests/test_chmod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-04-09 23:36:42.000000 symbolicmode-0.9.5.1/tests/test_modes.py
```

### Comparing `symbolicmode-0.9.5/LICENSE` & `symbolicmode-0.9.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `symbolicmode-0.9.5/PKG-INFO` & `symbolicmode-0.9.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbolicmode
-Version: 0.9.5
+Version: 0.9.5.1
 Summary: Code to handle symbolic permissions like GNU chmod does ('a=rx,u+w')
 Author-email: Sean Reifschneider <jafo00@gmail.com>
 Project-URL: Homepage, https://github.com/linsomniac/symbolicmode
 Project-URL: Bug Tracker, https://github.com/linsomniac/symbolicmode/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
```

### Comparing `symbolicmode-0.9.5/README.md` & `symbolicmode-0.9.5.1/README.md`

 * *Files identical despite different names*

### Comparing `symbolicmode-0.9.5/pyproject.toml` & `symbolicmode-0.9.5.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 pythonpath = "src"
 
 [project]
 name = "symbolicmode"
-version = "0.9.5"
+version = "0.9.5.1"
 authors = [
   { name="Sean Reifschneider", email="jafo00@gmail.com" },
 ]
 description = "Code to handle symbolic permissions like GNU chmod does ('a=rx,u+w')"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `symbolicmode-0.9.5/src/symbolicmode/__init__.py` & `symbolicmode-0.9.5.1/src/symbolicmode/__init__.py`

 * *Files identical despite different names*

### Comparing `symbolicmode-0.9.5/src/symbolicmode.egg-info/PKG-INFO` & `symbolicmode-0.9.5.1/src/symbolicmode.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbolicmode
-Version: 0.9.5
+Version: 0.9.5.1
 Summary: Code to handle symbolic permissions like GNU chmod does ('a=rx,u+w')
 Author-email: Sean Reifschneider <jafo00@gmail.com>
 Project-URL: Homepage, https://github.com/linsomniac/symbolicmode
 Project-URL: Bug Tracker, https://github.com/linsomniac/symbolicmode/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
```

### Comparing `symbolicmode-0.9.5/tests/test_chmod.py` & `symbolicmode-0.9.5.1/tests/test_chmod.py`

 * *Files identical despite different names*

### Comparing `symbolicmode-0.9.5/tests/test_modes.py` & `symbolicmode-0.9.5.1/tests/test_modes.py`

 * *Files identical despite different names*

