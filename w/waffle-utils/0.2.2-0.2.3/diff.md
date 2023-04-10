# Comparing `tmp/waffle_utils-0.2.2.tar.gz` & `tmp/waffle_utils-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waffle_utils-0.2.2.tar", last modified: Tue Mar 28 04:10:33 2023, max compression
+gzip compressed data, was "waffle_utils-0.2.3.tar", last modified: Mon Apr 10 10:41:33 2023, max compression
```

## Comparing `waffle_utils-0.2.2.tar` & `waffle_utils-0.2.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-03-28 04:10:33.864776 waffle_utils-0.2.2/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      140 2023-03-20 23:39:58.000000 waffle_utils-0.2.2/MANIFEST.in
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2619 2023-03-28 04:10:33.864776 waffle_utils-0.2.2/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1544 2023-03-20 23:39:58.000000 waffle_utils-0.2.2/README.md
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       71 2023-03-20 23:39:58.000000 waffle_utils-0.2.2/requirements.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-03-28 04:10:33.864776 waffle_utils-0.2.2/setup.cfg
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2667 2023-03-20 23:39:58.000000 waffle_utils-0.2.2/setup.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-03-28 04:10:33.864776 waffle_utils-0.2.2/tests/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3361 2023-03-28 03:57:15.000000 waffle_utils-0.2.2/tests/test_cli.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-03-28 04:10:33.864776 waffle_utils-0.2.2/waffle_utils/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       22 2023-03-28 03:57:15.000000 waffle_utils-0.2.2/waffle_utils/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-03-28 04:10:33.864776 waffle_utils-0.2.2/waffle_utils/dataset/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       89 2023-03-20 23:39:58.000000 waffle_utils-0.2.2/waffle_utils/dataset/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    25546 2023-03-28 03:57:15.000000 waffle_utils-0.2.2/waffle_utils/dataset/dataset.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-03-28 04:10:33.864776 waffle_utils-0.2.2/waffle_utils/dataset/fields/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      185 2023-03-20 23:39:58.000000 waffle_utils-0.2.2/waffle_utils/dataset/fields/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    12457 2023-03-20 23:39:58.000000 waffle_utils-0.2.2/waffle_utils/dataset/fields/annotation.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      550 2023-03-20 23:39:58.000000 waffle_utils-0.2.2/waffle_utils/dataset/fields/base_field.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     5283 2023-03-20 23:39:58.000000 waffle_utils-0.2.2/waffle_utils/dataset/fields/category.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2653 2023-03-20 23:39:58.000000 waffle_utils-0.2.2/waffle_utils/dataset/fields/image.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      188 2023-03-20 23:39:58.000000 waffle_utils-0.2.2/waffle_utils/dataset/format.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-03-28 04:10:33.864776 waffle_utils-0.2.2/waffle_utils/file/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-03-20 23:39:58.000000 waffle_utils-0.2.2/waffle_utils/file/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4706 2023-03-20 23:39:58.000000 waffle_utils-0.2.2/waffle_utils/file/io.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      475 2023-03-20 23:39:58.000000 waffle_utils-0.2.2/waffle_utils/file/network.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3240 2023-03-20 23:39:58.000000 waffle_utils-0.2.2/waffle_utils/file/search.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-03-28 04:10:33.864776 waffle_utils-0.2.2/waffle_utils/image/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      128 2023-03-20 23:39:58.000000 waffle_utils-0.2.2/waffle_utils/image/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      332 2023-03-20 23:39:58.000000 waffle_utils-0.2.2/waffle_utils/image/io.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-03-28 04:10:33.864776 waffle_utils-0.2.2/waffle_utils/log/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      120 2023-03-20 23:39:58.000000 waffle_utils-0.2.2/waffle_utils/log/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1701 2023-03-28 03:57:15.000000 waffle_utils-0.2.2/waffle_utils/log/template.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      238 2023-03-20 23:39:58.000000 waffle_utils-0.2.2/waffle_utils/log/time.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4698 2023-03-28 03:57:15.000000 waffle_utils-0.2.2/waffle_utils/run.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-03-28 04:10:33.864776 waffle_utils-0.2.2/waffle_utils/utils/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       69 2023-03-20 23:39:58.000000 waffle_utils-0.2.2/waffle_utils/utils/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      435 2023-03-20 23:39:58.000000 waffle_utils-0.2.2/waffle_utils/utils/validators.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-03-28 04:10:33.864776 waffle_utils-0.2.2/waffle_utils/video/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1089 2023-03-20 23:39:58.000000 waffle_utils-0.2.2/waffle_utils/video/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      693 2023-03-20 23:39:58.000000 waffle_utils-0.2.2/waffle_utils/video/io.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4104 2023-03-20 23:39:58.000000 waffle_utils-0.2.2/waffle_utils/video/tools.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-03-28 04:10:33.864776 waffle_utils-0.2.2/waffle_utils.egg-info/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2619 2023-03-28 04:10:33.000000 waffle_utils-0.2.2/waffle_utils.egg-info/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1023 2023-03-28 04:10:33.000000 waffle_utils-0.2.2/waffle_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-03-28 04:10:33.000000 waffle_utils-0.2.2/waffle_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       44 2023-03-28 04:10:33.000000 waffle_utils-0.2.2/waffle_utils.egg-info/entry_points.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       78 2023-03-28 04:10:33.000000 waffle_utils-0.2.2/waffle_utils.egg-info/requires.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       13 2023-03-28 04:10:33.000000 waffle_utils-0.2.2/waffle_utils.egg-info/top_level.txt
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      140 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/MANIFEST.in
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2619 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1544 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/README.md
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       71 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/requirements.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/setup.cfg
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2667 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/setup.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/tests/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3383 2023-04-10 10:41:06.000000 waffle_utils-0.2.3/tests/test_cli.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/waffle_utils/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       22 2023-04-10 10:41:06.000000 waffle_utils-0.2.3/waffle_utils/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/waffle_utils/dataset/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       89 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/dataset/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    25766 2023-04-10 10:41:06.000000 waffle_utils-0.2.3/waffle_utils/dataset/dataset.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/waffle_utils/dataset/fields/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      185 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/dataset/fields/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    12457 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/dataset/fields/annotation.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      550 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/dataset/fields/base_field.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     5283 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/dataset/fields/category.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2653 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/dataset/fields/image.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      188 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/dataset/format.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/waffle_utils/file/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/file/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4706 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/file/io.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      475 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/file/network.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3240 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/file/search.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/waffle_utils/image/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      128 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/image/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      332 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/image/io.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/waffle_utils/log/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      120 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/log/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1701 2023-03-28 04:12:00.000000 waffle_utils-0.2.3/waffle_utils/log/template.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      238 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/log/time.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4698 2023-03-28 04:12:00.000000 waffle_utils-0.2.3/waffle_utils/run.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/waffle_utils/utils/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       69 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/utils/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      435 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/utils/validators.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/waffle_utils/video/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1089 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/video/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      693 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/video/io.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4104 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/video/tools.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/waffle_utils.egg-info/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2619 2023-04-10 10:41:33.000000 waffle_utils-0.2.3/waffle_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1023 2023-04-10 10:41:33.000000 waffle_utils-0.2.3/waffle_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-04-10 10:41:33.000000 waffle_utils-0.2.3/waffle_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       44 2023-04-10 10:41:33.000000 waffle_utils-0.2.3/waffle_utils.egg-info/entry_points.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       78 2023-04-10 10:41:33.000000 waffle_utils-0.2.3/waffle_utils.egg-info/requires.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       13 2023-04-10 10:41:33.000000 waffle_utils-0.2.3/waffle_utils.egg-info/top_level.txt
```

### Comparing `waffle_utils-0.2.2/PKG-INFO` & `waffle_utils-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle_utils
-Version: 0.2.2
+Version: 0.2.3
 Summary: Waffle Utils 🥛
 Home-page: https://github.com/snuailab/waffle_utils
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_utils/issues
 Project-URL: Source, https://github.com/snuailab/waffle_utils
