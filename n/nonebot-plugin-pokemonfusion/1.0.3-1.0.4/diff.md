# Comparing `tmp/nonebot_plugin_pokemonfusion-1.0.3.tar.gz` & `tmp/nonebot_plugin_pokemonfusion-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pokemonfusion-1.0.3.tar", last modified: Mon Apr 10 05:18:06 2023, max compression
+gzip compressed data, was "nonebot_plugin_pokemonfusion-1.0.4.tar", last modified: Mon Apr 10 05:22:16 2023, max compression
```

## Comparing `nonebot_plugin_pokemonfusion-1.0.3.tar` & `nonebot_plugin_pokemonfusion-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 05:18:06.027426 nonebot_plugin_pokemonfusion-1.0.3/
--rw-rw-rw-   0        0        0     1084 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      590 2023-04-10 05:18:06.027426 nonebot_plugin_pokemonfusion-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       98 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 05:18:06.014426 nonebot_plugin_pokemonfusion-1.0.3/nonebot_plugin_pokemonfusion/
--rw-rw-rw-   0        0        0     3389 2023-04-10 05:15:55.000000 nonebot_plugin_pokemonfusion-1.0.3/nonebot_plugin_pokemonfusion/__init__.py
--rw-rw-rw-   0        0        0      304 2023-04-10 04:58:57.000000 nonebot_plugin_pokemonfusion-1.0.3/nonebot_plugin_pokemonfusion/tesrt.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:18:06.026426 nonebot_plugin_pokemonfusion-1.0.3/nonebot_plugin_pokemonfusion.egg-info/
--rw-rw-rw-   0        0        0      590 2023-04-10 05:18:05.000000 nonebot_plugin_pokemonfusion-1.0.3/nonebot_plugin_pokemonfusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-04-10 05:18:05.000000 nonebot_plugin_pokemonfusion-1.0.3/nonebot_plugin_pokemonfusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 05:18:05.000000 nonebot_plugin_pokemonfusion-1.0.3/nonebot_plugin_pokemonfusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-10 05:18:05.000000 nonebot_plugin_pokemonfusion-1.0.3/nonebot_plugin_pokemonfusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-04-10 05:18:05.000000 nonebot_plugin_pokemonfusion-1.0.3/nonebot_plugin_pokemonfusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 05:18:06.027426 nonebot_plugin_pokemonfusion-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      818 2023-04-10 05:17:46.000000 nonebot_plugin_pokemonfusion-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:22:16.024904 nonebot_plugin_pokemonfusion-1.0.4/
+-rw-rw-rw-   0        0        0     1084 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      590 2023-04-10 05:22:16.024904 nonebot_plugin_pokemonfusion-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       98 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 05:22:16.011896 nonebot_plugin_pokemonfusion-1.0.4/nonebot_plugin_pokemonfusion/
+-rw-rw-rw-   0        0        0     3389 2023-04-10 05:20:34.000000 nonebot_plugin_pokemonfusion-1.0.4/nonebot_plugin_pokemonfusion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:22:16.023903 nonebot_plugin_pokemonfusion-1.0.4/nonebot_plugin_pokemonfusion.egg-info/
+-rw-rw-rw-   0        0        0      590 2023-04-10 05:22:15.000000 nonebot_plugin_pokemonfusion-1.0.4/nonebot_plugin_pokemonfusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-04-10 05:22:15.000000 nonebot_plugin_pokemonfusion-1.0.4/nonebot_plugin_pokemonfusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 05:22:15.000000 nonebot_plugin_pokemonfusion-1.0.4/nonebot_plugin_pokemonfusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-10 05:22:15.000000 nonebot_plugin_pokemonfusion-1.0.4/nonebot_plugin_pokemonfusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-04-10 05:22:15.000000 nonebot_plugin_pokemonfusion-1.0.4/nonebot_plugin_pokemonfusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 05:22:16.024904 nonebot_plugin_pokemonfusion-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      818 2023-04-10 05:22:05.000000 nonebot_plugin_pokemonfusion-1.0.4/setup.py
```

### Comparing `nonebot_plugin_pokemonfusion-1.0.3/LICENSE` & `nonebot_plugin_pokemonfusion-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pokemonfusion-1.0.3/PKG-INFO` & `nonebot_plugin_pokemonfusion-1.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_pokemonfusion
-Version: 1.0.3
+Version: 1.0.4
 Summary: Nonebot2的Pokemon Infinite Fusion中文版融合计算器插件
 Home-page: https://github.com/IllusiveBull/nonebot_plugin_pokemonfusion
 Author: IllusiveBull
 Author-email: xjn233@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot_plugin_pokemonfusion-1.0.3/nonebot_plugin_pokemonfusion/__init__.py` & `nonebot_plugin_pokemonfusion-1.0.4/nonebot_plugin_pokemonfusion/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pokemonfusion-1.0.3/setup.py` & `nonebot_plugin_pokemonfusion-1.0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r",encoding='utf-8') as fh:
   long_description = fh.read()
 requirements = [r.strip() for r in open("requirements.txt", 'r', encoding='utf-8').readlines()]
 
 setuptools.setup(
   name="nonebot_plugin_pokemonfusion",
-  version="1.0.3",
+  version="1.0.4",
   author="IllusiveBull",
   author_email="xjn233@gmail.com",
   description="Nonebot2的Pokemon Infinite Fusion中文版融合计算器插件",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/IllusiveBull/nonebot_plugin_pokemonfusion",
   packages=setuptools.find_packages(),
```

