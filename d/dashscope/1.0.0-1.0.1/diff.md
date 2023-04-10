# Comparing `tmp/dashscope-1.0.0.tar.gz` & `tmp/dashscope-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dashscope-1.0.0.tar", last modified: Mon Apr 10 09:14:27 2023, max compression
+gzip compressed data, was "dist/dashscope-1.0.1.tar", last modified: Mon Apr 10 10:57:48 2023, max compression
```

## Comparing `dashscope-1.0.0.tar` & `dashscope-1.0.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 09:14:27.000000 dashscope-1.0.0/
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)    11413 2023-04-10 08:39:29.000000 dashscope-1.0.0/LICENSE
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     8124 2023-04-10 09:14:27.000000 dashscope-1.0.0/PKG-INFO
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     7301 2023-04-10 09:13:45.000000 dashscope-1.0.0/README.md
-drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 09:14:27.000000 dashscope-1.0.0/dashscope/
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)      835 2023-04-06 08:30:57.000000 dashscope-1.0.0/dashscope/__init__.py
-drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 09:14:27.000000 dashscope-1.0.0/dashscope/aigc/
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)       66 2023-03-31 05:34:25.000000 dashscope-1.0.0/dashscope/aigc/__init__.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     8217 2023-04-10 08:37:22.000000 dashscope-1.0.0/dashscope/aigc/conversation.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     3779 2023-04-10 08:37:22.000000 dashscope-1.0.0/dashscope/aigc/generation.py
-drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 09:14:27.000000 dashscope-1.0.0/dashscope/api_entities/
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)        0 2023-03-31 05:34:25.000000 dashscope-1.0.0/dashscope/api_entities/__init__.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)    10361 2023-04-06 08:30:57.000000 dashscope-1.0.0/dashscope/api_entities/aiohttp_request.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     5310 2023-04-06 08:30:57.000000 dashscope-1.0.0/dashscope/api_entities/api_request_data.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     4057 2023-04-06 08:30:57.000000 dashscope-1.0.0/dashscope/api_entities/api_request_factory.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)      608 2023-04-06 08:30:57.000000 dashscope-1.0.0/dashscope/api_entities/base_request.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     5712 2023-04-06 08:30:57.000000 dashscope-1.0.0/dashscope/api_entities/dashscope_response.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     9401 2023-04-10 08:37:22.000000 dashscope-1.0.0/dashscope/api_entities/http_request.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)    15625 2023-04-06 08:30:57.000000 dashscope-1.0.0/dashscope/api_entities/websocket_request.py
-drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 09:14:27.000000 dashscope-1.0.0/dashscope/audio/
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)       35 2023-03-31 05:34:25.000000 dashscope-1.0.0/dashscope/audio/__init__.py
-drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 09:14:27.000000 dashscope-1.0.0/dashscope/audio/asr/
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)       75 2023-04-06 08:30:57.000000 dashscope-1.0.0/dashscope/audio/asr/__init__.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     5103 2023-04-10 08:37:22.000000 dashscope-1.0.0/dashscope/audio/asr/transcription.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)    13361 2023-04-06 08:30:57.000000 dashscope-1.0.0/dashscope/cli.py
-drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 09:14:27.000000 dashscope-1.0.0/dashscope/client/
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)        0 2023-03-31 05:34:25.000000 dashscope-1.0.0/dashscope/client/__init__.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)    21665 2023-04-06 08:30:57.000000 dashscope-1.0.0/dashscope/client/base_api.py
-drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 09:14:27.000000 dashscope-1.0.0/dashscope/common/
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)        0 2023-03-31 05:34:25.000000 dashscope-1.0.0/dashscope/common/__init__.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     1986 2023-03-31 05:34:25.000000 dashscope-1.0.0/dashscope/common/api_key.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     1940 2023-04-06 08:30:57.000000 dashscope-1.0.0/dashscope/common/constants.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)      907 2023-04-06 08:30:57.000000 dashscope-1.0.0/dashscope/common/env.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     1592 2023-04-06 08:30:57.000000 dashscope-1.0.0/dashscope/common/error.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)      984 2023-03-31 05:34:25.000000 dashscope-1.0.0/dashscope/common/logging.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     3330 2023-04-06 08:30:57.000000 dashscope-1.0.0/dashscope/common/utils.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     3445 2023-04-06 08:30:57.000000 dashscope-1.0.0/dashscope/deployment.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     3753 2023-04-06 08:30:57.000000 dashscope-1.0.0/dashscope/file.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     4808 2023-04-06 08:30:57.000000 dashscope-1.0.0/dashscope/finetune.py
-drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 09:14:27.000000 dashscope-1.0.0/dashscope/io/
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)        0 2023-03-31 05:34:25.000000 dashscope-1.0.0/dashscope/io/__init__.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     2781 2023-04-06 08:30:57.000000 dashscope-1.0.0/dashscope/io/input_output.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     1696 2023-04-06 08:30:57.000000 dashscope-1.0.0/dashscope/model.py
-drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 09:14:27.000000 dashscope-1.0.0/dashscope/protocol/
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)        0 2023-03-31 05:34:25.000000 dashscope-1.0.0/dashscope/protocol/__init__.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)      561 2023-03-31 05:34:25.000000 dashscope-1.0.0/dashscope/protocol/websocket.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)       22 2023-04-10 08:37:22.000000 dashscope-1.0.0/dashscope/version.py
-drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 09:14:27.000000 dashscope-1.0.0/dashscope.egg-info/
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     8124 2023-04-10 09:14:27.000000 dashscope-1.0.0/dashscope.egg-info/PKG-INFO
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     1294 2023-04-10 09:14:27.000000 dashscope-1.0.0/dashscope.egg-info/SOURCES.txt
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)        1 2023-04-10 09:14:27.000000 dashscope-1.0.0/dashscope.egg-info/dependency_links.txt
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)       49 2023-04-10 09:14:27.000000 dashscope-1.0.0/dashscope.egg-info/entry_points.txt
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)        1 2023-03-31 05:53:35.000000 dashscope-1.0.0/dashscope.egg-info/not-zip-safe
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)       17 2023-04-10 09:14:27.000000 dashscope-1.0.0/dashscope.egg-info/requires.txt
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)       10 2023-04-10 09:14:27.000000 dashscope-1.0.0/dashscope.egg-info/top_level.txt
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)       53 2023-04-10 09:14:27.000000 dashscope-1.0.0/setup.cfg
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     2201 2023-04-10 09:13:51.000000 dashscope-1.0.0/setup.py
+drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 10:57:48.000000 dashscope-1.0.1/
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)    11413 2023-04-10 08:39:29.000000 dashscope-1.0.1/LICENSE
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     7512 2023-04-10 10:57:48.000000 dashscope-1.0.1/PKG-INFO
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     6689 2023-04-10 10:57:41.000000 dashscope-1.0.1/README.md
+drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope/
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)      835 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/__init__.py
+drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope/aigc/
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)       66 2023-03-31 05:34:25.000000 dashscope-1.0.1/dashscope/aigc/__init__.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     8217 2023-04-10 08:37:22.000000 dashscope-1.0.1/dashscope/aigc/conversation.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     3779 2023-04-10 08:37:22.000000 dashscope-1.0.1/dashscope/aigc/generation.py
+drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope/api_entities/
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)        0 2023-03-31 05:34:25.000000 dashscope-1.0.1/dashscope/api_entities/__init__.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)    10361 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/api_entities/aiohttp_request.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     5310 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/api_entities/api_request_data.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     4057 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/api_entities/api_request_factory.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)      608 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/api_entities/base_request.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     5712 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/api_entities/dashscope_response.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     9401 2023-04-10 08:37:22.000000 dashscope-1.0.1/dashscope/api_entities/http_request.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)    15625 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/api_entities/websocket_request.py
+drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope/audio/
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)       35 2023-03-31 05:34:25.000000 dashscope-1.0.1/dashscope/audio/__init__.py
+drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope/audio/asr/
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)       75 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/audio/asr/__init__.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     5103 2023-04-10 08:37:22.000000 dashscope-1.0.1/dashscope/audio/asr/transcription.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)    13361 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/cli.py
+drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope/client/
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)        0 2023-03-31 05:34:25.000000 dashscope-1.0.1/dashscope/client/__init__.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)    21665 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/client/base_api.py
+drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope/common/
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)        0 2023-03-31 05:34:25.000000 dashscope-1.0.1/dashscope/common/__init__.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     1986 2023-03-31 05:34:25.000000 dashscope-1.0.1/dashscope/common/api_key.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     1940 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/common/constants.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)      907 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/common/env.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     1592 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/common/error.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)      984 2023-03-31 05:34:25.000000 dashscope-1.0.1/dashscope/common/logging.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     3330 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/common/utils.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     3445 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/deployment.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     3753 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/file.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     4808 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/finetune.py
+drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope/io/
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)        0 2023-03-31 05:34:25.000000 dashscope-1.0.1/dashscope/io/__init__.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     2781 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/io/input_output.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     1696 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/model.py
+drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope/protocol/
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)        0 2023-03-31 05:34:25.000000 dashscope-1.0.1/dashscope/protocol/__init__.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)      561 2023-03-31 05:34:25.000000 dashscope-1.0.1/dashscope/protocol/websocket.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)       22 2023-04-10 10:57:41.000000 dashscope-1.0.1/dashscope/version.py
+drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope.egg-info/
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     7512 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope.egg-info/PKG-INFO
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     1294 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope.egg-info/SOURCES.txt
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)        1 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope.egg-info/dependency_links.txt
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)       49 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope.egg-info/entry_points.txt
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)        1 2023-03-31 05:53:35.000000 dashscope-1.0.1/dashscope.egg-info/not-zip-safe
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)       17 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope.egg-info/requires.txt
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)       10 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope.egg-info/top_level.txt
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)       53 2023-04-10 10:57:48.000000 dashscope-1.0.1/setup.cfg
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     2201 2023-04-10 09:13:51.000000 dashscope-1.0.1/setup.py
```

### Comparing `dashscope-1.0.0/LICENSE` & `dashscope-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/PKG-INFO` & `dashscope-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dashscope
-Version: 1.0.0
+Version: 1.0.1
 Summary: dashscope client sdk library
 Home-page: https://dashscope.aliyun.com/
 Author: Alibaba
 Author-email: dashscope@alibaba-inc.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -19,16 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h4 align="center">
     <p>
