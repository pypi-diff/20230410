# Comparing `tmp/object_store_python-0.1.8.tar.gz` & `tmp/object_store_python-0.1.9.tar.gz`

## Comparing `object_store_python-0.1.8.tar` & `object_store_python-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 object_store_python-0.1.8/Cargo.toml
--rw-r--r--   0     1001      123      302 2023-03-23 06:47:54.000000 object_store_python-0.1.8/.gitignore
--rw-r--r--   0     1001      123     7110 2023-03-23 06:47:54.000000 object_store_python-0.1.8/README.md
--rw-r--r--   0     1001      123     6190 2023-03-23 06:47:54.000000 object_store_python-0.1.8/object_store/__init__.py
--rw-r--r--   0     1001      123     6820 2023-03-23 06:47:54.000000 object_store_python-0.1.8/object_store/_internal.pyi
--rw-r--r--   0     1001      123     1228 2023-03-23 06:47:54.000000 object_store_python-0.1.8/object_store/arrow.py
--rw-r--r--   0     1001      123        0 2023-03-23 06:47:54.000000 object_store_python-0.1.8/object_store/py.typed
--rw-r--r--   0     1001      123     1321 2023-03-23 06:47:54.000000 object_store_python-0.1.8/pyproject.toml
--rw-r--r--   0     1001      123     8571 2023-03-23 06:47:54.000000 object_store_python-0.1.8/src/builder.rs
--rw-r--r--   0     1001      123    17371 2023-03-23 06:47:54.000000 object_store_python-0.1.8/src/file.rs
--rw-r--r--   0     1001      123    12289 2023-03-23 06:47:54.000000 object_store_python-0.1.8/src/lib.rs
--rw-r--r--   0     1001      123     2768 2023-03-23 06:47:54.000000 object_store_python-0.1.8/src/utils.rs
--rw-r--r--   0     1001      123     5655 2023-03-23 06:47:54.000000 object_store_python-0.1.8/tests/test_arrow.py
--rw-r--r--   0     1001      123     2727 2023-03-23 06:47:54.000000 object_store_python-0.1.8/tests/test_object_store.py
--rw-r--r--   0     1001      123    56523 2023-03-23 06:47:54.000000 object_store_python-0.1.8/Cargo.lock
--rw-r--r--   0        0        0     8205 1970-01-01 00:00:00.000000 object_store_python-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 object_store_python-0.1.9/Cargo.toml
+-rw-r--r--   0     1001      123      302 2023-03-23 08:50:53.000000 object_store_python-0.1.9/.gitignore
+-rw-r--r--   0     1001      123     7110 2023-03-23 08:50:53.000000 object_store_python-0.1.9/README.md
+-rw-r--r--   0     1001      123     6190 2023-03-23 08:50:53.000000 object_store_python-0.1.9/object_store/__init__.py
+-rw-r--r--   0     1001      123     6820 2023-03-23 08:50:53.000000 object_store_python-0.1.9/object_store/_internal.pyi
+-rw-r--r--   0     1001      123     1228 2023-03-23 08:50:53.000000 object_store_python-0.1.9/object_store/arrow.py
+-rw-r--r--   0     1001      123        0 2023-03-23 08:50:53.000000 object_store_python-0.1.9/object_store/py.typed
+-rw-r--r--   0     1001      123     1321 2023-03-23 08:50:53.000000 object_store_python-0.1.9/pyproject.toml
+-rw-r--r--   0     1001      123     8571 2023-03-23 08:50:53.000000 object_store_python-0.1.9/src/builder.rs
+-rw-r--r--   0     1001      123    17371 2023-03-23 08:50:53.000000 object_store_python-0.1.9/src/file.rs
+-rw-r--r--   0     1001      123    12289 2023-03-23 08:50:53.000000 object_store_python-0.1.9/src/lib.rs
+-rw-r--r--   0     1001      123     2768 2023-03-23 08:50:53.000000 object_store_python-0.1.9/src/utils.rs
+-rw-r--r--   0     1001      123     5655 2023-03-23 08:50:53.000000 object_store_python-0.1.9/tests/test_arrow.py
+-rw-r--r--   0     1001      123     2727 2023-03-23 08:50:53.000000 object_store_python-0.1.9/tests/test_object_store.py
+-rw-r--r--   0     1001      123    56523 2023-03-23 08:50:53.000000 object_store_python-0.1.9/Cargo.lock
+-rw-r--r--   0        0        0     8205 1970-01-01 00:00:00.000000 object_store_python-0.1.9/PKG-INFO
```

### Comparing `object_store_python-0.1.8/Cargo.toml` & `object_store_python-0.1.9/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "object-store-python"
-version = "0.1.8"
+version = "0.1.9"
 edition = "2021"
 authors = ["Robert Pack <robstar.pack@gmail.com>"]
 description = "A generic object store interface for uniformly interacting with AWS S3, Google Cloud Storage, Azure Storage and local files."
 
 [dependencies]
 async-trait = "0.1.57"
 bytes = "1.2.1"
