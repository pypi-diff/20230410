# Comparing `tmp/smannan_lotr_sdk-7.0.tar.gz` & `tmp/smannan_lotr_sdk-8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smannan_lotr_sdk-7.0.tar", last modified: Mon Apr 10 05:06:59 2023, max compression
+gzip compressed data, was "smannan_lotr_sdk-8.0.tar", last modified: Mon Apr 10 05:11:12 2023, max compression
```

## Comparing `smannan_lotr_sdk-7.0.tar` & `smannan_lotr_sdk-8.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 05:06:59.584017 smannan_lotr_sdk-7.0/
--rw-r--r--   0 soniamannan   (501) staff       (20)      256 2023-04-10 05:06:59.584306 smannan_lotr_sdk-7.0/PKG-INFO
--rw-r--r--   0 soniamannan   (501) staff       (20)      416 2023-04-10 04:10:34.000000 smannan_lotr_sdk-7.0/README.md
--rw-r--r--   0 soniamannan   (501) staff       (20)       79 2023-04-10 05:06:59.585937 smannan_lotr_sdk-7.0/setup.cfg
--rw-r--r--   0 soniamannan   (501) staff       (20)      338 2023-04-10 05:05:46.000000 smannan_lotr_sdk-7.0/setup.py
-drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 05:06:59.562334 smannan_lotr_sdk-7.0/src/
-drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 05:06:59.578508 smannan_lotr_sdk-7.0/src/smannan_lotr_sdk/
--rw-r--r--   0 soniamannan   (501) staff       (20)        0 2023-04-10 04:21:17.000000 smannan_lotr_sdk-7.0/src/smannan_lotr_sdk/__init__.py
--rw-r--r--   0 soniamannan   (501) staff       (20)      931 2023-04-10 03:44:05.000000 smannan_lotr_sdk-7.0/src/smannan_lotr_sdk/http_service.py
--rw-r--r--   0 soniamannan   (501) staff       (20)     3846 2023-04-10 05:05:27.000000 smannan_lotr_sdk-7.0/src/smannan_lotr_sdk/lotr_api_client.py
--rw-r--r--   0 soniamannan   (501) staff       (20)      591 2023-04-10 02:20:34.000000 smannan_lotr_sdk-7.0/src/smannan_lotr_sdk/movie.py
--rw-r--r--   0 soniamannan   (501) staff       (20)      274 2023-04-10 02:37:32.000000 smannan_lotr_sdk-7.0/src/smannan_lotr_sdk/quote.py
-drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 05:06:59.583081 smannan_lotr_sdk-7.0/src/smannan_lotr_sdk.egg-info/
--rw-r--r--   0 soniamannan   (501) staff       (20)      256 2023-04-10 05:06:59.000000 smannan_lotr_sdk-7.0/src/smannan_lotr_sdk.egg-info/PKG-INFO
--rw-r--r--   0 soniamannan   (501) staff       (20)      374 2023-04-10 05:06:59.000000 smannan_lotr_sdk-7.0/src/smannan_lotr_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 soniamannan   (501) staff       (20)        1 2023-04-10 05:06:59.000000 smannan_lotr_sdk-7.0/src/smannan_lotr_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 soniamannan   (501) staff       (20)       17 2023-04-10 05:06:59.000000 smannan_lotr_sdk-7.0/src/smannan_lotr_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 05:11:12.050711 smannan_lotr_sdk-8.0/
+-rw-r--r--   0 soniamannan   (501) staff       (20)      256 2023-04-10 05:11:12.050995 smannan_lotr_sdk-8.0/PKG-INFO
+-rw-r--r--   0 soniamannan   (501) staff       (20)      416 2023-04-10 04:10:34.000000 smannan_lotr_sdk-8.0/README.md
+-rw-r--r--   0 soniamannan   (501) staff       (20)       79 2023-04-10 05:11:12.052285 smannan_lotr_sdk-8.0/setup.cfg
+-rw-r--r--   0 soniamannan   (501) staff       (20)      338 2023-04-10 05:10:52.000000 smannan_lotr_sdk-8.0/setup.py
+drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 05:11:12.037517 smannan_lotr_sdk-8.0/src/
+drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 05:11:12.045246 smannan_lotr_sdk-8.0/src/smannan_lotr_sdk/
+-rw-r--r--   0 soniamannan   (501) staff       (20)        0 2023-04-10 04:21:17.000000 smannan_lotr_sdk-8.0/src/smannan_lotr_sdk/__init__.py
+-rw-r--r--   0 soniamannan   (501) staff       (20)      931 2023-04-10 03:44:05.000000 smannan_lotr_sdk-8.0/src/smannan_lotr_sdk/http_service.py
+-rw-r--r--   0 soniamannan   (501) staff       (20)     3820 2023-04-10 05:09:49.000000 smannan_lotr_sdk-8.0/src/smannan_lotr_sdk/lotr_api_client.py
+-rw-r--r--   0 soniamannan   (501) staff       (20)      591 2023-04-10 02:20:34.000000 smannan_lotr_sdk-8.0/src/smannan_lotr_sdk/movie.py
+-rw-r--r--   0 soniamannan   (501) staff       (20)      274 2023-04-10 02:37:32.000000 smannan_lotr_sdk-8.0/src/smannan_lotr_sdk/quote.py
+drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 05:11:12.049930 smannan_lotr_sdk-8.0/src/smannan_lotr_sdk.egg-info/
+-rw-r--r--   0 soniamannan   (501) staff       (20)      256 2023-04-10 05:11:11.000000 smannan_lotr_sdk-8.0/src/smannan_lotr_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 soniamannan   (501) staff       (20)      374 2023-04-10 05:11:11.000000 smannan_lotr_sdk-8.0/src/smannan_lotr_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 soniamannan   (501) staff       (20)        1 2023-04-10 05:11:11.000000 smannan_lotr_sdk-8.0/src/smannan_lotr_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 soniamannan   (501) staff       (20)       17 2023-04-10 05:11:11.000000 smannan_lotr_sdk-8.0/src/smannan_lotr_sdk.egg-info/top_level.txt
```

### Comparing `smannan_lotr_sdk-7.0/src/smannan_lotr_sdk/http_service.py` & `smannan_lotr_sdk-8.0/src/smannan_lotr_sdk/http_service.py`

 * *Files identical despite different names*

### Comparing `smannan_lotr_sdk-7.0/src/smannan_lotr_sdk/lotr_api_client.py` & `smannan_lotr_sdk-8.0/src/smannan_lotr_sdk/lotr_api_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
 	# optional query parameters for pagination
 	params = {
 		'limit': limit,
 		'page': page,
 		'offset': offset
 	}
-	response, status = http_service.get_request(relative_path, params=params)
+	response, status = get_request(relative_path, params=params)
 
 	# return an empty list of movies if the API call is unsuccessful
 	if status != 200:
 		return [], response['message']
 
 	# parse movies from API response
 	movies = []
@@ -111,15 +111,15 @@
 	# optional query parameters for pagination
 	params = {
 		'limit': limit,
 		'page': page,
 		'offset': offset
 	}
 
-	response, status = http_service.get_request(relative_path, params=params)
+	response, status = get_request(relative_path, params=params)
 
 	# return an empty list of movies if the API call is unsuccessful
 	if status != 200:
 		return [], response['message']
 
 	# parse movies from API response
 	quotes = []
```

### Comparing `smannan_lotr_sdk-7.0/src/smannan_lotr_sdk/movie.py` & `smannan_lotr_sdk-8.0/src/smannan_lotr_sdk/movie.py`

 * *Files identical despite different names*

