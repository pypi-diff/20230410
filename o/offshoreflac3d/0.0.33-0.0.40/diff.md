# Comparing `tmp/offshoreflac3d-0.0.33.tar.gz` & `tmp/offshoreflac3d-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\offshoreflac3d-0.0.33.tar", last modified: Mon Mar 27 04:16:41 2023, max compression
+gzip compressed data, was "dist\offshoreflac3d-0.0.40.tar", last modified: Mon Apr 10 07:14:12 2023, max compression
```

## Comparing `offshoreflac3d-0.0.33.tar` & `offshoreflac3d-0.0.40.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 04:16:41.000000 offshoreflac3d-0.0.33/
-drwxrwxrwx   0        0        0        0 2023-03-27 04:16:41.000000 offshoreflac3d-0.0.33/offshoreflac3d/
--rw-rw-rw-   0        0        0     3675 2022-12-17 07:07:37.000000 offshoreflac3d-0.0.33/offshoreflac3d/itasca_ini_rectangle.py
--rw-rw-rw-   0        0        0     5668 2023-01-07 14:18:39.000000 offshoreflac3d-0.0.33/offshoreflac3d/itasca_loading.py
--rw-rw-rw-   0        0        0     6474 2022-12-17 07:07:37.000000 offshoreflac3d-0.0.33/offshoreflac3d/itasca_model_rectangle.py
--rw-rw-rw-   0        0        0     3433 2023-03-27 02:43:45.000000 offshoreflac3d-0.0.33/offshoreflac3d/itasca_MonoBucket_Foundation.py
--rw-rw-rw-   0        0        0     6699 2023-02-08 08:48:01.000000 offshoreflac3d-0.0.33/offshoreflac3d/itasca_MonoBucket_gmsh_basic_col.py
--rw-rw-rw-   0        0        0     1964 2023-03-27 02:43:37.000000 offshoreflac3d-0.0.33/offshoreflac3d/itasca_MonoBucket_Initializing.py
--rw-rw-rw-   0        0        0     3075 2023-03-27 03:02:03.000000 offshoreflac3d-0.0.33/offshoreflac3d/itasca_MonoBucket_Loading.py
--rw-rw-rw-   0        0        0     3009 2023-03-27 02:43:30.000000 offshoreflac3d-0.0.33/offshoreflac3d/itasca_MonoBucket_Model.py
--rw-rw-rw-   0        0        0    25163 2022-12-19 08:17:35.000000 offshoreflac3d-0.0.33/offshoreflac3d/itasca_SBJackets_4.py
--rw-rw-rw-   0        0        0       49 2022-12-16 03:10:27.000000 offshoreflac3d-0.0.33/offshoreflac3d/__ini__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 04:16:41.000000 offshoreflac3d-0.0.33/offshoreflac3d.egg-info/
--rw-rw-rw-   0        0        0        1 2023-03-27 04:16:41.000000 offshoreflac3d-0.0.33/offshoreflac3d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      239 2023-03-27 04:16:41.000000 offshoreflac3d-0.0.33/offshoreflac3d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      579 2023-03-27 04:16:41.000000 offshoreflac3d-0.0.33/offshoreflac3d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       15 2023-03-27 04:16:41.000000 offshoreflac3d-0.0.33/offshoreflac3d.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      239 2023-03-27 04:16:41.000000 offshoreflac3d-0.0.33/PKG-INFO
--rw-rw-rw-   0        0        0      522 2022-12-16 08:40:25.000000 offshoreflac3d-0.0.33/README.md
--rw-rw-rw-   0        0        0       42 2023-03-27 04:16:41.000000 offshoreflac3d-0.0.33/setup.cfg
--rw-rw-rw-   0        0        0      641 2023-03-27 04:16:03.000000 offshoreflac3d-0.0.33/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 07:14:12.000000 offshoreflac3d-0.0.40/
+drwxrwxrwx   0        0        0        0 2023-04-10 07:14:12.000000 offshoreflac3d-0.0.40/offshoreflac3d/
+-rw-rw-rw-   0        0        0     3433 2023-03-27 02:43:45.000000 offshoreflac3d-0.0.40/offshoreflac3d/itasca_MonoBucket_Foundation.py
+-rw-rw-rw-   0        0        0     6699 2023-02-08 08:48:01.000000 offshoreflac3d-0.0.40/offshoreflac3d/itasca_MonoBucket_gmsh_basic_col.py
+-rw-rw-rw-   0        0        0     1964 2023-03-27 02:43:37.000000 offshoreflac3d-0.0.40/offshoreflac3d/itasca_MonoBucket_Initializing.py
+-rw-rw-rw-   0        0        0     3075 2023-03-27 03:02:03.000000 offshoreflac3d-0.0.40/offshoreflac3d/itasca_MonoBucket_Loading.py
+-rw-rw-rw-   0        0        0     3009 2023-03-27 02:43:30.000000 offshoreflac3d-0.0.40/offshoreflac3d/itasca_MonoBucket_Model.py
+-rw-rw-rw-   0        0        0     1829 2023-04-10 07:08:46.000000 offshoreflac3d-0.0.40/offshoreflac3d/itasca_RockSocketedPile_initial.py
+-rw-rw-rw-   0        0        0     7088 2023-04-10 07:08:46.000000 offshoreflac3d-0.0.40/offshoreflac3d/itasca_RockSocketedPile_loading.py
+-rw-rw-rw-   0        0        0     8650 2023-04-10 07:08:46.000000 offshoreflac3d-0.0.40/offshoreflac3d/itasca_RockSocketedPile_model.py
+-rw-rw-rw-   0        0        0     3801 2023-04-10 07:08:46.000000 offshoreflac3d-0.0.40/offshoreflac3d/itasca_RockSocketedPile_monopile.py
+-rw-rw-rw-   0        0        0       49 2022-12-16 03:10:27.000000 offshoreflac3d-0.0.40/offshoreflac3d/__ini__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 07:14:12.000000 offshoreflac3d-0.0.40/offshoreflac3d.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-10 07:14:12.000000 offshoreflac3d-0.0.40/offshoreflac3d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      239 2023-04-10 07:14:12.000000 offshoreflac3d-0.0.40/offshoreflac3d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      628 2023-04-10 07:14:12.000000 offshoreflac3d-0.0.40/offshoreflac3d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       15 2023-04-10 07:14:12.000000 offshoreflac3d-0.0.40/offshoreflac3d.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      239 2023-04-10 07:14:12.000000 offshoreflac3d-0.0.40/PKG-INFO
+-rw-rw-rw-   0        0        0      522 2022-12-16 08:40:25.000000 offshoreflac3d-0.0.40/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-10 07:14:12.000000 offshoreflac3d-0.0.40/setup.cfg
+-rw-rw-rw-   0        0        0      641 2023-04-10 07:11:32.000000 offshoreflac3d-0.0.40/setup.py
```

### Comparing `offshoreflac3d-0.0.33/offshoreflac3d/itasca_MonoBucket_Foundation.py` & `offshoreflac3d-0.0.40/offshoreflac3d/itasca_MonoBucket_Foundation.py`

 * *Files identical despite different names*

### Comparing `offshoreflac3d-0.0.33/offshoreflac3d/itasca_MonoBucket_gmsh_basic_col.py` & `offshoreflac3d-0.0.40/offshoreflac3d/itasca_MonoBucket_gmsh_basic_col.py`

 * *Files identical despite different names*

### Comparing `offshoreflac3d-0.0.33/offshoreflac3d/itasca_MonoBucket_Initializing.py` & `offshoreflac3d-0.0.40/offshoreflac3d/itasca_MonoBucket_Initializing.py`

 * *Files identical despite different names*

### Comparing `offshoreflac3d-0.0.33/offshoreflac3d/itasca_MonoBucket_Loading.py` & `offshoreflac3d-0.0.40/offshoreflac3d/itasca_MonoBucket_Loading.py`

 * *Files identical despite different names*

### Comparing `offshoreflac3d-0.0.33/offshoreflac3d/itasca_MonoBucket_Model.py` & `offshoreflac3d-0.0.40/offshoreflac3d/itasca_MonoBucket_Model.py`

 * *Files identical despite different names*

### Comparing `offshoreflac3d-0.0.33/offshoreflac3d.egg-info/SOURCES.txt` & `offshoreflac3d-0.0.40/offshoreflac3d.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 setup.py
 offshoreflac3d/__ini__.py
 offshoreflac3d/itasca_MonoBucket_Foundation.py
 offshoreflac3d/itasca_MonoBucket_Initializing.py
 offshoreflac3d/itasca_MonoBucket_Loading.py
 offshoreflac3d/itasca_MonoBucket_Model.py
 offshoreflac3d/itasca_MonoBucket_gmsh_basic_col.py
