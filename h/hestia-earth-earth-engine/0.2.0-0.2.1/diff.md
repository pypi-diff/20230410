# Comparing `tmp/hestia-earth-earth-engine-0.2.0.tar.gz` & `tmp/hestia-earth-earth-engine-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hestia-earth-earth-engine-0.2.0.tar", last modified: Fri Dec 30 10:27:31 2022, max compression
+gzip compressed data, was "hestia-earth-earth-engine-0.2.1.tar", last modified: Mon Apr 10 12:40:53 2023, max compression
```

## Comparing `hestia-earth-earth-engine-0.2.0.tar` & `hestia-earth-earth-engine-0.2.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 10:27:31.219704 hestia-earth-earth-engine-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2022-12-30 10:27:08.000000 hestia-earth-earth-engine-0.2.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       18 2022-12-30 10:27:08.000000 hestia-earth-earth-engine-0.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1851 2022-12-30 10:27:31.218705 hestia-earth-earth-engine-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1407 2022-12-30 10:27:08.000000 hestia-earth-earth-engine-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 10:27:31.209704 hestia-earth-earth-engine-0.2.0/hestia_earth/
--rw-rw-rw-   0 root         (0) root         (0)       56 2022-12-30 10:27:08.000000 hestia-earth-earth-engine-0.2.0/hestia_earth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 10:27:31.211704 hestia-earth-earth-engine-0.2.0/hestia_earth/earth_engine/
--rw-rw-rw-   0 root         (0) root         (0)     2515 2022-12-30 10:27:08.000000 hestia-earth-earth-engine-0.2.0/hestia_earth/earth_engine/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 10:27:31.212704 hestia-earth-earth-engine-0.2.0/hestia_earth/earth_engine/boundary/
--rw-rw-rw-   0 root         (0) root         (0)     1365 2022-12-30 10:27:08.000000 hestia-earth-earth-engine-0.2.0/hestia_earth/earth_engine/boundary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2347 2022-12-30 10:27:08.000000 hestia-earth-earth-engine-0.2.0/hestia_earth/earth_engine/boundary/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 10:27:31.213704 hestia-earth-earth-engine-0.2.0/hestia_earth/earth_engine/coordinates/
--rw-rw-rw-   0 root         (0) root         (0)      721 2022-12-30 10:27:08.000000 hestia-earth-earth-engine-0.2.0/hestia_earth/earth_engine/coordinates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1886 2022-12-30 10:27:08.000000 hestia-earth-earth-engine-0.2.0/hestia_earth/earth_engine/coordinates/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 10:27:31.213704 hestia-earth-earth-engine-0.2.0/hestia_earth/earth_engine/gadm/
--rw-rw-rw-   0 root         (0) root         (0)     1497 2022-12-30 10:27:08.000000 hestia-earth-earth-engine-0.2.0/hestia_earth/earth_engine/gadm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2469 2022-12-30 10:27:08.000000 hestia-earth-earth-engine-0.2.0/hestia_earth/earth_engine/gadm/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5917 2022-12-30 10:27:08.000000 hestia-earth-earth-engine-0.2.0/hestia_earth/earth_engine/gee_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1352 2022-12-30 10:27:08.000000 hestia-earth-earth-engine-0.2.0/hestia_earth/earth_engine/log.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2022-12-30 10:27:08.000000 hestia-earth-earth-engine-0.2.0/hestia_earth/earth_engine/utils.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2022-12-30 10:27:08.000000 hestia-earth-earth-engine-0.2.0/hestia_earth/earth_engine/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 10:27:31.215704 hestia-earth-earth-engine-0.2.0/hestia_earth_earth_engine.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1851 2022-12-30 10:27:31.000000 hestia-earth-earth-engine-0.2.0/hestia_earth_earth_engine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1064 2022-12-30 10:27:31.000000 hestia-earth-earth-engine-0.2.0/hestia_earth_earth_engine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-30 10:27:31.000000 hestia-earth-earth-engine-0.2.0/hestia_earth_earth_engine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2022-12-30 10:27:31.000000 hestia-earth-earth-engine-0.2.0/hestia_earth_earth_engine.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-12-30 10:27:31.000000 hestia-earth-earth-engine-0.2.0/hestia_earth_earth_engine.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-30 10:27:31.219704 hestia-earth-earth-engine-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      979 2022-12-30 10:27:08.000000 hestia-earth-earth-engine-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 10:27:31.206704 hestia-earth-earth-engine-0.2.0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 10:27:31.216704 hestia-earth-earth-engine-0.2.0/tests/integration/
--rw-rw-rw-   0 root         (0) root         (0)       60 2022-12-30 10:27:08.000000 hestia-earth-earth-engine-0.2.0/tests/integration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 10:27:31.217704 hestia-earth-earth-engine-0.2.0/tests/integration/boundary/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-30 10:27:08.000000 hestia-earth-earth-engine-0.2.0/tests/integration/boundary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2051 2022-12-30 10:27:08.000000 hestia-earth-earth-engine-0.2.0/tests/integration/boundary/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 10:27:31.217704 hestia-earth-earth-engine-0.2.0/tests/integration/coordinates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-30 10:27:08.000000 hestia-earth-earth-engine-0.2.0/tests/integration/coordinates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1718 2022-12-30 10:27:08.000000 hestia-earth-earth-engine-0.2.0/tests/integration/coordinates/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 10:27:31.218705 hestia-earth-earth-engine-0.2.0/tests/integration/gadm/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-30 10:27:08.000000 hestia-earth-earth-engine-0.2.0/tests/integration/gadm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2086 2022-12-30 10:27:08.000000 hestia-earth-earth-engine-0.2.0/tests/integration/gadm/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      430 2022-12-30 10:27:08.000000 hestia-earth-earth-engine-0.2.0/tests/integration/test_gee_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:40:53.482087 hestia-earth-earth-engine-0.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-04-10 12:40:53.482087 hestia-earth-earth-engine-0.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:40:53.473087 hestia-earth-earth-engine-0.2.1/hestia_earth/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/hestia_earth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:40:53.475087 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/
+-rw-rw-rw-   0 root         (0) root         (0)     2515 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:40:53.476087 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/boundary/
+-rw-rw-rw-   0 root         (0) root         (0)     1365 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/boundary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2347 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/boundary/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:40:53.477087 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/coordinates/
+-rw-rw-rw-   0 root         (0) root         (0)      721 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/coordinates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/coordinates/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:40:53.477087 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/gadm/
+-rw-rw-rw-   0 root         (0) root         (0)     1841 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/gadm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2469 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/gadm/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5917 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/gee_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1352 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:40:53.479087 hestia-earth-earth-engine-0.2.1/hestia_earth_earth_engine.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-04-10 12:40:53.000000 hestia-earth-earth-engine-0.2.1/hestia_earth_earth_engine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-04-10 12:40:53.000000 hestia-earth-earth-engine-0.2.1/hestia_earth_earth_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 12:40:53.000000 hestia-earth-earth-engine-0.2.1/hestia_earth_earth_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-04-10 12:40:53.000000 hestia-earth-earth-engine-0.2.1/hestia_earth_earth_engine.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-10 12:40:53.000000 hestia-earth-earth-engine-0.2.1/hestia_earth_earth_engine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 12:40:53.482087 hestia-earth-earth-engine-0.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:40:53.471087 hestia-earth-earth-engine-0.2.1/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:40:53.480087 hestia-earth-earth-engine-0.2.1/tests/integration/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/tests/integration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:40:53.480087 hestia-earth-earth-engine-0.2.1/tests/integration/boundary/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/tests/integration/boundary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2051 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/tests/integration/boundary/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:40:53.481087 hestia-earth-earth-engine-0.2.1/tests/integration/coordinates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/tests/integration/coordinates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1718 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/tests/integration/coordinates/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:40:53.482087 hestia-earth-earth-engine-0.2.1/tests/integration/gadm/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/tests/integration/gadm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2086 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/tests/integration/gadm/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/tests/integration/test_gee_utils.py
```

### Comparing `hestia-earth-earth-engine-0.2.0/PKG-INFO` & `hestia-earth-earth-engine-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hestia-earth-earth-engine
-Version: 0.2.0
+Version: 0.2.1
 Summary: Hestia's earth engine.
 Home-page: https://gitlab.com/hestia-earth/hestia-earth-engine
 Author: Hestia Team
 Author-email: guillaume@hestia.earth
 License: GPL
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hestia-earth-earth-engine-0.2.0/README.md` & `hestia-earth-earth-engine-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.0/hestia_earth/earth_engine/__init__.py` & `hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.0/hestia_earth/earth_engine/boundary/__init__.py` & `hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/boundary/__init__.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.0/hestia_earth/earth_engine/boundary/utils.py` & `hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/boundary/utils.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.0/hestia_earth/earth_engine/coordinates/__init__.py` & `hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/coordinates/__init__.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.0/hestia_earth/earth_engine/coordinates/utils.py` & `hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/coordinates/utils.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.0/hestia_earth/earth_engine/gadm/utils.py` & `hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/gadm/utils.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.0/hestia_earth/earth_engine/gee_utils.py` & `hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/gee_utils.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.0/hestia_earth/earth_engine/log.py` & `hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/log.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.0/hestia_earth/earth_engine/utils.py` & `hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/utils.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.0/hestia_earth_earth_engine.egg-info/PKG-INFO` & `hestia-earth-earth-engine-0.2.1/hestia_earth_earth_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hestia-earth-earth-engine
-Version: 0.2.0
+Version: 0.2.1
 Summary: Hestia's earth engine.
 Home-page: https://gitlab.com/hestia-earth/hestia-earth-engine
 Author: Hestia Team
 Author-email: guillaume@hestia.earth
 License: GPL
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hestia-earth-earth-engine-0.2.0/hestia_earth_earth_engine.egg-info/SOURCES.txt` & `hestia-earth-earth-engine-0.2.1/hestia_earth_earth_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.0/setup.py` & `hestia-earth-earth-engine-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.0/tests/integration/boundary/test_utils.py` & `hestia-earth-earth-engine-0.2.1/tests/integration/boundary/test_utils.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.0/tests/integration/coordinates/test_utils.py` & `hestia-earth-earth-engine-0.2.1/tests/integration/coordinates/test_utils.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.0/tests/integration/gadm/test_utils.py` & `hestia-earth-earth-engine-0.2.1/tests/integration/gadm/test_utils.py`

 * *Files identical despite different names*

