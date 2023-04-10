# Comparing `tmp/antelope_background-0.2.0.tar.gz` & `tmp/antelope_background-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antelope_background-0.2.0.tar", last modified: Thu Apr  6 23:20:17 2023, max compression
+gzip compressed data, was "antelope_background-0.2.1.tar", last modified: Mon Apr 10 21:46:06 2023, max compression
```

## Comparing `antelope_background-0.2.0.tar` & `antelope_background-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-06 23:20:17.265422 antelope_background-0.2.0/
--rw-r--r--   0 b          (500) b          (506)     1520 2020-09-29 23:44:37.000000 antelope_background-0.2.0/LICENSE
--rw-r--r--   0 b          (500) b          (506)     3732 2023-04-06 23:20:17.265422 antelope_background-0.2.0/PKG-INFO
--rw-r--r--   0 b          (500) b          (506)     3471 2021-03-10 07:59:31.000000 antelope_background-0.2.0/README.md
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-06 23:20:17.262089 antelope_background-0.2.0/antelope_background/
--rw-r--r--   0 b          (500) b          (506)     2069 2020-09-27 08:37:50.000000 antelope_background-0.2.0/antelope_background/__init__.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-06 23:20:17.265422 antelope_background-0.2.0/antelope_background/background/
--rw-r--r--   0 b          (500) b          (506)      115 2020-09-29 23:50:36.000000 antelope_background-0.2.0/antelope_background/background/__init__.py
--rw-r--r--   0 b          (500) b          (506)    23792 2023-04-05 07:40:09.000000 antelope_background-0.2.0/antelope_background/background/flat_background.py
--rw-r--r--   0 b          (500) b          (506)    10673 2023-04-05 07:40:09.000000 antelope_background-0.2.0/antelope_background/background/implementation.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-06 23:20:17.265422 antelope_background-0.2.0/antelope_background/background/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2018-07-20 18:48:36.000000 antelope_background-0.2.0/antelope_background/background/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     1621 2020-09-29 23:57:25.000000 antelope_background-0.2.0/antelope_background/background/tests/test_flat_background.py
--rw-r--r--   0 b          (500) b          (506)      145 2021-03-10 07:42:08.000000 antelope_background-0.2.0/antelope_background/background/tests/test_implementation.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-06 23:20:17.265422 antelope_background-0.2.0/antelope_background/engine/
--rw-r--r--   0 b          (500) b          (506)      346 2020-03-30 08:22:53.000000 antelope_background-0.2.0/antelope_background/engine/__init__.py
--rw-r--r--   0 b          (500) b          (506)    29699 2021-09-21 18:51:33.000000 antelope_background-0.2.0/antelope_background/engine/background_engine.py
--rw-r--r--   0 b          (500) b          (506)     2217 2021-01-29 21:46:30.000000 antelope_background-0.2.0/antelope_background/engine/emission.py
--rw-r--r--   0 b          (500) b          (506)     4656 2021-09-21 18:51:33.000000 antelope_background-0.2.0/antelope_background/engine/product_flow.py
--rw-r--r--   0 b          (500) b          (506)    10150 2018-07-20 18:48:36.000000 antelope_background-0.2.0/antelope_background/engine/tarjan_stack.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-06 23:20:17.265422 antelope_background-0.2.0/antelope_background/providers/
--rw-r--r--   0 b          (500) b          (506)      136 2022-08-25 07:41:55.000000 antelope_background-0.2.0/antelope_background/providers/__init__.py
--rw-r--r--   0 b          (500) b          (506)     2785 2021-09-21 18:51:33.000000 antelope_background-0.2.0/antelope_background/providers/bm_static.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-06 23:20:17.262089 antelope_background-0.2.0/antelope_background.egg-info/
--rw-r--r--   0 b          (500) b          (506)     3732 2023-04-06 23:20:17.000000 antelope_background-0.2.0/antelope_background.egg-info/PKG-INFO
--rw-r--r--   0 b          (500) b          (506)      881 2023-04-06 23:20:17.000000 antelope_background-0.2.0/antelope_background.egg-info/SOURCES.txt
--rw-r--r--   0 b          (500) b          (506)        1 2023-04-06 23:20:17.000000 antelope_background-0.2.0/antelope_background.egg-info/dependency_links.txt
--rw-r--r--   0 b          (500) b          (506)       44 2023-04-06 23:20:17.000000 antelope_background-0.2.0/antelope_background.egg-info/requires.txt
--rw-r--r--   0 b          (500) b          (506)       20 2023-04-06 23:20:17.000000 antelope_background-0.2.0/antelope_background.egg-info/top_level.txt
--rw-r--r--   0 b          (500) b          (506)       38 2023-04-06 23:20:17.265422 antelope_background-0.2.0/setup.cfg
--rw-r--r--   0 b          (500) b          (506)     1382 2023-04-06 22:45:36.000000 antelope_background-0.2.0/setup.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:46:06.502977 antelope_background-0.2.1/
+-rw-r--r--   0 b          (500) b          (506)     1520 2020-09-29 23:44:37.000000 antelope_background-0.2.1/LICENSE
+-rw-r--r--   0 b          (500) b          (506)     3732 2023-04-10 21:46:06.502977 antelope_background-0.2.1/PKG-INFO
+-rw-r--r--   0 b          (500) b          (506)     3471 2021-03-10 07:59:31.000000 antelope_background-0.2.1/README.md
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:46:06.499644 antelope_background-0.2.1/antelope_background/
+-rw-r--r--   0 b          (500) b          (506)     2069 2020-09-27 08:37:50.000000 antelope_background-0.2.1/antelope_background/__init__.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:46:06.499644 antelope_background-0.2.1/antelope_background/background/
+-rw-r--r--   0 b          (500) b          (506)      115 2020-09-29 23:50:36.000000 antelope_background-0.2.1/antelope_background/background/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    24312 2023-04-08 18:32:32.000000 antelope_background-0.2.1/antelope_background/background/flat_background.py
+-rw-r--r--   0 b          (500) b          (506)    10673 2023-04-08 18:31:19.000000 antelope_background-0.2.1/antelope_background/background/implementation.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:46:06.499644 antelope_background-0.2.1/antelope_background/background/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2018-07-20 18:48:36.000000 antelope_background-0.2.1/antelope_background/background/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     1621 2020-09-29 23:57:25.000000 antelope_background-0.2.1/antelope_background/background/tests/test_flat_background.py
+-rw-r--r--   0 b          (500) b          (506)      145 2021-03-10 07:42:08.000000 antelope_background-0.2.1/antelope_background/background/tests/test_implementation.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:46:06.499644 antelope_background-0.2.1/antelope_background/engine/
+-rw-r--r--   0 b          (500) b          (506)      346 2020-03-30 08:22:53.000000 antelope_background-0.2.1/antelope_background/engine/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    29699 2021-09-21 18:51:33.000000 antelope_background-0.2.1/antelope_background/engine/background_engine.py
+-rw-r--r--   0 b          (500) b          (506)     2217 2021-01-29 21:46:30.000000 antelope_background-0.2.1/antelope_background/engine/emission.py
+-rw-r--r--   0 b          (500) b          (506)     4656 2021-09-21 18:51:33.000000 antelope_background-0.2.1/antelope_background/engine/product_flow.py
+-rw-r--r--   0 b          (500) b          (506)    10150 2018-07-20 18:48:36.000000 antelope_background-0.2.1/antelope_background/engine/tarjan_stack.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:46:06.502977 antelope_background-0.2.1/antelope_background/providers/
+-rw-r--r--   0 b          (500) b          (506)      136 2022-08-25 07:41:55.000000 antelope_background-0.2.1/antelope_background/providers/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     2785 2021-09-21 18:51:33.000000 antelope_background-0.2.1/antelope_background/providers/bm_static.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:46:06.499644 antelope_background-0.2.1/antelope_background.egg-info/
+-rw-r--r--   0 b          (500) b          (506)     3732 2023-04-10 21:46:06.000000 antelope_background-0.2.1/antelope_background.egg-info/PKG-INFO
+-rw-r--r--   0 b          (500) b          (506)      881 2023-04-10 21:46:06.000000 antelope_background-0.2.1/antelope_background.egg-info/SOURCES.txt
+-rw-r--r--   0 b          (500) b          (506)        1 2023-04-10 21:46:06.000000 antelope_background-0.2.1/antelope_background.egg-info/dependency_links.txt
+-rw-r--r--   0 b          (500) b          (506)       44 2023-04-10 21:46:06.000000 antelope_background-0.2.1/antelope_background.egg-info/requires.txt
+-rw-r--r--   0 b          (500) b          (506)       20 2023-04-10 21:46:06.000000 antelope_background-0.2.1/antelope_background.egg-info/top_level.txt
+-rw-r--r--   0 b          (500) b          (506)       38 2023-04-10 21:46:06.502977 antelope_background-0.2.1/setup.cfg
+-rw-r--r--   0 b          (500) b          (506)     1491 2023-04-10 21:35:01.000000 antelope_background-0.2.1/setup.py
```

### Comparing `antelope_background-0.2.0/LICENSE` & `antelope_background-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.0/PKG-INFO` & `antelope_background-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antelope_background
-Version: 0.2.0
+Version: 0.2.1
 Home-page: https://github.com/AntelopeLCA/background
 Author: Brandon Kuczenski
 Author-email: bkuczenski@ucsb.edu
 License: BSD 3-clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `antelope_background-0.2.0/README.md` & `antelope_background-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.0/antelope_background/__init__.py` & `antelope_background-0.2.1/antelope_background/__init__.py`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.0/antelope_background/background/flat_background.py` & `antelope_background-0.2.1/antelope_background/background/flat_background.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 from scipy.sparse import csc_matrix, csr_matrix
 from scipy.sparse.linalg import inv, factorized, spsolve
 from scipy.sparse import eye
 from scipy.io import savemat, loadmat
 
 import os
