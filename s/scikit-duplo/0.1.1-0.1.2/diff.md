# Comparing `tmp/scikit-duplo-0.1.1.tar.gz` & `tmp/scikit-duplo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-duplo-0.1.1.tar", last modified: Mon Apr 10 06:21:32 2023, max compression
+gzip compressed data, was "scikit-duplo-0.1.2.tar", last modified: Mon Apr 10 21:57:45 2023, max compression
```

## Comparing `scikit-duplo-0.1.1.tar` & `scikit-duplo-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,22 @@
-drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2023-04-10 06:21:32.876671 scikit-duplo-0.1.1/
--rw-r--r--   0 johnhawkins   (501) staff       (20)     1082 2023-04-06 00:11:51.000000 scikit-duplo-0.1.1/LICENSE
--rw-r--r--   0 johnhawkins   (501) staff       (20)     1767 2023-04-10 06:21:32.876274 scikit-duplo-0.1.1/PKG-INFO
--rw-r--r--   0 johnhawkins   (501) staff       (20)     1227 2023-04-10 06:17:16.000000 scikit-duplo-0.1.1/README.md
-drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2023-04-10 06:21:32.875422 scikit-duplo-0.1.1/scikit_duplo.egg-info/
--rw-r--r--   0 johnhawkins   (501) staff       (20)     1767 2023-04-10 06:21:32.000000 scikit-duplo-0.1.1/scikit_duplo.egg-info/PKG-INFO
--rw-r--r--   0 johnhawkins   (501) staff       (20)      225 2023-04-10 06:21:32.000000 scikit-duplo-0.1.1/scikit_duplo.egg-info/SOURCES.txt
--rw-r--r--   0 johnhawkins   (501) staff       (20)        1 2023-04-10 06:21:32.000000 scikit-duplo-0.1.1/scikit_duplo.egg-info/dependency_links.txt
--rw-r--r--   0 johnhawkins   (501) staff       (20)       26 2023-04-10 06:21:32.000000 scikit-duplo-0.1.1/scikit_duplo.egg-info/requires.txt
--rw-r--r--   0 johnhawkins   (501) staff       (20)        8 2023-04-10 06:21:32.000000 scikit-duplo-0.1.1/scikit_duplo.egg-info/top_level.txt
--rw-r--r--   0 johnhawkins   (501) staff       (20)       38 2023-04-10 06:21:32.876792 scikit-duplo-0.1.1/setup.cfg
--rwxr-xr-x   0 johnhawkins   (501) staff       (20)     1116 2023-04-10 06:21:27.000000 scikit-duplo-0.1.1/setup.py
-drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2023-04-10 06:21:32.875693 scikit-duplo-0.1.1/skduplo/
--rw-r--r--   0 johnhawkins   (501) staff       (20)       22 2023-04-10 06:17:42.000000 scikit-duplo-0.1.1/skduplo/__init__.py
+drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2023-04-10 21:57:45.138040 scikit-duplo-0.1.2/
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     1082 2023-04-06 00:11:51.000000 scikit-duplo-0.1.2/LICENSE
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     1767 2023-04-10 21:57:45.137534 scikit-duplo-0.1.2/PKG-INFO
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     1227 2023-04-10 06:17:16.000000 scikit-duplo-0.1.2/README.md
+drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2023-04-10 21:57:45.130552 scikit-duplo-0.1.2/scikit_duplo.egg-info/
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     1767 2023-04-10 21:57:45.000000 scikit-duplo-0.1.2/scikit_duplo.egg-info/PKG-INFO
+-rw-r--r--   0 johnhawkins   (501) staff       (20)      449 2023-04-10 21:57:45.000000 scikit-duplo-0.1.2/scikit_duplo.egg-info/SOURCES.txt
+-rw-r--r--   0 johnhawkins   (501) staff       (20)        1 2023-04-10 21:57:45.000000 scikit-duplo-0.1.2/scikit_duplo.egg-info/dependency_links.txt
+-rw-r--r--   0 johnhawkins   (501) staff       (20)       26 2023-04-10 21:57:45.000000 scikit-duplo-0.1.2/scikit_duplo.egg-info/requires.txt
+-rw-r--r--   0 johnhawkins   (501) staff       (20)        8 2023-04-10 21:57:45.000000 scikit-duplo-0.1.2/scikit_duplo.egg-info/top_level.txt
+-rw-r--r--   0 johnhawkins   (501) staff       (20)       38 2023-04-10 21:57:45.138169 scikit-duplo-0.1.2/setup.cfg
+-rwxr-xr-x   0 johnhawkins   (501) staff       (20)     1163 2023-04-10 21:57:03.000000 scikit-duplo-0.1.2/setup.py
+drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2023-04-10 21:57:45.130998 scikit-duplo-0.1.2/skduplo/
+-rw-r--r--   0 johnhawkins   (501) staff       (20)       22 2023-04-10 21:57:16.000000 scikit-duplo-0.1.2/skduplo/__init__.py
+drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2023-04-10 21:57:45.133470 scikit-duplo-0.1.2/skduplo/meta/
+-rw-r--r--   0 johnhawkins   (501) staff       (20)      170 2023-04-06 21:57:24.000000 scikit-duplo-0.1.2/skduplo/meta/__init__.py
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     5862 2023-04-06 22:04:15.000000 scikit-duplo-0.1.2/skduplo/meta/quantile_stack_regressor.py
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     4894 2023-04-06 22:03:28.000000 scikit-duplo-0.1.2/skduplo/meta/regressor_stack.py
+drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2023-04-10 21:57:45.136379 scikit-duplo-0.1.2/skduplo/preprocessing/
+-rw-r--r--   0 johnhawkins   (501) staff       (20)      172 2023-04-06 21:55:06.000000 scikit-duplo-0.1.2/skduplo/preprocessing/__init__.py
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     1155 2023-04-06 00:24:35.000000 scikit-duplo-0.1.2/skduplo/preprocessing/column_concatenator.py
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     1217 2023-04-06 00:20:02.000000 scikit-duplo-0.1.2/skduplo/preprocessing/two_column_ratio_diff.py
```

### Comparing `scikit-duplo-0.1.1/LICENSE` & `scikit-duplo-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-duplo-0.1.1/PKG-INFO` & `scikit-duplo-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-duplo
-Version: 0.1.1
+Version: 0.1.2
 Summary: Sci-kit learn tools for machine learning pipelines
 Home-page: http://getting-data-science-done.com
 Author: John Hawkins
 Author-email: johnc@getting-data-science-done.com
 License: MIT
 Project-URL: Documentation, http://scikit-duplo.readthedocs.io
 Project-URL: Source, https://github.com/getting-data-science-done/scikit-duplo
