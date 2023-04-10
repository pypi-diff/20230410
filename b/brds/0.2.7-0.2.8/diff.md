# Comparing `tmp/brds-0.2.7.tar.gz` & `tmp/brds-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brds-0.2.7.tar", last modified: Mon Apr 10 21:53:27 2023, max compression
+gzip compressed data, was "brds-0.2.8.tar", last modified: Mon Apr 10 21:58:53 2023, max compression
```

## Comparing `brds-0.2.7.tar` & `brds-0.2.8.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:53:27.308915 brds-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-10 21:53:15.000000 brds-0.2.7/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-10 21:53:15.000000 brds-0.2.7/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-10 21:53:15.000000 brds-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 21:53:15.000000 brds-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 21:53:27.308915 brds-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-10 21:53:15.000000 brds-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:53:27.304915 brds-0.2.7/brds/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 21:53:15.000000 brds-0.2.7/brds/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-10 21:53:15.000000 brds-0.2.7/brds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-10 21:53:15.000000 brds-0.2.7/brds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-10 21:53:15.000000 brds-0.2.7/brds/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-10 21:53:15.000000 brds-0.2.7/brds/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-10 21:53:15.000000 brds-0.2.7/brds/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:53:27.304915 brds-0.2.7/brds/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-10 21:53:15.000000 brds-0.2.7/brds/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:53:27.304915 brds-0.2.7/brds/core/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-10 21:53:15.000000 brds-0.2.7/brds/core/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-10 21:53:15.000000 brds-0.2.7/brds/core/datasets/dataset_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-10 21:53:15.000000 brds-0.2.7/brds/core/datasets/dataset_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-10 21:53:15.000000 brds-0.2.7/brds/core/datasets/list_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-10 21:53:15.000000 brds-0.2.7/brds/core/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 21:53:15.000000 brds-0.2.7/brds/core/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:53:27.304915 brds-0.2.7/brds/core/fetch/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 21:53:15.000000 brds-0.2.7/brds/core/fetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-10 21:53:15.000000 brds-0.2.7/brds/core/fetch/fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:53:27.304915 brds-0.2.7/brds/core/fs/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-10 21:53:15.000000 brds-0.2.7/brds/core/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-10 21:53:15.000000 brds-0.2.7/brds/core/fs/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-10 21:53:15.000000 brds-0.2.7/brds/core/fs/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:53:27.304915 brds-0.2.7/brds/core/importer/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-10 21:53:15.000000 brds-0.2.7/brds/core/importer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-10 21:53:15.000000 brds-0.2.7/brds/core/importer/gunizp_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-10 21:53:15.000000 brds-0.2.7/brds/core/importer/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-10 21:53:15.000000 brds-0.2.7/brds/core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-10 21:53:15.000000 brds-0.2.7/brds/core/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:53:27.308915 brds-0.2.7/brds/humanize/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-10 21:53:15.000000 brds-0.2.7/brds/humanize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-10 21:53:15.000000 brds-0.2.7/brds/humanize/sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 21:53:15.000000 brds-0.2.7/brds/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:53:27.308915 brds-0.2.7/brds/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-10 21:53:15.000000 brds-0.2.7/brds/templates/dataset_files.html
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-10 21:53:15.000000 brds-0.2.7/brds/templates/datasets.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:53:27.304915 brds-0.2.7/brds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 21:53:27.000000 brds-0.2.7/brds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-10 21:53:27.000000 brds-0.2.7/brds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 21:53:27.000000 brds-0.2.7/brds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-10 21:53:27.000000 brds-0.2.7/brds.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-10 21:53:27.000000 brds-0.2.7/brds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 21:53:27.000000 brds-0.2.7/brds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 21:53:27.308915 brds-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-10 21:53:15.000000 brds-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:53:27.308915 brds-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 21:53:15.000000 brds-0.2.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-10 21:53:15.000000 brds-0.2.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-10 21:53:15.000000 brds-0.2.7/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:53.191722 brds-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-10 21:58:43.000000 brds-0.2.8/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-10 21:58:43.000000 brds-0.2.8/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-10 21:58:43.000000 brds-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 21:58:43.000000 brds-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 21:58:53.191722 brds-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-10 21:58:43.000000 brds-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:53.187722 brds-0.2.8/brds/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 21:58:43.000000 brds-0.2.8/brds/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-10 21:58:43.000000 brds-0.2.8/brds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-10 21:58:43.000000 brds-0.2.8/brds/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-10 21:58:43.000000 brds-0.2.8/brds/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-10 21:58:43.000000 brds-0.2.8/brds/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-10 21:58:43.000000 brds-0.2.8/brds/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:53.187722 brds-0.2.8/brds/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:53.187722 brds-0.2.8/brds/core/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/datasets/dataset_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/datasets/dataset_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/datasets/list_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:53.191722 brds-0.2.8/brds/core/fetch/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/fetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/fetch/fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:53.191722 brds-0.2.8/brds/core/fs/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/fs/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/fs/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:53.191722 brds-0.2.8/brds/core/importer/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/importer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/importer/gunizp_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/importer/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:53.191722 brds-0.2.8/brds/humanize/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-10 21:58:43.000000 brds-0.2.8/brds/humanize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-10 21:58:43.000000 brds-0.2.8/brds/humanize/sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:43.000000 brds-0.2.8/brds/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:53.191722 brds-0.2.8/brds/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-10 21:58:43.000000 brds-0.2.8/brds/templates/dataset_files.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-10 21:58:43.000000 brds-0.2.8/brds/templates/datasets.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:53.187722 brds-0.2.8/brds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 21:58:53.000000 brds-0.2.8/brds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-10 21:58:53.000000 brds-0.2.8/brds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 21:58:53.000000 brds-0.2.8/brds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-10 21:58:53.000000 brds-0.2.8/brds.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-10 21:58:53.000000 brds-0.2.8/brds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 21:58:53.000000 brds-0.2.8/brds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 21:58:53.191722 brds-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-10 21:58:43.000000 brds-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:53.191722 brds-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:43.000000 brds-0.2.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-10 21:58:43.000000 brds-0.2.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-10 21:58:43.000000 brds-0.2.8/tests/test_base.py
```

### Comparing `brds-0.2.7/HISTORY.md` & `brds-0.2.8/HISTORY.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Also tagging the version from the ref. [brahle]
+
+
+0.2.7 (2023-04-10)
+------------------
+- Release: version 0.2.7 🚀 [brahle]
 - Fixing the publishing. [brahle]
 
 
 0.2.6 (2023-04-10)
 ------------------
 - Release: version 0.2.6 🚀 [brahle]
 - Fixing return types. [brahle]
