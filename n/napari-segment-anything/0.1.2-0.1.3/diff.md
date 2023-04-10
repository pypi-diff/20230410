# Comparing `tmp/napari-segment-anything-0.1.2.tar.gz` & `tmp/napari-segment-anything-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-segment-anything-0.1.2.tar", last modified: Sat Apr  8 00:23:09 2023, max compression
+gzip compressed data, was "napari-segment-anything-0.1.3.tar", last modified: Mon Apr 10 18:27:40 2023, max compression
```

## Comparing `napari-segment-anything-0.1.2.tar` & `napari-segment-anything-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-08 00:23:09.720000 napari-segment-anything-0.1.2/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)    11358 2023-04-05 19:05:13.000000 napari-segment-anything-0.1.2/LICENSE
--rw-rw-r--   0 jordao    (1000) jordao    (1000)       96 2023-04-05 19:05:13.000000 napari-segment-anything-0.1.2/MANIFEST.in
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4805 2023-04-08 00:23:09.720000 napari-segment-anything-0.1.2/PKG-INFO
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3489 2023-04-06 18:38:18.000000 napari-segment-anything-0.1.2/README.md
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      180 2023-04-05 19:05:13.000000 napari-segment-anything-0.1.2/pyproject.toml
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1829 2023-04-08 00:23:09.720000 napari-segment-anything-0.1.2/setup.cfg
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-08 00:23:09.720000 napari-segment-anything-0.1.2/src/
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-08 00:23:09.720000 napari-segment-anything-0.1.2/src/napari_segment_anything/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      102 2023-04-08 00:22:57.000000 napari-segment-anything-0.1.2/src/napari_segment_anything/__init__.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-08 00:23:09.720000 napari-segment-anything-0.1.2/src/napari_segment_anything/_tests/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2023-04-05 19:05:13.000000 napari-segment-anything-0.1.2/src/napari_segment_anything/_tests/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2540 2023-04-08 00:22:57.000000 napari-segment-anything-0.1.2/src/napari_segment_anything/_tests/test_widget.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     7283 2023-04-08 00:22:57.000000 napari-segment-anything-0.1.2/src/napari_segment_anything/_widget.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      320 2023-04-05 20:29:57.000000 napari-segment-anything-0.1.2/src/napari_segment_anything/napari.yaml
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1806 2023-04-06 23:34:27.000000 napari-segment-anything-0.1.2/src/napari_segment_anything/utils.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-08 00:23:09.720000 napari-segment-anything-0.1.2/src/napari_segment_anything.egg-info/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4805 2023-04-08 00:23:09.000000 napari-segment-anything-0.1.2/src/napari_segment_anything.egg-info/PKG-INFO
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      615 2023-04-08 00:23:09.000000 napari-segment-anything-0.1.2/src/napari_segment_anything.egg-info/SOURCES.txt
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        1 2023-04-08 00:23:09.000000 napari-segment-anything-0.1.2/src/napari_segment_anything.egg-info/dependency_links.txt
--rw-rw-r--   0 jordao    (1000) jordao    (1000)       80 2023-04-08 00:23:09.000000 napari-segment-anything-0.1.2/src/napari_segment_anything.egg-info/entry_points.txt
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      111 2023-04-08 00:23:09.000000 napari-segment-anything-0.1.2/src/napari_segment_anything.egg-info/requires.txt
--rw-rw-r--   0 jordao    (1000) jordao    (1000)       24 2023-04-08 00:23:09.000000 napari-segment-anything-0.1.2/src/napari_segment_anything.egg-info/top_level.txt
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:27:40.828027 napari-segment-anything-0.1.3/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)    11358 2023-04-05 19:05:13.000000 napari-segment-anything-0.1.3/LICENSE
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)       96 2023-04-05 19:05:13.000000 napari-segment-anything-0.1.3/MANIFEST.in
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     5504 2023-04-10 18:27:40.828027 napari-segment-anything-0.1.3/PKG-INFO
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     4188 2023-04-10 15:53:01.000000 napari-segment-anything-0.1.3/README.md
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      180 2023-04-05 19:05:13.000000 napari-segment-anything-0.1.3/pyproject.toml
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1829 2023-04-10 18:27:40.828027 napari-segment-anything-0.1.3/setup.cfg
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:27:40.828027 napari-segment-anything-0.1.3/src/
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:27:40.828027 napari-segment-anything-0.1.3/src/napari_segment_anything/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      102 2023-04-10 18:26:52.000000 napari-segment-anything-0.1.3/src/napari_segment_anything/__init__.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:27:40.828027 napari-segment-anything-0.1.3/src/napari_segment_anything/_tests/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2023-04-05 19:05:13.000000 napari-segment-anything-0.1.3/src/napari_segment_anything/_tests/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2540 2023-04-08 00:22:57.000000 napari-segment-anything-0.1.3/src/napari_segment_anything/_tests/test_widget.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     7283 2023-04-08 00:22:57.000000 napari-segment-anything-0.1.3/src/napari_segment_anything/_widget.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      320 2023-04-05 20:29:57.000000 napari-segment-anything-0.1.3/src/napari_segment_anything/napari.yaml
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2157 2023-04-10 17:47:09.000000 napari-segment-anything-0.1.3/src/napari_segment_anything/utils.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:27:40.828027 napari-segment-anything-0.1.3/src/napari_segment_anything.egg-info/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     5504 2023-04-10 18:27:40.000000 napari-segment-anything-0.1.3/src/napari_segment_anything.egg-info/PKG-INFO
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      615 2023-04-10 18:27:40.000000 napari-segment-anything-0.1.3/src/napari_segment_anything.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        1 2023-04-10 18:27:40.000000 napari-segment-anything-0.1.3/src/napari_segment_anything.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)       80 2023-04-10 18:27:40.000000 napari-segment-anything-0.1.3/src/napari_segment_anything.egg-info/entry_points.txt
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      111 2023-04-10 18:27:40.000000 napari-segment-anything-0.1.3/src/napari_segment_anything.egg-info/requires.txt
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)       24 2023-04-10 18:27:40.000000 napari-segment-anything-0.1.3/src/napari_segment_anything.egg-info/top_level.txt
```

### Comparing `napari-segment-anything-0.1.2/LICENSE` & `napari-segment-anything-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-segment-anything-0.1.2/PKG-INFO` & `napari-segment-anything-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-segment-anything
-Version: 0.1.2
+Version: 0.1.3
 Summary: Napari plugin of Segment Anything Model (SAM)
 Home-page: https://github.com/jookuma/napari-segment-anything
 Author: Jordao Bragantini
 Author-email: jordao.bragantini@czbiohub.org
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/jookuma/napari-segment-anything/issues
 Project-URL: Documentation, https://github.com/jookuma/napari-segment-anything#README.md
