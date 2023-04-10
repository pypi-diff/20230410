# Comparing `tmp/leap_model_parser-0.1.91.dev3.tar.gz` & `tmp/leap_model_parser-0.1.91.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leap_model_parser-0.1.91.dev3.tar", max compression
+gzip compressed data, was "leap_model_parser-0.1.91.dev4.tar", max compression
```

## Comparing `leap_model_parser-0.1.91.dev3.tar` & `leap_model_parser-0.1.91.dev4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1067 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev3/LICENSE
--rw-r--r--   0        0        0       68 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev3/README.md
--rw-r--r--   0        0        0      132 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev3/leap_model_parser/__init__.py
--rw-r--r--   0        0        0        0 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev3/leap_model_parser/contract/__init__.py
--rw-r--r--   0        0        0      691 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev3/leap_model_parser/contract/importmodelresponse.py
--rw-r--r--   0        0        0    43326 2023-04-10 08:28:02.352136 leap_model_parser-0.1.91.dev3/leap_model_parser/contract/nodedata.py
--rw-r--r--   0        0        0   415723 2023-04-10 08:28:02.352136 leap_model_parser-0.1.91.dev3/leap_model_parser/contract/ui_components.json
--rw-r--r--   0        0        0    15485 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev3/leap_model_parser/keras_json_model_import.py
--rw-r--r--   0        0        0     6766 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev3/leap_model_parser/model_parser.py
--rw-r--r--   0        0        0        0 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev3/leap_model_parser/utils/__init__.py
--rw-r--r--   0        0        0        0 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev3/leap_model_parser/utils/layerpedia/__init__.py
--rw-r--r--   0        0        0     9291 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev3/leap_model_parser/utils/layerpedia/layerpedia.py
--rw-r--r--   0        0        0        1 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev3/leap_model_parser/utils/tlinspection/__init__.py
--rw-r--r--   0        0        0     2804 2023-04-10 08:27:17.067591 leap_model_parser-0.1.91.dev3/leap_model_parser/utils/tlinspection/leapinspection.py
--rw-r--r--   0        0        0      111 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev3/leap_model_parser/utils/uicomponents/__init__.py
--rw-r--r--   0        0        0     3035 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev3/leap_model_parser/utils/uicomponents/generatenodedata.py
--rw-r--r--   0        0        0     5799 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev3/leap_model_parser/utils/uicomponents/tensorflowinscpection.py
--rw-r--r--   0        0        0    19604 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev3/leap_model_parser/utils/uicomponents/ui_components_config.yaml
--rw-r--r--   0        0        0     1062 2023-04-10 08:26:18.902973 leap_model_parser-0.1.91.dev3/pyproject.toml
--rw-r--r--   0        0        0     1018 1970-01-01 00:00:00.000000 leap_model_parser-0.1.91.dev3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev4/LICENSE
+-rw-r--r--   0        0        0       68 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev4/README.md
+-rw-r--r--   0        0        0      132 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev4/leap_model_parser/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev4/leap_model_parser/contract/__init__.py
+-rw-r--r--   0        0        0      691 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev4/leap_model_parser/contract/importmodelresponse.py
+-rw-r--r--   0        0        0    43326 2023-04-10 08:45:01.664324 leap_model_parser-0.1.91.dev4/leap_model_parser/contract/nodedata.py
+-rw-r--r--   0        0        0   415723 2023-04-10 08:45:01.664324 leap_model_parser-0.1.91.dev4/leap_model_parser/contract/ui_components.json
+-rw-r--r--   0        0        0    15485 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev4/leap_model_parser/keras_json_model_import.py
+-rw-r--r--   0        0        0     6766 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev4/leap_model_parser/model_parser.py
+-rw-r--r--   0        0        0        0 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev4/leap_model_parser/utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev4/leap_model_parser/utils/layerpedia/__init__.py
+-rw-r--r--   0        0        0     9291 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev4/leap_model_parser/utils/layerpedia/layerpedia.py
+-rw-r--r--   0        0        0        1 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev4/leap_model_parser/utils/tlinspection/__init__.py
+-rw-r--r--   0        0        0     2804 2023-04-10 08:45:01.660324 leap_model_parser-0.1.91.dev4/leap_model_parser/utils/tlinspection/leapinspection.py
+-rw-r--r--   0        0        0      111 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev4/leap_model_parser/utils/uicomponents/__init__.py
+-rw-r--r--   0        0        0     3035 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev4/leap_model_parser/utils/uicomponents/generatenodedata.py
+-rw-r--r--   0        0        0     5799 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev4/leap_model_parser/utils/uicomponents/tensorflowinscpection.py
+-rw-r--r--   0        0        0    19604 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev4/leap_model_parser/utils/uicomponents/ui_components_config.yaml
+-rw-r--r--   0        0        0     1062 2023-04-10 08:45:01.656324 leap_model_parser-0.1.91.dev4/pyproject.toml
+-rw-r--r--   0        0        0     1018 1970-01-01 00:00:00.000000 leap_model_parser-0.1.91.dev4/PKG-INFO
```

### Comparing `leap_model_parser-0.1.91.dev3/LICENSE` & `leap_model_parser-0.1.91.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev3/leap_model_parser/contract/importmodelresponse.py` & `leap_model_parser-0.1.91.dev4/leap_model_parser/contract/importmodelresponse.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev3/leap_model_parser/contract/nodedata.py` & `leap_model_parser-0.1.91.dev4/leap_model_parser/contract/nodedata.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev3/leap_model_parser/contract/ui_components.json` & `leap_model_parser-0.1.91.dev4/leap_model_parser/contract/ui_components.json`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev3/leap_model_parser/keras_json_model_import.py` & `leap_model_parser-0.1.91.dev4/leap_model_parser/keras_json_model_import.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev3/leap_model_parser/model_parser.py` & `leap_model_parser-0.1.91.dev4/leap_model_parser/model_parser.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev3/leap_model_parser/utils/layerpedia/layerpedia.py` & `leap_model_parser-0.1.91.dev4/leap_model_parser/utils/layerpedia/layerpedia.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev3/leap_model_parser/utils/tlinspection/leapinspection.py` & `leap_model_parser-0.1.91.dev4/leap_model_parser/utils/tlinspection/leapinspection.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev3/leap_model_parser/utils/uicomponents/generatenodedata.py` & `leap_model_parser-0.1.91.dev4/leap_model_parser/utils/uicomponents/generatenodedata.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev3/leap_model_parser/utils/uicomponents/tensorflowinscpection.py` & `leap_model_parser-0.1.91.dev4/leap_model_parser/utils/uicomponents/tensorflowinscpection.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev3/leap_model_parser/utils/uicomponents/ui_components_config.yaml` & `leap_model_parser-0.1.91.dev4/leap_model_parser/utils/uicomponents/ui_components_config.yaml`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev3/pyproject.toml` & `leap_model_parser-0.1.91.dev4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "leap-model-parser"
-version = "0.1.91.dev3"
+version = "0.1.91.dev4"
 description = ""
 authors = ["idan <idan.yogev@tensorleap.ai>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/tensorleap/leap-model-parser"
 homepage = "https://github.com/tensorleap/leap-model-parser"
 include = [
```

### Comparing `leap_model_parser-0.1.91.dev3/PKG-INFO` & `leap_model_parser-0.1.91.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leap-model-parser
-Version: 0.1.91.dev3
+Version: 0.1.91.dev4
 Summary: 
 Home-page: https://github.com/tensorleap/leap-model-parser
 License: MIT
 Author: idan
 Author-email: idan.yogev@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

