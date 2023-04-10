# Comparing `tmp/nonebot_plugin_bilichat-1.1.0.tar.gz` & `tmp/nonebot_plugin_bilichat-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-1.1.0.tar", last modified: Sun Apr  9 10:45:51 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-1.1.1.tar", last modified: Mon Apr 10 05:00:08 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-1.1.0.tar` & `nonebot_plugin_bilichat-1.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    34523 2023-04-09 10:45:43.254714 nonebot_plugin_bilichat-1.1.0/LICENSE
--rw-r--r--   0        0        0     5965 2023-04-09 10:45:43.258714 nonebot_plugin_bilichat-1.1.0/README.md
--rw-r--r--   0        0        0     8383 2023-04-09 10:45:43.262714 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     4125 2023-04-09 10:45:43.262714 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-04-09 10:45:43.262714 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4592 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      927 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     4408 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0     8900 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3800 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      289 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     3678 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0     2854 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0      866 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0       93 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0      148 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0     2212 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/summary/content_summarise.py
--rw-r--r--   0        0        0     4388 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     1764 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1098 2023-04-09 10:45:51.690604 nonebot_plugin_bilichat-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     6785 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-10 04:59:59.836401 nonebot_plugin_bilichat-1.1.1/LICENSE
+-rw-r--r--   0        0        0     5965 2023-04-10 04:59:59.836401 nonebot_plugin_bilichat-1.1.1/README.md
+-rw-r--r--   0        0        0     8397 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     4142 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4592 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      927 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     4408 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0     8900 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3800 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      289 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     3678 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0     2854 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0      866 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0       93 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0      148 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0     2212 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/summary/content_summarise.py
+-rw-r--r--   0        0        0     4388 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     1764 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1098 2023-04-10 05:00:08.220473 nonebot_plugin_bilichat-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6785 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-1.1.0/LICENSE` & `nonebot_plugin_bilichat-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.0/README.md` & `nonebot_plugin_bilichat-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from nonebot.rule import Rule
 from nonebot.typing import T_State
 
 from .config import __version__, plugin_config
 from .lib.b23_extract import b23_extract
 from .lib.content_resolve import get_video_basic, get_video_cache
 from .model.exception import AbortError
