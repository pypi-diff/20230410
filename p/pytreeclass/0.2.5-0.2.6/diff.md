# Comparing `tmp/pytreeclass-0.2.5.tar.gz` & `tmp/pytreeclass-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytreeclass-0.2.5.tar", last modified: Tue Apr  4 12:54:45 2023, max compression
+gzip compressed data, was "pytreeclass-0.2.6.tar", last modified: Mon Apr 10 21:31:08 2023, max compression
```

## Comparing `pytreeclass-0.2.5.tar` & `pytreeclass-0.2.6.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:54:45.217214 pytreeclass-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-04 12:54:31.000000 pytreeclass-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29191 2023-04-04 12:54:45.217214 pytreeclass-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28315 2023-04-04 12:54:31.000000 pytreeclass-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:54:45.213214 pytreeclass-0.2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-04-04 12:54:31.000000 pytreeclass-0.2.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:54:45.213214 pytreeclass-0.2.5/pytreeclass/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-04 12:54:31.000000 pytreeclass-0.2.5/pytreeclass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:54:45.217214 pytreeclass-0.2.5/pytreeclass/_src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 12:54:31.000000 pytreeclass-0.2.5/pytreeclass/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-04-04 12:54:31.000000 pytreeclass-0.2.5/pytreeclass/_src/tree_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-04-04 12:54:31.000000 pytreeclass-0.2.5/pytreeclass/_src/tree_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-04-04 12:54:31.000000 pytreeclass-0.2.5/pytreeclass/_src/tree_freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)    25169 2023-04-04 12:54:31.000000 pytreeclass-0.2.5/pytreeclass/_src/tree_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    31357 2023-04-04 12:54:31.000000 pytreeclass-0.2.5/pytreeclass/_src/tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    13151 2023-04-04 12:54:31.000000 pytreeclass-0.2.5/pytreeclass/_src/tree_trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:54:45.213214 pytreeclass-0.2.5/pytreeclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29191 2023-04-04 12:54:45.000000 pytreeclass-0.2.5/pytreeclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-04 12:54:45.000000 pytreeclass-0.2.5/pytreeclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 12:54:45.000000 pytreeclass-0.2.5/pytreeclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 12:54:45.000000 pytreeclass-0.2.5/pytreeclass.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-04 12:54:45.000000 pytreeclass-0.2.5/pytreeclass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-04 12:54:45.000000 pytreeclass-0.2.5/pytreeclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 12:54:45.217214 pytreeclass-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-04 12:54:31.000000 pytreeclass-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:54:45.217214 pytreeclass-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 12:54:31.000000 pytreeclass-0.2.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17825 2023-04-04 12:54:31.000000 pytreeclass-0.2.5/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-04-04 12:54:31.000000 pytreeclass-0.2.5/tests/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-04-04 12:54:31.000000 pytreeclass-0.2.5/tests/test_tree_freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-04 12:54:31.000000 pytreeclass-0.2.5/tests/test_tree_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17761 2023-04-04 12:54:31.000000 pytreeclass-0.2.5/tests/test_tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-04 12:54:31.000000 pytreeclass-0.2.5/tests/test_tree_viz_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    16518 2023-04-04 12:54:31.000000 pytreeclass-0.2.5/tests/test_treeclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-04 12:54:31.000000 pytreeclass-0.2.5/tests/test_under_jit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:31:08.427071 pytreeclass-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28366 2023-04-10 21:31:08.427071 pytreeclass-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27490 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:31:08.423071 pytreeclass-0.2.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:31:08.423071 pytreeclass-0.2.6/pytreeclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/pytreeclass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:31:08.423071 pytreeclass-0.2.6/pytreeclass/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/pytreeclass/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25031 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/pytreeclass/_src/tree_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/pytreeclass/_src/tree_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25696 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/pytreeclass/_src/tree_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31254 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/pytreeclass/_src/tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13151 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/pytreeclass/_src/tree_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:31:08.423071 pytreeclass-0.2.6/pytreeclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28366 2023-04-10 21:31:08.000000 pytreeclass-0.2.6/pytreeclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-10 21:31:08.000000 pytreeclass-0.2.6/pytreeclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 21:31:08.000000 pytreeclass-0.2.6/pytreeclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 21:31:08.000000 pytreeclass-0.2.6/pytreeclass.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-10 21:31:08.000000 pytreeclass-0.2.6/pytreeclass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-10 21:31:08.000000 pytreeclass-0.2.6/pytreeclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 21:31:08.427071 pytreeclass-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:31:08.427071 pytreeclass-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17904 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/tests/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10145 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/tests/test_tree_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/tests/test_tree_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17761 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/tests/test_tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/tests/test_tree_viz_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/tests/test_treeclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/tests/test_under_jit.py
```

### Comparing `pytreeclass-0.2.5/LICENSE` & `pytreeclass-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.5/PKG-INFO` & `pytreeclass-0.2.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: pytreeclass
-Version: 0.2.5
-Summary: JAX compatible dataclass.
-Home-page: https://github.com/ASEM000/pytreeclass
-Author: Mahmoud Asem
-Author-email: asem00@kaist.ac.kr
-License: Apache-2.0
-Keywords: python machine-learning pytorch jax
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <!-- <h1 align="center" style="font-family:Monospace" >Py🌲Class</h1> -->
 <h5 align="center">
 <img width="250px" src="https://user-images.githubusercontent.com/48389287/227880173-bf78c02c-d28b-4cf4-95e6-fa49b82a43a1.svg"> <br>
 
 <br>
 
 [**Installation**](#installation)
@@ -731,56 +708,56 @@
 
 ```python
 import jax
 import pytreeclass as pytc
 
 tree = [1, [2,3], 4]
 
-print(pytc.tree_diagram(tree,depth=1))
+print(pytc.tree_diagram(tree, depth=1))
 # list
-#     ├── [0]=1
-#     ├── [1]=[..., ...]
-#     └── [2]=4
+# ├── [0]=1
+# ├── [1]=[...]
+# └── [2]=4
 
-print(pytc.tree_diagram(tree,depth=2))
+print(pytc.tree_diagram(tree, depth=2))
 # list
-#     ├── [0]=1
-#     ├── [1]:list
-#     │   ├── [0]=2
-#     │   └── [1]=3
-#     └── [2]=4
-
-
-print(pytc.tree_summary(tree,depth=1))
-# ┌────┬────┬─────┬───────┐
-# │Name│Type│Count│Size   │
-# ├────┼────┼─────┼───────┤
-# │[0] │int │1    │28.00B │
-# ├────┼────┼─────┼───────┤
-# │[1] │list│2    │56.00B │
-# ├────┼────┼─────┼───────┤
-# │[2] │int │1    │28.00B │
-# ├────┼────┼─────┼───────┤
-# │Σ   │list│4    │112.00B│
-# └────┴────┴─────┴───────┘
-
-print(pytc.tree_summary(tree,depth=2))
-# ┌──────┬────┬─────┬───────┐
-# │Name  │Type│Count│Size   │
-# ├──────┼────┼─────┼───────┤
-# │[0]   │int │1    │28.00B │
-# ├──────┼────┼─────┼───────┤
-# │[1][0]│int │1    │28.00B │
-# ├──────┼────┼─────┼───────┤
-# │[1][1]│int │1    │28.00B │
-# ├──────┼────┼─────┼───────┤
-# │[2]   │int │1    │28.00B │
-# ├──────┼────┼─────┼───────┤
-# │Σ     │list│4    │112.00B│
-# └──────┴────┴─────┴───────┘
+# ├── [0]=1
+# ├── [1]:list
+# │   ├── [0]=2
+# │   └── [1]=3
+# └── [2]=4
+
+
+print(pytc.tree_summary(tree, depth=1))
+# ┌────┬────┬─────┐
+# │Name│Type│Count│
+# ├────┼────┼─────┤
+# │[0] │int │1    │
+# ├────┼────┼─────┤
+# │[1] │list│1    │
+# ├────┼────┼─────┤
+# │[2] │int │1    │
+# ├────┼────┼─────┤
+# │Σ   │list│3    │
+# └────┴────┴─────┘
+
+print(pytc.tree_summary(tree, depth=2))
+# ┌──────┬────┬─────┐
+# │Name  │Type│Count│
+# ├──────┼────┼─────┤
+# │[0]   │int │1    │
+# ├──────┼────┼─────┤
+# │[1][0]│int │1    │
+# ├──────┼────┼─────┤
+# │[1][1]│int │1    │
+# ├──────┼────┼─────┤
+# │[2]   │int │1    │
+# ├──────┼────┼─────┤
+# │Σ     │list│4    │
+# └──────┴────┴─────┘
 ```
 
 </details>
 
 <details><summary>Use PyTreeClass components with other libraries</summary>
 
 ```python
@@ -817,34 +794,34 @@
 # FlaxTree(a=1, b=(2.0, 3.0), c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00]))
 
 print(f"{flax_tree!s}")
 # FlaxTree(a=1, b=(2.0, 3.0), c=[4. 5. 6.])
 
 print(pytc.tree_diagram(flax_tree))
 # FlaxTree
-#     ├── a=1
-#     ├── b:tuple
-#     │   ├── [0]=2.0
-#     │   └── [1]=3.0
-#     └── c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
+# ├── a=1
+# ├── b:tuple
+# │   ├── [0]=2.0
+# │   └── [1]=3.0
+# └── c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
 
 print(pytc.tree_summary(flax_tree))
-# ┌────┬────────┬─────┬──────┐
-# │Name│Type    │Count│Size  │
-# ├────┼────────┼─────┼──────┤
-# │a   │int     │1    │28.00B│
-# ├────┼────────┼─────┼──────┤
-# │b[0]│float   │1    │24.00B│
-# ├────┼────────┼─────┼──────┤
-# │b[1]│float   │1    │24.00B│
-# ├────┼────────┼─────┼──────┤
-# │c   │f32[3]  │3    │12.00B│
-# ├────┼────────┼─────┼──────┤
-# │Σ   │FlaxTree│6    │88.00B│
-# └────┴────────┴─────┴──────┘
+# ┌────┬────────┬─────┐
+# │Name│Type    │Count│
+# ├────┼────────┼─────┤
+# │a   │int     │1    │
+# ├────┼────────┼─────┤
+# │b[0]│float   │1    │
+# ├────┼────────┼─────┤
+# │b[1]│float   │1    │
+# ├────┼────────┼─────┤
+# │c   │f32[3]  │3    │
+# ├────┼────────┼─────┤
+# │Σ   │FlaxTree│6    │
+# └────┴────────┴─────┘
 
 flax_tree.at[0].get()
 # FlaxTree(a=1, b=(None, None), c=None)
 
 flax_tree.at["a"].set(10)
 # FlaxTree(a=10, b=(2.0, 3.0), c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00]))
 ```
@@ -905,38 +882,35 @@
 For example for the previous tree, the reuslting trace path for each leaf is :
 
 ### Named tree variant
 
 ```python
 >>> name_tree = pytc.tree_map_with_trace(lambda trace,x : trace[0], tree)
 >>> print(name_tree)
-Tree(a=(Tree, a), b=((Tree, b, [0]), (Tree, b, [1])), c=(Tree, c))
+Tree(a=(a), b=((b, [0]), (b, [1])), c=(c))
 ```
 
 ### Typed tree variant
 
 ```python
 >>> type_tree = pytc.tree_map_with_trace(lambda trace,x : f"{trace[1]!s}", tree)
 >>> print(type_tree)
 Tree(
-  a=(<class '__main__.Tree'>, <class 'int'>),
-  b=(
-    (<class '__main__.Tree'>, <class 'tuple'>, <class 'float'>),
-    (<class '__main__.Tree'>, <class 'tuple'>, <class 'float'>)
-  ),
-  c=(<class '__main__.Tree'>, <class 'jaxlib.xla_extension.ArrayImpl'>)
+  a=(<class 'int'>,),
+  b=((<class 'tuple'>, <class 'float'>), (<class 'tuple'>, <class 'float'>)),
+  c=(<class 'jaxlib.xla_extension.ArrayImpl'>,)
 )
 ```
 
 ### Index tree variant
 
 ```python
 >>> index_tree = pytc.tree_map_with_trace(lambda trace,x : trace[2], tree)
 >>> print(index_tree)
-Tree(a=(0, 0), b=((0, 1, 0), (0, 1, 1)), c=(0, 2))
+Tree(a=(0), b=((1, 0), (1, 1)), c=(2))
 ```
 
 In essence, each leaf contains information about the name path, type path, and indices path. The rules for custom types can be registered using `pytc.register_pytree_node_trace`
 
 </details>
 
 <details>
@@ -953,15 +927,15 @@
 <tr><td align="center">Generated str method</td> <td align="center">✅</td>  <td align="center"></td></tr>
 <tr><td align="center">Generated hash method</td> <td align="center">✅</td>  <td align="center">✅</td></tr>
 <tr><td align="center">Generated eq method</td> <td align="center">✅✅*</td>  <td align="center">✅</td></tr>
 <tr><td align="center">Support slots</td> <td align="center"></td>  <td align="center">✅</td></tr>
 <tr><td align="center">Keyword-only args</td> <td align="center">✅</td>  <td align="center">✅ 3.10+</td></tr>
 <tr><td align="center">Positional-only args</td> <td align="center">✅</td>  <td align="center"></td></tr>
 <tr><td align="center">Frozen instance</td> <td align="center">✅**</td>  <td align="center">✅</td></tr>
-<tr><td align="center">Match args support</td> <td align="center">✅</td>  <td align="center">✅</td></tr>
+<tr><td align="center">Match args support</td> <td align="center"></td>  <td align="center">✅</td></tr>
 <tr><td align="center">Support callbacks</td> <td align="center">✅</td>  <td align="center"></td></tr>
 </table>
 
 </div>
 
 `*` Either compare the whole instance and return `True/False` or treating it leafwise using `treeclass(..., leafwise=True)` and retrurn `Tree(a=True, ....)`
```

### Comparing `pytreeclass-0.2.5/README.md` & `pytreeclass-0.2.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: pytreeclass
+Version: 0.2.6
+Summary: JAX compatible dataclass.
+Home-page: https://github.com/ASEM000/pytreeclass
+Author: Mahmoud Asem
+Author-email: asem00@kaist.ac.kr
+License: Apache-2.0
+Keywords: python machine-learning pytorch jax
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <!-- <h1 align="center" style="font-family:Monospace" >Py🌲Class</h1> -->
 <h5 align="center">
 <img width="250px" src="https://user-images.githubusercontent.com/48389287/227880173-bf78c02c-d28b-4cf4-95e6-fa49b82a43a1.svg"> <br>
 
 <br>
 
 [**Installation**](#installation)
@@ -708,56 +731,56 @@
 
 ```python
 import jax
 import pytreeclass as pytc
 
 tree = [1, [2,3], 4]
 
-print(pytc.tree_diagram(tree,depth=1))
+print(pytc.tree_diagram(tree, depth=1))
 # list
-#     ├── [0]=1
-#     ├── [1]=[..., ...]
-#     └── [2]=4
+# ├── [0]=1
+# ├── [1]=[...]
+# └── [2]=4
 
-print(pytc.tree_diagram(tree,depth=2))
+print(pytc.tree_diagram(tree, depth=2))
 # list
-#     ├── [0]=1
-#     ├── [1]:list
-#     │   ├── [0]=2
-#     │   └── [1]=3
-#     └── [2]=4
-
-
-print(pytc.tree_summary(tree,depth=1))
-# ┌────┬────┬─────┬───────┐
-# │Name│Type│Count│Size   │
-# ├────┼────┼─────┼───────┤
-# │[0] │int │1    │28.00B │
-# ├────┼────┼─────┼───────┤
-# │[1] │list│2    │56.00B │
-# ├────┼────┼─────┼───────┤
-# │[2] │int │1    │28.00B │
-# ├────┼────┼─────┼───────┤
-# │Σ   │list│4    │112.00B│
-# └────┴────┴─────┴───────┘
-
-print(pytc.tree_summary(tree,depth=2))
-# ┌──────┬────┬─────┬───────┐
-# │Name  │Type│Count│Size   │
-# ├──────┼────┼─────┼───────┤
-# │[0]   │int │1    │28.00B │
-# ├──────┼────┼─────┼───────┤
-# │[1][0]│int │1    │28.00B │
-# ├──────┼────┼─────┼───────┤
-# │[1][1]│int │1    │28.00B │
-# ├──────┼────┼─────┼───────┤
-# │[2]   │int │1    │28.00B │
-# ├──────┼────┼─────┼───────┤
-# │Σ     │list│4    │112.00B│
-# └──────┴────┴─────┴───────┘
+# ├── [0]=1
+# ├── [1]:list
+# │   ├── [0]=2
+# │   └── [1]=3
+# └── [2]=4
+
+
+print(pytc.tree_summary(tree, depth=1))
+# ┌────┬────┬─────┐
+# │Name│Type│Count│
+# ├────┼────┼─────┤
+# │[0] │int │1    │
+# ├────┼────┼─────┤
+# │[1] │list│1    │
+# ├────┼────┼─────┤
+# │[2] │int │1    │
+# ├────┼────┼─────┤
+# │Σ   │list│3    │
+# └────┴────┴─────┘
+
+print(pytc.tree_summary(tree, depth=2))
+# ┌──────┬────┬─────┐
+# │Name  │Type│Count│
+# ├──────┼────┼─────┤
+# │[0]   │int │1    │
+# ├──────┼────┼─────┤
+# │[1][0]│int │1    │
+# ├──────┼────┼─────┤
+# │[1][1]│int │1    │
+# ├──────┼────┼─────┤
+# │[2]   │int │1    │
+# ├──────┼────┼─────┤
+# │Σ     │list│4    │
+# └──────┴────┴─────┘
 ```
 
 </details>
 
 <details><summary>Use PyTreeClass components with other libraries</summary>
 
 ```python
@@ -794,34 +817,34 @@
 # FlaxTree(a=1, b=(2.0, 3.0), c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00]))
 
 print(f"{flax_tree!s}")
 # FlaxTree(a=1, b=(2.0, 3.0), c=[4. 5. 6.])
 
 print(pytc.tree_diagram(flax_tree))
 # FlaxTree
-#     ├── a=1
-#     ├── b:tuple
-#     │   ├── [0]=2.0
-#     │   └── [1]=3.0
-#     └── c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
+# ├── a=1
+# ├── b:tuple
+# │   ├── [0]=2.0
+# │   └── [1]=3.0
+# └── c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
 
 print(pytc.tree_summary(flax_tree))
-# ┌────┬────────┬─────┬──────┐
-# │Name│Type    │Count│Size  │
-# ├────┼────────┼─────┼──────┤
-# │a   │int     │1    │28.00B│
-# ├────┼────────┼─────┼──────┤
-# │b[0]│float   │1    │24.00B│
-# ├────┼────────┼─────┼──────┤
-# │b[1]│float   │1    │24.00B│
-# ├────┼────────┼─────┼──────┤
-# │c   │f32[3]  │3    │12.00B│
-# ├────┼────────┼─────┼──────┤
-# │Σ   │FlaxTree│6    │88.00B│
-# └────┴────────┴─────┴──────┘
+# ┌────┬────────┬─────┐
+# │Name│Type    │Count│
+# ├────┼────────┼─────┤
+# │a   │int     │1    │
+# ├────┼────────┼─────┤
+# │b[0]│float   │1    │
+# ├────┼────────┼─────┤
+# │b[1]│float   │1    │
+# ├────┼────────┼─────┤
+# │c   │f32[3]  │3    │
+# ├────┼────────┼─────┤
+# │Σ   │FlaxTree│6    │
+# └────┴────────┴─────┘
 
 flax_tree.at[0].get()
 # FlaxTree(a=1, b=(None, None), c=None)
 
 flax_tree.at["a"].set(10)
 # FlaxTree(a=10, b=(2.0, 3.0), c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00]))
 ```
@@ -882,38 +905,35 @@
 For example for the previous tree, the reuslting trace path for each leaf is :
 
 ### Named tree variant
 
 ```python
 >>> name_tree = pytc.tree_map_with_trace(lambda trace,x : trace[0], tree)
 >>> print(name_tree)
-Tree(a=(Tree, a), b=((Tree, b, [0]), (Tree, b, [1])), c=(Tree, c))
+Tree(a=(a), b=((b, [0]), (b, [1])), c=(c))
 ```
 
 ### Typed tree variant
 
 ```python
 >>> type_tree = pytc.tree_map_with_trace(lambda trace,x : f"{trace[1]!s}", tree)
 >>> print(type_tree)
 Tree(
-  a=(<class '__main__.Tree'>, <class 'int'>),
-  b=(
-    (<class '__main__.Tree'>, <class 'tuple'>, <class 'float'>),
-    (<class '__main__.Tree'>, <class 'tuple'>, <class 'float'>)
-  ),
-  c=(<class '__main__.Tree'>, <class 'jaxlib.xla_extension.ArrayImpl'>)
+  a=(<class 'int'>,),
+  b=((<class 'tuple'>, <class 'float'>), (<class 'tuple'>, <class 'float'>)),
+  c=(<class 'jaxlib.xla_extension.ArrayImpl'>,)
 )
 ```
 
 ### Index tree variant
 
 ```python
 >>> index_tree = pytc.tree_map_with_trace(lambda trace,x : trace[2], tree)
 >>> print(index_tree)
-Tree(a=(0, 0), b=((0, 1, 0), (0, 1, 1)), c=(0, 2))
+Tree(a=(0), b=((1, 0), (1, 1)), c=(2))
 ```
 
 In essence, each leaf contains information about the name path, type path, and indices path. The rules for custom types can be registered using `pytc.register_pytree_node_trace`
 
 </details>
 
 <details>
@@ -930,15 +950,15 @@
 <tr><td align="center">Generated str method</td> <td align="center">✅</td>  <td align="center"></td></tr>
 <tr><td align="center">Generated hash method</td> <td align="center">✅</td>  <td align="center">✅</td></tr>
 <tr><td align="center">Generated eq method</td> <td align="center">✅✅*</td>  <td align="center">✅</td></tr>
 <tr><td align="center">Support slots</td> <td align="center"></td>  <td align="center">✅</td></tr>
 <tr><td align="center">Keyword-only args</td> <td align="center">✅</td>  <td align="center">✅ 3.10+</td></tr>
 <tr><td align="center">Positional-only args</td> <td align="center">✅</td>  <td align="center"></td></tr>
 <tr><td align="center">Frozen instance</td> <td align="center">✅**</td>  <td align="center">✅</td></tr>
-<tr><td align="center">Match args support</td> <td align="center">✅</td>  <td align="center">✅</td></tr>
+<tr><td align="center">Match args support</td> <td align="center"></td>  <td align="center">✅</td></tr>
 <tr><td align="center">Support callbacks</td> <td align="center">✅</td>  <td align="center"></td></tr>
 </table>
 
 </div>
 
 `*` Either compare the whole instance and return `True/False` or treating it leafwise using `treeclass(..., leafwise=True)` and retrurn `Tree(a=True, ....)`
```

### Comparing `pytreeclass-0.2.5/docs/conf.py` & `pytreeclass-0.2.6/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,22 +46,20 @@
 extensions = [
     "sphinx_copybutton",
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
     "sphinx.ext.doctest",
     "sphinx.ext.inheritance_diagram",
     "sphinx.ext.intersphinx",
-    "sphinx.ext.linkcode",
     "sphinx.ext.napoleon",
-    # "sphinxcontrib.bibtex",
+    "sphinx.ext.viewcode",
     "sphinxcontrib.katex",
     "sphinx_autodoc_typehints",
     "nbsphinx",
     "IPython.sphinxext.ipython_console_highlighting",
-    "sphinxcontrib.mermaid",
 ]
 
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
```

### Comparing `pytreeclass-0.2.5/pytreeclass/__init__.py` & `pytreeclass-0.2.6/pytreeclass/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from pytreeclass._src.tree_base import is_tree_equal, treeclass
-from pytreeclass._src.tree_decorator import field, fields, is_treeclass
+from pytreeclass._src.tree_decorator import field, fields, is_treeclass, treeclass
 from pytreeclass._src.tree_freeze import (
     ImmutableWrapper,
     freeze,
     is_frozen,
     is_nondiff,
     unfreeze,
 )
-from pytreeclass._src.tree_indexer import bcmap, tree_indexer
+from pytreeclass._src.tree_indexer import bcmap, is_tree_equal, tree_indexer
 from pytreeclass._src.tree_pprint import (
     tree_diagram,
     tree_indent,
     tree_mermaid,
     tree_repr,
     tree_repr_with_trace,
     tree_str,
@@ -51,8 +50,8 @@
     "register_pytree_node_trace",
     "tree_map_with_trace",
     "tree_leaves_with_trace",
     "tree_flatten_with_trace",
     "tree_repr_with_trace",
 )
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
```

### Comparing `pytreeclass-0.2.5/pytreeclass/_src/tree_decorator.py` & `pytreeclass-0.2.6/pytreeclass/_src/tree_decorator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,107 +1,124 @@
 from __future__ import annotations
 
-import copy
 import functools as ft
 import sys
-from collections import defaultdict
-from contextlib import contextmanager
+from contextlib import suppress
 from types import FunctionType, MappingProxyType
-from typing import Any, Callable, Mapping, NamedTuple, Sequence, TypeVar
+from typing import Any, Callable, NamedTuple, Sequence, TypeVar
+
+import jax.tree_util as jtu
+from typing_extensions import dataclass_transform
+
+from pytreeclass._src.tree_freeze import ImmutableWrapper, tree_hash
+from pytreeclass._src.tree_indexer import (
+    _conditional_mutable_method,
+    _leafwise_transform,
+    _mutable_context,
+    is_tree_equal,
+    tree_copy,
+    tree_indexer,
+)
+from pytreeclass._src.tree_pprint import tree_repr, tree_str
+from pytreeclass._src.tree_trace import register_pytree_node_trace
 
 _NOT_SET = type("NOT_SET", (), {"__repr__": lambda _: "?"})()
 _MUTABLE_TYPES = (list, dict, set)
 _ANNOTATIONS = "__annotations__"
 _POST_INIT = "__post_init__"
-_MUTABLE = "__mutable__"
+_VARS = "__dict__"
+_FIELD_MAP = "__field_map__"
 T = TypeVar("T")
 
-PyTree = Any
 
+PyTree = Any
 
-"""Define custom frozen `dataclasses.dataclass`-like decorator"""
-# similar to dataclass decorator for init code generation
-# the motivation for writing this is to avoid the need to use dataclasses
-# especially after this update https://github.com/google/jax/issues/14295
-# in essence, after this upadte jax arrays are considred mutable by the field logic
-
-
-# A registry to store the fields of the `treeclass` wrapped classes. fields are a similar concept to
-# `dataclasses.Field` but with the addition of `callbacks` attribute
-# While `dataclasses` fields are added as a class attribute to the class under `__dataclass_fields__`
-# in this implementation, the fields are stored in a `defaultdict` as an extra precaution
-# to avoid user-side modification of the fields while maintaining a cleaner namespace
-_field_registry: dict[type, Mapping[str, Field]] = defaultdict(dict)
-
-
-def register_pytree_field_map(klass: type[T], field_map: Mapping[str, Field]) -> None:
-    # register the field map of a class to the registry
-    # field map is a mapping of field name to `Field` object
-    # the fields are used to generate the `__init__`, `__str__`, `__repr__` functions
-    # and to define the leaves in `tree_flatten` and `tree_unflatten` functions
-    _field_registry[klass].update(field_map)
-
-
-def ovars(obj: Any) -> dict[str, Any]:
-    """Returns a dictionary of the object's attributes."""
-    return object.__getattribute__(obj, "__dict__")
+"""Define a class decorator that is compatible with JAX's transformation."""
 
 
 def is_treeclass(item: Any) -> bool:
-    """Returns `True` if a class or instance is a `treeclass`."""
-    klass = item if isinstance(item, type) else type(item)
-    return klass in _field_registry
+    """Returns `True` if an instance of class is decorated by `treeclass`"""
+    return hasattr(item, _FIELD_MAP)
 
 
 class Field(NamedTuple):
-    # Immutable version of dataclasses.Field
-    # with the addition `callbacks` attributes
     name: str | None = None
     type: type | None = None
     default: Any = _NOT_SET
     factory: Any = None
     init: bool = True
     repr: bool = True
     kw_only: bool = False
     pos_only: bool = False
     metadata: MappingProxyType[str, Any] | None = None
     callbacks: Sequence[Any] = ()
+    alias: str | None = None
+
+    def __hash__(self) -> int:
+        return tree_hash(self)
 
 
 def field(
     *,
     default: Any = _NOT_SET,
     factory: Callable | None = None,
     init: bool = True,
     repr: bool = True,
     kw_only: bool = False,
     pos_only: bool = False,
     metadata: dict[str, Any] | None = None,  # type: ignore
     callbacks: Sequence[Any] = (),
+    alias: str | None = None,
 ) -> Field:
     """
     Args:
         default: The default value of the field. Mutually exclusive with `factory`.
         factory: A 0-argument function called to initialize field value. Mutually exclusive with `default`.
         init: Whether the field is included in the object's __init__ function.
         repr: Whether the field is included in the object's __repr__ function.
         kw_only: Whether the field is keyword-only. Mutually exclusive with `pos_only`.
         pos_only: Whether the field is positional-only. Mutually exclusive with `kw_only`.
         metadata: A mapping of user-defined data for the field.
         callbacks: A sequence of functions to called on `setattr` during initialization to modify the field value.
+        alias: An a alias for the field name in the constructor.
 
     Example:
         >>> import pytreeclass as pytc
+        >>> def instance_cb_factory(klass):
+        ...    def wrapper(x):
+        ...        assert isinstance(x, klass)
+        ...        return x
+        ...    return wrapper
+
+
+        >>> def positive_check_callback(x):
+        ...    assert x > 0
+        ...    return x
+
         >>> @pytc.treeclass
-        ... class Foo:
-        ...     x: int = pytc.field(callbacks=[lambda x: x + 1])  # value is incremented by 1 after initialization
-        >>> foo = Foo(x=1)
-        >>> foo.x
-        2
+        ... class Employee:
+        ...    # assert employee `name` is str
+        ...    name: str = pytc.field(callbacks=[instance_cb_factory(str)])
+        ...    # use callback compostion to assert employee `age` is int and positive
+        ...    age: int = pytc.field(callbacks=[instance_cb_factory(int), positive_check_callback])
+        ...    # use `id` in the constructor for `_id` attribute
+        ...    # this is useful for private attributes that are not supposed to be accessed directly
+        ...    # and hide it from the repr, also add extra info for this field
+        ...    _id: int = pytc.field(alias="id", repr=False)
+
+        >>> tree = Employee(name="Asem", age=10, id=1)
+        >>> print(tree)  # _id is not shown
+        Employee(name=Asem, age=10)
+        >>> assert tree._id == 1  # this is the private attribute
     """
+    if not isinstance(alias, (str, type(None))):
+        msg = "`alias` must be a string or None, "
+        msg += f"got type=`{type(alias).__name__}` instead."
+        raise TypeError(msg)
+
     if default is not _NOT_SET and factory is not None:
         # mutually exclusive arguments
         # this is the similar behavior to `dataclasses`
         msg = "`default` and `factory` are mutually exclusive arguments."
         msg += f"got default={default} and factory={factory}"
         raise ValueError(msg)
 
@@ -136,38 +153,43 @@
         factory=factory,
         init=init,
         repr=repr,
         kw_only=kw_only,
         pos_only=pos_only,
         metadata=metadata,  # type: ignore
         callbacks=callbacks,
+        alias=alias,
     )
 
 
 def fields(item: Any) -> Sequence[Field]:
     """Get the fields of a `treeclass` instance."""
-    if (klass := item if isinstance(item, type) else type(item)) not in _field_registry:
+    if not hasattr(item, _FIELD_MAP):
         raise TypeError(f"Cannot get fields of {item!r}.")
 
-    return tuple(_field_registry[klass].values())
+    return tuple(vars(item)[_FIELD_MAP].values())
 
 
+@ft.lru_cache
 def _generate_field_map(klass: type) -> dict[str, Field]:
     # get all the fields of the class and its base classes
     # get the fields of the class and its base classes
     field_map = dict()
 
-    for base in reversed(klass.__mro__):
+    if klass is object:
+        # base case for recursion to stop
+        return field_map
+
+    for base in reversed(klass.__mro__[1:]):
         # get the fields of the base class in the MRO
         # in reverse order to ensure the correct order of the fields
         # are preserved, i.e. the fields of the base class are added first
         # and the fields of the derived class are added last so that
         # in case of name collision, the derived class fields are preserved
-        if base in _field_registry:
-            field_map.update(_field_registry[base])
+        field_map.update(_generate_field_map(base))
 
     # transform the annotated attributes of the class into Fields
     # while assigning the default values of the Fields to the annotated attributes
     # TODO: use inspect to get annotations, once we are on minimum python version >3.9
     if _ANNOTATIONS not in vars(klass):
         return field_map
 
@@ -231,39 +253,40 @@
     # generate the init method code string
     # in here, we generate the function head and body and add `default`/`factory`
     # for example, if we have a class with fields `x` and `y`
     # then generated code will something like  `def __init__(self, x, y): self.x = x; self.y = y`
     head = body = ""
 
     for field in fields:
-        key = field.name
+        name = field.name  # name in body
+        alias = field.alias or name  # name in constructor
 
-        mark0 = f"field_map['{key}'].default"
-        mark1 = f"field_map['{key}'].factory()"
-        mark2 = f"self.{key}"
+        mark0 = f"field_map['{name}'].default"
+        mark1 = f"field_map['{name}'].factory()"
+        mark2 = f"self.{name}"
 
         if field.kw_only and "*" not in head and field.init:
             # if the field is keyword only, and we have not added the `*` yet
             head += "*, "
 
         if field.default is not _NOT_SET:
             # we add the default into the function head (def f(.. x= default_value))
             # if the the field require initialization. if not, then omit it from head
-            head += f"{key}={mark0}, " if field.init else ""
+            head += f"{alias}={mark0}, " if field.init else ""
             # we then add self.x = x for the body function if field is initialized
             # otherwise, define the default value inside the body ( self.x = default_value)
-            body += f"\t\t{mark2}=" + (f"{key}\n " if field.init else f"{mark0}\n")
+            body += f"\t\t{mark2}=" + (f"{alias}\n " if field.init else f"{mark0}\n")
         elif field.factory is not None:
             # same story for functions as above
-            head += f"{key}={mark1}, " if field.init else ""
-            body += f"\t\t{mark2}=" + (f"{key}\n" if field.init else f"{mark1}\n")
+            head += f"{alias}={mark1}, " if field.init else ""
+            body += f"\t\t{mark2}=" + (f"{alias}\n" if field.init else f"{mark1}\n")
         else:
             # no defaults are added
-            head += f"{key}, " if field.init else ""
-            body += f"\t\t{mark2}={key}\n " if field.init else ""
+            head += f"{alias}, " if field.init else ""
+            body += f"\t\t{mark2}={alias}\n " if field.init else ""
 
         if field.pos_only and field.init:
             # if the field is positional only, we add a "/" marker after it
             if "/" in head:
                 head = head.replace("/,", "")
 
             head += "/, "
@@ -296,82 +319,300 @@
         globals=global_namespace,
         name=method.__name__,
         argdefs=method.__defaults__,
         closure=method.__closure__,
     )
 
 
