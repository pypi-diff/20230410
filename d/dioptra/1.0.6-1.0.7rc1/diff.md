# Comparing `tmp/dioptra-1.0.6.tar.gz` & `tmp/dioptra-1.0.7rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dioptra-1.0.6.tar", last modified: Fri Apr  7 15:50:15 2023, max compression
+gzip compressed data, was "dioptra-1.0.7rc1.tar", last modified: Sun Apr  9 22:53:28 2023, max compression
```

## Comparing `dioptra-1.0.6.tar` & `dioptra-1.0.7rc1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-07 15:50:15.733442 dioptra-1.0.6/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1471 2023-04-07 15:50:15.000000 dioptra-1.0.6/LICENSE.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2159 2023-04-07 15:50:15.729442 dioptra-1.0.6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1106 2023-04-07 15:50:15.000000 dioptra-1.0.6/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-07 15:50:15.729442 dioptra-1.0.6/dioptra/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       22 2023-04-07 15:50:15.000000 dioptra-1.0.6/dioptra/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-07 15:50:15.729442 dioptra-1.0.6/dioptra/inference/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-07 15:50:15.000000 dioptra-1.0.6/dioptra/inference/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1637 2023-04-07 15:50:15.000000 dioptra-1.0.6/dioptra/inference/inference_runner.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-07 15:50:15.729442 dioptra-1.0.6/dioptra/inference/tf/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-07 15:50:15.000000 dioptra-1.0.6/dioptra/inference/tf/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4231 2023-04-07 15:50:15.000000 dioptra-1.0.6/dioptra/inference/tf/tf_runner.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-07 15:50:15.729442 dioptra-1.0.6/dioptra/inference/torch/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-07 15:50:15.000000 dioptra-1.0.6/dioptra/inference/torch/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6774 2023-04-07 15:50:15.000000 dioptra-1.0.6/dioptra/inference/torch/torch_runner.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-07 15:50:15.729442 dioptra-1.0.6/dioptra/lake/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-07 15:50:15.000000 dioptra-1.0.6/dioptra/lake/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7912 2023-04-07 15:50:15.000000 dioptra-1.0.6/dioptra/lake/datasets.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-07 15:50:15.729442 dioptra-1.0.6/dioptra/lake/torch/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-07 15:50:15.000000 dioptra-1.0.6/dioptra/lake/torch/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4545 2023-04-07 15:50:15.000000 dioptra-1.0.6/dioptra/lake/torch/object_store_datasets.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    27205 2023-04-07 15:50:15.000000 dioptra-1.0.6/dioptra/lake/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-07 15:50:15.729442 dioptra-1.0.6/dioptra/miners/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      416 2023-04-07 15:50:15.000000 dioptra-1.0.6/dioptra/miners/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2842 2023-04-07 15:50:15.000000 dioptra-1.0.6/dioptra/miners/activation_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3661 2023-04-07 15:50:15.000000 dioptra-1.0.6/dioptra/miners/base_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3249 2023-04-07 15:50:15.000000 dioptra-1.0.6/dioptra/miners/coreset_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1804 2023-04-07 15:50:15.000000 dioptra-1.0.6/dioptra/miners/entropy_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3227 2023-04-07 15:50:15.000000 dioptra-1.0.6/dioptra/miners/knn_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1728 2023-04-07 15:50:15.000000 dioptra-1.0.6/dioptra/miners/random_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1804 2023-04-07 15:50:15.000000 dioptra-1.0.6/dioptra/miners/variance_miner.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-07 15:50:15.729442 dioptra-1.0.6/dioptra.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2159 2023-04-07 15:50:15.000000 dioptra-1.0.6/dioptra.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2023-04-07 15:50:15.000000 dioptra-1.0.6/dioptra.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-07 15:50:15.000000 dioptra-1.0.6/dioptra.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      229 2023-04-07 15:50:15.000000 dioptra-1.0.6/dioptra.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        8 2023-04-07 15:50:15.000000 dioptra-1.0.6/dioptra.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-07 15:50:15.733442 dioptra-1.0.6/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1656 2023-04-07 15:50:15.000000 dioptra-1.0.6/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 22:53:28.256914 dioptra-1.0.7rc1/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1471 2023-04-09 22:53:27.000000 dioptra-1.0.7rc1/LICENSE.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2162 2023-04-09 22:53:28.256914 dioptra-1.0.7rc1/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1106 2023-04-09 22:53:27.000000 dioptra-1.0.7rc1/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 22:53:28.248914 dioptra-1.0.7rc1/dioptra/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       26 2023-04-09 22:53:27.000000 dioptra-1.0.7rc1/dioptra/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 22:53:28.252914 dioptra-1.0.7rc1/dioptra/inference/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-09 22:53:27.000000 dioptra-1.0.7rc1/dioptra/inference/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1637 2023-04-09 22:53:27.000000 dioptra-1.0.7rc1/dioptra/inference/inference_runner.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 22:53:28.252914 dioptra-1.0.7rc1/dioptra/inference/tf/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-09 22:53:27.000000 dioptra-1.0.7rc1/dioptra/inference/tf/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5495 2023-04-09 22:53:27.000000 dioptra-1.0.7rc1/dioptra/inference/tf/tf_runner.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 22:53:28.252914 dioptra-1.0.7rc1/dioptra/inference/torch/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-09 22:53:27.000000 dioptra-1.0.7rc1/dioptra/inference/torch/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6689 2023-04-09 22:53:27.000000 dioptra-1.0.7rc1/dioptra/inference/torch/torch_runner.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 22:53:28.252914 dioptra-1.0.7rc1/dioptra/lake/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-09 22:53:27.000000 dioptra-1.0.7rc1/dioptra/lake/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7912 2023-04-09 22:53:27.000000 dioptra-1.0.7rc1/dioptra/lake/datasets.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 22:53:28.252914 dioptra-1.0.7rc1/dioptra/lake/torch/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-09 22:53:27.000000 dioptra-1.0.7rc1/dioptra/lake/torch/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4545 2023-04-09 22:53:27.000000 dioptra-1.0.7rc1/dioptra/lake/torch/object_store_datasets.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    27205 2023-04-09 22:53:27.000000 dioptra-1.0.7rc1/dioptra/lake/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 22:53:28.252914 dioptra-1.0.7rc1/dioptra/miners/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      416 2023-04-09 22:53:27.000000 dioptra-1.0.7rc1/dioptra/miners/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2830 2023-04-09 22:53:27.000000 dioptra-1.0.7rc1/dioptra/miners/activation_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3905 2023-04-09 22:53:27.000000 dioptra-1.0.7rc1/dioptra/miners/base_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3225 2023-04-09 22:53:27.000000 dioptra-1.0.7rc1/dioptra/miners/coreset_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1804 2023-04-09 22:53:27.000000 dioptra-1.0.7rc1/dioptra/miners/entropy_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3203 2023-04-09 22:53:27.000000 dioptra-1.0.7rc1/dioptra/miners/knn_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1728 2023-04-09 22:53:27.000000 dioptra-1.0.7rc1/dioptra/miners/random_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1804 2023-04-09 22:53:27.000000 dioptra-1.0.7rc1/dioptra/miners/variance_miner.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-09 22:53:28.252914 dioptra-1.0.7rc1/dioptra.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2162 2023-04-09 22:53:28.000000 dioptra-1.0.7rc1/dioptra.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2023-04-09 22:53:28.000000 dioptra-1.0.7rc1/dioptra.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-09 22:53:28.000000 dioptra-1.0.7rc1/dioptra.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      229 2023-04-09 22:53:28.000000 dioptra-1.0.7rc1/dioptra.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        8 2023-04-09 22:53:28.000000 dioptra-1.0.7rc1/dioptra.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-09 22:53:28.256914 dioptra-1.0.7rc1/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1656 2023-04-09 22:53:27.000000 dioptra-1.0.7rc1/setup.py
```

### Comparing `dioptra-1.0.6/LICENSE.md` & `dioptra-1.0.7rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.6/PKG-INFO` & `dioptra-1.0.7rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dioptra
-Version: 1.0.6
+Version: 1.0.7rc1
 Summary: Client library to log data to Dioptra API
 Home-page: https://github.com/dioptra-ai/collector-py
 Author: dioptra.ai
 Author-email: info@dioptra.ai
 License: BSD
 Project-URL: dioptra.ai, https://www.dioptra.ai
 Description: <div align="center">
