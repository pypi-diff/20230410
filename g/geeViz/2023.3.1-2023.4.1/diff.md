# Comparing `tmp/geeViz-2023.3.1.tar.gz` & `tmp/geeViz-2023.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geeViz-2023.3.1.tar", last modified: Wed Mar 22 17:54:46 2023, max compression
+gzip compressed data, was "geeViz-2023.4.1.tar", last modified: Mon Apr 10 21:03:29 2023, max compression
```

## Comparing `geeViz-2023.3.1.tar` & `geeViz-2023.4.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 17:54:33.007176 geeViz-2023.3.1/
--rw-rw-rw-   0        0        0      574 2021-03-05 23:03:09.000000 geeViz-2023.3.1/LICENSE
--rw-rw-rw-   0        0        0     3900 2023-03-22 17:54:46.023843 geeViz-2023.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     3180 2023-03-22 17:21:57.000000 geeViz-2023.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-22 17:54:35.632382 geeViz-2023.3.1/geeViz/
--rw-rw-rw-   0        0        0      118 2023-03-22 17:22:51.000000 geeViz-2023.3.1/geeViz/__init__.py
--rw-rw-rw-   0        0        0    18421 2022-12-22 20:16:14.000000 geeViz-2023.3.1/geeViz/assetManagerLib.py
--rw-rw-rw-   0        0        0    94753 2023-03-16 20:15:29.000000 geeViz-2023.3.1/geeViz/changeDetectionLib.py
-drwxrwxrwx   0        0        0        0 2023-03-22 17:54:41.914137 geeViz-2023.3.1/geeViz/examples/
--rw-rw-rw-   0        0        0     5366 2023-03-22 17:20:31.000000 geeViz-2023.3.1/geeViz/examples/CCDCViz.py
--rw-rw-rw-   0        0        0    11674 2023-03-17 22:07:28.000000 geeViz-2023.3.1/geeViz/examples/CCDCVizNotebook.ipynb
--rw-rw-rw-   0        0        0     7865 2022-02-07 19:59:20.000000 geeViz-2023.3.1/geeViz/examples/CCDCWrapper.py
--rw-rw-rw-   0        0        0     4342 2022-04-15 21:41:00.000000 geeViz-2023.3.1/geeViz/examples/GFSTimeLapse.py
--rw-rw-rw-   0        0        0     6156 2023-03-17 20:39:50.000000 geeViz-2023.3.1/geeViz/examples/LANDTRENDRViz.py
--rw-rw-rw-   0        0        0     9374 2023-03-22 17:42:33.000000 geeViz-2023.3.1/geeViz/examples/LANDTRENDRWrapper.py
--rw-rw-rw-   0        0        0    15519 2023-03-17 22:54:36.000000 geeViz-2023.3.1/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb
--rw-rw-rw-   0        0        0    12431 2023-03-22 17:20:58.000000 geeViz-2023.3.1/geeViz/examples/LCMAP_and_LCMS_Viewer.py
--rw-rw-rw-   0        0        0    19316 2023-03-17 23:04:04.000000 geeViz-2023.3.1/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb
--rw-rw-rw-   0        0        0      118 2023-03-22 17:22:51.000000 geeViz-2023.3.1/geeViz/examples/__init__.py
--rw-rw-rw-   0        0        0     5672 2023-03-22 17:20:22.000000 geeViz-2023.3.1/geeViz/examples/geeViewExample.py
--rw-rw-rw-   0        0        0    16777 2023-03-17 22:12:16.000000 geeViz-2023.3.1/geeViz/examples/geeViewExampleNotebook.ipynb
--rw-rw-rw-   0        0        0     5653 2022-02-07 23:21:45.000000 geeViz-2023.3.1/geeViz/examples/getClimateWrapper.py
--rw-rw-rw-   0        0        0    14015 2023-01-09 16:55:27.000000 geeViz-2023.3.1/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py
--rw-rw-rw-   0        0        0    11238 2022-06-15 22:15:23.000000 geeViz-2023.3.1/geeViz/examples/getLandsatWrapper.py
--rw-rw-rw-   0        0        0    18281 2023-03-17 22:20:04.000000 geeViz-2023.3.1/geeViz/examples/getLandsatWrapperNotebook.ipynb
--rw-rw-rw-   0        0        0    12016 2022-08-23 16:04:44.000000 geeViz-2023.3.1/geeViz/examples/getSentinel2Wrapper.py
--rw-rw-rw-   0        0        0     8991 2022-10-26 19:30:20.000000 geeViz-2023.3.1/geeViz/examples/harmonicRegressionWrapper.py
--rw-rw-rw-   0        0        0     8050 2023-03-22 17:46:00.000000 geeViz-2023.3.1/geeViz/examples/lcmsViewerExample.py
--rw-rw-rw-   0        0        0    18271 2023-03-22 17:21:17.000000 geeViz-2023.3.1/geeViz/examples/lcmsViewerExampleNotebook.ipynb
--rw-rw-rw-   0        0        0    13051 2022-02-16 00:28:08.000000 geeViz-2023.3.1/geeViz/examples/phEEnoVizWrapper.py
--rw-rw-rw-   0        0        0     1038 2022-02-01 00:39:23.000000 geeViz-2023.3.1/geeViz/examples/taskTrackerExample.py
--rw-rw-rw-   0        0        0     6171 2022-02-01 00:38:52.000000 geeViz-2023.3.1/geeViz/examples/timeLapseExample.py
--rw-rw-rw-   0        0        0     1741 2021-04-01 17:15:14.000000 geeViz-2023.3.1/geeViz/gcpLib.py
-drwxrwxrwx   0        0        0        0 2023-03-22 17:54:41.976648 geeViz-2023.3.1/geeViz/geeView/
-drwxrwxrwx   0        0        0        0 2023-03-22 17:54:42.070402 geeViz-2023.3.1/geeViz/geeView/css/
--rw-rw-rw-   0        0        0    18958 2023-03-09 02:29:15.000000 geeViz-2023.3.1/geeViz/geeView/css/style.min.css
-drwxrwxrwx   0        0        0        0 2023-03-22 17:54:44.554979 geeViz-2023.3.1/geeViz/geeView/images/
--rw-rw-rw-   0        0        0     7295 2021-04-01 17:15:14.000000 geeViz-2023.3.1/geeViz/geeView/images/EE-logo-150.png
--rw-rw-rw-   0        0        0    10301 2021-04-01 17:15:14.000000 geeViz-2023.3.1/geeViz/geeView/images/GEE.png
--rw-rw-rw-   0        0        0     5692 2022-08-19 21:41:40.000000 geeViz-2023.3.1/geeViz/geeView/images/GEE_logo_transparent.png
--rw-rw-rw-   0        0        0     4551 2021-04-01 17:15:14.000000 geeViz-2023.3.1/geeViz/geeView/images/RCR-logo.jpg
--rw-rw-rw-   0        0        0    35328 2022-12-07 01:04:30.000000 geeViz-2023.3.1/geeViz/geeView/images/Thumbs.db
--rw-rw-rw-   0        0        0     8352 2021-04-01 17:15:14.000000 geeViz-2023.3.1/geeViz/geeView/images/cumulative_icon.png
--rw-rw-rw-   0        0        0     1502 2021-04-01 17:15:15.000000 geeViz-2023.3.1/geeViz/geeView/images/layer_icon.png
--rw-rw-rw-   0        0        0   230271 2022-06-28 20:18:38.000000 geeViz-2023.3.1/geeViz/geeView/images/logos_usda-fs.svg
--rw-rw-rw-   0        0        0   229463 2022-06-30 19:30:12.000000 geeViz-2023.3.1/geeViz/geeView/images/logos_usda-fs_bn-dk-01.svg
--rw-rw-rw-   0        0        0      635 2022-06-29 22:17:42.000000 geeViz-2023.3.1/geeViz/geeView/images/menu-hamburger_ffffff.svg
--rw-rw-rw-   0        0        0     1489 2021-04-01 17:15:15.000000 geeViz-2023.3.1/geeViz/geeView/images/usdalogo.png
--rw-rw-rw-   0        0        0     8174 2021-04-01 17:15:15.000000 geeViz-2023.3.1/geeViz/geeView/images/usfslogo.png
--rw-rw-rw-   0        0        0     3309 2023-03-08 18:54:11.000000 geeViz-2023.3.1/geeViz/geeView/index.html
-drwxrwxrwx   0        0        0        0 2023-03-22 17:54:45.633195 geeViz-2023.3.1/geeViz/geeView/js/
--rw-rw-rw-   0        0        0    45351 2020-01-16 17:35:18.000000 geeViz-2023.3.1/geeViz/geeView/js/gena-gee-palettes.js
--rw-rw-rw-   0        0        0   329151 2023-03-08 19:33:13.000000 geeViz-2023.3.1/geeViz/geeView/js/lcms-viewer.min.js
--rw-rw-rw-   0        0        0     1021 2023-03-08 18:47:59.000000 geeViz-2023.3.1/geeViz/geeView/js/load.min.js
--rw-rw-rw-   0        0        0    31548 2023-03-22 17:46:34.000000 geeViz-2023.3.1/geeViz/geeView/js/runGeeViz.js
--rw-rw-rw-   0        0        0    11128 2023-03-22 17:11:41.000000 geeViz-2023.3.1/geeViz/geeView.py
--rw-rw-rw-   0        0        0   174861 2023-03-08 22:01:44.000000 geeViz-2023.3.1/geeViz/getImagesLib.py
--rw-rw-rw-   0        0        0     7467 2021-04-01 17:15:14.000000 geeViz-2023.3.1/geeViz/migrateGEEAssets.py
--rw-rw-rw-   0        0        0    20743 2022-06-01 18:25:26.000000 geeViz-2023.3.1/geeViz/phEEnoViz.py
--rw-rw-rw-   0        0        0     9885 2022-11-30 20:14:56.000000 geeViz-2023.3.1/geeViz/taskManagerLib.py
-drwxrwxrwx   0        0        0        0 2023-03-22 17:54:36.194930 geeViz-2023.3.1/geeViz.egg-info/
--rw-rw-rw-   0        0        0     3900 2023-03-22 17:54:32.000000 geeViz-2023.3.1/geeViz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1945 2023-03-22 17:54:32.000000 geeViz-2023.3.1/geeViz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 17:54:32.000000 geeViz-2023.3.1/geeViz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-03-22 17:54:32.000000 geeViz-2023.3.1/geeViz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-22 17:54:32.000000 geeViz-2023.3.1/geeViz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-22 17:54:46.101975 geeViz-2023.3.1/setup.cfg
--rw-rw-rw-   0        0        0     2200 2022-07-06 19:24:37.000000 geeViz-2023.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:03:23.710599 geeViz-2023.4.1/
+-rw-rw-rw-   0        0        0      574 2021-03-05 23:03:09.000000 geeViz-2023.4.1/LICENSE
+-rw-rw-rw-   0        0        0     3900 2023-04-10 21:03:29.304773 geeViz-2023.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3180 2023-03-22 17:21:57.000000 geeViz-2023.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 21:03:24.741896 geeViz-2023.4.1/geeViz/
+-rw-rw-rw-   0        0        0      118 2023-04-10 20:50:35.000000 geeViz-2023.4.1/geeViz/__init__.py
+-rw-rw-rw-   0        0        0    23523 2023-04-10 20:44:55.000000 geeViz-2023.4.1/geeViz/assetManagerLib.py
+-rw-rw-rw-   0        0        0    95071 2023-04-10 17:24:49.000000 geeViz-2023.4.1/geeViz/changeDetectionLib.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:03:27.507749 geeViz-2023.4.1/geeViz/examples/
+-rw-rw-rw-   0        0        0     5366 2023-04-10 20:44:09.000000 geeViz-2023.4.1/geeViz/examples/CCDCViz.py
+-rw-rw-rw-   0        0        0    11674 2023-03-17 22:07:28.000000 geeViz-2023.4.1/geeViz/examples/CCDCVizNotebook.ipynb
+-rw-rw-rw-   0        0        0     7865 2022-02-07 19:59:20.000000 geeViz-2023.4.1/geeViz/examples/CCDCWrapper.py
+-rw-rw-rw-   0        0        0     4342 2022-04-15 21:41:00.000000 geeViz-2023.4.1/geeViz/examples/GFSTimeLapse.py
+-rw-rw-rw-   0        0        0     6156 2023-03-17 20:39:50.000000 geeViz-2023.4.1/geeViz/examples/LANDTRENDRViz.py
+-rw-rw-rw-   0        0        0     9374 2023-03-22 17:42:33.000000 geeViz-2023.4.1/geeViz/examples/LANDTRENDRWrapper.py
+-rw-rw-rw-   0        0        0    15519 2023-03-17 22:54:36.000000 geeViz-2023.4.1/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb
+-rw-rw-rw-   0        0        0    12431 2023-03-22 17:20:58.000000 geeViz-2023.4.1/geeViz/examples/LCMAP_and_LCMS_Viewer.py
+-rw-rw-rw-   0        0        0    19316 2023-03-17 23:04:04.000000 geeViz-2023.4.1/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb
+-rw-rw-rw-   0        0        0      118 2023-04-10 20:50:35.000000 geeViz-2023.4.1/geeViz/examples/__init__.py
+-rw-rw-rw-   0        0        0     5672 2023-03-22 19:24:09.000000 geeViz-2023.4.1/geeViz/examples/geeViewExample.py
+-rw-rw-rw-   0        0        0    16777 2023-03-17 22:12:16.000000 geeViz-2023.4.1/geeViz/examples/geeViewExampleNotebook.ipynb
+-rw-rw-rw-   0        0        0     5653 2022-02-07 23:21:45.000000 geeViz-2023.4.1/geeViz/examples/getClimateWrapper.py
+-rw-rw-rw-   0        0        0    14015 2023-01-09 16:55:27.000000 geeViz-2023.4.1/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py
+-rw-rw-rw-   0        0        0    11238 2022-06-15 22:15:23.000000 geeViz-2023.4.1/geeViz/examples/getLandsatWrapper.py
+-rw-rw-rw-   0        0        0    18281 2023-03-17 22:20:04.000000 geeViz-2023.4.1/geeViz/examples/getLandsatWrapperNotebook.ipynb
+-rw-rw-rw-   0        0        0    12016 2022-08-23 16:04:44.000000 geeViz-2023.4.1/geeViz/examples/getSentinel2Wrapper.py
+-rw-rw-rw-   0        0        0     8991 2022-10-26 19:30:20.000000 geeViz-2023.4.1/geeViz/examples/harmonicRegressionWrapper.py
+-rw-rw-rw-   0        0        0     8050 2023-03-22 17:46:00.000000 geeViz-2023.4.1/geeViz/examples/lcmsViewerExample.py
+-rw-rw-rw-   0        0        0    18271 2023-03-22 17:21:17.000000 geeViz-2023.4.1/geeViz/examples/lcmsViewerExampleNotebook.ipynb
+-rw-rw-rw-   0        0        0    13051 2022-02-16 00:28:08.000000 geeViz-2023.4.1/geeViz/examples/phEEnoVizWrapper.py
+-rw-rw-rw-   0        0        0     1038 2022-02-01 00:39:23.000000 geeViz-2023.4.1/geeViz/examples/taskTrackerExample.py
+-rw-rw-rw-   0        0        0     6171 2022-02-01 00:38:52.000000 geeViz-2023.4.1/geeViz/examples/timeLapseExample.py
+-rw-rw-rw-   0        0        0     1741 2021-04-01 17:15:14.000000 geeViz-2023.4.1/geeViz/gcpLib.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:03:27.539006 geeViz-2023.4.1/geeViz/geeView/
+drwxrwxrwx   0        0        0        0 2023-04-10 21:03:27.585886 geeViz-2023.4.1/geeViz/geeView/css/
+-rw-rw-rw-   0        0        0    18958 2023-03-09 02:29:15.000000 geeViz-2023.4.1/geeViz/geeView/css/style.min.css
+drwxrwxrwx   0        0        0        0 2023-04-10 21:03:28.789104 geeViz-2023.4.1/geeViz/geeView/images/
+-rw-rw-rw-   0        0        0     7295 2021-04-01 17:15:14.000000 geeViz-2023.4.1/geeViz/geeView/images/EE-logo-150.png
+-rw-rw-rw-   0        0        0    10301 2021-04-01 17:15:14.000000 geeViz-2023.4.1/geeViz/geeView/images/GEE.png
+-rw-rw-rw-   0        0        0     5692 2022-08-19 21:41:40.000000 geeViz-2023.4.1/geeViz/geeView/images/GEE_logo_transparent.png
+-rw-rw-rw-   0        0        0     4551 2021-04-01 17:15:14.000000 geeViz-2023.4.1/geeViz/geeView/images/RCR-logo.jpg
+-rw-rw-rw-   0        0        0    35328 2022-12-07 01:04:30.000000 geeViz-2023.4.1/geeViz/geeView/images/Thumbs.db
+-rw-rw-rw-   0        0        0     8352 2021-04-01 17:15:14.000000 geeViz-2023.4.1/geeViz/geeView/images/cumulative_icon.png
+-rw-rw-rw-   0        0        0     1502 2021-04-01 17:15:15.000000 geeViz-2023.4.1/geeViz/geeView/images/layer_icon.png
+-rw-rw-rw-   0        0        0   230271 2022-06-28 20:18:38.000000 geeViz-2023.4.1/geeViz/geeView/images/logos_usda-fs.svg
+-rw-rw-rw-   0        0        0   229463 2022-06-30 19:30:12.000000 geeViz-2023.4.1/geeViz/geeView/images/logos_usda-fs_bn-dk-01.svg
+-rw-rw-rw-   0        0        0      635 2022-06-29 22:17:42.000000 geeViz-2023.4.1/geeViz/geeView/images/menu-hamburger_ffffff.svg
+-rw-rw-rw-   0        0        0     1489 2021-04-01 17:15:15.000000 geeViz-2023.4.1/geeViz/geeView/images/usdalogo.png
+-rw-rw-rw-   0        0        0     8174 2021-04-01 17:15:15.000000 geeViz-2023.4.1/geeViz/geeView/images/usfslogo.png
+-rw-rw-rw-   0        0        0     3309 2023-03-08 18:54:11.000000 geeViz-2023.4.1/geeViz/geeView/index.html
+drwxrwxrwx   0        0        0        0 2023-04-10 21:03:29.195389 geeViz-2023.4.1/geeViz/geeView/js/
+-rw-rw-rw-   0        0        0    45351 2020-01-16 17:35:18.000000 geeViz-2023.4.1/geeViz/geeView/js/gena-gee-palettes.js
+-rw-rw-rw-   0        0        0   338389 2023-04-10 20:57:43.000000 geeViz-2023.4.1/geeViz/geeView/js/lcms-viewer.min.js
+-rw-rw-rw-   0        0        0     1021 2023-03-08 18:47:59.000000 geeViz-2023.4.1/geeViz/geeView/js/load.min.js
+-rw-rw-rw-   0        0        0    93058 2023-04-10 20:57:59.000000 geeViz-2023.4.1/geeViz/geeView/js/runGeeViz.js
+-rw-rw-rw-   0        0        0    11675 2023-04-10 20:46:12.000000 geeViz-2023.4.1/geeViz/geeView.py
+-rw-rw-rw-   0        0        0   174861 2023-04-03 16:39:39.000000 geeViz-2023.4.1/geeViz/getImagesLib.py
+-rw-rw-rw-   0        0        0     7467 2021-04-01 17:15:14.000000 geeViz-2023.4.1/geeViz/migrateGEEAssets.py
+-rw-rw-rw-   0        0        0    20743 2022-06-01 18:25:26.000000 geeViz-2023.4.1/geeViz/phEEnoViz.py
+-rw-rw-rw-   0        0        0     9885 2022-11-30 20:14:56.000000 geeViz-2023.4.1/geeViz/taskManagerLib.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:03:25.023140 geeViz-2023.4.1/geeViz.egg-info/
+-rw-rw-rw-   0        0        0     3900 2023-04-10 21:03:23.000000 geeViz-2023.4.1/geeViz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1945 2023-04-10 21:03:23.000000 geeViz-2023.4.1/geeViz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 21:03:23.000000 geeViz-2023.4.1/geeViz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-04-10 21:03:23.000000 geeViz-2023.4.1/geeViz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-10 21:03:23.000000 geeViz-2023.4.1/geeViz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 21:03:29.320396 geeViz-2023.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     2200 2022-07-06 19:24:37.000000 geeViz-2023.4.1/setup.py
```

### Comparing `geeViz-2023.3.1/LICENSE` & `geeViz-2023.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/PKG-INFO` & `geeViz-2023.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geeViz
-Version: 2023.3.1
+Version: 2023.4.1
 Summary: A package to help with GEE data processing, analysis, and visualization
 Home-page: https://github.com/gee-community/geeViz
 Author: Ian Housman
 Author-email: ian.housman@gmail.com
 License: Apache
 Keywords: earthengine google remote sensing landsat sentinel modis forestry forest
 Classifier: Programming Language :: Python :: 2
```

### Comparing `geeViz-2023.3.1/README.md` & `geeViz-2023.4.1/README.md`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/changeDetectionLib.py` & `geeViz-2023.4.1/geeViz/changeDetectionLib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1744,20 +1744,18 @@
   if annualizeWithCompositeDates and compositeCollection != None:
     timeImgs = getTimeImageCollectionFromComposites(startJulian, endJulian, compositeCollection)
   else:
     timeImgs = getTimeImageCollection(startYear, endYear, startJulian ,endJulian, 1, yearStartMonth, yearStartDay)
   Map.addLayer(timeImgs,{},'time')
   # If selected, add a constant amount of time to last end segment to make sure the last year is annualized correctly.
   # tEndExtrapolationPeriod should be a fraction of a year.
-  finalTEnd = ccdcImg.select('tEnd')
-  finalTEnd = finalTEnd.arraySlice(0,-1,None).rename('tEnd').arrayGet(0).add(tEndExtrapolationPeriod).toArray(0)
+  finalTEnd = ccdcImg.select('tEnd').arraySlice(0,-1,None).rename('tEnd').arrayGet(0).add(tEndExtrapolationPeriod).toArray(0)
   tEnds = ccdcImg.select('tEnd')
   tEnds = tEnds.arraySlice(0,0,-1).arrayCat(finalTEnd,0).rename('tEnd')
-  keepBands = ccdcImg.bandNames().remove('tEnd')
-  ccdcImg = ccdcImg.select(keepBands).addBands(tEnds)
+  ccdcImg = ccdcImg.addBands(tEnds,None,True)
 
   # Loop through time image collection and grab the correct CCDC coefficients
   annualSegCoeffs = timeImgs.map(lambda img: getCCDCSegCoeffs(img,ccdcImg,True))
   return annualSegCoeffs
 
 
 # Using annualized time series, get fitted values and slopes from fitted values.
@@ -1833,50 +1831,57 @@
   monthDayFraction = ee.Number.parse(ee.Date.fromYMD(startYear, yearStartMonth, yearStartDay).format('DDD')).divide(365)
   yearImages = ee.ImageCollection(ee.List.sequence(ee.Number(startYear).add(monthDayFraction),ee.Number(endYear).add(monthDayFraction),step).map(getYrImage))
   return yearImages.filter(ee.Filter.calendarRange(startYear,endYear,'year'))\
                       .filter(ee.Filter.calendarRange(startJulian,endJulian))
 
 # This creates an image collection in the same format as getTimeImageCollection(), but gets the pixel-wise dates from a composite collection
 # Composite collection should be an imported and prepped image collection with 'julianDay' and 'year' bands
-def getTimeImageCollectionFromComposites(startJulian, endJulian, compositeCollection):
-  # Account for date wrapping. If julian day is less than startJulian, add one year.
-  # For PRUSVI CCDC, Year 2020 is day 152 2020 to day 151 2021
-  # For CONUS CCDC, Year 2020 is day 1 2020 to day 365 2020, so it will never be less.
-  def getWrappedFraction(jDay):
-    fraction = jDay.divide(365)
-    nextYearMask = jDay.lte(ee.Image.constant(startJulian))
-    thisYearMask = nextYearMask.Not()
-    nextYearFraction = fraction.updateMask(nextYearMask).add(1)
-    thisYearFraction = fraction.updateMask(thisYearMask)
-    fraction = nextYearFraction.addBands(thisYearFraction).reduce(ee.Reducer.max())
-    return fraction
-  medianFraction = compositeCollection.select('julianDay')\
-    .map(lambda jDay: getWrappedFraction(jDay))\
-    .reduce(ee.Reducer.median())
-
-  def getYearTimeImage(dateImg):
-    # Get Unmasked values
-    newDateImg = ee.Image(dateImg.select('year').add(dateImg.select('julianDay').divide(365))).copyProperties(dateImg, ['system:time_start'])    
+#def getTimeImageCollectionFromComposites(startJulian, endJulian, compositeCollection):
+  ## Account for date wrapping. If julian day is less than startJulian, add one year.
+  ## For PRUSVI CCDC, Year 2020 is day 152 2020 to day 151 2021
+  ## For CONUS CCDC, Year 2020 is day 1 2020 to day 365 2020, so it will never be less.
+  #def getWrappedFraction(jDay):
+    #fraction = jDay.divide(365)
+    #nextYearMask = jDay.lte(ee.Image.constant(startJulian))
+    #thisYearMask = nextYearMask.Not()
+    #nextYearFraction = fraction.updateMask(nextYearMask).add(1)
+    #thisYearFraction = fraction.updateMask(thisYearMask)
+    #fraction = nextYearFraction.addBands(thisYearFraction).reduce(ee.Reducer.max())
+    #return fraction
+  #medianFraction = compositeCollection.select('julianDay')\
+    #.map(lambda jDay: getWrappedFraction(jDay))\
+    #.reduce(ee.Reducer.median())
+
+  #def getYearTimeImage(dateImg):
+    ## Get Unmasked values
+    #newDateImg = ee.Image(dateImg.select('year').add(dateImg.select('julianDay').divide(365))).copyProperties(dateImg, ['system:time_start'])    
     
-    # Create values for masked pixels  
-    imgYear = dateImg.date().get('year');
-    medianValues = ee.Image.constant(imgYear).float().add(ee.Image(medianFraction)).rename('median_values');
+    ## Create values for masked pixels  
+    #imgYear = dateImg.date().get('year');
+    #medianValues = ee.Image.constant(imgYear).float().add(ee.Image(medianFraction)).rename('median_values');
     
-    # Fill masked Values with median fraction
-    compositeMask = ee.Image(newDateImg).mask()
-    out = ee.Image(newDateImg)\
-      .addBands(medianValues.updateMask(compositeMask.Not()))\
-      .reduce(ee.Reducer.max())\
-      .rename('year')\
-      .copyProperties(dateImg, ['system:time_start']);
+    ## Fill masked Values with median fraction
+    #compositeMask = ee.Image(newDateImg).mask()
+    #out = ee.Image(newDateImg)\
+      #.addBands(medianValues.updateMask(compositeMask.Not()))\
+      #.reduce(ee.Reducer.max())\
+      #.rename('year')\
+      #.copyProperties(dateImg, ['system:time_start']);
+
+    #return out
+  #yearImages = compositeCollection.map(lambda dateImg: getYearTimeImage(dateImg))
+
+  #return yearImages
+
+def getTimeImageCollectionFromComposites(startJulian, endJulian, compositeCollection): 
+  dates = compositeCollection.map(lambda img:img.select(['year']).add(img.select(['julianDay']).divide(365)).float().copyProperties(img,['system:time_start']))
+  nYears = dates.size().getInfo()
+  interpolated = linearInterp(dates, 365*nYears, -32768)
+  return interpolated
 
-    return out
-  yearImages = compositeCollection.map(lambda dateImg: getYearTimeImage(dateImg))
-
-  return yearImages
 ###################################################################################
 #Function for getting change years and magnitudes for a specified band from CCDC outputs
 #Only change from the breaks is extracted
 #As of now, if a segment has a high slope value, this method will not extract that 
 def ccdcChangeDetection(ccdcImg,bandName):
   magKeys = ['.*_magnitude']
   tBreakKeys = ['tBreak']
```

