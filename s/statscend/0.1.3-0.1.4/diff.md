# Comparing `tmp/statscend-0.1.3.tar.gz` & `tmp/statscend-0.1.4.tar.gz`

## Comparing `statscend-0.1.3.tar` & `statscend-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 statscend-0.1.3/.DS_Store
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 statscend-0.1.3/statscend/__init__.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 statscend-0.1.3/statscend/bn_logistic_regression.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 statscend-0.1.3/statscend/datasets.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 statscend-0.1.3/statscend/logistic_regression.py
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 statscend-0.1.3/statscend/mn_logistic_regression.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 statscend-0.1.3/statscend/ordinal_regression.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 statscend-0.1.3/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 statscend-0.1.3/LICENSE
--rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 statscend-0.1.3/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 statscend-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     7325 2020-02-02 00:00:00.000000 statscend-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 statscend-0.1.4/.DS_Store
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 statscend-0.1.4/statscend/__init__.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 statscend-0.1.4/statscend/bn_logistic_regression.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 statscend-0.1.4/statscend/datasets.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 statscend-0.1.4/statscend/linear_regression.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 statscend-0.1.4/statscend/mn_logistic_regression.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 statscend-0.1.4/statscend/ordinal_regression.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 statscend-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 statscend-0.1.4/LICENSE
+-rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 statscend-0.1.4/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 statscend-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     7325 2020-02-02 00:00:00.000000 statscend-0.1.4/PKG-INFO
```

### Comparing `statscend-0.1.3/.DS_Store` & `statscend-0.1.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `statscend-0.1.3/statscend/bn_logistic_regression.py` & `statscend-0.1.4/statscend/bn_logistic_regression.py`

 * *Files identical despite different names*

### Comparing `statscend-0.1.3/statscend/datasets.py` & `statscend-0.1.4/statscend/datasets.py`

 * *Files identical despite different names*

### Comparing `statscend-0.1.3/statscend/mn_logistic_regression.py` & `statscend-0.1.4/statscend/mn_logistic_regression.py`

 * *Files identical despite different names*

### Comparing `statscend-0.1.3/statscend/ordinal_regression.py` & `statscend-0.1.4/statscend/ordinal_regression.py`

 * *Files identical despite different names*

### Comparing `statscend-0.1.3/LICENSE` & `statscend-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `statscend-0.1.3/README.md` & `statscend-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `statscend-0.1.3/pyproject.toml` & `statscend-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "statscend"
-version = "0.1.3"
+version = "0.1.4"
 license = {file = "LICENSE"}
 authors = [
   { name="Hashim Puthiyakath", email="hashputhiyakath@gmail.com" },
 ]
 description = "A Python package for performing various statistical analyses"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `statscend-0.1.3/PKG-INFO` & `statscend-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statscend
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python package for performing various statistical analyses
 Project-URL: Homepage, https://github.com/hashimputhiyakath/statscend
 Project-URL: Bug Tracker, https://github.com/hashimputhiyakath/statscend/issues
 Author-email: Hashim Puthiyakath <hashputhiyakath@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hashim Puthiyakath
```

