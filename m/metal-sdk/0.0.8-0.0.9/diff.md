# Comparing `tmp/metal_sdk-0.0.8.tar.gz` & `tmp/metal_sdk-0.0.9.tar.gz`

## Comparing `metal_sdk-0.0.8.tar` & `metal_sdk-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metal_sdk-0.0.8/src/metal_sdk/__init__.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 metal_sdk-0.0.8/src/metal_sdk/metal.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 metal_sdk-0.0.8/src/metal_sdk/typings.py
--rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 metal_sdk-0.0.8/tests/test_metal.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 metal_sdk-0.0.8/.gitignore
--rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 metal_sdk-0.0.8/LICENSE
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 metal_sdk-0.0.8/README.md
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 metal_sdk-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 metal_sdk-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 metal_sdk-0.0.9/src/metal_sdk/Metal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metal_sdk-0.0.9/src/metal_sdk/__init__.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 metal_sdk-0.0.9/src/metal_sdk/typings.py
+-rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 metal_sdk-0.0.9/tests/test_metal.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 metal_sdk-0.0.9/.gitignore
+-rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 metal_sdk-0.0.9/LICENSE
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 metal_sdk-0.0.9/README.md
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 metal_sdk-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 metal_sdk-0.0.9/PKG-INFO
```

### Comparing `metal_sdk-0.0.8/src/metal_sdk/metal.py` & `metal_sdk-0.0.9/src/metal_sdk/Metal.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-0.0.8/src/metal_sdk/typings.py` & `metal_sdk-0.0.9/src/metal_sdk/typings.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-0.0.8/tests/test_metal.py` & `metal_sdk-0.0.9/tests/test_metal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from unittest import TestCase, mock
-from src.metal_sdk.metal import Metal
+from src.metal_sdk.Metal import Metal
 
 
 API_KEY = 'api-key'
 CLIENT_ID = 'client-id'
 
 class TestMetal(TestCase):
     def test_metal_instantiate(self):
```

### Comparing `metal_sdk-0.0.8/.gitignore` & `metal_sdk-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `metal_sdk-0.0.8/LICENSE` & `metal_sdk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `metal_sdk-0.0.8/README.md` & `metal_sdk-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `metal_sdk-0.0.8/PKG-INFO` & `metal_sdk-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metal_sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: SDK for getmetal.io
 Project-URL: Github, https://github.com/getmetal/metal-python
 Author-email: Metal Technologies Inc <james@getmetal.io>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

