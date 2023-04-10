# Comparing `tmp/skduplo-0.1.0.tar.gz` & `tmp/skduplo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skduplo-0.1.0.tar", last modified: Mon Apr 10 04:40:34 2023, max compression
+gzip compressed data, was "skduplo-0.1.1.tar", last modified: Mon Apr 10 06:18:21 2023, max compression
```

## Comparing `skduplo-0.1.0.tar` & `skduplo-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2023-04-10 04:40:34.370022 skduplo-0.1.0/
--rw-r--r--   0 johnhawkins   (501) staff       (20)     1082 2023-04-06 00:11:51.000000 skduplo-0.1.0/LICENSE
--rw-r--r--   0 johnhawkins   (501) staff       (20)     1510 2023-04-10 04:40:34.369762 skduplo-0.1.0/PKG-INFO
--rw-r--r--   0 johnhawkins   (501) staff       (20)      975 2023-04-10 04:39:54.000000 skduplo-0.1.0/README.md
--rw-r--r--   0 johnhawkins   (501) staff       (20)       38 2023-04-10 04:40:34.370104 skduplo-0.1.0/setup.cfg
--rwxr-xr-x   0 johnhawkins   (501) staff       (20)     1106 2023-04-06 23:15:01.000000 skduplo-0.1.0/setup.py
-drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2023-04-10 04:40:34.367698 skduplo-0.1.0/skduplo/
--rw-r--r--   0 johnhawkins   (501) staff       (20)       22 2023-04-10 02:50:15.000000 skduplo-0.1.0/skduplo/__init__.py
-drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2023-04-10 04:40:34.369296 skduplo-0.1.0/skduplo.egg-info/
--rw-r--r--   0 johnhawkins   (501) staff       (20)     1510 2023-04-10 04:40:34.000000 skduplo-0.1.0/skduplo.egg-info/PKG-INFO
--rw-r--r--   0 johnhawkins   (501) staff       (20)      200 2023-04-10 04:40:34.000000 skduplo-0.1.0/skduplo.egg-info/SOURCES.txt
--rw-r--r--   0 johnhawkins   (501) staff       (20)        1 2023-04-10 04:40:34.000000 skduplo-0.1.0/skduplo.egg-info/dependency_links.txt
--rw-r--r--   0 johnhawkins   (501) staff       (20)       21 2023-04-10 04:40:34.000000 skduplo-0.1.0/skduplo.egg-info/requires.txt
--rw-r--r--   0 johnhawkins   (501) staff       (20)        8 2023-04-10 04:40:34.000000 skduplo-0.1.0/skduplo.egg-info/top_level.txt
+drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2023-04-10 06:18:21.745989 skduplo-0.1.1/
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     1082 2023-04-06 00:11:51.000000 skduplo-0.1.1/LICENSE
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     1762 2023-04-10 06:18:21.745666 skduplo-0.1.1/PKG-INFO
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     1227 2023-04-10 06:17:16.000000 skduplo-0.1.1/README.md
+-rw-r--r--   0 johnhawkins   (501) staff       (20)       38 2023-04-10 06:18:21.746070 skduplo-0.1.1/setup.cfg
+-rwxr-xr-x   0 johnhawkins   (501) staff       (20)     1111 2023-04-10 06:12:55.000000 skduplo-0.1.1/setup.py
+drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2023-04-10 06:18:21.743386 skduplo-0.1.1/skduplo/
+-rw-r--r--   0 johnhawkins   (501) staff       (20)       22 2023-04-10 06:17:42.000000 skduplo-0.1.1/skduplo/__init__.py
+drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2023-04-10 06:18:21.745195 skduplo-0.1.1/skduplo.egg-info/
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     1762 2023-04-10 06:18:21.000000 skduplo-0.1.1/skduplo.egg-info/PKG-INFO
+-rw-r--r--   0 johnhawkins   (501) staff       (20)      200 2023-04-10 06:18:21.000000 skduplo-0.1.1/skduplo.egg-info/SOURCES.txt
+-rw-r--r--   0 johnhawkins   (501) staff       (20)        1 2023-04-10 06:18:21.000000 skduplo-0.1.1/skduplo.egg-info/dependency_links.txt
+-rw-r--r--   0 johnhawkins   (501) staff       (20)       26 2023-04-10 06:18:21.000000 skduplo-0.1.1/skduplo.egg-info/requires.txt
+-rw-r--r--   0 johnhawkins   (501) staff       (20)        8 2023-04-10 06:18:21.000000 skduplo-0.1.1/skduplo.egg-info/top_level.txt
```

### Comparing `skduplo-0.1.0/LICENSE` & `skduplo-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skduplo-0.1.0/PKG-INFO` & `skduplo-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skduplo
-Version: 0.1.0
+Version: 0.1.1
 Summary: Sci-kit learn tools for machine learning pipelines
 Home-page: http://getting-data-science-done.com
 Author: John Hawkins
 Author-email: johnc@getting-data-science-done.com
 License: MIT
 Project-URL: Documentation, http://scikit-duplo.readthedocs.io
 Project-URL: Source, https://github.com/getting-data-science-done/scikit-duplo
@@ -13,15 +13,16 @@
 License-File: LICENSE
 
 # scikit-duplo
 
 Very simple reusable blocks for scikit-learn pipelines  (inspired by scikit-lego)
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-
+[![PyPI](https://img.shields.io/pypi/v/scikit-duplo.svg)](https://pypi.org/project/scikit-duplo)
+[![Documentation Status](https://readthedocs.org/projects/scikit-duplo/badge/?version=latest)](https://scikit-duplo.readthedocs.io/en/latest/?badge=latest)
 
 # Installation
 
 Installation from the source tree:
 
 ```
 python setup.py install
```

### Comparing `skduplo-0.1.0/setup.py` & `skduplo-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     long_descr = f.read().decode("utf-8")
 
 setup(
       license="MIT",
       name = "skduplo",
       packages = ["skduplo"],
       install_requires=[
-        'pandas','numpy','sklearn'
+        'pandas','numpy','scikit-learn'
       ],
       include_package_data=True,
       version = version,
       description = "Sci-kit learn tools for machine learning pipelines",
       long_description = long_descr,
       long_description_content_type='text/markdown',
       author = "John Hawkins",
```

### Comparing `skduplo-0.1.0/skduplo.egg-info/PKG-INFO` & `skduplo-0.1.1/skduplo.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skduplo
-Version: 0.1.0
+Version: 0.1.1
 Summary: Sci-kit learn tools for machine learning pipelines
 Home-page: http://getting-data-science-done.com
 Author: John Hawkins
 Author-email: johnc@getting-data-science-done.com
 License: MIT
 Project-URL: Documentation, http://scikit-duplo.readthedocs.io
 Project-URL: Source, https://github.com/getting-data-science-done/scikit-duplo
@@ -13,15 +13,16 @@
 License-File: LICENSE
 
 # scikit-duplo
 
 Very simple reusable blocks for scikit-learn pipelines  (inspired by scikit-lego)
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-
+[![PyPI](https://img.shields.io/pypi/v/scikit-duplo.svg)](https://pypi.org/project/scikit-duplo)
+[![Documentation Status](https://readthedocs.org/projects/scikit-duplo/badge/?version=latest)](https://scikit-duplo.readthedocs.io/en/latest/?badge=latest)
 
 # Installation
 
 Installation from the source tree:
 
 ```
 python setup.py install
```

