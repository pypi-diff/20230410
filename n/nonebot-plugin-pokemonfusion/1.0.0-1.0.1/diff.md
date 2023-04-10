# Comparing `tmp/nonebot_plugin_pokemonfusion-1.0.0.tar.gz` & `tmp/nonebot_plugin_pokemonfusion-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pokemonfusion-1.0.0.tar", last modified: Mon Apr 10 03:50:03 2023, max compression
+gzip compressed data, was "nonebot_plugin_pokemonfusion-1.0.1.tar", last modified: Mon Apr 10 04:04:40 2023, max compression
```

## Comparing `nonebot_plugin_pokemonfusion-1.0.0.tar` & `nonebot_plugin_pokemonfusion-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 03:50:03.124424 nonebot_plugin_pokemonfusion-1.0.0/
--rw-rw-rw-   0        0        0     1084 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      590 2023-04-10 03:50:03.124424 nonebot_plugin_pokemonfusion-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       98 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 03:50:03.110424 nonebot_plugin_pokemonfusion-1.0.0/nonebot_plugin_pokemonfusion/
--rw-rw-rw-   0        0        0     3279 2023-04-10 01:40:52.000000 nonebot_plugin_pokemonfusion-1.0.0/nonebot_plugin_pokemonfusion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 03:50:03.123432 nonebot_plugin_pokemonfusion-1.0.0/nonebot_plugin_pokemonfusion.egg-info/
--rw-rw-rw-   0        0        0      590 2023-04-10 03:50:03.000000 nonebot_plugin_pokemonfusion-1.0.0/nonebot_plugin_pokemonfusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-04-10 03:50:03.000000 nonebot_plugin_pokemonfusion-1.0.0/nonebot_plugin_pokemonfusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 03:50:03.000000 nonebot_plugin_pokemonfusion-1.0.0/nonebot_plugin_pokemonfusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-04-10 03:50:03.000000 nonebot_plugin_pokemonfusion-1.0.0/nonebot_plugin_pokemonfusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 03:50:03.124424 nonebot_plugin_pokemonfusion-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      683 2023-04-10 03:49:59.000000 nonebot_plugin_pokemonfusion-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 04:04:40.154366 nonebot_plugin_pokemonfusion-1.0.1/
+-rw-rw-rw-   0        0        0     1084 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      590 2023-04-10 04:04:40.154366 nonebot_plugin_pokemonfusion-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       98 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 04:04:40.143366 nonebot_plugin_pokemonfusion-1.0.1/nonebot_plugin_pokemonfusion/
+-rw-rw-rw-   0        0        0     3279 2023-04-10 01:40:52.000000 nonebot_plugin_pokemonfusion-1.0.1/nonebot_plugin_pokemonfusion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 04:04:40.153366 nonebot_plugin_pokemonfusion-1.0.1/nonebot_plugin_pokemonfusion.egg-info/
+-rw-rw-rw-   0        0        0      590 2023-04-10 04:04:40.000000 nonebot_plugin_pokemonfusion-1.0.1/nonebot_plugin_pokemonfusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-04-10 04:04:40.000000 nonebot_plugin_pokemonfusion-1.0.1/nonebot_plugin_pokemonfusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 04:04:40.000000 nonebot_plugin_pokemonfusion-1.0.1/nonebot_plugin_pokemonfusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-04-10 04:04:40.000000 nonebot_plugin_pokemonfusion-1.0.1/nonebot_plugin_pokemonfusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-04-10 04:04:40.000000 nonebot_plugin_pokemonfusion-1.0.1/nonebot_plugin_pokemonfusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 04:04:40.154366 nonebot_plugin_pokemonfusion-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      818 2023-04-10 04:03:25.000000 nonebot_plugin_pokemonfusion-1.0.1/setup.py
```

### Comparing `nonebot_plugin_pokemonfusion-1.0.0/LICENSE` & `nonebot_plugin_pokemonfusion-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pokemonfusion-1.0.0/PKG-INFO` & `nonebot_plugin_pokemonfusion-1.0.1/nonebot_plugin_pokemonfusion.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nonebot_plugin_pokemonfusion
-Version: 1.0.0
+Name: nonebot-plugin-pokemonfusion
+Version: 1.0.1
 Summary: Nonebot2的Pokemon Infinite Fusion中文版融合计算器插件
 Home-page: https://github.com/IllusiveBull/nonebot_plugin_pokemonfusion
 Author: IllusiveBull
 Author-email: xjn233@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot_plugin_pokemonfusion-1.0.0/nonebot_plugin_pokemonfusion/__init__.py` & `nonebot_plugin_pokemonfusion-1.0.1/nonebot_plugin_pokemonfusion/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pokemonfusion-1.0.0/nonebot_plugin_pokemonfusion.egg-info/PKG-INFO` & `nonebot_plugin_pokemonfusion-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nonebot-plugin-pokemonfusion
-Version: 1.0.0
+Name: nonebot_plugin_pokemonfusion
+Version: 1.0.1
 Summary: Nonebot2的Pokemon Infinite Fusion中文版融合计算器插件
 Home-page: https://github.com/IllusiveBull/nonebot_plugin_pokemonfusion
 Author: IllusiveBull
 Author-email: xjn233@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot_plugin_pokemonfusion-1.0.0/setup.py` & `nonebot_plugin_pokemonfusion-1.0.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import setuptools
 
 with open("README.md", "r",encoding='utf-8') as fh:
   long_description = fh.read()
+requirements = [r.strip() for r in open("requirements.txt", 'r', encoding='utf-8').readlines()]
 
 setuptools.setup(
   name="nonebot_plugin_pokemonfusion",
-  version="1.0.0",
+  version="1.0.1",
   author="IllusiveBull",
   author_email="xjn233@gmail.com",
   description="Nonebot2的Pokemon Infinite Fusion中文版融合计算器插件",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/IllusiveBull/nonebot_plugin_pokemonfusion",
   packages=setuptools.find_packages(),
   classifiers=[
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   ],
+  install_requires=requirements,    
 )
```

