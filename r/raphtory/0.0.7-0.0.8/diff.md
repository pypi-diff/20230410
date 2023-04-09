# Comparing `tmp/raphtory-0.0.7-cp39-none-win_amd64.whl.zip` & `tmp/raphtory-0.0.8-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 1899955 bytes, number of entries: 7
--rw-r--r--  4.6 unx     8659 b- defN 23-Apr-05 00:41 raphtory-0.0.7.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Apr-05 00:41 raphtory-0.0.7.dist-info/WHEEL
--rw-r--r--  4.6 unx     2005 b- defN 23-Apr-05 00:41 raphtory/nullmodels.py
--rw-r--r--  4.6 unx    62425 b- defN 23-Apr-05 00:41 raphtory/plot.py
--rw-r--r--  4.6 unx      335 b- defN 23-Apr-05 00:41 raphtory/__init__.py
--rwxr-xr-x  4.6 unx  4986368 b- defN 23-Apr-05 00:41 raphtory/raphtory.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      534 b- defN 23-Apr-05 00:41 raphtory-0.0.7.dist-info/RECORD
-7 files, 5060422 bytes uncompressed, 1899025 bytes compressed:  62.5%
+Zip file size: 2037667 bytes, number of entries: 7
+-rw-r--r--  4.6 unx     8659 b- defN 23-Apr-09 22:32 raphtory-0.0.8.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-Apr-09 22:32 raphtory-0.0.8.dist-info/WHEEL
+-rw-r--r--  4.6 unx     2005 b- defN 23-Apr-09 22:32 raphtory/nullmodels.py
+-rw-r--r--  4.6 unx     7447 b- defN 23-Apr-09 22:32 raphtory/vis.py
+-rw-r--r--  4.6 unx      311 b- defN 23-Apr-09 22:32 raphtory/__init__.py
+-rwxr-xr-x  4.6 unx  5526528 b- defN 23-Apr-09 22:32 raphtory/raphtory.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      532 b- defN 23-Apr-09 22:32 raphtory-0.0.8.dist-info/RECORD
+7 files, 5545578 bytes uncompressed, 2036739 bytes compressed:  63.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: raphtory-0.0.7.dist-info/METADATA
+Filename: raphtory-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: raphtory-0.0.7.dist-info/WHEEL
+Filename: raphtory-0.0.8.dist-info/WHEEL
 Comment: 
 
 Filename: raphtory/nullmodels.py
 Comment: 
 
-Filename: raphtory/plot.py
+Filename: raphtory/vis.py
 Comment: 
 
 Filename: raphtory/__init__.py
 Comment: 
 
 Filename: raphtory/raphtory.cp39-win_amd64.pyd
 Comment: 
 
-Filename: raphtory-0.0.7.dist-info/RECORD
+Filename: raphtory-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## raphtory/__init__.py

```diff
@@ -1,13 +1,12 @@
 import sys
 from .raphtory import *
 sys.modules["raphtory.algorithms"] = algorithms
 sys.modules["raphtory.graph_gen"] = graph_gen
 sys.modules["raphtory.graph_loader"] = graph_loader
 
 
-from .plot import draw
 from .nullmodels import *
 
 __doc__ = raphtory.__doc__
 if hasattr(raphtory, "__all__"):
     __all__ = raphtory.__all__
```

## Comparing `raphtory-0.0.7.dist-info/METADATA` & `raphtory-0.0.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raphtory
-Version: 0.0.7
+Version: 0.0.8
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numpy >= 1.21.2
 Requires-Dist: matplotlib >= 3.4.3
 Requires-Dist: pandas >= 1.3.3
 Requires-Dist: networkx >= 2.6.3
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: raphtory Version: 0.0.7 Classifier: Programming
+Metadata-Version: 2.1 Name: raphtory Version: 0.0.8 Classifier: Programming
 Language :: Rust Classifier: Programming Language :: Python :: Implementation
 :: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numpy >= 1.21.2 Requires-Dist: matplotlib >= 3.4.3 Requires-
 Dist: pandas >= 1.3.3 Requires-Dist: networkx >= 2.6.3 Requires-Dist: scipy >=
 1.10.1 Summary: Python package for DocBrown, a temporal graph library Keywords:
 graph,temporal-graph,temporal Home-Page: https://github.com/Raphtory/docbrown/
 Author: Pometry License: AGPL-3.0-only Requires-Python: >=3.7 Description-
```

