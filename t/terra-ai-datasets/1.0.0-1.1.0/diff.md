# Comparing `tmp/terra_ai_datasets-1.0.0.tar.gz` & `tmp/terra_ai_datasets-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terra_ai_datasets-1.0.0.tar", last modified: Mon Mar 27 21:23:31 2023, max compression
+gzip compressed data, was "terra_ai_datasets-1.1.0.tar", last modified: Mon Apr 10 00:25:13 2023, max compression
```

## Comparing `terra_ai_datasets-1.0.0.tar` & `terra_ai_datasets-1.1.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:23:31.101968 terra_ai_datasets-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-27 21:23:31.101968 terra_ai_datasets-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-27 21:23:17.000000 terra_ai_datasets-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 21:23:31.101968 terra_ai_datasets-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-03-27 21:23:17.000000 terra_ai_datasets-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:23:31.101968 terra_ai_datasets-1.0.0/terra_ai_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 21:23:17.000000 terra_ai_datasets-1.0.0/terra_ai_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19074 2023-03-27 21:23:17.000000 terra_ai_datasets-1.0.0/terra_ai_datasets/create.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:23:31.101968 terra_ai_datasets-1.0.0/terra_ai_datasets/creation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 21:23:17.000000 terra_ai_datasets-1.0.0/terra_ai_datasets/creation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-03-27 21:23:18.000000 terra_ai_datasets-1.0.0/terra_ai_datasets/creation/arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)    23989 2023-03-27 21:23:18.000000 terra_ai_datasets-1.0.0/terra_ai_datasets/creation/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-03-27 21:23:18.000000 terra_ai_datasets-1.0.0/terra_ai_datasets/creation/preprocessings.py
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-03-27 21:23:18.000000 terra_ai_datasets-1.0.0/terra_ai_datasets/creation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:23:31.101968 terra_ai_datasets-1.0.0/terra_ai_datasets/creation/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 21:23:18.000000 terra_ai_datasets-1.0.0/terra_ai_datasets/creation/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-03-27 21:23:18.000000 terra_ai_datasets-1.0.0/terra_ai_datasets/creation/validators/creation_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-03-27 21:23:18.000000 terra_ai_datasets-1.0.0/terra_ai_datasets/creation/validators/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-03-27 21:23:18.000000 terra_ai_datasets-1.0.0/terra_ai_datasets/creation/validators/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-03-27 21:23:18.000000 terra_ai_datasets-1.0.0/terra_ai_datasets/creation/validators/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-27 21:23:18.000000 terra_ai_datasets-1.0.0/terra_ai_datasets/creation/validators/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-03-27 21:23:18.000000 terra_ai_datasets-1.0.0/terra_ai_datasets/creation/validators/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-03-27 21:23:18.000000 terra_ai_datasets-1.0.0/terra_ai_datasets/load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:23:31.101968 terra_ai_datasets-1.0.0/terra_ai_datasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-27 21:23:31.000000 terra_ai_datasets-1.0.0/terra_ai_datasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-27 21:23:31.000000 terra_ai_datasets-1.0.0/terra_ai_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 21:23:31.000000 terra_ai_datasets-1.0.0/terra_ai_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-03-27 21:23:31.000000 terra_ai_datasets-1.0.0/terra_ai_datasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-27 21:23:31.000000 terra_ai_datasets-1.0.0/terra_ai_datasets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:23:31.101968 terra_ai_datasets-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 21:23:18.000000 terra_ai_datasets-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-03-27 21:23:18.000000 terra_ai_datasets-1.0.0/tests/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-03-27 21:23:18.000000 terra_ai_datasets-1.0.0/tests/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-03-27 21:23:18.000000 terra_ai_datasets-1.0.0/tests/test_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-03-27 21:23:18.000000 terra_ai_datasets-1.0.0/tests/test_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:25:13.945727 terra_ai_datasets-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-10 00:25:13.945727 terra_ai_datasets-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 00:25:13.945727 terra_ai_datasets-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:25:13.945727 terra_ai_datasets-1.1.0/terra_ai_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19074 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/create.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:25:13.945727 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14466 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24383 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/preprocessings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:25:13.945727 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/creation_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:25:13.945727 terra_ai_datasets-1.1.0/terra_ai_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-10 00:25:13.000000 terra_ai_datasets-1.1.0/terra_ai_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-10 00:25:13.000000 terra_ai_datasets-1.1.0/terra_ai_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 00:25:13.000000 terra_ai_datasets-1.1.0/terra_ai_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-10 00:25:13.000000 terra_ai_datasets-1.1.0/terra_ai_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-10 00:25:13.000000 terra_ai_datasets-1.1.0/terra_ai_datasets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:25:13.945727 terra_ai_datasets-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/tests/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/tests/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/tests/test_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/tests/test_timeseries.py
```

### Comparing `terra_ai_datasets-1.0.0/setup.py` & `terra_ai_datasets-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 
 from setuptools import setup, find_packages
 
 DESCRIPTION = "Framework to create a dataset to train a neural network."
 LONG_DESCRIPTION = "terra_ai_datasets is a framework to create " \
                    "a dataset to train a neural network model based on a Keras."
