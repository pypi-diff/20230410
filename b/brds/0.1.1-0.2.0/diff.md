# Comparing `tmp/brds-0.1.1.tar.gz` & `tmp/brds-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brds-0.1.1.tar", last modified: Mon Apr 10 19:51:25 2023, max compression
+gzip compressed data, was "brds-0.2.0.tar", last modified: Mon Apr 10 20:18:14 2023, max compression
```

## Comparing `brds-0.1.1.tar` & `brds-0.2.0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:51:25.598150 brds-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-10 19:51:17.000000 brds-0.1.1/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-10 19:51:17.000000 brds-0.1.1/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-10 19:51:17.000000 brds-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 19:51:17.000000 brds-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 19:51:25.598150 brds-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-10 19:51:17.000000 brds-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:51:25.598150 brds-0.1.1/brds/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 19:51:17.000000 brds-0.1.1/brds/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-10 19:51:17.000000 brds-0.1.1/brds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-10 19:51:17.000000 brds-0.1.1/brds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-10 19:51:17.000000 brds-0.1.1/brds/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-10 19:51:17.000000 brds-0.1.1/brds/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-10 19:51:17.000000 brds-0.1.1/brds/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:51:25.598150 brds-0.1.1/brds/core/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:51:25.598150 brds-0.1.1/brds/core/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/datasets/dataset_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/datasets/dataset_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/datasets/list_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:51:25.598150 brds-0.1.1/brds/core/fetch/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/fetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/fetch/fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:51:25.598150 brds-0.1.1/brds/core/fs/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/fs/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/fs/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:51:25.598150 brds-0.1.1/brds/core/importer/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/importer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/importer/gunizp_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/importer/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:51:25.598150 brds-0.1.1/brds/humanize/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-10 19:51:17.000000 brds-0.1.1/brds/humanize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-10 19:51:17.000000 brds-0.1.1/brds/humanize/sizes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:51:25.598150 brds-0.1.1/brds/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-10 19:51:17.000000 brds-0.1.1/brds/templates/dataset_files.html
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-10 19:51:17.000000 brds-0.1.1/brds/templates/datasets.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:51:25.598150 brds-0.1.1/brds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 19:51:25.000000 brds-0.1.1/brds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-10 19:51:25.000000 brds-0.1.1/brds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:51:25.000000 brds-0.1.1/brds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-10 19:51:25.000000 brds-0.1.1/brds.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-10 19:51:25.000000 brds-0.1.1/brds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 19:51:25.000000 brds-0.1.1/brds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 19:51:25.598150 brds-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-10 19:51:17.000000 brds-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:51:25.598150 brds-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:51:17.000000 brds-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-10 19:51:17.000000 brds-0.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-10 19:51:17.000000 brds-0.1.1/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:18:14.306506 brds-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-10 20:18:03.000000 brds-0.2.0/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-10 20:18:03.000000 brds-0.2.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-10 20:18:03.000000 brds-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 20:18:03.000000 brds-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 20:18:14.306506 brds-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-10 20:18:03.000000 brds-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:18:14.306506 brds-0.2.0/brds/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 20:18:03.000000 brds-0.2.0/brds/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-10 20:18:03.000000 brds-0.2.0/brds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-10 20:18:03.000000 brds-0.2.0/brds/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-10 20:18:03.000000 brds-0.2.0/brds/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-10 20:18:03.000000 brds-0.2.0/brds/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-10 20:18:03.000000 brds-0.2.0/brds/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:18:14.306506 brds-0.2.0/brds/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-10 20:18:03.000000 brds-0.2.0/brds/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:18:14.306506 brds-0.2.0/brds/core/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-10 20:18:03.000000 brds-0.2.0/brds/core/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-10 20:18:03.000000 brds-0.2.0/brds/core/datasets/dataset_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-10 20:18:03.000000 brds-0.2.0/brds/core/datasets/dataset_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-10 20:18:03.000000 brds-0.2.0/brds/core/datasets/list_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-10 20:18:03.000000 brds-0.2.0/brds/core/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 20:18:03.000000 brds-0.2.0/brds/core/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:18:14.306506 brds-0.2.0/brds/core/fetch/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 20:18:03.000000 brds-0.2.0/brds/core/fetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-10 20:18:03.000000 brds-0.2.0/brds/core/fetch/fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:18:14.306506 brds-0.2.0/brds/core/fs/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-10 20:18:03.000000 brds-0.2.0/brds/core/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-10 20:18:03.000000 brds-0.2.0/brds/core/fs/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-10 20:18:03.000000 brds-0.2.0/brds/core/fs/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:18:14.306506 brds-0.2.0/brds/core/importer/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-10 20:18:03.000000 brds-0.2.0/brds/core/importer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-10 20:18:03.000000 brds-0.2.0/brds/core/importer/gunizp_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-10 20:18:03.000000 brds-0.2.0/brds/core/importer/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-10 20:18:03.000000 brds-0.2.0/brds/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-10 20:18:03.000000 brds-0.2.0/brds/core/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:18:14.306506 brds-0.2.0/brds/humanize/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-10 20:18:03.000000 brds-0.2.0/brds/humanize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-10 20:18:03.000000 brds-0.2.0/brds/humanize/sizes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:18:14.306506 brds-0.2.0/brds/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-10 20:18:03.000000 brds-0.2.0/brds/templates/dataset_files.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-10 20:18:03.000000 brds-0.2.0/brds/templates/datasets.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:18:14.306506 brds-0.2.0/brds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 20:18:14.000000 brds-0.2.0/brds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-10 20:18:14.000000 brds-0.2.0/brds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:18:14.000000 brds-0.2.0/brds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-10 20:18:14.000000 brds-0.2.0/brds.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-10 20:18:14.000000 brds-0.2.0/brds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 20:18:14.000000 brds-0.2.0/brds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 20:18:14.306506 brds-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-10 20:18:03.000000 brds-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:18:14.306506 brds-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:18:03.000000 brds-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-10 20:18:03.000000 brds-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-10 20:18:03.000000 brds-0.2.0/tests/test_base.py
```

### Comparing `brds-0.1.1/HISTORY.md` & `brds-0.2.0/HISTORY.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Edit (#7) [Bruno Rahle]
+
+
+0.1.1 (2023-04-10)
+------------------
+- Release: version 0.1.1 🚀 [brahle]
 - Release: version 0.1.0 🚀 [brahle]
 - Merge branch 'main' of github.com:brahle/brds into main. [brahle]
 - Br/updates (#6) [Bruno Rahle]
 
   * Adding FastAPI app to show the datasets
 
   * Updates to the container
```

### Comparing `brds-0.1.1/LICENSE` & `brds-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `brds-0.1.1/PKG-INFO` & `brds-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brds
-Version: 0.1.1
+Version: 0.2.0
 Summary: Awesome brds created by brahle
 Home-page: https://github.com/brahle/brds/
 Author: brahle
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `brds-0.1.1/brds/app.py` & `brds-0.2.0/brds/app.py`

 * *Files identical despite different names*

### Comparing `brds-0.1.1/brds/cli.py` & `brds-0.2.0/brds/cli.py`

 * *Files identical despite different names*

### Comparing `brds-0.1.1/brds/core/__init__.py` & `brds-0.2.0/brds/core/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 from .datasets import DatasetInfo, get_dataset_files, list_datasets
+from .edit import find, finder, replace, replacer, find_and_replace, find_and_replacer
 from .environment import reader_folder_path, root_folder_path, vault_token, writer_folder_path
 from .fetch import Fetcher
 from .fs import FileReader, FileWriter, fload
 from .importer import GunzipImporter, Importer
 from .logger import get_logger, set_logging_to_debug, set_logging_to_info, set_logging_to_warn
 from .vault import Vault
 
 __all__ = [
     "DatasetInfo",
     "Fetcher",
     "FileReader",
     "FileWriter",
+    "find_and_replace",
+    "find_and_replacer",
+    "find",
+    "finder",
     "fload",
     "get_dataset_files",
     "get_logger",
     "GunzipImporter",
     "Importer",
     "list_datasets",
     "reader_folder_path",
+    "replace",
+    "replacer",
     "root_folder_path",
     "set_logging_to_debug",
     "set_logging_to_info",
     "set_logging_to_warn",
-    "Vault",
     "vault_token",
+    "Vault",
     "writer_folder_path",
 ]
```

### Comparing `brds-0.1.1/brds/core/datasets/dataset_files.py` & `brds-0.2.0/brds/core/datasets/dataset_files.py`

 * *Files identical despite different names*

### Comparing `brds-0.1.1/brds/core/datasets/dataset_info.py` & `brds-0.2.0/brds/core/datasets/dataset_info.py`

 * *Files identical despite different names*

### Comparing `brds-0.1.1/brds/core/datasets/list_datasets.py` & `brds-0.2.0/brds/core/datasets/list_datasets.py`

 * *Files identical despite different names*

### Comparing `brds-0.1.1/brds/core/environment.py` & `brds-0.2.0/brds/core/environment.py`

 * *Files identical despite different names*

### Comparing `brds-0.1.1/brds/core/fetch/fetcher.py` & `brds-0.2.0/brds/core/fetch/fetcher.py`

 * *Files identical despite different names*

### Comparing `brds-0.1.1/brds/core/fs/reader.py` & `brds-0.2.0/brds/core/fs/reader.py`

 * *Files identical despite different names*

### Comparing `brds-0.1.1/brds/core/fs/writer.py` & `brds-0.2.0/brds/core/fs/writer.py`

 * *Files identical despite different names*

### Comparing `brds-0.1.1/brds/core/importer/gunizp_importer.py` & `brds-0.2.0/brds/core/importer/gunizp_importer.py`

 * *Files identical despite different names*

### Comparing `brds-0.1.1/brds/core/logger.py` & `brds-0.2.0/brds/core/logger.py`

 * *Files identical despite different names*

### Comparing `brds-0.1.1/brds/humanize/sizes.py` & `brds-0.2.0/brds/humanize/sizes.py`

 * *Files identical despite different names*

### Comparing `brds-0.1.1/brds/templates/dataset_files.html` & `brds-0.2.0/brds/templates/dataset_files.html`

 * *Files identical despite different names*

### Comparing `brds-0.1.1/brds/templates/datasets.html` & `brds-0.2.0/brds/templates/datasets.html`

 * *Files identical despite different names*

### Comparing `brds-0.1.1/brds.egg-info/PKG-INFO` & `brds-0.2.0/brds.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brds
-Version: 0.1.1
+Version: 0.2.0
 Summary: Awesome brds created by brahle
 Home-page: https://github.com/brahle/brds/
 Author: brahle
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `brds-0.1.1/brds.egg-info/SOURCES.txt` & `brds-0.2.0/brds.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 brds.egg-info/PKG-INFO
 brds.egg-info/SOURCES.txt
 brds.egg-info/dependency_links.txt
 brds.egg-info/entry_points.txt
 brds.egg-info/requires.txt
 brds.egg-info/top_level.txt
 brds/core/__init__.py
+brds/core/edit.py
 brds/core/environment.py
 brds/core/logger.py
 brds/core/vault.py
 brds/core/datasets/__init__.py
 brds/core/datasets/dataset_files.py
 brds/core/datasets/dataset_info.py
 brds/core/datasets/list_datasets.py
```

### Comparing `brds-0.1.1/setup.py` & `brds-0.2.0/setup.py`

 * *Files identical despite different names*

