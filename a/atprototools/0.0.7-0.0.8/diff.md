# Comparing `tmp/atprototools-0.0.7.tar.gz` & `tmp/atprototools-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atprototools-0.0.7.tar", last modified: Sun Apr  9 22:15:56 2023, max compression
+gzip compressed data, was "atprototools-0.0.8.tar", last modified: Mon Apr 10 18:59:40 2023, max compression
```

## Comparing `atprototools-0.0.7.tar` & `atprototools-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-09 22:15:56.184135 atprototools-0.0.7/
--rw-r--r--   0 user      (1000) user      (1000)      622 2023-04-09 22:15:56.184135 atprototools-0.0.7/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      567 2023-04-09 22:14:50.000000 atprototools-0.0.7/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-09 22:15:56.184135 atprototools-0.0.7/atprototools/
--rw-r--r--   0 user      (1000) user      (1000)     2965 2023-04-09 22:14:34.000000 atprototools-0.0.7/atprototools/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-09 22:15:56.184135 atprototools-0.0.7/atprototools.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      622 2023-04-09 22:15:56.000000 atprototools-0.0.7/atprototools.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      222 2023-04-09 22:15:56.000000 atprototools-0.0.7/atprototools.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-09 22:15:56.000000 atprototools-0.0.7/atprototools.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       17 2023-04-09 22:15:56.000000 atprototools-0.0.7/atprototools.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       13 2023-04-09 22:15:56.000000 atprototools-0.0.7/atprototools.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-09 22:15:56.184135 atprototools-0.0.7/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      760 2023-04-09 22:13:54.000000 atprototools-0.0.7/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-10 18:59:40.949046 atprototools-0.0.8/
+-rw-r--r--   0 user      (1000) user      (1000)      622 2023-04-10 18:59:40.949046 atprototools-0.0.8/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      753 2023-04-10 18:59:01.000000 atprototools-0.0.8/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-10 18:59:40.949046 atprototools-0.0.8/atprototools/
+-rw-r--r--   0 user      (1000) user      (1000)     6195 2023-04-10 18:56:45.000000 atprototools-0.0.8/atprototools/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-10 18:59:40.949046 atprototools-0.0.8/atprototools.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      622 2023-04-10 18:59:40.000000 atprototools-0.0.8/atprototools.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      222 2023-04-10 18:59:40.000000 atprototools-0.0.8/atprototools.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-10 18:59:40.000000 atprototools-0.0.8/atprototools.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       17 2023-04-10 18:59:40.000000 atprototools-0.0.8/atprototools.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       13 2023-04-10 18:59:40.000000 atprototools-0.0.8/atprototools.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-10 18:59:40.949046 atprototools-0.0.8/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      760 2023-04-10 18:59:04.000000 atprototools-0.0.8/setup.py
```

### Comparing `atprototools-0.0.7/PKG-INFO` & `atprototools-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: atprototools
-Version: 0.0.7
+Version: 0.0.8
 Summary: tools for posting / deleting things from bsky, in python
 Home-page: https://github.com/ianklatzco/atprototools
 Author: Ian Klatzco
 Author-email: iklatzco@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `atprototools-0.0.7/README.md` & `atprototools-0.0.8/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -3,31 +3,35 @@
 A couple of functions for making/deleting posts, packaged so you can `pip
 install` and go.
 
 Usage:
 
 ```bash
 pip install atprototools
-export BSKY_USERAME="yourname.bsky.social"
-export PASSWORD="yourpassword"
+export BSKY_USERNAME="yourname.bsky.social"
+export BSKY_PASSWORD="yourpassword"
 ```
 
 ```python
 import atprototools as atpt
 import os
 
 USERNAME = os.environ.get("BSKY_USERNAME")
 PASSWORD = os.environ.get("PASSWORD")
 
 atpt.login(USERNAME, PASSWORD)
 atpt.post_skoot("hello world from atprototools")
+latest_skoots = atpt.get_latest_n_skoots('klatz.co',1).content
+carfile = atpt.get_car_file().content
 ```
 
 PEP8 formatted; use autopep8.
 
 ### changelog
 
-0.0.7: getRepo (car files) and get_latest_n_skoots
+- 0.0.8: get_skoot_by_url, reskoot
+- 0.0.7: getRepo (car files) and get_latest_n_skoots
 
 ### Thanks to 
 
 - alice
+- [sirodoht](https://github.com/sirodoht)
```

### Comparing `atprototools-0.0.7/atprototools.egg-info/PKG-INFO` & `atprototools-0.0.8/atprototools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: atprototools
-Version: 0.0.7
+Version: 0.0.8
 Summary: tools for posting / deleting things from bsky, in python
 Home-page: https://github.com/ianklatzco/atprototools
 Author: Ian Klatzco
 Author-email: iklatzco@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `atprototools-0.0.7/setup.py` & `atprototools-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='atprototools',
-    version='0.0.7',
+    version='0.0.8',
     description='tools for posting / deleting things from bsky, in python',
     author='Ian Klatzco',
     author_email='iklatzco@gmail.com',
     url='https://github.com/ianklatzco/atprototools',
     packages=find_packages(),
     install_requires=[
         'requests>=2.22.0'
```

