# Comparing `tmp/bk_clustering-0.1.tar.gz` & `tmp/bk_clustering-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bk_clustering-0.1.tar", max compression
+gzip compressed data, was "bk_clustering-0.1.1.tar", max compression
```

## Comparing `bk_clustering-0.1.tar` & `bk_clustering-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0        0 2023-03-09 12:14:06.008282 bk_clustering-0.1/README.md
--rw-r--r--   0        0        0   893611 2023-04-09 07:14:20.570222 bk_clustering-0.1/bk_clustering/.ipynb_checkpoints/boxplots-checkpoint.ipynb
--rw-r--r--   0        0        0       40 2023-04-08 23:59:03.211844 bk_clustering-0.1/bk_clustering/__init__.py
--rw-r--r--   0        0        0    33769 2023-03-25 12:39:17.568753 bk_clustering-0.1/bk_clustering/_hierarchy.pyx
--rw-r--r--   0        0        0     9096 2023-04-09 13:38:51.890438 bk_clustering-0.1/bk_clustering/main.py
--rw-r--r--   0        0        0     3635 2023-04-10 13:47:29.443057 bk_clustering-0.1/bk_clustering/run_batch.py
--rw-r--r--   0        0        0        2 2023-04-10 20:34:39.948587 bk_clustering-0.1/bk_clustering/utilities/__init__.py
--rw-r--r--   0        0        0      182 2023-03-28 10:42:47.293233 bk_clustering-0.1/bk_clustering/utilities/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2394 2023-04-08 23:27:42.220376 bk_clustering-0.1/bk_clustering/utilities/__pycache__/calculation_utilities.cpython-310.pyc
--rw-r--r--   0        0        0     4423 2023-04-08 23:26:04.015216 bk_clustering-0.1/bk_clustering/utilities/__pycache__/cluster_calculations.cpython-310.pyc
--rw-r--r--   0        0        0     6256 2023-03-30 17:31:31.888383 bk_clustering-0.1/bk_clustering/utilities/__pycache__/density_peak.cpython-310.pyc
--rw-r--r--   0        0        0     1386 2023-04-03 15:10:41.814013 bk_clustering-0.1/bk_clustering/utilities/__pycache__/ext_linkage_matrix.cpython-310.pyc
--rw-r--r--   0        0        0     1708 2023-03-11 12:30:08.257315 bk_clustering-0.1/bk_clustering/utilities/__pycache__/hutils.cpython-310.pyc
--rw-r--r--   0        0        0     1002 2023-03-11 11:40:12.461914 bk_clustering-0.1/bk_clustering/utilities/__pycache__/hutils_calc.cpython-310.pyc
--rw-r--r--   0        0        0    14683 2023-03-11 11:40:12.469914 bk_clustering-0.1/bk_clustering/utilities/__pycache__/hutils_cluster.cpython-310.pyc
--rw-r--r--   0        0        0     4614 2023-04-08 23:27:42.548380 bk_clustering-0.1/bk_clustering/utilities/__pycache__/hutils_viz.cpython-310.pyc
--rw-r--r--   0        0        0     2108 2023-04-09 21:44:29.698931 bk_clustering-0.1/bk_clustering/utilities/__pycache__/load_save.cpython-310.pyc
--rw-r--r--   0        0        0     9148 2023-04-10 09:17:41.631628 bk_clustering-0.1/bk_clustering/utilities/__pycache__/method_comparison.cpython-310.pyc
--rw-r--r--   0        0        0     7864 2023-04-08 19:37:52.265849 bk_clustering-0.1/bk_clustering/utilities/__pycache__/metrics.cpython-310.pyc
--rw-r--r--   0        0        0     2738 2023-04-04 11:10:14.591320 bk_clustering-0.1/bk_clustering/utilities/__pycache__/preprocessing.cpython-310.pyc
--rw-r--r--   0        0        0     9262 2023-04-08 23:26:04.015216 bk_clustering-0.1/bk_clustering/utilities/__pycache__/tree_traversal.cpython-310.pyc
--rw-r--r--   0        0        0     2012 2023-04-08 23:21:19.153823 bk_clustering-0.1/bk_clustering/utilities/calculation_utilities.py
--rw-r--r--   0        0        0     5154 2023-04-09 13:33:11.001718 bk_clustering-0.1/bk_clustering/utilities/cluster_calculations.py
--rw-r--r--   0        0        0     6955 2023-03-30 17:31:18.984431 bk_clustering-0.1/bk_clustering/utilities/density_peak.py
--rw-r--r--   0        0        0     2953 2023-04-10 14:02:09.832507 bk_clustering-0.1/bk_clustering/utilities/load_save.py
--rw-r--r--   0        0        0    16414 2023-04-10 13:46:07.358769 bk_clustering-0.1/bk_clustering/utilities/method_comparison.py
--rw-r--r--   0        0        0     8236 2023-04-08 19:36:44.802893 bk_clustering-0.1/bk_clustering/utilities/metrics.py
--rw-r--r--   0        0        0     4511 2023-04-09 08:12:54.956531 bk_clustering-0.1/bk_clustering/utilities/plot_utilities.py
--rw-r--r--   0        0        0     2582 2023-04-04 11:10:05.075192 bk_clustering-0.1/bk_clustering/utilities/preprocessing.py
--rw-r--r--   0        0        0    13106 2023-04-09 08:13:24.269397 bk_clustering-0.1/bk_clustering/utilities/tree_traversal.py
--rw-r--r--   0        0        0      439 2023-04-10 20:38:34.309899 bk_clustering-0.1/pyproject.toml
--rw-r--r--   0        0        0      504 1970-01-01 00:00:00.000000 bk_clustering-0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-09 12:14:06.008282 bk_clustering-0.1.1/README.md
+-rw-r--r--   0        0        0   893611 2023-04-09 07:14:20.570222 bk_clustering-0.1.1/bk_clustering/.ipynb_checkpoints/boxplots-checkpoint.ipynb
+-rw-r--r--   0        0        0       40 2023-04-08 23:59:03.211844 bk_clustering-0.1.1/bk_clustering/__init__.py
+-rw-r--r--   0        0        0    33769 2023-03-25 12:39:17.568753 bk_clustering-0.1.1/bk_clustering/_hierarchy.pyx
+-rw-r--r--   0        0        0     9101 2023-04-10 21:45:41.383464 bk_clustering-0.1.1/bk_clustering/main.py
+-rw-r--r--   0        0        0     3635 2023-04-10 13:47:29.443057 bk_clustering-0.1.1/bk_clustering/run_batch.py
+-rw-r--r--   0        0        0        2 2023-04-10 20:34:39.948587 bk_clustering-0.1.1/bk_clustering/utilities/__init__.py
+-rw-r--r--   0        0        0      182 2023-03-28 10:42:47.293233 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2394 2023-04-08 23:27:42.220376 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/calculation_utilities.cpython-310.pyc
+-rw-r--r--   0        0        0     4423 2023-04-08 23:26:04.015216 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/cluster_calculations.cpython-310.pyc
+-rw-r--r--   0        0        0     6256 2023-03-30 17:31:31.888383 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/density_peak.cpython-310.pyc
+-rw-r--r--   0        0        0     1386 2023-04-03 15:10:41.814013 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/ext_linkage_matrix.cpython-310.pyc
+-rw-r--r--   0        0        0     1708 2023-03-11 12:30:08.257315 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/hutils.cpython-310.pyc
+-rw-r--r--   0        0        0     1002 2023-03-11 11:40:12.461914 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/hutils_calc.cpython-310.pyc
+-rw-r--r--   0        0        0    14683 2023-03-11 11:40:12.469914 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/hutils_cluster.cpython-310.pyc
+-rw-r--r--   0        0        0     4614 2023-04-08 23:27:42.548380 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/hutils_viz.cpython-310.pyc
+-rw-r--r--   0        0        0     2108 2023-04-09 21:44:29.698931 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/load_save.cpython-310.pyc
+-rw-r--r--   0        0        0     9148 2023-04-10 09:17:41.631628 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/method_comparison.cpython-310.pyc
+-rw-r--r--   0        0        0     7864 2023-04-08 19:37:52.265849 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/metrics.cpython-310.pyc
+-rw-r--r--   0        0        0     2738 2023-04-04 11:10:14.591320 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/preprocessing.cpython-310.pyc
+-rw-r--r--   0        0        0     9262 2023-04-08 23:26:04.015216 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/tree_traversal.cpython-310.pyc
+-rw-r--r--   0        0        0     2012 2023-04-08 23:21:19.153823 bk_clustering-0.1.1/bk_clustering/utilities/calculation_utilities.py
+-rw-r--r--   0        0        0     5154 2023-04-09 13:33:11.001718 bk_clustering-0.1.1/bk_clustering/utilities/cluster_calculations.py
+-rw-r--r--   0        0        0     6955 2023-03-30 17:31:18.984431 bk_clustering-0.1.1/bk_clustering/utilities/density_peak.py
+-rw-r--r--   0        0        0     2953 2023-04-10 14:02:09.832507 bk_clustering-0.1.1/bk_clustering/utilities/load_save.py
+-rw-r--r--   0        0        0    16414 2023-04-10 13:46:07.358769 bk_clustering-0.1.1/bk_clustering/utilities/method_comparison.py
+-rw-r--r--   0        0        0     8236 2023-04-08 19:36:44.802893 bk_clustering-0.1.1/bk_clustering/utilities/metrics.py
+-rw-r--r--   0        0        0     4511 2023-04-09 08:12:54.956531 bk_clustering-0.1.1/bk_clustering/utilities/plot_utilities.py
+-rw-r--r--   0        0        0     2582 2023-04-04 11:10:05.075192 bk_clustering-0.1.1/bk_clustering/utilities/preprocessing.py
+-rw-r--r--   0        0        0    13106 2023-04-09 08:13:24.269397 bk_clustering-0.1.1/bk_clustering/utilities/tree_traversal.py
+-rw-r--r--   0        0        0      441 2023-04-10 21:46:13.091338 bk_clustering-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 bk_clustering-0.1.1/PKG-INFO
```

### Comparing `bk_clustering-0.1/bk_clustering/.ipynb_checkpoints/boxplots-checkpoint.ipynb` & `bk_clustering-0.1.1/bk_clustering/.ipynb_checkpoints/boxplots-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1/bk_clustering/_hierarchy.pyx` & `bk_clustering-0.1.1/bk_clustering/_hierarchy.pyx`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1/bk_clustering/main.py` & `bk_clustering-0.1.1/bk_clustering/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
                 dtf,
                 cluster_df,
                 cluster_info,
                 node_tree,
             ) = self.calculate_clusters(X, linkage_type=self.linkage)
 
         self.labels_ = list(result_dict.values())
-        self.n_clusters = len(self.labels_)
+        self.n_clusters = len(set(self.labels_))
         self.dtf_ = dtf
         self.cluster_info_ = cluster_info
         self.cluster_df_ = cluster_df
         self.node_tree_ = node_tree
 
         return self
```