### Comparing `geeViz-2023.3.1/geeViz/examples/CCDCViz.py` & `geeViz-2023.4.1/geeViz/examples/CCDCViz.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/examples/CCDCVizNotebook.ipynb` & `geeViz-2023.4.1/geeViz/examples/CCDCVizNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/examples/CCDCWrapper.py` & `geeViz-2023.4.1/geeViz/examples/CCDCWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/examples/GFSTimeLapse.py` & `geeViz-2023.4.1/geeViz/examples/GFSTimeLapse.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/examples/LANDTRENDRViz.py` & `geeViz-2023.4.1/geeViz/examples/LANDTRENDRViz.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/examples/LANDTRENDRWrapper.py` & `geeViz-2023.4.1/geeViz/examples/LANDTRENDRWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb` & `geeViz-2023.4.1/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/examples/LCMAP_and_LCMS_Viewer.py` & `geeViz-2023.4.1/geeViz/examples/LCMAP_and_LCMS_Viewer.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb` & `geeViz-2023.4.1/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/examples/geeViewExample.py` & `geeViz-2023.4.1/geeViz/examples/geeViewExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/examples/geeViewExampleNotebook.ipynb` & `geeViz-2023.4.1/geeViz/examples/geeViewExampleNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/examples/getClimateWrapper.py` & `geeViz-2023.4.1/geeViz/examples/getClimateWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py` & `geeViz-2023.4.1/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/examples/getLandsatWrapper.py` & `geeViz-2023.4.1/geeViz/examples/getLandsatWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/examples/getLandsatWrapperNotebook.ipynb` & `geeViz-2023.4.1/geeViz/examples/getLandsatWrapperNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/examples/getSentinel2Wrapper.py` & `geeViz-2023.4.1/geeViz/examples/getSentinel2Wrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/examples/harmonicRegressionWrapper.py` & `geeViz-2023.4.1/geeViz/examples/harmonicRegressionWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/examples/lcmsViewerExample.py` & `geeViz-2023.4.1/geeViz/examples/lcmsViewerExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/examples/lcmsViewerExampleNotebook.ipynb` & `geeViz-2023.4.1/geeViz/examples/lcmsViewerExampleNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/examples/phEEnoVizWrapper.py` & `geeViz-2023.4.1/geeViz/examples/phEEnoVizWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/examples/taskTrackerExample.py` & `geeViz-2023.4.1/geeViz/examples/taskTrackerExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/examples/timeLapseExample.py` & `geeViz-2023.4.1/geeViz/examples/timeLapseExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/gcpLib.py` & `geeViz-2023.4.1/geeViz/gcpLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/geeView/css/style.min.css` & `geeViz-2023.4.1/geeViz/geeView/css/style.min.css`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/geeView/images/EE-logo-150.png` & `geeViz-2023.4.1/geeViz/geeView/images/EE-logo-150.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/geeView/images/GEE.png` & `geeViz-2023.4.1/geeViz/geeView/images/GEE.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/geeView/images/GEE_logo_transparent.png` & `geeViz-2023.4.1/geeViz/geeView/images/GEE_logo_transparent.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/geeView/images/RCR-logo.jpg` & `geeViz-2023.4.1/geeViz/geeView/images/RCR-logo.jpg`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/geeView/images/Thumbs.db` & `geeViz-2023.4.1/geeViz/geeView/images/Thumbs.db`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/geeView/images/cumulative_icon.png` & `geeViz-2023.4.1/geeViz/geeView/images/cumulative_icon.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/geeView/images/layer_icon.png` & `geeViz-2023.4.1/geeViz/geeView/images/layer_icon.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/geeView/images/logos_usda-fs.svg` & `geeViz-2023.4.1/geeViz/geeView/images/logos_usda-fs.svg`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/geeView/images/logos_usda-fs_bn-dk-01.svg` & `geeViz-2023.4.1/geeViz/geeView/images/logos_usda-fs_bn-dk-01.svg`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/geeView/images/menu-hamburger_ffffff.svg` & `geeViz-2023.4.1/geeViz/geeView/images/menu-hamburger_ffffff.svg`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/geeView/images/usdalogo.png` & `geeViz-2023.4.1/geeViz/geeView/images/usdalogo.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/geeView/images/usfslogo.png` & `geeViz-2023.4.1/geeViz/geeView/images/usfslogo.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/geeView/index.html` & `geeViz-2023.4.1/geeViz/geeView/index.html`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/geeView/js/gena-gee-palettes.js` & `geeViz-2023.4.1/geeViz/geeView/js/gena-gee-palettes.js`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/geeView/js/lcms-viewer.min.js` & `geeViz-2023.4.1/geeViz/geeView/js/lcms-viewer.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -675,49 +675,50 @@
     lcmsSpinner: "<div id='lcms-spinner' style='position:absolute;right:40%; bottom:40%;width:10rem;height:8rem;z-index:10000000;display:none;'><img  alt= \"LCMS logo spinner\" title=\"Background processing is occurring\" class=\"fa fa-spin\" src=\"./images/lcms-icon.png\"  style='width:100%;height:100%'><span id = 'lcms-spinner-message'></span></div>",
     authErrorMessage: `<p>---  Error --- Map Loading Error ---</p>\n                                                              <p>Map data did not load correctly and cannot be used at this time. We apologize for this inconvenience and are working to resolve this issue.</p>\n                                                              ${specificAuthErrorMessage} \n                                                              ${authErrorMessageContact}\n    `,
     exportContainer: "<div class = 'py-2' id = 'export-list-container'>\n                        <h5>Choose which images to export:</h5>\n                        <div class = 'py-2' id=\"export-list\"></div>\n                        <hr>\n                        <div class = 'pl-3'>\n                            <form class=\"form-inline\" title = 'Provide projection. Web mercator: \"EPSG:4326\", USGS Albers: \"EPSG:5070\", WGS 84 UTM Northern Hemisphere: \"EPSG:326\" + zone number (e.g. zone 17 would be EPSG:32617), NAD 83 UTM Northern Hemisphere: \"EPSG:269\" + zone number (e.g. zone 17 would be EPSG:26917) '>\n                              <label for=\"export-crs\">Projection: </label>\n                              <div class=\"form-group pl-1\">\n                                <input type=\"text\" id=\"export-crs\" oninput = 'cacheCRS()' name=\"rg-from\" value=\"EPSG:4326\" class=\"form-control\">\n                              </div>\n                            </form>\n                            <div class = 'py-2' id = 'export-area-drawing-div'>\n                                <button class = 'btn' onclick = 'selectExportArea()' title = 'Draw polygon by clicking on map. Double-click to complete polygon, press ctrl+z to undo most recent point, press Delete or Backspace to start over.'><i class=\"pr-1 fa fa-pencil\" aria-hidden=\"true\"></i> Draw area to download</button>\n                                <a href=\"#\" onclick = 'undoExportArea()' title = 'Click to undo last drawn point (ctrl z)'><i class=\"btn fa fa-undo\"></i></a>\n                                <a href=\"#\" onclick = 'deleteExportArea()' title = 'Click to clear current drawing'><i class=\"btn fa fa-trash\"></i></a>\n                            </div>\n                            <hr>  \n                            <div class = 'pt-1 pb-3' >\n                                <div id = 'export-button-div'>\n                                    <button class = 'btn' onclick = 'exportImages()' title = 'Click to export selected images across selected area'><i class=\"pr-1 fa fa-cloud-download\" aria-hidden=\"true\"></i>Export Images</button>\n                                    <button class = 'btn' onclick = 'cancelAllTasks()' title = 'Click to cancel all active exports'></i>Cancel All Exports</button>\n                                </div>\n                                <hr>\n                                <span style = 'display:none;' class=\"fa-stack fa-2x py-0\" id='export-spinner' title=\"\">\n\t\t\t\t\t\t    \t\t<img alt= \"Google Earth Engine logo spinner\" class=\"fa fa-spin fa-stack-2x\" src=\"images/GEE_logo_transparent.png\" alt=\"\" style='width:2em;height:2em;'>\n\t\t\t\t\t\t   \t\t\t<strong id = 'export-count'  class=\"fa-stack-1x\" style = 'padding-left: 0.2em;padding-top: 0.1em;cursor:pointer;'></strong>\n\t\t\t\t\t\t\t\t</span>\n                                <div id = 'export-count-div'></div>\n                            </div>  \n                        </div>\n                        \n                    </div>",
     topBanner: ` <div id = 'title-banner' class = 'white  title-banner '>\n                    <img id='title-banner-icon-left' style = 'height:1.7rem;margin-top:0.25rem;'  alt="USDA Forest Service icon" src="images/logos_usda-fs.svg">\n                    <div class="vl"></div>\n                    <img id='title-banner-icon-right' style = 'width:1.6rem;height:1.7rem;margin-left:0.0rem;margin-right:0.1rem;margin-top:0.25rem;' >\n                    <div  class='my-0'>\n                    ${topBannerParams.leftWords} <span class = 'gray' style="font-weight:1000;font-family: 'Roboto Black', sans-serif;">${topBannerParams.centerWords}</span> ${topBannerParams.rightWords}</div>\n                </div>`,
     studyAreaDropdown: "<li   id = 'study-area-dropdown' class=\"nav-item dropdown navbar-dark navbar-nav nav-link p-0 col-12  \"  data-toggle=\"dropdown\">\n\t\t                <h5 href = '#' onclick = \"$('#sidebar-left').show('fade');$('#study-area-list').toggle();\" class = 'teal-study-area-label p-0 caret nav-link dropdown-toggle ' id='study-area-label'></h5> \n\t\t                <div class=\"dropdown-menu\" id=\"study-area-list\">  \n\t\t                </div>\n\t\t            </li>",
     placesSearchDiv: '<section id = \'search-share-div\' class="input-group  text-center search-bar" \'>\n\t\t\t            <div role=\'list\' class="input-group-prepend">\n                            <button onclick = \'getLocation()\' title = \'Click to center map at your location\' class=" btn input-group-text bg-white search-box pr-1 pl-2" id="get-location-button"><i class="fa fa-map-marker text-black "></i></button>\n\t    \t\t\t\t\t<button onclick = \'TweetThis()\' title = \'Click to share your current view\' class=" btn input-group-text bg-white search-box pr-1 pl-2" id="share-button"><i class="fa fa-share-alt teal "></i></button>\n                            <buttom class="input-group-text bg-white search-box" id="search-icon"><i class="fa fa-search text-black "></i></buttom>\n\t  \t\t\t\t\t</div>\n\t\t\t            <input id = \'pac-input\' class="form-control bg-white search-box" title = \'Search for places on the map\' type="text" placeholder="Search Places">\n                        <div class="input-group-prepend">\n                            <button onclick = \'backView()\' title = \'Click to go back a view\' class=" btn input-group-text bg-white search-box pr-1 pl-2" id="back-view-button"><i class="fa fa-chevron-left teal "></i></button>\n                            <button onclick = \'forwardView()\' title = \'Click to go forward a view\' style = \'border-radius: 0px 3px 3px 0px\' class=" btn input-group-text bg-white search-box pr-1 pl-2" id="forward-view-button"><i class="fa fa-chevron-right teal "></i></button>\n                        </div>\n                    </section>\n                    <p class = \'mt-0 mb-1 text-center white\' style = \'display:none;font-size:1.25rem;font-weight:bold\' id = \'time-lapse-year-label\'></p>',
     introModal: {
-        LCMS: getIntroModal("./images/lcms-icon.png", "Welcome to the Landscape Change Monitoring System (LCMS) Data Explorer!", "<p class='my-2'>\n                                    This Data Explorer provides the ability to view, analyze, summarize, and download LCMS data. \n                                    </p>\n                                    <p class='my-2'>\n                            LCMS is a remote sensing-based system for mapping and monitoring landscape change across the United States produced by the USDA Forest Service. LCMS provides a \"best available\" map of landscape change that leverages advances in time series-based change detection techniques, Landsat and Sentinel 2 data availability, cloud-based computing power, and big data analysis methods.\n\n                            </p>\n                            ", '<div style=\'display:inline-block;margin-top:0.5rem;\'>\n                            <div style =\'float:left;\' title=\'LCMS is produced by the USDA Forest Service\'>\n                                <img class = \'logo\' alt="USDA Forest Service icon" src="images/logos_usda-fs_bn-dk-01.svg">\n                                \n                            </div>\n                            <div style =\'float:left;\'>\n                                <ul class="intro-list">\n                                  <li title = "The Geospatial Technology and Applications Center (GTAC) provides leadership in geospatial science implementation in the USDA Forest Service by delivering vital services, data products, tools, training, and innovation to solve today\'s land and resource management challenges. All operational LCMS production and support takes place at GTAC."><a class="intro-modal-links" href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">GTAC</a> Geospatial Technology and Applications Center\n                                  </li>\n                                  <li title = \'RedCastle Resources Inc. is the on-site contractor that has provided the technical expertise for LCMS\' operational production, documentation, and delivery at GTAC.\'><a class="intro-modal-links" href="https://www.redcastleresources.com/" target="_blank">RCR</a> RedCastle Resources Inc.\n                                  </li>\n                                  <li title = \'The Rocky Mountain Research Station provides the scientific foundation LCMS is built upon. They have been instrumental in developing and publishing the original LCMS methodology and continue to provide ongoing research and development to further improve LCMS methods.\'><a class="intro-modal-links" href="https://www.fs.usda.gov/rmrs/tools/landscape-change-monitoring-system-lcms" target="_blank">RMRS</a> Rocky Mountain Research Station\n                                  </li>\n                                  <li title = \'LCMS utilizes Google Earth Engine for most of its data acqusition, processing, and visualization through an enterprise agreement between the USDA Forest Service and Google. In its current form, LCMS would not be possible without Google Earth Engine.\'><a class="intro-modal-links" href="https://earthengine.google.com/" target="_blank">GEE</a> Google Earth Engine\n                                  </li>\n                                </ul>\n                                \n                            </div>\n                        \n                        </div>', '<p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n                        <div class =\'my-3\'>\n                           <a  class = \'intro-modal-links\' onclick = \'downloadTutorial()\' title="Click to launch tutorial that explains how to utilize the Data Explorer">TUTORIAL</a>\n                            <a class="intro-modal-links" onclick="downloadMethods(\'v2021-7\')" title="Open in-depth LCMS v2021.7 methods documentation">LCMS METHODS</a>\n                            <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >LCMS HELPDESK/FEEDBACK</a> \n                        </div>\n                        \n                        <div class =\'my-3\' title=\'There are additional data visualization tools available in these other sites\'>Other LCMS EXPLORERS:\n                            <a class = \'intro-modal-links\' title = "Visualize and explore summaries of LCMS data over different areas" href = "dashboard.html" target="_blank">LCMS Dashboard</a>\n                            <a class = \'intro-modal-links\' title = "Visualize and explore time series datasets used to create the LCMS map outputs" href = "lcms-base-learner.html" target="_blank">LCMS Base Learner Explorer</a>\n                            <a class = \'intro-modal-links\' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n                            \n                        </div>'),
-        "lcms-base-learner": getIntroModal("./images/lcms-icon.png", "Welcome to the Landscape Change Monitoring System (LCMS) Base-Learner Explorer!", "<p>LCMS is a landscape change detection program developed by the USDA Forest Service. This application is designed to provide a visualization of the change detection algorithm outputs that are used to produce LCMS products.</p>", "<p>In addition to the map layers, LandTrendr and CCDC outputs can be compared through charting under the <kbd>Tools</kbd> -> <kbd>Pixel Tools</kbd> and <kbd>Area Tools</kbd>\n                                    </p>", '<p>Please review this <a class = \'support-text\' onclick = \'downloadMethods("v2021-7")\' title = \'Open in-depth LCMS v2021.7 methods documentation\'>methods document</a> for more information about how these datasets are used to create LCMS products.   \n                            </p>\n                            <p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n                            <div class =\'my-3\'>\n                            <a class="intro-modal-links" onclick="downloadMethods(\'v2021-7\')" title="Open in-depth LCMS v2021.7 methods documentation">LCMS METHODS</a>\n                            <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >LCMS HELPDESK/FEEDBACK</a> \n                        </div>\n                        \n                        <div class =\'my-3\' title=\'There are additional data visualization tools available in these other sites\'>Other LCMS EXPLORERS:\n                            <a class = \'intro-modal-links\' title = "Visualize and explore LCMS final outputs" href = "index.html" target="_blank">LCMS Data Explorer</a>\n                            <a class = \'intro-modal-links\' title = "Visualize and explore summaries of LCMS data over different areas" href = "dashboard.html" target="_blank">LCMS Dashboard</a>\n                            <a class = \'intro-modal-links\' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n                            \n                        </div>'),
-        "lcms-dashboard": getIntroModal("./images/lcms-icon.png", "Welcome to the Landscape Change Monitoring System (LCMS) Data Dashboard!", "<p>LCMS is a landscape change detection program developed by the USDA Forest Service. This application is designed to provide the ability to quickly visualize and generate reports of how our landscapes are changing.</p>", '<p>Pre-calculated summary areas are available for generating custom reports.</p>\n                                    <p>Disclaimer: All summary numbers are based on modeled LCMS outputs. Known as model-based inference, error margins are difficult to compute directly from the summary pixel counts. Currently, error margins are calculated from the LCMS refence sample for each year from each summary area plus a 210km buffer. This assumes the statistical properties of the model-based and reference sample-based estimates are similar. Since this assumption is difficult to uphold, this method is still under scientific review. Theses tables are useful for understanding broad patterns of change on our landscape. For details on valid statistical conclusions and understanding map error, please refer to the <a class="intro-modal-links" onclick="downloadMethods(\'v2021-7\')" title="Open in-depth LCMS v2021.7 methods documentation">LCMS METHODS</a> document or reach out to the <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >LCMS HELPDESK</a>.\n                                    </p>', '<p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n                            <div class =\'my-3\'>\n                            <a class="intro-modal-links" onclick="startTour()" title="Click to take a tour of the LCMS Dashboard\'s features">DASHBOARD TOUR</a>\n                            <a class="intro-modal-links" onclick="downloadMethods(\'v2021-7\')" title="Open in-depth LCMS v2021.7 methods documentation">LCMS METHODS</a>\n                            <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >LCMS HELPDESK/FEEDBACK</a> \n                        </div>\n                        \n                        <div class =\'my-3\' title=\'There are additional data visualization tools available in these other sites\'>Other LCMS EXPLORERS:\n                            <a class = \'intro-modal-links\' title = "Visualize and explore LCMS final outputs" href = "index.html" target="_blank">LCMS Data Explorer</a>\n                            <a class = \'intro-modal-links\' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n                            \n                        </div>', "Loading LCMS summary areas. This can take some time"),
-        IDS: getIntroModal("./images/lcms-icon.png", "Welcome to the Landscape Change Monitoring System (LCMS) Insect and Disease Detection Survey (IDS) Explorer!", "<p>LCMS is a landscape change detection program developed by the USDA Forest Service. This application is designed to provide a visualization of the LCMS outputs alongside outputs from the USFS Forest Health Protection's <a class='intro-modal-links' href='https://www.fs.fed.us/foresthealth/applied-sciences/mapping-reporting/detection-surveys.shtml' title = 'IDS homepage' target=\"_blank\">Insect and Disease Detection Survey (IDS)</a>outputs.</p>\n           \n           <p>LCMS Change and IDS polygon data can be viewed simultaneously for each coincident year. These data can also be compared through charting under the <kbd>Tools</kbd> -> <kbd>Pixel Tools</kbd> and <kbd>Area Tools</kbd>\n           </p>", '\n    <p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n    <div class =\'my-3\'>\n    <a class="intro-modal-links" onclick="downloadMethods(\'v2021-7\')" title="Open in-depth LCMS v2021.7 methods documentation">LCMS METHODS</a>\n    <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >LCMS HELPDESK/FEEDBACK</a> \n</div>\n\n<div class =\'my-3\' title=\'There are additional data visualization tools available in these other sites\'>Other LCMS EXPLORERS:\n    <a class = \'intro-modal-links\' title = "Visualize and explore LCMS final outputs" href = "index.html" target="_blank">LCMS Data Explorer</a>\n    <a class = \'intro-modal-links\' title = "Visualize and explore summaries of LCMS data over different areas" href = "dashboard.html" target="_blank">LCMS Dashboard</a>\n    <a class = \'intro-modal-links\' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n    \n</div>', ""),
+        LCMS: getIntroModal("./images/lcms-icon.png", "Welcome to the Landscape Change Monitoring System (LCMS) Data Explorer!", "<p class='my-2'>\n                                    This Data Explorer provides the ability to view, analyze, summarize, and download LCMS data. \n                                    </p>\n                                    <p class='my-2'>\n                            LCMS is a remote sensing-based system for mapping and monitoring landscape change across the United States produced by the USDA Forest Service. LCMS provides a \"best available\" map of landscape change that leverages advances in time series-based change detection techniques, Landsat and Sentinel 2 data availability, cloud-based computing power, and big data analysis methods.\n\n                            </p>\n                            ", '<div style=\'display:inline-block;margin-top:0.5rem;\'>\n                            <div style =\'float:left;\' title=\'LCMS is produced by the USDA Forest Service\'>\n                                <img class = \'logo\' alt="USDA Forest Service icon" src="images/logos_usda-fs_bn-dk-01.svg">\n                                \n                            </div>\n                            <div style =\'float:left;\'>\n                                <ul class="intro-list">\n                                  <li title = "The Geospatial Technology and Applications Center (GTAC) provides leadership in geospatial science implementation in the USDA Forest Service by delivering vital services, data products, tools, training, and innovation to solve today\'s land and resource management challenges. All operational LCMS production and support takes place at GTAC."><a class="intro-modal-links" href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">GTAC</a> Geospatial Technology and Applications Center\n                                  </li>\n                                  <li title = \'RedCastle Resources Inc. is the on-site contractor that has provided the technical expertise for LCMS\' operational production, documentation, and delivery at GTAC.\'><a class="intro-modal-links" href="https://www.redcastleresources.com/" target="_blank">RCR</a> RedCastle Resources Inc.\n                                  </li>\n                                  <li title = \'The Rocky Mountain Research Station provides the scientific foundation LCMS is built upon. They have been instrumental in developing and publishing the original LCMS methodology and continue to provide ongoing research and development to further improve LCMS methods.\'><a class="intro-modal-links" href="https://www.fs.usda.gov/rmrs/tools/landscape-change-monitoring-system-lcms" target="_blank">RMRS</a> Rocky Mountain Research Station\n                                  </li>\n                                  <li title = \'LCMS utilizes Google Earth Engine for most of its data acqusition, processing, and visualization through an enterprise agreement between the USDA Forest Service and Google. In its current form, LCMS would not be possible without Google Earth Engine.\'><a class="intro-modal-links" href="https://earthengine.google.com/" target="_blank">GEE</a> Google Earth Engine\n                                  </li>\n                                </ul>\n                                \n                            </div>\n                        \n                        </div>', '<p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n                        <div class =\'my-3\'>\n                           <a  class = \'intro-modal-links\' onclick = \'downloadTutorial()\' title="Click to launch tutorial that explains how to utilize the Data Explorer">TUTORIAL</a>\n                            <a class="intro-modal-links" onclick="downloadMethods(\'v2021-7\')" title="Open in-depth LCMS v2021.7 methods documentation">LCMS METHODS</a>\n                            <a  class = \'intro-modal-links\'  onclick = \'openLCMSSurvey("splashScreen")\' title="Click to help us learn how you use LCMS and how we can make it better">LCMS USER SURVEY</a>\n                            <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >LCMS HELPDESK/FEEDBACK</a> \n                        </div>\n                        \n                        <div class =\'my-3\' title=\'There are additional data visualization tools available in these other sites\'>Other LCMS EXPLORERS:\n                            <a class = \'intro-modal-links\' title = "Visualize and explore summaries of LCMS data over different areas" href = "dashboard.html" target="_blank">LCMS Dashboard</a>\n                            <a class = \'intro-modal-links\' title = "Visualize and explore time series datasets used to create the LCMS map outputs" href = "lcms-base-learner.html" target="_blank">LCMS Base Learner Explorer</a>\n                            <a class = \'intro-modal-links\' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n                            \n                        </div>'),
+        "lcms-base-learner": getIntroModal("./images/lcms-icon.png", "Welcome to the Landscape Change Monitoring System (LCMS) Base-Learner Explorer!", "<p>LCMS is a landscape change detection program developed by the USDA Forest Service. This application is designed to provide a visualization of the change detection algorithm outputs that are used to produce LCMS products.</p>", "<p>In addition to the map layers, LandTrendr and CCDC outputs can be compared through charting under the <kbd>Tools</kbd> -> <kbd>Pixel Tools</kbd> and <kbd>Area Tools</kbd>\n                                    </p>", '<p>Please review this <a class = \'support-text\' onclick = \'downloadMethods("v2021-7")\' title = \'Open in-depth LCMS v2021.7 methods documentation\'>methods document</a> for more information about how these datasets are used to create LCMS products.   \n                            </p>\n                            <p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n                            <div class =\'my-3\'>\n                            <a class="intro-modal-links" onclick="downloadMethods(\'v2021-7\')" title="Open in-depth LCMS v2021.7 methods documentation">LCMS METHODS</a>\n                            <a  class = \'intro-modal-links\'  onclick = \'openLCMSSurvey("splashScreen")\' title="Click to help us learn how you use LCMS and how we can make it better">LCMS USER SURVEY</a>\n                            <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >LCMS HELPDESK/FEEDBACK</a> \n                        </div>\n                        \n                        <div class =\'my-3\' title=\'There are additional data visualization tools available in these other sites\'>Other LCMS EXPLORERS:\n                            <a class = \'intro-modal-links\' title = "Visualize and explore LCMS final outputs" href = "index.html" target="_blank">LCMS Data Explorer</a>\n                            <a class = \'intro-modal-links\' title = "Visualize and explore summaries of LCMS data over different areas" href = "dashboard.html" target="_blank">LCMS Dashboard</a>\n                            <a class = \'intro-modal-links\' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n                            \n                        </div>'),
+        "lcms-dashboard": getIntroModal("./images/lcms-icon.png", "Welcome to the Landscape Change Monitoring System (LCMS) Data Dashboard!", "<p>LCMS is a landscape change detection program developed by the USDA Forest Service. This application is designed to provide the ability to quickly visualize and generate reports of how our landscapes are changing.</p>", '<p>Pre-calculated summary areas are available for generating custom reports.</p>\n                                    <p>Disclaimer: All summary numbers are based on modeled LCMS outputs. Known as model-based inference, error margins are difficult to compute directly from the summary pixel counts. Currently, error margins are calculated from the LCMS refence sample for each year from each summary area plus a 210km buffer. This assumes the statistical properties of the model-based and reference sample-based estimates are similar. Since this assumption is difficult to uphold, this method is still under scientific review. Theses tables are useful for understanding broad patterns of change on our landscape. For details on valid statistical conclusions and understanding map error, please refer to the <a class="intro-modal-links" onclick="downloadMethods(\'v2021-7\')" title="Open in-depth LCMS v2021.7 methods documentation">LCMS METHODS</a> document or reach out to the <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >LCMS HELPDESK</a>.\n                                    </p>', '<p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n                            <div class =\'my-3\'>\n                            <a class="intro-modal-links" onclick="startTour()" title="Click to take a tour of the LCMS Dashboard\'s features">DASHBOARD TOUR</a>\n                            <a class="intro-modal-links" onclick="downloadMethods(\'v2021-7\')" title="Open in-depth LCMS v2021.7 methods documentation">LCMS METHODS</a>\n                            <a  class = \'intro-modal-links\'  onclick = \'openLCMSSurvey("splashScreen")\' title="Click to help us learn how you use LCMS and how we can make it better">LCMS USER SURVEY</a>\n                            <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >LCMS HELPDESK/FEEDBACK</a> \n                        </div>\n                        \n                        <div class =\'my-3\' title=\'There are additional data visualization tools available in these other sites\'>Other LCMS EXPLORERS:\n                            <a class = \'intro-modal-links\' title = "Visualize and explore LCMS final outputs" href = "index.html" target="_blank">LCMS Data Explorer</a>\n                            <a class = \'intro-modal-links\' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n                            \n                        </div>', "Loading LCMS summary areas. This can take some time"),
+        IDS: getIntroModal("./images/lcms-icon.png", "Welcome to the Landscape Change Monitoring System (LCMS) Insect and Disease Detection Survey (IDS) Explorer!", "<p>LCMS is a landscape change detection program developed by the USDA Forest Service. This application is designed to provide a visualization of the LCMS outputs alongside outputs from the USFS Forest Health Protection's <a class='intro-modal-links' href='https://www.fs.usda.gov/foresthealth/applied-sciences/mapping-reporting/detection-surveys.shtml' title = 'IDS homepage' target=\"_blank\">Insect and Disease Detection Survey (IDS)</a>outputs.</p>\n           \n           <p>LCMS Change and IDS polygon data can be viewed simultaneously for each coincident year. These data can also be compared through charting under the <kbd>Tools</kbd> -> <kbd>Pixel Tools</kbd> and <kbd>Area Tools</kbd>\n           </p>", '\n    <p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n    <div class =\'my-3\'>\n    <a class="intro-modal-links" onclick="downloadMethods(\'v2021-7\')" title="Open in-depth LCMS v2021.7 methods documentation">LCMS METHODS</a>\n    <a  class = \'intro-modal-links\'  onclick = \'openLCMSSurvey("splashScreen")\' title="Click to help us learn how you use LCMS and how we can make it better">LCMS USER SURVEY</a>\n    <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >LCMS HELPDESK/FEEDBACK</a> \n</div>\n\n<div class =\'my-3\' title=\'There are additional data visualization tools available in these other sites\'>Other LCMS EXPLORERS:\n    <a class = \'intro-modal-links\' title = "Visualize and explore LCMS final outputs" href = "index.html" target="_blank">LCMS Data Explorer</a>\n    <a class = \'intro-modal-links\' title = "Visualize and explore summaries of LCMS data over different areas" href = "dashboard.html" target="_blank">LCMS Dashboard</a>\n    <a class = \'intro-modal-links\' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n    \n</div>', ""),
         Ancillary: '<div class="modal fade "  id="introModal" tabindex="-1" role="dialog" >\n                <div class="modal-dialog modal-md " role="document">\n                    <div class="modal-content text-dark" style = \'background-color:rgba(230,230,230,0.95);\'>\n                        <button type="button" class="close p-2 ml-auto text-dark" data-dismiss="modal">&times;</button>\n                        <div class = \'modal-header\'>\n                            <h3 class="mb-0 ">Welcome to the TimeSync Ancillary Data Viewer!</h3>\n                        </div>\n                        <div class="modal-body" id = \'introModal-body\'>\n                            <p class="pb-2 ">This viewer is intended to provide an efficient way of looking at ancillary data to help with responses for the TimeSync tool.</p>\n                        </div>\n                        <div class = \'modal-footer\' id = \'introModal-footer\'>\n                        <div class = \' ml-0\' id = \'intro-modal-loading-div\'>\n                            <p>\n                              <img style="width:1.8em;" class="image-icon fa-spin mr-1" alt= "Google Earth Engine logo spinner" src="images/GEE_logo_transparent.png">\n                                Creating map services within Google Earth Engine. \n                             </p>\n                        </div>\n\t\t\t\t\t\t<div class="form-check  mr-0">\n                                <input role="option" type="checkbox" class="form-check-input" id="dontShowAgainCheckbox"   name = \'dontShowAgain\' value = \'true\'>\n                                <label class=" text-uppercase form-check-label " for="dontShowAgainCheckbox" >Don\'t show again</label>\n                            </div>\n                        </div>\n                    </div>\n                </div>\n            </div>',
         LT: getIntroModal("./images/lcms-icon.png", "Welcome to the LandTrendr Data Explorer!", '<li>\n           <p class="pb-2 ">This tool allows for quick exploration of significant changes visible in the Landsat time series using the <a class = \'intro-modal-links\' href="https://emapr.github.io/LT-GEE/" target="_blank">LandTrendr temporal segmentation algorithm</a>. While this tool can run across any area on earth, the quality of the output will be related to the availability of cloud-free Landsat observations.</p>\n       </li>\n       <li>\n           <p class="pb-2 ">LandTrendr will run across the entire extent of the map when it is loaded. If you would like to map a different area, move to the view extent you would like to map, and then press the <kbd>Submit</kbd> button at the bottom of the <kbd>PARAMETERS</kbd> collapse menu.</p>\n       </li>\n        <li>\n           <p class="pb-2 ">All Landsat image processing and LandTrendr algorithm application is being performed on-the-fly. This can take some time to run. If you try to run this tool across a very large extent (zoom level < 9), it may not run.</p>\n       </li>', '\n    <p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n    <div class =\'my-3\'>\n    <a class="intro-modal-links" href="https://emapr.github.io/LT-GEE/" target="_blank" title="Open additional LandTrendr resources">LandTrendr Guide</a>\n    <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >LCMS HELPDESK/FEEDBACK</a> \n</div>\n\n<div class =\'my-3\' title=\'There are additional data visualization tools available in these other sites\'>Other LCMS EXPLORERS:\n    <a class = \'intro-modal-links\' title = "Visualize and explore LCMS final outputs" href = "index.html" target="_blank">LCMS Data Explorer</a>\n    <a class = \'intro-modal-links\' title = "Visualize and explore time series datasets used to create the LCMS map outputs (Includes both LandTrendr and CCDC outputs)" href = "lcms-base-learner.html" target="_blank">LCMS Base Learner Explorer</a>\n    <a class = \'intro-modal-links\' title = "Visualize and explore summaries of LCMS data over different areas" href = "dashboard.html" target="_blank">LCMS Dashboard</a>\n    <a class = \'intro-modal-links\' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n    \n</div>', ""),
         MTBS: getIntroModal("./images/mtbs-logo.png", "Welcome to the MTBS Data Explorer!", "<p class='my-2'>This tool is intended to allow for interactive exploration of the Monitoring Trends in Burn Severity (MTBS) data record.\n            </p>\n            <p class='my-2'>\n            Monitoring Trends in Burn Severity (MTBS) is a multiagency program designed to consistently map the burn severity and perimeters of fires across all lands of the United States from 1984 and beyond. MTBS maps wildland and prescribed fires greater than 1,000 acres in the Western US and 500 acres in the Eastern US. \n    </p>\n    <p class='my-2'>\n    MTBS burn severity data are used to assess the impacts to landscape health and can be used to monitor trends in wildfire over time.\n    </p>\n    ", '<div style=\'display:inline-block;margin-top:0.5rem;\'>\n    <div style =\'float:left;display:block\' title=\'MTBS is jointly produced by the USDA Forest Service and USGS\'>\n        <img class = \'logo\' alt="USDA Forest Service icon" src="images/logos_usda-fs_bn-dk-01.svg">\n        <br>\n        <img class = \'logo\' style = \'margin-left:0.3rem;height:2.5rem;\' alt="USGS icon" src="images/USGS_logo_green.svg">\n    </div>\n    <div style =\'float:left;\'>\n        <ul class="intro-list">\n          <li title = "The Geospatial Technology and Applications Center (GTAC) provides leadership in geospatial science implementation in the USDA Forest Service by delivering vital services, data products, tools, training, and innovation to solve today\'s land and resource management challenges. This Explorer was developed at GTAC.""><a class="intro-modal-links" href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">GTAC</a> Geospatial Technology and Applications Center\n          </li>\n          <li title = "The Earth Resources Observation and Science (EROS) Center studies land change and produce land change data products used by researchers, resource managers, and policy makers across the nation and around the world. They also operate the Landsat satellite program with NASA, and maintain the largest civilian collection of images of the Earth\'s land surface in existence, including tens of millions of satellite images.""><a class="intro-modal-links" href="https://www.usgs.gov/centers/eros" target="_blank">EROS</a> Earth Resources Observation and Science Center\n          </li>\n          <li title = "This site utilizes Google Earth Engine for most of its data acqusition, processing, and visualization through an enterprise agreement between the USDA Forest Service and Google.""><a class="intro-modal-links" href="https://earthengine.google.com/" target="_blank">GEE</a> Google Earth Engine\n          </li>\n        </ul>\n        \n    </div>\n\n</div>', '<p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n<div class =\'my-3\'>\n   <a  class = \'intro-modal-links\' onclick = \'toggleWalkThroughCollapse()\' title="Run interactive walk-through of the features of the MTBS Data Explorer">Run Walk-Through</a>\n\n    <a class = "intro-modal-links" title = "Contact us" href="https://www.mtbs.gov/contact" target="_blank"  >CONTACT</a> \n</div>\n\n'),
         LAMDA: getIntroModal("./Icons_svg/logo_gtac_color-wt.svg", "Welcome to the Landscape Automated Monitoring and Detection Algorithm (LAMDA) Data Explorer!", "<li>\n           <p class=\"pb-2 \">LAMDA is a near real-time landscape-scale change detection program developed by the USDA Forest Service to serve as a 'hot spot' indicator for areas where finer resolution data may be used for further investigation and to serve as an indicator of severe changes over forested regions. This application is designed to provide a visualization of LAMDA outputs.</p>\n       </li>\n       ", '\n    <p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n    <div class =\'my-3\'>\n    <a class = "intro-modal-links" title = "Publication outlining the methods used to derive these products" href = "https://www.mdpi.com/2072-4292/10/8/1184" target="_blank" >LAMDA Methods Publication</a>\n    <a class="intro-modal-links" href="./lamda-downloads.html" target="_blank" title="LAMDA product download page">Download LAMDA Data</a>\n    <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >HELPDESK/FEEDBACK</a> \n</div>\n<div class =\'my-3\' title=\'There are additional change data visualization tools available in these other sites\'>Other EXPLORERS:\n    <a class = \'intro-modal-links\' title = "Visualize and explore LCMS final outputs" href = "index.html" target="_blank">LCMS Data Explorer</a>\n    <a class = \'intro-modal-links\' title = "Visualize and explore time series datasets used to create the LCMS map outputs (Includes both LandTrendr and CCDC outputs)" href = "lcms-base-learner.html" target="_blank">LCMS Base Learner Explorer</a>\n    <a class = \'intro-modal-links\' title = "Visualize and explore summaries of LCMS data over different areas" href = "dashboard.html" target="_blank">LCMS Dashboard</a>\n    <a class = \'intro-modal-links\' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n    \n</div>', ""),
         STORM: getIntroModal("./Icons_svg/logo_gtac_color-wt.svg", "Welcome to the Storm Damage Viewer!", "<p class='my-2'>\n                            This tool provides an interactive ability to upload storm tracks and produce modeled wind fields and tree damage. These outputs can then be downloaded for further analysis.\n\n                            </p>", '<div style=\'display:inline-block;margin-top:0.5rem;\'>\n    <div style =\'float:left;display:block\' title=\'This tool is produced by the USDA Forest Service\'>\n        <img class = \'logo\' alt="USDA Forest Service icon" src="images/logos_usda-fs_bn-dk-01.svg">\n    </div>\n    <div style =\'float:left;\'>\n        <ul class="intro-list">\n          <li title = "The Geospatial Technology and Applications Center (GTAC) provides leadership in geospatial science implementation in the USDA Forest Service by delivering vital services, data products, tools, training, and innovation to solve today\'s land and resource management challenges. This Explorer was developed at GTAC."><a class="intro-modal-links" href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">GTAC</a> Geospatial Technology and Applications Center\n          </li>\n          <li title = \'The Southern Research Station provided the original methods for this data explorer.\'><a class="intro-modal-links" href="https://www.srs.fs.usda.gov/" target="_blank">SRS</a> Southern Research Station\n                                  </li>\n            <li title = \'RedCastle Resources Inc. is the on-site contractor that has provided the technical expertise for adapting the original workflow from the SRS and developing this Viewer.\'><a class="intro-modal-links" href="https://www.redcastleresources.com/" target="_blank">RCR</a> RedCastle Resources Inc.\n            </li>\n          <li title = \'This site utilizes Google Earth Engine for most of its data acqusition, processing, and visualization through an enterprise agreement between the USDA Forest Service and Google.\'><a class="intro-modal-links" href="https://earthengine.google.com/" target="_blank">GEE</a> Google Earth Engine\n          </li>\n        </ul>\n        \n    </div>\n\n</div>', '<p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n\n<div class =\'my-3\'>\n    <a class = "intro-modal-links" title = "Report highlighting a project that used this tool" href = "https://apps.fs.usda.gov/gtac/publications/2022/tree-structure-damage-impact-predictive-trees-dip-modeling-phase-ii" target="_blank" >PROJECT REPORT</a>\n    <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >HELPDESK/FEEDBACK</a> \n</div>\n<div class =\'my-3\' title=\'There are additional change data visualization tools available in these other sites\'>Other EXPLORERS:\n    <a class = \'intro-modal-links\' title = "Visualize and explore LCMS final outputs" href = "index.html" target="_blank">LCMS Data Explorer</a>\n    <a class = \'intro-modal-links\' title = "Visualize and explore time series datasets used to create the LCMS map outputs (Includes both LandTrendr and CCDC outputs)" href = "lcms-base-learner.html" target="_blank">LCMS Base Learner Explorer</a>\n    <a class = \'intro-modal-links\' title = "Visualize and explore summaries of LCMS data over different areas" href = "dashboard.html" target="_blank">LCMS Dashboard</a>\n    <a class = \'intro-modal-links\' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n    \n</div>'),
-        "Bloom-Mapper": getIntroModal("./Icons_svg/logo_gtac_color-wt.svg", "Welcome to the Bloom MAPPER!", "<p class='my-2'>\n            This prototype tool provides an interactive map with the ability to view lakes with potential cyanobacteria or algae blooms. These outputs have been created as a collaborative effort between field experts throughout Wyoming and the Geospatial Technology and Applications Center. Current methods are being tested for preliminary review. These products are not conclusive and are intended for review purposes only. \n            </p>", `<div style='display:inline-block;margin-top:0.5rem;'>\n    <div style ='float:left;display:block' title='Bloom mapper is a joint effort between GTAC and WY USFS partners'>\n        <img class = 'logo' alt="USDA Forest Service icon" src="images/logos_usda-fs_bn-dk-01.svg">\n        \n       \n        \n    </div>\n    <div style ='float:left;'>\n        <ul class="intro-list">\n          <li title = "The Geospatial Technology and Applications Center (GTAC) provides leadership in geospatial science implementation in the USDA Forest Service by delivering vital services, data products, tools, training, and innovation to solve today's land and resource management challenges. This Explorer was developed at GTAC."><a class="intro-modal-links" href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">GTAC</a> Geospatial Technology and Applications Center\n          </li>\n          \n         \n            <li title = 'RedCastle Resources Inc. is the on-site contractor that has provided the technical expertise for adapting the original workflow from the SRS and developing this Viewer.'><a class="intro-modal-links" href="https://www.redcastleresources.com/" target="_blank">RCR</a> RedCastle Resources Inc.\n            </li>\n          <li title = 'This site utilizes Google Earth Engine for most of its data acqusition, processing, and visualization through an enterprise agreement between the USDA Forest Service and Google.'><a class="intro-modal-links" href="https://earthengine.google.com/" target="_blank">GEE</a> Google Earth Engine\n          </li>\n        </ul>\n        \n    </div>\n    <div class ='my-3'>\n                            <a class="intro-modal-links" onclick="startTour()" title="Click to take a tour of the ${mode}'s features">TOUR</a>\n                            <a class="intro-modal-links" onclick="downloadAnyMethods('./literature/Bloom_Mapper_v3_Methods_2023.pdf')" title="Open Bloom Mapper data creation methods documentation">METHODS</a>\n                            <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >HELPDESK/FEEDBACK</a> \n                        </div>\n\n</div>`, "<p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n\n")
+        "Bloom-Mapper": getIntroModal("./Icons_svg/logo_gtac_color-wt.svg", "Welcome to the Bloom MAPPER!", "<p class='my-2'>\n            This prototype tool provides an interactive map with the ability to view lakes with potential cyanobacteria or algae blooms. These outputs have been created as a collaborative effort between field experts throughout Wyoming and the Geospatial Technology and Applications Center. Current methods are being tested for preliminary review. These products are not conclusive and are intended for review purposes only. \n            </p>", `<div style='display:inline-block;margin-top:0.5rem;'>\n    <div style ='float:left;display:block' title='Bloom mapper is a joint effort between GTAC and WY USFS partners'>\n        <img class = 'logo' alt="USDA Forest Service icon" src="images/logos_usda-fs_bn-dk-01.svg">\n        \n       \n        \n    </div>\n    <div style ='float:left;'>\n        <ul class="intro-list">\n          <li title = "The Geospatial Technology and Applications Center (GTAC) provides leadership in geospatial science implementation in the USDA Forest Service by delivering vital services, data products, tools, training, and innovation to solve today's land and resource management challenges. This Explorer was developed at GTAC."><a class="intro-modal-links" href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">GTAC</a> Geospatial Technology and Applications Center\n          </li>\n          \n         \n            <li title = 'RedCastle Resources Inc. is the on-site contractor that has provided the technical expertise for adapting the original workflow from the SRS and developing this Viewer.'><a class="intro-modal-links" href="https://www.redcastleresources.com/" target="_blank">RCR</a> RedCastle Resources Inc.\n            </li>\n          <li title = 'This site utilizes Google Earth Engine for most of its data acqusition, processing, and visualization through an enterprise agreement between the USDA Forest Service and Google.'><a class="intro-modal-links" href="https://earthengine.google.com/" target="_blank">GEE</a> Google Earth Engine\n          </li>\n        </ul>\n        \n    </div>\n    <div class ='my-3'>\n                            <a class="intro-modal-links" onclick="startTour()" title="Click to take a tour of the ${mode}'s features">TOUR</a>\n                            <a class="intro-modal-links" onclick="downloadAnyMethods('./literature/Bloom_Mapper_v3_Methods_2023.pdf')" title="Open Bloom Mapper data creation methods documentation">METHODS</a>\n                            <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >HELPDESK/FEEDBACK</a> \n                        </div>\n\n</div>`, "<p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n\n"),
+        TreeMap: getIntroModal("./Icons_svg/logo_gtac_color-wt.svg", "Welcome to the TreeMap Explorer!", "<p class='my-2'>\n            This prototype tool provides an interactive map with the ability to view the 2016 TreeMap attributes. Source Data: Riley, Karin L.; Grenfell, Isaac C.; Finney, Mark A.; Shaw, John D. (2023). TreeMap 2016: A tree-level model of the forests of the conterminous United States circa 2016. Forest Service Research Data Archive. https://doi.org/10.2737/RDS-2021-0074. Accessed 2023-03-13. \n            </p>", `<div style='display:inline-block;margin-top:0.5rem;'>\n    <div style ='float:left;display:block' title='TreeMap Explorer is a joint effort between GTAC and USDA Forest Service Research'>\n        <img class = 'logo' alt="USDA Forest Service icon" src="images/logos_usda-fs_bn-dk-01.svg">\n        \n       \n        \n    </div>\n    <div style ='float:left;'>\n        <ul class="intro-list">\n          <li title = "The Geospatial Technology and Applications Center (GTAC) provides leadership in geospatial science implementation in the USDA Forest Service by delivering vital services, data products, tools, training, and innovation to solve today's land and resource management challenges. This Explorer was developed at GTAC."><a class="intro-modal-links" href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">GTAC</a> Geospatial Technology and Applications Center\n          </li>\n          \n         \n            <li title = 'RedCastle Resources Inc. is the on-site contractor that has provided the technical expertise for adapting the original workflow from the SRS and developing this Viewer.'><a class="intro-modal-links" href="https://www.redcastleresources.com/" target="_blank">RCR</a> RedCastle Resources Inc.\n            </li>\n          <li title = 'This site utilizes Google Earth Engine for most of its data acqusition, processing, and visualization through an enterprise agreement between the USDA Forest Service and Google.'><a class="intro-modal-links" href="https://earthengine.google.com/" target="_blank">GEE</a> Google Earth Engine\n          </li>\n          <li title = 'TreeMap 2016 Research Dataset source data.'><a class="intro-modal-links" href="https://data.nal.usda.gov/dataset/treemap-2016-tree-level-model-forests-conterminous-united-states-circa-2016" target="_blank">RDS</a> TreeMap 2016 Data Source\n          </li>\n        </ul>\n        \n    </div>\n    <div class ='my-3'>\n                            <a class="intro-modal-links" onclick="startTour()" title="Click to take a tour of the ${mode}'s features">TOUR</a>\n                            <a class="intro-modal-links" href="https://academic.oup.com/jof/article/120/6/607/6701541" target="_blank" title="Open 2016 TreeMap documentation">METHODS</a>\n                            <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >HELPDESK/FEEDBACK</a> \n                        </div>\n\n</div>`, "<p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n\n")
     },
     loadingModal: {
         all: function(e, a, t = "map services within Google Earth Engine") {
             let o = `<img class = 'logo' src="./images/${e}"   alt="${mode} logo image">`;
             return "" !== e && null != e || (o = ""), `<span>\n                                                           ${o} \n                                                            <h2 id = 'intro-modal-title-banner' title="" class = 'splash-title' style="font-weight:100;font-family: 'Roboto';">${topBannerParams.leftWords}<span  style="font-weight:1000;font-family: 'Roboto Black', sans-serif;"> ${topBannerParams.centerWords} </span> ${topBannerParams.rightWords}</h2>\n                                                        </span>\n\n                            \n\n                        <p style = 'margin-top:1rem;'>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n                <p style='font-weight:bold;margin-top:1rem;' title='Creating map services within Google Earth Engine. This can take some time. Thank you for your patience!'>\n                  <img style="width:2.1em;" class="image-icon fa-spin mr-1" alt= "Google Earth Engine logo spinner" src="images/GEE_logo_transparent.png">\n                    ${a} ${t}. This can take some time.\n                  \n                 </p>\n                  `
         },
         geeViz: '\n                <p>\n                  <img style="width:2.1em;" class="image-icon fa-spin mr-1" alt= "Google Earth Engine logo spinner" src="images/GEE_logo_transparent.png">\n                    Creating map services within Google Earth Engine. \n                  <br>\n                   <img style="width:2.1em;" class="image-icon fa-spin mr-1" alt= "Google Earth Engine logo spinner" src="images/GEE_logo_transparent.png">\n                    This can take some time. Thank you for your patience!\n                   <div id = \'loading-number-box\'></div>\n                 </p>\n                  '
     },
