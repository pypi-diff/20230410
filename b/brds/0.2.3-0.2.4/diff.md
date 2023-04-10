# Comparing `tmp/brds-0.2.3.tar.gz` & `tmp/brds-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brds-0.2.3.tar", last modified: Mon Apr 10 21:10:59 2023, max compression
+gzip compressed data, was "brds-0.2.4.tar", last modified: Mon Apr 10 21:19:17 2023, max compression
```

## Comparing `brds-0.2.3.tar` & `brds-0.2.4.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:10:59.584359 brds-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-10 21:10:50.000000 brds-0.2.3/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-10 21:10:50.000000 brds-0.2.3/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-10 21:10:50.000000 brds-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 21:10:50.000000 brds-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 21:10:59.584359 brds-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-10 21:10:50.000000 brds-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:10:59.580359 brds-0.2.3/brds/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 21:10:50.000000 brds-0.2.3/brds/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-10 21:10:50.000000 brds-0.2.3/brds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-10 21:10:50.000000 brds-0.2.3/brds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-10 21:10:50.000000 brds-0.2.3/brds/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-10 21:10:50.000000 brds-0.2.3/brds/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-10 21:10:50.000000 brds-0.2.3/brds/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:10:59.580359 brds-0.2.3/brds/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-10 21:10:50.000000 brds-0.2.3/brds/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:10:59.580359 brds-0.2.3/brds/core/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-10 21:10:50.000000 brds-0.2.3/brds/core/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-10 21:10:50.000000 brds-0.2.3/brds/core/datasets/dataset_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-10 21:10:50.000000 brds-0.2.3/brds/core/datasets/dataset_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-10 21:10:50.000000 brds-0.2.3/brds/core/datasets/list_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-10 21:10:50.000000 brds-0.2.3/brds/core/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 21:10:50.000000 brds-0.2.3/brds/core/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:10:59.580359 brds-0.2.3/brds/core/fetch/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 21:10:50.000000 brds-0.2.3/brds/core/fetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-10 21:10:50.000000 brds-0.2.3/brds/core/fetch/fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:10:59.580359 brds-0.2.3/brds/core/fs/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-10 21:10:50.000000 brds-0.2.3/brds/core/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-10 21:10:50.000000 brds-0.2.3/brds/core/fs/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-10 21:10:50.000000 brds-0.2.3/brds/core/fs/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:10:59.580359 brds-0.2.3/brds/core/importer/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-10 21:10:50.000000 brds-0.2.3/brds/core/importer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-10 21:10:50.000000 brds-0.2.3/brds/core/importer/gunizp_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-10 21:10:50.000000 brds-0.2.3/brds/core/importer/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-10 21:10:50.000000 brds-0.2.3/brds/core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-10 21:10:50.000000 brds-0.2.3/brds/core/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:10:59.580359 brds-0.2.3/brds/humanize/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-10 21:10:50.000000 brds-0.2.3/brds/humanize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-10 21:10:50.000000 brds-0.2.3/brds/humanize/sizes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:10:59.580359 brds-0.2.3/brds/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-10 21:10:50.000000 brds-0.2.3/brds/templates/dataset_files.html
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-10 21:10:50.000000 brds-0.2.3/brds/templates/datasets.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:10:59.580359 brds-0.2.3/brds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 21:10:59.000000 brds-0.2.3/brds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-10 21:10:59.000000 brds-0.2.3/brds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 21:10:59.000000 brds-0.2.3/brds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-10 21:10:59.000000 brds-0.2.3/brds.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-10 21:10:59.000000 brds-0.2.3/brds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 21:10:59.000000 brds-0.2.3/brds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 21:10:59.584359 brds-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-10 21:10:50.000000 brds-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:10:59.580359 brds-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 21:10:50.000000 brds-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-10 21:10:50.000000 brds-0.2.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-10 21:10:50.000000 brds-0.2.3/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:19:17.958867 brds-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-10 21:19:09.000000 brds-0.2.4/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-10 21:19:09.000000 brds-0.2.4/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-10 21:19:09.000000 brds-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 21:19:09.000000 brds-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 21:19:17.958867 brds-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-10 21:19:09.000000 brds-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:19:17.954867 brds-0.2.4/brds/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 21:19:09.000000 brds-0.2.4/brds/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-10 21:19:09.000000 brds-0.2.4/brds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-10 21:19:09.000000 brds-0.2.4/brds/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-10 21:19:09.000000 brds-0.2.4/brds/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-10 21:19:09.000000 brds-0.2.4/brds/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-10 21:19:09.000000 brds-0.2.4/brds/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:19:17.954867 brds-0.2.4/brds/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-10 21:19:09.000000 brds-0.2.4/brds/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:19:17.954867 brds-0.2.4/brds/core/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-10 21:19:09.000000 brds-0.2.4/brds/core/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-10 21:19:09.000000 brds-0.2.4/brds/core/datasets/dataset_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-10 21:19:09.000000 brds-0.2.4/brds/core/datasets/dataset_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-10 21:19:09.000000 brds-0.2.4/brds/core/datasets/list_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-10 21:19:09.000000 brds-0.2.4/brds/core/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 21:19:09.000000 brds-0.2.4/brds/core/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:19:17.954867 brds-0.2.4/brds/core/fetch/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 21:19:09.000000 brds-0.2.4/brds/core/fetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-10 21:19:09.000000 brds-0.2.4/brds/core/fetch/fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:19:17.954867 brds-0.2.4/brds/core/fs/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-10 21:19:09.000000 brds-0.2.4/brds/core/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-10 21:19:09.000000 brds-0.2.4/brds/core/fs/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-10 21:19:09.000000 brds-0.2.4/brds/core/fs/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:19:17.958867 brds-0.2.4/brds/core/importer/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-10 21:19:09.000000 brds-0.2.4/brds/core/importer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-10 21:19:09.000000 brds-0.2.4/brds/core/importer/gunizp_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-10 21:19:09.000000 brds-0.2.4/brds/core/importer/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-10 21:19:09.000000 brds-0.2.4/brds/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-10 21:19:09.000000 brds-0.2.4/brds/core/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:19:17.958867 brds-0.2.4/brds/humanize/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-10 21:19:09.000000 brds-0.2.4/brds/humanize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-10 21:19:09.000000 brds-0.2.4/brds/humanize/sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 21:19:09.000000 brds-0.2.4/brds/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:19:17.958867 brds-0.2.4/brds/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-10 21:19:09.000000 brds-0.2.4/brds/templates/dataset_files.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-10 21:19:09.000000 brds-0.2.4/brds/templates/datasets.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:19:17.954867 brds-0.2.4/brds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 21:19:17.000000 brds-0.2.4/brds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-10 21:19:17.000000 brds-0.2.4/brds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 21:19:17.000000 brds-0.2.4/brds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-10 21:19:17.000000 brds-0.2.4/brds.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-10 21:19:17.000000 brds-0.2.4/brds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 21:19:17.000000 brds-0.2.4/brds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 21:19:17.958867 brds-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-10 21:19:09.000000 brds-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:19:17.958867 brds-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 21:19:09.000000 brds-0.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-10 21:19:09.000000 brds-0.2.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-10 21:19:09.000000 brds-0.2.4/tests/test_base.py
```

### Comparing `brds-0.2.3/HISTORY.md` & `brds-0.2.4/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Fixing packaging. [brahle]
+
+
+0.2.3 (2023-04-10)
+------------------
+- Release: version 0.2.3 🚀 [brahle]
 - Adding .typed file. [brahle]
 
 
 0.2.2 (2023-04-10)
 ------------------
 - Release: version 0.2.2 🚀 [brahle]
 - Exposing some additional items. [brahle]
