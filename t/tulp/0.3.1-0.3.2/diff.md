# Comparing `tmp/tulp-0.3.1.tar.gz` & `tmp/tulp-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tulp-0.3.1.tar", last modified: Sun Apr  9 15:36:48 2023, max compression
+gzip compressed data, was "tulp-0.3.2.tar", last modified: Sun Apr  9 15:39:18 2023, max compression
```

## Comparing `tulp-0.3.1.tar` & `tulp-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-04-09 15:36:48.953483 tulp-0.3.1/
--rw-rw-r--   0 fede      (1000) fede      (1000)      599 2023-04-09 15:36:48.953483 tulp-0.3.1/PKG-INFO
--rw-rw-r--   0 fede      (1000) fede      (1000)     5010 2023-04-09 15:35:50.000000 tulp-0.3.1/README.md
--rw-rw-r--   0 fede      (1000) fede      (1000)     3977 2023-04-09 15:21:27.000000 tulp-0.3.1/filteringPrompt.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     2230 2023-04-09 15:21:27.000000 tulp-0.3.1/requestPrompt.py
--rw-rw-r--   0 fede      (1000) fede      (1000)       38 2023-04-09 15:36:48.953483 tulp-0.3.1/setup.cfg
--rw-rw-r--   0 fede      (1000) fede      (1000)      857 2023-04-09 15:36:45.000000 tulp-0.3.1/setup.py
-drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-04-09 15:36:48.953483 tulp-0.3.1/tulp.egg-info/
--rw-rw-r--   0 fede      (1000) fede      (1000)      599 2023-04-09 15:36:48.000000 tulp-0.3.1/tulp.egg-info/PKG-INFO
--rw-rw-r--   0 fede      (1000) fede      (1000)      246 2023-04-09 15:36:48.000000 tulp-0.3.1/tulp.egg-info/SOURCES.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)        1 2023-04-09 15:36:48.000000 tulp-0.3.1/tulp.egg-info/dependency_links.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)       53 2023-04-09 15:36:48.000000 tulp-0.3.1/tulp.egg-info/entry_points.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)        7 2023-04-09 15:36:48.000000 tulp-0.3.1/tulp.egg-info/requires.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)       46 2023-04-09 15:36:48.000000 tulp-0.3.1/tulp.egg-info/top_level.txt
--rwxrwxr-x   0 fede      (1000) fede      (1000)     5092 2023-04-09 15:21:27.000000 tulp-0.3.1/tulp.py
--rw-rw-r--   0 fede      (1000) fede      (1000)      972 2023-04-09 15:21:27.000000 tulp-0.3.1/tulplogger.py
+drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-04-09 15:39:18.130696 tulp-0.3.2/
+-rw-rw-r--   0 fede      (1000) fede      (1000)      599 2023-04-09 15:39:18.130696 tulp-0.3.2/PKG-INFO
+-rw-rw-r--   0 fede      (1000) fede      (1000)     5010 2023-04-09 15:35:50.000000 tulp-0.3.2/README.md
+-rw-rw-r--   0 fede      (1000) fede      (1000)     3977 2023-04-09 15:21:27.000000 tulp-0.3.2/filteringPrompt.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     2230 2023-04-09 15:21:27.000000 tulp-0.3.2/requestPrompt.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)       38 2023-04-09 15:39:18.130696 tulp-0.3.2/setup.cfg
+-rw-rw-r--   0 fede      (1000) fede      (1000)      871 2023-04-09 15:39:11.000000 tulp-0.3.2/setup.py
+drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-04-09 15:39:18.130696 tulp-0.3.2/tulp.egg-info/
+-rw-rw-r--   0 fede      (1000) fede      (1000)      599 2023-04-09 15:39:18.000000 tulp-0.3.2/tulp.egg-info/PKG-INFO
+-rw-rw-r--   0 fede      (1000) fede      (1000)      260 2023-04-09 15:39:18.000000 tulp-0.3.2/tulp.egg-info/SOURCES.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)        1 2023-04-09 15:39:18.000000 tulp-0.3.2/tulp.egg-info/dependency_links.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)       53 2023-04-09 15:39:18.000000 tulp-0.3.2/tulp.egg-info/entry_points.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)        7 2023-04-09 15:39:18.000000 tulp-0.3.2/tulp.egg-info/requires.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)       57 2023-04-09 15:39:18.000000 tulp-0.3.2/tulp.egg-info/top_level.txt
+-rwxrwxr-x   0 fede      (1000) fede      (1000)     5092 2023-04-09 15:21:27.000000 tulp-0.3.2/tulp.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1008 2023-04-09 15:28:22.000000 tulp-0.3.2/tulpconfig.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)      972 2023-04-09 15:21:27.000000 tulp-0.3.2/tulplogger.py
```

### Comparing `tulp-0.3.1/PKG-INFO` & `tulp-0.3.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: tulp
-Version: 0.3.1
+Version: 0.3.2
 Summary: TULP: TULP Understands Language Perfectly
 
 A command line tool, in the best essence of POSIX tooling, that will help you to **process**, **filter**, and **create** data in this new Artificial Intelligence world.
 
 Home-page: https://github.com/fedenunez/tulp
 Author: Federico Nuñez (fedenunez)
 Author-email: fedenunez@gmail.com
```

### Comparing `tulp-0.3.1/README.md` & `tulp-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `tulp-0.3.1/filteringPrompt.py` & `tulp-0.3.2/filteringPrompt.py`

 * *Files identical despite different names*

### Comparing `tulp-0.3.1/requestPrompt.py` & `tulp-0.3.2/requestPrompt.py`

 * *Files identical despite different names*

### Comparing `tulp-0.3.1/setup.py` & `tulp-0.3.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tulp',
-    version='0.3.1',
-    py_modules=("tulp","tulplogger", "requestPrompt", "filteringPrompt"),
+    version='0.3.2',
+    py_modules=("tulp","tulplogger", "tulpconfig", "requestPrompt", "filteringPrompt"),
     install_requires=[
         'openai',
     ],
     author='Federico Nuñez (fedenunez)',
     author_email='fedenunez@gmail.com',
     maintainer='Federico Nuñez (fedenunez)',
     maintainer_email='fedenunez@gmail.com',
```

### Comparing `tulp-0.3.1/tulp.egg-info/PKG-INFO` & `tulp-0.3.2/tulp.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: tulp
-Version: 0.3.1
+Version: 0.3.2
 Summary: TULP: TULP Understands Language Perfectly
 
 A command line tool, in the best essence of POSIX tooling, that will help you to **process**, **filter**, and **create** data in this new Artificial Intelligence world.
 
 Home-page: https://github.com/fedenunez/tulp
 Author: Federico Nuñez (fedenunez)
 Author-email: fedenunez@gmail.com
```

### Comparing `tulp-0.3.1/tulp.py` & `tulp-0.3.2/tulp.py`

 * *Files identical despite different names*

### Comparing `tulp-0.3.1/tulplogger.py` & `tulp-0.3.2/tulplogger.py`

 * *Files identical despite different names*

