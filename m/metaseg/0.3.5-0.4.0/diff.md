# Comparing `tmp/metaseg-0.3.5.tar.gz` & `tmp/metaseg-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaseg-0.3.5.tar", last modified: Sun Apr  9 14:15:24 2023, max compression
+gzip compressed data, was "metaseg-0.4.0.tar", last modified: Mon Apr 10 04:35:05 2023, max compression
```

## Comparing `metaseg-0.3.5.tar` & `metaseg-0.4.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 14:15:24.909224 metaseg-0.3.5/
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.3.5/LICENSE
--rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.3.5/MANIFEST.in
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2125 2023-04-09 14:15:24.909224 metaseg-0.3.5/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1851 2023-04-09 14:07:11.000000 metaseg-0.3.5/README.md
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 14:15:24.899224 metaseg-0.3.5/metaseg/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      556 2023-04-09 14:02:26.000000 metaseg-0.3.5/metaseg/__init__.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 14:15:24.899224 metaseg-0.3.5/metaseg/generator/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-09 13:51:55.000000 metaseg-0.3.5/metaseg/generator/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-09 13:58:07.000000 metaseg-0.3.5/metaseg/generator/automatic_mask_generator.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-06 18:52:09.000000 metaseg-0.3.5/metaseg/generator/build_sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-06 18:52:09.000000 metaseg-0.3.5/metaseg/generator/predictor.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5580 2023-04-09 13:58:07.000000 metaseg-0.3.5/metaseg/mask_predictor.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 14:15:24.902557 metaseg-0.3.5/metaseg/modeling/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.3.5/metaseg/modeling/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.3.5/metaseg/modeling/common.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.3.5/metaseg/modeling/image_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.3.5/metaseg/modeling/mask_decoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.3.5/metaseg/modeling/prompt_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.3.5/metaseg/modeling/sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.3.5/metaseg/modeling/transformer.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 14:15:24.905890 metaseg-0.3.5/metaseg/utils/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      310 2023-04-09 10:19:56.000000 metaseg-0.3.5/metaseg/utils/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.3.5/metaseg/utils/amg.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)      518 2023-04-09 10:19:56.000000 metaseg-0.3.5/metaseg/utils/data_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-08 17:15:08.000000 metaseg-0.3.5/metaseg/utils/file_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.3.5/metaseg/utils/onnx.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.3.5/metaseg/utils/transforms.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 14:15:24.909224 metaseg-0.3.5/metaseg/webapp/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-09 10:19:56.000000 metaseg-0.3.5/metaseg/webapp/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-09 10:19:56.000000 metaseg-0.3.5/metaseg/webapp/app.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 14:15:24.899224 metaseg-0.3.5/metaseg.egg-info/
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2125 2023-04-09 14:15:24.000000 metaseg-0.3.5/metaseg.egg-info/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)      834 2023-04-09 14:15:24.000000 metaseg-0.3.5/metaseg.egg-info/SOURCES.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-09 14:15:24.000000 metaseg-0.3.5/metaseg.egg-info/dependency_links.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      226 2023-04-09 14:15:24.000000 metaseg-0.3.5/metaseg.egg-info/requires.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-09 14:15:24.000000 metaseg-0.3.5/metaseg.egg-info/top_level.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.3.5/pyproject.toml
--rw-r--r--   0 kadir     (1000) kadir     (1001)      139 2023-04-08 09:21:23.000000 metaseg-0.3.5/requirements.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-09 14:15:24.909224 metaseg-0.3.5/setup.cfg
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.3.5/setup.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 04:35:05.771767 metaseg-0.4.0/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.4.0/LICENSE
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.4.0/MANIFEST.in
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2232 2023-04-10 04:35:05.771767 metaseg-0.4.0/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1958 2023-04-10 04:34:01.000000 metaseg-0.4.0/README.md
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 04:35:05.765100 metaseg-0.4.0/metaseg/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      556 2023-04-10 04:34:06.000000 metaseg-0.4.0/metaseg/__init__.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 04:35:05.768434 metaseg-0.4.0/metaseg/generator/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-09 13:51:55.000000 metaseg-0.4.0/metaseg/generator/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-09 13:58:07.000000 metaseg-0.4.0/metaseg/generator/automatic_mask_generator.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-06 18:52:09.000000 metaseg-0.4.0/metaseg/generator/build_sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-06 18:52:09.000000 metaseg-0.4.0/metaseg/generator/predictor.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     5984 2023-04-10 04:34:01.000000 metaseg-0.4.0/metaseg/mask_predictor.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 04:35:05.768434 metaseg-0.4.0/metaseg/modeling/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.4.0/metaseg/modeling/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.4.0/metaseg/modeling/common.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.4.0/metaseg/modeling/image_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.4.0/metaseg/modeling/mask_decoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.4.0/metaseg/modeling/prompt_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.4.0/metaseg/modeling/sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.4.0/metaseg/modeling/transformer.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 04:35:05.771767 metaseg-0.4.0/metaseg/utils/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      310 2023-04-09 10:19:56.000000 metaseg-0.4.0/metaseg/utils/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.4.0/metaseg/utils/amg.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      518 2023-04-09 10:19:56.000000 metaseg-0.4.0/metaseg/utils/data_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-08 17:15:08.000000 metaseg-0.4.0/metaseg/utils/file_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.4.0/metaseg/utils/onnx.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.4.0/metaseg/utils/transforms.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 04:35:05.771767 metaseg-0.4.0/metaseg/webapp/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-09 10:19:56.000000 metaseg-0.4.0/metaseg/webapp/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-09 10:19:56.000000 metaseg-0.4.0/metaseg/webapp/app.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 04:35:05.768434 metaseg-0.4.0/metaseg.egg-info/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2232 2023-04-10 04:35:05.000000 metaseg-0.4.0/metaseg.egg-info/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      834 2023-04-10 04:35:05.000000 metaseg-0.4.0/metaseg.egg-info/SOURCES.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-10 04:35:05.000000 metaseg-0.4.0/metaseg.egg-info/dependency_links.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      226 2023-04-10 04:35:05.000000 metaseg-0.4.0/metaseg.egg-info/requires.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-10 04:35:05.000000 metaseg-0.4.0/metaseg.egg-info/top_level.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.4.0/pyproject.toml
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      139 2023-04-08 09:21:23.000000 metaseg-0.4.0/requirements.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-10 04:35:05.775100 metaseg-0.4.0/setup.cfg
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.4.0/setup.py
```

### Comparing `metaseg-0.3.5/LICENSE` & `metaseg-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.5/PKG-INFO` & `metaseg-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.3.5
+Version: 0.4.0
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
@@ -52,26 +52,27 @@
     source="video.mp4",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=1000,
 )
 