-        <b>English</b> |
-        <a href="https://github.com/dashscope/dashscope/blob/master/README_zh.md">中文</a>
+        <b>English</b>
     <p>
 </h4>
 
 
 </div>
 
 # DashScope Python Library
@@ -47,89 +46,79 @@
 
 
 ## QuickStart
 
 You can use `Conversation` api to directly chat with model qwen-v1(通义千问).
 
 ```python
+from http import HTTPStatus
 import dashscope
 from dashscope import Conversation
 
-dashscope.api_key = '12344343222194ADSSDSSDSDSB9A511ED830AFA4166304A26'
-
-def stream_print(responses):
-    for r in responses:
-        if r.status_code == 200:
-            print(r.output.text.replace('\n', '  '), end='\r')
-            print(r.usage)
-        else:
-            print(r.message)
-
-chat = Conversation()
-
-responses = chat.call('qwen-v1',
-    prompt='以松柏为题，写一首七言诗。',
-    stream=True)
-stream_print(responses)
-
-responses = chat.call('qwen-v1',
-    prompt='现在假设你是一名精通中英双语的学者，将上面这首诗翻译成英文。',
-    stream=True)
-stream_print(responses)
+dashscope.api_key = 'YOUR-DASHSCOPE-API-KEY'
+responses = Generation.call(model=Generation.Models.qwen_v1,
+                            prompt='今天天气好吗？')
+
+if responses.status_code == HTTPStatus.OK:
+    print('Result is: %s' % responses.output)
+else:
+    print('Failed request_id: %s, status_code: %s, code: %s, message:%s' %
+            (responses.request_id, responses.status_code, responses.code,
+            responses.message))
 
 ```
 
 ## API Key Authentication
 