```

### Comparing `dioptra-1.0.6/README.md` & `dioptra-1.0.7rc1/README.md`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.6/dioptra/inference/inference_runner.py` & `dioptra-1.0.7rc1/dioptra/inference/inference_runner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.6/dioptra/inference/tf/tf_runner.py` & `dioptra-1.0.7rc1/dioptra/inference/tf/tf_runner.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,38 +5,48 @@
 from dioptra.inference.inference_runner import InferenceRunner
 from dioptra.lake.utils import _format_prediction
 
 class TfInferenceRunner(InferenceRunner):
     def __init__(
             self, model, model_type,
             model_name = None,
+            datapoint_ids = [],
             embeddings_layers=[],
-            logits_layer=None, class_names=[],
-            metadata=None):
+            logits_layer=None,
+            class_names=[],
+            datapoints_metadata=None,
+            dataset_metadata=None,
+            mc_dropout_samples=0):
         """
         Utility to perform model inference on a dataset and extract layers needed for AL.
 
         Parameters:
             model: model to be used to inference
+            model_name: the name of the model
             model_type: the type of the model use. Can be CLASSIFICATION or SEGMENTATION
-            embeddings_layers: an array of layer names that should be used as embeddings. Can be a jq style path to an embedding layer like [0].my_embedding
-            logits_layer: the name of the logit layer (pre softmax) to be used for AL. Can be a jq style path to an embedding layer like [0].my_logits
+            datapoint_ids: alist of datapoints to update with the predictions. Should be in the same order as the dataset.
+            embeddings_layers: an array of layer names that should be used as embeddings
+            logits_layer: the name of the logit layer (pre softmax) to be used for AL
             class_names: the class names corresponding to each logit. Indexes should match the logit layer
-            metadata: a list of dioptra style metadata to be added to teh datapoints. The indexes in this list should match the indexes in the dataset
+            datapoints_metadata: a list of dioptra style datapoints metadata to be added to teh datapoints. The indexes in this list should match the indexes in the dataset
+            dataset_metadata: a dioptra style dataset metadata to be added to the dataset
         """
 
         super().__init__()
 
         self.model = model
         self.model_name = model_name
+        self.datapoint_ids = datapoint_ids
         self.embeddings_layers = embeddings_layers
         self.logits_layer = logits_layer
         self.class_names = class_names
-        self.metadata = metadata
+        self.datapoints_metadata = datapoints_metadata
+        self.dataset_metadata = dataset_metadata
         self.model_type = model_type
+        self.mc_dropout_samples = mc_dropout_samples
 
         input_layer = model.inputs
         if input_layer is None:
             input_layer = model.layers[0].inputs
 
         output_layers = {}
 
@@ -69,44 +79,63 @@
                 Should be batched and pre processed to only return the data, not the groundtruth
                 Should not be shuffled if used with a metadata list
         """
 
         records = []
 
         global_idx = 0
+        nb_samples = 1 if self.mc_dropout_samples == 0 else self.mc_dropout_samples
+
+        for _, batch in tqdm(enumerate(dataset), desc='running inference...'):
+            samples_records = []
+            for _ in range(nb_samples):
+                batch_global_idx = global_idx
+                batch_records = []
+                output = self.logging_model(batch, training=self.mc_dropout_samples > 0)
+                for batch_idx in range(batch.shape[0]):
+                    batch_records.extend(self._build_records(batch_idx, batch_global_idx, output))
+                    batch_global_idx += 1
+                samples_records.append(batch_records)
+
+            resolved_records = self._resolve_records(samples_records)
+            records.extend(resolved_records)
+            global_idx += len(batch)
+
+            if len(records) > 0:
+                self._ingest_data(records)
+                records = []
 
-        for batch_index, batch in tqdm(enumerate(dataset), desc='running inference...'):
-            output = self.logging_model(batch)
-            for batch_idx in range(batch.shape[0]):
-                records.extend(self._build_records(batch_idx, global_idx, output))
-                global_idx += 1
-                if len(records) > self.max_batch_size:
-                    self._ingest_data(records)
-                    records = []
         if len(records) > 0:
             self._ingest_data(records)
             records = []
 
     def _build_records(self, record_batch_idx, record_global_idx, output):
+
+        datapoint_id = None
+        if record_global_idx < len(self.datapoint_ids):
+            datapoint_id = self.datapoint_ids[record_global_idx]
+
         logits = None
         if self.logits_layer is not None:
             logits = output[self.logits_layer][record_batch_idx].numpy()
-        
+
         embeddings = {}
         for my_layer in self.embeddings_layers:
             embeddings[my_layer] = output[my_layer][record_batch_idx].numpy()
 
         return [{
             **({
                 'prediction': _format_prediction(
                     logits=logits,
                     embeddings=embeddings,
                     task_type=self.model_type,
                     model_name=self.model_name,
                     class_names=self.class_names
                 )
-               } if logits or embeddings else {}
+               } if logits is not None or embeddings is not None else {}
+            ),
+            **({'id': datapoint_id} if datapoint_id is not None else {}),
+            **(self.datapoints_metadata[record_global_idx] \
+               if self.datapoints_metadata and len(self.datapoints_metadata) > record_global_idx else {}
             ),
-            **(self.metadata[record_global_idx] \
-               if self.metadata and len(self.metadata) > record_global_idx else {}
-            )
+            **(self.dataset_metadata if self.dataset_metadata else {})
         }]
```

