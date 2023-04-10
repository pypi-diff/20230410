# Comparing `tmp/opsramp-analytics-utils-3.2.6.tar.gz` & `tmp/opsramp-analytics-utils-3.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opsramp-analytics-utils-3.2.6.tar", last modified: Tue Mar 14 08:55:17 2023, max compression
+gzip compressed data, was "opsramp-analytics-utils-3.2.7.tar", last modified: Mon Apr 10 12:14:48 2023, max compression
```

## Comparing `opsramp-analytics-utils-3.2.6.tar` & `opsramp-analytics-utils-3.2.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-03-14 08:55:17.795812 opsramp-analytics-utils-3.2.6/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1073 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.6/LICENSE
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      186 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.6/MANIFEST.in
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1361 2023-03-14 08:55:17.795812 opsramp-analytics-utils-3.2.6/PKG-INFO
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      711 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.6/README.md
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-03-14 08:55:17.187812 opsramp-analytics-utils-3.2.6/analytics_sdk/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       30 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/__init__.py
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-03-14 08:55:17.483812 opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      921 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/main.js
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)  3321723 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/main.wrapper.css
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)  2628164 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/main.wrapper.js
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-03-14 08:55:17.739812 opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      320 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/close.82b1ae2d.svg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    34172 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)   148200 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    64440 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    29136 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    64608 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      602 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      861 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1403 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     7536 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    11968 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    12136 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      733 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     4129 2022-07-11 05:34:48.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/components.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       38 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/constants.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    10055 2023-01-25 12:47:16.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/oap_dash.py
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-03-14 08:55:17.767812 opsramp-analytics-utils-3.2.6/analytics_sdk/process/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)        0 2022-07-27 14:35:38.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/process/__init__.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     4972 2022-09-21 10:21:08.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/process/process.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     3287 2022-09-28 12:26:39.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/process/querybuilder.py
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-03-14 08:55:17.787812 opsramp-analytics-utils-3.2.6/analytics_sdk/renderer/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)        0 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/renderer/__init__.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    30959 2023-03-14 08:52:14.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/renderer/excel.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     2887 2022-10-28 05:58:48.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/renderer/pdf.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    34116 2023-03-08 06:27:43.000000 opsramp-analytics-utils-3.2.6/analytics_sdk/utilities.py
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-03-14 08:55:17.795812 opsramp-analytics-utils-3.2.6/opsramp_analytics_utils.egg-info/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1361 2023-03-14 08:55:16.000000 opsramp-analytics-utils-3.2.6/opsramp_analytics_utils.egg-info/PKG-INFO
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1542 2023-03-14 08:55:16.000000 opsramp-analytics-utils-3.2.6/opsramp_analytics_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)        1 2023-03-14 08:55:16.000000 opsramp-analytics-utils-3.2.6/opsramp_analytics_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      108 2023-03-14 08:55:16.000000 opsramp-analytics-utils-3.2.6/opsramp_analytics_utils.egg-info/requires.txt
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       14 2023-03-14 08:55:16.000000 opsramp-analytics-utils-3.2.6/opsramp_analytics_utils.egg-info/top_level.txt
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      108 2022-06-28 07:34:29.000000 opsramp-analytics-utils-3.2.6/requires-install.txt
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       38 2023-03-14 08:55:17.795812 opsramp-analytics-utils-3.2.6/setup.cfg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      941 2023-03-14 08:52:14.000000 opsramp-analytics-utils-3.2.6/setup.py
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-04-10 12:14:48.533606 opsramp-analytics-utils-3.2.7/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1073 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.7/LICENSE
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      186 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.7/MANIFEST.in
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1361 2023-04-10 12:14:48.533606 opsramp-analytics-utils-3.2.7/PKG-INFO
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      711 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.7/README.md
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-04-10 12:14:48.009606 opsramp-analytics-utils-3.2.7/analytics_sdk/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       30 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/__init__.py
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-04-10 12:14:48.261606 opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      921 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/main.js
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)  3321723 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/main.wrapper.css
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)  2628164 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/main.wrapper.js
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-04-10 12:14:48.513606 opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      320 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/close.82b1ae2d.svg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    34172 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)   148200 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    64440 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    29136 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    64608 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      602 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      861 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1403 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     7536 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    11968 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    12136 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      733 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     4129 2022-07-11 05:34:48.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/components.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       38 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/constants.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    10055 2023-01-25 12:47:16.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/oap_dash.py
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-04-10 12:14:48.517606 opsramp-analytics-utils-3.2.7/analytics_sdk/process/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)        0 2022-07-27 14:35:38.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/process/__init__.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     5809 2023-04-10 11:19:33.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/process/process.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     3287 2022-09-28 12:26:39.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/process/querybuilder.py
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-04-10 12:14:48.525606 opsramp-analytics-utils-3.2.7/analytics_sdk/renderer/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)        0 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/renderer/__init__.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    30959 2023-03-14 08:52:14.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/renderer/excel.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     2887 2022-10-28 05:58:48.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/renderer/pdf.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    39245 2023-04-10 12:13:38.000000 opsramp-analytics-utils-3.2.7/analytics_sdk/utilities.py
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-04-10 12:14:48.533606 opsramp-analytics-utils-3.2.7/opsramp_analytics_utils.egg-info/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1361 2023-04-10 12:14:47.000000 opsramp-analytics-utils-3.2.7/opsramp_analytics_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1542 2023-04-10 12:14:47.000000 opsramp-analytics-utils-3.2.7/opsramp_analytics_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)        1 2023-04-10 12:14:47.000000 opsramp-analytics-utils-3.2.7/opsramp_analytics_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      108 2023-04-10 12:14:47.000000 opsramp-analytics-utils-3.2.7/opsramp_analytics_utils.egg-info/requires.txt
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       14 2023-04-10 12:14:47.000000 opsramp-analytics-utils-3.2.7/opsramp_analytics_utils.egg-info/top_level.txt
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      108 2023-04-03 11:09:31.000000 opsramp-analytics-utils-3.2.7/requires-install.txt
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       38 2023-04-10 12:14:48.533606 opsramp-analytics-utils-3.2.7/setup.cfg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      941 2023-04-10 12:11:16.000000 opsramp-analytics-utils-3.2.7/setup.py
```

### Comparing `opsramp-analytics-utils-3.2.6/LICENSE` & `opsramp-analytics-utils-3.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.2.6/PKG-INFO` & `opsramp-analytics-utils-3.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opsramp-analytics-utils
-Version: 3.2.6
+Version: 3.2.7
 Summary: OpsRamp Analytics SDK
 Home-page: https://github.com/opsramp/analytics-sdk
 Author: OpsRamp
 Author-email: opsramp@support.com
 License: UNKNOWN
 Description: ## OpsRamp Analytics Utilities
