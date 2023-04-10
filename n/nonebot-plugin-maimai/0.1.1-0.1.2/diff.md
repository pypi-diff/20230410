# Comparing `tmp/nonebot_plugin_maimai-0.1.1.tar.gz` & `tmp/nonebot_plugin_maimai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_maimai-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_maimai-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_maimai-0.1.1.tar` & `nonebot_plugin_maimai-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1089 2023-02-08 00:46:07.674998 nonebot_plugin_maimai-0.1.1/LICENSE
--rw-r--r--   0        0        0    13071 2023-03-10 06:30:40.141102 nonebot_plugin_maimai-0.1.1/nonebot_plugin_maimai/__init__.py
--rw-r--r--   0        0        0        0 2023-02-08 03:30:51.719115 nonebot_plugin_maimai-0.1.1/nonebot_plugin_maimai/libraries/__init__.py
--rw-r--r--   0        0        0     1605 2023-02-08 01:36:17.843087 nonebot_plugin_maimai-0.1.1/nonebot_plugin_maimai/libraries/image.py
--rw-r--r--   0        0        0    17833 2023-02-13 15:25:45.342461 nonebot_plugin_maimai-0.1.1/nonebot_plugin_maimai/libraries/maimai_best_40.py
--rw-r--r--   0        0        0    17924 2023-02-08 01:57:57.403213 nonebot_plugin_maimai-0.1.1/nonebot_plugin_maimai/libraries/maimai_best_50.py
--rw-r--r--   0        0        0     5218 2023-02-08 06:25:11.968762 nonebot_plugin_maimai-0.1.1/nonebot_plugin_maimai/libraries/maimaidx_music.py
--rw-r--r--   0        0        0      397 2023-03-02 02:30:46.242798 nonebot_plugin_maimai-0.1.1/nonebot_plugin_maimai/libraries/tool.py
--rw-r--r--   0        0        0     2231 2023-02-14 02:53:56.234278 nonebot_plugin_maimai-0.1.1/nonebot_plugin_maimai/public.py
--rw-r--r--   0        0        0     1069 2023-03-24 06:39:17.045541 nonebot_plugin_maimai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3364 2023-03-24 06:38:53.188167 nonebot_plugin_maimai-0.1.1/README.md
--rw-r--r--   0        0        0     4244 1970-01-01 00:00:00.000000 nonebot_plugin_maimai-0.1.1/setup.py
--rw-r--r--   0        0        0     4514 1970-01-01 00:00:00.000000 nonebot_plugin_maimai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-02-08 00:46:07.674998 nonebot_plugin_maimai-0.1.2/LICENSE
+-rw-r--r--   0        0        0    13071 2023-03-10 06:30:40.141102 nonebot_plugin_maimai-0.1.2/nonebot_plugin_maimai/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-08 03:30:51.719115 nonebot_plugin_maimai-0.1.2/nonebot_plugin_maimai/libraries/__init__.py
+-rw-r--r--   0        0        0     1605 2023-02-08 01:36:17.843087 nonebot_plugin_maimai-0.1.2/nonebot_plugin_maimai/libraries/image.py
+-rw-r--r--   0        0        0    17833 2023-02-13 15:25:45.342461 nonebot_plugin_maimai-0.1.2/nonebot_plugin_maimai/libraries/maimai_best_40.py
+-rw-r--r--   0        0        0    17924 2023-02-08 01:57:57.403213 nonebot_plugin_maimai-0.1.2/nonebot_plugin_maimai/libraries/maimai_best_50.py
+-rw-r--r--   0        0        0     5218 2023-02-08 06:25:11.968762 nonebot_plugin_maimai-0.1.2/nonebot_plugin_maimai/libraries/maimaidx_music.py
+-rw-r--r--   0        0        0      397 2023-03-02 02:30:46.242798 nonebot_plugin_maimai-0.1.2/nonebot_plugin_maimai/libraries/tool.py
+-rw-r--r--   0        0        0     1876 2023-04-10 20:56:42.562761 nonebot_plugin_maimai-0.1.2/nonebot_plugin_maimai/public.py
+-rw-r--r--   0        0        0     1069 2023-04-10 20:57:05.203217 nonebot_plugin_maimai-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3364 2023-03-24 06:38:53.188167 nonebot_plugin_maimai-0.1.2/README.md
+-rw-r--r--   0        0        0     4244 1970-01-01 00:00:00.000000 nonebot_plugin_maimai-0.1.2/setup.py
+-rw-r--r--   0        0        0     4514 1970-01-01 00:00:00.000000 nonebot_plugin_maimai-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_maimai-0.1.1/LICENSE` & `nonebot_plugin_maimai-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.1.1/nonebot_plugin_maimai/__init__.py` & `nonebot_plugin_maimai-0.1.2/nonebot_plugin_maimai/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.1.1/nonebot_plugin_maimai/libraries/image.py` & `nonebot_plugin_maimai-0.1.2/nonebot_plugin_maimai/libraries/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.1.1/nonebot_plugin_maimai/libraries/maimai_best_40.py` & `nonebot_plugin_maimai-0.1.2/nonebot_plugin_maimai/libraries/maimai_best_40.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.1.1/nonebot_plugin_maimai/libraries/maimai_best_50.py` & `nonebot_plugin_maimai-0.1.2/nonebot_plugin_maimai/libraries/maimai_best_50.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.1.1/nonebot_plugin_maimai/libraries/maimaidx_music.py` & `nonebot_plugin_maimai-0.1.2/nonebot_plugin_maimai/libraries/maimaidx_music.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.1.1/nonebot_plugin_maimai/public.py` & `nonebot_plugin_maimai-0.1.2/nonebot_plugin_maimai/public.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,21 +40,7 @@
     await help.send(MessageSegment.image(pic))
 
 
 async def _group_poke(bot: Bot, event: Event) -> bool:
     value = (event.notice_type == "notify" and event.sub_type == "poke" and event.target_id == int(bot.self_id))
     return value
 
