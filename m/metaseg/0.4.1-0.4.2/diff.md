# Comparing `tmp/metaseg-0.4.1.tar.gz` & `tmp/metaseg-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaseg-0.4.1.tar", last modified: Mon Apr 10 09:24:19 2023, max compression
+gzip compressed data, was "metaseg-0.4.2.tar", last modified: Mon Apr 10 17:58:53 2023, max compression
```

## Comparing `metaseg-0.4.1.tar` & `metaseg-0.4.2.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 09:24:19.561351 metaseg-0.4.1/
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.4.1/LICENSE
--rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.4.1/MANIFEST.in
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2505 2023-04-10 09:24:19.561351 metaseg-0.4.1/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2231 2023-04-10 09:24:07.000000 metaseg-0.4.1/README.md
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 09:24:19.554684 metaseg-0.4.1/metaseg/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      556 2023-04-10 09:24:07.000000 metaseg-0.4.1/metaseg/__init__.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 09:24:19.558018 metaseg-0.4.1/metaseg/generator/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-09 13:51:55.000000 metaseg-0.4.1/metaseg/generator/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-09 13:58:07.000000 metaseg-0.4.1/metaseg/generator/automatic_mask_generator.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-06 18:52:09.000000 metaseg-0.4.1/metaseg/generator/build_sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-06 18:52:09.000000 metaseg-0.4.1/metaseg/generator/predictor.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6911 2023-04-10 09:24:07.000000 metaseg-0.4.1/metaseg/mask_predictor.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 09:24:19.558018 metaseg-0.4.1/metaseg/modeling/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.4.1/metaseg/modeling/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.4.1/metaseg/modeling/common.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.4.1/metaseg/modeling/image_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.4.1/metaseg/modeling/mask_decoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.4.1/metaseg/modeling/prompt_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.4.1/metaseg/modeling/sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.4.1/metaseg/modeling/transformer.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 09:24:19.561351 metaseg-0.4.1/metaseg/utils/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      310 2023-04-09 10:19:56.000000 metaseg-0.4.1/metaseg/utils/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.4.1/metaseg/utils/amg.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)      518 2023-04-09 10:19:56.000000 metaseg-0.4.1/metaseg/utils/data_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-08 17:15:08.000000 metaseg-0.4.1/metaseg/utils/file_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.4.1/metaseg/utils/onnx.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.4.1/metaseg/utils/transforms.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 09:24:19.561351 metaseg-0.4.1/metaseg/webapp/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-09 10:19:56.000000 metaseg-0.4.1/metaseg/webapp/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-09 10:19:56.000000 metaseg-0.4.1/metaseg/webapp/app.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 09:24:19.554684 metaseg-0.4.1/metaseg.egg-info/
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2505 2023-04-10 09:24:19.000000 metaseg-0.4.1/metaseg.egg-info/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)      834 2023-04-10 09:24:19.000000 metaseg-0.4.1/metaseg.egg-info/SOURCES.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-10 09:24:19.000000 metaseg-0.4.1/metaseg.egg-info/dependency_links.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      226 2023-04-10 09:24:19.000000 metaseg-0.4.1/metaseg.egg-info/requires.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-10 09:24:19.000000 metaseg-0.4.1/metaseg.egg-info/top_level.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.4.1/pyproject.toml
--rw-r--r--   0 kadir     (1000) kadir     (1001)      139 2023-04-08 09:21:23.000000 metaseg-0.4.1/requirements.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-10 09:24:19.561351 metaseg-0.4.1/setup.cfg
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.4.1/setup.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 17:58:53.921825 metaseg-0.4.2/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.4.2/LICENSE
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.4.2/MANIFEST.in
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2505 2023-04-10 17:58:53.921825 metaseg-0.4.2/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2231 2023-04-10 09:24:07.000000 metaseg-0.4.2/README.md
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 17:58:53.915158 metaseg-0.4.2/metaseg/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      556 2023-04-10 17:56:20.000000 metaseg-0.4.2/metaseg/__init__.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 17:58:53.918491 metaseg-0.4.2/metaseg/generator/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-09 13:51:55.000000 metaseg-0.4.2/metaseg/generator/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-09 13:58:07.000000 metaseg-0.4.2/metaseg/generator/automatic_mask_generator.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-06 18:52:09.000000 metaseg-0.4.2/metaseg/generator/build_sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-06 18:52:09.000000 metaseg-0.4.2/metaseg/generator/predictor.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6913 2023-04-10 17:57:10.000000 metaseg-0.4.2/metaseg/mask_predictor.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 17:58:53.918491 metaseg-0.4.2/metaseg/modeling/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.4.2/metaseg/modeling/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.4.2/metaseg/modeling/common.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.4.2/metaseg/modeling/image_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.4.2/metaseg/modeling/mask_decoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.4.2/metaseg/modeling/prompt_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.4.2/metaseg/modeling/sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.4.2/metaseg/modeling/transformer.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1205 2023-04-10 17:56:26.000000 metaseg-0.4.2/metaseg/sahi_predict.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 17:58:53.921825 metaseg-0.4.2/metaseg/utils/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      310 2023-04-09 10:19:56.000000 metaseg-0.4.2/metaseg/utils/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.4.2/metaseg/utils/amg.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      518 2023-04-09 10:19:56.000000 metaseg-0.4.2/metaseg/utils/data_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-08 17:15:08.000000 metaseg-0.4.2/metaseg/utils/file_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.4.2/metaseg/utils/onnx.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.4.2/metaseg/utils/transforms.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 17:58:53.921825 metaseg-0.4.2/metaseg/webapp/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-09 10:19:56.000000 metaseg-0.4.2/metaseg/webapp/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-09 10:19:56.000000 metaseg-0.4.2/metaseg/webapp/app.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 17:58:53.918491 metaseg-0.4.2/metaseg.egg-info/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2505 2023-04-10 17:58:53.000000 metaseg-0.4.2/metaseg.egg-info/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      858 2023-04-10 17:58:53.000000 metaseg-0.4.2/metaseg.egg-info/SOURCES.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-10 17:58:53.000000 metaseg-0.4.2/metaseg.egg-info/dependency_links.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      226 2023-04-10 17:58:53.000000 metaseg-0.4.2/metaseg.egg-info/requires.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-10 17:58:53.000000 metaseg-0.4.2/metaseg.egg-info/top_level.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.4.2/pyproject.toml
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      139 2023-04-08 09:21:23.000000 metaseg-0.4.2/requirements.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-10 17:58:53.921825 metaseg-0.4.2/setup.cfg
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.4.2/setup.py
```

### Comparing `metaseg-0.4.1/LICENSE` & `metaseg-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.1/PKG-INFO` & `metaseg-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.4.1
+Version: 0.4.2
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.4.1 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.4.2 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
```

### Comparing `metaseg-0.4.1/README.md` & `metaseg-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.1/metaseg/__init__.py` & `metaseg-0.4.2/metaseg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 # LICENSE file in the root directory of this source tree.
 
 from metaseg.generator.automatic_mask_generator import SamAutomaticMaskGenerator
 from metaseg.generator.build_sam import build_sam, build_sam_vit_b, build_sam_vit_h, build_sam_vit_l, sam_model_registry
 from metaseg.generator.predictor import SamPredictor
 from metaseg.mask_predictor import SegAutoMaskPredictor, SegManualMaskPredictor
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
```

### Comparing `metaseg-0.4.1/metaseg/generator/automatic_mask_generator.py` & `metaseg-0.4.2/metaseg/generator/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.1/metaseg/generator/build_sam.py` & `metaseg-0.4.2/metaseg/generator/build_sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.1/metaseg/generator/predictor.py` & `metaseg-0.4.2/metaseg/generator/predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.1/metaseg/mask_predictor.py` & `metaseg-0.4.2/metaseg/mask_predictor.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,10 +188,10 @@
                 image = self.load_box(box.cpu().numpy(), image)
 
         elif type(input_box[0]) == int:
             mask_image = self.load_mask(anns, True)
             image = self.load_box(input_box, image)
 
         combined_mask = cv2.add(image, mask_image)