-    bottomBar: '<footer class = \'bottombar\'  id = \'bottombar\' >\n        \t\t\t<span class = \'px-2\'  id=\'current-tool-selection\' title="Any tool that is currently active is shown here."></span>\n        \t\t\t<span class = \'px-2\' title="All map layers are dynamically requested from Google Earth Engine.  The number of outstanding requests is shown here.">Queue length for maps from GEE: <span id=\'outstanding-gee-requests\'>0</span></span>\n                    <span class = \'px-2\' title="The number of outstanding map layers currently loading tiles.">Number of map layers loading tiles: <span id=\'number-gee-tiles-downloading\'>0</span></span>\n                    <span title="Current location and elevation of mouse pointer and map zoom level and respective map scale" class = \'px-2\'  id=\'current-mouse-position\'  ></span>\n                    <span id = \'contributor-logos\' > \n                        <a href="https://earthengine.google.com/" target="_blank">\n                            <img src="images/GEE.png"   class = \'image-icon-bar\' alt="Powered by Google Earth Engine"  href="#" title="Click to learn more about Google Earth Engine">\n                        </a>\n                        <a href="http://www.fs.fed.us//" target="_blank">\n                            <img src="images/usfslogo.png" class = \'image-icon-bar\'  href="#"  alt= "USDA Forest Service logo" title="Click to learn more about the US Forest Service">\n                        </a>\n                        <a href="http://www.usda.gov" target="_blank">\n                            <img src="images/usdalogo.png" class = \'image-icon-bar\'  href="#"   alt= "USDA logo" title="Click to learn more about the USDA">\n                        </a>\n                    </span>\n                </footer>',
+    bottomBar: '<footer class = \'bottombar\'  id = \'bottombar\' >\n        \t\t\t<span class = \'px-2\'  id=\'current-tool-selection\' title="Any tool that is currently active is shown here."></span>\n        \t\t\t<span class = \'px-2\' title="All map layers are dynamically requested from Google Earth Engine.  The number of outstanding requests is shown here.">Queue length for maps from GEE: <span id=\'outstanding-gee-requests\'>0</span></span>\n                    <span class = \'px-2\' title="The number of outstanding map layers currently loading tiles.">Number of map layers loading tiles: <span id=\'number-gee-tiles-downloading\'>0</span></span>\n                    <span title="Current location and elevation of mouse pointer and map zoom level and respective map scale" class = \'px-2\'  id=\'current-mouse-position\'  ></span>\n                    <span id = \'contributor-logos\' > \n                        <a href="https://earthengine.google.com/" target="_blank">\n                            <img src="images/GEE.png"   class = \'image-icon-bar\' alt="Powered by Google Earth Engine"  href="#" title="Click to learn more about Google Earth Engine">\n                        </a>\n                        <a href="https://www.fs.usda.gov/" target="_blank">\n                            <img src="images/usfslogo.png" class = \'image-icon-bar\'  href="#"  alt= "USDA Forest Service logo" title="Click to learn more about the US Forest Service">\n                        </a>\n                        <a href="http://www.usda.gov" target="_blank">\n                            <img src="images/usdalogo.png" class = \'image-icon-bar\'  href="#"   alt= "USDA logo" title="Click to learn more about the USDA">\n                        </a>\n                    </span>\n                </footer>',
     dashboardResultsDiv: "<div class = 'dashboard-results-container' id = 'dashboard-results-container' style='display:none;'>\n                                <div id ='dashboard-results-expander' title='Click and drag up and down to resize charts'></div>\n                                <div id='dashboard-results-div' class='bg-black dashboard-results'></div>\n                            </div>",
     dashboardHighlightsDisclaimerText: "LCMS Dashboard Beta Disclaimer: All summary numbers are based on modeled LCMS outputs. Known as model-based inference, error margins are difficult to compute directly from the summary pixel counts. Currently, error margins are calculated from the LCMS refence sample for each year from each summary area plus a 210km buffer. This assumes the statistical properties of the model-based and reference sample-based estimates are similar. Since this assumption is difficult to uphold, this method is still under scientific review. Theses tables are useful for understanding broad patterns of change on our landscape. For details on valid statistical conclusions and understanding map error, please refer to the LCMS methods document or reach out to the LCMS HELPDESK",
     dashboardHighlightsDiv: "<div id='dashboard-highlights-container' class='dashboard-highlights bg-black'>\n        <img style='height:3rem;' title = 'Click to toggle highlights visibility' class='sidebar-toggler' src='./images/menu-hamburger_ffffff.svg' onclick = 'toggleHighlights()' >\n        <p class='highlights-title highlights-div' style='' title = 'As you move the map around, summary areas that are visible will be ranked according to classes selected within the PARAMETERS menu'>Change Highlights</p>\n        <div class='dashboard-download-div' id = 'download-dashboard-report-container' title='Click to download charts and tables in a single pdf report.'>\n        <button class='btn dashboard-download-button' id='dashboard-download-button' onclick='makeDashboardReport()' >\n          <i class=\"fa fa-download dashboard-download-icon\" aria-hidden=\"true\"></i>\n          Download Report\n          \n        </button>\n        \n        \n      </div>\n        <div id='highlights-tables-container'>\n            <ul class=\"nav nav-tabs px-2 highlights-table-tabs\"  role=\"tablist\" id='highlights-table-tabs'></ul>\n            <div class=\"tab-content\" id=\"highlights-table-divs\"></div>\n            <p class = 'highlights-disclaimer'>Disclaimer: All summary numbers are based on modeled LCMS outputs. Known as model-based inference, error margins are difficult to compute directly from the summary pixel counts. Currently, error margins are calculated from the LCMS refence sample for each year from each summary area plus a 210km buffer. This assumes the statistical properties of the model-based and reference sample-based estimates are similar. Since this assumption is difficult to uphold, this method is still under scientific review. Theses tables are useful for understanding broad patterns of change on our landscape. For details on valid statistical conclusions and understanding map error, please refer to the <a class=\"teal\" onclick=\"downloadMethods('v2021-7')\" title=\"Open in-depth LCMS v2021.7 methods documentation\">LCMS METHODS</a> document or reach out to the <a class = \"teal\" title = \"Send us an E-mail\" href = \"mailto: sm.fs.lcms@usda.gov\" >LCMS HELPDESK</a>.\n            </p>\n        </div>\n        \n        </p>",
     dashboardProgressDiv: `<div id = 'dashboard-progress-container' class='ml-3'>\n        <span  style = 'display: flex;'>\n        <img id = 'loading-spinner-logo' class = 'fa-spin progress-spinner' style='display:none;' src="./images/GEE_logo_transparent.png" height="${convertRemToPixels(.8)}"  alt="GEE logo image">\n        \n        <div class="progressbar" id='highlights-progressbar' class = 'px-2' title='Percent of summary areas that have finished downloading LCMS summary data'>\n            <span style="width: 0%;">0%</span>\n        </div>\n        <i  onclick='clearAllSelectedDashboardFeatures()' id='erase-all-dashboard-selected' title="Click to clear all selected features from this layer" class="fa fa-eraser eraser-all" ></i>\n        \n        </span>\n        \n        \n        \n        </div>`,
     walkThroughPopup: "<div class = 'walk-through-popup'>\n                            <div id = 'walk-through-popup-content' class = 'walk-through-popup-content'></div>\n\t                       \t\t<hr>\n\t\t                        <div class=\"icon-bar py-1 \">\n\t\t\t\t\t\t\t\t  <a onclick = 'previousWalkThrough()' title = 'Previous tutorial slide'><i class=\"fa fa-chevron-left text-black\"></i></a>\n\t\t\t\t\t\t\t\t  <a onclick = 'nextWalkThrough()'  title = 'Next tutorial slide'><i class=\"fa fa-chevron-right text-black\"></i></a>\n\t\t\t\t\t\t\t\t  <a id = 'walk-through-popup-progress'></a>\n                                  <a onclick = 'removeWalkThroughCollapse()' style = 'float:right;'  title = 'Turn off Walk-Through'><i class=\"fa fa-stop text-black\" aria-hidden=\"true\"></i></a>\n                                </div>\n\t\t\t\t\t\t</div>",
     studyAreaDropdownButtonEnabledTooltip: "Choose your study area",
     studyAreaDropdownButtonDisabledTooltip: "Still waiting on previous map layer requests. Can change study area once the previous requests are finished.",
     reRunButtonEnabledTooltip: "Once finished changing parameters, press this button to refresh map layers",
     reRunButtonDisabledTooltip: "Still waiting on previous map layer requests. Can re-submit once the previous requests are finished.",
     reRunButton: "<button id = 'reRun-button' onclick = 'reRun()' class = 'mb-1 ml-1 btn ' title=\"\">Submit</button>",
     addTimelapsesButton: "<button id = 'addTimelapses-button' onclick = 'addLCMSTimeLapses()' class = 'mb-1 ml-1 btn ' title=\"Add interactive time lapse of LCMS Change and Land Cover products. This will slow down the map loading\">Add LCMS Time Lapses To Map</button>",
     downloadDiv: '<div class = \'py-2\'>\n                        <a id = \'product-descriptions\' target = \'_blank\'>Detailed Product Description</a>\n        \t\t\t\t<hr>\n                        <label  title = \'Choose from dropdown below to download LCMS products. There can be a small delay before a download will begin, especially over slower networks.\' for="downloadDropdown">Select product to download:</label>\n    \t\t\t\t\t<select class="form-control" id = "downloadDropdown" onchange = "downloadSelectedArea()""></select>\n    \t\t\t\t </div>',
     lcmsProductionDownloadDiv: '<ul id="downloadTree" class = \'pl-0 mb-0\' title = \'Click through available LCMS products. Select which outputs to download, and then click the download button. Hold ctrl key to select multiples or shift to select blocks.\'>\n                                          <li class = \'pl-0\'><span class="caret caret-down">Conterminous United States (v2021.7)</span>\n                                            <ul class="nested active">\n                                              <li><span class="caret">Change</span>\n                                                <ul class="nested">\n                                                  <li><span class="caret" title = \'Single layer summaries of what year change was mapped by LCMS serve as the foundational LCMS product that is easiest to work with in your local GIS. These are the same as the Slow Loss, Fast Loss, and Gain Year layers in the viewer.\'>Summary</span>\n                                                    <ul class="nested" id = \'CONUS-change-summary-downloads\'></ul>\n                                                  </li>\n                                                  <li><span class="caret" title = \'Annual change layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the change time lapse.\'>Annual</span>\n                                                    <ul class="nested" id = \'CONUS-change-annual-downloads\'></ul>\n                                                  </li>\n                                                </ul>\n                                              </li>\n                                              <li><span class="caret" title = \'Annual land cover layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the land cover time lapse.\'>Land Cover</span>\n                                                <ul class="nested" id = \'CONUS-land_cover-annual-downloads\'></ul>\n                                              </li>\n                                              <li><span class="caret" title = \'Annual land use layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the land use time lapse.\'>Land Use</span>\n                                                <ul class="nested" id = \'CONUS-land_use-annual-downloads\'></ul>\n                                              </li>\n                                              <li><span class="caret" title = \'Annual QA-bits depict ancillary information about the origin of the data used to produce LCMS products.\'>QA Bits</span>\n                                                <ul class="nested" id = \'CONUS-qa_bits-annual-downloads\'></ul>\n                                              </li>\n                                            </ul>\n                                          </li>\n                                          <li><span class="caret caret-down">Southeastern Alaska (v2021.7)</span>\n                                            <ul class="nested active">\n                                              <li><span class="caret">Change</span>\n                                                <ul class="nested">\n                                                  <li><span class="caret" title = \'Single layer summaries of what year change was mapped by LCMS serve as the foundational LCMS product that is easiest to work with in your local GIS. These are the same as the Slow Loss, Fast Loss, and Gain Year layers in the viewer.\'>Summary</span>\n                                                    <ul class="nested" id = \'SEAK-change-summary-downloads\'></ul>\n                                                  </li>\n                                                  <li><span class="caret" title = \'Annual change layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the change time lapse.\'>Annual</span>\n                                                    <ul class="nested" id = \'SEAK-change-annual-downloads\'></ul>\n                                                  </li>\n                                                </ul>\n                                              </li>\n                                              <li><span class="caret" title = \'Annual land cover layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the land cover time lapse.\'>Land Cover</span>\n                                                <ul class="nested" id = \'SEAK-land_cover-annual-downloads\'></ul>\n                                              </li>\n                                              <li><span class="caret" title = \'Annual land use layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the land use time lapse.\'>Land Use</span>\n                                                <ul class="nested" id = \'SEAK-land_use-annual-downloads\'></ul>\n                                              </li>\n                                              <li><span class="caret" title = \'Annual QA-bits depict ancillary information about the origin of the data used to produce LCMS products.\'>QA Bits</span>\n                                                <ul class="nested" id = \'SEAK-qa_bits-annual-downloads\'></ul>\n                                              </li>\n                                            </ul>\n                                          </li>\n                                          <li><span class="caret caret-down">Puerto Rico - US Virgin Islands (v2020.6)</span>\n                                            <ul class="nested active">\n                                              <li><span class="caret">Change</span>\n                                                <ul class="nested">\n                                                  <li><span class="caret" title = \'Single layer summaries of what year change was mapped by LCMS serve as the foundational LCMS product that is easiest to work with in your local GIS. These are the same as the Fast Loss, and Gain Year layers in the viewer.\'>Summary</span>\n                                                    <ul class="nested" id = \'PRUSVI-change-summary-downloads\'></ul>\n                                                  </li>\n                                                  <li><span class="caret" title = \'Annual change layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the change time lapse.\'>Annual</span>\n                                                    <ul class="nested" id = \'PRUSVI-change-annual-downloads\'></ul>\n                                                  </li>\n                                                </ul>\n                                              </li>\n                                              <li><span class="caret" title = \'Annual land cover layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the land cover time lapse.\'>Land Cover</span>\n                                                <ul class="nested" id = \'PRUSVI-land_cover-annual-downloads\'></ul>\n                                              </li>\n                                              <li><span class="caret" title = \'Annual land use layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the land use time lapse.\'>Land Use</span>\n                                                <ul class="nested" id = \'PRUSVI-land_use-annual-downloads\'></ul>\n                                              </li>\n                                            </ul>\n                                          </li>\n                                        </ul>',
