# Comparing `tmp/metaseg-0.4.0.tar.gz` & `tmp/metaseg-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaseg-0.4.0.tar", last modified: Mon Apr 10 04:35:05 2023, max compression
+gzip compressed data, was "metaseg-0.4.1.tar", last modified: Mon Apr 10 09:24:19 2023, max compression
```

## Comparing `metaseg-0.4.0.tar` & `metaseg-0.4.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 04:35:05.771767 metaseg-0.4.0/
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.4.0/LICENSE
--rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.4.0/MANIFEST.in
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2232 2023-04-10 04:35:05.771767 metaseg-0.4.0/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1958 2023-04-10 04:34:01.000000 metaseg-0.4.0/README.md
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 04:35:05.765100 metaseg-0.4.0/metaseg/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      556 2023-04-10 04:34:06.000000 metaseg-0.4.0/metaseg/__init__.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 04:35:05.768434 metaseg-0.4.0/metaseg/generator/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-09 13:51:55.000000 metaseg-0.4.0/metaseg/generator/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-09 13:58:07.000000 metaseg-0.4.0/metaseg/generator/automatic_mask_generator.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-06 18:52:09.000000 metaseg-0.4.0/metaseg/generator/build_sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-06 18:52:09.000000 metaseg-0.4.0/metaseg/generator/predictor.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5984 2023-04-10 04:34:01.000000 metaseg-0.4.0/metaseg/mask_predictor.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 04:35:05.768434 metaseg-0.4.0/metaseg/modeling/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.4.0/metaseg/modeling/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.4.0/metaseg/modeling/common.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.4.0/metaseg/modeling/image_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.4.0/metaseg/modeling/mask_decoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.4.0/metaseg/modeling/prompt_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.4.0/metaseg/modeling/sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.4.0/metaseg/modeling/transformer.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 04:35:05.771767 metaseg-0.4.0/metaseg/utils/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      310 2023-04-09 10:19:56.000000 metaseg-0.4.0/metaseg/utils/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.4.0/metaseg/utils/amg.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)      518 2023-04-09 10:19:56.000000 metaseg-0.4.0/metaseg/utils/data_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-08 17:15:08.000000 metaseg-0.4.0/metaseg/utils/file_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.4.0/metaseg/utils/onnx.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.4.0/metaseg/utils/transforms.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 04:35:05.771767 metaseg-0.4.0/metaseg/webapp/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-09 10:19:56.000000 metaseg-0.4.0/metaseg/webapp/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-09 10:19:56.000000 metaseg-0.4.0/metaseg/webapp/app.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 04:35:05.768434 metaseg-0.4.0/metaseg.egg-info/
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2232 2023-04-10 04:35:05.000000 metaseg-0.4.0/metaseg.egg-info/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)      834 2023-04-10 04:35:05.000000 metaseg-0.4.0/metaseg.egg-info/SOURCES.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-10 04:35:05.000000 metaseg-0.4.0/metaseg.egg-info/dependency_links.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      226 2023-04-10 04:35:05.000000 metaseg-0.4.0/metaseg.egg-info/requires.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-10 04:35:05.000000 metaseg-0.4.0/metaseg.egg-info/top_level.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.4.0/pyproject.toml
--rw-r--r--   0 kadir     (1000) kadir     (1001)      139 2023-04-08 09:21:23.000000 metaseg-0.4.0/requirements.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-10 04:35:05.775100 metaseg-0.4.0/setup.cfg
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.4.0/setup.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 09:24:19.561351 metaseg-0.4.1/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.4.1/LICENSE
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.4.1/MANIFEST.in
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2505 2023-04-10 09:24:19.561351 metaseg-0.4.1/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2231 2023-04-10 09:24:07.000000 metaseg-0.4.1/README.md
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 09:24:19.554684 metaseg-0.4.1/metaseg/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      556 2023-04-10 09:24:07.000000 metaseg-0.4.1/metaseg/__init__.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 09:24:19.558018 metaseg-0.4.1/metaseg/generator/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-09 13:51:55.000000 metaseg-0.4.1/metaseg/generator/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-09 13:58:07.000000 metaseg-0.4.1/metaseg/generator/automatic_mask_generator.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-06 18:52:09.000000 metaseg-0.4.1/metaseg/generator/build_sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-06 18:52:09.000000 metaseg-0.4.1/metaseg/generator/predictor.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6911 2023-04-10 09:24:07.000000 metaseg-0.4.1/metaseg/mask_predictor.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 09:24:19.558018 metaseg-0.4.1/metaseg/modeling/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.4.1/metaseg/modeling/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.4.1/metaseg/modeling/common.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.4.1/metaseg/modeling/image_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.4.1/metaseg/modeling/mask_decoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.4.1/metaseg/modeling/prompt_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.4.1/metaseg/modeling/sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.4.1/metaseg/modeling/transformer.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 09:24:19.561351 metaseg-0.4.1/metaseg/utils/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      310 2023-04-09 10:19:56.000000 metaseg-0.4.1/metaseg/utils/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.4.1/metaseg/utils/amg.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      518 2023-04-09 10:19:56.000000 metaseg-0.4.1/metaseg/utils/data_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-08 17:15:08.000000 metaseg-0.4.1/metaseg/utils/file_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.4.1/metaseg/utils/onnx.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.4.1/metaseg/utils/transforms.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 09:24:19.561351 metaseg-0.4.1/metaseg/webapp/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-09 10:19:56.000000 metaseg-0.4.1/metaseg/webapp/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-09 10:19:56.000000 metaseg-0.4.1/metaseg/webapp/app.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 09:24:19.554684 metaseg-0.4.1/metaseg.egg-info/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2505 2023-04-10 09:24:19.000000 metaseg-0.4.1/metaseg.egg-info/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      834 2023-04-10 09:24:19.000000 metaseg-0.4.1/metaseg.egg-info/SOURCES.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-10 09:24:19.000000 metaseg-0.4.1/metaseg.egg-info/dependency_links.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      226 2023-04-10 09:24:19.000000 metaseg-0.4.1/metaseg.egg-info/requires.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-10 09:24:19.000000 metaseg-0.4.1/metaseg.egg-info/top_level.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.4.1/pyproject.toml
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      139 2023-04-08 09:21:23.000000 metaseg-0.4.1/requirements.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-10 09:24:19.561351 metaseg-0.4.1/setup.cfg
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.4.1/setup.py
```

### Comparing `metaseg-0.4.0/LICENSE` & `metaseg-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.0/PKG-INFO` & `metaseg-0.4.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.4.0
+Version: 0.4.1
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
@@ -57,22 +57,33 @@
 )
 
 # For manuel box and point selection
 
 seg_manual_mask_generator = SegManualMaskPredictor().save_image(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
-    point_coords=[[100, 100], [200, 200]]
-    point_labels=[0, 1]
-    input_box=[100, 100, 200, 200] # x,y,w,h
+    input_point=[[100, 100], [200, 200]],
+    input_label=[0, 1],
+    input_box=[100, 100, 200, 200], # x,y,w,h
     multimask_output=False,
 
 )
 
