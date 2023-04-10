# Comparing `tmp/h-shap-0.1.5.tar.gz` & `tmp/h-shap-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h-shap-0.1.5.tar", last modified: Mon Aug 22 21:48:59 2022, max compression
+gzip compressed data, was "h-shap-0.1.6.tar", last modified: Mon Apr 10 17:32:46 2023, max compression
```

## Comparing `h-shap-0.1.5.tar` & `h-shap-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-22 21:48:59.909411 h-shap-0.1.5/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      745 2022-08-22 21:48:59.909411 h-shap-0.1.5/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3043 2022-08-22 21:48:58.000000 h-shap-0.1.5/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-22 21:48:59.909411 h-shap-0.1.5/h_shap.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      745 2022-08-22 21:48:59.000000 h-shap-0.1.5/h_shap.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      251 2022-08-22 21:48:59.000000 h-shap-0.1.5/h_shap.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-08-22 21:48:59.000000 h-shap-0.1.5/h_shap.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2022-08-22 21:48:59.000000 h-shap-0.1.5/h_shap.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2022-08-22 21:48:59.000000 h-shap-0.1.5/h_shap.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-22 21:48:59.909411 h-shap-0.1.5/hshap/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       50 2022-08-22 21:48:59.000000 h-shap-0.1.5/hshap/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7232 2022-08-22 21:48:59.000000 h-shap-0.1.5/hshap/src.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3662 2022-08-22 21:48:59.000000 h-shap-0.1.5/hshap/test_src.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4882 2022-08-22 21:48:59.000000 h-shap-0.1.5/hshap/test_utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4502 2022-08-22 21:48:59.000000 h-shap-0.1.5/hshap/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-08-22 21:48:59.909411 h-shap-0.1.5/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1066 2022-08-22 21:48:59.000000 h-shap-0.1.5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-10 17:32:46.486636 h-shap-0.1.6/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      745 2023-04-10 17:32:46.486636 h-shap-0.1.6/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4358 2023-04-10 17:32:45.000000 h-shap-0.1.6/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-10 17:32:46.486636 h-shap-0.1.6/h_shap.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      745 2023-04-10 17:32:46.000000 h-shap-0.1.6/h_shap.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      251 2023-04-10 17:32:46.000000 h-shap-0.1.6/h_shap.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-10 17:32:46.000000 h-shap-0.1.6/h_shap.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-04-10 17:32:46.000000 h-shap-0.1.6/h_shap.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-04-10 17:32:46.000000 h-shap-0.1.6/h_shap.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-10 17:32:46.486636 h-shap-0.1.6/hshap/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2023-04-10 17:32:46.000000 h-shap-0.1.6/hshap/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7232 2023-04-10 17:32:46.000000 h-shap-0.1.6/hshap/src.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3662 2023-04-10 17:32:46.000000 h-shap-0.1.6/hshap/test_src.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4882 2023-04-10 17:32:46.000000 h-shap-0.1.6/hshap/test_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4502 2023-04-10 17:32:46.000000 h-shap-0.1.6/hshap/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-10 17:32:46.486636 h-shap-0.1.6/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1066 2023-04-10 17:32:46.000000 h-shap-0.1.6/setup.py
```

### Comparing `h-shap-0.1.5/PKG-INFO` & `h-shap-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h-shap
-Version: 0.1.5
+Version: 0.1.6
 Summary: Fast Hierarchical Games for Image Explanations
 Home-page: https://github.com/Sulam-Group/h-shap
 Author: Jacopo Teneggi
 Author-email: jtenegg1@jhu.edu
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
```

### Comparing `h-shap-0.1.5/h_shap.egg-info/PKG-INFO` & `h-shap-0.1.6/h_shap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h-shap
-Version: 0.1.5
+Version: 0.1.6
 Summary: Fast Hierarchical Games for Image Explanations
 Home-page: https://github.com/Sulam-Group/h-shap
 Author: Jacopo Teneggi
 Author-email: jtenegg1@jhu.edu
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
```

### Comparing `h-shap-0.1.5/hshap/src.py` & `h-shap-0.1.6/hshap/src.py`

 * *Files identical despite different names*

### Comparing `h-shap-0.1.5/hshap/test_src.py` & `h-shap-0.1.6/hshap/test_src.py`

 * *Files identical despite different names*

### Comparing `h-shap-0.1.5/hshap/test_utils.py` & `h-shap-0.1.6/hshap/test_utils.py`

 * *Files identical despite different names*

### Comparing `h-shap-0.1.5/hshap/utils.py` & `h-shap-0.1.6/hshap/utils.py`

 * *Files identical despite different names*

### Comparing `h-shap-0.1.5/setup.py` & `h-shap-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.1.5"
+VERSION = "0.1.6"
 PACKAGE_NAME = "h-shap"
 DESCRIPTION = "Fast Hierarchical Games for Image Explanations"
 LONG_DESCRIPTION = "`h-shap` provides a fast, hierarchical implementation of Shapley coefficients for image explanations. It is exact, and it does not rely on approximation. In binary classification scenarios, `h-shap` guarantees an exponential computational advantage when explaining an important concept contained in the image."
 AUTHOR = "Jacopo Teneggi"
 AUTHOR_EMAIL = "jtenegg1@jhu.edu"
 
 setup(
```

