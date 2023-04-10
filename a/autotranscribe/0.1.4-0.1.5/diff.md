# Comparing `tmp/autotranscribe-0.1.4.tar.gz` & `tmp/autotranscribe-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotranscribe-0.1.4.tar", max compression
+gzip compressed data, was "autotranscribe-0.1.5.tar", max compression
```

## Comparing `autotranscribe-0.1.4.tar` & `autotranscribe-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1072 2023-03-14 06:55:58.872966 autotranscribe-0.1.4/LICENSE
--rw-r--r--   0        0        0      841 2023-03-14 13:04:33.585886 autotranscribe-0.1.4/README.md
--rw-r--r--   0        0        0       85 2023-03-14 12:33:46.135480 autotranscribe-0.1.4/autotranscribe/__init__.py
--rw-r--r--   0        0        0      837 2023-03-17 06:09:18.561741 autotranscribe-0.1.4/autotranscribe/advanced.py
--rw-r--r--   0        0        0      445 2023-03-17 06:20:05.441494 autotranscribe-0.1.4/autotranscribe/splitter.py
--rw-r--r--   0        0        0     2638 2023-03-21 05:57:01.615553 autotranscribe-0.1.4/autotranscribe/transcriber.py
--rw-r--r--   0        0        0     1182 2023-03-21 05:57:24.752344 autotranscribe-0.1.4/autotranscribe/videoproc.py
--rw-r--r--   0        0        0      803 2023-03-21 06:01:03.703395 autotranscribe-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1956 1970-01-01 00:00:00.000000 autotranscribe-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-14 06:55:58.872966 autotranscribe-0.1.5/LICENSE
+-rw-r--r--   0        0        0      841 2023-03-14 13:04:33.585886 autotranscribe-0.1.5/README.md
+-rw-r--r--   0        0        0       85 2023-03-14 12:33:46.135480 autotranscribe-0.1.5/autotranscribe/__init__.py
+-rw-r--r--   0        0        0      851 2023-03-21 06:09:17.870792 autotranscribe-0.1.5/autotranscribe/advanced.py
+-rw-r--r--   0        0        0      445 2023-03-17 06:20:05.441494 autotranscribe-0.1.5/autotranscribe/splitter.py
+-rw-r--r--   0        0        0     2623 2023-03-21 06:42:26.376756 autotranscribe-0.1.5/autotranscribe/transcribe_cli.py
+-rw-r--r--   0        0        0     2638 2023-03-21 05:57:01.615553 autotranscribe-0.1.5/autotranscribe/transcriber.py
+-rw-r--r--   0        0        0     1160 2023-04-10 06:05:37.966271 autotranscribe-0.1.5/autotranscribe/videoproc.py
+-rw-r--r--   0        0        0      803 2023-04-10 06:06:00.472635 autotranscribe-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1956 1970-01-01 00:00:00.000000 autotranscribe-0.1.5/PKG-INFO
```

### Comparing `autotranscribe-0.1.4/LICENSE` & `autotranscribe-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autotranscribe-0.1.4/README.md` & `autotranscribe-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `autotranscribe-0.1.4/autotranscribe/advanced.py` & `autotranscribe-0.1.5/autotranscribe/advanced.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import whisper
 from autotranscribe.splitter import split
 from datetime import timedelta
 import multiprocessing
 import psutil
 import shutil
 import sys
+import os
 
 model = whisper.load_model("large")
 
 
 def subproc(path):
     result = model.transcribe(path, fp16=False)
     return result["text"]
@@ -17,15 +18,15 @@
 def result_multi(file_in, file_out):
 
     files = split(file_in)
     cpus = psutil.cpu_count(logical=True)
     process = cpus - 2
     if files < process:
         process = files
-    
+        
     pool = multiprocessing.Pool(process)
     processes = [pool.apply_async(subproc, args=("process_chunks/chunk{0}.wav".format(x),)) for x in range(files)]
 
     with open(file_out, "w") as f:
         for p in processes:
             f.write(p.get())
```

### Comparing `autotranscribe-0.1.4/autotranscribe/transcriber.py` & `autotranscribe-0.1.5/autotranscribe/transcriber.py`

 * *Files identical despite different names*

### Comparing `autotranscribe-0.1.4/autotranscribe/videoproc.py` & `autotranscribe-0.1.5/autotranscribe/videoproc.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
     h, m, s = time_str.split(':')
     return int(h) * 3600 + int(m) * 60 + int(s)
 
 
 def youtube_preprocess(link, start = None, end = None):
 
-    print(start, end)
     yt = pytube.YouTube(link)
     yt.register_on_progress_callback(show_progress_bar)
     destination = '.'
     video = yt.streams.filter(only_audio = True).first()
 
     out_file = video.download(output_path=destination)
```

### Comparing `autotranscribe-0.1.4/pyproject.toml` & `autotranscribe-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autotranscribe"
-version = "0.1.4"
+version = "0.1.5"
 description = "An auto transcription service for youtube and normal videos."
 authors = ["Devesh Paragiri <devesh.paragiri@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/DeveshParagiri/auto-transcribe"
 keywords = ["transcription", "text", "speech to text"]
 classifiers = [
```

### Comparing `autotranscribe-0.1.4/PKG-INFO` & `autotranscribe-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotranscribe
-Version: 0.1.4
+Version: 0.1.5
 Summary: An auto transcription service for youtube and normal videos.
 Home-page: https://github.com/DeveshParagiri/auto-transcribe
 License: MIT
 Keywords: transcription,text,speech to text
 Author: Devesh Paragiri
 Author-email: devesh.paragiri@gmail.com
 Requires-Python: >=3.8,<4.0
```