+# For multi box selection
+
+seg_manual_mask_generator = SegManualMaskPredictor().save_image(
+    source="data/brain.png",
+    model_type="vit_l",
+    input_point=None,
+    input_label=None,
+    input_box= [[100, 100, 400, 400]],
+    multimask_output=False,
+
+)
 ```
 # Extra Features
 
 - [x] Support for video files
 - [x] Support for pip installation
 - [x] Support for web application
-- [x] Support for manual box and point selection
+- [x] Support for manual single multi box and point selection
 - [x] Support for automatic download model weights
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.4.0 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.4.1 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
@@ -12,13 +12,16 @@
 points_per_side and points_per_batch. # For image autoseg_image =
 SegAutoMaskPredictor().save_image( source="image.jpg", model_type="vit_l", #
 vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=0, ) #
 For video autoseg_video = SegAutoMaskPredictor().save_video
 ( source="video.mp4", model_type="vit_l", # vit_l, vit_h, vit_b
 points_per_side=16, points_per_batch=64, min_area=1000, ) # For manuel box and
 point selection seg_manual_mask_generator = SegManualMaskPredictor().save_image
-( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b point_coords=[
-[100, 100], [200, 200]] point_labels=[0, 1] input_box=[100, 100, 200, 200] #
-x,y,w,h multimask_output=False, ) ``` # Extra Features - [x] Support for video
-files - [x] Support for pip installation - [x] Support for web application -
-[x] Support for manual box and point selection - [x] Support for automatic
-download model weights
+( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b input_point=[
+[100, 100], [200, 200]], input_label=[0, 1], input_box=[100, 100, 200, 200], #
+x,y,w,h multimask_output=False, ) # For multi box selection
+seg_manual_mask_generator = SegManualMaskPredictor().save_image( source="data/
+brain.png", model_type="vit_l", input_point=None, input_label=None, input_box=
+[[100, 100, 400, 400]], multimask_output=False, ) ``` # Extra Features - [x]
+Support for video files - [x] Support for pip installation - [x] Support for
+web application - [x] Support for manual single multi box and point selection -
+[x] Support for automatic download model weights
```