```

### Comparing `object_store_python-0.1.8/README.md` & `object_store_python-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `object_store_python-0.1.8/object_store/__init__.py` & `object_store_python-0.1.9/object_store/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         """Delete the object at the specified location.
 
         Args:
             location (PathLike): path / key to storage location
         """
         return super().delete(_as_path(location))
 
-    def list(self, prefix: Optional[PathLike] = None) -> list[ObjectMeta]:
+    def list(self, prefix: Optional[PathLike] = None) -> List[ObjectMeta]:
         """List all the objects with the given prefix.
 
         Prefixes are evaluated on a path segment basis, i.e. `foo/bar/` is a prefix
         of `foo/bar/x` but not of `foo/bar_baz/x`.
 
         Args:
             prefix (PathLike | None, optional): path prefix to filter limit list results. Defaults to None.
```

### Comparing `object_store_python-0.1.8/object_store/_internal.pyi` & `object_store_python-0.1.9/object_store/_internal.pyi`

 * *Files identical despite different names*

### Comparing `object_store_python-0.1.8/object_store/arrow.py` & `object_store_python-0.1.9/object_store/arrow.py`

 * *Files identical despite different names*

### Comparing `object_store_python-0.1.8/pyproject.toml` & `object_store_python-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15", "typing_extensions"]
 build-backend = "maturin"
 
 [project]
 name = "object-store-python"
-version = "0.1.8"
+version = "0.1.9"
 description = "A generic object store interface for uniformly interacting with AWS S3, Google Cloud Storage, Azure Storage and local files."
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = ["object-store", "azure", "aws", "gcp"]
 authors = [{ name = "Robert Pack", email = "robstar.pack@gmail.com" }]
 classifiers = [
   "Development Status :: 3 - Alpha",
```

### Comparing `object_store_python-0.1.8/src/builder.rs` & `object_store_python-0.1.9/src/builder.rs`

 * *Files identical despite different names*

### Comparing `object_store_python-0.1.8/src/file.rs` & `object_store_python-0.1.9/src/file.rs`

 * *Files identical despite different names*

### Comparing `object_store_python-0.1.8/src/lib.rs` & `object_store_python-0.1.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `object_store_python-0.1.8/src/utils.rs` & `object_store_python-0.1.9/src/utils.rs`

 * *Files identical despite different names*

### Comparing `object_store_python-0.1.8/tests/test_arrow.py` & `object_store_python-0.1.9/tests/test_arrow.py`

 * *Files identical despite different names*

### Comparing `object_store_python-0.1.8/tests/test_object_store.py` & `object_store_python-0.1.9/tests/test_object_store.py`

 * *Files identical despite different names*

### Comparing `object_store_python-0.1.8/Cargo.lock` & `object_store_python-0.1.9/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1024,15 +1024,15 @@
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "object-store-python"
-version = "0.1.8"
+version = "0.1.9"
 dependencies = [
  "async-trait",
  "bytes",
  "futures",
  "object_store",
  "once_cell",
  "percent-encoding",
```

### Comparing `object_store_python-0.1.8/PKG-INFO` & `object_store_python-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: object-store-python
-Version: 0.1.8
+Version: 0.1.9
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Rust
@@ -14,16 +14,16 @@
 Provides-Extra: pyarrow
 Summary: A generic object store interface for uniformly interacting with AWS S3, Google Cloud Storage, Azure Storage and local files.
 Keywords: object-store,azure,aws,gcp
 Author: Robert Pack <robstar.pack@gmail.com>
 Author-email: Robert Pack <robstar.pack@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Documentation, https://github.com/roeap/object-store-python#readme
 Project-URL: Repository, https://github.com/roeap/object-store-python
+Project-URL: Documentation, https://github.com/roeap/object-store-python#readme
 
 # object-store-python
 
 [![CI][ci-img]][ci-link]
 [![code style: black][black-img]][black-link]
 ![PyPI](https://img.shields.io/pypi/v/object-store-python)
 [![PyPI - Downloads][pypi-img]][pypi-link]
```