-@contextmanager
-def _mutable_context(tree: PyTree, *, kopy: bool = False):
-    tree = copy.copy(tree) if kopy else tree
-    ovars(tree)[_MUTABLE] = True
-    yield tree
-    ovars(tree).pop(_MUTABLE, None)
-
-
-def _setattr(self: PyTree, key: str, value: Any) -> None:
-    if _MUTABLE not in ovars(self):
-        # default behavior for frozen instances
-        msg = f"Cannot set {key}={value!r}. Use `.at['{key}'].set({value!r})` instead."
-        raise AttributeError(msg)
-
-    if key in _field_registry[type(self)]:
+@_conditional_mutable_method
+def _setattr(tree: PyTree, key: str, value: Any) -> None:
+    # setattr under `_mutable_context` context otherwise raise an error
+    if key in (field_map := vars(tree)[_FIELD_MAP]):
         # apply the callbacks on setting the value
         # check if the key is a field name
-        for callback in _field_registry[type(self)][key].callbacks:
+        for callback in field_map[key].callbacks:
             try:
                 # callback is a function that takes the value of the field
                 # and returns a modified value
                 value = callback(value)
             except Exception as e:
                 msg = f"Error for field=`{key}`:\n{e}"
                 raise type(e)(msg)
 
-    # set the value
-    ovars(self)[key] = value  # type: ignore
-
-
-def _delattr(self, key: str) -> None:
-    # Delete the attribute if tree is not frozen
-    if _MUTABLE not in ovars(self):
-        raise AttributeError(f"Cannot delete {key}.")
-    del ovars(self)[key]
+    if is_treeclass(value):
+        # auto registers the instance value if it is a registered `treeclass`
+        # this behavior is similar to PyTorch behavior in `nn.Module`
+        # with instances of `Parameter`/`Module`.
+        # the behavior is useful to avoid repetitive code pattern in field definition and
+        # and initialization inside init method.
+        F = Field(type=type(value), init=False, name=key)
+        vars(tree)[_FIELD_MAP] = {**vars(tree)[_FIELD_MAP], **{key: F}}
+
+    vars(tree)[key] = value  # type: ignore
+
+
+@_conditional_mutable_method
+def _delattr(tree, key: str) -> None:
+    # delete the attribute under `_mutable_context` context
+    # otherwise raise an error
+    del vars(tree)[key]
 
 
 def _init_wrapper(init_func: Callable) -> Callable:
     @ft.wraps(init_func)
