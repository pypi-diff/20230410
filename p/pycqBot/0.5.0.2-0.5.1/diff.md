# Comparing `tmp/pycqBot-0.5.0.2.tar.gz` & `tmp/pycqBot-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycqBot-0.5.0.2.tar", last modified: Tue Apr  4 11:00:23 2023, max compression
+gzip compressed data, was "pycqBot-0.5.1.tar", last modified: Sun Apr  9 17:49:13 2023, max compression
```

## Comparing `pycqBot-0.5.0.2.tar` & `pycqBot-0.5.1.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-04 11:00:23.069880 pycqBot-0.5.0.2/
--rw-r--r--   0 sakura    (1000) sakura    (1000)     2281 2023-04-04 11:00:23.069880 pycqBot-0.5.0.2/PKG-INFO
--rwxrwx---   0 sakura    (1000) sakura    (1000)     1449 2023-04-02 16:40:54.000000 pycqBot-0.5.0.2/README.md
-drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-04 11:00:23.065880 pycqBot-0.5.0.2/pycqBot/
--rwxrwx---   0 sakura    (1000) sakura    (1000)     2491 2023-04-04 10:44:37.000000 pycqBot-0.5.0.2/pycqBot/__init__.py
--rwxrwx---   0 sakura    (1000) sakura    (1000)     5640 2023-04-03 14:18:37.000000 pycqBot-0.5.0.2/pycqBot/asyncHttp.py
--rwxrwx---   0 sakura    (1000) sakura    (1000)    46204 2023-04-04 10:35:06.000000 pycqBot-0.5.0.2/pycqBot/cqApi.py
--rwxrwx---   0 sakura    (1000) sakura    (1000)     8414 2023-04-04 07:48:10.000000 pycqBot-0.5.0.2/pycqBot/cqCode.py
-drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-04 11:00:23.069880 pycqBot-0.5.0.2/pycqBot/data/
--rwxrwx---   0 sakura    (1000) sakura    (1000)      226 2023-04-03 10:50:19.000000 pycqBot-0.5.0.2/pycqBot/data/__init__.py
--rwxrwx---   0 sakura    (1000) sakura    (1000)     4123 2023-04-04 09:04:01.000000 pycqBot-0.5.0.2/pycqBot/data/event.py
--rwxrwx---   0 sakura    (1000) sakura    (1000)     4228 2023-04-04 07:44:06.000000 pycqBot-0.5.0.2/pycqBot/data/message.py
--rwxrwx---   0 sakura    (1000) sakura    (1000)     4502 2023-04-04 10:57:32.000000 pycqBot-0.5.0.2/pycqBot/data/user.py
--rwxrwx---   0 sakura    (1000) sakura    (1000)     8721 2023-04-04 07:30:50.000000 pycqBot-0.5.0.2/pycqBot/object.py
-drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-04 11:00:23.069880 pycqBot-0.5.0.2/pycqBot/plugin/
--rwxrwx---   0 sakura    (1000) sakura    (1000)        0 2023-04-02 16:34:46.000000 pycqBot-0.5.0.2/pycqBot/plugin/__init__.py
-drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-04 11:00:23.069880 pycqBot-0.5.0.2/pycqBot/plugin/bilibili/
--rwxrwx---   0 sakura    (1000) sakura    (1000)        0 2023-04-02 16:34:46.000000 pycqBot-0.5.0.2/pycqBot/plugin/bilibili/__init__.py
--rwxrwx---   0 sakura    (1000) sakura    (1000)    23483 2023-04-02 16:34:46.000000 pycqBot-0.5.0.2/pycqBot/plugin/bilibili/bilibili.py
-drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-04 11:00:23.069880 pycqBot-0.5.0.2/pycqBot/plugin/manage/
--rwxrwx---   0 sakura    (1000) sakura    (1000)        0 2023-04-02 16:34:46.000000 pycqBot-0.5.0.2/pycqBot/plugin/manage/__init__.py
--rwxrwx---   0 sakura    (1000) sakura    (1000)     4814 2023-04-03 15:11:18.000000 pycqBot-0.5.0.2/pycqBot/plugin/manage/manage.py
-drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-04 11:00:23.069880 pycqBot-0.5.0.2/pycqBot/plugin/pixiv/
--rwxrwx---   0 sakura    (1000) sakura    (1000)        0 2023-04-02 16:34:46.000000 pycqBot-0.5.0.2/pycqBot/plugin/pixiv/__init__.py
--rwxrwx---   0 sakura    (1000) sakura    (1000)    15781 2023-04-03 15:06:01.000000 pycqBot-0.5.0.2/pycqBot/plugin/pixiv/pixiv.py
-drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-04 11:00:23.069880 pycqBot-0.5.0.2/pycqBot/plugin/test/
--rwxrwx---   0 sakura    (1000) sakura    (1000)        0 2023-04-02 16:34:46.000000 pycqBot-0.5.0.2/pycqBot/plugin/test/__init__.py
--rwxrwx---   0 sakura    (1000) sakura    (1000)      864 2023-04-02 16:34:46.000000 pycqBot-0.5.0.2/pycqBot/plugin/test/test.py
-drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-04 11:00:23.069880 pycqBot-0.5.0.2/pycqBot/plugin/twitter/
--rwxrwx---   0 sakura    (1000) sakura    (1000)        0 2023-04-02 16:34:46.000000 pycqBot-0.5.0.2/pycqBot/plugin/twitter/__init__.py
--rwxrwx---   0 sakura    (1000) sakura    (1000)     4599 2023-04-02 16:34:46.000000 pycqBot-0.5.0.2/pycqBot/plugin/twitter/twitter.py
-drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-04 11:00:23.065880 pycqBot-0.5.0.2/pycqBot.egg-info/
--rwxrwx---   0 sakura    (1000) sakura    (1000)     2281 2023-04-04 11:00:22.000000 pycqBot-0.5.0.2/pycqBot.egg-info/PKG-INFO
--rwxrwx---   0 sakura    (1000) sakura    (1000)      715 2023-04-04 11:00:22.000000 pycqBot-0.5.0.2/pycqBot.egg-info/SOURCES.txt
--rwxrwx---   0 sakura    (1000) sakura    (1000)        1 2023-04-04 11:00:22.000000 pycqBot-0.5.0.2/pycqBot.egg-info/dependency_links.txt
--rwxrwx---   0 sakura    (1000) sakura    (1000)       57 2023-04-04 11:00:22.000000 pycqBot-0.5.0.2/pycqBot.egg-info/requires.txt
--rwxrwx---   0 sakura    (1000) sakura    (1000)        8 2023-04-04 11:00:22.000000 pycqBot-0.5.0.2/pycqBot.egg-info/top_level.txt
--rw-r--r--   0 sakura    (1000) sakura    (1000)       38 2023-04-04 11:00:23.069880 pycqBot-0.5.0.2/setup.cfg
--rwxrwx---   0 sakura    (1000) sakura    (1000)     1014 2023-04-04 10:58:55.000000 pycqBot-0.5.0.2/setup.py
+drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-09 17:49:13.335149 pycqBot-0.5.1/
+-rw-r--r--   0 sakura    (1000) sakura    (1000)     2815 2023-04-09 17:49:13.335149 pycqBot-0.5.1/PKG-INFO
+-rwxrwx---   0 sakura    (1000) sakura    (1000)     1785 2023-04-09 10:34:02.000000 pycqBot-0.5.1/README.md
+drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-09 17:49:13.331149 pycqBot-0.5.1/pycqBot/
+-rwxrwx---   0 sakura    (1000) sakura    (1000)     2484 2023-04-09 17:49:10.000000 pycqBot-0.5.1/pycqBot/__init__.py
+-rwxrwx---   0 sakura    (1000) sakura    (1000)     6178 2023-04-08 10:20:54.000000 pycqBot-0.5.1/pycqBot/asyncHttp.py
+-rw-r--r--   0 sakura    (1000) sakura    (1000)    45946 2023-04-09 07:34:10.000000 pycqBot-0.5.1/pycqBot/cqApi.py
+-rwxrwx---   0 sakura    (1000) sakura    (1000)    17794 2023-04-09 17:47:46.000000 pycqBot-0.5.1/pycqBot/cqCode.py
+-rw-r--r--   0 sakura    (1000) sakura    (1000)    11984 2023-04-09 07:33:21.000000 pycqBot-0.5.1/pycqBot/cqEvent.py
+-rwxrwx---   0 sakura    (1000) sakura    (1000)    33223 2023-04-09 17:48:08.000000 pycqBot-0.5.1/pycqBot/cqHttpApi.py
+drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-09 17:49:13.335149 pycqBot-0.5.1/pycqBot/data/
+-rwxrwx---   0 sakura    (1000) sakura    (1000)      226 2023-04-03 10:50:19.000000 pycqBot-0.5.1/pycqBot/data/__init__.py
+-rwxrwx---   0 sakura    (1000) sakura    (1000)     4127 2023-04-08 09:09:33.000000 pycqBot-0.5.1/pycqBot/data/event.py
+-rwxrwx---   0 sakura    (1000) sakura    (1000)     4221 2023-04-09 08:49:03.000000 pycqBot-0.5.1/pycqBot/data/message.py
+-rwxrwx---   0 sakura    (1000) sakura    (1000)     4502 2023-04-04 10:57:32.000000 pycqBot-0.5.1/pycqBot/data/user.py
+-rwxrwx---   0 sakura    (1000) sakura    (1000)      378 2023-04-08 11:46:45.000000 pycqBot-0.5.1/pycqBot/object.py
+drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-09 17:49:13.335149 pycqBot-0.5.1/pycqBot/plugin/
+-rwxrwx---   0 sakura    (1000) sakura    (1000)        0 2023-04-02 16:34:46.000000 pycqBot-0.5.1/pycqBot/plugin/__init__.py
+drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-09 17:49:13.335149 pycqBot-0.5.1/pycqBot/plugin/bilibili/
+-rwxrwx---   0 sakura    (1000) sakura    (1000)        0 2023-04-02 16:34:46.000000 pycqBot-0.5.1/pycqBot/plugin/bilibili/__init__.py
+-rwxrwx---   0 sakura    (1000) sakura    (1000)    23487 2023-04-08 09:09:33.000000 pycqBot-0.5.1/pycqBot/plugin/bilibili/bilibili.py
+drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-09 17:49:13.335149 pycqBot-0.5.1/pycqBot/plugin/manage/
+-rwxrwx---   0 sakura    (1000) sakura    (1000)        0 2023-04-02 16:34:46.000000 pycqBot-0.5.1/pycqBot/plugin/manage/__init__.py
+-rwxrwx---   0 sakura    (1000) sakura    (1000)     4818 2023-04-08 09:09:33.000000 pycqBot-0.5.1/pycqBot/plugin/manage/manage.py
+drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-09 17:49:13.335149 pycqBot-0.5.1/pycqBot/plugin/pixiv/
+-rwxrwx---   0 sakura    (1000) sakura    (1000)        0 2023-04-02 16:34:46.000000 pycqBot-0.5.1/pycqBot/plugin/pixiv/__init__.py
+-rwxrwx---   0 sakura    (1000) sakura    (1000)    15785 2023-04-08 09:09:33.000000 pycqBot-0.5.1/pycqBot/plugin/pixiv/pixiv.py
+drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-09 17:49:13.335149 pycqBot-0.5.1/pycqBot/plugin/test/
+-rwxrwx---   0 sakura    (1000) sakura    (1000)        0 2023-04-02 16:34:46.000000 pycqBot-0.5.1/pycqBot/plugin/test/__init__.py
+-rwxrwx---   0 sakura    (1000) sakura    (1000)      868 2023-04-08 09:09:33.000000 pycqBot-0.5.1/pycqBot/plugin/test/test.py
+drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-09 17:49:13.335149 pycqBot-0.5.1/pycqBot/plugin/twitter/
+-rwxrwx---   0 sakura    (1000) sakura    (1000)        0 2023-04-02 16:34:46.000000 pycqBot-0.5.1/pycqBot/plugin/twitter/__init__.py
+-rwxrwx---   0 sakura    (1000) sakura    (1000)     4603 2023-04-08 09:09:33.000000 pycqBot-0.5.1/pycqBot/plugin/twitter/twitter.py
+drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-09 17:49:13.331149 pycqBot-0.5.1/pycqBot.egg-info/
+-rwxrwx---   0 sakura    (1000) sakura    (1000)     2815 2023-04-09 17:49:13.000000 pycqBot-0.5.1/pycqBot.egg-info/PKG-INFO
+-rwxrwx---   0 sakura    (1000) sakura    (1000)      755 2023-04-09 17:49:13.000000 pycqBot-0.5.1/pycqBot.egg-info/SOURCES.txt
+-rwxrwx---   0 sakura    (1000) sakura    (1000)        1 2023-04-09 17:49:13.000000 pycqBot-0.5.1/pycqBot.egg-info/dependency_links.txt
+-rwxrwx---   0 sakura    (1000) sakura    (1000)       57 2023-04-09 17:49:13.000000 pycqBot-0.5.1/pycqBot.egg-info/requires.txt
+-rwxrwx---   0 sakura    (1000) sakura    (1000)        8 2023-04-09 17:49:13.000000 pycqBot-0.5.1/pycqBot.egg-info/top_level.txt
+-rw-r--r--   0 sakura    (1000) sakura    (1000)       38 2023-04-09 17:49:13.335149 pycqBot-0.5.1/setup.cfg
+-rwxrwx---   0 sakura    (1000) sakura    (1000)     1012 2023-04-09 10:10:46.000000 pycqBot-0.5.1/setup.py
```

### Comparing `pycqBot-0.5.0.2/pycqBot/__init__.py` & `pycqBot-0.5.1/pycqBot/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from pycqBot.cqApi import cqBot, cqHttpApi, cqLog
-from pycqBot.object import Plugin, cqEvent
+from pycqBot.cqHttpApi import cqBot, cqHttpApi, cqLog
+from pycqBot.object import Plugin
 
 
-__VERSIONS__ = "v0.5.0.1"
+__VERSIONS__ = "v0.5.1"
 
 
 TIT = """
 #################################################################
 ██████╗ ██╗   ██╗ ██████╗ ██████╗ ██████╗  ██████╗ ████████╗
 ██╔══██╗╚██╗ ██╔╝██╔════╝██╔═══██╗██╔══██╗██╔═══██╗╚══██╔══╝
 ██████╔╝ ╚████╔╝ ██║     ██║   ██║██████╔╝██║   ██║   ██║
```

### Comparing `pycqBot-0.5.0.2/pycqBot/asyncHttp.py` & `pycqBot-0.5.1/pycqBot/asyncHttp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from typing import Coroutine, Optional
+from typing import Any, Coroutine, Optional
 import logging
 from threading import Thread
 import asyncio
 import aiohttp
 import aiofiles
 import os
 
+import requests
+
 class asyncHttp:
 
     def __init__(self, download_path: str="./download", chunk_size: int=1024) -> None:
         self._loop = asyncio.new_event_loop()
         self._session = aiohttp.ClientSession(loop=self._loop)
         self._download_path = download_path
         self.chunk_size = chunk_size
@@ -77,14 +79,29 @@
                         http_data = await req.text(encoding=encoding)
             
             return http_data
         except Exception as err:
             self.apiLinkRunError(err)
 
             return None
+        
+    def _link(self, api: str, data: dict[str, Any]={}) -> Optional[dict[Any, Any]]:
+        try:
+            with requests.post(f"{self.http}{api}", data=data) as req:
+                json =  req.json()
+                logging.debug("cqAPI 响应: %s" % json)
+                if json["retcode"] != 0:
+                    self.apiLinkError(json)
+                    
+                return json
+            
+        except Exception as err:
+            self.apiLinkRunError(err)
+        
+        return None
     
     def add_task(self, coroutine: Coroutine) -> None:
         """向内部事件循环添加任务"""
         asyncio.run_coroutine_threadsafe(coroutine, self._loop)
     
     def add(self, api: str, data: dict=None) -> None:
         """向内部事件循环添加 go-cqhttp Api 任务"""
```

### Comparing `pycqBot-0.5.0.2/pycqBot/data/event.py` & `pycqBot-0.5.1/pycqBot/data/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from abc import ABCMeta, abstractmethod
 from typing import Any, Union, TYPE_CHECKING
 import json
 
 from pycqBot.data.message import Group_Message, Private_Message
 
 if TYPE_CHECKING:
-    from pycqBot.cqApi import cqHttpApi
+    from pycqBot.cqHttpApi import cqHttpApi
 
 
 class Message:
 
     MESSAGE_POST_TYPE: str = "message"
     """消息事件类型"""
```

### Comparing `pycqBot-0.5.0.2/pycqBot/data/message.py` & `pycqBot-0.5.1/pycqBot/data/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         """
         匿名信息\n
 
             如果不是匿名消息则为 null
         """
 
     def reply(self, message: str, auto_escape: bool = False) -> None:
-        self._cqapi.send_group_msg(self.group_id, "%s%s" % (reply(msg_id=self.id), message), auto_escape)
+        self._cqapi.send_group_msg(self.group_id, "%s%s" % (reply(self.id), message), auto_escape)
 
     def reply_not_code(self, message: str, auto_escape: bool=False) -> None:
         self._cqapi.send_group_msg(self.group_id, message, auto_escape)
 
     def set_essence(self):
         """
         设置精华消息
