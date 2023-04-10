# Comparing `tmp/dask_awkward-2023.3.2.tar.gz` & `tmp/dask_awkward-2023.4.0.tar.gz`

## Comparing `dask_awkward-2023.3.2.tar` & `dask_awkward-2023.4.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/src/dask_awkward/__init__.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/src/dask_awkward/awkward.yaml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/src/dask_awkward/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/src/dask_awkward/py.typed
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/src/dask_awkward/sizeof.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/src/dask_awkward/typing.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/src/dask_awkward/utils.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/src/dask_awkward/version.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/src/dask_awkward/version.pyi
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/src/dask_awkward/layers/__init__.py
--rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/src/dask_awkward/layers/layers.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/src/dask_awkward/lib/__init__.py
--rw-r--r--   0        0        0    60728 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/src/dask_awkward/lib/core.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/src/dask_awkward/lib/describe.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/src/dask_awkward/lib/inspect.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/src/dask_awkward/lib/operations.py
--rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/src/dask_awkward/lib/optimize.py
--rw-r--r--   0        0        0    11155 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/src/dask_awkward/lib/reducers.py
--rw-r--r--   0        0        0    29325 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/src/dask_awkward/lib/structure.py
--rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/src/dask_awkward/lib/testutils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/src/dask_awkward/lib/io/__init__.py
--rw-r--r--   0        0        0    15332 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/src/dask_awkward/lib/io/io.py
--rw-r--r--   0        0        0    15146 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/src/dask_awkward/lib/io/json.py
--rw-r--r--   0        0        0    14183 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/src/dask_awkward/lib/io/parquet.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/LICENSE
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/README.md
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/pyproject.toml
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 dask_awkward-2023.3.2/PKG-INFO
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/__init__.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/awkward.yaml
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/py.typed
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/sizeof.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/typing.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/utils.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/version.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/version.pyi
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/layers/__init__.py
+-rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/layers/layers.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/__init__.py
+-rw-r--r--   0        0        0    61123 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/core.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/describe.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/inspect.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/operations.py
+-rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/optimize.py
+-rw-r--r--   0        0        0    11155 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/reducers.py
+-rw-r--r--   0        0        0    28744 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/structure.py
+-rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/testutils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/io/__init__.py
+-rw-r--r--   0        0        0    15332 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/io/io.py
+-rw-r--r--   0        0        0    15172 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/io/json.py
+-rw-r--r--   0        0        0    14183 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/src/dask_awkward/lib/io/parquet.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/LICENSE
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/README.md
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 dask_awkward-2023.4.0/PKG-INFO
```

### Comparing `dask_awkward-2023.3.2/src/dask_awkward/awkward.yaml` & `dask_awkward-2023.4.0/src/dask_awkward/awkward.yaml`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.3.2/src/dask_awkward/typing.py` & `dask_awkward-2023.4.0/src/dask_awkward/typing.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.3.2/src/dask_awkward/utils.py` & `dask_awkward-2023.4.0/src/dask_awkward/utils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.3.2/src/dask_awkward/layers/layers.py` & `dask_awkward-2023.4.0/src/dask_awkward/layers/layers.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.3.2/src/dask_awkward/lib/__init__.py` & `dask_awkward-2023.4.0/src/dask_awkward/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.3.2/src/dask_awkward/lib/core.py` & `dask_awkward-2023.4.0/src/dask_awkward/lib/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -513,15 +513,15 @@
 
     __dask_optimize__ = globalmethod(
         all_optimizations, key="awkward_array_optimize", falsey=dont_optimize
     )
 
     __dask_scheduler__ = staticmethod(threaded_get)
 
-    def __setitem__(self, where: str, what: Any) -> None:
+    def __setitem__(self, where: Any, what: Any) -> None:
         if not (
             isinstance(where, str)
             or (isinstance(where, tuple) and all(isinstance(x, str) for x in where))
         ):
             raise TypeError("only fields may be assigned in-place (by field name)")
 
         if not isinstance(what, Array):
@@ -888,14 +888,24 @@
             try:
                 dtype = where[0].layout.dtype.type
             except AttributeError:
                 dtype = where[0].layout.content.dtype.type
             if issubclass(dtype, (np.bool_, bool, np.int64, np.int32, int)):
                 return self._getitem_outer_bool_or_int_lazy_array(where)
 
+        elif where[0] is Ellipsis:
+            if len(where) <= self.ndim:
+                return self._getitem_trivial_map_partitions(where)
+
+            raise DaskAwkwardNotImplemented(
+                "Array slicing doesn't currently support Ellipsis where "
+                "the total number of sliced axes is greater than the "
+                "dimensionality of the array."
+            )
+
         raise DaskAwkwardNotImplemented(
             f"Array.__getitem__ doesn't support multi object: {where}"
         )
 
     def _getitem_single(self, where: Any) -> Array:
         # a single string
         if isinstance(where, str):
```