-    supportDiv: `<div  class = 'py-2 pl-3 pr-1'>\n                        <header class = 'row ' title = 'Open LCMS Data Explorer tutorial'>\n                            <h3 class = ' text-capitalize'>Tutorial</h3>\n                        </header>\n                        <div class = 'row ' title = 'Open LCMS Data Explorer tutorial'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Information icon' src = './images/information--v2.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a id = 'tutorial-download' class = 'links' onclick = 'downloadTutorial()'>\n                                Click to launch a tutorial that explains how to utilize the Data Explorer</a>\n                            </div>\n                        </div>\n                        <hr>\n                         <header class = 'row ' title = 'Open in-depth LCMS methods documentation'>\n                            <h3 class = ' text-capitalize'>LCMS Methods</h3>\n                        </header>\n                        <div class = 'row ' title = 'Open in-depth LCMS methods documentation'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Methods icon' src = './images/methods-icon.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                Click to open in-depth methods document:\n                                <li>\n                                    <a class = 'links' onclick = 'downloadMethods("v2021-7")' title = 'Open in-depth LCMS v2021.7 methods documentation'>Version 2021.7 (CONUS and SEAK)</a>\n                                </li>\n                                <li>\n                                    <a class = 'links' onclick = 'downloadMethods("v2020-6")' title = 'Open in-depth LCMS v2020.6 methods documentation'>Version 2020.6 (PRUSVI)</a>\n                                </li>   \n                            </div>\n                        </div>\n                        <hr>\n                        <header class = 'row'>\n                            <h3 class = ' text-capitalize' title = "In addition to this viewer, there are viewers to help visualize and explore other aspects of the LCMS data flow">Other LCMS Viewers</h3>\n                        </header>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a title = "In addition to this viewer, there are viewers to help visualize and explore other aspects of the LCMS data flow" ><img class = 'support-icons' alt = 'Email icon' src = './images/lcms-icon.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a class = 'links' title = "Visualize and explore time series datasets used to create the LCMS map outputs" href = "lcms-base-learner.html" target="_blank">LCMS Base Learner Explorer</a>\n                                <hr>\n                                <a class = 'links' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n                            </div>\n                        </section>\n                        <hr>\n                        <header class = 'row'>\n                            <h3 class = ' text-capitalize'>Acknowledgements</h3>\n                        </header>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.fs.fed.us/gstc/" target="_blank">\n                                <img src="./images/GTAC_Logo.png" class = 'support-icons' alt="GTAC Logo"  href="#" alt = "Geospatial Technology and Applications Center logo" title="Click to learn more about the Geospatial Technology and Applications Center (GTAC)">\n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.fs.fed.us/gstc/" target="_blank">\n                                    <p class = 'support-text'>The Geospatial Technology and Applications Center (GTAC) provides leadership in geospatial science implementation in the USDA Forest Service by delivering vital services, data products, tools, training, and innovation to solve today's land and resource management challenges. All operational LCMS production and support takes place at GTAC.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.redcastleresources.com/" target="_blank">\n                                    <img src="images/RCR-logo.jpg"  class = 'support-icons' alt="RedCastle Inc. Logo"  href="#"   title="Click to learn more about RedCastle Resources Inc."> \n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.redcastleresources.com/" target="_blank">\n                                    <p class = 'support-text'>RedCastle Resources Inc. is the on-site contractor that has provided the technical expertise for LCMS' operational production, documentation, and delivery at GTAC.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.fs.usda.gov/rmrs/tools/landscape-change-monitoring-system-lcms" target="_blank">\n                                <img src="./images/usfslogo.png" class = 'support-icons' alt="USFS Logo"  href="#"  title="Click to learn more about the Rocky Mountain Research Station (RMRS)">\n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.fs.usda.gov/rmrs/tools/landscape-change-monitoring-system-lcms" target="_blank">\n                                    <p class = 'support-text'>The Rocky Mountain Research Station provides the scientific foundation LCMS is built upon. They have been instrumental in developing and publishing the original LCMS methodology and continue to provide ongoing research and development to further improve LCMS methods.</p>\n                                </a>\n                            </div>\n                        </section>\n                        \n                        <hr>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://earthengine.google.com/" target="_blank">\n                                    <img src="images/GEE_logo_transparent.png"  class = 'support-icons' alt="Google Earth Engine Logo"  href="#"   title="Click to learn more about Google Earth Engine">\n                                    \n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://earthengine.google.com/" target="_blank">\n                                    <p class = 'support-text'>LCMS utilizes Google Earth Engine for most of its data acqusition, processing, and visualization, through an enterprise agreement between the USDA Forest Service and Google. In its current form, LCMS would not be possible without Google Earth Engine.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <h2>"..."</h2>\n                            </div>\n                            <div class = 'col-lg-10  support-text'>\n                                    Suggested citation: \n                                    <p class = 'support-text' onclick = 'copyText("suggested-citation-text","copiedCitationMessageBox")' id = 'suggested-citation-text' title='Click to copy suggested citation to clipboard'>Forest Service, U.S. Department of Agriculture (2022). Landscape Change Monitoring System Data Explorer [Online]. Available at: https://apps.fs.usda.gov/lcms-viewer (Accessed: ${(new Date).toStringFormat()}).\n                                    </p>\n                                    <span>\n                                        <button onclick = 'copyText("suggested-citation-text","copiedCitationMessageBox")'' title = 'Click to copy suggested citation to clipboard' class="py-0 pr-1 fa fa-copy btn input-group-text bg-white" >\n                                        </button>\n                                        <p id = 'copiedCitationMessageBox'></p>\n                                    </span>\n                            </div>\n                        </section>\n                        <hr>\n                        <header class ='row'>\n                            <h3 class ='text-capitalize'>Contact</h3>\n                        </header>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov"><img class = 'support-icons' alt = 'Email icon' src = './images/email.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a class = 'support-text' title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov">\n                                Please contact the LCMS help desk <span href = "mailto: sm.fs.lcms@usda.gov">(sm.fs.lcms@usda.gov)</span> if you have questions/comments about LCMS or have feedback on the LCMS Data Explorer.</a>\n                            </div>\n                        </section>\n        \t\t\t</div>`,
-    supportDivDashboard: `<div  class = 'py-2 pl-3 pr-1'>\n                        <header class = 'row ' title = 'Open LCMS Data Explorer tutorial'>\n                            <h3 class = ' text-capitalize'>Tutorial</h3>\n                        </header>\n                        <div class = 'row ' onclick="startTour()" title="Click to take a tour of the LCMS Dashboard's features">\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Information icon' src = './images/information--v2.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                            <a class="intro-modal-links" onclick="startTour()" title="Click to take a tour of the LCMS Dashboard's features">DASHBOARD TOUR</a>\n                            </div>\n                        </div>\n                        <hr>\n                         <header class = 'row ' title = 'Open in-depth LCMS methods documentation'>\n                            <h3 class = ' text-capitalize'>LCMS Methods</h3>\n                        </header>\n                        <div class = 'row ' title = 'Open in-depth LCMS methods documentation'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Methods icon' src = './images/methods-icon.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                Click to open in-depth methods document:\n                                <li>\n                                    <a class = 'links' onclick = 'downloadMethods("v2021-7")' title = 'Open in-depth LCMS v2021.7 methods documentation'>Version 2021.7 (CONUS and SEAK)</a>\n                                </li>\n                                <li>\n                                    <a class = 'links' onclick = 'downloadMethods("v2020-6")' title = 'Open in-depth LCMS v2020.6 methods documentation'>Version 2020.6 (PRUSVI)</a>\n                                </li>   \n                            </div>\n                        </div>\n                        <hr>\n                        <header class = 'row'>\n                            <h3 class = ' text-capitalize' title = "In addition to this viewer, there are viewers to help visualize and explore other aspects of the LCMS data flow">Other LCMS Viewers</h3>\n                        </header>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a title = "In addition to this viewer, there are viewers to help visualize and explore other aspects of the LCMS data flow" ><img class = 'support-icons' alt = 'LCMS icon' src = './images/lcms-icon.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a class = 'links' title = "Visualize and explore LCMS map outputs" href = "index.html" target="_blank">LCMS Data Explorer</a>\n                                <hr>\n                                <a class = 'links' title = "Visualize and explore time series datasets used to create the LCMS map outputs" href = "lcms-base-learner.html" target="_blank">LCMS Base Learner Explorer</a>\n                                <hr>\n                                <a class = 'links' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n                            </div>\n                        </section>\n                        <hr>\n                        <header class = 'row'>\n                            <h3 class = ' text-capitalize'>Acknowledgements</h3>\n                        </header>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.fs.fed.us/gstc/" target="_blank">\n                                <img src="./images/GTAC_Logo.png" class = 'support-icons' alt="GTAC Logo"  href="#" alt = "Geospatial Technology and Applications Center logo" title="Click to learn more about the Geospatial Technology and Applications Center (GTAC)">\n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.fs.fed.us/gstc/" target="_blank">\n                                    <p class = 'support-text'>The Geospatial Technology and Applications Center (GTAC) provides leadership in geospatial science implementation in the USDA Forest Service by delivering vital services, data products, tools, training, and innovation to solve today's land and resource management challenges. All operational LCMS production and support takes place at GTAC.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.redcastleresources.com/" target="_blank">\n                                    <img src="images/RCR-logo.jpg"  class = 'support-icons' alt="RedCastle Inc. Logo"  href="#"   title="Click to learn more about RedCastle Resources Inc."> \n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.redcastleresources.com/" target="_blank">\n                                    <p class = 'support-text'>RedCastle Resources Inc. is the on-site contractor that has provided the technical expertise for LCMS' operational production, documentation, and delivery at GTAC.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.fs.usda.gov/rmrs/tools/landscape-change-monitoring-system-lcms" target="_blank">\n                                <img src="./images/usfslogo.png" class = 'support-icons' alt="USFS Logo"  href="#"  title="Click to learn more about the Rocky Mountain Research Station (RMRS)">\n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.fs.usda.gov/rmrs/tools/landscape-change-monitoring-system-lcms" target="_blank">\n                                    <p class = 'support-text'>The Rocky Mountain Research Station provides the scientific foundation LCMS is built upon. They have been instrumental in developing and publishing the original LCMS methodology and continue to provide ongoing research and development to further improve LCMS methods.</p>\n                                </a>\n                            </div>\n                        </section>\n                        \n                        <hr>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://earthengine.google.com/" target="_blank">\n                                    <img src="images/GEE_logo_transparent.png"  class = 'support-icons' alt="Google Earth Engine Logo"  href="#"   title="Click to learn more about Google Earth Engine">\n                                    \n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://earthengine.google.com/" target="_blank">\n                                    <p class = 'support-text'>LCMS utilizes Google Earth Engine for most of its data acqusition, processing, and visualization, through an enterprise agreement between the USDA Forest Service and Google. In its current form, LCMS would not be possible without Google Earth Engine.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <h2>"..."</h2>\n                            </div>\n                            <div class = 'col-lg-10  support-text'>\n                                    Suggested citation: \n                                    <p class = 'support-text' onclick = 'copyText("suggested-citation-text","copiedCitationMessageBox")' id = 'suggested-citation-text' title='Click to copy suggested citation to clipboard'>Forest Service, U.S. Department of Agriculture (2022). Landscape Change Monitoring System Dashboard [Online]. Available at: https://apps.fs.usda.gov/lcms-viewer/dashboard.html (Accessed: ${(new Date).toStringFormat()}).\n                                    </p>\n                                    <span>\n                                        <button onclick = 'copyText("suggested-citation-text","copiedCitationMessageBox")'' title = 'Click to copy suggested citation to clipboard' class="py-0 pr-1 fa fa-copy btn input-group-text bg-white" >\n                                        </button>\n                                        <p id = 'copiedCitationMessageBox'></p>\n                                    </span>\n                            </div>\n                        </section>\n                        <hr>\n                        <header class ='row'>\n                            <h3 class ='text-capitalize'>Contact</h3>\n                        </header>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov"><img class = 'support-icons' alt = 'Email icon' src = './images/email.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a class = 'support-text' title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov">\n                                Please contact the LCMS help desk <span href = "mailto: sm.fs.lcms@usda.gov">(sm.fs.lcms@usda.gov)</span> if you have questions/comments about LCMS or have feedback on the LCMS Dashboard.</a>\n                            </div>\n                        </section>\n        \t\t\t</div>`,
-    supportDivAlgal: `<div  class = 'py-2 pl-3 pr-1'>\n                        <header class = 'row ' title = 'Open ${mode} tutorial'>\n                            <h3 class = ' text-capitalize'>Tutorial</h3>\n                        </header>\n                        <div class = 'row ' onclick="startTour()" title="Click to take a tour of the ${mode}'s features">\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Information icon' src = './images/information--v2.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                            <a class="intro-modal-links" onclick="startTour()" title="Click to take a tour of the LCMS ${mode}'s features">${mode} TOUR</a>\n                            </div>\n                        </div>\n                        <hr>\n                         <header class = 'row ' title = 'Open in-depth ${mode} methods documentation'>\n                            <h3 class = ' text-capitalize'>${mode} Methods</h3>\n                        </header>\n                        <div class = 'row ' title = 'Open in-depth ${mode} methods documentation'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Methods icon' src = './images/methods-icon.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                Click to open in-depth methods document:\n                                <li>\n                                <a class="intro-modal-links" onclick="downloadAnyMethods('./literature/Bloom_Mapper_v3_Methods_2023.pdf')" title="Open Bloom Mapper data creation methods documentation">Bloom Mapper V3 METHODS</a>\n                                </li>\n                            </div>\n                        </div>\n                        \n                        <hr>\n                        <header class = 'row'>\n                            <h3 class = ' text-capitalize'>Acknowledgements</h3>\n                        </header>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.fs.fed.us/gstc/" target="_blank">\n                                <img src="./images/GTAC_Logo.png" class = 'support-icons' alt="GTAC Logo"  href="#" alt = "Geospatial Technology and Applications Center logo" title="Click to learn more about the Geospatial Technology and Applications Center (GTAC)">\n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.fs.fed.us/gstc/" target="_blank">\n                                    <p class = 'support-text'>The Geospatial Technology and Applications Center (GTAC) provides leadership in geospatial science implementation in the USDA Forest Service by delivering vital services, data products, tools, training, and innovation to solve today's land and resource management challenges. All operational LCMS production and support takes place at GTAC.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.redcastleresources.com/" target="_blank">\n                                    <img src="images/RCR-logo.jpg"  class = 'support-icons' alt="RedCastle Inc. Logo"  href="#"   title="Click to learn more about RedCastle Resources Inc."> \n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.redcastleresources.com/" target="_blank">\n                                    <p class = 'support-text'>RedCastle Resources Inc. is the on-site contractor that has provided the technical expertise for ${mode}'s methods development, documentation, and visualization (this viewer) at GTAC.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="" target="_blank">\n                                    <img src="./images/usfslogo.png" class = 'support-icons' alt="USFS Logo"  href="#"  title="Click to learn more about our field collaborators ">\n                                </a>\n                                \n                                <a href="" target="_blank" >\n                                    <img class = 'support-icons' alt="Wyoming Department of Environmental Quality icon" src="images/WY-DEQ-Logo.png" style="margin-top: 1rem;padding-right: 0.5rem;">\n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="" target="_blank">\n                                    <p class = 'support-text'>\n                                    USFS units in Regions 2 and 4 in Wyoming collaborated to help GTAC develop and train this tool based on actual bloom data collected by the Wyoming Department of Environmental Quality, Water Quality Division, Watershed Protection Program as part of their state-wide monitoring efforts to document the occurrence of Harmful Cyanobacterial Blooms. Thousands of lakes over ~1 acre exist on Forest system lands in Wyoming. This tool is critical in helping Forest staff focus efforts to address this public safety concern.</p>\n                                </a>\n                            </div>\n                        </section>\n                        \n                        <hr>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://earthengine.google.com/" target="_blank">\n                                    <img src="images/GEE_logo_transparent.png"  class = 'support-icons' alt="Google Earth Engine Logo"  href="#"   title="Click to learn more about Google Earth Engine">\n                                    \n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://earthengine.google.com/" target="_blank">\n                                    <p class = 'support-text'>${mode} utilizes Google Earth Engine for most of its data acqusition, processing, and visualization, through an enterprise agreement between the USDA Forest Service and Google. In its current form, ${mode} would not be possible without Google Earth Engine.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <h2>"..."</h2>\n                            </div>\n                            <div class = 'col-lg-10  support-text'>\n                                    Suggested citation: \n                                    <p class = 'support-text' onclick = 'copyText("suggested-citation-text","copiedCitationMessageBox")' id = 'suggested-citation-text' title='Click to copy suggested citation to clipboard'>Forest Service, U.S. Department of Agriculture (2022). ${mode} [Online]. Available at: https://apps.fs.usda.gov/lcms-viewer/${mode}.html (Accessed: ${(new Date).toStringFormat()}).\n                                    </p>\n                                    <span>\n                                        <button onclick = 'copyText("suggested-citation-text","copiedCitationMessageBox")'' title = 'Click to copy suggested citation to clipboard' class="py-0 pr-1 fa fa-copy btn input-group-text bg-white" >\n                                        </button>\n                                        <p id = 'copiedCitationMessageBox'></p>\n                                    </span>\n                            </div>\n                        </section>\n                        <hr>\n                        <header class ='row'>\n                            <h3 class ='text-capitalize'>Contact</h3>\n                        </header>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov"><img class = 'support-icons' alt = 'Email icon' src = './images/email.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a class = 'support-text' title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov">\n                                Please contact the ${mode} help desk <span href = "mailto: sm.fs.lcms@usda.gov">(sm.fs.lcms@usda.gov)</span> if you have questions/comments about ${mode} or have feedback on the ${mode}.</a>\n                            </div>\n                        </section>\n        \t\t\t</div>`,
+    supportDiv: `<div  class = 'py-2 pl-3 pr-1'>\n                        <header class = 'row ' title = 'Open LCMS Data Explorer tutorial'>\n                            <h3 class = ' text-capitalize'>Tutorial</h3>\n                        </header>\n                        <div class = 'row ' title = 'Open LCMS Data Explorer tutorial'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Information icon' src = './images/information--v2.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a id = 'tutorial-download' class = 'links' onclick = 'downloadTutorial()'>\n                                Click to launch a tutorial that explains how to utilize the Data Explorer</a>\n                            </div>\n                        </div>\n                        <hr>\n                        \n                        <header class = 'row ' title = 'Click to help us learn how you use LCMS and how we can make it better'>\n                        <h3 class = ' text-capitalize'>LCMS Survey</h3>\n                    </header>\n                    <div class = 'row ' title = 'Click to help us learn how you use LCMS and how we can make it better'>\n                        <div class = 'col-lg-2 p-0 m-0'>\n                            <img class = 'support-icons' alt = 'Methods icon' src = './Icons_svg/documentation_372e2c.svg'></a> \n                        </div>\n                        <div class = 'col-lg-10'>\n                            Click to open the LCMS Survey:\n                            <li>\n                            <a  class = 'intro-modal-links'  onclick = 'openLCMSSurvey("supportMenu")' title="Click to help us learn how you use LCMS and how we can make it better">SURVEY</a>\n                            </li>\n                             \n                        </div>\n                    </div>\n                    <hr>\n                         <header class = 'row ' title = 'Open in-depth LCMS methods documentation'>\n                            <h3 class = ' text-capitalize'>LCMS Methods</h3>\n                        </header>\n                        <div class = 'row ' title = 'Open in-depth LCMS methods documentation'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Methods icon' src = './images/methods-icon.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                Click to open in-depth methods document:\n                                <li>\n                                    <a class = 'links' onclick = 'downloadMethods("v2021-7")' title = 'Open in-depth LCMS v2021.7 methods documentation'>Version 2021.7 (CONUS and SEAK)</a>\n                                </li>\n                                <li>\n                                    <a class = 'links' onclick = 'downloadMethods("v2020-6")' title = 'Open in-depth LCMS v2020.6 methods documentation'>Version 2020.6 (PRUSVI)</a>\n                                </li>   \n                            </div>\n                        </div>\n                        <hr>\n                        <header class = 'row'>\n                            <h3 class = ' text-capitalize' title = "In addition to this viewer, there are viewers to help visualize and explore other aspects of the LCMS data flow">Other LCMS Viewers</h3>\n                        </header>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a title = "In addition to this viewer, there are viewers to help visualize and explore other aspects of the LCMS data flow" ><img class = 'support-icons' alt = 'Email icon' src = './images/lcms-icon.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a class = 'links' title = "Visualize and explore time series datasets used to create the LCMS map outputs" href = "lcms-base-learner.html" target="_blank">LCMS Base Learner Explorer</a>\n                                <hr>\n                                <a class = 'links' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n                            </div>\n                        </section>\n                        <hr>\n                        <header class = 'row'>\n                            <h3 class = ' text-capitalize'>Acknowledgements</h3>\n                        </header>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">\n                                <img src="./images/GTAC_Logo.png" class = 'support-icons' alt="GTAC Logo"  href="#" alt = "Geospatial Technology and Applications Center logo" title="Click to learn more about the Geospatial Technology and Applications Center (GTAC)">\n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">\n                                    <p class = 'support-text'>The Geospatial Technology and Applications Center (GTAC) provides leadership in geospatial science implementation in the USDA Forest Service by delivering vital services, data products, tools, training, and innovation to solve today's land and resource management challenges. All operational LCMS production and support takes place at GTAC.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.redcastleresources.com/" target="_blank">\n                                    <img src="images/RCR-logo.jpg"  class = 'support-icons' alt="RedCastle Inc. Logo"  href="#"   title="Click to learn more about RedCastle Resources Inc."> \n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.redcastleresources.com/" target="_blank">\n                                    <p class = 'support-text'>RedCastle Resources Inc. is the on-site contractor that has provided the technical expertise for LCMS' operational production, documentation, and delivery at GTAC.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.fs.usda.gov/rmrs/tools/landscape-change-monitoring-system-lcms" target="_blank">\n                                <img src="./images/usfslogo.png" class = 'support-icons' alt="USFS Logo"  href="#"  title="Click to learn more about the Rocky Mountain Research Station (RMRS)">\n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.fs.usda.gov/rmrs/tools/landscape-change-monitoring-system-lcms" target="_blank">\n                                    <p class = 'support-text'>The Rocky Mountain Research Station provides the scientific foundation LCMS is built upon. They have been instrumental in developing and publishing the original LCMS methodology and continue to provide ongoing research and development to further improve LCMS methods.</p>\n                                </a>\n                            </div>\n                        </section>\n                        \n                        <hr>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://earthengine.google.com/" target="_blank">\n                                    <img src="images/GEE_logo_transparent.png"  class = 'support-icons' alt="Google Earth Engine Logo"  href="#"   title="Click to learn more about Google Earth Engine">\n                                    \n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://earthengine.google.com/" target="_blank">\n                                    <p class = 'support-text'>LCMS utilizes Google Earth Engine for most of its data acqusition, processing, and visualization, through an enterprise agreement between the USDA Forest Service and Google. In its current form, LCMS would not be possible without Google Earth Engine.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <h2>"..."</h2>\n                            </div>\n                            <div class = 'col-lg-10  support-text'>\n                                    Suggested citation: \n                                    <p class = 'support-text' onclick = 'copyText("suggested-citation-text","copiedCitationMessageBox")' id = 'suggested-citation-text' title='Click to copy suggested citation to clipboard'>Forest Service, U.S. Department of Agriculture (2022). Landscape Change Monitoring System Data Explorer [Online]. Available at: https://apps.fs.usda.gov/lcms-viewer (Accessed: ${(new Date).toStringFormat()}).\n                                    </p>\n                                    <span>\n                                        <button onclick = 'copyText("suggested-citation-text","copiedCitationMessageBox")'' title = 'Click to copy suggested citation to clipboard' class="py-0 pr-1 fa fa-copy btn input-group-text bg-white" >\n                                        </button>\n                                        <p id = 'copiedCitationMessageBox'></p>\n                                    </span>\n                            </div>\n                        </section>\n                        <hr>\n                        <header class ='row'>\n                            <h3 class ='text-capitalize'>Contact</h3>\n                        </header>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov"><img class = 'support-icons' alt = 'Email icon' src = './images/email.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a class = 'support-text' title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov">\n                                Please contact the LCMS help desk <span href = "mailto: sm.fs.lcms@usda.gov">(sm.fs.lcms@usda.gov)</span> if you have questions/comments about LCMS or have feedback on the LCMS Data Explorer.</a>\n                            </div>\n                        </section>\n        \t\t\t</div>`,
+    supportDivDashboard: `<div  class = 'py-2 pl-3 pr-1'>\n                        <header class = 'row ' title = 'Open LCMS Data Explorer tutorial'>\n                            <h3 class = ' text-capitalize'>Tutorial</h3>\n                        </header>\n                        <div class = 'row ' onclick="startTour()" title="Click to take a tour of the LCMS Dashboard's features">\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Information icon' src = './images/information--v2.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                            <a class="intro-modal-links" onclick="startTour()" title="Click to take a tour of the LCMS Dashboard's features">DASHBOARD TOUR</a>\n                            </div>\n                        </div>\n                        <hr>\n                                                \n                        <header class = 'row ' title = 'Click to help us learn how you use LCMS and how we can make it better'>\n                        <h3 class = ' text-capitalize'>LCMS Survey</h3>\n                    </header>\n                    <div class = 'row ' title = 'Click to help us learn how you use LCMS and how we can make it better'>\n                        <div class = 'col-lg-2 p-0 m-0'>\n                            <img class = 'support-icons' alt = 'Methods icon' src = './Icons_svg/documentation_372e2c.svg'></a> \n                        </div>\n                        <div class = 'col-lg-10'>\n                            Click to open the LCMS Survey:\n                            <li>\n                            <a  class = 'intro-modal-links'  onclick = 'openLCMSSurvey("supportMenu")' title="Click to help us learn how you use LCMS and how we can make it better">SURVEY</a>\n                            </li>\n                             \n                        </div>\n                    </div>\n                    <hr>\n                         <header class = 'row ' title = 'Open in-depth LCMS methods documentation'>\n                            <h3 class = ' text-capitalize'>LCMS Methods</h3>\n                        </header>\n                        <div class = 'row ' title = 'Open in-depth LCMS methods documentation'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Methods icon' src = './images/methods-icon.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                Click to open in-depth methods document:\n                                <li>\n                                    <a class = 'links' onclick = 'downloadMethods("v2021-7")' title = 'Open in-depth LCMS v2021.7 methods documentation'>Version 2021.7 (CONUS and SEAK)</a>\n                                </li>\n                                <li>\n                                    <a class = 'links' onclick = 'downloadMethods("v2020-6")' title = 'Open in-depth LCMS v2020.6 methods documentation'>Version 2020.6 (PRUSVI)</a>\n                                </li>   \n                            </div>\n                        </div>\n                        <hr>\n                         <header class = 'row ' title = 'Open in-depth LCMS methods documentation'>\n                            <h3 class = ' text-capitalize'>LCMS Methods</h3>\n                        </header>\n                        <div class = 'row ' title = 'Open in-depth LCMS methods documentation'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Methods icon' src = './images/methods-icon.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                Click to open in-depth methods document:\n                                <li>\n                                    <a class = 'links' onclick = 'downloadMethods("v2021-7")' title = 'Open in-depth LCMS v2021.7 methods documentation'>Version 2021.7 (CONUS and SEAK)</a>\n                                </li>\n                                <li>\n                                    <a class = 'links' onclick = 'downloadMethods("v2020-6")' title = 'Open in-depth LCMS v2020.6 methods documentation'>Version 2020.6 (PRUSVI)</a>\n                                </li>   \n                            </div>\n                        </div>\n                        <hr>\n                        <header class = 'row'>\n                            <h3 class = ' text-capitalize' title = "In addition to this viewer, there are viewers to help visualize and explore other aspects of the LCMS data flow">Other LCMS Viewers</h3>\n                        </header>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a title = "In addition to this viewer, there are viewers to help visualize and explore other aspects of the LCMS data flow" ><img class = 'support-icons' alt = 'LCMS icon' src = './images/lcms-icon.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a class = 'links' title = "Visualize and explore LCMS map outputs" href = "index.html" target="_blank">LCMS Data Explorer</a>\n                                <hr>\n                                <a class = 'links' title = "Visualize and explore time series datasets used to create the LCMS map outputs" href = "lcms-base-learner.html" target="_blank">LCMS Base Learner Explorer</a>\n                                <hr>\n                                <a class = 'links' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n                            </div>\n                        </section>\n                        <hr>\n                        <header class = 'row'>\n                            <h3 class = ' text-capitalize'>Acknowledgements</h3>\n                        </header>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">\n                                <img src="./images/GTAC_Logo.png" class = 'support-icons' alt="GTAC Logo"  href="#" alt = "Geospatial Technology and Applications Center logo" title="Click to learn more about the Geospatial Technology and Applications Center (GTAC)">\n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">\n                                    <p class = 'support-text'>The Geospatial Technology and Applications Center (GTAC) provides leadership in geospatial science implementation in the USDA Forest Service by delivering vital services, data products, tools, training, and innovation to solve today's land and resource management challenges. All operational LCMS production and support takes place at GTAC.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.redcastleresources.com/" target="_blank">\n                                    <img src="images/RCR-logo.jpg"  class = 'support-icons' alt="RedCastle Inc. Logo"  href="#"   title="Click to learn more about RedCastle Resources Inc."> \n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.redcastleresources.com/" target="_blank">\n                                    <p class = 'support-text'>RedCastle Resources Inc. is the on-site contractor that has provided the technical expertise for LCMS' operational production, documentation, and delivery at GTAC.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.fs.usda.gov/rmrs/tools/landscape-change-monitoring-system-lcms" target="_blank">\n                                <img src="./images/usfslogo.png" class = 'support-icons' alt="USFS Logo"  href="#"  title="Click to learn more about the Rocky Mountain Research Station (RMRS)">\n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.fs.usda.gov/rmrs/tools/landscape-change-monitoring-system-lcms" target="_blank">\n                                    <p class = 'support-text'>The Rocky Mountain Research Station provides the scientific foundation LCMS is built upon. They have been instrumental in developing and publishing the original LCMS methodology and continue to provide ongoing research and development to further improve LCMS methods.</p>\n                                </a>\n                            </div>\n                        </section>\n                        \n                        <hr>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://earthengine.google.com/" target="_blank">\n                                    <img src="images/GEE_logo_transparent.png"  class = 'support-icons' alt="Google Earth Engine Logo"  href="#"   title="Click to learn more about Google Earth Engine">\n                                    \n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://earthengine.google.com/" target="_blank">\n                                    <p class = 'support-text'>LCMS utilizes Google Earth Engine for most of its data acqusition, processing, and visualization, through an enterprise agreement between the USDA Forest Service and Google. In its current form, LCMS would not be possible without Google Earth Engine.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <h2>"..."</h2>\n                            </div>\n                            <div class = 'col-lg-10  support-text'>\n                                    Suggested citation: \n                                    <p class = 'support-text' onclick = 'copyText("suggested-citation-text","copiedCitationMessageBox")' id = 'suggested-citation-text' title='Click to copy suggested citation to clipboard'>Forest Service, U.S. Department of Agriculture (2022). Landscape Change Monitoring System Dashboard [Online]. Available at: https://apps.fs.usda.gov/lcms-viewer/dashboard.html (Accessed: ${(new Date).toStringFormat()}).\n                                    </p>\n                                    <span>\n                                        <button onclick = 'copyText("suggested-citation-text","copiedCitationMessageBox")'' title = 'Click to copy suggested citation to clipboard' class="py-0 pr-1 fa fa-copy btn input-group-text bg-white" >\n                                        </button>\n                                        <p id = 'copiedCitationMessageBox'></p>\n                                    </span>\n                            </div>\n                        </section>\n                        <hr>\n                        <header class ='row'>\n                            <h3 class ='text-capitalize'>Contact</h3>\n                        </header>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov"><img class = 'support-icons' alt = 'Email icon' src = './images/email.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a class = 'support-text' title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov">\n                                Please contact the LCMS help desk <span href = "mailto: sm.fs.lcms@usda.gov">(sm.fs.lcms@usda.gov)</span> if you have questions/comments about LCMS or have feedback on the LCMS Dashboard.</a>\n                            </div>\n                        </section>\n        \t\t\t</div>`,
+    supportDivAlgal: `<div  class = 'py-2 pl-3 pr-1'>\n                        <header class = 'row ' title = 'Open ${mode} tutorial'>\n                            <h3 class = ' text-capitalize'>Tutorial</h3>\n                        </header>\n                        <div class = 'row ' onclick="startTour()" title="Click to take a tour of the ${mode}'s features">\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Information icon' src = './images/information--v2.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                            <a class="intro-modal-links" onclick="startTour()" title="Click to take a tour of the LCMS ${mode}'s features">${mode} TOUR</a>\n                            </div>\n                        </div>\n                        <hr>\n                         <header class = 'row ' title = 'Open in-depth ${mode} methods documentation'>\n                            <h3 class = ' text-capitalize'>${mode} Methods</h3>\n                        </header>\n                        <div class = 'row ' title = 'Open in-depth ${mode} methods documentation'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Methods icon' src = './images/methods-icon.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                Click to open in-depth methods document:\n                                <li>\n                                <a class="intro-modal-links" onclick="downloadAnyMethods('./literature/Bloom_Mapper_v3_Methods_2023.pdf')" title="Open Bloom Mapper data creation methods documentation">Bloom Mapper V3 METHODS</a>\n                                </li>\n                            </div>\n                        </div>\n                        \n                        <hr>\n                        <header class = 'row'>\n                            <h3 class = ' text-capitalize'>Acknowledgements</h3>\n                        </header>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">\n                                <img src="./images/GTAC_Logo.png" class = 'support-icons' alt="GTAC Logo"  href="#" alt = "Geospatial Technology and Applications Center logo" title="Click to learn more about the Geospatial Technology and Applications Center (GTAC)">\n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">\n                                    <p class = 'support-text'>The Geospatial Technology and Applications Center (GTAC) provides leadership in geospatial science implementation in the USDA Forest Service by delivering vital services, data products, tools, training, and innovation to solve today's land and resource management challenges. All operational LCMS production and support takes place at GTAC.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.redcastleresources.com/" target="_blank">\n                                    <img src="images/RCR-logo.jpg"  class = 'support-icons' alt="RedCastle Inc. Logo"  href="#"   title="Click to learn more about RedCastle Resources Inc."> \n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.redcastleresources.com/" target="_blank">\n                                    <p class = 'support-text'>RedCastle Resources Inc. is the on-site contractor that has provided the technical expertise for ${mode}'s methods development, documentation, and visualization (this viewer) at GTAC.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="" target="_blank">\n                                    <img src="./images/usfslogo.png" class = 'support-icons' alt="USFS Logo"  href="#"  title="Click to learn more about our field collaborators ">\n                                </a>\n                                \n                                <a href="" target="_blank" >\n                                    <img class = 'support-icons' alt="Wyoming Department of Environmental Quality icon" src="images/WY-DEQ-Logo.png" style="margin-top: 1rem;padding-right: 0.5rem;">\n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="" target="_blank">\n                                    <p class = 'support-text'>\n                                    USFS units in Regions 2 and 4 in Wyoming collaborated to help GTAC develop and train this tool based on actual bloom data collected by the Wyoming Department of Environmental Quality, Water Quality Division, Watershed Protection Program as part of their state-wide monitoring efforts to document the occurrence of Harmful Cyanobacterial Blooms. Thousands of lakes over ~1 acre exist on Forest system lands in Wyoming. This tool is critical in helping Forest staff focus efforts to address this public safety concern.</p>\n                                </a>\n                            </div>\n                        </section>\n                        \n                        <hr>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://earthengine.google.com/" target="_blank">\n                                    <img src="images/GEE_logo_transparent.png"  class = 'support-icons' alt="Google Earth Engine Logo"  href="#"   title="Click to learn more about Google Earth Engine">\n                                    \n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://earthengine.google.com/" target="_blank">\n                                    <p class = 'support-text'>${mode} utilizes Google Earth Engine for most of its data acqusition, processing, and visualization, through an enterprise agreement between the USDA Forest Service and Google. In its current form, ${mode} would not be possible without Google Earth Engine.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <h2>"..."</h2>\n                            </div>\n                            <div class = 'col-lg-10  support-text'>\n                                    Suggested citation: \n                                    <p class = 'support-text' onclick = 'copyText("suggested-citation-text","copiedCitationMessageBox")' id = 'suggested-citation-text' title='Click to copy suggested citation to clipboard'>Forest Service, U.S. Department of Agriculture (2022). ${mode} [Online]. Available at: https://apps.fs.usda.gov/lcms-viewer/${mode}.html (Accessed: ${(new Date).toStringFormat()}).\n                                    </p>\n                                    <span>\n                                        <button onclick = 'copyText("suggested-citation-text","copiedCitationMessageBox")'' title = 'Click to copy suggested citation to clipboard' class="py-0 pr-1 fa fa-copy btn input-group-text bg-white" >\n                                        </button>\n                                        <p id = 'copiedCitationMessageBox'></p>\n                                    </span>\n                            </div>\n                        </section>\n                        <hr>\n                        <header class ='row'>\n                            <h3 class ='text-capitalize'>Contact</h3>\n                        </header>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov"><img class = 'support-icons' alt = 'Email icon' src = './images/email.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a class = 'support-text' title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov">\n                                Please contact the ${mode} help desk <span href = "mailto: sm.fs.lcms@usda.gov">(sm.fs.lcms@usda.gov)</span> if you have questions/comments about ${mode} or have feedback on the ${mode}.</a>\n                            </div>\n                        </section>\n        \t\t\t</div>`,
     tooltipToggle: " <label class = 'mt-2'>If you turned off tool tips, but want them back:</label>\n                        <button  class = 'btn  bg-black' onclick = 'showToolTipsAgain()'>Show tooltips</button>",
     walkThroughButton: `<div >\n                            <label class = 'mt-2'>Run a walk-through of the ${mode} Data Explorer's features</label>\n                            <a  class = 'intro-modal-links ' onclick = 'toggleWalkThroughCollapse()' title = 'Run interactive walk-through of the features of the ${mode} Data Explorer'>Run Walk-Through</a>\n                          </div>`,
     distanceDiv: "Click on map to measure distance",
     distanceTip: "Click on map to measure distance. Press <kbd>ctrl+z</kbd> to undo most recent point. Double-click, press <kbd>Delete</kbd>, or press <kbd>Backspace</kbd> to clear measurment and start over.",
     areaDiv: "Click on map to measure area<variable-radio onclick1 = 'updateArea()' onclick2 = 'updateArea()' var='metricOrImperialArea' title2='' name2='Metric' name1='Imperial' value2='metric' value1='imperial' type='string' title='Toggle between imperial or metric units'></variable-radio>\n       ",
     areaTip: "Click on map to measure area. Double-click to complete polygon, press <kbd>ctrl+z</kbd> to undo most recent point, press <kbd>Delete</kbd> or <kbd>Backspace</kbd> to start over. Any number of polygons can be defined by repeating this process.",
     queryDiv: "<div>Double-click on map to query values of displayed layers at that location</div>",
