# Comparing `tmp/hdr-plot-0.6.0.tar.gz` & `tmp/hdr-plot-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdr-plot-0.6.0.tar", last modified: Fri Mar 24 16:25:33 2023, max compression
+gzip compressed data, was "hdr-plot-0.6.1.tar", last modified: Mon Apr 10 09:35:33 2023, max compression
```

## Comparing `hdr-plot-0.6.0.tar` & `hdr-plot-0.6.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 bruno      (501) staff       (20)        0 2023-03-24 16:25:33.467624 hdr-plot-0.6.0/
--rw-r--r--   0 bruno      (501) staff       (20)    11357 2018-05-07 20:20:13.000000 hdr-plot-0.6.0/LICENSE
--rw-r--r--   0 bruno      (501) staff       (20)     2888 2023-03-24 16:25:33.467429 hdr-plot-0.6.0/PKG-INFO
--rw-r--r--   0 bruno      (501) staff       (20)     2418 2023-03-24 13:56:46.000000 hdr-plot-0.6.0/README.md
-drwxr-xr-x   0 bruno      (501) staff       (20)        0 2023-03-24 16:25:33.465460 hdr-plot-0.6.0/bin/
--rwxr-xr-x   0 bruno      (501) staff       (20)      594 2023-03-24 15:45:01.000000 hdr-plot-0.6.0/bin/hdr-plot
-drwxr-xr-x   0 bruno      (501) staff       (20)        0 2023-03-24 16:25:33.465816 hdr-plot-0.6.0/hdr_plot/
--rw-r--r--   0 bruno      (501) staff       (20)       18 2018-06-26 23:05:06.000000 hdr-plot-0.6.0/hdr_plot/__init__.py
--rwxr-xr-x   0 bruno      (501) staff       (20)     8564 2023-03-24 15:45:17.000000 hdr-plot-0.6.0/hdr_plot/hdr_plot.py
-drwxr-xr-x   0 bruno      (501) staff       (20)        0 2023-03-24 16:25:33.467159 hdr-plot-0.6.0/hdr_plot.egg-info/
--rw-r--r--   0 bruno      (501) staff       (20)     2888 2023-03-24 16:25:33.000000 hdr-plot-0.6.0/hdr_plot.egg-info/PKG-INFO
--rw-r--r--   0 bruno      (501) staff       (20)      240 2023-03-24 16:25:33.000000 hdr-plot-0.6.0/hdr_plot.egg-info/SOURCES.txt
--rw-r--r--   0 bruno      (501) staff       (20)        1 2023-03-24 16:25:33.000000 hdr-plot-0.6.0/hdr_plot.egg-info/dependency_links.txt
--rw-r--r--   0 bruno      (501) staff       (20)       18 2023-03-24 16:25:33.000000 hdr-plot-0.6.0/hdr_plot.egg-info/requires.txt
--rw-r--r--   0 bruno      (501) staff       (20)        9 2023-03-24 16:25:33.000000 hdr-plot-0.6.0/hdr_plot.egg-info/top_level.txt
--rw-r--r--   0 bruno      (501) staff       (20)       38 2023-03-24 16:25:33.467689 hdr-plot-0.6.0/setup.cfg
--rw-r--r--   0 bruno      (501) staff       (20)      742 2023-03-24 16:25:20.000000 hdr-plot-0.6.0/setup.py
+drwxr-xr-x   0 bruno      (501) staff       (20)        0 2023-04-10 09:35:33.425914 hdr-plot-0.6.1/
+-rw-r--r--   0 bruno      (501) staff       (20)    11357 2018-05-07 20:20:13.000000 hdr-plot-0.6.1/LICENSE
+-rw-r--r--   0 bruno      (501) staff       (20)     2888 2023-04-10 09:35:33.425748 hdr-plot-0.6.1/PKG-INFO
+-rw-r--r--   0 bruno      (501) staff       (20)     2418 2023-03-24 13:56:46.000000 hdr-plot-0.6.1/README.md
+drwxr-xr-x   0 bruno      (501) staff       (20)        0 2023-04-10 09:35:33.424679 hdr-plot-0.6.1/bin/
+-rwxr-xr-x   0 bruno      (501) staff       (20)      594 2023-03-24 15:45:01.000000 hdr-plot-0.6.1/bin/hdr-plot
+drwxr-xr-x   0 bruno      (501) staff       (20)        0 2023-04-10 09:35:33.424931 hdr-plot-0.6.1/hdr_plot/
+-rw-r--r--   0 bruno      (501) staff       (20)       18 2018-06-26 23:05:06.000000 hdr-plot-0.6.1/hdr_plot/__init__.py
+-rwxr-xr-x   0 bruno      (501) staff       (20)     8885 2023-04-10 09:33:12.000000 hdr-plot-0.6.1/hdr_plot/hdr_plot.py
+drwxr-xr-x   0 bruno      (501) staff       (20)        0 2023-04-10 09:35:33.425549 hdr-plot-0.6.1/hdr_plot.egg-info/
+-rw-r--r--   0 bruno      (501) staff       (20)     2888 2023-04-10 09:35:33.000000 hdr-plot-0.6.1/hdr_plot.egg-info/PKG-INFO
+-rw-r--r--   0 bruno      (501) staff       (20)      240 2023-04-10 09:35:33.000000 hdr-plot-0.6.1/hdr_plot.egg-info/SOURCES.txt
+-rw-r--r--   0 bruno      (501) staff       (20)        1 2023-04-10 09:35:33.000000 hdr-plot-0.6.1/hdr_plot.egg-info/dependency_links.txt
+-rw-r--r--   0 bruno      (501) staff       (20)       18 2023-04-10 09:35:33.000000 hdr-plot-0.6.1/hdr_plot.egg-info/requires.txt
+-rw-r--r--   0 bruno      (501) staff       (20)        9 2023-04-10 09:35:33.000000 hdr-plot-0.6.1/hdr_plot.egg-info/top_level.txt
+-rw-r--r--   0 bruno      (501) staff       (20)       38 2023-04-10 09:35:33.425964 hdr-plot-0.6.1/setup.cfg
+-rw-r--r--   0 bruno      (501) staff       (20)      742 2023-04-10 09:33:39.000000 hdr-plot-0.6.1/setup.py
```

### Comparing `hdr-plot-0.6.0/LICENSE` & `hdr-plot-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hdr-plot-0.6.0/PKG-INFO` & `hdr-plot-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdr-plot
-Version: 0.6.0
+Version: 0.6.1
 Summary: A simple HdrHistogram plotting script.
 Home-page: https://github.com/BrunoBonacci/hdr-plot
 Author: Bruno Bonacci
 Author-email: bonacci.bruno@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hdr-plot-0.6.0/README.md` & `hdr-plot-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `hdr-plot-0.6.0/bin/hdr-plot` & `hdr-plot-0.6.1/bin/hdr-plot`

 * *Files identical despite different names*

