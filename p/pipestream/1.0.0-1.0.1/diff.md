# Comparing `tmp/pipestream-1.0.0.tar.gz` & `tmp/pipestream-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipestream-1.0.0.tar", last modified: Mon Apr 10 14:55:32 2023, max compression
+gzip compressed data, was "pipestream-1.0.1.tar", last modified: Mon Apr 10 15:16:35 2023, max compression
```

## Comparing `pipestream-1.0.0.tar` & `pipestream-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 colaborador   (501) staff       (20)        0 2023-04-10 14:55:32.845765 pipestream-1.0.0/
--rw-r--r--   0 colaborador   (501) staff       (20)     1073 2023-04-10 12:28:48.000000 pipestream-1.0.0/LICENSE
--rw-r--r--   0 colaborador   (501) staff       (20)     2296 2023-04-10 14:55:32.845584 pipestream-1.0.0/PKG-INFO
--rw-r--r--   0 colaborador   (501) staff       (20)     1733 2023-04-10 14:54:10.000000 pipestream-1.0.0/README.md
-drwxr-xr-x   0 colaborador   (501) staff       (20)        0 2023-04-10 14:55:32.842967 pipestream-1.0.0/pipestream/
--rw-r--r--   0 colaborador   (501) staff       (20)       30 2023-04-10 12:28:48.000000 pipestream-1.0.0/pipestream/__init__.py
--rw-r--r--   0 colaborador   (501) staff       (20)     2360 2023-04-10 14:54:23.000000 pipestream-1.0.0/pipestream/pipeline.py
-drwxr-xr-x   0 colaborador   (501) staff       (20)        0 2023-04-10 14:55:32.844702 pipestream-1.0.0/pipestream.egg-info/
--rw-r--r--   0 colaborador   (501) staff       (20)     2296 2023-04-10 14:55:32.000000 pipestream-1.0.0/pipestream.egg-info/PKG-INFO
--rw-r--r--   0 colaborador   (501) staff       (20)      237 2023-04-10 14:55:32.000000 pipestream-1.0.0/pipestream.egg-info/SOURCES.txt
--rw-r--r--   0 colaborador   (501) staff       (20)        1 2023-04-10 14:55:32.000000 pipestream-1.0.0/pipestream.egg-info/dependency_links.txt
--rw-r--r--   0 colaborador   (501) staff       (20)       11 2023-04-10 14:55:32.000000 pipestream-1.0.0/pipestream.egg-info/top_level.txt
--rw-r--r--   0 colaborador   (501) staff       (20)      635 2023-04-10 14:53:13.000000 pipestream-1.0.0/pyproject.toml
--rw-r--r--   0 colaborador   (501) staff       (20)       38 2023-04-10 14:55:32.845819 pipestream-1.0.0/setup.cfg
-drwxr-xr-x   0 colaborador   (501) staff       (20)        0 2023-04-10 14:55:32.845061 pipestream-1.0.0/tests/
--rw-r--r--   0 colaborador   (501) staff       (20)      963 2023-04-10 14:52:24.000000 pipestream-1.0.0/tests/test_pipeline.py
+drwxr-xr-x   0 colaborador   (501) staff       (20)        0 2023-04-10 15:16:35.887481 pipestream-1.0.1/
+-rw-r--r--   0 colaborador   (501) staff       (20)     1073 2023-04-10 12:28:48.000000 pipestream-1.0.1/LICENSE
+-rw-r--r--   0 colaborador   (501) staff       (20)     2330 2023-04-10 15:16:35.887284 pipestream-1.0.1/PKG-INFO
+-rw-r--r--   0 colaborador   (501) staff       (20)     1733 2023-04-10 14:54:10.000000 pipestream-1.0.1/README.md
+drwxr-xr-x   0 colaborador   (501) staff       (20)        0 2023-04-10 15:16:35.884667 pipestream-1.0.1/pipestream/
+-rw-r--r--   0 colaborador   (501) staff       (20)       30 2023-04-10 12:28:48.000000 pipestream-1.0.1/pipestream/__init__.py
+-rw-r--r--   0 colaborador   (501) staff       (20)     2360 2023-04-10 14:54:23.000000 pipestream-1.0.1/pipestream/pipeline.py
+drwxr-xr-x   0 colaborador   (501) staff       (20)        0 2023-04-10 15:16:35.886501 pipestream-1.0.1/pipestream.egg-info/
+-rw-r--r--   0 colaborador   (501) staff       (20)     2330 2023-04-10 15:16:35.000000 pipestream-1.0.1/pipestream.egg-info/PKG-INFO
+-rw-r--r--   0 colaborador   (501) staff       (20)      237 2023-04-10 15:16:35.000000 pipestream-1.0.1/pipestream.egg-info/SOURCES.txt
+-rw-r--r--   0 colaborador   (501) staff       (20)        1 2023-04-10 15:16:35.000000 pipestream-1.0.1/pipestream.egg-info/dependency_links.txt
+-rw-r--r--   0 colaborador   (501) staff       (20)       11 2023-04-10 15:16:35.000000 pipestream-1.0.1/pipestream.egg-info/top_level.txt
+-rw-r--r--   0 colaborador   (501) staff       (20)      677 2023-04-10 15:15:22.000000 pipestream-1.0.1/pyproject.toml
+-rw-r--r--   0 colaborador   (501) staff       (20)       38 2023-04-10 15:16:35.887539 pipestream-1.0.1/setup.cfg
+drwxr-xr-x   0 colaborador   (501) staff       (20)        0 2023-04-10 15:16:35.886878 pipestream-1.0.1/tests/
+-rw-r--r--   0 colaborador   (501) staff       (20)      963 2023-04-10 14:52:24.000000 pipestream-1.0.1/tests/test_pipeline.py
```

### Comparing `pipestream-1.0.0/LICENSE` & `pipestream-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pipestream-1.0.0/PKG-INFO` & `pipestream-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: pipestream
-Version: 1.0.0
+Version: 1.0.1
 Summary: A convenient way to 'pipe' a given input through a series of classes or callables
 Author-email: Rafael Acioly <aciolyr@gmail.com>
