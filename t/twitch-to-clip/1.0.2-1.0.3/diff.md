# Comparing `tmp/twitch-to-clip-1.0.2.tar.gz` & `tmp/twitch-to-clip-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitch-to-clip-1.0.2.tar", last modified: Mon Apr 10 15:42:19 2023, max compression
+gzip compressed data, was "twitch-to-clip-1.0.3.tar", last modified: Mon Apr 10 15:46:47 2023, max compression
```

## Comparing `twitch-to-clip-1.0.2.tar` & `twitch-to-clip-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       34 2023-04-10 15:35:13.923220 twitch-to-clip-1.0.2/.gitignore
--rw-r--r--   0        0        0    34821 2023-04-10 13:03:14.407817 twitch-to-clip-1.0.2/LICENSE
--rw-r--r--   0        0        0     3126 2023-04-10 15:38:35.898970 twitch-to-clip-1.0.2/README.md
--rw-r--r--   0        0        0      560 2023-04-10 15:42:11.077918 twitch-to-clip-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      331 2023-04-10 11:23:16.937249 twitch-to-clip-1.0.2/setup.py
--rw-r--r--   0        0        0       73 2023-04-10 15:41:52.695951 twitch-to-clip-1.0.2/twitch_to_clip/__init__.py
--rw-r--r--   0        0        0     1250 2023-04-10 11:23:52.904611 twitch-to-clip-1.0.2/twitch_to_clip/__main__.py
--rw-r--r--   0        0        0      539 2023-04-10 12:40:26.882091 twitch-to-clip-1.0.2/twitch_to_clip/create_short.py
--rw-r--r--   0        0        0      842 2023-04-10 13:26:52.737595 twitch-to-clip-1.0.2/twitch_to_clip/dl_and_create.py
--rw-r--r--   0        0        0     2093 2023-04-10 13:33:23.479615 twitch-to-clip-1.0.2/twitch_to_clip/dl_twitch.py
--rw-r--r--   0        0        0     1528 2023-04-10 13:22:53.294093 twitch-to-clip-1.0.2/twitch_to_clip/ffmpeg_funcs.py
--rw-r--r--   0        0        0     3366 1970-01-01 00:00:00.000000 twitch-to-clip-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       34 2023-04-10 15:35:13.923220 twitch-to-clip-1.0.3/.gitignore
+-rw-r--r--   0        0        0    34821 2023-04-10 13:03:14.407817 twitch-to-clip-1.0.3/LICENSE
+-rw-r--r--   0        0        0     3126 2023-04-10 15:38:35.898970 twitch-to-clip-1.0.3/README.md
+-rw-r--r--   0        0        0      578 2023-04-10 15:46:46.206366 twitch-to-clip-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      331 2023-04-10 11:23:16.937249 twitch-to-clip-1.0.3/setup.py
+-rw-r--r--   0        0        0       73 2023-04-10 15:45:50.881088 twitch-to-clip-1.0.3/twitch_to_clip/__init__.py
+-rw-r--r--   0        0        0     1250 2023-04-10 11:23:52.904611 twitch-to-clip-1.0.3/twitch_to_clip/__main__.py
+-rw-r--r--   0        0        0      539 2023-04-10 12:40:26.882091 twitch-to-clip-1.0.3/twitch_to_clip/create_short.py
+-rw-r--r--   0        0        0      842 2023-04-10 13:26:52.737595 twitch-to-clip-1.0.3/twitch_to_clip/dl_and_create.py
+-rw-r--r--   0        0        0     2093 2023-04-10 13:33:23.479615 twitch-to-clip-1.0.3/twitch_to_clip/dl_twitch.py
+-rw-r--r--   0        0        0     1528 2023-04-10 13:22:53.294093 twitch-to-clip-1.0.3/twitch_to_clip/ffmpeg_funcs.py
+-rw-r--r--   0        0        0     3432 1970-01-01 00:00:00.000000 twitch-to-clip-1.0.3/PKG-INFO
```

### Comparing `twitch-to-clip-1.0.2/LICENSE` & `twitch-to-clip-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `twitch-to-clip-1.0.2/README.md` & `twitch-to-clip-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `twitch-to-clip-1.0.2/pyproject.toml` & `twitch-to-clip-1.0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 
 [project]
 name="twitch-to-clip"
 authors = [
     {name = "Emmanuil Borovikovs", email = "eb.dev.99@gmail.com"},
 ]
 readme="README.md"
-repository = "https://github.com/EB1811/twitch-to-clip"
 classifiers=[
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)"
 ]
 requires-python=">=3.7"
 dynamic=[
     "version",
     "description",
 ]
 dependencies=[
     "twitch-dl>=2.*",
 ]
 
 [project.scripts]
-twitch-to-clip = "twitch_to_clip.__main__:main"
+twitch-to-clip = "twitch_to_clip.__main__:main"
+
+[project.urls]
+repository = "https://github.com/EB1811/twitch-to-clip"
```

### Comparing `twitch-to-clip-1.0.2/twitch_to_clip/__main__.py` & `twitch-to-clip-1.0.3/twitch_to_clip/__main__.py`

 * *Files identical despite different names*

### Comparing `twitch-to-clip-1.0.2/twitch_to_clip/create_short.py` & `twitch-to-clip-1.0.3/twitch_to_clip/create_short.py`

 * *Files identical despite different names*

### Comparing `twitch-to-clip-1.0.2/twitch_to_clip/dl_and_create.py` & `twitch-to-clip-1.0.3/twitch_to_clip/dl_and_create.py`

 * *Files identical despite different names*

### Comparing `twitch-to-clip-1.0.2/twitch_to_clip/dl_twitch.py` & `twitch-to-clip-1.0.3/twitch_to_clip/dl_twitch.py`

 * *Files identical despite different names*

### Comparing `twitch-to-clip-1.0.2/twitch_to_clip/ffmpeg_funcs.py` & `twitch-to-clip-1.0.3/twitch_to_clip/ffmpeg_funcs.py`

 * *Files identical despite different names*

### Comparing `twitch-to-clip-1.0.2/PKG-INFO` & `twitch-to-clip-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: twitch-to-clip
-Version: 1.0.2
+Version: 1.0.3
 Summary: Create vertical videos from twitch clips
 Author-email: Emmanuil Borovikovs <eb.dev.99@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Dist: twitch-dl>=2.*
+Project-URL: repository, https://github.com/EB1811/twitch-to-clip
 
 Twitch-To-Clip
 =================
 
 CLI tool that allows you to download Twitch clips or highlight videos and convert them into vertical videos ideal for TikTok and YouTube shorts.
 It uses the [twitch-dl](https://github.com/ihabunek/twitch-dl ) and ffmpeg packages to achieve this.
```