```

### Comparing `opsramp-analytics-utils-3.2.6/README.md` & `opsramp-analytics-utils-3.2.7/README.md`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/main.js` & `opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/main.js`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/main.wrapper.css` & `opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/main.wrapper.css`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/main.wrapper.js` & `opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/main.wrapper.js`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff` & `opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg` & `opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf` & `opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2` & `opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot` & `opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg` & `opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg` & `opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg` & `opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff` & `opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf` & `opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot` & `opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.2.6/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg` & `opsramp-analytics-utils-3.2.7/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.2.6/analytics_sdk/components.py` & `opsramp-analytics-utils-3.2.7/analytics_sdk/components.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.2.6/analytics_sdk/oap_dash.py` & `opsramp-analytics-utils-3.2.7/analytics_sdk/oap_dash.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.2.6/analytics_sdk/process/process.py` & `opsramp-analytics-utils-3.2.7/analytics_sdk/process/process.py`

 * *Files 16% similar despite different names*

```diff
@@ -153,8 +153,34 @@
     def set_app_description(self, app_description):
         self.app_description = app_description
 
     def set_query_builder(self, query_builder):
         self.query_builder = query_builder
     
     def get_query_builder(self):
-        return self.query_builder
+        return self.query_builder
+    
+    # Report Builder Methods
+    def get_dashboard_id(self):
+        self.dashboard_id = self.read_from_json('dashboardId', '')
+        return self.dashboard_id
+
+    def set_dashboard_id(self,dashboard_id):
+        self.dashboard_id = dashboard_id
+    
+    def get_partnerId(self):
+        self.partner_id = self.read_from_json('tenantId', '')
+        return self.partner_id
+    
+    def set_partnerId(self, partner_id):
+        self.partner_id = partner_id
+    
+    def get_tenantId(self):
+        self.get_client_id()
+        self.get_partnerId()
+        self.tenant_id = 0
+        if self.client_id is not None and self.client_id != '':
+            self.tenant_id = self.client_id
+        elif self.partner_id is not None and self.partner_id != '':
+            self.tenant_id = self.partner_id
+        return self.tenant_id
+
```

### Comparing `opsramp-analytics-utils-3.2.6/analytics_sdk/process/querybuilder.py` & `opsramp-analytics-utils-3.2.7/analytics_sdk/process/querybuilder.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.2.6/analytics_sdk/renderer/excel.py` & `opsramp-analytics-utils-3.2.7/analytics_sdk/renderer/excel.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.2.6/analytics_sdk/renderer/pdf.py` & `opsramp-analytics-utils-3.2.7/analytics_sdk/renderer/pdf.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.2.6/analytics_sdk/utilities.py` & `opsramp-analytics-utils-3.2.7/analytics_sdk/utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -407,15 +407,15 @@
                         logging.info(f'{pdf.analysis_run} pdf not found in storage trying for {storage_retry} time..')
                         continue
             else:
                 return response
         raise Exception(f'Generate_pdf:: pdf generation failed after max tries ({API_RETRY}), for run ::: {pdf.analysis_run}')
     except Exception as e:
         traceback.print_exc()
