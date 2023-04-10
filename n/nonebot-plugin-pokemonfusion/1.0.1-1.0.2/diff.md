# Comparing `tmp/nonebot_plugin_pokemonfusion-1.0.1.tar.gz` & `tmp/nonebot_plugin_pokemonfusion-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pokemonfusion-1.0.1.tar", last modified: Mon Apr 10 04:04:40 2023, max compression
+gzip compressed data, was "nonebot_plugin_pokemonfusion-1.0.2.tar", last modified: Mon Apr 10 05:12:35 2023, max compression
```

## Comparing `nonebot_plugin_pokemonfusion-1.0.1.tar` & `nonebot_plugin_pokemonfusion-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 04:04:40.154366 nonebot_plugin_pokemonfusion-1.0.1/
--rw-rw-rw-   0        0        0     1084 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      590 2023-04-10 04:04:40.154366 nonebot_plugin_pokemonfusion-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       98 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 04:04:40.143366 nonebot_plugin_pokemonfusion-1.0.1/nonebot_plugin_pokemonfusion/
--rw-rw-rw-   0        0        0     3279 2023-04-10 01:40:52.000000 nonebot_plugin_pokemonfusion-1.0.1/nonebot_plugin_pokemonfusion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 04:04:40.153366 nonebot_plugin_pokemonfusion-1.0.1/nonebot_plugin_pokemonfusion.egg-info/
--rw-rw-rw-   0        0        0      590 2023-04-10 04:04:40.000000 nonebot_plugin_pokemonfusion-1.0.1/nonebot_plugin_pokemonfusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-04-10 04:04:40.000000 nonebot_plugin_pokemonfusion-1.0.1/nonebot_plugin_pokemonfusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 04:04:40.000000 nonebot_plugin_pokemonfusion-1.0.1/nonebot_plugin_pokemonfusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-10 04:04:40.000000 nonebot_plugin_pokemonfusion-1.0.1/nonebot_plugin_pokemonfusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-04-10 04:04:40.000000 nonebot_plugin_pokemonfusion-1.0.1/nonebot_plugin_pokemonfusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 04:04:40.154366 nonebot_plugin_pokemonfusion-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      818 2023-04-10 04:03:25.000000 nonebot_plugin_pokemonfusion-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:12:35.435913 nonebot_plugin_pokemonfusion-1.0.2/
+-rw-rw-rw-   0        0        0     1084 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      590 2023-04-10 05:12:35.435913 nonebot_plugin_pokemonfusion-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       98 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 05:12:35.426913 nonebot_plugin_pokemonfusion-1.0.2/nonebot_plugin_pokemonfusion/
+-rw-rw-rw-   0        0        0     3496 2023-04-10 05:09:18.000000 nonebot_plugin_pokemonfusion-1.0.2/nonebot_plugin_pokemonfusion/__init__.py
+-rw-rw-rw-   0        0        0      304 2023-04-10 04:58:57.000000 nonebot_plugin_pokemonfusion-1.0.2/nonebot_plugin_pokemonfusion/tesrt.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:12:35.434917 nonebot_plugin_pokemonfusion-1.0.2/nonebot_plugin_pokemonfusion.egg-info/
+-rw-rw-rw-   0        0        0      590 2023-04-10 05:12:35.000000 nonebot_plugin_pokemonfusion-1.0.2/nonebot_plugin_pokemonfusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-04-10 05:12:35.000000 nonebot_plugin_pokemonfusion-1.0.2/nonebot_plugin_pokemonfusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 05:12:35.000000 nonebot_plugin_pokemonfusion-1.0.2/nonebot_plugin_pokemonfusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-10 05:12:35.000000 nonebot_plugin_pokemonfusion-1.0.2/nonebot_plugin_pokemonfusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-04-10 05:12:35.000000 nonebot_plugin_pokemonfusion-1.0.2/nonebot_plugin_pokemonfusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 05:12:35.435913 nonebot_plugin_pokemonfusion-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      818 2023-04-10 05:12:31.000000 nonebot_plugin_pokemonfusion-1.0.2/setup.py
```

### Comparing `nonebot_plugin_pokemonfusion-1.0.1/LICENSE` & `nonebot_plugin_pokemonfusion-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pokemonfusion-1.0.1/PKG-INFO` & `nonebot_plugin_pokemonfusion-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_pokemonfusion
-Version: 1.0.1
+Version: 1.0.2
 Summary: Nonebot2的Pokemon Infinite Fusion中文版融合计算器插件
 Home-page: https://github.com/IllusiveBull/nonebot_plugin_pokemonfusion
 Author: IllusiveBull
 Author-email: xjn233@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot_plugin_pokemonfusion-1.0.1/nonebot_plugin_pokemonfusion/__init__.py` & `nonebot_plugin_pokemonfusion-1.0.2/nonebot_plugin_pokemonfusion/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from nonebot.plugin import on_command
 from nonebot.adapters.onebot.v11 import Message, MessageSegment, MessageEvent
 from nonebot.params import CommandArg
 from nonebot.utils import run_sync
