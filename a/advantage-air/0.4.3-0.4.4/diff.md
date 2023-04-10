# Comparing `tmp/advantage_air-0.4.3.tar.gz` & `tmp/advantage_air-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advantage_air-0.4.3.tar", last modified: Mon Apr 10 03:31:53 2023, max compression
+gzip compressed data, was "advantage_air-0.4.4.tar", last modified: Mon Apr 10 04:34:28 2023, max compression
```

## Comparing `advantage_air-0.4.3.tar` & `advantage_air-0.4.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 03:31:53.667443 advantage_air-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-10 03:31:44.000000 advantage_air-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-10 03:31:53.667443 advantage_air-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-10 03:31:44.000000 advantage_air-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 03:31:53.667443 advantage_air-0.4.3/advantage_air/
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-04-10 03:31:44.000000 advantage_air-0.4.3/advantage_air/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 03:31:53.667443 advantage_air-0.4.3/advantage_air.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-10 03:31:53.000000 advantage_air-0.4.3/advantage_air.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-10 03:31:53.000000 advantage_air-0.4.3/advantage_air.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 03:31:53.000000 advantage_air-0.4.3/advantage_air.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 03:31:53.000000 advantage_air-0.4.3/advantage_air.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-10 03:31:53.000000 advantage_air-0.4.3/advantage_air.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 03:31:53.667443 advantage_air-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-10 03:31:44.000000 advantage_air-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:34:28.083202 advantage_air-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-10 04:34:16.000000 advantage_air-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-10 04:34:28.083202 advantage_air-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-10 04:34:16.000000 advantage_air-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:34:28.079202 advantage_air-0.4.4/advantage_air/
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-04-10 04:34:16.000000 advantage_air-0.4.4/advantage_air/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:34:28.083202 advantage_air-0.4.4/advantage_air.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-10 04:34:28.000000 advantage_air-0.4.4/advantage_air.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-10 04:34:28.000000 advantage_air-0.4.4/advantage_air.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 04:34:28.000000 advantage_air-0.4.4/advantage_air.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 04:34:28.000000 advantage_air-0.4.4/advantage_air.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-10 04:34:28.000000 advantage_air-0.4.4/advantage_air.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 04:34:28.083202 advantage_air-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-10 04:34:16.000000 advantage_air-0.4.4/setup.py
```

### Comparing `advantage_air-0.4.3/LICENSE` & `advantage_air-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `advantage_air-0.4.3/PKG-INFO` & `advantage_air-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: advantage_air
-Version: 0.4.3
+Version: 0.4.4
 Summary: API helper for Advantage Air's MyAir and e-zone API
 Home-page: https://github.com/Bre77/advantage_air
 Author: Brett Adams
 Author-email: brett@ba.id.au
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `advantage_air-0.4.3/README.md` & `advantage_air-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `advantage_air-0.4.3/advantage_air/__init__.py` & `advantage_air-0.4.4/advantage_air/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import asyncio
 import aiohttp
 import collections.abc
 
-ON = "ON"
-OFF = "OFF"
+ON = "on"
+OFF = "off"
 
 def update(d, u):
     for k, v in u.items():
         if isinstance(v, collections.abc.Mapping):
             d[k] = update(d.get(k, {}), v)
         else:
             d[k] = v
```

### Comparing `advantage_air-0.4.3/advantage_air.egg-info/PKG-INFO` & `advantage_air-0.4.4/advantage_air.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: advantage-air
-Version: 0.4.3
+Version: 0.4.4
 Summary: API helper for Advantage Air's MyAir and e-zone API
 Home-page: https://github.com/Bre77/advantage_air
 Author: Brett Adams
 Author-email: brett@ba.id.au
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `advantage_air-0.4.3/setup.py` & `advantage_air-0.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="advantage_air",
-    version="0.4.3",
+    version="0.4.4",
     author="Brett Adams",
     author_email="brett@ba.id.au",
     description="API helper for Advantage Air's MyAir and e-zone API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Bre77/advantage_air",
     packages=setuptools.find_packages(),
```