```

### Comparing `brds-0.2.7/LICENSE` & `brds-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `brds-0.2.7/PKG-INFO` & `brds-0.2.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brds
-Version: 0.2.7
+Version: 0.2.8
 Summary: Awesome brds created by brahle
 Home-page: https://github.com/brahle/brds/
 Author: brahle
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `brds-0.2.7/brds/__init__.py` & `brds-0.2.8/brds/__init__.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.7/brds/app.py` & `brds-0.2.8/brds/app.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.7/brds/cli.py` & `brds-0.2.8/brds/cli.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.7/brds/core/__init__.py` & `brds-0.2.8/brds/core/__init__.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.7/brds/core/datasets/dataset_files.py` & `brds-0.2.8/brds/core/datasets/dataset_files.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.7/brds/core/datasets/dataset_info.py` & `brds-0.2.8/brds/core/datasets/dataset_info.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.7/brds/core/datasets/list_datasets.py` & `brds-0.2.8/brds/core/datasets/list_datasets.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.7/brds/core/edit.py` & `brds-0.2.8/brds/core/edit.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.7/brds/core/environment.py` & `brds-0.2.8/brds/core/environment.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.7/brds/core/fetch/fetcher.py` & `brds-0.2.8/brds/core/fetch/fetcher.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.7/brds/core/fs/reader.py` & `brds-0.2.8/brds/core/fs/reader.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.7/brds/core/fs/writer.py` & `brds-0.2.8/brds/core/fs/writer.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.7/brds/core/importer/gunizp_importer.py` & `brds-0.2.8/brds/core/importer/gunizp_importer.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.7/brds/core/logger.py` & `brds-0.2.8/brds/core/logger.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.7/brds/humanize/sizes.py` & `brds-0.2.8/brds/humanize/sizes.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.7/brds/templates/dataset_files.html` & `brds-0.2.8/brds/templates/dataset_files.html`

 * *Files identical despite different names*

### Comparing `brds-0.2.7/brds/templates/datasets.html` & `brds-0.2.8/brds/templates/datasets.html`

 * *Files identical despite different names*

### Comparing `brds-0.2.7/brds.egg-info/PKG-INFO` & `brds-0.2.8/brds.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brds
-Version: 0.2.7
+Version: 0.2.8
 Summary: Awesome brds created by brahle
 Home-page: https://github.com/brahle/brds/
 Author: brahle
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `brds-0.2.7/brds.egg-info/SOURCES.txt` & `brds-0.2.8/brds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brds-0.2.7/setup.py` & `brds-0.2.8/setup.py`

 * *Files identical despite different names*

