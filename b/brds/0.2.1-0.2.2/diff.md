# Comparing `tmp/brds-0.2.1.tar.gz` & `tmp/brds-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brds-0.2.1.tar", last modified: Mon Apr 10 20:22:03 2023, max compression
+gzip compressed data, was "brds-0.2.2.tar", last modified: Mon Apr 10 20:54:37 2023, max compression
```

## Comparing `brds-0.2.1.tar` & `brds-0.2.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:22:03.732181 brds-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-10 20:21:49.000000 brds-0.2.1/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-10 20:21:49.000000 brds-0.2.1/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-10 20:21:49.000000 brds-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 20:21:49.000000 brds-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 20:22:03.728181 brds-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-10 20:21:49.000000 brds-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:22:03.724181 brds-0.2.1/brds/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 20:21:49.000000 brds-0.2.1/brds/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-10 20:21:49.000000 brds-0.2.1/brds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-10 20:21:49.000000 brds-0.2.1/brds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-10 20:21:49.000000 brds-0.2.1/brds/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-10 20:21:49.000000 brds-0.2.1/brds/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-10 20:21:49.000000 brds-0.2.1/brds/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:22:03.728181 brds-0.2.1/brds/core/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-10 20:21:49.000000 brds-0.2.1/brds/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:22:03.728181 brds-0.2.1/brds/core/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-10 20:21:49.000000 brds-0.2.1/brds/core/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-10 20:21:49.000000 brds-0.2.1/brds/core/datasets/dataset_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-10 20:21:49.000000 brds-0.2.1/brds/core/datasets/dataset_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-10 20:21:49.000000 brds-0.2.1/brds/core/datasets/list_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-10 20:21:49.000000 brds-0.2.1/brds/core/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 20:21:49.000000 brds-0.2.1/brds/core/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:22:03.728181 brds-0.2.1/brds/core/fetch/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 20:21:49.000000 brds-0.2.1/brds/core/fetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-10 20:21:49.000000 brds-0.2.1/brds/core/fetch/fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:22:03.728181 brds-0.2.1/brds/core/fs/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-10 20:21:49.000000 brds-0.2.1/brds/core/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-10 20:21:49.000000 brds-0.2.1/brds/core/fs/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-10 20:21:49.000000 brds-0.2.1/brds/core/fs/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:22:03.728181 brds-0.2.1/brds/core/importer/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-10 20:21:49.000000 brds-0.2.1/brds/core/importer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-10 20:21:49.000000 brds-0.2.1/brds/core/importer/gunizp_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-10 20:21:49.000000 brds-0.2.1/brds/core/importer/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-10 20:21:49.000000 brds-0.2.1/brds/core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-10 20:21:49.000000 brds-0.2.1/brds/core/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:22:03.728181 brds-0.2.1/brds/humanize/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-10 20:21:49.000000 brds-0.2.1/brds/humanize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-10 20:21:49.000000 brds-0.2.1/brds/humanize/sizes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:22:03.728181 brds-0.2.1/brds/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-10 20:21:49.000000 brds-0.2.1/brds/templates/dataset_files.html
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-10 20:21:49.000000 brds-0.2.1/brds/templates/datasets.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:22:03.728181 brds-0.2.1/brds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 20:22:03.000000 brds-0.2.1/brds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-10 20:22:03.000000 brds-0.2.1/brds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:22:03.000000 brds-0.2.1/brds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-10 20:22:03.000000 brds-0.2.1/brds.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-10 20:22:03.000000 brds-0.2.1/brds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 20:22:03.000000 brds-0.2.1/brds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 20:22:03.732181 brds-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-10 20:21:49.000000 brds-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:22:03.728181 brds-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:21:49.000000 brds-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-10 20:21:49.000000 brds-0.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-10 20:21:49.000000 brds-0.2.1/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:54:37.719099 brds-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-10 20:54:29.000000 brds-0.2.2/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-10 20:54:29.000000 brds-0.2.2/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-10 20:54:29.000000 brds-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 20:54:29.000000 brds-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 20:54:37.719099 brds-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-10 20:54:29.000000 brds-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:54:37.719099 brds-0.2.2/brds/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 20:54:29.000000 brds-0.2.2/brds/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-10 20:54:29.000000 brds-0.2.2/brds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-10 20:54:29.000000 brds-0.2.2/brds/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-10 20:54:29.000000 brds-0.2.2/brds/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-10 20:54:29.000000 brds-0.2.2/brds/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-10 20:54:29.000000 brds-0.2.2/brds/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:54:37.719099 brds-0.2.2/brds/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-10 20:54:29.000000 brds-0.2.2/brds/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:54:37.719099 brds-0.2.2/brds/core/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-10 20:54:29.000000 brds-0.2.2/brds/core/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-10 20:54:29.000000 brds-0.2.2/brds/core/datasets/dataset_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-10 20:54:29.000000 brds-0.2.2/brds/core/datasets/dataset_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-10 20:54:29.000000 brds-0.2.2/brds/core/datasets/list_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-10 20:54:29.000000 brds-0.2.2/brds/core/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 20:54:29.000000 brds-0.2.2/brds/core/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:54:37.719099 brds-0.2.2/brds/core/fetch/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 20:54:29.000000 brds-0.2.2/brds/core/fetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-10 20:54:29.000000 brds-0.2.2/brds/core/fetch/fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:54:37.719099 brds-0.2.2/brds/core/fs/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-10 20:54:29.000000 brds-0.2.2/brds/core/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-10 20:54:29.000000 brds-0.2.2/brds/core/fs/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-10 20:54:29.000000 brds-0.2.2/brds/core/fs/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:54:37.719099 brds-0.2.2/brds/core/importer/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-10 20:54:29.000000 brds-0.2.2/brds/core/importer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-10 20:54:29.000000 brds-0.2.2/brds/core/importer/gunizp_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-10 20:54:29.000000 brds-0.2.2/brds/core/importer/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-10 20:54:29.000000 brds-0.2.2/brds/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-10 20:54:29.000000 brds-0.2.2/brds/core/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:54:37.719099 brds-0.2.2/brds/humanize/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-10 20:54:29.000000 brds-0.2.2/brds/humanize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-10 20:54:29.000000 brds-0.2.2/brds/humanize/sizes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:54:37.719099 brds-0.2.2/brds/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-10 20:54:29.000000 brds-0.2.2/brds/templates/dataset_files.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-10 20:54:29.000000 brds-0.2.2/brds/templates/datasets.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:54:37.719099 brds-0.2.2/brds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 20:54:37.000000 brds-0.2.2/brds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-10 20:54:37.000000 brds-0.2.2/brds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:54:37.000000 brds-0.2.2/brds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-10 20:54:37.000000 brds-0.2.2/brds.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-10 20:54:37.000000 brds-0.2.2/brds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 20:54:37.000000 brds-0.2.2/brds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 20:54:37.719099 brds-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-10 20:54:29.000000 brds-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:54:37.719099 brds-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:54:29.000000 brds-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-10 20:54:29.000000 brds-0.2.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-10 20:54:29.000000 brds-0.2.2/tests/test_base.py
```

### Comparing `brds-0.2.1/HISTORY.md` & `brds-0.2.2/HISTORY.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Exposing some additional items. [brahle]
+
+
+0.2.1 (2023-04-10)
+------------------
+- Release: version 0.2.1 🚀 [brahle]
 - Fixing the formatting. [brahle]
 
 
 0.2.0 (2023-04-10)
 ------------------
 - Release: version 0.2.0 🚀 [brahle]
 - Edit (#7) [Bruno Rahle]
```

### Comparing `brds-0.2.1/LICENSE` & `brds-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `brds-0.2.1/PKG-INFO` & `brds-0.2.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brds
-Version: 0.2.1
+Version: 0.2.2
 Summary: Awesome brds created by brahle
 Home-page: https://github.com/brahle/brds/
 Author: brahle
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `brds-0.2.1/brds/__init__.py` & `brds-0.2.2/brds/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from .core import (
     DatasetInfo,
+    ExactMatch,
     Fetcher,
     FileReader,
     FileWriter,
+    FindCallBack,
     GunzipImporter,
     Importer,
+    Replacement,
     Vault,
     find,
     find_and_replace,
     find_and_replacer,
     finder,
     fload,
     get_dataset_files,
@@ -23,29 +26,32 @@
     set_logging_to_warn,
     vault_token,
     writer_folder_path,
 )
 
 __all__ = [
     "DatasetInfo",
+    "ExactMatch",
     "Fetcher",
     "FileReader",
     "FileWriter",
     "find_and_replace",
     "find_and_replacer",
     "find",
+    "FindCallBack",
     "finder",
     "fload",
     "get_dataset_files",
     "get_logger",
     "GunzipImporter",
     "Importer",
     "list_datasets",
     "reader_folder_path",
     "replace",
+    "Replacement",
     "replacer",
     "root_folder_path",
     "set_logging_to_debug",
     "set_logging_to_info",
     "set_logging_to_warn",
     "vault_token",
     "Vault",
```

### Comparing `brds-0.2.1/brds/app.py` & `brds-0.2.2/brds/app.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.1/brds/cli.py` & `brds-0.2.2/brds/cli.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.1/brds/core/__init__.py` & `brds-0.2.2/brds/core/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 from .datasets import DatasetInfo, get_dataset_files, list_datasets
-from .edit import find, find_and_replace, find_and_replacer, finder, replace, replacer
+from .edit import (
+    ExactMatch,
+    FindCallBack,
+    Replacement,
+    find,
+    find_and_replace,
+    find_and_replacer,
+    finder,
+    replace,
+    replacer,
+)
 from .environment import reader_folder_path, root_folder_path, vault_token, writer_folder_path
 from .fetch import Fetcher
 from .fs import FileReader, FileWriter, fload
 from .importer import GunzipImporter, Importer
 from .logger import get_logger, set_logging_to_debug, set_logging_to_info, set_logging_to_warn
 from .vault import Vault
 
 __all__ = [
     "DatasetInfo",
+    "ExactMatch",
     "Fetcher",
     "FileReader",
     "FileWriter",
     "find_and_replace",
     "find_and_replacer",
     "find",
+    "FindCallBack",
     "finder",
     "fload",
     "get_dataset_files",
     "get_logger",
     "GunzipImporter",
     "Importer",
     "list_datasets",
     "reader_folder_path",
     "replace",
+    "Replacement",
     "replacer",
     "root_folder_path",
     "set_logging_to_debug",
     "set_logging_to_info",
     "set_logging_to_warn",
     "vault_token",
     "Vault",
```

### Comparing `brds-0.2.1/brds/core/datasets/dataset_files.py` & `brds-0.2.2/brds/core/datasets/dataset_files.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.1/brds/core/datasets/dataset_info.py` & `brds-0.2.2/brds/core/datasets/dataset_info.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.1/brds/core/datasets/list_datasets.py` & `brds-0.2.2/brds/core/datasets/list_datasets.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.1/brds/core/edit.py` & `brds-0.2.2/brds/core/edit.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.1/brds/core/environment.py` & `brds-0.2.2/brds/core/environment.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.1/brds/core/fetch/fetcher.py` & `brds-0.2.2/brds/core/fetch/fetcher.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.1/brds/core/fs/reader.py` & `brds-0.2.2/brds/core/fs/reader.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.1/brds/core/fs/writer.py` & `brds-0.2.2/brds/core/fs/writer.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.1/brds/core/importer/gunizp_importer.py` & `brds-0.2.2/brds/core/importer/gunizp_importer.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.1/brds/core/logger.py` & `brds-0.2.2/brds/core/logger.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.1/brds/humanize/sizes.py` & `brds-0.2.2/brds/humanize/sizes.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.1/brds/templates/dataset_files.html` & `brds-0.2.2/brds/templates/dataset_files.html`

 * *Files identical despite different names*

### Comparing `brds-0.2.1/brds/templates/datasets.html` & `brds-0.2.2/brds/templates/datasets.html`

 * *Files identical despite different names*

### Comparing `brds-0.2.1/brds.egg-info/PKG-INFO` & `brds-0.2.2/brds.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brds
-Version: 0.2.1
+Version: 0.2.2
 Summary: Awesome brds created by brahle
 Home-page: https://github.com/brahle/brds/
 Author: brahle
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `brds-0.2.1/brds.egg-info/SOURCES.txt` & `brds-0.2.2/brds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brds-0.2.1/setup.py` & `brds-0.2.2/setup.py`

 * *Files identical despite different names*