### Comparing `hdr-plot-0.6.0/hdr_plot/hdr_plot.py` & `hdr-plot-0.6.1/hdr_plot/hdr_plot.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # This is just a quick and unsophisticated script to quickly plot the
 # HdrHistograms directly from the output of `wkr2` benchmarks.
 #
 #
 import argparse
 import re
 import sys
+import math
 import pandas as pd
 import matplotlib.pyplot as plt
 import matplotlib.ticker as ticker
 import pkg_resources
 
 #
 # parsing and plotting functions
@@ -105,28 +106,33 @@
             verticalalignment='top', bbox=props, fontname='monospace')
 
     return t
 
 
 def plot_summarybox(fig, ax, percentiles, metadata, labels, units, summary_fields):
     # add info box to the side
-    if len(labels) < 5:
+    box_length = 5
+    if len(labels) <= box_length:
         textstr = '\n'.join([info_text(labels[i], percentiles[i], metadata[i], units, summary_fields) for i in range(len(labels))])
         info_box(ax, textstr, 0.02)
     else:
-        textstr1 = '\n'.join([info_text(labels[i], percentiles[i], metadata[i], units, summary_fields) for i in range(4)])
-        textstr2 = '\n'.join([info_text(labels[i], percentiles[i], metadata[i], units, summary_fields) for i in range(4, len(labels))])
-
-        box1 = info_box(ax, textstr1, 0.01)
-
-        # align the second box next to the first one by retrieving its width
-        box1_dimensions = box1.get_window_extent(renderer=fig.canvas.get_renderer())
-        box1_edge = box1_dimensions.x1, 0
-        box2_edge_axes_coords = ax.transAxes.inverted().transform(box1_edge)
-        info_box(ax, textstr2, box2_edge_axes_coords[0] + 0.01)
+        previous_box = None
+        for n in range(0, len(labels), box_length):
+            start = n
+            end = min(n + box_length, len(labels))
+            textstr = '\n'.join([info_text(labels[i], percentiles[i], metadata[i], units, summary_fields) for i in range(start, end)])
+
+            if previous_box is None:
+                previous_box = info_box(ax, textstr, 0.01)
+            else:
+                # align the box next to the previous one
+                previous_box_dimensions = previous_box.get_window_extent(renderer=fig.canvas.get_renderer())
+                previous_box_edge = previous_box_dimensions.x1, 0
+                current_box_edge_axes_coords = ax.transAxes.inverted().transform(previous_box_edge)
+                previous_box = info_box(ax, textstr, current_box_edge_axes_coords[0] + 0.01)
 
 
 def plot_percentiles(percentiles, labels, units, percentiles_range_max):
     fig, ax = plt.subplots(figsize=(16, 8))
     plt.rc('font', size=8)
     plt.rc('figure', titlesize=12)
     plt.rc('axes', titlesize=10)
