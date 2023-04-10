# Comparing `tmp/streamlit-lightweight-charts-0.7.17.tar.gz` & `tmp/streamlit-lightweight-charts-0.7.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-lightweight-charts-0.7.17.tar", last modified: Sun Apr  2 15:24:30 2023, max compression
+gzip compressed data, was "streamlit-lightweight-charts-0.7.18.tar", last modified: Mon Apr 10 10:04:54 2023, max compression
```

## Comparing `streamlit-lightweight-charts-0.7.17.tar` & `streamlit-lightweight-charts-0.7.18.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-02 15:24:30.997170 streamlit-lightweight-charts-0.7.17/
--rw-r--r--   0 joerosa    (501) staff       (20)       64 2023-03-19 00:35:29.000000 streamlit-lightweight-charts-0.7.17/MANIFEST.in
--rw-r--r--   0 joerosa    (501) staff       (20)    28797 2023-04-02 15:24:30.996648 streamlit-lightweight-charts-0.7.17/PKG-INFO
--rw-r--r--   0 joerosa    (501) staff       (20)    22023 2023-04-02 15:19:36.000000 streamlit-lightweight-charts-0.7.17/README.md
--rw-r--r--   0 joerosa    (501) staff       (20)       38 2023-04-02 15:24:30.997276 streamlit-lightweight-charts-0.7.17/setup.cfg
--rw-r--r--   0 joerosa    (501) staff       (20)      936 2023-04-02 15:23:29.000000 streamlit-lightweight-charts-0.7.17/setup.py
-drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-02 15:24:30.982422 streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/
--rw-r--r--   0 joerosa    (501) staff       (20)    14198 2023-04-02 15:17:53.000000 streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/__init__.py
--rw-r--r--   0 joerosa    (501) staff       (20)    27943 2023-03-19 01:15:29.000000 streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/dataSamples.py
-drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-02 15:24:30.980041 streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/
-drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-02 15:24:30.986420 streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/build/
--rw-r--r--   0 joerosa    (501) staff       (20)      859 2023-03-19 12:58:31.000000 streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/build/asset-manifest.json
--rw-r--r--   0 joerosa    (501) staff       (20)     2052 2023-03-19 12:58:31.000000 streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/build/index.html
--rw-r--r--   0 joerosa    (501) staff       (20)      564 2023-03-19 12:58:31.000000 streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/build/precache-manifest.e6bd8d0d7ff31e7ed0c54de396b38e6a.js
--rw-r--r--   0 joerosa    (501) staff       (20)     1183 2023-03-19 12:58:31.000000 streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/build/service-worker.js
-drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-02 15:24:30.980396 streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/build/static/
-drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-02 15:24:30.995904 streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/build/static/js/
--rw-r--r--   0 joerosa    (501) staff       (20)   776592 2023-03-19 12:58:31.000000 streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js
--rw-r--r--   0 joerosa    (501) staff       (20)     2242 2023-03-19 12:58:31.000000 streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js.LICENSE.txt
--rw-r--r--   0 joerosa    (501) staff       (20)  2004921 2023-03-19 12:58:31.000000 streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js.map
--rw-r--r--   0 joerosa    (501) staff       (20)     2193 2023-03-19 12:58:31.000000 streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/build/static/js/main.57993593.chunk.js
--rw-r--r--   0 joerosa    (501) staff       (20)     7018 2023-03-19 12:58:31.000000 streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/build/static/js/main.57993593.chunk.js.map
--rw-r--r--   0 joerosa    (501) staff       (20)     1598 2023-03-19 12:58:31.000000 streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/build/static/js/runtime-main.e0d8c599.js
--rw-r--r--   0 joerosa    (501) staff       (20)     8317 2023-03-19 12:58:31.000000 streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/build/static/js/runtime-main.e0d8c599.js.map
-drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-02 15:24:30.984808 streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts.egg-info/
--rw-r--r--   0 joerosa    (501) staff       (20)    28797 2023-04-02 15:24:30.000000 streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts.egg-info/PKG-INFO
--rw-r--r--   0 joerosa    (501) staff       (20)     1211 2023-04-02 15:24:30.000000 streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts.egg-info/SOURCES.txt
--rw-r--r--   0 joerosa    (501) staff       (20)        1 2023-04-02 15:24:30.000000 streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts.egg-info/dependency_links.txt
--rw-r--r--   0 joerosa    (501) staff       (20)       16 2023-04-02 15:24:30.000000 streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts.egg-info/requires.txt
--rw-r--r--   0 joerosa    (501) staff       (20)       29 2023-04-02 15:24:30.000000 streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts.egg-info/top_level.txt
+drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-10 10:04:54.433588 streamlit-lightweight-charts-0.7.18/
+-rw-r--r--   0 joerosa    (501) staff       (20)       64 2023-03-19 00:35:29.000000 streamlit-lightweight-charts-0.7.18/MANIFEST.in
+-rw-r--r--   0 joerosa    (501) staff       (20)    28863 2023-04-10 10:04:54.432938 streamlit-lightweight-charts-0.7.18/PKG-INFO
+-rw-r--r--   0 joerosa    (501) staff       (20)    22081 2023-04-10 10:03:43.000000 streamlit-lightweight-charts-0.7.18/README.md
+-rw-r--r--   0 joerosa    (501) staff       (20)       38 2023-04-10 10:04:54.433764 streamlit-lightweight-charts-0.7.18/setup.cfg
+-rw-r--r--   0 joerosa    (501) staff       (20)      936 2023-04-10 10:01:24.000000 streamlit-lightweight-charts-0.7.18/setup.py
+drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-10 10:04:54.414935 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/
+-rw-r--r--   0 joerosa    (501) staff       (20)    14199 2023-04-10 09:54:11.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/__init__.py
+-rw-r--r--   0 joerosa    (501) staff       (20)    27943 2023-03-19 01:15:29.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/dataSamples.py
+drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-10 10:04:54.411455 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/
+drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-10 10:04:54.420082 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/
+-rw-r--r--   0 joerosa    (501) staff       (20)      859 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/asset-manifest.json
+-rw-r--r--   0 joerosa    (501) staff       (20)     2052 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/index.html
+-rw-r--r--   0 joerosa    (501) staff       (20)      564 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/precache-manifest.e348f70e7319498a2e6b3a0c95da5ac1.js
+-rw-r--r--   0 joerosa    (501) staff       (20)     1183 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/service-worker.js
+drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-10 10:04:54.412196 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/
+drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-10 10:04:54.431811 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/
+-rw-r--r--   0 joerosa    (501) staff       (20)   776592 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js
+-rw-r--r--   0 joerosa    (501) staff       (20)     2242 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js.LICENSE.txt
+-rw-r--r--   0 joerosa    (501) staff       (20)  2004921 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js.map
+-rw-r--r--   0 joerosa    (501) staff       (20)     2223 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/main.509cd3c1.chunk.js
+-rw-r--r--   0 joerosa    (501) staff       (20)     8156 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/main.509cd3c1.chunk.js.map
+-rw-r--r--   0 joerosa    (501) staff       (20)     1598 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/runtime-main.e0d8c599.js
+-rw-r--r--   0 joerosa    (501) staff       (20)     8317 2023-04-10 09:58:58.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/runtime-main.e0d8c599.js.map
+drwxr-xr-x   0 joerosa    (501) staff       (20)        0 2023-04-10 10:04:54.417874 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts.egg-info/
+-rw-r--r--   0 joerosa    (501) staff       (20)    28863 2023-04-10 10:04:54.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts.egg-info/PKG-INFO
+-rw-r--r--   0 joerosa    (501) staff       (20)     1211 2023-04-10 10:04:54.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts.egg-info/SOURCES.txt
+-rw-r--r--   0 joerosa    (501) staff       (20)        1 2023-04-10 10:04:54.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts.egg-info/dependency_links.txt
+-rw-r--r--   0 joerosa    (501) staff       (20)       16 2023-04-10 10:04:54.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts.egg-info/requires.txt
+-rw-r--r--   0 joerosa    (501) staff       (20)       29 2023-04-10 10:04:54.000000 streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts.egg-info/top_level.txt
```

### Comparing `streamlit-lightweight-charts-0.7.17/PKG-INFO` & `streamlit-lightweight-charts-0.7.18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-lightweight-charts
-Version: 0.7.17
+Version: 0.7.18
 Summary: Wrapper for TradingView lightweight-charts
 Home-page: https://github.com/freyastreamlit/streamlit-lightweight-charts
 Author: Joe Rosa
 Author-email: joe.rosa@itpmngt.co.uk
 License: MIT
 Description: # streamlit-lightweight-charts
         Streamlit wrapper for performant Tradingview's Financial: `lightweight-charts`
