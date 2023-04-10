# Comparing `tmp/metaseg-0.4.2.tar.gz` & `tmp/metaseg-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaseg-0.4.2.tar", last modified: Mon Apr 10 17:58:53 2023, max compression
+gzip compressed data, was "metaseg-0.4.4.tar", last modified: Mon Apr 10 19:54:43 2023, max compression
```

## Comparing `metaseg-0.4.2.tar` & `metaseg-0.4.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 17:58:53.921825 metaseg-0.4.2/
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.4.2/LICENSE
--rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.4.2/MANIFEST.in
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2505 2023-04-10 17:58:53.921825 metaseg-0.4.2/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2231 2023-04-10 09:24:07.000000 metaseg-0.4.2/README.md
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 17:58:53.915158 metaseg-0.4.2/metaseg/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      556 2023-04-10 17:56:20.000000 metaseg-0.4.2/metaseg/__init__.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 17:58:53.918491 metaseg-0.4.2/metaseg/generator/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-09 13:51:55.000000 metaseg-0.4.2/metaseg/generator/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-09 13:58:07.000000 metaseg-0.4.2/metaseg/generator/automatic_mask_generator.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-06 18:52:09.000000 metaseg-0.4.2/metaseg/generator/build_sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-06 18:52:09.000000 metaseg-0.4.2/metaseg/generator/predictor.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6913 2023-04-10 17:57:10.000000 metaseg-0.4.2/metaseg/mask_predictor.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 17:58:53.918491 metaseg-0.4.2/metaseg/modeling/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.4.2/metaseg/modeling/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.4.2/metaseg/modeling/common.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.4.2/metaseg/modeling/image_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.4.2/metaseg/modeling/mask_decoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.4.2/metaseg/modeling/prompt_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.4.2/metaseg/modeling/sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.4.2/metaseg/modeling/transformer.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1205 2023-04-10 17:56:26.000000 metaseg-0.4.2/metaseg/sahi_predict.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 17:58:53.921825 metaseg-0.4.2/metaseg/utils/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      310 2023-04-09 10:19:56.000000 metaseg-0.4.2/metaseg/utils/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.4.2/metaseg/utils/amg.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)      518 2023-04-09 10:19:56.000000 metaseg-0.4.2/metaseg/utils/data_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-08 17:15:08.000000 metaseg-0.4.2/metaseg/utils/file_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.4.2/metaseg/utils/onnx.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.4.2/metaseg/utils/transforms.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 17:58:53.921825 metaseg-0.4.2/metaseg/webapp/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-09 10:19:56.000000 metaseg-0.4.2/metaseg/webapp/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-09 10:19:56.000000 metaseg-0.4.2/metaseg/webapp/app.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 17:58:53.918491 metaseg-0.4.2/metaseg.egg-info/
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2505 2023-04-10 17:58:53.000000 metaseg-0.4.2/metaseg.egg-info/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)      858 2023-04-10 17:58:53.000000 metaseg-0.4.2/metaseg.egg-info/SOURCES.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-10 17:58:53.000000 metaseg-0.4.2/metaseg.egg-info/dependency_links.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      226 2023-04-10 17:58:53.000000 metaseg-0.4.2/metaseg.egg-info/requires.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-10 17:58:53.000000 metaseg-0.4.2/metaseg.egg-info/top_level.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.4.2/pyproject.toml
--rw-r--r--   0 kadir     (1000) kadir     (1001)      139 2023-04-08 09:21:23.000000 metaseg-0.4.2/requirements.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-10 17:58:53.921825 metaseg-0.4.2/setup.cfg
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.4.2/setup.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 19:54:43.552033 metaseg-0.4.4/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.4.4/LICENSE
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.4.4/MANIFEST.in
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2557 2023-04-10 19:54:43.552033 metaseg-0.4.4/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2283 2023-04-10 19:41:32.000000 metaseg-0.4.4/README.md
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 19:54:43.542033 metaseg-0.4.4/metaseg/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      556 2023-04-10 19:54:13.000000 metaseg-0.4.4/metaseg/__init__.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 19:54:43.548700 metaseg-0.4.4/metaseg/generator/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-10 18:01:14.000000 metaseg-0.4.4/metaseg/generator/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-10 18:01:14.000000 metaseg-0.4.4/metaseg/generator/automatic_mask_generator.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-10 18:01:14.000000 metaseg-0.4.4/metaseg/generator/build_sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-10 18:01:14.000000 metaseg-0.4.4/metaseg/generator/predictor.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     7009 2023-04-10 19:54:00.000000 metaseg-0.4.4/metaseg/mask_predictor.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 19:54:43.548700 metaseg-0.4.4/metaseg/modeling/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.4.4/metaseg/modeling/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.4.4/metaseg/modeling/common.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.4.4/metaseg/modeling/image_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.4.4/metaseg/modeling/mask_decoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.4.4/metaseg/modeling/prompt_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.4.4/metaseg/modeling/sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.4.4/metaseg/modeling/transformer.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1205 2023-04-10 18:01:14.000000 metaseg-0.4.4/metaseg/sahi_predict.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 19:54:43.552033 metaseg-0.4.4/metaseg/utils/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      310 2023-04-10 18:01:14.000000 metaseg-0.4.4/metaseg/utils/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.4.4/metaseg/utils/amg.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      518 2023-04-10 18:01:14.000000 metaseg-0.4.4/metaseg/utils/data_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-10 18:01:14.000000 metaseg-0.4.4/metaseg/utils/file_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.4.4/metaseg/utils/onnx.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.4.4/metaseg/utils/transforms.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 19:54:43.552033 metaseg-0.4.4/metaseg/webapp/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-10 18:01:14.000000 metaseg-0.4.4/metaseg/webapp/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-10 18:01:14.000000 metaseg-0.4.4/metaseg/webapp/app.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 19:54:43.545367 metaseg-0.4.4/metaseg.egg-info/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2557 2023-04-10 19:54:43.000000 metaseg-0.4.4/metaseg.egg-info/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      858 2023-04-10 19:54:43.000000 metaseg-0.4.4/metaseg.egg-info/SOURCES.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-10 19:54:43.000000 metaseg-0.4.4/metaseg.egg-info/dependency_links.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      231 2023-04-10 19:54:43.000000 metaseg-0.4.4/metaseg.egg-info/requires.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-10 19:54:43.000000 metaseg-0.4.4/metaseg.egg-info/top_level.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.4.4/pyproject.toml
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      144 2023-04-10 19:54:00.000000 metaseg-0.4.4/requirements.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-10 19:54:43.555367 metaseg-0.4.4/setup.cfg
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.4.4/setup.py
```

### Comparing `metaseg-0.4.2/LICENSE` & `metaseg-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.2/PKG-INFO` & `metaseg-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.4.2
+Version: 0.4.4
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
@@ -78,12 +78,12 @@
     input_box= [[100, 100, 400, 400]],
     multimask_output=False,
 
 )
 ```
 # Extra Features
 
-- [x] Support for video files
-- [x] Support for pip installation
-- [x] Support for web application
+- [x] Support for Yolov5/8, Detectron2, Mmdetection, Torchvision models
+- [x] Support for video and web application(Huggingface Spaces)
 - [x] Support for manual single multi box and point selection
-- [x] Support for automatic download model weights
+- [x] Support for pip installation
+- [x] Support for SAHI library
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.4.2 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.4.4 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
@@ -18,10 +18,11 @@
 point selection seg_manual_mask_generator = SegManualMaskPredictor().save_image
 ( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b input_point=[
 [100, 100], [200, 200]], input_label=[0, 1], input_box=[100, 100, 200, 200], #
 x,y,w,h multimask_output=False, ) # For multi box selection
 seg_manual_mask_generator = SegManualMaskPredictor().save_image( source="data/
 brain.png", model_type="vit_l", input_point=None, input_label=None, input_box=
 [[100, 100, 400, 400]], multimask_output=False, ) ``` # Extra Features - [x]
