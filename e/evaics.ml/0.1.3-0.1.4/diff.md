# Comparing `tmp/evaics.ml-0.1.3.tar.gz` & `tmp/evaics.ml-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evaics.ml-0.1.3.tar", last modified: Sat Apr  8 21:46:35 2023, max compression
+gzip compressed data, was "evaics.ml-0.1.4.tar", last modified: Mon Apr 10 20:34:37 2023, max compression
```

## Comparing `evaics.ml-0.1.3.tar` & `evaics.ml-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-08 21:46:35.173111 evaics.ml-0.1.3/
--rw-r--r--   0 divisor   (1000) root         (0)    11357 2023-03-29 17:24:22.000000 evaics.ml-0.1.3/LICENSE
--rw-r--r--   0 divisor   (1000) root         (0)      711 2023-04-08 21:46:35.173111 evaics.ml-0.1.3/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)      136 2023-04-08 21:45:24.000000 evaics.ml-0.1.3/README.md
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-08 21:46:35.173111 evaics.ml-0.1.3/evaics/
--rw-r--r--   0 divisor   (1000) root         (0)        0 2023-04-08 21:46:28.000000 evaics.ml-0.1.3/evaics/__init__.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-08 21:46:35.173111 evaics.ml-0.1.3/evaics/ml/
--rw-r--r--   0 divisor   (1000) root         (0)    15819 2023-04-08 21:46:28.000000 evaics.ml-0.1.3/evaics/ml/__init__.py
--rw-r--r--   0 divisor   (1000) root         (0)    12572 2023-04-08 21:46:28.000000 evaics.ml-0.1.3/evaics/ml/learning.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-08 21:46:35.173111 evaics.ml-0.1.3/evaics.ml.egg-info/
--rw-r--r--   0 divisor   (1000) root         (0)      711 2023-04-08 21:46:35.000000 evaics.ml-0.1.3/evaics.ml.egg-info/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)      253 2023-04-08 21:46:35.000000 evaics.ml-0.1.3/evaics.ml.egg-info/SOURCES.txt
--rw-r--r--   0 divisor   (1000) root         (0)        1 2023-04-08 21:46:35.000000 evaics.ml-0.1.3/evaics.ml.egg-info/dependency_links.txt
--rw-r--r--   0 divisor   (1000) root         (0)       60 2023-04-08 21:46:35.000000 evaics.ml-0.1.3/evaics.ml.egg-info/requires.txt
--rw-r--r--   0 divisor   (1000) root         (0)        7 2023-04-08 21:46:35.000000 evaics.ml-0.1.3/evaics.ml.egg-info/top_level.txt
--rw-r--r--   0 divisor   (1000) root         (0)       38 2023-04-08 21:46:35.173111 evaics.ml-0.1.3/setup.cfg
--rw-r--r--   0 divisor   (1000) root         (0)      918 2023-04-08 21:46:28.000000 evaics.ml-0.1.3/setup.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-10 20:34:37.887184 evaics.ml-0.1.4/
+-rw-r--r--   0 divisor   (1000) root         (0)    11357 2023-03-29 17:24:22.000000 evaics.ml-0.1.4/LICENSE
+-rw-r--r--   0 divisor   (1000) root         (0)      711 2023-04-10 20:34:37.887184 evaics.ml-0.1.4/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)      136 2023-04-08 21:45:24.000000 evaics.ml-0.1.4/README.md
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-10 20:34:37.887184 evaics.ml-0.1.4/evaics/
+-rw-r--r--   0 divisor   (1000) root         (0)        0 2023-04-10 20:34:34.000000 evaics.ml-0.1.4/evaics/__init__.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-10 20:34:37.887184 evaics.ml-0.1.4/evaics/ml/
+-rw-r--r--   0 divisor   (1000) root         (0)    15851 2023-04-10 20:34:34.000000 evaics.ml-0.1.4/evaics/ml/__init__.py
+-rw-r--r--   0 divisor   (1000) root         (0)    12572 2023-04-10 20:34:34.000000 evaics.ml-0.1.4/evaics/ml/learning.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-10 20:34:37.887184 evaics.ml-0.1.4/evaics.ml.egg-info/
+-rw-r--r--   0 divisor   (1000) root         (0)      711 2023-04-10 20:34:37.000000 evaics.ml-0.1.4/evaics.ml.egg-info/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)      253 2023-04-10 20:34:37.000000 evaics.ml-0.1.4/evaics.ml.egg-info/SOURCES.txt
+-rw-r--r--   0 divisor   (1000) root         (0)        1 2023-04-10 20:34:37.000000 evaics.ml-0.1.4/evaics.ml.egg-info/dependency_links.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       60 2023-04-10 20:34:37.000000 evaics.ml-0.1.4/evaics.ml.egg-info/requires.txt
+-rw-r--r--   0 divisor   (1000) root         (0)        7 2023-04-10 20:34:37.000000 evaics.ml-0.1.4/evaics.ml.egg-info/top_level.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       38 2023-04-10 20:34:37.887184 evaics.ml-0.1.4/setup.cfg
+-rw-r--r--   0 divisor   (1000) root         (0)      918 2023-04-10 20:34:34.000000 evaics.ml-0.1.4/setup.py
```

### Comparing `evaics.ml-0.1.3/LICENSE` & `evaics.ml-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `evaics.ml-0.1.3/PKG-INFO` & `evaics.ml-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evaics.ml
-Version: 0.1.3
+Version: 0.1.4
 Summary: EVA ICS v4 Machine Learning Kit
 Home-page: https://github.com/eva-ics/eva-mlkit-client-python
 Author: Bohemia Automation / Altertech
 Author-email: div@altertech.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `evaics.ml-0.1.3/evaics/ml/__init__.py` & `evaics.ml-0.1.4/evaics/ml/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.3'