-Project-URL: Homepage, https://github.com/rafa-acioly/pypeline
-Project-URL: Bug Tracker, https://github.com/rafa-acioly/pypeline/issues
+Project-URL: Homepage, https://github.com/rafa-acioly/pipestream
+Project-URL: Bug Tracker, https://github.com/rafa-acioly/pipestream/issues
+Keywords: pipeline,middleware
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pipestream-1.0.0/README.md` & `pipestream-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pipestream-1.0.0/pipestream/pipeline.py` & `pipestream-1.0.1/pipestream/pipeline.py`

 * *Files identical despite different names*

### Comparing `pipestream-1.0.0/pipestream.egg-info/PKG-INFO` & `pipestream-1.0.1/pipestream.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: pipestream
-Version: 1.0.0
+Version: 1.0.1
 Summary: A convenient way to 'pipe' a given input through a series of classes or callables
 Author-email: Rafael Acioly <aciolyr@gmail.com>
-Project-URL: Homepage, https://github.com/rafa-acioly/pypeline
-Project-URL: Bug Tracker, https://github.com/rafa-acioly/pypeline/issues
+Project-URL: Homepage, https://github.com/rafa-acioly/pipestream
+Project-URL: Bug Tracker, https://github.com/rafa-acioly/pipestream/issues
+Keywords: pipeline,middleware
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pipestream-1.0.0/pyproject.toml` & `pipestream-1.0.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pipestream"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Rafael Acioly", email="aciolyr@gmail.com" },
 ]
 description = "A convenient way to 'pipe' a given input through a series of classes or callables"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+keywords = ["pipeline", "middleware"]
 
 [project.urls]
-"Homepage" = "https://github.com/rafa-acioly/pypeline"
-"Bug Tracker" = "https://github.com/rafa-acioly/pypeline/issues"
+"Homepage" = "https://github.com/rafa-acioly/pipestream"
+"Bug Tracker" = "https://github.com/rafa-acioly/pipestream/issues"
```

### Comparing `pipestream-1.0.0/tests/test_pipeline.py` & `pipestream-1.0.1/tests/test_pipeline.py`

 * *Files identical despite different names*

