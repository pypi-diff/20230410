# Comparing `tmp/waffle_hub-0.1.5.tar.gz` & `tmp/waffle_hub-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waffle_hub-0.1.5.tar", last modified: Fri Apr  7 03:37:16 2023, max compression
+gzip compressed data, was "waffle_hub-0.1.6.tar", last modified: Mon Apr 10 11:42:10 2023, max compression
```

## Comparing `waffle_hub-0.1.5.tar` & `waffle_hub-0.1.6.tar`

### file list

```diff
@@ -1,44 +1,51 @@
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-07 03:37:16.645641 waffle_hub-0.1.5/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    35149 2023-03-20 23:40:26.000000 waffle_hub-0.1.5/LICENSE
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-03-20 23:40:26.000000 waffle_hub-0.1.5/MANIFEST.in
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1966 2023-04-07 03:37:16.645641 waffle_hub-0.1.5/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      885 2023-04-03 23:38:22.000000 waffle_hub-0.1.5/README.md
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      213 2023-04-03 23:38:22.000000 waffle_hub-0.1.5/requirements.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-04-07 03:37:16.645641 waffle_hub-0.1.5/setup.cfg
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2643 2023-04-03 23:38:22.000000 waffle_hub-0.1.5/setup.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-07 03:37:16.641641 waffle_hub-0.1.5/tests/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     5470 2023-04-07 00:35:34.000000 waffle_hub-0.1.5/tests/test_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-07 03:37:16.641641 waffle_hub-0.1.5/waffle_hub/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2500 2023-04-07 03:36:43.000000 waffle_hub-0.1.5/waffle_hub/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-07 03:37:16.641641 waffle_hub-0.1.5/waffle_hub/hub/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-03-28 04:35:11.000000 waffle_hub-0.1.5/waffle_hub/hub/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-07 03:37:16.641641 waffle_hub-0.1.5/waffle_hub/hub/adapter/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-03-28 04:35:11.000000 waffle_hub-0.1.5/waffle_hub/hub/adapter/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-07 03:37:16.641641 waffle_hub-0.1.5/waffle_hub/hub/adapter/tx_model/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       63 2023-03-28 04:35:11.000000 waffle_hub-0.1.5/waffle_hub/hub/adapter/tx_model/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-07 03:37:16.641641 waffle_hub-0.1.5/waffle_hub/hub/adapter/tx_model/configs/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      129 2023-03-28 04:35:11.000000 waffle_hub-0.1.5/waffle_hub/hub/adapter/tx_model/configs/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2573 2023-03-28 04:35:11.000000 waffle_hub-0.1.5/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1865 2023-03-28 04:35:11.000000 waffle_hub-0.1.5/waffle_hub/hub/adapter/tx_model/configs/model_cfg.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     8535 2023-04-03 23:38:22.000000 waffle_hub-0.1.5/waffle_hub/hub/adapter/tx_model/tx_model_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-07 03:37:16.641641 waffle_hub-0.1.5/waffle_hub/hub/adapter/ultralytics/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       74 2023-03-28 04:35:11.000000 waffle_hub-0.1.5/waffle_hub/hub/adapter/ultralytics/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    10566 2023-04-07 00:35:34.000000 waffle_hub-0.1.5/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    22096 2023-04-07 03:36:43.000000 waffle_hub-0.1.5/waffle_hub/hub/base_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-07 03:37:16.641641 waffle_hub-0.1.5/waffle_hub/hub/model/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-03-20 23:40:26.000000 waffle_hub-0.1.5/waffle_hub/hub/model/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     5026 2023-04-03 23:38:22.000000 waffle_hub-0.1.5/waffle_hub/hub/model/wrapper.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1247 2023-03-20 23:40:26.000000 waffle_hub-0.1.5/waffle_hub/run.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-07 03:37:16.641641 waffle_hub-0.1.5/waffle_hub/schemas/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-03-20 23:40:26.000000 waffle_hub-0.1.5/waffle_hub/schemas/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      679 2023-03-20 23:40:26.000000 waffle_hub-0.1.5/waffle_hub/schemas/configs.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-07 03:37:16.645641 waffle_hub-0.1.5/waffle_hub/utils/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-03-20 23:40:26.000000 waffle_hub-0.1.5/waffle_hub/utils/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     5252 2023-04-03 23:38:22.000000 waffle_hub-0.1.5/waffle_hub/utils/callback.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     5030 2023-04-03 23:38:22.000000 waffle_hub-0.1.5/waffle_hub/utils/image.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-07 03:37:16.641641 waffle_hub-0.1.5/waffle_hub.egg-info/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1966 2023-04-07 03:37:16.000000 waffle_hub-0.1.5/waffle_hub.egg-info/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      932 2023-04-07 03:37:16.000000 waffle_hub-0.1.5/waffle_hub.egg-info/SOURCES.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-04-07 03:37:16.000000 waffle_hub-0.1.5/waffle_hub.egg-info/dependency_links.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      172 2023-04-07 03:37:16.000000 waffle_hub-0.1.5/waffle_hub.egg-info/requires.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       11 2023-04-07 03:37:16.000000 waffle_hub-0.1.5/waffle_hub.egg-info/top_level.txt
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.650711 waffle_hub-0.1.6/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    35149 2023-03-20 23:40:26.000000 waffle_hub-0.1.6/LICENSE
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-03-20 23:40:26.000000 waffle_hub-0.1.6/MANIFEST.in
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1966 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      885 2023-04-03 23:38:22.000000 waffle_hub-0.1.6/README.md
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      213 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/requirements.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-04-10 11:42:10.650711 waffle_hub-0.1.6/setup.cfg
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2643 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/setup.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/tests/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     6036 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/tests/test_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/waffle_hub/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2500 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/waffle_hub/experimental/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/experimental/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2986 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/experimental/serve.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/waffle_hub/hub/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.6/waffle_hub/hub/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/waffle_hub/hub/adapter/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.6/waffle_hub/hub/adapter/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/waffle_hub/hub/adapter/tx_model/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       63 2023-04-10 11:40:54.000000 waffle_hub-0.1.6/waffle_hub/hub/adapter/tx_model/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/waffle_hub/hub/adapter/tx_model/configs/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      129 2023-04-10 11:40:54.000000 waffle_hub-0.1.6/waffle_hub/hub/adapter/tx_model/configs/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2573 2023-04-10 11:40:54.000000 waffle_hub-0.1.6/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1793 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/hub/adapter/tx_model/configs/model_cfg.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     8318 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/hub/adapter/tx_model/tx_model_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/waffle_hub/hub/adapter/ultralytics/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       74 2023-04-10 11:40:54.000000 waffle_hub-0.1.6/waffle_hub/hub/adapter/ultralytics/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    10931 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    21077 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/hub/base_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/waffle_hub/hub/model/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.6/waffle_hub/hub/model/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     6340 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/hub/model/wrapper.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1247 2023-04-10 11:40:54.000000 waffle_hub-0.1.6/waffle_hub/run.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/waffle_hub/schema/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/schema/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      614 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/schema/base_schema.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1257 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/schema/configs.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1170 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/schema/data.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/waffle_hub/utils/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.6/waffle_hub/utils/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     5252 2023-04-10 11:40:54.000000 waffle_hub-0.1.6/waffle_hub/utils/callback.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3385 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/utils/data.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2239 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/utils/draw.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/waffle_hub.egg-info/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1966 2023-04-10 11:42:10.000000 waffle_hub-0.1.6/waffle_hub.egg-info/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1119 2023-04-10 11:42:10.000000 waffle_hub-0.1.6/waffle_hub.egg-info/SOURCES.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-04-10 11:42:10.000000 waffle_hub-0.1.6/waffle_hub.egg-info/dependency_links.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       44 2023-04-10 11:42:10.000000 waffle_hub-0.1.6/waffle_hub.egg-info/entry_points.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      172 2023-04-10 11:42:10.000000 waffle_hub-0.1.6/waffle_hub.egg-info/requires.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       11 2023-04-10 11:42:10.000000 waffle_hub-0.1.6/waffle_hub.egg-info/top_level.txt
```

### Comparing `waffle_hub-0.1.5/LICENSE` & `waffle_hub-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.5/PKG-INFO` & `waffle_hub-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle_hub
-Version: 0.1.5
+Version: 0.1.6
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle_hub Version: 0.1.5 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle_hub Version: 0.1.6 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `waffle_hub-0.1.5/README.md` & `waffle_hub-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.5/setup.py` & `waffle_hub-0.1.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,9 +62,9 @@
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Scientific/Engineering :: Image Recognition",
         "Operating System :: POSIX :: Linux",
         # 'Operating System :: MacOS',
         # 'Operating System :: Microsoft :: Windows',
     ],
     keywords="machine-learning, deep-learning, vision, ML, DL, AI, YOLO, Ultralytics, SNUAILAB",
-    # entry_points={"console_scripts": ["wh = waffle_hub.run:app"]},
+    entry_points={"console_scripts": ["wu = waffle_utils.run:app"]},
 )
```

