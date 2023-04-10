# Comparing `tmp/nonebot_plugin_searchbiliinfo-1.7.5.tar.gz` & `tmp/nonebot_plugin_searchbiliinfo-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_searchbiliinfo-1.7.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_searchbiliinfo-1.7.6.tar", max compression
```

## Comparing `nonebot_plugin_searchbiliinfo-1.7.5.tar` & `nonebot_plugin_searchbiliinfo-1.7.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1084 2022-12-03 13:20:36.036837 nonebot_plugin_searchbiliinfo-1.7.5/LICENSE
--rw-r--r--   0        0        0   102689 2023-04-09 15:37:15.350122 nonebot_plugin_searchbiliinfo-1.7.5/nonebot_plugin_searchBiliInfo/__init__.py
--rw-r--r--   0        0        0   356769 2023-03-07 03:59:53.911011 nonebot_plugin_searchbiliinfo-1.7.5/nonebot_plugin_searchBiliInfo/data.py
--rw-r--r--   0        0        0  6937547 2023-02-20 03:35:57.148057 nonebot_plugin_searchbiliinfo-1.7.5/nonebot_plugin_searchBiliInfo/data_medal.py
--rw-r--r--   0        0        0     3484 2023-02-24 08:29:21.055074 nonebot_plugin_searchbiliinfo-1.7.5/nonebot_plugin_searchBiliInfo/html/composition_page.html
--rw-r--r--   0        0        0     1264 2023-04-09 15:39:34.583640 nonebot_plugin_searchbiliinfo-1.7.5/pyproject.toml
--rw-r--r--   0        0        0    30100 2023-04-09 15:38:31.455541 nonebot_plugin_searchbiliinfo-1.7.5/README.md
--rw-r--r--   0        0        0    31228 1970-01-01 00:00:00.000000 nonebot_plugin_searchbiliinfo-1.7.5/setup.py
--rw-r--r--   0        0        0    30607 1970-01-01 00:00:00.000000 nonebot_plugin_searchbiliinfo-1.7.5/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-12-03 13:20:36.036837 nonebot_plugin_searchbiliinfo-1.7.6/LICENSE
+-rw-r--r--   0        0        0   102900 2023-04-10 09:15:46.214907 nonebot_plugin_searchbiliinfo-1.7.6/nonebot_plugin_searchBiliInfo/__init__.py
+-rw-r--r--   0        0        0   356769 2023-03-07 03:59:53.911011 nonebot_plugin_searchbiliinfo-1.7.6/nonebot_plugin_searchBiliInfo/data.py
+-rw-r--r--   0        0        0  6937547 2023-02-20 03:35:57.148057 nonebot_plugin_searchbiliinfo-1.7.6/nonebot_plugin_searchBiliInfo/data_medal.py
+-rw-r--r--   0        0        0     3484 2023-02-24 08:29:21.055074 nonebot_plugin_searchbiliinfo-1.7.6/nonebot_plugin_searchBiliInfo/html/composition_page.html
+-rw-r--r--   0        0        0     1264 2023-04-10 09:20:29.361603 nonebot_plugin_searchbiliinfo-1.7.6/pyproject.toml
+-rw-r--r--   0        0        0    30178 2023-04-10 09:17:45.855439 nonebot_plugin_searchbiliinfo-1.7.6/README.md
+-rw-r--r--   0        0        0    31306 1970-01-01 00:00:00.000000 nonebot_plugin_searchbiliinfo-1.7.6/setup.py
+-rw-r--r--   0        0        0    30682 1970-01-01 00:00:00.000000 nonebot_plugin_searchbiliinfo-1.7.6/PKG-INFO
```

### Comparing `nonebot_plugin_searchbiliinfo-1.7.5/LICENSE` & `nonebot_plugin_searchbiliinfo-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_searchbiliinfo-1.7.5/nonebot_plugin_searchBiliInfo/__init__.py` & `nonebot_plugin_searchbiliinfo-1.7.6/nonebot_plugin_searchBiliInfo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,17 +178,21 @@
         guard_info_json = await common_get_return_json(url)
 
     if guard_info_json == None:
         msg = "请求失败喵~可能是网络问题或者API寄了喵~"
         await catch_str.finish(Message(f'{msg}'), reply_message=True)
 
     try:
-        msg = '用户名：' + base_info_json['card']['name'] + '\nUID：' + str(base_info_json['card']['mid']) + \
-            '\n房间号：' + str(room_id) + '\n粉丝数：' + str(base_info_json['card']['fans']) + '\n舰团数：' + str(
-            guard_info_json['data']['info']['num'])
+        msg = '用户名：' + base_info_json['card']['name'] + \
+            '\nUID：' + str(base_info_json['card']['mid']) + \
+            '\n房间号：' + str(room_id) + \
+            '\n粉丝数：' + str(base_info_json['card']['fans']) + \
+            '\n舰团数：' + str(guard_info_json['data']['info']['num']) + \
+            '\n主页：' + 'https://space.bilibili.com/' + str(base_info_json['card']['mid']) + \
+            '\n直播间：' + 'https://live.bilibili.com/' + str(room_id)
     except:
         msg = "数据解析异常，请重试。（如果多次重试都失败，建议提issue待开发者修复）"
     await catch_str.finish(Message(f'{msg}'), reply_message=True)
 
 
 # 查弹幕
 @catch_str1.handle()
```

### Comparing `nonebot_plugin_searchbiliinfo-1.7.5/nonebot_plugin_searchBiliInfo/data.py` & `nonebot_plugin_searchbiliinfo-1.7.6/nonebot_plugin_searchBiliInfo/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_searchbiliinfo-1.7.5/nonebot_plugin_searchBiliInfo/data_medal.py` & `nonebot_plugin_searchbiliinfo-1.7.6/nonebot_plugin_searchBiliInfo/data_medal.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_searchbiliinfo-1.7.5/nonebot_plugin_searchBiliInfo/html/composition_page.html` & `nonebot_plugin_searchbiliinfo-1.7.6/nonebot_plugin_searchBiliInfo/html/composition_page.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_searchbiliinfo-1.7.5/pyproject.toml` & `nonebot_plugin_searchbiliinfo-1.7.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-searchbiliinfo"
-version = "1.7.5"
+version = "1.7.6"
 description = "A plugin for nonebot2. Query Bilibili user information（一个Nonebot2的插件，b站用户信息查询插件【粉丝、舰团信息；直播收益数据；直播观看信息；关键词搜昵称、UID；主播营收榜单；查成分；查牌子等】）"
 authors = ["Ikaros <327209194@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_searchbiliinfo"}]
 homepage = "https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo"
 repository = "https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo"
```

### Comparing `nonebot_plugin_searchbiliinfo-1.7.5/README.md` & `nonebot_plugin_searchbiliinfo-1.7.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -685,14 +685,17 @@
 
 ### 1.7.4
 修改`eh查直播`为直接请求，不过跳过了ssl。  
 
 ### 1.7.5
 bug修复  
 
