# Comparing `tmp/nonebot_plugin_bilichat-1.1.1.tar.gz` & `tmp/nonebot_plugin_bilichat-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-1.1.1.tar", last modified: Mon Apr 10 05:00:08 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-1.1.2.tar", last modified: Mon Apr 10 14:54:51 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-1.1.1.tar` & `nonebot_plugin_bilichat-1.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    34523 2023-04-10 04:59:59.836401 nonebot_plugin_bilichat-1.1.1/LICENSE
--rw-r--r--   0        0        0     5965 2023-04-10 04:59:59.836401 nonebot_plugin_bilichat-1.1.1/README.md
--rw-r--r--   0        0        0     8397 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     4142 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4592 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      927 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     4408 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0     8900 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3800 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      289 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     3678 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0     2854 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0      866 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0       93 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0      148 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0     2212 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/summary/content_summarise.py
--rw-r--r--   0        0        0     4388 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     1764 2023-04-10 04:59:59.844401 nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1098 2023-04-10 05:00:08.220473 nonebot_plugin_bilichat-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     6785 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-10 14:54:40.221422 nonebot_plugin_bilichat-1.1.2/LICENSE
+-rw-r--r--   0        0        0     5965 2023-04-10 14:54:40.221422 nonebot_plugin_bilichat-1.1.2/README.md
+-rw-r--r--   0        0        0     8397 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     4142 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4592 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      927 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     4408 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0     8900 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3800 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      289 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     3678 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0     2854 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0      866 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0       93 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0      148 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0     2212 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/summary/content_summarise.py
+-rw-r--r--   0        0        0     4388 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     1764 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1184 2023-04-10 14:54:51.373477 nonebot_plugin_bilichat-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6953 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-1.1.1/LICENSE` & `nonebot_plugin_bilichat-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.1/README.md` & `nonebot_plugin_bilichat-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/summary/content_summarise.py` & `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/summary/content_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.1/pyproject.toml` & `nonebot_plugin_bilichat-1.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "1.1.1"
+version = "1.1.2"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "httpx>=0.23.3",
@@ -46,13 +46,18 @@
 wordcloud = [
     "jieba>=0.42.1",
     "wordcloud>=1.8.2.2",
 ]
 openai = [
     "tiktoken-async>=0.3.2",
 ]
+all = [
+    "jieba>=0.42.1",
+    "wordcloud>=1.8.2.2",
+    "tiktoken-async>=0.3.2",
+]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `nonebot_plugin_bilichat-1.1.1/PKG-INFO` & `nonebot_plugin_bilichat-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 1.1.1
+Version: 1.1.2
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: httpx>=0.23.3
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
@@ -12,17 +12,21 @@
 Requires-Dist: lxml>=4.9.2
 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot-adapter-onebot>=2.2.2
 Requires-Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra"
 Requires-Dist: jieba>=0.42.1; extra == "wordcloud"
 Requires-Dist: wordcloud>=1.8.2.2; extra == "wordcloud"
 Requires-Dist: tiktoken-async>=0.3.2; extra == "openai"
+Requires-Dist: jieba>=0.42.1; extra == "all"
+Requires-Dist: wordcloud>=1.8.2.2; extra == "all"
+Requires-Dist: tiktoken-async>=0.3.2; extra == "all"
 Provides-Extra: extra
 Provides-Extra: wordcloud
 Provides-Extra: openai
+Provides-Extra: all
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="docs/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="docs/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
```

#### html2text {}

```diff
@@ -1,19 +1,21 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 1.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 1.1.2 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 httpx>=0.23.3 Requires-Dist: bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-
 plugin-localstore>=0.4.1 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-
 Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra" Requires-Dist:
 jieba>=0.42.1; extra == "wordcloud" Requires-Dist: wordcloud>=1.8.2.2; extra ==
-"wordcloud" Requires-Dist: tiktoken-async>=0.3.2; extra == "openai" Provides-
-Extra: extra Provides-Extra: wordcloud Provides-Extra: openai Description-
-Content-Type: text/markdown
+"wordcloud" Requires-Dist: tiktoken-async>=0.3.2; extra == "openai" Requires-
+Dist: jieba>=0.42.1; extra == "all" Requires-Dist: wordcloud>=1.8.2.2; extra ==
+"all" Requires-Dist: tiktoken-async>=0.3.2; extra == "all" Provides-Extra:
+extra Provides-Extra: wordcloud Provides-Extra: openai Provides-Extra: all
+Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
     # nonebot-plugin-bilichat _â¨ å¤åè½çBç«è§é¢è§£æå·¥å· â¨_
                            [license] [pypi] [python]
 ## ð ä»ç»
 è§é¢é¾æ¥è§£æï¼å¹¶æ ¹æ®å¶åå®¹çæ**åºæ¬ä¿¡æ¯**ã**è¯äº**å**åå®¹æ»ç»**
 ææºç«¯è§å¾ ![](docs/mobile.png)   åºæ¬ä¿¡æ¯ ![](docs/basic.png)
```

