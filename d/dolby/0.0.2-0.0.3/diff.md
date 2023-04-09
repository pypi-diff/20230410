# Comparing `tmp/dolby-0.0.2.tar.gz` & `tmp/dolby-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolby-0.0.2.tar", last modified: Sun Apr  9 22:03:12 2023, max compression
+gzip compressed data, was "dolby-0.0.3.tar", last modified: Sun Apr  9 22:11:12 2023, max compression
```

## Comparing `dolby-0.0.2.tar` & `dolby-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 22:03:12.633502 dolby-0.0.2/
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      426 2023-04-09 22:03:12.633241 dolby-0.0.2/PKG-INFO
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)        7 2023-04-09 20:52:32.000000 dolby-0.0.2/README.md
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      520 2023-04-09 17:12:39.000000 dolby-0.0.2/pyproject.toml
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)       38 2023-04-09 22:03:12.633550 dolby-0.0.2/setup.cfg
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 22:03:12.621189 dolby-0.0.2/src/
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 22:03:12.629521 dolby-0.0.2/src/dolby/
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)     1849 2023-04-09 21:56:51.000000 dolby-0.0.2/src/dolby/DolbyAudio.py
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)     2709 2023-04-09 21:56:17.000000 dolby-0.0.2/src/dolby/DolbyImage.py
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      158 2023-04-09 20:59:29.000000 dolby-0.0.2/src/dolby/DolbyText.py
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)     1835 2023-04-09 21:57:37.000000 dolby-0.0.2/src/dolby/DolbyVideo.py
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)     2224 2023-04-09 21:59:54.000000 dolby-0.0.2/src/dolby/YouTube.py
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      164 2023-04-09 19:41:00.000000 dolby-0.0.2/src/dolby/__init__.py
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)     1279 2023-04-09 21:52:25.000000 dolby-0.0.2/src/dolby/constants.py
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      801 2023-04-09 21:58:18.000000 dolby-0.0.2/src/dolby/override.py
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 22:03:12.632782 dolby-0.0.2/src/dolby.egg-info/
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      426 2023-04-09 22:03:12.000000 dolby-0.0.2/src/dolby.egg-info/PKG-INFO
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      351 2023-04-09 22:03:12.000000 dolby-0.0.2/src/dolby.egg-info/SOURCES.txt
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)        1 2023-04-09 22:03:12.000000 dolby-0.0.2/src/dolby.egg-info/dependency_links.txt
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)       18 2023-04-09 22:03:12.000000 dolby-0.0.2/src/dolby.egg-info/top_level.txt
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      499 2023-04-09 22:02:17.000000 dolby-0.0.2/src/test.py
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 22:11:12.777801 dolby-0.0.3/
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      426 2023-04-09 22:11:12.777476 dolby-0.0.3/PKG-INFO
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)        7 2023-04-09 20:52:32.000000 dolby-0.0.3/README.md
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      612 2023-04-09 22:10:54.000000 dolby-0.0.3/pyproject.toml
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)       38 2023-04-09 22:11:12.777849 dolby-0.0.3/setup.cfg
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 22:11:12.759135 dolby-0.0.3/src/
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 22:11:12.773723 dolby-0.0.3/src/dolby/
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)     1841 2023-04-09 22:05:10.000000 dolby-0.0.3/src/dolby/DolbyAudio.py
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)     2677 2023-04-09 22:07:01.000000 dolby-0.0.3/src/dolby/DolbyImage.py
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      158 2023-04-09 20:59:29.000000 dolby-0.0.3/src/dolby/DolbyText.py
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)     1827 2023-04-09 22:06:12.000000 dolby-0.0.3/src/dolby/DolbyVideo.py
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)     2224 2023-04-09 22:06:23.000000 dolby-0.0.3/src/dolby/YouTube.py
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      164 2023-04-09 19:41:00.000000 dolby-0.0.3/src/dolby/__init__.py
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)     1279 2023-04-09 21:52:25.000000 dolby-0.0.3/src/dolby/constants.py
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      801 2023-04-09 21:58:18.000000 dolby-0.0.3/src/dolby/override.py
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 22:11:12.776565 dolby-0.0.3/src/dolby.egg-info/
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      426 2023-04-09 22:11:12.000000 dolby-0.0.3/src/dolby.egg-info/PKG-INFO
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      383 2023-04-09 22:11:12.000000 dolby-0.0.3/src/dolby.egg-info/SOURCES.txt
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)        1 2023-04-09 22:11:12.000000 dolby-0.0.3/src/dolby.egg-info/dependency_links.txt
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)       49 2023-04-09 22:11:12.000000 dolby-0.0.3/src/dolby.egg-info/requires.txt
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)       11 2023-04-09 22:11:12.000000 dolby-0.0.3/src/dolby.egg-info/top_level.txt
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      499 2023-04-09 22:02:17.000000 dolby-0.0.3/src/test.py
```

### Comparing `dolby-0.0.2/pyproject.toml` & `dolby-0.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dolby"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Gautam Veldanda", email="gautamveldanda@gmail.com" },
 ]
 description = "A Python library for Dolby AI"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+  "selenium",
