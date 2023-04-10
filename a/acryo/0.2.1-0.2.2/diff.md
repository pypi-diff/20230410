# Comparing `tmp/acryo-0.2.1.tar.gz` & `tmp/acryo-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acryo-0.2.1.tar", last modified: Wed Mar 15 04:52:43 2023, max compression
+gzip compressed data, was "acryo-0.2.2.tar", last modified: Mon Apr 10 14:05:45 2023, max compression
```

## Comparing `acryo-0.2.1.tar` & `acryo-0.2.2.tar`

### file list

```diff
@@ -1,54 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-03-15 04:52:43.600284 acryo-0.2.1/
--rw-rw-rw-   0        0        0     1547 2022-04-12 12:12:07.000000 acryo-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     2301 2023-03-15 04:52:43.597285 acryo-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2011 2023-03-15 04:48:31.000000 acryo-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-15 04:52:43.415726 acryo-0.2.1/acryo/
--rw-rw-rw-   0        0        0      380 2023-03-02 06:44:45.000000 acryo-0.2.1/acryo/__init__.py
--rw-rw-rw-   0        0        0    10606 2023-03-02 06:44:45.000000 acryo-0.2.1/acryo/_correlation.py
--rw-rw-rw-   0        0        0      661 2023-02-19 09:29:23.000000 acryo-0.2.1/acryo/_fft.py
--rw-rw-rw-   0        0        0     2929 2023-02-20 00:46:56.000000 acryo-0.2.1/acryo/_reader.py
--rw-rw-rw-   0        0        0     2784 2023-03-02 06:44:45.000000 acryo-0.2.1/acryo/_rotation.py
--rw-rw-rw-   0        0        0      244 2023-02-23 14:34:20.000000 acryo-0.2.1/acryo/_types.py
--rw-rw-rw-   0        0        0    11498 2023-02-21 08:34:02.000000 acryo-0.2.1/acryo/_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-15 04:52:43.483723 acryo-0.2.1/acryo/alignment/
--rw-rw-rw-   0        0        0      384 2023-03-02 06:44:45.000000 acryo-0.2.1/acryo/alignment/__init__.py
--rw-rw-rw-   0        0        0    25875 2023-03-02 06:44:45.000000 acryo-0.2.1/acryo/alignment/_base.py
--rw-rw-rw-   0        0        0     1637 2023-03-02 06:44:45.000000 acryo-0.2.1/acryo/alignment/_concrete.py
-drwxrwxrwx   0        0        0        0 2023-03-15 04:52:43.499158 acryo-0.2.1/acryo/classification/
--rw-rw-rw-   0        0        0       62 2022-04-12 15:56:50.000000 acryo-0.2.1/acryo/classification/__init__.py
--rw-rw-rw-   0        0        0    18578 2023-02-08 03:31:15.000000 acryo-0.2.1/acryo/classification/_dask_pca.py
--rw-rw-rw-   0        0        0     5185 2023-02-21 02:27:31.000000 acryo-0.2.1/acryo/classification/pca.py
-drwxrwxrwx   0        0        0        0 2023-03-15 04:52:43.535884 acryo-0.2.1/acryo/loader/
--rw-rw-rw-   0        0        0      187 2023-02-19 15:38:13.000000 acryo-0.2.1/acryo/loader/__init__.py
--rw-rw-rw-   0        0        0    35134 2023-02-27 14:09:35.000000 acryo-0.2.1/acryo/loader/_base.py
--rw-rw-rw-   0        0        0     7099 2023-02-26 13:13:09.000000 acryo-0.2.1/acryo/loader/_batch.py
--rw-rw-rw-   0        0        0     1696 2023-02-21 08:34:02.000000 acryo-0.2.1/acryo/loader/_cache.py
--rw-rw-rw-   0        0        0    17909 2023-02-27 14:09:35.000000 acryo-0.2.1/acryo/loader/_group.py
--rw-rw-rw-   0        0        0     9034 2023-02-25 12:12:36.000000 acryo-0.2.1/acryo/loader/_loader.py
--rw-rw-rw-   0        0        0     2222 2023-02-24 06:22:10.000000 acryo-0.2.1/acryo/loader/_misc.py
--rw-rw-rw-   0        0        0     9986 2023-03-15 04:51:58.000000 acryo-0.2.1/acryo/loader/_mock.py
--rw-rw-rw-   0        0        0    34029 2023-03-03 14:16:33.000000 acryo-0.2.1/acryo/molecules.py
-drwxrwxrwx   0        0        0        0 2023-03-15 04:52:43.547398 acryo-0.2.1/acryo/pick/
--rw-rw-rw-   0        0        0      129 2023-03-02 06:44:45.000000 acryo-0.2.1/acryo/pick/__init__.py
--rw-rw-rw-   0        0        0     4680 2023-03-02 06:44:45.000000 acryo-0.2.1/acryo/pick/_base.py
--rw-rw-rw-   0        0        0     4799 2023-03-02 06:44:45.000000 acryo-0.2.1/acryo/pick/_concrete.py
-drwxrwxrwx   0        0        0        0 2023-03-15 04:52:43.579945 acryo-0.2.1/acryo/pipe/
--rw-rw-rw-   0        0        0      647 2023-02-23 14:49:44.000000 acryo-0.2.1/acryo/pipe/__init__.py
--rw-rw-rw-   0        0        0    12167 2023-02-23 11:14:01.000000 acryo-0.2.1/acryo/pipe/_classes.py
--rw-rw-rw-   0        0        0     3843 2023-02-25 03:55:45.000000 acryo-0.2.1/acryo/pipe/_curry.py
--rw-rw-rw-   0        0        0     5436 2023-02-23 15:13:40.000000 acryo-0.2.1/acryo/pipe/_imread.py
--rw-rw-rw-   0        0        0     3459 2023-02-23 11:14:00.000000 acryo-0.2.1/acryo/pipe/_masking.py
--rw-rw-rw-   0        0        0     1215 2023-02-25 03:55:55.000000 acryo-0.2.1/acryo/pipe/_transform.py
--rw-rw-rw-   0        0        0    13577 2023-02-18 15:53:02.000000 acryo-0.2.1/acryo/simulator.py
-drwxrwxrwx   0        0        0        0 2023-03-15 04:52:43.593102 acryo-0.2.1/acryo/testing/
--rw-rw-rw-   0        0        0      130 2022-04-15 01:53:16.000000 acryo-0.2.1/acryo/testing/__init__.py
--rw-rw-rw-   0        0        0     1145 2022-05-02 14:08:55.000000 acryo-0.2.1/acryo/testing/_templates.py
--rw-rw-rw-   0        0        0     4432 2023-03-02 06:44:45.000000 acryo-0.2.1/acryo/testing/core.py
-drwxrwxrwx   0        0        0        0 2023-03-15 04:52:43.473597 acryo-0.2.1/acryo.egg-info/
--rw-rw-rw-   0        0        0     2301 2023-03-15 04:52:42.000000 acryo-0.2.1/acryo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      971 2023-03-15 04:52:43.000000 acryo-0.2.1/acryo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-15 04:52:42.000000 acryo-0.2.1/acryo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-03-15 04:52:42.000000 acryo-0.2.1/acryo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-15 04:52:42.000000 acryo-0.2.1/acryo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-15 04:52:43.600284 acryo-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      798 2023-01-30 07:15:08.000000 acryo-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:05:45.122452 acryo-0.2.2/
+-rw-rw-rw-   0        0        0     1547 2022-04-12 12:12:07.000000 acryo-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     2301 2023-04-10 14:05:45.121942 acryo-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2011 2023-03-15 04:48:31.000000 acryo-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 14:05:44.975348 acryo-0.2.2/acryo/
+-rw-rw-rw-   0        0        0      380 2023-04-09 13:27:24.000000 acryo-0.2.2/acryo/__init__.py
+-rw-rw-rw-   0        0        0    10606 2023-03-02 06:44:45.000000 acryo-0.2.2/acryo/_correlation.py
+-rw-rw-rw-   0        0        0      661 2023-02-19 09:29:23.000000 acryo-0.2.2/acryo/_fft.py
+-rw-rw-rw-   0        0        0     2929 2023-02-20 00:46:56.000000 acryo-0.2.2/acryo/_reader.py
+-rw-rw-rw-   0        0        0     2784 2023-03-02 06:44:45.000000 acryo-0.2.2/acryo/_rotation.py
+-rw-rw-rw-   0        0        0      244 2023-02-23 14:34:20.000000 acryo-0.2.2/acryo/_types.py
+-rw-rw-rw-   0        0        0    12048 2023-04-09 13:27:24.000000 acryo-0.2.2/acryo/_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:05:45.023437 acryo-0.2.2/acryo/alignment/
+-rw-rw-rw-   0        0        0      384 2023-03-02 06:44:45.000000 acryo-0.2.2/acryo/alignment/__init__.py
+-rw-rw-rw-   0        0        0    25875 2023-03-02 06:44:45.000000 acryo-0.2.2/acryo/alignment/_base.py
+-rw-rw-rw-   0        0        0     1637 2023-03-02 06:44:45.000000 acryo-0.2.2/acryo/alignment/_concrete.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:05:45.034215 acryo-0.2.2/acryo/classification/
+-rw-rw-rw-   0        0        0       62 2022-04-12 15:56:50.000000 acryo-0.2.2/acryo/classification/__init__.py
+-rw-rw-rw-   0        0        0    18578 2023-02-08 03:31:15.000000 acryo-0.2.2/acryo/classification/_dask_pca.py
+-rw-rw-rw-   0        0        0     5185 2023-02-21 02:27:31.000000 acryo-0.2.2/acryo/classification/pca.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:05:45.059301 acryo-0.2.2/acryo/loader/
+-rw-rw-rw-   0        0        0      187 2023-02-19 15:38:13.000000 acryo-0.2.2/acryo/loader/__init__.py
+-rw-rw-rw-   0        0        0    35134 2023-02-27 14:09:35.000000 acryo-0.2.2/acryo/loader/_base.py
+-rw-rw-rw-   0        0        0     7099 2023-02-26 13:13:09.000000 acryo-0.2.2/acryo/loader/_batch.py
+-rw-rw-rw-   0        0        0     1696 2023-02-21 08:34:02.000000 acryo-0.2.2/acryo/loader/_cache.py
+-rw-rw-rw-   0        0        0    17909 2023-02-27 14:09:35.000000 acryo-0.2.2/acryo/loader/_group.py
+-rw-rw-rw-   0        0        0     9034 2023-02-25 12:12:36.000000 acryo-0.2.2/acryo/loader/_loader.py
+-rw-rw-rw-   0        0        0     2222 2023-02-24 06:22:10.000000 acryo-0.2.2/acryo/loader/_misc.py
+-rw-rw-rw-   0        0        0     9986 2023-03-15 04:51:58.000000 acryo-0.2.2/acryo/loader/_mock.py
+-rw-rw-rw-   0        0        0    34451 2023-04-09 13:27:24.000000 acryo-0.2.2/acryo/molecules.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:05:45.068941 acryo-0.2.2/acryo/pick/
+-rw-rw-rw-   0        0        0      129 2023-03-02 06:44:45.000000 acryo-0.2.2/acryo/pick/__init__.py
+-rw-rw-rw-   0        0        0     4680 2023-03-02 06:44:45.000000 acryo-0.2.2/acryo/pick/_base.py
+-rw-rw-rw-   0        0        0     4799 2023-03-02 06:44:45.000000 acryo-0.2.2/acryo/pick/_concrete.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:05:45.087669 acryo-0.2.2/acryo/pipe/
+-rw-rw-rw-   0        0        0      647 2023-02-23 14:49:44.000000 acryo-0.2.2/acryo/pipe/__init__.py
+-rw-rw-rw-   0        0        0    12167 2023-02-23 11:14:01.000000 acryo-0.2.2/acryo/pipe/_classes.py
+-rw-rw-rw-   0        0        0     3843 2023-02-25 03:55:45.000000 acryo-0.2.2/acryo/pipe/_curry.py
+-rw-rw-rw-   0        0        0     5436 2023-02-23 15:13:40.000000 acryo-0.2.2/acryo/pipe/_imread.py
+-rw-rw-rw-   0        0        0     3459 2023-02-23 11:14:00.000000 acryo-0.2.2/acryo/pipe/_masking.py
+-rw-rw-rw-   0        0        0     1215 2023-02-25 03:55:55.000000 acryo-0.2.2/acryo/pipe/_transform.py
+-rw-rw-rw-   0        0        0    13577 2023-02-18 15:53:02.000000 acryo-0.2.2/acryo/simulator.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:05:45.097191 acryo-0.2.2/acryo/testing/
+-rw-rw-rw-   0        0        0      130 2022-04-15 01:53:16.000000 acryo-0.2.2/acryo/testing/__init__.py
+-rw-rw-rw-   0        0        0     1145 2022-05-02 14:08:55.000000 acryo-0.2.2/acryo/testing/_templates.py
+-rw-rw-rw-   0        0        0     4432 2023-03-02 06:44:45.000000 acryo-0.2.2/acryo/testing/core.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:05:45.014914 acryo-0.2.2/acryo.egg-info/
+-rw-rw-rw-   0        0        0     2301 2023-04-10 14:05:44.000000 acryo-0.2.2/acryo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1142 2023-04-10 14:05:44.000000 acryo-0.2.2/acryo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 14:05:44.000000 acryo-0.2.2/acryo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-04-10 14:05:44.000000 acryo-0.2.2/acryo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-10 14:05:44.000000 acryo-0.2.2/acryo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 14:05:45.123467 acryo-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      821 2023-04-10 14:01:42.000000 acryo-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:05:45.118937 acryo-0.2.2/tests/
+-rw-rw-rw-   0        0        0     3548 2023-04-09 13:27:24.000000 acryo-0.2.2/tests/test_alignment.py
+-rw-rw-rw-   0        0        0     2602 2023-02-21 08:34:02.000000 acryo-0.2.2/tests/test_batch.py
+-rw-rw-rw-   0        0        0     1360 2023-02-21 08:34:02.000000 acryo-0.2.2/tests/test_cache.py
+-rw-rw-rw-   0        0        0     1736 2023-02-23 14:27:37.000000 acryo-0.2.2/tests/test_group.py
+-rw-rw-rw-   0        0        0     6716 2023-02-24 04:50:51.000000 acryo-0.2.2/tests/test_molecules.py
+-rw-rw-rw-   0        0        0      691 2023-02-21 11:08:36.000000 acryo-0.2.2/tests/test_pipe.py
+-rw-rw-rw-   0        0        0     1545 2023-01-29 13:16:40.000000 acryo-0.2.2/tests/test_simulator.py
+-rw-rw-rw-   0        0        0      542 2023-02-14 03:49:57.000000 acryo-0.2.2/tests/test_utils.py
```

### Comparing `acryo-0.2.1/LICENSE` & `acryo-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/PKG-INFO` & `acryo-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acryo
-Version: 0.2.1
+Version: 0.2.2
 Summary: An extensible cryo-EM/ET toolkit for Python.
 Author: Hanjin Liu
 Author-email: liuhanjin-sc@g.ecc.u-tokyo.ac.jp
 License: BSD 3-Clause
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `acryo-0.2.1/README.md` & `acryo-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/_correlation.py` & `acryo-0.2.2/acryo/_correlation.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/_fft.py` & `acryo-0.2.2/acryo/_fft.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/_reader.py` & `acryo-0.2.2/acryo/_reader.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/_rotation.py` & `acryo-0.2.2/acryo/_rotation.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/_utils.py` & `acryo-0.2.2/acryo/_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # pyright: reportPrivateImportUsage=false
 from __future__ import annotations
 
-from typing import Sequence, TYPE_CHECKING
-from functools import lru_cache, reduce
+import warnings
+from typing import Callable, Sequence, TYPE_CHECKING, TypeVar
+from functools import lru_cache, reduce, wraps
 
 import numpy as np
 from numpy.typing import NDArray
 from dask import array as da
 from dask.delayed import delayed
 from scipy import ndimage as ndi
 from scipy.spatial.transform import Rotation
@@ -383,7 +384,27 @@
         ranges.append(np.fft.ifftshift(axis**2))
     if real:
         limit = shape[-1] // 2 + 1
         ranges[-1] = ranges[-1][:limit]
     q2 = reduce(np.add, np.meshgrid(*ranges, indexing="ij", sparse=True))
     wfilt = 1 / (1 + q2**order)
     return wfilt
+
+
+_F = TypeVar("_F", bound=Callable)
+
+
+def deprecated_kwarg(old: str, new: str) -> Callable[[_F], _F]:
+    def _inner(f):
+        @wraps(f)
+        def _func(*args, **kwargs):
+            if old in kwargs:
+                warnings.warn(
+                    f"`{old}` is deprecated, use `{new}` instead",
+                    DeprecationWarning,
+                )
+                kwargs[new] = kwargs.pop(old)
+            return f(*args, **kwargs)
+
+        return _func
+
+    return _inner
```