```

### Comparing `waffle_utils-0.2.2/README.md` & `waffle_utils-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `waffle_utils-0.2.2/setup.py` & `waffle_utils-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `waffle_utils-0.2.2/tests/test_cli.py` & `waffle_utils-0.2.3/tests/test_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,26 +44,26 @@
 @pytest.fixture(scope="module")
 def dataset_name():
     return "mnist"
 
 
 @pytest.fixture(scope="module")
 def coco_root_dir(extract_dir):
-    return extract_dir / "raw"
+    return extract_dir / "images"
 
 
 @pytest.fixture(scope="module")
 def coco_file(extract_dir):
-    return extract_dir / "exports/coco.json"
+    return extract_dir / "coco.json"
 
 
 # Define tests for dataset-related functions
 def test_get_file_from_url(zip_file):
     run(
-        f"python -m waffle_utils.run get_file_from_url --url https://github.com/snuailab/waffle_utils/raw/main/mnist.zip --file-path {zip_file}"
+        f"python -m waffle_utils.run get_file_from_url --url https://raw.githubusercontent.com/snuailab/assets/main/waffle/sample_dataset/mnist.zip --file-path {zip_file}"
     )
 
 
 def test_unzip(zip_file, extract_dir):
     run(
         f"python -m waffle_utils.run unzip --file-path {zip_file} --output-dir {extract_dir}"
     )