-from .optional import capture_exception
+from .optional import capture_exception  # type: ignore
 
 if plugin_config.bilichat_openai_token:
     from .summary.content_summarise import openai_summarization
 if plugin_config.bilichat_word_cloud:
     from .wordcloud.wordcloud import wordcloud
 
 __plugin_meta__ = PluginMetadata(
@@ -59,34 +59,36 @@
         return plugin_config.bilichat_enable_unkown_src
 
 
 bili = on_regex(
     r"av(\d{1,15})|BV(1[A-Za-z0-9]{2}4.1.7[A-Za-z0-9]{2})",
     block=plugin_config.bilichat_block,
     priority=1,
-    rule=Rule(_bili_check),  # type: ignore
+    rule=Rule(_bili_check),
 )
 
 
 @bili.handle()
 async def get_bili_number_re(state: T_State):
     state["bili_number"] = state[REGEX_STR]
 
 
 b23 = on_regex(
     r"b23.(tv|wtf)[\\/]+(\w+)",
     block=plugin_config.bilichat_block,
     priority=1,
-    rule=Rule(_bili_check),  # type: ignore
+    rule=Rule(_bili_check),
 )
 
 
 @b23.handle()
 async def get_bili_number_b23(state: T_State):
-    if matched := re.search(r"av(\d{1,15})|BV(1[A-Za-z0-9]{2}4.1.7[A-Za-z0-9]{2})", await b23_extract(state[REGEX_GROUP])):  # type: ignore
+    if matched := re.search(
+        r"av(\d{1,15})|BV(1[A-Za-z0-9]{2}4.1.7[A-Za-z0-9]{2})", await b23_extract(state[REGEX_GROUP])  # type: ignore
+    ):
         state["bili_number"] = matched.group()
 
 
 async def forword_msg_v11(bot: V11_Bot, event: V11_ME, forword_list: V11_Message):
     msgs = [
         {"type": "node", "data": {"name": plugin_config.nickname[0], "uin": bot.self_id, "content": msg}}
         for msg in forword_list
@@ -97,25 +99,26 @@
         await bot.send_private_forward_msg(id=str(event.user_id), messages=msgs)
     raise FinishedException
 
 
 @bili.handle()
 @b23.handle()
 async def video_info_v11(bot: V11_Bot, event: V11_ME, state: T_State, matcher: Matcher):
-    forword_list = []
+    # sourcery skip: raise-from-previous-error
+    forword_list: V11_Message = []  # type: ignore
     # basic info
     msg, img, info = await get_video_basic(state["bili_number"], state["_uid_"])
     if not msg or not info:
         await matcher.finish()
     reply = V11_MS.reply(event.message_id)
     if not img:
         await matcher.finish(reply + msg)
     image = V11_MS.image(img)
     if "info" in plugin_config.bilichat_forword_msg:
-        forword_list.append(reply + image + msg)
+        forword_list.append(image + msg)  # type: ignore
         reply = ""
     else:
         msgid = (await matcher.send(reply + image + msg))["message_id"]
         reply = V11_MS.reply(msgid)
 
     # furtuer fuctions
     if not plugin_config.bilichat_openai_token and not plugin_config.bilichat_word_cloud:
@@ -125,46 +128,48 @@
     try:
         cache = await get_video_cache(info)
     except AbortError as e:
         logger.exception(e)
         if "info" in plugin_config.bilichat_forword_msg:
             forword_list.append(f"视频字幕获取失败: {str(e)}")
             await forword_msg_v11(bot, event, forword_list)
+            raise FinishedException
         else:
             await matcher.finish(f"{reply}视频字幕获取失败: {str(e)}")
     except Exception as e:
         capture_exception()
         logger.exception(e)
         if "info" in plugin_config.bilichat_forword_msg:
             forword_list.append(f"未知错误: {e}")
             await forword_msg_v11(bot, event, forword_list)
+            raise FinishedException
         else:
-            await matcher.finish(f"{reply}未知错误: {e}")  # type: ignore
+            await matcher.finish(f"{reply}未知错误: {e}")
 
-    if image := await wordcloud(cache=cache, cid=str(info["cid"])):
-        if plugin_config.bilichat_word_cloud:
+    # wordcloud
+    if plugin_config.bilichat_word_cloud:
+        if image := await wordcloud(cache=cache, cid=str(info["cid"])):
             if "wordcloud" in plugin_config.bilichat_forword_msg:
                 forword_list.append(V11_MS.image(image))
             else:
-                await matcher.send(reply + V11_MS.image(image))  # type: ignore
-    elif plugin_config.bilichat_word_cloud:
-        if "wordcloud" in plugin_config.bilichat_forword_msg:
+                await matcher.send(reply + V11_MS.image(image))
+        elif "wordcloud" in plugin_config.bilichat_forword_msg:
             forword_list.append("视频无有效字幕")
             await forword_msg_v11(bot, event, forword_list)
         else:
             await matcher.finish(f"{reply}视频无有效字幕")
 
-    if summary := await openai_summarization(cache=cache, cid=str(info["cid"])):
-        if plugin_config.bilichat_openai_token:
+    # summary
+    if plugin_config.bilichat_openai_token:
+        if summary := await openai_summarization(cache=cache, cid=str(info["cid"])):
             if "summary" in plugin_config.bilichat_forword_msg:
                 forword_list.append(summary)
             else:
-                await matcher.send(reply + summary)  # type: ignore
-    elif plugin_config.bilichat_openai_token:
-        if "summary" in plugin_config.bilichat_forword_msg:
+                await matcher.send(reply + summary)
+        elif "summary" in plugin_config.bilichat_forword_msg:
             forword_list.append("视频无有效字幕")
             await forword_msg_v11(bot, event, forword_list)
         else:
             await matcher.finish(f"{reply}视频无有效字幕")
 
     if forword_list:
         await forword_msg_v11(bot, event, forword_list)
@@ -174,42 +179,42 @@
 @b23.handle()
 async def video_info_v12(bot: V12_Bot, event: V12_ME, state: T_State, matcher: Matcher):
     # basic info
     msg, img, info = await get_video_basic(state["bili_number"], state["_uid_"])
     if not msg:
         await matcher.finish()
     reply = V12_MS.reply(message_id=event.message_id, user_id=event.get_user_id())
-    if not img:
+    if not img or not info:
         await matcher.finish(reply + msg)
     fileid = await bot.upload_file(type="data", name=f"{state['bili_number']}.jpg", data=img)
     image = V12_MS.image(file_id=fileid["file_id"])
     msgid = (await matcher.send(reply + image + msg))["message_id"]
 
     # furtuer fuctions
     if not (plugin_config.bilichat_openai_token or plugin_config.bilichat_word_cloud):
         raise FinishedException
 
     reply = V12_MS.reply(message_id=msgid, user_id=bot.self_id)
     try:
-        cache = await get_video_cache(info)  # type: ignore
+        cache = await get_video_cache(info)
     except AbortError as e:
         logger.exception(e)
         await matcher.finish(f"{reply}视频字幕获取失败: {str(e)}")
     except Exception as e:
         capture_exception()
         logger.exception(e)
         await matcher.finish(f"{reply}未知错误: {str(e)}")
 
+    # wordcloud
     if plugin_config.bilichat_word_cloud:
         if image := await wordcloud(cache=cache, cid=str(info["cid"])):
-            fileid = await bot.upload_file(
-                type="data", name=f"{state['bili_number']}_wc.jpg", data=image
-            )  # type: ignore
+            fileid = await bot.upload_file(type="data", name=f"{state['bili_number']}_wc.jpg", data=image)
             await matcher.send(reply + V12_MS.image(file_id=fileid["file_id"]))
         else:
             await matcher.finish(f"{reply}视频无有效字幕")
 
+    # summary
     if plugin_config.bilichat_openai_token:
         if summary := await openai_summarization(cache=cache, cid=str(info["cid"])):
-            await matcher.send(reply + summary)  # type: ignore
+            await matcher.send(reply + summary)
         else:
             await matcher.finish(f"{reply}视频无有效字幕")
```

### Comparing `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     bilichat_enable_private: bool = True
     bilichat_enable_v12_channel: bool = True
     bilichat_enable_unkown_src: bool = False
     bilichat_whitelist: Sequence[str] = []
     bilichat_blacklist: Sequence[str] = []
     bilichat_dynamic_font: Optional[str]
     bilichat_cd_time: int = 120
-    bilichat_forword_msg: Sequence[str] = {}  # ("info", "wordcloud", "summary")
+    bilichat_forword_msg: Sequence[str] = []  # ("info", "wordcloud", "summary")
     nickname: Sequence[str] = ["awesome-nonebot"]
 
     # both WC and AI
     bilichat_use_bcut_asr: bool = True
 
     # Word Cloud
     bilichat_word_cloud: bool = True
@@ -52,14 +52,15 @@
             logger.warning(
                 "Forword_msg is not implemented by OneBot V12, events of OneBot V12 will not be sent as forword_msg!"
             )
         if "OneBot V11" in drivers:
             logger.warning(
                 "Using forward_msg may cause serious risk control restrictions, please enable this feature with caution!"
             )
+        return v
 
     @validator("nickname")
     def check_nickname(cls, v):
         return list(v) or ["awesome-nonebot"]
 
     @validator("bilichat_openai_proxy")
     def check_openai_proxy(cls, v, values):
```

### Comparing `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/summary/content_summarise.py` & `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/summary/content_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.0/pyproject.toml` & `nonebot_plugin_bilichat-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "1.1.0"
+version = "1.1.1"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "httpx>=0.23.3",
```

### Comparing `nonebot_plugin_bilichat-1.1.0/PKG-INFO` & `nonebot_plugin_bilichat-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 1.1.0
+Version: 1.1.1
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: httpx>=0.23.3
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 1.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 1.1.1 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 httpx>=0.23.3 Requires-Dist: bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-
 plugin-localstore>=0.4.1 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-
 Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra" Requires-Dist:
```

