# Comparing `tmp/dashscope-1.0.1.tar.gz` & `tmp/dashscope-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dashscope-1.0.1.tar", last modified: Mon Apr 10 10:57:48 2023, max compression
+gzip compressed data, was "dist/dashscope-1.0.2.tar", last modified: Mon Apr 10 11:41:53 2023, max compression
```

## Comparing `dashscope-1.0.1.tar` & `dashscope-1.0.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 10:57:48.000000 dashscope-1.0.1/
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)    11413 2023-04-10 08:39:29.000000 dashscope-1.0.1/LICENSE
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     7512 2023-04-10 10:57:48.000000 dashscope-1.0.1/PKG-INFO
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     6689 2023-04-10 10:57:41.000000 dashscope-1.0.1/README.md
-drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope/
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)      835 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/__init__.py
-drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope/aigc/
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)       66 2023-03-31 05:34:25.000000 dashscope-1.0.1/dashscope/aigc/__init__.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     8217 2023-04-10 08:37:22.000000 dashscope-1.0.1/dashscope/aigc/conversation.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     3779 2023-04-10 08:37:22.000000 dashscope-1.0.1/dashscope/aigc/generation.py
-drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope/api_entities/
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)        0 2023-03-31 05:34:25.000000 dashscope-1.0.1/dashscope/api_entities/__init__.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)    10361 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/api_entities/aiohttp_request.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     5310 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/api_entities/api_request_data.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     4057 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/api_entities/api_request_factory.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)      608 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/api_entities/base_request.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     5712 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/api_entities/dashscope_response.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     9401 2023-04-10 08:37:22.000000 dashscope-1.0.1/dashscope/api_entities/http_request.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)    15625 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/api_entities/websocket_request.py
-drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope/audio/
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)       35 2023-03-31 05:34:25.000000 dashscope-1.0.1/dashscope/audio/__init__.py
-drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope/audio/asr/
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)       75 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/audio/asr/__init__.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     5103 2023-04-10 08:37:22.000000 dashscope-1.0.1/dashscope/audio/asr/transcription.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)    13361 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/cli.py
-drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope/client/
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)        0 2023-03-31 05:34:25.000000 dashscope-1.0.1/dashscope/client/__init__.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)    21665 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/client/base_api.py
-drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope/common/
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)        0 2023-03-31 05:34:25.000000 dashscope-1.0.1/dashscope/common/__init__.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     1986 2023-03-31 05:34:25.000000 dashscope-1.0.1/dashscope/common/api_key.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     1940 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/common/constants.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)      907 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/common/env.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     1592 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/common/error.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)      984 2023-03-31 05:34:25.000000 dashscope-1.0.1/dashscope/common/logging.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     3330 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/common/utils.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     3445 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/deployment.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     3753 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/file.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     4808 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/finetune.py
-drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope/io/
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)        0 2023-03-31 05:34:25.000000 dashscope-1.0.1/dashscope/io/__init__.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     2781 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/io/input_output.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     1696 2023-04-06 08:30:57.000000 dashscope-1.0.1/dashscope/model.py
-drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope/protocol/
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)        0 2023-03-31 05:34:25.000000 dashscope-1.0.1/dashscope/protocol/__init__.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)      561 2023-03-31 05:34:25.000000 dashscope-1.0.1/dashscope/protocol/websocket.py
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)       22 2023-04-10 10:57:41.000000 dashscope-1.0.1/dashscope/version.py
-drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope.egg-info/
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     7512 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope.egg-info/PKG-INFO
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     1294 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope.egg-info/SOURCES.txt
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)        1 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope.egg-info/dependency_links.txt
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)       49 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope.egg-info/entry_points.txt
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)        1 2023-03-31 05:53:35.000000 dashscope-1.0.1/dashscope.egg-info/not-zip-safe
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)       17 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope.egg-info/requires.txt
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)       10 2023-04-10 10:57:48.000000 dashscope-1.0.1/dashscope.egg-info/top_level.txt
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)       53 2023-04-10 10:57:48.000000 dashscope-1.0.1/setup.cfg
--rw-r--r--   0 wenmeng.zwm (122285) users      (100)     2201 2023-04-10 09:13:51.000000 dashscope-1.0.1/setup.py
+drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 11:41:53.000000 dashscope-1.0.2/
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)    11413 2023-04-10 08:39:29.000000 dashscope-1.0.2/LICENSE
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     7494 2023-04-10 11:41:53.000000 dashscope-1.0.2/PKG-INFO
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     6671 2023-04-10 11:41:19.000000 dashscope-1.0.2/README.md
+drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 11:41:53.000000 dashscope-1.0.2/dashscope/
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)      835 2023-04-06 08:30:57.000000 dashscope-1.0.2/dashscope/__init__.py
+drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 11:41:53.000000 dashscope-1.0.2/dashscope/aigc/
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)       66 2023-03-31 05:34:25.000000 dashscope-1.0.2/dashscope/aigc/__init__.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     8217 2023-04-10 08:37:22.000000 dashscope-1.0.2/dashscope/aigc/conversation.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     3779 2023-04-10 08:37:22.000000 dashscope-1.0.2/dashscope/aigc/generation.py
+drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 11:41:53.000000 dashscope-1.0.2/dashscope/api_entities/
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)        0 2023-03-31 05:34:25.000000 dashscope-1.0.2/dashscope/api_entities/__init__.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)    10361 2023-04-06 08:30:57.000000 dashscope-1.0.2/dashscope/api_entities/aiohttp_request.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     5310 2023-04-06 08:30:57.000000 dashscope-1.0.2/dashscope/api_entities/api_request_data.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     4057 2023-04-06 08:30:57.000000 dashscope-1.0.2/dashscope/api_entities/api_request_factory.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)      608 2023-04-06 08:30:57.000000 dashscope-1.0.2/dashscope/api_entities/base_request.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     5712 2023-04-06 08:30:57.000000 dashscope-1.0.2/dashscope/api_entities/dashscope_response.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     9401 2023-04-10 08:37:22.000000 dashscope-1.0.2/dashscope/api_entities/http_request.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)    15625 2023-04-06 08:30:57.000000 dashscope-1.0.2/dashscope/api_entities/websocket_request.py
+drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 11:41:53.000000 dashscope-1.0.2/dashscope/audio/
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)       35 2023-03-31 05:34:25.000000 dashscope-1.0.2/dashscope/audio/__init__.py
+drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 11:41:53.000000 dashscope-1.0.2/dashscope/audio/asr/
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)       75 2023-04-06 08:30:57.000000 dashscope-1.0.2/dashscope/audio/asr/__init__.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     5103 2023-04-10 08:37:22.000000 dashscope-1.0.2/dashscope/audio/asr/transcription.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)    13361 2023-04-06 08:30:57.000000 dashscope-1.0.2/dashscope/cli.py
+drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 11:41:53.000000 dashscope-1.0.2/dashscope/client/
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)        0 2023-03-31 05:34:25.000000 dashscope-1.0.2/dashscope/client/__init__.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)    21665 2023-04-06 08:30:57.000000 dashscope-1.0.2/dashscope/client/base_api.py
+drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 11:41:53.000000 dashscope-1.0.2/dashscope/common/
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)        0 2023-03-31 05:34:25.000000 dashscope-1.0.2/dashscope/common/__init__.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     1986 2023-03-31 05:34:25.000000 dashscope-1.0.2/dashscope/common/api_key.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     1940 2023-04-06 08:30:57.000000 dashscope-1.0.2/dashscope/common/constants.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)      907 2023-04-06 08:30:57.000000 dashscope-1.0.2/dashscope/common/env.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     1592 2023-04-06 08:30:57.000000 dashscope-1.0.2/dashscope/common/error.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)      984 2023-03-31 05:34:25.000000 dashscope-1.0.2/dashscope/common/logging.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     3330 2023-04-06 08:30:57.000000 dashscope-1.0.2/dashscope/common/utils.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     3445 2023-04-06 08:30:57.000000 dashscope-1.0.2/dashscope/deployment.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     3753 2023-04-06 08:30:57.000000 dashscope-1.0.2/dashscope/file.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     4808 2023-04-06 08:30:57.000000 dashscope-1.0.2/dashscope/finetune.py
+drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 11:41:53.000000 dashscope-1.0.2/dashscope/io/
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)        0 2023-03-31 05:34:25.000000 dashscope-1.0.2/dashscope/io/__init__.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     2781 2023-04-06 08:30:57.000000 dashscope-1.0.2/dashscope/io/input_output.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     1696 2023-04-06 08:30:57.000000 dashscope-1.0.2/dashscope/model.py
+drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 11:41:53.000000 dashscope-1.0.2/dashscope/protocol/
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)        0 2023-03-31 05:34:25.000000 dashscope-1.0.2/dashscope/protocol/__init__.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)      561 2023-03-31 05:34:25.000000 dashscope-1.0.2/dashscope/protocol/websocket.py
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)       22 2023-04-10 11:41:19.000000 dashscope-1.0.2/dashscope/version.py
+drwxr-xr-x   0 wenmeng.zwm (122285) users      (100)        0 2023-04-10 11:41:53.000000 dashscope-1.0.2/dashscope.egg-info/
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     7494 2023-04-10 11:41:53.000000 dashscope-1.0.2/dashscope.egg-info/PKG-INFO
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     1294 2023-04-10 11:41:53.000000 dashscope-1.0.2/dashscope.egg-info/SOURCES.txt
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)        1 2023-04-10 11:41:53.000000 dashscope-1.0.2/dashscope.egg-info/dependency_links.txt
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)       49 2023-04-10 11:41:53.000000 dashscope-1.0.2/dashscope.egg-info/entry_points.txt
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)        1 2023-03-31 05:53:35.000000 dashscope-1.0.2/dashscope.egg-info/not-zip-safe
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)       17 2023-04-10 11:41:53.000000 dashscope-1.0.2/dashscope.egg-info/requires.txt
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)       10 2023-04-10 11:41:53.000000 dashscope-1.0.2/dashscope.egg-info/top_level.txt
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)       53 2023-04-10 11:41:53.000000 dashscope-1.0.2/setup.cfg
+-rw-r--r--   0 wenmeng.zwm (122285) users      (100)     2201 2023-04-10 09:13:51.000000 dashscope-1.0.2/setup.py
```

### Comparing `dashscope-1.0.1/LICENSE` & `dashscope-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/PKG-INFO` & `dashscope-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dashscope
-Version: 1.0.1
+Version: 1.0.2
 Summary: dashscope client sdk library
 Home-page: https://dashscope.aliyun.com/
 Author: Alibaba
 Author-email: dashscope@alibaba-inc.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -43,20 +43,20 @@
 pip install -e .
 ```
 
 
 
 ## QuickStart
 
-You can use `Conversation` api to directly chat with model qwen-v1(通义千问).
+You can use `Generation` api to call model qwen-v1(通义千问).
 
 ```python
 from http import HTTPStatus
 import dashscope
