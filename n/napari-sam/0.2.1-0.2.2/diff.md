# Comparing `tmp/napari-sam-0.2.1.tar.gz` & `tmp/napari-sam-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-sam-0.2.1.tar", last modified: Mon Apr 10 09:47:07 2023, max compression
+gzip compressed data, was "napari-sam-0.2.2.tar", last modified: Mon Apr 10 09:51:55 2023, max compression
```

## Comparing `napari-sam-0.2.1.tar` & `napari-sam-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:47:07.761876 napari-sam-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-10 09:46:52.000000 napari-sam-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-10 09:46:52.000000 napari-sam-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-10 09:47:07.761876 napari-sam-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-04-10 09:46:52.000000 napari-sam-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-10 09:46:52.000000 napari-sam-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-10 09:47:07.761876 napari-sam-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:47:07.757876 napari-sam-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:47:07.757876 napari-sam-0.2.1/src/napari_sam/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-10 09:46:52.000000 napari-sam-0.2.1/src/napari_sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26966 2023-04-10 09:46:52.000000 napari-sam-0.2.1/src/napari_sam/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-10 09:46:52.000000 napari-sam-0.2.1/src/napari_sam/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-10 09:46:52.000000 napari-sam-0.2.1/src/napari_sam/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:47:07.761876 napari-sam-0.2.1/src/napari_sam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-10 09:47:07.000000 napari-sam-0.2.1/src/napari_sam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-10 09:47:07.000000 napari-sam-0.2.1/src/napari_sam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 09:47:07.000000 napari-sam-0.2.1/src/napari_sam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-10 09:47:07.000000 napari-sam-0.2.1/src/napari_sam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-10 09:47:07.000000 napari-sam-0.2.1/src/napari_sam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-10 09:47:07.000000 napari-sam-0.2.1/src/napari_sam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:51:55.227294 napari-sam-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-10 09:51:34.000000 napari-sam-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-10 09:51:34.000000 napari-sam-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-10 09:51:55.227294 napari-sam-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-10 09:51:34.000000 napari-sam-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-10 09:51:34.000000 napari-sam-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-10 09:51:55.227294 napari-sam-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:51:55.223294 napari-sam-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:51:55.227294 napari-sam-0.2.2/src/napari_sam/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-10 09:51:34.000000 napari-sam-0.2.2/src/napari_sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26966 2023-04-10 09:51:34.000000 napari-sam-0.2.2/src/napari_sam/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-10 09:51:34.000000 napari-sam-0.2.2/src/napari_sam/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-10 09:51:34.000000 napari-sam-0.2.2/src/napari_sam/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:51:55.227294 napari-sam-0.2.2/src/napari_sam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-10 09:51:55.000000 napari-sam-0.2.2/src/napari_sam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-10 09:51:55.000000 napari-sam-0.2.2/src/napari_sam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 09:51:55.000000 napari-sam-0.2.2/src/napari_sam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-10 09:51:55.000000 napari-sam-0.2.2/src/napari_sam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-10 09:51:55.000000 napari-sam-0.2.2/src/napari_sam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-10 09:51:55.000000 napari-sam-0.2.2/src/napari_sam.egg-info/top_level.txt
```

### Comparing `napari-sam-0.2.1/LICENSE` & `napari-sam-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-sam-0.2.1/PKG-INFO` & `napari-sam-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.2.1
+Version: 0.2.2
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
@@ -36,15 +36,15 @@
 [![codecov](https://codecov.io/gh/MIC-DKFZ/napari-sam/branch/main/graph/badge.svg)](https://codecov.io/gh/MIC-DKFZ/napari-sam)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-sam)](https://napari-hub.org/plugins/napari-sam)
 
 Segment anything with Meta AI's new SAM model with thi Napari plugin!
 
 SAM is the new segmentation system from Meta AI capable of **one-click segmentation of any object** and now our plugin neatly integrates this into Napari.
 
-We already **extended** SAMs click-based foreground separation to full **click-based semantic segmentation & instance segmentation** will soon follow!
+We already **extended** SAMs click-based foreground separation to full **click-based semantic segmentation & instance segmentation**!
 
 ----------------------------------
 
 Everything mode             |  Click-based semantic segmentation mode |  Click-based instance segmentation mode
 :-------------------------:|:-------------------------:|:-------------------------:
 ![](cats_everything.png)  |  ![](cats_semantic.png)  |  ![](cats_instance.png)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-sam Version: 0.2.1 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.2.2 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
@@ -25,19 +25,19 @@
 badge.svg)](https://codecov.io/gh/MIC-DKFZ/napari-sam) [![napari hub](https://
 img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-sam)]
 (https://napari-hub.org/plugins/napari-sam) Segment anything with Meta AI's new
 SAM model with thi Napari plugin! SAM is the new segmentation system from Meta
 AI capable of **one-click segmentation of any object** and now our plugin
 neatly integrates this into Napari. We already **extended** SAMs click-based
 foreground separation to full **click-based semantic segmentation & instance
-segmentation** will soon follow! ---------------------------------- Everything
-mode | Click-based semantic segmentation mode | Click-based instance
-segmentation mode :-------------------------:|:-------------------------:|:----
----------------------: ![](cats_everything.png) | ![](cats_semantic.png) | ![]
-(cats_instance.png) ----------------------------------
+segmentation**! ---------------------------------- Everything mode | Click-
+based semantic segmentation mode | Click-based instance segmentation mode :----
+---------------------:|:-------------------------:|:-------------------------:
+![](cats_everything.png) | ![](cats_semantic.png) | ![](cats_instance.png) ----
+------------------------------
                         ***** SAM in Napari demo *****
                             Click to play the video
                                   [SAM_Demo]
 ---------------------------------- ## Installation The plugin requires
 `python>=3.8`, as well as `pytorch>=1.7` and `torchvision>=0.8`. Please follow
 the instructions here to install both PyTorch and TorchVision dependencies.
 Installing both PyTorch and TorchVision with CUDA support is strongly
```

### Comparing `napari-sam-0.2.1/README.md` & `napari-sam-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [![codecov](https://codecov.io/gh/MIC-DKFZ/napari-sam/branch/main/graph/badge.svg)](https://codecov.io/gh/MIC-DKFZ/napari-sam)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-sam)](https://napari-hub.org/plugins/napari-sam)
 
 Segment anything with Meta AI's new SAM model with thi Napari plugin!
 
 SAM is the new segmentation system from Meta AI capable of **one-click segmentation of any object** and now our plugin neatly integrates this into Napari.
 
-We already **extended** SAMs click-based foreground separation to full **click-based semantic segmentation & instance segmentation** will soon follow!
+We already **extended** SAMs click-based foreground separation to full **click-based semantic segmentation & instance segmentation**!
 
 ----------------------------------
 
 Everything mode             |  Click-based semantic segmentation mode |  Click-based instance segmentation mode
 :-------------------------:|:-------------------------:|:-------------------------:
 ![](cats_everything.png)  |  ![](cats_semantic.png)  |  ![](cats_instance.png)
```

#### html2text {}

```diff
@@ -9,19 +9,19 @@
 graph/badge.svg)](https://codecov.io/gh/MIC-DKFZ/napari-sam) [![napari hub]
 (https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-
 sam)](https://napari-hub.org/plugins/napari-sam) Segment anything with Meta
 AI's new SAM model with thi Napari plugin! SAM is the new segmentation system
 from Meta AI capable of **one-click segmentation of any object** and now our
 plugin neatly integrates this into Napari. We already **extended** SAMs click-
 based foreground separation to full **click-based semantic segmentation &
-instance segmentation** will soon follow! ---------------------------------
-- Everything mode | Click-based semantic segmentation mode | Click-based
-instance segmentation mode :-------------------------:|:-----------------------
---:|:-------------------------: ![](cats_everything.png) | ![]
-(cats_semantic.png) | ![](cats_instance.png) ----------------------------------
+instance segmentation**! ---------------------------------- Everything mode |
+Click-based semantic segmentation mode | Click-based instance segmentation mode
+:-------------------------:|:-------------------------:|:----------------------
+---: ![](cats_everything.png) | ![](cats_semantic.png) | ![](cats_instance.png)
+----------------------------------
                         ***** SAM in Napari demo *****
                             Click to play the video
                                   [SAM_Demo]
 ---------------------------------- ## Installation The plugin requires
 `python>=3.8`, as well as `pytorch>=1.7` and `torchvision>=0.8`. Please follow
 the instructions here to install both PyTorch and TorchVision dependencies.
 Installing both PyTorch and TorchVision with CUDA support is strongly
```

### Comparing `napari-sam-0.2.1/setup.cfg` & `napari-sam-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-sam-0.2.1/src/napari_sam/_widget.py` & `napari-sam-0.2.2/src/napari_sam/_widget.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.2.1/src/napari_sam/utils.py` & `napari-sam-0.2.2/src/napari_sam/utils.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.2.1/src/napari_sam.egg-info/PKG-INFO` & `napari-sam-0.2.2/src/napari_sam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.2.1
+Version: 0.2.2
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
@@ -36,15 +36,15 @@
 [![codecov](https://codecov.io/gh/MIC-DKFZ/napari-sam/branch/main/graph/badge.svg)](https://codecov.io/gh/MIC-DKFZ/napari-sam)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-sam)](https://napari-hub.org/plugins/napari-sam)
 
 Segment anything with Meta AI's new SAM model with thi Napari plugin!
 
 SAM is the new segmentation system from Meta AI capable of **one-click segmentation of any object** and now our plugin neatly integrates this into Napari.
 
-We already **extended** SAMs click-based foreground separation to full **click-based semantic segmentation & instance segmentation** will soon follow!
+We already **extended** SAMs click-based foreground separation to full **click-based semantic segmentation & instance segmentation**!
 
 ----------------------------------
 
 Everything mode             |  Click-based semantic segmentation mode |  Click-based instance segmentation mode
 :-------------------------:|:-------------------------:|:-------------------------:
 ![](cats_everything.png)  |  ![](cats_semantic.png)  |  ![](cats_instance.png)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-sam Version: 0.2.1 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.2.2 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
@@ -25,19 +25,19 @@
 badge.svg)](https://codecov.io/gh/MIC-DKFZ/napari-sam) [![napari hub](https://
 img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-sam)]
 (https://napari-hub.org/plugins/napari-sam) Segment anything with Meta AI's new
 SAM model with thi Napari plugin! SAM is the new segmentation system from Meta
 AI capable of **one-click segmentation of any object** and now our plugin
 neatly integrates this into Napari. We already **extended** SAMs click-based
 foreground separation to full **click-based semantic segmentation & instance
-segmentation** will soon follow! ---------------------------------- Everything
-mode | Click-based semantic segmentation mode | Click-based instance
-segmentation mode :-------------------------:|:-------------------------:|:----
----------------------: ![](cats_everything.png) | ![](cats_semantic.png) | ![]
-(cats_instance.png) ----------------------------------
+segmentation**! ---------------------------------- Everything mode | Click-
+based semantic segmentation mode | Click-based instance segmentation mode :----
+---------------------:|:-------------------------:|:-------------------------:
+![](cats_everything.png) | ![](cats_semantic.png) | ![](cats_instance.png) ----
+------------------------------
                         ***** SAM in Napari demo *****
                             Click to play the video
                                   [SAM_Demo]
 ---------------------------------- ## Installation The plugin requires
 `python>=3.8`, as well as `pytorch>=1.7` and `torchvision>=0.8`. Please follow
 the instructions here to install both PyTorch and TorchVision dependencies.
 Installing both PyTorch and TorchVision with CUDA support is strongly
```

