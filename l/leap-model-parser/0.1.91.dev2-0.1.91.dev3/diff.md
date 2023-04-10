# Comparing `tmp/leap_model_parser-0.1.91.dev2.tar.gz` & `tmp/leap_model_parser-0.1.91.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leap_model_parser-0.1.91.dev2.tar", max compression
+gzip compressed data, was "leap_model_parser-0.1.91.dev3.tar", max compression
```

## Comparing `leap_model_parser-0.1.91.dev2.tar` & `leap_model_parser-0.1.91.dev3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1067 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev2/LICENSE
--rw-r--r--   0        0        0       68 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev2/README.md
--rw-r--r--   0        0        0      132 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev2/leap_model_parser/__init__.py
--rw-r--r--   0        0        0        0 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev2/leap_model_parser/contract/__init__.py
--rw-r--r--   0        0        0      691 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev2/leap_model_parser/contract/importmodelresponse.py
--rw-r--r--   0        0        0    43327 2023-04-10 07:03:59.376411 leap_model_parser-0.1.91.dev2/leap_model_parser/contract/nodedata.py
--rw-r--r--   0        0        0   415724 2023-04-10 07:03:59.376411 leap_model_parser-0.1.91.dev2/leap_model_parser/contract/ui_components.json
--rw-r--r--   0        0        0    15485 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev2/leap_model_parser/keras_json_model_import.py
--rw-r--r--   0        0        0     6766 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev2/leap_model_parser/model_parser.py
--rw-r--r--   0        0        0        0 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev2/leap_model_parser/utils/__init__.py
--rw-r--r--   0        0        0        0 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev2/leap_model_parser/utils/layerpedia/__init__.py
--rw-r--r--   0        0        0     9291 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev2/leap_model_parser/utils/layerpedia/layerpedia.py
--rw-r--r--   0        0        0        1 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev2/leap_model_parser/utils/tlinspection/__init__.py
--rw-r--r--   0        0        0     2786 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev2/leap_model_parser/utils/tlinspection/leapinspection.py
--rw-r--r--   0        0        0      111 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev2/leap_model_parser/utils/uicomponents/__init__.py
--rw-r--r--   0        0        0     3035 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev2/leap_model_parser/utils/uicomponents/generatenodedata.py
--rw-r--r--   0        0        0     5799 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev2/leap_model_parser/utils/uicomponents/tensorflowinscpection.py
--rw-r--r--   0        0        0    19604 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev2/leap_model_parser/utils/uicomponents/ui_components_config.yaml
--rw-r--r--   0        0        0     1062 2023-04-10 07:05:49.776789 leap_model_parser-0.1.91.dev2/pyproject.toml
--rw-r--r--   0        0        0     1018 1970-01-01 00:00:00.000000 leap_model_parser-0.1.91.dev2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev3/LICENSE
+-rw-r--r--   0        0        0       68 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev3/README.md
+-rw-r--r--   0        0        0      132 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev3/leap_model_parser/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev3/leap_model_parser/contract/__init__.py
+-rw-r--r--   0        0        0      691 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev3/leap_model_parser/contract/importmodelresponse.py
+-rw-r--r--   0        0        0    43326 2023-04-10 08:28:02.352136 leap_model_parser-0.1.91.dev3/leap_model_parser/contract/nodedata.py
+-rw-r--r--   0        0        0   415723 2023-04-10 08:28:02.352136 leap_model_parser-0.1.91.dev3/leap_model_parser/contract/ui_components.json
+-rw-r--r--   0        0        0    15485 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev3/leap_model_parser/keras_json_model_import.py
+-rw-r--r--   0        0        0     6766 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev3/leap_model_parser/model_parser.py
+-rw-r--r--   0        0        0        0 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev3/leap_model_parser/utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev3/leap_model_parser/utils/layerpedia/__init__.py
+-rw-r--r--   0        0        0     9291 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev3/leap_model_parser/utils/layerpedia/layerpedia.py
+-rw-r--r--   0        0        0        1 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev3/leap_model_parser/utils/tlinspection/__init__.py
+-rw-r--r--   0        0        0     2804 2023-04-10 08:27:17.067591 leap_model_parser-0.1.91.dev3/leap_model_parser/utils/tlinspection/leapinspection.py
+-rw-r--r--   0        0        0      111 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev3/leap_model_parser/utils/uicomponents/__init__.py
+-rw-r--r--   0        0        0     3035 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev3/leap_model_parser/utils/uicomponents/generatenodedata.py
+-rw-r--r--   0        0        0     5799 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev3/leap_model_parser/utils/uicomponents/tensorflowinscpection.py
+-rw-r--r--   0        0        0    19604 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev3/leap_model_parser/utils/uicomponents/ui_components_config.yaml
+-rw-r--r--   0        0        0     1062 2023-04-10 08:26:18.902973 leap_model_parser-0.1.91.dev3/pyproject.toml
+-rw-r--r--   0        0        0     1018 1970-01-01 00:00:00.000000 leap_model_parser-0.1.91.dev3/PKG-INFO
```

### Comparing `leap_model_parser-0.1.91.dev2/LICENSE` & `leap_model_parser-0.1.91.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev2/leap_model_parser/contract/importmodelresponse.py` & `leap_model_parser-0.1.91.dev3/leap_model_parser/contract/importmodelresponse.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev2/leap_model_parser/contract/nodedata.py` & `leap_model_parser-0.1.91.dev3/leap_model_parser/contract/nodedata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from dataclasses import dataclass
-from typing import Union
 from typing import List
+from dataclasses import dataclass
 from enum import Enum
+from typing import Union
 
 
 class ActivationsEnum(Enum):
     relu = "relu"
     softmax = "softmax"
     selu = "selu"
     softplus = "softplus"
