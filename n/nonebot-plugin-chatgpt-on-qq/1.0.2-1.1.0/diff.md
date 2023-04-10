# Comparing `tmp/nonebot-plugin-chatgpt-on-qq-1.0.2.tar.gz` & `tmp/nonebot-plugin-chatgpt-on-qq-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-chatgpt-on-qq-1.0.2.tar", last modified: Sun Apr  9 16:02:18 2023, max compression
+gzip compressed data, was "nonebot-plugin-chatgpt-on-qq-1.1.0.tar", last modified: Mon Apr 10 03:57:48 2023, max compression
```

## Comparing `nonebot-plugin-chatgpt-on-qq-1.0.2.tar` & `nonebot-plugin-chatgpt-on-qq-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 16:02:18.884490 nonebot-plugin-chatgpt-on-qq-1.0.2/
--rw-rw-rw-   0        0        0      769 2023-04-09 16:02:18.880487 nonebot-plugin-chatgpt-on-qq-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-07 17:39:40.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-09 16:02:18.850300 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq/
--rw-rw-rw-   0        0        0    12538 2023-04-09 15:34:37.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq/__init__.py
--rw-rw-rw-   0        0        0     3660 2023-04-09 15:33:24.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq/chatGPT.py
--rw-rw-rw-   0        0        0      416 2023-04-08 19:05:12.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq/config.py
--rw-rw-rw-   0        0        0     4351 2023-04-08 19:05:35.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq/conversation.py
--rw-rw-rw-   0        0        0      502 2023-03-07 16:08:33.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq/custom_errors.py
--rw-rw-rw-   0        0        0     5422 2023-04-09 15:59:04.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq/loadpresets.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:02:18.876493 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq.egg-info/
--rw-rw-rw-   0        0        0      769 2023-04-09 16:02:18.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      533 2023-04-09 16:02:18.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 16:02:18.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2023-04-09 16:02:18.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-04-09 16:02:18.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 16:02:18.884490 nonebot-plugin-chatgpt-on-qq-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-04-09 16:01:36.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:57:48.036484 nonebot-plugin-chatgpt-on-qq-1.1.0/
+-rw-rw-rw-   0        0        0      769 2023-04-10 03:57:48.035511 nonebot-plugin-chatgpt-on-qq-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-07 17:39:40.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-10 03:57:48.014719 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq/
+-rw-rw-rw-   0        0        0    12808 2023-04-10 03:38:53.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq/__init__.py
+-rw-rw-rw-   0        0        0     3660 2023-04-09 15:33:24.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq/chatGPT.py
+-rw-rw-rw-   0        0        0      416 2023-04-08 19:05:12.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq/config.py
+-rw-rw-rw-   0        0        0     4351 2023-04-08 19:05:35.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq/conversation.py
+-rw-rw-rw-   0        0        0      502 2023-03-07 16:08:33.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq/custom_errors.py
+-rw-rw-rw-   0        0        0     5518 2023-04-10 03:56:33.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq/loadpresets.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:57:48.031421 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq.egg-info/
+-rw-rw-rw-   0        0        0      769 2023-04-10 03:57:47.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      533 2023-04-10 03:57:47.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 03:57:47.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2023-04-10 03:57:47.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-04-10 03:57:47.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 03:57:48.036484 nonebot-plugin-chatgpt-on-qq-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-04-10 03:56:57.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/setup.py
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.0.2/PKG-INFO` & `nonebot-plugin-chatgpt-on-qq-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-on-qq
-Version: 1.0.2
+Version: 1.1.0
 Summary: 具有多对话功能的chatGPT聊天插件
 Home-page: https://github.com/Suxmx/nonebot_plugin_chatgpt_turbo_on_qq
 Author: 颜曦
 Author-email: 424504326@qq.com
 Maintainer: 颜曦
 Maintainer-email: 424504326@qq.com
 License: BSD License
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq/__init__.py` & `nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import re
+import openai
 
 from nonebot import get_driver
 from nonebot.adapters.onebot.v11 import (Bot,
                                          Event,
                                          GroupMessageEvent, PrivateMessageEvent)
 from nonebot.log import logger
 from nonebot.plugin import on_regex, on_fullmatch
