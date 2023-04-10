# Comparing `tmp/datrafilcha-1.0.3.tar.gz` & `tmp/datrafilcha-1.0.4.tar.gz`

## Comparing `datrafilcha-1.0.3.tar` & `datrafilcha-1.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 datrafilcha-1.0.3/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datrafilcha-1.0.3/datrafilcha/__init__.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 datrafilcha-1.0.3/datrafilcha/facade.py
--rw-r--r--   0        0        0     5576 2020-02-02 00:00:00.000000 datrafilcha-1.0.3/datrafilcha/graph_functions.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 datrafilcha-1.0.3/LICENSE
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 datrafilcha-1.0.3/README.md
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 datrafilcha-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 datrafilcha-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 datrafilcha-1.0.4/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datrafilcha-1.0.4/datrafilcha/__init__.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 datrafilcha-1.0.4/datrafilcha/facade.py
+-rw-r--r--   0        0        0     5576 2020-02-02 00:00:00.000000 datrafilcha-1.0.4/datrafilcha/graph_functions.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 datrafilcha-1.0.4/LICENSE
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 datrafilcha-1.0.4/README.md
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 datrafilcha-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 datrafilcha-1.0.4/PKG-INFO
```

### Comparing `datrafilcha-1.0.3/datrafilcha/facade.py` & `datrafilcha-1.0.4/datrafilcha/facade.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from os import path
 
 from . import graph_functions
-from .graph_functions import _FactoryManager, _ColumnDataFromCSV
+from .graph_functions import _FactoryManager, ColumnDataFromCSV
 
 
 class DataFiltersFacade:
     def __init__(self):
         self.factory_manager = _FactoryManager
 
     def csv_column(self, function_cfg: dict, data_source_file: str, column: str):
```

### Comparing `datrafilcha-1.0.3/datrafilcha/graph_functions.py` & `datrafilcha-1.0.4/datrafilcha/graph_functions.py`

 * *Files identical despite different names*

### Comparing `datrafilcha-1.0.3/LICENSE` & `datrafilcha-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datrafilcha-1.0.3/README.md` & `datrafilcha-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `datrafilcha-1.0.3/PKG-INFO` & `datrafilcha-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datrafilcha
-Version: 1.0.3
+Version: 1.0.4
 Project-URL: Homepage, https://gitlab.com/gitm1993/datrafilcha
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

