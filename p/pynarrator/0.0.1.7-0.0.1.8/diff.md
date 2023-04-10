# Comparing `tmp/pynarrator-0.0.1.7.tar.gz` & `tmp/pynarrator-0.0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynarrator-0.0.1.7.tar", last modified: Sat Apr  8 19:49:25 2023, max compression
+gzip compressed data, was "pynarrator-0.0.1.8.tar", last modified: Mon Apr 10 06:14:00 2023, max compression
```

## Comparing `pynarrator-0.0.1.7.tar` & `pynarrator-0.0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 denisabdullin   (501) staff       (20)        0 2023-04-08 19:49:25.333199 pynarrator-0.0.1.7/
--rw-r--r--   0 denisabdullin   (501) staff       (20)     1071 2023-03-01 20:23:53.000000 pynarrator-0.0.1.7/LICENSE
--rw-r--r--   0 denisabdullin   (501) staff       (20)     1740 2023-04-08 19:49:25.333073 pynarrator-0.0.1.7/PKG-INFO
--rw-r--r--   0 denisabdullin   (501) staff       (20)      968 2023-04-08 18:46:26.000000 pynarrator-0.0.1.7/README.md
--rw-r--r--   0 denisabdullin   (501) staff       (20)       38 2023-04-08 19:49:25.333234 pynarrator-0.0.1.7/setup.cfg
--rw-r--r--   0 denisabdullin   (501) staff       (20)     1166 2023-04-08 19:49:19.000000 pynarrator-0.0.1.7/setup.py
-drwxr-xr-x   0 denisabdullin   (501) staff       (20)        0 2023-04-08 19:49:25.331831 pynarrator-0.0.1.7/src/
-drwxr-xr-x   0 denisabdullin   (501) staff       (20)        0 2023-04-08 19:49:25.332806 pynarrator-0.0.1.7/src/pynarrator.egg-info/
--rw-r--r--   0 denisabdullin   (501) staff       (20)     1740 2023-04-08 19:49:25.000000 pynarrator-0.0.1.7/src/pynarrator.egg-info/PKG-INFO
--rw-r--r--   0 denisabdullin   (501) staff       (20)      249 2023-04-08 19:49:25.000000 pynarrator-0.0.1.7/src/pynarrator.egg-info/SOURCES.txt
--rw-r--r--   0 denisabdullin   (501) staff       (20)        1 2023-04-08 19:49:25.000000 pynarrator-0.0.1.7/src/pynarrator.egg-info/dependency_links.txt
--rw-r--r--   0 denisabdullin   (501) staff       (20)       55 2023-04-08 19:49:25.000000 pynarrator-0.0.1.7/src/pynarrator.egg-info/requires.txt
--rw-r--r--   0 denisabdullin   (501) staff       (20)       43 2023-04-08 19:49:25.000000 pynarrator-0.0.1.7/src/pynarrator.egg-info/top_level.txt
-drwxr-xr-x   0 denisabdullin   (501) staff       (20)        0 2023-04-08 19:49:25.332910 pynarrator-0.0.1.7/tests/
--rw-r--r--   0 denisabdullin   (501) staff       (20)       68 2023-03-02 10:10:10.000000 pynarrator-0.0.1.7/tests/test_narrate_descriptive.py
+drwxr-xr-x   0 denisabdullin   (501) staff       (20)        0 2023-04-10 06:14:00.779440 pynarrator-0.0.1.8/
+-rw-r--r--   0 denisabdullin   (501) staff       (20)     1071 2023-03-01 20:23:53.000000 pynarrator-0.0.1.8/LICENSE
+-rw-r--r--   0 denisabdullin   (501) staff       (20)     1740 2023-04-10 06:14:00.779323 pynarrator-0.0.1.8/PKG-INFO
+-rw-r--r--   0 denisabdullin   (501) staff       (20)      968 2023-04-08 18:46:26.000000 pynarrator-0.0.1.8/README.md
+-rw-r--r--   0 denisabdullin   (501) staff       (20)       38 2023-04-10 06:14:00.779480 pynarrator-0.0.1.8/setup.cfg
+-rw-r--r--   0 denisabdullin   (501) staff       (20)     1166 2023-04-10 06:11:04.000000 pynarrator-0.0.1.8/setup.py
+drwxr-xr-x   0 denisabdullin   (501) staff       (20)        0 2023-04-10 06:14:00.777863 pynarrator-0.0.1.8/src/
+drwxr-xr-x   0 denisabdullin   (501) staff       (20)        0 2023-04-10 06:14:00.778924 pynarrator-0.0.1.8/src/pynarrator.egg-info/
+-rw-r--r--   0 denisabdullin   (501) staff       (20)     1740 2023-04-10 06:14:00.000000 pynarrator-0.0.1.8/src/pynarrator.egg-info/PKG-INFO
+-rw-r--r--   0 denisabdullin   (501) staff       (20)      249 2023-04-10 06:14:00.000000 pynarrator-0.0.1.8/src/pynarrator.egg-info/SOURCES.txt
+-rw-r--r--   0 denisabdullin   (501) staff       (20)        1 2023-04-10 06:14:00.000000 pynarrator-0.0.1.8/src/pynarrator.egg-info/dependency_links.txt
+-rw-r--r--   0 denisabdullin   (501) staff       (20)       55 2023-04-10 06:14:00.000000 pynarrator-0.0.1.8/src/pynarrator.egg-info/requires.txt
+-rw-r--r--   0 denisabdullin   (501) staff       (20)       43 2023-04-10 06:14:00.000000 pynarrator-0.0.1.8/src/pynarrator.egg-info/top_level.txt
+drwxr-xr-x   0 denisabdullin   (501) staff       (20)        0 2023-04-10 06:14:00.779038 pynarrator-0.0.1.8/tests/
+-rw-r--r--   0 denisabdullin   (501) staff       (20)       68 2023-03-02 10:10:10.000000 pynarrator-0.0.1.8/tests/test_narrate_descriptive.py
```

### Comparing `pynarrator-0.0.1.7/LICENSE` & `pynarrator-0.0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pynarrator-0.0.1.7/PKG-INFO` & `pynarrator-0.0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynarrator
-Version: 0.0.1.7
+Version: 0.0.1.8
 Summary: Template-based NLG framework for creating text narratives out of data
 Home-page: UNKNOWN
 Author: Denis Abdullin
 Author-email: denisabdullincz@gmail.com
 License: UNKNOWN
 Keywords: python,nlg,template,chatgpt
 Platform: UNKNOWN
```

### Comparing `pynarrator-0.0.1.7/README.md` & `pynarrator-0.0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pynarrator-0.0.1.7/setup.py` & `pynarrator-0.0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open('README.md', 'r') as fh:
    long_description = fh.read()
   
 setup(
   name = 'pynarrator',
-  version = '0.0.1.7',
+  version = '0.0.1.8',
   author = 'Denis Abdullin',
   author_email = 'denisabdullincz@gmail.com',
   description = 'Template-based NLG framework for creating text narratives out of data',
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   py_modules = [
     'narrate_descriptive',
```

### Comparing `pynarrator-0.0.1.7/src/pynarrator.egg-info/PKG-INFO` & `pynarrator-0.0.1.8/src/pynarrator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynarrator
-Version: 0.0.1.7
+Version: 0.0.1.8
 Summary: Template-based NLG framework for creating text narratives out of data
 Home-page: UNKNOWN
 Author: Denis Abdullin
 Author-email: denisabdullincz@gmail.com
 License: UNKNOWN
 Keywords: python,nlg,template,chatgpt
 Platform: UNKNOWN
```