```

### Comparing `terra_ai_datasets-1.0.0/terra_ai_datasets/create.py` & `terra_ai_datasets-1.1.0/terra_ai_datasets/create.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.0.0/terra_ai_datasets/creation/arrays.py` & `terra_ai_datasets-1.1.0/terra_ai_datasets/creation/arrays.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,120 @@
 from abc import ABC, abstractmethod
 from typing import Any
 
 import cv2
 import numpy as np
-import pymorphy2
 import librosa.feature as librosa_feature
 from librosa import load as librosa_load
 from PIL import Image
 from tensorflow.keras.preprocessing.text import Tokenizer
 
-from terra_ai_datasets.creation.utils import resize_frame
 from terra_ai_datasets.creation.validators.inputs import ImageNetworkTypes, ImageValidator, TextValidator, \
-    TextProcessTypes, TextModeTypes, AudioValidator, AudioParameterTypes, AudioModeTypes, RawValidator, \
-    TimeseriesValidator, ImageScalers
+    TextProcessTypes, TextModeTypes, AudioValidator, AudioParameterTypes, RawValidator, TimeseriesValidator, \
+    ImageScalers, ImageProcessTypes
 from terra_ai_datasets.creation.validators.outputs import SegmentationValidator, ClassificationValidator, \
     RegressionValidator, DepthValidator, TrendValidator
 
 
+def resize_frame(image_array, target_shape, frame_mode):
+    original_shape = (image_array.shape[0], image_array.shape[1])
+    resized = None
+    if frame_mode == ImageProcessTypes.stretch:
+        resized = cv2.resize(image_array, (target_shape[1], target_shape[0]))
+
+    elif frame_mode == ImageProcessTypes.fit:
+        if image_array.shape[1] >= image_array.shape[0]:
+            resized_shape = list(target_shape).copy()
+            resized_shape[0] = int(
+                image_array.shape[0] / (image_array.shape[1] / target_shape[1])
+            )
+            if resized_shape[0] > target_shape[0]:
+                resized_shape = list(target_shape).copy()
+                resized_shape[1] = int(
+                    image_array.shape[1] / (image_array.shape[0] / target_shape[0])
+                )
+            image_array = cv2.resize(image_array, (resized_shape[1], resized_shape[0]))
+        elif image_array.shape[0] >= image_array.shape[1]:
+            resized_shape = list(target_shape).copy()
+            resized_shape[1] = int(
+                image_array.shape[1] / (image_array.shape[0] / target_shape[0])
+            )
+            if resized_shape[1] > target_shape[1]:
+                resized_shape = list(target_shape).copy()
+                resized_shape[0] = int(
+                    image_array.shape[0] / (image_array.shape[1] / target_shape[1])
+                )
+            image_array = cv2.resize(image_array, (resized_shape[1], resized_shape[0]))
+        resized = image_array
+        if resized.shape[0] < target_shape[0]:
+            black_bar = np.zeros(
+                (int((target_shape[0] - resized.shape[0]) / 2), resized.shape[1], 3),
+                dtype="uint8",
+            )
+            resized = np.concatenate((black_bar, resized))
+            black_bar_2 = np.zeros(
+                (int((target_shape[0] - resized.shape[0])), resized.shape[1], 3),
+                dtype="uint8",
+            )
+            resized = np.concatenate((resized, black_bar_2))
+        if resized.shape[1] < target_shape[1]:
+            black_bar = np.zeros(
+                (target_shape[0], int((target_shape[1] - resized.shape[1]) / 2), 3),
+                dtype="uint8",
+            )
+            resized = np.concatenate((black_bar, resized), axis=1)
+            black_bar_2 = np.zeros(
+                (target_shape[0], int((target_shape[1] - resized.shape[1])), 3),
+                dtype="uint8",
+            )
+            resized = np.concatenate((resized, black_bar_2), axis=1)
+
+    elif frame_mode == ImageProcessTypes.cut:
+        resized = image_array.copy()
+        if original_shape[0] > target_shape[0]:
+            resized = resized[
+                int(original_shape[0] / 2 - target_shape[0] / 2) : int(
+                    original_shape[0] / 2 - target_shape[0] / 2
+                )
+                + target_shape[0],
+                :,
+            ]
+        else:
+            black_bar = np.zeros(
+                (int((target_shape[0] - original_shape[0]) / 2), original_shape[1], 3),
+                dtype="uint8",
+            )
+            resized = np.concatenate((black_bar, resized))
+            black_bar_2 = np.zeros(
+                (int((target_shape[0] - resized.shape[0])), original_shape[1], 3),
+                dtype="uint8",
+            )
+            resized = np.concatenate((resized, black_bar_2))
+        if original_shape[1] > target_shape[1]:
+            resized = resized[
+                :,
+                int(original_shape[1] / 2 - target_shape[1] / 2) : int(
+                    original_shape[1] / 2 - target_shape[1] / 2
+                )
+                + target_shape[1],
+            ]
+        else:
+            black_bar = np.zeros(
+                (target_shape[0], int((target_shape[1] - original_shape[1]) / 2), 3),
+                dtype="uint8",
+            )
+            resized = np.concatenate((black_bar, resized), axis=1)
+            black_bar_2 = np.zeros(
+                (target_shape[0], int((target_shape[1] - resized.shape[1])), 3),
+                dtype="uint8",
+            )
+            resized = np.concatenate((resized, black_bar_2), axis=1)
+    return resized
+
+
 class Array(ABC):
 
     @abstractmethod
     def create(self, source: Any, parameters: Any):
         pass
 
     @abstractmethod