-Support for video files - [x] Support for pip installation - [x] Support for
-web application - [x] Support for manual single multi box and point selection -
-[x] Support for automatic download model weights
+Support for Yolov5/8, Detectron2, Mmdetection, Torchvision models - [x] Support
+for video and web application(Huggingface Spaces) - [x] Support for manual
+single multi box and point selection - [x] Support for pip installation - [x]
+Support for SAHI library
```

### Comparing `metaseg-0.4.2/README.md` & `metaseg-0.4.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -66,12 +66,12 @@
     input_box= [[100, 100, 400, 400]],
     multimask_output=False,
 
 )
 ```
 # Extra Features
 
-- [x] Support for video files
-- [x] Support for pip installation
-- [x] Support for web application
+- [x] Support for Yolov5/8, Detectron2, Mmdetection, Torchvision models
+- [x] Support for video and web application(Huggingface Spaces)
 - [x] Support for manual single multi box and point selection
-- [x] Support for automatic download model weights
+- [x] Support for pip installation
+- [x] Support for SAHI library
```

#### html2text {}

```diff
@@ -14,10 +14,11 @@
 point selection seg_manual_mask_generator = SegManualMaskPredictor().save_image
 ( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b input_point=[
 [100, 100], [200, 200]], input_label=[0, 1], input_box=[100, 100, 200, 200], #
 x,y,w,h multimask_output=False, ) # For multi box selection
 seg_manual_mask_generator = SegManualMaskPredictor().save_image( source="data/
 brain.png", model_type="vit_l", input_point=None, input_label=None, input_box=
 [[100, 100, 400, 400]], multimask_output=False, ) ``` # Extra Features - [x]
