# Comparing `tmp/fast-weather-0.1.1.tar.gz` & `tmp/fast-weather-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-weather-0.1.1.tar", last modified: Fri Feb  3 06:53:42 2023, max compression
+gzip compressed data, was "fast-weather-0.1.2.tar", last modified: Mon Apr 10 15:59:20 2023, max compression
```

## Comparing `fast-weather-0.1.1.tar` & `fast-weather-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sunxianyong   (501) staff       (20)        0 2023-02-03 06:53:42.058557 fast-weather-0.1.1/
--rw-r--r--   0 sunxianyong   (501) staff       (20)     1060 2023-02-03 02:48:16.000000 fast-weather-0.1.1/LICENSE
--rw-r--r--   0 sunxianyong   (501) staff       (20)      646 2023-02-03 06:53:42.058145 fast-weather-0.1.1/PKG-INFO
--rw-r--r--   0 sunxianyong   (501) staff       (20)       12 2023-02-03 06:21:55.000000 fast-weather-0.1.1/README.md
-drwxr-xr-x   0 sunxianyong   (501) staff       (20)        0 2023-02-03 06:53:42.055266 fast-weather-0.1.1/fast_weather/
--rw-r--r--   0 sunxianyong   (501) staff       (20)       18 2023-02-03 06:51:53.000000 fast-weather-0.1.1/fast_weather/__init__.py
--rw-r--r--   0 sunxianyong   (501) staff       (20)        0 2023-02-03 06:26:49.000000 fast-weather-0.1.1/fast_weather/__version__.py
--rw-r--r--   0 sunxianyong   (501) staff       (20)      193 2023-02-03 06:52:44.000000 fast-weather-0.1.1/fast_weather/main.py
-drwxr-xr-x   0 sunxianyong   (501) staff       (20)        0 2023-02-03 06:53:42.057657 fast-weather-0.1.1/fast_weather.egg-info/
--rw-r--r--   0 sunxianyong   (501) staff       (20)      646 2023-02-03 06:53:41.000000 fast-weather-0.1.1/fast_weather.egg-info/PKG-INFO
--rw-r--r--   0 sunxianyong   (501) staff       (20)      279 2023-02-03 06:53:42.000000 fast-weather-0.1.1/fast_weather.egg-info/SOURCES.txt
--rw-r--r--   0 sunxianyong   (501) staff       (20)        1 2023-02-03 06:53:41.000000 fast-weather-0.1.1/fast_weather.egg-info/dependency_links.txt
--rw-r--r--   0 sunxianyong   (501) staff       (20)       17 2023-02-03 06:53:41.000000 fast-weather-0.1.1/fast_weather.egg-info/requires.txt
--rw-r--r--   0 sunxianyong   (501) staff       (20)       13 2023-02-03 06:53:41.000000 fast-weather-0.1.1/fast_weather.egg-info/top_level.txt
--rw-r--r--   0 sunxianyong   (501) staff       (20)       38 2023-02-03 06:53:42.058716 fast-weather-0.1.1/setup.cfg
--rw-r--r--   0 sunxianyong   (501) staff       (20)     3820 2023-02-03 06:53:37.000000 fast-weather-0.1.1/setup.py
+drwxr-xr-x   0 sunxianyong   (501) staff       (20)        0 2023-04-10 15:59:20.594186 fast-weather-0.1.2/
+-rw-r--r--   0 sunxianyong   (501) staff       (20)     1060 2023-02-03 02:48:16.000000 fast-weather-0.1.2/LICENSE
+-rw-r--r--   0 sunxianyong   (501) staff       (20)      646 2023-04-10 15:59:20.593906 fast-weather-0.1.2/PKG-INFO
+-rw-r--r--   0 sunxianyong   (501) staff       (20)       12 2023-02-03 06:21:55.000000 fast-weather-0.1.2/README.md
+drwxr-xr-x   0 sunxianyong   (501) staff       (20)        0 2023-04-10 15:59:20.591940 fast-weather-0.1.2/fast_weather/
+-rw-r--r--   0 sunxianyong   (501) staff       (20)       21 2023-04-10 15:32:40.000000 fast-weather-0.1.2/fast_weather/__init__.py
+-rw-r--r--   0 sunxianyong   (501) staff       (20)       22 2023-04-10 15:57:53.000000 fast-weather-0.1.2/fast_weather/__version__.py
+-rw-r--r--   0 sunxianyong   (501) staff       (20)      198 2023-04-10 15:49:09.000000 fast-weather-0.1.2/fast_weather/weather.py
+drwxr-xr-x   0 sunxianyong   (501) staff       (20)        0 2023-04-10 15:59:20.593588 fast-weather-0.1.2/fast_weather.egg-info/
+-rw-r--r--   0 sunxianyong   (501) staff       (20)      646 2023-04-10 15:59:20.000000 fast-weather-0.1.2/fast_weather.egg-info/PKG-INFO
+-rw-r--r--   0 sunxianyong   (501) staff       (20)      282 2023-04-10 15:59:20.000000 fast-weather-0.1.2/fast_weather.egg-info/SOURCES.txt
+-rw-r--r--   0 sunxianyong   (501) staff       (20)        1 2023-04-10 15:59:20.000000 fast-weather-0.1.2/fast_weather.egg-info/dependency_links.txt
+-rw-r--r--   0 sunxianyong   (501) staff       (20)       17 2023-04-10 15:59:20.000000 fast-weather-0.1.2/fast_weather.egg-info/requires.txt
+-rw-r--r--   0 sunxianyong   (501) staff       (20)       13 2023-04-10 15:59:20.000000 fast-weather-0.1.2/fast_weather.egg-info/top_level.txt
+-rw-r--r--   0 sunxianyong   (501) staff       (20)       38 2023-04-10 15:59:20.594256 fast-weather-0.1.2/setup.cfg
+-rw-r--r--   0 sunxianyong   (501) staff       (20)     3815 2023-04-10 15:59:18.000000 fast-weather-0.1.2/setup.py
```

### Comparing `fast-weather-0.1.1/LICENSE` & `fast-weather-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fast-weather-0.1.1/PKG-INFO` & `fast-weather-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-weather
-Version: 0.1.1
+Version: 0.1.2
 Summary: 天气查询
 Home-page: https://www.wolai.com/sunxianyong/u5SSoLUbfmHb2aELs5jPGn
 Author: Qin Qiu
 Author-email: sxy122333@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `fast-weather-0.1.1/fast_weather.egg-info/PKG-INFO` & `fast-weather-0.1.2/fast_weather.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-weather
-Version: 0.1.1
+Version: 0.1.2
 Summary: 天气查询
 Home-page: https://www.wolai.com/sunxianyong/u5SSoLUbfmHb2aELs5jPGn
 Author: Qin Qiu
 Author-email: sxy122333@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `fast-weather-0.1.1/setup.py` & `fast-weather-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'fast-weather'
 DESCRIPTION = open('README.md').read()
 URL = 'https://www.wolai.com/sunxianyong/u5SSoLUbfmHb2aELs5jPGn'
 EMAIL = 'sxy122333@outlook.com'
 AUTHOR = 'Qin Qiu'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.1'
+VERSION = ''
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
     'requests==2.28.2',
 ]
```

