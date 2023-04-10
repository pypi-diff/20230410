# Comparing `tmp/watchful-3.0.0.tar.gz` & `tmp/watchful-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchful-3.0.0.tar", last modified: Mon Apr 10 11:02:11 2023, max compression
+gzip compressed data, was "watchful-3.5.0.tar", last modified: Thu Apr  6 12:17:55 2023, max compression
```

## Comparing `watchful-3.0.0.tar` & `watchful-3.5.0.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 runyan     (501) staff       (20)        0 2023-04-10 11:02:11.218897 watchful-3.0.0/
--rw-r--r--   0 runyan     (501) staff       (20)     1075 2022-10-13 18:29:08.000000 watchful-3.0.0/LICENSE
--rw-r--r--   0 runyan     (501) staff       (20)      261 2022-11-15 05:56:43.000000 watchful-3.0.0/MANIFEST.in
--rw-r--r--   0 runyan     (501) staff       (20)     2650 2023-04-10 11:02:11.219024 watchful-3.0.0/PKG-INFO
--rw-r--r--   0 runyan     (501) staff       (20)     6405 2023-03-30 16:02:18.000000 watchful-3.0.0/README.md
--rw-r--r--   0 runyan     (501) staff       (20)     2064 2023-04-03 13:27:13.000000 watchful-3.0.0/README_PYPI.md
--rw-r--r--   0 runyan     (501) staff       (20)     1554 2023-03-30 16:02:18.000000 watchful-3.0.0/README_PY_ENV.md
-drwxr-xr-x   0 runyan     (501) staff       (20)        0 2023-04-10 11:02:11.210581 watchful-3.0.0/examples/
--rw-r--r--   0 runyan     (501) staff       (20)   325333 2023-04-06 11:52:46.000000 watchful-3.0.0/examples/api_intro.ipynb
--rw-r--r--   0 runyan     (501) staff       (20)     1900 2023-04-06 11:52:46.000000 watchful-3.0.0/examples/requirements_api_intro.txt
--rw-r--r--   0 runyan     (501) staff       (20)      998 2023-04-03 13:27:13.000000 watchful-3.0.0/pylama.ini
--rw-r--r--   0 runyan     (501) staff       (20)      375 2022-10-13 18:29:08.000000 watchful-3.0.0/pyproject.toml
--rw-r--r--   0 runyan     (501) staff       (20)      983 2023-04-10 11:02:11.219604 watchful-3.0.0/setup.cfg
-drwxr-xr-x   0 runyan     (501) staff       (20)        0 2023-04-10 11:02:11.203264 watchful-3.0.0/src/
-drwxr-xr-x   0 runyan     (501) staff       (20)        0 2023-04-10 11:02:11.215002 watchful-3.0.0/src/watchful/
--rw-r--r--   0 runyan     (501) staff       (20)        5 2023-04-10 11:00:16.000000 watchful-3.0.0/src/watchful/VERSION
--rw-r--r--   0 runyan     (501) staff       (20)      575 2022-11-15 05:56:43.000000 watchful-3.0.0/src/watchful/__init__.py
--rw-r--r--   0 runyan     (501) staff       (20)    39332 2023-04-06 11:52:46.000000 watchful-3.0.0/src/watchful/attributes.py
--rw-r--r--   0 runyan     (501) staff       (20)    48367 2023-04-03 13:27:13.000000 watchful-3.0.0/src/watchful/client.py
--rw-r--r--   0 runyan     (501) staff       (20)    15767 2023-04-06 11:52:46.000000 watchful-3.0.0/src/watchful/enrich.py
--rw-r--r--   0 runyan     (501) staff       (20)     6356 2023-04-06 11:52:46.000000 watchful-3.0.0/src/watchful/enricher.py
-drwxr-xr-x   0 runyan     (501) staff       (20)        0 2023-04-10 11:02:11.216509 watchful-3.0.0/src/watchful.egg-info/
--rw-r--r--   0 runyan     (501) staff       (20)     2650 2023-04-10 11:02:11.000000 watchful-3.0.0/src/watchful.egg-info/PKG-INFO
--rw-r--r--   0 runyan     (501) staff       (20)      615 2023-04-10 11:02:11.000000 watchful-3.0.0/src/watchful.egg-info/SOURCES.txt
--rw-r--r--   0 runyan     (501) staff       (20)        1 2023-04-10 11:02:11.000000 watchful-3.0.0/src/watchful.egg-info/dependency_links.txt
--rw-r--r--   0 runyan     (501) staff       (20)       93 2023-04-10 11:02:11.000000 watchful-3.0.0/src/watchful.egg-info/requires.txt
--rw-r--r--   0 runyan     (501) staff       (20)        9 2023-04-10 11:02:11.000000 watchful-3.0.0/src/watchful.egg-info/top_level.txt
-drwxr-xr-x   0 runyan     (501) staff       (20)        0 2023-04-10 11:02:11.218264 watchful-3.0.0/tests/
--rwxr-xr-x   0 runyan     (501) staff       (20)      388 2022-12-15 14:22:48.000000 watchful-3.0.0/tests/test_0000_import_sdk.py
--rw-r--r--   0 runyan     (501) staff       (20)     2691 2023-04-03 13:27:13.000000 watchful-3.0.0/tests/test_0001_sdk_version_and_default_conn.py
--rw-r--r--   0 runyan     (501) staff       (20)      772 2023-03-30 16:02:18.000000 watchful-3.0.0/tests/test_0002_encoding.py
--rw-r--r--   0 runyan     (501) staff       (20)     2145 2022-12-15 11:06:56.000000 watchful-3.0.0/tests/test_0003_enricher.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 12:17:55.945730 watchful-3.5.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-04-06 12:14:03.000000 watchful-3.5.0/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      261 2023-04-06 12:14:03.000000 watchful-3.5.0/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2650 2023-04-06 12:17:55.945730 watchful-3.5.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6405 2023-04-06 12:14:03.000000 watchful-3.5.0/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2064 2023-04-06 12:14:03.000000 watchful-3.5.0/README_PYPI.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1554 2023-04-06 12:14:03.000000 watchful-3.5.0/README_PY_ENV.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 12:17:55.945730 watchful-3.5.0/examples/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   325333 2023-04-06 12:14:03.000000 watchful-3.5.0/examples/api_intro.ipynb
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1900 2023-04-06 12:14:03.000000 watchful-3.5.0/examples/requirements_api_intro.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      998 2023-04-06 12:14:03.000000 watchful-3.5.0/pylama.ini
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      375 2023-04-06 12:14:03.000000 watchful-3.5.0/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      983 2023-04-06 12:17:55.949730 watchful-3.5.0/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 12:17:55.941730 watchful-3.5.0/src/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 12:17:55.945730 watchful-3.5.0/src/watchful/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2023-04-06 12:14:03.000000 watchful-3.5.0/src/watchful/VERSION
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      575 2023-04-06 12:14:03.000000 watchful-3.5.0/src/watchful/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    39332 2023-04-06 12:14:03.000000 watchful-3.5.0/src/watchful/attributes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    48367 2023-04-06 12:14:03.000000 watchful-3.5.0/src/watchful/client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15767 2023-04-06 12:14:03.000000 watchful-3.5.0/src/watchful/enrich.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6356 2023-04-06 12:14:03.000000 watchful-3.5.0/src/watchful/enricher.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 12:17:55.945730 watchful-3.5.0/src/watchful.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2650 2023-04-06 12:17:55.000000 watchful-3.5.0/src/watchful.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      587 2023-04-06 12:17:55.000000 watchful-3.5.0/src/watchful.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-06 12:17:55.000000 watchful-3.5.0/src/watchful.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       93 2023-04-06 12:17:55.000000 watchful-3.5.0/src/watchful.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-04-06 12:17:55.000000 watchful-3.5.0/src/watchful.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 12:17:55.945730 watchful-3.5.0/tests/
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      388 2023-04-06 12:14:03.000000 watchful-3.5.0/tests/test_0000_import_sdk.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2691 2023-04-06 12:14:03.000000 watchful-3.5.0/tests/test_0001_sdk_version_and_default_conn.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      772 2023-04-06 12:14:03.000000 watchful-3.5.0/tests/test_0002_encoding.py
```

### Comparing `watchful-3.0.0/LICENSE` & `watchful-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `watchful-3.0.0/PKG-INFO` & `watchful-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchful
-Version: 3.0.0
+Version: 3.5.0
 Summary: Watchful API for Interacting with Watchful Environment
 Home-page: https://github.com/Watchfulio/watchful-py
 Author: Watchful, Inc.
 Author-email: engineering@watchful.io
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/Watchfulio/watchful-py/issues
 Keywords: watchful
```

