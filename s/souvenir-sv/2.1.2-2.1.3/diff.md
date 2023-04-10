# Comparing `tmp/souvenir-sv-2.1.2.tar.gz` & `tmp/souvenir-sv-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "souvenir-sv-2.1.2.tar", last modified: Fri Apr  7 04:37:54 2023, max compression
+gzip compressed data, was "souvenir-sv-2.1.3.tar", last modified: Mon Apr 10 02:39:38 2023, max compression
```

## Comparing `souvenir-sv-2.1.2.tar` & `souvenir-sv-2.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      153 2023-04-07 04:37:47.502626 souvenir-sv-2.1.2/.deepsource.toml
--rw-r--r--   0        0        0     1228 2023-04-07 04:37:47.502626 souvenir-sv-2.1.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1831 2023-04-07 04:37:47.502626 souvenir-sv-2.1.2/.gitignore
--rw-r--r--   0        0        0    35149 2023-04-07 04:37:47.502626 souvenir-sv-2.1.2/LICENSE
--rw-r--r--   0        0        0     3159 2023-04-07 04:37:47.502626 souvenir-sv-2.1.2/README.md
--rw-r--r--   0        0        0      730 2023-04-07 04:37:47.502626 souvenir-sv-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     2490 2023-04-07 04:37:47.502626 souvenir-sv-2.1.2/requirements.txt
--rw-r--r--   0        0        0       84 2023-04-07 04:37:47.502626 souvenir-sv-2.1.2/souvenir/__init__.py
--rw-r--r--   0        0        0     2685 2023-04-07 04:37:47.502626 souvenir-sv-2.1.2/souvenir/image.py
--rw-r--r--   0        0        0     2710 2023-04-07 04:37:51.734784 souvenir-sv-2.1.2/souvenir/zipcode.py
--rw-r--r--   0        0        0        0 2023-04-07 04:37:47.502626 souvenir-sv-2.1.2/tests/__init__.py
--rw-r--r--   0        0        0     2085 2023-04-07 04:37:47.502626 souvenir-sv-2.1.2/tests/souvenir_modules.py
--rw-r--r--   0        0        0     3705 1970-01-01 00:00:00.000000 souvenir-sv-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0      153 2023-04-10 02:39:24.874729 souvenir-sv-2.1.3/.deepsource.toml
+-rw-r--r--   0        0        0     1228 2023-04-10 02:39:24.874729 souvenir-sv-2.1.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1831 2023-04-10 02:39:24.874729 souvenir-sv-2.1.3/.gitignore
+-rw-r--r--   0        0        0    35149 2023-04-10 02:39:24.874729 souvenir-sv-2.1.3/LICENSE
+-rw-r--r--   0        0        0     3159 2023-04-10 02:39:24.874729 souvenir-sv-2.1.3/README.md
+-rw-r--r--   0        0        0      730 2023-04-10 02:39:24.874729 souvenir-sv-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2490 2023-04-10 02:39:24.874729 souvenir-sv-2.1.3/requirements.txt
+-rw-r--r--   0        0        0       84 2023-04-10 02:39:24.874729 souvenir-sv-2.1.3/souvenir/__init__.py
+-rw-r--r--   0        0        0     2727 2023-04-10 02:39:24.874729 souvenir-sv-2.1.3/souvenir/image.py
+-rw-r--r--   0        0        0     2710 2023-04-10 02:39:34.994876 souvenir-sv-2.1.3/souvenir/zipcode.py
+-rw-r--r--   0        0        0        0 2023-04-10 02:39:24.874729 souvenir-sv-2.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     2085 2023-04-10 02:39:24.874729 souvenir-sv-2.1.3/tests/souvenir_modules.py
+-rw-r--r--   0        0        0     3705 1970-01-01 00:00:00.000000 souvenir-sv-2.1.3/PKG-INFO
```

### Comparing `souvenir-sv-2.1.2/.github/workflows/publish.yml` & `souvenir-sv-2.1.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `souvenir-sv-2.1.2/.gitignore` & `souvenir-sv-2.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `souvenir-sv-2.1.2/LICENSE` & `souvenir-sv-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `souvenir-sv-2.1.2/README.md` & `souvenir-sv-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `souvenir-sv-2.1.2/pyproject.toml` & `souvenir-sv-2.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `souvenir-sv-2.1.2/requirements.txt` & `souvenir-sv-2.1.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `souvenir-sv-2.1.2/souvenir/image.py` & `souvenir-sv-2.1.3/souvenir/image.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import abc
+from datetime import timedelta
 from random import randint
 from typing import Dict, List
 
 from bing_image_urls import bing_image_urls
 from requests_cache import CachedSession
 from serpapi import GoogleSearch
 
 
 class Image(abc.ABC):
     """Abstract class for image search engines."""
 
     def __init__(self, endpoint: str):
         self.query = endpoint
-        self.time = 604800
+        self.time = timedelta(days=7)
 
     @property
     @abc.abstractclassmethod
     def images(cls) -> List[str]:
         """Return a list of images urls."""
```

### Comparing `souvenir-sv-2.1.2/souvenir/zipcode.py` & `souvenir-sv-2.1.3/souvenir/zipcode.py`

 * *Files identical despite different names*

### Comparing `souvenir-sv-2.1.2/tests/souvenir_modules.py` & `souvenir-sv-2.1.3/tests/souvenir_modules.py`

 * *Files identical despite different names*

### Comparing `souvenir-sv-2.1.2/PKG-INFO` & `souvenir-sv-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: souvenir-sv
-Version: 2.1.2
+Version: 2.1.3
 Summary: A package to get zipcodes from El Salvador departments
 Author-email: standoge <stanlydoge@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: requests == 2.28.1
 Requires-Dist: beautifulsoup4 == 4.11.1
 Requires-Dist: bing-image-urls==0.1.5
```

