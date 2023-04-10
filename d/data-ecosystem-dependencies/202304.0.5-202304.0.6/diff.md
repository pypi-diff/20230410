# Comparing `tmp/data_ecosystem_dependencies-202304.0.5.tar.gz` & `tmp/data_ecosystem_dependencies-202304.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_dependencies-202304.0.5.tar", max compression
+gzip compressed data, was "data_ecosystem_dependencies-202304.0.6.tar", max compression
```

## Comparing `data_ecosystem_dependencies-202304.0.5.tar` & `data_ecosystem_dependencies-202304.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      842 2023-04-10 16:14:11.365289 data_ecosystem_dependencies-202304.0.5/data_ecosystem_dependencies/__init__.py
--rw-r--r--   0        0        0    11357 2023-04-10 16:14:11.365289 data_ecosystem_dependencies-202304.0.5/license.md
--rw-r--r--   0        0        0     2541 2023-04-10 16:18:34.853398 data_ecosystem_dependencies-202304.0.5/pyproject.toml
--rw-r--r--   0        0        0      341 2023-04-10 16:14:11.365289 data_ecosystem_dependencies-202304.0.5/readme.md
--rw-r--r--   0        0        0      160 2023-04-10 16:14:11.365289 data_ecosystem_dependencies-202304.0.5/setup.cfg
--rw-r--r--   0        0        0     3050 1970-01-01 00:00:00.000000 data_ecosystem_dependencies-202304.0.5/PKG-INFO
+-rw-r--r--   0        0        0      842 2023-04-10 17:10:57.559512 data_ecosystem_dependencies-202304.0.6/data_ecosystem_dependencies/__init__.py
+-rw-r--r--   0        0        0    11357 2023-04-10 17:10:57.559512 data_ecosystem_dependencies-202304.0.6/license.md
+-rw-r--r--   0        0        0     2541 2023-04-10 17:15:40.473935 data_ecosystem_dependencies-202304.0.6/pyproject.toml
+-rw-r--r--   0        0        0      341 2023-04-10 17:10:57.559512 data_ecosystem_dependencies-202304.0.6/readme.md
+-rw-r--r--   0        0        0      160 2023-04-10 17:10:57.559512 data_ecosystem_dependencies-202304.0.6/setup.cfg
+-rw-r--r--   0        0        0     3050 1970-01-01 00:00:00.000000 data_ecosystem_dependencies-202304.0.6/PKG-INFO
```

### Comparing `data_ecosystem_dependencies-202304.0.5/data_ecosystem_dependencies/__init__.py` & `data_ecosystem_dependencies-202304.0.6/data_ecosystem_dependencies/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_dependencies-202304.0.5/license.md` & `data_ecosystem_dependencies-202304.0.6/license.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_dependencies-202304.0.5/pyproject.toml` & `data_ecosystem_dependencies-202304.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name="data_ecosystem_dependencies"
-version="202304.0.5"
+version="202304.0.6"
 description="Data Ecosystem  Dependencies - Python (PADE)"
 authors=["John Bowyer <zfi4@cdc.gov>"]
 readme = "readme.md"
 license="Apache"
 homepage="https://github.com/cdcent/data_ecosystem_services"
 repository="https://github.com/cdcent/data_ecosystem_services"
 classifiers=[
```

### Comparing `data_ecosystem_dependencies-202304.0.5/PKG-INFO` & `data_ecosystem_dependencies-202304.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-dependencies
-Version: 202304.0.5
+Version: 202304.0.6
 Summary: Data Ecosystem  Dependencies - Python (PADE)
 Home-page: https://github.com/cdcent/data_ecosystem_services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