### Comparing `waffle_hub-0.1.5/tests/test_hub.py` & `waffle_hub-0.1.6/tests/test_hub.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import time
 from pathlib import Path
 
 import pytest
+import torch
 from waffle_utils.dataset import Dataset
 from waffle_utils.file import io, network
 
 from waffle_hub.hub.adapter.ultralytics import UltralyticsHub
 from waffle_hub.utils.callback import (
     ExportCallback,
     InferenceCallback,
@@ -34,20 +35,20 @@
 
 def test_ultralytics_object_detection(tmpdir: Path, dummy_dataset: Dataset):
 
     export_dir = dummy_dataset.export("yolo_detection")
 
     name = "test_det"
 
-    hub = UltralyticsHub(
+    hub = UltralyticsHub.new(
         name=name,
         task="object_detection",
         model_type="yolov8",
         model_size="n",
-        classes=["1", "2"],
+        categories=["1", "2"],
         root_dir=tmpdir,
     )
     hub = UltralyticsHub.load(name=name, root_dir=tmpdir)
     hub: UltralyticsHub = UltralyticsHub.from_model_config(
         name=name,
         model_config_file=tmpdir / name / UltralyticsHub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
@@ -73,27 +74,37 @@
     )
     assert inference_callback.get_progress() == 1
     assert Path(inference_callback.inference_dir).exists()
 
     export_callback: ExportCallback = hub.export()
     assert Path(export_callback.export_file).exists()
 
+    model = hub.get_model()
+
+    layer_names = model.get_layer_names()
+    assert len(layer_names) > 0
+
+    x = torch.randn(4, 3, 64, 64)
+    layer_name = layer_names[-1]
+    x, feature_maps = model.get_feature_maps(x, layer_name)
+    assert len(feature_maps) == 1
+
 
 def test_ultralytics_classification(tmpdir: Path, dummy_dataset: Dataset):
 
     export_dir = dummy_dataset.export("yolo_classification")
 
     name = "test_cls"
 
-    hub = UltralyticsHub(
+    hub = UltralyticsHub.new(
         name=name,
         task="classification",
         model_type="yolov8",
         model_size="n",
-        classes=["1", "2"],
+        categories=["1", "2"],
         root_dir=tmpdir,
     )
     hub = UltralyticsHub.load(name=name, root_dir=tmpdir)
     hub: UltralyticsHub = UltralyticsHub.from_model_config(
         name=name,
         model_config_file=tmpdir / name / UltralyticsHub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
@@ -119,27 +130,37 @@
     )
     assert inference_callback.get_progress() == 1
     assert Path(inference_callback.inference_dir).exists()
 
     export_callback: ExportCallback = hub.export()
     assert Path(export_callback.export_file).exists()
 
+    model = hub.get_model()
+
+    layer_names = model.get_layer_names()
+    assert len(layer_names) > 0
+
+    x = torch.randn(4, 3, 64, 64)
+    layer_name = layer_names[-1]
+    x, feature_maps = model.get_feature_maps(x, layer_name)
+    assert len(feature_maps) == 1
+
 
 def test_non_hold(tmpdir: Path, dummy_dataset: Dataset):
 
     export_dir = dummy_dataset.export("yolo_detection")
 
     name = "test_det"
 
-    hub = UltralyticsHub(
+    hub = UltralyticsHub.new(
         name=name,
         task="object_detection",
         model_type="yolov8",
         model_size="n",
-        classes=["1", "2"],
+        categories=["1", "2"],
         root_dir=tmpdir,
     )
     hub = UltralyticsHub.load(name=name, root_dir=tmpdir)
     hub: UltralyticsHub = UltralyticsHub.from_model_config(
         name=name,
         model_config_file=tmpdir / name / UltralyticsHub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
```

### Comparing `waffle_hub-0.1.5/waffle_hub/__init__.py` & `waffle_hub-0.1.6/waffle_hub/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 
 import importlib
 import warnings
 from collections import OrderedDict
 
 from tabulate import tabulate
 
@@ -27,15 +27,15 @@
     ]
 
     e.msg = "Need to install torch\n" + "\n".join(strings)
     raise e
 
 # backend supports
 _backends = OrderedDict(
-    {"ultralytics": ["8.0.54"], "autocare_tx_model": ["0.2.0"]}
+    {"ultralytics": ["8.0.72"], "autocare_tx_model": ["0.2.0"]}
 )
 
 
 def get_backends() -> dict:
     return _backends
```

### Comparing `waffle_hub-0.1.5/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py` & `waffle_hub-0.1.6/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.5/waffle_hub/hub/adapter/tx_model/configs/model_cfg.py` & `waffle_hub-0.1.6/waffle_hub/hub/adapter/tx_model/configs/model_cfg.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,63 @@
 def get_model_config(
     model_type: str,
     model_size: str,
-    classes: list[str],
+    categories: list[str],
     seed: int,
     letter_box: bool,
     epochs: int,
 ):
     return {
         "task": model_type,
         "model": {
             "model_size": model_size,
-            "backbone":{
-                "name":"YOLOv5Backbone",
-                "focus": False
-            },
-            "neck": {
-                "name":"YOLOv5Neck"
-            },
+            "backbone": {"name": "YOLOv5Backbone", "focus": False},
+            "neck": {"name": "YOLOv5Neck"},
             "head": {
                 "name": "YOLOv5Head",
                 "anchors": [
                     [10, 13, 16, 30, 33, 23],
                     [30, 61, 62, 45, 59, 119],
-                    [116, 90, 156, 198, 373, 326]
-                ]
-            }
+                    [116, 90, 156, 198, 373, 326],
+                ],
+            },
         },
         "loss": {
             "total_loss": {
                 "name": "YoloLoss",
                 "params": {
                     "hyp": {
                         "box": 0.05,
                         "cls": 0.3,
                         "cls_pw": 1.0,
                         "obj": 0.7,
                         "obj_pw": 1.0,
                         "anchor_t": 4.0,
                         "fl_alpha": -1,
                         "fl_gamma": 0.0,
-                        "label_smoothing": 0.0
+                        "label_smoothing": 0.0,
                     }
-                }
+                },
             }
         },
         "optim": {
             "name": "SGD",
             "lr": 0.001,
             "momentum": 0.937,
-            "weight_decay": 0.0005
-        }, 
+            "weight_decay": 0.0005,
+        },
         "lr_cfg": {
             "type": "cosine",
             "warmup": True,
             "warmup_epochs": 0.5,
-            "lrf": 0.1
-        },
-        "ema_cfg":{
-            "burn_in_epoch" : 1
+            "lrf": 0.1,
         },
+        "ema_cfg": {"burn_in_epoch": 1},
         "max_epoch": epochs,
         "nms_thresh": 0.65,
         "min_score": 0.25,
         "detections_per_img": 300,
         "seed": seed,
-        "classes": classes,
-        "num_classes": len(classes),
-        "letter_box": letter_box
-    }
+        "categories": categories,
+        "num_categories": len(categories),
+        "letter_box": letter_box,
+    }
```

### Comparing `waffle_hub-0.1.5/waffle_hub/hub/adapter/tx_model/tx_model_hub.py` & `waffle_hub-0.1.6/waffle_hub/hub/adapter/tx_model/tx_model_hub.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     def __init__(
         self,
         name: str,
         task: str = None,
         model_type: str = None,
         model_size: str = None,
-        classes: Union[list[dict], list] = None,
+        categories: Union[list[dict], list] = None,
         root_dir: str = None,
         backend: str = None,
         version: str = None,
     ):
         """Create Tx Model Hub Class. Do not use this class directly. Use TxModelHub.new() instead."""
 
         if backend is not None and backend != BACKEND_NAME:
@@ -82,63 +82,63 @@
         super().__init__(
             name=name,
             backend=BACKEND_NAME,
             version=BACKEND_VERSION,
             task=task,
             model_type=model_type,
             model_size=model_size,
-            classes=classes,
+            categories=categories,
             root_dir=root_dir,
         )
 
     @classmethod
     def new(
         cls,
         name: str,
         task: str = None,
         model_type: str = None,
         model_size: str = None,
-        classes: Union[list[dict], list] = None,
+        categories: Union[list[dict], list] = None,
         root_dir: str = None,
     ):
         """Create Tx Model Hub.
 
         Args:
             name (str): Hub name
             task (str, optional): Task Name. See UltralyticsHub.TASKS. Defaults to None.
             model_type (str, optional): Model Type. See UltralyticsHub.MODEL_TYPES. Defaults to None.
             model_size (str, optional): Model Size. See UltralyticsHub.MODEL_SIZES. Defaults to None.
-            classes (Union[list[dict], list]): class dictionary or list. [{"supercategory": "name"}, ] or ["name",].
+            categories (Union[list[dict], list]): class dictionary or list. [{"supercategory": "name"}, ] or ["name",].
             root_dir (str, optional): Root directory of hub repository. Defaults to None.
         """
         return cls(
             name=name,
             task=task,
             model_type=model_type,
             model_size=model_size,
-            classes=classes,
+            categories=categories,
             root_dir=root_dir,
         )
 
     # Hub Utils
     def get_preprocess(self, task: str, *args, **kwargs):
 
         if task == "object_detection":
             normalize = T.Normalize([0, 0, 0], [1, 1, 1], inplace=True)
 
-            def preprocess(x):
+            def preprocess(x, *args, **kwargs):
                 return normalize(x)
 
         return preprocess
 
     def get_postprocess(self, task: str, *args, **kwargs):
 
         if task == "object_detection":
 
-            def inner(x: torch.Tensor):
+            def inner(x: torch.Tensor, *args, **kwargs):
                 return x
 
         return inner
 
     def get_metrics(self) -> list[dict]:
         """Get metrics from tensorboard log directory.
         Args:
@@ -190,15 +190,15 @@
         )
         ctx.data_config = self.artifact_dir / "data.json"
         io.save_json(data_config, ctx.data_config, create_directory=True)
 
         model_config = get_model_config(
             self.model_type,
             self.model_size,
-            [x["name"] for x in self.classes],
+            [x["name"] for x in self.categories],
             ctx.seed,
             ctx.letter_box,
             ctx.epochs,
         )
         ctx.model_config = self.artifact_dir / "model.json"
         io.save_json(model_config, ctx.model_config, create_directory=True)
 
@@ -237,40 +237,34 @@
             self.artifact_dir / "train" / "last_epoch_ckpt.pth",
             self.last_ckpt_file,
             create_directory=True,
         )
         io.save_json(self.get_metrics(), self.metric_file)
 
     # Inference Hook
-    def get_model(
-        self, image_size: Union[int, list] = None, parser: ResultParser = None
-    ):
+    def get_model(self):
         """Get model.
-        Args:
-            image_size (Union[int, list], optional): Image size. Defaults to None.
-            parser (ResultParser, optional): Result parser. Defaults to None.
         Returns:
             ModelWrapper: Model wrapper
         """
         self.check_train_sanity()
 
         # get adapt functions
         preprocess = self.get_preprocess(self.task)
         postprocess = self.get_postprocess(self.task)
 
         # get model
-        classes = [x["name"] for x in self.classes]
+        categories = [x["name"] for x in self.categories]
         cfg = io.load_json(self.artifact_dir / "model.json")
-        cfg["model"]["head"]["num_classes"] = len(classes)
+        cfg["model"]["head"]["num_categories"] = len(categories)
         cfg["ckpt"] = str(self.best_ckpt_file)
-        cfg["classes"] = classes
-        cfg["num_classes"] = (len(classes),)
-        model, classes = build_model(AttrDict(cfg), strict=True)
+        cfg["categories"] = categories
+        cfg["num_categories"] = (len(categories),)
+        model, categories = build_model(AttrDict(cfg), strict=True)
 
         model = ModelWrapper(
             model=model.eval(),
             preprocess=preprocess,
             postprocess=postprocess,
-            parser=parser if parser else None,
         )
 
         return model
```

### Comparing `waffle_hub-0.1.5/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py` & `waffle_hub-0.1.6/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 from typing import Union
 
 import torch
 from torchvision import transforms as T
 from ultralytics import YOLO
 from waffle_utils.file import io
 
-from waffle_hub.hub.base_hub import BaseHub, InferenceContext, TrainContext
-from waffle_hub.hub.model.wrapper import ModelWrapper, ResultParser
+from waffle_hub.hub.base_hub import BaseHub
+from waffle_hub.hub.model.wrapper import ModelWrapper
+from waffle_hub.schema.configs import TrainConfig
 from waffle_hub.utils.callback import TrainCallback
 
 
 class UltralyticsHub(BaseHub):
 
     # Common
     MODEL_TYPES = {
@@ -40,21 +41,38 @@
     }
     TASK_SUFFIX = {
         "detect": "",
         "classify": "-cls",
         # "segment": "-seg",
     }
 
+    DEFAULT_PARAMAS = {
+        "object_detection": {
+            "epochs": 50,
+            "image_size": [640, 640],
+            "learning_rate": 0.01,
+            "letter_box": True,
+            "batch_size": 16,
+        },
+        "classification": {
+            "epochs": 50,
+            "image_size": [224, 224],
+            "learning_rate": 0.01,
+            "letter_box": False,
+            "batch_size": 16,
+        },
+    }
+
     def __init__(
         self,
         name: str,
         task: str = None,
         model_type: str = None,
         model_size: str = None,
-        classes: Union[list[dict], list] = None,
+        categories: Union[list[dict], list] = None,
         root_dir: str = None,
         backend: str = None,
         version: str = None,
     ):
         """Create Ultralytics Hub Class. Do not use this class directly. Use UltralyticsHub.new() instead."""
 
         if backend is not None and backend != BACKEND_NAME:
@@ -71,85 +89,81 @@
         super().__init__(
             name=name,
             backend=BACKEND_NAME,
             version=BACKEND_VERSION,
             task=task,
             model_type=model_type,
             model_size=model_size,
-            classes=classes,
+            categories=categories,
             root_dir=root_dir,
         )
 
         self.backend_task_name = self.TASK_MAP[self.task]
 
     @classmethod
     def new(
         cls,
         name: str,
         task: str = None,
         model_type: str = None,
         model_size: str = None,
-        classes: Union[list[dict], list] = None,
+        categories: Union[list[dict], list] = None,
         root_dir: str = None,
     ):
         """Create Ultralytics Hub.
 
         Args:
             name (str): Hub name
             task (str, optional): Task Name. See UltralyticsHub.TASKS. Defaults to None.
             model_type (str, optional): Model Type. See UltralyticsHub.MODEL_TYPES. Defaults to None.
             model_size (str, optional): Model Size. See UltralyticsHub.MODEL_SIZES. Defaults to None.