```

### Comparing `pycqBot-0.5.0.2/pycqBot/data/user.py` & `pycqBot-0.5.1/pycqBot/data/user.py`

 * *Files identical despite different names*

### Comparing `pycqBot-0.5.0.2/pycqBot/plugin/bilibili/bilibili.py` & `pycqBot-0.5.1/pycqBot/plugin/bilibili/bilibili.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import logging
 import requests
 import time
 from lxml import etree
-from pycqBot.cqApi import cqBot, cqHttpApi
+from pycqBot.cqHttpApi import cqBot, cqHttpApi
 from pycqBot.cqCode import image
 from pycqBot.object import Message, Plugin
 
 
 class bilibili(Plugin):
     """
     bilibili 监听动态/直播 消息 自动解析 bilibili qq 小程序分享信息
```

### Comparing `pycqBot-0.5.0.2/pycqBot/plugin/manage/manage.py` & `pycqBot-0.5.1/pycqBot/plugin/manage/manage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from pycqBot.cqApi import cqBot, cqHttpApi
+from pycqBot.cqHttpApi import cqBot, cqHttpApi
 from pycqBot.object import Plugin
 from pycqBot.data import *
 
 
 class manage(Plugin):
     """
     群管理插件
```

### Comparing `pycqBot-0.5.0.2/pycqBot/plugin/pixiv/pixiv.py` & `pycqBot-0.5.1/pycqBot/plugin/pixiv/pixiv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import random
 from lxml import etree
