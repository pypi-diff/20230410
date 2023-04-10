# Comparing `tmp/brds-0.2.5.tar.gz` & `tmp/brds-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brds-0.2.5.tar", last modified: Mon Apr 10 21:37:00 2023, max compression
+gzip compressed data, was "brds-0.2.6.tar", last modified: Mon Apr 10 21:49:54 2023, max compression
```

## Comparing `brds-0.2.5.tar` & `brds-0.2.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:37:00.589469 brds-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-10 21:36:51.000000 brds-0.2.5/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-10 21:36:51.000000 brds-0.2.5/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-10 21:36:51.000000 brds-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 21:36:51.000000 brds-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 21:37:00.589469 brds-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-10 21:36:51.000000 brds-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:37:00.577468 brds-0.2.5/brds/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 21:36:51.000000 brds-0.2.5/brds/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-10 21:36:51.000000 brds-0.2.5/brds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-10 21:36:51.000000 brds-0.2.5/brds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-10 21:36:51.000000 brds-0.2.5/brds/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-10 21:36:51.000000 brds-0.2.5/brds/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-10 21:36:51.000000 brds-0.2.5/brds/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:37:00.581468 brds-0.2.5/brds/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-10 21:36:51.000000 brds-0.2.5/brds/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:37:00.585469 brds-0.2.5/brds/core/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-10 21:36:51.000000 brds-0.2.5/brds/core/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-10 21:36:51.000000 brds-0.2.5/brds/core/datasets/dataset_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-10 21:36:51.000000 brds-0.2.5/brds/core/datasets/dataset_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-10 21:36:51.000000 brds-0.2.5/brds/core/datasets/list_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-10 21:36:51.000000 brds-0.2.5/brds/core/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 21:36:51.000000 brds-0.2.5/brds/core/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:37:00.585469 brds-0.2.5/brds/core/fetch/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 21:36:51.000000 brds-0.2.5/brds/core/fetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-10 21:36:51.000000 brds-0.2.5/brds/core/fetch/fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:37:00.585469 brds-0.2.5/brds/core/fs/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-10 21:36:51.000000 brds-0.2.5/brds/core/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-10 21:36:51.000000 brds-0.2.5/brds/core/fs/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-10 21:36:51.000000 brds-0.2.5/brds/core/fs/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:37:00.585469 brds-0.2.5/brds/core/importer/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-10 21:36:51.000000 brds-0.2.5/brds/core/importer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-10 21:36:51.000000 brds-0.2.5/brds/core/importer/gunizp_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-10 21:36:51.000000 brds-0.2.5/brds/core/importer/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-10 21:36:51.000000 brds-0.2.5/brds/core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-10 21:36:51.000000 brds-0.2.5/brds/core/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:37:00.589469 brds-0.2.5/brds/humanize/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-10 21:36:51.000000 brds-0.2.5/brds/humanize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-10 21:36:51.000000 brds-0.2.5/brds/humanize/sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 21:36:51.000000 brds-0.2.5/brds/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:37:00.589469 brds-0.2.5/brds/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-10 21:36:51.000000 brds-0.2.5/brds/templates/dataset_files.html
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-10 21:36:51.000000 brds-0.2.5/brds/templates/datasets.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:37:00.581468 brds-0.2.5/brds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 21:37:00.000000 brds-0.2.5/brds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-10 21:37:00.000000 brds-0.2.5/brds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 21:37:00.000000 brds-0.2.5/brds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-10 21:37:00.000000 brds-0.2.5/brds.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-10 21:37:00.000000 brds-0.2.5/brds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 21:37:00.000000 brds-0.2.5/brds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 21:37:00.589469 brds-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-10 21:36:51.000000 brds-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:37:00.589469 brds-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 21:36:51.000000 brds-0.2.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-10 21:36:51.000000 brds-0.2.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-10 21:36:51.000000 brds-0.2.5/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:49:54.930499 brds-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-10 21:49:46.000000 brds-0.2.6/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-10 21:49:46.000000 brds-0.2.6/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-10 21:49:46.000000 brds-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 21:49:46.000000 brds-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 21:49:54.930499 brds-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-10 21:49:46.000000 brds-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:49:54.926499 brds-0.2.6/brds/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 21:49:46.000000 brds-0.2.6/brds/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-10 21:49:46.000000 brds-0.2.6/brds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-10 21:49:46.000000 brds-0.2.6/brds/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-10 21:49:46.000000 brds-0.2.6/brds/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-10 21:49:46.000000 brds-0.2.6/brds/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-10 21:49:46.000000 brds-0.2.6/brds/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:49:54.926499 brds-0.2.6/brds/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-10 21:49:46.000000 brds-0.2.6/brds/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:49:54.926499 brds-0.2.6/brds/core/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-10 21:49:46.000000 brds-0.2.6/brds/core/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-10 21:49:46.000000 brds-0.2.6/brds/core/datasets/dataset_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-10 21:49:46.000000 brds-0.2.6/brds/core/datasets/dataset_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-10 21:49:46.000000 brds-0.2.6/brds/core/datasets/list_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-10 21:49:46.000000 brds-0.2.6/brds/core/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 21:49:46.000000 brds-0.2.6/brds/core/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:49:54.930499 brds-0.2.6/brds/core/fetch/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 21:49:46.000000 brds-0.2.6/brds/core/fetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-10 21:49:46.000000 brds-0.2.6/brds/core/fetch/fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:49:54.930499 brds-0.2.6/brds/core/fs/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-10 21:49:46.000000 brds-0.2.6/brds/core/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-10 21:49:46.000000 brds-0.2.6/brds/core/fs/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-10 21:49:46.000000 brds-0.2.6/brds/core/fs/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:49:54.930499 brds-0.2.6/brds/core/importer/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-10 21:49:46.000000 brds-0.2.6/brds/core/importer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-10 21:49:46.000000 brds-0.2.6/brds/core/importer/gunizp_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-10 21:49:46.000000 brds-0.2.6/brds/core/importer/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-10 21:49:46.000000 brds-0.2.6/brds/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-10 21:49:46.000000 brds-0.2.6/brds/core/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:49:54.930499 brds-0.2.6/brds/humanize/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-10 21:49:46.000000 brds-0.2.6/brds/humanize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-10 21:49:46.000000 brds-0.2.6/brds/humanize/sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 21:49:46.000000 brds-0.2.6/brds/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:49:54.930499 brds-0.2.6/brds/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-10 21:49:46.000000 brds-0.2.6/brds/templates/dataset_files.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-10 21:49:46.000000 brds-0.2.6/brds/templates/datasets.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:49:54.926499 brds-0.2.6/brds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 21:49:54.000000 brds-0.2.6/brds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-10 21:49:54.000000 brds-0.2.6/brds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 21:49:54.000000 brds-0.2.6/brds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-10 21:49:54.000000 brds-0.2.6/brds.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-10 21:49:54.000000 brds-0.2.6/brds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 21:49:54.000000 brds-0.2.6/brds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 21:49:54.930499 brds-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-10 21:49:46.000000 brds-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:49:54.930499 brds-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 21:49:46.000000 brds-0.2.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-10 21:49:46.000000 brds-0.2.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-10 21:49:46.000000 brds-0.2.6/tests/test_base.py
```

### Comparing `brds-0.2.5/HISTORY.md` & `brds-0.2.6/HISTORY.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Fixing return types. [brahle]
+- Publish to docker. [brahle]
+
+
+0.2.5 (2023-04-10)
+------------------
+- Release: version 0.2.5 🚀 [brahle]
 - Adding pandas stubs. [brahle]
 
 
 0.2.4 (2023-04-10)
 ------------------
 - Release: version 0.2.4 🚀 [brahle]
 - Fixing packaging. [brahle]