### Comparing `metaseg-0.4.0/README.md` & `metaseg-0.4.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -45,22 +45,33 @@
 )
 
 # For manuel box and point selection
 
 seg_manual_mask_generator = SegManualMaskPredictor().save_image(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
-    point_coords=[[100, 100], [200, 200]]
-    point_labels=[0, 1]
-    input_box=[100, 100, 200, 200] # x,y,w,h
+    input_point=[[100, 100], [200, 200]],
+    input_label=[0, 1],
+    input_box=[100, 100, 200, 200], # x,y,w,h
     multimask_output=False,
 
 )
 
+# For multi box selection
+
+seg_manual_mask_generator = SegManualMaskPredictor().save_image(
+    source="data/brain.png",
+    model_type="vit_l",
+    input_point=None,
+    input_label=None,
+    input_box= [[100, 100, 400, 400]],
+    multimask_output=False,
+
+)
 ```
 # Extra Features
 
 - [x] Support for video files
 - [x] Support for pip installation
 - [x] Support for web application
-- [x] Support for manual box and point selection
+- [x] Support for manual single multi box and point selection
 - [x] Support for automatic download model weights
```

#### html2text {}

```diff
@@ -8,13 +8,16 @@
 points_per_side and points_per_batch. # For image autoseg_image =
 SegAutoMaskPredictor().save_image( source="image.jpg", model_type="vit_l", #
 vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=0, ) #
 For video autoseg_video = SegAutoMaskPredictor().save_video
 ( source="video.mp4", model_type="vit_l", # vit_l, vit_h, vit_b
 points_per_side=16, points_per_batch=64, min_area=1000, ) # For manuel box and
 point selection seg_manual_mask_generator = SegManualMaskPredictor().save_image
-( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b point_coords=[
-[100, 100], [200, 200]] point_labels=[0, 1] input_box=[100, 100, 200, 200] #
-x,y,w,h multimask_output=False, ) ``` # Extra Features - [x] Support for video
-files - [x] Support for pip installation - [x] Support for web application -
-[x] Support for manual box and point selection - [x] Support for automatic
-download model weights
+( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b input_point=[
+[100, 100], [200, 200]], input_label=[0, 1], input_box=[100, 100, 200, 200], #
+x,y,w,h multimask_output=False, ) # For multi box selection
+seg_manual_mask_generator = SegManualMaskPredictor().save_image( source="data/
+brain.png", model_type="vit_l", input_point=None, input_label=None, input_box=
+[[100, 100, 400, 400]], multimask_output=False, ) ``` # Extra Features - [x]
+Support for video files - [x] Support for pip installation - [x] Support for
+web application - [x] Support for manual single multi box and point selection -
+[x] Support for automatic download model weights
```

