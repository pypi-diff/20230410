# Comparing `tmp/tair-1.3.2.tar.gz` & `tmp/tair-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tair-1.3.2.tar", last modified: Fri Feb 17 10:04:34 2023, max compression
+gzip compressed data, was "tair-1.3.3.tar", last modified: Mon Apr 10 06:00:31 2023, max compression
```

## Comparing `tair-1.3.2.tar` & `tair-1.3.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-02-17 10:04:34.629145 tair-1.3.2/
--rw-r--r--   0 yangbodong   (502) staff       (20)     1064 2022-07-27 06:08:53.000000 tair-1.3.2/LICENSE
--rw-r--r--   0 yangbodong   (502) staff       (20)     4612 2023-02-17 10:04:34.628947 tair-1.3.2/PKG-INFO
--rw-r--r--   0 yangbodong   (502) staff       (20)     4331 2023-01-05 08:19:35.000000 tair-1.3.2/README.md
--rw-r--r--   0 yangbodong   (502) staff       (20)       38 2023-02-17 10:04:34.629201 tair-1.3.2/setup.cfg
--rwxr-xr-x   0 yangbodong   (502) staff       (20)      486 2023-02-17 10:03:39.000000 tair-1.3.2/setup.py
-drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-02-17 10:04:34.621341 tair-1.3.2/tair/
--rw-r--r--   0 yangbodong   (502) staff       (20)     1557 2023-02-17 07:55:24.000000 tair-1.3.2/tair/__init__.py
-drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-02-17 10:04:34.623816 tair-1.3.2/tair/asyncio/
--rw-r--r--   0 yangbodong   (502) staff       (20)     1412 2022-08-16 03:42:18.000000 tair-1.3.2/tair/asyncio/__init__.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     3293 2023-01-05 06:47:04.000000 tair-1.3.2/tair/asyncio/client.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     1639 2023-01-05 07:08:21.000000 tair-1.3.2/tair/asyncio/cluster.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     1005 2023-01-05 06:47:04.000000 tair-1.3.2/tair/asyncio/pipeline.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     3308 2022-08-16 03:42:18.000000 tair-1.3.2/tair/client.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     1866 2022-08-16 03:42:18.000000 tair-1.3.2/tair/cluster.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     5361 2023-02-17 07:55:24.000000 tair-1.3.2/tair/commands.py
--rw-r--r--   0 yangbodong   (502) staff       (20)      334 2022-07-27 06:08:53.000000 tair-1.3.2/tair/exceptions.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     1184 2022-08-16 03:42:18.000000 tair-1.3.2/tair/pipeline.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     1582 2022-08-16 03:42:18.000000 tair-1.3.2/tair/tairbloom.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    11976 2022-09-01 08:46:46.000000 tair-1.3.2/tair/taircpc.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     3156 2022-08-25 09:35:31.000000 tair-1.3.2/tair/tairdoc.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     5190 2022-08-25 09:35:31.000000 tair-1.3.2/tair/tairgis.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    14354 2022-08-25 09:35:31.000000 tair-1.3.2/tair/tairhash.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     4944 2022-08-16 03:42:18.000000 tair-1.3.2/tair/tairroaring.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     5467 2023-02-17 09:59:58.000000 tair-1.3.2/tair/tairsearch.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     9196 2023-01-05 06:47:04.000000 tair-1.3.2/tair/tairstring.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    13708 2022-09-01 08:46:46.000000 tair-1.3.2/tair/tairts.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    14047 2023-02-17 07:55:24.000000 tair-1.3.2/tair/tairvector.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     7377 2022-08-16 03:42:18.000000 tair-1.3.2/tair/tairzset.py
--rw-r--r--   0 yangbodong   (502) staff       (20)      259 2022-08-16 03:42:18.000000 tair-1.3.2/tair/typing.py
-drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-02-17 10:04:34.622352 tair-1.3.2/tair.egg-info/
--rw-r--r--   0 yangbodong   (502) staff       (20)     4612 2023-02-17 10:04:34.000000 tair-1.3.2/tair.egg-info/PKG-INFO
--rw-r--r--   0 yangbodong   (502) staff       (20)      874 2023-02-17 10:04:34.000000 tair-1.3.2/tair.egg-info/SOURCES.txt
--rw-r--r--   0 yangbodong   (502) staff       (20)        1 2023-02-17 10:04:34.000000 tair-1.3.2/tair.egg-info/dependency_links.txt
--rw-r--r--   0 yangbodong   (502) staff       (20)       11 2023-02-17 10:04:34.000000 tair-1.3.2/tair.egg-info/requires.txt
--rw-r--r--   0 yangbodong   (502) staff       (20)        5 2023-02-17 10:04:34.000000 tair-1.3.2/tair.egg-info/top_level.txt
-drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-02-17 10:04:34.628603 tair-1.3.2/tests/
--rw-r--r--   0 yangbodong   (502) staff       (20)     2256 2023-01-05 07:58:42.000000 tair-1.3.2/tests/test_from_url.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     2223 2023-01-05 06:47:04.000000 tair-1.3.2/tests/test_pipeline.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     2484 2022-08-16 03:42:18.000000 tair-1.3.2/tests/test_tairbloom.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    24057 2022-09-01 08:46:46.000000 tair-1.3.2/tests/test_taircpc.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     4708 2022-08-25 09:35:31.000000 tair-1.3.2/tests/test_tairdoc.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     8533 2022-08-25 09:35:31.000000 tair-1.3.2/tests/test_tairgis.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    41035 2022-08-16 03:42:18.000000 tair-1.3.2/tests/test_tairhash.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     9432 2022-08-16 03:42:18.000000 tair-1.3.2/tests/test_tairroaring.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    15944 2023-02-17 09:59:58.000000 tair-1.3.2/tests/test_tairsearch.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    19152 2022-08-16 03:42:18.000000 tair-1.3.2/tests/test_tairstring.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    13908 2022-09-01 08:46:46.000000 tair-1.3.2/tests/test_tairts.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    16086 2023-02-17 07:55:24.000000 tair-1.3.2/tests/test_tairvector.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    23955 2022-08-16 03:42:18.000000 tair-1.3.2/tests/test_tairzset.py
+drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-04-10 06:00:31.554691 tair-1.3.3/
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1064 2022-07-27 06:08:53.000000 tair-1.3.3/LICENSE
+-rw-r--r--   0 yangbodong   (502) staff       (20)     4612 2023-04-10 06:00:31.554505 tair-1.3.3/PKG-INFO
+-rw-r--r--   0 yangbodong   (502) staff       (20)     4331 2023-01-05 08:19:35.000000 tair-1.3.3/README.md
+-rw-r--r--   0 yangbodong   (502) staff       (20)       38 2023-04-10 06:00:31.554752 tair-1.3.3/setup.cfg
+-rwxr-xr-x   0 yangbodong   (502) staff       (20)      488 2023-04-10 05:59:28.000000 tair-1.3.3/setup.py
+drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-04-10 06:00:31.547172 tair-1.3.3/tair/
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1557 2023-02-17 07:55:24.000000 tair-1.3.3/tair/__init__.py
+drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-04-10 06:00:31.549170 tair-1.3.3/tair/asyncio/
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1412 2022-08-16 03:42:18.000000 tair-1.3.3/tair/asyncio/__init__.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     3293 2023-01-05 06:47:04.000000 tair-1.3.3/tair/asyncio/client.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1639 2023-01-05 07:08:21.000000 tair-1.3.3/tair/asyncio/cluster.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1005 2023-01-05 06:47:04.000000 tair-1.3.3/tair/asyncio/pipeline.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     3308 2022-08-16 03:42:18.000000 tair-1.3.3/tair/client.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1866 2022-08-16 03:42:18.000000 tair-1.3.3/tair/cluster.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     5361 2023-02-17 07:55:24.000000 tair-1.3.3/tair/commands.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)      334 2022-07-27 06:08:53.000000 tair-1.3.3/tair/exceptions.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1184 2022-08-16 03:42:18.000000 tair-1.3.3/tair/pipeline.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1582 2022-08-16 03:42:18.000000 tair-1.3.3/tair/tairbloom.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    11976 2022-09-01 08:46:46.000000 tair-1.3.3/tair/taircpc.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     3156 2022-08-25 09:35:31.000000 tair-1.3.3/tair/tairdoc.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     5190 2022-08-25 09:35:31.000000 tair-1.3.3/tair/tairgis.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    14354 2022-08-25 09:35:31.000000 tair-1.3.3/tair/tairhash.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     4944 2022-08-16 03:42:18.000000 tair-1.3.3/tair/tairroaring.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     6759 2023-04-10 02:26:45.000000 tair-1.3.3/tair/tairsearch.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     9196 2023-01-05 06:47:04.000000 tair-1.3.3/tair/tairstring.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    13708 2022-09-01 08:46:46.000000 tair-1.3.3/tair/tairts.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    14047 2023-02-17 07:55:24.000000 tair-1.3.3/tair/tairvector.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     7377 2022-08-16 03:42:18.000000 tair-1.3.3/tair/tairzset.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)      259 2022-08-16 03:42:18.000000 tair-1.3.3/tair/typing.py
+drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-04-10 06:00:31.548043 tair-1.3.3/tair.egg-info/
+-rw-r--r--   0 yangbodong   (502) staff       (20)     4612 2023-04-10 06:00:31.000000 tair-1.3.3/tair.egg-info/PKG-INFO
+-rw-r--r--   0 yangbodong   (502) staff       (20)      874 2023-04-10 06:00:31.000000 tair-1.3.3/tair.egg-info/SOURCES.txt
+-rw-r--r--   0 yangbodong   (502) staff       (20)        1 2023-04-10 06:00:31.000000 tair-1.3.3/tair.egg-info/dependency_links.txt
+-rw-r--r--   0 yangbodong   (502) staff       (20)       13 2023-04-10 06:00:31.000000 tair-1.3.3/tair.egg-info/requires.txt
+-rw-r--r--   0 yangbodong   (502) staff       (20)        5 2023-04-10 06:00:31.000000 tair-1.3.3/tair.egg-info/top_level.txt
+drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-04-10 06:00:31.554112 tair-1.3.3/tests/
+-rw-r--r--   0 yangbodong   (502) staff       (20)     2256 2023-01-05 07:58:42.000000 tair-1.3.3/tests/test_from_url.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     2223 2023-01-05 06:47:04.000000 tair-1.3.3/tests/test_pipeline.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     2484 2022-08-16 03:42:18.000000 tair-1.3.3/tests/test_tairbloom.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    24057 2022-09-01 08:46:46.000000 tair-1.3.3/tests/test_taircpc.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     4708 2022-08-25 09:35:31.000000 tair-1.3.3/tests/test_tairdoc.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     8533 2022-08-25 09:35:31.000000 tair-1.3.3/tests/test_tairgis.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    41035 2022-08-16 03:42:18.000000 tair-1.3.3/tests/test_tairhash.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     9432 2022-08-16 03:42:18.000000 tair-1.3.3/tests/test_tairroaring.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    18793 2023-04-10 02:26:45.000000 tair-1.3.3/tests/test_tairsearch.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    19152 2022-08-16 03:42:18.000000 tair-1.3.3/tests/test_tairstring.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    13908 2022-09-01 08:46:46.000000 tair-1.3.3/tests/test_tairts.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    16086 2023-02-17 07:55:24.000000 tair-1.3.3/tests/test_tairvector.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    23955 2022-08-16 03:42:18.000000 tair-1.3.3/tests/test_tairzset.py
```

### Comparing `tair-1.3.2/LICENSE` & `tair-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/PKG-INFO` & `tair-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tair
-Version: 1.3.2
+Version: 1.3.3
 Summary: Python client for Tair
 Home-page: https://github.com/alibaba/tair-py
 Author: Vincil Lau
 Author-email: vincillau@outlook.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `tair-1.3.2/README.md` & `tair-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tair/__init__.py` & `tair-1.3.3/tair/__init__.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tair/asyncio/__init__.py` & `tair-1.3.3/tair/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tair/asyncio/client.py` & `tair-1.3.3/tair/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tair/asyncio/cluster.py` & `tair-1.3.3/tair/asyncio/cluster.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tair/asyncio/pipeline.py` & `tair-1.3.3/tair/asyncio/pipeline.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tair/client.py` & `tair-1.3.3/tair/client.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tair/cluster.py` & `tair-1.3.3/tair/cluster.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tair/commands.py` & `tair-1.3.3/tair/commands.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tair/pipeline.py` & `tair-1.3.3/tair/pipeline.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tair/tairbloom.py` & `tair-1.3.3/tair/tairbloom.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tair/taircpc.py` & `tair-1.3.3/tair/taircpc.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tair/tairdoc.py` & `tair-1.3.3/tair/tairdoc.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tair/tairgis.py` & `tair-1.3.3/tair/tairgis.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tair/tairhash.py` & `tair-1.3.3/tair/tairhash.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tair/tairroaring.py` & `tair-1.3.3/tair/tairroaring.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tair/tairsearch.py` & `tair-1.3.3/tair/tairsearch.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Dict, Iterable, List, Optional
 
+import tair
 from tair.typing import CommandsProtocol, EncodableT, KeyT, ResponseT
 
 
 class ScandocidResult:
     def __init__(self, cursor: str, doc_ids: Iterable[str]):
         self.cursor = cursor
         self.doc_ids = list(doc_ids)
@@ -26,14 +27,20 @@
 
     def tft_updateindex(self, index: KeyT, mappings: str) -> ResponseT:
         return self.execute_command("TFT.UPDATEINDEX", index, mappings)
 
     def tft_getindex(self, index: KeyT) -> ResponseT:
         return self.execute_command("TFT.GETINDEX", index)
 
+    def tft_getindex_mappings(self, index: KeyT) -> ResponseT:
+        return self.execute_command("TFT.GETINDEX", index, "mappings")
+
+    def tft_getindex_settings(self, index: KeyT) -> ResponseT:
+        return self.execute_command("TFT.GETINDEX", index, "settings")
+
     def tft_adddoc(
         self,
         index: KeyT,
         document: str,
         doc_id: Optional[str] = None,
     ) -> ResponseT:
         if doc_id is not None:
@@ -130,26 +137,49 @@
             pieces.append(match)
         if count is not None:
             pieces.append("COUNT")
             pieces.append(count)
 
         return self.execute_command("TFT.SCANDOCID", *pieces)
 
-    def tft_deldoc(self, index: KeyT, doc_id: str, fields: Iterable[str]) -> ResponseT:
-        return self.execute_command("TFT.DELDOC", index, doc_id, *fields)
+    def tft_deldoc(self, index: KeyT, doc_id: Iterable[str]) -> ResponseT:
+        return self.execute_command("TFT.DELDOC", index, *doc_id)
 
     def tft_delall(self, index: KeyT) -> ResponseT:
         return self.execute_command("TFT.DELALL", index)
 
-    def tft_search(self, index: KeyT, query: str) -> ResponseT:
-        return self.execute_command("TFT.SEARCH", index, query)
+    def tft_search(self, index: KeyT, query: str, use_cache: bool = False) -> ResponseT:
+        pieces: List[EncodableT] = [index, query]
+        if use_cache:
+            pieces.append("use_cache")
+        return self.execute_command("TFT.SEARCH", *pieces)
 
     def tft_msearch(self, index_count: int, index: Iterable[KeyT], query: str) -> ResponseT:
         return self.execute_command("TFT.MSEARCH", index_count, *index, query)
 
+    def tft_analyzer(self, analyzer_name: str, text: str, index: Optional[KeyT] = None,
+                     show_time: Optional[bool] = False) -> ResponseT:
+        pieces: List[EncodableT] = [analyzer_name, text]
+        if index is not None:
+            pieces.append("INDEX")
+            pieces.append(index)
+        if show_time:
+            pieces.append("show_time")
+        target_nodes = None
+        if isinstance(self, tair.TairCluster):
+            if index is None:
+                target_nodes = 'random'
+            else:
+                target_nodes = self.nodes_manager.get_node_from_slot(self.keyslot(index))
+        return self.execute_command("TFT.ANALYZER", *pieces, target_nodes=target_nodes)
+
+    def tft_explaincost(self, index: KeyT, query: str) -> ResponseT:
+        pieces: List[EncodableT] = [index, query]
+        return self.execute_command("TFT.EXPLAINCOST", *pieces)
+
     def tft_addsug(self, index: KeyT, mapping: Dict[str, int]) -> ResponseT:
         pieces: List[EncodableT] = [index]
 
         for text, weight in mapping.items():
             pieces.append(text)
             pieces.append(weight)
```

