# Comparing `tmp/scENVI-0.0.7.tar.gz` & `tmp/scENVI-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scENVI-0.0.7.tar", last modified: Mon Apr 10 18:38:30 2023, max compression
+gzip compressed data, was "scENVI-0.0.8.tar", last modified: Mon Apr 10 18:49:01 2023, max compression
```

## Comparing `scENVI-0.0.7.tar` & `scENVI-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 havivd    (1777) peer      (6070)        0 2023-04-10 18:38:30.913244 scENVI-0.0.7/
--rw-r--r--   0 havivd    (1777) peer      (6070)        0 2023-03-15 16:56:55.000000 scENVI-0.0.7/LICENSE
--rw-r--r--   0 havivd    (1777) peer      (6070)     1916 2023-04-10 18:38:30.912462 scENVI-0.0.7/PKG-INFO
--rw-r--r--   0 havivd    (1777) peer      (6070)     1419 2023-04-07 21:20:08.000000 scENVI-0.0.7/README.md
--rw-r--r--   0 havivd    (1777) peer      (6070)      819 2023-04-10 18:38:09.000000 scENVI-0.0.7/pyproject.toml
-drwxr-xr-x   0 havivd    (1777) peer      (6070)        0 2023-04-10 18:38:30.899910 scENVI-0.0.7/scENVI/
--rw-r--r--   0 havivd    (1777) peer      (6070)    56995 2023-04-10 18:00:17.000000 scENVI-0.0.7/scENVI/ENVI.py
--rw-r--r--   0 havivd    (1777) peer      (6070)        0 2023-03-15 16:52:08.000000 scENVI-0.0.7/scENVI/__init__.py
--rw-r--r--   0 havivd    (1777) peer      (6070)     8697 2023-04-10 17:57:36.000000 scENVI-0.0.7/scENVI/output_layer.py
--rw-r--r--   0 havivd    (1777) peer      (6070)    12047 2023-04-10 17:56:54.000000 scENVI-0.0.7/scENVI/utils.py
-drwxr-xr-x   0 havivd    (1777) peer      (6070)        0 2023-04-10 18:38:30.911124 scENVI-0.0.7/scENVI.egg-info/
--rw-r--r--   0 havivd    (1777) peer      (6070)     1916 2023-04-10 18:38:30.907367 scENVI-0.0.7/scENVI.egg-info/PKG-INFO
--rw-r--r--   0 havivd    (1777) peer      (6070)      254 2023-04-10 18:38:30.908490 scENVI-0.0.7/scENVI.egg-info/SOURCES.txt
--rw-r--r--   0 havivd    (1777) peer      (6070)        1 2023-04-10 18:38:30.909438 scENVI-0.0.7/scENVI.egg-info/dependency_links.txt
--rw-r--r--   0 havivd    (1777) peer      (6070)      143 2023-04-10 18:38:30.910384 scENVI-0.0.7/scENVI.egg-info/requires.txt
--rw-r--r--   0 havivd    (1777) peer      (6070)        7 2023-04-10 18:38:30.911421 scENVI-0.0.7/scENVI.egg-info/top_level.txt
--rw-r--r--   0 havivd    (1777) peer      (6070)       38 2023-04-10 18:38:30.913472 scENVI-0.0.7/setup.cfg
+drwxr-xr-x   0 havivd    (1777) peer      (6070)        0 2023-04-10 18:49:01.612679 scENVI-0.0.8/
+-rw-r--r--   0 havivd    (1777) peer      (6070)        0 2023-03-15 16:56:55.000000 scENVI-0.0.8/LICENSE
+-rw-r--r--   0 havivd    (1777) peer      (6070)     1899 2023-04-10 18:49:01.611881 scENVI-0.0.8/PKG-INFO
+-rw-r--r--   0 havivd    (1777) peer      (6070)     1419 2023-04-07 21:20:08.000000 scENVI-0.0.8/README.md
+-rw-r--r--   0 havivd    (1777) peer      (6070)      785 2023-04-10 18:47:30.000000 scENVI-0.0.8/pyproject.toml
+drwxr-xr-x   0 havivd    (1777) peer      (6070)        0 2023-04-10 18:49:01.604969 scENVI-0.0.8/scENVI/
+-rw-r--r--   0 havivd    (1777) peer      (6070)    56995 2023-04-10 18:00:17.000000 scENVI-0.0.8/scENVI/ENVI.py
+-rw-r--r--   0 havivd    (1777) peer      (6070)        0 2023-03-15 16:52:08.000000 scENVI-0.0.8/scENVI/__init__.py
+-rw-r--r--   0 havivd    (1777) peer      (6070)     8697 2023-04-10 17:57:36.000000 scENVI-0.0.8/scENVI/output_layer.py
+-rw-r--r--   0 havivd    (1777) peer      (6070)    12047 2023-04-10 17:56:54.000000 scENVI-0.0.8/scENVI/utils.py
+drwxr-xr-x   0 havivd    (1777) peer      (6070)        0 2023-04-10 18:49:01.610470 scENVI-0.0.8/scENVI.egg-info/
+-rw-r--r--   0 havivd    (1777) peer      (6070)     1899 2023-04-10 18:49:01.606013 scENVI-0.0.8/scENVI.egg-info/PKG-INFO
+-rw-r--r--   0 havivd    (1777) peer      (6070)      254 2023-04-10 18:49:01.606720 scENVI-0.0.8/scENVI.egg-info/SOURCES.txt
+-rw-r--r--   0 havivd    (1777) peer      (6070)        1 2023-04-10 18:49:01.608670 scENVI-0.0.8/scENVI.egg-info/dependency_links.txt
+-rw-r--r--   0 havivd    (1777) peer      (6070)      140 2023-04-10 18:49:01.609701 scENVI-0.0.8/scENVI.egg-info/requires.txt
+-rw-r--r--   0 havivd    (1777) peer      (6070)        7 2023-04-10 18:49:01.610712 scENVI-0.0.8/scENVI.egg-info/top_level.txt
+-rw-r--r--   0 havivd    (1777) peer      (6070)       38 2023-04-10 18:49:01.612932 scENVI-0.0.8/setup.cfg
```

### Comparing `scENVI-0.0.7/PKG-INFO` & `scENVI-0.0.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: scENVI
-Version: 0.0.7
-Summary: A small example package
-Author-email: Example Author <author@example.com>
+Version: 0.0.8
+Summary: ENVI
+Author-email: Doron Haviv <doron.haviv12@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `scENVI-0.0.7/README.md` & `scENVI-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `scENVI-0.0.7/pyproject.toml` & `scENVI-0.0.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "scENVI"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
-  { name="Example Author", email="author@example.com" },
+  { name="Doron Haviv", email="doron.haviv12@gmail.com" },
 ]