@@ -58,18 +58,38 @@
 
 We recommend installing the latest development version because this package is being developed:
 
 ```bash
 pip install git+https://github.com/jookuma/napari-segment-anything.git
 ```
 
-IMPORTANT: `napari` won't work if you don't have `pyqt5` or `pyside2` installed.
+**IMPORTANT**: `napari` won't work if you don't have `pyqt5` or `pyside2` installed.
 
 ## Instructions
 
+### Opening napari-segment-anything
+
+This software is napari plugin, so once you have napari installed you can open it using the command line:
+
+```bash
+napari <your image path> -w napari-segment-anything 'Segment Anything'
+```
+
+I noticed that sometimes napari fails to load the plugin widget from the command line, go to step 2 from below to load it.
+
+If you prefer the user interface you need to:
+
+1) Drag and drop your image into napari to load it;
+2) Go to the "Plugins" file menu in the upper right corner and select the "Segment Anything" plugin.
+3) Follow the instructions below for usage.
+
+**IMPORTANT**: If you get an error make sure you have `pyqt5` or `pyside2` installed.
+
+### Usage
+
 - Interactions are done on the "SAM points" and "SAM box" layers using the existing functionalities of napari. Only rectangle shapes trigger the network prediction.
 - For points supervision, left clicks are positive cues (object) and right clicks are negative (background).
 - Press the "Confirm Annot." button (or the "C" key) to propagate the current segmentation mask to the label image.
 - Use the napari labels layer features to delete or edit already confirmed labels.
 
 ## Contributing