@@ -854,14 +855,18 @@
     null == e && (e = "modal-id"), $("#" + e + "-title .modal-title").html(""), $("#" + e + "-header").html(""), $("#" + e + "-body").html(""), $("#" + e + "-footer").html(""), $(".modal").modal("hide"), $(".modal-backdrop").remove()
 }
 
 function showMessage(e, a, t, o) {
     null == e && (e = ""), null == a && (a = ""), null == o && (o = !0), null == t && (t = "error-modal"), clearModal(t), addModal("main-container", t, !0), "" !== e && null != e && addModalTitle(t, e), $("#" + t + "-body").append(a), o && $("#" + t).modal()
 }
 
+function appendMessage2(e, a) {
+    null == e && (e = ""), null == a && (a = "error-modal"), $("#" + a + "-body").append(e)
+}
+
 function showTip(e, a) {
     null != localStorage.showToolTipModal && "undefined" != localStorage.showToolTipModal || (localStorage.showToolTipModal = "true"), "true" === localStorage.showToolTipModal && 0 == walkThroughAdded && (showMessage("", '<span class = "font-weight-bold text-uppercase" >' + e + " </span><span>" + a + "</span>", "tip-modal", !1), $("#tip-modal-body").append('<form class="form-inline pt-3 pb-0">\n\t\t\t\t\t\t\t\t  <div class="form-check  mr-0">\n                                \t<input role="option" type="checkbox" class="form-check-input" id="dontShowTipAgainCheckbox"   name = \'dontShowAgain\' value = \'true\'>\n                                \t<label class=" text-uppercase form-check-label " for="dontShowTipAgainCheckbox" >Turn off tips</label>\n                            \t\t</div>\n\t\t\t\t\t\t\t\t</form>'), $("#tip-modal").modal().show()), $("#dontShowTipAgainCheckbox").change((function() {
         console.log(this.checked), localStorage.showToolTipModal = !this.checked, "false" === localStorage.showToolTipModal ? $("#tooltip-radio-second_toggle_label").click() : "true" === localStorage.showToolTipModal && $("#tooltip-radio-first_toggle_label").click()
     }))
 }
 
 function addStudyAreaToDropdown(e, a) {
@@ -1047,15 +1052,15 @@
 }
 
 function moveCollapse(e, a = getWalkThroughCollapseContainerID()) {
     $("#" + e + "-label").detach().appendTo("#" + a), $("#" + e + "-div").detach().appendTo("#" + a)
 }
 
 function addLegendCollapse() {
-    addCollapse(getWalkThroughCollapseContainerID(), "legend-collapse-label", "legend-collapse-div", "LEGEND", '<i class="fa fa-location-arrow fa-rotate-45 mx-1" aria-hidden="true"></i>', !0, "", "LEGEND of the layers displayed on the map"), $("#legend-collapse-div").append('<div role="list" id="legend-layer-list"></div>'), $("#legend-collapse-div").append('<div role="list" id="legend-reference-layer-list"></div>'), $("#legend-collapse-div").append('<div role="list" id="legend-fhp-div"></div>'), $("#legend-collapse-div").append('<div role="list" id="time-lapse-legend-list"></div>'), $("#legend-collapse-div").append('<div role="list" id="legend-area-charting-select-layer-list"></div>')
+    addCollapse(getWalkThroughCollapseContainerID(), "legend-collapse-label", "legend-collapse-div", "LEGEND", '<i class="fa fa-location-arrow fa-rotate-45 mx-1" aria-hidden="true"></i>', !0, "", "LEGEND of the layers displayed on the map"), addCollapse(getWalkThroughCollapseContainerID(), "chart-collapse-label", "chart-collapse-div", "QUERY OUTPUTS", '<i class="fa fa-graph fa-rotate-45 mx-1" aria-hidden="true"></i>', !0, "", "Charts go here"), $("#chart-collapse-div").append('<div role="list" id="chart-list"></div>'), $("#chart-collapse-label-chart-collapse-div").hide(), $("#chart-collapse-div").removeClass("px-5"), $("#chart-collapse-div").addClass("px-3"), $("#legend-collapse-div").append('<div role="list" id="legend-layer-list"></div>'), $("#legend-collapse-div").append('<div role="list" id="legend-reference-layer-list"></div>'), $("#legend-collapse-div").append('<div role="list" id="legend-fhp-div"></div>'), $("#legend-collapse-div").append('<div role="list" id="time-lapse-legend-list"></div>'), $("#legend-collapse-div").append('<div role="list" id="legend-area-charting-select-layer-list"></div>')
 }
 
 function addLegendContainer(e, a, t, o) {
     null == a && (a = "legend-collapse-div"), null == t && (t = !0), t = t ? "block" : "none", $("#" + a).prepend(`<div class = 'py-1 row' title= '${o}' style = 'display:${t};' id = '${e}'>\n\t\t\t\t\t\t\t\t</div>`)
 }
 
 function addClassLegendContainer(e, a, t) {
@@ -1135,19 +1140,19 @@
         e.loadError = !0, console.log("GEE Tile Service request failed for " + e.name), console.log(o), $("#" + o).css("background", "red"), $("#" + o).attr("title", 'Layer failed to load. Error message: "' + a + '"')
     }
 
     function g() {
         p(), layerObj[a].visible = e.visible, layerObj[a].opacity = e.opacity
     }
 
