# Comparing `tmp/plotly_gif-0.0.3.tar.gz` & `tmp/plotly_gif-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotly_gif-0.0.3.tar", last modified: Fri Jan  7 13:23:46 2022, max compression
+gzip compressed data, was "C:\Users\nicep\Desktop\pyth_proj\plotly_gif\dist\.tmp-cxo7zlz2\plotly_gif-0.0.4.tar", last modified: Mon Apr 10 12:37:18 2023, max compression
```

## Comparing `plotly_gif-0.0.3.tar` & `plotly_gif-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-01-07 13:23:46.771643 plotly_gif-0.0.3/
--rw-rw-rw-   0        0        0     1564 2022-01-06 00:31:06.000000 plotly_gif-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     2851 2022-01-07 13:23:46.772644 plotly_gif-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2288 2022-01-07 03:45:23.000000 plotly_gif-0.0.3/README.md
--rw-rw-rw-   0        0        0      114 2022-01-06 00:32:43.000000 plotly_gif-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      777 2022-01-07 13:23:46.776641 plotly_gif-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0       75 2022-01-06 00:22:57.000000 plotly_gif-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-01-07 13:23:46.646715 plotly_gif-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2022-01-07 13:23:46.701683 plotly_gif-0.0.3/src/plotly_gif/
--rw-rw-rw-   0        0        0      770 2022-01-06 20:46:11.000000 plotly_gif-0.0.3/src/plotly_gif/__init__.py
--rw-rw-rw-   0        0        0      880 2022-01-06 20:50:07.000000 plotly_gif-0.0.3/src/plotly_gif/format_.py
--rw-rw-rw-   0        0        0     5315 2022-01-07 03:39:07.000000 plotly_gif-0.0.3/src/plotly_gif/gif.py
--rw-rw-rw-   0        0        0     1678 2022-01-07 03:30:31.000000 plotly_gif-0.0.3/src/plotly_gif/three_d_plots.py
--rw-rw-rw-   0        0        0     1590 2022-01-06 21:08:42.000000 plotly_gif-0.0.3/src/plotly_gif/two_d_plots.py
-drwxrwxrwx   0        0        0        0 2022-01-07 13:23:46.768644 plotly_gif-0.0.3/src/plotly_gif.egg-info/
--rw-rw-rw-   0        0        0     2851 2022-01-07 13:23:46.000000 plotly_gif-0.0.3/src/plotly_gif.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      418 2022-01-07 13:23:46.000000 plotly_gif-0.0.3/src/plotly_gif.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-07 13:23:46.000000 plotly_gif-0.0.3/src/plotly_gif.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-01-06 03:09:42.000000 plotly_gif-0.0.3/src/plotly_gif.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       43 2022-01-07 13:23:46.000000 plotly_gif-0.0.3/src/plotly_gif.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-01-07 13:23:46.000000 plotly_gif-0.0.3/src/plotly_gif.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 12:37:18.000000 plotly_gif-0.0.4/
+-rw-rw-rw-   0        0        0     1564 2023-04-10 11:53:18.000000 plotly_gif-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     3514 2023-04-10 12:37:18.000000 plotly_gif-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2904 2023-04-10 12:32:47.000000 plotly_gif-0.0.4/README.md
+-rw-rw-rw-   0        0        0      114 2023-04-10 11:53:18.000000 plotly_gif-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      833 2023-04-10 12:37:18.000000 plotly_gif-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0       75 2023-04-10 11:53:18.000000 plotly_gif-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:37:18.000000 plotly_gif-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-10 12:37:18.000000 plotly_gif-0.0.4/src/plotly_gif/
+-rw-rw-rw-   0        0        0      783 2023-04-10 12:09:21.000000 plotly_gif-0.0.4/src/plotly_gif/__init__.py
+-rw-rw-rw-   0        0        0      880 2023-04-10 11:53:18.000000 plotly_gif-0.0.4/src/plotly_gif/format_.py
+-rw-rw-rw-   0        0        0     5361 2023-04-10 12:22:06.000000 plotly_gif-0.0.4/src/plotly_gif/gif.py
+-rw-rw-rw-   0        0        0     2327 2023-04-10 12:13:37.000000 plotly_gif-0.0.4/src/plotly_gif/three_d_plots.py
+-rw-rw-rw-   0        0        0     1603 2023-04-10 12:13:37.000000 plotly_gif-0.0.4/src/plotly_gif/two_d_plots.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:37:18.000000 plotly_gif-0.0.4/src/plotly_gif.egg-info/
+-rw-rw-rw-   0        0        0     3514 2023-04-10 12:37:18.000000 plotly_gif-0.0.4/src/plotly_gif.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      418 2023-04-10 12:37:18.000000 plotly_gif-0.0.4/src/plotly_gif.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 12:37:18.000000 plotly_gif-0.0.4/src/plotly_gif.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-10 12:28:51.000000 plotly_gif-0.0.4/src/plotly_gif.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       57 2023-04-10 12:37:18.000000 plotly_gif-0.0.4/src/plotly_gif.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-10 12:37:18.000000 plotly_gif-0.0.4/src/plotly_gif.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `plotly_gif-0.0.3/LICENSE.txt` & `plotly_gif-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plotly_gif-0.0.3/PKG-INFO` & `plotly_gif-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: plotly_gif
-Version: 0.0.3
-Summary: Create gif from your plotly figures!
-Home-page: https://github.com/dylanwal/plotly_gif
-Author: Dylan Walsh
-License: BSD
-Platform: any
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Plotly-gif 
 
 ---
 ---
 ![PyPI](https://img.shields.io/pypi/v/plotly_gif)
 ![downloads](https://img.shields.io/pypi/dm/plotly_gif)
 ![license](https://img.shields.io/github/license/dylanwal/plotly_gif)
@@ -31,20 +14,26 @@
 ```
 pip install plotly-gif
 ```
 
 ### Dependencies
 
 If you are already using plotly, then you should be good. But, just in case, these are the dependencies:
-```python
-pip install plotly    
-pip install kaleido   # used by plotly to generate png
-pip install Pillow    # used to convert png to gif
-```    
-
+* [plotly](https://github.com/plotly/plotly.py) (5.9.0)
+  * Plots molecules
+* [kaleido](https://github.com/plotly/Kaleido)  (0.1.0post1)
+  * Converts plotly graphs to images (png, svg, etc.)
+  * I am not using the most recent version of kaleido as it does not play nice with my computer. Try the newest 
+    version, but if you are having issues install this specific version.
+* [Pillow](https://github.com/python-pillow/Pillow) (9.2.0)
+  * Used to convert png to gif.
+* [numpy](https://github.com/numpy/numpy) (1.23.1)
+  * Used for math
+  
+    
 ---
 ## Usage
 
 There are three common methods:
 
 ### Built-in Functions/ Macros
 Currently, we have the follow:
@@ -107,24 +96,25 @@
     
     return fig
 
 gif.create_gif() # generate gif
 ```
 
 ---
