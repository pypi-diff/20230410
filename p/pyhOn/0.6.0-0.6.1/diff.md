# Comparing `tmp/pyhOn-0.6.0.tar.gz` & `tmp/pyhOn-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhOn-0.6.0.tar", last modified: Mon Apr 10 04:55:12 2023, max compression
+gzip compressed data, was "pyhOn-0.6.1.tar", last modified: Mon Apr 10 15:06:54 2023, max compression
```

## Comparing `pyhOn-0.6.0.tar` & `pyhOn-0.6.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:55:12.230599 pyhOn-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-10 04:55:02.000000 pyhOn-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-10 04:55:12.230599 pyhOn-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-10 04:55:02.000000 pyhOn-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:55:12.230599 pyhOn-0.6.0/pyhOn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-10 04:55:12.000000 pyhOn-0.6.0/pyhOn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-10 04:55:12.000000 pyhOn-0.6.0/pyhOn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 04:55:12.000000 pyhOn-0.6.0/pyhOn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 04:55:12.000000 pyhOn-0.6.0/pyhOn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 04:55:12.000000 pyhOn-0.6.0/pyhOn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 04:55:12.000000 pyhOn-0.6.0/pyhOn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:55:12.230599 pyhOn-0.6.0/pyhon/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4839 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/appliance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:55:12.230599 pyhOn-0.6.0/pyhon/appliances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/appliances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/appliances/ov.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/appliances/td.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/appliances/wd.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/appliances/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:55:12.230599 pyhOn-0.6.0/pyhon/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/connection/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/connection/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/connection/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/connection/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/hon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-10 04:55:02.000000 pyhOn-0.6.0/pyhon/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 04:55:12.230599 pyhOn-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-10 04:55:02.000000 pyhOn-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:06:54.561832 pyhOn-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-10 15:06:42.000000 pyhOn-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-10 15:06:54.561832 pyhOn-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-10 15:06:42.000000 pyhOn-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:06:54.557832 pyhOn-0.6.1/pyhOn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-10 15:06:54.000000 pyhOn-0.6.1/pyhOn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-10 15:06:54.000000 pyhOn-0.6.1/pyhOn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:06:54.000000 pyhOn-0.6.1/pyhOn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 15:06:54.000000 pyhOn-0.6.1/pyhOn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 15:06:54.000000 pyhOn-0.6.1/pyhOn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 15:06:54.000000 pyhOn-0.6.1/pyhOn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:06:54.557832 pyhOn-0.6.1/pyhon/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4839 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/appliance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:06:54.557832 pyhOn-0.6.1/pyhon/appliances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/appliances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/appliances/ov.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/appliances/td.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/appliances/wd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/appliances/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:06:54.561832 pyhOn-0.6.1/pyhon/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/connection/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/connection/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/connection/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/connection/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/hon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-04-10 15:06:42.000000 pyhOn-0.6.1/pyhon/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 15:06:54.561832 pyhOn-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-10 15:06:42.000000 pyhOn-0.6.1/setup.py
```

### Comparing `pyhOn-0.6.0/LICENSE` & `pyhOn-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.0/PKG-INFO` & `pyhOn-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.6.0
+Version: 0.6.1
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.6.0/README.md` & `pyhOn-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.0/pyhOn.egg-info/PKG-INFO` & `pyhOn-0.6.1/pyhOn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.6.0
+Version: 0.6.1
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.6.0/pyhOn.egg-info/SOURCES.txt` & `pyhOn-0.6.1/pyhOn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.0/pyhon/__main__.py` & `pyhOn-0.6.1/pyhon/__main__.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.0/pyhon/appliance.py` & `pyhOn-0.6.1/pyhon/appliance.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.0/pyhon/appliances/ov.py` & `pyhOn-0.6.1/pyhon/appliances/ov.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.0/pyhon/commands.py` & `pyhOn-0.6.1/pyhon/commands.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.0/pyhon/connection/api.py` & `pyhOn-0.6.1/pyhon/connection/api.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.0/pyhon/connection/auth.py` & `pyhOn-0.6.1/pyhon/connection/auth.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.0/pyhon/connection/device.py` & `pyhOn-0.6.1/pyhon/connection/device.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.0/pyhon/connection/handler.py` & `pyhOn-0.6.1/pyhon/connection/handler.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.0/pyhon/hon.py` & `pyhOn-0.6.1/pyhon/hon.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.0/pyhon/parameter.py` & `pyhOn-0.6.1/pyhon/parameter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import re
 
 
+def str_to_float(string):
+    return float(string.replace(",", "."))
+
+
 class HonParameter:
     def __init__(self, key, attributes):
         self._key = key
         self._category = attributes.get("category")
         self._typology = attributes.get("typology")
         self._mandatory = attributes.get("mandatory")
         self._value = ""
@@ -47,18 +51,18 @@
         if not value == self._value:
             raise ValueError("Can't change fixed value")
 
 
 class HonParameterRange(HonParameter):
     def __init__(self, key, attributes):
         super().__init__(key, attributes)
-        self._min = int(attributes["minimumValue"])
-        self._max = int(attributes["maximumValue"])
-        self._step = int(attributes["incrementValue"])
-        self._default = int(attributes.get("defaultValue", self._min))
+        self._min = str_to_float(attributes["minimumValue"])
+        self._max = str_to_float(attributes["maximumValue"])
+        self._step = str_to_float(attributes["incrementValue"])
+        self._default = str_to_float(attributes.get("defaultValue", self._min))
         self._value = self._default
 
     def __repr__(self):
         return f"{self.__class__} (<{self.key}> [{self._min} - {self._max}])"
 
     @property
     def min(self):
@@ -74,15 +78,15 @@
 
     @property
     def value(self):
         return self._value if self._value is not None else self._min
 
     @value.setter
     def value(self, value):
-        value = int(value)
+        value = str_to_float(value)
         if self._min <= value <= self._max and not value % self._step:
             self._value = value
         else:
             raise ValueError(
                 f"Allowed: min {self._min} max {self._max} step {self._step}"
             )
```

### Comparing `pyhOn-0.6.0/setup.py` & `pyhOn-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pyhOn",
-    version="0.6.0",
+    version="0.6.1",
     author="Andre Basche",
     description="Control hOn devices with python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         "GitHub": "https://github.com/Andre0512/pyhOn",
         "PyPI": "https://pypi.org/project/pyhOn",
```

