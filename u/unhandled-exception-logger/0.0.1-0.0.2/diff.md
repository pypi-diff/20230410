# Comparing `tmp/unhandled_exception_logger-0.0.1.tar.gz` & `tmp/unhandled_exception_logger-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unhandled_exception_logger-0.0.1.tar", last modified: Sun Apr  9 16:33:04 2023, max compression
+gzip compressed data, was "unhandled_exception_logger-0.0.2.tar", last modified: Sun Apr  9 16:39:42 2023, max compression
```

## Comparing `unhandled_exception_logger-0.0.1.tar` & `unhandled_exception_logger-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-04-09 16:33:04.233006 unhandled_exception_logger-0.0.1/
--rw-rw-r--   0 chris     (1000) chris     (1000)      734 2023-04-09 16:33:04.233006 unhandled_exception_logger-0.0.1/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      337 2023-04-09 15:48:19.000000 unhandled_exception_logger-0.0.1/README.md
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2023-04-09 16:33:04.233006 unhandled_exception_logger-0.0.1/setup.cfg
--rw-rw-r--   0 chris     (1000) chris     (1000)      584 2023-04-09 16:05:22.000000 unhandled_exception_logger-0.0.1/setup.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-04-09 16:33:04.233006 unhandled_exception_logger-0.0.1/unhandled_exception_logger.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)      734 2023-04-09 16:33:04.000000 unhandled_exception_logger-0.0.1/unhandled_exception_logger.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      248 2023-04-09 16:33:04.000000 unhandled_exception_logger-0.0.1/unhandled_exception_logger.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-04-09 16:33:04.000000 unhandled_exception_logger-0.0.1/unhandled_exception_logger.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       27 2023-04-09 16:33:04.000000 unhandled_exception_logger-0.0.1/unhandled_exception_logger.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      763 2023-04-09 16:31:17.000000 unhandled_exception_logger-0.0.1/unhandled_exception_logger.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-04-09 16:39:42.896582 unhandled_exception_logger-0.0.2/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      734 2023-04-09 16:39:42.896582 unhandled_exception_logger-0.0.2/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      337 2023-04-09 16:37:19.000000 unhandled_exception_logger-0.0.2/README.md
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2023-04-09 16:39:42.896582 unhandled_exception_logger-0.0.2/setup.cfg
+-rw-rw-r--   0 chris     (1000) chris     (1000)      584 2023-04-09 16:39:28.000000 unhandled_exception_logger-0.0.2/setup.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-04-09 16:39:42.896582 unhandled_exception_logger-0.0.2/unhandled_exception_logger.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      734 2023-04-09 16:39:42.000000 unhandled_exception_logger-0.0.2/unhandled_exception_logger.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      248 2023-04-09 16:39:42.000000 unhandled_exception_logger-0.0.2/unhandled_exception_logger.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-04-09 16:39:42.000000 unhandled_exception_logger-0.0.2/unhandled_exception_logger.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       27 2023-04-09 16:39:42.000000 unhandled_exception_logger-0.0.2/unhandled_exception_logger.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      763 2023-04-09 16:31:17.000000 unhandled_exception_logger-0.0.2/unhandled_exception_logger.py
```

### Comparing `unhandled_exception_logger-0.0.1/setup.py` & `unhandled_exception_logger-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 
 with open("README.md", "r") as fp:
     README = fp.read()
 
 setup(
     name="unhandled_exception_logger",
     version=VERSION,
```

### Comparing `unhandled_exception_logger-0.0.1/unhandled_exception_logger.egg-info/PKG-INFO` & `unhandled_exception_logger-0.0.2/unhandled_exception_logger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unhandled-exception-logger
-Version: 0.0.1
+Version: 0.0.2
 Summary: Log unhandled exceptions as critical
 Home-page: https://github.com/karmacomputing/unhandled_exception
 Author: Chris Simpson
 Author-email: oss@karmacomputing.co.uk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -13,15 +13,15 @@
 # Log Unhandled Exceptions
 
 This package will log unhandled exceptions as a critical error.
 
 # Install
 
 ```
-pip install unhandled_exception_logger
+pip install unhandled-exception-logger
 ```
 
 # Usage
 
 ```
 from unhandled_exception_logger import unhandled_exception_setup
```

### Comparing `unhandled_exception_logger-0.0.1/unhandled_exception_logger.py` & `unhandled_exception_logger-0.0.2/unhandled_exception_logger.py`

 * *Files identical despite different names*

