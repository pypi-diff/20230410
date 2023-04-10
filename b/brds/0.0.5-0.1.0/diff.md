# Comparing `tmp/brds-0.0.5.tar.gz` & `tmp/brds-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brds-0.0.5.tar", last modified: Sat Feb 18 21:13:24 2023, max compression
+gzip compressed data, was "brds-0.1.0.tar", last modified: Mon Apr 10 19:48:49 2023, max compression
```

## Comparing `brds-0.0.5.tar` & `brds-0.1.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 21:13:24.436722 brds-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-18 21:13:12.000000 brds-0.0.5/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-02-18 21:13:12.000000 brds-0.0.5/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-02-18 21:13:12.000000 brds-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-02-18 21:13:12.000000 brds-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-02-18 21:13:24.436722 brds-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-02-18 21:13:12.000000 brds-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 21:13:24.432722 brds-0.0.5/brds/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-18 21:13:12.000000 brds-0.0.5/brds/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-02-18 21:13:12.000000 brds-0.0.5/brds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-18 21:13:12.000000 brds-0.0.5/brds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-02-18 21:13:12.000000 brds-0.0.5/brds/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-02-18 21:13:12.000000 brds-0.0.5/brds/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 21:13:24.436722 brds-0.0.5/brds/core/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-02-18 21:13:12.000000 brds-0.0.5/brds/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-02-18 21:13:12.000000 brds-0.0.5/brds/core/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 21:13:24.436722 brds-0.0.5/brds/core/fetch/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-18 21:13:12.000000 brds-0.0.5/brds/core/fetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-02-18 21:13:12.000000 brds-0.0.5/brds/core/fetch/fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 21:13:24.436722 brds-0.0.5/brds/core/fs/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-02-18 21:13:12.000000 brds-0.0.5/brds/core/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-02-18 21:13:12.000000 brds-0.0.5/brds/core/fs/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-02-18 21:13:12.000000 brds-0.0.5/brds/core/fs/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 21:13:24.436722 brds-0.0.5/brds/core/importer/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-02-18 21:13:12.000000 brds-0.0.5/brds/core/importer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-18 21:13:12.000000 brds-0.0.5/brds/core/importer/gunizp_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-02-18 21:13:12.000000 brds-0.0.5/brds/core/importer/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-02-18 21:13:12.000000 brds-0.0.5/brds/core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-02-18 21:13:12.000000 brds-0.0.5/brds/core/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 21:13:24.432722 brds-0.0.5/brds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-02-18 21:13:24.000000 brds-0.0.5/brds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-02-18 21:13:24.000000 brds-0.0.5/brds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-18 21:13:24.000000 brds-0.0.5/brds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-18 21:13:24.000000 brds-0.0.5/brds.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-02-18 21:13:24.000000 brds-0.0.5/brds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-18 21:13:24.000000 brds-0.0.5/brds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-18 21:13:24.436722 brds-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-02-18 21:13:12.000000 brds-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 21:13:24.436722 brds-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 21:13:12.000000 brds-0.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-02-18 21:13:12.000000 brds-0.0.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-18 21:13:12.000000 brds-0.0.5/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:48:49.989295 brds-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-10 19:48:37.000000 brds-0.1.0/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-10 19:48:37.000000 brds-0.1.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-10 19:48:37.000000 brds-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 19:48:37.000000 brds-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 19:48:49.989295 brds-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-10 19:48:37.000000 brds-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:48:49.989295 brds-0.1.0/brds/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 19:48:37.000000 brds-0.1.0/brds/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-10 19:48:37.000000 brds-0.1.0/brds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-10 19:48:37.000000 brds-0.1.0/brds/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-10 19:48:37.000000 brds-0.1.0/brds/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-10 19:48:37.000000 brds-0.1.0/brds/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:48:49.989295 brds-0.1.0/brds/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-10 19:48:37.000000 brds-0.1.0/brds/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-10 19:48:37.000000 brds-0.1.0/brds/core/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:48:49.989295 brds-0.1.0/brds/core/fetch/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 19:48:37.000000 brds-0.1.0/brds/core/fetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-10 19:48:37.000000 brds-0.1.0/brds/core/fetch/fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:48:49.989295 brds-0.1.0/brds/core/fs/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-10 19:48:37.000000 brds-0.1.0/brds/core/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-10 19:48:37.000000 brds-0.1.0/brds/core/fs/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-10 19:48:37.000000 brds-0.1.0/brds/core/fs/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:48:49.989295 brds-0.1.0/brds/core/importer/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-10 19:48:37.000000 brds-0.1.0/brds/core/importer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-10 19:48:37.000000 brds-0.1.0/brds/core/importer/gunizp_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-10 19:48:37.000000 brds-0.1.0/brds/core/importer/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-10 19:48:37.000000 brds-0.1.0/brds/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-10 19:48:37.000000 brds-0.1.0/brds/core/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:48:49.989295 brds-0.1.0/brds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 19:48:49.000000 brds-0.1.0/brds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-10 19:48:49.000000 brds-0.1.0/brds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:48:49.000000 brds-0.1.0/brds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-10 19:48:49.000000 brds-0.1.0/brds.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-10 19:48:49.000000 brds-0.1.0/brds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 19:48:49.000000 brds-0.1.0/brds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 19:48:49.989295 brds-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-10 19:48:37.000000 brds-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:48:49.989295 brds-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:48:37.000000 brds-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-10 19:48:37.000000 brds-0.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-10 19:48:37.000000 brds-0.1.0/tests/test_base.py
```

### Comparing `brds-0.0.5/HISTORY.md` & `brds-0.1.0/HISTORY.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Changelog
 =========
 
 