@@ -46,44 +47,66 @@
     msg = event.get_plaintext()
     userInput: str = re.sub(r"^/talk\s+", '', msg)
     if not userInput:
         await Chat.finish("输入不能为空!", at_sender=True)
     if isinstance(event, GroupMessageEvent):
         groupId = event.group_id
         userId = event.get_user_id()
-        if not groupPanels.get(groupId):
-            await Chat.finish("当前群尚未创建过对话!请用/chat create命令来创建对话!", at_sender=True)
-        else:  # 获取GroupPanel
+        if not groupPanels.get(groupId) or not groupPanels.get(groupId).userInConversation.get(userId):# 若没有对话则先自动创建一个
+            try:
+                newConversation = Conversation.CreateWithTemplate("1", userId)
+            except:
+                await Chat.finish("自动创建失败!请检查模板是否存在", at_sender=True)
+            await Chat.send(f"自动创建{newConversation.name}成功",at_sender=True)
+            groupPanels[event.group_id] = GroupPanel()
+            groupPanels[event.group_id].userInConversation[userId] = newConversation
+            groupPanels[event.group_id].conversations.append(newConversation)
+            try:
+                answer = await newConversation.ask(userInput)
+                await newConversation.GroupAutoSave(groupId)
+            except openai.InvalidRequestError as e:
+                await Chat.finish(str(e))
+            
+        else:  # 获取GroupPanel以及用户所在的对话
             groupPanel = groupPanels.get(groupId)
-        if not groupPanel.userInConversation.get(userId):
-            await Chat.finish("你还没有加入一个对话!请用/chat create命令来创建对话!", at_sender=True)
-        else:  # 获取用户当前加入的对话
             userConversation: Conversation = groupPanel.userInConversation.get(
                 userId)
-        # try:
-        answer = await userConversation.ask(userInput)
-        await userConversation.GroupAutoSave(groupId)
-        # except Exception as e:
-        #     answer = "获取gpt回答失败,访问请求速度过快或是网络波动orz\n若反复出现,可尝试使用/chat delete 序号 命令来删除该对话并重新创建"
-        #     logger.error(str(e))
+            try:
+                answer = await userConversation.ask(userInput)
+                await userConversation.GroupAutoSave(groupId)
+            except openai.InvalidRequestError as e:
+                await Chat.finish(str(e))
+
         await Chat.finish(answer, at_sender=True)
     if isinstance(event, PrivateMessageEvent):
         userId = event.get_user_id()
-        if not privateConversations.get(userId):
-            await Chat.finish("尚未创建过对话!请用/chat create命令来创建对话!")
+        if not privateConversations.get(userId):# 自动创建
+            newConversation=None
+            try:
+                newConversation = Conversation.CreateWithTemplate("1", userId)
+            except:
+                await Chat.finish("自动创建失败!请检查模板是否存在")
+            if newConversation is not None:
+                await Chat.send(f"自动创建{newConversation.name}成功",at_sender=True)
+                privateConversations[userId] = newConversation
+                try:
+                    answer = await newConversation.ask(userInput)
+                    await Chat.send(answer)
+                    await newConversation.PrivateAutoSave()
+                except openai.InvalidRequestError as e:
+                    await Chat.finish(str(e))
         else:
             userConversation: Conversation = privateConversations.get(userId)
-            # try:
-            answer = await userConversation.ask(userInput)
-            await Chat.send(answer)
-            await userConversation.PrivateAutoSave()
-            # except Exception as e:
-            #     answer="test获取gpt回答失败,访问请求速度过快或是网络波动orz\n若反复出现,可尝试使用/chat delete 序号 命令来删除该对话并重新创建"
-            #     logger.error(str(e))
-            #     await Chat.finish(answer,at_sender=True)
+            try:
+                answer = await userConversation.ask(userInput)
+                await Chat.send(answer)
+                await userConversation.PrivateAutoSave()
+            except openai.InvalidRequestError as e:
+                    await Chat.finish(str(e))
+
 
 
 @Join.handle()
 async def _(event: Event):
     msg = event.get_plaintext()
     msg = re.sub(r"^/chat\s+join\s+", '', msg)
     id = int(msg)