-# For manuel box selection
+# For manuel box and point selection
 
 seg_manual_mask_generator = SegManualMaskPredictor().save_image(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
-    x0=100,
-    y0=100,
-    x1=200,
-    y1=200,
+    point_coords=[[100, 100], [200, 200]]
+    point_labels=[0, 1]
+    input_box=[100, 100, 200, 200] # x,y,w,h
+    multimask_output=False,
+
 )
+
 ```
 # Extra Features
 
 - [x] Support for video files
 - [x] Support for pip installation
 - [x] Support for web application
-- [x] Support for box to polygon conversion
+- [x] Support for manual box and point selection
 - [x] Support for automatic download model weights
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.3.5 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.4.0 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
@@ -10,14 +10,15 @@
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskPredictor,
 SegManualMaskPredictor # If gpu memory is not enough, reduce the
 points_per_side and points_per_batch. # For image autoseg_image =
 SegAutoMaskPredictor().save_image( source="image.jpg", model_type="vit_l", #
 vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=0, ) #
 For video autoseg_video = SegAutoMaskPredictor().save_video
 ( source="video.mp4", model_type="vit_l", # vit_l, vit_h, vit_b
-points_per_side=16, points_per_batch=64, min_area=1000, ) # For manuel box
-selection seg_manual_mask_generator = SegManualMaskPredictor().save_image
-( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b x0=100, y0=100,
-x1=200, y1=200, ) ``` # Extra Features - [x] Support for video files - [x]
-Support for pip installation - [x] Support for web application - [x] Support
-for box to polygon conversion - [x] Support for automatic download model
-weights
+points_per_side=16, points_per_batch=64, min_area=1000, ) # For manuel box and
+point selection seg_manual_mask_generator = SegManualMaskPredictor().save_image
+( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b point_coords=[
+[100, 100], [200, 200]] point_labels=[0, 1] input_box=[100, 100, 200, 200] #
+x,y,w,h multimask_output=False, ) ``` # Extra Features - [x] Support for video
+files - [x] Support for pip installation - [x] Support for web application -
+[x] Support for manual box and point selection - [x] Support for automatic
+download model weights
```

### Comparing `metaseg-0.3.5/README.md` & `metaseg-0.4.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -40,26 +40,27 @@
     source="video.mp4",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=1000,
 )
 