-description = "A small example package"
+description = "ENVI"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     'tensorflow >= 2.4.0',
     'tensorflow_probability >= 0.12.2',
     'numpy>=1.22.4',
     'scikit-learn>=1.2.1',
     'scipy>=1.10.1',
-    'scanpy',
+    'scanpy>=1.9.1',
     'anndata>=0.8.0',
     'pandas>=1.5.3',
-    'os',
-    'pickle',
 ]
 
     
     
 [project.urls]
 "Homepage" = "https://github.com/pypa/sampleproject"
 "Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
```

### Comparing `scENVI-0.0.7/scENVI/ENVI.py` & `scENVI-0.0.8/scENVI/ENVI.py`

 * *Files identical despite different names*

### Comparing `scENVI-0.0.7/scENVI/output_layer.py` & `scENVI-0.0.8/scENVI/output_layer.py`

 * *Files identical despite different names*

### Comparing `scENVI-0.0.7/scENVI/utils.py` & `scENVI-0.0.8/scENVI/utils.py`

 * *Files identical despite different names*

### Comparing `scENVI-0.0.7/scENVI.egg-info/PKG-INFO` & `scENVI-0.0.8/scENVI.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: scENVI
-Version: 0.0.7
-Summary: A small example package
-Author-email: Example Author <author@example.com>
+Version: 0.0.8
+Summary: ENVI
+Author-email: Doron Haviv <doron.haviv12@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