-Support for video files - [x] Support for pip installation - [x] Support for
-web application - [x] Support for manual single multi box and point selection -
-[x] Support for automatic download model weights
+Support for Yolov5/8, Detectron2, Mmdetection, Torchvision models - [x] Support
+for video and web application(Huggingface Spaces) - [x] Support for manual
+single multi box and point selection - [x] Support for pip installation - [x]
+Support for SAHI library
```

### Comparing `metaseg-0.4.2/metaseg/__init__.py` & `metaseg-0.4.4/metaseg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 # LICENSE file in the root directory of this source tree.
 
 from metaseg.generator.automatic_mask_generator import SamAutomaticMaskGenerator
 from metaseg.generator.build_sam import build_sam, build_sam_vit_b, build_sam_vit_h, build_sam_vit_l, sam_model_registry
 from metaseg.generator.predictor import SamPredictor
 from metaseg.mask_predictor import SegAutoMaskPredictor, SegManualMaskPredictor
 
-__version__ = "0.4.2"
+__version__ = "0.4.4"
```

### Comparing `metaseg-0.4.2/metaseg/generator/automatic_mask_generator.py` & `metaseg-0.4.4/metaseg/generator/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.2/metaseg/generator/build_sam.py` & `metaseg-0.4.4/metaseg/generator/build_sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.2/metaseg/generator/predictor.py` & `metaseg-0.4.4/metaseg/generator/predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.2/metaseg/mask_predictor.py` & `metaseg-0.4.4/metaseg/mask_predictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Dict, List, Optional
 
 import cv2
 import numpy as np
 import torch
+from tqdm import tqdm
 
 from metaseg import SamAutomaticMaskGenerator, SamPredictor, sam_model_registry
 from metaseg.utils import download_model, load_image, load_video
 
 
 class SegAutoMaskPredictor:
     def __init__(self):
