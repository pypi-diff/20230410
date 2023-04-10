# Comparing `tmp/percy-appium-app-1.0.1.tar.gz` & `tmp/percy-appium-app-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "percy-appium-app-1.0.1.tar", last modified: Mon Apr  3 11:37:40 2023, max compression
+gzip compressed data, was "percy-appium-app-1.1.0.tar", last modified: Mon Apr 10 08:10:06 2023, max compression
```

## Comparing `percy-appium-app-1.0.1.tar` & `percy-appium-app-1.1.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:37:40.784965 percy-appium-app-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-03 11:37:40.784965 percy-appium-app-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:37:40.768965 percy-appium-app-1.0.1/percy/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/percy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:37:40.768965 percy-appium-app-1.0.1/percy/common/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/percy/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:37:40.768965 percy-appium-app-1.0.1/percy/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/percy/configs/devices.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:37:40.768965 percy-appium-app-1.0.1/percy/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/percy/errors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:37:40.772965 percy-appium-app-1.0.1/percy/lib/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/percy/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/percy/lib/app_percy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/percy/lib/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/percy/lib/cli_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/percy/lib/percy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/percy/lib/tile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:37:40.772965 percy-appium-app-1.0.1/percy/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/percy/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/percy/metadata/android_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/percy/metadata/ios_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/percy/metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/percy/metadata/metadata_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:37:40.776965 percy-appium-app-1.0.1/percy/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/percy/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/percy/providers/app_automate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/percy/providers/generic_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/percy/providers/provider_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/percy/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/percy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:37:40.776965 percy-appium-app-1.0.1/percy_appium_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-03 11:37:40.000000 percy-appium-app-1.0.1/percy_appium_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-03 11:37:40.000000 percy-appium-app-1.0.1/percy_appium_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 11:37:40.000000 percy-appium-app-1.0.1/percy_appium_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 11:37:40.000000 percy-appium-app-1.0.1/percy_appium_app.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-03 11:37:40.000000 percy-appium-app-1.0.1/percy_appium_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-03 11:37:40.000000 percy-appium-app-1.0.1/percy_appium_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 11:37:40.784965 percy-appium-app-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:37:40.784965 percy-appium-app-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/tests/test_android_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/tests/test_app_automate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/tests/test_app_percy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/tests/test_cli_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/tests/test_generic_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/tests/test_ios_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/tests/test_metadata_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/tests/test_percy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/tests/test_screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-03 11:37:17.000000 percy-appium-app-1.0.1/tests/test_tile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:10:06.352512 percy-appium-app-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-10 08:10:06.352512 percy-appium-app-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:10:06.348512 percy-appium-app-1.1.0/percy/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:10:06.348512 percy-appium-app-1.1.0/percy/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:10:06.348512 percy-appium-app-1.1.0/percy/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/configs/devices.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:10:06.348512 percy-appium-app-1.1.0/percy/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/errors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:10:06.352512 percy-appium-app-1.1.0/percy/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/lib/app_percy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/lib/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/lib/cli_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/lib/percy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/lib/tile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:10:06.352512 percy-appium-app-1.1.0/percy/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/metadata/android_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/metadata/ios_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/metadata/metadata_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:10:06.352512 percy-appium-app-1.1.0/percy/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/providers/app_automate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/providers/generic_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/providers/provider_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/percy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:10:06.352512 percy-appium-app-1.1.0/percy_appium_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-10 08:10:06.000000 percy-appium-app-1.1.0/percy_appium_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-10 08:10:06.000000 percy-appium-app-1.1.0/percy_appium_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:10:06.000000 percy-appium-app-1.1.0/percy_appium_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:10:06.000000 percy-appium-app-1.1.0/percy_appium_app.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-10 08:10:06.000000 percy-appium-app-1.1.0/percy_appium_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 08:10:06.000000 percy-appium-app-1.1.0/percy_appium_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 08:10:06.352512 percy-appium-app-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:10:06.352512 percy-appium-app-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/tests/test_android_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/tests/test_app_automate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/tests/test_app_percy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/tests/test_cli_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/tests/test_generic_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/tests/test_ios_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/tests/test_metadata_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/tests/test_percy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/tests/test_screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-10 08:09:38.000000 percy-appium-app-1.1.0/tests/test_tile.py
```

### Comparing `percy-appium-app-1.0.1/LICENSE` & `percy-appium-app-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/PKG-INFO` & `percy-appium-app-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: percy-appium-app
-Version: 1.0.1
+Version: 1.1.0
 Summary: Python client for visual testing with Percy for mobile apps
 Home-page: https://github.com/percy/percy-appium-python
 Author: Perceptual Inc.
 Author-email: team@percy.io
 License: MIT
 Keywords: appium percy visual testing
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -34,14 +34,15 @@
 ```
 
 pip install Percy appium package:
 
 ```ssh-session
 $ pip install percy-appium-app
 ```
+> Note: This package is tested on Python versions 3.6, 3.8, 3.9 as part of unit tests. It should ideally work on all Python 3.6+ versions
 
 ## Usage
 
 This is an example test using the `percy_screenshot` function.
 
 ``` python
 from appium import webdriver