### Comparing `dioptra-1.0.6/dioptra/inference/torch/torch_runner.py` & `dioptra-1.0.7rc1/dioptra/inference/torch/torch_runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,19 +46,14 @@
         self.datapoints_metadata = datapoints_metadata
         self.dataset_metadata = dataset_metadata
         self.data_transform = data_transform
         self.device = device
         self.model_type = model_type
         self.mc_dropout_samples = mc_dropout_samples
 
-        if mc_dropout_samples > 0:
-            for m in self.model.modules():
-                if m.__class__.__name__.startswith('Dropout'):
-                    m.train()
-
         self.activation = {}
 
         for my_layer_name in embeddings_layers + [logits_layer]:
             if my_layer_name is not None:
                 my_layer = self._get_layer_by_name(my_layer_name)
                 my_layer.register_forward_hook(self._get_activation(my_layer_name))
 
@@ -87,30 +82,34 @@
 
         Parameters:
             dataset: a torch.utils.data.Dataset
                 Should be batched. data_transform can be used to pre process teh data to only return the data, not the groundtruth
                 Should not be shuffled if used with a datapoints_metadata list
         """
 
-        self.model.eval()
+        if self.mc_dropout_samples == 0:
+            self.model.eval()
+        else:
+            self.model.train()
+
         self.model.to(self.device)
 
         records = []
 
         global_idx = 0
+        nb_samples = 1 if self.mc_dropout_samples == 0 else self.mc_dropout_samples
+
         if hasattr(dataloader, 'dataset'):
             dataset_size = len(dataloader.dataset) # we are using a dataloader
         else:
             dataset_size = len(dataloader)  # we are using a dataset directly
         for _, batch in tqdm(enumerate(dataloader), desc='running inference...'):
             if self.data_transform:
                 batch = self.data_transform(batch)
             batch = batch.to(self.device)
-
-            nb_samples = 1 if self.mc_dropout_samples == 0 else self.mc_dropout_samples
             samples_records = []
 
             for _ in range(nb_samples):
                 batch_global_idx = global_idx
                 batch_records = []
                 with torch.no_grad():
                     self.model(batch)
```

### Comparing `dioptra-1.0.6/dioptra/lake/datasets.py` & `dioptra-1.0.7rc1/dioptra/lake/datasets.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.6/dioptra/lake/torch/object_store_datasets.py` & `dioptra-1.0.7rc1/dioptra/lake/torch/object_store_datasets.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.6/dioptra/lake/utils.py` & `dioptra-1.0.7rc1/dioptra/lake/utils.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.6/dioptra/miners/activation_miner.py` & `dioptra-1.0.7rc1/dioptra/miners/activation_miner.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         """
         Activation miner
         Will perform a AL query based on activation
 
         Parameters:
             display_name: name to be displayed in Dioptra
             size: number of datapoints to query
