# Comparing `tmp/nonebot_plugin_pokemonfusion-1.0.4.tar.gz` & `tmp/nonebot_plugin_pokemonfusion-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pokemonfusion-1.0.4.tar", last modified: Mon Apr 10 05:22:16 2023, max compression
+gzip compressed data, was "nonebot_plugin_pokemonfusion-1.0.5.tar", last modified: Mon Apr 10 05:39:52 2023, max compression
```

## Comparing `nonebot_plugin_pokemonfusion-1.0.4.tar` & `nonebot_plugin_pokemonfusion-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 05:22:16.024904 nonebot_plugin_pokemonfusion-1.0.4/
--rw-rw-rw-   0        0        0     1084 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      590 2023-04-10 05:22:16.024904 nonebot_plugin_pokemonfusion-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       98 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 05:22:16.011896 nonebot_plugin_pokemonfusion-1.0.4/nonebot_plugin_pokemonfusion/
--rw-rw-rw-   0        0        0     3389 2023-04-10 05:20:34.000000 nonebot_plugin_pokemonfusion-1.0.4/nonebot_plugin_pokemonfusion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:22:16.023903 nonebot_plugin_pokemonfusion-1.0.4/nonebot_plugin_pokemonfusion.egg-info/
--rw-rw-rw-   0        0        0      590 2023-04-10 05:22:15.000000 nonebot_plugin_pokemonfusion-1.0.4/nonebot_plugin_pokemonfusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-04-10 05:22:15.000000 nonebot_plugin_pokemonfusion-1.0.4/nonebot_plugin_pokemonfusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 05:22:15.000000 nonebot_plugin_pokemonfusion-1.0.4/nonebot_plugin_pokemonfusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-10 05:22:15.000000 nonebot_plugin_pokemonfusion-1.0.4/nonebot_plugin_pokemonfusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-04-10 05:22:15.000000 nonebot_plugin_pokemonfusion-1.0.4/nonebot_plugin_pokemonfusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 05:22:16.024904 nonebot_plugin_pokemonfusion-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      818 2023-04-10 05:22:05.000000 nonebot_plugin_pokemonfusion-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:39:52.610388 nonebot_plugin_pokemonfusion-1.0.5/
+-rw-rw-rw-   0        0        0     1084 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      590 2023-04-10 05:39:52.610388 nonebot_plugin_pokemonfusion-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       98 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 05:39:52.602388 nonebot_plugin_pokemonfusion-1.0.5/nonebot_plugin_pokemonfusion/
+-rw-rw-rw-   0        0        0     3497 2023-04-10 05:36:37.000000 nonebot_plugin_pokemonfusion-1.0.5/nonebot_plugin_pokemonfusion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:39:52.609388 nonebot_plugin_pokemonfusion-1.0.5/nonebot_plugin_pokemonfusion.egg-info/
+-rw-rw-rw-   0        0        0      590 2023-04-10 05:39:52.000000 nonebot_plugin_pokemonfusion-1.0.5/nonebot_plugin_pokemonfusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-04-10 05:39:52.000000 nonebot_plugin_pokemonfusion-1.0.5/nonebot_plugin_pokemonfusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 05:39:52.000000 nonebot_plugin_pokemonfusion-1.0.5/nonebot_plugin_pokemonfusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-10 05:39:52.000000 nonebot_plugin_pokemonfusion-1.0.5/nonebot_plugin_pokemonfusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-04-10 05:39:52.000000 nonebot_plugin_pokemonfusion-1.0.5/nonebot_plugin_pokemonfusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 05:39:52.610388 nonebot_plugin_pokemonfusion-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      818 2023-04-10 05:39:47.000000 nonebot_plugin_pokemonfusion-1.0.5/setup.py
```

### Comparing `nonebot_plugin_pokemonfusion-1.0.4/LICENSE` & `nonebot_plugin_pokemonfusion-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pokemonfusion-1.0.4/PKG-INFO` & `nonebot_plugin_pokemonfusion-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_pokemonfusion
-Version: 1.0.4
+Version: 1.0.5
 Summary: Nonebot2的Pokemon Infinite Fusion中文版融合计算器插件
 Home-page: https://github.com/IllusiveBull/nonebot_plugin_pokemonfusion
 Author: IllusiveBull
 Author-email: xjn233@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot_plugin_pokemonfusion-1.0.4/nonebot_plugin_pokemonfusion/__init__.py` & `nonebot_plugin_pokemonfusion-1.0.5/nonebot_plugin_pokemonfusion/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+import nonebot
 from nonebot.plugin import on_command
 from nonebot.adapters.onebot.v11 import Message, MessageSegment, MessageEvent
 from nonebot.params import CommandArg
 
 import httpx
 import json
 import difflib
 from io import BytesIO
 from PIL import Image
 import random
 from pathlib import Path
 
+try:
+    enable_transparent = nonebot.get_driver().config.enable_transparent
+except:
+    enable_transparent = False
 data_path = Path(__file__).parent/"resources/pokemons.json"
 with open(data_path,"r") as f:
     pokemons = json.load(f)
 
 def string_similar(s1, s2):
     return difflib.SequenceMatcher(None, s1, s2).quick_ratio()
 
@@ -25,15 +30,15 @@
     for i in range(3):
         result_list.append(newlist[similarity_list.index(sorted_list[0])])
         similarity_list.remove(sorted_list[0])
         sorted_list.pop(0)
         newlist.remove(result_list[i])
     return result_list
 
-def res2BytesIO(res, enable_transparent = False):
+def res2BytesIO(res):
     if enable_transparent == True:
         return BytesIO(res.content)
     else:
         im = Image.open(BytesIO(res.content)).convert("RGBA")
         p = Image.new('RGBA', im.size, (255,255,255))
         p.paste(im, (0, 0),mask=im)
         newim = BytesIO()
```

### Comparing `nonebot_plugin_pokemonfusion-1.0.4/nonebot_plugin_pokemonfusion.egg-info/PKG-INFO` & `nonebot_plugin_pokemonfusion-1.0.5/nonebot_plugin_pokemonfusion.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pokemonfusion
-Version: 1.0.4
+Version: 1.0.5
 Summary: Nonebot2的Pokemon Infinite Fusion中文版融合计算器插件
 Home-page: https://github.com/IllusiveBull/nonebot_plugin_pokemonfusion
 Author: IllusiveBull
 Author-email: xjn233@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot_plugin_pokemonfusion-1.0.4/setup.py` & `nonebot_plugin_pokemonfusion-1.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r",encoding='utf-8') as fh:
   long_description = fh.read()
 requirements = [r.strip() for r in open("requirements.txt", 'r', encoding='utf-8').readlines()]
 
 setuptools.setup(
   name="nonebot_plugin_pokemonfusion",
-  version="1.0.4",
+  version="1.0.5",
   author="IllusiveBull",
   author_email="xjn233@gmail.com",
   description="Nonebot2的Pokemon Infinite Fusion中文版融合计算器插件",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/IllusiveBull/nonebot_plugin_pokemonfusion",
   packages=setuptools.find_packages(),
```

