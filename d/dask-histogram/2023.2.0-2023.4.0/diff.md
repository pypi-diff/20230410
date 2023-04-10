# Comparing `tmp/dask_histogram-2023.2.0.tar.gz` & `tmp/dask_histogram-2023.4.0.tar.gz`

## Comparing `dask_histogram-2023.2.0.tar` & `dask_histogram-2023.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 dask_histogram-2023.2.0/src/dask_histogram/__init__.py
--rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 dask_histogram-2023.2.0/src/dask_histogram/bins.py
--rw-r--r--   0        0        0    29132 2020-02-02 00:00:00.000000 dask_histogram-2023.2.0/src/dask_histogram/boost.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 dask_histogram-2023.2.0/src/dask_histogram/config.py
--rw-r--r--   0        0        0    36284 2020-02-02 00:00:00.000000 dask_histogram-2023.2.0/src/dask_histogram/core.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 dask_histogram-2023.2.0/src/dask_histogram/histogram.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_histogram-2023.2.0/src/dask_histogram/py.typed
--rw-r--r--   0        0        0    16836 2020-02-02 00:00:00.000000 dask_histogram-2023.2.0/src/dask_histogram/routines.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 dask_histogram-2023.2.0/src/dask_histogram/sizeof.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dask_histogram-2023.2.0/src/dask_histogram/typing.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_histogram-2023.2.0/src/dask_histogram/version.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 dask_histogram-2023.2.0/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_histogram-2023.2.0/LICENSE
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 dask_histogram-2023.2.0/README.md
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 dask_histogram-2023.2.0/pyproject.toml
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 dask_histogram-2023.2.0/PKG-INFO
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/src/dask_histogram/__init__.py
+-rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/src/dask_histogram/bins.py
+-rw-r--r--   0        0        0    29132 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/src/dask_histogram/boost.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/src/dask_histogram/config.py
+-rw-r--r--   0        0        0    36197 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/src/dask_histogram/core.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/src/dask_histogram/histogram.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/src/dask_histogram/py.typed
+-rw-r--r--   0        0        0    16836 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/src/dask_histogram/routines.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/src/dask_histogram/sizeof.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/src/dask_histogram/typing.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/src/dask_histogram/version.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/LICENSE
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/README.md
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/PKG-INFO
```

### Comparing `dask_histogram-2023.2.0/src/dask_histogram/__init__.py` & `dask_histogram-2023.4.0/src/dask_histogram/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.2.0/src/dask_histogram/bins.py` & `dask_histogram-2023.4.0/src/dask_histogram/bins.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.2.0/src/dask_histogram/boost.py` & `dask_histogram-2023.4.0/src/dask_histogram/boost.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.2.0/src/dask_histogram/core.py` & `dask_histogram-2023.4.0/src/dask_histogram/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -684,22 +684,20 @@
 
 
 def _dependencies(
     *args: DaskCollection,
     weights: DaskCollection | None = None,
     sample: DaskCollection | None = None,
 ) -> tuple[DaskCollection, ...]:
-    dask_args = tuple(arg for arg in args if is_dask_collection(arg))
-    if weights is not None and sample is None:
-        return (*dask_args, weights)
-    elif weights is None and sample is not None:
-        return (*dask_args, sample)
-    elif weights is not None and sample is not None:
-        return (*dask_args, weights, sample)
-    return dask_args
+    dask_args = [arg for arg in args if is_dask_collection(arg)]
+    if is_dask_collection(weights):
+        dask_args.append(weights)
+    if is_dask_collection(sample):
+        dask_args.append(sample)
+    return tuple(dask_args)
 
 
 def _weight_sample_check(
     *data: DaskCollection,
     weights: DaskCollection | None = None,
     sample: DaskCollection | None = None,
 ) -> int:
@@ -789,15 +787,16 @@
 ) -> PartitionedHistogram:
     name = f"hist-on-block-{tokenize(data, histref, weights, sample, split_every)}"
     dask_data = tuple(datum for datum in data if is_dask_collection(datum))
     if len(dask_data) == 0:
         dask_data = data
     data_is_df = is_dataframe_like(dask_data[0])
     data_is_dak = is_dask_awkward_like(dask_data[0])
-    _weight_sample_check(*dask_data, weights=weights)
+    if is_dask_collection(weights):
+        _weight_sample_check(*dask_data, weights=weights)
 
     # Single awkward array object.
     if len(data) == 1 and data_is_dak:
         from dask_awkward.lib.core import partitionwise_layer as dak_pwl
 
         x = data[0]
         if weights is not None and sample is not None:
```

### Comparing `dask_histogram-2023.2.0/src/dask_histogram/routines.py` & `dask_histogram-2023.4.0/src/dask_histogram/routines.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.2.0/src/dask_histogram/sizeof.py` & `dask_histogram-2023.4.0/src/dask_histogram/sizeof.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.2.0/.gitignore` & `dask_histogram-2023.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.2.0/LICENSE` & `dask_histogram-2023.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.2.0/README.md` & `dask_histogram-2023.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.2.0/pyproject.toml` & `dask_histogram-2023.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.2.0/PKG-INFO` & `dask_histogram-2023.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-histogram
-Version: 2023.2.0
+Version: 2023.4.0
 Summary: Histogramming with Dask.
 Project-URL: Homepage, https://github.com/dask-contrib/dask-histogram
 Project-URL: Documentation, https://dask-histogram.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/dask-contrib/dask-histogram/issues
 Author-email: Doug Davis <ddavis@ddavis.io>
 License: BSD-3-Clause
 License-File: LICENSE
```