-            embeddings_field: embedding fields to run the analysis on. Could be 'embeddings' 'prediction.embeddings'
+            embeddings_field: embedding fields to run the analysis on. Could be 'embeddings' or 'logits'
             select_filters: dioptra style filters to select the data to be queried from
             select_limit: limit to selected the data
             select_order_by: field to use to sort the data to control how limit is performed
             select_desc: whether to order by dec or not
             skip_caching: whether to skip vector caching or not
 
         """
```

### Comparing `dioptra-1.0.6/dioptra/miners/base_miner.py` & `dioptra-1.0.7rc1/dioptra/miners/base_miner.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             'content-type': 'application/json',
             'x-api-key': self.api_key
         })
         r.raise_for_status()
 
         return r.json()
 
-    def get_results(self):
+    def get_results(self, retry_on_empty_success=True):
         sleepTimeSecs = 1
         totalSleepTimeSecs = 0
 
         while True:
             if totalSleepTimeSecs > 3600:
                 raise RuntimeError('Timed out waiting for miner results')
                 
@@ -52,15 +52,20 @@
             })
             r.raise_for_status()
             response_json = r.json()
             task = response_json['task']
             status = task['status']
 
             if status == 'SUCCESS':
-                return task['result']
+                results =  task['result']
+                # TODO: remove this.
+                if len(results) == 0 and retry_on_empty_success:
+                    time.sleep(2)
+                    return self.get_results(retry_on_empty_success=False)
+
             elif status == 'FAILURE' or status == 'REVOKED':
                 raise RuntimeError('Miner failed')
             else:
                 time.sleep(sleepTimeSecs)
                 totalSleepTimeSecs += sleepTimeSecs
                 sleepTimeSecs = min(sleepTimeSecs * 2, 60)
```

### Comparing `dioptra-1.0.6/dioptra/miners/coreset_miner.py` & `dioptra-1.0.7rc1/dioptra/miners/coreset_miner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import requests
 from .base_miner import BaseMiner
 
 class CoresetMiner(BaseMiner):
     def __init__(
             self, display_name, size, select_filters, model_name,
-            embeddings_field='EMBEDDINGS', metric='euclidean',
+            embeddings_field='embeddings', metric='euclidean',
             select_limit=None, select_order_by=None, select_desc=None,
             select_reference_filters=None, select_reference_limit=None,
             select_reference_order_by=None, select_reference_desc=None,
             skip_caching=True):
         """
         CoreSet miner
         Will perform a AL query based on CoreSet
 
         Parameters:
             display_name: name to be displayed in Dioptra
             size: number of datapoints to query