@@ -1806,17 +1806,17 @@
     alpha: float
     beta: float
     type: NodeType
 
 
 @dataclass
 class OnnxLSTM:
-    units: None
-    return_sequences: None
-    return_lstm_state: None
+    units: int
+    return_sequences: bool
+    return_lstm_state: bool
     type: NodeType
 
 
 @dataclass
 class OnnxReduceMean:
     axes: List[int]
     keepdims: bool
```

### Comparing `leap_model_parser-0.1.91.dev2/leap_model_parser/contract/ui_components.json` & `leap_model_parser-0.1.91.dev3/leap_model_parser/contract/ui_components.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999591503267974%*

 * *Differences: {'135': "{'properties': {0: {'type': 'int'}, 1: {'type': 'bool'}, 2: {'type': 'bool'}}}"}*

```diff
@@ -14596,27 +14596,27 @@
             "onnxlstm"
         ],
         "properties": [
             {
                 "default_val": null,
                 "isdefault": false,
                 "name": "units",
-                "type": "None"
+                "type": "int"
             },
             {
                 "default_val": null,
                 "isdefault": false,
                 "name": "return_sequences",
-                "type": "None"
+                "type": "bool"
             },
             {
                 "default_val": null,
                 "isdefault": false,
                 "name": "return_lstm_state",
-                "type": "None"
+                "type": "bool"
             }
         ],
         "receptive_fields_func": "IdentityReceptiveFieldsFunc",
         "shape_calc": [
             "IdentityFunc"
         ],
         "type": "Layer"
```

### Comparing `leap_model_parser-0.1.91.dev2/leap_model_parser/keras_json_model_import.py` & `leap_model_parser-0.1.91.dev3/leap_model_parser/keras_json_model_import.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev2/leap_model_parser/model_parser.py` & `leap_model_parser-0.1.91.dev3/leap_model_parser/model_parser.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev2/leap_model_parser/utils/layerpedia/layerpedia.py` & `leap_model_parser-0.1.91.dev3/leap_model_parser/utils/layerpedia/layerpedia.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev2/leap_model_parser/utils/tlinspection/leapinspection.py` & `leap_model_parser-0.1.91.dev3/leap_model_parser/utils/tlinspection/leapinspection.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                 classes.append(cls_dict)
 
         return classes
 
     @staticmethod
     def get_type(func, pval):
         dtype_map = {'int': ['int', 'Integer', 'number'], 'float': ['float'], 'str': ['string', 'str'],
-                     'name': ['name'], 'tuple': ["tuple", "Tuple"]}
+                     'name': ['name'], 'tuple': ["tuple", "Tuple"], 'bool': ['bool']}
         if pval.default != inspect._empty:
             return str(type(pval.default)).split('\'')[1]
         # TODO: comment out due to missing CallableMeta type in python 3.8, if an error occurs from this section consider
         # finding the right way to write this if in python 3.8
         # if isinstance(pval.annotation, CallableMeta):
         #     return Callable
         if pval.annotation is str:
```

### Comparing `leap_model_parser-0.1.91.dev2/leap_model_parser/utils/uicomponents/generatenodedata.py` & `leap_model_parser-0.1.91.dev3/leap_model_parser/utils/uicomponents/generatenodedata.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev2/leap_model_parser/utils/uicomponents/tensorflowinscpection.py` & `leap_model_parser-0.1.91.dev3/leap_model_parser/utils/uicomponents/tensorflowinscpection.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev2/leap_model_parser/utils/uicomponents/ui_components_config.yaml` & `leap_model_parser-0.1.91.dev3/leap_model_parser/utils/uicomponents/ui_components_config.yaml`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev2/pyproject.toml` & `leap_model_parser-0.1.91.dev3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "leap-model-parser"
-version = "0.1.91.dev2"
+version = "0.1.91.dev3"
 description = ""
 authors = ["idan <idan.yogev@tensorleap.ai>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/tensorleap/leap-model-parser"
 homepage = "https://github.com/tensorleap/leap-model-parser"
 include = [
@@ -14,15 +14,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 tensorflow = {version = "2.11.0", markers = "platform_machine  == 'x86_64'"}
 tensorflow-macos = {version = "2.11.0", markers = "platform_machine  == 'arm64'"}
 numpy = "^1.22.3"
 onnx = "1.10.1"
-onnx2kerastl = "0.0.82.dev6"
+onnx2kerastl = "0.0.82.dev7"
 keras-data-format-converter = "0.1.14"
 leap-model-rebuilder = "0.1.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.1"
 mypy = "^0.941"
 grappa = "^1.0.1"
```

### Comparing `leap_model_parser-0.1.91.dev2/PKG-INFO` & `leap_model_parser-0.1.91.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leap-model-parser
-Version: 0.1.91.dev2
+Version: 0.1.91.dev3
 Summary: 
 Home-page: https://github.com/tensorleap/leap-model-parser
 License: MIT
 Author: idan
 Author-email: idan.yogev@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: keras-data-format-converter (==0.1.14)
 Requires-Dist: leap-model-rebuilder (==0.1.5)
 Requires-Dist: numpy (>=1.22.3,<2.0.0)
 Requires-Dist: onnx (==1.10.1)
-Requires-Dist: onnx2kerastl (==0.0.82.dev6)
+Requires-Dist: onnx2kerastl (==0.0.82.dev7)
 Requires-Dist: tensorflow (==2.11.0) ; platform_machine == "x86_64"
 Requires-Dist: tensorflow-macos (==2.11.0) ; platform_machine == "arm64"
 Project-URL: Repository, https://github.com/tensorleap/leap-model-parser
 Description-Content-Type: text/markdown
 
 # Tensorleap model parser
 Used to parse model to the import format
```

