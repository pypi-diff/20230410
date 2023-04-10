# Comparing `tmp/e3psi-0.2.0.tar.gz` & `tmp/e3psi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e3psi-0.2.0.tar", last modified: Tue Nov  8 16:48:02 2022, max compression
+gzip compressed data, was "e3psi-0.3.0.tar", last modified: Mon Apr 10 17:07:10 2023, max compression
```

## Comparing `e3psi-0.2.0.tar` & `e3psi-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
--rw-r--r--   0        0        0       59 2022-09-21 13:31:15.699437 e3psi-0.2.0/.bandit
--rw-r--r--   0        0        0     1413 2022-08-08 10:16:14.742612 e3psi-0.2.0/.circleci/config.yml
--rw-r--r--   0        0        0       71 2022-08-08 10:16:14.730612 e3psi-0.2.0/.coveragerc
--rw-r--r--   0        0        0      284 2022-08-08 10:16:14.730612 e3psi-0.2.0/.deepsource.toml
--rw-r--r--   0        0        0      289 2022-08-08 10:16:14.742612 e3psi-0.2.0/.editorconfig
--rw-r--r--   0        0        0      147 2022-11-08 16:36:39.811850 e3psi-0.2.0/.flake8
--rw-r--r--   0        0        0      209 2022-08-08 10:16:14.718612 e3psi-0.2.0/.gitattributes
--rw-r--r--   0        0        0      238 2022-08-08 10:16:14.750611 e3psi-0.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1272 2022-10-05 20:00:58.188837 e3psi-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     7425 2022-09-01 10:35:52.505704 e3psi-0.2.0/.gitignore
--rw-r--r--   0        0        0      887 2022-09-21 13:40:54.655359 e3psi-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     7652 2022-08-08 10:40:28.332088 e3psi-0.2.0/LICENSE
--rw-r--r--   0        0        0     3628 2022-09-21 12:54:18.528047 e3psi-0.2.0/README.md
--rw-r--r--   0        0        0      220 2022-09-21 13:13:32.142227 e3psi-0.2.0/e3psi/__init__.py
--rw-r--r--   0        0        0     3984 2022-11-08 16:40:06.915912 e3psi-0.2.0/e3psi/graphs.py
--rw-r--r--   0        0        0     8941 2022-11-08 16:37:16.527860 e3psi-0.2.0/e3psi/models.py
--rw-r--r--   0        0        0      218 2022-10-07 12:28:08.438364 e3psi-0.2.0/e3psi/provides.py
--rw-r--r--   0        0        0      353 2022-11-08 16:47:32.871601 e3psi-0.2.0/e3psi/version.py
--rw-r--r--   0        0        0     1772 2022-11-08 16:36:51.335853 e3psi-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       35 2022-08-08 10:16:14.742612 e3psi-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     2277 2022-10-05 19:39:34.373140 e3psi-0.2.0/tests/test_graphs.py
--rw-r--r--   0        0        0     1639 2022-10-05 19:39:34.373140 e3psi-0.2.0/tests/test_models.py
--rw-r--r--   0        0        0     4840 1970-01-01 00:00:00.000000 e3psi-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       59 2022-09-21 13:31:15.699437 e3psi-0.3.0/.bandit
+-rw-r--r--   0        0        0     1413 2022-08-08 10:16:14.742612 e3psi-0.3.0/.circleci/config.yml
+-rw-r--r--   0        0        0       71 2022-08-08 10:16:14.730612 e3psi-0.3.0/.coveragerc
+-rw-r--r--   0        0        0      284 2022-08-08 10:16:14.730612 e3psi-0.3.0/.deepsource.toml
+-rw-r--r--   0        0        0      289 2022-08-08 10:16:14.742612 e3psi-0.3.0/.editorconfig
+-rw-r--r--   0        0        0      147 2022-11-08 16:48:14.951381 e3psi-0.3.0/.flake8
+-rw-r--r--   0        0        0      209 2022-08-08 10:16:14.718612 e3psi-0.3.0/.gitattributes
+-rw-r--r--   0        0        0      238 2022-08-08 10:16:14.750611 e3psi-0.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1272 2022-11-08 16:48:14.951381 e3psi-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     7425 2022-09-01 10:35:52.505704 e3psi-0.3.0/.gitignore
+-rw-r--r--   0        0        0      887 2023-04-10 16:53:58.648745 e3psi-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     7652 2022-08-08 10:40:28.332088 e3psi-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3628 2022-09-21 12:54:18.528047 e3psi-0.3.0/README.md
+-rw-r--r--   0        0        0      315 2023-04-10 16:53:58.648745 e3psi-0.3.0/e3psi/__init__.py
+-rw-r--r--   0        0        0     4627 2023-04-10 16:53:58.648745 e3psi-0.3.0/e3psi/base.py
+-rw-r--r--   0        0        0     1088 2023-04-10 16:53:58.648745 e3psi-0.3.0/e3psi/distances.py
+-rw-r--r--   0        0        0     3529 2023-04-10 16:53:58.648745 e3psi-0.3.0/e3psi/graphs.py
+-rw-r--r--   0        0        0     1261 2023-04-10 16:53:58.648745 e3psi-0.3.0/e3psi/mincepy_types.py
+-rw-r--r--   0        0        0     8999 2023-04-10 17:00:15.902417 e3psi-0.3.0/e3psi/models.py
+-rw-r--r--   0        0        0      232 2023-04-10 16:53:58.652745 e3psi-0.3.0/e3psi/provides.py
+-rw-r--r--   0        0        0      353 2023-04-10 17:04:27.760309 e3psi-0.3.0/e3psi/version.py
+-rw-r--r--   0        0        0     1772 2022-11-08 16:48:14.955381 e3psi-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       35 2022-08-08 10:16:14.742612 e3psi-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     2277 2022-10-05 19:39:34.373140 e3psi-0.3.0/tests/test_graphs.py
+-rw-r--r--   0        0        0     1684 2023-04-10 16:53:58.652745 e3psi-0.3.0/tests/test_models.py
+-rw-r--r--   0        0        0     4840 1970-01-01 00:00:00.000000 e3psi-0.3.0/PKG-INFO
```

### Comparing `e3psi-0.2.0/.circleci/config.yml` & `e3psi-0.3.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `e3psi-0.2.0/.github/workflows/ci.yml` & `e3psi-0.3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `e3psi-0.2.0/.gitignore` & `e3psi-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `e3psi-0.2.0/.pre-commit-config.yaml` & `e3psi-0.3.0/.pre-commit-config.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
     -   id: check-added-large-files
         args: ['--maxkb=5000']
     -   id: end-of-file-fixer
     -   id: check-case-conflict
     -   id: detect-private-key
     -   id: check-docstring-first
 -   repo: https://github.com/psf/black
-    rev: 22.6.0
+    rev: 23.3.0
     hooks:
     -   id: black
         exclude: (.*)/migrations
-- repo: https://gitlab.com/PyCQA/flake8
-  rev: 3.9.2
+- repo: https://github.com/PyCQA/flake8
+  rev: 6.0.0
   hooks:
     - id: flake8
 -   repo: https://github.com/PyCQA/bandit
-    rev: 1.7.4
+    rev: 1.7.5
     hooks:
     - id: bandit
       args: [ "-c", "pyproject.toml" ]
       additional_dependencies: [ "bandit[toml]" ]
 - repo: https://github.com/commitizen-tools/commitizen
-  rev: v2.29.5
+  rev: v2.42.1
   hooks:
     - id: commitizen
       stages: [commit-msg]
```

