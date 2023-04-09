# Comparing `tmp/nonebot-plugin-SDGPT-0.0.9.tar.gz` & `tmp/nonebot-plugin-SDGPT-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-SDGPT-0.0.9.tar", last modified: Sun Apr  9 00:36:06 2023, max compression
+gzip compressed data, was "nonebot-plugin-SDGPT-0.1.0.tar", last modified: Sun Apr  9 22:13:52 2023, max compression
```

## Comparing `nonebot-plugin-SDGPT-0.0.9.tar` & `nonebot-plugin-SDGPT-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 00:36:06.534931 nonebot-plugin-SDGPT-0.0.9/
--rw-rw-rw-   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot-plugin-SDGPT-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      210 2023-04-09 00:36:06.534931 nonebot-plugin-SDGPT-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      699 2023-04-09 00:32:22.000000 nonebot-plugin-SDGPT-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 00:36:06.524923 nonebot-plugin-SDGPT-0.0.9/nonebot_plugin_SDGPT/
--rw-rw-rw-   0        0        0     3550 2023-04-08 23:48:23.000000 nonebot-plugin-SDGPT-0.0.9/nonebot_plugin_SDGPT/__init__.py
--rw-rw-rw-   0        0        0     9400 2023-04-09 00:35:17.000000 nonebot-plugin-SDGPT-0.0.9/nonebot_plugin_SDGPT/bot.py
-drwxrwxrwx   0        0        0        0 2023-04-09 00:36:06.532930 nonebot-plugin-SDGPT-0.0.9/nonebot_plugin_SDGPT.egg-info/
--rw-rw-rw-   0        0        0      210 2023-04-09 00:36:06.000000 nonebot-plugin-SDGPT-0.0.9/nonebot_plugin_SDGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-04-09 00:36:06.000000 nonebot-plugin-SDGPT-0.0.9/nonebot_plugin_SDGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 00:36:06.000000 nonebot-plugin-SDGPT-0.0.9/nonebot_plugin_SDGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      101 2023-04-09 00:36:06.000000 nonebot-plugin-SDGPT-0.0.9/nonebot_plugin_SDGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-09 00:36:06.000000 nonebot-plugin-SDGPT-0.0.9/nonebot_plugin_SDGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 00:36:06.535933 nonebot-plugin-SDGPT-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      663 2023-04-09 00:35:06.000000 nonebot-plugin-SDGPT-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 22:13:52.437157 nonebot-plugin-SDGPT-0.1.0/
+-rw-rw-rw-   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot-plugin-SDGPT-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      210 2023-04-09 22:13:52.436156 nonebot-plugin-SDGPT-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1034 2023-04-09 01:25:35.000000 nonebot-plugin-SDGPT-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 22:13:52.423164 nonebot-plugin-SDGPT-0.1.0/nonebot_plugin_SDGPT/
+-rw-rw-rw-   0        0        0     3550 2023-04-08 23:48:23.000000 nonebot-plugin-SDGPT-0.1.0/nonebot_plugin_SDGPT/__init__.py
+-rw-rw-rw-   0        0        0     9410 2023-04-09 22:11:16.000000 nonebot-plugin-SDGPT-0.1.0/nonebot_plugin_SDGPT/bot.py
+drwxrwxrwx   0        0        0        0 2023-04-09 22:13:52.433153 nonebot-plugin-SDGPT-0.1.0/nonebot_plugin_SDGPT.egg-info/
+-rw-rw-rw-   0        0        0      210 2023-04-09 22:13:52.000000 nonebot-plugin-SDGPT-0.1.0/nonebot_plugin_SDGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-04-09 22:13:52.000000 nonebot-plugin-SDGPT-0.1.0/nonebot_plugin_SDGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 22:13:52.000000 nonebot-plugin-SDGPT-0.1.0/nonebot_plugin_SDGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2023-04-09 22:13:52.000000 nonebot-plugin-SDGPT-0.1.0/nonebot_plugin_SDGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-09 22:13:52.000000 nonebot-plugin-SDGPT-0.1.0/nonebot_plugin_SDGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 22:13:52.437157 nonebot-plugin-SDGPT-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      663 2023-04-09 22:13:43.000000 nonebot-plugin-SDGPT-0.1.0/setup.py
```

### Comparing `nonebot-plugin-SDGPT-0.0.9/LICENSE` & `nonebot-plugin-SDGPT-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-SDGPT-0.0.9/README.md` & `nonebot-plugin-SDGPT-0.1.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -19,8 +19,18 @@
 ```
 - 方式二：使用`pip`安装
 ```
 python -m pip install nonebot-plugin-SDGPT
 ```
 > 如果你没有使用过NoneBot,  
 > 这里有一个现成的NoneBot基于SDGPT机器人:  
-> [**SDGPT-BOT**](https://github.com/thx114/SDGPT-BOT)
+> [**SDGPT-BOT**](https://github.com/thx114/SDGPT-BOT)
+>
+## more
+
+[**QQ 群 391517834**](https://jq.qq.com/?_wv=1027&k=eKsgovej)  
+[**SDGPT BOT**](https://github.com/thx114/SDGPT-BOT)  
+   
+[**NoneBot**](https://v2.nonebot.dev/)  
+[**ChatGPT**](https://github.com/acheong08/ChatGPT)  
+[**BingGPT**](https://github.com/dice2o/BingGPT)  
+[**SD-api**](https://github.com/mix1009/sdwebuiapi)
```

### Comparing `nonebot-plugin-SDGPT-0.0.9/nonebot_plugin_SDGPT/__init__.py` & `nonebot-plugin-SDGPT-0.1.0/nonebot_plugin_SDGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-SDGPT-0.0.9/nonebot_plugin_SDGPT/bot.py` & `nonebot-plugin-SDGPT-0.1.0/nonebot_plugin_SDGPT/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 'cookies_file_path': "./cookies.json",
 }
 
 
 
 async def Chat(func,message:str,mode=1): 
     if not message or len(message)<1:return
-    Rtime = cfg['Chat_stream_waitTime']
+    Rtime = int(cfg['Chat_stream_waitTime'])
     endStr = cfg['Chat_stream_endStr']
     text = ''
     out_text=''
     info('ChatGPT','开始询问 (网页)')
     for data in chatbot.ask(message):
         text = data["message"] # type: ignore
         try: not now # type: ignore
@@ -113,15 +113,15 @@
         success('ChatGPT api', text)
         await func.send(text)
     if mode ==2:
         return text.replace(r'.*\.AIP','')
 
 async def Bing(func,message,mode=1):
     if not message or len(message)<1:return
-    Rtime = cfg['Chat_stream_waitTime']
+    Rtime = int(cfg['Chat_stream_waitTime'])
     endStr = cfg['Chat_stream_endStr']
     text = ''
     out_text=''
     info('Bing','开始询问 api')
     async for data in bingbot.ask_stream(message):
         istrue , string = data
         if type(string) == str : text = string
```

### Comparing `nonebot-plugin-SDGPT-0.0.9/setup.py` & `nonebot-plugin-SDGPT-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 
 
 setuptools.setup(
     name="nonebot-plugin-SDGPT",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.0.9",  # 程序版本
+    version="0.1.0",  # 程序版本
     author="F_thx",  # 项目作者
     author_email="thx1140093097@gmail.com",  # 作者邮件
     url="https://github.com/thx114/SDGPT",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
     license="MIT Licence",
     install_requires=[
         'nonebot2',
```

