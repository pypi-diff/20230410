# Comparing `tmp/dioptra-1.0.7rc2.tar.gz` & `tmp/dioptra-1.0.7rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dioptra-1.0.7rc2.tar", last modified: Sun Apr  9 23:31:18 2023, max compression
+gzip compressed data, was "dioptra-1.0.7rc3.tar", last modified: Sun Apr  9 23:54:38 2023, max compression
```

## Comparing `dioptra-1.0.7rc2.tar` & `dioptra-1.0.7rc3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:31:18.794820 dioptra-1.0.7rc2/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1471 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/LICENSE.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2162 2023-04-09 23:31:18.794820 dioptra-1.0.7rc2/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1106 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:31:18.790820 dioptra-1.0.7rc2/dioptra/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       26 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/dioptra/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:31:18.790820 dioptra-1.0.7rc2/dioptra/inference/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/dioptra/inference/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1637 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/dioptra/inference/inference_runner.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:31:18.790820 dioptra-1.0.7rc2/dioptra/inference/tf/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/dioptra/inference/tf/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5495 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/dioptra/inference/tf/tf_runner.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:31:18.790820 dioptra-1.0.7rc2/dioptra/inference/torch/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/dioptra/inference/torch/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6689 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/dioptra/inference/torch/torch_runner.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:31:18.790820 dioptra-1.0.7rc2/dioptra/lake/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/dioptra/lake/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7912 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/dioptra/lake/datasets.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:31:18.790820 dioptra-1.0.7rc2/dioptra/lake/torch/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/dioptra/lake/torch/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4545 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/dioptra/lake/torch/object_store_datasets.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    27205 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/dioptra/lake/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:31:18.794820 dioptra-1.0.7rc2/dioptra/miners/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      416 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/dioptra/miners/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2830 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/dioptra/miners/activation_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3962 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/dioptra/miners/base_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3225 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/dioptra/miners/coreset_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1804 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/dioptra/miners/entropy_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3203 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/dioptra/miners/knn_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1728 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/dioptra/miners/random_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1804 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/dioptra/miners/variance_miner.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:31:18.790820 dioptra-1.0.7rc2/dioptra.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2162 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/dioptra.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/dioptra.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/dioptra.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      229 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/dioptra.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        8 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/dioptra.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-09 23:31:18.794820 dioptra-1.0.7rc2/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1656 2023-04-09 23:31:18.000000 dioptra-1.0.7rc2/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.699961 dioptra-1.0.7rc3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1471 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/LICENSE.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2162 2023-04-09 23:54:38.699961 dioptra-1.0.7rc3/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1106 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.695961 dioptra-1.0.7rc3/dioptra/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       26 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.699961 dioptra-1.0.7rc3/dioptra/inference/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/inference/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1637 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/inference/inference_runner.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.699961 dioptra-1.0.7rc3/dioptra/inference/tf/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/inference/tf/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5495 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/inference/tf/tf_runner.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.699961 dioptra-1.0.7rc3/dioptra/inference/torch/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/inference/torch/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6689 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/inference/torch/torch_runner.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.699961 dioptra-1.0.7rc3/dioptra/lake/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/lake/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7912 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/lake/datasets.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.699961 dioptra-1.0.7rc3/dioptra/lake/torch/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/lake/torch/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4545 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/lake/torch/object_store_datasets.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    27205 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/lake/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.699961 dioptra-1.0.7rc3/dioptra/miners/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      416 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/miners/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2848 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/miners/activation_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3962 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/miners/base_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3230 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/miners/coreset_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1802 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/miners/entropy_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3208 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/miners/knn_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1787 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/miners/random_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1804 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra/miners/variance_miner.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 23:54:38.699961 dioptra-1.0.7rc3/dioptra.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2162 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      229 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        8 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/dioptra.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-09 23:54:38.699961 dioptra-1.0.7rc3/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1656 2023-04-09 23:54:38.000000 dioptra-1.0.7rc3/setup.py
```

### Comparing `dioptra-1.0.7rc2/LICENSE.md` & `dioptra-1.0.7rc3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.7rc2/PKG-INFO` & `dioptra-1.0.7rc3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dioptra
-Version: 1.0.7rc2
+Version: 1.0.7rc3
 Summary: Client library to log data to Dioptra API
 Home-page: https://github.com/dioptra-ai/collector-py
 Author: dioptra.ai
 Author-email: info@dioptra.ai
 License: BSD
 Project-URL: dioptra.ai, https://www.dioptra.ai
 Description: <div align="center">