### Comparing `e3psi-0.2.0/LICENSE` & `e3psi-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `e3psi-0.2.0/README.md` & `e3psi-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `e3psi-0.2.0/e3psi/models.py` & `e3psi-0.3.0/e3psi/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import abc
 import uuid
 from typing import Union, Tuple
 
-import mincepy
 from mincepy_sci import pytorch_types
-import mincepy_sci.pytorch_types
 from e3nn import nn
 from e3nn import o3
 import torch
 
+from . import base
 from . import graphs
 
 __all__ = "OnsiteModel", "IntersiteModel", "Model"
 
 
 class Module(torch.nn.Module):
     @property
@@ -42,41 +41,44 @@
         x = self.first(*input)
         return self.second(x)
 
 
 class Model(Module, pytorch_types.SavableModuleMixin, abc.ABC):
     @property
     @abc.abstractmethod
-    def graph(self) -> graphs.AbstractObj:
+    def graph(self) -> base.AbstractObj:
         """Get the graph that described this model"""
 
     def __hash__(self):
         return object.__hash__(self)
 
 
 class OnsiteModel(Model):
     """Model for predicting onsite values i.e. a node with self interactions"""
 
     def __init__(
         self,
-        graph: graphs.AbstractObj,
-        nn_irreps_out: Union[str, o3.Irreps] = None,
+        graph: graphs.OneSite,
+        feature_irreps: Union[str, o3.Irreps] = None,
         irreps_out="0e",
         irrep_normalization="component",
         hidden_layers=1,
         rescaler=None,
     ):
+        if not isinstance(graph, graphs.OneSite):
+            raise ValueError(
+                f"Expected '{graphs.OneSite.__name__}' instance, got '{graph.__class__.__name__}'"
+            )
         super().__init__()
 
         self._graph = graph