-(unreleased)
-------------
+0.0.5 (2023-02-18)
+------------------
+- Release: version 0.0.5 🚀 [brahle]
 - Feat: Adding gunzip imporer (#5) [Bruno Rahle]
 
 
 0.0.4 (2023-02-18)
 ------------------
 - Release: version 0.0.4 🚀 [brahle]
 - Updating version (#4) [Bruno Rahle]
```

### Comparing `brds-0.0.5/LICENSE` & `brds-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `brds-0.0.5/PKG-INFO` & `brds-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brds
-Version: 0.0.5
+Version: 0.1.0
 Summary: Awesome brds created by brahle
 Home-page: https://github.com/brahle/brds/
 Author: brahle
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `brds-0.0.5/brds/cli.py` & `brds-0.1.0/brds/cli.py`

 * *Files identical despite different names*

### Comparing `brds-0.0.5/brds/core/environment.py` & `brds-0.1.0/brds/core/environment.py`

 * *Files identical despite different names*

### Comparing `brds-0.0.5/brds/core/fetch/fetcher.py` & `brds-0.1.0/brds/core/fetch/fetcher.py`

 * *Files identical despite different names*

### Comparing `brds-0.0.5/brds/core/fs/reader.py` & `brds-0.1.0/brds/core/fs/reader.py`

 * *Files identical despite different names*

### Comparing `brds-0.0.5/brds/core/fs/writer.py` & `brds-0.1.0/brds/core/fs/writer.py`

 * *Files identical despite different names*

### Comparing `brds-0.0.5/brds/core/importer/gunizp_importer.py` & `brds-0.1.0/brds/core/importer/gunizp_importer.py`

 * *Files identical despite different names*

### Comparing `brds-0.0.5/brds/core/logger.py` & `brds-0.1.0/brds/core/logger.py`

 * *Files identical despite different names*

### Comparing `brds-0.0.5/brds.egg-info/PKG-INFO` & `brds-0.1.0/brds.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brds
-Version: 0.0.5
+Version: 0.1.0
 Summary: Awesome brds created by brahle
 Home-page: https://github.com/brahle/brds/
 Author: brahle
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `brds-0.0.5/brds.egg-info/SOURCES.txt` & `brds-0.1.0/brds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brds-0.0.5/setup.py` & `brds-0.1.0/setup.py`

 * *Files identical despite different names*