```

### Comparing `waffle_utils-0.2.2/waffle_utils/dataset/dataset.py` & `waffle_utils-0.2.3/waffle_utils/dataset/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,21 @@
     def test_set_file(self) -> Path:
         return self.set_dir / Dataset.TEST_SET_FILE_NAME
 
     @cached_property
     def unlabeled_set_file(self) -> Path:
         return self.set_dir / Dataset.UNLABELED_SET_FILE_NAME
 
+    @cached_property
+    def classes(self) -> list[str]:
+        categories: list[Category] = self.get_categories()
+        return [
+            c.name for c in sorted(categories, key=lambda c: c.category_id)
+        ]
+
     # factories
     @classmethod
     def new(cls, name: str, root_dir: str = None) -> "Dataset":
         """Create New Dataset
 
         Args:
             name (str): Dataset name
```

### Comparing `waffle_utils-0.2.2/waffle_utils/dataset/fields/annotation.py` & `waffle_utils-0.2.3/waffle_utils/dataset/fields/annotation.py`

 * *Files identical despite different names*

### Comparing `waffle_utils-0.2.2/waffle_utils/dataset/fields/base_field.py` & `waffle_utils-0.2.3/waffle_utils/dataset/fields/base_field.py`

 * *Files identical despite different names*

### Comparing `waffle_utils-0.2.2/waffle_utils/dataset/fields/category.py` & `waffle_utils-0.2.3/waffle_utils/dataset/fields/category.py`

 * *Files identical despite different names*

### Comparing `waffle_utils-0.2.2/waffle_utils/dataset/fields/image.py` & `waffle_utils-0.2.3/waffle_utils/dataset/fields/image.py`

 * *Files identical despite different names*

### Comparing `waffle_utils-0.2.2/waffle_utils/file/io.py` & `waffle_utils-0.2.3/waffle_utils/file/io.py`

 * *Files identical despite different names*

### Comparing `waffle_utils-0.2.2/waffle_utils/file/search.py` & `waffle_utils-0.2.3/waffle_utils/file/search.py`

 * *Files identical despite different names*

### Comparing `waffle_utils-0.2.2/waffle_utils/log/template.py` & `waffle_utils-0.2.3/waffle_utils/log/template.py`

 * *Files identical despite different names*

### Comparing `waffle_utils-0.2.2/waffle_utils/run.py` & `waffle_utils-0.2.3/waffle_utils/run.py`

 * *Files identical despite different names*

### Comparing `waffle_utils-0.2.2/waffle_utils/video/__init__.py` & `waffle_utils-0.2.3/waffle_utils/video/__init__.py`

 * *Files identical despite different names*

### Comparing `waffle_utils-0.2.2/waffle_utils/video/io.py` & `waffle_utils-0.2.3/waffle_utils/video/io.py`

 * *Files identical despite different names*

### Comparing `waffle_utils-0.2.2/waffle_utils/video/tools.py` & `waffle_utils-0.2.3/waffle_utils/video/tools.py`

 * *Files identical despite different names*

### Comparing `waffle_utils-0.2.2/waffle_utils.egg-info/PKG-INFO` & `waffle_utils-0.2.3/waffle_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle-utils
-Version: 0.2.2
+Version: 0.2.3
 Summary: Waffle Utils 🥛
 Home-page: https://github.com/snuailab/waffle_utils
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_utils/issues
 Project-URL: Source, https://github.com/snuailab/waffle_utils
```

### Comparing `waffle_utils-0.2.2/waffle_utils.egg-info/SOURCES.txt` & `waffle_utils-0.2.3/waffle_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