-            classes (Union[list[dict], list]): class dictionary or list. [{"supercategory": "name"}, ] or ["name",].
+            categories (Union[list[dict], list]): class dictionary or list. [{"supercategory": "name"}, ] or ["name",].
             root_dir (str, optional): Root directory of hub repository. Defaults to None.
         """
         return cls(
             name=name,
             task=task,
             model_type=model_type,
             model_size=model_size,
-            classes=classes,
+            categories=categories,
             root_dir=root_dir,
         )
 
     # Hub Utils
     def get_preprocess(self, task: str, *args, **kwargs):
 
         if task == "classification":
             normalize = T.Normalize([0, 0, 0], [1, 1, 1], inplace=True)
 
-            def preprocess(x):
+            def preprocess(x, *args, **kwargs):
                 return normalize(x)
 
         elif task == "object_detection":
             normalize = T.Normalize([0, 0, 0], [1, 1, 1], inplace=True)
 
-            def preprocess(x):
+            def preprocess(x, *args, **kwargs):
                 return normalize(x)
 
         else:
             raise NotImplementedError(f"Task {task} is not implemented.")
 
         return preprocess
 
     def get_postprocess(self, task: str, *args, **kwargs):
 
         if task == "classification":
 
-            def inner(x: torch.Tensor):
+            def inner(x: torch.Tensor, *args, **kwargs):
                 return [x]
 
         elif task == "object_detection":
-            image_size = kwargs.get("image_size")
-            image_size = (
-                image_size
-                if isinstance(image_size, list)
-                else [image_size, image_size]
-            )
 
-            def inner(x: torch.Tensor):
+            def inner(
+                x: torch.Tensor, image_size: tuple[int, int], *args, **kwargs
+            ):
                 x = x[0]  # x[0]: prediction, x[1]: TODO: what is this...?
                 x = x.transpose(1, 2)
 
                 cxcywh = x[:, :, :4]
                 cx, cy, w, h = torch.unbind(cxcywh, dim=-1)
                 x1 = cx - w / 2
                 y1 = cy - h / 2
@@ -199,111 +213,113 @@
                     }
                 )
             metrics.append(metric)
 
         return metrics
 
     # Train Hook
-    def on_train_start(self, ctx: TrainContext):
+    def on_train_start(self, cfg: TrainConfig):
+
         # set data
-        ctx.dataset_path: Path = Path(ctx.dataset_path)
+        cfg.dataset_path: Path = Path(cfg.dataset_path)
         if self.backend_task_name in ["detect", "segment"]:
-            if ctx.dataset_path.suffix not in [".yml", ".yaml"]:
-                yaml_files = list(ctx.dataset_path.glob("*.yaml")) + list(
-                    ctx.dataset_path.glob("*.yml")
+            if cfg.dataset_path.suffix not in [".yml", ".yaml"]:
+                yaml_files = list(cfg.dataset_path.glob("*.yaml")) + list(
+                    cfg.dataset_path.glob("*.yml")
                 )
                 if len(yaml_files) != 1:
                     raise FileNotFoundError(
                         f"Ambiguous data file. Detected files: {yaml_files}"
                     )
-                ctx.dataset_path = Path(yaml_files[0]).absolute()
+                cfg.dataset_path = Path(yaml_files[0]).absolute()
             else:
-                ctx.dataset_path = ctx.dataset_path.absolute()
+                cfg.dataset_path = cfg.dataset_path.absolute()
         elif self.backend_task_name == "classify":
 
             from torchvision.datasets.folder import ImageFolder
 
-            def find_classes(_, directory: str):
+            def find_categories(_, directory: str):
                 return directory, {
-                    v["name"]: i for i, v in enumerate(self.classes)
+                    v["name"]: i for i, v in enumerate(self.categories)
                 }
 
-            ImageFolder.find_classes = find_classes
+            ImageFolder.find_categories = find_categories
 
-            if not ctx.dataset_path.is_dir():
+            if not cfg.dataset_path.is_dir():
                 raise ValueError(
-                    f"Classification dataset should be directory. Not {ctx.dataset_path}"
+                    f"Classification dataset should be directory. Not {cfg.dataset_path}"
                 )
-            ctx.dataset_path = ctx.dataset_path.absolute()
-        ctx.dataset_path = str(ctx.dataset_path)
+            cfg.dataset_path = cfg.dataset_path.absolute()
+        cfg.dataset_path = str(cfg.dataset_path)
 
         # pretrained model
-        ctx.pretrained_model = (
-            ctx.pretrained_model
-            if ctx.pretrained_model
+        cfg.pretrained_model = (
+            cfg.pretrained_model
+            if cfg.pretrained_model
             else self.model_type
             + self.model_size
             + self.TASK_SUFFIX[self.backend_task_name]
             + ".pt"
         )
 
-    def training(self, ctx: TrainContext, callback: TrainCallback):
+        # overwrite train config with default config
+        for k, v in cfg.to_dict().items():
+            if v is None:
+                setattr(cfg, k, self.DEFAULT_PARAMAS[self.task][k])
+
+    def training(self, cfg: TrainConfig, callback: TrainCallback):
 
-        model = YOLO(ctx.pretrained_model, task=self.backend_task_name)
+        model = YOLO(cfg.pretrained_model, task=self.backend_task_name)
         model.train(
-            data=ctx.dataset_path,
-            epochs=ctx.epochs,
-            batch=ctx.batch_size,
-            imgsz=ctx.image_size,
-            rect=ctx.letter_box,
-            device=ctx.device,
-            workers=ctx.workers,
-            seed=ctx.seed,
-            verbose=ctx.verbose,
+            data=cfg.dataset_path,
+            epochs=cfg.epochs,
+            batch=cfg.batch_size,
+            imgsz=cfg.image_size,
+            lr0=cfg.learning_rate,
+            lrf=cfg.learning_rate,
+            rect=cfg.letter_box,
+            device=cfg.device,
+            workers=cfg.workers,
+            seed=cfg.seed,
+            verbose=cfg.verbose,
             project=self.hub_dir,
             name=self.ARTIFACT_DIR,
         )
         del model
 
-    def on_train_end(self, ctx: TrainContext):
+    def on_train_end(self, cfg: TrainConfig):
         io.copy_file(
             self.artifact_dir / "weights" / "best.pt",
             self.best_ckpt_file,
             create_directory=True,
         )
         io.copy_file(
             self.artifact_dir / "weights" / "last.pt",
             self.last_ckpt_file,
             create_directory=True,
         )
         io.save_json(self.get_metrics(), self.metric_file)
 
     # Inference Hook
-    def get_model(
-        self, image_size: Union[int, list] = None, parser: ResultParser = None
-    ):
+    def get_model(self):
+        """Get model.
+        Returns:
+            ModelWrapper: Model wrapper
+        """
         self.check_train_sanity()
 
-        if image_size is None:
-            train_config = io.load_yaml(self.train_config_file)
-            image_size = train_config.get("image_size")
-
         # get adapt functions
         preprocess = self.get_preprocess(self.task)
-        postprocess = self.get_postprocess(self.task, image_size=image_size)
+        postprocess = self.get_postprocess(self.task)
 
         # get model
         model = ModelWrapper(
             model=YOLO(self.best_ckpt_file).model.eval(),
             preprocess=preprocess,
             postprocess=postprocess,
-            parser=parser if parser else None,
         )
 
         return model
 
-    def on_inference_end(self, ctx: InferenceContext):
-        pass
-
     # Evaluate Hook
     def evaluating(self):
         raise NotImplementedError
```

### Comparing `waffle_hub-0.1.5/waffle_hub/hub/base_hub.py` & `waffle_hub-0.1.6/waffle_hub/hub/base_hub.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,91 +1,43 @@
 """
 Base Hub Class
 Do not use this Class directly.
 Use {Backend}Hub instead.
 """
-import contextlib
 import logging
-import os
-import sys
 import threading
 from abc import abstractmethod
-from dataclasses import asdict, dataclass
 from functools import cached_property
-from io import StringIO
 from pathlib import Path
 from typing import Union
 
 import cv2
 import torch
 import tqdm
 from waffle_utils.file import io
 from waffle_utils.utils import type_validator
 
 from waffle_hub.hub.model.wrapper import get_parser
-from waffle_hub.schemas.configs import Model, Train
+from waffle_hub.schema.configs import (
+    ExportConfig,
+    InferenceConfig,
+    ModelConfig,
+    TrainConfig,
+)
 from waffle_hub.utils.callback import (
     ExportCallback,
     InferenceCallback,
     TrainCallback,
 )
-from waffle_hub.utils.image import ImageDataset, draw_results
+from waffle_hub.utils.data import ImageDataset
+from waffle_hub.utils.draw import draw_results
 
 logger = logging.getLogger(__name__)
 
 
-class ConfigContext:
-    def __enter__(self):
-        return self
-
-    def __exit__(self, exc_type, exc_value, exc_traceback):
-        return
-
-
-@dataclass
-class TrainContext(ConfigContext):
-    dataset_path: str
-    epochs: int
-    batch_size: int
-    image_size: int
-    letter_box: bool
-    pretrained_model: str
-    device: str
-    workers: int
-    seed: int
-    verbose: bool
-
-
-@dataclass
-class InferenceContext(ConfigContext):
-    source: str
-    batch_size: int
-    recursive: bool
-    image_size: int
-    letter_box: bool
-    confidence_threshold: float
-    iou_threshold: float
-    half: bool
-    workers: int
-    device: str
-    draw: bool
-
-    model = None
-    dataloader = None
-
-
-@dataclass
-class ExportContext(ConfigContext):
-    image_size: Union[int, list]
-    batch_size: int
-    input_name: list[str]
-    output_name: list[str]
-    opset_version: int
-
-
 class BaseHub:
 
     MODEL_TYPES = {}
 
     # directory settings
     DEFAULT_ROOT_DIR = Path("./hubs")
 
@@ -114,50 +66,46 @@
         self,
         name: str,
         backend: str = None,
         version: str = None,
         task: str = None,
         model_type: str = None,
         model_size: str = None,
-        classes: Union[list[dict], list] = None,
+        categories: Union[list[dict], list] = None,
         root_dir: str = None,
     ):
         self.name: str = name
         self.task: str = task
         self.model_type: str = model_type
         self.model_size: str = model_size
-        self.classes: list[dict] = classes
+        self.categories: list[dict] = categories
         self.root_dir: Path = Path(root_dir) if root_dir else None
 
         self.backend: str = backend
         self.version: str = version
 
         # check task supports
         if self.task not in self.MODEL_TYPES:
             io.remove_directory()
             raise ValueError(
                 f"{self.task} is not supported with {self.backend}"
             )
 
         try:
             # save model config
-            model_config = Model(
+            model_config = ModelConfig(
                 name=self.name,
                 backend=self.backend,
                 version=self.version,
                 task=self.task,
                 model_type=self.model_type,
                 model_size=self.model_size,
-                classes=self.classes,
-            )
-            io.save_yaml(
-                asdict(model_config),
-                self.model_config_file,
-                create_directory=True,
+                categories=self.categories,
             )
+            model_config.save_yaml(self.model_config_file)
         except Exception as e:
             raise e
 
     @classmethod
     def load(cls, name: str, root_dir: str = None) -> "BaseHub":
         """Load Hub by name.
 
