# Comparing `tmp/tatarubot2-0.1.1.tar.gz` & `tmp/tatarubot2-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tatarubot2-0.1.1.tar", last modified: Mon Apr 10 09:02:16 2023, max compression
+gzip compressed data, was "tatarubot2-0.1.2.tar", max compression
```

## Comparing `tatarubot2-0.1.1.tar` & `tatarubot2-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 09:02:16.000000 tatarubot2-0.1.1/
--rw-r--r--   0 root         (0) root         (0)     1066 2022-08-12 03:44:26.000000 tatarubot2-0.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2908 2023-04-10 09:02:16.000000 tatarubot2-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2734 2023-03-14 01:51:48.000000 tatarubot2-0.1.1/README.md
--rw-r--r--   0 root         (0) root         (0)      387 2022-06-22 03:02:25.000000 tatarubot2-0.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 09:02:16.000000 tatarubot2-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      572 2023-04-10 08:55:17.000000 tatarubot2-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 09:02:16.000000 tatarubot2-0.1.1/tatarubot2/
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-10 08:55:17.000000 tatarubot2-0.1.1/tatarubot2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 09:02:16.000000 tatarubot2-0.1.1/tatarubot2/plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 02:51:28.000000 tatarubot2-0.1.1/tatarubot2/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      713 2022-11-15 08:07:47.000000 tatarubot2-0.1.1/tatarubot2/plugins/auto_response.py
--rw-r--r--   0 root         (0) root         (0)     1627 2023-04-07 06:02:20.000000 tatarubot2-0.1.1/tatarubot2/plugins/bot_help.py
--rw-r--r--   0 root         (0) root         (0)     1211 2023-04-07 02:28:25.000000 tatarubot2-0.1.1/tatarubot2/plugins/chat_ai.py
--rw-r--r--   0 root         (0) root         (0)     2262 2022-08-16 07:15:05.000000 tatarubot2-0.1.1/tatarubot2/plugins/ff_weibo.py
--rw-r--r--   0 root         (0) root         (0)     4409 2022-08-17 03:31:15.000000 tatarubot2-0.1.1/tatarubot2/plugins/house.py
--rw-r--r--   0 root         (0) root         (0)    17045 2023-01-29 07:09:23.000000 tatarubot2-0.1.1/tatarubot2/plugins/item.py
--rw-r--r--   0 root         (0) root         (0)    17338 2023-04-07 06:02:20.000000 tatarubot2-0.1.1/tatarubot2/plugins/item_new.py
--rw-r--r--   0 root         (0) root         (0)     7011 2023-04-07 06:02:20.000000 tatarubot2-0.1.1/tatarubot2/plugins/logs_dps.py
--rw-r--r--   0 root         (0) root         (0)     1230 2022-08-12 01:48:07.000000 tatarubot2-0.1.1/tatarubot2/plugins/lottery.py
--rw-r--r--   0 root         (0) root         (0)     7754 2022-08-15 08:28:24.000000 tatarubot2-0.1.1/tatarubot2/plugins/market.py
--rw-r--r--   0 root         (0) root         (0)     8223 2023-04-07 06:02:20.000000 tatarubot2-0.1.1/tatarubot2/plugins/market_new.py
--rw-r--r--   0 root         (0) root         (0)     3103 2022-09-24 04:17:17.000000 tatarubot2-0.1.1/tatarubot2/plugins/nuannuan.py
--rw-r--r--   0 root         (0) root         (0)      899 2022-08-12 01:48:15.000000 tatarubot2-0.1.1/tatarubot2/plugins/precious.py
--rw-r--r--   0 root         (0) root         (0)     1196 2022-06-23 07:26:19.000000 tatarubot2-0.1.1/tatarubot2/plugins/weather.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 09:02:16.000000 tatarubot2-0.1.1/tatarubot2/tools/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-12 07:58:45.000000 tatarubot2-0.1.1/tatarubot2/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5058 2023-04-07 06:02:20.000000 tatarubot2-0.1.1/tatarubot2/tools/download_boss.py
--rw-r--r--   0 root         (0) root         (0)     1962 2023-01-30 01:23:02.000000 tatarubot2-0.1.1/tatarubot2/tools/download_item2id.py
--rw-r--r--   0 root         (0) root         (0)     1725 2023-04-07 06:02:20.000000 tatarubot2-0.1.1/tatarubot2/tools/normal_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 09:02:16.000000 tatarubot2-0.1.1/tatarubot2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2908 2023-04-10 09:02:16.000000 tatarubot2-0.1.1/tatarubot2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      825 2023-04-10 09:02:16.000000 tatarubot2-0.1.1/tatarubot2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 09:02:16.000000 tatarubot2-0.1.1/tatarubot2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-10 09:02:16.000000 tatarubot2-0.1.1/tatarubot2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-10 09:02:16.000000 tatarubot2-0.1.1/tatarubot2.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1066 2022-08-12 03:44:26.000000 tatarubot2-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2734 2023-03-14 01:51:48.000000 tatarubot2-0.1.2/README.md
+-rw-r--r--   0        0        0      394 2023-04-10 09:23:37.000000 tatarubot2-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-04-10 08:55:17.000000 tatarubot2-0.1.2/tatarubot2/__init__.py
+-rw-r--r--   0        0        0    82117 2023-01-12 06:12:13.000000 tatarubot2-0.1.2/tatarubot2/data/boss.json
+-rw-r--r--   0        0        0  1218488 2023-01-30 01:23:59.000000 tatarubot2-0.1.2/tatarubot2/data/item_dict.json
+-rw-r--r--   0        0        0     2422 2022-12-26 09:14:52.000000 tatarubot2-0.1.2/tatarubot2/data/job.json
+-rw-r--r--   0        0        0        0 2023-04-07 02:51:28.000000 tatarubot2-0.1.2/tatarubot2/plugins/__init__.py
+-rw-r--r--   0        0        0      713 2022-11-15 08:07:47.000000 tatarubot2-0.1.2/tatarubot2/plugins/auto_response.py
+-rw-r--r--   0        0        0     1627 2023-04-07 06:02:20.000000 tatarubot2-0.1.2/tatarubot2/plugins/bot_help.py
+-rw-r--r--   0        0        0     1211 2023-04-07 02:28:25.000000 tatarubot2-0.1.2/tatarubot2/plugins/chat_ai.py
+-rw-r--r--   0        0        0     2262 2022-08-16 07:15:05.000000 tatarubot2-0.1.2/tatarubot2/plugins/ff_weibo.py
+-rw-r--r--   0        0        0     4409 2022-08-17 03:31:15.000000 tatarubot2-0.1.2/tatarubot2/plugins/house.py
+-rw-r--r--   0        0        0    17045 2023-01-29 07:09:23.000000 tatarubot2-0.1.2/tatarubot2/plugins/item.py
+-rw-r--r--   0        0        0    17338 2023-04-07 06:02:20.000000 tatarubot2-0.1.2/tatarubot2/plugins/item_new.py
+-rw-r--r--   0        0        0     7011 2023-04-07 06:02:20.000000 tatarubot2-0.1.2/tatarubot2/plugins/logs_dps.py
+-rw-r--r--   0        0        0     1230 2022-08-12 01:48:07.000000 tatarubot2-0.1.2/tatarubot2/plugins/lottery.py
+-rw-r--r--   0        0        0     7754 2022-08-15 08:28:24.000000 tatarubot2-0.1.2/tatarubot2/plugins/market.py
+-rw-r--r--   0        0        0     8223 2023-04-07 06:02:20.000000 tatarubot2-0.1.2/tatarubot2/plugins/market_new.py
+-rw-r--r--   0        0        0     3103 2022-09-24 04:17:17.000000 tatarubot2-0.1.2/tatarubot2/plugins/nuannuan.py
+-rw-r--r--   0        0        0      899 2022-08-12 01:48:15.000000 tatarubot2-0.1.2/tatarubot2/plugins/precious.py
+-rw-r--r--   0        0        0     1196 2022-06-23 07:26:19.000000 tatarubot2-0.1.2/tatarubot2/plugins/weather.py
+-rw-r--r--   0        0        0        0 2022-08-12 07:58:45.000000 tatarubot2-0.1.2/tatarubot2/tools/__init__.py
+-rw-r--r--   0        0        0  1010264 2022-08-12 20:09:39.000000 tatarubot2-0.1.2/tatarubot2/tools/data.json
+-rw-r--r--   0        0        0     5058 2023-04-07 06:02:20.000000 tatarubot2-0.1.2/tatarubot2/tools/download_boss.py
+-rw-r--r--   0        0        0     1962 2023-01-30 01:23:02.000000 tatarubot2-0.1.2/tatarubot2/tools/download_item2id.py
+-rw-r--r--   0        0        0    82117 2023-01-12 06:12:13.000000 tatarubot2-0.1.2/tatarubot2/tools/new_boss.json
+-rw-r--r--   0        0        0     2422 2022-12-26 09:13:22.000000 tatarubot2-0.1.2/tatarubot2/tools/new_job.json
+-rw-r--r--   0        0        0     1725 2023-04-07 06:02:20.000000 tatarubot2-0.1.2/tatarubot2/tools/normal_data.py
+-rw-r--r--   0        0        0     3180 1970-01-01 00:00:00.000000 tatarubot2-0.1.2/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tatarubot2-0.1.1/LICENSE` & `tatarubot2-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.1/PKG-INFO` & `tatarubot2-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: tatarubot2
-Version: 0.1.1
-Summary: FF14 bot Tataru
-Author: aaron-li
-Author-email: 
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # TataruBot2
 
 基于NoneBot2的FF14机器人塔塔露
 
 ## 当前功能
 
 1. 暖暖：本周时尚品鉴作业