-The SDK uses API key authentication. [Get your API key here](https://aliyuque.antfin.com/zztrg2/zl1nqe/qo56foez7a2hgwyk).
+The SDK uses API key for authentication. Please refer to [official documentation](https://dashscope.aliyun.com) regarding how to obtain your api-key.
 
 ### Using the API Key
 
 1. Set the API key via code
 ```python
 import dashscope
 
-dashscope.api_key = 'your-api-key'
+dashscope.api_key = 'YOUR-DASHSCOPE-API-KEY'
 # Or specify the API key file path via code
 # dashscope.api_key_file_path='~/.dashscope/api_key'
 
 ```
 
 2. Set the API key via environment variables
 
 a. Set the API key directly using the environment variable below
 
 ```python
-export DASHSCOPE_API_KEY='your_api_key'
+export DASHSCOPE_API_KEY='YOUR-DASHSCOPE-API-KEY'
 ```
 
 b. Specify the API key file path via an environment variable
 
 ```python
 export DASHSCOPE_API_KEY_FILE_PATH='~/.dashscope/api_key'
 ```
 
 3. Save the API key to a file
 ```python
 from dashscope import save_api_key
 
-save_api_key(api_key='your_api_key',
+save_api_key(api_key='YOUR-DASHSCOPE-API-KEY',
              api_key_file_path='api_key_file_location or (None, will save to default location "~/.dashscope/api_key"')
 
 ```
 
 
 ## Sample Code
 
-`call` function provides  synchronous call, the function call will return when the whole computing process finish on the server side.
+`call` function provides  synchronous call, the function call will return when computation is done on the server side.
 
 ```python
 from http import HTTPStatus
 from dashscope import Generation
-# export DASHSCOPE_API_KEY='your_api_key' in environment
+# export DASHSCOPE_API_KEY='YOUR-DASHSCOPE-API-KEY' in environment
 def sync_dashscope_sample():
     responses = Generation.call(
         model=Generation.Models.qwen_v1,
         prompt='Is the weather good today?')
 
     if responses.status_code == HTTPStatus.OK:
         print('Result is: %s'%responses.output)
@@ -243,18 +232,12 @@
 ```
 
 ## Error Handling
 Currently, errors are thrown as exceptions.
 
 
 ## Contributing
-We welcome contributions to the DashScope Python SDK! To contribute, please follow these steps:
+Coming soon.
 
-Fork the repository on GitHub.
-Create a new branch for your changes.
-Implement your changes and add tests.
-Make sure all tests pass by running pytest.
-Submit a pull request to the main branch.
-For more information on contributing, please read our contributing guidelines.
 
 ## License
-This project is licensed under the [Apache License (Version 2.0)](https://github.com/dashscope/dashscope/blob/master/LICENSE).
+This project is licensed under the Apache License (Version 2.0).
```

### Comparing `dashscope-1.0.0/README.md` & `dashscope-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 <h4 align="center">
     <p>
-        <b>English</b> |
-        <a href="https://github.com/dashscope/dashscope/blob/master/README_zh.md">中文</a>
+        <b>English</b>
     <p>
 </h4>
 
 
 </div>
 
 # DashScope Python Library
@@ -24,89 +23,79 @@
 
 
 ## QuickStart
 
 You can use `Conversation` api to directly chat with model qwen-v1(通义千问).
 
 ```python
+from http import HTTPStatus
 import dashscope
 from dashscope import Conversation
 
-dashscope.api_key = '12344343222194ADSSDSSDSDSB9A511ED830AFA4166304A26'
-
-def stream_print(responses):
-    for r in responses:
-        if r.status_code == 200:
-            print(r.output.text.replace('\n', '  '), end='\r')
-            print(r.usage)
-        else:
-            print(r.message)
-
-chat = Conversation()
-
-responses = chat.call('qwen-v1',
-    prompt='以松柏为题，写一首七言诗。',
-    stream=True)
-stream_print(responses)
-
-responses = chat.call('qwen-v1',
-    prompt='现在假设你是一名精通中英双语的学者，将上面这首诗翻译成英文。',
-    stream=True)
-stream_print(responses)
+dashscope.api_key = 'YOUR-DASHSCOPE-API-KEY'
+responses = Generation.call(model=Generation.Models.qwen_v1,
+                            prompt='今天天气好吗？')
+
+if responses.status_code == HTTPStatus.OK:
+    print('Result is: %s' % responses.output)
+else:
+    print('Failed request_id: %s, status_code: %s, code: %s, message:%s' %
+            (responses.request_id, responses.status_code, responses.code,
+            responses.message))
 
 ```
 
 ## API Key Authentication
 
-The SDK uses API key authentication. [Get your API key here](https://aliyuque.antfin.com/zztrg2/zl1nqe/qo56foez7a2hgwyk).
+The SDK uses API key for authentication. Please refer to [official documentation](https://dashscope.aliyun.com) regarding how to obtain your api-key.
 
 ### Using the API Key
 
 1. Set the API key via code
 ```python
 import dashscope
 
-dashscope.api_key = 'your-api-key'
+dashscope.api_key = 'YOUR-DASHSCOPE-API-KEY'
 # Or specify the API key file path via code
 # dashscope.api_key_file_path='~/.dashscope/api_key'
 
 ```
 
 2. Set the API key via environment variables
 
 a. Set the API key directly using the environment variable below
 
 ```python
-export DASHSCOPE_API_KEY='your_api_key'
+export DASHSCOPE_API_KEY='YOUR-DASHSCOPE-API-KEY'
 ```
 
 b. Specify the API key file path via an environment variable
 
 ```python
 export DASHSCOPE_API_KEY_FILE_PATH='~/.dashscope/api_key'
 ```
 
 3. Save the API key to a file
 ```python
 from dashscope import save_api_key
 
-save_api_key(api_key='your_api_key',
+save_api_key(api_key='YOUR-DASHSCOPE-API-KEY',
              api_key_file_path='api_key_file_location or (None, will save to default location "~/.dashscope/api_key"')
 
 ```
 
 
 ## Sample Code
 
-`call` function provides  synchronous call, the function call will return when the whole computing process finish on the server side.
+`call` function provides  synchronous call, the function call will return when computation is done on the server side.
 
 ```python
 from http import HTTPStatus
 from dashscope import Generation
-# export DASHSCOPE_API_KEY='your_api_key' in environment
+# export DASHSCOPE_API_KEY='YOUR-DASHSCOPE-API-KEY' in environment
 def sync_dashscope_sample():
     responses = Generation.call(
         model=Generation.Models.qwen_v1,
         prompt='Is the weather good today?')
 
     if responses.status_code == HTTPStatus.OK:
         print('Result is: %s'%responses.output)
@@ -220,18 +209,12 @@
 ```
 
 ## Error Handling
 Currently, errors are thrown as exceptions.
 
 
 ## Contributing
-We welcome contributions to the DashScope Python SDK! To contribute, please follow these steps:
+Coming soon.
 
-Fork the repository on GitHub.
-Create a new branch for your changes.
-Implement your changes and add tests.
-Make sure all tests pass by running pytest.
-Submit a pull request to the main branch.
-For more information on contributing, please read our contributing guidelines.
 
 ## License
-This project is licensed under the [Apache License (Version 2.0)](https://github.com/dashscope/dashscope/blob/master/LICENSE).
+This project is licensed under the Apache License (Version 2.0).
```

### Comparing `dashscope-1.0.0/dashscope/__init__.py` & `dashscope-1.0.1/dashscope/__init__.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/dashscope/aigc/conversation.py` & `dashscope-1.0.1/dashscope/aigc/conversation.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/dashscope/aigc/generation.py` & `dashscope-1.0.1/dashscope/aigc/generation.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/dashscope/api_entities/aiohttp_request.py` & `dashscope-1.0.1/dashscope/api_entities/aiohttp_request.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/dashscope/api_entities/api_request_data.py` & `dashscope-1.0.1/dashscope/api_entities/api_request_data.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/dashscope/api_entities/api_request_factory.py` & `dashscope-1.0.1/dashscope/api_entities/api_request_factory.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/dashscope/api_entities/base_request.py` & `dashscope-1.0.1/dashscope/api_entities/base_request.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/dashscope/api_entities/dashscope_response.py` & `dashscope-1.0.1/dashscope/api_entities/dashscope_response.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/dashscope/api_entities/http_request.py` & `dashscope-1.0.1/dashscope/api_entities/http_request.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/dashscope/api_entities/websocket_request.py` & `dashscope-1.0.1/dashscope/api_entities/websocket_request.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/dashscope/audio/asr/transcription.py` & `dashscope-1.0.1/dashscope/audio/asr/transcription.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/dashscope/cli.py` & `dashscope-1.0.1/dashscope/cli.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/dashscope/client/base_api.py` & `dashscope-1.0.1/dashscope/client/base_api.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/dashscope/common/api_key.py` & `dashscope-1.0.1/dashscope/common/api_key.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/dashscope/common/constants.py` & `dashscope-1.0.1/dashscope/common/constants.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/dashscope/common/env.py` & `dashscope-1.0.1/dashscope/common/env.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/dashscope/common/error.py` & `dashscope-1.0.1/dashscope/common/error.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/dashscope/common/logging.py` & `dashscope-1.0.1/dashscope/common/logging.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/dashscope/common/utils.py` & `dashscope-1.0.1/dashscope/common/utils.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/dashscope/deployment.py` & `dashscope-1.0.1/dashscope/deployment.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/dashscope/file.py` & `dashscope-1.0.1/dashscope/file.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/dashscope/finetune.py` & `dashscope-1.0.1/dashscope/finetune.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/dashscope/io/input_output.py` & `dashscope-1.0.1/dashscope/io/input_output.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/dashscope/model.py` & `dashscope-1.0.1/dashscope/model.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/dashscope/protocol/websocket.py` & `dashscope-1.0.1/dashscope/protocol/websocket.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/dashscope.egg-info/PKG-INFO` & `dashscope-1.0.1/dashscope.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dashscope
-Version: 1.0.0
+Version: 1.0.1
 Summary: dashscope client sdk library
 Home-page: https://dashscope.aliyun.com/
 Author: Alibaba
 Author-email: dashscope@alibaba-inc.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -19,16 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h4 align="center">
     <p>
-        <b>English</b> |
-        <a href="https://github.com/dashscope/dashscope/blob/master/README_zh.md">中文</a>
+        <b>English</b>
     <p>
 </h4>
 
 
 </div>
 
 # DashScope Python Library
@@ -47,89 +46,79 @@
 
 
 ## QuickStart
 
 You can use `Conversation` api to directly chat with model qwen-v1(通义千问).
 
 ```python
+from http import HTTPStatus
 import dashscope
 from dashscope import Conversation
 
-dashscope.api_key = '12344343222194ADSSDSSDSDSB9A511ED830AFA4166304A26'
-
-def stream_print(responses):
-    for r in responses:
-        if r.status_code == 200:
-            print(r.output.text.replace('\n', '  '), end='\r')
-            print(r.usage)
-        else:
-            print(r.message)
-
-chat = Conversation()
-
-responses = chat.call('qwen-v1',
-    prompt='以松柏为题，写一首七言诗。',
-    stream=True)
-stream_print(responses)
-
-responses = chat.call('qwen-v1',
-    prompt='现在假设你是一名精通中英双语的学者，将上面这首诗翻译成英文。',
-    stream=True)
-stream_print(responses)
+dashscope.api_key = 'YOUR-DASHSCOPE-API-KEY'
+responses = Generation.call(model=Generation.Models.qwen_v1,
+                            prompt='今天天气好吗？')
+
+if responses.status_code == HTTPStatus.OK:
+    print('Result is: %s' % responses.output)
+else:
+    print('Failed request_id: %s, status_code: %s, code: %s, message:%s' %
+            (responses.request_id, responses.status_code, responses.code,
+            responses.message))
 
 ```
 
 ## API Key Authentication
 
-The SDK uses API key authentication. [Get your API key here](https://aliyuque.antfin.com/zztrg2/zl1nqe/qo56foez7a2hgwyk).
+The SDK uses API key for authentication. Please refer to [official documentation](https://dashscope.aliyun.com) regarding how to obtain your api-key.
 
 ### Using the API Key
 
 1. Set the API key via code
 ```python
 import dashscope
 
-dashscope.api_key = 'your-api-key'
+dashscope.api_key = 'YOUR-DASHSCOPE-API-KEY'
 # Or specify the API key file path via code
 # dashscope.api_key_file_path='~/.dashscope/api_key'
 
 ```
 
 2. Set the API key via environment variables
 
 a. Set the API key directly using the environment variable below
 
 ```python
-export DASHSCOPE_API_KEY='your_api_key'
+export DASHSCOPE_API_KEY='YOUR-DASHSCOPE-API-KEY'
 ```
 
 b. Specify the API key file path via an environment variable
 
 ```python
 export DASHSCOPE_API_KEY_FILE_PATH='~/.dashscope/api_key'
 ```
 
 3. Save the API key to a file
 ```python
 from dashscope import save_api_key
 
-save_api_key(api_key='your_api_key',
+save_api_key(api_key='YOUR-DASHSCOPE-API-KEY',
              api_key_file_path='api_key_file_location or (None, will save to default location "~/.dashscope/api_key"')
 
 ```
 
 
 ## Sample Code
 
-`call` function provides  synchronous call, the function call will return when the whole computing process finish on the server side.
+`call` function provides  synchronous call, the function call will return when computation is done on the server side.
 
 ```python
 from http import HTTPStatus
 from dashscope import Generation
-# export DASHSCOPE_API_KEY='your_api_key' in environment
+# export DASHSCOPE_API_KEY='YOUR-DASHSCOPE-API-KEY' in environment
 def sync_dashscope_sample():
     responses = Generation.call(
         model=Generation.Models.qwen_v1,
         prompt='Is the weather good today?')
 
     if responses.status_code == HTTPStatus.OK:
         print('Result is: %s'%responses.output)
@@ -243,18 +232,12 @@
 ```
 
 ## Error Handling
 Currently, errors are thrown as exceptions.
 
 
 ## Contributing
-We welcome contributions to the DashScope Python SDK! To contribute, please follow these steps:
+Coming soon.
 
-Fork the repository on GitHub.
-Create a new branch for your changes.
-Implement your changes and add tests.
-Make sure all tests pass by running pytest.
-Submit a pull request to the main branch.
-For more information on contributing, please read our contributing guidelines.
 
 ## License
-This project is licensed under the [Apache License (Version 2.0)](https://github.com/dashscope/dashscope/blob/master/LICENSE).
+This project is licensed under the Apache License (Version 2.0).
```

### Comparing `dashscope-1.0.0/dashscope.egg-info/SOURCES.txt` & `dashscope-1.0.1/dashscope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.0/setup.py` & `dashscope-1.0.1/setup.py`

 * *Files identical despite different names*

