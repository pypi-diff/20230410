# Comparing `tmp/smannan_lotr_sdk-5.0.tar.gz` & `tmp/smannan_lotr_sdk-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smannan_lotr_sdk-5.0.tar", last modified: Mon Apr 10 04:58:09 2023, max compression
+gzip compressed data, was "smannan_lotr_sdk-6.0.tar", last modified: Mon Apr 10 05:02:26 2023, max compression
```

## Comparing `smannan_lotr_sdk-5.0.tar` & `smannan_lotr_sdk-6.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 04:58:09.900945 smannan_lotr_sdk-5.0/
--rw-r--r--   0 soniamannan   (501) staff       (20)      256 2023-04-10 04:58:09.901255 smannan_lotr_sdk-5.0/PKG-INFO
--rw-r--r--   0 soniamannan   (501) staff       (20)      416 2023-04-10 04:10:34.000000 smannan_lotr_sdk-5.0/README.md
--rw-r--r--   0 soniamannan   (501) staff       (20)       79 2023-04-10 04:58:09.903020 smannan_lotr_sdk-5.0/setup.cfg
--rw-r--r--   0 soniamannan   (501) staff       (20)      338 2023-04-10 04:57:36.000000 smannan_lotr_sdk-5.0/setup.py
-drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 04:58:09.883199 smannan_lotr_sdk-5.0/src/
-drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 04:58:09.895184 smannan_lotr_sdk-5.0/src/smannan_lotr_sdk/
--rw-r--r--   0 soniamannan   (501) staff       (20)        0 2023-04-10 04:21:17.000000 smannan_lotr_sdk-5.0/src/smannan_lotr_sdk/__init__.py
--rw-r--r--   0 soniamannan   (501) staff       (20)      931 2023-04-10 03:44:05.000000 smannan_lotr_sdk-5.0/src/smannan_lotr_sdk/http_service.py
--rw-r--r--   0 soniamannan   (501) staff       (20)     2131 2023-04-10 03:44:05.000000 smannan_lotr_sdk-5.0/src/smannan_lotr_sdk/lotr_api_client.py
--rw-r--r--   0 soniamannan   (501) staff       (20)      591 2023-04-10 02:20:34.000000 smannan_lotr_sdk-5.0/src/smannan_lotr_sdk/movie.py
--rw-r--r--   0 soniamannan   (501) staff       (20)      274 2023-04-10 02:37:32.000000 smannan_lotr_sdk-5.0/src/smannan_lotr_sdk/quote.py
--rw-r--r--   0 soniamannan   (501) staff       (20)      870 2023-04-10 03:44:05.000000 smannan_lotr_sdk-5.0/src/smannan_lotr_sdk/test_lotr_client.py
-drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 04:58:09.900156 smannan_lotr_sdk-5.0/src/smannan_lotr_sdk.egg-info/
--rw-r--r--   0 soniamannan   (501) staff       (20)      256 2023-04-10 04:58:09.000000 smannan_lotr_sdk-5.0/src/smannan_lotr_sdk.egg-info/PKG-INFO
--rw-r--r--   0 soniamannan   (501) staff       (20)      415 2023-04-10 04:58:09.000000 smannan_lotr_sdk-5.0/src/smannan_lotr_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 soniamannan   (501) staff       (20)        1 2023-04-10 04:58:09.000000 smannan_lotr_sdk-5.0/src/smannan_lotr_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 soniamannan   (501) staff       (20)       17 2023-04-10 04:58:09.000000 smannan_lotr_sdk-5.0/src/smannan_lotr_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 05:02:26.149956 smannan_lotr_sdk-6.0/
+-rw-r--r--   0 soniamannan   (501) staff       (20)      256 2023-04-10 05:02:26.150189 smannan_lotr_sdk-6.0/PKG-INFO
+-rw-r--r--   0 soniamannan   (501) staff       (20)      416 2023-04-10 04:10:34.000000 smannan_lotr_sdk-6.0/README.md
+-rw-r--r--   0 soniamannan   (501) staff       (20)       79 2023-04-10 05:02:26.151253 smannan_lotr_sdk-6.0/setup.cfg
+-rw-r--r--   0 soniamannan   (501) staff       (20)      338 2023-04-10 05:01:58.000000 smannan_lotr_sdk-6.0/setup.py
+drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 05:02:26.138880 smannan_lotr_sdk-6.0/src/
+drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 05:02:26.145645 smannan_lotr_sdk-6.0/src/smannan_lotr_sdk/
+-rw-r--r--   0 soniamannan   (501) staff       (20)        0 2023-04-10 04:21:17.000000 smannan_lotr_sdk-6.0/src/smannan_lotr_sdk/__init__.py
+-rw-r--r--   0 soniamannan   (501) staff       (20)      931 2023-04-10 03:44:05.000000 smannan_lotr_sdk-6.0/src/smannan_lotr_sdk/http_service.py
+-rw-r--r--   0 soniamannan   (501) staff       (20)     3026 2023-04-10 05:00:50.000000 smannan_lotr_sdk-6.0/src/smannan_lotr_sdk/lotr_api_client.py
+-rw-r--r--   0 soniamannan   (501) staff       (20)      591 2023-04-10 02:20:34.000000 smannan_lotr_sdk-6.0/src/smannan_lotr_sdk/movie.py
+-rw-r--r--   0 soniamannan   (501) staff       (20)      274 2023-04-10 02:37:32.000000 smannan_lotr_sdk-6.0/src/smannan_lotr_sdk/quote.py
+drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 05:02:26.149366 smannan_lotr_sdk-6.0/src/smannan_lotr_sdk.egg-info/
+-rw-r--r--   0 soniamannan   (501) staff       (20)      256 2023-04-10 05:02:25.000000 smannan_lotr_sdk-6.0/src/smannan_lotr_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 soniamannan   (501) staff       (20)      374 2023-04-10 05:02:26.000000 smannan_lotr_sdk-6.0/src/smannan_lotr_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 soniamannan   (501) staff       (20)        1 2023-04-10 05:02:25.000000 smannan_lotr_sdk-6.0/src/smannan_lotr_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 soniamannan   (501) staff       (20)       17 2023-04-10 05:02:25.000000 smannan_lotr_sdk-6.0/src/smannan_lotr_sdk.egg-info/top_level.txt
```

### Comparing `smannan_lotr_sdk-5.0/src/smannan_lotr_sdk/http_service.py` & `smannan_lotr_sdk-6.0/src/smannan_lotr_sdk/http_service.py`

 * *Files identical despite different names*

### Comparing `smannan_lotr_sdk-5.0/src/smannan_lotr_sdk/lotr_api_client.py` & `smannan_lotr_sdk-6.0/src/smannan_lotr_sdk/lotr_api_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,40 @@
-from http_service import get_request
+import json
+import logging
+import os
+import requests
+import sys
+
 from movie import Movie
 from quote import Quote
 
