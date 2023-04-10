# Comparing `tmp/chunked-uploads-attentive-0.0.1.tar.gz` & `tmp/chunked-uploads-attentive-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chunked-uploads-attentive-0.0.1.tar", last modified: Mon Apr  3 19:28:34 2023, max compression
+gzip compressed data, was "chunked-uploads-attentive-0.0.2.tar", last modified: Mon Apr 10 10:31:39 2023, max compression
```

## Comparing `chunked-uploads-attentive-0.0.1.tar` & `chunked-uploads-attentive-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 19:28:34.485827 chunked-uploads-attentive-0.0.1/
--rw-rw-rw-   0        0        0      583 2023-04-03 19:28:34.438879 chunked-uploads-attentive-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-03 19:28:34.423251 chunked-uploads-attentive-0.0.1/chunked_uploads_attentive.egg-info/
--rw-rw-rw-   0        0        0      583 2023-04-03 19:28:34.000000 chunked-uploads-attentive-0.0.1/chunked_uploads_attentive.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-04-03 19:28:34.000000 chunked-uploads-attentive-0.0.1/chunked_uploads_attentive.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 19:28:34.000000 chunked-uploads-attentive-0.0.1/chunked_uploads_attentive.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-04-03 19:28:34.000000 chunked-uploads-attentive-0.0.1/chunked_uploads_attentive.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 19:28:34.000000 chunked-uploads-attentive-0.0.1/chunked_uploads_attentive.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-03 19:28:34.485827 chunked-uploads-attentive-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      940 2023-04-03 19:26:06.000000 chunked-uploads-attentive-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:31:39.836020 chunked-uploads-attentive-0.0.2/
+-rw-rw-rw-   0        0        0      583 2023-04-10 10:31:39.835019 chunked-uploads-attentive-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 10:31:39.834033 chunked-uploads-attentive-0.0.2/chunked_uploads_attentive.egg-info/
+-rw-rw-rw-   0        0        0      583 2023-04-10 10:31:39.000000 chunked-uploads-attentive-0.0.2/chunked_uploads_attentive.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-04-10 10:31:39.000000 chunked-uploads-attentive-0.0.2/chunked_uploads_attentive.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 10:31:39.000000 chunked-uploads-attentive-0.0.2/chunked_uploads_attentive.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-04-10 10:31:39.000000 chunked-uploads-attentive-0.0.2/chunked_uploads_attentive.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 10:31:39.000000 chunked-uploads-attentive-0.0.2/chunked_uploads_attentive.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 10:31:39.836020 chunked-uploads-attentive-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      940 2023-04-10 10:30:31.000000 chunked-uploads-attentive-0.0.2/setup.py
```

### Comparing `chunked-uploads-attentive-0.0.1/PKG-INFO` & `chunked-uploads-attentive-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chunked-uploads-attentive
-Version: 0.0.1
+Version: 0.0.2
 Summary: Chunked Upload of files on gcs using Django
 Author: Ayion
 Author-email: <ayan@attentive.ai>
 Keywords: python,file,transfer,chunk,chunks,upload
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `chunked-uploads-attentive-0.0.1/chunked_uploads_attentive.egg-info/PKG-INFO` & `chunked-uploads-attentive-0.0.2/chunked_uploads_attentive.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chunked-uploads-attentive
-Version: 0.0.1
+Version: 0.0.2
 Summary: Chunked Upload of files on gcs using Django
 Author: Ayion
 Author-email: <ayan@attentive.ai>
 Keywords: python,file,transfer,chunk,chunks,upload
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `chunked-uploads-attentive-0.0.1/setup.py` & `chunked-uploads-attentive-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Chunked Upload of files on gcs using Django'
 LONG_DESCRIPTION = 'A package that allows to transfer files and resume in case of data failure'
 
 # Setting up
 setup(
     name="chunked-uploads-attentive",
     version=VERSION,
```