@@ -288,23 +236,23 @@
 
     @version.setter
     @type_validator(str)
     def version(self, v):
         self.__version = v
 
     @property
-    def classes(self) -> list[dict]:
-        return self.__classes
+    def categories(self) -> list[dict]:
+        return self.__categories
 
-    @classes.setter
+    @categories.setter
     @type_validator(list)
-    def classes(self, v):
+    def categories(self, v):
         if isinstance(v[0], str):
             v = [{"supercategory": "object", "name": n} for n in v]
-        self.__classes = v
+        self.__categories = v
 
     @cached_property
     def hub_dir(self) -> Path:
         """Hub(Model) Directory"""
         return self.root_dir / self.name
 
     @cached_property
@@ -377,123 +325,118 @@
             self.model_config_file.exists()
             and self.best_ckpt_file.exists()
             # and self.last_ckpt_file.exists()
         ):
             raise FileNotFoundError("Train first! hub.train(...).")
         return True
 
+    def get_train_config(self):
+        return TrainConfig.load(self.train_config_file)
+
+    def get_model_config(self):
+        return ModelConfig.load(self.model_config_file)
+
     # Train Hook
-    def before_train(self, ctx: TrainContext):
+    def before_train(self, cfg: TrainConfig):
         if self.artifact_dir.exists():
             raise FileExistsError(
                 f"{self.artifact_dir}\n"
                 "Train artifacts already exist. Remove artifact to re-train (hub.delete_artifact())."
             )
 
-    def on_train_start(self, ctx: TrainContext):
+    def on_train_start(self, cfg: TrainConfig):
         pass
 
-    def save_train_config(self, ctx: TrainContext):
-        io.save_yaml(
-            asdict(
-                Train(
-                    image_size=ctx.image_size,
-                    letter_box=ctx.letter_box,
-                    batch_size=ctx.batch_size,
-                    pretrained_model=ctx.pretrained_model,
-                    seed=ctx.seed,
-                )
-            ),
-            self.train_config_file,
-            create_directory=True,
-        )
+    def save_train_config(self, cfg: TrainConfig):
+        cfg.save_yaml(self.train_config_file)
 
-    def training(self, ctx: TrainContext):
+    def training(self, cfg: TrainConfig):
         pass
 
-    def on_train_end(self, ctx: TrainContext):
+    def on_train_end(self, cfg: TrainConfig):
         pass
 
-    def after_train(self, ctx: TrainContext):
+    def after_train(self, cfg: TrainConfig):
         pass
 
     def train(
         self,
         dataset_path: str,
-        epochs: int,
-        batch_size: int,
-        image_size: int,
-        letter_box: bool = False,
+        epochs: int = None,
+        batch_size: int = None,
+        image_size: Union[int, list[int]] = None,
+        learning_rate: float = None,
+        letter_box: bool = None,
         pretrained_model: str = None,
         device: str = "0",
         workers: int = 2,
         seed: int = 0,
         verbose: bool = True,
         hold: bool = True,
-    ) -> str:
+    ) -> TrainCallback:
         """Start Train
 
         Args:
-            dataset_path (str): Dataset Path. Recommend to use result of waffle_utils.dataset.Dataset.export.
-            epochs (int): total epochs
-            batch_size (int): batch size
-            image_size (int): image size
-            letter_box (bool): letter box preprocess. Defaults to False.
-            pretrained_model (str, optional): pretrained model file. Defaults to None.
-            device (str, optional): gpu device. Defaults to "0".
-            workers (int, optional): num workers. Defaults to 2.
+            dataset_path (str): dataset path
+            epochs (int, optional): number of epochs. None to use default. Defaults to None.
+            batch_size (int, optional): batch size. None to use default. Defaults to None.
+            image_size (Union[int, list[int]], optional): image size. None to use default. Defaults to None.
+            learning_rate (float, optional): learning rate. None to use default. Defaults to None.
+            letter_box (bool, optional): letter box. None to use default. Defaults to None.
+            pretrained_model (str, optional): pretrained model. None to use default. Defaults to None.
+            device (str, optional): device. "cpu" or "gpu_id". Defaults to "0".
+            workers (int, optional): number of workers. Defaults to 2.
             seed (int, optional): random seed. Defaults to 0.
             verbose (bool, optional): verbose. Defaults to True.
-            hold (bool, optional): hold or not.
-                If True then it holds until task finished.
-                If False then return Inferece Callback and run in background. Defaults to True.
+            hold (bool, optional): hold process. Defaults to True.
 
         Raises:
             FileExistsError: if trained artifact exists.
             FileNotFoundError: if can not detect appropriate dataset.
             ValueError: if can not detect appropriate dataset.
             e: something gone wrong with ultralytics
 
         Returns:
-            str: hub directory
+            TrainCallback: train callback
         """
 
