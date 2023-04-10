# Comparing `tmp/tatarubot2-0.1.0.tar.gz` & `tmp/tatarubot2-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tatarubot2-0.1.0.tar", last modified: Sun Apr  9 02:59:39 2023, max compression
+gzip compressed data, was "dist/tatarubot2-0.1.1.tar", last modified: Mon Apr 10 09:02:16 2023, max compression
```

## Comparing `tatarubot2-0.1.0.tar` & `tatarubot2-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 02:59:39.000000 tatarubot2-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     1066 2022-08-12 03:44:26.000000 tatarubot2-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2908 2023-04-09 02:59:39.000000 tatarubot2-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2734 2023-03-14 01:51:48.000000 tatarubot2-0.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)      387 2022-06-22 03:02:25.000000 tatarubot2-0.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 02:59:39.000000 tatarubot2-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      572 2023-04-09 02:59:04.000000 tatarubot2-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 02:59:39.000000 tatarubot2-0.1.0/tatarubot2/
--rw-r--r--   0 root         (0) root         (0)       32 2023-04-07 06:02:20.000000 tatarubot2-0.1.0/tatarubot2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 02:59:39.000000 tatarubot2-0.1.0/tatarubot2/plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 02:51:28.000000 tatarubot2-0.1.0/tatarubot2/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      713 2022-11-15 08:07:47.000000 tatarubot2-0.1.0/tatarubot2/plugins/auto_response.py
--rw-r--r--   0 root         (0) root         (0)     1627 2023-04-07 06:02:20.000000 tatarubot2-0.1.0/tatarubot2/plugins/bot_help.py
--rw-r--r--   0 root         (0) root         (0)     1211 2023-04-07 02:28:25.000000 tatarubot2-0.1.0/tatarubot2/plugins/chat_ai.py
--rw-r--r--   0 root         (0) root         (0)     2262 2022-08-16 07:15:05.000000 tatarubot2-0.1.0/tatarubot2/plugins/ff_weibo.py
--rw-r--r--   0 root         (0) root         (0)     4409 2022-08-17 03:31:15.000000 tatarubot2-0.1.0/tatarubot2/plugins/house.py
--rw-r--r--   0 root         (0) root         (0)    17045 2023-01-29 07:09:23.000000 tatarubot2-0.1.0/tatarubot2/plugins/item.py
--rw-r--r--   0 root         (0) root         (0)    17338 2023-04-07 06:02:20.000000 tatarubot2-0.1.0/tatarubot2/plugins/item_new.py
--rw-r--r--   0 root         (0) root         (0)     7011 2023-04-07 06:02:20.000000 tatarubot2-0.1.0/tatarubot2/plugins/logs_dps.py
--rw-r--r--   0 root         (0) root         (0)     1230 2022-08-12 01:48:07.000000 tatarubot2-0.1.0/tatarubot2/plugins/lottery.py
--rw-r--r--   0 root         (0) root         (0)     7754 2022-08-15 08:28:24.000000 tatarubot2-0.1.0/tatarubot2/plugins/market.py
--rw-r--r--   0 root         (0) root         (0)     8223 2023-04-07 06:02:20.000000 tatarubot2-0.1.0/tatarubot2/plugins/market_new.py
--rw-r--r--   0 root         (0) root         (0)     3103 2022-09-24 04:17:17.000000 tatarubot2-0.1.0/tatarubot2/plugins/nuannuan.py
--rw-r--r--   0 root         (0) root         (0)      899 2022-08-12 01:48:15.000000 tatarubot2-0.1.0/tatarubot2/plugins/precious.py
--rw-r--r--   0 root         (0) root         (0)     1196 2022-06-23 07:26:19.000000 tatarubot2-0.1.0/tatarubot2/plugins/weather.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 02:59:39.000000 tatarubot2-0.1.0/tatarubot2/tools/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-12 07:58:45.000000 tatarubot2-0.1.0/tatarubot2/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5058 2023-04-07 06:02:20.000000 tatarubot2-0.1.0/tatarubot2/tools/download_boss.py
--rw-r--r--   0 root         (0) root         (0)     1962 2023-01-30 01:23:02.000000 tatarubot2-0.1.0/tatarubot2/tools/download_item2id.py
--rw-r--r--   0 root         (0) root         (0)     1725 2023-04-07 06:02:20.000000 tatarubot2-0.1.0/tatarubot2/tools/normal_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 02:59:39.000000 tatarubot2-0.1.0/tatarubot2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2908 2023-04-09 02:59:39.000000 tatarubot2-0.1.0/tatarubot2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      825 2023-04-09 02:59:39.000000 tatarubot2-0.1.0/tatarubot2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 02:59:39.000000 tatarubot2-0.1.0/tatarubot2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-09 02:59:39.000000 tatarubot2-0.1.0/tatarubot2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-09 02:59:39.000000 tatarubot2-0.1.0/tatarubot2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 09:02:16.000000 tatarubot2-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)     1066 2022-08-12 03:44:26.000000 tatarubot2-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2908 2023-04-10 09:02:16.000000 tatarubot2-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2734 2023-03-14 01:51:48.000000 tatarubot2-0.1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      387 2022-06-22 03:02:25.000000 tatarubot2-0.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 09:02:16.000000 tatarubot2-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      572 2023-04-10 08:55:17.000000 tatarubot2-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 09:02:16.000000 tatarubot2-0.1.1/tatarubot2/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-10 08:55:17.000000 tatarubot2-0.1.1/tatarubot2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 09:02:16.000000 tatarubot2-0.1.1/tatarubot2/plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 02:51:28.000000 tatarubot2-0.1.1/tatarubot2/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      713 2022-11-15 08:07:47.000000 tatarubot2-0.1.1/tatarubot2/plugins/auto_response.py
+-rw-r--r--   0 root         (0) root         (0)     1627 2023-04-07 06:02:20.000000 tatarubot2-0.1.1/tatarubot2/plugins/bot_help.py
+-rw-r--r--   0 root         (0) root         (0)     1211 2023-04-07 02:28:25.000000 tatarubot2-0.1.1/tatarubot2/plugins/chat_ai.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2022-08-16 07:15:05.000000 tatarubot2-0.1.1/tatarubot2/plugins/ff_weibo.py
+-rw-r--r--   0 root         (0) root         (0)     4409 2022-08-17 03:31:15.000000 tatarubot2-0.1.1/tatarubot2/plugins/house.py
+-rw-r--r--   0 root         (0) root         (0)    17045 2023-01-29 07:09:23.000000 tatarubot2-0.1.1/tatarubot2/plugins/item.py
+-rw-r--r--   0 root         (0) root         (0)    17338 2023-04-07 06:02:20.000000 tatarubot2-0.1.1/tatarubot2/plugins/item_new.py
+-rw-r--r--   0 root         (0) root         (0)     7011 2023-04-07 06:02:20.000000 tatarubot2-0.1.1/tatarubot2/plugins/logs_dps.py
+-rw-r--r--   0 root         (0) root         (0)     1230 2022-08-12 01:48:07.000000 tatarubot2-0.1.1/tatarubot2/plugins/lottery.py
+-rw-r--r--   0 root         (0) root         (0)     7754 2022-08-15 08:28:24.000000 tatarubot2-0.1.1/tatarubot2/plugins/market.py
+-rw-r--r--   0 root         (0) root         (0)     8223 2023-04-07 06:02:20.000000 tatarubot2-0.1.1/tatarubot2/plugins/market_new.py
+-rw-r--r--   0 root         (0) root         (0)     3103 2022-09-24 04:17:17.000000 tatarubot2-0.1.1/tatarubot2/plugins/nuannuan.py
+-rw-r--r--   0 root         (0) root         (0)      899 2022-08-12 01:48:15.000000 tatarubot2-0.1.1/tatarubot2/plugins/precious.py
+-rw-r--r--   0 root         (0) root         (0)     1196 2022-06-23 07:26:19.000000 tatarubot2-0.1.1/tatarubot2/plugins/weather.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 09:02:16.000000 tatarubot2-0.1.1/tatarubot2/tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-12 07:58:45.000000 tatarubot2-0.1.1/tatarubot2/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5058 2023-04-07 06:02:20.000000 tatarubot2-0.1.1/tatarubot2/tools/download_boss.py
+-rw-r--r--   0 root         (0) root         (0)     1962 2023-01-30 01:23:02.000000 tatarubot2-0.1.1/tatarubot2/tools/download_item2id.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-04-07 06:02:20.000000 tatarubot2-0.1.1/tatarubot2/tools/normal_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 09:02:16.000000 tatarubot2-0.1.1/tatarubot2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2908 2023-04-10 09:02:16.000000 tatarubot2-0.1.1/tatarubot2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      825 2023-04-10 09:02:16.000000 tatarubot2-0.1.1/tatarubot2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 09:02:16.000000 tatarubot2-0.1.1/tatarubot2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-10 09:02:16.000000 tatarubot2-0.1.1/tatarubot2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-10 09:02:16.000000 tatarubot2-0.1.1/tatarubot2.egg-info/top_level.txt
```

### Comparing `tatarubot2-0.1.0/LICENSE` & `tatarubot2-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.0/PKG-INFO` & `tatarubot2-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tatarubot2
-Version: 0.1.0
+Version: 0.1.1
 Summary: FF14 bot Tataru
 Author: aaron-li
 Author-email: 
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TataruBot2
```

### Comparing `tatarubot2-0.1.0/README.md` & `tatarubot2-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.0/setup.py` & `tatarubot2-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='tatarubot2',
-      version='0.1.0',
+      version='0.1.1',
       description='FF14 bot Tataru',
       long_description=open("README.md", encoding="utf-8").read(),
       long_description_content_type="text/markdown",
       author='aaron-li',
       author_email='',
       install_requires= ["requests"], # 定义依赖哪些模块
       # packages=find_packages(),  # 系统自动从当前目录开始找包