-offshoreflac3d/itasca_SBJackets_4.py
-offshoreflac3d/itasca_ini_rectangle.py
-offshoreflac3d/itasca_loading.py
-offshoreflac3d/itasca_model_rectangle.py
+offshoreflac3d/itasca_RockSocketedPile_initial.py
+offshoreflac3d/itasca_RockSocketedPile_loading.py
+offshoreflac3d/itasca_RockSocketedPile_model.py
+offshoreflac3d/itasca_RockSocketedPile_monopile.py
 offshoreflac3d.egg-info/PKG-INFO
 offshoreflac3d.egg-info/SOURCES.txt
 offshoreflac3d.egg-info/dependency_links.txt
 offshoreflac3d.egg-info/top_level.txt
```

### Comparing `offshoreflac3d-0.0.33/README.md` & `offshoreflac3d-0.0.40/README.md`

 * *Files identical despite different names*

### Comparing `offshoreflac3d-0.0.33/setup.py` & `offshoreflac3d-0.0.40/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # -*- coding:utf-8 -*-
 
 from distutils.core import  setup
 import setuptools
 packages = ['offshoreflac3d']# 唯一的包名，自己取名
 setup(name='offshoreflac3d',
-	version='0.0.33',
+	version='0.0.40',
 	author='Xiangming Ge',
 	packages=packages,
 	package_dir={'requests': 'requests'},)
 
 # from setuptools import setup, find_packages
 
 # setup(
```