@@ -249,15 +343,15 @@
         return array
 
 
 class DepthArray(Array):
 
     def create(self, source: list, parameters: DepthValidator):
 
-        array = np.array(source)
+        array = np.array(source)[:parameters.depth]
         array = np.expand_dims(array, 1)
 
         return array
 
     def preprocess(self, array: np.ndarray, preprocess: Any, parameters: DepthValidator):
 
         orig_shape = array.shape
```

### Comparing `terra_ai_datasets-1.0.0/terra_ai_datasets/creation/dataset.py` & `terra_ai_datasets-1.1.0/terra_ai_datasets/creation/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import json
-import os
 from pathlib import Path
 from datetime import datetime
-from typing import Union, Dict, Any, List
+from typing import Union, Dict, Any
 
+from IPython.display import display
 from tensorflow.python.data.ops.dataset_ops import DatasetV2 as Dataset
 from tensorflow import TensorSpec
 from tqdm import tqdm
 import numpy as np
 import pandas as pd
 import joblib
 
-from terra_ai_datasets.creation import arrays, preprocessings, utils
-from terra_ai_datasets.creation.utils import apply_pymorphy, process_directory_paths
+from terra_ai_datasets.creation import preprocessings, utils, visualize
+from terra_ai_datasets.creation.utils import apply_pymorphy, process_directory_paths, decamelize, create_put_array, \
+    preprocess_put_array
 from terra_ai_datasets.creation.validators import creation_data
 from terra_ai_datasets.creation.validators.creation_data import InputData, OutputData, InputInstructionsData, \
     OutputInstructionsData
 from terra_ai_datasets.creation.validators import dataset
 from terra_ai_datasets.creation.validators import inputs, outputs
 from terra_ai_datasets.creation.validators.inputs import CategoricalValidator, ImageScalers, TextProcessTypes
 from terra_ai_datasets.creation.validators.structure import DatasetData
@@ -42,111 +43,118 @@
         put_arr = np.array(put_arr[0])
     return put_arr
 
 
 class TerraDataset:
 
     def __init__(self):
-        self.X: Dict[str, Dict[int, np.ndarray]] = {"train": {}, "val": {}}
-        self.Y: Dict[str, Dict[int, np.ndarray]] = {"train": {}, "val": {}}
+        self.X: Dict[str, Dict[str, np.ndarray]] = {"train": {}, "val": {}}
+        self.Y: Dict[str, Dict[str, np.ndarray]] = {"train": {}, "val": {}}
         self.preprocessing: Dict[str, Any] = {}
         self.dataframe: Dict[str, pd.DataFrame] = {}
         self.dataset_data: DatasetData = None
         self.put_instructions: Dict[int, Dict[str, Union[InputInstructionsData, OutputInstructionsData]]] = {}
 
         self._dataset: Dict[str, Dataset] = {"train": None, "val": None}
 
     @property
     def dataset(self):
         if not self._dataset["train"] and not self._dataset["val"]:
             return 'Массивы не были созданы. Вызовите метод .create(use_generator: bool = False)'
         return self._dataset
 
     @staticmethod
-    def create_dataset_object_from_arrays(x_arrays: Dict[int, np.ndarray], y_arrays: Dict[int, np.ndarray]) -> Dataset:
+    def create_dataset_object_from_arrays(x_arrays: Dict[str, np.ndarray], y_arrays: Dict[str, np.ndarray]) -> Dataset:
         return Dataset.from_tensor_slices((x_arrays, y_arrays))
 
     def create_dataset_object_from_instructions(self, put_instr, dataframe) -> Dataset:
 
         output_signature = [{}, {}]
         length, step, offset, total_samples = 1, 1, 0, len(dataframe)
+        inp_id, out_id = 1, 1
         for put_id, cols_dict in put_instr.items():
             put_array = []
             for col_name, put_data in cols_dict.items():
                 if put_data.type in \
                         [LayerInputTypeChoice.Timeseries, LayerOutputTypeChoice.Depth, LayerOutputTypeChoice.Trend]:
                     length = put_data.parameters.length
                     total_samples -= length * 2
                     if put_data.type in [LayerOutputTypeChoice.Depth, LayerOutputTypeChoice.Trend]:
                         offset = put_data.parameters.length
                         if put_data.type == LayerOutputTypeChoice.Trend:
                             offset -= 1
                 data_to_send = dataframe.loc[0 + offset:0 + offset + length - 1, col_name].to_list()
                 data_to_send = data_to_send[0] if len(data_to_send) == 1 else data_to_send
