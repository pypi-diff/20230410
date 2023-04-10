# Comparing `tmp/nonebot_plugin_blive_danmaku-0.1.3.tar.gz` & `tmp/nonebot_plugin_blive_danmaku-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_blive_danmaku-0.1.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_blive_danmaku-0.1.4.tar", max compression
```

## Comparing `nonebot_plugin_blive_danmaku-0.1.3.tar` & `nonebot_plugin_blive_danmaku-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,34 @@
--rw-r--r--   0        0        0     1085 2023-04-07 16:32:26.658635 nonebot_plugin_blive_danmaku-0.1.3/LICENSE
--rw-r--r--   0        0        0      127 2023-04-07 18:53:54.995600 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/__init__.py
--rw-r--r--   0        0        0       32 2023-04-04 00:23:10.472267 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/.git
--rw-r--r--   0        0        0       68 2023-04-04 00:23:14.371312 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/.gitattributes
--rw-r--r--   0        0        0     1260 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/.gitignore
--rw-r--r--   0        0        0       96 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/blivedm/__init__.py
--rw-r--r--   0        0        0    21920 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py
--rw-r--r--   0        0        0     5365 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py
--rw-r--r--   0        0        0    12447 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py
--rw-r--r--   0        0        0     1084 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/LICENSE
--rw-r--r--   0        0        0      457 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/README.md
--rw-r--r--   0        0        0       31 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/requirements.txt
--rw-r--r--   0        0        0     2928 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/sample.py
--rw-r--r--   0        0        0       67 2023-04-07 19:00:18.585303 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/__init__.py
--rw-r--r--   0        0        0     3111 2023-04-08 17:55:07.052693 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/pusher.py
--rw-r--r--   0        0        0     1407 2023-04-07 18:48:25.619184 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/sub_add.py
--rw-r--r--   0        0        0     1396 2023-04-07 18:49:55.897456 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/sub_delete.py
--rw-r--r--   0        0        0      916 2023-04-07 18:53:16.447915 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/sub_list.py
--rw-r--r--   0        0        0      829 2023-04-07 18:52:14.308552 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/sub_off.py
--rw-r--r--   0        0        0      820 2023-04-07 18:50:57.288389 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/sub_on.py
--rw-r--r--   0        0        0       18 2023-04-07 06:14:41.544558 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/database/__init__.py
--rw-r--r--   0        0        0     1953 2023-04-07 19:33:48.683619 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/database/db.py
--rw-r--r--   0        0        0     1330 2023-04-07 05:20:29.198527 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/database/model.py
--rw-r--r--   0        0        0     3752 2023-04-08 17:54:45.409318 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/utils/__init__.py
--rw-r--r--   0        0        0      950 2023-04-08 19:06:24.287928 nonebot_plugin_blive_danmaku-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1738 2023-04-08 19:03:48.106577 nonebot_plugin_blive_danmaku-0.1.3/README.md
--rw-r--r--   0        0        0     2797 1970-01-01 00:00:00.000000 nonebot_plugin_blive_danmaku-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-07 16:32:26.658635 nonebot_plugin_blive_danmaku-0.1.4/LICENSE
+-rw-r--r--   0        0        0      127 2023-04-07 18:53:54.995600 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/__init__.py
+-rw-r--r--   0        0        0       32 2023-04-04 00:23:10.472267 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/.git
+-rw-r--r--   0        0        0       68 2023-04-04 00:23:14.371312 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/.gitattributes
+-rw-r--r--   0        0        0     1260 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/.gitignore
+-rw-r--r--   0        0        0       96 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/blivedm/__init__.py
+-rw-r--r--   0        0        0    21920 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py
+-rw-r--r--   0        0        0     5365 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py
+-rw-r--r--   0        0        0    12447 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py
+-rw-r--r--   0        0        0     1084 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/LICENSE
+-rw-r--r--   0        0        0      457 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/README.md
+-rw-r--r--   0        0        0       31 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/requirements.txt
+-rw-r--r--   0        0        0     2928 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/sample.py
+-rw-r--r--   0        0        0       99 2023-04-10 07:39:11.035690 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 17:28:27.970418 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/live/__init__.py
+-rw-r--r--   0        0        0      848 2023-04-09 17:33:40.134826 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/live/live_off.py
+-rw-r--r--   0        0        0      847 2023-04-09 17:32:58.298393 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/live/live_on.py
+-rw-r--r--   0        0        0        0 2023-04-09 17:26:16.349686 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/sub/__init__.py
+-rw-r--r--   0        0        0     1421 2023-04-09 17:51:35.475589 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/sub/sub_add.py
+-rw-r--r--   0        0        0     1398 2023-04-09 17:27:28.520785 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py
+-rw-r--r--   0        0        0      980 2023-04-09 17:52:09.092145 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/sub/sub_list.py
+-rw-r--r--   0        0        0      831 2023-04-09 17:27:43.407410 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/sub/sub_off.py
+-rw-r--r--   0        0        0      822 2023-04-09 17:27:52.919328 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/sub/sub_on.py
+-rw-r--r--   0        0        0        0 2023-04-10 07:19:16.340181 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/subscribe/__init__.py
+-rw-r--r--   0        0        0     3671 2023-04-10 09:03:17.352805 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py
+-rw-r--r--   0        0        0     2645 2023-04-10 15:15:45.271259 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/subscribe/live.py
+-rw-r--r--   0        0        0      261 2023-04-10 15:15:41.674275 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/config.py
+-rw-r--r--   0        0        0       18 2023-04-07 06:14:41.544558 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/database/__init__.py
+-rw-r--r--   0        0        0     2830 2023-04-10 15:01:41.440478 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/database/db.py
+-rw-r--r--   0        0        0     1984 2023-04-10 14:49:04.632614 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/database/model.py
+-rw-r--r--   0        0        0     3870 2023-04-10 13:46:27.863711 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/utils/__init__.py
+-rw-r--r--   0        0        0      950 2023-04-09 16:52:22.392021 nonebot_plugin_blive_danmaku-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2835 2023-04-10 17:47:03.111172 nonebot_plugin_blive_danmaku-0.1.4/README.md
+-rw-r--r--   0        0        0     3869 1970-01-01 00:00:00.000000 nonebot_plugin_blive_danmaku-0.1.4/PKG-INFO
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.3/LICENSE` & `nonebot_plugin_blive_danmaku-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/.gitignore` & `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/.gitignore`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py` & `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py` & `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py` & `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/LICENSE` & `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/sample.py` & `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/sample.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/pusher.py` & `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import time
 import asyncio
 from bilireq.live import get_rooms_info_by_uids, get_room_info_by_id
-from ..utils import send_msg, get_timespan, get_time_difference
-from ..blivedm import blivedm
-from ..database import Db as db
+from ...utils import send_msg, get_timespan, get_time_difference, scheduler
+from ...blivedm import blivedm
+from ...database import Db as db
 from nonebot.log import logger
-from nonebot import require, get_driver
-require("nonebot_plugin_apscheduler")
-from nonebot_plugin_apscheduler import scheduler
 
 
 class ClientModel:
     def __init__(self, room_id):
         self.uid=""
         self.name=""
         self.live_time=0
@@ -22,23 +19,23 @@
 
 
 @scheduler.scheduled_job(
     "interval", seconds=15, id="street_lamp_sched"
 )
 async def danmaku():
     """ 连接直播间 """
-    uids = db.get_sub_list()
+    uids = db.get_sub_list("street_lamp")
 
     if not uids:
         return
     
     res = await get_rooms_info_by_uids(uids, reqtype="web", proxies=None)
     if not res:
         return
-    logger.info(f'爬取路灯列表')
+    logger.debug(f'爬取路灯列表')
     handler = MsgHandler()
     for uid, info in res.items():
         new_status = 0 if info["live_status"] == 2 else info["live_status"]
         index = [x for x in clients if x.uid == uid]
         if not index:
             if new_status:
                 logger.info(f'{info["uname"]}开播了，连接直播间')
@@ -57,24 +54,41 @@
                 client = model.client
                 try:
                     asyncio.gather(client.join())
                 finally:
                     await asyncio.gather(client.stop_and_close())
                     clients.remove(model)
                     logger.info(f'{info["uname"]}下播了，断开直播间连接')
+
     
 
 class MsgHandler(blivedm.BaseHandler):
     async def _on_danmaku(self, client: blivedm.BLiveClient, message: blivedm.DanmakuMessage):
         if(message.msg.startswith("#路灯")):
+            logger.info(f'{client.room_owner_uid}的直播间收到路灯：{message.uname} -> {message.msg}')
             subs = await db.get_subs(uid=client.room_owner_uid)
             if not subs:
                 return
             for sub in subs:
                 index = [x for x in clients if x.uid == str(sub.uid)]
+                if not index:
+                    continue
                 model = index[0]
-                logger.info(f'{model.name}的直播间收到路灯：{message.uname} -> {message.msg}')
+                if sub.street_lamp is False:
+                    await disconnect_room(model)
+                    continue
                 dt = get_time_difference(model.live_time)
                 datetime = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
-                msg = f'【{model.name}】 在 {datetime}({dt}) 收到了 {message.uname} 发来的路灯【{message.msg.replace("#路灯","", 1).strip()}】'
+                blive_danmaku = message.msg.replace("#路灯","", 1).strip()
+                msg = f'【{model.name}】 在 {datetime}({dt}) 收到了 {message.uname} 发来的路灯【{blive_danmaku}】'
                 await send_msg(bot_id=sub.bot_id,send_type=sub.type,type_id=sub.type_id,message=msg)
+                await db.add_danmaku(room_id=client.room_id, uname=message.uname, message=blive_danmaku, create_time=datetime, live_duration=dt)
+
 
+async def disconnect_room(model):
+    client = model.client
+    try:
+        asyncio.gather(client.join())
+    finally:
+        await asyncio.gather(client.stop_and_close())
+        clients.remove(model)
+        logger.info(f'{model.name} 断开直播间连接')
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/sub_add.py` & `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/sub/sub_add.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from ..database import Db as db
+from ...database import Db as db
 from nonebot.adapters.onebot.v11.event import MessageEvent
 from nonebot.params import ArgPlainText
 from nonebot import on_command
-from ..utils import get_type_id,handle_uid,permission_check,uid_check
+from ...utils import get_type_id,handle_uid,permission_check,uid_check
 from bilireq.user import get_user_info
 from bilireq.exceptions import ResponseCodeError
 
 sub_add = on_command("添加订阅", priority=5)
 sub_add.__doc__ = """添加订阅 UID"""
 sub_add.handle()(permission_check)
 sub_add.handle()(handle_uid)
@@ -21,12 +21,12 @@
     except ResponseCodeError as ex:
         if ex.code == -400 or ex.code == -404:
             await sub_add.finish(f"UID {uid}不存在，请检查后重试")
         elif ex.code == -412:
             await sub_add.finish(f"操作过于频繁，请半小时后再试")
         else:
             await sub_add.finish("发送未知错误")
-    res = await db.add_sub(uid=uid, type=event.message_type, type_id=type_id, street_lamp=True, bot_id=event.self_id)
+    res = await db.add_sub(uid=uid, type=event.message_type, type_id=type_id, street_lamp=True, live=False, bot_id=event.self_id)
     name = user["name"]
     if res:
         await sub_add.finish(f"添加订阅 {name}({uid}) 成功")
     await sub_add.finish(f"{name}({uid}) 已经订阅")
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/sub_delete.py` & `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from nonebot.adapters.onebot.v11.event import MessageEvent
 from nonebot.params import ArgPlainText
 from nonebot import on_command
-from ..utils import get_type_id,handle_uid,permission_check,uid_check
+from ...utils import get_type_id,handle_uid,permission_check,uid_check
 from bilireq.user import get_user_info
 from bilireq.exceptions import ResponseCodeError
-from ..database import Db as db
+from ...database import Db as db
 
 sub_delete = on_command("取消订阅", priority=5)
 sub_delete.__doc__ = """取消订阅 UID"""
 sub_delete.handle()(permission_check)
 sub_delete.handle()(handle_uid)
 sub_delete.got("uid", prompt="请输入一个UID")(uid_check)
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/sub_list.py` & `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/sub/sub_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from nonebot.adapters.onebot.v11.event import MessageEvent
 from nonebot.adapters.onebot.v11 import Bot
 from nonebot import on_command
-from ..utils import get_type_id,permission_check
+from ...utils import get_type_id,permission_check
 from bilireq.user import get_user_info
-from ..database import Db as db
+from ...database import Db as db
 
 
 sub_list = on_command("订阅列表", priority=5)
 sub_list.__doc__ = """订阅列表"""
 sub_list.handle()(permission_check)
 
 @sub_list.handle()
@@ -18,9 +18,10 @@
     msg = "订阅列表：\n\n"
     for sub in subs:
         user = await get_user_info(sub.uid, reqtype="web", proxies=None)
         name = user["name"]
         msg += (
             f"{name}({sub.uid})"
             f"路灯：{'开' if sub.street_lamp else '关'}"
+            f"开播提醒：{'开' if sub.live else '关'}"
         )
     await sub_list.finish(msg)
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/sub_off.py` & `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/sub/sub_off.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from nonebot.adapters.onebot.v11.event import MessageEvent
 from nonebot.params import ArgPlainText
 from nonebot import on_command
-from ..utils import get_type_id,handle_uid,permission_check,uid_check
-from ..database import Db as db
+from ...utils import get_type_id,handle_uid,permission_check,uid_check
+from ...database import Db as db
 
 sub_off = on_command("关闭路灯", priority=5)
 sub_off.__doc__ = """关闭路灯 UID"""
 sub_off.handle()(permission_check)
 sub_off.handle()(handle_uid)
 sub_off.got("uid", prompt="请输入一个UID")(uid_check)
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/sub_on.py` & `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/sub/sub_on.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from nonebot.adapters.onebot.v11.event import MessageEvent
 from nonebot.params import ArgPlainText
 from nonebot import on_command
-from ..utils import get_type_id,handle_uid,permission_check,uid_check
-from ..database import Db as db
+from ...utils import get_type_id,handle_uid,permission_check,uid_check
+from ...database import Db as db
 
 sub_on = on_command("开启路灯", priority=5)
 sub_on.__doc__ = """开启路灯 UID"""
 sub_on.handle()(permission_check)
 sub_on.handle()(handle_uid)
 sub_on.got("uid", prompt="请输入一个UID")(uid_check)
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/utils/__init__.py` & `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/utils/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -105,7 +105,10 @@
     now = int(time.time())
     sub = now - live_time
     m, s = divmod(sub, 60)
     h, m = divmod(m, 60)
     dt = ("%02d:%02d:%02d" % (h, m, s))
     return dt
 
+from nonebot import require
+require("nonebot_plugin_apscheduler")
+from nonebot_plugin_apscheduler import scheduler
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.3/pyproject.toml` & `nonebot_plugin_blive_danmaku-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-blive-danmaku"
-version = "0.1.3"
+version = "0.1.4"
 description = "A danmaku plugin for Nonebot2"
 authors = ["ricardo <thespirit@vip.qq.com>"]
 documentation = "https://github.com/zangxx66/nonebot_plugin_blive_danmaku#readme"
 license = "MIT"
 homepage = "https://github.com/zangxx66/nonebot_plugin_blive_danmaku"
 readme = "README.md"
 keywords = ["nonebot", "nonebot2", "bilibili", "danmaku"]
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.3/README.md` & `nonebot_plugin_blive_danmaku-0.1.4/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,109 +1,178 @@
-00000000: 2320 6e6f 6e65 626f 745f 706c 7567 696e  # nonebot_plugin
-00000010: 5f62 6c69 7665 5f64 616e 6d61 6b75 0d0a  _blive_danmaku..
-00000020: 2d20 e59f bae4 ba8e 5b6e 6f6e 6562 6f74  - ......[nonebot
-00000030: 325d 2868 7474 7073 3a2f 2f76 322e 6e6f  2](https://v2.no
-00000040: 6e65 626f 742e 6465 762f 29e5 bc80 e58f  nebot.dev/).....
-00000050: 91e7 9a84 42e7 ab99 e79b b4e6 92ad e997  ....B...........
-00000060: b4e5 bcb9 e5b9 95e7 9b91 e590 ac42 6f74  .............Bot
-00000070: efbc 8ce5 8f82 e880 83e4 ba86 4861 7275  ............Haru
-00000080: 6b61 e592 8c62 6c69 7665 6368 6174 e79a  ka...blivechat..
-00000090: 84e9 83a8 e588 86e4 bba3 e7a0 81e3 8082  ................
-000000a0: 2020 0d0a 2d20 e8b5 b7e6 ba90 e4ba 8e5b    ..- .........[
-000000b0: e593 88e9 b9bf 6861 6c6c 755d 2868 7474  ......hallu](htt
-000000c0: 7073 3a2f 2f73 7061 6365 2e62 696c 6962  ps://space.bilib
-000000d0: 696c 692e 636f 6d2f 3334 3933 3131 3834  ili.com/34931184
-000000e0: 3934 3131 3637 3937 29e7 9a84 e4b8 80e6  94116797).......
-000000f0: 9da1 e58a a8e6 8081 efbc 8ce8 8ba6 e4ba  ................
-00000100: 8ee5 819a e8a7 86e9 a291 e697 b6e6 b2a1  ................
-00000110: e69c 89e4 baba e581 9ae8 b7af e781 afef  ................
-00000120: bc8c e7bf bbe5 bd95 e692 ade7 9a84 e697  ................
-00000130: b6e5 8099 e5a4 b4e9 83bd e5a4 a7e4 ba86  ................
-00000140: efbc 8ce8 afb4 e8a6 81e8 8ab1 e992 b1e8  ................
-00000150: afb7 e4b8 aae5 85a8 e881 8ce8 b7af e781  ................
-00000160: afef bc8c e688 91e5 afbb e680 9de4 b88e  ................
-00000170: e585 b6e6 8a8a e992 b1e9 8081 e7bb 99e5  ................
-00000180: 88ab e4ba baef bc8c e4b8 8de5 a682 e4ba  ................
-00000190: a4e7 bb99 426f 74e5 8ebb e581 9ae8 b7af  ....Bot.........
-000001a0: e781 afe3 8082 0d0a 3c63 656e 7465 723e  ........<center>
-000001b0: 3c69 6d61 6765 2073 7263 3d22 2f64 6f63  <image src="/doc
-000001c0: 2f73 6372 6565 6e73 686f 7431 2e70 6e67  /screenshot1.png
-000001d0: 223e 3c2f 696d 6167 653e 3c2f 6365 6e74  "></image></cent
-000001e0: 6572 3e0d 0a2d 20e8 b7af e781 afef bc9a  er>..- .........
-000001f0: e68c 87e6 8a8a e79b b4e6 92ad e8bf 87e7  ................
-00000200: a88b e4b8 ade6 9c89 e8b6 a3e7 9a84 e782  ................
-00000210: b9e8 aeb0 e5bd 95e4 b88b e69d a5ef bc8c  ................
-00000220: e7bb 99e5 89aa e8be 91e6 a0b9 e68d aee8  ................
-00000230: aeb0 e5bd 95e7 9a84 e697 b6e9 97b4 e782  ................
-00000240: b9e5 928c e586 85e5 aeb9 e581 9ae5 87ba  ................
-00000250: e5af b9e5 ba94 e79a 84e8 a786 e9a2 91e3  ................
-00000260: 8082 0d0a 0d0a 2323 20e5 8a9f e883 bd0d  ......## .......
-00000270: 0a0d 0a2d 20e7 94a8 e5bc b9e5 b995 e79a  ...- ...........
-00000280: 84e5 bda2 e5bc 8fe8 aeb0 e5bd 95e7 9bb4  ................
-00000290: e692 ade9 ab98 e883 bde7 82b9 0d0a 2d20  ..............- 
-000002a0: e5bc b9e5 b995 e68c 87e4 bba4 e4b8 ba60  ...............`
-000002b0: 23e8 b7af e781 af60 e58a a0e4 b88a e8ae  #......`........
-000002c0: b0e5 bd95 e79a 84e5 8685 e5ae b90d 0a2d  ...............-
-000002d0: 20e4 bb85 e59c a8e5 bc80 e692 ade6 97b6   ...............
-000002e0: e5bc b9e5 b995 e68c 87e4 bba4 e689 8de4  ................
-000002f0: bc9a e794 9fe6 9588 0d0a 0d0a 2323 20e5  ............## .
-00000300: ae89 e8a3 850d 0a2d 2050 7974 686f 6e20  .......- Python 
-00000310: 3e3d 2033 2e31 300d 0a2d 20e6 96b9 e5bc  >= 3.10..- .....
-00000320: 8fe4 b880 efbc 9ae4 bdbf e794 a860 6e62  .............`nb
-00000330: 2d63 6c69 60e5 ae89 e8a3 85e6 8f92 e4bb  -cli`...........
-00000340: b620 200d 0a60 6060 0d0a 6e62 2070 6c75  .  ..```..nb plu
-00000350: 6769 6e20 696e 7374 616c 6c20 6e6f 6e65  gin install none
-00000360: 626f 742d 706c 7567 696e 2d62 6c69 7665  bot-plugin-blive
-00000370: 2d64 616e 6d61 6b75 0d0a 6060 600d 0a2d  -danmaku..```..-
-00000380: 20e6 96b9 e5bc 8fe4 ba8c efbc 9ae4 bdbf   ...............
-00000390: e794 a860 7069 7060 e5ae 89e8 a385 0d0a  ...`pip`........
-000003a0: 6060 600d 0a70 7974 686f 6e20 2d6d 2070  ```..python -m p
-000003b0: 6970 2069 6e73 7461 6c6c 206e 6f6e 6562  ip install noneb
-000003c0: 6f74 2d70 6c75 6769 6e2d 626c 6976 652d  ot-plugin-blive-
-000003d0: 6461 6e6d 616b 750d 0a60 6060 0d0a 0d0a  danmaku..```....
-000003e0: 2323 20e6 8c87 e4bb a40d 0a0d 0a7c e68c  ## ..........|..
-000003f0: 87e4 bba4 7ce8 afb4 e698 8e7c 0d0a 7c2d  ....|......|..|-
-00000400: 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 7c0d 0a7c  -----|------|..|
-00000410: 2fe6 b7bb e58a a0e8 aea2 e998 8520 5549  /............ UI
-00000420: 447c 5549 44e4 b8ba 42e7 ab99 e794 a8e6  D|UID...B.......
-00000430: 88b7 e79a 8475 6964 efbc 8ce4 b88d e698  .....uid........
-00000440: afe7 9bb4 e692 ade9 97b4 6964 efbc 8ce4  ..........id....
-00000450: bba5 e4b8 8be5 908c e790 867c 0d0a 7c2f  ...........|..|/
-00000460: e58f 96e6 b688 e8ae a2e9 9885 2055 4944  ............ UID
-00000470: 7ce5 88a0 e999 a4e8 aea2 e998 857c 0d0a  |............|..
-00000480: 7c2f e5bc 80e5 90af e8b7 afe7 81af 2055  |/............ U
-00000490: 4944 7ce5 bc80 e590 afe7 9bb4 e692 ade9  ID|.............
-000004a0: 97b4 e5bc b9e5 b995 e79b 91e5 90ac 7c0d  ..............|.
-000004b0: 0a7c 2fe5 85b3 e997 ade8 b7af e781 af20  .|/............ 
-000004c0: 5549 447c e585 b3e9 97ad e79b b4e6 92ad  UID|............
-000004d0: e997 b4e5 bcb9 e5b9 95e7 9b91 e590 ac7c  ...............|
-000004e0: 0d0a 7c2f e8ae a2e9 9885 e588 97e8 a1a8  ..|/............
-000004f0: 7c7c 200d 0a0d 0a23 2320 e695 88e6 9e9c  || ....## ......
-00000500: e9a2 84e8 a788 200d 0a0d 0a21 5b5d 282f  ...... ....![](/
-00000510: 646f 632f 7363 7265 656e 7368 6f74 2e70  doc/screenshot.p
-00000520: 6e67 290d 0a0d 0a23 2320 e69b b4e6 96b0  ng)....## ......
-00000530: e697 a5e5 bf97 2020 0d0a 2d20 7630 2e31  ......  ..- v0.1
-00000540: 2e33 0d0a 2020 2020 2d20 626f 74e6 8f90  .3..    - bot...
-00000550: e986 92e5 9ca8 e697 b6e9 97b4 e590 8ee9  ................
-00000560: 9da2 e58a a0e4 b88a e79b b4e6 92ad e697  ................
-00000570: b6e9 95bf e698 bee7 a4ba efbc 8ce9 81bf  ................
-00000580: e585 8de7 9bb4 e692 ade7 94bb e99d a2e6  ................
-00000590: b2a1 e69c 89e5 bd93 e589 8de6 97b6 e997  ................
-000005a0: b4e7 9a84 e59c bae6 99af 0d0a 2d20 7630  ............- v0
-000005b0: 2e31 2e32 0d0a 2020 2020 2d20 6669 78e5  .1.2..    - fix.
-000005c0: b180 e983 a8e5 8f98 e987 8fe6 97a0 e6b3  ................
-000005d0: 95e6 ada3 e5b8 b8e6 9bb4 e696 b0e7 9a84  ................
-000005e0: 6275 670d 0a2d 2076 302e 312e 300d 0a20  bug..- v0.1.0.. 
-000005f0: 2020 202d 20e5 9fba e4ba 8e6e 6f6e 6562     - ......noneb
-00000600: 6f74 32ef bc8c e5ae 9ee7 8eb0 e590 8ce6  ot2.............
-00000610: ada5 e8b7 afe7 81af e5bc b9e5 b995 e588  ................
-00000620: b071 71e7 bea4 2020 0d0a 0d0a 2323 20e6  .qq...  ....## .
-00000630: 849f e8b0 a20d 0a2d 205b 4861 7275 6b61  .......- [Haruka
-00000640: 426f 745d 2868 7474 7073 3a2f 2f67 6974  Bot](https://git
-00000650: 6875 622e 636f 6d2f 534b 2d34 3135 2f48  hub.com/SK-415/H
-00000660: 6172 756b 6142 6f74 290d 0a2d 205b 626c  arukaBot)..- [bl
-00000670: 6976 6563 6861 745d 2868 7474 7073 3a2f  ivechat](https:/
-00000680: 2f67 6974 6875 622e 636f 6d2f 7866 6772  /github.com/xfgr
-00000690: 7975 6a6b 2f62 6c69 7665 6368 6174 290d  yujk/blivechat).
-000006a0: 0a2d 205b 6e6f 6e65 626f 7432 5d28 6874  .- [nonebot2](ht
-000006b0: 7470 733a 2f2f 7632 2e6e 6f6e 6562 6f74  tps://v2.nonebot
-000006c0: 2e64 6576 2f29 0d0a 0d0a                 .dev/)....
+00000000: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+00000010: 6572 223e 0d0a 2020 3c61 2068 7265 663d  er">..  <a href=
+00000020: 2268 7474 7073 3a2f 2f76 322e 6e6f 6e65  "https://v2.none
+00000030: 626f 742e 6465 762f 7374 6f72 6522 3e3c  bot.dev/store"><
+00000040: 696d 6720 7372 633d 2264 6f63 2f6e 6270  img src="doc/nbp
+00000050: 5f6c 6f67 6f2e 706e 6722 2077 6964 7468  _logo.png" width
+00000060: 3d22 3138 3022 2068 6569 6768 743d 2231  ="180" height="1
+00000070: 3830 2220 616c 743d 224e 6f6e 6542 6f74  80" alt="NoneBot
+00000080: 506c 7567 696e 4c6f 676f 223e 3c2f 613e  PluginLogo"></a>
+00000090: 0d0a 2020 3c62 723e 0d0a 2020 3c70 3e3c  ..  <br>..  <p><
+000000a0: 696d 6720 7372 633d 2264 6f63 2f4e 6f6e  img src="doc/Non
+000000b0: 6542 6f74 506c 7567 696e 2e73 7667 2220  eBotPlugin.svg" 
+000000c0: 7769 6474 683d 2232 3430 2220 616c 743d  width="240" alt=
+000000d0: 224e 6f6e 6542 6f74 506c 7567 696e 5465  "NoneBotPluginTe
+000000e0: 7874 223e 3c2f 703e 0d0a 3c2f 6469 763e  xt"></p>..</div>
+000000f0: 0d0a 0d0a 3c64 6976 2061 6c69 676e 3d22  ....<div align="
+00000100: 6365 6e74 6572 223e 2020 0d0a 0d0a 2320  center">  ....# 
+00000110: 6e6f 6e65 626f 745f 706c 7567 696e 5f62  nonebot_plugin_b
+00000120: 6c69 7665 5f64 616e 6d61 6b75 2020 0d0a  live_danmaku  ..
+00000130: 0d0a 5ff0 9f92 ab20 42e7 ab99 e79b b4e6  .._.... B.......
+00000140: 92ad e997 b4e8 b7af e781 afe6 8f92 e4bb  ................
+00000150: b620 f09f 92ab 5f20 0d0a 0d0a 5b21 5b70  . ...._ ....[![p
+00000160: 7970 695d 2868 7474 7073 3a2f 2f69 6d67  ypi](https://img
+00000170: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00000180: 2f76 2f6e 6f6e 6562 6f74 2d70 6c75 6769  /v/nonebot-plugi
+00000190: 6e2d 626c 6976 652d 6461 6e6d 616b 752e  n-blive-danmaku.
+000001a0: 7376 6729 5d28 6874 7470 733a 2f2f 7079  svg)](https://py
+000001b0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f6e  pi.org/project/n
+000001c0: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 626c  onebot-plugin-bl
+000001d0: 6976 652d 6461 6e6d 616b 752f 2920 2021  ive-danmaku/)  !
+000001e0: 5b70 7974 686f 6e5d 2868 7474 7073 3a2f  [python](https:/
+000001f0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000200: 7079 7069 2f70 7976 6572 7369 6f6e 732f  pypi/pyversions/
+00000210: 6e6f 6e65 626f 742d 706c 7567 696e 2d62  nonebot-plugin-b
+00000220: 6c69 7665 2d64 616e 6d61 6b75 2920 205b  live-danmaku)  [
+00000230: 215b 6c69 6365 6e73 655d 2868 7474 7073  ![license](https
+00000240: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000250: 6f2f 6769 7468 7562 2f6c 6963 656e 7365  o/github/license
+00000260: 2f7a 616e 6778 7836 362f 6e6f 6e65 626f  /zangxx66/nonebo
+00000270: 745f 706c 7567 696e 5f62 6c69 7665 5f64  t_plugin_blive_d
+00000280: 616e 6d61 6b75 2e73 7667 295d 2868 7474  anmaku.svg)](htt
+00000290: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+000002a0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f7a  sercontent.com/z
+000002b0: 616e 6778 7836 362f 6e6f 6e65 626f 745f  angxx66/nonebot_
+000002c0: 706c 7567 696e 5f62 6c69 7665 5f64 616e  plugin_blive_dan
+000002d0: 6d61 6b75 2f6d 6169 6e2f 4c49 4345 4e53  maku/main/LICENS
+000002e0: 4529 2020 0d0a 0d0a 3c2f 6469 763e 2020  E)  ....</div>  
+000002f0: 0d0a 0d0a 2323 20e7 ae80 e4bb 8b20 200d  ....## ......  .
+00000300: 0a2d 20e5 9fba e4ba 8e5b 6e6f 6e65 626f  .- ......[nonebo
+00000310: 7432 5d28 6874 7470 733a 2f2f 7632 2e6e  t2](https://v2.n
+00000320: 6f6e 6562 6f74 2e64 6576 2f29 e5bc 80e5  onebot.dev/)....
+00000330: 8f91 e79a 8442 e7ab 99e7 9bb4 e692 ade9  .....B..........
+00000340: 97b4 e5bc b9e5 b995 e79b 91e5 90ac e68f  ................
+00000350: 92e4 bbb6 efbc 8ce5 8f82 e880 83e4 ba86  ................
+00000360: 4861 7275 6b61 e592 8c62 6c69 7665 6368  Haruka...blivech
+00000370: 6174 e79a 84e9 83a8 e588 86e4 bba3 e7a0  at..............
+00000380: 81e3 8082 2020 0d0a 2d20 e8b5 b7e6 ba90  ....  ..- ......
+00000390: e4ba 8e5b e593 88e9 b9bf 6861 6c6c 755d  ...[......hallu]
+000003a0: 2868 7474 7073 3a2f 2f73 7061 6365 2e62  (https://space.b
+000003b0: 696c 6962 696c 692e 636f 6d2f 3334 3933  ilibili.com/3493
+000003c0: 3131 3834 3934 3131 3637 3937 29e7 9a84  118494116797)...
+000003d0: e4b8 80e6 9da1 e58a a8e6 8081 efbc 8ce8  ................
+000003e0: 8ba6 e4ba 8ee5 819a e8a7 86e9 a291 e697  ................
+000003f0: b6e6 b2a1 e69c 89e4 baba e581 9ae8 b7af  ................
+00000400: e781 afef bc8c e7bf bbe5 bd95 e692 ade7  ................
+00000410: 9a84 e697 b6e5 8099 e5a4 b4e9 83bd e5a4  ................
+00000420: a7e4 ba86 efbc 8ce8 afb4 e8a6 81e8 8ab1  ................
+00000430: e992 b1e8 afb7 e4b8 aae5 85a8 e881 8ce8  ................
+00000440: b7af e781 afef bc8c e688 91e5 afbb e680  ................
+00000450: 9de4 b88e e585 b6e6 8a8a e992 b1e9 8081  ................
+00000460: e7bb 99e5 88ab e4ba baef bc8c e4b8 8de5  ................
+00000470: a682 e4ba a4e7 bb99 426f 74e5 8ebb e581  ........Bot.....
+00000480: 9ae8 b7af e781 afe3 8082 0d0a 215b 5d28  ............![](
+00000490: 2f64 6f63 2f73 6372 6565 6e73 686f 7431  /doc/screenshot1
+000004a0: 2e70 6e67 290d 0a2d 20e8 b7af e781 afef  .png)..- .......
+000004b0: bc9a e68c 87e6 8a8a e79b b4e6 92ad e8bf  ................
+000004c0: 87e7 a88b e4b8 ade6 9c89 e8b6 a3e7 9a84  ................
+000004d0: e782 b9e8 aeb0 e5bd 95e4 b88b e69d a5ef  ................
+000004e0: bc8c e7bb 99e5 89aa e8be 91e6 a0b9 e68d  ................
+000004f0: aee8 aeb0 e5bd 95e7 9a84 e697 b6e9 97b4  ................
+00000500: e782 b9e5 928c e586 85e5 aeb9 e581 9ae5  ................
+00000510: 87ba e5af b9e5 ba94 e79a 84e8 a786 e9a2  ................
+00000520: 91e3 8082 0d0a 0d0a 2323 20e5 8a9f e883  ........## .....
+00000530: bd0d 0a0d 0a2d 20e7 94a8 e5bc b9e5 b995  .....- .........
+00000540: e79a 84e5 bda2 e5bc 8fe8 aeb0 e5bd 95e7  ................
+00000550: 9bb4 e692 ade9 ab98 e883 bde7 82b9 0d0a  ................
+00000560: 2d20 e5bc b9e5 b995 e68c 87e4 bba4 e4b8  - ..............
+00000570: ba60 23e8 b7af e781 af60 e58a a0e4 b88a  .`#......`......
+00000580: e8ae b0e5 bd95 e79a 84e5 8685 e5ae b90d  ................
+00000590: 0a2d 20e4 bb85 e59c a8e5 bc80 e692 ade6  .- .............
+000005a0: 97b6 e5bc b9e5 b995 e68c 87e4 bba4 e689  ................
+000005b0: 8de4 bc9a e794 9fe6 9588 0d0a 0d0a 2323  ..............##
+000005c0: 20e4 be9d e8b5 9620 200d 0a0d 0a2d 2050   ......  ....- P
+000005d0: 7974 686f 6e20 3e3d 2033 2e31 300d 0a2d  ython >= 3.10..-
+000005e0: 204f 6e65 426f 7420 5631 310d 0a0d 0a23   OneBot V11....#
+000005f0: 2320 e5ae 89e8 a385 0d0a 2d20 e696 b9e5  # ........- ....
+00000600: bc8f e4b8 80ef bc9a e4bd bfe7 94a8 606e  ..............`n
+00000610: 622d 636c 6960 e5ae 89e8 a385 e68f 92e4  b-cli`..........
+00000620: bbb6 2020 0d0a 6060 600d 0a6e 6220 706c  ..  ..```..nb pl
+00000630: 7567 696e 2069 6e73 7461 6c6c 206e 6f6e  ugin install non
+00000640: 6562 6f74 2d70 6c75 6769 6e2d 626c 6976  ebot-plugin-bliv
+00000650: 652d 6461 6e6d 616b 750d 0a60 6060 0d0a  e-danmaku..```..
+00000660: 2d20 e696 b9e5 bc8f e4ba 8cef bc9a e4bd  - ..............
+00000670: bfe7 94a8 6070 6970 60e5 ae89 e8a3 850d  ....`pip`.......
+00000680: 0a60 6060 0d0a 7079 7468 6f6e 202d 6d20  .```..python -m 
+00000690: 7069 7020 696e 7374 616c 6c20 6e6f 6e65  pip install none
+000006a0: 626f 742d 706c 7567 696e 2d62 6c69 7665  bot-plugin-blive
+000006b0: 2d64 616e 6d61 6b75 0d0a 6060 6020 200d  -danmaku..```  .
+000006c0: 0a0d 0a23 2320 e68c 87e4 bba4 0d0a 0d0a  ...## ..........
+000006d0: 7ce6 8c87 e4bb a47c e8af b4e6 988e 7c0d  |......|......|.
+000006e0: 0a7c 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d7c  .|------|------|
+000006f0: 0d0a 7c2f e6b7 bbe5 8aa0 e8ae a2e9 9885  ..|/............
+00000700: 2055 4944 7c55 4944 e4b8 ba42 e7ab 99e7   UID|UID...B....
+00000710: 94a8 e688 b7e7 9a84 7569 64ef bc8c e4b8  ........uid.....
+00000720: 8de6 98af e79b b4e6 92ad e997 b469 64ef  .............id.
+00000730: bc8c e4bb a5e4 b88b e590 8ce7 9086 7c0d  ..............|.
+00000740: 0a7c 2fe5 8f96 e6b6 88e8 aea2 e998 8520  .|/............ 
+00000750: 5549 447c e588 a0e9 99a4 e8ae a2e9 9885  UID|............
+00000760: 7c0d 0a7c 2fe5 bc80 e590 afe8 b7af e781  |..|/...........
+00000770: af20 5549 447c e5bc 80e5 90af e79b b4e6  . UID|..........
+00000780: 92ad e997 b4e5 bcb9 e5b9 95e7 9b91 e590  ................
+00000790: ac7c 0d0a 7c2f e585 b3e9 97ad e8b7 afe7  .|..|/..........
+000007a0: 81af 2055 4944 7ce5 85b3 e997 ade7 9bb4  .. UID|.........
+000007b0: e692 ade9 97b4 e5bc b9e5 b995 e79b 91e5  ................
+000007c0: 90ac 7c0d 0a7c 2fe5 bc80 e590 afe7 9bb4  ..|..|/.........
+000007d0: e692 ade6 8ea8 e980 8120 5549 447c e5bc  ......... UID|..
+000007e0: 80e5 90af e5bc 80e6 92ad e68f 90e9 8692  ................
+000007f0: 7c0d 0a7c 2fe5 85b3 e997 ade7 9bb4 e692  |..|/...........
+00000800: ade6 8ea8 e980 8120 5549 447c e585 b3e9  ....... UID|....
+00000810: 97ad e5bc 80e6 92ad e68f 90e9 8692 7c0d  ..............|.
+00000820: 0a7c 2fe8 aea2 e998 85e5 8897 e8a1 a87c  .|/............|
+00000830: 7c20 0d0a 0d0a 2323 20e6 9588 e69e 9ce9  | ....## .......
+00000840: a284 e8a7 8820 0d0a 0d0a 215b 5d28 2f64  ..... ....![](/d
+00000850: 6f63 2f73 6372 6565 6e73 686f 742e 706e  oc/screenshot.pn
+00000860: 6729 0d0a 0d0a 2323 20e6 9bb4 e696 b0e6  g)....## .......
+00000870: 97a5 e5bf 9720 200d 0a2d 2076 302e 312e  .....  ..- v0.1.
+00000880: 340d 0a20 2020 202d 20e6 b7bb e58a a0e5  4..    - .......
+00000890: bc80 e692 ade6 8f90 e986 92ef bc8c 602e  ..............`.
+000008a0: 656e 7660 e696 b0e5 a29e e585 a8e5 b180  env`............
+000008b0: e985 8de7 bdae e9a1 b960 6461 6e6d 616b  .........`danmak
+000008c0: 755f 6772 6f75 705f 6e6f 7469 6365 60e5  u_group_notice`.
+000008d0: bc80 e585 b320 5b23 335d 2868 7474 7073  ..... [#3](https
+000008e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7a61  ://github.com/za
+000008f0: 6e67 7878 3636 2f6e 6f6e 6562 6f74 5f70  ngxx66/nonebot_p
+00000900: 6c75 6769 6e5f 626c 6976 655f 6461 6e6d  lugin_blive_danm
+00000910: 616b 752f 6973 7375 6573 2f33 2920 200d  aku/issues/3)  .
+00000920: 0a20 2020 202d 20e8 b083 e695 b4e6 97a5  .    - .........
+00000930: e5bf 97e7 baa7 e588 ab20 5b23 355d 2868  ......... [#5](h
+00000940: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000950: 6d2f 7a61 6e67 7878 3636 2f6e 6f6e 6562  m/zangxx66/noneb
+00000960: 6f74 5f70 6c75 6769 6e5f 626c 6976 655f  ot_plugin_blive_
+00000970: 6461 6e6d 616b 752f 6973 7375 6573 2f35  danmaku/issues/5
+00000980: 290d 0a2d 2076 302e 312e 330d 0a20 2020  )..- v0.1.3..   
+00000990: 202d 2062 6f74 e68f 90e9 8692 e59c a8e6   - bot..........
+000009a0: 97b6 e997 b4e5 908e e99d a2e5 8aa0 e4b8  ................
+000009b0: 8ae7 9bb4 e692 ade6 97b6 e995 bfe6 98be  ................
+000009c0: e7a4 baef bc8c e981 bfe5 858d e79b b4e6  ................
+000009d0: 92ad e794 bbe9 9da2 e6b2 a1e6 9c89 e5bd  ................
+000009e0: 93e5 898d e697 b6e9 97b4 e79a 84e5 9cba  ................
+000009f0: e699 af0d 0a2d 2076 302e 312e 320d 0a20  .....- v0.1.2.. 
+00000a00: 2020 202d 2066 6978 e5b1 80e9 83a8 e58f     - fix........
+00000a10: 98e9 878f e697 a0e6 b395 e6ad a3e5 b8b8  ................
+00000a20: e69b b4e6 96b0 e79a 8462 7567 0d0a 2d20  .........bug..- 
+00000a30: 7630 2e31 2e30 0d0a 2020 2020 2d20 e59f  v0.1.0..    - ..
+00000a40: bae4 ba8e 6e6f 6e65 626f 7432 efbc 8ce5  ....nonebot2....
+00000a50: ae9e e78e b0e5 908c e6ad a5e8 b7af e781  ................
+00000a60: afe5 bcb9 e5b9 95e5 88b0 7171 e7be a420  ..........qq... 
+00000a70: 200d 0a0d 0a23 2320 e684 9fe8 b0a2 0d0a   ....## ........
+00000a80: 2d20 5b48 6172 756b 6142 6f74 5d28 6874  - [HarukaBot](ht
+00000a90: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000aa0: 2f53 4b2d 3431 352f 4861 7275 6b61 426f  /SK-415/HarukaBo
+00000ab0: 7429 0d0a 2d20 5b62 6c69 7665 6368 6174  t)..- [blivechat
+00000ac0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000ad0: 2e63 6f6d 2f78 6667 7279 756a 6b2f 626c  .com/xfgryujk/bl
+00000ae0: 6976 6563 6861 7429 0d0a 2d20 5b6e 6f6e  ivechat)..- [non
+00000af0: 6562 6f74 325d 2868 7474 7073 3a2f 2f76  ebot2](https://v
+00000b00: 322e 6e6f 6e65 626f 742e 6465 762f 290d  2.nonebot.dev/).
+00000b10: 0a0d 0a                                  ...
```

