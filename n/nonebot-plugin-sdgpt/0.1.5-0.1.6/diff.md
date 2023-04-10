# Comparing `tmp/nonebot-plugin-SDGPT-0.1.5.tar.gz` & `tmp/nonebot_plugin_sdgpt-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-SDGPT-0.1.5.tar", last modified: Mon Apr 10 17:14:05 2023, max compression
+gzip compressed data, was "nonebot_plugin_sdgpt-0.1.6.tar", max compression
```

## Comparing `nonebot-plugin-SDGPT-0.1.5.tar` & `nonebot_plugin_sdgpt-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,6 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 17:14:05.347478 nonebot-plugin-SDGPT-0.1.5/
--rw-rw-rw-   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot-plugin-SDGPT-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      210 2023-04-10 17:14:05.347478 nonebot-plugin-SDGPT-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1034 2023-04-09 01:25:35.000000 nonebot-plugin-SDGPT-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 17:14:05.336736 nonebot-plugin-SDGPT-0.1.5/nonebot_plugin_SDGPT/
--rw-rw-rw-   0        0        0     3339 2023-04-10 14:07:48.000000 nonebot-plugin-SDGPT-0.1.5/nonebot_plugin_SDGPT/__init__.py
--rw-rw-rw-   0        0        0     9918 2023-04-10 17:13:14.000000 nonebot-plugin-SDGPT-0.1.5/nonebot_plugin_SDGPT/bot.py
-drwxrwxrwx   0        0        0        0 2023-04-10 17:14:05.345525 nonebot-plugin-SDGPT-0.1.5/nonebot_plugin_SDGPT.egg-info/
--rw-rw-rw-   0        0        0      210 2023-04-10 17:14:05.000000 nonebot-plugin-SDGPT-0.1.5/nonebot_plugin_SDGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-04-10 17:14:05.000000 nonebot-plugin-SDGPT-0.1.5/nonebot_plugin_SDGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 17:14:05.000000 nonebot-plugin-SDGPT-0.1.5/nonebot_plugin_SDGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      101 2023-04-10 17:14:05.000000 nonebot-plugin-SDGPT-0.1.5/nonebot_plugin_SDGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-10 17:14:05.000000 nonebot-plugin-SDGPT-0.1.5/nonebot_plugin_SDGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 17:14:05.347478 nonebot-plugin-SDGPT-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      663 2023-04-10 17:12:20.000000 nonebot-plugin-SDGPT-0.1.5/setup.py
+-rw-r--r--   0        0        0     3339 2023-04-10 14:07:48.620257 nonebot_plugin_sdgpt-0.1.6/__init__.py
+-rw-r--r--   0        0        0     9983 2023-04-10 17:22:24.976760 nonebot_plugin_sdgpt-0.1.6/bot.py
+-rw-r--r--   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot_plugin_sdgpt-0.1.6/LICENSE
+-rw-r--r--   0        0        0      983 2023-04-10 17:40:24.012798 nonebot_plugin_sdgpt-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1034 2023-04-09 01:25:35.547383 nonebot_plugin_sdgpt-0.1.6/README.md
+-rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 nonebot_plugin_sdgpt-0.1.6/PKG-INFO
```

### Comparing `nonebot-plugin-SDGPT-0.1.5/LICENSE` & `nonebot_plugin_sdgpt-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-SDGPT-0.1.5/README.md` & `nonebot_plugin_sdgpt-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-SDGPT-0.1.5/nonebot_plugin_SDGPT/__init__.py` & `nonebot_plugin_sdgpt-0.1.6/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-SDGPT-0.1.5/nonebot_plugin_SDGPT/bot.py` & `nonebot_plugin_sdgpt-0.1.6/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from nonebot.log import logger_id
 from nonebot.log import  default_filter
 from nonebot import logger
 import webuiapi
 from revChatGPT.V1 import Chatbot as chatGPT
 from revChatGPT.V3 import Chatbot as chatGPT_api
 from EdgeGPT import Chatbot as bing
+import ast
 logger.remove(logger_id)
 
 def formatter(record):
     record['message']
     level = record['level'].name
     add = ''
     Dir = {
@@ -69,15 +70,15 @@
 }
 
 
 
 async def Chat(func,message:str,mode=1): 
     if not message or len(message)<1:return
     Rtime = int(cfg['Chat_stream_waitTime'])
-    endStr = cfg['Chat_stream_endStr']
+    endStr = ast.literal_eval(cfg['Chat_stream_endStr'])
     text = ''
     out_text=''
     info('ChatGPT','开始询问 (网页)')
     for data in chatbot.ask(message):
         text = data["message"] # type: ignore
         try: not now # type: ignore
         except: now = time.time()
@@ -94,15 +95,15 @@
         outText = text.replace(out_text,'')
         success('ChatGPT', outText)
         await func.send(outText)
     
 async def Chat_api(func,message:str,mode=1):
     if not message or len(message)<1:return
     Rtime = cfg['Chat_stream_waitTime']
-    endStr = cfg['Chat_stream_endStr']
+    endStr = ast.literal_eval(cfg['Chat_stream_endStr'])
     text = ''
     info('ChatGPT api','开始询问 api')
     for data in chatbot_api.ask_stream(message):
         text += data 
         try: not now # type: ignore
         except: now = time.time()
         if time.time() - now > Rtime and text.endswith(endStr) and mode == 1: # type: ignore
@@ -117,15 +118,15 @@
         success('ChatGPT api', text)
         await func.send(text)
 
 
 async def Bing(func,message,mode=1):
     if not message or len(message)<1:return
     Rtime = int(cfg['Chat_stream_waitTime'])
-    endStr = cfg['Chat_stream_endStr']
+    endStr = ast.literal_eval(cfg['Chat_stream_endStr'])
     text = ''
     out_text=''
     info('Bing','开始询问 api')
     async for data in bingbot.ask_stream(message):
         istrue , string = data
         if type(string) == str : text = string
         try: not now # type: ignore
```

