# Comparing `tmp/fitsmap-0.9.0.tar.gz` & `tmp/fitsmap-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fitsmap-0.9.0.tar", last modified: Tue Apr 12 10:09:05 2022, max compression
+gzip compressed data, was "dist/fitsmap-0.9.1.tar", last modified: Tue May 10 17:41:31 2022, max compression
```

## Comparing `fitsmap-0.9.0.tar` & `fitsmap-0.9.1.tar`

### file list

```diff
@@ -1,43 +1,42 @@
-drwxrwxr-x   0 ryanhausen  (1000) ryanhausen  (1000)        0 2022-04-12 10:09:05.000000 fitsmap-0.9.0/
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)      485 2022-04-12 10:08:42.000000 fitsmap-0.9.0/MANIFEST.in
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)    13174 2022-04-12 10:09:05.000000 fitsmap-0.9.0/PKG-INFO
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)    10065 2022-04-12 09:31:12.000000 fitsmap-0.9.0/README.rst
-drwxrwxr-x   0 ryanhausen  (1000) ryanhausen  (1000)        0 2022-04-12 10:09:05.000000 fitsmap-0.9.0/fitsmap/
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)        0 2021-07-18 22:09:25.000000 fitsmap-0.9.0/fitsmap/__init__.py
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     5646 2021-11-29 23:42:53.000000 fitsmap-0.9.0/fitsmap/__main__.py
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)       12 2022-04-12 09:31:52.000000 fitsmap-0.9.0/fitsmap/__version__.py
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)    17768 2022-04-12 09:32:17.000000 fitsmap-0.9.0/fitsmap/cartographer.py
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)    40915 2022-04-12 09:32:18.000000 fitsmap-0.9.0/fitsmap/convert.py
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     8152 2021-11-29 23:42:53.000000 fitsmap-0.9.0/fitsmap/kdbush.py
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)    17630 2021-11-29 23:42:53.000000 fitsmap-0.9.0/fitsmap/supercluster.py
-drwxrwxr-x   0 ryanhausen  (1000) ryanhausen  (1000)        0 2022-04-12 10:09:05.000000 fitsmap-0.9.0/fitsmap/support/
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     1604 2021-11-29 23:42:53.000000 fitsmap-0.9.0/fitsmap/support/MarkerCluster.Default.css
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     1279 2022-04-12 09:31:12.000000 fitsmap-0.9.0/fitsmap/support/MarkerCluster.Default.min.css
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)      872 2021-07-18 22:09:25.000000 fitsmap-0.9.0/fitsmap/support/MarkerCluster.css
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)      688 2022-04-12 09:31:12.000000 fitsmap-0.9.0/fitsmap/support/MarkerCluster.min.css
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)       33 2022-04-12 09:31:12.000000 fitsmap-0.9.0/fitsmap/support/MarkerPopup.min.css
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)      930 2021-07-18 22:09:25.000000 fitsmap-0.9.0/fitsmap/support/TileNearestNeighbor.css
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)      508 2022-04-12 09:31:12.000000 fitsmap-0.9.0/fitsmap/support/TileNearestNeighbor.min.css
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)      712 2022-04-12 09:31:12.000000 fitsmap-0.9.0/fitsmap/support/customSearch.min.js
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     1166 2022-04-12 09:31:12.000000 fitsmap-0.9.0/fitsmap/support/favicon.ico
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     3157 2021-07-18 22:09:25.000000 fitsmap-0.9.0/fitsmap/support/l.ellipse.min.js
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     7788 2022-04-12 09:31:12.000000 fitsmap-0.9.0/fitsmap/support/loading-logo.svg
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     2862 2022-04-12 09:31:12.000000 fitsmap-0.9.0/fitsmap/support/tiledMarkers.min.js
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     2683 2021-11-29 23:42:53.000000 fitsmap-0.9.0/fitsmap/support/urlCoords.js.tmp
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     3468 2021-11-29 23:42:53.000000 fitsmap-0.9.0/fitsmap/support/vector-tile.min.js
-drwxrwxr-x   0 ryanhausen  (1000) ryanhausen  (1000)        0 2022-04-12 10:09:05.000000 fitsmap-0.9.0/fitsmap/tests/
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)        0 2021-07-18 22:09:25.000000 fitsmap-0.9.0/fitsmap/tests/__init__.py
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     4882 2022-04-12 09:31:12.000000 fitsmap-0.9.0/fitsmap/tests/helpers.py
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)    16414 2022-04-12 09:32:17.000000 fitsmap-0.9.0/fitsmap/tests/test_cartographer.py
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)    22162 2022-04-12 09:52:46.000000 fitsmap-0.9.0/fitsmap/tests/test_convert.py
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     3080 2022-04-12 09:31:12.000000 fitsmap-0.9.0/fitsmap/tests/test_utils.py
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     3925 2021-12-20 02:12:03.000000 fitsmap-0.9.0/fitsmap/utils.py
-drwxrwxr-x   0 ryanhausen  (1000) ryanhausen  (1000)        0 2022-04-12 10:09:05.000000 fitsmap-0.9.0/fitsmap.egg-info/
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)    13174 2022-04-12 10:09:05.000000 fitsmap-0.9.0/fitsmap.egg-info/PKG-INFO
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     1042 2022-04-12 10:09:05.000000 fitsmap-0.9.0/fitsmap.egg-info/SOURCES.txt
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)        1 2022-04-12 10:09:05.000000 fitsmap-0.9.0/fitsmap.egg-info/dependency_links.txt
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)       50 2022-04-12 10:09:05.000000 fitsmap-0.9.0/fitsmap.egg-info/entry_points.txt
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)       99 2022-04-12 10:09:05.000000 fitsmap-0.9.0/fitsmap.egg-info/requires.txt
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)        8 2022-04-12 10:09:05.000000 fitsmap-0.9.0/fitsmap.egg-info/top_level.txt
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)       38 2022-04-12 10:09:05.000000 fitsmap-0.9.0/setup.cfg
--rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     2591 2022-04-12 09:31:12.000000 fitsmap-0.9.0/setup.py
+drwxrwxr-x   0 ryanhausen  (1000) ryanhausen  (1000)        0 2022-05-10 17:41:31.000000 fitsmap-0.9.1/
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)      485 2022-05-10 15:55:29.000000 fitsmap-0.9.1/MANIFEST.in
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)    13174 2022-05-10 17:41:31.000000 fitsmap-0.9.1/PKG-INFO
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)    10065 2022-05-10 15:55:29.000000 fitsmap-0.9.1/README.rst
+drwxrwxr-x   0 ryanhausen  (1000) ryanhausen  (1000)        0 2022-05-10 17:41:31.000000 fitsmap-0.9.1/fitsmap/
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)        0 2019-01-11 00:27:22.000000 fitsmap-0.9.1/fitsmap/__init__.py
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     5646 2022-05-10 15:55:29.000000 fitsmap-0.9.1/fitsmap/__main__.py
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)       12 2022-05-10 17:32:53.000000 fitsmap-0.9.1/fitsmap/__version__.py
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)    17862 2022-05-10 16:51:58.000000 fitsmap-0.9.1/fitsmap/cartographer.py
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)    40915 2022-05-10 15:55:29.000000 fitsmap-0.9.1/fitsmap/convert.py
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     8152 2022-05-10 15:55:29.000000 fitsmap-0.9.1/fitsmap/kdbush.py
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)    17630 2022-05-10 15:55:29.000000 fitsmap-0.9.1/fitsmap/supercluster.py
+drwxrwxr-x   0 ryanhausen  (1000) ryanhausen  (1000)        0 2022-05-10 17:41:31.000000 fitsmap-0.9.1/fitsmap/support/
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     1604 2022-05-10 15:55:29.000000 fitsmap-0.9.1/fitsmap/support/MarkerCluster.Default.css
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     1279 2022-05-10 15:55:29.000000 fitsmap-0.9.1/fitsmap/support/MarkerCluster.Default.min.css
+-rw-r--r--   0 ryanhausen  (1000) ryanhausen  (1000)      872 2019-11-18 21:55:06.000000 fitsmap-0.9.1/fitsmap/support/MarkerCluster.css
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)      688 2022-05-10 15:55:29.000000 fitsmap-0.9.1/fitsmap/support/MarkerCluster.min.css
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)       33 2022-05-10 15:55:29.000000 fitsmap-0.9.1/fitsmap/support/MarkerPopup.min.css
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)      508 2022-05-10 15:55:29.000000 fitsmap-0.9.1/fitsmap/support/TileNearestNeighbor.min.css
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)      712 2022-05-10 15:55:29.000000 fitsmap-0.9.1/fitsmap/support/customSearch.min.js
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     1166 2022-05-10 15:55:29.000000 fitsmap-0.9.1/fitsmap/support/favicon.ico
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     3157 2022-05-10 15:55:29.000000 fitsmap-0.9.1/fitsmap/support/l.ellipse.min.js
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     7788 2022-05-10 15:55:29.000000 fitsmap-0.9.1/fitsmap/support/loading-logo.svg
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     2862 2022-05-10 15:55:29.000000 fitsmap-0.9.1/fitsmap/support/tiledMarkers.min.js
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     2683 2022-05-10 15:55:29.000000 fitsmap-0.9.1/fitsmap/support/urlCoords.js.tmp
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     3468 2022-05-10 15:55:29.000000 fitsmap-0.9.1/fitsmap/support/vector-tile.min.js
+drwxrwxr-x   0 ryanhausen  (1000) ryanhausen  (1000)        0 2022-05-10 17:41:31.000000 fitsmap-0.9.1/fitsmap/tests/
+-rw-r--r--   0 ryanhausen  (1000) ryanhausen  (1000)        0 2020-01-14 21:13:11.000000 fitsmap-0.9.1/fitsmap/tests/__init__.py
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     4882 2022-05-10 15:55:29.000000 fitsmap-0.9.1/fitsmap/tests/helpers.py
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)    16303 2022-05-10 16:59:53.000000 fitsmap-0.9.1/fitsmap/tests/test_cartographer.py
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)    23409 2022-05-10 17:03:57.000000 fitsmap-0.9.1/fitsmap/tests/test_convert.py
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     3080 2022-05-10 15:55:29.000000 fitsmap-0.9.1/fitsmap/tests/test_utils.py
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     3925 2022-05-10 15:55:29.000000 fitsmap-0.9.1/fitsmap/utils.py
+drwxrwxr-x   0 ryanhausen  (1000) ryanhausen  (1000)        0 2022-05-10 17:41:31.000000 fitsmap-0.9.1/fitsmap.egg-info/
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)    13174 2022-05-10 17:41:31.000000 fitsmap-0.9.1/fitsmap.egg-info/PKG-INFO
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     1002 2022-05-10 17:41:31.000000 fitsmap-0.9.1/fitsmap.egg-info/SOURCES.txt
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)        1 2022-05-10 17:41:31.000000 fitsmap-0.9.1/fitsmap.egg-info/dependency_links.txt
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)       50 2022-05-10 17:41:31.000000 fitsmap-0.9.1/fitsmap.egg-info/entry_points.txt
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)       99 2022-05-10 17:41:31.000000 fitsmap-0.9.1/fitsmap.egg-info/requires.txt
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)        8 2022-05-10 17:41:31.000000 fitsmap-0.9.1/fitsmap.egg-info/top_level.txt
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)       38 2022-05-10 17:41:31.000000 fitsmap-0.9.1/setup.cfg
+-rw-rw-r--   0 ryanhausen  (1000) ryanhausen  (1000)     2591 2022-05-10 15:55:29.000000 fitsmap-0.9.1/setup.py
```

### Comparing `fitsmap-0.9.0/PKG-INFO` & `fitsmap-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: fitsmap
-Version: 0.9.0
+Version: 0.9.1
 Summary: Turn fits files/catalogs into a leafletjs map
 Home-page: https://github.com/ryanhausen/fitsmap
 Author: Ryan Hausen
 Author-email: rhausen@ucsc.edu
 License: MIT
 Description: .. Variables to ensure the hyperlink gets used
         .. |convert| replace:: `fitsmap.convert <https://fitsmap.readthedocs.io/en/latest/source/fitsmap.html#module-fitsmap.convert>`__
