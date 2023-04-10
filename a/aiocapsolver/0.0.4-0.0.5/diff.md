# Comparing `tmp/aiocapsolver-0.0.4.tar.gz` & `tmp/aiocapsolver-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocapsolver-0.0.4.tar", last modified: Mon Apr 10 05:12:00 2023, max compression
+gzip compressed data, was "aiocapsolver-0.0.5.tar", last modified: Mon Apr 10 09:18:24 2023, max compression
```

## Comparing `aiocapsolver-0.0.4.tar` & `aiocapsolver-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 05:12:00.458583 aiocapsolver-0.0.4/
--rw-rw-rw-   0        0        0     1088 2023-04-10 03:23:54.000000 aiocapsolver-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1284 2023-04-10 05:12:00.458583 aiocapsolver-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      627 2023-04-10 04:34:28.000000 aiocapsolver-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 05:12:00.429576 aiocapsolver-0.0.4/aiocapsolver/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:14:21.000000 aiocapsolver-0.0.4/aiocapsolver/__init__.py
--rw-rw-rw-   0        0        0     3909 2023-04-10 05:11:44.000000 aiocapsolver-0.0.4/aiocapsolver/capsolver.py
--rw-rw-rw-   0        0        0      161 2023-04-10 03:12:54.000000 aiocapsolver-0.0.4/aiocapsolver/captcha_error.py
--rw-rw-rw-   0        0        0       25 2023-04-10 03:12:54.000000 aiocapsolver-0.0.4/aiocapsolver/solution.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:12:00.455583 aiocapsolver-0.0.4/aiocapsolver.egg-info/
--rw-rw-rw-   0        0        0     1284 2023-04-10 05:12:00.000000 aiocapsolver-0.0.4/aiocapsolver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-04-10 05:12:00.000000 aiocapsolver-0.0.4/aiocapsolver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 05:12:00.000000 aiocapsolver-0.0.4/aiocapsolver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      194 2023-04-10 05:12:00.000000 aiocapsolver-0.0.4/aiocapsolver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-10 05:12:00.000000 aiocapsolver-0.0.4/aiocapsolver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 05:12:00.459584 aiocapsolver-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1403 2023-04-10 05:11:54.000000 aiocapsolver-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 09:18:24.448565 aiocapsolver-0.0.5/
+-rw-rw-rw-   0        0        0     1088 2023-04-10 03:23:54.000000 aiocapsolver-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1284 2023-04-10 09:18:24.447575 aiocapsolver-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      627 2023-04-10 04:34:28.000000 aiocapsolver-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 09:18:24.423569 aiocapsolver-0.0.5/aiocapsolver/
+-rw-rw-rw-   0        0        0        0 2023-04-10 03:14:21.000000 aiocapsolver-0.0.5/aiocapsolver/__init__.py
+-rw-rw-rw-   0        0        0     3925 2023-04-10 09:11:01.000000 aiocapsolver-0.0.5/aiocapsolver/capsolver.py
+-rw-rw-rw-   0        0        0      161 2023-04-10 03:12:54.000000 aiocapsolver-0.0.5/aiocapsolver/captcha_error.py
+-rw-rw-rw-   0        0        0       25 2023-04-10 03:12:54.000000 aiocapsolver-0.0.5/aiocapsolver/solution.py
+drwxrwxrwx   0        0        0        0 2023-04-10 09:18:24.444574 aiocapsolver-0.0.5/aiocapsolver.egg-info/
+-rw-rw-rw-   0        0        0     1284 2023-04-10 09:18:24.000000 aiocapsolver-0.0.5/aiocapsolver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-04-10 09:18:24.000000 aiocapsolver-0.0.5/aiocapsolver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 09:18:24.000000 aiocapsolver-0.0.5/aiocapsolver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      194 2023-04-10 09:18:24.000000 aiocapsolver-0.0.5/aiocapsolver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-10 09:18:24.000000 aiocapsolver-0.0.5/aiocapsolver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 09:18:24.448565 aiocapsolver-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1403 2023-04-10 09:18:16.000000 aiocapsolver-0.0.5/setup.py
```

### Comparing `aiocapsolver-0.0.4/LICENSE` & `aiocapsolver-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocapsolver-0.0.4/PKG-INFO` & `aiocapsolver-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocapsolver
-Version: 0.0.4
+Version: 0.0.5
 Summary: Async API wrapper for capsolver.com
 Home-page: UNKNOWN
 Author: Eli Chandler
 Author-email: eli.chandler@gmail.com
 License: UNKNOWN
 Keywords: python,captcha,solver,capsolver,api,wrapper
 Platform: UNKNOWN
```

### Comparing `aiocapsolver-0.0.4/README.md` & `aiocapsolver-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `aiocapsolver-0.0.4/aiocapsolver/capsolver.py` & `aiocapsolver-0.0.5/aiocapsolver/capsolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import base64
 import aiofiles
 import aiohttp
+import asyncio
 from aiocapsolver.captcha_error import CaptchaError
 
 
 class AsyncCapSolver:
     __session = None
 
     def __init__(self, api_key: str, retry_interval=0.2):
```

### Comparing `aiocapsolver-0.0.4/aiocapsolver.egg-info/PKG-INFO` & `aiocapsolver-0.0.5/aiocapsolver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocapsolver
-Version: 0.0.4
+Version: 0.0.5
 Summary: Async API wrapper for capsolver.com
 Home-page: UNKNOWN
 Author: Eli Chandler
 Author-email: eli.chandler@gmail.com
 License: UNKNOWN
 Keywords: python,captcha,solver,capsolver,api,wrapper
 Platform: UNKNOWN
```

### Comparing `aiocapsolver-0.0.4/setup.py` & `aiocapsolver-0.0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Async API wrapper for capsolver.com'
 LONG_DESCRIPTION = 'An asynchronous API wrapper for capsolver.com, built to be reliable and versatile.'
 
 # Setting up
 setup(
     name="aiocapsolver",
     version=VERSION,
```

