# Comparing `tmp/nonebot_plugin_sdgpt-0.1.6.tar.gz` & `tmp/nonebot_plugin_sdgpt-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sdgpt-0.1.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_sdgpt-0.1.7.tar", max compression
```

## Comparing `nonebot_plugin_sdgpt-0.1.6.tar` & `nonebot_plugin_sdgpt-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3339 2023-04-10 14:07:48.620257 nonebot_plugin_sdgpt-0.1.6/__init__.py
--rw-r--r--   0        0        0     9983 2023-04-10 17:22:24.976760 nonebot_plugin_sdgpt-0.1.6/bot.py
--rw-r--r--   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot_plugin_sdgpt-0.1.6/LICENSE
--rw-r--r--   0        0        0      983 2023-04-10 17:40:24.012798 nonebot_plugin_sdgpt-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1034 2023-04-09 01:25:35.547383 nonebot_plugin_sdgpt-0.1.6/README.md
--rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 nonebot_plugin_sdgpt-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot_plugin_sdgpt-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3339 2023-04-10 14:07:48.620257 nonebot_plugin_sdgpt-0.1.7/nonebot_plugin_SDGPT/__init__.py
+-rw-r--r--   0        0        0     9983 2023-04-10 17:22:24.976760 nonebot_plugin_sdgpt-0.1.7/nonebot_plugin_SDGPT/bot.py
+-rw-r--r--   0        0        0     1004 2023-04-10 17:47:44.163226 nonebot_plugin_sdgpt-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1034 2023-04-09 01:25:35.547383 nonebot_plugin_sdgpt-0.1.7/README.md
+-rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 nonebot_plugin_sdgpt-0.1.7/PKG-INFO
```

### Comparing `nonebot_plugin_sdgpt-0.1.6/__init__.py` & `nonebot_plugin_sdgpt-0.1.7/nonebot_plugin_SDGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.1.6/bot.py` & `nonebot_plugin_sdgpt-0.1.7/nonebot_plugin_SDGPT/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.1.6/LICENSE` & `nonebot_plugin_sdgpt-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.1.6/pyproject.toml` & `nonebot_plugin_sdgpt-0.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "nonebot-plugin-SDGPT"
-version = "0.1.6"
+version = "0.1.7"
 description = "ChatBot for NoneBot : 链接 ChatGPT / Bing / Stable-Diffusion : ChatGPT Bing聊天, gpt解析自然语言转Stable-Diffusion生成图像"
 license = "MIT"
 authors = ["F_thx <thx1140093097@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/thx114/SDGPT"
 repository = "https://github.com/thx114/SDGPT"
 documentation = "https://github.com/thx114/SDGPTreadme"
 keywords = ["nonebot", "nonebot2", "chatgpt", "new bing","Stable-Diffusion"]
 packages = [
-    { include = "*.py"}
+    { include = "nonebot_plugin_SDGPT/*.py"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = "^2.0.0-beta.1"
 python-dotenv = "*"
 revChatGPT = "*"
```

### Comparing `nonebot_plugin_sdgpt-0.1.6/README.md` & `nonebot_plugin_sdgpt-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.1.6/PKG-INFO` & `nonebot_plugin_sdgpt-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sdgpt
-Version: 0.1.6
+Version: 0.1.7
 Summary: ChatBot for NoneBot : 链接 ChatGPT / Bing / Stable-Diffusion : ChatGPT Bing聊天, gpt解析自然语言转Stable-Diffusion生成图像
 Home-page: https://github.com/thx114/SDGPT
 License: MIT
 Keywords: nonebot,nonebot2,chatgpt,new bing,Stable-Diffusion
 Author: F_thx
 Author-email: thx1140093097@gmail.com
 Requires-Python: >=3.8,<4.0
```