-from collections import namedtuple, defaultdict
+from collections import namedtuple
 
 from antelope import CONTEXT_STATUS_, comp_dir  # , num_dir
+from antelope.models import UnallocatedExchange, Exchange
 from ..engine import BackgroundEngine
 from antelope_core import from_json, to_json
-from antelope_core.contexts import Context
 
 
 SUPPORTED_FILETYPES = ('.mat', )
 
 _FLATTEN_AF = False
 
 
@@ -69,14 +69,22 @@
     def __array__(self):
         return self.flow_ref, self._d, self.term_ref, self._s
 
     def __iter__(self):
         return iter(self.__array__())
 
 
+"""
+An ExchDef is a serialized exchange definition. It should contain:
+.process = a string node ref
+.flow = a string flow ref
+.direction = a valid direction
+.term = EITHER a string term_ref (interior flow) OR a tuple of strings (context) OR None (cutoff)
+.value = float
+"""
 ExchDef = namedtuple('ExchDef', ('process', 'flow', 'direction', 'term', 'value'))
 
 
 def _iterate_a_matrix(a, y, threshold=1e-8, count=100, quiet=False, solver=None):
     if solver == 'spsolve':
         ima = eye(a.shape[0]) - a
         x = spsolve(ima, y)
@@ -162,16 +170,18 @@
 
     non, scc = split_af(af, scc_inds)
 
     scc_inv = inv(eye(ts.pdim).tocsc() - scc)
 
     return non * scc_inv, ad * scc_inv, bf * scc_inv
 