### Comparing `metaseg-0.4.0/metaseg/__init__.py` & `metaseg-0.4.1/metaseg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 # LICENSE file in the root directory of this source tree.
 
 from metaseg.generator.automatic_mask_generator import SamAutomaticMaskGenerator
 from metaseg.generator.build_sam import build_sam, build_sam_vit_b, build_sam_vit_h, build_sam_vit_l, sam_model_registry
 from metaseg.generator.predictor import SamPredictor
 from metaseg.mask_predictor import SegAutoMaskPredictor, SegManualMaskPredictor
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
```

### Comparing `metaseg-0.4.0/metaseg/generator/automatic_mask_generator.py` & `metaseg-0.4.1/metaseg/generator/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.0/metaseg/generator/build_sam.py` & `metaseg-0.4.1/metaseg/generator/build_sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.0/metaseg/generator/predictor.py` & `metaseg-0.4.1/metaseg/generator/predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.0/metaseg/mask_predictor.py` & `metaseg-0.4.1/metaseg/mask_predictor.py`

 * *Files 11% similar despite different names*

```diff
@@ -110,64 +110,88 @@
         return self.model
 
     def load_mask(self, mask, random_color):
         if random_color:
             color = np.random.rand(3) * 255
         else:
             color = np.array([100, 50, 0])
+
         h, w = mask.shape[-2:]
         mask_image = mask.reshape(h, w, 1) * color.reshape(1, 1, -1)
         mask_image = mask_image.astype(np.uint8)
         return mask_image
 
     def load_box(self, box, image):
-        x0, y0 = box[0], box[1]
-        x1, y1 = box[2], box[3]
-        cv2.rectangle(image, (x0, y0), (x1, y1), (0, 255, 0), 2)
+        x, y, w, h = int(box[0]), int(box[1]), int(box[2]), int(box[3])
+        cv2.rectangle(image, (x, y), (w, h), (0, 255, 0), 2)
         return image
 
+    def multi_boxes(self, boxes, predictor, image):
+        input_boxes = torch.tensor(boxes, device=predictor.device)
+        transformed_boxes = predictor.transform.apply_boxes_torch(input_boxes, image.shape[:2])
+        return input_boxes, transformed_boxes
+
     def predict(
         self,
         frame,
         model_type,
         input_box=None,
         input_point=None,
         input_label=None,
         multimask_output=False,
     ):
         model = self.load_model(model_type)
         predictor = SamPredictor(model)
-
         predictor.set_image(frame)
-        input_box = np.array(input_box)
-        masks, _, _ = predictor.predict(
-            point_coords=input_point,
-            point_labels=input_label,
-            box=input_box[None, :],
-            multimask_output=multimask_output,
-        )
 
-        return frame, masks, input_box
+        if type(input_box[0]) == list:
+            input_boxes, new_boxes = self.multi_boxes(input_box, predictor, frame)
+
+            masks, _, _ = predictor.predict_torch(
+                point_coords=None,
+                point_labels=None,
+                boxes=new_boxes,
+                multimask_output=False,
+            )
+
+        elif type(input_box[0]) == int:
+            input_boxes = np.array(input_box)[None, :]
+
+            masks, _, _ = predictor.predict(
+                point_coords=input_point,
+                point_labels=input_label,
+                box=input_boxes,
+                multimask_output=multimask_output,
+            )
+
+        return frame, masks, input_boxes
 
     def save_image(
         self,
         source,
         model_type,
         input_box=None,
         input_point=None,
         input_label=None,
         multimask_output=False,
-        output_path="output.jpg",
+        output_path="v0.jpg",
     ):
         read_image = load_image(source)
-        image, anns, input_box = self.predict(
-            read_image, model_type, input_box, input_point, input_label, multimask_output
-        )
+        image, anns, boxes = self.predict(read_image, model_type, input_box, input_point, input_label, multimask_output)
         if len(anns) == 0:
             return
 
-        mask_image = self.load_mask(anns, True)
-        image = self.load_box(input_box, image)
+        if type(input_box[0]) == list:
+            for mask in anns:
+                mask_image = self.load_mask(mask.cpu().numpy(), False)
+
+            for box in boxes:
+                image = self.load_box(box.cpu().numpy(), image)
+
+        elif type(input_box[0]) == int:
+            mask_image = self.load_mask(anns, True)
+            image = self.load_box(input_box, image)
+
         combined_mask = cv2.add(image, mask_image)
-        cv2.imwrite(output_path, combined_mask)
+        cv2.write(output_path, combined_mask)
 
         return output_path