+__version__ = '0.1.4'
 
 import sys
 import requests
 import gzip
 import logging
 import time
 import json
@@ -422,23 +422,23 @@
     if output == 'arrow':
         return df
     if tz == 'local':
         tz = time.tzname[0]
     if output == 'pandas':
         import pandas as pd
         df = df.to_pandas()
-        if t_col != 'drop' and tz is not None:
+        if len(df) > 0 and t_col != 'drop' and tz is not None:
             if not from_ipc:
                 df['time'] = pd.to_datetime(df['time'], unit='s')
             df['time'] = df['time'].dt.tz_localize('UTC').dt.tz_convert(tz)
         return df
     elif output == 'polars':
         import polars as pl
         df = pl.from_arrow(df)
-        if t_col != 'drop' and tz is not None:
+        if len(df) > 0 and t_col != 'drop' and tz is not None:
             if not from_ipc:
                 df = df.with_column(pl.from_epoch('time', unit='s'))
             df = df.with_columns(df['time'].dt.replace_time_zone('UTC'))
             df = df.with_columns(df['time'].dt.convert_time_zone(tz))
         return df
     else:
         raise RuntimeError('output unsupported')
```

### Comparing `evaics.ml-0.1.3/evaics/ml/learning.py` & `evaics.ml-0.1.4/evaics/ml/learning.py`

 * *Files identical despite different names*

### Comparing `evaics.ml-0.1.3/evaics.ml.egg-info/PKG-INFO` & `evaics.ml-0.1.4/evaics.ml.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evaics.ml
-Version: 0.1.3
+Version: 0.1.4
 Summary: EVA ICS v4 Machine Learning Kit
 Home-page: https://github.com/eva-ics/eva-mlkit-client-python
 Author: Bohemia Automation / Altertech
 Author-email: div@altertech.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `evaics.ml-0.1.3/setup.py` & `evaics.ml-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.3'
+__version__ = '0.1.4'
 
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
```