```

### Comparing `tatarubot2-0.1.1/tatarubot2/plugins/auto_response.py` & `tatarubot2-0.1.2/tatarubot2/plugins/auto_response.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.1/tatarubot2/plugins/bot_help.py` & `tatarubot2-0.1.2/tatarubot2/plugins/bot_help.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.1/tatarubot2/plugins/chat_ai.py` & `tatarubot2-0.1.2/tatarubot2/plugins/chat_ai.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.1/tatarubot2/plugins/ff_weibo.py` & `tatarubot2-0.1.2/tatarubot2/plugins/ff_weibo.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.1/tatarubot2/plugins/house.py` & `tatarubot2-0.1.2/tatarubot2/plugins/house.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.1/tatarubot2/plugins/item.py` & `tatarubot2-0.1.2/tatarubot2/plugins/item.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.1/tatarubot2/plugins/item_new.py` & `tatarubot2-0.1.2/tatarubot2/plugins/item_new.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.1/tatarubot2/plugins/logs_dps.py` & `tatarubot2-0.1.2/tatarubot2/plugins/logs_dps.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.1/tatarubot2/plugins/lottery.py` & `tatarubot2-0.1.2/tatarubot2/plugins/lottery.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.1/tatarubot2/plugins/market.py` & `tatarubot2-0.1.2/tatarubot2/plugins/market.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.1/tatarubot2/plugins/market_new.py` & `tatarubot2-0.1.2/tatarubot2/plugins/market_new.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.1/tatarubot2/plugins/nuannuan.py` & `tatarubot2-0.1.2/tatarubot2/plugins/nuannuan.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.1/tatarubot2/plugins/precious.py` & `tatarubot2-0.1.2/tatarubot2/plugins/precious.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.1/tatarubot2/plugins/weather.py` & `tatarubot2-0.1.2/tatarubot2/plugins/weather.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.1/tatarubot2/tools/download_boss.py` & `tatarubot2-0.1.2/tatarubot2/tools/download_boss.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.1/tatarubot2/tools/download_item2id.py` & `tatarubot2-0.1.2/tatarubot2/tools/download_item2id.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.1/tatarubot2/tools/normal_data.py` & `tatarubot2-0.1.2/tatarubot2/tools/normal_data.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.1/tatarubot2.egg-info/PKG-INFO` & `tatarubot2-0.1.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 Metadata-Version: 2.1
 Name: tatarubot2
-Version: 0.1.1
-Summary: FF14 bot Tataru
-Author: aaron-li
-Author-email: 
+Version: 0.1.2
+Summary: tatarubot2
+Requires-Python: >=3.7.3,<4.0.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: nonebot2 (>=2.0.0-beta.1,<3.0.0)
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # TataruBot2
 
 基于NoneBot2的FF14机器人塔塔露
 
 ## 当前功能
 
@@ -81,7 +85,8 @@
 NoneBot2官方文档：https://v2.nonebot.dev/
 
 NoneBot2 github：https://github.com/nonebot/nonebot2
 
 go-cqhttp连接配置：https://adapter-onebot.netlify.app/docs/guide/setup
 
 go-cqhttp github：https://github.com/Mrs4s/go-cqhttp
+
```

