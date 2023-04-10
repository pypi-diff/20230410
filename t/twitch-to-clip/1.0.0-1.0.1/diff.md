# Comparing `tmp/twitch-to-clip-1.0.0.tar.gz` & `tmp/twitch-to-clip-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitch-to-clip-1.0.0.tar", last modified: Mon Apr 10 15:33:44 2023, max compression
+gzip compressed data, was "twitch-to-clip-1.0.1.tar", last modified: Mon Apr 10 15:38:56 2023, max compression
```

## Comparing `twitch-to-clip-1.0.0.tar` & `twitch-to-clip-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       45 2023-04-10 15:30:25.776794 twitch-to-clip-1.0.0/.gitignore
--rw-r--r--   0        0        0    34821 2023-04-10 13:03:14.407817 twitch-to-clip-1.0.0/LICENSE
--rw-r--r--   0        0        0     2976 2023-04-10 15:21:20.041184 twitch-to-clip-1.0.0/README.md
--rw-r--r--   0        0        0      503 2023-04-10 15:23:48.621330 twitch-to-clip-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      331 2023-04-10 11:23:16.937249 twitch-to-clip-1.0.0/setup.py
--rw-r--r--   0        0        0       73 2023-04-10 15:16:40.186531 twitch-to-clip-1.0.0/twitch_to_clip/__init__.py
--rw-r--r--   0        0        0     1250 2023-04-10 11:23:52.904611 twitch-to-clip-1.0.0/twitch_to_clip/__main__.py
--rw-r--r--   0        0        0      539 2023-04-10 12:40:26.882091 twitch-to-clip-1.0.0/twitch_to_clip/create_short.py
--rw-r--r--   0        0        0      842 2023-04-10 13:26:52.737595 twitch-to-clip-1.0.0/twitch_to_clip/dl_and_create.py
--rw-r--r--   0        0        0     2093 2023-04-10 13:33:23.479615 twitch-to-clip-1.0.0/twitch_to_clip/dl_twitch.py
--rw-r--r--   0        0        0     1528 2023-04-10 13:22:53.294093 twitch-to-clip-1.0.0/twitch_to_clip/ffmpeg_funcs.py
--rw-r--r--   0        0        0     3224 1970-01-01 00:00:00.000000 twitch-to-clip-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       34 2023-04-10 15:35:13.923220 twitch-to-clip-1.0.1/.gitignore
+-rw-r--r--   0        0        0    34821 2023-04-10 13:03:14.407817 twitch-to-clip-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3126 2023-04-10 15:38:35.898970 twitch-to-clip-1.0.1/README.md
+-rw-r--r--   0        0        0      503 2023-04-10 15:23:48.621330 twitch-to-clip-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      331 2023-04-10 11:23:16.937249 twitch-to-clip-1.0.1/setup.py
+-rw-r--r--   0        0        0       73 2023-04-10 15:38:52.200965 twitch-to-clip-1.0.1/twitch_to_clip/__init__.py
+-rw-r--r--   0        0        0     1250 2023-04-10 11:23:52.904611 twitch-to-clip-1.0.1/twitch_to_clip/__main__.py
+-rw-r--r--   0        0        0      539 2023-04-10 12:40:26.882091 twitch-to-clip-1.0.1/twitch_to_clip/create_short.py
+-rw-r--r--   0        0        0      842 2023-04-10 13:26:52.737595 twitch-to-clip-1.0.1/twitch_to_clip/dl_and_create.py
+-rw-r--r--   0        0        0     2093 2023-04-10 13:33:23.479615 twitch-to-clip-1.0.1/twitch_to_clip/dl_twitch.py
+-rw-r--r--   0        0        0     1528 2023-04-10 13:22:53.294093 twitch-to-clip-1.0.1/twitch_to_clip/ffmpeg_funcs.py
+-rw-r--r--   0        0        0     3366 1970-01-01 00:00:00.000000 twitch-to-clip-1.0.1/PKG-INFO
```

### Comparing `twitch-to-clip-1.0.0/LICENSE` & `twitch-to-clip-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twitch-to-clip-1.0.0/README.md` & `twitch-to-clip-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 Twitch-To-Clip
 =================
 
 CLI tool that allows you to download Twitch clips or highlight videos and convert them into vertical videos ideal for TikTok and YouTube shorts.
 It uses the [twitch-dl](https://github.com/ihabunek/twitch-dl ) and ffmpeg packages to achieve this.
 
+Installation
+---------
+
+You can install using pip. Open your terminal and run the following command:
+
+```shell
+pip install twitch-to-clip
+```
 
 Requirements
 ---------
 - Python 3.7 or higher installed on your system
 - [ffmpeg](https://ffmpeg.org/download.html), installed and on the system path
 
 To check if ffmpeg is properly installed on your system, open your terminal and run the following command:
```

### Comparing `twitch-to-clip-1.0.0/twitch_to_clip/__main__.py` & `twitch-to-clip-1.0.1/twitch_to_clip/__main__.py`

 * *Files identical despite different names*

### Comparing `twitch-to-clip-1.0.0/twitch_to_clip/create_short.py` & `twitch-to-clip-1.0.1/twitch_to_clip/create_short.py`

 * *Files identical despite different names*

### Comparing `twitch-to-clip-1.0.0/twitch_to_clip/dl_and_create.py` & `twitch-to-clip-1.0.1/twitch_to_clip/dl_and_create.py`

 * *Files identical despite different names*

### Comparing `twitch-to-clip-1.0.0/twitch_to_clip/dl_twitch.py` & `twitch-to-clip-1.0.1/twitch_to_clip/dl_twitch.py`

 * *Files identical despite different names*

### Comparing `twitch-to-clip-1.0.0/twitch_to_clip/ffmpeg_funcs.py` & `twitch-to-clip-1.0.1/twitch_to_clip/ffmpeg_funcs.py`

 * *Files identical despite different names*

### Comparing `twitch-to-clip-1.0.0/PKG-INFO` & `twitch-to-clip-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 Metadata-Version: 2.1
 Name: twitch-to-clip
-Version: 1.0.0
+Version: 1.0.1
 Summary: Create vertical videos from twitch clips
 Author-email: Emmanuil Borovikovs <eb.dev.99@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Dist: twitch-dl>=2.*
 
 Twitch-To-Clip
 =================
 
 CLI tool that allows you to download Twitch clips or highlight videos and convert them into vertical videos ideal for TikTok and YouTube shorts.
 It uses the [twitch-dl](https://github.com/ihabunek/twitch-dl ) and ffmpeg packages to achieve this.
 
+Installation
+---------
+
+You can install using pip. Open your terminal and run the following command:
+
+```shell
+pip install twitch-to-clip
+```
 
 Requirements
 ---------
 - Python 3.7 or higher installed on your system
 - [ffmpeg](https://ffmpeg.org/download.html), installed and on the system path
 
 To check if ffmpeg is properly installed on your system, open your terminal and run the following command:
```