@@ -150,15 +156,17 @@
            title='Latency Percentiles (lower is better)')
     ax.set_xscale('logit')
     plt.xticks(all_percentiles[0:percentiles_max_index + 1])
     plt.xlim([0, max_percentile])
     majors = all_percentile_labels[0:percentiles_max_index + 1]
     ax.xaxis.set_major_formatter(ticker.FixedFormatter(majors))
     ax.xaxis.set_minor_formatter(ticker.NullFormatter())
-    plt.legend(bbox_to_anchor=(0.125, 0.01, 1, 0.102), bbox_transform=fig.transFigure, loc=3, ncol=2,
+    # we would like the labels box to have at most 3 lines
+    n_col = math.ceil(len(labels) / 3)
+    plt.legend(bbox_to_anchor=(0.125, 0.01, 1, 0.102), bbox_transform=fig.transFigure, loc=3, ncol=n_col,
                borderaxespad=0, labels=labels)
     # make room for the legend
     plt.subplots_adjust(bottom=0.11)
     return fig, ax
 
 
 def arg_parse():
```

### Comparing `hdr-plot-0.6.0/hdr_plot.egg-info/PKG-INFO` & `hdr-plot-0.6.1/hdr_plot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdr-plot
-Version: 0.6.0
+Version: 0.6.1
 Summary: A simple HdrHistogram plotting script.
 Home-page: https://github.com/BrunoBonacci/hdr-plot
 Author: Bruno Bonacci
 Author-email: bonacci.bruno@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hdr-plot-0.6.0/setup.py` & `hdr-plot-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hdr-plot",
-    version="0.6.0",
+    version="0.6.1",
     author="Bruno Bonacci",
     author_email="bonacci.bruno@gmail.com",
     description="A simple HdrHistogram plotting script.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BrunoBonacci/hdr-plot",
     packages=setuptools.find_packages(),
```