-                sample_array = self.create_put_array(data_to_send, put_data)
+                sample_array = create_put_array(data_to_send, put_data)
                 if self.preprocessing.get(col_name):
-                    sample_array = self.preprocess_put_array(
+                    sample_array = preprocess_put_array(
                         sample_array, put_data, self.preprocessing[col_name]
                     )
                 put_array.append(
                     sample_array[0] if type(sample_array) == np.ndarray and len(sample_array) == 1 else sample_array
                 )
             if put_data.type in [LayerInputTypeChoice.Timeseries, LayerOutputTypeChoice.Depth]:
                 put_array = np.expand_dims(np.array(put_array), 1)
                 put_array = postprocess_put_array(put_array, put_data.type)[0]
             else:
                 put_array = postprocess_put_array(put_array, put_data.type)
 
             if put_data.type in LayerInputTypeChoice:
-                output_signature[0][put_id] = TensorSpec(shape=put_array.shape, dtype=put_array.dtype)
+                output_signature[0][f"input_{inp_id}"] = TensorSpec(shape=put_array.shape, dtype=put_array.dtype)
+                inp_id += 1
             else:
-                output_signature[1][put_id] = TensorSpec(shape=put_array.shape, dtype=put_array.dtype)
+                output_signature[1][f"output_{out_id}"] = TensorSpec(shape=put_array.shape, dtype=put_array.dtype)
+                out_id += 1
 
         return Dataset.from_generator(lambda: self.generator(put_instr, dataframe, length, step, total_samples),
                                       output_signature=tuple(output_signature))
 
     def generator(self, put_instr, dataframe: pd.DataFrame, length, step, total_samples):
 
         for i in range(0, total_samples, step):
+            inp_id, out_id = 1, 1
             inp_dict, out_dict = {}, {}
             for put_id, cols_dict in put_instr.items():
                 put_array = []
                 for col_name, put_data in cols_dict.items():
                     offset = 0
                     if put_data.type in [LayerOutputTypeChoice.Depth, LayerOutputTypeChoice.Trend]:
                         offset = put_data.parameters.length
                     data_to_send = dataframe.loc[i+offset: i+offset+length-1, col_name].to_list()
                     data_to_send = data_to_send[0] if len(data_to_send) == 1 else data_to_send
-                    sample_array = self.create_put_array(data_to_send, put_data)
+                    sample_array = create_put_array(data_to_send, put_data)
 
-                    # sample_array = self.create_put_array(dataframe.loc[i, col_name], put_data)
+                    # sample_array = create_put_array(dataframe.loc[i, col_name], put_data)
                     if self.preprocessing.get(col_name):
-                        sample_array = self.preprocess_put_array(
+                        sample_array = preprocess_put_array(
                             sample_array, put_data, self.preprocessing[col_name]
                         )
                     put_array.append(
                         sample_array[0] if type(sample_array) == np.ndarray and len(sample_array) == 1 else sample_array
                     )
 
                 if put_data.type in [LayerInputTypeChoice.Timeseries, LayerOutputTypeChoice.Depth]:
                     put_array = np.expand_dims(np.array(put_array), 1)
                     put_array = postprocess_put_array(put_array, put_data.type)[0]
                 else:
                     put_array = postprocess_put_array(put_array, put_data.type)
 
                 if put_data.type in LayerInputTypeChoice:
-                    inp_dict[put_id] = put_array
+                    inp_dict[f"input_{inp_id}"] = put_array
+                    inp_id += 1
                 else:
-                    out_dict[put_id] = put_array
+                    out_dict[f"output_{out_id}"] = put_array
+                    out_id += 1
 
             yield inp_dict, out_dict
 
     def create(self, use_generator: bool = False):
 
         for split, dataframe in self.dataframe.items():
+            inp_id, out_id = 1, 1
             for put_id, cols_dict in self.put_instructions.items():
                 if use_generator and split != "train":
                     continue
                 for col_name, put_data in cols_dict.items():
                     if split == "train":
                         if "preprocessing" in put_data.parameters.dict() and put_data.parameters.preprocessing.value != 'None':
                             create_preprocessing_parameters = {"parameters": put_data.parameters}
@@ -174,71 +182,70 @@
                                 offset -= 1
                     for row_idx in tqdm(
                             range(0, total_samples, step),
                             desc=f"{datetime.now().strftime('%H:%M:%S')} | Формирование массивов {split} - {put_data.type} - {col_name}"
                     ):
                         data_to_send = dataframe.loc[row_idx+offset:row_idx+offset+length-1, col_name].to_list()
                         data_to_send = data_to_send[0] if len(data_to_send) == 1 else data_to_send
-                        sample_array = self.create_put_array(data_to_send, put_data)
+                        sample_array = create_put_array(data_to_send, put_data)
                         if self.preprocessing.get(col_name) and split == "train":
                             if put_data.type == LayerInputTypeChoice.Text:
-                                if put_data.parameters.preprocessing != TextProcessTypes.word_to_vec:
-                                    self.preprocessing[col_name].fit_on_texts(sample_array.split())
+                                pass
                             elif put_data.type == LayerInputTypeChoice.Image and put_data.parameters.preprocessing == ImageScalers.terra_image_scaler:
                                 self.preprocessing[col_name].fit(sample_array)
                             else:
-                                self.preprocessing[col_name].fit(sample_array.reshape(-1, 1))
+                                self.preprocessing[col_name].partial_fit(sample_array.reshape(-1, 1))
                         if not use_generator:
                             col_array.append(
                                 sample_array[0] if type(sample_array) == np.ndarray and len(sample_array) == 1 else sample_array
                             )
 
+                    if self.preprocessing.get(col_name) and split == "train":
+                        if put_data.type == LayerInputTypeChoice.Text:
+                            if put_data.parameters.preprocessing != TextProcessTypes.word_to_vec:
+                                self.preprocessing[col_name].fit_on_texts(col_array)
+
                     if self.preprocessing.get(col_name) and not use_generator:
-                        col_array = self.preprocess_put_array(
+                        col_array = preprocess_put_array(
                             np.array(col_array), put_data, self.preprocessing[col_name]
                         )
                     if not use_generator:
                         put_array.append(col_array if len(col_array) > 1 else col_array[0])
 
                 if not use_generator:
                     put_array = postprocess_put_array(put_array, put_data.type)
                     if isinstance(put_data, InputInstructionsData):
-                        self.X[split][put_id] = put_array
+                        self.X[split][f"input_{inp_id}"] = put_array
+                        inp_id += 1
                     else:
-                        self.Y[split][put_id] = put_array
+                        self.Y[split][f"output_{out_id}"] = put_array
+                        out_id += 1
 
             if not use_generator:
                 self._dataset[split] = self.create_dataset_object_from_arrays(self.X[split], self.Y[split])
             else:
                 self._dataset[split] = self.create_dataset_object_from_instructions(
                     self.put_instructions, dataframe
                 )
         self.dataset_data.is_created = True
 
-    @staticmethod
-    def create_put_array(data: Any, put_data: Union[InputInstructionsData, OutputInstructionsData]):
-
-        sample_array = getattr(arrays, f"{put_data.type}Array")().create(data, put_data.parameters)
-
-        return sample_array
-
-    @staticmethod
-    def preprocess_put_array(
-            data: Any, put_data: Union[InputInstructionsData, OutputInstructionsData], preprocessing: Any
-    ):
-
-        preprocessed_array = getattr(arrays, f"{put_data.type}Array")().preprocess(
-            data, preprocessing, put_data.parameters
+    def visualize(self):
+        getattr(visualize, f"visualize_{decamelize(self.dataset_data.task)}")(
+            put_instructions=self.put_instructions,
+            preprocessing=self.preprocessing
         )
 
-        return preprocessed_array
+    def evaluate_on_model(self, model, batch_size: int):
+        for inp, out in self.dataset["val"].batch(batch_size):
+            pred = model.predict(inp)
+            yield inp, out, pred
 
     def summary(self):
 
-        print(self.dataframe['train'].head())
+        display(self.dataframe['train'].head())
         print(f"\n\033[1mКол-во примеров в train выборке:\033[0m {len(self.dataframe['train'])}\n"
               f"\033[1mКол-во примеров в val выборке:\033[0m {len(self.dataframe['val'])}")
         print()
         if self.dataset_data.is_created:
             for inp_id, array in enumerate(self.X["train"].values(), 1):
                 print(f"\033[1mРазмерность входного массива {inp_id}:\033[0m", array[0].shape)
             for out_id, array in enumerate(self.Y["train"].values(), 1):
@@ -256,15 +263,15 @@
             classes_names = self.put_instructions[put_id][col_name].parameters.classes_names
             dataframe_dict = {cl_name: [] for cl_name in classes_names}
             for split in ['train', 'val']:
                 list_of_elements = self.dataframe[split].loc[:, col_name].tolist()
                 for cl_name in classes_names:
                     dataframe_dict[cl_name].append(list_of_elements.count(cl_name))
 
-            print(pd.DataFrame(dataframe_dict, index=['train', 'val']))
+            display(pd.DataFrame(dataframe_dict, index=['train', 'val']))
 
         elif output_type == LayerOutputTypeChoice.Segmentation:
             text_to_print = "\033[1mКлассы в масках сегментации и их цвета в RGB:\033[0m"
             classes = self.put_instructions[put_id][col_name].parameters.classes
             for name, color in classes.items():
                 text_to_print += f"\n{name}: {color.as_rgb_tuple()}"
             print(text_to_print)
```

### Comparing `terra_ai_datasets-1.0.0/terra_ai_datasets/creation/preprocessings.py` & `terra_ai_datasets-1.1.0/terra_ai_datasets/creation/preprocessings.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.0.0/terra_ai_datasets/creation/validators/creation_data.py` & `terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/creation_data.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.0.0/terra_ai_datasets/creation/validators/dataset.py` & `terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/dataset.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.0.0/terra_ai_datasets/creation/validators/inputs.py` & `terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/inputs.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.0.0/terra_ai_datasets/creation/validators/outputs.py` & `terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/outputs.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.0.0/terra_ai_datasets/creation/validators/tasks.py` & `terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/tasks.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 from enum import Enum
 
 
 class TasksChoice(str, Enum):
     ImageClassification = "ImageClassification"
     ImageSegmentation = "ImageSegmentation"
-    ImageRegression = "ImageRegression"
     TextClassification = "TextClassification"
-    TextSegmentation = "TextSegmentation"
-    TextRegression = "TextRegression"
     AudioClassification = "AudioClassification"
     DataframeClassification = "DataframeClassification"
-    DataframeDataset = "DataframeDataset"
     DataframeRegression = "DataframeRegression"
     TimeseriesDepth = "TimeseriesDepth"
     TimeseriesTrend = "TimeseriesTrend"
 
 
 class LayerInputTypeChoice(str, Enum):
     Image = "Image"
```

### Comparing `terra_ai_datasets-1.0.0/terra_ai_datasets/load.py` & `terra_ai_datasets-1.1.0/terra_ai_datasets/load.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.0.0/terra_ai_datasets.egg-info/SOURCES.txt` & `terra_ai_datasets-1.1.0/terra_ai_datasets.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 terra_ai_datasets.egg-info/requires.txt
 terra_ai_datasets.egg-info/top_level.txt
 terra_ai_datasets/creation/__init__.py
 terra_ai_datasets/creation/arrays.py
 terra_ai_datasets/creation/dataset.py
 terra_ai_datasets/creation/preprocessings.py
 terra_ai_datasets/creation/utils.py
+terra_ai_datasets/creation/visualize.py
 terra_ai_datasets/creation/validators/__init__.py
 terra_ai_datasets/creation/validators/creation_data.py
 terra_ai_datasets/creation/validators/dataset.py
 terra_ai_datasets/creation/validators/inputs.py
 terra_ai_datasets/creation/validators/outputs.py
 terra_ai_datasets/creation/validators/structure.py
 terra_ai_datasets/creation/validators/tasks.py
```

### Comparing `terra_ai_datasets-1.0.0/tests/test_classification.py` & `terra_ai_datasets-1.1.0/tests/test_classification.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,54 +9,54 @@
     dataset = ImageClassification(source_path=['./tests/dataset/cars/Мерседес', './tests/dataset/cars/Феррари'],
                                   width=80, height=64, preprocessing='MinMaxScaler', network="Linear", process='Fit',
                                   train_size=0.7, one_hot_encoding=True)
 
     dataset.create(use_generator=True)
 
     for inp, out in dataset.dataset['train'].batch(4):
-        assert inp[1].shape == (4, 64*80*3), 'Input shape does not match'
-        assert out[2].shape == (4, 2), 'Output shape does not match'
+        assert inp["input_1"].shape == (4, 64*80*3), 'Input shape does not match'
+        assert out["output_1"].shape == (4, 2), 'Output shape does not match'
 
-        assert inp[1].dtype == np.float32, 'Input outputs wrong datatype'
-        assert out[2].dtype == np.uint8, 'Output outputs wrong datatype'
+        assert inp["input_1"].dtype == np.float32, 'Input outputs wrong datatype'
+        assert out["output_1"].dtype == np.uint8, 'Output outputs wrong datatype'
 
         break
 
 
 def test_image_classification_terra_image():
     dataset = ImageClassification(source_path=['./tests/dataset/cars'], width=160, height=128,
                                   preprocessing='TerraImageScaler', network="Convolutional", process='Stretch',
                                   train_size=0.7, one_hot_encoding=False)
 
     dataset.create()
 
     for inp, out in dataset.dataset['train'].batch(6):
-        assert inp[1].shape == (6, 128, 160, 3), 'Input shape does not match'
-        assert out[2].shape == (6, ), 'Output shape does not match'
+        assert inp["input_1"].shape == (6, 128, 160, 3), 'Input shape does not match'
+        assert out["output_1"].shape == (6, ), 'Output shape does not match'
 
-        assert inp[1].dtype == np.float32
-        assert out[2].dtype == np.uint8
+        assert inp["input_1"].dtype == np.float32
+        assert out["output_1"].dtype == np.uint8
 
         break
 
 
 def test_image_classification_no_scaler():
     dataset = ImageClassification(source_path=['./tests/dataset/cars/Мерседес', './tests/dataset/cars/Рено',
                                                './tests/dataset/cars/Феррари'], width=80, height=64,
                                   preprocessing='None', network="Convolutional", process='Cut',
                                   train_size=0.7, one_hot_encoding=True)
 
     dataset.create()
 
     for inp, out in dataset.dataset['train'].batch(6):
-        assert inp[1].shape == (6, 64, 80, 3), 'Input shape does not match'
-        assert out[2].shape == (6, 3), 'Output shape does not match'
+        assert inp["input_1"].shape == (6, 64, 80, 3), 'Input shape does not match'
+        assert out["output_1"].shape == (6, 3), 'Output shape does not match'
 
-        assert inp[1].dtype == np.uint8
-        assert out[2].dtype == np.uint8
+        assert inp["input_1"].dtype == np.uint8
+        assert out["output_1"].dtype == np.uint8
 
         break
 
 
 def test_text_classification_emb():
 
     dataset = TextClassification(
@@ -70,19 +70,19 @@
         step=30,
         one_hot_encoding=True,
         pymorphy=True
     )
     dataset.create()
 
     for inp, out in dataset.dataset['train'].batch(2):
-        assert inp[1].shape == (2, 100), 'Input shape does not match'
-        assert out[2].shape == (2, 3), 'Output shape does not match'
+        assert inp["input_1"].shape == (2, 100), 'Input shape does not match'
+        assert out["output_1"].shape == (2, 3), 'Output shape does not match'
 
-        assert inp[1].dtype == np.int32
-        assert out[2].dtype == np.uint8
+        assert inp["input_1"].dtype == np.int32
+        assert out["output_1"].dtype == np.uint8
 
         break
 
 
 def test_text_classification_bow():
 
     dataset = TextClassification(
@@ -95,19 +95,19 @@
         one_hot_encoding=True,
         pymorphy=False
     )
 
     dataset.create(use_generator=True)
 
     for inp, out in dataset.dataset['train'].batch(3):
-        assert inp[1].shape == (3, 10000), 'Input shape does not match'
-        assert out[2].shape == (3, 10), 'Output shape does not match'
+        assert inp["input_1"].shape == (3, 10000), 'Input shape does not match'
+        assert out["output_1"].shape == (3, 10), 'Output shape does not match'
 
-        assert inp[1].dtype == np.int8
-        assert out[2].dtype == np.uint8
+        assert inp["input_1"].dtype == np.int8
+        assert out["output_1"].dtype == np.uint8
 
         break
 
 
 def test_text_classification_w2v():
 
     dataset = TextClassification(
@@ -122,19 +122,19 @@
         one_hot_encoding=True,
         pymorphy=False
     )
 
     dataset.create(use_generator=True)
 
     for inp, out in dataset.dataset['train'].batch(16):
-        assert inp[1].shape == (16, 100, 50), 'Input shape does not match'
-        assert out[2].shape == (16, 10), 'Output shape does not match'
+        assert inp["input_1"].shape == (16, 100, 50), 'Input shape does not match'
+        assert out["output_1"].shape == (16, 10), 'Output shape does not match'
 
-        assert inp[1].dtype == np.float64
-        assert out[2].dtype == np.uint8
+        assert inp["input_1"].dtype == np.float64
+        assert out["output_1"].dtype == np.uint8
 
         break
 
 
 def test_audio_classification():
 
     dataset = AudioClassification(
@@ -151,46 +151,46 @@
         step=0.4,
         one_hot_encoding=True
         )
 
     dataset.create(use_generator=True)
 
     for inp, out in dataset.dataset['train'].batch(16):
-        assert inp[1].shape == (16, 11025), 'Input shape does not match'
-        assert inp[2].shape == (16, 22, 20), 'Input shape does not match'
-        assert inp[3].shape == (16, 22), 'Input shape does not match'
-        assert out[4].shape == (16, 2), 'Output shape does not match'
-
-        assert inp[1].dtype == np.float32
-        assert inp[2].dtype == np.float32
-        assert inp[3].dtype == np.float32
-        assert out[4].dtype == np.uint8
+        assert inp["input_1"].shape == (16, 11025), 'Input shape does not match'
+        assert inp["input_2"].shape == (16, 22, 20), 'Input shape does not match'
+        assert inp["input_3"].shape == (16, 22), 'Input shape does not match'
+        assert out["output_1"].shape == (16, 2), 'Output shape does not match'
+
+        assert inp["input_1"].dtype == np.float32
+        assert inp["input_2"].dtype == np.float32
+        assert inp["input_3"].dtype == np.float32
+        assert out["output_1"].dtype == np.uint8
 
         break
 
 
-def test_audio_classification():
+def test_dataframe_classification():
     dataset = DataframeClassification(
         csv_path='./tests/dataset/flats/flats_cut.csv',
         train_size=0.5,
         inputs=[
             {"columns": ["Станция метро", "Пешком или на транспорте"], "type": "Categorical", "parameters": {"one_hot_encoding": True}},
             {"columns": ["Этаж"], "type": "Raw", "parameters": {}},
             {"columns": ["Примечание"], "type": "Text", "parameters": {"max_words_count": 20, "mode": "Full", "preprocessing": "Embedding", "max_words": 10, "pymorphy": False}},
         ],
         output="Тип дома",
         one_hot_encoding=False
     )
     dataset.create()
 
     for inp, out in dataset.dataset['train'].batch(4):
-        assert inp[1].shape == (4, 11), 'Input shape does not match'
-        assert inp[2].shape == (4, ), 'Input shape does not match'
-        assert inp[3].shape == (4, 10), 'Input shape does not match'
-        assert out[4].shape == (4, ), 'Output shape does not match'
-
-        assert inp[1].dtype == np.uint8
-        assert inp[2].dtype == np.int32
-        assert inp[3].dtype == np.int32
-        assert out[4].dtype == np.uint8
+        assert inp["input_1"].shape == (4, 11), 'Input shape does not match'
+        assert inp["input_2"].shape == (4, ), 'Input shape does not match'
+        assert inp["input_3"].shape == (4, 10), 'Input shape does not match'
+        assert out["output_1"].shape == (4, ), 'Output shape does not match'
+
+        assert inp["input_1"].dtype == np.uint8
+        assert inp["input_2"].dtype == np.int32
+        assert inp["input_3"].dtype == np.int32
+        assert out["output_1"].dtype == np.uint8
 
         break
```

### Comparing `terra_ai_datasets-1.0.0/tests/test_segmentation.py` & `terra_ai_datasets-1.1.0/tests/test_segmentation.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,31 +8,31 @@
     dataset = ImageSegmentation(source_path=['./airplane/Самолеты'], target_path=['./airplane/Сегменты'], train_size=.8,
                                 width=64, height=80, preprocessing="MinMaxScaler", network="Convolutional",
                                 process='Fit', rgb_range=50, num_classes=2)
 
     dataset.create()
 
     for inp, out in dataset.dataset['train'].batch(16):
-        assert inp[1].shape == (16, 80, 64, 3), 'Input shape does not match'
-        assert out[2].shape == (16, 80, 64, 2), 'Output shape does not match'
+        assert inp["input_1"].shape == (16, 80, 64, 3), 'Input shape does not match'
+        assert out["output_1"].shape == (16, 80, 64, 2), 'Output shape does not match'
 
-        assert inp[1].dtype == np.float32
-        assert out[2].dtype == np.uint8
+        assert inp["input_1"].dtype == np.float32
+        assert out["output_1"].dtype == np.uint8
 
         break
 
 
 def test_segmentation_no_scaler_from_file():
     dataset = ImageSegmentation(source_path=['./airplane/Самолеты'], target_path=['./airplane/Сегменты'], train_size=.8,
                                 width=32, height=40, preprocessing="None", network="Convolutional",
                                 process='Fit', rgb_range=50, classes_path='./airplane/labelmap.txt')
 
     dataset.create(use_generator=True)
 
     for inp, out in dataset.dataset['train'].batch(16):
-        assert inp[1].shape == (16, 40, 32, 3), 'Input shape does not match'
-        assert out[2].shape == (16, 40, 32, 2), 'Output shape does not match'
+        assert inp["input_1"].shape == (16, 40, 32, 3), 'Input shape does not match'
+        assert out["output_1"].shape == (16, 40, 32, 2), 'Output shape does not match'
 
-        assert inp[1].dtype == np.uint8
-        assert out[2].dtype == np.uint8
+        assert inp["input_1"].dtype == np.uint8
+        assert out["output_1"].dtype == np.uint8
 
         break
```

### Comparing `terra_ai_datasets-1.0.0/tests/test_timeseries.py` & `terra_ai_datasets-1.1.0/tests/test_timeseries.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,19 +14,19 @@
         length=30,
         step=7,
         depth=10,
     )
     dataset.create(use_generator=True)
 
     for inp, out in dataset.dataset['train'].batch(4):
-        assert inp[1].shape == (4, 30, 4), 'Input shape does not match'
-        assert out[2].shape == (4, 30, 2), 'Output shape does not match'
+        assert inp["input_1"].shape == (4, 30, 4), 'Input shape does not match'
+        assert out["output_1"].shape == (4, 10, 2), 'Output shape does not match'
 
-        assert inp[1].dtype == np.float64
-        assert out[2].dtype == np.float64
+        assert inp["input_1"].dtype == np.float64
+        assert out["output_1"].dtype == np.float64
 
         break
 
 
 def test_timeseries_trend():
 
     dataset = TimeseriesTrend(
@@ -39,14 +39,14 @@
         step=30,
         deviation=.5,
         one_hot_encoding=False
     )
     dataset.create()
 
     for inp, out in dataset.dataset['train'].batch(4):
-        assert inp[1].shape == (4, 100, 4), 'Input shape does not match'
-        assert out[2].shape == (4, ), 'Output shape does not match'
+        assert inp["input_1"].shape == (4, 100, 4), 'Input shape does not match'
+        assert out["output_1"].shape == (4, ), 'Output shape does not match'
 
-        assert inp[1].dtype == np.float64
-        assert out[2].dtype == np.int32
+        assert inp["input_1"].dtype == np.float64
+        assert out["output_1"].dtype == np.int32
 
         break
```