```

### Comparing `scikit-duplo-0.1.1/README.md` & `scikit-duplo-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `scikit-duplo-0.1.1/scikit_duplo.egg-info/PKG-INFO` & `scikit-duplo-0.1.2/scikit_duplo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-duplo
-Version: 0.1.1
+Version: 0.1.2
 Summary: Sci-kit learn tools for machine learning pipelines
 Home-page: http://getting-data-science-done.com
 Author: John Hawkins
 Author-email: johnc@getting-data-science-done.com
 License: MIT
 Project-URL: Documentation, http://scikit-duplo.readthedocs.io
 Project-URL: Source, https://github.com/getting-data-science-done/scikit-duplo
```

### Comparing `scikit-duplo-0.1.1/setup.py` & `scikit-duplo-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
  
 """setup.py: setuptools control."""
  
+from setuptools import setup, find_packages
 import re
-from setuptools import setup
  
 version = re.search(
         '^__version__\s*=\s*"(.*)"',
         open('skduplo/__init__.py').read(),
         re.M
     ).group(1)
  
 with open("README.md", "rb") as f:
     long_descr = f.read().decode("utf-8")
 
 setup(
       license="MIT",
       name = "scikit-duplo",
-      packages = ["skduplo"],
+      packages=find_packages(exclude=["notebooks", "tests"]),
       install_requires=[
         'pandas','numpy','scikit-learn'
       ],
       include_package_data=True,
       version = version,
       description = "Sci-kit learn tools for machine learning pipelines",
       long_description = long_descr,
```