```

### Comparing `dioptra-1.0.7rc2/README.md` & `dioptra-1.0.7rc3/README.md`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.7rc2/dioptra/inference/inference_runner.py` & `dioptra-1.0.7rc3/dioptra/inference/inference_runner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.7rc2/dioptra/inference/tf/tf_runner.py` & `dioptra-1.0.7rc3/dioptra/inference/tf/tf_runner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.7rc2/dioptra/inference/torch/torch_runner.py` & `dioptra-1.0.7rc3/dioptra/inference/torch/torch_runner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.7rc2/dioptra/lake/datasets.py` & `dioptra-1.0.7rc3/dioptra/lake/datasets.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.7rc2/dioptra/lake/torch/object_store_datasets.py` & `dioptra-1.0.7rc3/dioptra/lake/torch/object_store_datasets.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.7rc2/dioptra/lake/utils.py` & `dioptra-1.0.7rc3/dioptra/lake/utils.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.7rc2/dioptra/miners/activation_miner.py` & `dioptra-1.0.7rc3/dioptra/miners/activation_miner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import requests
 from .base_miner import BaseMiner
 
 class ActivationMiner(BaseMiner):
     def __init__(
-            self, display_name, size, select_filters, model_name,
-            embeddings_field,
+            self, display_name, size, select_filters, model_name=None,
+            embeddings_field='embeddings',
             select_limit=None, select_order_by=None, select_desc=None,
             select_reference_filters=None, select_reference_limit=None,
             select_reference_order_by=None, select_reference_desc=None,
             skip_caching=True):
         """
         Activation miner
         Will perform a AL query based on activation
```

### Comparing `dioptra-1.0.7rc2/dioptra/miners/base_miner.py` & `dioptra-1.0.7rc3/dioptra/miners/base_miner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.7rc2/dioptra/miners/coreset_miner.py` & `dioptra-1.0.7rc3/dioptra/miners/coreset_miner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 from .base_miner import BaseMiner
 
 class CoresetMiner(BaseMiner):
     def __init__(
-            self, display_name, size, select_filters, model_name,
+            self, display_name, size, select_filters, model_name=None,
             embeddings_field='embeddings', metric='euclidean',
             select_limit=None, select_order_by=None, select_desc=None,
             select_reference_filters=None, select_reference_limit=None,
             select_reference_order_by=None, select_reference_desc=None,
             skip_caching=True):
         """
         CoreSet miner
```

### Comparing `dioptra-1.0.7rc2/dioptra/miners/entropy_miner.py` & `dioptra-1.0.7rc3/dioptra/miners/entropy_miner.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
                 'content-type': 'application/json',
                 'x-api-key': self.api_key
             },
             json={
                 'display_name': display_name,
                 'strategy': 'ENTROPY',
                 'size': size,
-                'model_name': 'model_name',
+                'model_name': model_name,
                 'select': {
                     'filters': select_filters,
                     **({'limit': select_limit} if select_limit is not None else {}),
                     **({'order_by': select_order_by} if select_order_by is not None else {}),
                     **({'desc': select_desc} if select_desc is not None else {}),
                 }
             })
```

### Comparing `dioptra-1.0.7rc2/dioptra/miners/knn_miner.py` & `dioptra-1.0.7rc3/dioptra/miners/knn_miner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 from .base_miner import BaseMiner
 
 class KNNMiner(BaseMiner):
     def __init__(
-            self, display_name, size, select_filters, model_name,
+            self, display_name, size, select_filters, model_name=None,
             embeddings_field='embeddings', metric='euclidean',
             select_limit=None, select_order_by=None, select_desc=None,
             select_reference_filters=None, select_reference_limit=None,
             select_reference_order_by=None, select_reference_desc=None,
             skip_caching=True):
         """
         KNN miner
```

### Comparing `dioptra-1.0.7rc2/dioptra/miners/random_miner.py` & `dioptra-1.0.7rc3/dioptra/miners/random_miner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import requests
 from .base_miner import BaseMiner
 
 class RandomMiner(BaseMiner):
     def __init__(
             self, display_name, size, select_filters,
-            select_limit=None, select_order_by=None, select_desc=None):
+            select_limit=None, select_order_by=None, select_desc=None, model_name=None):
         """
         Random miner
         Will perform a random query
 
         Parameters:
             display_name: name to be displayed in Dioptra
             size: number of datapoints to query
@@ -25,14 +25,15 @@
                 'content-type': 'application/json',
                 'x-api-key': self.api_key
             },
             json={
                 'display_name': display_name,
                 'strategy': 'RANDOM',
                 'size': size,
+                'model_name': model_name,
                 'select': {
                     'filters': select_filters,
                     **({'limit': select_limit} if select_limit is not None else {}),
                     **({'order_by': select_order_by} if select_order_by is not None else {}),
                     **({'desc': select_desc} if select_desc is not None else {}),
                 }
             })
```

### Comparing `dioptra-1.0.7rc2/dioptra/miners/variance_miner.py` & `dioptra-1.0.7rc3/dioptra/miners/variance_miner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.7rc2/dioptra.egg-info/PKG-INFO` & `dioptra-1.0.7rc3/dioptra.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dioptra
-Version: 1.0.7rc2
+Version: 1.0.7rc3
 Summary: Client library to log data to Dioptra API
 Home-page: https://github.com/dioptra-ai/collector-py
 Author: dioptra.ai
 Author-email: info@dioptra.ai
 License: BSD
 Project-URL: dioptra.ai, https://www.dioptra.ai
 Description: <div align="center">
```

### Comparing `dioptra-1.0.7rc2/dioptra.egg-info/SOURCES.txt` & `dioptra-1.0.7rc3/dioptra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.7rc2/setup.py` & `dioptra-1.0.7rc3/setup.py`

 * *Files identical despite different names*