### Comparing `acryo-0.2.1/acryo/alignment/_base.py` & `acryo-0.2.2/acryo/alignment/_base.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/alignment/_concrete.py` & `acryo-0.2.2/acryo/alignment/_concrete.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/classification/_dask_pca.py` & `acryo-0.2.2/acryo/classification/_dask_pca.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/classification/pca.py` & `acryo-0.2.2/acryo/classification/pca.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/loader/_base.py` & `acryo-0.2.2/acryo/loader/_base.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/loader/_batch.py` & `acryo-0.2.2/acryo/loader/_batch.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/loader/_cache.py` & `acryo-0.2.2/acryo/loader/_cache.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/loader/_group.py` & `acryo-0.2.2/acryo/loader/_group.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/loader/_loader.py` & `acryo-0.2.2/acryo/loader/_loader.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/loader/_misc.py` & `acryo-0.2.2/acryo/loader/_misc.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/loader/_mock.py` & `acryo-0.2.2/acryo/loader/_mock.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/molecules.py` & `acryo-0.2.2/acryo/molecules.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,20 @@
     overload,
 )
 import numpy as np
 from numpy.typing import ArrayLike, NDArray
 import polars as pl
 from scipy.spatial.transform import Rotation
 from acryo._types import nm
+from acryo._utils import deprecated_kwarg
 
 if TYPE_CHECKING:
     from typing_extensions import Self, TypeGuard