```

### Comparing `napari-segment-anything-0.1.2/README.md` & `napari-segment-anything-0.1.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -29,18 +29,38 @@
 
 We recommend installing the latest development version because this package is being developed:
 
 ```bash
 pip install git+https://github.com/jookuma/napari-segment-anything.git
 ```
 
-IMPORTANT: `napari` won't work if you don't have `pyqt5` or `pyside2` installed.
+**IMPORTANT**: `napari` won't work if you don't have `pyqt5` or `pyside2` installed.
 
 ## Instructions
 
+### Opening napari-segment-anything
+
+This software is napari plugin, so once you have napari installed you can open it using the command line:
+
+```bash
+napari <your image path> -w napari-segment-anything 'Segment Anything'
+```
+
+I noticed that sometimes napari fails to load the plugin widget from the command line, go to step 2 from below to load it.
+
+If you prefer the user interface you need to:
+
+1) Drag and drop your image into napari to load it;
+2) Go to the "Plugins" file menu in the upper right corner and select the "Segment Anything" plugin.
+3) Follow the instructions below for usage.
+
+**IMPORTANT**: If you get an error make sure you have `pyqt5` or `pyside2` installed.
+
+### Usage
+
 - Interactions are done on the "SAM points" and "SAM box" layers using the existing functionalities of napari. Only rectangle shapes trigger the network prediction.
 - For points supervision, left clicks are positive cues (object) and right clicks are negative (background).
 - Press the "Confirm Annot." button (or the "C" key) to propagate the current segmentation mask to the label image.
 - Use the napari labels layer features to delete or edit already confirmed labels.
 
 ## Contributing
```

### Comparing `napari-segment-anything-0.1.2/setup.cfg` & `napari-segment-anything-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-segment-anything-0.1.2/src/napari_segment_anything/_tests/test_widget.py` & `napari-segment-anything-0.1.3/src/napari_segment_anything/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-segment-anything-0.1.2/src/napari_segment_anything/_widget.py` & `napari-segment-anything-0.1.3/src/napari_segment_anything/_widget.py`

 * *Files identical despite different names*

### Comparing `napari-segment-anything-0.1.2/src/napari_segment_anything/utils.py` & `napari-segment-anything-0.1.3/src/napari_segment_anything/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,69 @@
 import urllib.request
 import warnings
 from pathlib import Path
 from typing import Optional
 
+import toolz as tz
+from napari.utils import progress
+
 SAM_WEIGHTS_URL = {
     "default": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth",
     "vit_h": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth",
     "vit_l": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_l_0b3195.pth",
     "vit_b": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_b_01ec64.pth",
 }
 
 
-def _report_hook(block_num: int, block_size: int, total_size: int) -> None:
+@tz.curry
+def _report_hook(
+    block_num: int,
+    block_size: int,
+    total_size: int,
+    pbr: "progress" = None,
+) -> None:
     downloaded = block_num * block_size
     percent = downloaded * 100 / total_size
     downloaded_mb = downloaded / 1024 / 1024
     total_size_mb = total_size / 1024 / 1024
+    increment = int(percent) - pbr.n
+    if increment > 1:  # faster than increment at every iteration
+        pbr.update(increment)
     print(
         f"Download progress: {percent:.1f}% ({downloaded_mb:.1f}/{total_size_mb:.1f} MB)",
         end="\r",
     )
 
 