-        # self.irreps_in = o3.Irrep('0e') + self._graph.irreps
-        self.irreps_in = self._graph.irreps
+        self.irreps_in = base.irreps(self._graph.site)
         feature_irreps = (
-            o3.Irreps(nn_irreps_out)
-            if nn_irreps_out is not None
+            o3.Irreps(feature_irreps)
+            if feature_irreps is not None
             else o3.ReducedTensorProducts("ij=ji", i=self.irreps_in).irreps_out
         )
 
         # First layer
         self.layers = torch.nn.ModuleList(
             _self_interaction(
                 self.irreps_in, feature_irreps, irrep_normalization=irrep_normalization
@@ -108,20 +110,14 @@
 
     @property
     def graph(self):
         return self._graph
 
     def forward(self, inputs: torch.Tensor) -> torch.Tensor:
         out = inputs["site"]
-        # if len(out.shape) == 2:
-        #     one = torch.ones(out.shape[0], 1, dtype=out.dtype, device=out.device)
-        # else:
-        #     one = torch.ones(1, dtype=out.dtype, device=out.device)
-        #
-        # out = torch.hstack((one, out))
 
         for layer in self.layers:
             out = layer(out)
 
         return out
 
 
@@ -129,44 +125,49 @@
     """Model for predicting intersite values, i.e. a two-body property"""
 
     TYPE_ID = uuid.UUID("8d3f024e-c9d7-48d0-92e1-88448d483936")
 
     def __init__(
         self,
         graph: graphs.TwoSite,
-        n1n2_irreps_out=None,
-        n1n2e_irreps_out=None,
+        node_features=None,
         irreps_out="0e",
         hidden_layers=1,
         irrep_normalization="component",
         rescaler=None,
     ):
+        if not isinstance(graph, graphs.TwoSite):
+            raise ValueError(
+                f"Expected '{graphs.TwoSite.__name__}' instance, got '{graph.__class__.__name__}'"
+            )
         super().__init__()
         self._graph = graph
         self.layers = torch.nn.ModuleList()
 
         # Node-node TP
         node_node_tp_irreps_out = (
-            o3.Irreps(n1n2_irreps_out)
-            if n1n2_irreps_out is not None
-            else o3.FullTensorProduct(self.graph.site1.irreps, self.graph.site2.irreps).irreps_out
+            o3.Irreps(node_features)
+            if node_features is not None
+            else o3.FullTensorProduct(
+                base.irreps(self.graph.site1), base.irreps(self.graph.site2)
+            ).irreps_out
         )
 
         # Input layers
         self.node_node_tp = o3.FullyConnectedTensorProduct(
-            self.graph.site1.irreps,
-            self.graph.site2.irreps,
+            base.irreps(self.graph.site1),
+            base.irreps(self.graph.site2),
             irreps_out=node_node_tp_irreps_out,
             irrep_normalization="component",
         )
 
         # Node-node output * edge TP
         node_node_edge_tp_irreps_out = (
-            o3.Irreps(n1n2e_irreps_out)
-            if n1n2e_irreps_out is not None
+            o3.Irreps(node_features)
+            if node_features is not None
             else o3.FullTensorProduct(
                 self.node_node_tp.irreps_out, self.graph.edge.irreps
             ).irreps_out
         )
 
         self.node_node_edge_tp, gate = _interaction(
             node_node_tp_irreps_out,
@@ -177,15 +178,15 @@
 
         self.layers.append(gate)
 
         # Intermediate layers
         if hidden_layers > 1:
             # Intermediate hidden
             for _ in range(hidden_layers - 1):
-                self.layers.append(
+                self.layers.extend(
                     _self_interaction(
                         self.layers[-1].irreps_out,
                         irreps_out=node_node_edge_tp_irreps_out,
                         irrep_normalization=irrep_normalization,
                     )
                 )
```

### Comparing `e3psi-0.2.0/pyproject.toml` & `e3psi-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `e3psi-0.2.0/tests/test_graphs.py` & `e3psi-0.3.0/tests/test_graphs.py`

 * *Files identical despite different names*

### Comparing `e3psi-0.2.0/tests/test_models.py` & `e3psi-0.3.0/tests/test_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,28 +9,29 @@
 from mincepy import testing
 from mincepy.testing import historian, mongodb_archive, archive_uri
 
 
 def test_onsite_save_load(historian: mincepy.Historian):  # noqa: F811
     # Build the model
     site = e3psi.IrrepsObj(species=e3psi.Attr("4x0e"), pos=e3psi.Attr("1e"))
+    graph = e3psi.OneSite(site)
 
     torch.manual_seed(0)
-    model = e3psi.OnsiteModel(site)
+    model = e3psi.OnsiteModel(graph)
 
     # Create random inputs
     data = dict(site=site.irreps.randn(-1))
     ref_out = model(data)  # Reference output
 
     # Save/load a new model
     torch.manual_seed(0)
-    loaded = testing.do_round_trip(historian, e3psi.OnsiteModel, site)
+    loaded = testing.do_round_trip(historian, e3psi.OnsiteModel, graph)
 
     # Check that all agrees
-    assert loaded.graph == site
+    assert loaded.graph.site == graph.site
     assert torch.allclose(ref_out, loaded(data))
 
 
 def test_intersite_save_load(historian: mincepy.Historian):  # noqa: F811
     # Build the model
     site1 = e3psi.IrrepsObj(species=e3psi.Attr("4x0e"), pos=e3psi.Attr("1e"))
     site2 = e3psi.IrrepsObj(species=e3psi.Attr("4x0e"), pos=e3psi.Attr("1e"))
```

### Comparing `e3psi-0.2.0/PKG-INFO` & `e3psi-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e3psi
-Version: 0.2.0
+Version: 0.3.0
 Summary: Equivariant machine learning library for learning from electronic structures.
 Keywords: machine learning,equivariant,electronic structure
 Author-email: Martin Uhrin <martin.uhrin.10@ucl.ac.uk>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

