# Comparing `tmp/nonebot-plugin-SDGPT-0.1.4.tar.gz` & `tmp/nonebot-plugin-SDGPT-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-SDGPT-0.1.4.tar", last modified: Mon Apr 10 16:58:07 2023, max compression
+gzip compressed data, was "nonebot-plugin-SDGPT-0.1.5.tar", last modified: Mon Apr 10 17:14:05 2023, max compression
```

## Comparing `nonebot-plugin-SDGPT-0.1.4.tar` & `nonebot-plugin-SDGPT-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 16:58:07.542768 nonebot-plugin-SDGPT-0.1.4/
--rw-rw-rw-   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot-plugin-SDGPT-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      210 2023-04-10 16:58:07.541791 nonebot-plugin-SDGPT-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1034 2023-04-09 01:25:35.000000 nonebot-plugin-SDGPT-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 16:58:07.533002 nonebot-plugin-SDGPT-0.1.4/nonebot_plugin_SDGPT/
--rw-rw-rw-   0        0        0     3339 2023-04-10 14:07:48.000000 nonebot-plugin-SDGPT-0.1.4/nonebot_plugin_SDGPT/__init__.py
--rw-rw-rw-   0        0        0     9917 2023-04-10 16:31:39.000000 nonebot-plugin-SDGPT-0.1.4/nonebot_plugin_SDGPT/bot.py
-drwxrwxrwx   0        0        0        0 2023-04-10 16:58:07.540814 nonebot-plugin-SDGPT-0.1.4/nonebot_plugin_SDGPT.egg-info/
--rw-rw-rw-   0        0        0      210 2023-04-10 16:58:07.000000 nonebot-plugin-SDGPT-0.1.4/nonebot_plugin_SDGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-04-10 16:58:07.000000 nonebot-plugin-SDGPT-0.1.4/nonebot_plugin_SDGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 16:58:07.000000 nonebot-plugin-SDGPT-0.1.4/nonebot_plugin_SDGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      101 2023-04-10 16:58:07.000000 nonebot-plugin-SDGPT-0.1.4/nonebot_plugin_SDGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-10 16:58:07.000000 nonebot-plugin-SDGPT-0.1.4/nonebot_plugin_SDGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 16:58:07.542768 nonebot-plugin-SDGPT-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      663 2023-04-10 16:56:53.000000 nonebot-plugin-SDGPT-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 17:14:05.347478 nonebot-plugin-SDGPT-0.1.5/
+-rw-rw-rw-   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot-plugin-SDGPT-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      210 2023-04-10 17:14:05.347478 nonebot-plugin-SDGPT-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1034 2023-04-09 01:25:35.000000 nonebot-plugin-SDGPT-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 17:14:05.336736 nonebot-plugin-SDGPT-0.1.5/nonebot_plugin_SDGPT/
+-rw-rw-rw-   0        0        0     3339 2023-04-10 14:07:48.000000 nonebot-plugin-SDGPT-0.1.5/nonebot_plugin_SDGPT/__init__.py
+-rw-rw-rw-   0        0        0     9918 2023-04-10 17:13:14.000000 nonebot-plugin-SDGPT-0.1.5/nonebot_plugin_SDGPT/bot.py
+drwxrwxrwx   0        0        0        0 2023-04-10 17:14:05.345525 nonebot-plugin-SDGPT-0.1.5/nonebot_plugin_SDGPT.egg-info/
+-rw-rw-rw-   0        0        0      210 2023-04-10 17:14:05.000000 nonebot-plugin-SDGPT-0.1.5/nonebot_plugin_SDGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-04-10 17:14:05.000000 nonebot-plugin-SDGPT-0.1.5/nonebot_plugin_SDGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 17:14:05.000000 nonebot-plugin-SDGPT-0.1.5/nonebot_plugin_SDGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2023-04-10 17:14:05.000000 nonebot-plugin-SDGPT-0.1.5/nonebot_plugin_SDGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-10 17:14:05.000000 nonebot-plugin-SDGPT-0.1.5/nonebot_plugin_SDGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 17:14:05.347478 nonebot-plugin-SDGPT-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      663 2023-04-10 17:12:20.000000 nonebot-plugin-SDGPT-0.1.5/setup.py
```

### Comparing `nonebot-plugin-SDGPT-0.1.4/LICENSE` & `nonebot-plugin-SDGPT-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-SDGPT-0.1.4/README.md` & `nonebot-plugin-SDGPT-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-SDGPT-0.1.4/nonebot_plugin_SDGPT/__init__.py` & `nonebot-plugin-SDGPT-0.1.5/nonebot_plugin_SDGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-SDGPT-0.1.4/nonebot_plugin_SDGPT/bot.py` & `nonebot-plugin-SDGPT-0.1.5/nonebot_plugin_SDGPT/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
 text2img_step=27 # 文生图 渲染步数
 text2img_negative_prompt="(worst quality, low quality:1.4),NSFW,r18" #文生图 固定负面提示词
 text2img_proxy='127.0.0.1:7860' #Stable-Diffusion api地址 (SD内配置 --server-name 127.0.0.1 --port 7860 --api)
 
 chat # 聊天 api 通用设置:
 presets_dir='./presets' # 预设文件夹
 Chat_stream_waitTime=2 # 频道内 分条发送间隔 (秒)
-Chat_stream_endStr=('？','。','?','\n') # 频道内 分条发送分割依据
+Chat_stream_endStr=('？','。','?','\\n') # 频道内 分条发送分割依据
 defaultAI='ChatGPT' # 默认 AI
 
 ChatGPT # ChatGPT 配置 (网页):
 access_token="" # access_token  获取:https://chat.openai.com/api/auth/session
 
 ChatGPT_api # ChatGPT api 配置:
 api_key="" # api_key 获取:https://platform.openai.com/account/api-keys
```

### Comparing `nonebot-plugin-SDGPT-0.1.4/setup.py` & `nonebot-plugin-SDGPT-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 
 
 setuptools.setup(
     name="nonebot-plugin-SDGPT",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.1.4",  # 程序版本
+    version="0.1.5",  # 程序版本
     author="F_thx",  # 项目作者
     author_email="thx1140093097@gmail.com",  # 作者邮件
     url="https://github.com/thx114/SDGPT",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
     license="MIT Licence",
     install_requires=[
         'nonebot2',
```