```

### Comparing `fitsmap-0.9.0/README.rst` & `fitsmap-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `fitsmap-0.9.0/fitsmap/__main__.py` & `fitsmap-0.9.1/fitsmap/__main__.py`

 * *Files identical despite different names*

### Comparing `fitsmap-0.9.0/fitsmap/cartographer.py` & `fitsmap-0.9.1/fitsmap/cartographer.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     with open(os.path.join(out_dir, "js", "index.js"), "w") as f:
         f.write(
             build_index_js(img_layer_dicts, cat_layer_dicts, rows_per_column, max_xy)
         )
     # generated javascript =====================================================
 
     # HTML file contents =======================================================
-    extra_js = build_conditional_js(out_dir) if cat_layer_dicts else ""
+    extra_js = build_conditional_js(out_dir, bool(cat_layer_dicts))
 
     extra_css = build_conditional_css(out_dir)
 
     move_support_images(out_dir)
 
     with open(os.path.join(out_dir, "index.html"), "w") as f:
         f.write(build_html(title, extra_js, extra_css))
@@ -265,15 +265,15 @@
     )
 
     local_css = list(map(lambda f: f"css/{f}", local_css_files))
 
     return "\n".join(map(lambda s: css_string.format(s), [search_css] + local_css))
 
 
-def build_conditional_js(out_dir: str) -> str:
+def build_conditional_js(out_dir: str, include_markerjs:bool) -> str:
 
     support_dir = os.path.join(os.path.dirname(__file__), "support")
     out_js_dir = os.path.join(out_dir, "js")
 
     local_js_files = list(
         sorted(filter(lambda f: f.endswith(".min.js"), os.listdir(support_dir)))
     )