+
 ORDERING_SUFFIX = '.ordering.json.gz'
 
+
 class FlatBackground(object):
     """
     Static, ordered background stored in an easily serializable way
     """
     @classmethod
     def from_index(cls, index, quiet=True, **kwargs):
         """
@@ -583,67 +593,82 @@
             return 1
         return -1
 
     def sys_lci(self, demand, quiet=None, **kwargs):
         """
 
         :param demand: an iterable of exchanges, each of which must be mapped to a foreground, interior, or exterior
-        TermRef
+        TermRef. The exchanges can either be proper exchanges, or ExchangeRefs, or UnallocatedExchange or
+        AllocatedExchange models
+        :param quiet: whether to silence debugging info
         :return:
         """
         node_ref = None
-        data = defaultdict(list)
-        for x in demand:
+
+        fg_ind = []
+        fg_val = []
+        bg_ind = []
+        bg_val = []
+        ex_ind = []
+        ex_val = []
+
+        missed = []
+
+        for exch in demand:
+
+            if isinstance(exch, Exchange):  # the model
+                x = exch
+            else:
+                x = UnallocatedExchange.from_inv(exch)
+
             if node_ref is None:  # just take the first one
-                node_ref = x.process.external_ref
-            if isinstance(x.termination, Context):
-                key = ('; '.join(x.termination.as_list()), x.flow.external_ref, comp_dir(x.direction))
-                try:
-                    ind = self._ex_index[key]
-                    data['ex_ind'].append(ind)
-                    data['ex_val'].append(x.value * self._check_dirn(self._ex[ind], x))
-                except KeyError:
-                    data['missed'].append(x)
+                node_ref = x.process
+            if x.type == 'context':
+                missed.append(ExchDef(x.process, x.flow.external_ref, x.direction,
+                                      tuple(x.context), x.value))
             elif x.termination is None:
-                data['missed'].append(x)
+                missed.append(ExchDef(x.process, x.flow.external_ref, x.direction, None, x.value))
             else:
                 key = (x.termination, x.flow.external_ref)
                 if key in self._fg_index:
                     ind = self._fg_index[key]
-                    data['fg_ind'].append(ind)
-                    data['fg_val'].append(x.value * self._check_dirn(self._fg[ind], x))
+                    fg_ind.append(ind)
+                    fg_val.append(x.value * self._check_dirn(self._fg[ind], x))
                 elif key in self._bg_index:
                     ind = self._bg_index[key]
-                    data['bg_ind'].append(ind)
-                    data['bg_val'].append(x.value * self._check_dirn(self._bg[ind], x))
+                    bg_ind.append(ind)
+                    bg_val.append(x.value * self._check_dirn(self._bg[ind], x))
                 else:
-                    data['missed'].append(x)
+                    xd = ExchDef(x.process, key[1], x.direction, key[0], x.value)
+                    if not quiet:
+                        print('missed %s-%s-%s-%s-%s' % xd)
+                    missed.append(xd)
 
         # compute ad_tilde  # csr_matrix(((1,), ((inx,), (0,))), shape=(dim, 1))
-        x_dmd = csr_matrix((data['fg_val'], (data['fg_ind'], [0]*len(data['fg_ind']))), shape=(self.pdim, 1))
+        x_dmd = csr_matrix((fg_val, (fg_ind, [0]*len(fg_ind))), shape=(self.pdim, 1))
         x_tilde = _iterate_a_matrix(self._af, x_dmd, quiet=True, **kwargs)
         ad_tilde = self._ad.dot(x_tilde).todense()
         bf_tilde = self._bf.dot(x_tilde).todense()
 
         # consolidate bg dependencies
-        for i in range(len(data['bg_ind'])):
-            ad_tilde[data['bg_ind'][i]] += data['bg_val'][i]
+        for i in range(len(bg_ind)):
+            ad_tilde[bg_ind[i]] += bg_val[i]
 
         # compute b
         bx = self._compute_bg_lci(ad_tilde, quiet=quiet, **kwargs) + bf_tilde
 
         # consolidate direct emissions
-        for i in range(len(data['ex_ind'])):
-            bx[data['ex_ind'][i]] += data['ex_val'][i]
+        for i in range(len(ex_ind)):
+            bx[ex_ind[i]] += ex_val[i]
 
         for x in self._generate_em_defs(node_ref, csr_matrix(bx)):
             yield x
 
-        for x in data['missed']:
-            yield ExchDef(x.process, x.flow, x.direction, x.termination, x.value)
+        for x in missed:  #
+            yield x
 
     def _write_ordering(self, filename):
         if not filename.endswith(ORDERING_SUFFIX):
             filename += ORDERING_SUFFIX
 
         ordr = {'foreground': [tuple(f) for f in self._fg],
                 'background': [tuple(f) for f in self._bg],
```

### Comparing `antelope_background-0.2.0/antelope_background/background/implementation.py` & `antelope_background-0.2.1/antelope_background/background/implementation.py`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.0/antelope_background/background/tests/test_flat_background.py` & `antelope_background-0.2.1/antelope_background/background/tests/test_flat_background.py`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.0/antelope_background/engine/background_engine.py` & `antelope_background-0.2.1/antelope_background/engine/background_engine.py`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.0/antelope_background/engine/emission.py` & `antelope_background-0.2.1/antelope_background/engine/emission.py`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.0/antelope_background/engine/product_flow.py` & `antelope_background-0.2.1/antelope_background/engine/product_flow.py`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.0/antelope_background/engine/tarjan_stack.py` & `antelope_background-0.2.1/antelope_background/engine/tarjan_stack.py`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.0/antelope_background/providers/bm_static.py` & `antelope_background-0.2.1/antelope_background/providers/bm_static.py`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.0/antelope_background.egg-info/PKG-INFO` & `antelope_background-0.2.1/antelope_background.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antelope-background
-Version: 0.2.0
+Version: 0.2.1
 Home-page: https://github.com/AntelopeLCA/background
 Author: Brandon Kuczenski
 Author-email: bkuczenski@ucsb.edu
 License: BSD 3-clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `antelope_background-0.2.0/antelope_background.egg-info/SOURCES.txt` & `antelope_background-0.2.1/antelope_background.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.0/setup.py` & `antelope_background-0.2.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from setuptools import setup, find_packages
 
 requires = [
-    "antelope_core>=0.2.0",
+    "antelope_core>=0.2.1",
     "scipy>=1.5",
     "numpy>=1.19"
 ]
 
 """
 Change Log
+0.2.1 - 2023-04-10 - xdb passes benchmarks.
+                     sys_lci running both locally and remotely.
+
 0.2.0 - 2023-04-06 - Redefine sys_lci to omit spurious node argument. sync with virtualize branches upstream.
                      TODO: get rid of tail recursion in background Tarjan engine
 
 0.1.8 - 2022-04-08 - version bump release to match core 0.1.8
  - Normalize how contexts are serialized and deserialized
  - add 'emitters' API route
  - preferred provider catch-all config
@@ -21,15 +24,15 @@
 0.1.5 - 2021-02-05 - bump version to keep pace with antelope_core 
 0.1.4 - 2021-01-29 - bugfixes to get CI passing.  match consistent versions with other packages.
 
 0.1.0 - 2021-01-06 - first published release
 """
 
 
-VERSION = '0.2.0'
+VERSION = '0.2.1'
 
 setup(
     name="antelope_background",
     version=VERSION,
     author="Brandon Kuczenski",
     author_email="bkuczenski@ucsb.edu",
     license="BSD 3-clause",
```