-    def wrapper(self, *a, **k) -> None:
-        with _mutable_context(self):
-            output = init_func(self, *a, **k)
+    def wrapper(tree, *a, **k) -> None:
+        with _mutable_context(tree):
+            vars(tree)[_FIELD_MAP] = dict(_generate_field_map(type(tree)))
+            output = init_func(tree, *a, **k)
 
-            if post_init_func := getattr(type(self), _POST_INIT, None):
+            if post_init_func := getattr(type(tree), _POST_INIT, None):
                 # to simplify the logic, we call the post init method
                 # even if the init method is not code-generated.
-                post_init_func(self)
+                post_init_func(tree)
 
         # handle non-initialized fields
-        if len(keys := set(_field_registry[type(self)]) - set(ovars(self))) > 0:
+        if len(keys := set(vars(tree)[_FIELD_MAP]) - set(vars(tree))) > 0:
             msg = f"Uninitialized fields: ({', '.join(keys)}) "
-            msg += f"in class `{type(self).__name__}`"
+            msg += f"in class `{type(tree).__name__}`"
             raise AttributeError(msg)
-
-        if wrapper.has_run is False:
-            # handle instance variables of registered types once per class
-            wrapper.has_run = True
-            # auto registers the instance value if it is a registered `treeclass`
-            # this behavior is similar to PyTorch behavior in `nn.Module`
-            # with `Parameter` class. where registered classes are equivalent to nn.Parameter.
-            # the behavior is useful to avoid repetitive code pattern in field definition and
-            # and initialization inside init method.
-            for key in ovars(self):
-                if (
-                    key not in _field_registry[type(self)]
-                    and type(value := ovars(self)[key]) in _field_registry
-                ):
-                    # register the field with `init=False`.the field is not part of
-                    # the init method signature, but defined in the `__post_init__` method
-                    field = Field(name=key, type=type(value), init=False)
-                    register_pytree_field_map(type(self), {key: field})
         return output
 
