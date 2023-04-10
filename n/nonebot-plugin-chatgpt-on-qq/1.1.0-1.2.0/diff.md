# Comparing `tmp/nonebot-plugin-chatgpt-on-qq-1.1.0.tar.gz` & `tmp/nonebot-plugin-chatgpt-on-qq-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-chatgpt-on-qq-1.1.0.tar", last modified: Mon Apr 10 03:57:48 2023, max compression
+gzip compressed data, was "nonebot-plugin-chatgpt-on-qq-1.2.0.tar", last modified: Mon Apr 10 17:07:23 2023, max compression
```

## Comparing `nonebot-plugin-chatgpt-on-qq-1.1.0.tar` & `nonebot-plugin-chatgpt-on-qq-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 03:57:48.036484 nonebot-plugin-chatgpt-on-qq-1.1.0/
--rw-rw-rw-   0        0        0      769 2023-04-10 03:57:48.035511 nonebot-plugin-chatgpt-on-qq-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-07 17:39:40.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-10 03:57:48.014719 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq/
--rw-rw-rw-   0        0        0    12808 2023-04-10 03:38:53.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq/__init__.py
--rw-rw-rw-   0        0        0     3660 2023-04-09 15:33:24.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq/chatGPT.py
--rw-rw-rw-   0        0        0      416 2023-04-08 19:05:12.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq/config.py
--rw-rw-rw-   0        0        0     4351 2023-04-08 19:05:35.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq/conversation.py
--rw-rw-rw-   0        0        0      502 2023-03-07 16:08:33.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq/custom_errors.py
--rw-rw-rw-   0        0        0     5518 2023-04-10 03:56:33.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq/loadpresets.py
-drwxrwxrwx   0        0        0        0 2023-04-10 03:57:48.031421 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq.egg-info/
--rw-rw-rw-   0        0        0      769 2023-04-10 03:57:47.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      533 2023-04-10 03:57:47.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 03:57:47.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2023-04-10 03:57:47.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-04-10 03:57:47.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 03:57:48.036484 nonebot-plugin-chatgpt-on-qq-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-04-10 03:56:57.000000 nonebot-plugin-chatgpt-on-qq-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 17:07:23.007055 nonebot-plugin-chatgpt-on-qq-1.2.0/
+-rw-rw-rw-   0        0        0      770 2023-04-10 17:07:23.007055 nonebot-plugin-chatgpt-on-qq-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-07 17:39:40.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-10 17:07:22.983122 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq/
+-rw-rw-rw-   0        0        0    12808 2023-04-10 03:38:53.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq/__init__.py
+-rw-rw-rw-   0        0        0     3660 2023-04-09 15:33:24.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq/chatGPT.py
+-rw-rw-rw-   0        0        0      416 2023-04-08 19:05:12.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq/config.py
+-rw-rw-rw-   0        0        0     4351 2023-04-08 19:05:35.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq/conversation.py
+-rw-rw-rw-   0        0        0      502 2023-03-07 16:08:33.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq/custom_errors.py
+-rw-rw-rw-   0        0        0     6773 2023-04-10 17:03:53.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq/loadpresets.py
+drwxrwxrwx   0        0        0        0 2023-04-10 17:07:22.999040 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq.egg-info/
+-rw-rw-rw-   0        0        0      770 2023-04-10 17:07:22.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      533 2023-04-10 17:07:22.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 17:07:22.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2023-04-10 17:07:22.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-04-10 17:07:22.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 17:07:23.007055 nonebot-plugin-chatgpt-on-qq-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1220 2023-04-10 17:07:09.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/setup.py
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.1.0/PKG-INFO` & `nonebot-plugin-chatgpt-on-qq-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-on-qq
-Version: 1.1.0
+Version: 1.2.0
 Summary: 具有多对话功能的chatGPT聊天插件
 Home-page: https://github.com/Suxmx/nonebot_plugin_chatgpt_turbo_on_qq
 Author: 颜曦
 Author-email: 424504326@qq.com
 Maintainer: 颜曦
 Maintainer-email: 424504326@qq.com
 License: BSD License
 Platform: all
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq/__init__.py` & `nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq/chatGPT.py` & `nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq/chatGPT.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq/conversation.py` & `nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq/conversation.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO` & `nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-on-qq
-Version: 1.1.0
+Version: 1.2.0
 Summary: 具有多对话功能的chatGPT聊天插件
 Home-page: https://github.com/Suxmx/nonebot_plugin_chatgpt_turbo_on_qq
 Author: 颜曦
 Author-email: 424504326@qq.com
 Maintainer: 颜曦
 Maintainer-email: 424504326@qq.com
 License: BSD License
 Platform: all
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.1.0/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt` & `nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-on-qq-1.1.0/setup.py` & `nonebot-plugin-chatgpt-on-qq-1.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding:utf-8
 
 from setuptools import find_packages, setup
 
 setup(
     name='nonebot-plugin-chatgpt-on-qq',
-    version='1.1.0',
+    version='1.2.0',
     description='具有多对话功能的chatGPT聊天插件',
     long_description=open('README.rst').read(),
     author='颜曦',
     author_email='424504326@qq.com',
     maintainer='颜曦',
     maintainer_email='424504326@qq.com',
     packages=find_packages(),
@@ -26,12 +26,12 @@
     license='BSD License',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Operating System :: OS Independent',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2.7',
+        'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy'
     ],
 )
```

