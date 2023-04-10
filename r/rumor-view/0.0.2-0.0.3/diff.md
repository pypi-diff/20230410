# Comparing `tmp/rumor_view-0.0.2.tar.gz` & `tmp/rumor_view-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rumor_view-0.0.2.tar", last modified: Mon Apr 10 02:40:43 2023, max compression
+gzip compressed data, was "rumor_view-0.0.3.tar", last modified: Mon Apr 10 05:52:53 2023, max compression
```

## Comparing `rumor_view-0.0.2.tar` & `rumor_view-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-04-10 02:40:43.102229 rumor_view-0.0.2/
--rw-r--r--   0 neo       (1000) neo       (1000)     1658 2023-04-10 02:40:43.102229 rumor_view-0.0.2/PKG-INFO
--rwxr-xr-x   0 neo       (1000) neo       (1000)     1226 2023-04-10 02:40:06.000000 rumor_view-0.0.2/README.md
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-04-10 02:40:43.102229 rumor_view-0.0.2/rumor_view/
--rwxr-xr-x   0 neo       (1000) neo       (1000)       28 2023-04-06 04:35:16.000000 rumor_view-0.0.2/rumor_view/__init__.py
--rwxr-xr-x   0 neo       (1000) neo       (1000)      498 2023-04-06 00:32:35.000000 rumor_view-0.0.2/rumor_view/categoricalization.py
--rwxr-xr-x   0 neo       (1000) neo       (1000)     7439 2023-04-10 02:39:47.000000 rumor_view-0.0.2/rumor_view/view.py
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-04-10 02:40:43.102229 rumor_view-0.0.2/rumor_view.egg-info/
--rw-r--r--   0 neo       (1000) neo       (1000)     1658 2023-04-10 02:40:43.000000 rumor_view-0.0.2/rumor_view.egg-info/PKG-INFO
--rw-r--r--   0 neo       (1000) neo       (1000)      281 2023-04-10 02:40:43.000000 rumor_view-0.0.2/rumor_view.egg-info/SOURCES.txt
--rw-r--r--   0 neo       (1000) neo       (1000)        1 2023-04-10 02:40:43.000000 rumor_view-0.0.2/rumor_view.egg-info/dependency_links.txt
--rw-r--r--   0 neo       (1000) neo       (1000)       34 2023-04-10 02:40:43.000000 rumor_view-0.0.2/rumor_view.egg-info/requires.txt
--rw-r--r--   0 neo       (1000) neo       (1000)       11 2023-04-10 02:40:43.000000 rumor_view-0.0.2/rumor_view.egg-info/top_level.txt
--rw-r--r--   0 neo       (1000) neo       (1000)       38 2023-04-10 02:40:43.102229 rumor_view-0.0.2/setup.cfg
--rwxr-xr-x   0 neo       (1000) neo       (1000)      862 2023-04-10 02:40:28.000000 rumor_view-0.0.2/setup.py
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-04-10 02:40:43.102229 rumor_view-0.0.2/tests/
--rwxr-xr-x   0 neo       (1000) neo       (1000)     3175 2023-04-10 02:16:20.000000 rumor_view-0.0.2/tests/test_view.py
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-04-10 05:52:53.580647 rumor_view-0.0.3/
+-rw-r--r--   0 neo       (1000) neo       (1000)     1658 2023-04-10 05:52:53.580647 rumor_view-0.0.3/PKG-INFO
+-rwxr-xr-x   0 neo       (1000) neo       (1000)     1226 2023-04-10 02:40:06.000000 rumor_view-0.0.3/README.md
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-04-10 05:52:53.580647 rumor_view-0.0.3/rumor_view/
+-rwxr-xr-x   0 neo       (1000) neo       (1000)       28 2023-04-06 04:35:16.000000 rumor_view-0.0.3/rumor_view/__init__.py
+-rwxr-xr-x   0 neo       (1000) neo       (1000)      498 2023-04-06 00:32:35.000000 rumor_view-0.0.3/rumor_view/categoricalization.py
+-rwxr-xr-x   0 neo       (1000) neo       (1000)     7388 2023-04-10 05:47:55.000000 rumor_view-0.0.3/rumor_view/view.py
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-04-10 05:52:53.580647 rumor_view-0.0.3/rumor_view.egg-info/
+-rw-r--r--   0 neo       (1000) neo       (1000)     1658 2023-04-10 05:52:53.000000 rumor_view-0.0.3/rumor_view.egg-info/PKG-INFO
+-rw-r--r--   0 neo       (1000) neo       (1000)      281 2023-04-10 05:52:53.000000 rumor_view-0.0.3/rumor_view.egg-info/SOURCES.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)        1 2023-04-10 05:52:53.000000 rumor_view-0.0.3/rumor_view.egg-info/dependency_links.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)       34 2023-04-10 05:52:53.000000 rumor_view-0.0.3/rumor_view.egg-info/requires.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)       11 2023-04-10 05:52:53.000000 rumor_view-0.0.3/rumor_view.egg-info/top_level.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)       38 2023-04-10 05:52:53.580647 rumor_view-0.0.3/setup.cfg
+-rwxr-xr-x   0 neo       (1000) neo       (1000)      862 2023-04-10 05:51:49.000000 rumor_view-0.0.3/setup.py
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-04-10 05:52:53.580647 rumor_view-0.0.3/tests/
+-rwxr-xr-x   0 neo       (1000) neo       (1000)     3175 2023-04-10 02:16:20.000000 rumor_view-0.0.3/tests/test_view.py
```

### Comparing `rumor_view-0.0.2/PKG-INFO` & `rumor_view-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rumor_view
-Version: 0.0.2
+Version: 0.0.3
 Summary: Visualization of column value relationship
 Home-page: https://github.com/not-so-fat/rumor_view
 Author: @not-so-fat
 Author-email: conjurer.not.so.fat@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rumor_view-0.0.2/README.md` & `rumor_view-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `rumor_view-0.0.2/rumor_view/view.py` & `rumor_view-0.0.3/rumor_view/view.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import copy
 import logging
+import itertools
 import numpy
 from scipy.sparse import csc_array
 import pandas
 import networkx as nx
 from pyvis.network import Network
 
 
@@ -54,25 +55,26 @@
             min_size (float): minimum probability of column value to be considered for lift. default=0.01
             physics (bool): whether to use physics model for visualization results. default=False
         """
         column_summary = self._create_column_summary(min_size)
         if columns is None:
             columns = self.column_names
         column_summary = column_summary[
-            (column_summary["from"].isin(columns))&(column_summary["to"].isin(columns))
+            (column_summary["left"].isin(columns))&(column_summary["right"].isin(columns))
         ]
 
         nxg = nx.Graph()
         for c in columns:
             color = "#fe6708" if c == target_column else "#a7c0f7"
             nxg.add_node(c, title=f"{c}\n cardinality={len(self.index_dict[c])}", color=color)
         for row_ind, row in column_summary.iterrows():
             if row["max(lift)"] >= min_lift:
                 nxg.add_edge(
-                    row["from"], row["to"], title=f'lift={row["max(lift)"]:.1%}', value=row["max(lift)"]
+                    row["left"], row["right"], value=row["max(lift)"], 
+                    title=f'lift={row["max(lift)"]:.1%}'
                 )
         print(f"showing edges with lift >= {min_lift}")
         if target_column:
             nxg = nx.generators.ego_graph(nxg, target_column, n_hops)
             print(f"showing nodes within {n_hops} edges from {target_column}")
         nx_args = _overwrite_dict(NX_OPTIONS_DEFAULT, nx_options)
         g = Network(**nx_args)
@@ -140,33 +142,30 @@
     
     def _extract_matrix_for_2columns(self, df, c1, c2):
         c1_ind = list(self.index_dict[c1].values())
         c2_ind = list(self.index_dict[c2].values())
         return df.iloc[c1_ind, c2_ind]
     
     def _create_column_summary(self, min_size):
-        from_list = []
-        to_list = []
+        left_list = []
+        right_list = []
         lift_list = []
-        for c1 in self.index_dict.keys():
+        for c1, c2 in itertools.combinations(self.index_dict.keys(), 2):
             c1_ind = sorted(self.index_dict[c1].values())
+            c2_ind = sorted(self.index_dict[c2].values())
             c1_nodes = [self.node_names[c] for c in c1_ind if self.node_prob[c] > min_size]
-            for c2 in self.index_dict.keys():
-                if c1 == c2:
-                    continue
-                c2_ind = sorted(self.index_dict[c2].values())
-                c2_nodes = [self.node_names[c] for c in c2_ind if self.node_prob[c] > min_size]
-                lift_df_2c = self.lift_df.loc[c2_nodes, c1_nodes]
-                max_lift = lift_df_2c.max().max()
-                from_list.append(c1)
-                to_list.append(c2)
-                lift_list.append(max_lift)
+            c2_nodes = [self.node_names[c] for c in c2_ind if self.node_prob[c] > min_size]
+            lift_df = self.lift_df.loc[c1_nodes, c2_nodes]
+            max_lift = lift_df.max().max()
+            left_list.append(c1)
+            right_list.append(c2)
+            lift_list.append(max_lift)
         return pandas.DataFrame({
-            "from": from_list,
-            "to": to_list,
+            "left": left_list,
+            "right": right_list,
             "max(lift)": lift_list
         })
     
 
 def _overwrite_dict(d1, d2):
     ret_dict = copy.deepcopy(d1)
     for k, v in d2.items():
```

### Comparing `rumor_view-0.0.2/rumor_view.egg-info/PKG-INFO` & `rumor_view-0.0.3/rumor_view.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rumor-view
-Version: 0.0.2
+Version: 0.0.3
 Summary: Visualization of column value relationship
 Home-page: https://github.com/not-so-fat/rumor_view
 Author: @not-so-fat
 Author-email: conjurer.not.so.fat@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rumor_view-0.0.2/setup.py` & `rumor_view-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     requirements = [str(req) for req in pkg_resources.parse_requirements(f)]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rumor_view",
-    version="0.0.2",
+    version="0.0.3",
     author="@not-so-fat",
     author_email="conjurer.not.so.fat@gmail.com",
     description="Visualization of column value relationship",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/not-so-fat/rumor_view",
     install_requires=requirements,
```

### Comparing `rumor_view-0.0.2/tests/test_view.py` & `rumor_view-0.0.3/tests/test_view.py`

 * *Files identical despite different names*