-    wrapper.has_run = False
     return wrapper
+
+
+def _tree_unflatten(klass: type, treedef: Any, leaves: list[Any]):
+    """Unflatten rule for `treeclass` to use with `jax.tree_unflatten`."""
+    tree = object.__new__(klass)
+    # update through vars, to avoid calling the `setattr` method
+    # that will check for callbacks.
+    # calling `setattr` will trigger any defined callbacks by the user
+    # on each unflattening which is not efficient.
+    # however it might be useful to constantly check if the updated value is
+    # satisfying the constraints defined by the user in the callbacks.
+    vars(tree).update(treedef[1])
+    vars(tree).update(zip(treedef[0], leaves))
+    return tree
+
+
+def _tree_flatten(tree: PyTree):
+    """Flatten rule for `treeclass` to use with `jax.tree_flatten`."""
+    static, dynamic = dict(vars(tree)), dict()
+    for key in static[_FIELD_MAP]:
+        dynamic[key] = static.pop(key)
+    return list(dynamic.values()), (tuple(dynamic.keys()), static)
+
+
+def _tree_trace(tree: PyTree) -> list[tuple[Any, Any, Any, Any]]:
+    """Trace flatten rule to be used with the `tree_trace` module."""
+    leaves, (keys, _) = _tree_flatten(tree)
+    names = (f"{key}" for key in keys)
+    types = map(type, leaves)
+    indices = range(len(leaves))
+    metadatas = (dict(repr=F.repr, id=id(getattr(tree, F.name))) for F in fields(tree))  # type: ignore
+    return [*zip(names, types, indices, metadatas)]
+
+
+def _register_treeclass(klass: type[T]) -> type[T]:
+    with suppress(ValueError):
+        # `ValueError` is raised for duplicate registration.
+        # there are two cases where a class is registered more than once:
+        # first, when a class is decorated with `treeclass` more than once (e.g. `treeclass(treeclass(Class))`)
+        # second when a class is decorated with `treeclass` and has a parent class that is decorated with `treeclass`
+        # in that case `__init_subclass__` registers the class before the decorator registers it.
+        # this can be also be done using metaclass that registers the class on initialization
+        # but we are trying to stay away from deep magic.
+        # register the trace flatten rule
+        register_pytree_node_trace(klass, _tree_trace)
+        # register the flatten/unflatten rules with jax
+        jtu.register_pytree_node(klass, _tree_flatten, ft.partial(_tree_unflatten, klass))  # type: ignore
+
+    return klass
+
+
+def _tree_unwrap(value: Any) -> Any:
+    # enables the transparent wrapper behavior iniside `treeclass` wrapped classes
+    def is_leaf(x: Any) -> bool:
+        return isinstance(x, ImmutableWrapper) or is_treeclass(x)
+
+    def unwrap(value: Any) -> Any:
+        return value.unwrap() if isinstance(value, ImmutableWrapper) else value
+
+    return jtu.tree_map(unwrap, value, is_leaf=is_leaf)
+
+
+def _getattribute_wrapper(getattribute_method: Callable[[T, str], Any]):
+    # this current approach replaces the older metdata based approach
+    # that is used in `dataclasses`-based libraries like `flax.struct.dataclass` and v0.1 of `treeclass`.
+    # the metadata approach is defined at class variable and can not be changed at runtime while the current
+    # approach is more flexible because it can be changed at runtime using `tree_map` or by using `at`
+    # moreover, metadata-based approach falls short when handling nested data structures values.
+    # for example if a field value is a tuple of (1, 2, 3), then metadata-based approach will only be able
+    # to freeze the whole tuple, but not its elements.
+    # with the current approach, we can use `tree_map`/ or direct application to freeze certain tuple elements
+    # and leave the rest of the tuple as is.
+    # another pro of the current approach is that the field metadata is not checked during flattening/unflattening
+    # so in essence, it's more efficient than the metadata-based approach during applying `jax` transformations
+    # that flatten/unflatten the tree.
+    # Example: when fetching `tree.a` it will be unwrapped
+    # >>> @pytc.treeclass
+    # ... class Tree:
+    # ...    a:int = pytc.freeze(1)
+    # >>> tree = Tree()
+    # >>> tree
+    # Tree(a=#1)  # frozen value is displayed in the repr with a prefix `#`
+    # >>> tree.a
+    # 1  # the value is unwrapped when accessed directly
+    @ft.wraps(getattribute_method)
+    def wrapper(tree, key: str) -> Any:
+        value = getattribute_method(tree, key)
+        return _tree_unwrap(value) if key in getattribute_method(tree, _VARS) else value
+
+    return wrapper
+
+
+def _init_subclass_wrapper(init_subclass_method: Callable) -> Callable:
+    # Non-decorated subclasses uses the base `treeclass` leaves only
+    # this behavior is aligned with `dataclasses` not registering non-decorated
+    # subclasses dataclass fields. for example:
+    # >>> @treeclass
+    # ... class A:
+    # ...   a:int=1
+    # >>> class B(A):
+    # ...    b:int=2
+    # >>> tree = B()
+    # >>> jax.tree_leaves(tree)
+    # [1]
+    # however if we decorate `B` with `treeclass` then the fields of `B` will be registered as leaves
+    # >>> @treeclass
+    # ... class B(A):
+    # ...    b:int=2
+    # >>> tree = B()
+    # >>> jax.tree_leaves(tree)
+    # [1, 2]
+    # this behavior is different from `flax.struct.dataclass`
+    # as it does not register non-decorated subclasses field that inherited from decorated subclasses.
+    @classmethod  # type: ignore
+    @ft.wraps(init_subclass_method)
+    def wrapper(klass: type, *a, **k) -> None:
+        init_subclass_method(*a, **k)
+        _register_treeclass(klass)
+
+    return wrapper
+
+
+def _treeclass_transform(klass: type[T]) -> type[T]:
+    # the method is called after registering the class with `_register_treeclass`
+    # cached to prevent wrapping the same class multiple times
+
+    for key, method in (("__setattr__", _setattr), ("__delattr__", _delattr)):
+        # basic required methods
+        if key in vars(klass):
+            if vars(klass)[key] is method:
+                return klass  # already transformed
+            # the user defined a method that conflicts with the required method
+            msg = f"Unable to transform the class `{klass.__name__}` with {key} method defined."
+            raise TypeError(msg)
+        setattr(klass, key, method)
+
+    if "__init__" not in vars(klass):
+        # generate the init method in case it is not defined by the user
+        setattr(klass, "__init__", _generate_init(klass))
+
+    for key, wrapper in (
+        ("__init__", _init_wrapper),
+        ("__init_subclass__", _init_subclass_wrapper),
+        ("__getattribute__", _getattribute_wrapper),
+    ):
+        # wrappers to enable the field initialization,
+        # callback functionality and transparent wrapper behavior
+        setattr(klass, key, wrapper(getattr(klass, key)))
+
+    # basic optional methods
+    for key, method in (
+        ("__repr__", tree_repr),
+        ("__str__", tree_str),
+        ("__copy__", tree_copy),
+        ("__hash__", tree_hash),
+        ("__eq__", is_tree_equal),
+        ("at", property(tree_indexer)),
+    ):
+        if key not in vars(klass):
+            # keep the original method if it is defined by the user
+            # this behavior similar is to `dataclasses.dataclass`
+            setattr(klass, key, method)
+
+    return klass
+
+
+@dataclass_transform(field_specifiers=(field, Field))
+def treeclass(klass: type[T], *, leafwise: bool = False) -> type[T]:
+    """Convert a class to a JAX compatible tree structure.
+
+    Args:
+        klass: class to be converted to a `treeclass`
+        leafwise: Wether to generate leafwise math operations methods. Defaults to `False`.
+
+    Example:
+        >>> import functools as ft
+        >>> import jax
+        >>> import pytreeclass as pytc
+
+        >>> # Tree leaves are defined by type hinted fields at the class level
+        >>> @pytc.treeclass
+        ... class Tree:
+        ...     a:int = 1
+        ...     b:float = 2.0
+        >>> tree = Tree()
+        >>> jax.tree_util.tree_leaves(tree)
+        [1, 2.0]
+
+        >>> # Leaf-wise math operations are supported by setting `leafwise=True`
+        >>> @ft.partial(pytc.treeclass, leafwise=True)
+        ... class Tree:
+        ...     a:int = 1
+        ...     b:float = 2.0
+        >>> tree = Tree()
+        >>> tree + 1
+        Tree(a=2, b=3.0)
+
+        >>> # Advanced indexing is supported using `at` property
+        >>> @pytc.treeclass
+        ... class Tree:
+        ...     a:int = 1
+        ...     b:float = 2.0
+        >>> tree = Tree()
+        >>> tree.at[0].get()
+        Tree(a=1, b=None)
+        >>> tree.at["a"].get()
+        Tree(a=1, b=None)
+
+    Note:
+        Indexing is supported for {`list`, `tuple`, `dict`, `defaultdict`, `OrderedDict`, `namedtuple`}
+        and `treeclass` wrapped classes.
+
+        Extending indexing to other types is possible by registering the type with
+        `pytreeclass.register_pytree_node_trace`
+
+    Note:
+        `leafwise`=True adds the following methods to the class:
+        .. code-block:: python
+            '__add__', '__and__', '__ceil__', '__divmod__', '__eq__', '__floor__', '__floordiv__',
+            '__ge__', '__gt__', '__invert__', '__le__', '__lshift__', '__lt__',
+            '__matmul__', '__mod__', '__mul__', '__ne__', '__neg__', '__or__', '__pos__',
+            '__pow__', '__radd__', '__rand__', '__rdivmod__', '__reduce__', '__rfloordiv__',
+            '__rlshift__', '__rmatmul__', '__rmod__', '__rmul__', '__ror__', '__round__', '__rpow__',
+            '__rrshift__', '__rshift__', '__rsub__', '__rtruediv__', '__rxor__', '__sub__',
+            '__truediv__', '__trunc__', '__xor__',
+
+    Raises:
+        TypeError: if the input is not a class.
+    """
+    klass = _register_treeclass(klass)
+    # add math operations methods if leafwise
+    # do not override any user defined methods
+    klass = _leafwise_transform(klass) if leafwise else klass
+    # add `repr`,'str', 'at', 'copy', 'hash', 'copy'
+    # add the immutable setters and deleters
+    # generate the `__init__` method if not present using type hints.
+    klass = _treeclass_transform(klass)
+
+    return klass
```

### Comparing `pytreeclass-0.2.5/pytreeclass/_src/tree_freeze.py` & `pytreeclass-0.2.6/pytreeclass/_src/tree_freeze.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,28 +84,28 @@
     # the metadata.
     def __eq__(self, rhs: Any) -> bool:
         if not isinstance(rhs, _HashableWrapper):
             return False
         return _hash_node(self.unwrap()) == _hash_node(rhs.unwrap())
 
     def __hash__(self) -> int:
-        return _hash_node(self.unwrap())
+        return tree_hash(self.unwrap())
 
 
 class FrozenWrapper(ImmutableWrapper):
     def __repr__(self):
         return f"#{self.unwrap()!r}"
 
     def __eq__(self, rhs: Any) -> bool:
         if not isinstance(rhs, FrozenWrapper):
             return False
         return self.unwrap() == rhs.unwrap()
 
     def __hash__(self) -> int:
-        return hash(self.unwrap())
+        return tree_hash(self.unwrap())
 
 
 def _frozen_flatten(tree: Any) -> tuple[tuple, Any]:
     return (None,), _HashableWrapper(tree.unwrap())
 
 
 def _frozen_unflatten(treedef: Any, _: Sequence[Any]) -> PyTree:
```

### Comparing `pytreeclass-0.2.5/pytreeclass/_src/tree_indexer.py` & `pytreeclass-0.2.6/pytreeclass/_src/tree_indexer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,58 @@
 # this script defines methods used in indexing using `at` property
 # and decorator using to enable masking and math operations
 
 from __future__ import annotations
 
+import copy
 import functools as ft
 import operator as op
 from collections.abc import Callable
+from contextlib import contextmanager
 from math import ceil, floor, trunc
 from typing import Any, NamedTuple, TypeVar
 
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import numpy as np
 
-from pytreeclass._src.tree_decorator import _mutable_context
 from pytreeclass._src.tree_trace import tree_map_with_trace
 
 PyTree = Any
 _no_initializer = object()
 _non_partial = object()
 T = TypeVar("T")
 
+# allow methods in mutable context to be called without raising an error
+# this is done by registering the instance id in a set before entering the
+# mutable context and removing it after exiting the context
+_mutable_instance_registry: set[int] = set()
+
+
+def _conditional_mutable_method(method: Callable) -> Callable:
+    # decorator to allow for decorated methods to be called
+    # within the mutable context and raise an error otherwise
+    @ft.wraps(method)
+    def wrapper(self, *a, **k):
+        if id(self) in _mutable_instance_registry:
+            return method(self, *a, **k)
+        msg = f"Cannot call `{method.__name__}` on frozen instance."
+        raise AttributeError(msg)
+
+    return wrapper
+
+
+@contextmanager
+def _mutable_context(tree: PyTree, *, kopy: bool = False):
+    tree = copy.copy(tree) if kopy else tree
+    _mutable_instance_registry.add(id(tree))
+    yield tree
+    _mutable_instance_registry.discard(id(tree))
+
 
 def _is_leaf_bool(node: Any) -> bool:
     if hasattr(node, "dtype"):
         return node.dtype == "bool"
     return isinstance(node, bool)
 
 
@@ -129,15 +156,15 @@
     # does not support `is_leaf` argument, but it is supported here
     tree = tree.at[where].get(is_leaf=is_leaf)
     if initializer is _no_initializer:
         return jtu.tree_reduce(func, tree)
     return jtu.tree_reduce(func, tree, initializer)
 
 
-class _TreeAtMask(NamedTuple):
+class TreeAtMask(NamedTuple):
     tree: PyTree
     where: PyTree
 
     def get(self, *, is_leaf: Callable[[Any], bool] | None = None) -> PyTree:
         where = _true_tree(self.tree, is_leaf) if self.where is ... else self.where
         return _get_at_mask(self.tree, where, is_leaf)
 
@@ -162,38 +189,33 @@
         initializer: Callable[[Any, Any], Any] | Any = _no_initializer,
         *,
         is_leaf: Callable[[Any], bool] | None = None,
     ) -> Any:
         where = _true_tree(self.tree, is_leaf) if self.where is ... else self.where
         return _reduce_at_mask(self.tree, where, func, initializer, is_leaf)
 