-            embeddings_field: embedding fields to run the analysis on. Could be 'embeddings' 'prediction.embeddings'
+            embeddings_field: embedding fields to run the analysis on. Could be 'embeddings'
             select_filters: dioptra style filters to select the data to be queried from
             select_limit: limit to selected the data
             select_order_by: field to use to sort the data to control how limit is performed
             select_desc: whether to order by dec or not
             select_reference_filters: dioptra style filters to select the data that is already in your training dataset
             select_reference_limit: like previous but for teh reference data
             select_reference_order_by: like previous but for teh reference data
```

### Comparing `dioptra-1.0.6/dioptra/miners/entropy_miner.py` & `dioptra-1.0.7rc1/dioptra/miners/entropy_miner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.6/dioptra/miners/knn_miner.py` & `dioptra-1.0.7rc1/dioptra/miners/knn_miner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import requests
 from .base_miner import BaseMiner
 
 class KNNMiner(BaseMiner):
     def __init__(
             self, display_name, size, select_filters, model_name,
-            embeddings_field='EMBEDDINGS', metric='euclidean',
+            embeddings_field='embeddings', metric='euclidean',
             select_limit=None, select_order_by=None, select_desc=None,
             select_reference_filters=None, select_reference_limit=None,
             select_reference_order_by=None, select_reference_desc=None,
             skip_caching=True):
         """
         KNN miner
         Will perform a AL query based on CoreSet
 
         Parameters:
             display_name: name to be displayed in Dioptra
             size: number of datapoints to query
-            embeddings_field: embedding fields to run the analysis on. Could be 'embeddings' 'prediction.embeddings'
+            embeddings_field: embedding fields to run the analysis on. Could be 'embeddings'
             metric: the metrics to be used to do KNN. Could be 'euclidian' or 'cosine'
             select_filters: dioptra style filters to select the data to be queried from
             select_limit: limit to selected the data
             select_order_by: field to use to sort the data to control how limit is performed
             select_desc: whether to order by dec or not
             select_reference_filters: dioptra style filters to select the data that is already in your training dataset
             select_reference_limit: like previous but for teh reference data
```

### Comparing `dioptra-1.0.6/dioptra/miners/random_miner.py` & `dioptra-1.0.7rc1/dioptra/miners/random_miner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.6/dioptra/miners/variance_miner.py` & `dioptra-1.0.7rc1/dioptra/miners/variance_miner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.6/dioptra.egg-info/PKG-INFO` & `dioptra-1.0.7rc1/dioptra.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dioptra
-Version: 1.0.6
+Version: 1.0.7rc1
 Summary: Client library to log data to Dioptra API
 Home-page: https://github.com/dioptra-ai/collector-py
 Author: dioptra.ai
 Author-email: info@dioptra.ai
 License: BSD
 Project-URL: dioptra.ai, https://www.dioptra.ai
 Description: <div align="center">
```

### Comparing `dioptra-1.0.6/dioptra.egg-info/SOURCES.txt` & `dioptra-1.0.7rc1/dioptra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.6/setup.py` & `dioptra-1.0.7rc1/setup.py`

 * *Files identical despite different names*

