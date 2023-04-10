# Comparing `tmp/nonebot_plugin_pokemonfusion-1.0.5.tar.gz` & `tmp/nonebot_plugin_pokemonfusion-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pokemonfusion-1.0.5.tar", last modified: Mon Apr 10 05:39:52 2023, max compression
+gzip compressed data, was "nonebot_plugin_pokemonfusion-1.0.6.tar", last modified: Mon Apr 10 05:55:43 2023, max compression
```

## Comparing `nonebot_plugin_pokemonfusion-1.0.5.tar` & `nonebot_plugin_pokemonfusion-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 05:39:52.610388 nonebot_plugin_pokemonfusion-1.0.5/
--rw-rw-rw-   0        0        0     1084 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      590 2023-04-10 05:39:52.610388 nonebot_plugin_pokemonfusion-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       98 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 05:39:52.602388 nonebot_plugin_pokemonfusion-1.0.5/nonebot_plugin_pokemonfusion/
--rw-rw-rw-   0        0        0     3497 2023-04-10 05:36:37.000000 nonebot_plugin_pokemonfusion-1.0.5/nonebot_plugin_pokemonfusion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:39:52.609388 nonebot_plugin_pokemonfusion-1.0.5/nonebot_plugin_pokemonfusion.egg-info/
--rw-rw-rw-   0        0        0      590 2023-04-10 05:39:52.000000 nonebot_plugin_pokemonfusion-1.0.5/nonebot_plugin_pokemonfusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-04-10 05:39:52.000000 nonebot_plugin_pokemonfusion-1.0.5/nonebot_plugin_pokemonfusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 05:39:52.000000 nonebot_plugin_pokemonfusion-1.0.5/nonebot_plugin_pokemonfusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-04-10 05:39:52.000000 nonebot_plugin_pokemonfusion-1.0.5/nonebot_plugin_pokemonfusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-04-10 05:39:52.000000 nonebot_plugin_pokemonfusion-1.0.5/nonebot_plugin_pokemonfusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 05:39:52.610388 nonebot_plugin_pokemonfusion-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      818 2023-04-10 05:39:47.000000 nonebot_plugin_pokemonfusion-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:55:43.064290 nonebot_plugin_pokemonfusion-1.0.6/
+-rw-rw-rw-   0        0        0     1084 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      590 2023-04-10 05:55:43.064290 nonebot_plugin_pokemonfusion-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       98 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 05:55:43.058283 nonebot_plugin_pokemonfusion-1.0.6/nonebot_plugin_pokemonfusion/
+-rw-rw-rw-   0        0        0     3497 2023-04-10 05:36:37.000000 nonebot_plugin_pokemonfusion-1.0.6/nonebot_plugin_pokemonfusion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:55:43.064290 nonebot_plugin_pokemonfusion-1.0.6/nonebot_plugin_pokemonfusion/resources/
+-rw-rw-rw-   0        0        0    13834 2023-04-09 07:34:55.000000 nonebot_plugin_pokemonfusion-1.0.6/nonebot_plugin_pokemonfusion/resources/pokemons.json
+drwxrwxrwx   0        0        0        0 2023-04-10 05:55:43.063292 nonebot_plugin_pokemonfusion-1.0.6/nonebot_plugin_pokemonfusion.egg-info/
+-rw-rw-rw-   0        0        0      590 2023-04-10 05:55:42.000000 nonebot_plugin_pokemonfusion-1.0.6/nonebot_plugin_pokemonfusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2023-04-10 05:55:43.000000 nonebot_plugin_pokemonfusion-1.0.6/nonebot_plugin_pokemonfusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 05:55:42.000000 nonebot_plugin_pokemonfusion-1.0.6/nonebot_plugin_pokemonfusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-10 05:55:42.000000 nonebot_plugin_pokemonfusion-1.0.6/nonebot_plugin_pokemonfusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-04-10 05:55:42.000000 nonebot_plugin_pokemonfusion-1.0.6/nonebot_plugin_pokemonfusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 05:55:43.065291 nonebot_plugin_pokemonfusion-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      959 2023-04-10 05:55:41.000000 nonebot_plugin_pokemonfusion-1.0.6/setup.py
```

### Comparing `nonebot_plugin_pokemonfusion-1.0.5/LICENSE` & `nonebot_plugin_pokemonfusion-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pokemonfusion-1.0.5/PKG-INFO` & `nonebot_plugin_pokemonfusion-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_pokemonfusion
-Version: 1.0.5
+Version: 1.0.6
 Summary: Nonebot2的Pokemon Infinite Fusion中文版融合计算器插件
 Home-page: https://github.com/IllusiveBull/nonebot_plugin_pokemonfusion
 Author: IllusiveBull
 Author-email: xjn233@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot_plugin_pokemonfusion-1.0.5/nonebot_plugin_pokemonfusion/__init__.py` & `nonebot_plugin_pokemonfusion-1.0.6/nonebot_plugin_pokemonfusion/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pokemonfusion-1.0.5/nonebot_plugin_pokemonfusion.egg-info/PKG-INFO` & `nonebot_plugin_pokemonfusion-1.0.6/nonebot_plugin_pokemonfusion.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pokemonfusion
-Version: 1.0.5
+Version: 1.0.6
 Summary: Nonebot2的Pokemon Infinite Fusion中文版融合计算器插件
 Home-page: https://github.com/IllusiveBull/nonebot_plugin_pokemonfusion
 Author: IllusiveBull
 Author-email: xjn233@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot_plugin_pokemonfusion-1.0.5/setup.py` & `nonebot_plugin_pokemonfusion-1.0.6/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 
 with open("README.md", "r",encoding='utf-8') as fh:
   long_description = fh.read()
 requirements = [r.strip() for r in open("requirements.txt", 'r', encoding='utf-8').readlines()]
 
 setuptools.setup(
   name="nonebot_plugin_pokemonfusion",
-  version="1.0.5",
+  version="1.0.6",
   author="IllusiveBull",
   author_email="xjn233@gmail.com",
   description="Nonebot2的Pokemon Infinite Fusion中文版融合计算器插件",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/IllusiveBull/nonebot_plugin_pokemonfusion",
+  include_package_data = True,
   packages=setuptools.find_packages(),
   classifiers=[
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   ],
   install_requires=requirements,    
+  package_data = {"nonebot_plugin_pokemonfusion":["nonebot_plugin_pokemonfusion/resources/pokemons.json"]},
 )
```

