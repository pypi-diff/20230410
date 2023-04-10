# Comparing `tmp/ytpodgen-0.2.4.tar.gz` & `tmp/ytpodgen-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytpodgen-0.2.4.tar", max compression
+gzip compressed data, was "ytpodgen-0.2.5.tar", max compression
```

## Comparing `ytpodgen-0.2.4.tar` & `ytpodgen-0.2.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-03-27 04:22:24.231435 ytpodgen-0.2.4/LICENSE
--rw-r--r--   0        0        0     3019 2023-04-01 03:12:31.866761 ytpodgen-0.2.4/README.md
--rw-r--r--   0        0        0      616 2023-04-10 03:48:04.648702 ytpodgen-0.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-27 04:22:24.232397 ytpodgen-0.2.4/ytpodgen/__init__.py
--rw-r--r--   0        0        0     1527 2023-04-08 05:51:59.526544 ytpodgen-0.2.4/ytpodgen/downloader.py
--rw-r--r--   0        0        0     1225 2023-04-10 03:41:14.385965 ytpodgen-0.2.4/ytpodgen/feedgenerator.py
--rw-r--r--   0        0        0     1795 2023-04-08 05:56:06.207718 ytpodgen-0.2.4/ytpodgen/uploader.py
--rw-r--r--   0        0        0     2870 2023-04-10 03:32:52.623757 ytpodgen-0.2.4/ytpodgen/ytpodgen.py
--rw-r--r--   0        0        0     3809 1970-01-01 00:00:00.000000 ytpodgen-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-03-27 04:22:24.231435 ytpodgen-0.2.5/LICENSE
+-rw-r--r--   0        0        0     3019 2023-04-01 03:12:31.866761 ytpodgen-0.2.5/README.md
+-rw-r--r--   0        0        0      616 2023-04-10 05:16:14.794097 ytpodgen-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-27 04:22:24.232397 ytpodgen-0.2.5/ytpodgen/__init__.py
+-rw-r--r--   0        0        0     1631 2023-04-10 05:13:17.721804 ytpodgen-0.2.5/ytpodgen/downloader.py
+-rw-r--r--   0        0        0     1225 2023-04-10 03:41:14.385965 ytpodgen-0.2.5/ytpodgen/feedgenerator.py
+-rw-r--r--   0        0        0     1795 2023-04-08 05:56:06.207718 ytpodgen-0.2.5/ytpodgen/uploader.py
+-rw-r--r--   0        0        0     2870 2023-04-10 03:32:52.623757 ytpodgen-0.2.5/ytpodgen/ytpodgen.py
+-rw-r--r--   0        0        0     3809 1970-01-01 00:00:00.000000 ytpodgen-0.2.5/PKG-INFO
```

### Comparing `ytpodgen-0.2.4/LICENSE` & `ytpodgen-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ytpodgen-0.2.4/README.md` & `ytpodgen-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ytpodgen-0.2.4/pyproject.toml` & `ytpodgen-0.2.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ytpodgen"
-version = "0.2.4"
+version = "0.2.5"
 description = "turns YouTube live streams into podcasts"
 license = "MIT"
 authors = ["harupong <harupong@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/harupong/ytpodgen"
 
 [tool.poetry.dependencies]
```

### Comparing `ytpodgen-0.2.4/ytpodgen/downloader.py` & `ytpodgen-0.2.5/ytpodgen/downloader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from yt_dlp import YoutubeDL
+import yt_dlp
 
 
 class Downloader:
     def __init__(self):
         pass
 
     @staticmethod
@@ -28,17 +28,20 @@
             ],
             "postprocessor_args": [
                 "-ac",
                 "1",  # audio channel mono
             ],
         }
 
-        with YoutubeDL(ydl_opts) as ydl:
+        with yt_dlp.YoutubeDL(ydl_opts) as ydl:
             ydl.download(liveurl)
 
     @staticmethod
     def _is_live(liveurl):
         ydl_opts = {}
-        with YoutubeDL(ydl_opts) as ydl:
-            info = ydl.extract_info(liveurl, download=False)
-            live_status = info["live_status"].rstrip("\n")
-            return True if live_status == "is_live" else False
+        with yt_dlp.YoutubeDL(ydl_opts) as ydl:
+            try:
+                info = ydl.extract_info(liveurl, download=False)
+                live_status = info["live_status"].rstrip("\n")
+                return True if live_status == "is_live" else False
+            except yt_dlp.utils.DownloadError:
+                return False
```

### Comparing `ytpodgen-0.2.4/ytpodgen/feedgenerator.py` & `ytpodgen-0.2.5/ytpodgen/feedgenerator.py`

 * *Files identical despite different names*

### Comparing `ytpodgen-0.2.4/ytpodgen/uploader.py` & `ytpodgen-0.2.5/ytpodgen/uploader.py`

 * *Files identical despite different names*

### Comparing `ytpodgen-0.2.4/ytpodgen/ytpodgen.py` & `ytpodgen-0.2.5/ytpodgen/ytpodgen.py`

 * *Files identical despite different names*

### Comparing `ytpodgen-0.2.4/PKG-INFO` & `ytpodgen-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytpodgen
-Version: 0.2.4
+Version: 0.2.5
 Summary: turns YouTube live streams into podcasts
 Home-page: https://github.com/harupong/ytpodgen
 License: MIT
 Author: harupong
 Author-email: harupong@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ytpodgen Version: 0.2.4 Summary: turns YouTube live
+Metadata-Version: 2.1 Name: ytpodgen Version: 0.2.5 Summary: turns YouTube live
 streams into podcasts Home-page: https://github.com/harupong/ytpodgen License:
 MIT Author: harupong Author-email: harupong@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: boto3
 (>=1.26.89,<2.0.0) Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist: loguru
 (>=0.6.0,<0.7.0) Requires-Dist: podgen (>=1.1.0,<2.0.0) Requires-Dist: requests
```

