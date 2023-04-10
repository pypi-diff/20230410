# Comparing `tmp/onnx2kerastl-0.0.82.dev5.tar.gz` & `tmp/onnx2kerastl-0.0.82.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx2kerastl-0.0.82.dev5.tar", max compression
+gzip compressed data, was "onnx2kerastl-0.0.82.dev6.tar", max compression
```

## Comparing `onnx2kerastl-0.0.82.dev5.tar` & `onnx2kerastl-0.0.82.dev6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1067 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev5/LICENSE
--rw-r--r--   0        0        0       66 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev5/onnx2kerastl/__init__.py
--rw-r--r--   0        0        0     8121 2023-04-03 08:32:59.779031 onnx2kerastl-0.0.82.dev5/onnx2kerastl/activation_layers.py
--rw-r--r--   0        0        0     1127 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev5/onnx2kerastl/caffe2_layers.py
--rw-r--r--   0        0        0      780 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev5/onnx2kerastl/constant_layers.py
--rw-r--r--   0        0        0    13188 2023-04-03 08:32:59.779031 onnx2kerastl-0.0.82.dev5/onnx2kerastl/converter.py
--rw-r--r--   0        0        0    11246 2023-04-03 08:32:59.779031 onnx2kerastl-0.0.82.dev5/onnx2kerastl/convolution_layers.py
--rw-r--r--   0        0        0      584 2023-04-04 08:56:02.330516 onnx2kerastl-0.0.82.dev5/onnx2kerastl/customonnxlayer/__init__.py
--rw-r--r--   0        0        0      236 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev5/onnx2kerastl/customonnxlayer/onnxabs.py
--rw-r--r--   0        0        0      236 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev5/onnx2kerastl/customonnxlayer/onnxerf.py
--rw-r--r--   0        0        0      606 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev5/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
--rw-r--r--   0        0        0     1327 2023-04-04 08:56:02.330516 onnx2kerastl-0.0.82.dev5/onnx2kerastl/customonnxlayer/onnxlstm.py
--rw-r--r--   0        0        0      605 2022-09-29 08:59:30.260148 onnx2kerastl-0.0.82.dev5/onnx2kerastl/customonnxlayer/onnxreducemean.py
--rw-r--r--   0        0        0      238 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev5/onnx2kerastl/customonnxlayer/onnxsqrt.py
--rw-r--r--   0        0        0     9300 2023-04-03 08:32:59.783031 onnx2kerastl-0.0.82.dev5/onnx2kerastl/elementwise_layers.py
--rw-r--r--   0        0        0      179 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev5/onnx2kerastl/exceptions.py
--rw-r--r--   0        0        0     3693 2023-04-03 08:32:59.783031 onnx2kerastl-0.0.82.dev5/onnx2kerastl/layers.py
--rw-r--r--   0        0        0     2301 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev5/onnx2kerastl/linear_layers.py
--rw-r--r--   0        0        0     3779 2023-04-04 08:56:02.330516 onnx2kerastl-0.0.82.dev5/onnx2kerastl/ltsm_layers.py
--rw-r--r--   0        0        0      368 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev5/onnx2kerastl/main.py
--rw-r--r--   0        0        0     5328 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev5/onnx2kerastl/normalization_layers.py
--rw-r--r--   0        0        0    15397 2023-04-03 08:32:59.783031 onnx2kerastl-0.0.82.dev5/onnx2kerastl/operation_layers.py
--rw-r--r--   0        0        0     2940 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev5/onnx2kerastl/padding_layers.py
--rw-r--r--   0        0        0     7464 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev5/onnx2kerastl/pooling_layers.py
--rw-r--r--   0        0        0    17567 2023-04-04 09:35:47.872126 onnx2kerastl-0.0.82.dev5/onnx2kerastl/reshape_layers.py
--rw-r--r--   0        0        0     1655 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev5/onnx2kerastl/upsampling_layers.py
--rw-r--r--   0        0        0     4415 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev5/onnx2kerastl/utils.py
--rw-r--r--   0        0        0     1035 2023-04-04 09:37:13.696773 onnx2kerastl-0.0.82.dev5/pyproject.toml
--rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.82.dev5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev6/LICENSE
+-rw-r--r--   0        0        0       66 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev6/onnx2kerastl/__init__.py
+-rw-r--r--   0        0        0     8121 2023-04-03 08:32:59.779031 onnx2kerastl-0.0.82.dev6/onnx2kerastl/activation_layers.py
+-rw-r--r--   0        0        0     1127 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev6/onnx2kerastl/caffe2_layers.py
+-rw-r--r--   0        0        0      780 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev6/onnx2kerastl/constant_layers.py
+-rw-r--r--   0        0        0    13188 2023-04-03 08:32:59.779031 onnx2kerastl-0.0.82.dev6/onnx2kerastl/converter.py
+-rw-r--r--   0        0        0    11246 2023-04-03 08:32:59.779031 onnx2kerastl-0.0.82.dev6/onnx2kerastl/convolution_layers.py
+-rw-r--r--   0        0        0      584 2023-04-04 08:56:02.330516 onnx2kerastl-0.0.82.dev6/onnx2kerastl/customonnxlayer/__init__.py
+-rw-r--r--   0        0        0      236 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev6/onnx2kerastl/customonnxlayer/onnxabs.py
+-rw-r--r--   0        0        0      236 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev6/onnx2kerastl/customonnxlayer/onnxerf.py
+-rw-r--r--   0        0        0      606 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev6/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
+-rw-r--r--   0        0        0     1344 2023-04-10 06:56:54.734936 onnx2kerastl-0.0.82.dev6/onnx2kerastl/customonnxlayer/onnxlstm.py
+-rw-r--r--   0        0        0      605 2022-09-29 08:59:30.260148 onnx2kerastl-0.0.82.dev6/onnx2kerastl/customonnxlayer/onnxreducemean.py
+-rw-r--r--   0        0        0      238 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev6/onnx2kerastl/customonnxlayer/onnxsqrt.py
+-rw-r--r--   0        0        0     9300 2023-04-03 08:32:59.783031 onnx2kerastl-0.0.82.dev6/onnx2kerastl/elementwise_layers.py
+-rw-r--r--   0        0        0      179 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev6/onnx2kerastl/exceptions.py
+-rw-r--r--   0        0        0     3693 2023-04-03 08:32:59.783031 onnx2kerastl-0.0.82.dev6/onnx2kerastl/layers.py
+-rw-r--r--   0        0        0     2301 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev6/onnx2kerastl/linear_layers.py
+-rw-r--r--   0        0        0     3779 2023-04-10 06:56:54.738936 onnx2kerastl-0.0.82.dev6/onnx2kerastl/ltsm_layers.py
+-rw-r--r--   0        0        0      368 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev6/onnx2kerastl/main.py
+-rw-r--r--   0        0        0     5328 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev6/onnx2kerastl/normalization_layers.py
+-rw-r--r--   0        0        0    15397 2023-04-03 08:32:59.783031 onnx2kerastl-0.0.82.dev6/onnx2kerastl/operation_layers.py
+-rw-r--r--   0        0        0     2940 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev6/onnx2kerastl/padding_layers.py
+-rw-r--r--   0        0        0     7464 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev6/onnx2kerastl/pooling_layers.py
+-rw-r--r--   0        0        0    17567 2023-04-10 06:56:54.742936 onnx2kerastl-0.0.82.dev6/onnx2kerastl/reshape_layers.py
+-rw-r--r--   0        0        0     1655 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev6/onnx2kerastl/upsampling_layers.py
+-rw-r--r--   0        0        0     4415 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev6/onnx2kerastl/utils.py
+-rw-r--r--   0        0        0     1035 2023-04-10 06:59:44.895533 onnx2kerastl-0.0.82.dev6/pyproject.toml
+-rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.82.dev6/PKG-INFO
```

### Comparing `onnx2kerastl-0.0.82.dev5/LICENSE` & `onnx2kerastl-0.0.82.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev5/onnx2kerastl/activation_layers.py` & `onnx2kerastl-0.0.82.dev6/onnx2kerastl/activation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev5/onnx2kerastl/caffe2_layers.py` & `onnx2kerastl-0.0.82.dev6/onnx2kerastl/caffe2_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev5/onnx2kerastl/constant_layers.py` & `onnx2kerastl-0.0.82.dev6/onnx2kerastl/constant_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev5/onnx2kerastl/converter.py` & `onnx2kerastl-0.0.82.dev6/onnx2kerastl/converter.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev5/onnx2kerastl/convolution_layers.py` & `onnx2kerastl-0.0.82.dev6/onnx2kerastl/convolution_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev5/onnx2kerastl/customonnxlayer/__init__.py` & `onnx2kerastl-0.0.82.dev6/onnx2kerastl/customonnxlayer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev5/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py` & `onnx2kerastl-0.0.82.dev6/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev5/onnx2kerastl/customonnxlayer/onnxlstm.py` & `onnx2kerastl-0.0.82.dev6/onnx2kerastl/customonnxlayer/onnxlstm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from keras.layers import Layer
 import tensorflow as tf
 
 
 class OnnxLSTM(Layer):
