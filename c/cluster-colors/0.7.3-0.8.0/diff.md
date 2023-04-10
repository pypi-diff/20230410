# Comparing `tmp/cluster_colors-0.7.3.tar.gz` & `tmp/cluster_colors-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cluster_colors-0.7.3.tar", max compression
+gzip compressed data, was "cluster_colors-0.8.0.tar", max compression
```

## Comparing `cluster_colors-0.7.3.tar` & `cluster_colors-0.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1457 2023-03-19 19:45:07.561425 cluster_colors-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     3466 2023-03-14 22:59:21.524870 cluster_colors-0.7.3/README.md
--rw-r--r--   0        0        0      383 2023-03-14 23:49:36.976311 cluster_colors-0.7.3/src/cluster_colors/__init__.py
--rw-r--r--   0        0        0    20568 2023-03-14 23:50:51.728098 cluster_colors-0.7.3/src/cluster_colors/clusters.py
--rw-r--r--   0        0        0      290 2023-03-14 18:50:46.788014 cluster_colors-0.7.3/src/cluster_colors/config.py
--rw-r--r--   0        0        0     3009 2023-03-14 02:27:27.128539 cluster_colors-0.7.3/src/cluster_colors/cut_colors.py
--rw-r--r--   0        0        0     2994 2023-03-14 21:53:29.144736 cluster_colors-0.7.3/src/cluster_colors/distance_matrix.py
--rw-r--r--   0        0        0     5339 2023-03-16 03:07:18.975108 cluster_colors-0.7.3/src/cluster_colors/image_colors.py
--rw-r--r--   0        0        0     4539 2023-03-15 00:01:08.405918 cluster_colors-0.7.3/src/cluster_colors/kmedians.py
--rw-r--r--   0        0        0      295 2023-03-13 11:40:04.953104 cluster_colors-0.7.3/src/cluster_colors/paths.py
--rw-r--r--   0        0        0     5159 2023-03-19 19:41:53.291090 cluster_colors-0.7.3/src/cluster_colors/pool_colors.py
--rw-r--r--   0        0        0        0 2023-03-09 22:18:11.789791 cluster_colors-0.7.3/src/cluster_colors/py.typed
--rw-r--r--   0        0        0      908 2023-03-19 18:05:34.503213 cluster_colors-0.7.3/src/cluster_colors/type_hints.py
--rw-r--r--   0        0        0     3245 2023-03-11 21:43:47.338567 cluster_colors-0.7.3/src/cluster_colors/vector_stacker.py
--rw-r--r--   0        0        0     4261 1970-01-01 00:00:00.000000 cluster_colors-0.7.3/setup.py
--rw-r--r--   0        0        0     4016 1970-01-01 00:00:00.000000 cluster_colors-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1457 2023-04-10 15:33:44.793581 cluster_colors-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3533 2023-04-10 15:14:34.401917 cluster_colors-0.8.0/README.md
+-rw-r--r--   0        0        0      383 2023-03-14 23:49:36.976311 cluster_colors-0.8.0/src/cluster_colors/__init__.py
+-rw-r--r--   0        0        0    28521 2023-04-10 15:14:34.449282 cluster_colors-0.8.0/src/cluster_colors/clusters.py
+-rw-r--r--   0        0        0      290 2023-03-14 18:50:46.788014 cluster_colors-0.8.0/src/cluster_colors/config.py
+-rw-r--r--   0        0        0     3009 2023-03-14 02:27:27.128539 cluster_colors-0.8.0/src/cluster_colors/cut_colors.py
+-rw-r--r--   0        0        0     3004 2023-04-10 15:14:34.433735 cluster_colors-0.8.0/src/cluster_colors/distance_matrix.py
+-rw-r--r--   0        0        0     5239 2023-04-10 15:14:34.433735 cluster_colors-0.8.0/src/cluster_colors/image_colors.py
+-rw-r--r--   0        0        0     1290 2023-04-10 15:14:34.433735 cluster_colors-0.8.0/src/cluster_colors/kmedians.py
+-rw-r--r--   0        0        0      295 2023-03-13 11:40:04.953104 cluster_colors-0.8.0/src/cluster_colors/paths.py
+-rw-r--r--   0        0        0     5159 2023-03-19 19:41:53.291090 cluster_colors-0.8.0/src/cluster_colors/pool_colors.py
+-rw-r--r--   0        0        0        0 2023-03-09 22:18:11.789791 cluster_colors-0.8.0/src/cluster_colors/py.typed
+-rw-r--r--   0        0        0      908 2023-03-19 18:05:34.503213 cluster_colors-0.8.0/src/cluster_colors/type_hints.py
+-rw-r--r--   0        0        0     3245 2023-03-11 21:43:47.338567 cluster_colors-0.8.0/src/cluster_colors/vector_stacker.py
+-rw-r--r--   0        0        0     4325 1970-01-01 00:00:00.000000 cluster_colors-0.8.0/setup.py
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 cluster_colors-0.8.0/PKG-INFO
```

### Comparing `cluster_colors-0.7.3/pyproject.toml` & `cluster_colors-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cluster-colors"
-version = "0.7.3"
+version = "0.8.0"
 description = "Cluster color vectors with kmedians"
 authors = ["Shay Hill <shay_public@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "cluster_colors", from = "src"}]
 
 [tool.poetry.dependencies]
@@ -21,15 +21,15 @@
 matplotlib = "^3.6.3"
 pre-commit = "^2.21.0"
 black = "^23.1.0"
 tox = "^4.4.7"
 
 [tool.commitizen]
 name = "cz_conventionalish"
-version = "0.7.3"
+version = "0.8.0"
 tag_format = "$version"
 version_files = [
     "pyproject.toml:^version"
 ]
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `cluster_colors-0.7.3/README.md` & `cluster_colors-0.8.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,50 @@
 Divisive (but not hierarchical) clustering.
 
-Slow, but clustering exactly how I wanted it. Iteratively split cluster with highest SSE. Splits are used to find new exemplars, which are thrown into k-medians with existing exemplars.
+Slow, but clustering exactly how I want it. Iteratively split cluster with highest SSE. Splits are used to find new exemplars, which are thrown into k-medians with existing exemplars. Takes pretty extreme measures to avoid not only non-determinism but also non-arbitrary-ism:
+
+* a Clusters instance, when asked to split, will split the cluster with the highest SSE. If there is a tie, the Clusters instance will not arbitrarily decide between the tied clusters, but will instead split all clusters tied for max SSE. This means there is a small chance you will not be able to split a group of colors into exactly n clusters.
+* delta-e is non-commutative, so delta-e is computed *twice* for each distance (a -> b and b -> a). The maximum of these two is used. This doubles the time of an already slow calculation, but delta-e is only used for distances between clusters, and this module is designed to work with small numbers of clusters (Agglomerative clustering may be a better bet if you want to use small clusters.)
 
 Advantages:
 * finds big clusters
-* deterministic
+* deterministic and non-arbitrary
 * robust to outliers
 * fast for what it is, can easily split a few thousand members into a small number of clusters
 * decisions made early on do not effect the result as much as they would in true hierarchical clustering
-* has strategies to avoid ties or arbitrary (even if deterministic) decisions with small member sets
+* has strategies to avoid ties or arbitrary (even if deterministic) decisions with small member sets. This is important when dealing with questions like "which of these five colors is most unlike the others?"
 
 Disadvantages:
-* child clusters will not necessarily contain (or only contain) the members of the parent, so this is not hierarchical (unlike agglomerative clustering where you can build a tree and then transverse it cheaply)
-* as a result of not being hierarchical, it is not straightforward to undo changes if you end up with, for instance, two near-identical exemplars. I have implemented "undo" for the specific method `split_to_se`, but I have not implemented a general "undo" method. Tie-breaking strategies will always use merge instead of undo anyway, so it's important to expect that one list of members might end up in n-clusters multiple ways.
-* slows down as the number of clusters grows, not the best way to de-cluster all the way back to constituent members
+* child clusters will not necessarily contain (or only contain) the members of the parent, so this is not hierarchical, though you can "merge" split clusters by regressing to previous states.
+* sloooows down as the number of clusters grows, not the best way to de-cluster all the way back to constituent members.
 * uses Euclidean distance (sum squared error) for many steps. Delta e is used for final splitting criteria.
 
-This clustering is designed for questions like "what are the two dominant colors in this image (respecting transparency)?"
-
-Once you split a cluster, it's acceptable to just throw it away. And you will probably only need the exemplars of the clusters you do keep, though you could re-cluster each cluster's members for a semi-hierarchical clustering scheme.
+This clustering is designed for questions like "what are the five dominant colors in this image (respecting transparency)?"
 
 ## Three large steps in the background
 
 ### Average colors by n-bit representation
 
 `pool_colors`: reduce 8-bit image colors (potentially 16_777_216 colors) to a maximum of 262_144 by averaging. The ouput of `pool_colors` will also contain a weight axis for each color, representing the combined opacity of all pixels of that color.
 
 ### Median cut along longest axis
 
 `cut_colors`: reduce colors to around 512 by recursively splitting along longest axis (longest actual axis. Not constrained to x, y, or, z axes).
 
 ### k-medians clustering
 
-`KMediansClusters`: split and merge clusters. Again this is *not* hierarchical, so the sequence
-
-* start
-* split
-* merge
-
-is not guaranteed to bring you back to start. The merge methods are "public", but their principal use is to break ties in order to maintain deterministic results. For example:
+`KMediansClusters`: split and merge (undo split) clusters.
 
 * start with one cluster with 100 members
 * split this cluster recursively into five clusters (30, 30, 20, 10, 10)
 * ask for the largest cluster, and there's a tie
-* KMediansClusters will recursively merge the closest two clusters until the tie is broken
+* KMediansClusters will recursively unsplit clusters until all ties are broken. This will *rarely* be needed.
 
 
-##
+## Installation
 
     pip install cluster_colors
 
 ## Basic usage
 
 ~~~python
 from cluster_colors import get_image_clusters
```

### Comparing `cluster_colors-0.7.3/src/cluster_colors/cut_colors.py` & `cluster_colors-0.8.0/src/cluster_colors/cut_colors.py`

 * *Files identical despite different names*

### Comparing `cluster_colors-0.7.3/src/cluster_colors/distance_matrix.py` & `cluster_colors-0.8.0/src/cluster_colors/distance_matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
         :param item: item to add
         """
         for other in self._items:
             self.cache[item, other] = self.func(item, other)
         self._items.add(item)
 
-    def min(self, a: _T) -> float:
+    def min_from_item(self, a: _T) -> float:
         """Return the minimum value of the function for a given item.
 
         :param a: item to find the minimum for
         :return: minimum value of the function for a
         """
         others = self._items - {a}
         return min(self(a, b) for b in others)
```

### Comparing `cluster_colors-0.7.3/src/cluster_colors/image_colors.py` & `cluster_colors-0.8.0/src/cluster_colors/image_colors.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 from __future__ import annotations
 
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 import numpy as np
-from _operator import attrgetter
 from PIL import Image
 
 from cluster_colors.config import CACHE_DIR
 from cluster_colors.cut_colors import cut_colors
 from cluster_colors.kmedians import KMediansClusters
 from cluster_colors.paths import BINARIES_DIR
 from cluster_colors.pool_colors import pool_colors
@@ -84,17 +83,15 @@
     :return: the color with the highest weight
 
     Cluster into large clusters, then return the exemplar of the biggest cluster.
     """
     quarter_colorspace_se = 64**2
     clusters = KMediansClusters.from_stacked_vectors(stacked_colors)
     clusters.split_to_delta_e(quarter_colorspace_se)
-    clusters.merge_to_find_winner()
-    winner = max(clusters, key=attrgetter("w"))
-    return winner.exemplar
+    return clusters.get_rsorted_exemplars()[0]
 
 
 def get_image_clusters(
     filename: Path | str,
     num_colors: int = 512,
     pool_bits: NBits = 6,
     *,
```

### Comparing `cluster_colors-0.7.3/src/cluster_colors/pool_colors.py` & `cluster_colors-0.8.0/src/cluster_colors/pool_colors.py`

 * *Files identical despite different names*

### Comparing `cluster_colors-0.7.3/src/cluster_colors/type_hints.py` & `cluster_colors-0.8.0/src/cluster_colors/type_hints.py`

 * *Files identical despite different names*

### Comparing `cluster_colors-0.7.3/src/cluster_colors/vector_stacker.py` & `cluster_colors-0.8.0/src/cluster_colors/vector_stacker.py`

 * *Files identical despite different names*

### Comparing `cluster_colors-0.7.3/setup.py` & `cluster_colors-0.8.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 ['colormath>=3.0.0,<4.0.0',
  'numpy>=1.24.1,<2.0.0',
  'paragraphs>=0.2.0,<0.3.0',
  'stacked-quantile>=0.3.0,<0.4.0']
 
 setup_kwargs = {
     'name': 'cluster-colors',
-    'version': '0.7.3',
+    'version': '0.8.0',
     'description': 'Cluster color vectors with kmedians',
-    'long_description': 'Divisive (but not hierarchical) clustering.\n\nSlow, but clustering exactly how I wanted it. Iteratively split cluster with highest SSE. Splits are used to find new exemplars, which are thrown into k-medians with existing exemplars.\n\nAdvantages:\n* finds big clusters\n* deterministic\n* robust to outliers\n* fast for what it is, can easily split a few thousand members into a small number of clusters\n* decisions made early on do not effect the result as much as they would in true hierarchical clustering\n* has strategies to avoid ties or arbitrary (even if deterministic) decisions with small member sets\n\nDisadvantages:\n* child clusters will not necessarily contain (or only contain) the members of the parent, so this is not hierarchical (unlike agglomerative clustering where you can build a tree and then transverse it cheaply)\n* as a result of not being hierarchical, it is not straightforward to undo changes if you end up with, for instance, two near-identical exemplars. I have implemented "undo" for the specific method `split_to_se`, but I have not implemented a general "undo" method. Tie-breaking strategies will always use merge instead of undo anyway, so it\'s important to expect that one list of members might end up in n-clusters multiple ways.\n* slows down as the number of clusters grows, not the best way to de-cluster all the way back to constituent members\n* uses Euclidean distance (sum squared error) for many steps. Delta e is used for final splitting criteria.\n\nThis clustering is designed for questions like "what are the two dominant colors in this image (respecting transparency)?"\n\nOnce you split a cluster, it\'s acceptable to just throw it away. And you will probably only need the exemplars of the clusters you do keep, though you could re-cluster each cluster\'s members for a semi-hierarchical clustering scheme.\n\n## Three large steps in the background\n\n### Average colors by n-bit representation\n\n`pool_colors`: reduce 8-bit image colors (potentially 16_777_216 colors) to a maximum of 262_144 by averaging. The ouput of `pool_colors` will also contain a weight axis for each color, representing the combined opacity of all pixels of that color.\n\n### Median cut along longest axis\n\n`cut_colors`: reduce colors to around 512 by recursively splitting along longest axis (longest actual axis. Not constrained to x, y, or, z axes).\n\n### k-medians clustering\n\n`KMediansClusters`: split and merge clusters. Again this is *not* hierarchical, so the sequence\n\n* start\n* split\n* merge\n\nis not guaranteed to bring you back to start. The merge methods are "public", but their principal use is to break ties in order to maintain deterministic results. For example:\n\n* start with one cluster with 100 members\n* split this cluster recursively into five clusters (30, 30, 20, 10, 10)\n* ask for the largest cluster, and there\'s a tie\n* KMediansClusters will recursively merge the closest two clusters until the tie is broken\n\n\n##\n\n    pip install cluster_colors\n\n## Basic usage\n\n~~~python\nfrom cluster_colors import get_image_clusters\n\nclusters = get_image_clusters(image_filename) # one cluster at this point\nclusters.split_to_delta_e(16)\nsplit_clusters = clusters.get_rsorted_clusters()\n\ncolors: list[tuple[float, float, float]] = [c.exemplar for c in split_clusters]\n\n# to save the cluster exemplars as an image file\n\nshow_clusters(split_clusters, "open_file_to_see_clusters")\n~~~\n',
+    'long_description': 'Divisive (but not hierarchical) clustering.\n\nSlow, but clustering exactly how I want it. Iteratively split cluster with highest SSE. Splits are used to find new exemplars, which are thrown into k-medians with existing exemplars. Takes pretty extreme measures to avoid not only non-determinism but also non-arbitrary-ism:\n\n* a Clusters instance, when asked to split, will split the cluster with the highest SSE. If there is a tie, the Clusters instance will not arbitrarily decide between the tied clusters, but will instead split all clusters tied for max SSE. This means there is a small chance you will not be able to split a group of colors into exactly n clusters.\n* delta-e is non-commutative, so delta-e is computed *twice* for each distance (a -> b and b -> a). The maximum of these two is used. This doubles the time of an already slow calculation, but delta-e is only used for distances between clusters, and this module is designed to work with small numbers of clusters (Agglomerative clustering may be a better bet if you want to use small clusters.)\n\nAdvantages:\n* finds big clusters\n* deterministic and non-arbitrary\n* robust to outliers\n* fast for what it is, can easily split a few thousand members into a small number of clusters\n* decisions made early on do not effect the result as much as they would in true hierarchical clustering\n* has strategies to avoid ties or arbitrary (even if deterministic) decisions with small member sets. This is important when dealing with questions like "which of these five colors is most unlike the others?"\n\nDisadvantages:\n* child clusters will not necessarily contain (or only contain) the members of the parent, so this is not hierarchical, though you can "merge" split clusters by regressing to previous states.\n* sloooows down as the number of clusters grows, not the best way to de-cluster all the way back to constituent members.\n* uses Euclidean distance (sum squared error) for many steps. Delta e is used for final splitting criteria.\n\nThis clustering is designed for questions like "what are the five dominant colors in this image (respecting transparency)?"\n\n## Three large steps in the background\n\n### Average colors by n-bit representation\n\n`pool_colors`: reduce 8-bit image colors (potentially 16_777_216 colors) to a maximum of 262_144 by averaging. The ouput of `pool_colors` will also contain a weight axis for each color, representing the combined opacity of all pixels of that color.\n\n### Median cut along longest axis\n\n`cut_colors`: reduce colors to around 512 by recursively splitting along longest axis (longest actual axis. Not constrained to x, y, or, z axes).\n\n### k-medians clustering\n\n`KMediansClusters`: split and merge (undo split) clusters.\n\n* start with one cluster with 100 members\n* split this cluster recursively into five clusters (30, 30, 20, 10, 10)\n* ask for the largest cluster, and there\'s a tie\n* KMediansClusters will recursively unsplit clusters until all ties are broken. This will *rarely* be needed.\n\n\n## Installation\n\n    pip install cluster_colors\n\n## Basic usage\n\n~~~python\nfrom cluster_colors import get_image_clusters\n\nclusters = get_image_clusters(image_filename) # one cluster at this point\nclusters.split_to_delta_e(16)\nsplit_clusters = clusters.get_rsorted_clusters()\n\ncolors: list[tuple[float, float, float]] = [c.exemplar for c in split_clusters]\n\n# to save the cluster exemplars as an image file\n\nshow_clusters(split_clusters, "open_file_to_see_clusters")\n~~~\n',
     'author': 'Shay Hill',
     'author_email': 'shay_public@hotmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `cluster_colors-0.7.3/PKG-INFO` & `cluster_colors-0.8.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cluster-colors
-Version: 0.7.3
+Version: 0.8.0
 Summary: Cluster color vectors with kmedians
 License: MIT
 Author: Shay Hill
 Author-email: shay_public@hotmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,61 +14,55 @@
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
 Requires-Dist: paragraphs (>=0.2.0,<0.3.0)
 Requires-Dist: stacked-quantile (>=0.3.0,<0.4.0)
 Description-Content-Type: text/markdown
 
 Divisive (but not hierarchical) clustering.
 
-Slow, but clustering exactly how I wanted it. Iteratively split cluster with highest SSE. Splits are used to find new exemplars, which are thrown into k-medians with existing exemplars.
+Slow, but clustering exactly how I want it. Iteratively split cluster with highest SSE. Splits are used to find new exemplars, which are thrown into k-medians with existing exemplars. Takes pretty extreme measures to avoid not only non-determinism but also non-arbitrary-ism:
+
+* a Clusters instance, when asked to split, will split the cluster with the highest SSE. If there is a tie, the Clusters instance will not arbitrarily decide between the tied clusters, but will instead split all clusters tied for max SSE. This means there is a small chance you will not be able to split a group of colors into exactly n clusters.
+* delta-e is non-commutative, so delta-e is computed *twice* for each distance (a -> b and b -> a). The maximum of these two is used. This doubles the time of an already slow calculation, but delta-e is only used for distances between clusters, and this module is designed to work with small numbers of clusters (Agglomerative clustering may be a better bet if you want to use small clusters.)
 
 Advantages:
 * finds big clusters
-* deterministic
+* deterministic and non-arbitrary
 * robust to outliers
 * fast for what it is, can easily split a few thousand members into a small number of clusters
 * decisions made early on do not effect the result as much as they would in true hierarchical clustering
-* has strategies to avoid ties or arbitrary (even if deterministic) decisions with small member sets
+* has strategies to avoid ties or arbitrary (even if deterministic) decisions with small member sets. This is important when dealing with questions like "which of these five colors is most unlike the others?"
 
 Disadvantages:
-* child clusters will not necessarily contain (or only contain) the members of the parent, so this is not hierarchical (unlike agglomerative clustering where you can build a tree and then transverse it cheaply)
-* as a result of not being hierarchical, it is not straightforward to undo changes if you end up with, for instance, two near-identical exemplars. I have implemented "undo" for the specific method `split_to_se`, but I have not implemented a general "undo" method. Tie-breaking strategies will always use merge instead of undo anyway, so it's important to expect that one list of members might end up in n-clusters multiple ways.
-* slows down as the number of clusters grows, not the best way to de-cluster all the way back to constituent members
+* child clusters will not necessarily contain (or only contain) the members of the parent, so this is not hierarchical, though you can "merge" split clusters by regressing to previous states.
+* sloooows down as the number of clusters grows, not the best way to de-cluster all the way back to constituent members.
 * uses Euclidean distance (sum squared error) for many steps. Delta e is used for final splitting criteria.
 
-This clustering is designed for questions like "what are the two dominant colors in this image (respecting transparency)?"
-
-Once you split a cluster, it's acceptable to just throw it away. And you will probably only need the exemplars of the clusters you do keep, though you could re-cluster each cluster's members for a semi-hierarchical clustering scheme.
+This clustering is designed for questions like "what are the five dominant colors in this image (respecting transparency)?"
 
 ## Three large steps in the background
 
 ### Average colors by n-bit representation
 
 `pool_colors`: reduce 8-bit image colors (potentially 16_777_216 colors) to a maximum of 262_144 by averaging. The ouput of `pool_colors` will also contain a weight axis for each color, representing the combined opacity of all pixels of that color.
 
 ### Median cut along longest axis
 
 `cut_colors`: reduce colors to around 512 by recursively splitting along longest axis (longest actual axis. Not constrained to x, y, or, z axes).
 
 ### k-medians clustering
 
-`KMediansClusters`: split and merge clusters. Again this is *not* hierarchical, so the sequence
-
-* start
-* split
-* merge
-
-is not guaranteed to bring you back to start. The merge methods are "public", but their principal use is to break ties in order to maintain deterministic results. For example:
+`KMediansClusters`: split and merge (undo split) clusters.
 
 * start with one cluster with 100 members
 * split this cluster recursively into five clusters (30, 30, 20, 10, 10)
 * ask for the largest cluster, and there's a tie
-* KMediansClusters will recursively merge the closest two clusters until the tie is broken
+* KMediansClusters will recursively unsplit clusters until all ties are broken. This will *rarely* be needed.
 
 
-##
+## Installation
 
     pip install cluster_colors
 
 ## Basic usage
 
 ~~~python
 from cluster_colors import get_image_clusters
```

