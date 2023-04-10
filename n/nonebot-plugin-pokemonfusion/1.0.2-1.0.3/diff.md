# Comparing `tmp/nonebot_plugin_pokemonfusion-1.0.2.tar.gz` & `tmp/nonebot_plugin_pokemonfusion-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pokemonfusion-1.0.2.tar", last modified: Mon Apr 10 05:12:35 2023, max compression
+gzip compressed data, was "nonebot_plugin_pokemonfusion-1.0.3.tar", last modified: Mon Apr 10 05:18:06 2023, max compression
```

## Comparing `nonebot_plugin_pokemonfusion-1.0.2.tar` & `nonebot_plugin_pokemonfusion-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 05:12:35.435913 nonebot_plugin_pokemonfusion-1.0.2/
--rw-rw-rw-   0        0        0     1084 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      590 2023-04-10 05:12:35.435913 nonebot_plugin_pokemonfusion-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       98 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 05:12:35.426913 nonebot_plugin_pokemonfusion-1.0.2/nonebot_plugin_pokemonfusion/
--rw-rw-rw-   0        0        0     3496 2023-04-10 05:09:18.000000 nonebot_plugin_pokemonfusion-1.0.2/nonebot_plugin_pokemonfusion/__init__.py
--rw-rw-rw-   0        0        0      304 2023-04-10 04:58:57.000000 nonebot_plugin_pokemonfusion-1.0.2/nonebot_plugin_pokemonfusion/tesrt.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:12:35.434917 nonebot_plugin_pokemonfusion-1.0.2/nonebot_plugin_pokemonfusion.egg-info/
--rw-rw-rw-   0        0        0      590 2023-04-10 05:12:35.000000 nonebot_plugin_pokemonfusion-1.0.2/nonebot_plugin_pokemonfusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-04-10 05:12:35.000000 nonebot_plugin_pokemonfusion-1.0.2/nonebot_plugin_pokemonfusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 05:12:35.000000 nonebot_plugin_pokemonfusion-1.0.2/nonebot_plugin_pokemonfusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-10 05:12:35.000000 nonebot_plugin_pokemonfusion-1.0.2/nonebot_plugin_pokemonfusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-04-10 05:12:35.000000 nonebot_plugin_pokemonfusion-1.0.2/nonebot_plugin_pokemonfusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 05:12:35.435913 nonebot_plugin_pokemonfusion-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      818 2023-04-10 05:12:31.000000 nonebot_plugin_pokemonfusion-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:18:06.027426 nonebot_plugin_pokemonfusion-1.0.3/
+-rw-rw-rw-   0        0        0     1084 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      590 2023-04-10 05:18:06.027426 nonebot_plugin_pokemonfusion-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       98 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 05:18:06.014426 nonebot_plugin_pokemonfusion-1.0.3/nonebot_plugin_pokemonfusion/
+-rw-rw-rw-   0        0        0     3389 2023-04-10 05:15:55.000000 nonebot_plugin_pokemonfusion-1.0.3/nonebot_plugin_pokemonfusion/__init__.py
+-rw-rw-rw-   0        0        0      304 2023-04-10 04:58:57.000000 nonebot_plugin_pokemonfusion-1.0.3/nonebot_plugin_pokemonfusion/tesrt.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:18:06.026426 nonebot_plugin_pokemonfusion-1.0.3/nonebot_plugin_pokemonfusion.egg-info/
+-rw-rw-rw-   0        0        0      590 2023-04-10 05:18:05.000000 nonebot_plugin_pokemonfusion-1.0.3/nonebot_plugin_pokemonfusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-04-10 05:18:05.000000 nonebot_plugin_pokemonfusion-1.0.3/nonebot_plugin_pokemonfusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 05:18:05.000000 nonebot_plugin_pokemonfusion-1.0.3/nonebot_plugin_pokemonfusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-10 05:18:05.000000 nonebot_plugin_pokemonfusion-1.0.3/nonebot_plugin_pokemonfusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-04-10 05:18:05.000000 nonebot_plugin_pokemonfusion-1.0.3/nonebot_plugin_pokemonfusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 05:18:06.027426 nonebot_plugin_pokemonfusion-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      818 2023-04-10 05:17:46.000000 nonebot_plugin_pokemonfusion-1.0.3/setup.py
```

### Comparing `nonebot_plugin_pokemonfusion-1.0.2/LICENSE` & `nonebot_plugin_pokemonfusion-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pokemonfusion-1.0.2/PKG-INFO` & `nonebot_plugin_pokemonfusion-1.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_pokemonfusion
-Version: 1.0.2
+Version: 1.0.3
 Summary: Nonebot2的Pokemon Infinite Fusion中文版融合计算器插件
 Home-page: https://github.com/IllusiveBull/nonebot_plugin_pokemonfusion
 Author: IllusiveBull
 Author-email: xjn233@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot_plugin_pokemonfusion-1.0.2/nonebot_plugin_pokemonfusion/__init__.py` & `nonebot_plugin_pokemonfusion-1.0.3/nonebot_plugin_pokemonfusion/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from nonebot.plugin import on_command
 from nonebot.adapters.onebot.v11 import Message, MessageSegment, MessageEvent
 from nonebot.params import CommandArg
-from nonebot.utils import run_sync
-from nonebot.log import logger
 
 import httpx
 import json
 import difflib
 from io import BytesIO
 from PIL import Image
 import random
@@ -76,11 +74,10 @@
             fusion_ids = [f"{pokemons[name]}.{a}.png",f"{a}.{pokemons[name]}.png"]
     elif names == ['']:
         a = random.randint(1,420)
         b = random.randint(1,420)
         fusion_ids = [f"{b}.{a}.png",f"{a}.{b}.png"]
     try:
         msgs = [MessageSegment.image(await get_image(fusionid)) for fusionid in fusion_ids]
-    except Exception as e:
-        logger.info(e)
+    except:
         pass
     await fusion.finish(Message(msgs))
```

### Comparing `nonebot_plugin_pokemonfusion-1.0.2/nonebot_plugin_pokemonfusion.egg-info/PKG-INFO` & `nonebot_plugin_pokemonfusion-1.0.3/nonebot_plugin_pokemonfusion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pokemonfusion
-Version: 1.0.2
+Version: 1.0.3
 Summary: Nonebot2的Pokemon Infinite Fusion中文版融合计算器插件
 Home-page: https://github.com/IllusiveBull/nonebot_plugin_pokemonfusion
 Author: IllusiveBull
 Author-email: xjn233@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot_plugin_pokemonfusion-1.0.2/setup.py` & `nonebot_plugin_pokemonfusion-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r",encoding='utf-8') as fh:
   long_description = fh.read()
 requirements = [r.strip() for r in open("requirements.txt", 'r', encoding='utf-8').readlines()]
 
 setuptools.setup(
   name="nonebot_plugin_pokemonfusion",
-  version="1.0.2",
+  version="1.0.3",
   author="IllusiveBull",
   author_email="xjn233@gmail.com",
   description="Nonebot2的Pokemon Infinite Fusion中文版融合计算器插件",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/IllusiveBull/nonebot_plugin_pokemonfusion",
   packages=setuptools.find_packages(),
```