-    function f() {
+    function v() {
         e.loadError || (e.visible ? (ga("send", "event", "layer-off", e.layerType, e.name), "dynamicMapService" === e.layerType ? (e.layer.setMap(null), e.visible = !1, e.percent = 0, e.rangeOpacity = 0, p(), u(), $("#" + e.legendDivID).hide()) : "geeVector" !== e.layerType && "geoJSONVector" !== e.layerType ? (e.visible = !1, e.map.overlayMapTypes.setAt(e.layerId, null), e.percent = 0, u(), $("#" + e.legendDivID).hide(), e.rangeOpacity = 0, "tileMapService" !== e.layerType && "dynamicMapService" !== e.layerType && e.canQuery && (queryObj[t].visible = e.visible)) : (e.visible = !1, e.percent = 0, u(), $("#" + e.legendDivID).hide(), e.layer.setMap(null), e.rangeOpacity = 0, $("#" + i + "2").hide(), "geeVector" === e.layerType && e.canQuery && (queryObj[t].visible = e.visible)), e.viz.dashboardSummaryLayer && (Object.keys(e.dashboardSelectedFeatures).map((a => e.dashboardSelectedFeatures[a].polyList.map((e => e.setMap(null))))), updateDashboardCharts(), updateDashboardHighlights()), e.loading = !1, updateGEETileLayersDownloading(), $("#" + i + "2").hide(), $("#" + i + "3").hide(), g()) : (ga("send", "event", "layer-on", e.layerType, e.name), e.viz.isTimeLapse || turnOffTimeLapseCheckboxes(), "dynamicMapService" === e.layerType ? (e.layer.setMap(map), e.visible = !0, e.percent = 100, e.rangeOpacity = e.opacity, p(), u(), $("#" + e.legendDivID).show()) : "geeVector" !== e.layerType && "geoJSONVector" !== e.layerType ? (e.visible = !0, e.map.overlayMapTypes.setAt(e.layerId, e.layer), $("#" + e.legendDivID).show(), e.rangeOpacity = e.opacity, e.isTileMapService && (e.percent = 100, u()), e.layer.setOpacity(e.opacity), "tileMapService" !== e.layerType && "dynamicMapService" !== e.layerType && e.canQuery && (queryObj[t].visible = e.visible)) : (e.visible = !0, e.percent = 100, u(), $("#" + e.legendDivID).show(), e.layer.setMap(e.map), e.rangeOpacity = e.opacity, "geeVector" === e.layerType && e.canQuery && (queryObj[t].visible = e.visible)), e.viz.dashboardSummaryLayer && (Object.keys(e.dashboardSelectedFeatures).map((a => e.dashboardSelectedFeatures[a].polyList.map((e => e.setMap(map))))), "lcms-dashboard" === mode ? dashboardBoxSelect() : (updateDashboardCharts(), updateDashboardHighlights())), g()))
     }
 
-    function v() {
+    function f() {
         e.visible && $("#" + r).click()
     }
 
     function y() {
         e.visible || $("#" + r).click()
     }
     layerObj[a] = e, e.wasJittered = !1, e.loading = !1, e.refreshNumber = refreshNumber, e.visible && (c = "checked"), e.viz.isTimeLapse && (timeLapseObj[e.viz.timeLapseID].loadingLayerIDs.push(a), timeLapseObj[e.viz.timeLapseID].sliders.push(l), timeLapseObj[e.viz.timeLapseID].layerVisibleIDs.push(r)), $("#" + e.whichLayerList).prepend(`<li id = '${o}' aria-label="Map layer controls container for ${e.name}" class = 'layer-container'  title= '${e.helpBoxMessage}'>\n\t\t\t\t\t\t\t\t           <div id="${l}" aria-labelledby="${o}" Opacity range slider for ${e.name}" class = 'simple-layer-opacity-range'></div>\n\t\t\t\t\t\t\t\t           <input  role="option" id="${r}" aria-label="Layer visibility toggle checkbox for ${e.name}" type="checkbox" ${c}  />\n\t\t\t\t\t\t\t\t            <label class = 'layer-checkbox' id="${s}" aria-label="Layer visibility toggle checkbox for ${e.name}" style = 'margin-bottom:0px;display:none;'  for="${r}"></label>\n\t\t\t\t\t\t\t\t            <i id = "${i}" class="fa fa-spinner fa-spin layer-spinner" title='Waiting for layer service from Google Earth Engine'></i>\n\t\t\t\t\t\t\t\t            <i id = "${i}2" style = 'display:none;' class="fa fa-cog fa-spin layer-spinner" title='Waiting for map tiles from Google Earth Engine'></i>\n\t\t\t\t\t\t\t\t            <i id = "${i}3" style = 'display:none;' class="fa fa-cog fa-spin layer-spinner" title='Waiting for map tiles from Google Earth Engine'></i>\n                                            <i title = 'Click to clear all selected features from this layer' id='${d}' class="fa fa-eraser eraser" style="display:none;"></i>\n\t\t\t\t\t\t\t\t            <span id = '${n}' aria-labelledby="${o}" class = 'layer-span'>${e.name}</span>\n\t\t\t\t\t\t\t\t       </li>`), $("#" + l).slider({
@@ -1172,27 +1177,27 @@
         })), $("#" + i + "2").click((function() {
             $("#" + r).click()
         })), $("#" + n).dblclick((function() {
             m(), b = !0, m(), e.visible || $("#" + r).click(), setTimeout((function() {
                 b = !1
             }), 200)
         })), $("#" + r).change((function() {
-            f()
-        })), layerObj[a].visible = e.visible, layerObj[a].opacity = e.opacity, e.viz.isTimeLapse || $(".layer-checkbox").on("turnOffAll", (function() {
             v()
+        })), layerObj[a].visible = e.visible, layerObj[a].opacity = e.opacity, e.viz.isTimeLapse || $(".layer-checkbox").on("turnOffAll", (function() {
+            f()
         })), "geeVector" !== e.layerType && "geeVectorImage" !== e.layerType && "geoJSONVector" !== e.layerType || ($("#" + s).addClass("vector-layer-checkbox"), $(".vector-layer-checkbox").on("turnOffAll", (function() {
-            v()
+            f()
         })), $(".vector-layer-checkbox").on("turnOnAll", (function() {
             y()
         })), $(".vector-layer-checkbox").on("turnOffAllVectors", (function() {
-            v()
+            f()
         })), $(".vector-layer-checkbox").on("turnOnAllVectors", (function() {
             y()
         })), e.viz.isUploadedLayer && ($("#" + s).addClass("uploaded-layer-checkbox"), selectionTracker.uploadedLayerIndices.push(e.layerId), $(".vector-layer-checkbox").on("turnOffAllUploadedLayers", (function() {
-            v()
+            f()
         })), $(".vector-layer-checkbox").on("turnOnAllUploadedLayers", (function() {
             y()
         })))), "geeImage" === e.layerType || "geeVectorImage" === e.layerType || "geeImageCollection" === e.layerType) {
         if ("geeImageCollection" === e.layerType) {
             e.imageCollection = e.item, null !== e.viz.reducer && void 0 !== e.viz.reducer || (e.viz.reducer = ee.Reducer.lastNonNull());
             var w = ee.Image(e.item.first()).bandNames();
             e.item = ee.ImageCollection(e.item).reduce(e.viz.reducer).rename(w).copyProperties(e.imageCollection.first())
@@ -1202,34 +1207,34 @@
                     layerName: e.name,
                     filterList: [],
                     geoJSON: new google.maps.Data,
                     id: e.id,
                     rawGeoJSON: {},
                     selection: ee.FeatureCollection([])
                 }, $("#" + s).addClass("select-layer-checkbox"), $(".vector-layer-checkbox").on("turnOffAllSelectLayers", (function() {
-                    v()
+                    f()
                 })), $(".vector-layer-checkbox").on("turnOnAllSelectLayers", (function() {
                     y()
                 })), $(".vector-layer-checkbox").on("turnOffAll", (function() {
-                    v()
+                    f()
                 })), $(".vector-layer-checkbox").on("turnOnAll", (function() {
                     y()
                 }))), e.queryItem = e.item, "geeVectorImage" === e.layerType && (e.item = ee.Image().paint(e.item, null, e.viz.strokeWeight), e.viz.palette = e.viz.strokeColor), e.viz.isSelectLayer)
                 if (void 0 === e.viz.selectLayerNameProperty) e.queryItem.first().propertyNames().evaluate((function(a, t) {
                     void 0 !== t ? C = "system:index" : (a.map((function(e) {
                         -1 !== e.toLowerCase().indexOf("name") && (C = e)
                     })), void 0 === C && (C = "system:index")), selectedFeaturesJSON[e.name].fieldName = C, selectedFeaturesJSON[e.name].eeObject = e.queryItem.select([C], ["name"])
                 }));
                 else selectedFeaturesJSON[e.name].fieldName = e.viz.selectLayerNamePropertyname, selectedFeaturesJSON[e.name].eeObject = e.queryItem.select([e.viz.selectLayerNameProperty], ["name"]);
             e.viz.isSelectedLayer && ($("#" + s).addClass("selected-layer-checkbox"), $(".vector-layer-checkbox").on("turnOffAllSelectLayers", (function() {
-                v()
+                f()
             })), $(".vector-layer-checkbox").on("turnOnAllSelectLayers", (function() {
                 y()
             })), $(".vector-layer-checkbox").on("turnOffAllSelectedLayers", (function() {
-                v()
+                f()
             })), $(".vector-layer-checkbox").on("turnOnAllSelectedLayers", (function() {
                 y()
             })), selectionTracker.seletedFeatureLayerIndices.push(e.layerId))
         }
 
         function S() {
             var a = Object.values(layerObj).filter((function(a) {
@@ -1649,15 +1654,15 @@
                     }));
                 $("#summary-spinner").slideUp(), createHurricaneDamageWrapper(ee.FeatureCollection(n))
             }, e.readAsText(jQuery("#stormTrackUpload")[0].files[0])
         } else $("#summary-spinner").hide(), showMessage("No storm track provided", 'Please download storm track from <a href="https://www.wunderground.com/hurricane" target="_blank">here</a> . Copy and paste the storm track coordinates into a text editor. Save the table. Then upload that table above.')
     }
     canExport = !0, addCollapse("sidebar-left", "parameters-collapse-label", "parameters-collapse-div", "PARAMETERS", '<i role="img" class="fa fa-sliders mr-1" aria-hidden="true"></i>', !0, null, "Adjust parameters used to prepare storm outputs"), $("#parameters-collapse-div").append('\n    <label>Download storm track from <a href="https://www.wunderground.com/hurricane" target="_blank">here</a>. Copy and paste the storm track coordinates into a text editor. Save the table. Then upload that table below. <a href="./geojson/michael.txt" download="michael.txt" >Download test data here.</a></label>\n    <input class = \'file-input my-1\' type="file" id="stormTrackUpload" name="upload"  style="display: inline-block;" title = "Download storm track from https://www.wunderground.com/hurricane">\n    <hr>\n    <label>Provide name for storm (optional):</label>\n    <input title = \'Provide a name for the storm. The name of the provided storm track file will be used if left blank.\'  type="user-selected-area-name" class="form-control" id="storm-name"  placeholder="Name your storm!" style=\'width:80%;\'><hr>'), addRangeSlider("parameters-collapse-div", "Refinement iterations", "refinementIterations", 0, 10, 5, 1, "refinement-factor-slider", "null", "Specify number of iterations to perform a linear interpolation of provided track. A higher number is needed for tracks with fewer real observations"), addRangeSlider("parameters-collapse-div", "Max distance (km)", "maxDistance", 50, 500, 200, 50, "max-distance-slider", "null", "Specify max distance in km from storm track to include in output"), addRangeSlider("parameters-collapse-div", "Min wind (mph)", "minWind", 0, 75, 30, 5, "min-wind-slider", "null", "Specify min wind speed in mph to include in output"), $("#parameters-collapse-div").append('\n        <hr>\n        <label style = \'width:90%\'>The MOD of Rupture is intended to indicate how much force it takes to snap a tree. A single value can be provided by providing a constant image (e.g. ee.Image(1)) and a simple lookup to convert that image to a desired MOD of Rupture (e.g. {1:8500}). If different MOD of Rupture values are needed for different tree types, you can provide an EE image that may have tree classes or land cover classes that can then be cross-walked to a MOD of Rupture image with different values for different tree/land cover classes (e.g. ee.Image( "USGS/NLCD_RELEASES/2016_REL/2016" ).select([ 0 ]) with a lookup of {41:8500,42:2000,43:5000,90:4000}</label>\n        <hr>\n        <label>MOD of Rupture Image</label>\n        <textarea   title = \'Provide an image with relevant land cover/tree classes. Provide a constant raster (ee.Image(1)) if you would like to use a constant\'   class="form-control" id="mod-image"   oninput="auto_grow(this)" style=\'width:90%;\'>ee.Image("USGS/NLCD_RELEASES/2016_REL/2016").select([0])</textarea>\n        <hr>\n        <label>MOD of Rupture Lookup</label>\n        <textarea   title = \'Provide a lookup table to remap each class of the image provided above with a MOD of Rupture value.\'  type="user-selected-area-name" class="form-control" id="mod-lookup" oninput="auto_grow(this)" style=\'width:90%;\'>{41:8500, 42:2000, 43:5000, 90:4000}</textarea>\n       '), $("#parameters-collapse-div").append("<hr>\n      <button class = 'btn' style = 'margin-bottom: 0.5em!important;' onclick = 'ingestStormTrack()' title = 'Click to ingest storm track and map damage'>Ingest Storm Track</button>\n      <button class = 'btn' style = 'margin-bottom: 0.5em!important;' onclick = 'reRun()' title = 'Click to remove existing layers and exports'>Clear All Layers/Exports</button><br>"), addCollapse("sidebar-left", "layer-list-collapse-label", "layer-list-collapse-div", mode + " DATA", "<img style = 'width:1.1em;' class='image-icon mr-1' alt=\"Layers icon\" src=\"images/layer_icon.png\">", !0, null, mode + " DATA layers to view on map"), $("#layer-list-collapse-div").append('<ul id="layer-list" class = "layer-list"></ul>'), addCollapse("sidebar-left", "tools-collapse-label", "tools-collapse-div", "TOOLS", '<i role="img" class="fa fa-gear mr-1" aria-hidden="true"></i>', !1, "", "Tools to measure and chart data provided on the map"), addCollapse("sidebar-left", "download-collapse-label", "download-collapse-div", "DOWNLOAD DATA", '<i role="img" class="fa fa-cloud-download mr-1" aria-hidden="true"></i>', !1, "", "Download " + mode + " products for further analysis")
 } else "TreeMap" === mode ? (addCollapse("sidebar-left", "layer-list-collapse-label", "layer-list-collapse-div", "TreeMap DATA", "<img style = 'width:1.1em;' class='image-icon mr-1' alt=\"Layers icon\" src=\"images/layer_icon.png\">", !0, null, mode + " DATA layers to view on map"), addCollapse("sidebar-left", "tools-collapse-label", "tools-collapse-div", "TOOLS", '<i role="img" class="fa fa-gear mr-1" aria-hidden="true"></i>', !1, "", "Tools to measure and chart data provided on the map"), $("#layer-list-collapse-div").append('<ul id="layer-list" class = "layer-list"></ul>')) : (addCollapse("sidebar-left", "layer-list-collapse-label", "layer-list-collapse-div", "ANCILLARY DATA", "<img style = 'width:1.1em;' class='image-icon mr-1' alt=\"Layers icon\" src=\"images/layer_icon.png\">", !0, null, mode + " DATA layers to view on map"), addCollapse("sidebar-left", "reference-layer-list-collapse-label", "reference-layer-list-collapse-div", "PLOT DATA", "<img style = 'width:1.1em;' class='image-icon mr-1' alt=\"Layers icon\" src=\"images/layer_icon.png\">", !1, null, "Additional relevant layers to view on map intended to provide context for " + mode + " DATA"), addCollapse("sidebar-left", "tools-collapse-label", "tools-collapse-div", "TOOLS", '<i role="img" class="fa fa-gear mr-1" aria-hidden="true"></i>', !1, "", "Tools to measure and chart data provided on the map"), $("#layer-list-collapse-div").append('<ul id="layer-list" class = "layer-list"></ul>'), $("#reference-layer-list-collapse-div").append('<ul id="reference-layer-list" class = "layer-list"></ul>'), plotsOn = !0);