-from pycqBot.cqApi import cqBot, cqHttpApi
+from pycqBot.cqHttpApi import cqBot, cqHttpApi
 from pycqBot.cqCode import image, node_list
 from pycqBot.object import Plugin
 from pycqBot.data import *
 
 
 class pixiv(Plugin):
     """
```

### Comparing `pycqBot-0.5.0.2/pycqBot/plugin/test/test.py` & `pycqBot-0.5.1/pycqBot/plugin/test/test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pyexpat.errors import messages
-from pycqBot.cqApi import cqBot, cqHttpApi
+from pycqBot.cqHttpApi import cqBot, cqHttpApi
 from pycqBot.object import Plugin, Message
 
 
 class test(Plugin):
     """
     测试插件
     """
```

### Comparing `pycqBot-0.5.0.2/pycqBot/plugin/twitter/twitter.py` & `pycqBot-0.5.1/pycqBot/plugin/twitter/twitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import time
 from pycqBot.object import Plugin
-from pycqBot.cqApi import cqBot, cqHttpApi
+from pycqBot.cqHttpApi import cqBot, cqHttpApi
 
 
 class twitter(Plugin):
     """
     基于 twitter API 监听推文
 
     插件配置
```

### Comparing `pycqBot-0.5.0.2/pycqBot.egg-info/SOURCES.txt` & `pycqBot-0.5.1/pycqBot.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 README.md
 setup.py
 pycqBot/__init__.py
 pycqBot/asyncHttp.py
 pycqBot/cqApi.py
 pycqBot/cqCode.py
+pycqBot/cqEvent.py
+pycqBot/cqHttpApi.py
 pycqBot/object.py
 pycqBot.egg-info/PKG-INFO
 pycqBot.egg-info/SOURCES.txt
 pycqBot.egg-info/dependency_links.txt
 pycqBot.egg-info/requires.txt
 pycqBot.egg-info/top_level.txt
 pycqBot/data/__init__.py
```

### Comparing `pycqBot-0.5.0.2/setup.py` & `pycqBot-0.5.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="pycqBot",
-    version="0.5.0.2",
+    version="0.5.1",
     description="go-cqhttp python 框架，可以用于快速塔建 bot",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
```

