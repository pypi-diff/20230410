# Comparing `tmp/pyhOn-0.6.1.tar.gz` & `tmp/pyhOn-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhOn-0.6.1.tar", last modified: Mon Apr 10 15:06:54 2023, max compression
+gzip compressed data, was "pyhOn-0.6.2.tar", last modified: Mon Apr 10 16:51:00 2023, max compression
```

## Comparing `pyhOn-0.6.1.tar` & `pyhOn-0.6.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:06:54.561832 pyhOn-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-10 15:06:42.000000 pyhOn-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-10 15:06:54.561832 pyhOn-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-10 15:06:42.000000 pyhOn-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:06:54.557832 pyhOn-0.6.1/pyhOn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-10 15:06:54.000000 pyhOn-0.6.1/pyhOn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-10 15:06:54.000000 pyhOn-0.6.1/pyhOn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:06:54.000000 pyhOn-0.6.1/pyhOn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 15:06:54.000000 pyhOn-0.6.1/pyhOn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 15:06:54.000000 pyhOn-0.6.1/pyhOn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 15:06:54.000000 pyhOn-0.6.1/pyhOn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:06:54.557832 pyhOn-0.6.1/pyhon/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4839 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/appliance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:06:54.557832 pyhOn-0.6.1/pyhon/appliances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/appliances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/appliances/ov.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/appliances/td.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/appliances/wd.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/appliances/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:06:54.561832 pyhOn-0.6.1/pyhon/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/connection/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/connection/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/connection/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/connection/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/hon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 15:06:54.561832 pyhOn-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-10 15:06:42.000000 pyhOn-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:51:00.737891 pyhOn-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-10 16:50:51.000000 pyhOn-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-10 16:51:00.737891 pyhOn-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-10 16:50:51.000000 pyhOn-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:51:00.737891 pyhOn-0.6.2/pyhOn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-10 16:51:00.000000 pyhOn-0.6.2/pyhOn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-10 16:51:00.000000 pyhOn-0.6.2/pyhOn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:51:00.000000 pyhOn-0.6.2/pyhOn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 16:51:00.000000 pyhOn-0.6.2/pyhOn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 16:51:00.000000 pyhOn-0.6.2/pyhOn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 16:51:00.000000 pyhOn-0.6.2/pyhOn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:51:00.737891 pyhOn-0.6.2/pyhon/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4839 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/appliance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:51:00.737891 pyhOn-0.6.2/pyhon/appliances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/appliances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/appliances/ov.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/appliances/td.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/appliances/wd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/appliances/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:51:00.737891 pyhOn-0.6.2/pyhon/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/connection/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/connection/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/connection/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/connection/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/hon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-10 16:50:51.000000 pyhOn-0.6.2/pyhon/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 16:51:00.737891 pyhOn-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-10 16:50:51.000000 pyhOn-0.6.2/setup.py
```

### Comparing `pyhOn-0.6.1/LICENSE` & `pyhOn-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.1/PKG-INFO` & `pyhOn-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.6.1
+Version: 0.6.2
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.6.1/README.md` & `pyhOn-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.1/pyhOn.egg-info/PKG-INFO` & `pyhOn-0.6.2/pyhOn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.6.1
+Version: 0.6.2
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.6.1/pyhOn.egg-info/SOURCES.txt` & `pyhOn-0.6.2/pyhOn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.1/pyhon/__main__.py` & `pyhOn-0.6.2/pyhon/__main__.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.1/pyhon/appliance.py` & `pyhOn-0.6.2/pyhon/appliance.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.1/pyhon/appliances/ov.py` & `pyhOn-0.6.2/pyhon/appliances/ov.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.1/pyhon/commands.py` & `pyhOn-0.6.2/pyhon/commands.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.1/pyhon/connection/api.py` & `pyhOn-0.6.2/pyhon/connection/api.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.1/pyhon/connection/auth.py` & `pyhOn-0.6.2/pyhon/connection/auth.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.1/pyhon/connection/device.py` & `pyhOn-0.6.2/pyhon/connection/device.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.1/pyhon/connection/handler.py` & `pyhOn-0.6.2/pyhon/connection/handler.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.1/pyhon/hon.py` & `pyhOn-0.6.2/pyhon/hon.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.1/pyhon/parameter.py` & `pyhOn-0.6.2/pyhon/parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import re
 
 
 def str_to_float(string):
-    return float(string.replace(",", "."))
+    try:
+        return int(string)
+    except ValueError:
+        return float(str(string.replace(",", ".")))
 
 
 class HonParameter:
     def __init__(self, key, attributes):
         self._key = key
         self._category = attributes.get("category")
         self._typology = attributes.get("typology")
```

### Comparing `pyhOn-0.6.1/setup.py` & `pyhOn-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pyhOn",
-    version="0.6.1",
+    version="0.6.2",
     author="Andre Basche",
     description="Control hOn devices with python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         "GitHub": "https://github.com/Andre0512/pyhOn",
         "PyPI": "https://pypi.org/project/pyhOn",
```