-    from polars.internals.dataframe.groupby import GroupBy
+    from polars.type_aliases import IntoExpr
+    from polars.dataframe.groupby import GroupBy
 
 _CSV_COLUMNS = ["z", "y", "x", "zvec", "yvec", "xvec"]
 PathLike = Union[str, Path, bytes]
 
 
 class Molecules:
     """
@@ -876,18 +878,18 @@
     def groupby(self, by: str | pl.Expr) -> MoleculeGroup[str]:
         ...
 
     @overload
     def groupby(self, by: Sequence[str | pl.Expr]) -> MoleculeGroup[tuple[str, ...]]:
         ...
 
-    def groupby(self, by):
+    def groupby(self, by: IntoExpr | Iterable[IntoExpr], *more_by: IntoExpr):
         """Group molecules into sub-groups."""
         df = self.to_dataframe()
-        return MoleculeGroup(df.groupby(by, maintain_order=True))
+        return MoleculeGroup(df.groupby(by, *more_by, maintain_order=True))
 
     def filter(
         self,
         predicate: pl.Expr | str | pl.Series | list[bool] | np.ndarray,
     ) -> Self:
         """Filter molecules by its features."""
         df = self.to_dataframe()
@@ -905,47 +907,55 @@
         return self.__class__.from_dataframe(df.tail(n))
 
     def sample(self, n: int = 10, seed: int | None = None) -> Self:
         """Return n randomly sampled molecules."""
         df = self.to_dataframe()
         return self.__class__.from_dataframe(df.sample(n, seed=seed))
 
+    @deprecated_kwarg(old="reverse", new="descending")
     def sort(
         self,
-        by: str | pl.Expr | Sequence[str] | Sequence[pl.Expr],
-        *,
-        reverse: bool = False,
+        by: IntoExpr | Iterable[IntoExpr],
+        *more_by: IntoExpr,
+        descending: bool = False,
     ) -> Self:
         """
         Return a new instance with sorted molecules and features.
 
         Parameters
         ----------
         by : str or Expr or sequence of them
             Column name or expression to sort by.