```

### Comparing `brds-0.2.5/LICENSE` & `brds-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `brds-0.2.5/PKG-INFO` & `brds-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brds
-Version: 0.2.5
+Version: 0.2.6
 Summary: Awesome brds created by brahle
 Home-page: https://github.com/brahle/brds/
 Author: brahle
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `brds-0.2.5/brds/__init__.py` & `brds-0.2.6/brds/__init__.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.5/brds/app.py` & `brds-0.2.6/brds/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         df = fload(filename)
         return df.to_dict(orient="records")
     except FileNotFoundError as exc:
         raise HTTPException(status_code=404, detail=f"Parquet file '{filename}' not found") from exc
 
 
 @app.get("/html/{filename:path}", response_class=HTMLResponse)
-async def read_html(filename: str = Path(..., regex=r"[\w\-/]+")) -> Response:
+async def read_html(filename: str = Path(..., regex=r"[\w\-/]+")) -> str:
     try:
         df: pd.DataFrame = fload(filename)
         return df.to_html()
     except FileNotFoundError as exc:
         raise HTTPException(status_code=404, detail=f"Parquet file '{filename}' not found") from exc
```

### Comparing `brds-0.2.5/brds/cli.py` & `brds-0.2.6/brds/cli.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.5/brds/core/__init__.py` & `brds-0.2.6/brds/core/__init__.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.5/brds/core/datasets/dataset_files.py` & `brds-0.2.6/brds/core/datasets/dataset_files.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.5/brds/core/datasets/dataset_info.py` & `brds-0.2.6/brds/core/datasets/dataset_info.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.5/brds/core/datasets/list_datasets.py` & `brds-0.2.6/brds/core/datasets/list_datasets.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.5/brds/core/edit.py` & `brds-0.2.6/brds/core/edit.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.5/brds/core/environment.py` & `brds-0.2.6/brds/core/environment.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.5/brds/core/fetch/fetcher.py` & `brds-0.2.6/brds/core/fetch/fetcher.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.5/brds/core/fs/reader.py` & `brds-0.2.6/brds/core/fs/reader.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.5/brds/core/fs/writer.py` & `brds-0.2.6/brds/core/fs/writer.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.5/brds/core/importer/gunizp_importer.py` & `brds-0.2.6/brds/core/importer/gunizp_importer.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.5/brds/core/logger.py` & `brds-0.2.6/brds/core/logger.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.5/brds/humanize/sizes.py` & `brds-0.2.6/brds/humanize/sizes.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.5/brds/templates/dataset_files.html` & `brds-0.2.6/brds/templates/dataset_files.html`

 * *Files identical despite different names*

### Comparing `brds-0.2.5/brds/templates/datasets.html` & `brds-0.2.6/brds/templates/datasets.html`

 * *Files identical despite different names*

### Comparing `brds-0.2.5/brds.egg-info/PKG-INFO` & `brds-0.2.6/brds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brds
-Version: 0.2.5
+Version: 0.2.6
 Summary: Awesome brds created by brahle
 Home-page: https://github.com/brahle/brds/
 Author: brahle
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `brds-0.2.5/brds.egg-info/SOURCES.txt` & `brds-0.2.6/brds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brds-0.2.5/setup.py` & `brds-0.2.6/setup.py`

 * *Files identical despite different names*

