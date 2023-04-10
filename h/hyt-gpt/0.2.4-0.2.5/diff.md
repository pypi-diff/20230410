# Comparing `tmp/hyt-gpt-0.2.4.tar.gz` & `tmp/hyt-gpt-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyt-gpt-0.2.4.tar", last modified: Sun Apr  9 17:30:28 2023, max compression
+gzip compressed data, was "hyt-gpt-0.2.5.tar", last modified: Mon Apr 10 05:25:44 2023, max compression
```

## Comparing `hyt-gpt-0.2.4.tar` & `hyt-gpt-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-04-09 17:30:28.616542 hyt-gpt-0.2.4/
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-04-09 17:30:28.616542 hyt-gpt-0.2.4/PKG-INFO
-drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-04-09 17:30:28.616542 hyt-gpt-0.2.4/hyt_gpt/
--rw-rw-r--   0 haibin    (1000) haibin    (1000)        0 2023-03-26 03:01:59.000000 hyt-gpt-0.2.4/hyt_gpt/__init__.py
--rw-rw-r--   0 haibin    (1000) haibin    (1000)     3736 2023-04-09 17:29:47.000000 hyt-gpt-0.2.4/hyt_gpt/gpt.py
--rw-rw-r--   0 haibin    (1000) haibin    (1000)     2886 2023-03-26 03:01:59.000000 hyt-gpt-0.2.4/hyt_gpt/notion.py
--rw-rw-r--   0 haibin    (1000) haibin    (1000)     6366 2023-04-09 15:45:37.000000 hyt-gpt-0.2.4/hyt_gpt/youtube.py
-drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-04-09 17:30:28.616542 hyt-gpt-0.2.4/hyt_gpt.egg-info/
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-04-09 17:30:28.000000 hyt-gpt-0.2.4/hyt_gpt.egg-info/PKG-INFO
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      204 2023-04-09 17:30:28.000000 hyt-gpt-0.2.4/hyt_gpt.egg-info/SOURCES.txt
--rw-rw-r--   0 haibin    (1000) haibin    (1000)        1 2023-04-09 17:30:28.000000 hyt-gpt-0.2.4/hyt_gpt.egg-info/dependency_links.txt
--rw-rw-r--   0 haibin    (1000) haibin    (1000)        8 2023-04-09 17:30:28.000000 hyt-gpt-0.2.4/hyt_gpt.egg-info/top_level.txt
--rw-rw-r--   0 haibin    (1000) haibin    (1000)       38 2023-04-09 17:30:28.616542 hyt-gpt-0.2.4/setup.cfg
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      837 2023-04-09 17:30:19.000000 hyt-gpt-0.2.4/setup.py
+drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-04-10 05:25:44.227964 hyt-gpt-0.2.5/
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-04-10 05:25:44.227964 hyt-gpt-0.2.5/PKG-INFO
+drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-04-10 05:25:44.227964 hyt-gpt-0.2.5/hyt_gpt/
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)        0 2023-03-26 03:01:59.000000 hyt-gpt-0.2.5/hyt_gpt/__init__.py
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)     4000 2023-04-10 05:20:52.000000 hyt-gpt-0.2.5/hyt_gpt/gpt.py
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)     2886 2023-03-26 03:01:59.000000 hyt-gpt-0.2.5/hyt_gpt/notion.py
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)     6366 2023-04-10 05:21:38.000000 hyt-gpt-0.2.5/hyt_gpt/youtube.py
+drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-04-10 05:25:44.227964 hyt-gpt-0.2.5/hyt_gpt.egg-info/
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-04-10 05:25:44.000000 hyt-gpt-0.2.5/hyt_gpt.egg-info/PKG-INFO
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      204 2023-04-10 05:25:44.000000 hyt-gpt-0.2.5/hyt_gpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)        1 2023-04-10 05:25:44.000000 hyt-gpt-0.2.5/hyt_gpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)        8 2023-04-10 05:25:44.000000 hyt-gpt-0.2.5/hyt_gpt.egg-info/top_level.txt
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)       38 2023-04-10 05:25:44.227964 hyt-gpt-0.2.5/setup.cfg
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      837 2023-04-10 05:25:41.000000 hyt-gpt-0.2.5/setup.py
```

### Comparing `hyt-gpt-0.2.4/PKG-INFO` & `hyt-gpt-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyt-gpt
-Version: 0.2.4
+Version: 0.2.5
 Summary: A library for GPT and Youtube
 Author: Harbin
 Author-email: harbinfate@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyt-gpt-0.2.4/hyt_gpt/gpt.py` & `hyt-gpt-0.2.5/hyt_gpt/gpt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 from typing import List
 import logging