@@ -220,25 +243,14 @@
         newConversation = Conversation.CreateWithTemplate(id, userId)
     except NoApiKeyError:
         await CreateConversationWithTemplate.finish("请机器人管理员在设置中添加APIKEY！")
     if newConversation is not None:
         await CreateConversationWithTemplate.send(f"创建{newConversation.name}模板成功!",at_sender=True)
     else :
         await CreateConversationWithTemplate.finish("输入ID无效!")
-    # if int(id) == 1:
-    #     if newConversation is not None:
-    #         await CreateConversationWithTemplate.send("创建普通模板成功!", at_sender=True)
-    # elif int(id) == 2:
-    #     if newConversation is not None:
-    #         await CreateConversationWithTemplate.send("创建猫娘模板成功!", at_sender=True)
-    # elif int(id) == 3:
-    #     if newConversation is not None:
-    #         await CreateConversationWithTemplate.send("创建诺拉模板成功!", at_sender=True)
-    # else:
-    #     await CreateConversationWithTemplate.finish("不存在该序号!")
     if ifGroup:
         if not groupPanels.get(event.group_id):
             groupPanels[event.group_id] = GroupPanel()
         groupPanels[event.group_id].userInConversation[userId] = newConversation
         groupPanels[event.group_id].conversations.append(newConversation)
     else:
         privateConversations[userId] = newConversation
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq/chatGPT.py` & `nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq/chatGPT.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq/conversation.py` & `nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq/conversation.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq/loadpresets.py` & `nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq/loadpresets.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,16 +23,18 @@
 
 def loadall(path: Path) -> list[presetcls]:
     if not os.path.exists(path):
         os.makedirs(path)
     presets: list[presetcls] = []
     presets.append(
         presetcls(name="ChatGPT", preset=BASIC_PROMPT, id=len(presets)+1))
+    logger.success(f"读取内置预设ChatGPT成功!")
     presets.append(
         presetcls(name="猫娘", preset=CAT_GIRL_PROMPT, id=len(presets)+1))
+    logger.success(f"读取内置预设猫娘成功!")
     for root, dirs, files in os.walk(path):
         for file in files:
             if file.endswith(".json"):
                 logger.debug(root)
                 try:
                     with open(os.path.join(root, file), "r", encoding="utf8") as f:
                         flag = True
@@ -66,15 +68,15 @@
                         filename = file.split(".")[0]
                         try:
                             logger.warning(
                                 f"以UTF-8读取预设:{filename}失败，尝试使用GB2312读取")
                             preset: list[dict[str, str]] = json.load(f)
                         except:
                             flag = False
-                            logger.error(f"预设: {filename} 读取失败!json格式错误!")
+                            logger.error(f"预设: {filename} 读取失败!")
                             break
                         # name = file.split(".")[0]
 
                         if not isinstance(preset, list):
                             flag = False
                         else:
                             for item in preset:
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO` & `nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-on-qq
-Version: 1.0.2
+Version: 1.1.0
 Summary: 具有多对话功能的chatGPT聊天插件
 Home-page: https://github.com/Suxmx/nonebot_plugin_chatgpt_turbo_on_qq
 Author: 颜曦
 Author-email: 424504326@qq.com
 Maintainer: 颜曦
 Maintainer-email: 424504326@qq.com
 License: BSD License
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt` & `nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-on-qq-1.0.2/setup.py` & `nonebot-plugin-chatgpt-on-qq-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding:utf-8
 
 from setuptools import find_packages, setup
 
 setup(
     name='nonebot-plugin-chatgpt-on-qq',
-    version='1.0.2',
+    version='1.1.0',
     description='具有多对话功能的chatGPT聊天插件',
     long_description=open('README.rst').read(),
     author='颜曦',
     author_email='424504326@qq.com',
     maintainer='颜曦',
     maintainer_email='424504326@qq.com',
     packages=find_packages(),
```