### Comparing `tair-1.3.2/tair/tairstring.py` & `tair-1.3.3/tair/tairstring.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tair/tairts.py` & `tair-1.3.3/tair/tairts.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tair/tairvector.py` & `tair-1.3.3/tair/tairvector.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tair/tairzset.py` & `tair-1.3.3/tair/tairzset.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tair.egg-info/PKG-INFO` & `tair-1.3.3/tair.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tair
-Version: 1.3.2
+Version: 1.3.3
 Summary: Python client for Tair
 Home-page: https://github.com/alibaba/tair-py
 Author: Vincil Lau
 Author-email: vincillau@outlook.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `tair-1.3.2/tair.egg-info/SOURCES.txt` & `tair-1.3.3/tair.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tests/test_from_url.py` & `tair-1.3.3/tests/test_from_url.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tests/test_pipeline.py` & `tair-1.3.3/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tests/test_tairbloom.py` & `tair-1.3.3/tests/test_tairbloom.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tests/test_taircpc.py` & `tair-1.3.3/tests/test_taircpc.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tests/test_tairdoc.py` & `tair-1.3.3/tests/test_tairdoc.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tests/test_tairgis.py` & `tair-1.3.3/tests/test_tairgis.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tests/test_tairhash.py` & `tair-1.3.3/tests/test_tairhash.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tests/test_tairroaring.py` & `tair-1.3.3/tests/test_tairroaring.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tests/test_tairsearch.py` & `tair-1.3.3/tests/test_tairsearch.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,14 +19,15 @@
       "product_title": { "type": "text", "analyzer": "jieba" },
       "price": { "type": "double" }
     }
   }
 }"""
 
         assert t.tft_createindex(index, mappings)
+        t.delete(index)
 
     def test_tft_updateindex(self, t: Tair):
         index = "idx_" + str(uuid.uuid4())
         mappings1 = """
 {
   "mappings": {
     "_source": { "enabled": true },
@@ -43,14 +44,16 @@
   "mappings": {
     "properties": { "product_group": { "type": "text", "analyzer": "chinese" } }
   }
 }"""
 
         assert t.tft_createindex(index, mappings1)
         assert t.tft_updateindex(index, mappings2)
+        t.delete(index)
+
 
     def test_tft_getindex(self, t: Tair):
         index = "idx_" + str(uuid.uuid4())
         mappings = """
 {
   "mappings": {
     "_source": { "enabled": true },
@@ -62,14 +65,78 @@
     }
   }
 }"""
 
         assert t.tft_getindex(index) is None
         assert t.tft_createindex(index, mappings)
         assert t.tft_getindex(index) is not None
+        mappings1 = f"""
+{{
+  "{index}":{{
+    "mappings":{{
+      "_source":{{
+        "enabled":true,
+        "excludes":[
+        ],
+        "includes":[
+        ]
+      }},
+      "dynamic":"false",
+      "properties":{{
+        "price":{{
+          "boost":1.0,
+          "enabled":true,
+          "ignore_above":-1,
+          "index":true,
+          "similarity":"classic",
+          "type":"double"
+        }},
+        "product_id":{{
+          "boost":1.0,
+          "enabled":true,
+          "ignore_above":128,
+          "index":true,
+          "similarity":"classic",
+          "type":"keyword"
+        }},
+        "product_name":{{
+          "boost":1.0,
+          "enabled":true,
+          "ignore_above":-1,
+          "index":true,
+          "similarity":"classic",
+          "type":"text"
+        }},
+        "product_title":{{
+          "analyzer":"jieba",
+          "boost":1.0,
+          "enabled":true,
+          "ignore_above":-1,
+          "index":true,
+          "similarity":"classic",
+          "type":"text"
+        }}
+      }}
+    }}
+  }}
+}}
+"""
+        result = t.tft_getindex_mappings(index)
+        assert json.loads(mappings1) == json.loads(result)
+        settings = f"""
+{{
+  "{index}":{{
+    "settings":{{
+    }}
+  }}
+}}
+"""
+        result = t.tft_getindex_settings(index)
+        assert json.loads(settings) == json.loads(result)
+        t.delete(index)
 
     def test_tft_adddoc(self, t: Tair):
         index = "idx_" + str(uuid.uuid4())
         mappings = """
 {
   "mappings": {
     "_source": { "enabled": true },
@@ -82,14 +149,15 @@
   }
 }"""
         document = '{"product_id":"product test"}'
 
         assert t.tft_createindex(index, mappings)
         assert t.tft_adddoc(index, document, doc_id="00001") == '{"_id":"00001"}'
         assert t.tft_adddoc(index, document)
+        t.delete(index)
 
     def test_tft_madddoc(self, t: Tair):
         index = "idx_" + str(uuid.uuid4())
         mappings = """
 {
   "mappings": {
     "_source": { "enabled": true },
@@ -102,14 +170,15 @@
   }
 }"""
         document1 = '{"product_id":"test1"}'
         document2 = '{"product_id":"test2"}'
 
         assert t.tft_createindex(index, mappings)
         assert t.tft_madddoc(index, {document1: "00001", document2: "00002"})
+        t.delete(index)
 
     def test_tft_updatedocfield(self, t: Tair):
         index = "idx_" + str(uuid.uuid4())
         mappings = """
 {
   "mappings": {
     "_source": { "enabled": true },
@@ -123,14 +192,15 @@
 }"""
         document1 = '{"product_id":"test1"}'
         document2 = '{"product_id":"test2"}'
 
         assert t.tft_createindex(index, mappings)
         assert t.tft_adddoc(index, document1, doc_id="00001") == '{"_id":"00001"}'
         assert t.tft_updatedocfield(index, "00001", document2)
+        t.delete(index)
 
     def test_tft_deldocfield(self, t: Tair):
         index = "idx_" + str(uuid.uuid4())
         mappings = """
 {
   "mappings": {
     "_source": { "enabled": true },
@@ -143,14 +213,15 @@
   }
 }"""
         document = '{"product_id":"test1","product_name":"product test"}'
 
         assert t.tft_createindex(index, mappings)
         assert t.tft_adddoc(index, document, doc_id="00001") == '{"_id":"00001"}'
         assert t.tft_deldocfield(index, "00001", ["product_name"]) == 1
+        t.delete(index)
 
     def test_tft_incrlongdocfield(self, t: Tair):
         index = "idx_" + str(uuid.uuid4())
         mappings = """
 {
   "mappings": {
     "_source": { "enabled": true },
@@ -163,14 +234,15 @@
   }
 }"""
         document = '{"product_id":"test1","price":100}'
 
         assert t.tft_createindex(index, mappings)
         assert t.tft_adddoc(index, document, doc_id="00001") == '{"_id":"00001"}'
         assert t.tft_incrlongdocfield(index, "00001", "price", 200) == 300
+        t.delete(index)
 
     def test_tft_incrfloatdocfield(self, t: Tair):
         index = "idx_" + str(uuid.uuid4())
         mappings = """
 {
   "mappings": {
     "_source": { "enabled": true },
@@ -185,14 +257,15 @@
         document = '{"product_id":"test1","price":1.1}'
 
         assert t.tft_createindex(index, mappings)
         assert t.tft_adddoc(index, document, doc_id="00001") == '{"_id":"00001"}'
         assert t.tft_incrfloatdocfield(index, "00001", "price", 2.2) == pytest.approx(
             3.3
         )
+        t.delete(index)
 
     def test_tft_getdoc(self, t: Tair):
         index = "idx_" + str(uuid.uuid4())
         mappings = """
 {
   "mappings": {
     "_source": { "enabled": true },
@@ -209,14 +282,15 @@
         assert t.tft_createindex(index, mappings)
         assert t.tft_adddoc(index, document, doc_id="00001") == '{"_id":"00001"}'
         assert t.tft_getdoc(index, "00002") is None
         assert (
             t.tft_getdoc(index, "00001")
             == '{"_id":"00001","_source":{"product_id":"test1","price":1.1}}'
         )
+        t.delete(index)
 
     def test_tft_exists(self, t: Tair):
         index = "idx_" + str(uuid.uuid4())
         mappings = """
 {
   "mappings": {
     "_source": { "enabled": true },
@@ -230,14 +304,15 @@
 }"""
         document = '{"product_id":"test1","price":1.1}'
 
         assert t.tft_createindex(index, mappings)
         assert t.tft_adddoc(index, document, doc_id="00001") == '{"_id":"00001"}'
         assert t.tft_exists(index, "00001") == 1
         assert t.tft_exists(index, "00002") == 0
+        t.delete(index)
 
     def test_tft_docnum(self, t: Tair):
         index = "idx_" + str(uuid.uuid4())
         mappings = """
 {
   "mappings": {
     "_source": { "enabled": true },
@@ -251,14 +326,15 @@
 }"""
         document1 = '{"product_id":"test1"}'
         document2 = '{"product_id":"test2"}'
 
         assert t.tft_createindex(index, mappings)
         assert t.tft_madddoc(index, {document1: "00001", document2: "00002"})
         assert t.tft_docnum(index) == 2
+        t.delete(index)
 
     def test_tft_scandocid(self, t: Tair):
         index = "idx_" + str(uuid.uuid4())
         mappings = """
 {
   "mappings": {
     "_source": { "enabled": true },
@@ -277,14 +353,15 @@
         assert t.tft_createindex(index, mappings)
         assert t.tft_madddoc(
             index, {document1: "00001", document2: "00002", document3: "00003"}
         )
         assert t.tft_scandocid(index, 0, count=3, match="*") == ScandocidResult(
             "0", ["00001", "00002", "00003"]
         )
+        t.delete(index)
 
     def test_tft_deldoc(self, t: Tair):
         index = "idx_" + str(uuid.uuid4())
         mappings = """
 {
   "mappings": {
     "_source": { "enabled": true },
@@ -296,15 +373,16 @@
     }
   }
 }"""
         document = '{"product_id":"test1","product_name":"product test"}'
 
         assert t.tft_createindex(index, mappings)
         assert t.tft_adddoc(index, document, doc_id="00001") == '{"_id":"00001"}'
-        assert t.tft_deldoc(index, "00001", "00002") == 1
+        assert t.tft_deldoc(index, {"00001", "00002"}) == 1
+        t.delete(index)
 
     def test_tft_delall(self, t: Tair):
         index = "idx_" + str(uuid.uuid4())
         mappings = """
 {
   "mappings": {
     "_source": { "enabled": true },
@@ -317,14 +395,15 @@
   }
 }"""
         document = '{"product_id":"test1","product_name":"product test"}'
 
         assert t.tft_createindex(index, mappings)
         assert t.tft_adddoc(index, document, doc_id="00001") == '{"_id":"00001"}'
         assert t.tft_delall(index)
+        t.delete(index)
 
     def test_tft_search(self, t: Tair):
         index = "idx_" + str(uuid.uuid4())
         mappings = """
 {
   "mappings": {
     "_source": { "enabled": true },
@@ -369,18 +448,23 @@
     ],
     "max_score": 1.0,
     "total": {{ "relation": "eq", "value": 3 }}
   }}
 }}"""
         result = t.tft_search(index, '{"sort":[{"price":{"order":"desc"}}]}')
         assert json.loads(want) == json.loads(result)
+        result = t.tft_search(index, '{"sort":[{"price":{"order":"desc"}}]}', True)
+        assert json.loads(want) == json.loads(result)
+        result = t.tft_explaincost(index, '{"sort":[{"price":{"order":"desc"}}]}')
+        assert json.loads(result)['QUERY_COST']
+        t.delete(index)
 
     def test_tft_msearch(self, t: Tair):
-        index1 = "idx_" + str(uuid.uuid4())
-        index2 = "idx_" + str(uuid.uuid4())
+        index1 = "{idx}_" + str(uuid.uuid4())
+        index2 = "{idx}_" + str(uuid.uuid4())
         mappings = """
 {
   "mappings": {
     "_source": { "enabled": true },
     "properties": {
       "product_id": { "type": "keyword", "ignore_above": 128 },
       "product_name": { "type": "text" },
@@ -432,66 +516,103 @@
             "_source": {{ "product_id": "test4" }}
           }}
         ],
         "max_score": 1.0,
         "total": {{ "relation": "eq", "value": 4 }}
       }}
     }}"""
-        result = t.tft_msearch(2, {index1, index2}, '{"sort":[{"price":{"order":"desc"}}]}')
+        result = t.tft_msearch(2, {index1, index2}, '{"sort":[{"_doc":{"order":"asc"}}]}')
         assert json.loads(want) == json.loads(result)
+        t.delete(index1)
+        t.delete(index2)
+
+    def test_tft_analyzer(self, t: Tair):
+        index = "idx_" + str(uuid.uuid4())
+        mappings = """
+{
+  "mappings":{
+    "properties":{
+      "f0":{
+        "type":"text",
+        "analyzer":"my_analyzer"
+      }
+    }
+  },
+  "settings":{
+    "analysis":{
+      "analyzer":{
+        "my_analyzer":{
+          "type":"standard"
+        }
+      }
+    }
+  }
+}"""
+        text = 'This is tair-py.'
+
+        assert t.tft_createindex(index, mappings)
+        assert t.tft_analyzer("standard", text) == t.tft_analyzer("my_analyzer", text, index)
+        assert 'consuming time' in str(t.tft_analyzer("standard", text, None, True))
+
+        t.delete(index)
 
     def test_tft_addsug(self, t: Tair):
         index = "idx_" + str(uuid.uuid4())
 
         assert (
             t.tft_addsug(index, {"redis is a memory database": 3, "redis cluster": 10})
             == 2
         )
+        t.delete(index)
 
     def test_tft_delsug(self, t: Tair):
         index = "idx_" + str(uuid.uuid4())
 
         assert (
             t.tft_addsug(index, {"redis is a memory database": 3, "redis cluster": 10})
             == 2
         )
         assert t.tft_delsug(index, ("redis is a memory database", "redis cluster")) == 2
+        t.delete(index)
 
     def test_tft_sugnum(self, t: Tair):
         index = "idx_" + str(uuid.uuid4())
 
         assert (
             t.tft_addsug(index, {"redis is a memory database": 3, "redis cluster": 10})
             == 2
         )
         assert t.tft_sugnum(index) == 2
+        t.delete(index)
 
     def test_tft_getsug(self, t: Tair):
         index = "idx_" + str(uuid.uuid4())
 
         assert (
             t.tft_addsug(index, {"redis is a memory database": 3, "redis cluster": 10})
             == 2
         )
         assert sorted(t.tft_getsug(index, "res", max_count=2, fuzzy=True)) == [
             "redis cluster",
             "redis is a memory database",
         ]
+        t.delete(index)
 
     def test_tft_getallsugs(self, t: Tair):
         index = "idx_" + str(uuid.uuid4())
 
         assert (
             t.tft_addsug(index, {"redis is a memory database": 3, "redis cluster": 10})
             == 2
         )
         assert sorted(t.tft_getallsugs(index)) == [
             "redis cluster",
             "redis is a memory database",
         ]
+        t.delete(index)
 
     def test_scandocid_result_eq(self):
         assert ScandocidResult("0", ["00001", "00002", "00003"]) == ScandocidResult(
             "0", ["00001", "00002", "00003"]
         )
         assert not ScandocidResult("0", ["00001", "00002", "00003"]) == ScandocidResult(
             "0", ["00001", "00002"]
```

### Comparing `tair-1.3.2/tests/test_tairstring.py` & `tair-1.3.3/tests/test_tairstring.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tests/test_tairts.py` & `tair-1.3.3/tests/test_tairts.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tests/test_tairvector.py` & `tair-1.3.3/tests/test_tairvector.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.2/tests/test_tairzset.py` & `tair-1.3.3/tests/test_tairzset.py`

 * *Files identical despite different names*