+import tiktoken
 
 
 def chat_gpt(key, prompt, text):
     API_KEY = key
     headers = {
         'Content-Type': 'application/json',
         'Authorization': f'Bearer {API_KEY}',
@@ -27,24 +28,24 @@
 
 
 def seg_transcript(transcript: List[str]) -> List[str]:
     transcript = [{"text": item["text"], "index": index,
                    "timestamp": item["start"]} for index, item in enumerate(transcript)]
     text = " ".join([x["text"]
                     for x in sorted(transcript, key=lambda x: x["index"])])
-    len_original = len(text)
-    seg_length = 4096
+    enc = tiktoken.get_encoding("cl100k_base")
+    len_original = len(enc.encode(text))
+    seg_length = 4000
     if len_original >= seg_length:
-        chunkedText = getChunckedTranscripts(transcript, transcript)
+        chunkedText = getChunckedTranscripts(transcript, transcript, enc)
         print(
-            f'Transcript length: {len_original} is too long, truncated via lossy compression to {len(chunkedText)}.')
+            f'Transcript token length: {len_original} is too long, truncated via lossy compression to {len(enc.encode(chunkedText))}.')
         return [chunkedText]
-    length = len(text)
-    print(f'Processing text length: {length}.')
-    n = length // seg_length + 1
+    print(f'Processing text token length: {len_original}.')
+    n = len_original // seg_length + 1
     division = len(transcript) // n
     new_l = [transcript[i * division: (i + 1) * division] for i in range(n)]
     segedTranscipt = [" ".join([x["text"] for x in sorted(
         j, key=lambda x: x["index"])]) for j in new_l]
     return segedTranscipt
 
 
@@ -54,38 +55,39 @@
 A helpful rule of thumb is that one token generally corresponds to ~4 
 characters of text for common English text. 
 
 This translates to roughly ¾ of a word (so 100 tokens ~= 75 words).
 """
 
 
-def getChunckedTranscripts(textData, textDataOriginal, limit=3072) -> str:
+def getChunckedTranscripts(textData, textDataOriginal, enc, limit=4000) -> str:
 
     result = ""
     text = " ".join([x["text"]
                     for x in sorted(textData, key=lambda x: x["index"])])
 
-    if len(text) > limit:
+    if len(enc.encode(text)) > limit:
         evenTextData = [t for i, t in enumerate(textData) if i % 2 == 0]
-        result = getChunckedTranscripts(evenTextData, textDataOriginal)
+        result = getChunckedTranscripts(evenTextData, textDataOriginal, enc)
     else:
         if len(textDataOriginal) != len(textData):
             for obj in textDataOriginal:
                 if any(t["text"] == obj["text"] for t in textData):
                     continue
                 textData.append(obj)
                 newText = " ".join([x["text"] for x in sorted(
                     textData, key=lambda x: x["index"])])
-
-                if len(newText) < limit:
+                newTextTokenLength = len(enc.encode(newText))
+                if newTextTokenLength < limit:
                     nextText = textDataOriginal[[
                         t["text"] for t in textDataOriginal].index(obj["text"]) + 1]
-                    if len(newText) + len(nextText["text"]) > limit:
-                        overRate = ((len(newText) + len(nextText["text"])) -
-                                    limit) / len(nextText["text"])
+                    nextTextTokenLength = len(enc.encode(nextText["text"]))
+                    if newTextTokenLength + nextTextTokenLength > limit:
+                        overRate = ((newTextTokenLength + nextTextTokenLength) -
+                                    limit) / nextTextTokenLength
                         chunkedText = nextText["text"][:int(
                             len(nextText["text"])*overRate)]
                         textData.append(
                             {"text": chunkedText, "index": nextText["index"]})
                         result = " ".join([x["text"] for x in sorted(
                             textData, key=lambda x: x["index"])])
```

### Comparing `hyt-gpt-0.2.4/hyt_gpt/notion.py` & `hyt-gpt-0.2.5/hyt_gpt/notion.py`

 * *Files identical despite different names*

### Comparing `hyt-gpt-0.2.4/hyt_gpt/youtube.py` & `hyt-gpt-0.2.5/hyt_gpt/youtube.py`

 * *Files identical despite different names*

### Comparing `hyt-gpt-0.2.4/hyt_gpt.egg-info/PKG-INFO` & `hyt-gpt-0.2.5/hyt_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyt-gpt
-Version: 0.2.4
+Version: 0.2.5
 Summary: A library for GPT and Youtube
 Author: Harbin
 Author-email: harbinfate@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyt-gpt-0.2.4/setup.py` & `hyt-gpt-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages, find_namespace_packages
 
 setup(
     name='hyt-gpt',
-    version='0.2.4',
+    version='0.2.5',
     description='A library for GPT and Youtube',
     author='Harbin',
     author_email='harbinfate@gmail.com',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