-
-poke = on_notice(rule=_group_poke, priority=10, block=True)
-
-
-@poke.handle()
-async def _(bot: Bot, event: Event, state: T_State):
-    if event.__getattribute__('group_id') is None:
-        event.__delattr__('group_id')
-    await poke.send(Message([
-        MessageSegment("poke",  {
-           "qq": f"{event.sender_id}"
-       })
-    ]))
-
```

### Comparing `nonebot_plugin_maimai-0.1.1/pyproject.toml` & `nonebot_plugin_maimai-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_maimai"
-version = "0.1.1"
+version = "0.1.2"
 description= "Maimai DX plugin for NoneBot"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai"
 repository = "https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai"
 keywords = ["maimai", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_maimai-0.1.1/README.md` & `nonebot_plugin_maimai-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.1.1/setup.py` & `nonebot_plugin_maimai-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'nonebot-adapter-onebot>=2.1.3',
  'nonebot-plugin-txt2img>=0.3.0,<0.4.0',
  'nonebot2>=2.0.0rc3,<3.0.0',
  'pillow>=8.3.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-maimai',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Maimai DX plugin for NoneBot',
     'long_description': '<div align="center">\n  <img src="https://s2.loli.net/2022/06/16/opBDE8Swad5rU3n.png" width="180" height="180" alt="NoneBotPluginLogo">\n  <br>\n  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_maimai\n_✨maimaiDX，nonebot2插件版本✨_\n\n<a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai/stargazers">\n        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Umamusume-Agnes-Digital/nonebot_plugin_maimai" alt="stars">\n</a>\n<a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai/issues">\n        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Umamusume-Agnes-Digital/nonebot_plugin_maimai" alt="issues">\n</a>\n<a href="https://jq.qq.com/?_wv=1027&k=l82tMuPG">\n        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-424506063-orange?style=flat-square" alt="QQ Chat Group">\n</a>\n    <img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="python">\n    <img src="https://img.shields.io/badge/nonebot-2.0.0rc1+-red.svg" alt="NoneBot">\n</div>\n\n## 说明\n\n从[mai-bot](https://github.com/Diving-Fish/mai-bot)适配nonebot2插件，测试环境nonebot2.0.0rc1\n\n修改部分：\n - b40/b50可以艾特人查询\n - static文件可以放maimai插件文件夹中，或机器人路径下/data/maimai/static\n\n我做的适配有问题请冲我来不要打扰原作者捏，可以提iss或者[加群qq](https://jq.qq.com/?_wv=1027&k=l82tMuPG)反馈,\n\n## 前置步骤（和原项目一样）\n\n安装:\n\n    pip3 install nonebot_plugin_maimai\n    nb plugin install nonebot_plugin_maimai\n    # git clone 那我建议你还是用原作者的罢\n\n您需要从[此链接](https://www.diving-fish.com/maibot/static.zip)下载资源文件并，并将其static文件解压到:(以下方法2选1)\n\n - pypi`nonebot_plugin_maimai`文件夹中 - 最终路径类似是/path/to/nonebot_plugin_maimai/static\n - 机器人目录下 - 最终路径类似是/path/to/data/maimai/static中。其中bot.py文件在/path/to位置\n\n> 资源文件仅供学习交流使用，请自觉在下载 24 小时内删除资源文件。\n\n## FAQ\n\n配置 nonebot 或 cq-http 过程中出错？\n> 请查阅 https://github.com/nonebot/nonebot2 以及 https://github.com/Mrs4s/go-cqhttp 中的文档。\n\n部分消息发不出来？\n> 被风控了。解决方式：换号或者让这个号保持登陆状态和一定的聊天频率，持续一段时间。\n\n## 说明\n\n本 bot 提供了如下功能：\n\n命令 | 功能\n--- | ---\nhelp | 查看帮助文档\n今日舞萌 | 查看今天的舞萌运势\nXXXmaimaiXXX什么 | 随机一首歌\n随个[dx/标准][绿黄红紫白]<难度> | 随机一首指定条件的乐曲\n查歌<乐曲标题的一部分> | 查询符合条件的乐曲\n[绿黄红紫白]id<歌曲编号> | 查询乐曲信息或谱面信息\n定数查歌 <定数> <br> 定数查歌 <定数下限> <定数上限> |  查询定数对应的乐曲\n分数线 <难度+歌曲id> <分数线> | 展示歌曲的分数线\n\n## 原作者\n\n[Diving-Fish](https://github.com/Diving-Fish),感谢大佬为音游人的无私奉献\n\n## License\n\nMIT\n\n您可以自由使用本项目的代码用于商业或非商业的用途，但必须附带 MIT 授权协议。\n',
     'author': 'Agnes_Digital',
     'author_email': 'Z735803792@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai',
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_maimai', 'nonebot_plugin_maimai.libraries'] package_data = \
 {'': ['*']} install_requires = \ ['aiohttp>=3.8.1,<4.0.0', 'httpx>=0.23.0',
 'nonebot-adapter-onebot>=2.1.3', 'nonebot-plugin-txt2img>=0.3.0,<0.4.0',
 'nonebot2>=2.0.0rc3,<3.0.0', 'pillow>=8.3.0'] setup_kwargs = { 'name':
-'nonebot-plugin-maimai', 'version': '0.1.1', 'description': 'Maimai DX plugin
+'nonebot-plugin-maimai', 'version': '0.1.2', 'description': 'Maimai DX plugin
 for NoneBot', 'long_description': '
                            \n [NoneBotPluginLogo]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
 \n\n
   \n\n# nonebot_plugin_maimai\n_â¨maimaiDXï¼nonebot2æä»¶çæ¬â¨_\n\n\n_
```

### Comparing `nonebot_plugin_maimai-0.1.1/PKG-INFO` & `nonebot_plugin_maimai-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-maimai
-Version: 0.1.1
+Version: 0.1.2
 Summary: Maimai DX plugin for NoneBot
 Home-page: https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai
 License: MIT
 Keywords: maimai,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-maimai Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-maimai Version: 0.1.2 Summary:
 Maimai DX plugin for NoneBot Home-page: https://github.com/Umamusume-Agnes-
 Digital/nonebot_plugin_maimai License: MIT Keywords: maimai,nonebot2,plugin
 Author: Agnes_Digital Author-email: Z735803792@163.com Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