-        reverse : bool, default is False
+        descending : bool, default is False
             If true, sort in descending order.
         """
         df = self.to_dataframe()
-        return self.__class__.from_dataframe(df.sort(by=by, reverse=reverse))
+        return self.__class__.from_dataframe(
+            df.sort(by, *more_by, descending=descending)
+        )
 
-    def with_features(self, exprs) -> Self:
+    def with_features(
+        self,
+        exprs: IntoExpr | Iterable[IntoExpr],
+        *more_exprs: IntoExpr,
+        **named_exprs: IntoExpr,
+    ) -> Self:
         """Return a new instance with updated features."""
         return self.__class__(
             self.pos,
             self.rotator,
-            features=self.features.with_columns(exprs),
+            features=self.features.with_columns(exprs, *more_exprs, **named_exprs),
         )
 
-    def drop_features(self, columns: str | Sequence[str]) -> Self:
+    def drop_features(self, columns: str | Sequence[str], *more_columns: str) -> Self:
         """Return a new instance with updated features."""
         return self.__class__(
             self.pos,
             self.rotator,
-            features=self.features.drop(columns),
+            features=self.features.drop(columns, *more_columns),
         )
 
 
 _K = TypeVar("_K", bound=Hashable)
 
 
 class MoleculeGroup(Generic[_K]):
```

### Comparing `acryo-0.2.1/acryo/pick/_base.py` & `acryo-0.2.2/acryo/pick/_base.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/pick/_concrete.py` & `acryo-0.2.2/acryo/pick/_concrete.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/pipe/__init__.py` & `acryo-0.2.2/acryo/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/pipe/_classes.py` & `acryo-0.2.2/acryo/pipe/_classes.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/pipe/_curry.py` & `acryo-0.2.2/acryo/pipe/_curry.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/pipe/_imread.py` & `acryo-0.2.2/acryo/pipe/_imread.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/pipe/_masking.py` & `acryo-0.2.2/acryo/pipe/_masking.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/pipe/_transform.py` & `acryo-0.2.2/acryo/pipe/_transform.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/simulator.py` & `acryo-0.2.2/acryo/simulator.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/testing/_templates.py` & `acryo-0.2.2/acryo/testing/_templates.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo/testing/core.py` & `acryo-0.2.2/acryo/testing/core.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.1/acryo.egg-info/PKG-INFO` & `acryo-0.2.2/acryo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acryo
-Version: 0.2.1
+Version: 0.2.2
 Summary: An extensible cryo-EM/ET toolkit for Python.
 Author: Hanjin Liu
 Author-email: liuhanjin-sc@g.ecc.u-tokyo.ac.jp
 License: BSD 3-Clause
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `acryo-0.2.1/acryo.egg-info/SOURCES.txt` & `acryo-0.2.2/acryo.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -36,8 +36,16 @@
 acryo/pipe/_classes.py
 acryo/pipe/_curry.py
 acryo/pipe/_imread.py
 acryo/pipe/_masking.py
 acryo/pipe/_transform.py
 acryo/testing/__init__.py
 acryo/testing/_templates.py
-acryo/testing/core.py
+acryo/testing/core.py
+tests/test_alignment.py
+tests/test_batch.py
+tests/test_cache.py
+tests/test_group.py
+tests/test_molecules.py
+tests/test_pipe.py
+tests/test_simulator.py
+tests/test_utils.py
```

### Comparing `acryo-0.2.1/setup.py` & `acryo-0.2.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from setuptools import setup, find_packages
 
-with open("acryo/__init__.py", encoding="utf-8") as f:
+ACRYO = "acryo"
+
+with open(f"{ACRYO}/__init__.py", encoding="utf-8") as f:
     line = next(f)
     VERSION = line.strip().split()[-1][1:-1]
 
 with open("README.md", "r") as f:
-    readme = f.read()
+    README = f.read()
 
 setup(
-    name="acryo",
+    name=ACRYO,
     version=VERSION,
     description="An extensible cryo-EM/ET toolkit for Python.",
-    long_description=readme,
+    long_description=README,
     long_description_content_type="text/markdown",
     author="Hanjin Liu",
     author_email="liuhanjin-sc@g.ecc.u-tokyo.ac.jp",
     license="BSD 3-Clause",
     packages=find_packages(exclude=["tests", "tests.*"]),
     install_requires=[
         "numpy>=1.21",
         "scipy>=1.7.3",
-        "polars>=0.16",
+        "polars>=0.16.18",
         "dask>=2021.6.0",
         "typing_extensions>=4.1.1",
     ],
     python_requires=">=3.8",
 )
```

