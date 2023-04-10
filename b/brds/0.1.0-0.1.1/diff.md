# Comparing `tmp/brds-0.1.0.tar.gz` & `tmp/brds-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brds-0.1.0.tar", last modified: Mon Apr 10 19:48:49 2023, max compression
+gzip compressed data, was "brds-0.1.1.tar", last modified: Mon Apr 10 19:51:25 2023, max compression
```

## Comparing `brds-0.1.0.tar` & `brds-0.1.1.tar`

### file list

```diff
@@ -1,42 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:48:49.989295 brds-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-10 19:48:37.000000 brds-0.1.0/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-10 19:48:37.000000 brds-0.1.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-10 19:48:37.000000 brds-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 19:48:37.000000 brds-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 19:48:49.989295 brds-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-10 19:48:37.000000 brds-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:48:49.989295 brds-0.1.0/brds/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 19:48:37.000000 brds-0.1.0/brds/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-10 19:48:37.000000 brds-0.1.0/brds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-10 19:48:37.000000 brds-0.1.0/brds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-10 19:48:37.000000 brds-0.1.0/brds/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-10 19:48:37.000000 brds-0.1.0/brds/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:48:49.989295 brds-0.1.0/brds/core/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-10 19:48:37.000000 brds-0.1.0/brds/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-10 19:48:37.000000 brds-0.1.0/brds/core/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:48:49.989295 brds-0.1.0/brds/core/fetch/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 19:48:37.000000 brds-0.1.0/brds/core/fetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-10 19:48:37.000000 brds-0.1.0/brds/core/fetch/fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:48:49.989295 brds-0.1.0/brds/core/fs/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-10 19:48:37.000000 brds-0.1.0/brds/core/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-10 19:48:37.000000 brds-0.1.0/brds/core/fs/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-10 19:48:37.000000 brds-0.1.0/brds/core/fs/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:48:49.989295 brds-0.1.0/brds/core/importer/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-10 19:48:37.000000 brds-0.1.0/brds/core/importer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-10 19:48:37.000000 brds-0.1.0/brds/core/importer/gunizp_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-10 19:48:37.000000 brds-0.1.0/brds/core/importer/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-10 19:48:37.000000 brds-0.1.0/brds/core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-10 19:48:37.000000 brds-0.1.0/brds/core/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:48:49.989295 brds-0.1.0/brds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 19:48:49.000000 brds-0.1.0/brds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-10 19:48:49.000000 brds-0.1.0/brds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:48:49.000000 brds-0.1.0/brds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-10 19:48:49.000000 brds-0.1.0/brds.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-10 19:48:49.000000 brds-0.1.0/brds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 19:48:49.000000 brds-0.1.0/brds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 19:48:49.989295 brds-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-10 19:48:37.000000 brds-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:48:49.989295 brds-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:48:37.000000 brds-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-10 19:48:37.000000 brds-0.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-10 19:48:37.000000 brds-0.1.0/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:51:25.598150 brds-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-10 19:51:17.000000 brds-0.1.1/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-10 19:51:17.000000 brds-0.1.1/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-10 19:51:17.000000 brds-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 19:51:17.000000 brds-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 19:51:25.598150 brds-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-10 19:51:17.000000 brds-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:51:25.598150 brds-0.1.1/brds/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 19:51:17.000000 brds-0.1.1/brds/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-10 19:51:17.000000 brds-0.1.1/brds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-10 19:51:17.000000 brds-0.1.1/brds/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-10 19:51:17.000000 brds-0.1.1/brds/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-10 19:51:17.000000 brds-0.1.1/brds/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-10 19:51:17.000000 brds-0.1.1/brds/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:51:25.598150 brds-0.1.1/brds/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:51:25.598150 brds-0.1.1/brds/core/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/datasets/dataset_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/datasets/dataset_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/datasets/list_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:51:25.598150 brds-0.1.1/brds/core/fetch/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/fetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/fetch/fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:51:25.598150 brds-0.1.1/brds/core/fs/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/fs/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/fs/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:51:25.598150 brds-0.1.1/brds/core/importer/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/importer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/importer/gunizp_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/importer/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-10 19:51:17.000000 brds-0.1.1/brds/core/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:51:25.598150 brds-0.1.1/brds/humanize/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-10 19:51:17.000000 brds-0.1.1/brds/humanize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-10 19:51:17.000000 brds-0.1.1/brds/humanize/sizes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:51:25.598150 brds-0.1.1/brds/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-10 19:51:17.000000 brds-0.1.1/brds/templates/dataset_files.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-10 19:51:17.000000 brds-0.1.1/brds/templates/datasets.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:51:25.598150 brds-0.1.1/brds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 19:51:25.000000 brds-0.1.1/brds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-10 19:51:25.000000 brds-0.1.1/brds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:51:25.000000 brds-0.1.1/brds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-10 19:51:25.000000 brds-0.1.1/brds.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-10 19:51:25.000000 brds-0.1.1/brds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 19:51:25.000000 brds-0.1.1/brds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 19:51:25.598150 brds-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-10 19:51:17.000000 brds-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:51:25.598150 brds-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:51:17.000000 brds-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-10 19:51:17.000000 brds-0.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-10 19:51:17.000000 brds-0.1.1/tests/test_base.py
```

### Comparing `brds-0.1.0/LICENSE` & `brds-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `brds-0.1.0/PKG-INFO` & `brds-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brds
-Version: 0.1.0
+Version: 0.1.1
 Summary: Awesome brds created by brahle
 Home-page: https://github.com/brahle/brds/
 Author: brahle
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `brds-0.1.0/brds/cli.py` & `brds-0.1.1/brds/cli.py`

 * *Files identical despite different names*

### Comparing `brds-0.1.0/brds/core/environment.py` & `brds-0.1.1/brds/core/environment.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,47 @@
+"""
+This module contains the environment variables used by the application.
+"""
+
 from os import environ as _environ
 from os.path import expanduser as _expanduser
 from os.path import join as _join
 
 from dotenv import load_dotenv as _load_dotenv
 
 _load_dotenv()
 
 
 def root_folder_path() -> str:
+    """
+    Get the root folder path for the data storage.
+    """
     if "ROOT_FOLDER_PATH" in _environ:
         return _environ["ROOT_FOLDER_PATH"]
     return _join(_expanduser("~"), "data")
 
 
 def writer_folder_path() -> str:
+    """
+    Get the folder path for the data writer.
+    """
     if "FILE_WRITER_PATH" in _environ:
         return _environ["FILE_WRITER_PATH"]
     return root_folder_path()
 
 
 def reader_folder_path() -> str:
+    """
+    Get the folder path for the data reader.
+    """
     if "FILE_READER_PATH" in _environ:
         return _environ["FILE_READER_PATH"]
     return root_folder_path()
 
 
 def vault_token() -> str:
+    """
+    Get the vault token.
+    """
     if "VAULT_TOKEN" in _environ:
         return _environ["VAULT_TOKEN"]
     return ""
```

### Comparing `brds-0.1.0/brds/core/fetch/fetcher.py` & `brds-0.1.1/brds/core/fetch/fetcher.py`

 * *Files identical despite different names*

### Comparing `brds-0.1.0/brds/core/fs/reader.py` & `brds-0.1.1/brds/core/fs/reader.py`

 * *Files identical despite different names*

### Comparing `brds-0.1.0/brds/core/fs/writer.py` & `brds-0.1.1/brds/core/fs/writer.py`

 * *Files identical despite different names*

### Comparing `brds-0.1.0/brds/core/importer/gunizp_importer.py` & `brds-0.1.1/brds/core/importer/gunizp_importer.py`

 * *Files identical despite different names*

### Comparing `brds-0.1.0/brds/core/logger.py` & `brds-0.1.1/brds/core/logger.py`

 * *Files identical despite different names*

### Comparing `brds-0.1.0/brds.egg-info/PKG-INFO` & `brds-0.1.1/brds.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brds
-Version: 0.1.0
+Version: 0.1.1
 Summary: Awesome brds created by brahle
 Home-page: https://github.com/brahle/brds/
 Author: brahle
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `brds-0.1.0/brds.egg-info/SOURCES.txt` & `brds-0.1.1/brds.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -3,30 +3,39 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 brds/VERSION
 brds/__init__.py
 brds/__main__.py
+brds/app.py
 brds/base.py
 brds/cli.py
 brds.egg-info/PKG-INFO
 brds.egg-info/SOURCES.txt
 brds.egg-info/dependency_links.txt
 brds.egg-info/entry_points.txt
 brds.egg-info/requires.txt
 brds.egg-info/top_level.txt
 brds/core/__init__.py
 brds/core/environment.py
 brds/core/logger.py
 brds/core/vault.py
+brds/core/datasets/__init__.py
+brds/core/datasets/dataset_files.py
+brds/core/datasets/dataset_info.py
+brds/core/datasets/list_datasets.py
 brds/core/fetch/__init__.py
 brds/core/fetch/fetcher.py
 brds/core/fs/__init__.py
 brds/core/fs/reader.py
 brds/core/fs/writer.py
 brds/core/importer/__init__.py
 brds/core/importer/gunizp_importer.py
 brds/core/importer/importer.py
+brds/humanize/__init__.py
+brds/humanize/sizes.py
+brds/templates/dataset_files.html
+brds/templates/datasets.html
 tests/__init__.py
 tests/conftest.py
 tests/test_base.py
```

### Comparing `brds-0.1.0/setup.py` & `brds-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,9 +38,12 @@
     long_description_content_type="text/markdown",
     author="brahle",
     packages=find_packages(exclude=["tests", ".github"]),
     install_requires=read_requirements("requirements.txt"),
     entry_points={
         "console_scripts": ["brds = brds.__main__:main"]
     },
+    package_data={
+        'brds': ['brds/templates/**.html']
+    },
     extras_require={"test": read_requirements("requirements-test.txt")},
 )
```