```

### Comparing `metaseg-0.4.0/metaseg/modeling/common.py` & `metaseg-0.4.1/metaseg/modeling/common.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.0/metaseg/modeling/image_encoder.py` & `metaseg-0.4.1/metaseg/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.0/metaseg/modeling/mask_decoder.py` & `metaseg-0.4.1/metaseg/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.0/metaseg/modeling/prompt_encoder.py` & `metaseg-0.4.1/metaseg/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.0/metaseg/modeling/sam.py` & `metaseg-0.4.1/metaseg/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.0/metaseg/modeling/transformer.py` & `metaseg-0.4.1/metaseg/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.0/metaseg/utils/amg.py` & `metaseg-0.4.1/metaseg/utils/amg.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.0/metaseg/utils/data_utils.py` & `metaseg-0.4.1/metaseg/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.0/metaseg/utils/file_utils.py` & `metaseg-0.4.1/metaseg/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.0/metaseg/utils/onnx.py` & `metaseg-0.4.1/metaseg/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.0/metaseg/utils/transforms.py` & `metaseg-0.4.1/metaseg/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.0/metaseg/webapp/app.py` & `metaseg-0.4.1/metaseg/webapp/app.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.0/metaseg.egg-info/PKG-INFO` & `metaseg-0.4.1/metaseg.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.4.0
+Version: 0.4.1
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
@@ -57,22 +57,33 @@
 )
 
 # For manuel box and point selection
 
 seg_manual_mask_generator = SegManualMaskPredictor().save_image(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
-    point_coords=[[100, 100], [200, 200]]
-    point_labels=[0, 1]
-    input_box=[100, 100, 200, 200] # x,y,w,h
+    input_point=[[100, 100], [200, 200]],
+    input_label=[0, 1],
+    input_box=[100, 100, 200, 200], # x,y,w,h
     multimask_output=False,
 
 )
 
+# For multi box selection
+
+seg_manual_mask_generator = SegManualMaskPredictor().save_image(
+    source="data/brain.png",
+    model_type="vit_l",
+    input_point=None,
+    input_label=None,
+    input_box= [[100, 100, 400, 400]],
+    multimask_output=False,
+
+)
 ```
 # Extra Features
 
 - [x] Support for video files
 - [x] Support for pip installation
 - [x] Support for web application
-- [x] Support for manual box and point selection
+- [x] Support for manual single multi box and point selection
 - [x] Support for automatic download model weights
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.4.0 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.4.1 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
@@ -12,13 +12,16 @@
 points_per_side and points_per_batch. # For image autoseg_image =
 SegAutoMaskPredictor().save_image( source="image.jpg", model_type="vit_l", #
 vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=0, ) #
 For video autoseg_video = SegAutoMaskPredictor().save_video
 ( source="video.mp4", model_type="vit_l", # vit_l, vit_h, vit_b
 points_per_side=16, points_per_batch=64, min_area=1000, ) # For manuel box and
 point selection seg_manual_mask_generator = SegManualMaskPredictor().save_image
-( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b point_coords=[
-[100, 100], [200, 200]] point_labels=[0, 1] input_box=[100, 100, 200, 200] #
-x,y,w,h multimask_output=False, ) ``` # Extra Features - [x] Support for video
-files - [x] Support for pip installation - [x] Support for web application -
-[x] Support for manual box and point selection - [x] Support for automatic
-download model weights
+( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b input_point=[
+[100, 100], [200, 200]], input_label=[0, 1], input_box=[100, 100, 200, 200], #
+x,y,w,h multimask_output=False, ) # For multi box selection
+seg_manual_mask_generator = SegManualMaskPredictor().save_image( source="data/
+brain.png", model_type="vit_l", input_point=None, input_label=None, input_box=
+[[100, 100, 400, 400]], multimask_output=False, ) ``` # Extra Features - [x]
+Support for video files - [x] Support for pip installation - [x] Support for
+web application - [x] Support for manual single multi box and point selection -
+[x] Support for automatic download model weights
```

### Comparing `metaseg-0.4.0/metaseg.egg-info/SOURCES.txt` & `metaseg-0.4.1/metaseg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.0/setup.py` & `metaseg-0.4.1/setup.py`

 * *Files identical despite different names*