-        err_msg = f'Generate_pdf:: Exeception - pdf generation failed after max tries({API_RETRY}), for run ::: {analysis_run}'
+        err_msg = f'Generate_pdf:: Exeception - pdf generation failed after max tries({API_RETRY}), for run ::: {pdf.analysis_run}'
         raise Exception(err_msg)
 
 
 def is_file_in_storage(file_path: str):
     try:
         if storage_name == 's3':
             s3 = get_s3_client()
@@ -917,8 +917,123 @@
     res = call_put_requests(url , data=json.dumps(data), verify=False);
     if res == None or not res.ok:
         logger.error('Update run progress API is failed')
         return res
     else:
         logger.error('Update run progress result updated upto %d',  percent)
         return res
-    #TODO : Implement logic here to update the run
+    #TODO : Implement logic here to update the run
+    
+       
+# Report Builder Methods
+def generate_dashboard_pdf(dashboard_id):
+    logger.info(f'{dashboard_id} :: Entered into dashboard pdf generation process')
+    try:
+        url = os.getenv("DASH_BOARD_PDF_SERVICE")
+        jwt_token = os.getenv("OPSRAMP_JWT_TOKEN")
+        current_date = datetime.now()
+        # file_name = APP_ID.lower() + '-' + pdf.analysis_run[:8] + '-' + current_date.strftime("%Y-%m-%d-%H-%M-%S") + '.pdf'
+        report_path = ''
+        if storage_name == 's3':
+            report_path = PLATFORM_ROUTE
+        elif storage_name == 'ceph':
+            report_path = APP_ID.lower()
+        pdf = PDF(dashboard_id, url, report_path, current_date.strftime("%Y-%m-%d-%H-%M-%S"))
+        file_name = pdf.prepare_file_name(APP_ID.lower(), 'pdf')
+        file_path = pdf.report_path + '/' + pdf.analysis_run + '/pdf/' + file_name
+        data = {
+            'domain': BASE_API_URL,
+            'report': PLATFORM_ROUTE,
+            'run': pdf.analysis_run,
+            'route': '/full-view',
+            'token': jwt_token,
+            'app_id': APP_ID,
+            'size': 'A4',
+            'storage': storage_name,
+            'file_name': file_name,
+            'file_path': file_path
+        }
+
+        gen_retry = 1
+        while gen_retry <= 2:
+            logging.info(f'{pdf.analysis_run} :: pdf generation trying {gen_retry} time..')
+            gen_retry += 1
+            logging.info(f'b4 generation >> full file path : {file_path}')
+            response = pdf.generate(data)
+            logging.info(f'after generation >> full file path : {file_path}')
+            if response == 504:
+                storage_retry = 1
+                file_found = False
+                while storage_retry <= API_RETRY:
+                    logging.info(f'{pdf.analysis_run} checking the file is existing in storage or not {storage_retry} time..')
+                    file_found = is_file_in_storage(file_path)
+                    if file_found == True:
+                        logging.info(f'{pdf.analysis_run} the pdf file is found in storage')
+                        return file_path
+                    else:
+                        time.sleep(storage_retry * 30)
+                        storage_retry += 1
+                        logging.info(f'{pdf.analysis_run} pdf not found in storage trying for {storage_retry} time..')
+                        continue
+            else:
+                return response
+        raise Exception(f'Generate_pdf:: pdf generation failed after max tries ({API_RETRY}), for run ::: {pdf.analysis_run}')
+    except Exception as e:
+        traceback.print_exc()
+        err_msg = f'Generate_pdf:: Exeception - pdf generation failed after max tries({API_RETRY}), for run ::: {pdf.analysis_run}'
+        raise Exception(err_msg)
+
+
+def dashboard_init_mail(org_id, dashboard_id, toEmails, filePath, fileName):
+    logger.info('Entered into init_mail method')
+    try:
+        # /tenants/{tenantId}/runs/{id}/sends
+        url = BASE_API_URL + f'/reporting/api/v3/tenants/{org_id}/reportbuilder/sendmail'
+        data={
+                "recipients":toEmails,
+                "filePath":filePath,
+                "fileName":fileName
+            }
+        t1 = int(time.time())
+        res = call_post_requests(url , data=json.dumps(data), verify=False)
+        t2 = int(time.time())
+        duration = t2-t1
+        if duration > API_TIME_STACKS:
+            logging.info('Status update response took %d (greater than %d) seconds', duration, API_TIME_STACKS)
+        logger.info('Status update response is %s', res)
+    except Exception as e:
+        logger.error("Exception raised due to : " + repr(e))
+        traceback.print_exc()
+    logger.info('finished init_mail method')
+    
+    
+def get_dashboard_result(dashboard_Id, path, field=None, default_value=None):
+    try:
+        # run_id= f'{PLATFORM_ROUTE}/{run_id}/json/{run_id}'
+        #PLATFORM_ROUTE = 'report-builder'
+        #print('pathhh', path)
+        if storage_name == 's3':
+            run_id= f'{PLATFORM_ROUTE}/{dashboard_Id}/json/{path}/{dashboard_Id}'
+            print('locationnn',run_id)
+            s3 = get_s3_client()
+            res_object = s3.get_object(Bucket=BUCKET_NAME,Key=run_id)
+            serializedObject = res_object['Body'].read()
+            result = json.loads(serializedObject)
+            if field:
+                result = result.get(field, default_value)
+            return result
+        elif storage_name == 'ceph':
+            run_id= f'{APP_ID.lower()}/{dashboard_Id}/json/{path}/{dashboard_Id}'
+            s3 = get_ceph_resource()
+            data = BytesIO()
+            res_object = s3.Bucket(BUCKET_NAME).download_fileobj(Fileobj=data,Key=run_id)
+            res_object = data.getvalue()
+            result = json.loads(res_object)
+            if field:
+                result = result.get(field, default_value)
+            return result
+        else:
+            logger.info("No storages are found")
+    except Exception:
+        logger.error('An error occurred (NoSuchKey) when calling the GetObject operation: The specified key does not exist')
+        pass
+
```

### Comparing `opsramp-analytics-utils-3.2.6/opsramp_analytics_utils.egg-info/PKG-INFO` & `opsramp-analytics-utils-3.2.7/opsramp_analytics_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opsramp-analytics-utils
-Version: 3.2.6
+Version: 3.2.7
 Summary: OpsRamp Analytics SDK
 Home-page: https://github.com/opsramp/analytics-sdk
 Author: OpsRamp
 Author-email: opsramp@support.com
 License: UNKNOWN
 Description: ## OpsRamp Analytics Utilities
```

### Comparing `opsramp-analytics-utils-3.2.6/opsramp_analytics_utils.egg-info/SOURCES.txt` & `opsramp-analytics-utils-3.2.7/opsramp_analytics_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.2.6/setup.py` & `opsramp-analytics-utils-3.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     with open("requires-{}.txt".format(req_type)) as fp:
         requires = (line.strip() for line in fp)
         return [req for req in requires if req and not req.startswith("#")]
 
 
 setuptools.setup(
     name="opsramp-analytics-utils",
-    version="3.2.6",
+    version="3.2.7",
     author="OpsRamp",
     author_email="opsramp@support.com",
     description="OpsRamp Analytics SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=read_req_file("install"),
     url="https://github.com/opsramp/analytics-sdk",
```