### Comparing `watchful-3.0.0/README.md` & `watchful-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `watchful-3.0.0/README_PYPI.md` & `watchful-3.5.0/README_PYPI.md`

 * *Files identical despite different names*

### Comparing `watchful-3.0.0/README_PY_ENV.md` & `watchful-3.5.0/README_PY_ENV.md`

 * *Files identical despite different names*

### Comparing `watchful-3.0.0/examples/api_intro.ipynb` & `watchful-3.5.0/examples/api_intro.ipynb`

 * *Files identical despite different names*

### Comparing `watchful-3.0.0/examples/requirements_api_intro.txt` & `watchful-3.5.0/examples/requirements_api_intro.txt`

 * *Files identical despite different names*

### Comparing `watchful-3.0.0/pylama.ini` & `watchful-3.5.0/pylama.ini`

 * *Files identical despite different names*

### Comparing `watchful-3.0.0/setup.cfg` & `watchful-3.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `watchful-3.0.0/src/watchful/__init__.py` & `watchful-3.5.0/src/watchful/__init__.py`

 * *Files identical despite different names*

### Comparing `watchful-3.0.0/src/watchful/attributes.py` & `watchful-3.5.0/src/watchful/attributes.py`

 * *Files identical despite different names*

### Comparing `watchful-3.0.0/src/watchful/client.py` & `watchful-3.5.0/src/watchful/client.py`

 * *Files identical despite different names*

### Comparing `watchful-3.0.0/src/watchful/enrich.py` & `watchful-3.5.0/src/watchful/enrich.py`

 * *Files identical despite different names*

### Comparing `watchful-3.0.0/src/watchful/enricher.py` & `watchful-3.5.0/src/watchful/enricher.py`

 * *Files identical despite different names*

### Comparing `watchful-3.0.0/src/watchful.egg-info/PKG-INFO` & `watchful-3.5.0/src/watchful.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchful
-Version: 3.0.0
+Version: 3.5.0
 Summary: Watchful API for Interacting with Watchful Environment
 Home-page: https://github.com/Watchfulio/watchful-py
 Author: Watchful, Inc.
 Author-email: engineering@watchful.io
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/Watchfulio/watchful-py/issues
 Keywords: watchful
```

### Comparing `watchful-3.0.0/tests/test_0001_sdk_version_and_default_conn.py` & `watchful-3.5.0/tests/test_0001_sdk_version_and_default_conn.py`

 * *Files identical despite different names*

### Comparing `watchful-3.0.0/tests/test_0002_encoding.py` & `watchful-3.5.0/tests/test_0002_encoding.py`

 * *Files identical despite different names*