-        ctx = TrainContext(
+        cfg = TrainConfig(
             dataset_path=dataset_path,
             epochs=epochs,
             batch_size=batch_size,
             image_size=image_size,
+            learning_rate=learning_rate,
             letter_box=letter_box,
             pretrained_model=pretrained_model,
             device=device,
             workers=workers,
             seed=seed,
             verbose=verbose,
         )
-        self.before_train(ctx)
-        self.on_train_start(ctx)
-        self.save_train_config(ctx)
+        self.before_train(cfg)
+        self.on_train_start(cfg)
+        self.save_train_config(cfg)
 
         def inner(callback: TrainCallback):
             try:
-                self.training(ctx, callback)
+                self.training(cfg, callback)
                 callback.best_ckpt_file = self.best_ckpt_file
                 callback.last_ckpt_file = self.last_ckpt_file
                 callback.metric_file = self.metric_file
                 callback.result_dir = self.hub_dir
-                self.on_train_end(ctx)
-                self.after_train(ctx)
+                self.on_train_end(cfg)
+                self.after_train(cfg)
                 callback.force_finish()
             except Exception as e:
                 if self.artifact_dir.exists():
                     io.remove_directory(self.artifact_dir)
                 callback.force_finish()
                 raise e
 
-        callback = TrainCallback(ctx.epochs, self.get_metrics)
+        callback = TrainCallback(cfg.epochs, self.get_metrics)
         if hold:
             inner(callback)
         else:
             thread = threading.Thread(
                 target=inner, args=(callback,), daemon=True
             )
             callback.register_thread(thread)
@@ -501,148 +444,150 @@
 
         return callback
 
     # Inference Hook
     def get_model(self):
         raise NotImplementedError
 
-    def before_inference(self, ctx: InferenceContext):
+    def before_inference(self, cfg: InferenceConfig):
         self.check_train_sanity()
 
         # overwrite training config
-        train_config = io.load_yaml(self.train_config_file)
-        if ctx.image_size is None:
-            ctx.image_size = train_config.get("image_size")
-        if ctx.letter_box is None:
-            ctx.letter_box = train_config.get("letter_box")
-
-    def on_inference_start(self, ctx: InferenceContext):
-        ctx.model = self.get_model(
-            ctx.image_size, get_parser(self.task)(**asdict(ctx))
-        )
-        ctx.dataloader = ImageDataset(
-            ctx.source, ctx.image_size, letter_box=ctx.letter_box
-        ).get_dataloader(ctx.batch_size, ctx.workers)
+        train_config = self.get_train_config()
+        if cfg.image_size is None:
+            cfg.image_size = train_config.image_size
+        if cfg.letter_box is None:
+            cfg.letter_box = train_config.letter_box
+
+    def on_inference_start(self, cfg: InferenceConfig):
+        pass
 
     def inferencing(
-        self, ctx: InferenceContext, callback: InferenceCallback
+        self, cfg: InferenceConfig, callback: InferenceCallback
     ) -> str:
-        model = ctx.model.to(ctx.device)
-        dataloader = ctx.dataloader
-        device = ctx.device
+        device = cfg.device
 
+        model = self.get_model().to(device)
+        dataloader = ImageDataset(
+            cfg.source, cfg.image_size, letter_box=cfg.letter_box
+        ).get_dataloader(cfg.batch_size, cfg.workers)
+
+        result_parser = get_parser(self.task)(**cfg.to_dict())
+
+        callback._total_steps = len(dataloader)
         for i, (images, image_infos) in tqdm.tqdm(
             enumerate(dataloader, start=1), total=len(dataloader)
         ):
-            result_batch = model(images.to(device), image_infos)
+            result_batch = model(images.to(device))
+            result_batch = result_parser(result_batch, image_infos)
             results = []
             for result, image_info in zip(result_batch, image_infos):
-                image_path = image_info.get("image_path")
+                image_path = image_info.image_path
+
+                relpath = Path(image_path).relative_to(cfg.source)
 
-                relpath = Path(image_path).relative_to(ctx.source)
                 io.save_json(
-                    result,
+                    [res.to_dict() for res in result],
                     self.inference_dir / relpath.with_suffix(".json"),
                     create_directory=True,
                 )
 
                 results.append(result)
 
-                if ctx.draw:
+                if cfg.draw:
                     draw = draw_results(
                         image_path,
                         result,
-                        task=self.task,
-                        names=[x["name"] for x in self.classes],
+                        names=[x["name"] for x in self.categories],
                     )
                     draw_path = self.draw_dir / relpath.with_suffix(".png")
                     io.make_directory(draw_path.parent)
                     cv2.imwrite(str(draw_path), draw)
 
             callback.update(i)
 
-    def on_inference_end(self, ctx: InferenceContext):
+    def on_inference_end(self, cfg: InferenceConfig):
         pass
 
-    def after_inference(self, ctx: InferenceContext):
+    def after_inference(self, cfg: InferenceConfig):
         pass
 
     def inference(
         self,
         source: str,
         recursive: bool = True,
-        image_size: int = None,
+        image_size: Union[int, list[int]] = None,
         letter_box: bool = None,
         batch_size: int = 4,
         confidence_threshold: float = 0.25,
         iou_threshold: float = 0.5,
         half: bool = False,
         workers: int = 2,
         device: str = "0",
         draw: bool = False,
         hold: bool = True,
-    ) -> str:
+    ) -> InferenceCallback:
         """Start Inference
 
         Args:
-            source (str): dataset source. image file or image directory. TODO: video
-            recursive (bool, optional): get images from directory recursively. Defaults to True.
-            image_size (int, optional): inference image size. None for same with train_config (recommended).
-            letter_box (bool, optional): letter box preprocess. None for same with train_config (recommended).
+            source (str): source directory
+            recursive (bool, optional): recursive. Defaults to True.
+            image_size (Union[int, list[int]], optional): image size. None for using training config. Defaults to None.
+            letter_box (bool, optional): letter box. None for using training config. Defaults to None.
             batch_size (int, optional): batch size. Defaults to 4.
             confidence_threshold (float, optional): confidence threshold. Defaults to 0.25.
-            iou_threshold (float, optional): iou threshold. Defaults to 0.7.
-            half (bool, optional): fp16 inference. Defaults to False.
-            device (str, optional): gpu device. Defaults to "0".
-            draw (bool, optional): save draw or not. Defaults to False.
-            hold (bool, optional): hold or not.
-                If True then it holds until task finished.
-                If False then return Inferece Callback and run in background. Defaults to True.
+            iou_threshold (float, optional): iou threshold. Defaults to 0.5.
+            half (bool, optional): half. Defaults to False.
+            workers (int, optional): workers. Defaults to 2.
+            device (str, optional): device. "cpu" or "gpu_id". Defaults to "0".
+            draw (bool, optional): draw. Defaults to False.
+            hold (bool, optional): hold. Defaults to True.
+
 
         Raises:
             FileNotFoundError: if can not detect appropriate dataset.
             e: something gone wrong with ultralytics
 
         Returns:
-            str: inference result directory
+            InferenceCallback: inference callback
         """
         self.check_train_sanity()
 
