# Comparing `tmp/python-yate-0.4.0.tar.gz` & `tmp/python-yate-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-yate-0.4.0.tar", last modified: Wed Aug 10 19:39:37 2022, max compression
+gzip compressed data, was "python-yate-0.4.1.tar", last modified: Sun Apr  9 22:35:44 2023, max compression
```

## Comparing `python-yate-0.4.0.tar` & `python-yate-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 19:39:37.570745 python-yate-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-08-10 19:39:26.000000 python-yate-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-08-10 19:39:26.000000 python-yate-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-08-10 19:39:37.570745 python-yate-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-08-10 19:39:26.000000 python-yate-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 19:39:37.570745 python-yate-0.4.0/python_yate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-08-10 19:39:37.000000 python-yate-0.4.0/python_yate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-08-10 19:39:37.000000 python-yate-0.4.0/python_yate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-10 19:39:37.000000 python-yate-0.4.0/python_yate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-08-10 19:39:37.000000 python-yate-0.4.0/python_yate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-10 19:39:37.000000 python-yate-0.4.0/python_yate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-10 19:39:37.570745 python-yate-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-08-10 19:39:26.000000 python-yate-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 19:39:37.570745 python-yate-0.4.0/yate/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-10 19:39:26.000000 python-yate-0.4.0/yate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6413 2022-08-10 19:39:26.000000 python-yate-0.4.0/yate/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (121)     9995 2022-08-10 19:39:26.000000 python-yate-0.4.0/yate/ivr.py
--rw-r--r--   0 runner    (1001) docker     (121)    10591 2022-08-10 19:39:26.000000 python-yate-0.4.0/yate/protocol.py
--rw-r--r--   0 runner    (1001) docker     (121)     8096 2022-08-10 19:39:26.000000 python-yate-0.4.0/yate/yate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 22:35:44.761064 python-yate-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-09 22:35:31.000000 python-yate-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-09 22:35:31.000000 python-yate-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-09 22:35:44.761064 python-yate-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-09 22:35:31.000000 python-yate-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 22:35:44.761064 python-yate-0.4.1/python_yate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-09 22:35:44.000000 python-yate-0.4.1/python_yate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-09 22:35:44.000000 python-yate-0.4.1/python_yate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 22:35:44.000000 python-yate-0.4.1/python_yate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-09 22:35:44.000000 python-yate-0.4.1/python_yate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-09 22:35:44.000000 python-yate-0.4.1/python_yate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 22:35:44.000000 python-yate-0.4.1/python_yate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 22:35:44.761064 python-yate-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-09 22:35:31.000000 python-yate-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 22:35:44.761064 python-yate-0.4.1/yate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 22:35:31.000000 python-yate-0.4.1/yate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-04-09 22:35:31.000000 python-yate-0.4.1/yate/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-04-09 22:35:31.000000 python-yate-0.4.1/yate/callgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-04-09 22:35:31.000000 python-yate-0.4.1/yate/ivr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10591 2023-04-09 22:35:31.000000 python-yate-0.4.1/yate/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-04-09 22:35:31.000000 python-yate-0.4.1/yate/yate.py
```

### Comparing `python-yate-0.4.0/LICENSE` & `python-yate-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-yate-0.4.0/PKG-INFO` & `python-yate-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-yate
-Version: 0.4.0
+Version: 0.4.1
 Summary: An (asyncio enabled) python library for yate IVRs and extmodules
 Home-page: https://github.com/eventphone/python-yate
 Author: Martin Lang
 Author-email: Martin.Lang@rwth-aachen.de
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `python-yate-0.4.0/python_yate.egg-info/PKG-INFO` & `python-yate-0.4.1/python_yate.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-yate
-Version: 0.4.0
+Version: 0.4.1
 Summary: An (asyncio enabled) python library for yate IVRs and extmodules
 Home-page: https://github.com/eventphone/python-yate
 Author: Martin Lang
 Author-email: Martin.Lang@rwth-aachen.de
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `python-yate-0.4.0/setup.py` & `python-yate-0.4.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_dir = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(this_dir, "README.md"), "r") as f:
     long_description = f.read()
 
 setup(
     name='python-yate',
-    version='0.4.0',
+    version='0.4.1',
     packages=['yate'],
     url='https://github.com/eventphone/python-yate',
     license='MIT',
     author='Martin Lang',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email='Martin.Lang@rwth-aachen.de',
@@ -24,8 +24,13 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: MIT License",
     ],
     install_requires=[
         'async_timeout',
     ],
+    entry_points={
+        "console_scripts": [
+            "yate_callgen=yate.callgen:main",
+        ],
+    },
 )
```

### Comparing `python-yate-0.4.0/yate/asyncio.py` & `python-yate-0.4.1/yate/asyncio.py`

 * *Files identical despite different names*

### Comparing `python-yate-0.4.0/yate/ivr.py` & `python-yate-0.4.1/yate/ivr.py`

 * *Files identical despite different names*

### Comparing `python-yate-0.4.0/yate/protocol.py` & `python-yate-0.4.1/yate/protocol.py`

 * *Files identical despite different names*

### Comparing `python-yate-0.4.0/yate/yate.py` & `python-yate-0.4.1/yate/yate.py`

 * *Files identical despite different names*