@@ -290,32 +290,31 @@
         )
     )
 
     # some files have to be loaded before index.js, so that index.js can
     # sucessfully run. Other files get placed after index.js so that the map
     # can load first and then those will load in the background
     pre_index_files = [
-        "https://cdnjs.cloudflare.com/ajax/libs/leaflet/1.7.1/leaflet.min.js",
-        "https://cdnjs.cloudflare.com/ajax/libs/leaflet-search/3.0.2/leaflet-search.src.min.js",
-        "js/customSearch.min.js",
-        "js/tiledMarkers.min.js",
+        "https://cdnjs.cloudflare.com/ajax/libs/leaflet-search/3.0.2/leaflet-search.src.min.js" * include_markerjs,
+        "js/customSearch.min.js" * include_markerjs,
+        "js/tiledMarkers.min.js" * include_markerjs,
         "js/urlCoords.js",
         "js/index.js",
     ]
 
     post_index_files = [
-        "https://unpkg.com/cbor-web@8.1.0/dist/cbor.js",
-        "https://unpkg.com/pbf@3.0.5/dist/pbf.js",
-        "js/l.ellipse.min.js",
-        "js/vector-tile.min.js",
+        "https://unpkg.com/cbor-web@8.1.0/dist/cbor.js" * include_markerjs,
+        "https://unpkg.com/pbf@3.0.5/dist/pbf.js" * include_markerjs,
+        "js/l.ellipse.min.js" * include_markerjs,
+        "js/vector-tile.min.js" * include_markerjs,
     ]
 
     js_string = "    <script defer src='{}'></script>"
     js_tags = list(
-        map(lambda s: js_string.format(s), pre_index_files + post_index_files)
+        map(lambda s: js_string.format(s), filter(lambda x: x, pre_index_files + post_index_files))
     )
 
     return "\n".join(js_tags)
 
 
 def leaflet_layer_control_declaration(
     img_layer_dicts: List[Dict], cat_layer_dicts: List[Dict],
```

### Comparing `fitsmap-0.9.0/fitsmap/convert.py` & `fitsmap-0.9.1/fitsmap/convert.py`

 * *Files identical despite different names*

### Comparing `fitsmap-0.9.0/fitsmap/kdbush.py` & `fitsmap-0.9.1/fitsmap/kdbush.py`

 * *Files identical despite different names*

### Comparing `fitsmap-0.9.0/fitsmap/supercluster.py` & `fitsmap-0.9.1/fitsmap/supercluster.py`

 * *Files identical despite different names*

### Comparing `fitsmap-0.9.0/fitsmap/support/MarkerCluster.Default.css` & `fitsmap-0.9.1/fitsmap/support/MarkerCluster.Default.css`

 * *Files identical despite different names*

### Comparing `fitsmap-0.9.0/fitsmap/support/MarkerCluster.Default.min.css` & `fitsmap-0.9.1/fitsmap/support/MarkerCluster.Default.min.css`

 * *Files identical despite different names*

### Comparing `fitsmap-0.9.0/fitsmap/support/MarkerCluster.css` & `fitsmap-0.9.1/fitsmap/support/MarkerCluster.css`

 * *Files identical despite different names*

### Comparing `fitsmap-0.9.0/fitsmap/support/MarkerCluster.min.css` & `fitsmap-0.9.1/fitsmap/support/MarkerCluster.min.css`

 * *Files identical despite different names*

### Comparing `fitsmap-0.9.0/fitsmap/support/customSearch.min.js` & `fitsmap-0.9.1/fitsmap/support/customSearch.min.js`

 * *Files identical despite different names*

### Comparing `fitsmap-0.9.0/fitsmap/support/favicon.ico` & `fitsmap-0.9.1/fitsmap/support/favicon.ico`

 * *Files identical despite different names*

### Comparing `fitsmap-0.9.0/fitsmap/support/l.ellipse.min.js` & `fitsmap-0.9.1/fitsmap/support/l.ellipse.min.js`

 * *Files identical despite different names*

### Comparing `fitsmap-0.9.0/fitsmap/support/loading-logo.svg` & `fitsmap-0.9.1/fitsmap/support/loading-logo.svg`

 * *Files identical despite different names*

### Comparing `fitsmap-0.9.0/fitsmap/support/tiledMarkers.min.js` & `fitsmap-0.9.1/fitsmap/support/tiledMarkers.min.js`

 * *Files identical despite different names*

### Comparing `fitsmap-0.9.0/fitsmap/support/urlCoords.js.tmp` & `fitsmap-0.9.1/fitsmap/support/urlCoords.js.tmp`

 * *Files identical despite different names*

### Comparing `fitsmap-0.9.0/fitsmap/support/vector-tile.min.js` & `fitsmap-0.9.1/fitsmap/support/vector-tile.min.js`

 * *Files identical despite different names*

### Comparing `fitsmap-0.9.0/fitsmap/tests/helpers.py` & `fitsmap-0.9.1/fitsmap/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `fitsmap-0.9.0/fitsmap/tests/test_cartographer.py` & `fitsmap-0.9.1/fitsmap/tests/test_cartographer.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,19 +314,18 @@
 @pytest.mark.unit
 @pytest.mark.cartographer
 def test_build_conditional_js():
     """test cartographer.build_conditional_js"""
 
     helpers.setup()
 
-    acutal_js = c.build_conditional_js(helpers.TEST_PATH)
+    acutal_js = c.build_conditional_js(helpers.TEST_PATH, True)
 
     expected_js = "\n".join(
         [
-            "    <script defer src='https://cdnjs.cloudflare.com/ajax/libs/leaflet/1.7.1/leaflet.min.js'></script>",
             "    <script defer src='https://cdnjs.cloudflare.com/ajax/libs/leaflet-search/3.0.2/leaflet-search.src.min.js'></script>",
             "    <script defer src='js/customSearch.min.js'></script>",
             "    <script defer src='js/tiledMarkers.min.js'></script>",
             "    <script defer src='js/urlCoords.js'></script>",
             "    <script defer src='js/index.js'></script>",
             "    <script defer src='https://unpkg.com/cbor-web@8.1.0/dist/cbor.js'></script>",
             "    <script defer src='https://unpkg.com/pbf@3.0.5/dist/pbf.js'></script>",
```

### Comparing `fitsmap-0.9.0/fitsmap/tests/test_convert.py` & `fitsmap-0.9.1/fitsmap/tests/test_convert.py`

 * *Files 3% similar despite different names*

```diff
@@ -813,7 +813,54 @@
 
     dirs_match = helpers.compare_file_directories(expected_dir, actual_dir)
 
     helpers.tear_down()
     helpers.enable_tqdm()
 
     assert dirs_match
+
+
+@pytest.mark.integration
+@pytest.mark.convert
+@pytest.mark.filterwarnings("ignore:.*:astropy.io.fits.verify.VerifyWarning")
+def test_dir_to_map_no_markers():
+    """Integration test for making files into map"""
+    helpers.disbale_tqdm()
+    helpers.setup(with_data=True)
+
+    with_path = lambda f: os.path.join(helpers.TEST_PATH, f)
+    out_dir = with_path("test_web")
+    in_dir = with_path("test_web_in")
+    if not os.path.exists(in_dir):
+        os.mkdir(in_dir)
+
+    files = [
+        "test_tiling_image.jpg",
+    ]
+
+    for f in files:
+        shutil.copy(with_path(f), os.path.join(in_dir, f))
+
+    expected_dir = with_path("expected_test_web_no_marker")
+
+    # inject current version in to test_index.html
+    version = helpers.get_version()
+    raw_path = os.path.join(expected_dir, "index.html")
+    with open(raw_path, "r") as f:
+        converted = list(map(lambda l: l.replace("VERSION", version), f.readlines()))
+
+    with open(raw_path, "w") as f:
+        f.writelines(converted)
+
+    convert.dir_to_map(
+        in_dir,
+        out_dir=out_dir,
+    )
+
+    actual_dir = out_dir
+
+    dirs_match = helpers.compare_file_directories(expected_dir, actual_dir)
+
+    helpers.tear_down()
+    helpers.enable_tqdm()
+
+    assert dirs_match
```

### Comparing `fitsmap-0.9.0/fitsmap/tests/test_utils.py` & `fitsmap-0.9.1/fitsmap/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fitsmap-0.9.0/fitsmap/utils.py` & `fitsmap-0.9.1/fitsmap/utils.py`

 * *Files identical despite different names*

### Comparing `fitsmap-0.9.0/fitsmap.egg-info/PKG-INFO` & `fitsmap-0.9.1/fitsmap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: fitsmap
-Version: 0.9.0
+Version: 0.9.1
 Summary: Turn fits files/catalogs into a leafletjs map
 Home-page: https://github.com/ryanhausen/fitsmap
 Author: Ryan Hausen
 Author-email: rhausen@ucsc.edu
 License: MIT
 Description: .. Variables to ensure the hyperlink gets used
         .. |convert| replace:: `fitsmap.convert <https://fitsmap.readthedocs.io/en/latest/source/fitsmap.html#module-fitsmap.convert>`__
```

### Comparing `fitsmap-0.9.0/fitsmap.egg-info/SOURCES.txt` & `fitsmap-0.9.1/fitsmap.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 fitsmap.egg-info/requires.txt
 fitsmap.egg-info/top_level.txt
 fitsmap/support/MarkerCluster.Default.css
 fitsmap/support/MarkerCluster.Default.min.css
 fitsmap/support/MarkerCluster.css
 fitsmap/support/MarkerCluster.min.css
 fitsmap/support/MarkerPopup.min.css
-fitsmap/support/TileNearestNeighbor.css
 fitsmap/support/TileNearestNeighbor.min.css
 fitsmap/support/customSearch.min.js
 fitsmap/support/favicon.ico
 fitsmap/support/l.ellipse.min.js
 fitsmap/support/loading-logo.svg
 fitsmap/support/tiledMarkers.min.js
 fitsmap/support/urlCoords.js.tmp
```

### Comparing `fitsmap-0.9.0/setup.py` & `fitsmap-0.9.1/setup.py`

 * *Files identical despite different names*