-if ($("body").append("<div class = 'legendDiv flexcroll col-sm-5 col-md-3 col-lg-3 col-xl-2 p-0 m-0' id = 'legendDiv'></div>"), $(".legendDiv").css("bottom", $(".bottombar").height()), $(".sidebar").css("max-height", $("body").height() - $(".bottombar").height()), addLegendCollapse(), addAccordianContainer("tools-collapse-div", "tools-accordian"), $("#tools-accordian").append("<h5 class = 'pt-2' style = 'border-top: 0.0em solid black;'>Measuring Tools</h5>"), addSubAccordianCard("tools-accordian", "measure-distance-label", "measure-distance-div", "Distance Measuring", staticTemplates.distanceDiv, !1, "toggleTool(toolFunctions.measuring.distance)", staticTemplates.distanceTipHover), addSubAccordianCard("tools-accordian", "measure-area-label", "measure-area-div", "Area Measuring", staticTemplates.areaDiv, !1, "toggleTool(toolFunctions.measuring.area)", staticTemplates.areaTipHover), addRadio("measure-distance-div", "metricOrImperialDistance-radio", "", "Imperial", "Metric", "metricOrImperialDistance", "imperial", "metric", "updateDistance()", "updateDistance()", "Toggle between imperial or metric units"), addRadio("measure-area-div", "metricOrImperialArea-radio", "", "Imperial", "Metric", "metricOrImperialArea", "imperial", "metric", "updateArea()", "updateArea()", "Toggle between imperial or metric units"), addShapeEditToolbar("measure-distance-div", "measure-distance-div-icon-bar", "undoDistanceMeasuring()", "resetPolyline()"), addColorPicker("measure-distance-div-icon-bar", "distance-color-picker", "updateDistanceColor", distancePolylineOptions.strokeColor), addShapeEditToolbar("measure-area-div", "measure-area-div-icon-bar", "undoAreaMeasuring()", "resetPolys()"), addColorPicker("measure-area-div-icon-bar", "area-color-picker", "updateAreaColor", areaPolygonOptions.strokeColor), $("#tools-accordian").append("<h5 class = 'pt-2' style = 'border-top: 0.1em solid black;'>Pixel Tools</h5>"), addSubAccordianCard("tools-accordian", "query-label", "query-div", "Query Visible Map Layers", staticTemplates.queryDiv, !1, "toggleTool(toolFunctions.pixel.query)", staticTemplates.queryTipHover), "Bloom-Mapper" !== mode && (addSubAccordianCard("tools-accordian", "pixel-chart-label", "pixel-chart-div", "Query " + mode + " Time Series", staticTemplates.pixelChartDiv, !1, "toggleTool(toolFunctions.pixel.chart)", staticTemplates.pixelChartTipHover), addDropdown("pixel-chart-div", "pixel-collection-dropdown", "Choose which " + mode + " time series to chart", "whichPixelChartCollection", "Choose which " + mode + " time series to chart.")), "geeViz" === mode) {
+if ($("body").append("<div class = 'legendDiv flexcroll col-sm-5 col-md-3 col-lg-3 col-xl-2 p-0 m-0' id = 'legendDiv'></div>"), $(".legendDiv").css("bottom", $(".bottombar").height()), $(".sidebar").css("max-height", $("body").height() - $(".bottombar").height()), addLegendCollapse(), addAccordianContainer("tools-collapse-div", "tools-accordian"), $("#tools-accordian").append("<h5 class = 'pt-2' style = 'border-top: 0.0em solid black;'>Measuring Tools</h5>"), addSubAccordianCard("tools-accordian", "measure-distance-label", "measure-distance-div", "Distance Measuring", staticTemplates.distanceDiv, !1, "toggleTool(toolFunctions.measuring.distance)", staticTemplates.distanceTipHover), addSubAccordianCard("tools-accordian", "measure-area-label", "measure-area-div", "Area Measuring", staticTemplates.areaDiv, !1, "toggleTool(toolFunctions.measuring.area)", staticTemplates.areaTipHover), addRadio("measure-distance-div", "metricOrImperialDistance-radio", "", "Imperial", "Metric", "metricOrImperialDistance", "imperial", "metric", "updateDistance()", "updateDistance()", "Toggle between imperial or metric units"), addRadio("measure-area-div", "metricOrImperialArea-radio", "", "Imperial", "Metric", "metricOrImperialArea", "imperial", "metric", "updateArea()", "updateArea()", "Toggle between imperial or metric units"), addShapeEditToolbar("measure-distance-div", "measure-distance-div-icon-bar", "undoDistanceMeasuring()", "resetPolyline()"), addColorPicker("measure-distance-div-icon-bar", "distance-color-picker", "updateDistanceColor", distancePolylineOptions.strokeColor), addShapeEditToolbar("measure-area-div", "measure-area-div-icon-bar", "undoAreaMeasuring()", "resetPolys()"), addColorPicker("measure-area-div-icon-bar", "area-color-picker", "updateAreaColor", areaPolygonOptions.strokeColor), $("#tools-accordian").append("<h5 class = 'pt-2' style = 'border-top: 0.1em solid black;'>Pixel Tools</h5>"), addSubAccordianCard("tools-accordian", "query-label", "query-div", "Query Visible Map Layers", staticTemplates.queryDiv, !1, "toggleTool(toolFunctions.pixel.query)", staticTemplates.queryTipHover), -1 === ["Bloom-Mapper", "TreeMap"].indexOf(mode) && (addSubAccordianCard("tools-accordian", "pixel-chart-label", "pixel-chart-div", "Query " + mode + " Time Series", staticTemplates.pixelChartDiv, !1, "toggleTool(toolFunctions.pixel.chart)", staticTemplates.pixelChartTipHover), addDropdown("pixel-chart-div", "pixel-collection-dropdown", "Choose which " + mode + " time series to chart", "whichPixelChartCollection", "Choose which " + mode + " time series to chart.")), "geeViz" === mode) {
     $("#pixel-chart-label").remove(), $("#share-button").remove(), $("#tools-accordian").append("<hr>");
     var tShowToolTipModal = !0;
     null !== localStorage.showToolTipModal && void 0 !== localStorage.showToolTipModal && (tShowToolTipModal = localStorage.showToolTipModal), addRadio("tools-accordian", "tooltip-radio", "Show tool tips", "Yes", "No", "localStorage.showToolTipModal", "true", "false", "", "", "Whether to show tool tips to help explain how to use the tools."), "false" === tShowToolTipModal && $("#tooltip-radio-second_toggle_label").click()
 }
 if ("LAMDA" === mode && $("#pixel-chart-label").remove(), "LCMS-pilot" === mode || "MTBS" === mode || "lcms-base-learner" === mode || "IDS" === mode || "LCMS" === mode) {
     if ($("#tools-accordian").append("<h5 class = 'pt-2' style = 'border-top: 0.1em solid black;'>Area Tools</h5>"), addSubCollapse("tools-accordian", "area-chart-params-label", "area-chart-params-div", "Area Tools Parameters", "", !1, ""), $("#area-chart-params-label").prop("title", "Click here to select which LCMS products to chart, and change which area units are used. "), addDropdown("area-chart-params-div", "area-collection-dropdown", "Choose which " + mode + " product to summarize", "whichAreaChartCollection", "Choose which " + mode + " time series to summarize."), $("#parameters-collapse-div").append("<hr>"), addMultiRadio("area-chart-params-div", "area-summary-format", "Area Units", "areaChartFormat", {
             Percentage: !0,
@@ -1676,15 +1681,15 @@
     function cacheCRS() {
         localStorage.export_crs = $("#export-crs").val()
     }
     $("#download-collapse-div").append(staticTemplates.exportContainer), void 0 !== localStorage.export_crs && null !== localStorage.export_crs && localStorage.export_crs.indexOf("EPSG") > -1 ? $("#export-crs").val(localStorage.export_crs) : localStorage.export_crs = $("#export-crs").val(), "STORM" === mode && ($("#export-area-drawing-div").append("<hr>\n                                            <button class = 'btn' onclick = 'addTrackBounds()' title = 'Add bounds of storm track for export area.'><i class=\"pr-1 fa fa-square-o\" aria-hidden=\"true\"></i> Use storm track bound as area to download</button>\n                                            "), $("#export-button-div").append("<hr>"), addRangeSlider("export-button-div", "Quick look spatial resolution", "quickLookRes", 1200, 6e3, 3e3, 300, "quick-look-res-slider", "null", "Specify spatial resolution for quick look downloads."), $("#export-button-div").append("<button class = 'btn' onclick = 'downloadQuickLooks()'  title = 'Quickly download outputs at coarse resolution'><i class=\"pr-1 fa fa-cloud-download\" aria-hidden=\"true\"></i>Download Quick Look Outputs</button>\n                                            "))
 }
 
 function resizeViewerPanes() {
-    "lcms-dashboard" !== mode && moveCollapse("legend-collapse"), $(".legendDiv").css("bottom", $(".bottombar").height()), $(".legendDiv").css("max-height", window.innerHeight - $(".bottombar").height()), $(".sidebar").css("max-height", $("body").height() - $(".bottombar").height()), walkThroughAdded && moveCollapse("walk-through-collapse")
+    "lcms-dashboard" !== mode && (moveCollapse("legend-collapse"), moveCollapse("chart-collapse")), $(".legendDiv").css("bottom", $(".bottombar").height()), $(".legendDiv").css("max-height", window.innerHeight - $(".bottombar").height()), $(".sidebar").css("max-height", $("body").height() - $(".bottombar").height()), walkThroughAdded && moveCollapse("walk-through-collapse")
 }
 
 function resizeDashboardPanes() {
     let e = $("#layer-list-collapse-label-layer-list-collapse-div").width(),
         a = $(".bottombar").height(),
         t = $("#dashboard-results-container").height(),
         o = $("#sidebar-left-container").height(),
@@ -2239,23 +2244,23 @@
                 Object.keys(a.classLegendDict).map((function(e) {
                     var o = {};
                     o.name = t, o.helpBoxMessage = n, o.classColor = a.classLegendDict[e], o.classStrokeColor = "999", o.classStrokeWeight = 1, o.className = e, addClassLegendEntry(h, o)
                 }))
             } else {
                 (y = {}).name = t, y.helpBoxMessage = n;
                 var g = a.strokeColor.slice(1),
-                    f = a.fillColor.slice(1);
+                    v = a.fillColor.slice(1);
                 3 === g.length && (g = g.split("").map((function(e) {
                     return e + e
-                })).join().replaceAll(",", "")), 3 === f.length && (f = f.split("").map((function(e) {
+                })).join().replaceAll(",", "")), 3 === v.length && (v = v.split("").map((function(e) {
                     return e + e
-                })).join().replaceAll(",", "")), y.classColor = f + Math.floor(a.fillOpacity / 2 * 255).toString(16), y.classStrokeColor = g + Math.floor(255 * a.strokeOpacity).toString(16), y.classStrokeWeight = a.strokeWeight + 1, y.className = "", addClassLegendEntry(h, y)
+                })).join().replaceAll(",", "")), y.classColor = v + Math.floor(a.fillOpacity / 2 * 255).toString(16), y.classStrokeColor = g + Math.floor(255 * a.strokeOpacity).toString(16), y.classStrokeWeight = a.strokeWeight + 1, y.className = "", addClassLegendEntry(h, y)
             }
-            var v = {};
-            v.name = t, v.helpBoxMessage = n
+            var f = {};
+            f.name = t, f.helpBoxMessage = n
         }
     } else {
         addLegendContainer(p, "legend-" + s, !1, n);
         var y = {};
         if (null !== a.legendTitle && void 0 !== a.legendTitle ? y.name = a.legendTitle : y.name = t, y.helpBoxMessage = n, null != a.palette) var b = a.palette;
         else b = "000,FFF";
         var w = b;
@@ -2440,16 +2445,27 @@
         clearDownloadDropdown()
     } catch (e) {}
     google.maps.event.clearListeners(mapDiv, "click"), setTimeout((function() {
         run(), "lcms-dashboard" !== mode && ($(".modal").modal("hide"), $(".modal-backdrop").remove()), setupAreaLayerSelection(), addLabelOverlay(), ("true" === urlParams.sankey || "true" === urlParams.beta) && urlParams.endYear - urlParams.startYear < 5 && showMessage("No Transition Charting", "The year range must be 5 years or more to perform transition charting")
     }), 1500)
 }
 
+function mulberry32(e) {
+    return function() {
+        var a = e += 1831565813;
+        return a = Math.imul(a ^ a >>> 15, 1 | a), (((a ^= a + Math.imul(a ^ a >>> 7, 61 | a)) ^ a >>> 14) >>> 0) / 4294967296
+    }
+}
+"false" === urlParams.addLayer && Object.keys(Map2).filter((e => e.indexOf("add") > -1)).map((e => {
+    Map2[e] = function() {}
+}));
+var randomN = mulberry32(1);
+
 function getRandomInt(e, a) {
-    return Math.floor(Math.random() * (a - e + 1)) + e
+    return Math.floor(randomN() * (a - e + 1)) + e
 }
 
 function padLeft(e, a, t) {
     return Array(a - String(e).length + 1).join(t || "0") + e
 }
 
 function rgbToHex(e, a, t) {
@@ -2494,17 +2510,14 @@
     return [getRandomInt(100, 225), getRandomInt(100, 225), getRandomInt(100, 225)]
 }
 
 function randomColors(e) {
     for (var a = []; e > 0;) a.push(randomColor()), e -= 1;
     return a
 }
-"false" === urlParams.addLayer && Object.keys(Map2).filter((e => e.indexOf("add") > -1)).map((e => {
-    Map2[e] = function() {}
-}));
 var colorList = ["#e6194b", "#3cb44b", "#ffe119", "#4363d8", "#f58231", "#911eb4", "#46f0f0", "#f032e6", "#bcf60c", "#fabebe", "#008080", "#e6beff", "#9a6324", "#fffac8", "#800000", "#aaffc3", "#808000", "#ffd8b1", "#000075", "#808080", "#ffffff", "#000000"],
     colorMod = colorList.length;
 
 function getColor() {
     var e = colorList[colorMod % colorList.length];
     return colorMod++, e
 }
@@ -3132,60 +3145,69 @@
 
 function clearQueryGeoJSON() {
     queryGeoJSON.forEach((function(e) {
         queryGeoJSON.remove(e)
     }))
 }
 $(document).ready(map_load);