-    def __init__(self, units, return_sequences, return_lstm_state,  **kwargs):
+    def __init__(self, units: int, return_sequences: bool, return_lstm_state: bool,  **kwargs):
         super().__init__(**kwargs)
         self.lstm_layer = tf.keras.layers.LSTM(units, return_sequences=return_sequences,
                                                return_state=return_lstm_state)
         self.return_lstm_state = return_lstm_state
         self.return_sequences = return_sequences
         self.units = units
```

### Comparing `onnx2kerastl-0.0.82.dev5/onnx2kerastl/customonnxlayer/onnxreducemean.py` & `onnx2kerastl-0.0.82.dev6/onnx2kerastl/customonnxlayer/onnxreducemean.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev5/onnx2kerastl/elementwise_layers.py` & `onnx2kerastl-0.0.82.dev6/onnx2kerastl/elementwise_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev5/onnx2kerastl/layers.py` & `onnx2kerastl-0.0.82.dev6/onnx2kerastl/layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev5/onnx2kerastl/linear_layers.py` & `onnx2kerastl-0.0.82.dev6/onnx2kerastl/linear_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev5/onnx2kerastl/ltsm_layers.py` & `onnx2kerastl-0.0.82.dev6/onnx2kerastl/ltsm_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev5/onnx2kerastl/normalization_layers.py` & `onnx2kerastl-0.0.82.dev6/onnx2kerastl/normalization_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev5/onnx2kerastl/operation_layers.py` & `onnx2kerastl-0.0.82.dev6/onnx2kerastl/operation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev5/onnx2kerastl/padding_layers.py` & `onnx2kerastl-0.0.82.dev6/onnx2kerastl/padding_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev5/onnx2kerastl/pooling_layers.py` & `onnx2kerastl-0.0.82.dev6/onnx2kerastl/pooling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev5/onnx2kerastl/reshape_layers.py` & `onnx2kerastl-0.0.82.dev6/onnx2kerastl/reshape_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev5/onnx2kerastl/upsampling_layers.py` & `onnx2kerastl-0.0.82.dev6/onnx2kerastl/upsampling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev5/onnx2kerastl/utils.py` & `onnx2kerastl-0.0.82.dev6/onnx2kerastl/utils.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev5/pyproject.toml` & `onnx2kerastl-0.0.82.dev6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onnx2kerastl"
-version = "0.0.82.dev5"
+version = "0.0.82.dev6"
 description = ""
 authors = ["dorhar <doron.harnoy@tensorleap.ai>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 tensorflow = {version = "2.11.0", markers = "platform_machine  == 'x86_64'"}
```

### Comparing `onnx2kerastl-0.0.82.dev5/PKG-INFO` & `onnx2kerastl-0.0.82.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx2kerastl
-Version: 0.0.82.dev5
+Version: 0.0.82.dev6
 Summary: 
 License: MIT
 Author: dorhar
 Author-email: doron.harnoy@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