-# For manuel box selection
+# For manuel box and point selection
 
 seg_manual_mask_generator = SegManualMaskPredictor().save_image(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
-    x0=100,
-    y0=100,
-    x1=200,
-    y1=200,
+    point_coords=[[100, 100], [200, 200]]
+    point_labels=[0, 1]
+    input_box=[100, 100, 200, 200] # x,y,w,h
+    multimask_output=False,
+
 )
+
 ```
 # Extra Features
 
 - [x] Support for video files
 - [x] Support for pip installation
 - [x] Support for web application
-- [x] Support for box to polygon conversion
+- [x] Support for manual box and point selection
 - [x] Support for automatic download model weights
-
```

#### html2text {}

```diff
@@ -6,14 +6,15 @@
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskPredictor,
 SegManualMaskPredictor # If gpu memory is not enough, reduce the
 points_per_side and points_per_batch. # For image autoseg_image =
 SegAutoMaskPredictor().save_image( source="image.jpg", model_type="vit_l", #
 vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=0, ) #
 For video autoseg_video = SegAutoMaskPredictor().save_video
 ( source="video.mp4", model_type="vit_l", # vit_l, vit_h, vit_b
-points_per_side=16, points_per_batch=64, min_area=1000, ) # For manuel box
-selection seg_manual_mask_generator = SegManualMaskPredictor().save_image
-( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b x0=100, y0=100,
-x1=200, y1=200, ) ``` # Extra Features - [x] Support for video files - [x]
-Support for pip installation - [x] Support for web application - [x] Support
-for box to polygon conversion - [x] Support for automatic download model
-weights
+points_per_side=16, points_per_batch=64, min_area=1000, ) # For manuel box and
+point selection seg_manual_mask_generator = SegManualMaskPredictor().save_image
+( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b point_coords=[
+[100, 100], [200, 200]] point_labels=[0, 1] input_box=[100, 100, 200, 200] #
+x,y,w,h multimask_output=False, ) ``` # Extra Features - [x] Support for video
+files - [x] Support for pip installation - [x] Support for web application -
+[x] Support for manual box and point selection - [x] Support for automatic
+download model weights
```

### Comparing `metaseg-0.3.5/metaseg/__init__.py` & `metaseg-0.4.0/metaseg/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 # LICENSE file in the root directory of this source tree.
 
 from metaseg.generator.automatic_mask_generator import SamAutomaticMaskGenerator
 from metaseg.generator.build_sam import build_sam, build_sam_vit_b, build_sam_vit_h, build_sam_vit_l, sam_model_registry
 from metaseg.generator.predictor import SamPredictor
 from metaseg.mask_predictor import SegAutoMaskPredictor, SegManualMaskPredictor
 
-__version__ = "0.3.5"
+__version__ = "0.4.0"
```

### Comparing `metaseg-0.3.5/metaseg/generator/automatic_mask_generator.py` & `metaseg-0.4.0/metaseg/generator/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.5/metaseg/generator/build_sam.py` & `metaseg-0.4.0/metaseg/generator/build_sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.5/metaseg/generator/predictor.py` & `metaseg-0.4.0/metaseg/generator/predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.5/metaseg/mask_predictor.py` & `metaseg-0.4.0/metaseg/mask_predictor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Any, Dict, List, Optional
+
 import cv2
 import numpy as np
 import torch
 
 from metaseg import SamAutomaticMaskGenerator, SamPredictor, sam_model_registry
 from metaseg.utils import download_model, load_image, load_video
 
@@ -119,33 +121,53 @@
 
     def load_box(self, box, image):
         x0, y0 = box[0], box[1]
         x1, y1 = box[2], box[3]
         cv2.rectangle(image, (x0, y0), (x1, y1), (0, 255, 0), 2)
         return image
 
-    def predict(self, frame, model_type, x0, y0, x1, y1):
+    def predict(
+        self,
+        frame,
+        model_type,
+        input_box=None,
+        input_point=None,
+        input_label=None,
+        multimask_output=False,
+    ):
         model = self.load_model(model_type)
         predictor = SamPredictor(model)
+
         predictor.set_image(frame)
-        input_box = np.array([x0, y0, x1, y1])
+        input_box = np.array(input_box)
         masks, _, _ = predictor.predict(
-            point_coords=None,
-            point_labels=None,
+            point_coords=input_point,
+            point_labels=input_label,
             box=input_box[None, :],
-            multimask_output=False,
+            multimask_output=multimask_output,
         )
 
         return frame, masks, input_box
 
