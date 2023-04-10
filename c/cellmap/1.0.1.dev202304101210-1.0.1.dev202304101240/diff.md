# Comparing `tmp/cellmap-1.0.1.dev202304101210-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304101240-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 8542 bytes, number of entries: 5
+Zip file size: 8550 bytes, number of entries: 5
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    40790 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1587 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304101210.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304101210.dist-info/WHEEL
-?rw-r--r--  2.0 unx      404 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304101210.dist-info/RECORD
-5 files, 42921 bytes uncompressed, 7788 bytes compressed:  81.9%
+-rw-r--r--  2.0 unx    40811 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1587 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304101240.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304101240.dist-info/WHEEL
+?rw-r--r--  2.0 unx      404 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304101240.dist-info/RECORD
+5 files, 42942 bytes uncompressed, 7796 bytes compressed:  81.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304101210.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304101240.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304101210.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304101240.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304101210.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304101240.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -6,14 +6,15 @@
 import scipy
 import sklearn.preprocessing
 import sklearn.neighbors
 import matplotlib.colors
 import pandas as pd
 import logging
 import scanpy
+import scvelo as scv
 
 
 def create_graph(
     X,
     Y,
     cutedge_vol = None,
     cutedge_length = None,
```

## Comparing `cellmap-1.0.1.dev202304101210.dist-info/METADATA` & `cellmap-1.0.1.dev202304101240.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304101210
+Version: 1.0.1.dev202304101240
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