+### 1.7.6
+`查`命令，追加返回用户主页和直播间链接。    
+
 </details>
 
 ## 致谢
 - [nonebot-plugin-htmlrender](https://github.com/kexue-z/nonebot-plugin-htmlrender) - 图片合成的好手
 - [danmakus.com](https://danmakus.com/) - b站主播、用户弹幕直播信息等来源（开放API接口很赞！）
 - [vtbs.moe](https://vtbs.moe) - VTB本地数据信息来源（还有数据提供，TQL）  
 - [laplace.live](https://laplace.live/) - 也是b站主播用户查询站点，部分数据也是源自danmakus，UI不错
```

#### html2text {}

```diff
@@ -349,17 +349,17 @@
 3.ä¼åè¯´æææ¡£ã ### 1.6.8 ä¿®å¤`lapdd`å½ä»¤ä¸ä¼ åçbugã ###
 1.6.9 æ°å¢æ­£åå¹éç`æè«`ç©æ³ï¼å·ä½çå½ä»¤è¯´æã ### 1.7.0
 ä¿®å¤htmlrenderå¯¼å¥é®é¢ã ### 1.7.1
 æ°å¢å½ä»¤`ehæ¥ç´æ­`æ`è¯¶å¿æ¥ç´æ­`ã ### 1.7.2
 ä¿®æ¹`ehæ¥ç´æ­`çè¯·æ±å°åä¸ºhttpï¼æå¡å¨ä¸è·è¯ä¹¦ä¸è¡ï¼ç»·ã
 ### 1.7.3 ä¿®æ¹`ehæ¥ç´æ­`ä¸ºplaywrightï¼é¾ç»·ã ### 1.7.4
 ä¿®æ¹`ehæ¥ç´æ­`ä¸ºç´æ¥è¯·æ±ï¼ä¸è¿è·³è¿äºsslã ### 1.7.5 bugä¿®å¤
-## è´è°¢ - [nonebot-plugin-htmlrender](https://github.com/kexue-z/nonebot-
-plugin-htmlrender) - å¾çåæçå¥½æ - [danmakus.com](https://
-danmakus.com/) -
+### 1.7.6 `æ¥`å½ä»¤ï¼è¿½å è¿åç¨æ·ä¸»é¡µåç´æ­é´é¾æ¥ã  ##
+è´è°¢ - [nonebot-plugin-htmlrender](https://github.com/kexue-z/nonebot-plugin-
+htmlrender) - å¾çåæçå¥½æ - [danmakus.com](https://danmakus.com/) -
 bç«ä¸»æ­ãç¨æ·å¼¹å¹ç´æ­ä¿¡æ¯ç­æ¥æºï¼å¼æ¾APIæ¥å£å¾èµï¼ï¼ -
 [vtbs.moe](https://vtbs.moe) -
 VTBæ¬å°æ°æ®ä¿¡æ¯æ¥æºï¼è¿ææ°æ®æä¾ï¼TQLï¼ - [laplace.live]
 (https://laplace.live/) -
 ä¹æ¯bç«ä¸»æ­ç¨æ·æ¥è¯¢ç«ç¹ï¼é¨åæ°æ®ä¹æ¯æºèªdanmakusï¼UIä¸é
 ## é¡¹ç®æåä¸ä¼ è³pypi å®ç½ï¼https://
 pypi.orgï¼æ³¨åè´¦å·ï¼å¨ç³»ç»ç¨æ·æ ¹ç®å½ä¸åå»º`.pypirc`ï¼éç½®
```

### Comparing `nonebot_plugin_searchbiliinfo-1.7.5/setup.py` & `nonebot_plugin_searchbiliinfo-1.7.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'asyncio>=3.4.3,<4.0.0',
  'nonebot-adapter-onebot>=2.1.3,<3.0.0',
  'nonebot-plugin-htmlrender>=0.2.0.1,<0.3.0.0',
  'nonebot2>=2.0.0b5,<3.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-searchbiliinfo',
-    'version': '1.7.5',
+    'version': '1.7.6',
     'description': 'A plugin for nonebot2. Query Bilibili user information（一个Nonebot2的插件，b站用户信息查询插件【粉丝、舰团信息；直播收益数据；直播观看信息；关键词搜昵称、UID；主播营收榜单；查成分；查牌子等】）',
-    'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_searchBiliInfo\n  \n_✨ NoneBot b站用户信息查询插件 ✨_\n  \n<a href="https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo/stargazers">\n    <img alt="GitHub stars" src="https://img.shields.io/github/stars/Ikaros-521/nonebot_plugin_searchBiliInfo?color=%09%2300BFFF&style=flat-square">\n</a>\n<a href="https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo/issues">\n    <img alt="GitHub issues" src="https://img.shields.io/github/issues/Ikaros-521/nonebot_plugin_searchBiliInfo?color=Emerald%20green&style=flat-square">\n</a>\n<a href="https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo/network">\n    <img alt="GitHub forks" src="https://img.shields.io/github/forks/Ikaros-521/nonebot_plugin_searchBiliInfo?color=%2300BFFF&style=flat-square">\n</a>\n<a href="./LICENSE">\n    <img src="https://img.shields.io/github/license/Ikaros-521/nonebot_plugin_searchBiliInfo.svg" alt="license">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_searchBiliInfo">\n    <img src="https://img.shields.io/pypi/v/nonebot_plugin_searchBiliInfo.svg" alt="pypi">\n</a>\n<a href="https://www.python.org">\n    <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">\n</a>\n\n</div>\n\n适用于nonebot2 v11的b站用户信息查询插件【粉丝、舰团信息；直播收益数据；直播观看信息；关键词搜昵称、UID；主播营收榜单；查成分；查牌子等】  \n（ps：微调源码可以兼容其他版本）   \n调用的相关API源自b站官方接口、danmakus.com和vtbs.fun\n\n<!-- START doctoc generated TOC please keep comment here to allow auto update -->\n<!-- DON\'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->\n## 📖目录\n\n- [🔧 开发环境](#-%E5%BC%80%E5%8F%91%E7%8E%AF%E5%A2%83)\n- [💿 安装](#-%E5%AE%89%E8%A3%85)\n  - [1. nb-cli安装（推荐）](#1-nb-cli%E5%AE%89%E8%A3%85%E6%8E%A8%E8%8D%90)\n  - [2. 本地安装](#2-%E6%9C%AC%E5%9C%B0%E5%AE%89%E8%A3%85)\n  - [3. pip安装](#3-pip%E5%AE%89%E8%A3%85)\n  - [更新版本](#%E6%9B%B4%E6%96%B0%E7%89%88%E6%9C%AC)\n- [🔧 配置](#-%E9%85%8D%E7%BD%AE)\n  - [cookie获取方式](#cookie%E8%8E%B7%E5%8F%96%E6%96%B9%E5%BC%8F)\n  - [env配置](#env%E9%85%8D%E7%BD%AE)\n- [🎉 功能](#-%E5%8A%9F%E8%83%BD)\n- [👉 命令(命令前缀自行替换喵~)](#-%E5%91%BD%E4%BB%A4%E5%91%BD%E4%BB%A4%E5%89%8D%E7%BC%80%E8%87%AA%E8%A1%8C%E6%9B%BF%E6%8D%A2%E5%96%B5)\n  - [/查](#%E6%9F%A5)\n  - [/查直播](#%E6%9F%A5%E7%9B%B4%E6%92%AD)\n  - [/查舰团](#%E6%9F%A5%E8%88%B0%E5%9B%A2)\n  - [/查昵称](#%E6%9F%A5%E6%98%B5%E7%A7%B0)\n  - [/查收益](#%E6%9F%A5%E6%94%B6%E7%9B%8A)\n  - [/查观看](#%E6%9F%A5%E8%A7%82%E7%9C%8B)\n  - [/查观看2](#%E6%9F%A5%E8%A7%82%E7%9C%8B2)\n  - [/查弹幕](#%E6%9F%A5%E5%BC%B9%E5%B9%95)\n  - [/查弹幕2](#%E6%9F%A5%E5%BC%B9%E5%B9%952)\n  - [/查牌子](#%E6%9F%A5%E7%89%8C%E5%AD%90)\n  - [/查人气](#%E6%9F%A5%E4%BA%BA%E6%B0%94)\n  - [/查装扮](#%E6%9F%A5%E8%A3%85%E6%89%AE)\n  - [/营收](#%E8%90%A5%E6%94%B6)\n  - [/涨粉](#%E6%B6%A8%E7%B2%89)\n  - [/DD风云榜 或 /dd风云榜 或 /风云榜 (寄了)](#dd%E9%A3%8E%E4%BA%91%E6%A6%9C-%E6%88%96-dd%E9%A3%8E%E4%BA%91%E6%A6%9C-%E6%88%96-%E9%A3%8E%E4%BA%91%E6%A6%9C-%E5%AF%84%E4%BA%86)\n  - [/v详情 或 /V详情 或 /v详细 或 /V详细](#v%E8%AF%A6%E6%83%85-%E6%88%96-v%E8%AF%A6%E6%83%85-%E6%88%96-v%E8%AF%A6%E7%BB%86-%E6%88%96-v%E8%AF%A6%E7%BB%86)\n  - [/v直播势 或 /V直播势](#v%E7%9B%B4%E6%92%AD%E5%8A%BF-%E6%88%96-v%E7%9B%B4%E6%92%AD%E5%8A%BF)\n  - [/v急上升 或 /V急上升](#v%E6%80%A5%E4%B8%8A%E5%8D%87-%E6%88%96-v%E6%80%A5%E4%B8%8A%E5%8D%87)\n  - [/v急下降 或 /V急下降](#v%E6%80%A5%E4%B8%8B%E9%99%8D-%E6%88%96-v%E6%80%A5%E4%B8%8B%E9%99%8D)\n  - [/v舰团 或 /V舰团](#v%E8%88%B0%E5%9B%A2-%E6%88%96-v%E8%88%B0%E5%9B%A2)\n  - [/vdd 或 /VDD 或 /VDD风云榜 或 /vdd风云榜](#vdd-%E6%88%96-vdd-%E6%88%96-vdd%E9%A3%8E%E4%BA%91%E6%A6%9C-%E6%88%96-vdd%E9%A3%8E%E4%BA%91%E6%A6%9C)\n  - [/V宏观 或 /v宏观](#v%E5%AE%8F%E8%A7%82-%E6%88%96-v%E5%AE%8F%E8%A7%82)\n  - [/dmk查用户 或 /DMK查用户](#dmk%E6%9F%A5%E7%94%A8%E6%88%B7-%E6%88%96-dmk%E6%9F%A5%E7%94%A8%E6%88%B7)\n  - [/dmk查直播 或 /DMK查直播](#dmk%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-dmk%E6%9F%A5%E7%9B%B4%E6%92%AD)\n  - [/blg查弹幕 或 /BLG查弹幕](#blg%E6%9F%A5%E5%BC%B9%E5%B9%95-%E6%88%96-blg%E6%9F%A5%E5%BC%B9%E5%B9%95)\n  - [/blg查入场 或 /BLG查入场](#blg%E6%9F%A5%E5%85%A5%E5%9C%BA-%E6%88%96-blg%E6%9F%A5%E5%85%A5%E5%9C%BA)\n  - [/blg查礼物 或 /BLG查礼物](#blg%E6%9F%A5%E7%A4%BC%E7%89%A9-%E6%88%96-blg%E6%9F%A5%E7%A4%BC%E7%89%A9)\n  - [/blg直播记录 或 /BLG直播记录](#blg%E7%9B%B4%E6%92%AD%E8%AE%B0%E5%BD%95-%E6%88%96-blg%E7%9B%B4%E6%92%AD%E8%AE%B0%E5%BD%95)\n  - [/blg直播间sc 或 /BLG直播间SC](#blg%E7%9B%B4%E6%92%AD%E9%97%B4sc-%E6%88%96-blg%E7%9B%B4%E6%92%AD%E9%97%B4sc)\n  - [/icu查直播 或 /ICU查直播 或 /matsuri查直播](#icu%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-icu%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-matsuri%E6%9F%A5%E7%9B%B4%E6%92%AD)\n  - [/lap查用户 或 /LAP查用户](#lap%E6%9F%A5%E7%94%A8%E6%88%B7-%E6%88%96-lap%E6%9F%A5%E7%94%A8%E6%88%B7)\n  - [/lap查牌子 或 /LAP查牌子](#lap%E6%9F%A5%E7%89%8C%E5%AD%90-%E6%88%96-lap%E6%9F%A5%E7%89%8C%E5%AD%90)\n  - [/lap查充电 或 /LAP查充电](#lap%E6%9F%A5%E5%85%85%E7%94%B5-%E6%88%96-lap%E6%9F%A5%E5%85%85%E7%94%B5)\n  - [/lapdd 或 /LAPDD 或 /lapdd排行榜](#lapdd-%E6%88%96-lapdd-%E6%88%96-lapdd%E6%8E%92%E8%A1%8C%E6%A6%9C)\n  - [/zero查用户 或 /ZERO查用户](#zero%E6%9F%A5%E7%94%A8%E6%88%B7-%E6%88%96-zero%E6%9F%A5%E7%94%A8%E6%88%B7)\n  - [/zero被关注 或 /ZERO被关注](#zero%E8%A2%AB%E5%85%B3%E6%B3%A8-%E6%88%96-zero%E8%A2%AB%E5%85%B3%E6%B3%A8)\n  - [斗虫 或 主播pk 或 主播PK](#%E6%96%97%E8%99%AB-%E6%88%96-%E4%B8%BB%E6%92%ADpk-%E6%88%96-%E4%B8%BB%E6%92%ADpk)\n  - [eh查直播 或 诶嘿查直播 或 eihei查直播](#eh%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-%E8%AF%B6%E5%98%BF%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-eihei%E6%9F%A5%E7%9B%B4%E6%92%AD)\n  - [/vtb网站](#vtb%E7%BD%91%E7%AB%99)\n- [⚙ 拓展](#-%E6%8B%93%E5%B1%95)\n- [📝 更新日志](#-%E6%9B%B4%E6%96%B0%E6%97%A5%E5%BF%97)\n- [致谢](#%E8%87%B4%E8%B0%A2)\n- [项目打包上传至pypi](#%E9%A1%B9%E7%9B%AE%E6%89%93%E5%8C%85%E4%B8%8A%E4%BC%A0%E8%87%B3pypi)\n  - [poetry](#poetry)\n  - [twine](#twine)\n- [目录自动生成](#%E7%9B%AE%E5%BD%95%E8%87%AA%E5%8A%A8%E7%94%9F%E6%88%90)\n  - [安装](#%E5%AE%89%E8%A3%85)\n  - [使用](#%E4%BD%BF%E7%94%A8)\n\n<!-- END doctoc generated TOC please keep comment here to allow auto update -->\n\n## 🔧 开发环境\nNonebot2：2.0.0b5  \npython：3.8.13  \n操作系统：Windows10（CentOS7下正常运行，Linux兼容性问题不大）  \n编辑器：pycharm  \n\n## 💿 安装\n环境依赖`aiohttp`和`nonebot_plugin_htmlrender`库   \n部分功能需要获取自己的cookie，配置env后才能正常使用！  \n\n### 1. nb-cli安装（推荐）\n在你bot工程的文件夹下，运行cmd（运行路径要对啊），执行nb命令安装插件，插件配置会自动添加至配置文件  \n```\nnb plugin install nonebot_plugin_searchBiliInfo\n```\n\n### 2. 本地安装\n先安装下 `aiohttp` 和 `htmlrender`  \n```\npip install aiohttp\npip install nonebot_plugin_htmlrender\n```\n将项目clone到你的机器人插件下的对应插件目录内（一般为机器人文件夹下的`src/plugins`），然后把`nonebot_plugin_searchBiliInfo`文件夹里的内容拷贝至上一级目录即可。  \nclone命令参考（得先装`git`，懂的都懂）：\n```\ngit clone https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo.git\n``` \n也可以直接下载压缩包到插件目录解压，然后同样提取`nonebot_plugin_searchBiliInfo`至上一级目录。  \n目录结构： ```你的bot/src/plugins/nonebot_plugin_searchBiliInfo/__init__.py```  \n\n\n### 3. pip安装\n```\npip install nonebot_plugin_searchBiliInfo\n```  \n打开 nonebot2 项目的 ```bot.py``` 文件, 在其中写入  \n```nonebot.load_plugin(\'nonebot_plugin_searchBiliInfo\')```  \n当然，如果是默认nb-cli创建的nonebot2的话，在bot路径```pyproject.toml```的```[tool.nonebot]```的```plugins```中添加```nonebot_plugin_searchBiliInfo```即可  \npyproject.toml配置例如：  \n``` \n[tool.nonebot]\nplugin_dirs = ["src/plugins"]\nplugins = ["nonebot_plugin_searchBiliInfo"]\n``` \n\n### 更新版本\n```\nnb plugin update nonebot_plugin_searchBiliInfo\n```\n\n## 🔧 配置\n\n### cookie获取方式\n浏览器进入b站官网并登录: `https://www.bilibili.com/`  \nedge（或其他浏览器）按`f12`（或鼠标右键`“检查”` `“开发者工具”`等）, 然后点击右上角那个`">>"`符号, 进入`"网络"`  \n再按`ctrl+r`（或`f5`）刷新元素  \n随便点击一个请求, 在`“请求标头”`里面找到cookie（没有就换一个）  \ncookie冒号后面的就是cookie，复制一下, 可以把ta添加到env里  \n如果不想放太多cookie信息，只需要`buvid3`字段即可。  \n\n### env配置\n```\n# 在你的env文件中添加如下配置（我的是.env.prod） 仅需要buvid3字段即可\nsearchBiliInfo_cookie="buvid3=XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXXXXXXXinfoc;"\n```\n|       配置项        | 必填 | 默认值  |                      说明                      |\n|:----------------:|:----:|:----:|:----------------------------:|\n| `searchBiliInfo_cookie` | 否 | `""` | b站cookie，仅需要`buvid3`字段即可 |\n\n\n## 🎉 功能\n通过uid 或 设定好的短语 或 b站接口搜索查询指定b站用户的粉丝、舰团信息；直播收益数据；直播观看信息；关键词搜昵称、UID等信息；主播营收榜单。\n\n## 👉 命令(命令前缀自行替换喵~)\n\n### /查\n命令结构：```/查 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/查 uid:3709626``` 或 ```/查 :3709626``` 或 ```/查 bishi```  \nbot返回内容：  \n![](docs/search.png)\n\n### /查直播\n命令结构：```/查直播 (uid:或UID:或：或:)+用户uid或昵称关键词 场次数（默认不写为全部）```  \n例如：```/查直播 UID:3709626 1``` 或 ```/查直播 bishi```  \nbot返回内容（图片）：  \n![](docs/live_info.png)\n\n### /查舰团\n命令结构：```/查舰团 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/查舰团 ：3709626``` 或 ```/查舰团 bishi```  \nbot返回内容(图片)：  \n![](docs/guard.png)\n\n### /查昵称\n命令结构：```/查昵称 昵称关键词```  \n例如：```/查昵称 伊卡洛斯```\nbot返回内容(图片)：  \n![](docs/search_name.png)\n\n### /查收益\n命令结构：```/查收益 (uid:或UID:或：或:)+用户uid或昵称关键词 收益类型(默认1: 礼物，2: 上舰，3: SC) 倒叙第n场(从0开始)```  \n例如：```/查收益 :3709626 礼物 1``` 或 ```/查收益 bishi 2 0```  \nbot返回内容(图片)：  \n![](docs/income.png)\n\n### /查观看\n命令结构：```/查观看 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/查观看 UID:666666``` 或 ```/查观看 bishi```  \nbot返回内容(图片)：  \n![](docs/watch.png)\n\n### /查观看2\n命令结构：```/查观看2 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/查观看2 UID:666666``` 或 ```/查观看2 bishi```  \nbot返回内容(图片)：  \n![](docs/watch2.png)\n\n### /查弹幕\n命令结构：```/查弹幕 (uid:或UID:或：或:)+用户uid或昵称关键词 查询的主播昵称关键词或(uid:或UID:或：或:)+ 页数(可不填，默认0) 条数(可不填，默认3)```  \n例如：```/查弹幕 uid:3709626 Love丶伊卡洛斯 1 1``` 或 ```/查弹幕 uid:3709626 Love丶伊卡洛斯 1```   \nbot返回内容(图片)：  \n![](docs/danmu.png)\n\n### /查弹幕2\n命令结构：```/查弹幕2 (uid:或UID:或：或:)+用户uid或昵称关键词 页数(可不填，默认0) 条数(可不填，默认3)```  \n例如：```/查弹幕2 uid:3709626 2 2``` 或 ```/查弹幕2 uid:3709626 2```   \nbot返回内容(图片)：  \n![](docs/danmu2.png)\n\n### /查牌子\n命令结构：```/查牌子 主播牌子关键词```  \n例如：```/查牌子 天``` 或 ```/查牌子 天降```  \nbot返回内容(图片)：  \n![](docs/medal.png)\n\n### /查人气\n命令结构：```/查人气 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/查人气 uid:3709626``` 或 ```/查人气 Love丶伊卡洛斯```   \nbot返回内容(图片)：  \n![](docs/popularity.png)\n\n### /查装扮\n命令结构：```/查装扮 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/查装扮 uid:2``` 或 ```/查装扮 ：2```   \nbot返回内容(图片)：  \n![](docs/garb.png)\n\n### /营收\n命令结构：```/营收 日/周/月榜 人数（不填默认100）```  \n例如：```/营收 日榜 3``` 或 ```/营收 月榜```  \nbot返回内容(图片)：  \n![](docs/revenue.png)\n\n### /涨粉\n命令结构：```/涨粉 日/周/月榜 人数（不填默认100）```  \n例如：```/涨粉 日榜 3``` 或 ```/涨粉 月榜```  \nbot返回内容(图片)：  \n![](docs/incfans.png)\n\n### /DD风云榜 或 /dd风云榜 或 /风云榜 (寄了)\n命令结构：```/DD风云榜 top人数（不填默认10）```  \n例如：```/DD风云榜``` 或 ```/风云榜 20```  \nbot返回内容(图片)：  \n![](docs/ddstats.png)\n\n### /v详情 或 /V详情 或 /v详细 或 /V详细\n命令结构：```/v详情 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/v详情 uid:3709626``` 或 ```/V详情 ：2``` 或 ```/v详细 Love丶伊卡洛斯``` 或 ```/V详细 :2```    \nbot返回内容(图片)：  \n![](docs/v_detail.png)\n\n### /v直播势 或 /V直播势\n命令结构：```/v直播势```  \n例如：```/v直播势``` 或 ```/V直播势```  \nbot返回内容(图片)：  \n![](docs/v_live.png)\n\n### /v急上升 或 /V急上升\n命令结构：```/v急上升```  \n例如：```/v急上升``` 或 ```/V急上升```  \nbot返回内容(图片)：  \n![](docs/v_rise.png)\n\n### /v急下降 或 /V急下降\n命令结构：```/v急下降```  \n例如：```/v急下降``` 或 ```/V急下降```  \nbot返回内容(图片)：  \n![](docs/v_drop.png)\n\n### /v舰团 或 /V舰团\n命令结构：```/v舰团```  \n例如：```/v舰团``` 或 ```/V舰团```  \nbot返回内容(图片)：  \n![](docs/v_guard.png)\n\n### /vdd 或 /VDD 或 /VDD风云榜 或 /vdd风云榜\n命令结构：```/vdd```  \n例如：```/vdd``` 或 ```/VDD```  或 ```/vdd风云榜```   \nbot返回内容(图片)：  \n![](docs/v_dd.png)\n\n### /V宏观 或 /v宏观\n命令结构：```/vdd```  \n例如：```/V宏观``` 或 ```/v宏观```   \nbot返回内容(图片)：  \n![](docs/v_macro.png)\n\n### /dmk查用户 或 /DMK查用户\n命令结构：```/dmk查用户 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/dmk查用户 uid:3709626``` 或 ```/DMK查用户 Love丶伊卡洛斯```  \nbot返回内容(图片)：  \n![](docs/dmk_user.png)\n\n### /dmk查直播 或 /DMK查直播\n命令结构：```/dmk查直播 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/dmk查直播 uid:3709626``` 或 ```/DMK查直播 Love丶伊卡洛斯```  \nbot返回内容(图片)：  \n![](docs/dmk_live.png)\n\n### /blg查弹幕 或 /BLG查弹幕\n命令结构：```/blg查弹幕 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/blg查弹幕 uid:3709626``` 或 ```/BLG查弹幕 Love丶伊卡洛斯```  \nbot返回内容(图片)：  \n![](docs/blg_danmu.png)\n\n### /blg查入场 或 /BLG查入场\n命令结构：```/blg查入场 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/blg查入场 uid:3709626``` 或 ```/BLG查入场 Love丶伊卡洛斯```  \nbot返回内容(图片)：  \n![](docs/blg_enter.png)\n\n### /blg查礼物 或 /BLG查礼物\n命令结构：```/blg查礼物 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/blg查礼物 uid:3709626``` 或 ```/BLG查礼物 Love丶伊卡洛斯```  \nbot返回内容(图片)：  \n![](docs/blg_gift.png)\n\n### /blg直播记录 或 /BLG直播记录\n命令结构：```/blg直播记录 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/blg直播记录 uid:3709626``` 或 ```/BLG直播记录 Love丶伊卡洛斯```  \nbot返回内容(图片)：  \n![](docs/blg_tp.png)\n\n### /blg直播间sc 或 /BLG直播间SC\n命令结构：```/blg直播间sc (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/blg直播间sc uid:3709626``` 或 ```/BLG直播间SC Love丶伊卡洛斯```  \nbot返回内容(图片)：  \n![](docs/blg_sc.png)\n\n### /icu查直播 或 /ICU查直播 或 /matsuri查直播\n命令结构：```/icu查直播 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/icu查直播 uid:3709626``` 或 ```/ICU查直播 Love丶伊卡洛斯```  \nbot返回内容(图片)：  \n![](docs/icu_live.png)\n\n### /lap查用户 或 /LAP查用户\n命令结构：```/lap查用户 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/lap查用户 uid:387636363``` 或 ```/LAP查用户 雫るる```  \nbot返回内容(图片)：  \n![](docs/laplace_user.png)\n\n### /lap查牌子 或 /LAP查牌子\n命令结构：```/lap查牌子 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/lap查牌子 uid:387636363``` 或 ```/LAP查牌子 雫るる```  \nbot返回内容(图片)：  \n![](docs/laplace_medal.png)\n\n### /lap查充电 或 /LAP查充电\n命令结构：```/lap查充电 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/lap查充电 uid:387636363``` 或 ```/LAP查充电 雫るる```  \nbot返回内容(图片)：  \n![](docs/laplace_upower.png)\n\n### /lapdd 或 /LAPDD 或 /lapdd排行榜\n命令结构：```/lapdd 搜索类型(默认0: 月供，1: 总督，2: 提督，3：舰长)```  \n例如：```/lapdd``` 或 ```/lapdd 1``` 或 ```/LAPDD 舰长```  \nbot返回内容(图片)：  \n![](docs/laplace_dd.png)\n\n### /zero查用户 或 /ZERO查用户\n命令结构：```/zero查用户 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/zero查用户 uid:387636363``` 或 ```/ZERO查用户 雫るる```  \nbot返回内容(图片)：  \n![](docs/zeroroku_author.png)\n\n### /zero被关注 或 /ZERO被关注\n命令结构：```/zero被关注 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/zero被关注 uid:387636363``` 或 ```/ZERO被关注 雫るる```  \nbot返回内容(图片)：  \n![](docs/zeroroku_famous_fans.png)\n\n### 斗虫 或 主播pk 或 主播PK\n命令结构：`斗虫|主播pk|主播PK 用户1的uid或昵称关键词 用户2的uid或昵称关键词 用户n的uid或昵称关键词 #当天向过去偏移天(起始) 当天向过去偏移天数(结尾)`\n注意：`#`和后面的`日期偏移`可以默认不填，不填写的话默认是一个月前到今天的数据。另外，传入的用户必须大于等于2人以上。（`日期偏移`其实就是`数据区间`啦）\n例如：```斗虫 雫酱 neol``` 或 ```斗虫 雫酱 neol #5 0``` 或 ```主播pk 雫酱 雫 #15 0```    \nbot返回内容(图片)：  \n![](docs/stats_nailv_live_compare.png)\n\n\n### eh查直播 或 诶嘿查直播 或 eihei查直播\n命令结构：```/eh查直播 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/诶嘿查直播 uid:3493132603754688``` 或 ```/诶嘿查直播 罗亚Roya```  \nbot返回内容(图片)：  \n![](docs/eihei_livepic.png)\n\n### /vtb网站\n命令结构：```/vtb网站``` 或 ```/vtb资源```  \n例如：```/vtb网站``` 或 ```/vtb资源```  \nbot返回内容：  \n```\nVTB数据看板：https://ikaros-521.gitee.io/vtb_data_board/\nmatsuri：https://matsuri.icu/\ndanmakus：https://danmakus.com/\nvtbs.fun：http://www.vtbs.fun/\nbiligank：https://biligank.com/\n火龙榜：https://huolonglive.com/#/\nvtbs.moe：https://vtbs.moe/\nvup.loveava.top：https://vup.loveava.top/ranking\nddstats：https://ddstats.ericlamm.xyz/\nzeroroku：https://zeroroku.com/bilibili\nlaplace：https://laplace.live/\n```\n\n## ⚙ 拓展\n启用关键词搜索，需要在`.env.xx`中配置自己的`cookie`。\n\n命令修改：  \n昵称自定义，修改`data.py`，在文件头部追加你需要定义的用户的json串，注意json格式！！！  \n命令自定义，修改`__init__.py`，`catch_str = on_command`这部分的代码即可。  \n\nbot返回内容格式修改对应的msg、out_str变量的内容  \n\n## 📝 更新日志\n\n<details>\n<summary>展开/收起</summary>\n\n### 0.0.1\n\n- 插件初次发布\n\n### 0.1.0\n\n- 更新基于vtbs.moe的主播数据，添加关键词搜索功能\n\n### 1.0.0\n\n新增以下功能（其实是LX_Bot的相关命令融进来了）\n- /查 昵称关键词\n- /查直播 昵称关键词 场次数\n- /查舰团 昵称关键词\n- /查昵称 昵称关键词\n- /查收益 收益类型(默认1: 礼物，2: 上舰，3: SC) 用户uid或昵称关键词 倒叙第n场(从0开始)\n- /查成分 观看 昵称关键词\n- /查成分 弹幕 查询的目标人 查询的主播 页数 条数\n\n### 1.0.4\n\n优化针对uid解析方式\n\n### 1.0.5\n\n修改cookie配置从env获取，方便用户配置\n\n### 1.0.6\n\n修复 /查成分 弹幕 数据解析bug；\n优化整体代码实现；\n\n### 1.1.0\n新增功能\n- /营收 日/周/月榜 人数（不填默认100）\n\n### 1.2.0\n弃用requests库，改为aiohttp  \n\n### 1.2.1\n修复查命令aiohttp适配性bug  \n\n### 1.3.0\n修改 查成分 弹幕 和 查成分 观看 命令为 查弹幕 和 查观看。  \n优化命令解析实现。  \n修复查弹幕数据解析bug。  \n\n### 1.3.1\n新增 /查弹幕2 命令。  \n修复查弹幕数据解析bug。 \n图片UI优化。  \n\n### 1.3.2\n优化 /查弹幕2 命令，增加主播名。  \n\n### 1.3.3\n修复 /查观看 因为数据源有同一用户名不同uid的情况导致的越界bug。  \n\n### 1.3.4\n优化异常报错的处理。  \n优化UI设计和部分功能。  \n\n### 1.3.5\n新增`/查收益 xx 舰长`和`uid：`的匹配。（但是舰长仍然是所有上舰数据）    \n\n### 1.3.6\n优化API挂彩时候的异常捕获处理。  \n\n### 1.3.7\n插件补充元信息。 \n\n### 1.3.8\n新增`vtb网站` 或 `vtb资源` 命令（命令前缀自行添加） \n\n### 1.3.9\n补充2个VTB资源站点  \n\n### 1.3.10\n适配vtbs.fun的营收接口变动  \n\n### 1.4.0\n修改on_keyword为on_command，从而适配自定义的命令前缀  \n\n### 1.4.1\n修改danmakus.com到新域名danmakus.com，接口也同步替换了。  \n\n### 1.4.2\n新增markdown的特殊字符过滤和文本超长换行。  \nps：vtbs.fun挂了，`营收`功能暂时无法使用。\n\n### 1.4.3\nvtbs.fun活了，加了ssl，已兼容。  \n\n### 1.4.4\n新增命令 涨粉，接口源自vtbs.fun（和营收 基本一致）  \n\n### 1.4.5\n新增命令 DD风云榜，接口源自ddstats-api.ericlamm.xyz  \n\n### 1.4.6\n补充遗漏的插件元信息    \n\n### 1.4.7\n新增功能 查牌子，数据源自本地爬取（vtbs.moe中主播牌子信息，共4273条数据）   \n\n### 1.4.8\n补充插牌子遗漏的1条数据   \n\n### 1.4.9\n补充遗漏的 vtb网站 功能元信息   \n\n### 1.4.10\n新增功能`v详情` `dmk查用户` `dmk查直播`，直接采用浏览器页面截图形式返回结果。（流量消耗会多一些，酌情使用）     \n\n### 1.4.11\n延长`v详情` `dmk查用户` `dmk查直播`的请求超时至5min（服务器4M跑也超时，功能很吃紧）  \n\n### 1.4.12\n追加最新的vtbs.moe的主播信息，并同步更新了牌子信息。  \n缩短`v详情` `dmk查用户` `dmk查直播`的请求超时至2min（前面是对面服务器炸了）  \n\n### 1.4.13\n优化请求错误或无数据时的消息返回和日志打印。  \n\n### 1.5.0\n新增功能`blg查弹幕` `blg查入场` `blg查礼物` `blg直播记录` `blg直播间sc`，直接采用浏览器页面截图形式返回结果。（流量消耗会多一些，酌情使用）     \n\n### 1.5.1\n新增4000+的用户数据和牌子数据  \n\n### 1.5.2\n新增b站用户数据至10w  \n新增粉丝牌数据至4w+  \n\n### 1.5.3\n新增网站laplace.live  \n新增`icu查直播`命令，同样是playwright的直接加载  \n\n### 1.5.4\n新用户数据爬自b站直播间各大分区列表，比起直接uid爬全站更具有针对性，实际效果也很好。  \n新增b站用户数据至23w+  \n新增粉丝牌数据至6.7w+  \n\n### 1.5.5\n由于出现低配置设备内存不足导致的无法启动问题，已将本地数据`data.py`清空至一个demo配置。如有本地配置需要的可以去旧版获取。  \n\n### 1.5.6\n新增粉丝牌数据至8.6w+，爬了一周的直播页，正式收工。  \n\n### 1.5.7\n新增命令`查人气`，用于查询b站主播最近一场直播的人气峰值  \n\n### 1.5.8\n新增`lap查用户`命令，同样是playwright，并做了js内嵌  \n\n### 1.5.9\n优化`lap查用户`的内容加载样式，显示内容更加全面（也更卡，乐）  \n\n### 1.5.10\n增加耗时的网页截图查询反馈，优化异常处理，不让你的人生浪费在等待中  \n\n### 1.5.11\n新增`zero查用户`命令，同理  \n\n### 1.5.12\n修复文档描述错误（不影响功能，暂不发版）  \n文档新增目录    \n\n### 1.5.13\n新增`lap查牌子`命令，调用laplace.live的接口，全站太卡了，绷  \n\n### 1.5.14\n修复`lap查牌子`接口返回uid固定问题导致的显示错误  \n优化文档  \n\n### 1.5.15\n升级`查观看`功能，统计观看次数。  \n\n### 1.5.16\n新增`查观看2`命令（查观看plus版），统计观看次数，以饼图形式返回。  \n\n### 1.5.17\n优化网页截图相关功能的图片存储名，减少短时间多请求导致的数据覆盖问题  \n修复`查观看2`的提示语延迟问题  \n修订文档错误  \n\n### 1.5.18\n新增`lap查充电`命令，查询up的充电排行榜。  \n新增`zero被关注`命令，查询用户的被哪些知名up主关注。  \n升级`查观看2`的主题为夜间模式，增加高级感。  \n\n### 1.6.0\n对类似的GET请求做了优化，降低代码冗余。  \n\n### 1.6.1\n删除`lap查用户`的小作文  \n\n### 1.6.2\n1、新增以下命令：  \n- /v直播势  （大写也可以）\n- /v急上升  （大写也可以）\n- /v急下降  （大写也可以）\n- /v舰团  （大写也可以）\n- /vdd  （大写也可以）\n- /v宏观  （大写也可以）  \n2、优化异常处理\n\n### 1.6.3\n优化`v详情`的请求延时，帮助数据加载。  \n\n### 1.6.4\n新增`查装扮`命令。  \n优化文档排序。 \n\n### 1.6.5\n1.`v详情`增加别名`v详细`。  \n2.修复`查收益`的传参bug。  \n3.优化代码实现，增加提示互动。  \n\n### 1.6.6\n1.修复`查弹幕`和`查弹幕2`的bug（让GPT帮忙写，很好，bug写得不错）  \n\n### 1.6.7\n1.命令文本消息内容改艾特为回复。  \n2.新增命令`lapdd`或`lapdd排行榜`，截图laplace.live的dd页面。  \n3.优化说明文档。  \n\n### 1.6.8\n修复`lapdd`命令不传参的bug。  \n\n### 1.6.9\n新增正则匹配的`斗虫`玩法，具体看命令说明。  \n\n### 1.7.0\n修复htmlrender导入问题。  \n\n### 1.7.1\n新增命令`eh查直播`或`诶嘿查直播`。  \n\n### 1.7.2\n修改`eh查直播`的请求地址为http，服务器上跑证书不行，绷。  \n\n### 1.7.3\n修改`eh查直播`为playwright，难绷。  \n\n### 1.7.4\n修改`eh查直播`为直接请求，不过跳过了ssl。  \n\n### 1.7.5\nbug修复  \n\n</details>\n\n## 致谢\n- [nonebot-plugin-htmlrender](https://github.com/kexue-z/nonebot-plugin-htmlrender) - 图片合成的好手\n- [danmakus.com](https://danmakus.com/) - b站主播、用户弹幕直播信息等来源（开放API接口很赞！）\n- [vtbs.moe](https://vtbs.moe) - VTB本地数据信息来源（还有数据提供，TQL）  \n- [laplace.live](https://laplace.live/) - 也是b站主播用户查询站点，部分数据也是源自danmakus，UI不错  \n\n## 项目打包上传至pypi\n\n官网：https://pypi.org，注册账号，在系统用户根目录下创建`.pypirc`，配置  \n``` \n[distutils] \nindex-servers=pypi \n \n[pypi] repository = https://upload.pypi.org/legacy/ \nusername = 用户名 \npassword = 密码\n```\n\n### poetry\n\n```\n# 参考 https://www.freesion.com/article/58051228882/\n\n# 1、安装poetry\npip install poetry\n\n# 2、初始化配置文件（根据提示填写）\npoetry init\n\n# 3、微调配置文件pyproject.toml\n\n# 4、运行 poetry install, 可生成 “poetry.lock” 文件（可跳过）\npoetry install\n\n# 5、编译，生成dist\npoetry build\n\n# 6、发布\npoetry publish\n\n```\n\n### twine\n\n```\n# 参考 https://www.cnblogs.com/danhuai/p/14915042.html\n#创建setup.py文件 填写相关信息\n\n# 1、可以先升级打包工具\npip install --upgrade setuptools wheel twine\n\n# 2、打包\npython setup.py sdist bdist_wheel\n\n# 3、可以先检查一下包\ntwine check dist/*\n\n# 4、上传包到pypi（需输入用户名、密码）\ntwine upload dist/*\n```\n\n## 目录自动生成\n\n[doctoc](https://github.com/thlorenz/doctoc),在本地git存储库中生成降价文件的目录。链接通过命令行标志兼容github或其他网站生成的锚。\n\n### 安装\n进入包含本地git项目的目录，键入: `npm install -g doctoc`  \n\n### 使用\n在`README.md`中，找个生成目录位置，写入如下代码，确认生成位置：\n```\n<!-- START doctoc -->\n<!-- END doctoc -->\n```\ncmd输入命令即可：`doctoc /path/to/file`  \n例如：`doctoc README.md`  \n\n',
+    'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_searchBiliInfo\n  \n_✨ NoneBot b站用户信息查询插件 ✨_\n  \n<a href="https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo/stargazers">\n    <img alt="GitHub stars" src="https://img.shields.io/github/stars/Ikaros-521/nonebot_plugin_searchBiliInfo?color=%09%2300BFFF&style=flat-square">\n</a>\n<a href="https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo/issues">\n    <img alt="GitHub issues" src="https://img.shields.io/github/issues/Ikaros-521/nonebot_plugin_searchBiliInfo?color=Emerald%20green&style=flat-square">\n</a>\n<a href="https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo/network">\n    <img alt="GitHub forks" src="https://img.shields.io/github/forks/Ikaros-521/nonebot_plugin_searchBiliInfo?color=%2300BFFF&style=flat-square">\n</a>\n<a href="./LICENSE">\n    <img src="https://img.shields.io/github/license/Ikaros-521/nonebot_plugin_searchBiliInfo.svg" alt="license">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_searchBiliInfo">\n    <img src="https://img.shields.io/pypi/v/nonebot_plugin_searchBiliInfo.svg" alt="pypi">\n</a>\n<a href="https://www.python.org">\n    <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">\n</a>\n\n</div>\n\n适用于nonebot2 v11的b站用户信息查询插件【粉丝、舰团信息；直播收益数据；直播观看信息；关键词搜昵称、UID；主播营收榜单；查成分；查牌子等】  \n（ps：微调源码可以兼容其他版本）   \n调用的相关API源自b站官方接口、danmakus.com和vtbs.fun\n\n<!-- START doctoc generated TOC please keep comment here to allow auto update -->\n<!-- DON\'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->\n## 📖目录\n\n- [🔧 开发环境](#-%E5%BC%80%E5%8F%91%E7%8E%AF%E5%A2%83)\n- [💿 安装](#-%E5%AE%89%E8%A3%85)\n  - [1. nb-cli安装（推荐）](#1-nb-cli%E5%AE%89%E8%A3%85%E6%8E%A8%E8%8D%90)\n  - [2. 本地安装](#2-%E6%9C%AC%E5%9C%B0%E5%AE%89%E8%A3%85)\n  - [3. pip安装](#3-pip%E5%AE%89%E8%A3%85)\n  - [更新版本](#%E6%9B%B4%E6%96%B0%E7%89%88%E6%9C%AC)\n- [🔧 配置](#-%E9%85%8D%E7%BD%AE)\n  - [cookie获取方式](#cookie%E8%8E%B7%E5%8F%96%E6%96%B9%E5%BC%8F)\n  - [env配置](#env%E9%85%8D%E7%BD%AE)\n- [🎉 功能](#-%E5%8A%9F%E8%83%BD)\n- [👉 命令(命令前缀自行替换喵~)](#-%E5%91%BD%E4%BB%A4%E5%91%BD%E4%BB%A4%E5%89%8D%E7%BC%80%E8%87%AA%E8%A1%8C%E6%9B%BF%E6%8D%A2%E5%96%B5)\n  - [/查](#%E6%9F%A5)\n  - [/查直播](#%E6%9F%A5%E7%9B%B4%E6%92%AD)\n  - [/查舰团](#%E6%9F%A5%E8%88%B0%E5%9B%A2)\n  - [/查昵称](#%E6%9F%A5%E6%98%B5%E7%A7%B0)\n  - [/查收益](#%E6%9F%A5%E6%94%B6%E7%9B%8A)\n  - [/查观看](#%E6%9F%A5%E8%A7%82%E7%9C%8B)\n  - [/查观看2](#%E6%9F%A5%E8%A7%82%E7%9C%8B2)\n  - [/查弹幕](#%E6%9F%A5%E5%BC%B9%E5%B9%95)\n  - [/查弹幕2](#%E6%9F%A5%E5%BC%B9%E5%B9%952)\n  - [/查牌子](#%E6%9F%A5%E7%89%8C%E5%AD%90)\n  - [/查人气](#%E6%9F%A5%E4%BA%BA%E6%B0%94)\n  - [/查装扮](#%E6%9F%A5%E8%A3%85%E6%89%AE)\n  - [/营收](#%E8%90%A5%E6%94%B6)\n  - [/涨粉](#%E6%B6%A8%E7%B2%89)\n  - [/DD风云榜 或 /dd风云榜 或 /风云榜 (寄了)](#dd%E9%A3%8E%E4%BA%91%E6%A6%9C-%E6%88%96-dd%E9%A3%8E%E4%BA%91%E6%A6%9C-%E6%88%96-%E9%A3%8E%E4%BA%91%E6%A6%9C-%E5%AF%84%E4%BA%86)\n  - [/v详情 或 /V详情 或 /v详细 或 /V详细](#v%E8%AF%A6%E6%83%85-%E6%88%96-v%E8%AF%A6%E6%83%85-%E6%88%96-v%E8%AF%A6%E7%BB%86-%E6%88%96-v%E8%AF%A6%E7%BB%86)\n  - [/v直播势 或 /V直播势](#v%E7%9B%B4%E6%92%AD%E5%8A%BF-%E6%88%96-v%E7%9B%B4%E6%92%AD%E5%8A%BF)\n  - [/v急上升 或 /V急上升](#v%E6%80%A5%E4%B8%8A%E5%8D%87-%E6%88%96-v%E6%80%A5%E4%B8%8A%E5%8D%87)\n  - [/v急下降 或 /V急下降](#v%E6%80%A5%E4%B8%8B%E9%99%8D-%E6%88%96-v%E6%80%A5%E4%B8%8B%E9%99%8D)\n  - [/v舰团 或 /V舰团](#v%E8%88%B0%E5%9B%A2-%E6%88%96-v%E8%88%B0%E5%9B%A2)\n  - [/vdd 或 /VDD 或 /VDD风云榜 或 /vdd风云榜](#vdd-%E6%88%96-vdd-%E6%88%96-vdd%E9%A3%8E%E4%BA%91%E6%A6%9C-%E6%88%96-vdd%E9%A3%8E%E4%BA%91%E6%A6%9C)\n  - [/V宏观 或 /v宏观](#v%E5%AE%8F%E8%A7%82-%E6%88%96-v%E5%AE%8F%E8%A7%82)\n  - [/dmk查用户 或 /DMK查用户](#dmk%E6%9F%A5%E7%94%A8%E6%88%B7-%E6%88%96-dmk%E6%9F%A5%E7%94%A8%E6%88%B7)\n  - [/dmk查直播 或 /DMK查直播](#dmk%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-dmk%E6%9F%A5%E7%9B%B4%E6%92%AD)\n  - [/blg查弹幕 或 /BLG查弹幕](#blg%E6%9F%A5%E5%BC%B9%E5%B9%95-%E6%88%96-blg%E6%9F%A5%E5%BC%B9%E5%B9%95)\n  - [/blg查入场 或 /BLG查入场](#blg%E6%9F%A5%E5%85%A5%E5%9C%BA-%E6%88%96-blg%E6%9F%A5%E5%85%A5%E5%9C%BA)\n  - [/blg查礼物 或 /BLG查礼物](#blg%E6%9F%A5%E7%A4%BC%E7%89%A9-%E6%88%96-blg%E6%9F%A5%E7%A4%BC%E7%89%A9)\n  - [/blg直播记录 或 /BLG直播记录](#blg%E7%9B%B4%E6%92%AD%E8%AE%B0%E5%BD%95-%E6%88%96-blg%E7%9B%B4%E6%92%AD%E8%AE%B0%E5%BD%95)\n  - [/blg直播间sc 或 /BLG直播间SC](#blg%E7%9B%B4%E6%92%AD%E9%97%B4sc-%E6%88%96-blg%E7%9B%B4%E6%92%AD%E9%97%B4sc)\n  - [/icu查直播 或 /ICU查直播 或 /matsuri查直播](#icu%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-icu%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-matsuri%E6%9F%A5%E7%9B%B4%E6%92%AD)\n  - [/lap查用户 或 /LAP查用户](#lap%E6%9F%A5%E7%94%A8%E6%88%B7-%E6%88%96-lap%E6%9F%A5%E7%94%A8%E6%88%B7)\n  - [/lap查牌子 或 /LAP查牌子](#lap%E6%9F%A5%E7%89%8C%E5%AD%90-%E6%88%96-lap%E6%9F%A5%E7%89%8C%E5%AD%90)\n  - [/lap查充电 或 /LAP查充电](#lap%E6%9F%A5%E5%85%85%E7%94%B5-%E6%88%96-lap%E6%9F%A5%E5%85%85%E7%94%B5)\n  - [/lapdd 或 /LAPDD 或 /lapdd排行榜](#lapdd-%E6%88%96-lapdd-%E6%88%96-lapdd%E6%8E%92%E8%A1%8C%E6%A6%9C)\n  - [/zero查用户 或 /ZERO查用户](#zero%E6%9F%A5%E7%94%A8%E6%88%B7-%E6%88%96-zero%E6%9F%A5%E7%94%A8%E6%88%B7)\n  - [/zero被关注 或 /ZERO被关注](#zero%E8%A2%AB%E5%85%B3%E6%B3%A8-%E6%88%96-zero%E8%A2%AB%E5%85%B3%E6%B3%A8)\n  - [斗虫 或 主播pk 或 主播PK](#%E6%96%97%E8%99%AB-%E6%88%96-%E4%B8%BB%E6%92%ADpk-%E6%88%96-%E4%B8%BB%E6%92%ADpk)\n  - [eh查直播 或 诶嘿查直播 或 eihei查直播](#eh%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-%E8%AF%B6%E5%98%BF%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-eihei%E6%9F%A5%E7%9B%B4%E6%92%AD)\n  - [/vtb网站](#vtb%E7%BD%91%E7%AB%99)\n- [⚙ 拓展](#-%E6%8B%93%E5%B1%95)\n- [📝 更新日志](#-%E6%9B%B4%E6%96%B0%E6%97%A5%E5%BF%97)\n- [致谢](#%E8%87%B4%E8%B0%A2)\n- [项目打包上传至pypi](#%E9%A1%B9%E7%9B%AE%E6%89%93%E5%8C%85%E4%B8%8A%E4%BC%A0%E8%87%B3pypi)\n  - [poetry](#poetry)\n  - [twine](#twine)\n- [目录自动生成](#%E7%9B%AE%E5%BD%95%E8%87%AA%E5%8A%A8%E7%94%9F%E6%88%90)\n  - [安装](#%E5%AE%89%E8%A3%85)\n  - [使用](#%E4%BD%BF%E7%94%A8)\n\n<!-- END doctoc generated TOC please keep comment here to allow auto update -->\n\n## 🔧 开发环境\nNonebot2：2.0.0b5  \npython：3.8.13  \n操作系统：Windows10（CentOS7下正常运行，Linux兼容性问题不大）  \n编辑器：pycharm  \n\n## 💿 安装\n环境依赖`aiohttp`和`nonebot_plugin_htmlrender`库   \n部分功能需要获取自己的cookie，配置env后才能正常使用！  \n\n### 1. nb-cli安装（推荐）\n在你bot工程的文件夹下，运行cmd（运行路径要对啊），执行nb命令安装插件，插件配置会自动添加至配置文件  \n```\nnb plugin install nonebot_plugin_searchBiliInfo\n```\n\n### 2. 本地安装\n先安装下 `aiohttp` 和 `htmlrender`  \n```\npip install aiohttp\npip install nonebot_plugin_htmlrender\n```\n将项目clone到你的机器人插件下的对应插件目录内（一般为机器人文件夹下的`src/plugins`），然后把`nonebot_plugin_searchBiliInfo`文件夹里的内容拷贝至上一级目录即可。  \nclone命令参考（得先装`git`，懂的都懂）：\n```\ngit clone https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo.git\n``` \n也可以直接下载压缩包到插件目录解压，然后同样提取`nonebot_plugin_searchBiliInfo`至上一级目录。  \n目录结构： ```你的bot/src/plugins/nonebot_plugin_searchBiliInfo/__init__.py```  \n\n\n### 3. pip安装\n```\npip install nonebot_plugin_searchBiliInfo\n```  \n打开 nonebot2 项目的 ```bot.py``` 文件, 在其中写入  \n```nonebot.load_plugin(\'nonebot_plugin_searchBiliInfo\')```  \n当然，如果是默认nb-cli创建的nonebot2的话，在bot路径```pyproject.toml```的```[tool.nonebot]```的```plugins```中添加```nonebot_plugin_searchBiliInfo```即可  \npyproject.toml配置例如：  \n``` \n[tool.nonebot]\nplugin_dirs = ["src/plugins"]\nplugins = ["nonebot_plugin_searchBiliInfo"]\n``` \n\n### 更新版本\n```\nnb plugin update nonebot_plugin_searchBiliInfo\n```\n\n## 🔧 配置\n\n### cookie获取方式\n浏览器进入b站官网并登录: `https://www.bilibili.com/`  \nedge（或其他浏览器）按`f12`（或鼠标右键`“检查”` `“开发者工具”`等）, 然后点击右上角那个`">>"`符号, 进入`"网络"`  \n再按`ctrl+r`（或`f5`）刷新元素  \n随便点击一个请求, 在`“请求标头”`里面找到cookie（没有就换一个）  \ncookie冒号后面的就是cookie，复制一下, 可以把ta添加到env里  \n如果不想放太多cookie信息，只需要`buvid3`字段即可。  \n\n### env配置\n```\n# 在你的env文件中添加如下配置（我的是.env.prod） 仅需要buvid3字段即可\nsearchBiliInfo_cookie="buvid3=XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXXXXXXXinfoc;"\n```\n|       配置项        | 必填 | 默认值  |                      说明                      |\n|:----------------:|:----:|:----:|:----------------------------:|\n| `searchBiliInfo_cookie` | 否 | `""` | b站cookie，仅需要`buvid3`字段即可 |\n\n\n## 🎉 功能\n通过uid 或 设定好的短语 或 b站接口搜索查询指定b站用户的粉丝、舰团信息；直播收益数据；直播观看信息；关键词搜昵称、UID等信息；主播营收榜单。\n\n## 👉 命令(命令前缀自行替换喵~)\n\n### /查\n命令结构：```/查 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/查 uid:3709626``` 或 ```/查 :3709626``` 或 ```/查 bishi```  \nbot返回内容：  \n![](docs/search.png)\n\n### /查直播\n命令结构：```/查直播 (uid:或UID:或：或:)+用户uid或昵称关键词 场次数（默认不写为全部）```  \n例如：```/查直播 UID:3709626 1``` 或 ```/查直播 bishi```  \nbot返回内容（图片）：  \n![](docs/live_info.png)\n\n### /查舰团\n命令结构：```/查舰团 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/查舰团 ：3709626``` 或 ```/查舰团 bishi```  \nbot返回内容(图片)：  \n![](docs/guard.png)\n\n### /查昵称\n命令结构：```/查昵称 昵称关键词```  \n例如：```/查昵称 伊卡洛斯```\nbot返回内容(图片)：  \n![](docs/search_name.png)\n\n### /查收益\n命令结构：```/查收益 (uid:或UID:或：或:)+用户uid或昵称关键词 收益类型(默认1: 礼物，2: 上舰，3: SC) 倒叙第n场(从0开始)```  \n例如：```/查收益 :3709626 礼物 1``` 或 ```/查收益 bishi 2 0```  \nbot返回内容(图片)：  \n![](docs/income.png)\n\n### /查观看\n命令结构：```/查观看 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/查观看 UID:666666``` 或 ```/查观看 bishi```  \nbot返回内容(图片)：  \n![](docs/watch.png)\n\n### /查观看2\n命令结构：```/查观看2 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/查观看2 UID:666666``` 或 ```/查观看2 bishi```  \nbot返回内容(图片)：  \n![](docs/watch2.png)\n\n### /查弹幕\n命令结构：```/查弹幕 (uid:或UID:或：或:)+用户uid或昵称关键词 查询的主播昵称关键词或(uid:或UID:或：或:)+ 页数(可不填，默认0) 条数(可不填，默认3)```  \n例如：```/查弹幕 uid:3709626 Love丶伊卡洛斯 1 1``` 或 ```/查弹幕 uid:3709626 Love丶伊卡洛斯 1```   \nbot返回内容(图片)：  \n![](docs/danmu.png)\n\n### /查弹幕2\n命令结构：```/查弹幕2 (uid:或UID:或：或:)+用户uid或昵称关键词 页数(可不填，默认0) 条数(可不填，默认3)```  \n例如：```/查弹幕2 uid:3709626 2 2``` 或 ```/查弹幕2 uid:3709626 2```   \nbot返回内容(图片)：  \n![](docs/danmu2.png)\n\n### /查牌子\n命令结构：```/查牌子 主播牌子关键词```  \n例如：```/查牌子 天``` 或 ```/查牌子 天降```  \nbot返回内容(图片)：  \n![](docs/medal.png)\n\n### /查人气\n命令结构：```/查人气 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/查人气 uid:3709626``` 或 ```/查人气 Love丶伊卡洛斯```   \nbot返回内容(图片)：  \n![](docs/popularity.png)\n\n### /查装扮\n命令结构：```/查装扮 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/查装扮 uid:2``` 或 ```/查装扮 ：2```   \nbot返回内容(图片)：  \n![](docs/garb.png)\n\n### /营收\n命令结构：```/营收 日/周/月榜 人数（不填默认100）```  \n例如：```/营收 日榜 3``` 或 ```/营收 月榜```  \nbot返回内容(图片)：  \n![](docs/revenue.png)\n\n### /涨粉\n命令结构：```/涨粉 日/周/月榜 人数（不填默认100）```  \n例如：```/涨粉 日榜 3``` 或 ```/涨粉 月榜```  \nbot返回内容(图片)：  \n![](docs/incfans.png)\n\n### /DD风云榜 或 /dd风云榜 或 /风云榜 (寄了)\n命令结构：```/DD风云榜 top人数（不填默认10）```  \n例如：```/DD风云榜``` 或 ```/风云榜 20```  \nbot返回内容(图片)：  \n![](docs/ddstats.png)\n\n### /v详情 或 /V详情 或 /v详细 或 /V详细\n命令结构：```/v详情 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/v详情 uid:3709626``` 或 ```/V详情 ：2``` 或 ```/v详细 Love丶伊卡洛斯``` 或 ```/V详细 :2```    \nbot返回内容(图片)：  \n![](docs/v_detail.png)\n\n### /v直播势 或 /V直播势\n命令结构：```/v直播势```  \n例如：```/v直播势``` 或 ```/V直播势```  \nbot返回内容(图片)：  \n![](docs/v_live.png)\n\n### /v急上升 或 /V急上升\n命令结构：```/v急上升```  \n例如：```/v急上升``` 或 ```/V急上升```  \nbot返回内容(图片)：  \n![](docs/v_rise.png)\n\n### /v急下降 或 /V急下降\n命令结构：```/v急下降```  \n例如：```/v急下降``` 或 ```/V急下降```  \nbot返回内容(图片)：  \n![](docs/v_drop.png)\n\n### /v舰团 或 /V舰团\n命令结构：```/v舰团```  \n例如：```/v舰团``` 或 ```/V舰团```  \nbot返回内容(图片)：  \n![](docs/v_guard.png)\n\n### /vdd 或 /VDD 或 /VDD风云榜 或 /vdd风云榜\n命令结构：```/vdd```  \n例如：```/vdd``` 或 ```/VDD```  或 ```/vdd风云榜```   \nbot返回内容(图片)：  \n![](docs/v_dd.png)\n\n### /V宏观 或 /v宏观\n命令结构：```/vdd```  \n例如：```/V宏观``` 或 ```/v宏观```   \nbot返回内容(图片)：  \n![](docs/v_macro.png)\n\n### /dmk查用户 或 /DMK查用户\n命令结构：```/dmk查用户 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/dmk查用户 uid:3709626``` 或 ```/DMK查用户 Love丶伊卡洛斯```  \nbot返回内容(图片)：  \n![](docs/dmk_user.png)\n\n### /dmk查直播 或 /DMK查直播\n命令结构：```/dmk查直播 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/dmk查直播 uid:3709626``` 或 ```/DMK查直播 Love丶伊卡洛斯```  \nbot返回内容(图片)：  \n![](docs/dmk_live.png)\n\n### /blg查弹幕 或 /BLG查弹幕\n命令结构：```/blg查弹幕 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/blg查弹幕 uid:3709626``` 或 ```/BLG查弹幕 Love丶伊卡洛斯```  \nbot返回内容(图片)：  \n![](docs/blg_danmu.png)\n\n### /blg查入场 或 /BLG查入场\n命令结构：```/blg查入场 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/blg查入场 uid:3709626``` 或 ```/BLG查入场 Love丶伊卡洛斯```  \nbot返回内容(图片)：  \n![](docs/blg_enter.png)\n\n### /blg查礼物 或 /BLG查礼物\n命令结构：```/blg查礼物 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/blg查礼物 uid:3709626``` 或 ```/BLG查礼物 Love丶伊卡洛斯```  \nbot返回内容(图片)：  \n![](docs/blg_gift.png)\n\n### /blg直播记录 或 /BLG直播记录\n命令结构：```/blg直播记录 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/blg直播记录 uid:3709626``` 或 ```/BLG直播记录 Love丶伊卡洛斯```  \nbot返回内容(图片)：  \n![](docs/blg_tp.png)\n\n### /blg直播间sc 或 /BLG直播间SC\n命令结构：```/blg直播间sc (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/blg直播间sc uid:3709626``` 或 ```/BLG直播间SC Love丶伊卡洛斯```  \nbot返回内容(图片)：  \n![](docs/blg_sc.png)\n\n### /icu查直播 或 /ICU查直播 或 /matsuri查直播\n命令结构：```/icu查直播 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/icu查直播 uid:3709626``` 或 ```/ICU查直播 Love丶伊卡洛斯```  \nbot返回内容(图片)：  \n![](docs/icu_live.png)\n\n### /lap查用户 或 /LAP查用户\n命令结构：```/lap查用户 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/lap查用户 uid:387636363``` 或 ```/LAP查用户 雫るる```  \nbot返回内容(图片)：  \n![](docs/laplace_user.png)\n\n### /lap查牌子 或 /LAP查牌子\n命令结构：```/lap查牌子 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/lap查牌子 uid:387636363``` 或 ```/LAP查牌子 雫るる```  \nbot返回内容(图片)：  \n![](docs/laplace_medal.png)\n\n### /lap查充电 或 /LAP查充电\n命令结构：```/lap查充电 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/lap查充电 uid:387636363``` 或 ```/LAP查充电 雫るる```  \nbot返回内容(图片)：  \n![](docs/laplace_upower.png)\n\n### /lapdd 或 /LAPDD 或 /lapdd排行榜\n命令结构：```/lapdd 搜索类型(默认0: 月供，1: 总督，2: 提督，3：舰长)```  \n例如：```/lapdd``` 或 ```/lapdd 1``` 或 ```/LAPDD 舰长```  \nbot返回内容(图片)：  \n![](docs/laplace_dd.png)\n\n### /zero查用户 或 /ZERO查用户\n命令结构：```/zero查用户 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/zero查用户 uid:387636363``` 或 ```/ZERO查用户 雫るる```  \nbot返回内容(图片)：  \n![](docs/zeroroku_author.png)\n\n### /zero被关注 或 /ZERO被关注\n命令结构：```/zero被关注 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/zero被关注 uid:387636363``` 或 ```/ZERO被关注 雫るる```  \nbot返回内容(图片)：  \n![](docs/zeroroku_famous_fans.png)\n\n### 斗虫 或 主播pk 或 主播PK\n命令结构：`斗虫|主播pk|主播PK 用户1的uid或昵称关键词 用户2的uid或昵称关键词 用户n的uid或昵称关键词 #当天向过去偏移天(起始) 当天向过去偏移天数(结尾)`\n注意：`#`和后面的`日期偏移`可以默认不填，不填写的话默认是一个月前到今天的数据。另外，传入的用户必须大于等于2人以上。（`日期偏移`其实就是`数据区间`啦）\n例如：```斗虫 雫酱 neol``` 或 ```斗虫 雫酱 neol #5 0``` 或 ```主播pk 雫酱 雫 #15 0```    \nbot返回内容(图片)：  \n![](docs/stats_nailv_live_compare.png)\n\n\n### eh查直播 或 诶嘿查直播 或 eihei查直播\n命令结构：```/eh查直播 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/诶嘿查直播 uid:3493132603754688``` 或 ```/诶嘿查直播 罗亚Roya```  \nbot返回内容(图片)：  \n![](docs/eihei_livepic.png)\n\n### /vtb网站\n命令结构：```/vtb网站``` 或 ```/vtb资源```  \n例如：```/vtb网站``` 或 ```/vtb资源```  \nbot返回内容：  \n```\nVTB数据看板：https://ikaros-521.gitee.io/vtb_data_board/\nmatsuri：https://matsuri.icu/\ndanmakus：https://danmakus.com/\nvtbs.fun：http://www.vtbs.fun/\nbiligank：https://biligank.com/\n火龙榜：https://huolonglive.com/#/\nvtbs.moe：https://vtbs.moe/\nvup.loveava.top：https://vup.loveava.top/ranking\nddstats：https://ddstats.ericlamm.xyz/\nzeroroku：https://zeroroku.com/bilibili\nlaplace：https://laplace.live/\n```\n\n## ⚙ 拓展\n启用关键词搜索，需要在`.env.xx`中配置自己的`cookie`。\n\n命令修改：  \n昵称自定义，修改`data.py`，在文件头部追加你需要定义的用户的json串，注意json格式！！！  \n命令自定义，修改`__init__.py`，`catch_str = on_command`这部分的代码即可。  \n\nbot返回内容格式修改对应的msg、out_str变量的内容  \n\n## 📝 更新日志\n\n<details>\n<summary>展开/收起</summary>\n\n### 0.0.1\n\n- 插件初次发布\n\n### 0.1.0\n\n- 更新基于vtbs.moe的主播数据，添加关键词搜索功能\n\n### 1.0.0\n\n新增以下功能（其实是LX_Bot的相关命令融进来了）\n- /查 昵称关键词\n- /查直播 昵称关键词 场次数\n- /查舰团 昵称关键词\n- /查昵称 昵称关键词\n- /查收益 收益类型(默认1: 礼物，2: 上舰，3: SC) 用户uid或昵称关键词 倒叙第n场(从0开始)\n- /查成分 观看 昵称关键词\n- /查成分 弹幕 查询的目标人 查询的主播 页数 条数\n\n### 1.0.4\n\n优化针对uid解析方式\n\n### 1.0.5\n\n修改cookie配置从env获取，方便用户配置\n\n### 1.0.6\n\n修复 /查成分 弹幕 数据解析bug；\n优化整体代码实现；\n\n### 1.1.0\n新增功能\n- /营收 日/周/月榜 人数（不填默认100）\n\n### 1.2.0\n弃用requests库，改为aiohttp  \n\n### 1.2.1\n修复查命令aiohttp适配性bug  \n\n### 1.3.0\n修改 查成分 弹幕 和 查成分 观看 命令为 查弹幕 和 查观看。  \n优化命令解析实现。  \n修复查弹幕数据解析bug。  \n\n### 1.3.1\n新增 /查弹幕2 命令。  \n修复查弹幕数据解析bug。 \n图片UI优化。  \n\n### 1.3.2\n优化 /查弹幕2 命令，增加主播名。  \n\n### 1.3.3\n修复 /查观看 因为数据源有同一用户名不同uid的情况导致的越界bug。  \n\n### 1.3.4\n优化异常报错的处理。  \n优化UI设计和部分功能。  \n\n### 1.3.5\n新增`/查收益 xx 舰长`和`uid：`的匹配。（但是舰长仍然是所有上舰数据）    \n\n### 1.3.6\n优化API挂彩时候的异常捕获处理。  \n\n### 1.3.7\n插件补充元信息。 \n\n### 1.3.8\n新增`vtb网站` 或 `vtb资源` 命令（命令前缀自行添加） \n\n### 1.3.9\n补充2个VTB资源站点  \n\n### 1.3.10\n适配vtbs.fun的营收接口变动  \n\n### 1.4.0\n修改on_keyword为on_command，从而适配自定义的命令前缀  \n\n### 1.4.1\n修改danmakus.com到新域名danmakus.com，接口也同步替换了。  \n\n### 1.4.2\n新增markdown的特殊字符过滤和文本超长换行。  \nps：vtbs.fun挂了，`营收`功能暂时无法使用。\n\n### 1.4.3\nvtbs.fun活了，加了ssl，已兼容。  \n\n### 1.4.4\n新增命令 涨粉，接口源自vtbs.fun（和营收 基本一致）  \n\n### 1.4.5\n新增命令 DD风云榜，接口源自ddstats-api.ericlamm.xyz  \n\n### 1.4.6\n补充遗漏的插件元信息    \n\n### 1.4.7\n新增功能 查牌子，数据源自本地爬取（vtbs.moe中主播牌子信息，共4273条数据）   \n\n### 1.4.8\n补充插牌子遗漏的1条数据   \n\n### 1.4.9\n补充遗漏的 vtb网站 功能元信息   \n\n### 1.4.10\n新增功能`v详情` `dmk查用户` `dmk查直播`，直接采用浏览器页面截图形式返回结果。（流量消耗会多一些，酌情使用）     \n\n### 1.4.11\n延长`v详情` `dmk查用户` `dmk查直播`的请求超时至5min（服务器4M跑也超时，功能很吃紧）  \n\n### 1.4.12\n追加最新的vtbs.moe的主播信息，并同步更新了牌子信息。  \n缩短`v详情` `dmk查用户` `dmk查直播`的请求超时至2min（前面是对面服务器炸了）  \n\n### 1.4.13\n优化请求错误或无数据时的消息返回和日志打印。  \n\n### 1.5.0\n新增功能`blg查弹幕` `blg查入场` `blg查礼物` `blg直播记录` `blg直播间sc`，直接采用浏览器页面截图形式返回结果。（流量消耗会多一些，酌情使用）     \n\n### 1.5.1\n新增4000+的用户数据和牌子数据  \n\n### 1.5.2\n新增b站用户数据至10w  \n新增粉丝牌数据至4w+  \n\n### 1.5.3\n新增网站laplace.live  \n新增`icu查直播`命令，同样是playwright的直接加载  \n\n### 1.5.4\n新用户数据爬自b站直播间各大分区列表，比起直接uid爬全站更具有针对性，实际效果也很好。  \n新增b站用户数据至23w+  \n新增粉丝牌数据至6.7w+  \n\n### 1.5.5\n由于出现低配置设备内存不足导致的无法启动问题，已将本地数据`data.py`清空至一个demo配置。如有本地配置需要的可以去旧版获取。  \n\n### 1.5.6\n新增粉丝牌数据至8.6w+，爬了一周的直播页，正式收工。  \n\n### 1.5.7\n新增命令`查人气`，用于查询b站主播最近一场直播的人气峰值  \n\n### 1.5.8\n新增`lap查用户`命令，同样是playwright，并做了js内嵌  \n\n### 1.5.9\n优化`lap查用户`的内容加载样式，显示内容更加全面（也更卡，乐）  \n\n### 1.5.10\n增加耗时的网页截图查询反馈，优化异常处理，不让你的人生浪费在等待中  \n\n### 1.5.11\n新增`zero查用户`命令，同理  \n\n### 1.5.12\n修复文档描述错误（不影响功能，暂不发版）  \n文档新增目录    \n\n### 1.5.13\n新增`lap查牌子`命令，调用laplace.live的接口，全站太卡了，绷  \n\n### 1.5.14\n修复`lap查牌子`接口返回uid固定问题导致的显示错误  \n优化文档  \n\n### 1.5.15\n升级`查观看`功能，统计观看次数。  \n\n### 1.5.16\n新增`查观看2`命令（查观看plus版），统计观看次数，以饼图形式返回。  \n\n### 1.5.17\n优化网页截图相关功能的图片存储名，减少短时间多请求导致的数据覆盖问题  \n修复`查观看2`的提示语延迟问题  \n修订文档错误  \n\n### 1.5.18\n新增`lap查充电`命令，查询up的充电排行榜。  \n新增`zero被关注`命令，查询用户的被哪些知名up主关注。  \n升级`查观看2`的主题为夜间模式，增加高级感。  \n\n### 1.6.0\n对类似的GET请求做了优化，降低代码冗余。  \n\n### 1.6.1\n删除`lap查用户`的小作文  \n\n### 1.6.2\n1、新增以下命令：  \n- /v直播势  （大写也可以）\n- /v急上升  （大写也可以）\n- /v急下降  （大写也可以）\n- /v舰团  （大写也可以）\n- /vdd  （大写也可以）\n- /v宏观  （大写也可以）  \n2、优化异常处理\n\n### 1.6.3\n优化`v详情`的请求延时，帮助数据加载。  \n\n### 1.6.4\n新增`查装扮`命令。  \n优化文档排序。 \n\n### 1.6.5\n1.`v详情`增加别名`v详细`。  \n2.修复`查收益`的传参bug。  \n3.优化代码实现，增加提示互动。  \n\n### 1.6.6\n1.修复`查弹幕`和`查弹幕2`的bug（让GPT帮忙写，很好，bug写得不错）  \n\n### 1.6.7\n1.命令文本消息内容改艾特为回复。  \n2.新增命令`lapdd`或`lapdd排行榜`，截图laplace.live的dd页面。  \n3.优化说明文档。  \n\n### 1.6.8\n修复`lapdd`命令不传参的bug。  \n\n### 1.6.9\n新增正则匹配的`斗虫`玩法，具体看命令说明。  \n\n### 1.7.0\n修复htmlrender导入问题。  \n\n### 1.7.1\n新增命令`eh查直播`或`诶嘿查直播`。  \n\n### 1.7.2\n修改`eh查直播`的请求地址为http，服务器上跑证书不行，绷。  \n\n### 1.7.3\n修改`eh查直播`为playwright，难绷。  \n\n### 1.7.4\n修改`eh查直播`为直接请求，不过跳过了ssl。  \n\n### 1.7.5\nbug修复  \n\n### 1.7.6\n`查`命令，追加返回用户主页和直播间链接。    \n\n</details>\n\n## 致谢\n- [nonebot-plugin-htmlrender](https://github.com/kexue-z/nonebot-plugin-htmlrender) - 图片合成的好手\n- [danmakus.com](https://danmakus.com/) - b站主播、用户弹幕直播信息等来源（开放API接口很赞！）\n- [vtbs.moe](https://vtbs.moe) - VTB本地数据信息来源（还有数据提供，TQL）  \n- [laplace.live](https://laplace.live/) - 也是b站主播用户查询站点，部分数据也是源自danmakus，UI不错  \n\n## 项目打包上传至pypi\n\n官网：https://pypi.org，注册账号，在系统用户根目录下创建`.pypirc`，配置  \n``` \n[distutils] \nindex-servers=pypi \n \n[pypi] repository = https://upload.pypi.org/legacy/ \nusername = 用户名 \npassword = 密码\n```\n\n### poetry\n\n```\n# 参考 https://www.freesion.com/article/58051228882/\n\n# 1、安装poetry\npip install poetry\n\n# 2、初始化配置文件（根据提示填写）\npoetry init\n\n# 3、微调配置文件pyproject.toml\n\n# 4、运行 poetry install, 可生成 “poetry.lock” 文件（可跳过）\npoetry install\n\n# 5、编译，生成dist\npoetry build\n\n# 6、发布\npoetry publish\n\n```\n\n### twine\n\n```\n# 参考 https://www.cnblogs.com/danhuai/p/14915042.html\n#创建setup.py文件 填写相关信息\n\n# 1、可以先升级打包工具\npip install --upgrade setuptools wheel twine\n\n# 2、打包\npython setup.py sdist bdist_wheel\n\n# 3、可以先检查一下包\ntwine check dist/*\n\n# 4、上传包到pypi（需输入用户名、密码）\ntwine upload dist/*\n```\n\n## 目录自动生成\n\n[doctoc](https://github.com/thlorenz/doctoc),在本地git存储库中生成降价文件的目录。链接通过命令行标志兼容github或其他网站生成的锚。\n\n### 安装\n进入包含本地git项目的目录，键入: `npm install -g doctoc`  \n\n### 使用\n在`README.md`中，找个生成目录位置，写入如下代码，确认生成位置：\n```\n<!-- START doctoc -->\n<!-- END doctoc -->\n```\ncmd输入命令即可：`doctoc /path/to/file`  \n例如：`doctoc README.md`  \n\n',
     'author': 'Ikaros',
     'author_email': '327209194@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_searchbiliinfo'] package_data = \ {'': ['*'],
 'nonebot_plugin_searchbiliinfo': ['html/*']} install_requires = \
 ['aiohttp>=3.8.3,<4.0.0', 'asyncio>=3.4.3,<4.0.0', 'nonebot-adapter-
 onebot>=2.1.3,<3.0.0', 'nonebot-plugin-htmlrender>=0.2.0.1,<0.3.0.0',
 'nonebot2>=2.0.0b5,<3.0.0'] setup_kwargs = { 'name': 'nonebot-plugin-
-searchbiliinfo', 'version': '1.7.5', 'description': 'A plugin for nonebot2.
+searchbiliinfo', 'version': '1.7.6', 'description': 'A plugin for nonebot2.
 Query Bilibili user
 informationï¼ä¸ä¸ªNonebot2çæä»¶ï¼bç«ç¨æ·ä¿¡æ¯æ¥è¯¢æä»¶ãç²ä¸ãè°å¢ä¿¡æ¯ï¼ç´æ­æ¶çæ°æ®ï¼ç´æ­è§çä¿¡æ¯ï¼å³é®è¯ææµç§°ãUIDï¼ä¸»æ­è¥æ¶æ¦åï¼æ¥æåï¼æ¥çå­ç­ãï¼',
 'long_description': '
                            \n [NoneBotPluginLogo]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
@@ -385,17 +385,19 @@
 \n3.ä¼åè¯´æææ¡£ã \n\n### 1.6.8\nä¿®å¤`lapdd`å½ä»¤ä¸ä¼ åçbugã
 \n\n### 1.6.9\næ°å¢æ­£åå¹éç`æè«`ç©æ³ï¼å·ä½çå½ä»¤è¯´æã
 \n\n### 1.7.0\nä¿®å¤htmlrenderå¯¼å¥é®é¢ã \n\n###
 1.7.1\næ°å¢å½ä»¤`ehæ¥ç´æ­`æ`è¯¶å¿æ¥ç´æ­`ã \n\n###
 1.7.2\nä¿®æ¹`ehæ¥ç´æ­`çè¯·æ±å°åä¸ºhttpï¼æå¡å¨ä¸è·è¯ä¹¦ä¸è¡ï¼ç»·ã
 \n\n### 1.7.3\nä¿®æ¹`ehæ¥ç´æ­`ä¸ºplaywrightï¼é¾ç»·ã \n\n###
 1.7.4\nä¿®æ¹`ehæ¥ç´æ­`ä¸ºç´æ¥è¯·æ±ï¼ä¸è¿è·³è¿äºsslã \n\n###
-1.7.5\nbugä¿®å¤ \n\n\n\n## è´è°¢\n- [nonebot-plugin-htmlrender](https://
-github.com/kexue-z/nonebot-plugin-htmlrender) - å¾çåæçå¥½æ\n-
-[danmakus.com](https://danmakus.com/) -
+1.7.5\nbugä¿®å¤ \n\n###
+1.7.6\n`æ¥`å½ä»¤ï¼è¿½å è¿åç¨æ·ä¸»é¡µåç´æ­é´é¾æ¥ã \n\n\n\n##
+è´è°¢\n- [nonebot-plugin-htmlrender](https://github.com/kexue-z/nonebot-
+plugin-htmlrender) - å¾çåæçå¥½æ\n- [danmakus.com](https://
+danmakus.com/) -
 bç«ä¸»æ­ãç¨æ·å¼¹å¹ç´æ­ä¿¡æ¯ç­æ¥æºï¼å¼æ¾APIæ¥å£å¾èµï¼ï¼\n-
 [vtbs.moe](https://vtbs.moe) -
 VTBæ¬å°æ°æ®ä¿¡æ¯æ¥æºï¼è¿ææ°æ®æä¾ï¼TQLï¼ \n- [laplace.live]
 (https://laplace.live/) -
 ä¹æ¯bç«ä¸»æ­ç¨æ·æ¥è¯¢ç«ç¹ï¼é¨åæ°æ®ä¹æ¯æºèªdanmakusï¼UIä¸é
 \n\n## é¡¹ç®æåä¸ä¼ è³pypi\n\nå®ç½ï¼https://
 pypi.orgï¼æ³¨åè´¦å·ï¼å¨ç³»ç»ç¨æ·æ ¹ç®å½ä¸åå»º`.pypirc`ï¼éç½®
```

### Comparing `nonebot_plugin_searchbiliinfo-1.7.5/PKG-INFO` & `nonebot_plugin_searchbiliinfo-1.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-searchbiliinfo
-Version: 1.7.5
+Version: 1.7.6
 Summary: A plugin for nonebot2. Query Bilibili user information（一个Nonebot2的插件，b站用户信息查询插件【粉丝、舰团信息；直播收益数据；直播观看信息；关键词搜昵称、UID；主播营收榜单；查成分；查牌子等】）
 Home-page: https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo
 License: MIT
 Author: Ikaros
 Author-email: 327209194@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -709,14 +709,17 @@
 
 ### 1.7.4
 修改`eh查直播`为直接请求，不过跳过了ssl。  
 
 ### 1.7.5
 bug修复  
 
+### 1.7.6
+`查`命令，追加返回用户主页和直播间链接。    
+
 </details>
 
 ## 致谢
 - [nonebot-plugin-htmlrender](https://github.com/kexue-z/nonebot-plugin-htmlrender) - 图片合成的好手
 - [danmakus.com](https://danmakus.com/) - b站主播、用户弹幕直播信息等来源（开放API接口很赞！）
 - [vtbs.moe](https://vtbs.moe) - VTB本地数据信息来源（还有数据提供，TQL）  
 - [laplace.live](https://laplace.live/) - 也是b站主播用户查询站点，部分数据也是源自danmakus，UI不错
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-searchbiliinfo Version: 1.7.5
+Metadata-Version: 2.1 Name: nonebot-plugin-searchbiliinfo Version: 1.7.6
 Summary: A plugin for nonebot2. Query Bilibili user
 informationï¼ä¸ä¸ªNonebot2çæä»¶ï¼bç«ç¨æ·ä¿¡æ¯æ¥è¯¢æä»¶ãç²ä¸ãè°å¢ä¿¡æ¯ï¼ç´æ­æ¶çæ°æ®ï¼ç´æ­è§çä¿¡æ¯ï¼å³é®è¯ææµç§°ãUIDï¼ä¸»æ­è¥æ¶æ¦åï¼æ¥æåï¼æ¥çå­ç­ãï¼
 Home-page: https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo License:
 MIT Author: Ikaros Author-email: 327209194@qq.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
@@ -365,17 +365,17 @@
 3.ä¼åè¯´æææ¡£ã ### 1.6.8 ä¿®å¤`lapdd`å½ä»¤ä¸ä¼ åçbugã ###
 1.6.9 æ°å¢æ­£åå¹éç`æè«`ç©æ³ï¼å·ä½çå½ä»¤è¯´æã ### 1.7.0
 ä¿®å¤htmlrenderå¯¼å¥é®é¢ã ### 1.7.1
 æ°å¢å½ä»¤`ehæ¥ç´æ­`æ`è¯¶å¿æ¥ç´æ­`ã ### 1.7.2
 ä¿®æ¹`ehæ¥ç´æ­`çè¯·æ±å°åä¸ºhttpï¼æå¡å¨ä¸è·è¯ä¹¦ä¸è¡ï¼ç»·ã
 ### 1.7.3 ä¿®æ¹`ehæ¥ç´æ­`ä¸ºplaywrightï¼é¾ç»·ã ### 1.7.4
 ä¿®æ¹`ehæ¥ç´æ­`ä¸ºç´æ¥è¯·æ±ï¼ä¸è¿è·³è¿äºsslã ### 1.7.5 bugä¿®å¤
-## è´è°¢ - [nonebot-plugin-htmlrender](https://github.com/kexue-z/nonebot-
-plugin-htmlrender) - å¾çåæçå¥½æ - [danmakus.com](https://
-danmakus.com/) -
+### 1.7.6 `æ¥`å½ä»¤ï¼è¿½å è¿åç¨æ·ä¸»é¡µåç´æ­é´é¾æ¥ã  ##
+è´è°¢ - [nonebot-plugin-htmlrender](https://github.com/kexue-z/nonebot-plugin-
+htmlrender) - å¾çåæçå¥½æ - [danmakus.com](https://danmakus.com/) -
 bç«ä¸»æ­ãç¨æ·å¼¹å¹ç´æ­ä¿¡æ¯ç­æ¥æºï¼å¼æ¾APIæ¥å£å¾èµï¼ï¼ -
 [vtbs.moe](https://vtbs.moe) -
 VTBæ¬å°æ°æ®ä¿¡æ¯æ¥æºï¼è¿ææ°æ®æä¾ï¼TQLï¼ - [laplace.live]
 (https://laplace.live/) -
 ä¹æ¯bç«ä¸»æ­ç¨æ·æ¥è¯¢ç«ç¹ï¼é¨åæ°æ®ä¹æ¯æºèªdanmakusï¼UIä¸é
 ## é¡¹ç®æåä¸ä¼ è³pypi å®ç½ï¼https://
 pypi.orgï¼æ³¨åè´¦å·ï¼å¨ç³»ç»ç¨æ·æ ¹ç®å½ä¸åå»º`.pypirc`ï¼éç½®
```

