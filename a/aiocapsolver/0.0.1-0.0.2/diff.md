# Comparing `tmp/aiocapsolver-0.0.1.tar.gz` & `tmp/aiocapsolver-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocapsolver-0.0.1.tar", last modified: Mon Apr 10 04:32:18 2023, max compression
+gzip compressed data, was "aiocapsolver-0.0.2.tar", last modified: Mon Apr 10 04:40:22 2023, max compression
```

## Comparing `aiocapsolver-0.0.1.tar` & `aiocapsolver-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 04:32:18.784835 aiocapsolver-0.0.1/
--rw-rw-rw-   0        0        0     1088 2023-04-10 03:23:54.000000 aiocapsolver-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1134 2023-04-10 04:32:18.784835 aiocapsolver-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      539 2023-04-10 04:27:53.000000 aiocapsolver-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 04:32:18.765829 aiocapsolver-0.0.1/aiocapsolver/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:14:21.000000 aiocapsolver-0.0.1/aiocapsolver/__init__.py
--rw-rw-rw-   0        0        0     3761 2023-04-10 04:13:32.000000 aiocapsolver-0.0.1/aiocapsolver/capsolver.py
--rw-rw-rw-   0        0        0      161 2023-04-10 03:12:54.000000 aiocapsolver-0.0.1/aiocapsolver/captcha_error.py
--rw-rw-rw-   0        0        0       25 2023-04-10 03:12:54.000000 aiocapsolver-0.0.1/aiocapsolver/solution.py
-drwxrwxrwx   0        0        0        0 2023-04-10 04:32:18.781836 aiocapsolver-0.0.1/aiocapsolver.egg-info/
--rw-rw-rw-   0        0        0     1134 2023-04-10 04:32:18.000000 aiocapsolver-0.0.1/aiocapsolver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-04-10 04:32:18.000000 aiocapsolver-0.0.1/aiocapsolver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 04:32:18.000000 aiocapsolver-0.0.1/aiocapsolver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      152 2023-04-10 04:32:18.000000 aiocapsolver-0.0.1/aiocapsolver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-10 04:32:18.000000 aiocapsolver-0.0.1/aiocapsolver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 04:32:18.785835 aiocapsolver-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1319 2023-04-10 04:32:06.000000 aiocapsolver-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 04:40:22.127786 aiocapsolver-0.0.2/
+-rw-rw-rw-   0        0        0     1088 2023-04-10 03:23:54.000000 aiocapsolver-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1284 2023-04-10 04:40:22.126785 aiocapsolver-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      627 2023-04-10 04:34:28.000000 aiocapsolver-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 04:40:22.100777 aiocapsolver-0.0.2/aiocapsolver/
+-rw-rw-rw-   0        0        0        0 2023-04-10 03:14:21.000000 aiocapsolver-0.0.2/aiocapsolver/__init__.py
+-rw-rw-rw-   0        0        0     3761 2023-04-10 04:13:32.000000 aiocapsolver-0.0.2/aiocapsolver/capsolver.py
+-rw-rw-rw-   0        0        0      161 2023-04-10 03:12:54.000000 aiocapsolver-0.0.2/aiocapsolver/captcha_error.py
+-rw-rw-rw-   0        0        0       25 2023-04-10 03:12:54.000000 aiocapsolver-0.0.2/aiocapsolver/solution.py
+drwxrwxrwx   0        0        0        0 2023-04-10 04:40:22.123793 aiocapsolver-0.0.2/aiocapsolver.egg-info/
+-rw-rw-rw-   0        0        0     1284 2023-04-10 04:40:21.000000 aiocapsolver-0.0.2/aiocapsolver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-04-10 04:40:22.000000 aiocapsolver-0.0.2/aiocapsolver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 04:40:21.000000 aiocapsolver-0.0.2/aiocapsolver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      194 2023-04-10 04:40:21.000000 aiocapsolver-0.0.2/aiocapsolver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-10 04:40:21.000000 aiocapsolver-0.0.2/aiocapsolver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 04:40:22.128784 aiocapsolver-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1403 2023-04-10 04:37:50.000000 aiocapsolver-0.0.2/setup.py
```

### Comparing `aiocapsolver-0.0.1/LICENSE` & `aiocapsolver-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocapsolver-0.0.1/aiocapsolver/capsolver.py` & `aiocapsolver-0.0.2/aiocapsolver/capsolver.py`

 * *Files identical despite different names*

### Comparing `aiocapsolver-0.0.1/setup.py` & `aiocapsolver-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from setuptools import setup, find_packages
 import codecs
 import os
 
+from setuptools import setup, find_packages
+
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Async API wrapper for capsolver.com'
 LONG_DESCRIPTION = 'An asynchronous API wrapper for capsolver.com, built to be reliable and versatile.'
 
 # Setting up
 setup(
     name="aiocapsolver",
     version=VERSION,
     author="Eli Chandler",
     author_email="eli.chandler@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['async-timeout', 'build', 'certifi', 'charset-normalizer', 'colorama', 'filelock', 'idna', 'packaging', 'platformdirs', 'pyproject_hooks', 'requests', 'tomli', 'uritools', 'urlextract', 'urllib3'],
+    install_requires=['aiofiles', 'aiohttp', 'aiosignal', 'async-timeout', 'attrs', 'build', 'charset-normalizer', 'colorama', 'filelock', 'frozenlist', 'idna', 'multidict', 'packaging',
+                      'platformdirs', 'pyproject-hooks', 'tomli', 'uritools', 'urlextract', 'urllib3', 'yarl'],
     keywords=['python', 'captcha', 'solver', 'capsolver', 'api', 'wrapper'],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
-)
+)
```