-        cv2.write(output_path, combined_mask)
+        cv2.imwrite(output_path, combined_mask)
 
         return output_path
```

### Comparing `metaseg-0.4.1/metaseg/modeling/common.py` & `metaseg-0.4.2/metaseg/modeling/common.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.1/metaseg/modeling/image_encoder.py` & `metaseg-0.4.2/metaseg/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.1/metaseg/modeling/mask_decoder.py` & `metaseg-0.4.2/metaseg/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.1/metaseg/modeling/prompt_encoder.py` & `metaseg-0.4.2/metaseg/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.1/metaseg/modeling/sam.py` & `metaseg-0.4.2/metaseg/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.1/metaseg/modeling/transformer.py` & `metaseg-0.4.2/metaseg/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.1/metaseg/utils/amg.py` & `metaseg-0.4.2/metaseg/utils/amg.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.1/metaseg/utils/data_utils.py` & `metaseg-0.4.2/metaseg/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.1/metaseg/utils/file_utils.py` & `metaseg-0.4.2/metaseg/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.1/metaseg/utils/onnx.py` & `metaseg-0.4.2/metaseg/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.1/metaseg/utils/transforms.py` & `metaseg-0.4.2/metaseg/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.1/metaseg/webapp/app.py` & `metaseg-0.4.2/metaseg/webapp/app.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.1/metaseg.egg-info/PKG-INFO` & `metaseg-0.4.2/metaseg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.4.1
+Version: 0.4.2
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.4.1 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.4.2 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
```

### Comparing `metaseg-0.4.1/metaseg.egg-info/SOURCES.txt` & `metaseg-0.4.2/metaseg.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 metaseg/__init__.py
 metaseg/mask_predictor.py
+metaseg/sahi_predict.py
 metaseg.egg-info/PKG-INFO
 metaseg.egg-info/SOURCES.txt
 metaseg.egg-info/dependency_links.txt
 metaseg.egg-info/requires.txt
 metaseg.egg-info/top_level.txt
 metaseg/generator/__init__.py
 metaseg/generator/automatic_mask_generator.py
```

### Comparing `metaseg-0.4.1/setup.py` & `metaseg-0.4.2/setup.py`

 * *Files identical despite different names*