+from nonebot.log import logger
 
-import requests
+import httpx
 import json
 import difflib
 from io import BytesIO
 from PIL import Image
 import random
 from pathlib import Path
 
@@ -37,25 +38,26 @@
         im = Image.open(BytesIO(res.content)).convert("RGBA")
         p = Image.new('RGBA', im.size, (255,255,255))
         p.paste(im, (0, 0),mask=im)
         newim = BytesIO()
         p.save(newim,format="png")
         return newim
 
-@run_sync
-def get_image(fusionid):
-    fusionUrl = "https://raw.githubusercontent.com/Aegide/custom-fusion-sprites/main/CustomBattlers/" + fusionid
-    res = requests.get(fusionUrl)
+async def get_image(fusionid):
+    fusionUrl = "https://ghproxy.com/https://raw.githubusercontent.com/Aegide/custom-fusion-sprites/main/CustomBattlers/" + fusionid
+    async with httpx.AsyncClient() as client:
+        res = await client.get(fusionUrl)
     if res.status_code != 404:
         return(res2BytesIO(res))
     else:
-        fallbackFusionRepository = "https://raw.githubusercontent.com/Aegide/autogen-fusion-sprites/master/Battlers/"
+        fallbackFusionRepository = "https://ghproxy.com/https://raw.githubusercontent.com/Aegide/autogen-fusion-sprites/master/Battlers/"
         headId = fusionid.split(".")[0]
         fallbackFusionUrl = fallbackFusionRepository + headId + "/" + fusionid
-        res = requests.get(fallbackFusionUrl)
+        async with httpx.AsyncClient() as client:
+            res = await client.get(fallbackFusionUrl)
         return(res2BytesIO(res))
 
 fusion = on_command("融合", aliases={"融合"},priority=3)
 @fusion.handle()
 async def _(event: MessageEvent, args: Message = CommandArg()):
     names = args.extract_plain_text().split(" ")
     msgs = []
@@ -74,10 +76,11 @@
             fusion_ids = [f"{pokemons[name]}.{a}.png",f"{a}.{pokemons[name]}.png"]
     elif names == ['']:
         a = random.randint(1,420)
         b = random.randint(1,420)
         fusion_ids = [f"{b}.{a}.png",f"{a}.{b}.png"]
     try:
         msgs = [MessageSegment.image(await get_image(fusionid)) for fusionid in fusion_ids]
-    except:
+    except Exception as e:
+        logger.info(e)
         pass
     await fusion.finish(Message(msgs))
```

### Comparing `nonebot_plugin_pokemonfusion-1.0.1/nonebot_plugin_pokemonfusion.egg-info/PKG-INFO` & `nonebot_plugin_pokemonfusion-1.0.2/nonebot_plugin_pokemonfusion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pokemonfusion
-Version: 1.0.1
+Version: 1.0.2
 Summary: Nonebot2的Pokemon Infinite Fusion中文版融合计算器插件
 Home-page: https://github.com/IllusiveBull/nonebot_plugin_pokemonfusion
 Author: IllusiveBull
 Author-email: xjn233@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot_plugin_pokemonfusion-1.0.1/setup.py` & `nonebot_plugin_pokemonfusion-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r",encoding='utf-8') as fh:
   long_description = fh.read()
 requirements = [r.strip() for r in open("requirements.txt", 'r', encoding='utf-8').readlines()]
 
 setuptools.setup(
   name="nonebot_plugin_pokemonfusion",
-  version="1.0.1",
+  version="1.0.2",
   author="IllusiveBull",
   author_email="xjn233@gmail.com",
   description="Nonebot2的Pokemon Infinite Fusion中文版融合计算器插件",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/IllusiveBull/nonebot_plugin_pokemonfusion",
   packages=setuptools.find_packages(),
```