### Comparing `bk_clustering-0.1/bk_clustering/run_batch.py` & `bk_clustering-0.1.1/bk_clustering/run_batch.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1/bk_clustering/utilities/__pycache__/calculation_utilities.cpython-310.pyc` & `bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/calculation_utilities.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1/bk_clustering/utilities/__pycache__/cluster_calculations.cpython-310.pyc` & `bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/cluster_calculations.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1/bk_clustering/utilities/__pycache__/density_peak.cpython-310.pyc` & `bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/density_peak.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1/bk_clustering/utilities/__pycache__/ext_linkage_matrix.cpython-310.pyc` & `bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/ext_linkage_matrix.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1/bk_clustering/utilities/__pycache__/hutils.cpython-310.pyc` & `bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/hutils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1/bk_clustering/utilities/__pycache__/hutils_calc.cpython-310.pyc` & `bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/hutils_calc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1/bk_clustering/utilities/__pycache__/hutils_cluster.cpython-310.pyc` & `bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/hutils_cluster.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1/bk_clustering/utilities/__pycache__/hutils_viz.cpython-310.pyc` & `bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/hutils_viz.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1/bk_clustering/utilities/__pycache__/load_save.cpython-310.pyc` & `bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/load_save.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1/bk_clustering/utilities/__pycache__/method_comparison.cpython-310.pyc` & `bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/method_comparison.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1/bk_clustering/utilities/__pycache__/metrics.cpython-310.pyc` & `bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/metrics.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1/bk_clustering/utilities/__pycache__/preprocessing.cpython-310.pyc` & `bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/preprocessing.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1/bk_clustering/utilities/__pycache__/tree_traversal.cpython-310.pyc` & `bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/tree_traversal.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1/bk_clustering/utilities/calculation_utilities.py` & `bk_clustering-0.1.1/bk_clustering/utilities/calculation_utilities.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1/bk_clustering/utilities/cluster_calculations.py` & `bk_clustering-0.1.1/bk_clustering/utilities/cluster_calculations.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1/bk_clustering/utilities/density_peak.py` & `bk_clustering-0.1.1/bk_clustering/utilities/density_peak.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1/bk_clustering/utilities/load_save.py` & `bk_clustering-0.1.1/bk_clustering/utilities/load_save.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1/bk_clustering/utilities/method_comparison.py` & `bk_clustering-0.1.1/bk_clustering/utilities/method_comparison.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1/bk_clustering/utilities/metrics.py` & `bk_clustering-0.1.1/bk_clustering/utilities/metrics.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1/bk_clustering/utilities/plot_utilities.py` & `bk_clustering-0.1.1/bk_clustering/utilities/plot_utilities.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1/bk_clustering/utilities/preprocessing.py` & `bk_clustering-0.1.1/bk_clustering/utilities/preprocessing.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1/bk_clustering/utilities/tree_traversal.py` & `bk_clustering-0.1.1/bk_clustering/utilities/tree_traversal.py`

 * *Files identical despite different names*