```

### Comparing `percy-appium-app-1.0.1/README.md` & `percy-appium-app-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 ```
 
 pip install Percy appium package:
 
 ```ssh-session
 $ pip install percy-appium-app
 ```
+> Note: This package is tested on Python versions 3.6, 3.8, 3.9 as part of unit tests. It should ideally work on all Python 3.6+ versions
 
 ## Usage
 
 This is an example test using the `percy_screenshot` function.
 
 ``` python
 from appium import webdriver
```

### Comparing `percy-appium-app-1.0.1/percy/configs/devices.json` & `percy-appium-app-1.1.0/percy/configs/devices.json`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/percy/lib/app_percy.py` & `percy-appium-app-1.1.0/percy/lib/app_percy.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/percy/lib/cache.py` & `percy-appium-app-1.1.0/percy/lib/cache.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/percy/lib/cli_wrapper.py` & `percy-appium-app-1.1.0/percy/lib/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/percy/lib/percy_options.py` & `percy-appium-app-1.1.0/percy/lib/percy_options.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/percy/lib/tile.py` & `percy-appium-app-1.1.0/percy/lib/tile.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/percy/metadata/android_metadata.py` & `percy-appium-app-1.1.0/percy/metadata/android_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/percy/metadata/ios_metadata.py` & `percy-appium-app-1.1.0/percy/metadata/ios_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/percy/metadata/metadata.py` & `percy-appium-app-1.1.0/percy/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/percy/providers/app_automate.py` & `percy-appium-app-1.1.0/percy/providers/app_automate.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/percy/providers/generic_provider.py` & `percy-appium-app-1.1.0/percy/providers/generic_provider.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/percy/providers/provider_resolver.py` & `percy-appium-app-1.1.0/percy/providers/provider_resolver.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/percy/screenshot.py` & `percy-appium-app-1.1.0/percy/screenshot.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/percy_appium_app.egg-info/PKG-INFO` & `percy-appium-app-1.1.0/percy_appium_app.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: percy-appium-app
-Version: 1.0.1
+Version: 1.1.0
 Summary: Python client for visual testing with Percy for mobile apps
 Home-page: https://github.com/percy/percy-appium-python
 Author: Perceptual Inc.
 Author-email: team@percy.io
 License: MIT
 Keywords: appium percy visual testing
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -34,14 +34,15 @@
 ```
 
 pip install Percy appium package:
 
 ```ssh-session
 $ pip install percy-appium-app
 ```
+> Note: This package is tested on Python versions 3.6, 3.8, 3.9 as part of unit tests. It should ideally work on all Python 3.6+ versions
 
 ## Usage
 
 This is an example test using the `percy_screenshot` function.
 
 ``` python
 from appium import webdriver
```

### Comparing `percy-appium-app-1.0.1/percy_appium_app.egg-info/SOURCES.txt` & `percy-appium-app-1.1.0/percy_appium_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/setup.py` & `percy-appium-app-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/tests/test_android_metadata.py` & `percy-appium-app-1.1.0/tests/test_android_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/tests/test_app_automate.py` & `percy-appium-app-1.1.0/tests/test_app_automate.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/tests/test_app_percy.py` & `percy-appium-app-1.1.0/tests/test_app_percy.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/tests/test_cache.py` & `percy-appium-app-1.1.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/tests/test_cli_wrapper.py` & `percy-appium-app-1.1.0/tests/test_cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/tests/test_generic_provider.py` & `percy-appium-app-1.1.0/tests/test_generic_provider.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/tests/test_ios_metadata.py` & `percy-appium-app-1.1.0/tests/test_ios_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/tests/test_metadata.py` & `percy-appium-app-1.1.0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/tests/test_metadata_resolver.py` & `percy-appium-app-1.1.0/tests/test_metadata_resolver.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/tests/test_percy_options.py` & `percy-appium-app-1.1.0/tests/test_percy_options.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/tests/test_screenshot.py` & `percy-appium-app-1.1.0/tests/test_screenshot.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.0.1/tests/test_tile.py` & `percy-appium-app-1.1.0/tests/test_tile.py`

 * *Files identical despite different names*

