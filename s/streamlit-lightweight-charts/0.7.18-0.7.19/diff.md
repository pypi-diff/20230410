# Comparing `tmp/streamlit-lightweight-charts-0.7.18.tar.gz` & `tmp/streamlit-lightweight-charts-0.7.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-lightweight-charts-0.7.18.tar", last modified: Mon Apr 10 10:04:54 2023, max compression
+gzip compressed data, was "streamlit-lightweight-charts-0.7.19.tar", last modified: Mon Apr 10 10:34:30 2023, max compression
```

## Comparing `streamlit-lightweight-charts-0.7.18.tar` & `streamlit-lightweight-charts-0.7.19.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-10 10:04:54.433588 streamlit-lightweight-charts-0.7.18/
--rw-r--r--   0 joerosa    (501) staff       (20)       64 2023-03-19 00:35:29.000000 streamlit-lightweight-charts-0.7.18/MANIFEST.in
--rw-r--r--   0 joerosa    (501) staff       (20)    28863 2023-04-10 10:04:54.432938 streamlit-lightweight-charts-0.7.18/PKG-INFO
--rw-r--r--   0 joerosa    (501) staff       (20)    22081 2023-04-10 10:03:43.000000 streamlit-lightweight-charts-0.7.18/README.md
--rw-r--r--   0 joerosa    (501) staff       (20)       38 2023-04-10 10:04:54.433764 streamlit-lightweight-charts-0.7.18/setup.cfg
--rw-r--r--   0 joerosa    (501) staff       (20)      936 2023-04-10 10:01:24.000000 streamlit-lightweight-charts-0.7.18/setup.py
-drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-10 10:04:54.414935 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/
--rw-r--r--   0 joerosa    (501) staff       (20)    14199 2023-04-10 09:54:11.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/__init__.py
--rw-r--r--   0 joerosa    (501) staff       (20)    27943 2023-03-19 01:15:29.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/dataSamples.py
-drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-10 10:04:54.411455 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/
-drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-10 10:04:54.420082 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/
--rw-r--r--   0 joerosa    (501) staff       (20)      859 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/asset-manifest.json
--rw-r--r--   0 joerosa    (501) staff       (20)     2052 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/index.html
--rw-r--r--   0 joerosa    (501) staff       (20)      564 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/precache-manifest.e348f70e7319498a2e6b3a0c95da5ac1.js
--rw-r--r--   0 joerosa    (501) staff       (20)     1183 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/service-worker.js
-drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-10 10:04:54.412196 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/
-drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-10 10:04:54.431811 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/
--rw-r--r--   0 joerosa    (501) staff       (20)   776592 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js
--rw-r--r--   0 joerosa    (501) staff       (20)     2242 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js.LICENSE.txt
--rw-r--r--   0 joerosa    (501) staff       (20)  2004921 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js.map
--rw-r--r--   0 joerosa    (501) staff       (20)     2223 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/main.509cd3c1.chunk.js
--rw-r--r--   0 joerosa    (501) staff       (20)     8156 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/main.509cd3c1.chunk.js.map
--rw-r--r--   0 joerosa    (501) staff       (20)     1598 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/runtime-main.e0d8c599.js
--rw-r--r--   0 joerosa    (501) staff       (20)     8317 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/runtime-main.e0d8c599.js.map
-drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-10 10:04:54.417874 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts.egg-info/
--rw-r--r--   0 joerosa    (501) staff       (20)    28863 2023-04-10 10:04:54.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts.egg-info/PKG-INFO
--rw-r--r--   0 joerosa    (501) staff       (20)     1211 2023-04-10 10:04:54.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts.egg-info/SOURCES.txt
--rw-r--r--   0 joerosa    (501) staff       (20)        1 2023-04-10 10:04:54.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts.egg-info/dependency_links.txt
--rw-r--r--   0 joerosa    (501) staff       (20)       16 2023-04-10 10:04:54.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts.egg-info/requires.txt
--rw-r--r--   0 joerosa    (501) staff       (20)       29 2023-04-10 10:04:54.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts.egg-info/top_level.txt
+drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-10 10:34:30.688988 streamlit-lightweight-charts-0.7.19/
+-rw-r--r--   0 joerosa    (501) staff       (20)       64 2023-03-19 00:35:29.000000 streamlit-lightweight-charts-0.7.19/MANIFEST.in
+-rw-r--r--   0 joerosa    (501) staff       (20)    28936 2023-04-10 10:34:30.688453 streamlit-lightweight-charts-0.7.19/PKG-INFO
+-rw-r--r--   0 joerosa    (501) staff       (20)    22146 2023-04-10 10:34:10.000000 streamlit-lightweight-charts-0.7.19/README.md
+-rw-r--r--   0 joerosa    (501) staff       (20)       38 2023-04-10 10:34:30.689158 streamlit-lightweight-charts-0.7.19/setup.cfg
+-rw-r--r--   0 joerosa    (501) staff       (20)      936 2023-04-10 10:34:26.000000 streamlit-lightweight-charts-0.7.19/setup.py
+drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-10 10:34:30.670589 streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/
+-rw-r--r--   0 joerosa    (501) staff       (20)    14198 2023-04-10 10:30:08.000000 streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/__init__.py
+-rw-r--r--   0 joerosa    (501) staff       (20)    27943 2023-03-19 01:15:29.000000 streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/dataSamples.py
+drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-10 10:34:30.668010 streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/
+drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-10 10:34:30.675898 streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/build/
+-rw-r--r--   0 joerosa    (501) staff       (20)      859 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/build/asset-manifest.json
+-rw-r--r--   0 joerosa    (501) staff       (20)     2052 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/build/index.html
+-rw-r--r--   0 joerosa    (501) staff       (20)      564 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/build/precache-manifest.e348f70e7319498a2e6b3a0c95da5ac1.js
+-rw-r--r--   0 joerosa    (501) staff       (20)     1183 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/build/service-worker.js
+drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-10 10:34:30.668399 streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/build/static/
+drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-10 10:34:30.687293 streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/build/static/js/
+-rw-r--r--   0 joerosa    (501) staff       (20)   776592 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js
+-rw-r--r--   0 joerosa    (501) staff       (20)     2242 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js.LICENSE.txt
+-rw-r--r--   0 joerosa    (501) staff       (20)  2004921 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js.map
+-rw-r--r--   0 joerosa    (501) staff       (20)     2223 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/build/static/js/main.509cd3c1.chunk.js
+-rw-r--r--   0 joerosa    (501) staff       (20)     8156 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/build/static/js/main.509cd3c1.chunk.js.map
+-rw-r--r--   0 joerosa    (501) staff       (20)     1598 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/build/static/js/runtime-main.e0d8c599.js
+-rw-r--r--   0 joerosa    (501) staff       (20)     8317 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/build/static/js/runtime-main.e0d8c599.js.map
+drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-10 10:34:30.673304 streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts.egg-info/
+-rw-r--r--   0 joerosa    (501) staff       (20)    28936 2023-04-10 10:34:30.000000 streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts.egg-info/PKG-INFO
+-rw-r--r--   0 joerosa    (501) staff       (20)     1211 2023-04-10 10:34:30.000000 streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts.egg-info/SOURCES.txt
+-rw-r--r--   0 joerosa    (501) staff       (20)        1 2023-04-10 10:34:30.000000 streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts.egg-info/dependency_links.txt
+-rw-r--r--   0 joerosa    (501) staff       (20)       16 2023-04-10 10:34:30.000000 streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts.egg-info/requires.txt
+-rw-r--r--   0 joerosa    (501) staff       (20)       29 2023-04-10 10:34:30.000000 streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts.egg-info/top_level.txt
```

### Comparing `streamlit-lightweight-charts-0.7.18/PKG-INFO` & `streamlit-lightweight-charts-0.7.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: streamlit-lightweight-charts
-Version: 0.7.18
+Version: 0.7.19
 Summary: Wrapper for TradingView lightweight-charts
 Home-page: https://github.com/freyastreamlit/streamlit-lightweight-charts
 Author: Joe Rosa
 Author-email: joe.rosa@itpmngt.co.uk
 License: MIT
 Description: # streamlit-lightweight-charts
         Streamlit wrapper for performant Tradingview's Financial: `lightweight-charts`
         
         The Lightweight Charts library is the best choice to display financial data as an interactive chart on a web page without affecting loading speed and performance.
         
         - [Features Demo](https://www.tradingview.com/lightweight-charts/)
         - [Documentation](https://tradingview.github.io/lightweight-charts/)
         - [GitHub](https://github.com/tradingview/lightweight-charts)
+        - [Pypi](https://pypi.org/project/streamlit-lightweight-charts/)
         
         ### Versions
         - Version 0.7.12 - Added "markers" to series
         - Version 0.7.13 - Example of watermarks
         - Version 0.7.15 - Example using Pandas
         - Version 0.7.16 - Work examples on [Streamlit Cloud](https://share.streamlit.io/)
         - Version 0.7.17 - Added integration example for Data Toggling
-        - Version 0.7.18 - FIX: React build was not been commited
+        - Version 0.7.19 - FIX: React build was not been commited
         
         ## How to install:
         ```
         python -m pip install streamlit-lightweight-charts
         ```
         
         ## How to use:
```

### Comparing `streamlit-lightweight-charts-0.7.18/README.md` & `streamlit-lightweight-charts-0.7.19/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 Streamlit wrapper for performant Tradingview's Financial: `lightweight-charts`
 
 The Lightweight Charts library is the best choice to display financial data as an interactive chart on a web page without affecting loading speed and performance.
 
 - [Features Demo](https://www.tradingview.com/lightweight-charts/)
 - [Documentation](https://tradingview.github.io/lightweight-charts/)
 - [GitHub](https://github.com/tradingview/lightweight-charts)
+- [Pypi](https://pypi.org/project/streamlit-lightweight-charts/)
 
 ### Versions
 - Version 0.7.12 - Added "markers" to series
 - Version 0.7.13 - Example of watermarks
 - Version 0.7.15 - Example using Pandas
 - Version 0.7.16 - Work examples on [Streamlit Cloud](https://share.streamlit.io/)
 - Version 0.7.17 - Added integration example for Data Toggling
-- Version 0.7.18 - FIX: React build was not been commited
+- Version 0.7.19 - FIX: React build was not been commited
 
 ## How to install:
 ```
 python -m pip install streamlit-lightweight-charts
 ```
 
 ## How to use:
```

### Comparing `streamlit-lightweight-charts-0.7.18/setup.py` & `streamlit-lightweight-charts-0.7.19/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="streamlit-lightweight-charts",
-    version="0.7.18",
+    version="0.7.19",
     author="Joe Rosa",
     author_email="joe.rosa@itpmngt.co.uk",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
```

### Comparing `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/__init__.py` & `streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from typing import Dict
 from enum import Enum
 import streamlit.components.v1 as components
 
 _COMPONENT_NAME = "streamlit_lightweight_charts"
-_RELEASE = False
+_RELEASE = True
 
 class Chart(str, Enum):
     Area = 'addAreaSeries'
     Baseline = 'addBaselineSeries'
     Histogram = 'addHistogramSeries'
     Line = 'addLineSeries'
     Bar = 'addBarSeries'
@@ -16,16 +16,16 @@
 
 parent_dir = os.path.dirname(os.path.abspath(__file__))
 build_dir = os.path.join(parent_dir, "frontend","build")
 
 if not _RELEASE:
     _component_func = components.declare_component(
         _COMPONENT_NAME,
-        path=build_dir,
-        # url="http://localhost:3001",
+        # path=build_dir,
+        url="http://localhost:3001",
     )
 else:
     _component_func = components.declare_component(
         _COMPONENT_NAME,
         path=build_dir
     )
```

### Comparing `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/dataSamples.py` & `streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/dataSamples.py`

 * *Files identical despite different names*

### Comparing `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/asset-manifest.json` & `streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/index.html` & `streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/precache-manifest.e348f70e7319498a2e6b3a0c95da5ac1.js` & `streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/build/precache-manifest.e348f70e7319498a2e6b3a0c95da5ac1.js`

 * *Files identical despite different names*

### Comparing `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/service-worker.js` & `streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js` & `streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js.LICENSE.txt` & `streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js.map` & `streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/main.509cd3c1.chunk.js` & `streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/build/static/js/main.509cd3c1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/main.509cd3c1.chunk.js.map` & `streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/build/static/js/main.509cd3c1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/runtime-main.e0d8c599.js` & `streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/build/static/js/runtime-main.e0d8c599.js`

 * *Files identical despite different names*

### Comparing `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/runtime-main.e0d8c599.js.map` & `streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts/frontend/build/static/js/runtime-main.e0d8c599.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts.egg-info/PKG-INFO` & `streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: streamlit-lightweight-charts
-Version: 0.7.18
+Version: 0.7.19
 Summary: Wrapper for TradingView lightweight-charts
 Home-page: https://github.com/freyastreamlit/streamlit-lightweight-charts
 Author: Joe Rosa
 Author-email: joe.rosa@itpmngt.co.uk
 License: MIT
 Description: # streamlit-lightweight-charts
         Streamlit wrapper for performant Tradingview's Financial: `lightweight-charts`
         
         The Lightweight Charts library is the best choice to display financial data as an interactive chart on a web page without affecting loading speed and performance.
         
         - [Features Demo](https://www.tradingview.com/lightweight-charts/)
         - [Documentation](https://tradingview.github.io/lightweight-charts/)
         - [GitHub](https://github.com/tradingview/lightweight-charts)
+        - [Pypi](https://pypi.org/project/streamlit-lightweight-charts/)
         
         ### Versions
         - Version 0.7.12 - Added "markers" to series
         - Version 0.7.13 - Example of watermarks
         - Version 0.7.15 - Example using Pandas
         - Version 0.7.16 - Work examples on [Streamlit Cloud](https://share.streamlit.io/)
         - Version 0.7.17 - Added integration example for Data Toggling
-        - Version 0.7.18 - FIX: React build was not been commited
+        - Version 0.7.19 - FIX: React build was not been commited
         
         ## How to install:
         ```
         python -m pip install streamlit-lightweight-charts
         ```
         
         ## How to use:
```

### Comparing `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts.egg-info/SOURCES.txt` & `streamlit-lightweight-charts-0.7.19/streamlit_lightweight_charts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

