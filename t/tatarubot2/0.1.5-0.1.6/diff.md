# Comparing `tmp/tatarubot2-0.1.5.tar.gz` & `tmp/tatarubot2-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tatarubot2-0.1.5.tar", max compression
+gzip compressed data, was "tatarubot2-0.1.6.tar", max compression
```

## Comparing `tatarubot2-0.1.5.tar` & `tatarubot2-0.1.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1066 2022-08-12 03:44:26.000000 tatarubot2-0.1.5/LICENSE
--rw-r--r--   0        0        0     2734 2023-03-14 01:51:48.000000 tatarubot2-0.1.5/README.md
--rw-r--r--   0        0        0      394 2023-04-10 10:17:00.000000 tatarubot2-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-10 10:03:09.000000 tatarubot2-0.1.5/tatarubot2/__init__.py
--rw-r--r--   0        0        0    82117 2023-01-12 06:12:13.000000 tatarubot2-0.1.5/tatarubot2/data/boss.json
--rw-r--r--   0        0        0  1218488 2023-01-30 01:23:59.000000 tatarubot2-0.1.5/tatarubot2/data/item_dict.json
--rw-r--r--   0        0        0     2422 2022-12-26 09:14:52.000000 tatarubot2-0.1.5/tatarubot2/data/job.json
--rw-r--r--   0        0        0       72 2023-04-10 10:16:51.000000 tatarubot2-0.1.5/tatarubot2/plugins/__init__.py
--rw-r--r--   0        0        0      713 2022-11-15 08:07:47.000000 tatarubot2-0.1.5/tatarubot2/plugins/auto_response.py
--rw-r--r--   0        0        0     1627 2023-04-07 06:02:20.000000 tatarubot2-0.1.5/tatarubot2/plugins/bot_help.py
--rw-r--r--   0        0        0     1211 2023-04-07 02:28:25.000000 tatarubot2-0.1.5/tatarubot2/plugins/chat_ai.py
--rw-r--r--   0        0        0     2262 2022-08-16 07:15:05.000000 tatarubot2-0.1.5/tatarubot2/plugins/ff_weibo.py
--rw-r--r--   0        0        0     4409 2022-08-17 03:31:15.000000 tatarubot2-0.1.5/tatarubot2/plugins/house.py
--rw-r--r--   0        0        0    17045 2023-01-29 07:09:23.000000 tatarubot2-0.1.5/tatarubot2/plugins/item.py
--rw-r--r--   0        0        0    17338 2023-04-07 06:02:20.000000 tatarubot2-0.1.5/tatarubot2/plugins/item_new.py
--rw-r--r--   0        0        0     7011 2023-04-07 06:02:20.000000 tatarubot2-0.1.5/tatarubot2/plugins/logs_dps.py
--rw-r--r--   0        0        0     1230 2022-08-12 01:48:07.000000 tatarubot2-0.1.5/tatarubot2/plugins/lottery.py
--rw-r--r--   0        0        0     7754 2022-08-15 08:28:24.000000 tatarubot2-0.1.5/tatarubot2/plugins/market.py
--rw-r--r--   0        0        0     8223 2023-04-07 06:02:20.000000 tatarubot2-0.1.5/tatarubot2/plugins/market_new.py
--rw-r--r--   0        0        0     3103 2022-09-24 04:17:17.000000 tatarubot2-0.1.5/tatarubot2/plugins/nuannuan.py
--rw-r--r--   0        0        0      899 2022-08-12 01:48:15.000000 tatarubot2-0.1.5/tatarubot2/plugins/precious.py
--rw-r--r--   0        0        0     1196 2022-06-23 07:26:19.000000 tatarubot2-0.1.5/tatarubot2/plugins/weather.py
--rw-r--r--   0        0        0        0 2022-08-12 07:58:45.000000 tatarubot2-0.1.5/tatarubot2/tools/__init__.py
--rw-r--r--   0        0        0  1010264 2022-08-12 20:09:39.000000 tatarubot2-0.1.5/tatarubot2/tools/data.json
--rw-r--r--   0        0        0     5058 2023-04-07 06:02:20.000000 tatarubot2-0.1.5/tatarubot2/tools/download_boss.py
--rw-r--r--   0        0        0     1962 2023-01-30 01:23:02.000000 tatarubot2-0.1.5/tatarubot2/tools/download_item2id.py
--rw-r--r--   0        0        0    82117 2023-01-12 06:12:13.000000 tatarubot2-0.1.5/tatarubot2/tools/new_boss.json
--rw-r--r--   0        0        0     2422 2022-12-26 09:13:22.000000 tatarubot2-0.1.5/tatarubot2/tools/new_job.json
--rw-r--r--   0        0        0     1725 2023-04-07 06:02:20.000000 tatarubot2-0.1.5/tatarubot2/tools/normal_data.py
--rw-r--r--   0        0        0     3180 1970-01-01 00:00:00.000000 tatarubot2-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-08-12 03:44:26.000000 tatarubot2-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2734 2023-03-14 01:51:48.000000 tatarubot2-0.1.6/README.md
+-rw-r--r--   0        0        0      424 2023-04-10 14:58:41.000000 tatarubot2-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-10 10:03:09.000000 tatarubot2-0.1.6/tatarubot2/__init__.py
+-rw-r--r--   0        0        0    82117 2023-01-12 06:12:13.000000 tatarubot2-0.1.6/tatarubot2/data/boss.json
+-rw-r--r--   0        0        0  1218488 2023-01-30 01:23:59.000000 tatarubot2-0.1.6/tatarubot2/data/item_dict.json
+-rw-r--r--   0        0        0     2422 2022-12-26 09:14:52.000000 tatarubot2-0.1.6/tatarubot2/data/job.json
+-rw-r--r--   0        0        0     1525 2023-04-10 14:58:41.000000 tatarubot2-0.1.6/tatarubot2/plugins/__init__.py
+-rw-r--r--   0        0        0      713 2022-11-15 08:07:47.000000 tatarubot2-0.1.6/tatarubot2/plugins/auto_response.py
+-rw-r--r--   0        0        0     1627 2023-04-07 06:02:20.000000 tatarubot2-0.1.6/tatarubot2/plugins/bot_help.py
+-rw-r--r--   0        0        0     1211 2023-04-07 02:28:25.000000 tatarubot2-0.1.6/tatarubot2/plugins/chat_ai.py
+-rw-r--r--   0        0        0     2262 2022-08-16 07:15:05.000000 tatarubot2-0.1.6/tatarubot2/plugins/ff_weibo.py
+-rw-r--r--   0        0        0     4409 2022-08-17 03:31:15.000000 tatarubot2-0.1.6/tatarubot2/plugins/house.py
+-rw-r--r--   0        0        0    17045 2023-01-29 07:09:23.000000 tatarubot2-0.1.6/tatarubot2/plugins/item.py
+-rw-r--r--   0        0        0    17442 2023-04-10 14:32:15.000000 tatarubot2-0.1.6/tatarubot2/plugins/item_new.py
+-rw-r--r--   0        0        0     7150 2023-04-10 14:58:41.000000 tatarubot2-0.1.6/tatarubot2/plugins/logs_dps.py
+-rw-r--r--   0        0        0     1230 2022-08-12 01:48:07.000000 tatarubot2-0.1.6/tatarubot2/plugins/lottery.py
+-rw-r--r--   0        0        0     7754 2022-08-15 08:28:24.000000 tatarubot2-0.1.6/tatarubot2/plugins/market.py
+-rw-r--r--   0        0        0     8327 2023-04-10 14:32:15.000000 tatarubot2-0.1.6/tatarubot2/plugins/market_new.py
+-rw-r--r--   0        0        0     3103 2022-09-24 04:17:17.000000 tatarubot2-0.1.6/tatarubot2/plugins/nuannuan.py
+-rw-r--r--   0        0        0      899 2022-08-12 01:48:15.000000 tatarubot2-0.1.6/tatarubot2/plugins/precious.py
+-rw-r--r--   0        0        0     1196 2022-06-23 07:26:19.000000 tatarubot2-0.1.6/tatarubot2/plugins/weather.py
+-rw-r--r--   0        0        0        0 2022-08-12 07:58:45.000000 tatarubot2-0.1.6/tatarubot2/tools/__init__.py
+-rw-r--r--   0        0        0  1010264 2022-08-12 20:09:39.000000 tatarubot2-0.1.6/tatarubot2/tools/data.json
+-rw-r--r--   0        0        0     5058 2023-04-07 06:02:20.000000 tatarubot2-0.1.6/tatarubot2/tools/download_boss.py
+-rw-r--r--   0        0        0     1962 2023-01-30 01:23:02.000000 tatarubot2-0.1.6/tatarubot2/tools/download_item2id.py
+-rw-r--r--   0        0        0    82117 2023-01-12 06:12:13.000000 tatarubot2-0.1.6/tatarubot2/tools/new_boss.json
+-rw-r--r--   0        0        0     2422 2022-12-26 09:13:22.000000 tatarubot2-0.1.6/tatarubot2/tools/new_job.json
+-rw-r--r--   0        0        0     1725 2023-04-07 06:02:20.000000 tatarubot2-0.1.6/tatarubot2/tools/normal_data.py
+-rw-r--r--   0        0        0     3226 1970-01-01 00:00:00.000000 tatarubot2-0.1.6/PKG-INFO
```

### Comparing `tatarubot2-0.1.5/LICENSE` & `tatarubot2-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.5/README.md` & `tatarubot2-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.5/tatarubot2/data/boss.json` & `tatarubot2-0.1.6/tatarubot2/data/boss.json`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.5/tatarubot2/data/item_dict.json` & `tatarubot2-0.1.6/tatarubot2/data/item_dict.json`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.5/tatarubot2/data/job.json` & `tatarubot2-0.1.6/tatarubot2/data/job.json`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.5/tatarubot2/plugins/auto_response.py` & `tatarubot2-0.1.6/tatarubot2/plugins/auto_response.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.5/tatarubot2/plugins/bot_help.py` & `tatarubot2-0.1.6/tatarubot2/plugins/bot_help.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.5/tatarubot2/plugins/chat_ai.py` & `tatarubot2-0.1.6/tatarubot2/plugins/chat_ai.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.5/tatarubot2/plugins/ff_weibo.py` & `tatarubot2-0.1.6/tatarubot2/plugins/ff_weibo.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.5/tatarubot2/plugins/house.py` & `tatarubot2-0.1.6/tatarubot2/plugins/house.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.5/tatarubot2/plugins/item.py` & `tatarubot2-0.1.6/tatarubot2/plugins/item.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.5/tatarubot2/plugins/item_new.py` & `tatarubot2-0.1.6/tatarubot2/plugins/item_new.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from nonebot import on_command
 from nonebot.adapters.onebot.v11 import Message, MessageSegment
 from nonebot.rule import to_me
 from nonebot.typing import T_State
 from nonebot.adapters import Bot, Event
 
+import os
 import re
 import base64
 import json
 import requests
 import urllib
 import logging
 import traceback
@@ -78,15 +79,17 @@
     'Fast': '快',
     'Very Fast': '非常快',
     'V. Fast': '非常快'
 }
 
 # 加载字典
 item_dict = {}
-with open("tatarubot2/data/item_dict.json", "r", encoding="utf-8") as f_r:
+this_dir = os.path.split(os.path.realpath(__file__))[0]
+json_path = os.path.join(this_dir, "../data/item_dict.json")
+with open(json_path, "r", encoding="utf-8") as f_r:
     for line in f_r.readlines():
         item_dict = eval(line)
 # print(item_dict)
 
 
 def craft_garland_url(item_category, item_id, name_lang):
     is_cn = (name_lang == "chs")
```