+BASE_URL = 'https://the-one-api.dev/v2'
+API_ACCESS_KEY_NAME = 'LOTR_API_ACCESS_KEY'
+
+"""
+@param path: the relative path to the resource
+@param params: dictionary with optional query parameters
+
+@return (status, response_json): http status code and response json from get request
+"""
+def get_request(path: str, params={}) -> tuple:
+	# get API access key from environment if available
+	access_key = ''
+	if API_ACCESS_KEY_NAME in os.environ:
+		access_key = os.environ[API_ACCESS_KEY_NAME]
+	else:
+		logging.warning("Access key not found. Set environment variable: export LOTR_API_ACCESS_KEY=<your-api-key>")
+
+	# make get request
+	headers = {"Authorization": "Bearer {0}".format(access_key)}
+	response = requests.get("{0}/{1}".format(BASE_URL, path), headers=headers, params=params)
+
+	# return status code and json
+	return json.loads(response.text), response.status_code
+
 """
 Get all movies or optionally one movie specified by movie_id
 
 @param movie_id: the id of the movie to retrieve from the API
 @param limit: the maximum number of results to return
 @param page: the current page of results
 @param offset: the offset into the page
```

### Comparing `smannan_lotr_sdk-5.0/src/smannan_lotr_sdk/movie.py` & `smannan_lotr_sdk-6.0/src/smannan_lotr_sdk/movie.py`

 * *Files identical despite different names*