@@ -55,17 +56,18 @@
         combined_mask = cv2.add(image, mask_image)
         cv2.imwrite("output.jpg", combined_mask)
 
         return "output.jpg"
 
     def save_video(self, source, model_type, points_per_side, points_per_batch, min_area):
         cap, out = load_video(source)
+        length = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
         colors = np.random.randint(0, 255, size=(256, 3), dtype=np.uint8)
 
-        while True:
+        for _ in tqdm(range(length)):
             ret, frame = cap.read()
             if not ret:
                 break
 
             image, anns = self.predict(frame, model_type, points_per_side, points_per_batch, min_area)
             if len(anns) == 0:
                 continue
```

### Comparing `metaseg-0.4.2/metaseg/modeling/common.py` & `metaseg-0.4.4/metaseg/modeling/common.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.2/metaseg/modeling/image_encoder.py` & `metaseg-0.4.4/metaseg/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.2/metaseg/modeling/mask_decoder.py` & `metaseg-0.4.4/metaseg/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.2/metaseg/modeling/prompt_encoder.py` & `metaseg-0.4.4/metaseg/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.2/metaseg/modeling/sam.py` & `metaseg-0.4.4/metaseg/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.2/metaseg/modeling/transformer.py` & `metaseg-0.4.4/metaseg/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.2/metaseg/sahi_predict.py` & `metaseg-0.4.4/metaseg/sahi_predict.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.2/metaseg/utils/amg.py` & `metaseg-0.4.4/metaseg/utils/amg.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.2/metaseg/utils/data_utils.py` & `metaseg-0.4.4/metaseg/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.2/metaseg/utils/file_utils.py` & `metaseg-0.4.4/metaseg/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.2/metaseg/utils/onnx.py` & `metaseg-0.4.4/metaseg/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.2/metaseg/utils/transforms.py` & `metaseg-0.4.4/metaseg/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.2/metaseg/webapp/app.py` & `metaseg-0.4.4/metaseg/webapp/app.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.2/metaseg.egg-info/PKG-INFO` & `metaseg-0.4.4/metaseg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.4.2
+Version: 0.4.4
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
@@ -78,12 +78,12 @@
     input_box= [[100, 100, 400, 400]],
     multimask_output=False,
 
 )
 ```
 # Extra Features
 
-- [x] Support for video files
-- [x] Support for pip installation
-- [x] Support for web application
+- [x] Support for Yolov5/8, Detectron2, Mmdetection, Torchvision models
+- [x] Support for video and web application(Huggingface Spaces)
 - [x] Support for manual single multi box and point selection
-- [x] Support for automatic download model weights
+- [x] Support for pip installation
+- [x] Support for SAHI library
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.4.2 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.4.4 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
@@ -18,10 +18,11 @@
 point selection seg_manual_mask_generator = SegManualMaskPredictor().save_image
 ( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b input_point=[
 [100, 100], [200, 200]], input_label=[0, 1], input_box=[100, 100, 200, 200], #
 x,y,w,h multimask_output=False, ) # For multi box selection
 seg_manual_mask_generator = SegManualMaskPredictor().save_image( source="data/
 brain.png", model_type="vit_l", input_point=None, input_label=None, input_box=
 [[100, 100, 400, 400]], multimask_output=False, ) ``` # Extra Features - [x]
-Support for video files - [x] Support for pip installation - [x] Support for
-web application - [x] Support for manual single multi box and point selection -
-[x] Support for automatic download model weights
+Support for Yolov5/8, Detectron2, Mmdetection, Torchvision models - [x] Support
+for video and web application(Huggingface Spaces) - [x] Support for manual
+single multi box and point selection - [x] Support for pip installation - [x]
+Support for SAHI library
```

### Comparing `metaseg-0.4.2/metaseg.egg-info/SOURCES.txt` & `metaseg-0.4.4/metaseg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.2/setup.py` & `metaseg-0.4.4/setup.py`

 * *Files identical despite different names*

