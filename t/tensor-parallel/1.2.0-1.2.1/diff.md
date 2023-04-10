# Comparing `tmp/tensor_parallel-1.2.0.tar.gz` & `tmp/tensor_parallel-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensor_parallel-1.2.0.tar", last modified: Mon Apr  3 12:31:33 2023, max compression
+gzip compressed data, was "tensor_parallel-1.2.1.tar", last modified: Mon Apr 10 16:52:57 2023, max compression
```

## Comparing `tensor_parallel-1.2.0.tar` & `tensor_parallel-1.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:31:33.743795 tensor_parallel-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-03 12:31:19.000000 tensor_parallel-1.2.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-04-03 12:31:33.743795 tensor_parallel-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-04-03 12:31:19.000000 tensor_parallel-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-03 12:31:19.000000 tensor_parallel-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-03 12:31:33.743795 tensor_parallel-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:31:33.735795 tensor_parallel-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:31:33.739795 tensor_parallel-1.2.0/src/tensor_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-03 12:31:19.000000 tensor_parallel-1.2.0/src/tensor_parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-04-03 12:31:19.000000 tensor_parallel-1.2.0/src/tensor_parallel/autoconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-03 12:31:19.000000 tensor_parallel-1.2.0/src/tensor_parallel/aux_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-03 12:31:19.000000 tensor_parallel-1.2.0/src/tensor_parallel/communications.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-03 12:31:19.000000 tensor_parallel-1.2.0/src/tensor_parallel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-04-03 12:31:19.000000 tensor_parallel-1.2.0/src/tensor_parallel/cross_device_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-03 12:31:19.000000 tensor_parallel-1.2.0/src/tensor_parallel/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-04-03 12:31:19.000000 tensor_parallel-1.2.0/src/tensor_parallel/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-03 12:31:19.000000 tensor_parallel-1.2.0/src/tensor_parallel/per_device_tensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-04-03 12:31:19.000000 tensor_parallel-1.2.0/src/tensor_parallel/pretrained_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-04-03 12:31:19.000000 tensor_parallel-1.2.0/src/tensor_parallel/shard.py
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-04-03 12:31:19.000000 tensor_parallel-1.2.0/src/tensor_parallel/sharding.py
--rw-r--r--   0 runner    (1001) docker     (123)    16965 2023-04-03 12:31:19.000000 tensor_parallel-1.2.0/src/tensor_parallel/slicing_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-04-03 12:31:19.000000 tensor_parallel-1.2.0/src/tensor_parallel/state_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-04-03 12:31:19.000000 tensor_parallel-1.2.0/src/tensor_parallel/tensor_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-03 12:31:19.000000 tensor_parallel-1.2.0/src/tensor_parallel/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-03 12:31:19.000000 tensor_parallel-1.2.0/src/tensor_parallel/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:31:33.739795 tensor_parallel-1.2.0/src/tensor_parallel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-04-03 12:31:33.000000 tensor_parallel-1.2.0/src/tensor_parallel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-03 12:31:33.000000 tensor_parallel-1.2.0/src/tensor_parallel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 12:31:33.000000 tensor_parallel-1.2.0/src/tensor_parallel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-03 12:31:33.000000 tensor_parallel-1.2.0/src/tensor_parallel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-03 12:31:33.000000 tensor_parallel-1.2.0/src/tensor_parallel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:31:33.743795 tensor_parallel-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-04-03 12:31:19.000000 tensor_parallel-1.2.0/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-03 12:31:19.000000 tensor_parallel-1.2.0/tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-03 12:31:19.000000 tensor_parallel-1.2.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-03 12:31:19.000000 tensor_parallel-1.2.0/tests/test_saving.py
--rw-r--r--   0 runner    (1001) docker     (123)     9034 2023-04-03 12:31:19.000000 tensor_parallel-1.2.0/tests/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:57.526558 tensor_parallel-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-04-10 16:52:57.526558 tensor_parallel-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-10 16:52:57.526558 tensor_parallel-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:57.518557 tensor_parallel-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:57.522557 tensor_parallel-1.2.1/src/tensor_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/autoconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/aux_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/communications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/cross_device_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/per_device_tensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/pretrained_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/shard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/sharding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19224 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/slicing_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/state_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/tensor_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:57.522557 tensor_parallel-1.2.1/src/tensor_parallel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-04-10 16:52:57.000000 tensor_parallel-1.2.1/src/tensor_parallel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-10 16:52:57.000000 tensor_parallel-1.2.1/src/tensor_parallel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:52:57.000000 tensor_parallel-1.2.1/src/tensor_parallel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-10 16:52:57.000000 tensor_parallel-1.2.1/src/tensor_parallel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-10 16:52:57.000000 tensor_parallel-1.2.1/src/tensor_parallel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:57.526558 tensor_parallel-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/tests/test_saving.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/tests/test_transformers.py
```

### Comparing `tensor_parallel-1.2.0/LICENCE` & `tensor_parallel-1.2.1/LICENCE`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.0/PKG-INFO` & `tensor_parallel-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensor_parallel
-Version: 1.2.0
+Version: 1.2.1
 Summary: Automatically shard your large model between multiple GPUs, works without torch.distributed
 Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak
 Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -31,15 +31,15 @@
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![CI status](https://github.com/BlackSamorez/tensor_parallel/actions/workflows/run-tests.yaml/badge.svg?branch=main)](https://github.com/BlackSamorez/tensor_parallel/actions)
 
 <p align="center">
     🚀 &nbsp;<b><a href="https://www.kaggle.com/code/blacksamorez/tensor-parallel-int8-llm/">Try new 20B LLMs demo in Kaggle</a></b>
 </p>
 
-Run large PyTorch models on multiple GPUs in one line of code.
+Run large PyTorch models on multiple GPUs in one line of code with potentially linear speedup.
 
 ```python
 import transformers
 import tensor_parallel as tp
 tokenizer = transformers.AutoTokenizer.from_pretrained("facebook/opt-13b")
 model = transformers.AutoModelForCausalLM.from_pretrained("facebook/opt-13b")  # use opt-125m for testing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tensor_parallel Version: 1.2.0 Summary:
+Metadata-Version: 2.1 Name: tensor_parallel Version: 1.2.1 Summary:
 Automatically shard your large model between multiple GPUs, works without
 torch.distributed Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/
 issues Classifier: Development Status :: 4 - Beta Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
@@ -18,20 +18,20 @@
 [PyPI version](https://img.shields.io/pypi/v/tensor-parallel.svg?color=blue)]
 (https://pypi.org/project/tensor-parallel/) [![Black](https://img.shields.io/
 badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![CI
 status](https://github.com/BlackSamorez/tensor_parallel/actions/workflows/run-
 tests.yaml/badge.svg?branch=main)](https://github.com/BlackSamorez/
 tensor_parallel/actions)
                      ð  Try_new_20B_LLMs_demo_in_Kaggle
-Run large PyTorch models on multiple GPUs in one line of code. ```python import
-transformers import tensor_parallel as tp tokenizer =
-transformers.AutoTokenizer.from_pretrained("facebook/opt-13b") model =
-transformers.AutoModelForCausalLM.from_pretrained("facebook/opt-13b") # use
-opt-125m for testing model = tp.tensor_parallel(model, ["cuda:0", "cuda:1"]) #
-<- each GPU has half the weights inputs = tokenizer("A cat sat",
+Run large PyTorch models on multiple GPUs in one line of code with potentially
+linear speedup. ```python import transformers import tensor_parallel as tp
+tokenizer = transformers.AutoTokenizer.from_pretrained("facebook/opt-13b")
+model = transformers.AutoModelForCausalLM.from_pretrained("facebook/opt-13b") #
+use opt-125m for testing model = tp.tensor_parallel(model, ["cuda:0", "cuda:
+1"]) # <- each GPU has half the weights inputs = tokenizer("A cat sat",
 return_tensors="pt")["input_ids"].to("cuda:0") outputs = model.generate(inputs,
 num_beams=5) print(tokenizer.decode(outputs[0])) # A cat sat on my lap for a
 few minutes ... model(input_ids=inputs, labels=inputs).loss.backward() #
 training works as usual ``` ## Installation Latest stable version
 (recommended): ``` pip install tensor_parallel ``` Bleeding edge version: ```
 pip install https://github.com/BlackSamorez/tensor_parallel/archive/main.zip
 ``` ## Usage Simply wrap your PyTorch model with `tp.tensor_parallel` and use
```

### Comparing `tensor_parallel-1.2.0/README.md` & `tensor_parallel-1.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![CI status](https://github.com/BlackSamorez/tensor_parallel/actions/workflows/run-tests.yaml/badge.svg?branch=main)](https://github.com/BlackSamorez/tensor_parallel/actions)
 
 <p align="center">
     🚀 &nbsp;<b><a href="https://www.kaggle.com/code/blacksamorez/tensor-parallel-int8-llm/">Try new 20B LLMs demo in Kaggle</a></b>
 </p>
 
-Run large PyTorch models on multiple GPUs in one line of code.
+Run large PyTorch models on multiple GPUs in one line of code with potentially linear speedup.
 
 ```python
 import transformers
 import tensor_parallel as tp
 tokenizer = transformers.AutoTokenizer.from_pretrained("facebook/opt-13b")
 model = transformers.AutoModelForCausalLM.from_pretrained("facebook/opt-13b")  # use opt-125m for testing
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
 # tensor_parallel [![PyPI version](https://img.shields.io/pypi/v/tensor-
 parallel.svg?color=blue)](https://pypi.org/project/tensor-parallel/) [![Black]
 (https://img.shields.io/badge/code%20style-black-000000.svg)](https://
 github.com/psf/black) [![CI status](https://github.com/BlackSamorez/
 tensor_parallel/actions/workflows/run-tests.yaml/badge.svg?branch=main)](https:
 //github.com/BlackSamorez/tensor_parallel/actions)
                      ð  Try_new_20B_LLMs_demo_in_Kaggle
-Run large PyTorch models on multiple GPUs in one line of code. ```python import
-transformers import tensor_parallel as tp tokenizer =
-transformers.AutoTokenizer.from_pretrained("facebook/opt-13b") model =
-transformers.AutoModelForCausalLM.from_pretrained("facebook/opt-13b") # use
-opt-125m for testing model = tp.tensor_parallel(model, ["cuda:0", "cuda:1"]) #
-<- each GPU has half the weights inputs = tokenizer("A cat sat",
+Run large PyTorch models on multiple GPUs in one line of code with potentially
+linear speedup. ```python import transformers import tensor_parallel as tp
+tokenizer = transformers.AutoTokenizer.from_pretrained("facebook/opt-13b")
+model = transformers.AutoModelForCausalLM.from_pretrained("facebook/opt-13b") #
+use opt-125m for testing model = tp.tensor_parallel(model, ["cuda:0", "cuda:
+1"]) # <- each GPU has half the weights inputs = tokenizer("A cat sat",
 return_tensors="pt")["input_ids"].to("cuda:0") outputs = model.generate(inputs,
 num_beams=5) print(tokenizer.decode(outputs[0])) # A cat sat on my lap for a
 few minutes ... model(input_ids=inputs, labels=inputs).loss.backward() #
 training works as usual ``` ## Installation Latest stable version
 (recommended): ``` pip install tensor_parallel ``` Bleeding edge version: ```
 pip install https://github.com/BlackSamorez/tensor_parallel/archive/main.zip
 ``` ## Usage Simply wrap your PyTorch model with `tp.tensor_parallel` and use
```

### Comparing `tensor_parallel-1.2.0/setup.cfg` & `tensor_parallel-1.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tensor_parallel
-version = 1.2.0
+version = 1.2.1
 author = Andrei Panferov and Yaroslav Lisnyak
 author_email = yalisnyak@nes.com
 description = Automatically shard your large model between multiple GPUs, works without torch.distributed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BlackSamorez/tensor_parallel
 project_urls =
```

### Comparing `tensor_parallel-1.2.0/src/tensor_parallel/__init__.py` & `tensor_parallel-1.2.1/src/tensor_parallel/__init__.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.0/src/tensor_parallel/autoconfig.py` & `tensor_parallel-1.2.1/src/tensor_parallel/autoconfig.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.0/src/tensor_parallel/aux_actions.py` & `tensor_parallel-1.2.1/src/tensor_parallel/aux_actions.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.0/src/tensor_parallel/communications.py` & `tensor_parallel-1.2.1/src/tensor_parallel/communications.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.0/src/tensor_parallel/config.py` & `tensor_parallel-1.2.1/src/tensor_parallel/config.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.0/src/tensor_parallel/cross_device_ops.py` & `tensor_parallel-1.2.1/src/tensor_parallel/cross_device_ops.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.0/src/tensor_parallel/dispatch.py` & `tensor_parallel-1.2.1/src/tensor_parallel/dispatch.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.0/src/tensor_parallel/factory.py` & `tensor_parallel-1.2.1/src/tensor_parallel/factory.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.0/src/tensor_parallel/per_device_tensors.py` & `tensor_parallel-1.2.1/src/tensor_parallel/per_device_tensors.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.0/src/tensor_parallel/pretrained_model.py` & `tensor_parallel-1.2.1/src/tensor_parallel/pretrained_model.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.0/src/tensor_parallel/shard.py` & `tensor_parallel-1.2.1/src/tensor_parallel/shard.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.0/src/tensor_parallel/sharding.py` & `tensor_parallel-1.2.1/src/tensor_parallel/sharding.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.0/src/tensor_parallel/slicing_configs.py` & `tensor_parallel-1.2.1/src/tensor_parallel/slicing_configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,15 +350,61 @@
                 "embed_dim": partial(split_inner_dim, num_heads=num_heads // 4, world_size=world_size),
                 "num_attention_heads": partial(split_codegen_num_heads, world_size=world_size),
             }
         },
     )
 
 
+def get_llama_config(model_config: PretrainedConfig, devices: Sequence[torch.device]) -> Config:
+    # We can't use LlamaConfig since it requires pre-release `transformers``
+    assert model_config.model_type == "llama", f"Trying to pass {model_config.model_type} as llama config"
+
+    world_size = len(devices)
+    num_heads = model_config.num_attention_heads
+    head_dim = model_config.hidden_size // model_config.num_attention_heads
+
+    gather_kv_across_ranks = CollectiveOperation(
+        world_size=world_size, func=lambda *kvs: gather_kv(*kvs, world_size=world_size)
+    )  # this operation ensures that we get attention cache for all heads on each device
+
+    return Config(
+        state_rules={
+            # LlamaAttention
+            r".*self_attn\.q_proj\.weight$": SplitInChunks(world_size=world_size, dim=0, chunk_size=head_dim),
+            r".*self_attn\.k_proj\.weight$": SplitInChunks(world_size=world_size, dim=0, chunk_size=head_dim),
+            r".*self_attn\.v_proj\.weight$": SplitInChunks(world_size=world_size, dim=0, chunk_size=head_dim),
+            r".*self_attn\.o_proj\.weight$": SplitInChunks(world_size=world_size, dim=1, chunk_size=head_dim),
+            # LlamaFeedForward
+            r".*mlp\.gate_proj\.weight$": Split(world_size=world_size, dim=0),
+            r".*mlp\.down_proj\.weight$": Split(world_size=world_size, dim=1),
+            r".*mlp\.up_proj\.weight$": Split(world_size=world_size, dim=0),
+            # LlamaModel
+            r".*embed_tokens.weight$": Split(world_size=world_size, dim=1),
+            r".*lm_head\.weight$": Split(world_size=world_size, dim=0),
+        },
+        input_rules={
+            r".*self_attn$": {"past_key_value": select_kv_for_rank},
+        },
+        output_rules={
+            r".*self_attn$": {0: "sum", 2: gather_kv_across_ranks},
+            r".*mlp$": {0: "sum"},
+            r".*embed_tokens$": {0: "gather -1"},
+            r".*lm_head$": {0: "gather -1"},
+        },
+        attr_rules={
+            r".*self_attn$": {
+                "hidden_size": partial(split_inner_dim, num_heads=num_heads, world_size=world_size),
+                "num_heads": partial(split_num_heads, world_size=world_size),
+            }
+        },
+    )
+
+
 PREDEFINED_CONFIGS: Dict[str, ConfigGetter] = {
     "bloom": get_bloom_config,
     "t5": get_t5_config,
     "bert": get_bert_config,
     "gpt2": get_gpt2_config,
     "gpt_neox": get_gpt_neox_config,
     "codegen": get_codegen_config,
+    "llama": get_llama_config,
 }
```

### Comparing `tensor_parallel-1.2.0/src/tensor_parallel/state_actions.py` & `tensor_parallel-1.2.1/src/tensor_parallel/state_actions.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.0/src/tensor_parallel/tensor_parallel.py` & `tensor_parallel-1.2.1/src/tensor_parallel/tensor_parallel.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.0/src/tensor_parallel/utils.py` & `tensor_parallel-1.2.1/src/tensor_parallel/utils.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.0/src/tensor_parallel/wrapper.py` & `tensor_parallel-1.2.1/src/tensor_parallel/wrapper.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.0/src/tensor_parallel.egg-info/PKG-INFO` & `tensor_parallel-1.2.1/src/tensor_parallel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensor-parallel
-Version: 1.2.0
+Version: 1.2.1
 Summary: Automatically shard your large model between multiple GPUs, works without torch.distributed
 Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak
 Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -31,15 +31,15 @@
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![CI status](https://github.com/BlackSamorez/tensor_parallel/actions/workflows/run-tests.yaml/badge.svg?branch=main)](https://github.com/BlackSamorez/tensor_parallel/actions)
 
 <p align="center">
     🚀 &nbsp;<b><a href="https://www.kaggle.com/code/blacksamorez/tensor-parallel-int8-llm/">Try new 20B LLMs demo in Kaggle</a></b>
 </p>
 
-Run large PyTorch models on multiple GPUs in one line of code.
+Run large PyTorch models on multiple GPUs in one line of code with potentially linear speedup.
 
 ```python
 import transformers
 import tensor_parallel as tp
 tokenizer = transformers.AutoTokenizer.from_pretrained("facebook/opt-13b")
 model = transformers.AutoModelForCausalLM.from_pretrained("facebook/opt-13b")  # use opt-125m for testing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tensor-parallel Version: 1.2.0 Summary:
+Metadata-Version: 2.1 Name: tensor-parallel Version: 1.2.1 Summary:
 Automatically shard your large model between multiple GPUs, works without
 torch.distributed Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/
 issues Classifier: Development Status :: 4 - Beta Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
@@ -18,20 +18,20 @@
 [PyPI version](https://img.shields.io/pypi/v/tensor-parallel.svg?color=blue)]
 (https://pypi.org/project/tensor-parallel/) [![Black](https://img.shields.io/
 badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![CI
 status](https://github.com/BlackSamorez/tensor_parallel/actions/workflows/run-
 tests.yaml/badge.svg?branch=main)](https://github.com/BlackSamorez/
 tensor_parallel/actions)
                      ð  Try_new_20B_LLMs_demo_in_Kaggle
-Run large PyTorch models on multiple GPUs in one line of code. ```python import
-transformers import tensor_parallel as tp tokenizer =
-transformers.AutoTokenizer.from_pretrained("facebook/opt-13b") model =
-transformers.AutoModelForCausalLM.from_pretrained("facebook/opt-13b") # use
-opt-125m for testing model = tp.tensor_parallel(model, ["cuda:0", "cuda:1"]) #
-<- each GPU has half the weights inputs = tokenizer("A cat sat",
+Run large PyTorch models on multiple GPUs in one line of code with potentially
+linear speedup. ```python import transformers import tensor_parallel as tp
+tokenizer = transformers.AutoTokenizer.from_pretrained("facebook/opt-13b")
+model = transformers.AutoModelForCausalLM.from_pretrained("facebook/opt-13b") #
+use opt-125m for testing model = tp.tensor_parallel(model, ["cuda:0", "cuda:
+1"]) # <- each GPU has half the weights inputs = tokenizer("A cat sat",
 return_tensors="pt")["input_ids"].to("cuda:0") outputs = model.generate(inputs,
 num_beams=5) print(tokenizer.decode(outputs[0])) # A cat sat on my lap for a
 few minutes ... model(input_ids=inputs, labels=inputs).loss.backward() #
 training works as usual ``` ## Installation Latest stable version
 (recommended): ``` pip install tensor_parallel ``` Bleeding edge version: ```
 pip install https://github.com/BlackSamorez/tensor_parallel/archive/main.zip
 ``` ## Usage Simply wrap your PyTorch model with `tp.tensor_parallel` and use
```

### Comparing `tensor_parallel-1.2.0/src/tensor_parallel.egg-info/SOURCES.txt` & `tensor_parallel-1.2.1/src/tensor_parallel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.0/tests/test_basic.py` & `tensor_parallel-1.2.1/tests/test_basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,16 @@
         if isinstance(module, nn.Linear):
             assert module.weight.shape == (module.out_features, module.in_features), f"For module {name}"
 
 
 @pytest.mark.parametrize("emb_cls", [nn.Embedding, nn.EmbeddingBag])
 @pytest.mark.parametrize("devices", [None, ("cpu",), ("cpu", "cpu"), ("cpu", "cpu", "cpu")])
 def test_embeds_and_linear(emb_cls, devices):
+    torch.manual_seed(0)
+
     model = nn.Sequential(
         emb_cls(num_embeddings=1337, embedding_dim=64),
         nn.LayerNorm(64),
         nn.Linear(64, 128),
         nn.ReLU(),
         nn.Linear(128, 10),
     )
@@ -51,14 +53,16 @@
     our_grad = torch.cat([next(shard[0].parameters()).grad for shard in model_tp.module_shards], dim=1)
     torch.testing.assert_close(model[0].weight.grad, our_grad, atol=1e-6, rtol=1e-05)
 
 
 @pytest.mark.parametrize("devices", [None, ("cpu",), ("cpu",) * 2, ("cpu",) * 3, ("cpu",) * 4])
 @pytest.mark.parametrize("extra_options", [{}, {"padding": "same"}, {"stride": 2}, {"dilation": 2}, {"groups": 2}])
 def test_convs(devices, extra_options):
+    torch.manual_seed(0)
+
     batchnorm_cls = (None, nn.BatchNorm1d, nn.BatchNorm2d, nn.BatchNorm3d)
     # ^-- note: batchnorms test that tensor_parallel handles buffers (non-parameter state tensors) correctly
     for Conv, nd in (
         (nn.Conv1d, 1),
         (nn.Conv2d, 2),
         (nn.Conv3d, 3),
         (nn.ConvTranspose1d, 1),
@@ -97,14 +101,16 @@
             msg=lambda msg: f"{msg}\n where Conv is {Conv} with extra_options {extra_options}",
         )
 
 
 @pytest.mark.parametrize("emb_cls", [nn.Embedding, nn.EmbeddingBag])
 @pytest.mark.parametrize("devices", [None, ("cpu",), ("cpu", "cpu"), ("cpu", "cpu", "cpu")])
 def test_sharding(emb_cls, devices):
+    torch.manual_seed(0)
+
     model = nn.Sequential(
         emb_cls(num_embeddings=1337, embedding_dim=64),
         nn.LayerNorm(64),
         nn.Linear(64, 128),
         nn.ReLU(),
         nn.Linear(128, 10),
     )
```

### Comparing `tensor_parallel-1.2.0/tests/test_factory.py` & `tensor_parallel-1.2.1/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.0/tests/test_integration.py` & `tensor_parallel-1.2.1/tests/test_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from tensor_parallel import Config, TensorParallel
 from tensor_parallel.state_actions import Scale, Split
 
 
 @pytest.mark.parametrize("custom_config", [True, False])
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3, ("cpu",) * 4])
 def test_tp_bloom_block(devices, custom_config):
+    torch.manual_seed(0)
+
     bloom_config = BloomConfig.from_pretrained("bigscience/bloom-560m")
     bloom_config.torch_dtype = torch.float32
     block = BloomBlock(bloom_config)
 
     tp_config = None
     if custom_config:
         tp_config = Config(
```

### Comparing `tensor_parallel-1.2.0/tests/test_saving.py` & `tensor_parallel-1.2.1/tests/test_saving.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.0/tests/test_transformers.py` & `tensor_parallel-1.2.1/tests/test_transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,18 +46,24 @@
 @pytest.mark.parametrize(
     "model_name",
     [
         "bigscience/bloom-560m",
         "gpt2",
         "trl-internal-testing/tiny-random-GPTNeoXForCausalLM",
         "Salesforce/codegen-350M-mono",
+        "decapoda-research/llama-7b-hf",
     ],
 )
 def test_forward_gpt2_like(use_config, devices, model_name):
-    model = AutoModelForCausalLM.from_pretrained(model_name, low_cpu_mem_usage=True).float().to(devices[0])
+    torch.manual_seed(0)
+
+    try:
+        model = AutoModelForCausalLM.from_pretrained(model_name, low_cpu_mem_usage=True).float().to(devices[0])
+    except KeyError as err:
+        pytest.skip(f"Could not create model {model_name} with error {err}")
 
     inp1 = torch.randint(1, 1000, size=(2, 3), device=devices[0])
     inp2 = torch.randint(1, 1000, size=(2, 1), device=devices[0])
     inp3 = torch.randint(1, 1000, size=(2, 2), device=devices[0])
 
     out1_ref = model(inp1, use_cache=True, output_hidden_states=True)
     out2_ref = model(inp2, use_cache=True, past_key_values=out1_ref.past_key_values)
@@ -79,14 +85,16 @@
     torch.testing.assert_close(out3_ref.logits, out3.logits, atol=3e-3, rtol=1e-05)
 
 
 @pytest.mark.parametrize("use_config", [False, True])
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
 @pytest.mark.parametrize("model_name", ["t5-small"])
 def test_forward_t5_like(use_config, devices, model_name):
+    torch.manual_seed(0)
+
     model = T5ForConditionalGeneration.from_pretrained(model_name, low_cpu_mem_usage=True).float().to(devices[0])
 
     enc = torch.randint(1, 1000, size=(2, 3), device=devices[0])
     dec1 = torch.randint(1, 1000, size=(2, 3), device=devices[0])
     dec2 = torch.randint(1, 1000, size=(2, 1), device=devices[0])
     dec3 = torch.randint(1, 1000, size=(2, 2), device=devices[0])
 
@@ -112,14 +120,16 @@
     torch.testing.assert_close(out3_ref.logits, out3.logits, atol=3e-3, rtol=1e-05)
 
 
 @pytest.mark.parametrize("use_config", [False, True])
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
 @pytest.mark.parametrize("model_name", ["bert-base-uncased"])
 def test_forward_bert_like(use_config, devices, model_name):
+    torch.manual_seed(0)
+
     model = BertModel.from_pretrained(model_name).to(devices[0])
 
     inp1 = torch.randint(1, 1000, size=(2, 3), device=devices[0])
     inp2 = torch.randint(1, 1000, size=(2, 1), device=devices[0])
     inp3 = torch.randint(1, 1000, size=(2, 2), device=devices[0])
 
     out1_ref = model(inp1, output_hidden_states=True)
@@ -139,18 +149,27 @@
     torch.testing.assert_close(out1_ref.hidden_states[-1], out1.hidden_states[-1], atol=3e-3, rtol=1e-05)
     torch.testing.assert_close(out2_ref.hidden_states[-1], out2.hidden_states[-1], atol=3e-3, rtol=1e-05)
     torch.testing.assert_close(out3_ref.hidden_states[-1], out3.hidden_states[-1], atol=3e-3, rtol=1e-05)
 
 
 @pytest.mark.parametrize("generate_kwargs", [{"num_beams": 3}, {}, {"top_p": 0.5}])
 @pytest.mark.parametrize(
-    "model_name", ["t5-small", "bigscience/bloom-560m", "gpt2", "trl-internal-testing/tiny-random-GPTNeoXForCausalLM"]
+    "model_name",
+    [
+        "t5-small",
+        "bigscience/bloom-560m",
+        "gpt2",
+        "trl-internal-testing/tiny-random-GPTNeoXForCausalLM",
+        "decapoda-research/llama-7b-hf",
+    ],
 )
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
 def test_generate(generate_kwargs, model_name, devices):
+    torch.manual_seed(0)
+
     def _generate_scores(model, input_ids, generate_kwargs):
         scores_tuple = model.generate(
             input_ids,
             min_length=10,
             return_dict_in_generate=True,
             output_scores=True,
             **generate_kwargs,
@@ -165,20 +184,28 @@
                 first_scores[i],
                 second_scores[i],
                 atol=3e-3,
                 rtol=1e-05,
                 msg=lambda msg: f"Diverged at {'%d%s' % (i + 1,'tsnrhtdd'[((i + 1)//10%10!=1)*((i + 1)%10<4)*(i + 1)%10::4])} token: {msg}",
             )
 
-    if model_name == "t5-small":
-        model = T5ForConditionalGeneration.from_pretrained(model_name, low_cpu_mem_usage=True).float().to(devices[0])
-    else:
-        model = (
-            transformers.AutoModelForCausalLM.from_pretrained(model_name, low_cpu_mem_usage=True).float().to(devices[0])
-        )
+    try:
+        if model_name == "t5-small":
+            model = (
+                T5ForConditionalGeneration.from_pretrained(model_name, low_cpu_mem_usage=True).float().to(devices[0])
+            )
+        else:
+            model = (
+                transformers.AutoModelForCausalLM.from_pretrained(model_name, low_cpu_mem_usage=True)
+                .float()
+                .to(devices[0])
+            )
+    except KeyError as err:
+        pytest.skip(f"Could not create model {model_name} with error {err}")
+
     input_ids = torch.randint(1, 1000, size=(2, 10), device=devices[0])
 
     scores_ref = _generate_scores(model, input_ids, generate_kwargs)
 
     model_tp = tensor_parallel(model, devices)
     del model
 
@@ -187,14 +214,16 @@
     _assert_scores_allclose_long_enough(scores_ref, scores)
 
 
 @pytest.mark.parametrize("use_predefined_config", [False, True])
 @pytest.mark.parametrize("model_name", ["t5-small"])
 @pytest.mark.parametrize("sharded", [False, True])
 def test_encoder(use_predefined_config, model_name, sharded):
+    torch.manual_seed(0)
+
     devices = ["cpu"] * 2
     model = T5ForConditionalGeneration.from_pretrained(model_name, low_cpu_mem_usage=True).float().to(devices[0])
 
     input = torch.randint(1, 1000, size=(2, 3), device=devices[0])
     out_ref = model.get_encoder()(input)
 
     if not use_predefined_config:
```

