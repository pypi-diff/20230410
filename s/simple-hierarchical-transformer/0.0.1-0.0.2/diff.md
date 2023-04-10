# Comparing `tmp/simple-hierarchical-transformer-0.0.1.tar.gz` & `tmp/simple-hierarchical-transformer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-hierarchical-transformer-0.0.1.tar", last modified: Sun Apr  9 18:29:56 2023, max compression
+gzip compressed data, was "simple-hierarchical-transformer-0.0.2.tar", last modified: Mon Apr 10 15:14:51 2023, max compression
```

## Comparing `simple-hierarchical-transformer-0.0.1.tar` & `simple-hierarchical-transformer-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:29:56.587769 simple-hierarchical-transformer-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-09 18:29:47.000000 simple-hierarchical-transformer-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-09 18:29:56.587769 simple-hierarchical-transformer-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-09 18:29:47.000000 simple-hierarchical-transformer-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 18:29:56.587769 simple-hierarchical-transformer-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-09 18:29:47.000000 simple-hierarchical-transformer-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:29:56.587769 simple-hierarchical-transformer-0.0.1/simple_hierarchical_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-09 18:29:47.000000 simple-hierarchical-transformer-0.0.1/simple_hierarchical_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-09 18:29:47.000000 simple-hierarchical-transformer-0.0.1/simple_hierarchical_transformer/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-09 18:29:47.000000 simple-hierarchical-transformer-0.0.1/simple_hierarchical_transformer/simple_hierarchical_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:29:56.587769 simple-hierarchical-transformer-0.0.1/simple_hierarchical_transformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-09 18:29:56.000000 simple-hierarchical-transformer-0.0.1/simple_hierarchical_transformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-09 18:29:56.000000 simple-hierarchical-transformer-0.0.1/simple_hierarchical_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 18:29:56.000000 simple-hierarchical-transformer-0.0.1/simple_hierarchical_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-09 18:29:56.000000 simple-hierarchical-transformer-0.0.1/simple_hierarchical_transformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-09 18:29:56.000000 simple-hierarchical-transformer-0.0.1/simple_hierarchical_transformer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:14:51.249723 simple-hierarchical-transformer-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-10 15:14:42.000000 simple-hierarchical-transformer-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-10 15:14:51.249723 simple-hierarchical-transformer-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-10 15:14:42.000000 simple-hierarchical-transformer-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 15:14:51.249723 simple-hierarchical-transformer-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-10 15:14:42.000000 simple-hierarchical-transformer-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:14:51.245723 simple-hierarchical-transformer-0.0.2/simple_hierarchical_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-10 15:14:42.000000 simple-hierarchical-transformer-0.0.2/simple_hierarchical_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-10 15:14:42.000000 simple-hierarchical-transformer-0.0.2/simple_hierarchical_transformer/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-10 15:14:42.000000 simple-hierarchical-transformer-0.0.2/simple_hierarchical_transformer/simple_hierarchical_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:14:51.249723 simple-hierarchical-transformer-0.0.2/simple_hierarchical_transformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-10 15:14:51.000000 simple-hierarchical-transformer-0.0.2/simple_hierarchical_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-10 15:14:51.000000 simple-hierarchical-transformer-0.0.2/simple_hierarchical_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:14:51.000000 simple-hierarchical-transformer-0.0.2/simple_hierarchical_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-10 15:14:51.000000 simple-hierarchical-transformer-0.0.2/simple_hierarchical_transformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-10 15:14:51.000000 simple-hierarchical-transformer-0.0.2/simple_hierarchical_transformer.egg-info/top_level.txt
```

### Comparing `simple-hierarchical-transformer-0.0.1/LICENSE` & `simple-hierarchical-transformer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-hierarchical-transformer-0.0.1/PKG-INFO` & `simple-hierarchical-transformer-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-hierarchical-transformer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple Hierarchical Transformer
 Home-page: https://github.com/lucidrains/simple-hierarchical-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,hierarchical
 Classifier: Development Status :: 4 - Beta