+def download_weights(weight_url: str, weight_path: "Path"):
+    print(f"Downloading {weight_url} to {weight_path} ...")
+    pbr = progress(total=100)
+    try:
+        urllib.request.urlretrieve(
+            weight_url, weight_path, reporthook=_report_hook(pbr=pbr)
+        )
+    except (
+        urllib.error.HTTPError,
+        urllib.error.URLError,
+        urllib.error.ContentTooShortError,
+    ) as e:
+        warnings.warn(f"Error downloading {weight_url}: {e}")
+        return None
+    else:
+        print("\rDownload complete.                            ")
+    pbr.close()
+
+
 def get_weights_path(model_type: str) -> Optional[Path]:
     """Returns the path to the weight of a given model architecture."""
     weight_url = SAM_WEIGHTS_URL[model_type]
 
     cache_dir = Path.home() / ".cache/napari-segment-anything"
     cache_dir.mkdir(parents=True, exist_ok=True)
 
     weight_path = cache_dir / weight_url.split("/")[-1]
 
     # Download the weights if they don't exist
     if not weight_path.exists():
-        print(f"Downloading {weight_url} to {weight_path} ...")
-        try:
-            urllib.request.urlretrieve(
-                weight_url, weight_path, reporthook=_report_hook
-            )
-        except (
-            urllib.error.HTTPError,
-            urllib.error.URLError,
-            urllib.error.ContentTooShortError,
-        ) as e:
-            warnings.warn(f"Error downloading {weight_url}: {e}")
-            return None
-        else:
-            print("\rDownload complete.                            ")
+        download_weights(weight_url, weight_path)
 
     return weight_path
```

### Comparing `napari-segment-anything-0.1.2/src/napari_segment_anything.egg-info/PKG-INFO` & `napari-segment-anything-0.1.3/src/napari_segment_anything.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-segment-anything
-Version: 0.1.2
+Version: 0.1.3
 Summary: Napari plugin of Segment Anything Model (SAM)
 Home-page: https://github.com/jookuma/napari-segment-anything
 Author: Jordao Bragantini
 Author-email: jordao.bragantini@czbiohub.org
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/jookuma/napari-segment-anything/issues
 Project-URL: Documentation, https://github.com/jookuma/napari-segment-anything#README.md
@@ -58,18 +58,38 @@
 
 We recommend installing the latest development version because this package is being developed:
 
 ```bash
 pip install git+https://github.com/jookuma/napari-segment-anything.git
 ```
 
-IMPORTANT: `napari` won't work if you don't have `pyqt5` or `pyside2` installed.
+**IMPORTANT**: `napari` won't work if you don't have `pyqt5` or `pyside2` installed.
 
 ## Instructions
 
+### Opening napari-segment-anything
+
+This software is napari plugin, so once you have napari installed you can open it using the command line:
+
+```bash
+napari <your image path> -w napari-segment-anything 'Segment Anything'
+```
+
+I noticed that sometimes napari fails to load the plugin widget from the command line, go to step 2 from below to load it.
+
+If you prefer the user interface you need to:
+
+1) Drag and drop your image into napari to load it;
+2) Go to the "Plugins" file menu in the upper right corner and select the "Segment Anything" plugin.
+3) Follow the instructions below for usage.
+
+**IMPORTANT**: If you get an error make sure you have `pyqt5` or `pyside2` installed.
+
+### Usage
+
 - Interactions are done on the "SAM points" and "SAM box" layers using the existing functionalities of napari. Only rectangle shapes trigger the network prediction.
 - For points supervision, left clicks are positive cues (object) and right clicks are negative (background).
 - Press the "Confirm Annot." button (or the "C" key) to propagate the current segmentation mask to the label image.
 - Use the napari labels layer features to delete or edit already confirmed labels.
 
 ## Contributing
```

### Comparing `napari-segment-anything-0.1.2/src/napari_segment_anything.egg-info/SOURCES.txt` & `napari-segment-anything-0.1.3/src/napari_segment_anything.egg-info/SOURCES.txt`

 * *Files identical despite different names*