-    def save_image(self, source, model_type, x0, y0, x1, y1):
+    def save_image(
+        self,
+        source,
+        model_type,
+        input_box=None,
+        input_point=None,
+        input_label=None,
+        multimask_output=False,
+        output_path="output.jpg",
+    ):
         read_image = load_image(source)
-        image, anns, input_box = self.predict(read_image, model_type, x0, y0, x1, y1)
+        image, anns, input_box = self.predict(
+            read_image, model_type, input_box, input_point, input_label, multimask_output
+        )
         if len(anns) == 0:
             return
 
         mask_image = self.load_mask(anns, True)
         image = self.load_box(input_box, image)
         combined_mask = cv2.add(image, mask_image)
-        cv2.imwrite("output.jpg", combined_mask)
+        cv2.imwrite(output_path, combined_mask)
 
-        return "output.jpg"
+        return output_path
```

### Comparing `metaseg-0.3.5/metaseg/modeling/common.py` & `metaseg-0.4.0/metaseg/modeling/common.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.5/metaseg/modeling/image_encoder.py` & `metaseg-0.4.0/metaseg/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.5/metaseg/modeling/mask_decoder.py` & `metaseg-0.4.0/metaseg/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.5/metaseg/modeling/prompt_encoder.py` & `metaseg-0.4.0/metaseg/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.5/metaseg/modeling/sam.py` & `metaseg-0.4.0/metaseg/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.5/metaseg/modeling/transformer.py` & `metaseg-0.4.0/metaseg/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.5/metaseg/utils/amg.py` & `metaseg-0.4.0/metaseg/utils/amg.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.5/metaseg/utils/data_utils.py` & `metaseg-0.4.0/metaseg/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.5/metaseg/utils/file_utils.py` & `metaseg-0.4.0/metaseg/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.5/metaseg/utils/onnx.py` & `metaseg-0.4.0/metaseg/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.5/metaseg/utils/transforms.py` & `metaseg-0.4.0/metaseg/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.5/metaseg/webapp/app.py` & `metaseg-0.4.0/metaseg/webapp/app.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.5/metaseg.egg-info/PKG-INFO` & `metaseg-0.4.0/metaseg.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.3.5
+Version: 0.4.0
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
@@ -52,26 +52,27 @@
     source="video.mp4",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=1000,
 )
 
-# For manuel box selection
+# For manuel box and point selection
 
 seg_manual_mask_generator = SegManualMaskPredictor().save_image(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
-    x0=100,
-    y0=100,
-    x1=200,
-    y1=200,
+    point_coords=[[100, 100], [200, 200]]
+    point_labels=[0, 1]
+    input_box=[100, 100, 200, 200] # x,y,w,h
+    multimask_output=False,
+
 )
+
 ```
 # Extra Features
 
 - [x] Support for video files
 - [x] Support for pip installation
 - [x] Support for web application
-- [x] Support for box to polygon conversion
+- [x] Support for manual box and point selection
 - [x] Support for automatic download model weights
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.3.5 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.4.0 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
@@ -10,14 +10,15 @@
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskPredictor,
 SegManualMaskPredictor # If gpu memory is not enough, reduce the
 points_per_side and points_per_batch. # For image autoseg_image =
 SegAutoMaskPredictor().save_image( source="image.jpg", model_type="vit_l", #
 vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=0, ) #
 For video autoseg_video = SegAutoMaskPredictor().save_video
 ( source="video.mp4", model_type="vit_l", # vit_l, vit_h, vit_b
-points_per_side=16, points_per_batch=64, min_area=1000, ) # For manuel box
-selection seg_manual_mask_generator = SegManualMaskPredictor().save_image
-( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b x0=100, y0=100,
-x1=200, y1=200, ) ``` # Extra Features - [x] Support for video files - [x]
-Support for pip installation - [x] Support for web application - [x] Support
-for box to polygon conversion - [x] Support for automatic download model
-weights
+points_per_side=16, points_per_batch=64, min_area=1000, ) # For manuel box and
+point selection seg_manual_mask_generator = SegManualMaskPredictor().save_image
+( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b point_coords=[
+[100, 100], [200, 200]] point_labels=[0, 1] input_box=[100, 100, 200, 200] #
+x,y,w,h multimask_output=False, ) ``` # Extra Features - [x] Support for video
+files - [x] Support for pip installation - [x] Support for web application -
+[x] Support for manual box and point selection - [x] Support for automatic
+download model weights
```

### Comparing `metaseg-0.3.5/metaseg.egg-info/SOURCES.txt` & `metaseg-0.4.0/metaseg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.5/setup.py` & `metaseg-0.4.0/setup.py`

 * *Files identical despite different names*

