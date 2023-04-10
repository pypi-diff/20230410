# Comparing `tmp/aiocapsolver-0.0.3.tar.gz` & `tmp/aiocapsolver-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocapsolver-0.0.3.tar", last modified: Mon Apr 10 05:06:40 2023, max compression
+gzip compressed data, was "aiocapsolver-0.0.4.tar", last modified: Mon Apr 10 05:12:00 2023, max compression
```

## Comparing `aiocapsolver-0.0.3.tar` & `aiocapsolver-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 05:06:40.829039 aiocapsolver-0.0.3/
--rw-rw-rw-   0        0        0     1088 2023-04-10 03:23:54.000000 aiocapsolver-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1284 2023-04-10 05:06:40.828039 aiocapsolver-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      627 2023-04-10 04:34:28.000000 aiocapsolver-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 05:06:40.791030 aiocapsolver-0.0.3/aiocapsolver/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:14:21.000000 aiocapsolver-0.0.3/aiocapsolver/__init__.py
--rw-rw-rw-   0        0        0     3896 2023-04-10 04:52:41.000000 aiocapsolver-0.0.3/aiocapsolver/capsolver.py
--rw-rw-rw-   0        0        0      161 2023-04-10 03:12:54.000000 aiocapsolver-0.0.3/aiocapsolver/captcha_error.py
--rw-rw-rw-   0        0        0       25 2023-04-10 03:12:54.000000 aiocapsolver-0.0.3/aiocapsolver/solution.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:06:40.825038 aiocapsolver-0.0.3/aiocapsolver.egg-info/
--rw-rw-rw-   0        0        0     1284 2023-04-10 05:06:40.000000 aiocapsolver-0.0.3/aiocapsolver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-04-10 05:06:40.000000 aiocapsolver-0.0.3/aiocapsolver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 05:06:40.000000 aiocapsolver-0.0.3/aiocapsolver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      194 2023-04-10 05:06:40.000000 aiocapsolver-0.0.3/aiocapsolver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-10 05:06:40.000000 aiocapsolver-0.0.3/aiocapsolver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 05:06:40.829039 aiocapsolver-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1403 2023-04-10 05:06:25.000000 aiocapsolver-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:12:00.458583 aiocapsolver-0.0.4/
+-rw-rw-rw-   0        0        0     1088 2023-04-10 03:23:54.000000 aiocapsolver-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1284 2023-04-10 05:12:00.458583 aiocapsolver-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      627 2023-04-10 04:34:28.000000 aiocapsolver-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 05:12:00.429576 aiocapsolver-0.0.4/aiocapsolver/
+-rw-rw-rw-   0        0        0        0 2023-04-10 03:14:21.000000 aiocapsolver-0.0.4/aiocapsolver/__init__.py
+-rw-rw-rw-   0        0        0     3909 2023-04-10 05:11:44.000000 aiocapsolver-0.0.4/aiocapsolver/capsolver.py
+-rw-rw-rw-   0        0        0      161 2023-04-10 03:12:54.000000 aiocapsolver-0.0.4/aiocapsolver/captcha_error.py
+-rw-rw-rw-   0        0        0       25 2023-04-10 03:12:54.000000 aiocapsolver-0.0.4/aiocapsolver/solution.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:12:00.455583 aiocapsolver-0.0.4/aiocapsolver.egg-info/
+-rw-rw-rw-   0        0        0     1284 2023-04-10 05:12:00.000000 aiocapsolver-0.0.4/aiocapsolver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-04-10 05:12:00.000000 aiocapsolver-0.0.4/aiocapsolver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 05:12:00.000000 aiocapsolver-0.0.4/aiocapsolver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      194 2023-04-10 05:12:00.000000 aiocapsolver-0.0.4/aiocapsolver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-10 05:12:00.000000 aiocapsolver-0.0.4/aiocapsolver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 05:12:00.459584 aiocapsolver-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1403 2023-04-10 05:11:54.000000 aiocapsolver-0.0.4/setup.py
```

### Comparing `aiocapsolver-0.0.3/LICENSE` & `aiocapsolver-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocapsolver-0.0.3/PKG-INFO` & `aiocapsolver-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocapsolver
-Version: 0.0.3
+Version: 0.0.4
 Summary: Async API wrapper for capsolver.com
 Home-page: UNKNOWN
 Author: Eli Chandler
 Author-email: eli.chandler@gmail.com
 License: UNKNOWN
 Keywords: python,captcha,solver,capsolver,api,wrapper
 Platform: UNKNOWN
```

### Comparing `aiocapsolver-0.0.3/README.md` & `aiocapsolver-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `aiocapsolver-0.0.3/aiocapsolver/capsolver.py` & `aiocapsolver-0.0.4/aiocapsolver/capsolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import base64
 import aiofiles
 import aiohttp
-from captcha_error import CaptchaError
+from aiocapsolver.captcha_error import CaptchaError
 
 
 class AsyncCapSolver:
     __session = None
 
     def __init__(self, api_key: str, retry_interval=0.2):
         self.api_key = api_key
```

### Comparing `aiocapsolver-0.0.3/aiocapsolver.egg-info/PKG-INFO` & `aiocapsolver-0.0.4/aiocapsolver.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocapsolver
-Version: 0.0.3
+Version: 0.0.4
 Summary: Async API wrapper for capsolver.com
 Home-page: UNKNOWN
 Author: Eli Chandler
 Author-email: eli.chandler@gmail.com
 License: UNKNOWN
 Keywords: python,captcha,solver,capsolver,api,wrapper
 Platform: UNKNOWN
```

### Comparing `aiocapsolver-0.0.3/setup.py` & `aiocapsolver-0.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Async API wrapper for capsolver.com'
 LONG_DESCRIPTION = 'An asynchronous API wrapper for capsolver.com, built to be reliable and versatile.'
 
 # Setting up
 setup(
     name="aiocapsolver",
     version=VERSION,
```