### Comparing `dask_awkward-2023.3.2/src/dask_awkward/lib/describe.py` & `dask_awkward-2023.4.0/src/dask_awkward/lib/describe.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.3.2/src/dask_awkward/lib/inspect.py` & `dask_awkward-2023.4.0/src/dask_awkward/lib/inspect.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.3.2/src/dask_awkward/lib/operations.py` & `dask_awkward-2023.4.0/src/dask_awkward/lib/operations.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.3.2/src/dask_awkward/lib/optimize.py` & `dask_awkward-2023.4.0/src/dask_awkward/lib/optimize.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.3.2/src/dask_awkward/lib/reducers.py` & `dask_awkward-2023.4.0/src/dask_awkward/lib/reducers.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.3.2/src/dask_awkward/lib/structure.py` & `dask_awkward-2023.4.0/src/dask_awkward/lib/structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,28 +230,14 @@
 
 
 class _CartesianFn:
     def __init__(self, **kwargs):
         self.kwargs = kwargs
 
     def __call__(self, *arrays):
-        # TODO: remove backend check when typetracer support exists for this
-        if ak.backend(*arrays) == "typetracer":
-            for array in arrays:
-                array.layout._touch_data(recursive=True)
-            out = ak.cartesian(
-                list(
-                    array.layout.form.length_zero_array(behavior=array.behavior)
-                    for array in arrays
-                ),
-                **self.kwargs,
-            )
-            return ak.Array(
-                out.layout.to_typetracer(forget_length=True), behavior=out.behavior
-            )
         return ak.cartesian(list(arrays), **self.kwargs)
 
 
 @borrow_docstring(ak.cartesian)
 def cartesian(
     arrays,
     axis=1,
```

### Comparing `dask_awkward-2023.3.2/src/dask_awkward/lib/testutils.py` & `dask_awkward-2023.4.0/src/dask_awkward/lib/testutils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.3.2/src/dask_awkward/lib/io/io.py` & `dask_awkward-2023.4.0/src/dask_awkward/lib/io/io.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.3.2/src/dask_awkward/lib/io/json.py` & `dask_awkward-2023.4.0/src/dask_awkward/lib/io/json.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import warnings
 from typing import TYPE_CHECKING, Any
 
 try:
     import ujson as json
 except ImportError:
-    import json
+    import json  # type: ignore[no-redef]
 
 import awkward as ak
 from dask.base import tokenize
 from dask.blockwise import BlockIndex
 from dask.bytes.core import read_bytes
 from dask.core import flatten
 from dask.highlevelgraph import HighLevelGraph
```

### Comparing `dask_awkward-2023.3.2/src/dask_awkward/lib/io/parquet.py` & `dask_awkward-2023.4.0/src/dask_awkward/lib/io/parquet.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.3.2/.gitignore` & `dask_awkward-2023.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.3.2/LICENSE` & `dask_awkward-2023.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.3.2/README.md` & `dask_awkward-2023.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.3.2/pyproject.toml` & `dask_awkward-2023.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -5,68 +5,68 @@
 [project]
 name = "dask-awkward"
 description = "Awkward Array meets Dask"
 readme = "README.md"
 license = {text = "BSD-3-Clause"}
 requires-python = ">=3.8"
 authors = [
-    { name = "Doug Davis", email = "ddavis@ddavis.io" },
-    { name = "Martin Durant", email = "mdurant@anaconda.com" },
+  { name = "Doug Davis", email = "ddavis@ddavis.io" },
+  { name = "Martin Durant", email = "mdurant@anaconda.com" },
 ]
 maintainers = [
-    { name = "Doug Davis", email = "ddavis@ddavis.io" },
-    { name = "Martin Durant", email = "mdurant@anaconda.com" },
+  { name = "Doug Davis", email = "ddavis@ddavis.io" },
+  { name = "Martin Durant", email = "mdurant@anaconda.com" },
 ]
 classifiers = [
-    "Development Status :: 3 - Alpha",
-    "License :: OSI Approved :: BSD License",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Topic :: Scientific/Engineering",
+  "Development Status :: 3 - Alpha",
+  "License :: OSI Approved :: BSD License",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Topic :: Scientific/Engineering",
 ]
 dependencies = [
-    "awkward >=2.0.8",
-    "dask >=2022.02.1",
+  "awkward >=2.1.2",
+  "dask >=2022.02.1",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/dask-contrib/dask-awkward"
 "Bug Tracker" = "https://github.com/dask-contrib/dask-awkward/issues"
 
 [project.optional-dependencies]
 complete = [
-    "aiohttp",
-    "pyarrow",
-    "pytest >=6.0",
-    "pytest-cov >=3.0.0",
-    "requests >=2.27.1",
+  "aiohttp",
+  "pyarrow",
+  "pytest >=6.0",
+  "pytest-cov >=3.0.0",
+  "requests >=2.27.1",
 ]
 docs = [
-    "dask-sphinx-theme >=3.0.2",
-    "pyarrow",
-    "sphinx-design",
-    "pytest >=6.0",
-    "pytest-cov >=3.0.0",
-    "requests >=2.27.1",
+  "dask-sphinx-theme >=3.0.2",
+  "pyarrow",
+  "sphinx-design",
+  "pytest >=6.0",
+  "pytest-cov >=3.0.0",
+  "requests >=2.27.1",
 ]
 io = [
-    "aiohttp",
-    "pyarrow",
+  "aiohttp",
+  "pyarrow",
 ]
 test = [
-    "aiohttp",
-    "distributed",
-    "pyarrow",
-    "pytest >=6.0",
-    "pytest-cov >=3.0.0",
-    "requests >=2.27.1",
+  "aiohttp",
+  "distributed",
+  "pyarrow",
+  "pytest >=6.0",
+  "pytest-cov >=3.0.0",
+  "requests >=2.27.1",
 ]
 
 [project.entry-points."dask.sizeof"]
 awkward = "dask_awkward.sizeof:register"
 
 [tool.hatch.version]
 source = "vcs"
@@ -81,79 +81,85 @@
 [tool.setuptools_scm]
 write_to = "src/dask_awkward/_version.py"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = ["tests"]
 addopts = [
-    "-v",
-    "-ra",
-    "--showlocals",
-    "--strict-markers",
-    "--strict-config",
+  "-v",
+  "-ra",
+  "--showlocals",
+  "--strict-markers",
+  "--strict-config",
 ]
 log_cli_level = "DEBUG"
 filterwarnings = [
-    "ignore:There is no current event loop",
+  "ignore:There is no current event loop",
 ]
 
 [tool.isort]
 profile = "black"
 line_length = 88
 src_paths = ["src", "tests"]
 
 [tool.mypy]
 python_version = "3.9"
 files = ["src", "tests"]
 warn_unused_configs = true
 show_error_codes = true
 allow_incomplete_defs = false
 allow_untyped_decorators = false
-ignore_missing_imports = true
 no_implicit_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_unreachable = true
 
+[[tool.mypy.overrides]]
+  module = ["awkward.*"]
+  ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+  module = ["IPython.*"]
+  ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
-module = ["IPython.*"]
-ignore_missing_imports = true
+  module = ["fsspec.*"]
+  ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
-module = ["fsspec.*"]
-ignore_missing_imports = true
+  module = ["pyarrow.*"]
+  ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
-module = ["ujson.*"]
-ignore_missing_imports = true
+  module = ["tlz.*"]
+  ignore_missing_imports = true
 
 [tool.pyright]
 include = ["src"]
-pythonVersion = "3.8"
+pythonVersion = "3.9"
 reportPrivateImportUsage = false
 
 [tool.coverage.report]
 exclude_lines = [
-    "pragma: no cover",
-    "if TYPE_CHECKING:",
-    "except ImportError:",
-    "NotImplementedError",
-    "DaskAwkwardNotImplemented",
-    "_ipython_key_completions_",
-    "Only highlevel=True is supported",
-    "\\.\\.\\.$",
+  "pragma: no cover",
+  "if TYPE_CHECKING:",
+  "except ImportError:",
+  "NotImplementedError",
+  "DaskAwkwardNotImplemented",
+  "_ipython_key_completions_",
+  "Only highlevel=True is supported",
+  "\\.\\.\\.$",
 ]
 fail_under = 90
 show_missing = true
 
 [tool.coverage.run]
 omit = [
-     "*/tests/test_*.py",
-     "*/tests/__init__.py",
-     "*/version.py",
+  "*/tests/test_*.py",
+  "*/tests/__init__.py",
+  "*/version.py",
 ]
 source = ["src/"]
 
 [tool.ruff]
 ignore = ["E501", "E402"]
 per-file-ignores = {"__init__.py" = ["E402", "F401"]}
```

### Comparing `dask_awkward-2023.3.2/PKG-INFO` & `dask_awkward-2023.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-awkward
-Version: 2023.3.2
+Version: 2023.4.0
 Summary: Awkward Array meets Dask
 Project-URL: Homepage, https://github.com/dask-contrib/dask-awkward
 Project-URL: Bug Tracker, https://github.com/dask-contrib/dask-awkward/issues
 Author-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 Maintainer-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 License: BSD-3-Clause
 License-File: LICENSE
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
-Requires-Dist: awkward>=2.0.8
+Requires-Dist: awkward>=2.1.2
 Requires-Dist: dask>=2022.02.1
 Provides-Extra: complete
 Requires-Dist: aiohttp; extra == 'complete'
 Requires-Dist: pyarrow; extra == 'complete'
 Requires-Dist: pytest-cov>=3.0.0; extra == 'complete'
 Requires-Dist: pytest>=6.0; extra == 'complete'
 Requires-Dist: requests>=2.27.1; extra == 'complete'
```