-var getQueryImages = function(e, a) {
+var queryWindowMode = "infoWindow",
+    getQueryImages = function(e, a) {
         var t = [e, a];
-        $(".gm-ui-hover-effect").show(), $("#summary-spinner").slideDown(), infowindow.setMap(null), infowindow.setPosition({
-            lng: e,
-            lat: a
-        });
+        $(".gm-ui-hover-effect").show(), $("#summary-spinner").slideDown();
         var o = " Queried Values for Lng " + e.toFixed(3) + " Lat " + a.toFixed(3),
             l = `<div>\n\t\t\t\t\t\t\t<h6 style = 'font-weight:bold;'>Queried values for<br>lng: ${e.toFixed(3).toString()} lat: ${a.toFixed(3).toString()}</h6>\n\t\t\t\t\t\t\t<li id = 'query-list-container'></li>\n\t\t\t\t\t\t\t\n\t\t\t\t\t\t</div>`;
-        infowindow.setOptions({
+        "infoWindow" === queryWindowMode ? ($("#chart-collapse-label-chart-collapse-div").hide(), $("#chart-collapse-div").empty(), $("#legendDiv").css("max-width", ""), $("#legendDiv").css("max-height", "60%"), infowindow.setMap(null), infowindow.setPosition({
+            lng: e,
+            lat: a
+        }), infowindow.setOptions({
             maxWidth: 350
-        }), infowindow.setContent(l), infowindow.open(map);
+        }), infowindow.setContent(l), infowindow.open(map)) : (infowindow.setContent(""), infowindow.setMap(null), $("#legendDiv").css("max-width", ""), $("#legendDiv").css("max-height", "80%"), $("#chart-collapse-label-chart-collapse-div").show(), $("#chart-collapse-div").empty(), $("#chart-collapse-div").append(l));
         var r = 1;
 
         function n(e, a, t) {
             var l = t + "-container-" + r.toString();
             if (r++, $("#query-list-container").append("<table class=\"table table-hover bg-white\">\n\t\t\t\t\t\t\t\t\t\t\t\t<tbody>\n\t\t\t\t\t\t\t\t\t\t\t\t\t<tr class = 'bg-black'><th></th></tr>\n\t\t\t\t\t\t\t\t\t\t\t\t</tbody>\n\t\t\t\t\t\t\t\t\t\t\t  </table>"), null == e) $("#query-list-container").append(`<table class="table table-hover bg-white">\n\t\t\t\t\t\t\t\t\t\t\t\t<tbody id = '${l}'></tbody>\n\t\t\t\t\t\t\t\t\t\t\t  </table>`), $("#" + l).append(`<tr><th>${a.name}</th><th>NULL</th></tr>`);
-            else if ("geeImage" === a.type)
-                if ($("#query-list-container").append(`<table class="table table-hover bg-white">\n\t\t\t\t\t\t\t\t\t\t\t\t<tbody id = '${l}'></tbody>\n\t\t\t\t\t\t\t\t\t\t\t  </table>`), 1 === Object.keys(e).length) {
+            else if ("geeImage" === a.type) {
+                $("#query-list-container").append(`<table class="table table-hover bg-white">\n\t\t\t\t\t\t\t\t\t\t\t\t<tbody id = '${l}'></tbody>\n\t\t\t\t\t\t\t\t\t\t\t  </table>`);
+                let t = Object.keys(e);
+                if (1 === t.length) {
                     var n = JSON.stringify(Object.values(e)[0]);
                     null !== a.queryDict && void 0 !== a.queryDict && (n = a.queryDict[parseInt(n)]), $("#" + l).append(`<tr><th>${a.name}</th><td>${n}</td></tr>`)
+                } else if (4 === t.length && t.indexOf("viz-blue") > -1 && t.indexOf("viz-green") > -1 && t.indexOf("viz-red") > -1) {
+                    let o = t.filter((e => -1 === e.indexOf("viz-")))[0];
+                    n = JSON.stringify(e[o]);
+                    null !== a.queryDict && void 0 !== a.queryDict && (n = a.queryDict[parseInt(n)]), $("#" + l).append(`<tr><th>${a.name}</th><td>${n}</td></tr>`)
                 } else $("#" + l).append(`<tr><th>${a.name}</th><th>Multi band</th></tr>`), Object.keys(e).map((function(a) {
                     try {
                         var t = e[a];
                         null !== t && (t = t.toFixed(2).toString()), $("#" + l).append(`<tr><td>${a}</td><td>${t}</td></tr>`)
                     } catch (e) {
                         $("#" + l).append(`<tr><td>${a}</td><td>${JSON.stringify(t)}</td></tr>`)
                     }
-                }));
-            else if ("geeImageCollection" === a.type) {
-                $("#query-list-container").append("<ul class = 'bg-black dropdown-divider'></ul>"), $("#query-list-container").append(`<ul class = 'm-0 p-0 bg-white' id = '${l}'></ul>`), infowindow.setOptions({
+                }))
+            } else if ("geeImageCollection" === a.type) {
+                $("#query-list-container").append("<ul class = 'bg-black dropdown-divider'></ul>"), $("#query-list-container").append(`<ul class = 'm-0 p-0 bg-white' id = '${l}'></ul>`);
+                let t = 600;
+                "infoWindow" === queryWindowMode ? (infowindow.setOptions({
                     maxWidth: 1200
-                }), infowindow.open(map);
+                }), infowindow.open(map)) : ($("#legendDiv").css("max-width", "575px"), t = 550);
                 var s = {
                         plot_bgcolor: "#D6D1CA",
                         paper_bgcolor: "#D6D1CA",
                         font: {
                             family: "Roboto Condensed, sans-serif"
                         },
                         margin: {
                             l: 50,
                             r: 10,
                             b: 80,
                             t: 80,
                             pad: 0
                         },
-                        width: 600,
+                        width: t,
                         height: 400,
                         title: {
                             text: a.name
                         },
                         xaxis: {
                             tickangle: 45,
                             tickfont: {
@@ -3200,15 +3222,15 @@
                         toImageButtonOptions: {
                             filename: a.name + o,
                             width: 1200,
                             height: 800,
                             format: "png"
                         }
                     };
-                console.log(e.table), Plotly.newPlot(l, e.table, s, i)
+                Plotly.newPlot(l, e.table, s, i)
             } else if ("geeVectorImage" === a.type || "geeVector" === a.type) {
                 $("#query-list-container").append(`<table class="table table-hover bg-white">\n\t\t\t\t\t\t\t\t\t\t\t\t<tbody id = '${l}'></tbody>\n\t\t\t\t\t\t\t\t\t\t\t  </table>`);
                 var p = Object.keys(e);
                 $("#" + l).append(`<tr><th>${a.name}</th><th>Attribute Table</th></tr>`), p.map((function(a) {
                     var t = e[a];
                     $("#" + l).append(`<tr><th>${a}</th><td>${t}</td></tr>`)
                 }))
@@ -3483,24 +3505,24 @@
                         };
                     let d, c = [],
                         p = [],
                         u = [],
                         m = {},
                         h = 0,
                         g = [],
-                        f = {};
+                        v = {};
                     Object.keys(t).map((e => g.push(e.split("---")[0].split("--")[0], e.split("---")[1].split("--")[0]))), Object.keys(t).map((e => u.push(e.split("---")[0].split("--")[1], e.split("---")[1].split("--")[1]))), g = unique(g), u = unique(u).map((e => parseInt(e))).sort(((e, a) => e - a)), g.map((e => {
                         areaChartCollections[whichAreaChartCollection].names.map((a => {
                             const t = e + " " + a;
                             p.push(t), m[t] = h, h++
                         })), areaChartCollections[whichAreaChartCollection].colors.map((e => {
                             c.push(e)
                         }))
                     })), d = "Percentage" === areaChartFormat ? 1 / s * 100 : chartFormatDict[areaChartFormat].mult;
-                    let v = [],
+                    let f = [],
                         y = 1;
 
                     function r(e, t = 20, o = 25, l = 10) {
                         i.hovertemplate = "%{value}" + chartFormatDict[areaChartFormat].label + " %{source.label}-%{target.label}<extra></extra>";
                         var r = [r = {
                                 type: "sankey",
                                 orientation: "h",
@@ -3546,36 +3568,36 @@
                         return Plotly.newPlot(e, r, n, s)
                     }
                     g.slice(0, g.length - 1).map((e => {
                         let a = e,
                             o = g[y];
                         y++;
                         let l = [""];
-                        u.map((e => l.push(o + " " + areaChartCollections[whichAreaChartCollection].names[e - 1]))), v.push(l), u.map((e => {
+                        u.map((e => l.push(o + " " + areaChartCollections[whichAreaChartCollection].names[e - 1]))), f.push(l), u.map((e => {
                             let l = [a + " " + areaChartCollections[whichAreaChartCollection].names[e - 1]];
                             u.map((r => {
                                 let n = t[`${a}--${e}---${o}--${r}`][1][1] * d;
                                 l.push(n)
-                            })), v.push(l)
-                        })), v.push([""])
-                    })), v = v.slice(0, v.length - 1), dataTable = v, Object.keys(t).map((e => {
+                            })), f.push(l)
+                        })), f.push([""])
+                    })), f = f.slice(0, f.length - 1), dataTable = f, Object.keys(t).map((e => {
                         const a = e.split("---")[0].split("--")[0],
                             o = e.split("---")[1].split("--")[0],
                             l = parseInt(e.split("---")[0].split("--")[1]) - 1,
                             r = parseInt(e.split("---")[1].split("--")[1]) - 1,
                             n = areaChartCollections[whichAreaChartCollection].names[l],
                             s = areaChartCollections[whichAreaChartCollection].names[r],
                             c = t[e][1][1] * d,
                             p = a + " " + n,
                             u = o + " " + s;
-                        f[e] = c, i.source.push(m[p]), i.target.push(m[u]), i.value.push(c)
+                        v[e] = c, i.source.push(m[p]), i.target.push(m[u]), i.value.push(c)
                     })), configChartModal("Plotly"), r("chart-canvas", thickness = 20, nodePad = 25, fontSize = 10), plotlyDownloadChartObject = r("chart-download-canvas", thickness = 40, nodePad = 20, fontSize = 20), $("#chart-download-dropdown").empty(), $("#chart-modal-footer").append(`<div class="dropdown">\n\t\t\t\t\t\t\t\t\t\t\t\t<div class=" dropdown-toggle"  id="chartDownloadDropdown" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">\n\t\t\t\t\t\t\t\t\t\t\t\t\tDownload\n\t\t\t\t\t\t\t\t\t\t\t\t</div>\n\t\t\t\t\t\t\t\t\t\t\t\t<div id = 'chart-download-dropdown' class="dropdown-menu px-2" aria-labelledby="chartDownloadDropdown">\n\t\t\t\t\t\t\t\t\t\t\t\t\t<a class="dropdown-item" href="#" onclick = "downloadPlotly(plotlyDownloadChartObject,'${a}.png')">PNG</a>\n\t\t\t\t\t\t\t\t\t\t\t\t\t<a class="dropdown-item" href="#" onclick = "exportToCsv('${a}.csv', dataTable)">CSV</a>\n\t\t\t\t\t\t\t\t\t\t\t\t</div>\n\t\t\t\t\t\t\t\t\t\t\t\t</div>\n\t\t\t\t\t\t\t\t\t\t\t\t\n\t\t\t\t\t\t\t\t\t\t\t\t</div>\n\t\t\t\t\t\t\t\t\t\t\t\t<div class="dropdown">\n\t\t\t\t\t\t\t\t\t\t\t\t<div class=" dropdown-toggle"  id="chartTypeDropdown" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">\n\t\t\t\t\t\t\t\t\t\t\t\t\tChart Type\n\t\t\t\t\t\t\t\t\t\t\t\t</div>\n\t\t\t\t\t\t\t\t\t\t\t\t<div id = 'chart-type-dropdown' class="dropdown-menu px-2" aria-labelledby="chartTypeDropdown">\n\t\t\t\t\t\t\t\t\t\t\t\t\t<a class="dropdown-item" href="#" onclick = "toggleChartTable('chart');">Sankey Chart</a>\n\t\t\t\t\t\t\t\t\t\t\t\t\t<a class="dropdown-item" href="#" onclick = "toggleChartTable('table')">Table</a>\n\t\t\t\t\t\t\t\t\t\t\t\t</div>\n\t\t\t\t\t\t\t\t\t\t\t\t</div>\n\t\t\t\t\t\t\t\t\t\t\t\t\n\t\t\t\t\t\t\t\t\t\t\t\t`);
                     var n = htmlTable(dataTable);
                     $("#chart-table").append(n), toggleChartTable(localStorage.tableOrChart), e.evaluate((function(e, t) {
-                        areaGeoJson = e, areaGeoJson.properties = f, void 0 === t && null != areaGeoJson ? $("#chart-download-dropdown").append(`<a class="dropdown-item" href="#" onclick = "exportJSON('${a}.geojson', areaGeoJson)">geoJSON</a>`) : showMessage("Error", "Could not convert summary area to geoJSON " + t)
+                        areaGeoJson = e, areaGeoJson.properties = v, void 0 === t && null != areaGeoJson ? $("#chart-download-dropdown").append(`<a class="dropdown-item" href="#" onclick = "exportJSON('${a}.geojson', areaGeoJson)">geoJSON</a>`) : showMessage("Error", "Could not convert summary area to geoJSON " + t)
                     })), ga("send", "event", mode, "sankeyAreaChart", whichAreaChartCollection), $("#chart-modal").modal()
                 }
                 $("#summary-spinner").slideUp()
             }))
         } else $("#summary-spinner").slideUp()
     } else {
         var l = areaChartCollections[whichAreaChartCollection].collection,
@@ -3588,30 +3610,28 @@
         ["Acres", "Hectares"].indexOf(areaChartFormat) > -1 ? multiplier = d.multiply(areaChartFormatDict[areaChartFormat].mult) : multiplier = areaChartFormatDict[areaChartFormat].mult;
         var c = ee.Image(l.first()).bandNames().getInfo();
         (c = c.map((function(e) {
             return e.replaceAll("_", " ") + " " + areaChartFormatDict[areaChartFormat].label
         }))).unshift(r);
         var p = getAreaSummaryTable(l, e, r, multiplier, i, crs, transform, scale),
             u = 0,
-            m = 60,
-            h = 1e4,
-            g = new Date;
+            m = new Date;
         ! function t() {
             console.log("Evaluating area chart tables"), p.evaluate((function(l, r) {
                 print(u), print(l), print(r), print(areaChartingCount);
-                var i = new Date - g;
-                if (console.log("dt: " + i.toString()), void 0 !== r && u < m && currentChartID === o && i < h) t();
+                var i = new Date - m;
+                if (console.log("dt: " + i.toString()), void 0 !== r && u < 60 && currentChartID === o && i < 1e4) t();
                 else if (void 0 === r && currentChartID === o) {
                     l.unshift(c), $("#summary-spinner").slideUp();
                     var d = areaChartCollections[whichAreaChartCollection].stacked,
                         p = areaChartCollections[whichAreaChartCollection].steppedLine,
-                        f = areaChartCollections[whichAreaChartCollection].colors,
-                        v = areaChartCollections[whichAreaChartCollection].chartType,
-                        y = areaChartCollections[whichAreaChartCollection].fieldsHidden;
-                    null == v && (v = "line"), ga("send", "event", mode, "areaChart", whichAreaChartCollection), addChartJS(l, a, v, d, p, f, n, s, y), e.evaluate((function(e, t) {
+                        h = areaChartCollections[whichAreaChartCollection].colors,
+                        g = areaChartCollections[whichAreaChartCollection].chartType,
+                        v = areaChartCollections[whichAreaChartCollection].fieldsHidden;
+                    null == g && (g = "line"), ga("send", "event", mode, "areaChart", whichAreaChartCollection), addChartJS(l, a, g, d, p, h, n, s, v), e.evaluate((function(e, t) {
                         areaGeoJson = e, areaGeoJson[a] = l, void 0 === t && null != areaGeoJson ? $("#chart-download-dropdown").append(`<a class="dropdown-item" href="#" onclick = "exportJSON('${a}.geojson', areaGeoJson)">geoJSON</a>`) : showMessage("Error", "Could not convert summary area to geoJSON " + t)
                     })), areaChartingCount--
                 } else void 0 !== r && ($("#summary-spinner").slideUp(), (r.indexOf("Dictionary.toArray: Unable to convert dictionary to array") > -1 || r.indexOf("Array: Parameter 'values' is required.") > -1) && (r = "Most likely selected area does not overlap with selected LCMS study area<br>Please select area that overlaps with products<br>Raw Error Message:<br>" + r), showMessage('<i class="text-dark text-uppercase fa fa-exclamation-triangle"></i> Error! Try again', r));
                 u++
             }))
         }()
     }
@@ -3717,15 +3737,15 @@
     try {
         mapHammer.destroy(), map.setOptions({
             draggableCursor: "hand"
         }), map.setOptions({
             cursor: "hand"
         }), google.maps.event.clearListeners(mapDiv, "dblclick"), map.setOptions({
             cursor: "hand"
-        }), infowindow.setMap(null), marker.setMap(null)
+        }), infowindow.setMap(null), marker.setMap(null), $("#legendDiv").css("max-width", ""), $("#chart-collapse-div").empty(), $("#chart-collapse-label-chart-collapse-div").hide()
     } catch (e) {}
 }
 
 function getImageCollectionValuesForCharting(e) {
     var a = ee.ImageCollection(chartCollection.filterBounds(e));
     try {
         var t = a.getRegion(e, null, "EPSG:5070", [30, 0, -2361915, 0, -30, 3177735]).evaluate();
```

### Comparing `geeViz-2023.3.1/geeViz/geeView/js/load.min.js` & `geeViz-2023.4.1/geeViz/geeView/js/load.min.js`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/geeView.py` & `geeViz-2023.4.1/geeViz/geeView.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,15 @@
         self.port = port
         self.layerNumber = 1
         self.idDictList = []
         self.mapCommandList  = []
         self.ee_run_name = 'runGeeViz'
         self.refreshTokenPath = ee.oauth.get_credentials_path()
         self.serviceKeyPath = None
+        self.queryWindowMode = 'sidePane'
         
     #Function for adding a layer to the map
     def addLayer(self,image,viz = {},name= None,visible= True):
         if name == None:
             name = 'Layer '+str(self.layerNumber)
             self.layerNumber+=1
         print('Adding layer: ' +name)
@@ -200,15 +201,18 @@
             lines += t
         lines += 'if(layerLoadErrorMessages.length>0){showMessage("Map.addLayer Error List",layerLoadErrorMessages.join("<br>"));}\n'
         lines += "setTimeout(function(){if(layerLoadErrorMessages.length===0){$('#close-modal-button').click();}}, 2500);\n"
 
         #Iterate across each map command
         for mapCommand in self.mapCommandList:
             lines += mapCommand + '\n'
-
+        
+        # Set location of query outputs
+        lines += 'queryWindowMode = "{}"\n'.format(self.queryWindowMode)
+        
         lines+= "}"
         
         #Write out js file
         self.ee_run = os.path.join(ee_run_dir, '{}.js'.format(self.ee_run_name))
         oo = open(self.ee_run,'w')
         oo.writelines(lines)
         oo.close()
@@ -242,29 +246,37 @@
     def setQueryCRS(self,crs):
         print('Setting click query crs to: {}'.format(crs))
         cmd = "crs='{}'".format(crs)
         if cmd not in self.mapCommandList:
             self.mapCommandList.append(cmd)
     def setQueryScale(self,scale):
         print('Setting click query scale to: {}'.format(scale))
-        cmd = "tansform=null;scale={}".format(scale)
+        cmd = "tansform=null;scale={};plotRadius={}".format(scale,scale/2.)
         if cmd not in self.mapCommandList:
             self.mapCommandList.append(cmd)
     def setQueryTransform(self,transform):
         print('Setting click query transform to: {}'.format(transform))
-        cmd = "scale=null;transform={}".format(transform)
+        cmd = "scale=null;transform={};plotRadius={}".format(transform,transform[0]/2.)
         if cmd not in self.mapCommandList:
             self.mapCommandList.append(cmd)
     def setQueryBoxColor(self,color):
         if color[0] != '#':color = '#{}'.format(color)
         print('Setting click query box color to: {}'.format(color))
         cmd = "clickBoundsColor='{}'".format(color)
         if cmd not in self.mapCommandList:
             self.mapCommandList.append(cmd)
-
+    # Functions to handle location of query outputs
+    def setQueryWindowMode(self,mode):
+        self.queryWindowMode = mode
+    def setQueryToInfoWindow(self):
+        self.setQueryWindowMode('infoWindow')
+    def setQueryToSidePane(self):
+        self.setQueryWindowMode('sidePane')
+    
+    # Turn on query inspector 
     def turnOnInspector(self):
         # self.mapCommandList.append("$('#tools-collapse-div').addClass('show')")
         query_command = "$('#query-label').click();"
         if query_command not in self.mapCommandList:
             self.mapCommandList.append(query_command)
         
     def turnOffAllLayers(self):
```

### Comparing `geeViz-2023.3.1/geeViz/getImagesLib.py` & `geeViz-2023.4.1/geeViz/getImagesLib.py`

 * *Files 0% similar despite different names*

```diff
@@ -5702,50 +5702,50 @@
 00016450: 6c61 725a 656e 6974 6827 2c20 2756 6965  larZenith', 'Vie
 00016460: 775a 656e 6974 6827 2c20 2752 656c 6174  wZenith', 'Relat
 00016470: 6976 6541 7a69 6d75 7468 275d 0d0a 2344  iveAzimuth']..#D
 00016480: 6963 7469 6f6e 6172 7920 6f66 204d 4f44  ictionary of MOD
 00016490: 4953 2063 6f6c 6c65 6374 696f 6e73 0d0a  IS collections..
 000164a0: 6d6f 6469 7343 4469 6374 203d 207b 5c0d  modisCDict = {\.
 000164b0: 0a20 2027 6569 6768 7444 6179 4e44 5649  .  'eightDayNDVI
-000164c0: 4127 203a 2027 4d4f 4449 532f 3030 362f  A' : 'MODIS/006/
+000164c0: 4127 203a 2027 4d4f 4449 532f 3036 312f  A' : 'MODIS/061/
 000164d0: 4d59 4431 3351 3127 2c5c 0d0a 2020 2765  MYD13Q1',\..  'e
 000164e0: 6967 6874 4461 794e 4456 4954 2720 3a20  ightDayNDVIT' : 
-000164f0: 274d 4f44 4953 2f30 3036 2f4d 4f44 3133  'MODIS/006/MOD13
+000164f0: 274d 4f44 4953 2f30 3631 2f4d 4f44 3133  'MODIS/061/MOD13
 00016500: 5131 272c 5c0d 0a20 2027 6569 6768 7444  Q1',\..  'eightD
 00016510: 6179 5352 3235 3041 2720 3a20 274d 4f44  aySR250A' : 'MOD
-00016520: 4953 2f30 3036 2f4d 5944 3039 5131 272c  IS/006/MYD09Q1',
+00016520: 4953 2f30 3631 2f4d 5944 3039 5131 272c  IS/061/MYD09Q1',
 00016530: 5c0d 0a20 2027 6569 6768 7444 6179 5352  \..  'eightDaySR
 00016540: 3235 3054 2720 3a20 274d 4f44 4953 2f30  250T' : 'MODIS/0
-00016550: 3036 2f4d 4f44 3039 5131 272c 5c0d 0a20  06/MOD09Q1',\.. 
+00016550: 3631 2f4d 4f44 3039 5131 272c 5c0d 0a20  61/MOD09Q1',\.. 
 00016560: 2027 6569 6768 7444 6179 5352 3530 3041   'eightDaySR500A
-00016570: 2720 3a20 274d 4f44 4953 2f30 3036 2f4d  ' : 'MODIS/006/M
+00016570: 2720 3a20 274d 4f44 4953 2f30 3631 2f4d  ' : 'MODIS/061/M
 00016580: 5944 3039 4131 272c 5c0d 0a20 2027 6569  YD09A1',\..  'ei
 00016590: 6768 7444 6179 5352 3530 3054 2720 3a20  ghtDaySR500T' : 
-000165a0: 274d 4f44 4953 2f30 3036 2f4d 4f44 3039  'MODIS/006/MOD09
+000165a0: 274d 4f44 4953 2f30 3631 2f4d 4f44 3039  'MODIS/061/MOD09
 000165b0: 4131 272c 5c0d 0a20 2027 6569 6768 7444  A1',\..  'eightD
 000165c0: 6179 4c53 5431 3030 3041 2720 3a20 274d  ayLST1000A' : 'M
-000165d0: 4f44 4953 2f30 3036 2f4d 5944 3131 4132  ODIS/006/MYD11A2
+000165d0: 4f44 4953 2f30 3631 2f4d 5944 3131 4132  ODIS/061/MYD11A2
 000165e0: 272c 5c0d 0a20 2027 6569 6768 7444 6179  ',\..  'eightDay
 000165f0: 4c53 5431 3030 3054 2720 3a20 274d 4f44  LST1000T' : 'MOD
-00016600: 4953 2f30 3036 2f4d 4f44 3131 4132 272c  IS/006/MOD11A2',
+00016600: 4953 2f30 3631 2f4d 4f44 3131 4132 272c  IS/061/MOD11A2',
 00016610: 5c0d 0a20 2027 6461 696c 7953 5232 3530  \..  'dailySR250
-00016620: 4127 203a 2027 4d4f 4449 532f 3030 362f  A' : 'MODIS/006/
+00016620: 4127 203a 2027 4d4f 4449 532f 3036 312f  A' : 'MODIS/061/
 00016630: 4d59 4430 3947 5127 2c5c 0d0a 2020 2764  MYD09GQ',\..  'd
 00016640: 6169 6c79 5352 3235 3054 2720 3a20 274d  ailySR250T' : 'M
-00016650: 4f44 4953 2f30 3036 2f4d 4f44 3039 4751  ODIS/006/MOD09GQ
+00016650: 4f44 4953 2f30 3631 2f4d 4f44 3039 4751  ODIS/061/MOD09GQ
 00016660: 272c 5c0d 0a20 2027 6461 696c 7953 5235  ',\..  'dailySR5
-00016670: 3030 4127 203a 2027 4d4f 4449 532f 3030  00A' : 'MODIS/00
-00016680: 362f 4d59 4430 3947 4127 2c5c 0d0a 2020  6/MYD09GA',\..  
+00016670: 3030 4127 203a 2027 4d4f 4449 532f 3036  00A' : 'MODIS/06
+00016680: 312f 4d59 4430 3947 4127 2c5c 0d0a 2020  1/MYD09GA',\..  
 00016690: 2764 6169 6c79 5352 3530 3054 2720 3a20  'dailySR500T' : 
-000166a0: 274d 4f44 4953 2f30 3036 2f4d 4f44 3039  'MODIS/006/MOD09
+000166a0: 274d 4f44 4953 2f30 3631 2f4d 4f44 3039  'MODIS/061/MOD09
 000166b0: 4741 272c 5c0d 0a20 2027 6461 696c 794c  GA',\..  'dailyL
 000166c0: 5354 3130 3030 4127 203a 2027 4d4f 4449  ST1000A' : 'MODI
-000166d0: 532f 3030 362f 4d59 4431 3141 3127 2c5c  S/006/MYD11A1',\
+000166d0: 532f 3036 312f 4d59 4431 3141 3127 2c5c  S/061/MYD11A1',\
 000166e0: 0d0a 2020 2764 6169 6c79 4c53 5431 3030  ..  'dailyLST100
-000166f0: 3054 2720 3a20 274d 4f44 4953 2f30 3036  0T' : 'MODIS/006
+000166f0: 3054 2720 3a20 274d 4f44 4953 2f30 3631  0T' : 'MODIS/061
 00016700: 2f4d 4f44 3131 4131 275c 0d0a 7d0d 0a6d  /MOD11A1'\..}..m
 00016710: 756c 744d 6f64 6973 4469 6374 203d 207b  ultModisDict = {
 00016720: 5c0d 0a20 2020 2027 7465 6d70 4e6f 416e  \..    'tempNoAn
 00016730: 676c 6544 6169 6c79 273a 205b 6565 2e49  gleDaily': [ee.I
 00016740: 6d61 6765 285b 302e 3030 3031 2c30 2e30  mage([0.0001,0.0
 00016750: 3030 312c 302e 3030 3031 2c30 2e30 3030  001,0.0001,0.000
 00016760: 312c 302e 3030 3031 2c30 2e30 3030 312c  1,0.0001,0.0001,
```

### Comparing `geeViz-2023.3.1/geeViz/migrateGEEAssets.py` & `geeViz-2023.4.1/geeViz/migrateGEEAssets.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/phEEnoViz.py` & `geeViz-2023.4.1/geeViz/phEEnoViz.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz/taskManagerLib.py` & `geeViz-2023.4.1/geeViz/taskManagerLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/geeViz.egg-info/PKG-INFO` & `geeViz-2023.4.1/geeViz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geeViz
-Version: 2023.3.1
+Version: 2023.4.1
 Summary: A package to help with GEE data processing, analysis, and visualization
 Home-page: https://github.com/gee-community/geeViz
 Author: Ian Housman
 Author-email: ian.housman@gmail.com
 License: Apache
 Keywords: earthengine google remote sensing landsat sentinel modis forestry forest
 Classifier: Programming Language :: Python :: 2
```

### Comparing `geeViz-2023.3.1/geeViz.egg-info/SOURCES.txt` & `geeViz-2023.4.1/geeViz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geeViz-2023.3.1/setup.py` & `geeViz-2023.4.1/setup.py`

 * *Files identical despite different names*