-from dashscope import Conversation
+from dashscope import Generation
 
 dashscope.api_key = 'YOUR-DASHSCOPE-API-KEY'
 responses = Generation.call(model=Generation.Models.qwen_v1,
                             prompt='今天天气好吗？')
 
 if responses.status_code == HTTPStatus.OK:
     print('Result is: %s' % responses.output)
```

### Comparing `dashscope-1.0.1/README.md` & `dashscope-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,20 @@
 pip install -e .
 ```
 
 
 
 ## QuickStart
 
-You can use `Conversation` api to directly chat with model qwen-v1(通义千问).
+You can use `Generation` api to call model qwen-v1(通义千问).
 
 ```python
 from http import HTTPStatus
 import dashscope
-from dashscope import Conversation
+from dashscope import Generation
 
 dashscope.api_key = 'YOUR-DASHSCOPE-API-KEY'
 responses = Generation.call(model=Generation.Models.qwen_v1,
                             prompt='今天天气好吗？')
 
 if responses.status_code == HTTPStatus.OK:
     print('Result is: %s' % responses.output)
```

### Comparing `dashscope-1.0.1/dashscope/__init__.py` & `dashscope-1.0.2/dashscope/__init__.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/dashscope/aigc/conversation.py` & `dashscope-1.0.2/dashscope/aigc/conversation.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/dashscope/aigc/generation.py` & `dashscope-1.0.2/dashscope/aigc/generation.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/dashscope/api_entities/aiohttp_request.py` & `dashscope-1.0.2/dashscope/api_entities/aiohttp_request.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/dashscope/api_entities/api_request_data.py` & `dashscope-1.0.2/dashscope/api_entities/api_request_data.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/dashscope/api_entities/api_request_factory.py` & `dashscope-1.0.2/dashscope/api_entities/api_request_factory.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/dashscope/api_entities/base_request.py` & `dashscope-1.0.2/dashscope/api_entities/base_request.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/dashscope/api_entities/dashscope_response.py` & `dashscope-1.0.2/dashscope/api_entities/dashscope_response.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/dashscope/api_entities/http_request.py` & `dashscope-1.0.2/dashscope/api_entities/http_request.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/dashscope/api_entities/websocket_request.py` & `dashscope-1.0.2/dashscope/api_entities/websocket_request.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/dashscope/audio/asr/transcription.py` & `dashscope-1.0.2/dashscope/audio/asr/transcription.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/dashscope/cli.py` & `dashscope-1.0.2/dashscope/cli.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/dashscope/client/base_api.py` & `dashscope-1.0.2/dashscope/client/base_api.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/dashscope/common/api_key.py` & `dashscope-1.0.2/dashscope/common/api_key.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/dashscope/common/constants.py` & `dashscope-1.0.2/dashscope/common/constants.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/dashscope/common/env.py` & `dashscope-1.0.2/dashscope/common/env.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/dashscope/common/error.py` & `dashscope-1.0.2/dashscope/common/error.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/dashscope/common/logging.py` & `dashscope-1.0.2/dashscope/common/logging.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/dashscope/common/utils.py` & `dashscope-1.0.2/dashscope/common/utils.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/dashscope/deployment.py` & `dashscope-1.0.2/dashscope/deployment.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/dashscope/file.py` & `dashscope-1.0.2/dashscope/file.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/dashscope/finetune.py` & `dashscope-1.0.2/dashscope/finetune.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/dashscope/io/input_output.py` & `dashscope-1.0.2/dashscope/io/input_output.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/dashscope/model.py` & `dashscope-1.0.2/dashscope/model.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/dashscope/protocol/websocket.py` & `dashscope-1.0.2/dashscope/protocol/websocket.py`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/dashscope.egg-info/PKG-INFO` & `dashscope-1.0.2/dashscope.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dashscope
-Version: 1.0.1
+Version: 1.0.2
 Summary: dashscope client sdk library
 Home-page: https://dashscope.aliyun.com/
 Author: Alibaba
 Author-email: dashscope@alibaba-inc.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -43,20 +43,20 @@
 pip install -e .
 ```
 
 
 
 ## QuickStart
 
-You can use `Conversation` api to directly chat with model qwen-v1(通义千问).
+You can use `Generation` api to call model qwen-v1(通义千问).
 
 ```python
 from http import HTTPStatus
 import dashscope
-from dashscope import Conversation
+from dashscope import Generation
 
 dashscope.api_key = 'YOUR-DASHSCOPE-API-KEY'
 responses = Generation.call(model=Generation.Models.qwen_v1,
                             prompt='今天天气好吗？')
 
 if responses.status_code == HTTPStatus.OK:
     print('Result is: %s' % responses.output)
```

### Comparing `dashscope-1.0.1/dashscope.egg-info/SOURCES.txt` & `dashscope-1.0.2/dashscope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dashscope-1.0.1/setup.py` & `dashscope-1.0.2/setup.py`

 * *Files identical despite different names*