### Comparing `tatarubot2-0.1.5/tatarubot2/plugins/logs_dps.py` & `tatarubot2-0.1.6/tatarubot2/plugins/logs_dps.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 
 from nonebot import on_command
 from nonebot.rule import to_me
 from nonebot.typing import T_State
 from nonebot.adapters import Bot, Event
 
-
+import os
 import requests
 import re
 import traceback
 import base64
 import json
 import urllib
 import logging
@@ -27,17 +27,20 @@
 
 async def logs_dps_help():
     return this_command + "boss名 职业名 (国服) (rdps) (day2):\n" \
            "查询logs上对应boss和职业的dps分段，括号内为可选的参数，默认国际服、adps、截止最后一天"
 
 
 # 加载职业和boss信息
-with open("tatarubot2/data/job.json", "r", encoding="utf-8") as j_r:
+this_dir = os.path.split(os.path.realpath(__file__))[0]
+job_path = os.path.join(this_dir, "../data/job.json")
+boss_path = os.path.join(this_dir, "../data/boss.json")
+with open(job_path, "r", encoding="utf-8") as j_r:
     data_job = json.load(j_r)
-with open("tatarubot2/data/boss.json", "r", encoding="utf-8") as b_r:
+with open(boss_path, "r", encoding="utf-8") as b_r:
     data_boss = json.load(b_r)
 
 
 # 检查是哪个职业
 def check_job(job):
     for j in data_job:
         if job == j["name"] or job == j["cn_name"] or job in j["nickname"]:
```

### Comparing `tatarubot2-0.1.5/tatarubot2/plugins/lottery.py` & `tatarubot2-0.1.6/tatarubot2/plugins/lottery.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.5/tatarubot2/plugins/market.py` & `tatarubot2-0.1.6/tatarubot2/plugins/market.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.5/tatarubot2/plugins/market_new.py` & `tatarubot2-0.1.6/tatarubot2/plugins/market_new.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 
 from nonebot import on_command
 from nonebot.rule import to_me
 from nonebot.typing import T_State
 from nonebot.adapters import Bot, Event
 
+import os
 import requests
 from difflib import SequenceMatcher
 import re
 import time
 import random
 
 this_command = "新价格 "
@@ -20,15 +21,17 @@
 # 超时时间
 time_out = 60
 # 重试次数
 retry_num = 20
 
 # 加载字典
 item_dict = {}
-with open("tatarubot2/data/item_dict.json", "r", encoding="utf-8") as f_r:
+this_dir = os.path.split(os.path.realpath(__file__))[0]
+json_path = os.path.join(this_dir, "../data/item_dict.json")
+with open(json_path, "r", encoding="utf-8") as f_r:
     for line in f_r.readlines():
         item_dict = eval(line)
 
 
 # 减少requests错误
 def get_headers():
     agent = ['Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 '
```

### Comparing `tatarubot2-0.1.5/tatarubot2/plugins/nuannuan.py` & `tatarubot2-0.1.6/tatarubot2/plugins/nuannuan.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.5/tatarubot2/plugins/precious.py` & `tatarubot2-0.1.6/tatarubot2/plugins/precious.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.5/tatarubot2/plugins/weather.py` & `tatarubot2-0.1.6/tatarubot2/plugins/weather.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.5/tatarubot2/tools/data.json` & `tatarubot2-0.1.6/tatarubot2/tools/data.json`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.5/tatarubot2/tools/download_boss.py` & `tatarubot2-0.1.6/tatarubot2/tools/download_boss.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.5/tatarubot2/tools/download_item2id.py` & `tatarubot2-0.1.6/tatarubot2/tools/download_item2id.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.5/tatarubot2/tools/new_boss.json` & `tatarubot2-0.1.6/tatarubot2/tools/new_boss.json`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.5/tatarubot2/tools/new_job.json` & `tatarubot2-0.1.6/tatarubot2/tools/new_job.json`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.5/tatarubot2/tools/normal_data.py` & `tatarubot2-0.1.6/tatarubot2/tools/normal_data.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.5/PKG-INFO` & `tatarubot2-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: tatarubot2
-Version: 0.1.5
-Summary: tatarubot2
+Version: 0.1.6
+Summary: FF14 bot Tataru
+Author: aaron-li
 Requires-Python: >=3.7.3,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: nonebot2 (>=2.0.0-beta.1,<3.0.0)
+Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # TataruBot2
 
 基于NoneBot2的FF14机器人塔塔露
 
 ## 当前功能
```