-        ctx = InferenceContext(
+        cfg = InferenceConfig(
             source=source,
             batch_size=batch_size,
             recursive=recursive,
             image_size=image_size,
             letter_box=letter_box,
             confidence_threshold=confidence_threshold,
             iou_threshold=iou_threshold,
             half=half,
             workers=workers,
             device="cpu" if device == "cpu" else f"cuda:{device}",
             draw=draw,
         )
 
-        self.before_inference(ctx)
-        self.on_inference_start(ctx)
+        self.before_inference(cfg)
+        self.on_inference_start(cfg)
 
         def inner(callback):
             try:
-                self.inferencing(ctx, callback)
+                self.inferencing(cfg, callback)
                 callback.inference_dir = self.inference_dir
-                callback.draw_dir = self.draw_dir if ctx.draw else None
-                self.on_inference_end(ctx)
-                self.after_inference(ctx)
+                callback.draw_dir = self.draw_dir if cfg.draw else None
+                self.on_inference_end(cfg)
+                self.after_inference(cfg)
                 callback.force_finish()
             except Exception as e:
                 if self.inference_dir.exists():
                     io.remove_directory(self.inference_dir)
                 callback.force_finish()
                 raise e
 
-        callback = InferenceCallback(len(ctx.dataloader))
+        callback = InferenceCallback(0)
 
         if hold:
             inner(callback)
         else:
             thread = threading.Thread(
                 target=inner, args=(callback,), daemon=True
             )
@@ -650,44 +595,44 @@
             callback.start()
 
         return callback
 
     # Export Hook
     def export(
         self,
-        image_size: int = None,
-        batch_size: int = 1,
+        image_size: Union[int, list[int]] = None,
+        batch_size: int = 16,
         opset_version: int = 11,
         hold: bool = True,
-    ) -> str:
+    ) -> ExportCallback:
         """Export Model
 
         Args:
-            image_size (int, optional): inference image size. None for same with train_config (recommended).
+            image_size (Union[int, list[int]], optional): inference image size. None for same with train_config (recommended).
             batch_size (int, optional): dynamic batch size. Defaults to 16.
             opset_version (int, optional): onnx opset version. Defaults to 11.
             hold (bool, optional): hold or not.
                 If True then it holds until task finished.
                 If False then return Inferece Callback and run in background. Defaults to True.
 
         Returns:
-            str: export onnx file path
+            ExportCallback: export callback
         """
         self.check_train_sanity()
 
-        train_config = Train(**io.load_yaml(self.train_config_file))
+        train_config = self.get_train_config()
 
         image_size = image_size if image_size else train_config.image_size
         image_size = (
             [image_size, image_size]
             if isinstance(image_size, int)
             else image_size
         )
 
-        model = self.get_model(train_config.image_size)
+        model = self.get_model()
 
         input_name = ["inputs"]
         if self.task == "object_detection":
             output_names = ["bbox", "conf", "class_id"]
         elif self.task == "classification":
             output_names = ["predictions"]
         else:
```

### Comparing `waffle_hub-0.1.5/waffle_hub/hub/model/wrapper.py` & `waffle_hub-0.1.6/waffle_hub/hub/model/wrapper.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,17 +4,25 @@
     NotImplementedError: _description_
     ValueError: _description_
 
 Returns:
     _type_: _description_
 """
 
+from typing import Union
+
 import torch
 from torchvision.ops import batched_nms
 
+from waffle_hub.schema.data import (
+    ClassificationResult,
+    ImageInfo,
+    ObjectDetectionResult,
+)
+
 
 class PreprocessFunction:
     pass
 
 
 class PostprocessFunction:
     pass
@@ -24,27 +32,35 @@
     pass
 
 
 class ClassificationResultParser(ResultParser):
     def __init__(self, *args, **kwargs):
         pass
 
-    def __call__(self, results: list[torch.Tensor], *args, **kwargs):
+    def __call__(
+        self,
+        results: list[torch.Tensor],
+        image_infos: list[ImageInfo] = None,
+        *args,
+        **kwargs
+    ) -> list[ClassificationResult]:
         parseds = []
 
         results = results[0]  # TODO: multi label
         scores, class_ids = results.cpu().topk(results.shape[1], dim=-1)
         results = torch.cat(
             [class_ids.unsqueeze(-1), scores.unsqueeze(-1)], dim=-1
         )
         for result in results:
             parsed = []
             for class_id, score in result:
                 parsed.append(
-                    {"category_id": int(class_id), "score": float(score)}
+                    ClassificationResult(
+                        category_id=int(class_id), score=float(score)
+                    )
                 )
             parseds.append(parsed)
         return parseds
 
 
 class ObjectDetectionResultParser(ResultParser):
     def __init__(
@@ -56,18 +72,18 @@
     ):
         self.confidence_threshold = confidence_threshold
         self.iou_threshold = iou_threshold
 
     def __call__(
         self,
         results: list[torch.Tensor],
-        image_infos: list[dict],
+        image_infos: list[ImageInfo],
         *args,
         **kwargs
-    ):
+    ) -> list[ObjectDetectionResult]:
         parseds = []
 
         bboxes_batch, confs_batch, class_ids_batch = results
         for bboxes, confs, class_ids, image_info in zip(
             bboxes_batch, confs_batch, class_ids_batch, image_infos
         ):
 
@@ -80,36 +96,36 @@
             )
             idxs = batched_nms(bboxes, confs, class_ids, self.iou_threshold)
 
             bboxes = bboxes[idxs, :].cpu()
             confs = confs[idxs].cpu()
             class_ids = class_ids[idxs].cpu()
 
-            W, H = image_info.get("input_shape")
-            left_pad, top_pad = image_info.get("pad")
-            ori_w, ori_h = image_info.get("ori_shape")
-            new_w, new_h = image_info.get("new_shape")
+            W, H = image_info.input_shape
+            left_pad, top_pad = image_info.pad
+            ori_w, ori_h = image_info.ori_shape
+            new_w, new_h = image_info.new_shape
 
             parsed = []
             for (x1, y1, x2, y2), conf, class_id in zip(
                 bboxes, confs, class_ids
             ):
 
                 x1 = max(float((x1 * W - left_pad) / new_w * ori_w), 0)
                 y1 = max(float((y1 * H - top_pad) / new_h * ori_h), 0)
                 x2 = min(float((x2 * W - left_pad) / new_w * ori_w), ori_w)
                 y2 = min(float((y2 * H - top_pad) / new_h * ori_h), ori_h)
 
                 parsed.append(
-                    {
-                        "bbox": [x1, y1, x2 - x1, y2 - y1],
-                        "area": float((x2 - x1) * (y2 - y1)),
-                        "category_id": int(class_id),
-                        "score": float(conf),
-                    }
+                    ObjectDetectionResult(
+                        bbox=[x1, y1, x2 - x1, y2 - y1],
+                        area=float((x2 - x1) * (y2 - y1)),
+                        category_id=int(class_id),
+                        score=float(conf),
+                    )
                 )
             parseds.append(parsed)
         return parseds
 
 
 def get_parser(task: str):
     if task == "classification":
@@ -120,25 +136,24 @@
 
 class ModelWrapper(torch.nn.Module):
     def __init__(
         self,
         model: torch.nn.Module,
         preprocess: PreprocessFunction,
         postprocess: PostprocessFunction,
-        parser: ResultParser = None,
     ):
         """
         Model Wrapper.
         Use this wrapper when inference, export.
 
         Args:
             model (torch.nn.Module): model
             preprocess (PreprocessFunction):
                 Preprocess Function that
-                recieves [batch, channel, height, width],
+                recieves [batch, channel, height, width] (0~1),
                 and
                 outputs [batch, channel, height, width].
 
             postprocess (PostprocessFunction):
                 Postprocess Function that
                 recieves model raw output,
                 and