-
-def _at_mask(tree: PyTree, where: PyTree) -> PyTree:
-    class TreeAtMask(_TreeAtMask):
-        def __getitem__(self, rhs_where: str | int | PyTree):
-            if isinstance(rhs_where, (str, int)):
-                # promote `rhs` path to boolean mask
-                mask = self.tree != self.tree
-                mask = mask.at[rhs_where].set(True)
-                rhs_where = mask
-
-            rhs_where = self.where & rhs_where
-            return TreeAtMask(tree=tree, where=rhs_where)
-
-        def __getattr__(self, name):
-            # support for nested `.at`
-            if name == "at":
-                # pass the current where condition to the next level
-                return TreeAtMask(tree=tree, where=self.where)
-
-            msg = f"{name} is not a valid attribute of {self}\n"
-            msg += f"Did you mean to use .at[{name!r}]?"
-            raise AttributeError(msg)
-
-    return TreeAtMask(tree=tree, where=where)
+    def __getitem__(self, rhs_where: str | int | PyTree) -> TreeAtMask:
+        if isinstance(rhs_where, (str, int)):
+            # promote `rhs` path to boolean mask
+            mask = self.tree != self.tree
+            mask = mask.at[rhs_where].set(True)
+            rhs_where = mask
+
+        rhs_where = self.where & rhs_where
+        return TreeAtMask(tree=self.tree, where=rhs_where)
+
+    def __getattr__(self, name: str) -> TreeAtMask:
+        # support for nested `.at`
+        if name == "at":
+            # pass the current where condition to the next level
+            return TreeAtMask(tree=self.tree, where=self.where)
+
+        msg = f"{name} is not a valid attribute of {self}\n"
+        msg += f"Did you mean to use .at[{name!r}]?"
+        raise AttributeError(msg)
 
 
 # tree indexing by name or index  path
 
 
 def _get_at_trace(
     tree: PyTree,
@@ -311,23 +333,26 @@
 
     tree = tree_map_with_trace(lhs_reduce, tree, is_leaf=is_leaf)
     if initializer is _no_initializer:
         return jtu.tree_reduce(func, tree)
     return jtu.tree_reduce(func, tree, initializer=initializer)
 
 
-class _TreeAtPath(NamedTuple):
+class TreeAtTrace(NamedTuple):
     tree: PyTree
     where: tuple[int | str]
 
     def get(self, *, is_leaf: Callable[[Any], bool] | None = None) -> PyTree:
         return _get_at_trace(self.tree, self.where, is_leaf)
 
     def set(
-        self, set_value: Any, *, is_leaf: Callable[[Any], bool] | None = None
+        self,
+        set_value: Any,
+        *,
+        is_leaf: Callable[[Any], bool] | None = None,
     ) -> PyTree:
         return _set_at_trace(self.tree, self.where, set_value, is_leaf)
 
     def apply(
         self,
         func: Callable[[Any], Any],
         *,
@@ -359,47 +384,72 @@
                 msg += f"of type={type(method_name).__name__}."
                 raise TypeError(msg)
 
             method = getattr(tree, method_name)
             value = method(*a, **k)
         return value, tree
 
+    def __getitem__(self, rhs_where: tuple[str | int] | PyTree):
+        if isinstance(rhs_where, type(self.tree)):
+            # promote `lhs` name path to boolean mask
+            # and pass to `TreeAtMask`
+            lhs_mask = self.tree != self.tree
+            (lhs_where,) = self.where
+            lhs_mask = lhs_mask.at[lhs_where].set(True)
+            return TreeAtMask(tree=self.tree, where=lhs_mask & rhs_where)
+
+        # case for name/index path rhs
+        rhs_where = (*self.where, rhs_where)
+        return TreeAtTrace(tree=self.tree, where=rhs_where)
+
+    def __getattr__(self, name: str) -> TreeAtTrace:
+        # support nested `.at``
+        # for example `.at[A].at[B]` represents model.A.B
+        if name == "at":
+            # pass the current tree and the current path to the next `.at`
+            return TreeAtTrace(tree=self.tree, where=self.where)
+
+        msg = f"{name} is not a valid attribute of {self}\n"
+        msg += f"Did you mean to use .at[{name!r}]?"
+        raise AttributeError(msg)
 
-def _at_trace(tree: PyTree, where: tuple[str | int] | PyTree) -> PyTree:
-    class TreeAtPath(_TreeAtPath):
-        def __getitem__(self, rhs_where: tuple[str | int] | PyTree):
-            # support for nested `.at``
-
-            if isinstance(rhs_where, type(tree)):
-                # promote `lhs` name path to boolean mask
-                # and pass to `TreeAtMask`
-                lhs_mask = self.tree != self.tree
-                (lhs_where,) = self.where
-                lhs_mask = lhs_mask.at[lhs_where].set(True)
-                return _at_mask(tree=tree, where=lhs_mask & rhs_where)
-
-            # case for name/index path rhs
-            rhs_where = (*self.where, rhs_where)
-            return _at_trace(tree=tree, where=rhs_where)
-
-        def __getattr__(self, name):
-            # support nested `.at``
-            # for example `.at[A].at[B]` represents model.A.B
-            if name == "at":
-                # pass the current tree and the current path to the next `.at`
-                return TreeAtPath(tree=tree, where=self.where)
-
-            msg = f"{name} is not a valid attribute of {self}\n"
-            msg += f"Did you mean to use .at[{name!r}]?"
-            raise AttributeError(msg)
 
-    return TreeAtPath(tree=tree, where=where)
+class AtIndexer(NamedTuple):
+    tree: PyTree
+
+    def __getitem__(self, where: Any) -> TreeAtTrace | TreeAtMask:
+        if isinstance(where, (str, int)):
+            # indexing by name or index
+            # name and index rules are defined using
+            # `register_pytree_node_trace_func`
+            return TreeAtTrace(tree=self.tree, where=(where,))
+
+        if isinstance(where, (type(self.tree), type(...))):
+            # indexing by boolean pytree
+            # Ellipsis as an alias for all elements
+            # model.at[model == model ] <--> model.at[...]
+            return TreeAtMask(tree=self.tree, where=where)
+
+        raise NotImplementedError(
+            f"Indexing with {type(where).__name__} is not implemented.\n"
+            "Example of supported indexing:\n\n"
+            "@pytc.treeclass\n"
+            f"class {type(self.tree).__name__}:\n"
+            "    ...\n\n"
+            f">>> tree = {type(self.tree).__name__}(...)\n"
+            ">>> # indexing by boolean pytree\n"
+            ">>> tree.at[tree > 0].get()\n\n"
+            ">>> # indexing by attribute name\n"
+            ">>> tree.at[`attribute_name`].get()\n\n"
+            ">>> # indexing by attribute index\n"
+            ">>> tree.at[`attribute_index`].get()"
+        )
 
 
-def tree_indexer(tree: PyTree) -> PyTree:
+def tree_indexer(tree: PyTree) -> AtIndexer:
     """Adds `.at` indexing abilities to a PyTree.
 
     Example:
         >>> import jax
         >>> import pytreeclass as pytc
 
         >>> @jax.tree_util.register_pytree_node_class
@@ -427,57 +477,26 @@
         ...     return [*zip(names, types, indices, metadatas)]
 
         >>> pytc.register_pytree_node_trace(Tree, test_trace_func)
 
         >>> Tree(1, 2).at["a"].get()
         Tree(a=1, b=None)
     """
-
-    class AtIndexer:
-        def __getitem__(self, where):
-            if isinstance(where, (str, int)):
-                # indexing by name or index
-                # name and index rules are defined using
-                # `register_pytree_node_trace_func`
-                return _at_trace(tree=tree, where=(where,))
-
-            if isinstance(where, (type(tree), type(...))):
-                # indexing by boolean pytree
-                # Ellipsis as an alias for all elements
-                # model.at[model == model ] <--> model.at[...]
-                return _at_mask(tree=tree, where=where)
-
-            raise NotImplementedError(
-                f"Indexing with {type(where).__name__} is not implemented.\n"
-                "Example of supported indexing:\n\n"
-                "@pytc.treeclass\n"
-                f"class {type(tree).__name__}:\n"
-                "    ...\n\n"
-                f">>> tree = {type(tree).__name__}(...)\n"
-                ">>> # indexing by boolean pytree\n"
-                ">>> tree.at[tree > 0].get()\n\n"
-                ">>> # indexing by attribute name\n"
-                ">>> tree.at[`attribute_name`].get()\n\n"
-                ">>> # indexing by attribute index\n"
-                ">>> tree.at[`attribute_index`].get()"
-            )
-
-    return AtIndexer()
+    return AtIndexer(tree=tree)
 
 
 class BroadcastablePartial(ft.partial):
     def __call__(self, *args, **keywords) -> Callable:
         # https://stackoverflow.com/a/7811270
         keywords = {**self.keywords, **keywords}
         iargs = iter(args)
         args = (next(iargs) if arg is _non_partial else arg for arg in self.args)  # type: ignore
         return self.func(*args, *iargs, **keywords)
 
 
-@ft.lru_cache(maxsize=None)
 def bcmap(
     func: Callable[..., Any], *, is_leaf: Callable[[Any], bool] | None = None
 ) -> Callable:
     """(map)s a function over pytrees leaves with automatic (b)road(c)asting for scalar arguments
 
     Args:
         func: the function to be mapped over the pytree
@@ -685,10 +704,10 @@
         leaves, treedef = jtu.tree_flatten(tree)
         if (treedef != treedef0) or verdict is False:
             return False
         verdict = ft.reduce(op.and_, map(_is_lhs_rhs_equal, leaves0, leaves), verdict)
     return verdict
 
 
-def tree_copy(tree: PyTree) -> PyTree:
+def tree_copy(tree: T) -> T:
     """Return a copy of the tree."""
     return jtu.tree_unflatten(*jtu.tree_flatten(tree)[::-1])  # type: ignore
```

### Comparing `pytreeclass-0.2.5/pytreeclass/_src/tree_pprint.py` & `pytreeclass-0.2.6/pytreeclass/_src/tree_pprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,24 +404,22 @@
             [2]:list
                 [0]=4
                 [1]:list
                     [0]=5
                     [1]=6
 
     """
-    traces_leaves = pytc.tree_leaves_with_trace(
-        tree=tree,
-        is_leaf=is_leaf,
-        is_trace_leaf=_is_trace_leaf_depth_factory(depth),
-    )
-
     fmt = f"{type(tree).__name__}"
     seen = set()
 
-    for trace, leaf in traces_leaves:
+    for trace, leaf in pytc.tree_leaves_with_trace(
+        tree=tree,
+        is_leaf=is_leaf,
+        is_trace_leaf=_is_trace_leaf_depth_factory(depth),
+    ):
         names, types = trace[0], trace[1]
 
         for j, (name, type_) in enumerate(zip(names, types)):
             if names[: j + 1] in seen:
                 continue  # skip printing the common parent node twice
             seen.add(names[: j + 1])
 
@@ -614,29 +612,25 @@
         depth: depth of the tree to print. default is max depth
         is_leaf: function to determine if a node is a leaf. default is None
 
     Example:
         >>> import pytreeclass as pytc
         >>> tree = [1, [2, 3], [4, [5, 6]]]
         >>> print(pytc.tree_mermaid(tree, depth=1))  # doctest: +SKIP
-
-        .. mermaid::
-
-            flowchart LR
-
-                id2 --- id3("</b>[0]=2</b>")
-                id2 --- id4("</b>[1]=3</b>")
-                id5 --- id6("</b>[0]=4</b>")
-                id5 --- id7("</b>[1]:list</b>")
-                id0(<b>list</b>)
-                id0 --- id1("</b>[0]=1</b>")
-                id0 --- id2("</b>[1]:list</b>")
-                id0 --- id5("</b>[2]:list</b>")
-                id7 --- id8("</b>[0]=5</b>")
-                id7 --- id9("</b>[1]=6</b>")
+        flowchart LR
+            id2 --- id3("</b>[0]=2</b>")
+            id2 --- id4("</b>[1]=3</b>")
+            id5 --- id6("</b>[0]=4</b>")
+            id5 --- id7("</b>[1]:list</b>")
+            id0(<b>list</b>)
+            id0 --- id1("</b>[0]=1</b>")
+            id0 --- id2("</b>[1]:list</b>")
+            id0 --- id5("</b>[2]:list</b>")
+            id7 --- id8("</b>[0]=5</b>")
+            id7 --- id9("</b>[1]=6</b>")
     """
 
     indent_repr = tree_indent(
         tree,
         width=width,
         depth=depth,
         is_leaf=is_leaf,
```

### Comparing `pytreeclass-0.2.5/pytreeclass/_src/tree_trace.py` & `pytreeclass-0.2.6/pytreeclass/_src/tree_trace.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.5/pytreeclass.egg-info/PKG-INFO` & `pytreeclass-0.2.6/pytreeclass.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytreeclass
-Version: 0.2.5
+Version: 0.2.6
 Summary: JAX compatible dataclass.
 Home-page: https://github.com/ASEM000/pytreeclass
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: Apache-2.0
 Keywords: python machine-learning pytorch jax
 Classifier: Development Status :: 5 - Production/Stable
@@ -731,56 +731,56 @@
 
 ```python
 import jax
 import pytreeclass as pytc
 
 tree = [1, [2,3], 4]
 
-print(pytc.tree_diagram(tree,depth=1))
+print(pytc.tree_diagram(tree, depth=1))
 # list
-#     ├── [0]=1
-#     ├── [1]=[..., ...]
-#     └── [2]=4
+# ├── [0]=1
+# ├── [1]=[...]
+# └── [2]=4
 
-print(pytc.tree_diagram(tree,depth=2))
+print(pytc.tree_diagram(tree, depth=2))
 # list
-#     ├── [0]=1
-#     ├── [1]:list
-#     │   ├── [0]=2
-#     │   └── [1]=3
-#     └── [2]=4
-
-
-print(pytc.tree_summary(tree,depth=1))
-# ┌────┬────┬─────┬───────┐
-# │Name│Type│Count│Size   │
-# ├────┼────┼─────┼───────┤
-# │[0] │int │1    │28.00B │
-# ├────┼────┼─────┼───────┤
-# │[1] │list│2    │56.00B │
-# ├────┼────┼─────┼───────┤
-# │[2] │int │1    │28.00B │
-# ├────┼────┼─────┼───────┤
-# │Σ   │list│4    │112.00B│
-# └────┴────┴─────┴───────┘
-
-print(pytc.tree_summary(tree,depth=2))
-# ┌──────┬────┬─────┬───────┐
-# │Name  │Type│Count│Size   │
-# ├──────┼────┼─────┼───────┤
-# │[0]   │int │1    │28.00B │
-# ├──────┼────┼─────┼───────┤
-# │[1][0]│int │1    │28.00B │
-# ├──────┼────┼─────┼───────┤
-# │[1][1]│int │1    │28.00B │
-# ├──────┼────┼─────┼───────┤
-# │[2]   │int │1    │28.00B │
-# ├──────┼────┼─────┼───────┤
-# │Σ     │list│4    │112.00B│
-# └──────┴────┴─────┴───────┘
+# ├── [0]=1
+# ├── [1]:list
+# │   ├── [0]=2
+# │   └── [1]=3
+# └── [2]=4
+
+
+print(pytc.tree_summary(tree, depth=1))
+# ┌────┬────┬─────┐
+# │Name│Type│Count│
+# ├────┼────┼─────┤
+# │[0] │int │1    │
+# ├────┼────┼─────┤
+# │[1] │list│1    │
+# ├────┼────┼─────┤
+# │[2] │int │1    │
+# ├────┼────┼─────┤
+# │Σ   │list│3    │
+# └────┴────┴─────┘
+
+print(pytc.tree_summary(tree, depth=2))
+# ┌──────┬────┬─────┐
+# │Name  │Type│Count│
+# ├──────┼────┼─────┤
+# │[0]   │int │1    │
+# ├──────┼────┼─────┤
+# │[1][0]│int │1    │
+# ├──────┼────┼─────┤
+# │[1][1]│int │1    │
+# ├──────┼────┼─────┤
+# │[2]   │int │1    │
+# ├──────┼────┼─────┤
+# │Σ     │list│4    │
+# └──────┴────┴─────┘
 ```
 
 </details>
 
 <details><summary>Use PyTreeClass components with other libraries</summary>
 
 ```python
@@ -817,34 +817,34 @@
 # FlaxTree(a=1, b=(2.0, 3.0), c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00]))
 
 print(f"{flax_tree!s}")
 # FlaxTree(a=1, b=(2.0, 3.0), c=[4. 5. 6.])
 
 print(pytc.tree_diagram(flax_tree))
 # FlaxTree
-#     ├── a=1
-#     ├── b:tuple
-#     │   ├── [0]=2.0
-#     │   └── [1]=3.0
-#     └── c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
+# ├── a=1
+# ├── b:tuple
+# │   ├── [0]=2.0
+# │   └── [1]=3.0
+# └── c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00])
 
 print(pytc.tree_summary(flax_tree))
-# ┌────┬────────┬─────┬──────┐
-# │Name│Type    │Count│Size  │
-# ├────┼────────┼─────┼──────┤
-# │a   │int     │1    │28.00B│
-# ├────┼────────┼─────┼──────┤
-# │b[0]│float   │1    │24.00B│
-# ├────┼────────┼─────┼──────┤
-# │b[1]│float   │1    │24.00B│
-# ├────┼────────┼─────┼──────┤
-# │c   │f32[3]  │3    │12.00B│
-# ├────┼────────┼─────┼──────┤
-# │Σ   │FlaxTree│6    │88.00B│
-# └────┴────────┴─────┴──────┘
+# ┌────┬────────┬─────┐
+# │Name│Type    │Count│
+# ├────┼────────┼─────┤
+# │a   │int     │1    │
+# ├────┼────────┼─────┤
+# │b[0]│float   │1    │
+# ├────┼────────┼─────┤
+# │b[1]│float   │1    │
+# ├────┼────────┼─────┤
+# │c   │f32[3]  │3    │
+# ├────┼────────┼─────┤
+# │Σ   │FlaxTree│6    │
+# └────┴────────┴─────┘
 
 flax_tree.at[0].get()
 # FlaxTree(a=1, b=(None, None), c=None)
 
 flax_tree.at["a"].set(10)
 # FlaxTree(a=10, b=(2.0, 3.0), c=f32[3](μ=5.00, σ=0.82, ∈[4.00,6.00]))
 ```
@@ -905,38 +905,35 @@
 For example for the previous tree, the reuslting trace path for each leaf is :
 
 ### Named tree variant
 
 ```python
 >>> name_tree = pytc.tree_map_with_trace(lambda trace,x : trace[0], tree)
 >>> print(name_tree)
-Tree(a=(Tree, a), b=((Tree, b, [0]), (Tree, b, [1])), c=(Tree, c))
+Tree(a=(a), b=((b, [0]), (b, [1])), c=(c))
 ```
 
 ### Typed tree variant
 
 ```python
 >>> type_tree = pytc.tree_map_with_trace(lambda trace,x : f"{trace[1]!s}", tree)
 >>> print(type_tree)
 Tree(
-  a=(<class '__main__.Tree'>, <class 'int'>),
-  b=(
-    (<class '__main__.Tree'>, <class 'tuple'>, <class 'float'>),
-    (<class '__main__.Tree'>, <class 'tuple'>, <class 'float'>)
-  ),
-  c=(<class '__main__.Tree'>, <class 'jaxlib.xla_extension.ArrayImpl'>)
+  a=(<class 'int'>,),
+  b=((<class 'tuple'>, <class 'float'>), (<class 'tuple'>, <class 'float'>)),
+  c=(<class 'jaxlib.xla_extension.ArrayImpl'>,)
 )
 ```
 
 ### Index tree variant
 
 ```python
 >>> index_tree = pytc.tree_map_with_trace(lambda trace,x : trace[2], tree)
 >>> print(index_tree)
-Tree(a=(0, 0), b=((0, 1, 0), (0, 1, 1)), c=(0, 2))
+Tree(a=(0), b=((1, 0), (1, 1)), c=(2))
 ```
 
 In essence, each leaf contains information about the name path, type path, and indices path. The rules for custom types can be registered using `pytc.register_pytree_node_trace`
 
 </details>
 
 <details>
@@ -953,15 +950,15 @@
 <tr><td align="center">Generated str method</td> <td align="center">✅</td>  <td align="center"></td></tr>
 <tr><td align="center">Generated hash method</td> <td align="center">✅</td>  <td align="center">✅</td></tr>
 <tr><td align="center">Generated eq method</td> <td align="center">✅✅*</td>  <td align="center">✅</td></tr>
 <tr><td align="center">Support slots</td> <td align="center"></td>  <td align="center">✅</td></tr>
 <tr><td align="center">Keyword-only args</td> <td align="center">✅</td>  <td align="center">✅ 3.10+</td></tr>
 <tr><td align="center">Positional-only args</td> <td align="center">✅</td>  <td align="center"></td></tr>
 <tr><td align="center">Frozen instance</td> <td align="center">✅**</td>  <td align="center">✅</td></tr>
-<tr><td align="center">Match args support</td> <td align="center">✅</td>  <td align="center">✅</td></tr>
+<tr><td align="center">Match args support</td> <td align="center"></td>  <td align="center">✅</td></tr>
 <tr><td align="center">Support callbacks</td> <td align="center">✅</td>  <td align="center"></td></tr>
 </table>
 
 </div>
 
 `*` Either compare the whole instance and return `True/False` or treating it leafwise using `treeclass(..., leafwise=True)` and retrurn `Tree(a=True, ....)`
```

### Comparing `pytreeclass-0.2.5/pytreeclass.egg-info/SOURCES.txt` & `pytreeclass-0.2.6/pytreeclass.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 pytreeclass.egg-info/PKG-INFO
 pytreeclass.egg-info/SOURCES.txt
 pytreeclass.egg-info/dependency_links.txt
 pytreeclass.egg-info/not-zip-safe
 pytreeclass.egg-info/requires.txt
 pytreeclass.egg-info/top_level.txt
 pytreeclass/_src/__init__.py
-pytreeclass/_src/tree_base.py
 pytreeclass/_src/tree_decorator.py
 pytreeclass/_src/tree_freeze.py
 pytreeclass/_src/tree_indexer.py
 pytreeclass/_src/tree_pprint.py
 pytreeclass/_src/tree_trace.py
 tests/__init__.py
 tests/test_indexing.py
```

### Comparing `pytreeclass-0.2.5/setup.py` & `pytreeclass-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.5/tests/test_indexing.py` & `pytreeclass-0.2.6/tests/test_indexing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import functools as ft
 
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
+import numpy.testing as npt
 import pytest
 
 import pytreeclass as pytc
 from pytreeclass._src.tree_indexer import _mutable_context
 
 
 @ft.partial(pytc.treeclass, leafwise=True)
@@ -348,23 +349,27 @@
     tree = StackedLinear(in_dim=1, out_dim=1, hidden_dim=5, key=jax.random.PRNGKey(0))
 
     assert (
         tree.at[tree > 0].reduce(
             lambda x, y: jnp.minimum(x, jnp.min(y)), initializer=jnp.inf
         )
     ) == 0.98507565
-    assert (
+    npt.assert_allclose(
         tree.at[tree > 0].reduce(
             lambda x, y: jnp.maximum(x, jnp.max(y)), initializer=-jnp.inf
-        )
-    ) == 1.3969219
-    assert (
-        tree.at[tree > 0].reduce(lambda x, y: x + jnp.sum(y), initializer=0)
-    ) == 10.6970625
-    assert (tree.at[tree > 0].reduce(lambda x, y: x * jnp.product(y), initializer=1)) == 1.8088213  # fmt: skip
+        ),
+        1.3969219,
+    )
+    npt.assert_allclose(
+        tree.at[tree > 0].reduce(lambda x, y: x + jnp.sum(y), initializer=0), 10.6970625
+    )
+    npt.assert_allclose(
+        tree.at[tree > 0].reduce(lambda x, y: x * jnp.product(y), initializer=1),
+        1.8088213,
+    )
 
 
 def test_is_leaf():
     @ft.partial(pytc.treeclass, leafwise=True)
     class Tree:
         a: int
 
@@ -629,16 +634,16 @@
     @ft.partial(pytc.treeclass, leafwise=True)
     class Tree:
         a: int = 1
         b: int = 2
 
     t = Tree()
 
-    assert repr(t.at["a"]) == "TreeAtPath(tree=Tree(a=1, b=2), where=('a',))"
-    assert str(t.at["a"]) == "TreeAtPath(tree=Tree(a=1, b=2), where=('a',))"
+    assert repr(t.at["a"]) == "TreeAtTrace(tree=Tree(a=1, b=2), where=('a',))"
+    assert str(t.at["a"]) == "TreeAtTrace(tree=Tree(a=1, b=2), where=('a',))"
     assert repr(t.at[...]) == "TreeAtMask(tree=Tree(a=1, b=2), where=Ellipsis)"
 
 
 def test_not_equal():
     @ft.partial(pytc.treeclass, leafwise=True)
     class Tree:
         a: int = 1
```

### Comparing `pytreeclass-0.2.5/tests/test_nn.py` & `pytreeclass-0.2.6/tests/test_nn.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,114 +1,110 @@
 import functools as ft
 from typing import Callable, Sequence
 
 import jax
 import jax.numpy as jnp
+import jax.random as jr
 import jax.tree_util as jtu
 import numpy as np
 import pytest
 
 import pytreeclass as pytc
 
 
 def test_nn():
     @ft.partial(pytc.treeclass, leafwise=True)
     class Linear:
-        weight: jnp.ndarray
-        bias: jnp.ndarray
+        weight: jax.Array
+        bias: jax.Array
 
         def __init__(self, key, in_dim, out_dim):
-            self.weight = jax.random.normal(
-                key, shape=(in_dim, out_dim)) * jnp.sqrt(2 / in_dim)  # fmt: skip
+            self.weight = jr.normal(key, shape=(in_dim, out_dim)) * jnp.sqrt(2 / in_dim)
             self.bias = jnp.ones((1, out_dim))
 
         def __call__(self, x):
             return x @ self.weight + self.bias
 
     @ft.partial(pytc.treeclass, leafwise=True)
     class StackedLinear:
         layers: Sequence[Linear]
 
         def __init__(self, key, layers):
-            keys = jax.random.split(key, len(layers) - 1)
+            keys = jr.split(key, len(layers) - 1)
 
             self.layers = []
 
             for ki, in_dim, out_dim in zip(keys, layers[:-1], layers[1:]):
                 self.layers += [Linear(ki, in_dim, out_dim)]
 
         def __call__(self, x):
             for layer in self.layers[:-1]:
                 x = layer(x)
                 x = jax.nn.tanh(x)
 
             return self.layers[-1](x)
 
     x = jnp.linspace(0, 1, 100)[:, None]
-    y = x**3 + jax.random.uniform(jax.random.PRNGKey(0), (100, 1)) * 0.01
+    y = x**3 + jr.uniform(jr.PRNGKey(0), (100, 1)) * 0.01
 
-    model = StackedLinear(layers=[1, 128, 128, 1], key=jax.random.PRNGKey(0))
+    NN = StackedLinear(layers=[1, 128, 128, 1], key=jr.PRNGKey(0))
 
-    def loss_func(model, x, y):
-        return jnp.mean((model(x) - y) ** 2)
+    def loss_func(NN, x, y):
+        return jnp.mean((NN(x) - y) ** 2)
 
     @jax.jit
-    def update(model, x, y):
-        value, grads = jax.value_and_grad(loss_func)(model, x, y)
-        return value, jax.tree_map(lambda x, y: x - 1e-3 * y, model, grads)
+    def update(NN, x, y):
+        value, grads = jax.value_and_grad(loss_func)(NN, x, y)
+        return value, jax.tree_map(lambda x, y: x - 1e-3 * y, NN, grads)
 
     for _ in range(1, 2001):
-        value, model = update(model, x, y)
+        value, NN = update(NN, x, y)
 
     np.testing.assert_allclose(value, jnp.array(0.00103019), atol=1e-5)
 
 
 def test_nn_with_func_input():
     @ft.partial(pytc.treeclass, leafwise=True)
     class Linear:
-        weight: jnp.ndarray
-        bias: jnp.ndarray
+        weight: jax.Array
+        bias: jax.Array
         act_func: Callable
 
         def __init__(self, key, in_dim, out_dim, act_func):
             self.act_func = act_func
-            self.weight = jax.random.normal(key, shape=(in_dim, out_dim)) * jnp.sqrt(
-                2 / in_dim
-            )
+            self.weight = jr.normal(key, shape=(in_dim, out_dim)) * jnp.sqrt(2 / in_dim)
             self.bias = jnp.ones((1, out_dim))
 
         def __call__(self, x):
             return self.act_func(x @ self.weight + self.bias)
 
-    layer = Linear(key=jax.random.PRNGKey(0), in_dim=1, out_dim=1, act_func=jax.nn.tanh)
+    layer = Linear(key=jr.PRNGKey(0), in_dim=1, out_dim=1, act_func=jax.nn.tanh)
     x = jnp.linspace(0, 1, 100)[:, None]
-    # y = x**3 + jax.random.uniform(jax.random.PRNGKey(0), (100, 1)) * 0.01
+    # y = x**3 + jr.uniform(jr.PRNGKey(0), (100, 1)) * 0.01
     layer(x)
     return True
 
 
 def test_compact_nn():
     @ft.partial(pytc.treeclass, leafwise=True)
     class Linear:
-        weight: jnp.ndarray
-        bias: jnp.ndarray
+        weight: jax.Array
+        bias: jax.Array
 
         def __init__(self, key, in_dim, out_dim):
-            self.weight = jax.random.normal(key, shape=(in_dim, out_dim)) * jnp.sqrt(
-                2 / in_dim
-            )
+            self.weight = jr.normal(key, shape=(in_dim, out_dim)) * jnp.sqrt(2 / in_dim)
             self.bias = jnp.ones((1, out_dim))
 
         def __call__(self, x):
             return x @ self.weight + self.bias
 
     @ft.partial(pytc.treeclass, leafwise=True)
     class StackedLinear:
         def __init__(self, key, in_dim, out_dim, hidden_dim):
-            keys = jax.random.split(key, 3)
+            keys = jr.split(key, 3)
 
             self.l1 = Linear(key=keys[0], in_dim=in_dim, out_dim=hidden_dim)
             self.l2 = Linear(key=keys[1], in_dim=hidden_dim, out_dim=hidden_dim)
             self.l3 = Linear(key=keys[2], in_dim=hidden_dim, out_dim=out_dim)
 
         def __call__(self, x):
             x = self.l1(x)
@@ -116,66 +112,64 @@
             x = self.l2(x)
             x = jax.nn.tanh(x)
             x = self.l3(x)
 
             return x
 
     x = jnp.linspace(0, 1, 100)[:, None]
-    y = x**3 + jax.random.uniform(jax.random.PRNGKey(0), (100, 1)) * 0.01
+    y = x**3 + jr.uniform(jr.PRNGKey(0), (100, 1)) * 0.01
 
-    model = StackedLinear(in_dim=1, out_dim=1, hidden_dim=10, key=jax.random.PRNGKey(0))
+    NN = StackedLinear(in_dim=1, out_dim=1, hidden_dim=10, key=jr.PRNGKey(0))
 
-    def loss_func(model, x, y):
-        return jnp.mean((model(x) - y) ** 2)
+    def loss_func(NN, x, y):
+        return jnp.mean((NN(x) - y) ** 2)
 
     @jax.jit
-    def update(model, x, y):
-        value, grads = jax.value_and_grad(loss_func)(model, x, y)
+    def update(NN, x, y):
+        value, grads = jax.value_and_grad(loss_func)(NN, x, y)
 
-        # no need to use `jax.tree_map` to update the model
-        #  as it model is wrapped by @ft.partial(pytc.treeclass, leafwise=True)
-        return value, model - 1e-3 * grads
+        # no need to use `jax.tree_map` to update the NN
+        #  as it NN is wrapped by @ft.partial(pytc.treeclass, leafwise=True)
+        return value, NN - 1e-3 * grads
 
     for _ in range(1, 10_001):
-        value, model = update(model, x, y)
+        value, NN = update(NN, x, y)
 
     np.testing.assert_allclose(value, jnp.array(0.0031012), atol=1e-5)
 
 
 def test_freeze_nondiff():
     @ft.partial(pytc.treeclass, leafwise=True)
     class Linear:
-        weight: jnp.ndarray
-        bias: jnp.ndarray
+        weight: jax.Array
+        bias: jax.Array
         count: int
         use_bias: bool
 
         def __init__(self, key, in_dim, out_dim):
-            self.weight = jax.random.normal(key, shape=(in_dim, out_dim)) * jnp.sqrt(
-                2 / in_dim
-            )
+            self.weight = jr.normal(key, shape=(in_dim, out_dim)) * jnp.sqrt(2 / in_dim)
             self.bias = jnp.ones((1, out_dim))
             self.use_bias = True
             self.count = 0
 
         def __call__(self, x):
             return x @ self.weight + self.bias
 
     @ft.partial(pytc.treeclass, leafwise=True)
     class StackedLinear:
         name: str
-        exact_array: jnp.ndarray
-        bool_array: jnp.ndarray
+        exact_array: jax.Array
+        bool_array: jax.Array
 
         def __init__(self, key, in_dim, out_dim, hidden_dim):
             self.name = "stack"
             self.exact_array = jnp.array([1, 2, 3])
             self.bool_array = jnp.array([True, True])
 
-            keys = jax.random.split(key, 3)
+            keys = jr.split(key, 3)
 
             self.l1 = Linear(key=keys[0], in_dim=in_dim, out_dim=hidden_dim)
             self.l2 = Linear(key=keys[1], in_dim=hidden_dim, out_dim=hidden_dim)
             self.l3 = Linear(key=keys[2], in_dim=hidden_dim, out_dim=out_dim)
 
         def __call__(self, x):
             x = self.l1(x)
@@ -183,45 +177,45 @@
             x = self.l2(x)
             x = jax.nn.tanh(x)
             x = self.l3(x)
 
             return x
 
     x = jnp.linspace(0, 1, 100)[:, None]
-    y = x**3 + jax.random.uniform(jax.random.PRNGKey(0), (100, 1)) * 0.01
+    y = x**3 + jr.uniform(jr.PRNGKey(0), (100, 1)) * 0.01
 
-    model = StackedLinear(in_dim=1, out_dim=1, hidden_dim=10, key=jax.random.PRNGKey(0))
+    NN = StackedLinear(in_dim=1, out_dim=1, hidden_dim=10, key=jr.PRNGKey(0))
 
-    def loss_func(model, x, y):
-        return jnp.mean((model(x) - y) ** 2)
+    def loss_func(NN, x, y):
+        return jnp.mean((NN(x) - y) ** 2)
 
     with pytest.raises(TypeError):
 
         @jax.jit
-        def update(model, x, y):
-            value, grads = jax.value_and_grad(loss_func)(model, x, y)
-            return value, model - 1e-3 * grads
+        def update(NN, x, y):
+            value, grads = jax.value_and_grad(loss_func)(NN, x, y)
+            return value, NN - 1e-3 * grads
 
         for _ in range(1, 10_001):
-            value, model = update(model, x, y)
+            value, NN = update(NN, x, y)
 
     @jax.jit
-    def update(model, x, y):
-        value, grads = jax.value_and_grad(loss_func)(model, x, y)
-        return value, model - 1e-3 * grads
+    def update(NN, x, y):
+        value, grads = jax.value_and_grad(loss_func)(NN, x, y)
+        return value, NN - 1e-3 * grads
 
-    mask = jtu.tree_map(pytc.is_nondiff, model)
-    freezeed_model = model.at[mask].apply(pytc.freeze)
+    mask = jtu.tree_map(pytc.is_nondiff, NN)
+    freezeed_NN = NN.at[mask].apply(pytc.freeze)
 
     for _ in range(1, 10_001):
-        value, freezeed_model = update(freezeed_model, x, y)
+        value, freezeed_NN = update(freezeed_NN, x, y)
 
     np.testing.assert_allclose(value, jnp.array(0.0031012), atol=1e-5)
 
-    X = StackedLinear(in_dim=1, out_dim=1, hidden_dim=10, key=jax.random.PRNGKey(0))
+    X = StackedLinear(in_dim=1, out_dim=1, hidden_dim=10, key=jr.PRNGKey(0))
 
     frozen_ = jtu.tree_map(pytc.freeze, X)
     unfrozen_ = jtu.tree_map(pytc.unfreeze, frozen_, is_leaf=pytc.is_frozen)
     assert jtu.tree_leaves(X) == jtu.tree_leaves(unfrozen_)
 
 
 @pytest.mark.benchmark
```

### Comparing `pytreeclass-0.2.5/tests/test_tree_freeze.py` & `pytreeclass-0.2.6/tests/test_tree_freeze.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import pytest
 
 import pytreeclass as pytc
-from pytreeclass._src.tree_freeze import _HashableWrapper
+from pytreeclass._src.tree_freeze import _HashableWrapper, tree_hash
 
 
 def test_freeze_unfreeze():
     @ft.partial(pytc.treeclass, leafwise=True)
     class A:
         a: int
         b: int
@@ -379,25 +379,25 @@
     # print(model)
     # Test(a=-0.45068058,*b=2,*c=3,*act=tanh(x))
     assert model.a == pytest.approx(-0.45068058, 1e-5)
 
 
 def test_wrapper():
     # only apply last wrapper
-    assert hash((pytc.freeze(1))) == hash(1)
+    assert hash((pytc.freeze(1))) == tree_hash(1)
 
     lhs = _HashableWrapper(1)
     # test getter
     assert lhs.__wrapped__ == 1
     assert lhs.__wrapped__
 
     # comparison with the wrapped object
     assert lhs != 1
     # hash of the wrapped object
-    assert hash(lhs) == hash(1)
+    assert hash(lhs) == tree_hash(1)
 
     # test immutability
     frozen_value = pytc.freeze(1)
 
     with pytest.raises(AttributeError):
         frozen_value.__wrapped__ = 2
```

### Comparing `pytreeclass-0.2.5/tests/test_tree_operator.py` & `pytreeclass-0.2.6/tests/test_tree_operator.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.5/tests/test_tree_pprint.py` & `pytreeclass-0.2.6/tests/test_tree_pprint.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.5/tests/test_tree_viz_util.py` & `pytreeclass-0.2.6/tests/test_tree_viz_util.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.5/tests/test_treeclass.py` & `pytreeclass-0.2.6/tests/test_treeclass.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 import copy
 import dataclasses as dc
 import functools as ft
+from typing import Any
 
 import jax
 import jax.tree_util as jtu
 import numpy.testing as npt
 import pytest
 from jax import numpy as jnp
 
 import pytreeclass as pytc
-from pytreeclass._src.tree_decorator import _field_registry
 
 
-def test_field():
+def test_field_metadata():
+    @ft.partial(pytc.treeclass, leafwise=True)
+    class Test:
+        a: int = pytc.field(default=1, metadata={"a": 1})
+
+    assert Test().__field_map__["a"].metadata["a"] == 1
+
+
+def test_field_mutually_exclusive():
     with pytest.raises(ValueError):
         pytc.field(default=1, factory=lambda: 1)
 
+    with pytest.raises(ValueError):
+        pytc.field(default=1, pos_only=True, kw_only=True)
+
+
+def test_field():
     assert pytc.field(default=1).default == 1
 
     with pytest.raises(TypeError):
         pytc.field(metadata=1)
 
     @ft.partial(pytc.treeclass, leafwise=True)
     class Test:
-        a: int = pytc.field(default=1, metadata={"a": 1})
-
-    assert _field_registry[Test]["a"].metadata["a"] == 1
-
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Test:
         a: int = pytc.field(default=1, pos_only=True)
         b: int = 2
 
     with pytest.raises(TypeError):
         # positonal only for a
         Test(a=1, b=2)
 
@@ -57,21 +64,14 @@
         Test(1, 2)
 
     with pytest.raises(TypeError):
         Test(1, b=2)
 
     assert Test(a=1, b=2).a == 1
 
-    with pytest.raises(ValueError):
-        # keyword only and pos_only are mutually exclusive
-        @ft.partial(pytc.treeclass, leafwise=True)
-        class Test:
-            a: int = pytc.field(default=1, pos_only=True, kw_only=True)
-
-    # pos_only, kw_only
     @ft.partial(pytc.treeclass, leafwise=True)
     class Test:
         a: int = pytc.field(default=1, pos_only=True)
         b: int = pytc.field(default=2, kw_only=True)
 
     with pytest.raises(TypeError):
         Test(1, 2)
@@ -91,48 +91,45 @@
         Test(1, 2)
 
     assert Test(b=2).a == 1
 
     with pytest.raises(TypeError):
         pytc.fields(1)
 
-    assert len(pytc.fields(Test)) == 2
+    assert len(pytc.fields(Test())) == 2
 
     @pytc.treeclass
     class Test:
         a: int = pytc.field(default=1)
         b: int = pytc.field(factory=lambda: 1)
 
         def __init__(self) -> None:
             pass
 
     with pytest.raises(AttributeError):
         Test()
 
 
-def test_field_nondiff():
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Test:
-        a: int = 1
-        b: int = 2
-        c: int = 3
+def test_field_alias():
+    @pytc.treeclass
+    class Tree:
+        _name: str = pytc.field(alias="name")
 
-    test = Test()
+    tree = Tree(name="test")
+    assert tree._name == "test"
 
-    @ft.partial(pytc.treeclass, leafwise=True)
-    class Test:
-        a: jnp.ndarray
-        b: jnp.ndarray
+    with pytest.raises(TypeError):
+        pytc.field(alias=1)
 
-        def __init__(self, a=jnp.array([1, 2, 3]), b=jnp.array([4, 5, 6])):
-            self.a = a
-            self.b = b
 
-    test = Test()
+def test_field_hash():
+    hash(pytc.field(default=1)) == hash(pytc.field(default=1))
 
+
+def test_field_nondiff():
     @ft.partial(pytc.treeclass, leafwise=True)
     class Test:
         a: jnp.ndarray
         b: jnp.ndarray
 
         def __init__(
             self,
@@ -720,7 +717,29 @@
 def test_repeated_treeclass():
     @pytc.treeclass
     @pytc.treeclass
     class Tree:
         a: int = pytc.field()
 
     assert True
+
+
+def test_instance_field_map():
+    @pytc.treeclass
+    class Parameter:
+        value: Any
+
+    @pytc.treeclass
+    class Tree:
+        bias: int = 0
+
+        def add_param(self, name, param):
+            return setattr(self, name, param)
+
+    tree = Tree()
+
+    _, tree_with_weight = tree.at["add_param"]("weight", Parameter(3))
+
+    assert tree.__field_map__ != tree_with_weight.__field_map__
+    assert tree_with_weight.weight == Parameter(3)
+    assert "weight" not in vars(tree)
+    assert "weight" not in tree.__field_map__
```

### Comparing `pytreeclass-0.2.5/tests/test_under_jit.py` & `pytreeclass-0.2.6/tests/test_under_jit.py`

 * *Files identical despite different names*

