# Comparing `tmp/brawling-2.0.0.tar.gz` & `tmp/brawling-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brawling-2.0.0.tar", max compression
+gzip compressed data, was "brawling-2.0.1.tar", max compression
```

## Comparing `brawling-2.0.0.tar` & `brawling-2.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1085 2022-12-06 22:13:25.032898 brawling-2.0.0/LICENSE
--rw-r--r--   0        0        0      767 2023-03-29 16:16:27.339464 brawling-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     3695 2023-03-29 16:15:48.467254 brawling-2.0.0/README.md
--rw-r--r--   0        0        0      172 2023-03-27 21:20:34.840269 brawling-2.0.0/src/brawling/__init__.py
--rw-r--r--   0        0        0      131 2022-10-10 09:51:42.909311 brawling-2.0.0/src/brawling/__version__.py
--rw-r--r--   0        0        0    10753 2023-03-29 16:09:25.651150 brawling-2.0.0/src/brawling/base_client.py
--rw-r--r--   0        0        0      105 2023-03-27 21:57:39.309697 brawling-2.0.0/src/brawling/brawlapi/__init__.py
--rw-r--r--   0        0        0     4148 2023-03-29 15:48:47.249132 brawling-2.0.0/src/brawling/brawlapi/client.py
--rw-r--r--   0        0        0      422 2023-03-27 22:27:23.529943 brawling-2.0.0/src/brawling/brawlapi/exceptions.py
--rw-r--r--   0        0        0      111 2023-03-27 22:00:35.784108 brawling-2.0.0/src/brawling/brawlapi/models/__init__.py
--rw-r--r--   0        0        0     1950 2023-03-29 15:06:21.255083 brawling-2.0.0/src/brawling/brawlapi/models/brawlers.py
--rw-r--r--   0        0        0     2821 2023-03-29 15:35:27.368756 brawling-2.0.0/src/brawling/brawlapi/models/events.py
--rw-r--r--   0        0        0     1156 2023-03-29 15:34:50.854849 brawling-2.0.0/src/brawling/brawlapi/models/icons.py
--rw-r--r--   0        0        0     1168 2023-03-29 15:27:18.567859 brawling-2.0.0/src/brawling/brawlapi/models/maps.py
--rw-r--r--   0        0        0     1146 2023-03-29 15:28:45.546947 brawling-2.0.0/src/brawling/brawlapi/models/modes.py
--rw-r--r--   0        0        0    15762 2023-03-29 16:00:36.811569 brawling-2.0.0/src/brawling/client.py
--rw-r--r--   0        0        0     1979 2022-09-24 19:28:39.261647 brawling-2.0.0/src/brawling/exceptions.py
--rw-r--r--   0        0        0      138 2022-09-23 20:47:56.912552 brawling-2.0.0/src/brawling/models/__init__.py
--rw-r--r--   0        0        0      759 2023-03-29 15:26:58.006678 brawling-2.0.0/src/brawling/models/base.py
--rw-r--r--   0        0        0      946 2022-09-24 13:37:43.971563 brawling-2.0.0/src/brawling/models/brawlers.py
--rw-r--r--   0        0        0     1539 2023-03-29 14:48:55.063168 brawling-2.0.0/src/brawling/models/clubs.py
--rw-r--r--   0        0        0     1177 2022-09-23 17:59:55.603744 brawling-2.0.0/src/brawling/models/events.py
--rw-r--r--   0        0        0     6424 2023-03-29 14:48:08.523954 brawling-2.0.0/src/brawling/models/players.py
--rw-r--r--   0        0        0     1443 2023-03-29 14:48:37.310325 brawling-2.0.0/src/brawling/models/rankings.py
--rw-r--r--   0        0        0     4558 2023-03-29 16:17:59.526890 brawling-2.0.0/src/brawling/util.py
--rw-r--r--   0        0        0     4626 1970-01-01 00:00:00.000000 brawling-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2022-12-06 22:13:25.032898 brawling-2.0.1/LICENSE
+-rw-r--r--   0        0        0      767 2023-04-09 22:18:43.626059 brawling-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3695 2023-03-29 16:15:48.467254 brawling-2.0.1/README.md
+-rw-r--r--   0        0        0      172 2023-03-27 21:20:34.840269 brawling-2.0.1/src/brawling/__init__.py
+-rw-r--r--   0        0        0      131 2022-10-10 09:51:42.909311 brawling-2.0.1/src/brawling/__version__.py
+-rw-r--r--   0        0        0    10791 2023-04-09 22:21:56.841828 brawling-2.0.1/src/brawling/base_client.py
+-rw-r--r--   0        0        0      105 2023-03-27 21:57:39.309697 brawling-2.0.1/src/brawling/brawlapi/__init__.py
+-rw-r--r--   0        0        0     4148 2023-03-29 15:48:47.249132 brawling-2.0.1/src/brawling/brawlapi/client.py
+-rw-r--r--   0        0        0      422 2023-03-27 22:27:23.529943 brawling-2.0.1/src/brawling/brawlapi/exceptions.py
+-rw-r--r--   0        0        0      111 2023-03-27 22:00:35.784108 brawling-2.0.1/src/brawling/brawlapi/models/__init__.py
+-rw-r--r--   0        0        0     1950 2023-03-29 15:06:21.255083 brawling-2.0.1/src/brawling/brawlapi/models/brawlers.py
+-rw-r--r--   0        0        0     2821 2023-03-29 15:35:27.368756 brawling-2.0.1/src/brawling/brawlapi/models/events.py
+-rw-r--r--   0        0        0     1156 2023-03-29 15:34:50.854849 brawling-2.0.1/src/brawling/brawlapi/models/icons.py
+-rw-r--r--   0        0        0     1168 2023-03-29 15:27:18.567859 brawling-2.0.1/src/brawling/brawlapi/models/maps.py
+-rw-r--r--   0        0        0     1146 2023-03-29 15:28:45.546947 brawling-2.0.1/src/brawling/brawlapi/models/modes.py
+-rw-r--r--   0        0        0    15762 2023-03-29 16:00:36.811569 brawling-2.0.1/src/brawling/client.py
+-rw-r--r--   0        0        0     1979 2022-09-24 19:28:39.261647 brawling-2.0.1/src/brawling/exceptions.py
+-rw-r--r--   0        0        0      138 2022-09-23 20:47:56.912552 brawling-2.0.1/src/brawling/models/__init__.py
+-rw-r--r--   0        0        0      759 2023-03-29 15:26:58.006678 brawling-2.0.1/src/brawling/models/base.py
+-rw-r--r--   0        0        0      946 2022-09-24 13:37:43.971563 brawling-2.0.1/src/brawling/models/brawlers.py
+-rw-r--r--   0        0        0     1539 2023-03-29 14:48:55.063168 brawling-2.0.1/src/brawling/models/clubs.py
+-rw-r--r--   0        0        0     1177 2022-09-23 17:59:55.603744 brawling-2.0.1/src/brawling/models/events.py
+-rw-r--r--   0        0        0     6424 2023-03-29 14:48:08.523954 brawling-2.0.1/src/brawling/models/players.py
+-rw-r--r--   0        0        0     1443 2023-03-29 14:48:37.310325 brawling-2.0.1/src/brawling/models/rankings.py
+-rw-r--r--   0        0        0     4558 2023-03-29 16:17:59.526890 brawling-2.0.1/src/brawling/util.py
+-rw-r--r--   0        0        0     4626 1970-01-01 00:00:00.000000 brawling-2.0.1/PKG-INFO
```

### Comparing `brawling-2.0.0/LICENSE` & `brawling-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `brawling-2.0.0/pyproject.toml` & `brawling-2.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brawling"
-version = "2.0.0"
+version = "2.0.1"
 description = "Brawl stars API wrapper (sync + async + proxy + brawlapi)"
 authors = ["dankmeme01 <divanbotinkovich@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `brawling-2.0.0/README.md` & `brawling-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `brawling-2.0.0/src/brawling/base_client.py` & `brawling-2.0.1/src/brawling/base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,16 +237,17 @@
 class BaseAsyncClient(BaseClient):
     def __init__(self, base_url: str, strict_errors: bool = True, caching: bool = False) -> None:
         if not HAS_AIOHTTP:
             raise NotImplementedError("async support not installed")
 
         super().__init__(base_url, strict_errors, caching)
 
+        self._session_open = False
         if caching:
-            if not CACHE_ENABLED:
+            if not HAS_ASYNC_CACHE:
                 raise ValueError(f'caching was enabled but the \'aiohttp-client-cache\' module is not installed')
 
             self.session = CachedAiohttpSession(cache=AIOSQLiteBackend(
                     expire_after=timedelta(minutes=10),
                     cache_control=True,
                     use_temp=True,
                     cache_name='.brawling_acache'
```