@@ -17,14 +17,15 @@
         
         ### Versions
         - Version 0.7.12 - Added "markers" to series
         - Version 0.7.13 - Example of watermarks
         - Version 0.7.15 - Example using Pandas
         - Version 0.7.16 - Work examples on [Streamlit Cloud](https://share.streamlit.io/)
         - Version 0.7.17 - Added integration example for Data Toggling
+        - Version 0.7.18 - FIX: React build was not been commited
         
         ## How to install:
         ```
         python -m pip install streamlit-lightweight-charts
         ```
         
         ## How to use:
```

### Comparing `streamlit-lightweight-charts-0.7.17/README.md` & `streamlit-lightweight-charts-0.7.18/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 ### Versions
 - Version 0.7.12 - Added "markers" to series
 - Version 0.7.13 - Example of watermarks
 - Version 0.7.15 - Example using Pandas
 - Version 0.7.16 - Work examples on [Streamlit Cloud](https://share.streamlit.io/)
 - Version 0.7.17 - Added integration example for Data Toggling
+- Version 0.7.18 - FIX: React build was not been commited
 
 ## How to install:
 ```
 python -m pip install streamlit-lightweight-charts
 ```
 
 ## How to use:
```

### Comparing `streamlit-lightweight-charts-0.7.17/setup.py` & `streamlit-lightweight-charts-0.7.18/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="streamlit-lightweight-charts",
-    version="0.7.17",
+    version="0.7.18",
     author="Joe Rosa",
     author_email="joe.rosa@itpmngt.co.uk",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
```

### Comparing `streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/__init__.py` & `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from typing import Dict
 from enum import Enum
 import streamlit.components.v1 as components
 
 _COMPONENT_NAME = "streamlit_lightweight_charts"
-_RELEASE = True
+_RELEASE = False
 
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
-        # path=build_dir,
-        url="http://localhost:3001",
+        path=build_dir,
+        # url="http://localhost:3001",
     )
 else:
     _component_func = components.declare_component(
         _COMPONENT_NAME,
         path=build_dir
     )
```

### Comparing `streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/dataSamples.py` & `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/dataSamples.py`

 * *Files identical despite different names*

### Comparing `streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/build/asset-manifest.json` & `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/asset-manifest.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8068181818181819%*

 * *Differences: {"'entrypoints'": "{insert: [(2, 'static/js/main.509cd3c1.chunk.js')], delete: [2]}",*

 * * "'files'": "{'main.js': './static/js/main.509cd3c1.chunk.js', 'main.js.map': "*

 * *            "'./static/js/main.509cd3c1.chunk.js.map', "*

 * *            "'precache-manifest.e348f70e7319498a2e6b3a0c95da5ac1.js': "*

 * *            "'./precache-manifest.e348f70e7319498a2e6b3a0c95da5ac1.js', delete: "*

 * *            "['precache-manifest.e6bd8d0d7ff31e7ed0c54de396b38e6a.js']}"}*

```diff
@@ -1,18 +1,18 @@
 {
     "entrypoints": [
         "static/js/runtime-main.e0d8c599.js",
         "static/js/2.70acfc76.chunk.js",
-        "static/js/main.57993593.chunk.js"
+        "static/js/main.509cd3c1.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
-        "main.js": "./static/js/main.57993593.chunk.js",
-        "main.js.map": "./static/js/main.57993593.chunk.js.map",
-        "precache-manifest.e6bd8d0d7ff31e7ed0c54de396b38e6a.js": "./precache-manifest.e6bd8d0d7ff31e7ed0c54de396b38e6a.js",
+        "main.js": "./static/js/main.509cd3c1.chunk.js",
+        "main.js.map": "./static/js/main.509cd3c1.chunk.js.map",
+        "precache-manifest.e348f70e7319498a2e6b3a0c95da5ac1.js": "./precache-manifest.e348f70e7319498a2e6b3a0c95da5ac1.js",
         "runtime-main.js": "./static/js/runtime-main.e0d8c599.js",
         "runtime-main.js.map": "./static/js/runtime-main.e0d8c599.js.map",
         "service-worker.js": "./service-worker.js",
         "static/js/2.70acfc76.chunk.js": "./static/js/2.70acfc76.chunk.js",
         "static/js/2.70acfc76.chunk.js.LICENSE.txt": "./static/js/2.70acfc76.chunk.js.LICENSE.txt",
         "static/js/2.70acfc76.chunk.js.map": "./static/js/2.70acfc76.chunk.js.map"
     }
```

### Comparing `streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/build/index.html` & `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,i,l=t[0],a=t[1],f=t[2],p=0,s=[];p<l.length;p++)i=l[p],Object.prototype.hasOwnProperty.call(o,i)&&o[i]&&s.push(o[i][0]),o[i]=0;for(n in a)Object.prototype.hasOwnProperty.call(a,n)&&(e[n]=a[n]);for(c&&c(t);s.length;)s.shift()();return u.push.apply(u,f||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,l=1;l<r.length;l++){var a=r[l];0!==o[a]&&(n=!1)}n&&(u.splice(t--,1),e=i(i.s=r[0]))}return e}var n={},o={1:0},u=[];function i(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,i),r.l=!0,r.exports}i.m=e,i.c=n,i.d=function(e,t,r){i.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},i.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},i.t=function(e,t){if(1&t&&(e=i(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(i.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)i.d(r,n,function(t){return e[t]}.bind(null,n));return r},i.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return i.d(t,"a",t),t},i.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},i.p="./";var l=this.webpackJsonpstreamlit_lightweight_charts=this.webpackJsonpstreamlit_lightweight_charts||[],a=l.push.bind(l);l.push=t,l=l.slice();for(var f=0;f<l.length;f++)t(l[f]);var c=a;r()}([])</script><script src="./static/js/2.70acfc76.chunk.js"></script><script src="./static/js/main.57993593.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,i,l=t[0],a=t[1],f=t[2],p=0,s=[];p<l.length;p++)i=l[p],Object.prototype.hasOwnProperty.call(o,i)&&o[i]&&s.push(o[i][0]),o[i]=0;for(n in a)Object.prototype.hasOwnProperty.call(a,n)&&(e[n]=a[n]);for(c&&c(t);s.length;)s.shift()();return u.push.apply(u,f||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,l=1;l<r.length;l++){var a=r[l];0!==o[a]&&(n=!1)}n&&(u.splice(t--,1),e=i(i.s=r[0]))}return e}var n={},o={1:0},u=[];function i(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,i),r.l=!0,r.exports}i.m=e,i.c=n,i.d=function(e,t,r){i.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},i.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},i.t=function(e,t){if(1&t&&(e=i(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(i.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)i.d(r,n,function(t){return e[t]}.bind(null,n));return r},i.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return i.d(t,"a",t),t},i.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},i.p="./";var l=this.webpackJsonpstreamlit_lightweight_charts=this.webpackJsonpstreamlit_lightweight_charts||[],a=l.push.bind(l);l.push=t,l=l.slice();for(var f=0;f<l.length;f++)t(l[f]);var c=a;r()}([])</script><script src="./static/js/2.70acfc76.chunk.js"></script><script src="./static/js/main.509cd3c1.chunk.js"></script></body></html>
```

### Comparing `streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/build/precache-manifest.e6bd8d0d7ff31e7ed0c54de396b38e6a.js` & `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/precache-manifest.e348f70e7319498a2e6b3a0c95da5ac1.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 self.__precacheManifest = (self.__precacheManifest || []).concat([{
-    "revision": "3551421bff8730fe05c41e013b5e9ee6",
+    "revision": "db6357f0bcc0d206ab0c3579b9cc45d0",
     "url": "./index.html"
 }, {
     "revision": "98d8c28a96c309ff10d7",
     "url": "./static/js/2.70acfc76.chunk.js"
 }, {
     "revision": "f263fa2f915c7728c49ada0765c8d30c",
     "url": "./static/js/2.70acfc76.chunk.js.LICENSE.txt"
 }, {
-    "revision": "3f2d319813cb7f92e702",
-    "url": "./static/js/main.57993593.chunk.js"
+    "revision": "79531bf4cf4d8373b518",
+    "url": "./static/js/main.509cd3c1.chunk.js"
 }, {
     "revision": "f67f485cd6c9968cb460",
     "url": "./static/js/runtime-main.e0d8c599.js"
 }]);
```

### Comparing `streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/build/service-worker.js` & `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/service-worker.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
  * and re-run your build process.
  * See https://goo.gl/2aRDsh
  */
 
 importScripts("https://storage.googleapis.com/workbox-cdn/releases/4.3.1/workbox-sw.js");
 
 importScripts(
-    "./precache-manifest.e6bd8d0d7ff31e7ed0c54de396b38e6a.js"
+    "./precache-manifest.e348f70e7319498a2e6b3a0c95da5ac1.js"
 );
 
 self.addEventListener('message', (event) => {
     if (event.data && event.data.type === 'SKIP_WAITING') {
         self.skipWaiting();
     }
 });
```

### Comparing `streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js` & `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js.LICENSE.txt` & `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js.map` & `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/build/static/js/main.57993593.chunk.js` & `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/main.509cd3c1.chunk.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,113 +1,113 @@
 (this.webpackJsonpstreamlit_lightweight_charts = this.webpackJsonpstreamlit_lightweight_charts || []).push([
     [0], {
-        26: function(e, t, i) {
-            e.exports = i(36)
+        26: function(e, t, r) {
+            e.exports = r(36)
         },
-        36: function(e, t, i) {
+        36: function(e, t, r) {
             "use strict";
-            i.r(t);
-            var a = i(10),
-                r = i.n(a),
-                n = i(23),
-                c = i.n(n),
-                o = i(16),
-                s = i(5),
-                l = i(9),
-                u = i(25),
+            r.r(t);
+            var a = r(10),
+                i = r.n(a),
+                n = r(23),
+                c = r.n(n),
+                o = r(16),
+                s = r(5),
+                l = r(9),
+                u = r(25),
                 f = function() {
                     var e = Object(o.useRenderData)().args.charts,
                         t = Object(a.useRef)(null),
-                        i = Array(e.length).fill(Object(a.useRef)(null)),
+                        r = Array(e.length).fill(Object(a.useRef)(null)),
                         n = Object(a.useRef)([]);
                     return Object(a.useEffect)((function() {
-                        if (!i.find((function(e) {
+                        if (!r.find((function(e) {
                                 return !e.current
                             }))) {
-                            i.forEach((function(t, a) {
-                                var r = n.current[a] = Object(u.a)(t.current, Object(l.a)({
-                                    height: 300,
-                                    width: i[a].current.clientWidth
-                                }, e[a].chart));
-                                r.timeScale().fitContent();
-                                var c, o = Object(s.a)(e[a].series);
+                            r.forEach((function(t, a) {
+                                var i, c = n.current[a] = Object(u.a)(t.current, Object(l.a)({
+                                        height: 300,
+                                        width: r[a].current.clientWidth
+                                    }, e[a].chart)),
+                                    o = Object(s.a)(e[a].series);
                                 try {
-                                    for (o.s(); !(c = o.n()).done;) {
-                                        var f = c.value,
+                                    for (o.s(); !(i = o.n()).done;) {
+                                        var f = i.value,
                                             d = void 0;
                                         switch (f.type) {
                                             case "Area":
-                                                d = r.addAreaSeries(f.options);
+                                                d = c.addAreaSeries(f.options);
                                                 break;
                                             case "Bar":
-                                                d = r.addBarSeries(f.options);
+                                                d = c.addBarSeries(f.options);
                                                 break;
                                             case "Baseline":
-                                                d = r.addBaselineSeries(f.options);
+                                                d = c.addBaselineSeries(f.options);
                                                 break;
                                             case "Candlestick":
-                                                d = r.addCandlestickSeries(f.options);
+                                                d = c.addCandlestickSeries(f.options);
                                                 break;
                                             case "Histogram":
-                                                d = r.addHistogramSeries(f.options);
+                                                d = c.addHistogramSeries(f.options);
                                                 break;
                                             case "Line":
-                                                d = r.addLineSeries(f.options);
+                                                d = c.addLineSeries(f.options);
                                                 break;
                                             default:
                                                 return
                                         }
-                                        f.priceScale && r.priceScale(f.options.priceScaleId || "").applyOptions(f.priceScale), d.setData(f.data)
+                                        f.priceScale && c.priceScale(f.options.priceScaleId || "").applyOptions(f.priceScale), d.setData(f.data), f.markers && d.setMarkers(f.markers)
                                     }
                                 } catch (h) {
                                     o.e(h)
                                 } finally {
                                     o.f()
                                 }
+                                c.timeScale().fitContent()
                             }));
                             var t = n.current.map((function(e) {
                                 return e
                             }));
                             return e.length > 1 && t.forEach((function(e) {
-                                    e && (e.timeScale().subscribeVisibleTimeRangeChange((function(i) {
+                                    e && (e.timeScale().subscribeVisibleTimeRangeChange((function(r) {
                                         t.filter((function(t) {
                                             return t !== e
                                         })).forEach((function(t) {
                                             t.timeScale().applyOptions({
                                                 rightOffset: e.timeScale().scrollPosition()
                                             })
                                         }))
-                                    })), e.timeScale().subscribeVisibleLogicalRangeChange((function(i) {
-                                        i && t.filter((function(t) {
+                                    })), e.timeScale().subscribeVisibleLogicalRangeChange((function(r) {
+                                        r && t.filter((function(t) {
                                             return t !== e
                                         })).forEach((function(e) {
                                             e.timeScale().setVisibleLogicalRange({
-                                                from: null === i || void 0 === i ? void 0 : i.from,
-                                                to: null === i || void 0 === i ? void 0 : i.to
+                                                from: null === r || void 0 === r ? void 0 : r.from,
+                                                to: null === r || void 0 === r ? void 0 : r.to
                                             })
                                         }))
                                     })))
                                 })),
                                 function() {
                                     t.forEach((function(e) {
                                         e.remove()
                                     }))
                                 }
                         }
-                    }), [e, i, n]), r.a.createElement("div", {
+                    }), [e, r, n]), i.a.createElement("div", {
                         ref: t
-                    }, i.map((function(e, t) {
-                        return r.a.createElement("div", {
+                    }, r.map((function(e, t) {
+                        return i.a.createElement("div", {
                             ref: e,
                             id: "lightweight-charts-".concat(t),
                             key: "lightweight-charts-".concat(t)
                         })
                     })))
                 };
-            c.a.render(r.a.createElement(r.a.StrictMode, null, r.a.createElement(o.StreamlitProvider, null, r.a.createElement(f, null))), document.getElementById("root"))
+            c.a.render(i.a.createElement(i.a.StrictMode, null, i.a.createElement(o.StreamlitProvider, null, i.a.createElement(f, null))), document.getElementById("root"))
         }
     },
     [
         [26, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.57993593.chunk.js.map
+//# sourceMappingURL=main.509cd3c1.chunk.js.map
```

### Comparing `streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/build/static/js/main.57993593.chunk.js.map` & `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/main.509cd3c1.chunk.js.map`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8023809523809524%*

 * *Differences: {"'file'": "'static/js/main.509cd3c1.chunk.js'",*

 * * "'mappings'": "'4PAiJeA,EA1ImC,WAIhD,IACMC,EADaC,0BACWC,KAAa,OAErCC,EAAqBC,iBAAuB,MAC5CC,EAAcC,MAAMN,EAAWO,QAAQC,KAAKJ,iBAAuB,OACnEK,EAAYL,iBAAoB,IAmHpC,OAjHAM,qBAAU,WACR,IAAIL,EAAYM,MAAK,SAACC,GAAG,OAAMA,EAAIC,WAAnC,CAEAR,EAAYS,SAAQ,SAACF,EAAKG,GACxB,IAQyCC,EARnCC,EAAQR,EAAUI,QAAQE,GAAKG,YACnCN,EAAIC,QAAOM,YAAA,CACTC,OAAQ,IACRC,MAAOhB,EAAYU,GAAGF,QAAQS,aAC3BtB,EAAWe,GAAGE,QAEnBM,EAAAC,YAEmBxB,EAAWe,GAAGU,QAAM,IAAzC,IAAAF,EAAAG,MAAAV,EAAAO,EAAAI,KAAAC,MAA0C, […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.57993593.chunk.js",
-    "mappings": "4PAqHeA,EA9GmC,WAIhD,IACMC,EADaC,0BACWC,KAAa,OAErCC,EAAqBC,iBAAuB,MAC5CC,EAAcC,MAAMN,EAAWO,QAAQC,KAAKJ,iBAAuB,OACnEK,EAAYL,iBAAoB,IAuFpC,OArFAM,qBAAU,WACR,IAAIL,EAAYM,MAAK,SAACC,GAAG,OAAMA,EAAIC,WAAnC,CAEAR,EAAYS,SAAQ,SAACF,EAAKG,GACxB,IAAMC,EAAQP,EAAUI,QAAQE,GAAKE,YACnCL,EAAIC,QAAOK,YAAA,CACTC,OAAQ,IACRC,MAAOf,EAAYU,GAAGF,QAAQQ,aAC3BrB,EAAWe,GAAGC,QAIrBA,EAAMM,YAAYC,aAAa,IAEUC,EAFVC,EAAAC,YAEV1B,EAAWe,GAAGY,QAAM,IAAzC,IAAAF,EAAAG,MAAAJ,EAAAC,EAAAI,KAAAC,MAA0C,CAAC,IAAhCH,EAAMH,EAAAO,MAEXC,OAAW,EACf,OAAOL,EAAOM,MACZ,IAAK,OACHD,EAAchB,EAAMkB,cAAcP,EAAOQ,SACzC,MACF,IAAK,MACHH,EAAchB,EAAMoB,aAAaT,EAAOQ,SACxC,MACF,IAAK,WACHH,EAAchB,EAAMqB,kBAAkBV,EAAOQ,SAC7C,MACF,IAAK,cACHH,EAAchB,EAAMsB,qBAAqBX,EAAOQ,SAChD,MACF,IAAK,YACHH,EAAchB,EAAMuB,mBAAmBZ,EAAOQ,SAC9C,MACF,IAAK,OACHH,EAAchB,EAAMwB,cAAcb,EAAOQ,SACzC,MACF,QACI,OAGHR,EAAOc,YACRzB,EAAMyB,WAAWd,EAAOQ,QAAQO,cAAgB,IAAIC,aAAahB,EAAOc,YAE1ET,EAAYY,QAAQjB,EAAOkB,OAC5B,MAAAC,GAAArB,EAAAsB,EAAAD,GAAA,QAAArB,EAAAuB,QAIH,IAAMC,EAASxC,EAAUI,QAAQqC,KAAI,SAACC,GAAC,OAAKA,KA6B5C,OA3BGnD,EAAWO,OAAS,GACrB0C,EAAOnC,SAAQ,SAACE,GACTA,IAELA,EAAMM,YAAY8B,iCAAgC,SAACL,GACjDE,EACGI,QAAO,SAACF,GAAC,OAAKA,IAAMnC,KACpBF,SAAQ,SAACqC,GACRA,EAAE7B,YAAYqB,aAAa,CACzBW,YAAatC,EAAMM,YAAYiC,yBAIvCvC,EAAMM,YAAYkC,oCAAmC,SAACC,GAChDA,GACFR,EACGI,QAAO,SAACF,GAAC,OAAKA,IAAMnC,KACpBF,SAAQ,SAACqC,GACRA,EAAE7B,YAAYoC,uBAAuB,CACnCC,KAAW,OAALF,QAAK,IAALA,OAAK,EAALA,EAAOE,KACbC,GAAS,OAALH,QAAK,IAALA,OAAK,EAALA,EAAOG,eAOlB,WACLX,EAAOnC,SAAQ,SAACE,GACdA,EAAM6C,gBAIT,CAAE7D,EAAYK,EAAaI,IAG5BqD,IAAAC,cAAA,OAAKnD,IAAKT,GACPE,EAAY6C,KAAI,SAACtC,EAAKG,GAAC,OACtB+C,IAAAC,cAAA,OACEnD,IAAKA,EACLoD,GAAE,sBAAAC,OAAwBlD,GAC1BmD,IAAG,sBAAAD,OAAwBlD,UCxGvCoD,IAASC,OACPN,IAAAC,cAACD,IAAMO,WAAU,KACfP,IAAAC,cAACO,oBAAiB,KAChBR,IAAAC,cAACQ,EAAiB,QAGtBC,SAASC,eAAe,W",
+    "file": "static/js/main.509cd3c1.chunk.js",
+    "mappings": "4PAiJeA,EA1ImC,WAIhD,IACMC,EADaC,0BACWC,KAAa,OAErCC,EAAqBC,iBAAuB,MAC5CC,EAAcC,MAAMN,EAAWO,QAAQC,KAAKJ,iBAAuB,OACnEK,EAAYL,iBAAoB,IAmHpC,OAjHAM,qBAAU,WACR,IAAIL,EAAYM,MAAK,SAACC,GAAG,OAAMA,EAAIC,WAAnC,CAEAR,EAAYS,SAAQ,SAACF,EAAKG,GACxB,IAQyCC,EARnCC,EAAQR,EAAUI,QAAQE,GAAKG,YACnCN,EAAIC,QAAOM,YAAA,CACTC,OAAQ,IACRC,MAAOhB,EAAYU,GAAGF,QAAQS,aAC3BtB,EAAWe,GAAGE,QAEnBM,EAAAC,YAEmBxB,EAAWe,GAAGU,QAAM,IAAzC,IAAAF,EAAAG,MAAAV,EAAAO,EAAAI,KAAAC,MAA0C,CAAC,IAAhCH,EAAMT,EAAAa,MAEXC,OAAW,EACf,OAAOL,EAAOM,MACZ,IAAK,OACHD,EAAcb,EAAMe,cAAcP,EAAOQ,SACzC,MACF,IAAK,MACHH,EAAcb,EAAMiB,aAAaT,EAAOQ,SACxC,MACF,IAAK,WACHH,EAAcb,EAAMkB,kBAAkBV,EAAOQ,SAC7C,MACF,IAAK,cACHH,EAAcb,EAAMmB,qBAAqBX,EAAOQ,SAChD,MACF,IAAK,YACHH,EAAcb,EAAMoB,mBAAmBZ,EAAOQ,SAC9C,MACF,IAAK,OACHH,EAAcb,EAAMqB,cAAcb,EAAOQ,SACzC,MACF,QACI,OAGHR,EAAOc,YACRtB,EAAMsB,WAAWd,EAAOQ,QAAQO,cAAgB,IAAIC,aAAahB,EAAOc,YAE1ET,EAAYY,QAAQjB,EAAOkB,MAExBlB,EAAOmB,SACRd,EAAYe,WAAWpB,EAAOmB,UAEjC,MAAAE,GAAAvB,EAAAwB,EAAAD,GAAA,QAAAvB,EAAAyB,IAED/B,EAAMgC,YAAYC,gBAIpB,IAAMC,EAAS1C,EAAUI,QAAQuC,KAAI,SAACC,GAAC,OAAKA,KAoD5C,OAlDGrD,EAAWO,OAAS,GACrB4C,EAAOrC,SAAQ,SAACG,GACTA,IAELA,EAAMgC,YAAYK,iCAAgC,SAACP,GACjDI,EACGI,QAAO,SAACF,GAAC,OAAKA,IAAMpC,KACpBH,SAAQ,SAACuC,GACRA,EAAEJ,YAAYR,aAAa,CACzBe,YAAavC,EAAMgC,YAAYQ,yBAGvCxC,EAAMgC,YAAYS,oCAAmC,SAACC,GAChDA,GACFR,EACGI,QAAO,SAACF,GAAC,OAAKA,IAAMpC,KACpBH,SAAQ,SAACuC,GACRA,EAAEJ,YAAYW,uBAAuB,CACnCC,KAAW,OAALF,QAAK,IAALA,OAAK,EAALA,EAAOE,KACbC,GAAS,OAALH,QAAK,IAALA,OAAK,EAALA,EAAOG,eA+BlB,WACLX,EAAOrC,SAAQ,SAACG,GACdA,EAAM8C,gBAIT,CAAE/D,EAAYK,EAAaI,IAI5BuD,IAAAC,cAAA,OAAKrD,IAAKT,GACPE,EAAY+C,KAAI,SAACxC,EAAKG,GAAC,OACtBiD,IAAAC,cAAA,OACErD,IAAKA,EACLsD,GAAE,sBAAAC,OAAwBpD,GAC1BqD,IAAG,sBAAAD,OAAwBpD,UCpIvCsD,IAASC,OACPN,IAAAC,cAACD,IAAMO,WAAU,KACfP,IAAAC,cAACO,oBAAiB,KAChBR,IAAAC,cAACQ,EAAiB,QAGtBC,SAASC,eAAe,W",
     "names": [
         "LightweightChartsMultiplePanes",
         "chartsData",
         "useRenderData",
         "args",
         "chartsContainerRef",
         "useRef",
@@ -15,23 +15,21 @@
         "chartRefs",
         "useEffect",
         "find",
         "ref",
         "current",
         "forEach",
         "i",
+        "_step",
         "chart",
         "createChart",
         "_objectSpread",
         "height",
         "width",
         "clientWidth",
-        "timeScale",
-        "fitContent",
-        "_step",
         "_iterator",
         "_createForOfIteratorHelper",
         "series",
         "s",
         "n",
         "done",
         "value",
@@ -45,17 +43,21 @@
         "addHistogramSeries",
         "addLineSeries",
         "priceScale",
         "priceScaleId",
         "applyOptions",
         "setData",
         "data",
+        "markers",
+        "setMarkers",
         "err",
         "e",
         "f",
+        "timeScale",
+        "fitContent",
         "charts",
         "map",
         "c",
         "subscribeVisibleTimeRangeChange",
         "filter",
         "rightOffset",
         "scrollPosition",
@@ -80,12 +82,12 @@
     ],
     "sourceRoot": "",
     "sources": [
         "LightweightCharts.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
-        "import { useRenderData } from \"streamlit-component-lib-react-hooks\"\nimport {\n  createChart,\n  IChartApi,\n} from \"lightweight-charts\"\nimport React, { useRef, useEffect } from \"react\"\n\nconst LightweightChartsMultiplePanes: React.VFC = () => {\n\n  // returns the renderData passed from Python\n  // { args: object, disabled: boolean, theme: object }\n  const renderData = useRenderData()\n  const chartsData = renderData.args[\"charts\"]\n\n  const chartsContainerRef = useRef<HTMLDivElement>(null)\n  const chartElRefs = Array(chartsData.length).fill(useRef<HTMLDivElement>(null))\n  const chartRefs = useRef<IChartApi[]>([])\n\n    useEffect(() => {\n      if (chartElRefs.find((ref) => !ref.current)) return;\n\n      chartElRefs.forEach((ref, i) => {\n        const chart = chartRefs.current[i] = createChart(\n          ref.current as HTMLDivElement,{\n            height: 300,\n            width: chartElRefs[i].current.clientWidth,\n            ...chartsData[i].chart,\n          }\n        );\n        \n        chart.timeScale().fitContent();\n\n        for (const series of chartsData[i].series){\n          \n          let chartSeries\n          switch(series.type) {\n            case 'Area':\n              chartSeries = chart.addAreaSeries(series.options)\n              break\n            case 'Bar':\n              chartSeries = chart.addBarSeries(series.options )\n              break\n            case 'Baseline':\n              chartSeries = chart.addBaselineSeries(series.options)\n              break\n            case 'Candlestick':\n              chartSeries = chart.addCandlestickSeries(series.options)\n              break\n            case 'Histogram':\n              chartSeries = chart.addHistogramSeries(series.options)\n              break\n            case 'Line':\n              chartSeries = chart.addLineSeries(series.options)\n              break\n            default:\n                return\n          }\n\n          if(series.priceScale)\n            chart.priceScale(series.options.priceScaleId || '').applyOptions(series.priceScale)\n\n          chartSeries.setData(series.data)\n        }\n        \n      })\n  \n      const charts = chartRefs.current.map((c) => c as IChartApi);\n      \n      if(chartsData.length > 1){ // sync charts\n        charts.forEach((chart) => {\n          if (!chart) return;\n\n          chart.timeScale().subscribeVisibleTimeRangeChange((e) => {\n            charts\n              .filter((c) => c !== chart)\n              .forEach((c) => {\n                c.timeScale().applyOptions({\n                  rightOffset: chart.timeScale().scrollPosition()\n                })\n              })\n          })\n          chart.timeScale().subscribeVisibleLogicalRangeChange((range) => {\n            if (range) {\n              charts\n                .filter((c) => c !== chart)\n                .forEach((c) => {\n                  c.timeScale().setVisibleLogicalRange({\n                    from: range?.from,\n                    to: range?.to\n      }) }) } }) }) }\n\n      // const handleResize = () => {\n      //   chart.applyOptions({ width: chartsContainerRef?.current?.clientWidth })\n      // }\n      // window.addEventListener('resize', handleResize)\n      return () => { // required because how useEffect() works\n        charts.forEach((chart) => {\n          chart.remove()\n        })\n      }\n\n    }, [ chartsData, chartElRefs, chartRefs])\n  \n    return (\n      <div ref={chartsContainerRef}>\n        {chartElRefs.map((ref, i) => (\n          <div\n            ref={ref}\n            id={`lightweight-charts-${i}`}\n            key={`lightweight-charts-${i}`}\n          />\n        ))}\n      </div>\n    )\n\n}\n\nexport default LightweightChartsMultiplePanes\n",
+        "import { useRenderData } from \"streamlit-component-lib-react-hooks\"\nimport {\n  createChart,\n  IChartApi,\n} from \"lightweight-charts\"\nimport React, { useRef, useEffect } from \"react\"\n\nconst LightweightChartsMultiplePanes: React.VFC = () => {\n\n  // returns the renderData passed from Python\n  // { args: object, disabled: boolean, theme: object }\n  const renderData = useRenderData()\n  const chartsData = renderData.args[\"charts\"]\n\n  const chartsContainerRef = useRef<HTMLDivElement>(null)\n  const chartElRefs = Array(chartsData.length).fill(useRef<HTMLDivElement>(null))\n  const chartRefs = useRef<IChartApi[]>([])\n\n    useEffect(() => {\n      if (chartElRefs.find((ref) => !ref.current)) return;\n\n      chartElRefs.forEach((ref, i) => {\n        const chart = chartRefs.current[i] = createChart(\n          ref.current as HTMLDivElement,{\n            height: 300,\n            width: chartElRefs[i].current.clientWidth,\n            ...chartsData[i].chart,\n          }\n        );\n\n        for (const series of chartsData[i].series){\n          \n          let chartSeries\n          switch(series.type) {\n            case 'Area':\n              chartSeries = chart.addAreaSeries(series.options)\n              break\n            case 'Bar':\n              chartSeries = chart.addBarSeries(series.options )\n              break\n            case 'Baseline':\n              chartSeries = chart.addBaselineSeries(series.options)\n              break\n            case 'Candlestick':\n              chartSeries = chart.addCandlestickSeries(series.options)\n              break\n            case 'Histogram':\n              chartSeries = chart.addHistogramSeries(series.options)\n              break\n            case 'Line':\n              chartSeries = chart.addLineSeries(series.options)\n              break\n            default:\n                return\n          }\n\n          if(series.priceScale)\n            chart.priceScale(series.options.priceScaleId || '').applyOptions(series.priceScale)\n\n          chartSeries.setData(series.data)\n\n          if(series.markers)\n            chartSeries.setMarkers(series.markers)\n\n        }\n\n        chart.timeScale().fitContent();\n\n      })\n  \n      const charts = chartRefs.current.map((c) => c as IChartApi);\n      \n      if(chartsData.length > 1){ // sync charts\n        charts.forEach((chart) => {\n          if (!chart) return;\n\n          chart.timeScale().subscribeVisibleTimeRangeChange((e) => {\n            charts\n              .filter((c) => c !== chart)\n              .forEach((c) => {\n                c.timeScale().applyOptions({\n                  rightOffset: chart.timeScale().scrollPosition()\n          }) }) })\n\n          chart.timeScale().subscribeVisibleLogicalRangeChange((range) => {\n            if (range) {\n              charts\n                .filter((c) => c !== chart)\n                .forEach((c) => {\n                  c.timeScale().setVisibleLogicalRange({\n                    from: range?.from,\n                    to: range?.to\n          }) }) } })\n\n          // chart.subscribeCrosshairMove((handler) => {\n          //   charts\n          //     .filter((c) => c !== chart)\n          //     .forEach((c) => {\n          //       // if (handler.time !== undefined) {\n          //       //   var xx = c.timeScale().timeToCoordinate(handler.time);\n          //       //   c.setCrossHairXY(xx,50,true);\n          //       // } else if (handler.point !== undefined){\n          //       //   c.setCrossHairXY(handler.point.x,10,false);\n          //       // }\n          //       // c.timeScale().applyOptions({\n          //       //   rightOffset: chart.timeScale().scrollPosition()\n          //       // })\n          //       console.log('handler',handler)\n          //       if (handler.time !== undefined) {\n          //         const xx = c.timeScale().timeToCoordinate(handler.time);\n          //         if(xx) c.timeScale().scrollToPosition(xx,true)\n          //         console.log('const xx',xx)\n          //       }\n          //     })\n          // })\n\n      }) }\n\n      // const handleResize = () => {\n      //   chart.applyOptions({ width: chartsContainerRef?.current?.clientWidth })\n      // }\n      // window.addEventListener('resize', handleResize)\n      return () => { // required because how useEffect() works\n        charts.forEach((chart) => {\n          chart.remove()\n        })\n      }\n\n    }, [ chartsData, chartElRefs, chartRefs])\n\n\n    return (\n      <div ref={chartsContainerRef}>\n        {chartElRefs.map((ref, i) => (\n          <div\n            ref={ref}\n            id={`lightweight-charts-${i}`}\n            key={`lightweight-charts-${i}`}\n          />\n        ))}\n      </div>\n    )\n\n}\n\nexport default LightweightChartsMultiplePanes\n",
         "import React from \"react\"\nimport ReactDOM from \"react-dom\"\nimport { StreamlitProvider } from \"streamlit-component-lib-react-hooks\"\nimport LightweightCharts from \"./LightweightCharts\"\n\nReactDOM.render(\n  <React.StrictMode>\n    <StreamlitProvider>\n      <LightweightCharts />\n    </StreamlitProvider>\n  </React.StrictMode>,\n  document.getElementById(\"root\")\n)\n"
     ],
     "version": 3
 }
```

### Comparing `streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/build/static/js/runtime-main.e0d8c599.js` & `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/runtime-main.e0d8c599.js`

 * *Files identical despite different names*

### Comparing `streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts/frontend/build/static/js/runtime-main.e0d8c599.js.map` & `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts/frontend/build/static/js/runtime-main.e0d8c599.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts.egg-info/PKG-INFO` & `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-lightweight-charts
-Version: 0.7.17
+Version: 0.7.18
 Summary: Wrapper for TradingView lightweight-charts
 Home-page: https://github.com/freyastreamlit/streamlit-lightweight-charts
 Author: Joe Rosa
 Author-email: joe.rosa@itpmngt.co.uk
 License: MIT
 Description: # streamlit-lightweight-charts
         Streamlit wrapper for performant Tradingview's Financial: `lightweight-charts`
@@ -17,14 +17,15 @@
         
         ### Versions
         - Version 0.7.12 - Added "markers" to series
         - Version 0.7.13 - Example of watermarks
         - Version 0.7.15 - Example using Pandas
         - Version 0.7.16 - Work examples on [Streamlit Cloud](https://share.streamlit.io/)
         - Version 0.7.17 - Added integration example for Data Toggling
+        - Version 0.7.18 - FIX: React build was not been commited
         
         ## How to install:
         ```
         python -m pip install streamlit-lightweight-charts
         ```
         
         ## How to use:
```

### Comparing `streamlit-lightweight-charts-0.7.17/streamlit_lightweight_charts.egg-info/SOURCES.txt` & `streamlit-lightweight-charts-0.7.18/streamlit_lightweight_charts.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 streamlit_lightweight_charts.egg-info/PKG-INFO
 streamlit_lightweight_charts.egg-info/SOURCES.txt
 streamlit_lightweight_charts.egg-info/dependency_links.txt
 streamlit_lightweight_charts.egg-info/requires.txt
 streamlit_lightweight_charts.egg-info/top_level.txt
 streamlit_lightweight_charts/frontend/build/asset-manifest.json
 streamlit_lightweight_charts/frontend/build/index.html
-streamlit_lightweight_charts/frontend/build/precache-manifest.e6bd8d0d7ff31e7ed0c54de396b38e6a.js
+streamlit_lightweight_charts/frontend/build/precache-manifest.e348f70e7319498a2e6b3a0c95da5ac1.js
 streamlit_lightweight_charts/frontend/build/service-worker.js
 streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js
 streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js.LICENSE.txt
 streamlit_lightweight_charts/frontend/build/static/js/2.70acfc76.chunk.js.map
-streamlit_lightweight_charts/frontend/build/static/js/main.57993593.chunk.js
-streamlit_lightweight_charts/frontend/build/static/js/main.57993593.chunk.js.map
+streamlit_lightweight_charts/frontend/build/static/js/main.509cd3c1.chunk.js
+streamlit_lightweight_charts/frontend/build/static/js/main.509cd3c1.chunk.js.map
 streamlit_lightweight_charts/frontend/build/static/js/runtime-main.e0d8c599.js
 streamlit_lightweight_charts/frontend/build/static/js/runtime-main.e0d8c599.js.map
```