```

### Comparing `simple-hierarchical-transformer-0.0.1/README.md` & `simple-hierarchical-transformer-0.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -40,7 +40,26 @@
     title   = {ProphetNet: Predicting Future N-gram for Sequence-to-Sequence Pre-training},
     author  = {Yu Yan and Weizhen Qi and Yeyun Gong and Dayiheng Liu and Nan Duan and Jiusheng Chen and Ruofei Zhang and Ming Zhou},
     journal = {ArXiv},
     year    = {2020},
     volume  = {abs/2001.04063}
 }
 ```
+
+```bibtex
+@misc{su2021roformer,
+    title   = {RoFormer: Enhanced Transformer with Rotary Position Embedding},
+    author  = {Jianlin Su and Yu Lu and Shengfeng Pan and Bo Wen and Yunfeng Liu},
+    year    = {2021},
+    eprint  = {2104.09864},
+    archivePrefix = {arXiv},
+    primaryClass = {cs.CL}
+}
+```
+
+```bibtex
+@inproceedings{Sun2022ALT,
+    title     = {A Length-Extrapolatable Transformer},
+    author    = {Yutao Sun and Li Dong and Barun Patra and Shuming Ma and Shaohan Huang and Alon Benhaim and Vishrav Chaudhary and Xia Song and Furu Wei},
+    year      = {2022}
+}
+```
```

#### html2text {}

```diff
@@ -17,7 +17,14 @@
 Exact Attention with {IO}-Awareness}, author = {Dao, Tri and Fu, Daniel Y. and
 Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher}, booktitle = {Advances
 in Neural Information Processing Systems}, year = {2022} } ``` ```bibtex
 @article{Yan2020ProphetNetPF, title = {ProphetNet: Predicting Future N-gram for
 Sequence-to-Sequence Pre-training}, author = {Yu Yan and Weizhen Qi and Yeyun
 Gong and Dayiheng Liu and Nan Duan and Jiusheng Chen and Ruofei Zhang and Ming
 Zhou}, journal = {ArXiv}, year = {2020}, volume = {abs/2001.04063} } ```
+```bibtex @misc{su2021roformer, title = {RoFormer: Enhanced Transformer with
+Rotary Position Embedding}, author = {Jianlin Su and Yu Lu and Shengfeng Pan
+and Bo Wen and Yunfeng Liu}, year = {2021}, eprint = {2104.09864},
+archivePrefix = {arXiv}, primaryClass = {cs.CL} } ``` ```bibtex @inproceedings
+{Sun2022ALT, title = {A Length-Extrapolatable Transformer}, author = {Yutao Sun
+and Li Dong and Barun Patra and Shuming Ma and Shaohan Huang and Alon Benhaim
+and Vishrav Chaudhary and Xia Song and Furu Wei}, year = {2022} } ```
```

### Comparing `simple-hierarchical-transformer-0.0.1/setup.py` & `simple-hierarchical-transformer-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'simple-hierarchical-transformer',
   packages = find_packages(exclude=[]),
-  version = '0.0.1',
+  version = '0.0.2',
   license='MIT',
   description = 'Simple Hierarchical Transformer',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/simple-hierarchical-transformer',
   keywords = [
@@ -16,15 +16,14 @@
     'transformers',
     'attention mechanism',
     'hierarchical'
   ],
   install_requires=[
     'accelerate',
     'einops>=0.4',
-    'local-attention',
     'torch>=1.6',
     'vector-quantize-pytorch'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
```

### Comparing `simple-hierarchical-transformer-0.0.1/simple_hierarchical_transformer/attention.py` & `simple-hierarchical-transformer-0.0.2/simple_hierarchical_transformer/attention.py`

 * *Files identical despite different names*

### Comparing `simple-hierarchical-transformer-0.0.1/simple_hierarchical_transformer.egg-info/PKG-INFO` & `simple-hierarchical-transformer-0.0.2/simple_hierarchical_transformer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-hierarchical-transformer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple Hierarchical Transformer
 Home-page: https://github.com/lucidrains/simple-hierarchical-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,hierarchical
 Classifier: Development Status :: 4 - Beta
```