### Comparing `brawling-2.0.0/src/brawling/brawlapi/client.py` & `brawling-2.0.1/src/brawling/brawlapi/client.py`

 * *Files identical despite different names*

### Comparing `brawling-2.0.0/src/brawling/brawlapi/models/brawlers.py` & `brawling-2.0.1/src/brawling/brawlapi/models/brawlers.py`

 * *Files identical despite different names*

### Comparing `brawling-2.0.0/src/brawling/brawlapi/models/events.py` & `brawling-2.0.1/src/brawling/brawlapi/models/events.py`

 * *Files identical despite different names*

### Comparing `brawling-2.0.0/src/brawling/brawlapi/models/icons.py` & `brawling-2.0.1/src/brawling/brawlapi/models/icons.py`

 * *Files identical despite different names*

### Comparing `brawling-2.0.0/src/brawling/brawlapi/models/maps.py` & `brawling-2.0.1/src/brawling/brawlapi/models/maps.py`

 * *Files identical despite different names*

### Comparing `brawling-2.0.0/src/brawling/brawlapi/models/modes.py` & `brawling-2.0.1/src/brawling/brawlapi/models/modes.py`

 * *Files identical despite different names*

### Comparing `brawling-2.0.0/src/brawling/client.py` & `brawling-2.0.1/src/brawling/client.py`

 * *Files identical despite different names*