@@ -157,16 +172,57 @@
                 Segmentation:
                     # TODO: segmentation support
         """
         super().__init__()
         self.model = model
         self.preprocess = preprocess
         self.postprocess = postprocess
-        self.parser = parser
 
-    def forward(self, x, image_infos: list[dict] = None, *args, **kwargs):
+    def forward(self, x):
+        _, _, H, W = x.shape
         x = self.preprocess(x)
         x = self.model(x)
-        x = self.postprocess(x)
-        if self.parser is not None:
-            x = self.parser(x, image_infos=image_infos, *args, **kwargs)
+        x = self.postprocess(x, image_size=(W, H))
         return x
+
+    def get_layer_names(self) -> list[str]:
+        """
+        Get all layer names in model.
+        """
+        return [name for name, _ in self.model.named_modules()]
+
+    def get_feature_maps(
+        self, x, layer_names: Union[list[str], str] = None
+    ) -> tuple[torch.Tensor, dict]:
+        """
+        Get feature maps from model.
+
+        Args:
+            x (torch.Tensor): input image
+            layer_names (Union[list[str], str]): layer names to get feature maps
+
+        Returns:
+            x (torch.Tensor): model output
+            feature_maps (dict): feature maps
+        """
+
+        feature_maps = {}
+
+        def hook(name):
+            def hook_fn(m, i, o):
+                feature_maps[name] = o
+
+            return hook_fn
+
+        if layer_names is None:
+            layer_names = self.get_layer_names()[-1]
+        elif isinstance(layer_names, str):
+            layer_names = [layer_names]
+
+        for name, module in self.model.named_modules():
+            if name in layer_names:
+                print(name)
+                module.register_forward_hook(hook(name))
+
+        x = self.forward(x)
+
+        return x, feature_maps
```

### Comparing `waffle_hub-0.1.5/waffle_hub/run.py` & `waffle_hub-0.1.6/waffle_hub/run.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.5/waffle_hub/utils/callback.py` & `waffle_hub-0.1.6/waffle_hub/utils/callback.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.5/waffle_hub/utils/image.py` & `waffle_hub-0.1.6/waffle_hub/utils/data.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,67 +2,15 @@
 from typing import Union
 
 import cv2
 import numpy as np
 import torch
 from torchvision import transforms as T
 
-
-# TODO: draw utils..
-def draw_results(
-    image: Union[np.ndarray, str],
-    results: list[dict],
-    task: str,
-    names: list[str],
-):
-
-    if task == "classification":
-
-        def draw(image, results):
-            image = cv2.putText(
-                image,
-                f"{names[results[0].get('category_id')]}",
-                (10, 30),
-                2,
-                1.0,
-                (0, 0, 255),
-            )
-            return image
-
-    elif task == "object_detection":
-
-        def draw(image, results):
-            for result in results:
-                x1, y1, w, h = result["bbox"]
-                x2 = x1 + w
-                y2 = y1 + h
-                image = cv2.putText(
-                    image,
-                    f"{names[result.get('category_id')]}",
-                    (int(x1), int(y1) - 2),
-                    2,
-                    1.0,
-                    (0, 0, 255),
-                )
-                image = cv2.rectangle(
-                    image,
-                    (int(x1), int(y1)),
-                    (int(x2), int(y2)),
-                    (0, 0, 255),
-                    2,
-                )
-            return image
-
-    else:
-        raise NotImplementedError(f"{task} draw function not implemented")
-
-    if isinstance(image, str):
-        image = cv2.imread(image)
-
-    return draw(image, results)
+from waffle_hub.schema.data import ImageInfo
 
 
 def get_images(d, recursive: bool = True) -> list[str]:
     exp = "**/*" if recursive else "*"
     return list(
         map(
             str,
@@ -70,27 +18,26 @@
             + list(Path(d).glob(exp + ".jpg"))
             + list(Path(d).glob(exp + ".PNG"))
             + list(Path(d).glob(exp + ".JPG")),
         )
     )
 
 
-# TODO: define image_info schema
 def resize_image(
     image: np.ndarray, image_size: list[int], letter_box: bool = False
-) -> list[np.ndarray, list[int], list[int], list[int], list[int]]:
+) -> list[np.ndarray, ImageInfo]:
     """Resize Image.
 
     Args:
         image (np.ndarray): opencv image.
         image_size (list[int]): image [width, height].
         letter_box (bool): letter box.
 
     Returns:
-        list: resized_image, (ori_width, ori_height), (new_width, new_height), (left_pad, top_pad)
+        list[np.ndarray, ImageInfo]: resized image, image info.
     """
 
     h, w = image.shape[:2]
     W, H = image_size
 
     if letter_box:
         if w > h:
@@ -114,21 +61,25 @@
             top, bottom = 0, 0
 
         image = cv2.resize(image, (w_, h_), interpolation=cv2.INTER_CUBIC)
         image = cv2.copyMakeBorder(
             image, top, bottom, left, right, None, value=(114, 114, 114)
         )
 
-        return image, (w, h), (w_, h_), (W, H), (left, top)
-
     else:
         w_, h_ = W, H
+        left, top = 0, 0
         image = cv2.resize(image, (w_, h_), interpolation=cv2.INTER_CUBIC)
 
-        return image, (w, h), (w_, h_), (W, H), (0, 0)
+    return image, ImageInfo(
+        ori_shape=(w, h),
+        new_shape=(w_, h_),
+        input_shape=(W, H),
+        pad=(left, top),
+    )
 
 
 def collate_fn(batch):
     images, infos = list(zip(*batch))
     return torch.stack(images, dim=0), infos
 
 
@@ -162,29 +113,21 @@
         return len(self.image_paths)
 
     def __getitem__(self, idx):
         image_path = self.image_paths[idx]
 
         image = cv2.imread(image_path)
         image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
-        (
-            image,
-            (ori_w, ori_h),
-            (new_w, new_h),
-            (input_w, input_h),
-            (left_pad, top_pad),
-        ) = resize_image(image, self.image_size, self.letter_box)
-
-        return self.transform(image), {
-            "image_path": image_path,
-            "ori_shape": (ori_w, ori_h),
-            "new_shape": (new_w, new_h),
-            "input_shape": (input_w, input_h),
-            "pad": (left_pad, top_pad),
-        }
+        image, image_info = resize_image(
+            image, self.image_size, self.letter_box
+        )
+
+        image_info.image_path = image_path
+
+        return self.transform(image), image_info
 
     def get_dataloader(self, batch_size: int, num_workers: int):
         return torch.utils.data.DataLoader(
             self,
             batch_size,
             num_workers=num_workers,
             collate_fn=collate_fn,
```

### Comparing `waffle_hub-0.1.5/waffle_hub.egg-info/PKG-INFO` & `waffle_hub-0.1.6/waffle_hub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle-hub
-Version: 0.1.5
+Version: 0.1.6
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle-hub Version: 0.1.5 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle-hub Version: 0.1.6 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `waffle_hub-0.1.5/waffle_hub.egg-info/SOURCES.txt` & `waffle_hub-0.1.6/waffle_hub.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,26 +5,32 @@
 setup.py
 tests/test_hub.py
 waffle_hub/__init__.py
 waffle_hub/run.py
 waffle_hub.egg-info/PKG-INFO
 waffle_hub.egg-info/SOURCES.txt
 waffle_hub.egg-info/dependency_links.txt
+waffle_hub.egg-info/entry_points.txt
 waffle_hub.egg-info/requires.txt
 waffle_hub.egg-info/top_level.txt
+waffle_hub/experimental/__init__.py
+waffle_hub/experimental/serve.py
 waffle_hub/hub/__init__.py
 waffle_hub/hub/base_hub.py
 waffle_hub/hub/adapter/__init__.py
 waffle_hub/hub/adapter/tx_model/__init__.py
 waffle_hub/hub/adapter/tx_model/tx_model_hub.py
 waffle_hub/hub/adapter/tx_model/configs/__init__.py
 waffle_hub/hub/adapter/tx_model/configs/data_cfg.py
 waffle_hub/hub/adapter/tx_model/configs/model_cfg.py
 waffle_hub/hub/adapter/ultralytics/__init__.py
 waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
 waffle_hub/hub/model/__init__.py
 waffle_hub/hub/model/wrapper.py
-waffle_hub/schemas/__init__.py
-waffle_hub/schemas/configs.py
+waffle_hub/schema/__init__.py
+waffle_hub/schema/base_schema.py
+waffle_hub/schema/configs.py
+waffle_hub/schema/data.py
 waffle_hub/utils/__init__.py
 waffle_hub/utils/callback.py
-waffle_hub/utils/image.py
+waffle_hub/utils/data.py
+waffle_hub/utils/draw.py
```