-## Options
-
-
-
----
 ## Examples
 See examples folder
 
-![3d gif](https://github.com/dylanwal/plotly_gif/blob/master/examples/gifs/fig.gif)
+![2d gif](https://github.com/dylanwal/plotly_gif/blob/master/examples/gifs/example_1.gif)
+
+
+![3d gif](https://github.com/dylanwal/plotly_gif/blob/master/examples/gifs/example_3.gif)
 
-## Notes:
 
 
 ### Time to generate gif (60 images per gif)
 * Simple 2D plots with small data sets (100 pts): ~10 sec
 * Simple 3D plots with small data sets (100 pts): ~1.5 min
 
+
+## Warning
+
+* If your code 'hangs' or 'gets stuck and doesn't complete' try changing kaleido versions `pip install kaleido==0.1.0post1`
```

### Comparing `plotly_gif-0.0.3/setup.cfg` & `plotly_gif-0.0.4/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6c6f 746c 795f 6769 660d 0a76   = plotly_gif..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e33 0d0a  ersion = 0.0.3..
+00000020: 6572 7369 6f6e 203d 2030 2e30 2e34 0d0a  ersion = 0.0.4..
 00000030: 6465 7363 7269 7074 696f 6e20 3d20 4372  description = Cr
 00000040: 6561 7465 2067 6966 2066 726f 6d20 796f  eate gif from yo
 00000050: 7572 2070 6c6f 746c 7920 6669 6775 7265  ur plotly figure
 00000060: 7321 0d0a 6c6f 6e67 5f64 6573 6372 6970  s!..long_descrip
 00000070: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000080: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 00000090: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
@@ -24,26 +24,30 @@
 00000170: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
 00000180: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
 00000190: 3a3a 2033 0d0a 0950 726f 6772 616d 6d69  :: 3...Programmi
 000001a0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
 000001b0: 7974 686f 6e20 3a3a 2033 203a 3a20 4f6e  ython :: 3 :: On
 000001c0: 6c79 0d0a 0950 726f 6772 616d 6d69 6e67  ly...Programming
 000001d0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000001e0: 686f 6e20 3a3a 2033 2e38 0d0a 0950 726f  hon :: 3.8...Pro
+000001e0: 686f 6e20 3a3a 2033 2e37 0d0a 0950 726f  hon :: 3.7...Pro
 000001f0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
 00000200: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000210: 2e39 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  .9....[options].
-00000220: 0a70 6163 6b61 6765 7320 3d20 0d0a 0970  .packages = ...p
-00000230: 6c6f 746c 795f 6769 660d 0a70 7974 686f  lotly_gif..pytho
-00000240: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-00000250: 2e38 0d0a 7061 636b 6167 655f 6469 7220  .8..package_dir 
-00000260: 3d20 0d0a 093d 7372 630d 0a7a 6970 5f73  = ...=src..zip_s
-00000270: 6166 6520 3d20 6e6f 0d0a 696e 636c 7564  afe = no..includ
-00000280: 655f 7061 636b 6167 655f 6461 7461 203d  e_package_data =
-00000290: 2074 7275 650d 0a69 6e73 7461 6c6c 5f72   true..install_r
-000002a0: 6571 7569 7265 7320 3d20 0d0a 0950 696c  equires = ...Pil
-000002b0: 6c6f 773e 3d39 2e30 2e30 0d0a 0970 6c6f  low>=9.0.0...plo
-000002c0: 746c 793e 3d35 2e35 2e30 0d0a 096b 616c  tly>=5.5.0...kal
-000002d0: 6569 646f 3e3d 302e 322e 310d 0a0d 0a5b  eido>=0.2.1....[
-000002e0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-000002f0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-00000300: 6520 3d20 300d 0a0d 0a                   e = 0....
+00000210: 2e38 0d0a 0950 726f 6772 616d 6d69 6e67  .8...Programming
+00000220: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000230: 686f 6e20 3a3a 2033 2e39 0d0a 0d0a 5b6f  hon :: 3.9....[o
+00000240: 7074 696f 6e73 5d0d 0a70 6163 6b61 6765  ptions]..package
+00000250: 7320 3d20 0d0a 0970 6c6f 746c 795f 6769  s = ...plotly_gi
+00000260: 660d 0a70 7974 686f 6e5f 7265 7175 6972  f..python_requir
+00000270: 6573 203d 203e 3d33 2e37 0d0a 7061 636b  es = >=3.7..pack
+00000280: 6167 655f 6469 7220 3d20 0d0a 093d 7372  age_dir = ...=sr
+00000290: 630d 0a7a 6970 5f73 6166 6520 3d20 6e6f  c..zip_safe = no
+000002a0: 0d0a 696e 636c 7564 655f 7061 636b 6167  ..include_packag
+000002b0: 655f 6461 7461 203d 2074 7275 650d 0a69  e_data = true..i
+000002c0: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
+000002d0: 3d20 0d0a 0950 696c 6c6f 773e 3d39 2e30  = ...Pillow>=9.0
+000002e0: 2e30 0d0a 0970 6c6f 746c 793e 3d35 2e35  .0...plotly>=5.5
+000002f0: 2e30 0d0a 096b 616c 6569 646f 3e3d 302e  .0...kaleido>=0.
+00000300: 322e 310d 0a09 6e75 6d70 793e 3d31 2e32  2.1...numpy>=1.2
+00000310: 312e 360d 0a0d 0a5b 6567 675f 696e 666f  1.6....[egg_info
+00000320: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+00000330: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000340: 0a                                       .
```

### Comparing `plotly_gif-0.0.3/src/plotly_gif/__init__.py` & `plotly_gif-0.0.4/src/plotly_gif/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from functools import wraps
 import logging
 
-from .gif import GIF
-from .two_d_plots import two_d_time_series
-from .three_d_plots import three_d_scatter_rotate
+from plotly_gif.gif import GIF
+from plotly_gif.two_d_plots import two_d_time_series
+from plotly_gif.three_d_plots import three_d_scatter_rotate
 
 __all__ = ["GIF", "capture", "two_d_time_series", "three_d_scatter_rotate"]
 
-
-level = logging.INFO
-logging.basicConfig(level=level, format='  %(message)s')
+logging.basicConfig(level=logging.INFO, format='  %(message)s')
 
 
 def capture(gif_: GIF):
     """ Capture
     Captures images as they are created.
 
     Parameters
```

### Comparing `plotly_gif-0.0.3/src/plotly_gif/format_.py` & `plotly_gif-0.0.4/src/plotly_gif/format_.py`

 * *Files identical despite different names*

### Comparing `plotly_gif-0.0.3/src/plotly_gif/gif.py` & `plotly_gif-0.0.4/src/plotly_gif/gif.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 import sys
 from io import BytesIO
 from pathlib import Path
 from datetime import datetime, timedelta
 import glob
 import copy
 import re
+import logging
 
 from PIL import Image
 
-from . import logging
-
 
 def get_exec_path():
     try:
         file = os.path.abspath(sys.modules['__main__'].__file__)
     except Exception:
         file = sys.executable
     return os.path.dirname(file)
@@ -117,14 +116,15 @@
 
             if self.imgs is None:
                 self.imgs = [img]
             else:
                 self.imgs.append(img)
         if self.mode == "png":
             if not self._image_folder_present:
+                self._image_folder_present = True
                 self._create_folder()
             png_path = self.image_path / f"img_{self.num_images}.png"
             fig.write_image(png_path)
 
         self.num_images += 1
 
         if self.verbose:
@@ -146,15 +146,15 @@
         kwargs:
             See https://pillow.readthedocs.io/en/stable/handbook/image-file-formats.html#gif
 
         """
         if gif_path is None:
             gif_path = self.gif_path / "fig.gif" if self.gif_name is None else self.gif_path / self.gif_name
         else:
-            if gif_path.endswith(".gif"):
+            if not gif_path.endswith(".gif"):
                 raise ValueError(f"gif path must end with '.gif'. Provide value: {gif_path}")
 
         _kwargs = {
             "fp": gif_path,
             "save_all": True,
             "optimize": True,
             "between": "startend",
```

### Comparing `plotly_gif-0.0.3/src/plotly_gif/two_d_plots.py` & `plotly_gif-0.0.4/src/plotly_gif/two_d_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import copy
 
 import plotly.graph_objs as go
 
-from . import GIF
+from plotly_gif.gif import GIF
 
 
 def two_d_time_series(
         gif_: GIF,
         fig: go.Figure,
         frames: int = 60,
         auto_create: bool = True,
```

### Comparing `plotly_gif-0.0.3/src/plotly_gif.egg-info/PKG-INFO` & `plotly_gif-0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
-Name: plotly-gif
-Version: 0.0.3
+Name: plotly_gif
+Version: 0.0.4
 Summary: Create gif from your plotly figures!
 Home-page: https://github.com/dylanwal/plotly_gif
 Author: Dylan Walsh
 License: BSD
 Platform: any
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Plotly-gif 
 
 ---
 ---
@@ -31,20 +32,26 @@
 ```
 pip install plotly-gif
 ```
 
 ### Dependencies
 
 If you are already using plotly, then you should be good. But, just in case, these are the dependencies:
-```python
-pip install plotly    
-pip install kaleido   # used by plotly to generate png
-pip install Pillow    # used to convert png to gif
-```    
-
+* [plotly](https://github.com/plotly/plotly.py) (5.9.0)
+  * Plots molecules
+* [kaleido](https://github.com/plotly/Kaleido)  (0.1.0post1)
+  * Converts plotly graphs to images (png, svg, etc.)
+  * I am not using the most recent version of kaleido as it does not play nice with my computer. Try the newest 
+    version, but if you are having issues install this specific version.
+* [Pillow](https://github.com/python-pillow/Pillow) (9.2.0)
+  * Used to convert png to gif.
+* [numpy](https://github.com/numpy/numpy) (1.23.1)
+  * Used for math
+  
+    
 ---
 ## Usage
 
 There are three common methods:
 
 ### Built-in Functions/ Macros
 Currently, we have the follow:
@@ -107,24 +114,25 @@
     
     return fig
 
 gif.create_gif() # generate gif
 ```
 
 ---
-## Options
-
-
-
----
 ## Examples
 See examples folder
 
-![3d gif](https://github.com/dylanwal/plotly_gif/blob/master/examples/gifs/fig.gif)
+![2d gif](https://github.com/dylanwal/plotly_gif/blob/master/examples/gifs/example_1.gif)
+
+
+![3d gif](https://github.com/dylanwal/plotly_gif/blob/master/examples/gifs/example_3.gif)
 
-## Notes:
 
 
 ### Time to generate gif (60 images per gif)
 * Simple 2D plots with small data sets (100 pts): ~10 sec
 * Simple 3D plots with small data sets (100 pts): ~1.5 min
 
+
+## Warning
+
+* If your code 'hangs' or 'gets stuck and doesn't complete' try changing kaleido versions `pip install kaleido==0.1.0post1`
```