```

### Comparing `brds-0.2.3/LICENSE` & `brds-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `brds-0.2.3/PKG-INFO` & `brds-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brds
-Version: 0.2.3
+Version: 0.2.4
 Summary: Awesome brds created by brahle
 Home-page: https://github.com/brahle/brds/
 Author: brahle
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `brds-0.2.3/brds/__init__.py` & `brds-0.2.4/brds/__init__.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.3/brds/app.py` & `brds-0.2.4/brds/app.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.3/brds/cli.py` & `brds-0.2.4/brds/cli.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.3/brds/core/__init__.py` & `brds-0.2.4/brds/core/__init__.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.3/brds/core/datasets/dataset_files.py` & `brds-0.2.4/brds/core/datasets/dataset_files.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.3/brds/core/datasets/dataset_info.py` & `brds-0.2.4/brds/core/datasets/dataset_info.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.3/brds/core/datasets/list_datasets.py` & `brds-0.2.4/brds/core/datasets/list_datasets.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.3/brds/core/edit.py` & `brds-0.2.4/brds/core/edit.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.3/brds/core/environment.py` & `brds-0.2.4/brds/core/environment.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.3/brds/core/fetch/fetcher.py` & `brds-0.2.4/brds/core/fetch/fetcher.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.3/brds/core/fs/reader.py` & `brds-0.2.4/brds/core/fs/reader.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.3/brds/core/fs/writer.py` & `brds-0.2.4/brds/core/fs/writer.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.3/brds/core/importer/gunizp_importer.py` & `brds-0.2.4/brds/core/importer/gunizp_importer.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.3/brds/core/logger.py` & `brds-0.2.4/brds/core/logger.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.3/brds/humanize/sizes.py` & `brds-0.2.4/brds/humanize/sizes.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.3/brds/templates/dataset_files.html` & `brds-0.2.4/brds/templates/dataset_files.html`

 * *Files identical despite different names*

### Comparing `brds-0.2.3/brds/templates/datasets.html` & `brds-0.2.4/brds/templates/datasets.html`

 * *Files identical despite different names*

### Comparing `brds-0.2.3/brds.egg-info/PKG-INFO` & `brds-0.2.4/brds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brds
-Version: 0.2.3
+Version: 0.2.4
 Summary: Awesome brds created by brahle
 Home-page: https://github.com/brahle/brds/
 Author: brahle
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `brds-0.2.3/brds.egg-info/SOURCES.txt` & `brds-0.2.4/brds.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 setup.py
 brds/VERSION
 brds/__init__.py
 brds/__main__.py
 brds/app.py
 brds/base.py
 brds/cli.py
+brds/py.typed
 brds.egg-info/PKG-INFO
 brds.egg-info/SOURCES.txt
 brds.egg-info/dependency_links.txt
 brds.egg-info/entry_points.txt
 brds.egg-info/requires.txt
 brds.egg-info/top_level.txt
 brds/core/__init__.py
```

### Comparing `brds-0.2.3/setup.py` & `brds-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,11 +39,11 @@
     author="brahle",
     packages=find_packages(exclude=["tests", ".github"]),
     install_requires=read_requirements("requirements.txt"),
     entry_points={
         "console_scripts": ["brds = brds.__main__:main"]
     },
     package_data={
-        'brds': ['brds/templates/**.html', "py.typed"],
+        'brds': ['templates/**.html', "py.typed"],
     },
     extras_require={"test": read_requirements("requirements-test.txt")},
 )
```