### Comparing `brawling-2.0.0/src/brawling/exceptions.py` & `brawling-2.0.1/src/brawling/exceptions.py`

 * *Files identical despite different names*

### Comparing `brawling-2.0.0/src/brawling/models/base.py` & `brawling-2.0.1/src/brawling/models/base.py`

 * *Files identical despite different names*

### Comparing `brawling-2.0.0/src/brawling/models/brawlers.py` & `brawling-2.0.1/src/brawling/models/brawlers.py`

 * *Files identical despite different names*

### Comparing `brawling-2.0.0/src/brawling/models/clubs.py` & `brawling-2.0.1/src/brawling/models/clubs.py`

 * *Files identical despite different names*

### Comparing `brawling-2.0.0/src/brawling/models/events.py` & `brawling-2.0.1/src/brawling/models/events.py`

 * *Files identical despite different names*

### Comparing `brawling-2.0.0/src/brawling/models/players.py` & `brawling-2.0.1/src/brawling/models/players.py`

 * *Files identical despite different names*

### Comparing `brawling-2.0.0/src/brawling/models/rankings.py` & `brawling-2.0.1/src/brawling/models/rankings.py`

 * *Files identical despite different names*

### Comparing `brawling-2.0.0/src/brawling/util.py` & `brawling-2.0.1/src/brawling/util.py`

 * *Files identical despite different names*

### Comparing `brawling-2.0.0/PKG-INFO` & `brawling-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brawling
-Version: 2.0.0
+Version: 2.0.1
 Summary: Brawl stars API wrapper (sync + async + proxy + brawlapi)
 License: MIT
 Author: dankmeme01
 Author-email: divanbotinkovich@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