+  "beautifulsoup4",
+  "icrawler",
+  "openai",
+  "requests"
+]
 [project.urls]
 "Homepage" = "https://github.com/gautamveldanda/dolby"
```

### Comparing `dolby-0.0.2/src/dolby/DolbyAudio.py` & `dolby-0.0.3/src/dolby/DolbyAudio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pathlib import Path
 from .constants import *
 from .YouTube import YouTube
 
 
 class DolbyAudio:
     """
     Class representing a Dolby Audio instance that can download audio from various sources.
@@ -11,15 +12,14 @@
         """
         Constructor method that initializes the path for storing downloaded audio files.
 
         Args:
             path (str): The path to the directory where downloaded audio files will be saved.
         """
         self.path = path
-        from pathlib import Path
         Path(path).mkdir(parents=True, exist_ok=True)
 
     def __youtube__(self, query: str, query_type: QueryType = QueryType.NAME):
         """
         Private method that downloads audio from YouTube given a query string.
 
         Args:
```

### Comparing `dolby-0.0.2/src/dolby/DolbyImage.py` & `dolby-0.0.3/src/dolby/DolbyImage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+import requests
+import openai
 from pathlib import Path
 from icrawler.builtin import GoogleImageCrawler
 from .constants import *
 from .override import *
+import logging
+logging.basicConfig(level=logging.WARNING)
 
 
 class DolbyImage:
     def init(self, path, OPENAI_API_KEY=None, PEEXELS_API_KEY=None):
         """
         Initialize DolbyImage object with the path to the directory where the image will be stored,
         and the API keys for OpenAI and Pexels APIs if needed.
@@ -25,22 +29,20 @@
     def __openai__(self, query: str):
         """
         Private method to download an image using OpenAI API.
 
         Args:
         - query: str, the search query for the image
         """
-        import openai
         openai.api_key = self.openai_api_key
         response = openai.Image.create(
             prompt=query,
             size="full",
         )
         url = response["data"][0]["url"]  # type: ignore
-        import requests
         data = requests.get(url).content
         with open(f"{self.path}/image.png", 'wb') as handler:
             handler.write(data)
 
     def __pexels__(self, query: str):
         """
         Private method to download an image using Pexels API.
@@ -53,16 +55,14 @@
     def __google__(self, query: str):
         """
         Private method to download an image using Google Image search.
 
         Args:
         - query: str, the search query for the image
         """
-        import logging
-        logging.basicConfig(level=logging.WARNING)
         self.gc = GoogleImageCrawler(downloader_cls=FileName, storage={
             'root_dir': f"{self.path}"})
         self.gc.crawl(keyword=query, max_num=1,
                       file_idx_offset='auto')  # type: ignore
 
     def download(self, query: str, source: ImageSource = ImageSource.GOOGLE):
         """
```

### Comparing `dolby-0.0.2/src/dolby/DolbyVideo.py` & `dolby-0.0.3/src/dolby/DolbyVideo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pathlib import Path
 from .constants import *
 from .YouTube import YouTube
 
 
 class DolbyVideo:
     """
     Class representing a Dolby Video instance that can download video from various sources.
@@ -11,15 +12,14 @@
         """
         Constructor method that initializes the path for storing downloaded video files.
 
         Args:
             path (str): The path to the directory where downloaded video files will be saved.
         """
         self.path = path
-        from pathlib import Path
         Path(path).mkdir(parents=True, exist_ok=True)
 
     def __youtube__(self, query: str, query_type: QueryType = QueryType.NAME):
         """
         Private method that downloads video from YouTube given a query string.
 
         Args:
```

### Comparing `dolby-0.0.2/src/dolby/YouTube.py` & `dolby-0.0.3/src/dolby/YouTube.py`

 * *Files identical despite different names*

### Comparing `dolby-0.0.2/src/dolby/constants.py` & `dolby-0.0.3/src/dolby/constants.py`

 * *Files identical despite different names*

### Comparing `dolby-0.0.2/src/dolby/override.py` & `dolby-0.0.3/src/dolby/override.py`

 * *Files identical despite different names*