```

### Comparing `tatarubot2-0.1.0/tatarubot2/plugins/auto_response.py` & `tatarubot2-0.1.1/tatarubot2/plugins/auto_response.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.0/tatarubot2/plugins/bot_help.py` & `tatarubot2-0.1.1/tatarubot2/plugins/bot_help.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.0/tatarubot2/plugins/chat_ai.py` & `tatarubot2-0.1.1/tatarubot2/plugins/chat_ai.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.0/tatarubot2/plugins/ff_weibo.py` & `tatarubot2-0.1.1/tatarubot2/plugins/ff_weibo.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.0/tatarubot2/plugins/house.py` & `tatarubot2-0.1.1/tatarubot2/plugins/house.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.0/tatarubot2/plugins/item.py` & `tatarubot2-0.1.1/tatarubot2/plugins/item.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.0/tatarubot2/plugins/item_new.py` & `tatarubot2-0.1.1/tatarubot2/plugins/item_new.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.0/tatarubot2/plugins/logs_dps.py` & `tatarubot2-0.1.1/tatarubot2/plugins/logs_dps.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.0/tatarubot2/plugins/lottery.py` & `tatarubot2-0.1.1/tatarubot2/plugins/lottery.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.0/tatarubot2/plugins/market.py` & `tatarubot2-0.1.1/tatarubot2/plugins/market.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.0/tatarubot2/plugins/market_new.py` & `tatarubot2-0.1.1/tatarubot2/plugins/market_new.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.0/tatarubot2/plugins/nuannuan.py` & `tatarubot2-0.1.1/tatarubot2/plugins/nuannuan.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.0/tatarubot2/plugins/precious.py` & `tatarubot2-0.1.1/tatarubot2/plugins/precious.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.0/tatarubot2/plugins/weather.py` & `tatarubot2-0.1.1/tatarubot2/plugins/weather.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.0/tatarubot2/tools/download_boss.py` & `tatarubot2-0.1.1/tatarubot2/tools/download_boss.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.0/tatarubot2/tools/download_item2id.py` & `tatarubot2-0.1.1/tatarubot2/tools/download_item2id.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.0/tatarubot2/tools/normal_data.py` & `tatarubot2-0.1.1/tatarubot2/tools/normal_data.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.0/tatarubot2.egg-info/PKG-INFO` & `tatarubot2-0.1.1/tatarubot2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tatarubot2
-Version: 0.1.0
+Version: 0.1.1
 Summary: FF14 bot Tataru
 Author: aaron-li
 Author-email: 
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TataruBot2
```

### Comparing `tatarubot2-0.1.0/tatarubot2.egg-info/SOURCES.txt` & `tatarubot2-0.1.1/tatarubot2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

