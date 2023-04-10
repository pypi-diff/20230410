# Comparing `tmp/arrow_odbc-1.0.0.tar.gz` & `tmp/arrow_odbc-1.0.1.tar.gz`

## Comparing `arrow_odbc-1.0.0.tar` & `arrow_odbc-1.0.1.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 arrow_odbc-1.0.0/Cargo.toml
--rw-r--r--   0      501       20      136 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/.gitattributes
--rw-r--r--   0      501       20      131 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/.github/dependabot.yml
--rw-r--r--   0      501       20     1522 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/.github/workflows/test.yml
--rw-r--r--   0      501       20     1807 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/.github/workflows/wheel.yml
--rw-r--r--   0      501       20      286 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/.gitignore
--rw-r--r--   0      501       20      841 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/.readthedocs.yaml
--rw-r--r--   0      501       20     4815 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/Changelog.md
--rw-r--r--   0      501       20     1834 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/Contributing.md
--rw-r--r--   0      501       20     1069 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/LICENSE
--rw-r--r--   0      501       20     7305 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/README.md
--rw-r--r--   0      501       20       14 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/cbindgen.toml
--rw-r--r--   0      501       20      639 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/conftest.py
--rw-r--r--   0      501       20      638 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/doc/Makefile
--rw-r--r--   0      501       20      804 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/doc/make.bat
--rw-r--r--   0      501       20       16 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/doc/requirements.txt
--rw-r--r--   0      501       20      155 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/doc/source/arrow_odbc.rst
--rw-r--r--   0      501       20     1965 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/doc/source/conf.py
--rw-r--r--   0      501       20      458 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/doc/source/index.rst
--rw-r--r--   0      501       20       67 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/doc/source/modules.rst
--rw-r--r--   0      501       20      348 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/docker-compose.yml
--rw-r--r--   0      501       20      564 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/manylinux/Dockerfile
--rw-r--r--   0      501       20      121 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/manylinux/Readme.md
--rw-r--r--   0      501       20      148 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/manylinux/WHEEL
--rw-r--r--   0      501       20     1256 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/manylinux/build_wheel.sh
--rw-r--r--   0      501       20      617 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/pyproject.toml
--rw-r--r--   0      501       20      307 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/python/arrow_odbc/__init__.py
--rw-r--r--   0      501       20     1645 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/python/arrow_odbc/connect.py
--rw-r--r--   0      501       20      672 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/python/arrow_odbc/error.py
--rw-r--r--   0      501       20    13961 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/python/arrow_odbc/reader.py
--rw-r--r--   0      501       20     7915 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/python/arrow_odbc/writer.py
--rw-r--r--   0      501       20     2131 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/src/error.rs
--rw-r--r--   0      501       20     2842 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/src/lib.rs
--rw-r--r--   0      501       20     1239 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/src/parameter.rs
--rw-r--r--   0      501       20     8314 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/src/reader.rs
--rw-r--r--   0      501       20     3613 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/src/writer.rs
--rw-r--r--   0      501       20        0 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/tests/__init__.py
--rw-r--r--   0      501       20     4115 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/tests/iris.csv
--rw-r--r--   0      501       20     2413 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/tests/iris.parquet
--rw-r--r--   0      501       20    19182 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/tests/test_arrow_odbc.py
--rw-r--r--   0      501       20    35304 2023-04-09 12:12:48.000000 arrow_odbc-1.0.0/Cargo.lock
--rw-r--r--   0        0        0     7829 1970-01-01 00:00:00.000000 arrow_odbc-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 arrow_odbc-1.0.1/Cargo.toml
+-rw-r--r--   0      501       20      136 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/.gitattributes
+-rw-r--r--   0      501       20      131 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/.github/dependabot.yml
+-rw-r--r--   0      501       20     1522 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/.github/workflows/test.yml
+-rw-r--r--   0      501       20     1807 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/.github/workflows/wheel.yml
+-rw-r--r--   0      501       20      286 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/.gitignore
+-rw-r--r--   0      501       20      841 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/.readthedocs.yaml
+-rw-r--r--   0      501       20     4861 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/Changelog.md
+-rw-r--r--   0      501       20     1954 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/Contributing.md
+-rw-r--r--   0      501       20     1069 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/LICENSE
+-rw-r--r--   0      501       20     7727 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/README.md
+-rw-r--r--   0      501       20       14 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/cbindgen.toml
+-rw-r--r--   0      501       20      639 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/conftest.py
+-rw-r--r--   0      501       20      638 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/doc/Makefile
+-rw-r--r--   0      501       20      804 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/doc/make.bat
+-rw-r--r--   0      501       20       16 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/doc/requirements.txt
+-rw-r--r--   0      501       20      155 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/doc/source/arrow_odbc.rst
+-rw-r--r--   0      501       20     1965 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/doc/source/conf.py
+-rw-r--r--   0      501       20      458 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/doc/source/index.rst
+-rw-r--r--   0      501       20       67 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/doc/source/modules.rst
+-rw-r--r--   0      501       20      348 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/docker-compose.yml
+-rw-r--r--   0      501       20      564 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/manylinux/Dockerfile
+-rw-r--r--   0      501       20      121 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/manylinux/Readme.md
+-rw-r--r--   0      501       20      148 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/manylinux/WHEEL
+-rw-r--r--   0      501       20     1256 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/manylinux/build_wheel.sh
+-rw-r--r--   0      501       20      617 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/pyproject.toml
+-rw-r--r--   0      501       20      307 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/python/arrow_odbc/__init__.py
+-rw-r--r--   0      501       20     1645 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/python/arrow_odbc/connect.py
+-rw-r--r--   0      501       20      672 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/python/arrow_odbc/error.py
+-rw-r--r--   0      501       20    15067 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/python/arrow_odbc/reader.py
+-rw-r--r--   0      501       20     9164 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/python/arrow_odbc/writer.py
+-rw-r--r--   0      501       20     2322 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/src/error.rs
+-rw-r--r--   0      501       20     2841 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/src/lib.rs
+-rw-r--r--   0      501       20     1239 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/src/parameter.rs
+-rw-r--r--   0      501       20     3033 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/src/reader/arrow_odbc_reader.rs
+-rw-r--r--   0      501       20     6484 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/src/reader.rs
+-rw-r--r--   0      501       20     3613 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/src/writer.rs
+-rw-r--r--   0      501       20        0 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/tests/__init__.py
+-rw-r--r--   0      501       20     4115 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/tests/iris.csv
+-rw-r--r--   0      501       20     2413 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/tests/iris.parquet
+-rw-r--r--   0      501       20    19183 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/tests/test_arrow_odbc.py
+-rw-r--r--   0      501       20    35304 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/Cargo.lock
+-rw-r--r--   0        0        0     8251 1970-01-01 00:00:00.000000 arrow_odbc-1.0.1/PKG-INFO
```

### Comparing `arrow_odbc-1.0.0/Cargo.toml` & `arrow_odbc-1.0.1/Cargo.toml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.0/.github/workflows/test.yml` & `arrow_odbc-1.0.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.0/.github/workflows/wheel.yml` & `arrow_odbc-1.0.1/.github/workflows/wheel.yml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.0/.readthedocs.yaml` & `arrow_odbc-1.0.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.0/Changelog.md` & `arrow_odbc-1.0.1/Changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 1.0.1
+
+- More code examples in Docstrings
+
 ## 1.0.0
 
 - Breaking change: `read_arrow_batches_from_odbc` now also returns a batch reader instead of `None`, even if the SQL statement did not produce a result set. The resulting reader will be empty, i.e. iterating over batches stops immediatly. The assaciated schema attribute will contain no columns.
 - Support for querying stored procedures returning multiple result sets is added. Call `more_results` on the reader to advance to the next result set.
 
 ## 0.3.14
```

### Comparing `arrow_odbc-1.0.0/Contributing.md` & `arrow_odbc-1.0.1/Contributing.md`

 * *Files 4% similar despite different names*

```diff
@@ -49,11 +49,19 @@
 ```shell
 python -m pip install build
 python -m build
 ```
 
 ## Generate documentation
 
+### Posix (with make installed)
+
 ```shell
 cd docs
 make html
 ```
+
+### Windows (without make)
+
+```shell
+sphinx-build -M html ./doc/source ./doc/build
+```
```

### Comparing `arrow_odbc-1.0.0/LICENSE` & `arrow_odbc-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.0/README.md` & `arrow_odbc-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,17 @@
 
 [![Licence](https://img.shields.io/crates/l/arrow-odbc)](https://github.com/pacman82/arrow-odbc-py/blob/master/License)
 [![PyPI version](https://badge.fury.io/py/arrow-odbc.svg)](https://pypi.org/project/arrow-odbc/)
 [![Documentation Status](https://readthedocs.org/projects/arrow-odbc/badge/?version=latest)](https://arrow-odbc.readthedocs.io/en/latest/?badge=latest)
 
 Fill Apache Arrow arrays from ODBC data sources. This package is build on top of the [`pyarrow`](https://pypi.org/project/arrow/) Python package and [`arrow-odbc`](https://crates.io/crates/arrow-odbc) Rust crate and enables you to read the data of an ODBC data source as sequence of Apache Arrow record batches.
 
-This package can also be used to insert data in Arrow record batches to database tables.
-
-This package has been designed to be easily deployable, so it provides a prebuild many linux wheel which is independent of the specific version of your Python interpreter and the specific Arrow Version you want to use. It will dynamically link against the ODBC driver manager provided by your system.
-
-Users looking for more features than just bulk fetching/inserting data from/into ODBC data sources in Python should also take a look at [`turbodbc`](https://github.com/blue-yonder/turbodbc) which has a helpful community and seen a lot of battle testing. This Python package is more narrow in Scope (which is a fancy way of saying it has less features), as it is only concerned with bulk fetching Arrow Arrays. `arrow-odbc` may have less features than `turbodbc`, but it is easier to install and more resilient to version changes in `pyarrow`, since it is independent of C++ ABI, system dependencies (with the exeception of your ODBC driver manager of course) and your specific Python ABI. It also offers pre build wheels windows, linux and OS-X on [`pypi`](https://pypi.org/project/arrow-odbc/). In addition to that there is also a conda-forge recipie (thanks to @timkpaine).
+* **Fast**. Makes efficient use of ODBC bulk reads and writes, to lower IO overhead.
+* **Flexible**. Query any ODBC data source you have a driver for. MySQL, MS SQL, Excel, ...
+* **Portable**. Easy to install and update dependencies. No binary dependency to specific implemenations of Python interpreter, Arrow or ODBC driver manager.
 
 ## About Arrow
 
 > [Apache Arrow](https://arrow.apache.org/) defines a language-independent columnar memory format for flat and hierarchical data, organized for efficient analytic operations on modern hardware like CPUs and GPUs. The Arrow memory format also supports zero-copy reads for lightning-fast data access without serialization overhead.
 
 ## About ODBC
 
@@ -85,30 +83,47 @@
 
 You can use homebrew to install UnixODBC
 
 ```shell
 brew install unixodbc
 ```
 
-### Installing Rust toolchain
-
-Note: **Only required if building from source**
-
-To build from source you need to install the Rust toolchain. Installation instruction can be found here: <https://www.rust-lang.org/tools/install>
-
 ### Installing the wheel
 
-Wheels have been uploaded to [PyPi](https://pypi.org) and can be installed using pip. The wheel (including the manylinux wheel) will link against the your system ODBC driver manager at runtime. If there are no prebuild wheels for your platform, you can build the wheel from source. For this the rust toolchain must be installed.
+This package has been designed to be easily deployable, so it provides a prebuild many linux wheel which is independent of the specific version of your Python interpreter and the specific Arrow Version you want to use. It will dynamically link against the ODBC driver manager provided by your system.
+
+Wheels have been uploaded to [`PyPi`](https://pypi.org/project/arrow-odbc/) and can be installed using pip. The wheel (including the manylinux wheel) will link against the your system ODBC driver manager at runtime. If there are no prebuild wheels for your platform, you can build the wheel from source. For this the rust toolchain must be installed.
 
 ```shell
 pip install arrow-odbc
 ```
 
 `arrow-odbc` utilizes `cffi` and the Arrow C-Interface to glue Rust and Python code together. Therefore the wheel does not need to be build against the precise version either of Python or Arrow.
 
+### Installing with conda
+
+```shell
+conda install -c conda-forge turbodbc
+```
+
+Thanks to @timkpaine for maintaining the recipie!
+
+### Building wheel from source
+
+There is no ready made wheel for the platform you want to target? Do not worry, you can probably build it from source.
+
+* To build from source you need to install the Rust toolchain. Installation instruction can be found here: <https://www.rust-lang.org/tools/install>
+* Install ODBC driver manager. See above.
+* Build wheel
+
+  ```shell
+  python -m pip install build
+  python -m build
+  ```
+
 ## Matching of ODBC to Arrow types then querying
 
 | ODBC                     | Arrow                |
 | ------------------------ | -------------------- |
 | Numeric(p <= 38)         | Decimal128           |
 | Decimal(p <= 38, s >= 0) | Decimal128           |
 | Integer                  | Int32                |
@@ -157,7 +172,12 @@
 | Time32 s              | Time               |
 | Time32 ms             | VarChar(12)        |
 | Time64 us             | VarChar(15)        |
 | Time64 ns             | VarChar(16)        |
 | Binary                | Varbinary          |
 | FixedBinary(l)        | Varbinary(l)       |
 | All others            | Unsupported        |
+
+## Comparision to other Python ODBC bindings
+
+* [`pyodbc`](https://github.com/mkleehammer/pyodbc) - General purpose ODBC python bindings. In contrast `arrow-odbc` is specifically concerned with bulk reads and writes to arrow arrays.
+* [`turbodbc`](https://github.com/blue-yonder/turbodbc) - Complies with the Python Database API Specification 2.0 (PEP 249) which `arrow-odbc` does not aim to do. Like `arrow-odbc` bulk read and writes is the strong point of `turbodbc`. `turbodbc` has more system dependencies, which can make it cumbersome to install if not using conda. `turbodbc` is build against the C++ implementation of Arrow, which implies it is only compatible with matching version of `pyarrow`.
```

### Comparing `arrow_odbc-1.0.0/conftest.py` & `arrow_odbc-1.0.1/conftest.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.0/doc/Makefile` & `arrow_odbc-1.0.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.0/doc/make.bat` & `arrow_odbc-1.0.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.0/doc/source/conf.py` & `arrow_odbc-1.0.1/doc/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "arrow-odbc"
 copyright = "2021, Markus Klein"
 author = "Markus Klein"
 
 # The full version, including alpha/beta/rc tags
-release = "1.0.0"
+release = "1.0.1"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `arrow_odbc-1.0.0/manylinux/Dockerfile` & `arrow_odbc-1.0.1/manylinux/Dockerfile`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.0/manylinux/build_wheel.sh` & `arrow_odbc-1.0.1/manylinux/build_wheel.sh`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.0/pyproject.toml` & `arrow_odbc-1.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "maturin"
 
 [project]
 name = "arrow-odbc"
 authors = [{name = "Markus Klein"}]
 description="Read the data of an ODBC data source as sequence of Apache Arrow record batches."
 readme = "README.md"
-version = "1.0.0"
+version = "1.0.1"
 dependencies = ["cffi", "pyarrow"]
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 test = ["pytest < 8.0.0"]
```

### Comparing `arrow_odbc-1.0.0/python/arrow_odbc/connect.py` & `arrow_odbc-1.0.1/python/arrow_odbc/connect.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.0/python/arrow_odbc/error.py` & `arrow_odbc-1.0.1/python/arrow_odbc/error.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.0/python/arrow_odbc/reader.py` & `arrow_odbc-1.0.1/python/arrow_odbc/reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,26 +12,21 @@
 from .error import raise_on_error
 
 
 def _schema_from_handle(handle) -> Schema:
     """
     Take a handle to an ArrowOdbcReader and return the associated pyarrow schema
     """
-    if handle == ffi.NULL:
-        # The query ran successfully, but did not produce a result
-        return pa.schema([])
-    else:
-        # Expose schema as attribute
-        # https://github.com/apache/arrow/blob/5ead37593472c42f61c76396dde7dcb8954bde70/python/pyarrow/tests/test_cffi.py
-        with arrow_ffi.new("struct ArrowSchema *") as schema_out:
-            error = lib.arrow_odbc_reader_schema(handle, schema_out)
-
-            raise_on_error(error)
-            ptr_schema = int(ffi.cast("uintptr_t", schema_out))
-            return Schema._import_from_c(ptr_schema)
+    # Expose schema as attribute
+    # https://github.com/apache/arrow/blob/5ead37593472c42f61c76396dde7dcb8954bde70/python/pyarrow/tests/test_cffi.py
+    with arrow_ffi.new("struct ArrowSchema *") as schema_out:
+        error = lib.arrow_odbc_reader_schema(handle, schema_out)
+        raise_on_error(error)
+        ptr_schema = int(ffi.cast("uintptr_t", schema_out))
+        return Schema._import_from_c(ptr_schema)
 
 
 class BatchReader:
     """
     Iterates over Arrow batches from an ODBC data source
     """
 
@@ -53,17 +48,16 @@
         self.handle = handle
 
         # If this raises `__del__` will be invoked and free the handle, so we do not leak
         # resources here.
         self.schema = _schema_from_handle(self.handle)
 
     def __del__(self):
-        if self.handle != ffi.NULL:
-            # Free the resources associated with this handle.
-            lib.arrow_odbc_reader_free(self.handle)
+        # Free the resources associated with this handle.
+        lib.arrow_odbc_reader_free(self.handle)
 
     def __iter__(self):
         # Implement iterable protocol so reader can be used in for loops.
         return self
 
     def __next__(self) -> RecordBatch:
         # Implment iterator protocol
@@ -99,14 +93,43 @@
         """
         Move the reader to the next result set returned by the data source.
 
         A datasource may return multiple results if multiple SQL statements are executed in a single
         query or a stored procedure is called. This method closes the current cursor and moves it to
         the next result set. You may move to the next result set without extracting the current one.
 
+        Example:
+
+        .. code-block:: python
+
+            from arrow_odbc import read_arrow_batches_from_odbc
+
+            connection_string="Driver={ODBC Driver 17 for SQL Server};Server=localhost;"
+            reader = read_arrow_batches_from_odbc(
+                query=f"SELECT * FROM MyTable; SELECT * FROM OtherTable;",
+                connection_string=connection_string,
+                batch_size=1000,
+                user="SA",
+                password="My@Test@Password",
+            )
+
+            # Process first result
+            for batch in reader:
+                # Process arrow batches
+                df = batch.to_pandas()
+                # ...
+
+            reader.more_results()
+
+            # Process second result
+            for batch in reader:
+                # Process arrow batches
+                df = batch.to_pandas()
+                # ...
+
         :param batch_size: The maximum number rows within each batch. Batch size can be individually
             choosen for each result set.
         :param max_text_size: An upper limit for the size of buffers bound to variadic text columns
             of the data source. This limit does not (directly) apply to the size of the created
             arrow buffers, but rather applies to the buffers used for the data in transit. Use this
             option if you have e.g. VARCHAR(MAX) fields the next batch.
         :param max_binary_size: An upper limit for the size of buffers bound to variadic binary
@@ -118,46 +141,38 @@
             which scales with the batch size parameter (but not with the amount of actual data in
             the source). In case you can test your query against the schema you can safely set this
             to ``False``. The required memory will not depend on the amount of data in the data
             source. Default is ``True`` though, safety first.
         :return: ``True`` in case there is another result set. ``False`` in case that the last
             result set has been processed.
         """
-        if self.handle == ffi.NULL:
-            # Last result set has already been processed
-            return False
-
         if max_text_size is None:
             max_text_size = 0
         if max_binary_size is None:
             max_binary_size = 0
 
-        reader_out = ffi.new("ArrowOdbcReader **")
-
-        error = lib.arrow_odbc_reader_more_results(
-            self.handle,
-            reader_out,
-            batch_size,
-            max_text_size,
-            max_binary_size,
-            falliable_allocations,
-        )
-
-        # We passed ownership of handle to more_results. We must do this before raising, since
-        # self.handle is otherwise invalid.
-        self.handle = reader_out[0]
+        with ffi.new("bool *") as has_more_results_c:
+            error = lib.arrow_odbc_reader_more_results(
+                self.handle,
+                has_more_results_c,
+                batch_size,
+                max_text_size,
+                max_binary_size,
+                falliable_allocations,
+            )
+            # See if we managed to execute the query successfully and return an
+            # error if not
+            raise_on_error(error)
 
-        # See if we managed to execute the query successfully and return an
-        # error if not
-        raise_on_error(error)
+            has_more_results = has_more_results_c[0] != 0
 
         # Every result set can have its own schema, so we must update our member
         self.schema = _schema_from_handle(self.handle)
 
-        return self.handle != FFI.NULL
+        return has_more_results
 
 
 def read_arrow_batches_from_odbc(
     query: str,
     batch_size: int,
     connection_string: str,
     user: Optional[str] = None,
@@ -167,14 +182,36 @@
     max_binary_size: Optional[int] = None,
     falliable_allocations: bool = True,
     login_timeout_sec: Optional[int] = None,
 ) -> Optional[BatchReader]:
     """
     Execute the query and read the result as an iterator over Arrow batches.
 
+    Example:
+
+    .. code-block:: python
+
+        from arrow_odbc import read_arrow_batches_from_odbc
+
+        connection_string="Driver={ODBC Driver 17 for SQL Server};Server=localhost;"
+
+        reader = read_arrow_batches_from_odbc(
+            query=f"SELECT * FROM MyTable WHERE a=?",
+            connection_string=connection_string,
+            batch_size=1000,
+            parameters=["I'm a positional query parameter"],
+            user="SA",
+            password="My@Test@Password",
+        )
+
+        for batch in reader:
+            # Process arrow batches
+            df = batch.to_pandas()
+            # ...
+
     :param query: The SQL statement yielding the result set which is converted into arrow record
         batches.
     :param batch_size: The maximum number rows within each batch. Please note that the actual batch
         size is up to the ODBC driver of your database. This parameter influences primarily the size
         of the buffers the ODBC driver is supposed to fill with data, yet it is up to the driver how
         many values it fills in one go. Also note that the primary use-case of batching is to reduce
         IO overhead. So even if you fetch millions of rows a batch size of 100 or 1000 may be
```

### Comparing `arrow_odbc-1.0.0/python/arrow_odbc/writer.py` & `arrow_odbc-1.0.1/python/arrow_odbc/writer.py`

 * *Files 10% similar despite different names*

```diff
@@ -61,14 +61,35 @@
     user: Optional[str] = None,
     password: Optional[str] = None,
     login_timeout_sec: Optional[int] = None,
 ):
     """
     Consume the batches in the reader and insert them into a table on the database.
 
+    Example:
+
+    .. code-block:: python
+
+        from arrow_odbc import insert_into_table
+        import pyarrow as pa
+        import pandas
+
+
+        def dataframe_to_table(df):
+            table = pa.Table.from_pandas(df)
+            reader = pa.RecordBatchReader.from_batches(table.schema, table.to_batches())
+            insert_into_table(
+                connection_string=connection_string,
+                user="SA",
+                password="My@Test@Password",
+                chunk_size=1000,
+                table="MyTable",
+                reader=reader,
+            )
+
     :param reader: Reader is used to iterate over record batches. It must expose a `schema`
         attribute, referencing an Arrow schema. Each field in the schema must correspond to a
         column in the table with identical name. The iterator must yield individual arrow tables
     :param chunk_size: Number of records to insert in each roundtrip to the database. Independent of
         batch size (i.e. number of rows in an individual record batch).
     :param table: Name of a database table to insert into. Used to generate the insert statement for
         the bulk writer.
@@ -134,14 +155,37 @@
     user: Optional[str] = None,
     password: Optional[str] = None,
     login_timeout_sec: Optional[int] = None,
 ):
     """
     Reads an arrow table and inserts its contents into a relational table on the database.
 
+    This is a convinience wrapper around ``insert_into_table`` which converts an arrow table into a
+    record batch reader for you.
+
+    Example:
+
+    .. code-block:: python
+
+        from arrow_odbc import from_table_to_db
+        import pyarrow as pa
+        import pandas
+
+
+        def dataframe_to_table(df):
+            table = pa.Table.from_pandas(df)
+            from_table_to_db(
+                source=table
+                connection_string=connection_string,
+                user="SA",
+                password="My@Test@Password",
+                chunk_size=1000,
+                table="MyTable",
+            )
+
     :param source: PyArrow table with content to be inserted into the target table on the database.
         Each column of the table must correspond to a column in the target table with identical
         name.
     :param target: Name of the database table to insert into.
     :param connection_string: ODBC Connection string used to connect to the data source. To find a
         connection string for your data source try https://www.connectionstrings.com/.
     :param chunk_size: Number of records to insert in each roundtrip to the database. The number
```

### Comparing `arrow_odbc-1.0.0/src/error.rs` & `arrow_odbc-1.0.1/src/error.rs`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,23 @@
 
     /// Moves the instance to the heap and return a pointer to it.
     pub fn into_raw(self) -> *mut ArrowOdbcError {
         Box::into_raw(Box::new(self))
     }
 }
 
+impl<T> From<T> for ArrowOdbcError
+where
+    T: Display,
+{
+    fn from(source: T) -> ArrowOdbcError {
+        ArrowOdbcError::new(source)
+    }
+}
+
 /// Deallocates the resources associated with an error.
 ///
 /// # Safety
 ///
 /// Error must be a valid non null pointer to an Error.
 #[no_mangle]
 pub unsafe extern "C" fn arrow_odbc_error_free(error: NonNull<ArrowOdbcError>) {
@@ -48,15 +57,16 @@
 #[macro_export]
 macro_rules! try_ {
     ($call:expr) => {
         match $call {
             Ok(value) => value,
             Err(error) => {
                 // Early return in case of error
-                return ArrowOdbcError::new(error).into_raw();
+                let error = Into::<ArrowOdbcError>::into(error);
+                return error.into_raw();
             }
         }
     };
 }
 
 #[cfg(test)]
 mod tests {
```

### Comparing `arrow_odbc-1.0.0/src/lib.rs` & `arrow_odbc-1.0.1/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 //! Defines C bindings for `arrow-odbc` to enable using it from Python.
-
 mod error;
 mod parameter;
 mod reader;
 mod writer;
 
 use std::{borrow::Cow, ptr::null_mut, slice, str};
```

### Comparing `arrow_odbc-1.0.0/src/parameter.rs` & `arrow_odbc-1.0.1/src/parameter.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.0/src/reader.rs` & `arrow_odbc-1.0.1/src/reader.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,23 @@
+mod arrow_odbc_reader;
+
 use std::{
     ffi::c_void,
     mem::swap,
     os::raw::c_int,
     ptr::{null_mut, NonNull},
     slice, str,
 };
 
-use arrow::ffi::{ArrowArray, ArrowArrayRef, FFI_ArrowArray, FFI_ArrowSchema};
-use arrow_odbc::{
-    arrow::{
-        array::{Array, StructArray},
-        record_batch::RecordBatchReader,
-    },
-    odbc_api::{Cursor, CursorImpl, StatementConnection},
-    BufferAllocationOptions, OdbcReader,
-};
+use arrow::ffi::{FFI_ArrowArray, FFI_ArrowSchema};
+use arrow_odbc::BufferAllocationOptions;
 
 use crate::{parameter::ArrowOdbcParameter, try_, ArrowOdbcError, OdbcConnection};
 
-/// Opaque type holding all the state associated with an ODBC reader implementation in Rust. This
-/// type also has ownership of the ODBC Connection handle.
-pub struct ArrowOdbcReader(OdbcReader<CursorImpl<StatementConnection<'static>>>);
+pub use self::arrow_odbc_reader::ArrowOdbcReader;
 
 /// Creates an Arrow ODBC reader instance.
 ///
 /// Takes ownership of connection even in case of an error. `reader_out` is assigned a NULL pointer
 /// in case the query does not return a result set.
 ///
 /// # Safety
@@ -70,44 +63,28 @@
     } else {
         slice::from_raw_parts(parameters, parameters_len)
             .iter()
             .map(|&p| Box::from_raw(p).unwrap())
             .collect()
     };
 
-    let max_text_size = if max_text_size == 0 {
-        None
-    } else {
-        Some(max_text_size)
-    };
-
-    let max_binary_size = if max_binary_size == 0 {
-        None
-    } else {
-        Some(max_binary_size)
-    };
-
-    let buffer_allocation_options = BufferAllocationOptions {
-        max_text_size,
-        max_binary_size,
-        fallibale_allocations,
-    };
+    let buffer_allocation_options =
+        alloc_opts_from_c_args(max_text_size, max_binary_size, fallibale_allocations);
 
     let maybe_cursor = try_!(connection.0.into_cursor(query, &parameters[..]));
-    if let Some(cursor) = maybe_cursor {
-        let reader = try_!(OdbcReader::with(
+    let reader = if let Some(cursor) = maybe_cursor {
+        try_!(ArrowOdbcReader::new(
             cursor,
             batch_size,
-            None,
             buffer_allocation_options
-        ));
-        *reader_out = Box::into_raw(Box::new(ArrowOdbcReader(reader)))
+        ))
     } else {
-        *reader_out = null_mut()
-    }
+        ArrowOdbcReader::empty()
+    };
+    *reader_out = Box::into_raw(Box::new(reader));
     null_mut() // Ok(())
 }
 
 /// Frees the resources associated with an ArrowOdbcReader
 ///
 /// # Safety
 ///
@@ -130,108 +107,83 @@
     array: *mut c_void,
     schema: *mut c_void,
     has_next_out: *mut c_int,
 ) -> *mut ArrowOdbcError {
     let schema = schema as *mut FFI_ArrowSchema;
     let array = array as *mut FFI_ArrowArray;
 
-    if let Some(result) = reader.as_mut().0.next() {
-        // In case of an error fail early, before we change the output paramters.
-        let batch = try_!(result);
-        let struct_array: StructArray = batch.into();
-        let arrow_array = try_!(ArrowArray::try_new(struct_array.data().clone()));
+    // In case of an error fail early, before we change the output paramters.
+    let batch = try_!(reader.as_mut().next_batch());
 
+    if let Some((mut ffi_array, mut ffi_schema)) = batch {
         // Create two empty instances, so array and schema now point to valid instances.
         *array = FFI_ArrowArray::empty();
         *schema = FFI_ArrowSchema::empty();
         // Now that the instances are valid it safe to use them as references rather than pointers
         // (references must always be valid)
         let array = &mut *array;
         let schema = &mut *schema;
 
-        let array_data = arrow_array.to_data().unwrap();
-
-        let mut ffi_array = FFI_ArrowArray::new(&array_data);
-        let mut ffi_schema = FFI_ArrowSchema::try_from(array_data.data_type()).unwrap();
-
         swap(array, &mut ffi_array);
         swap(schema, &mut ffi_schema);
 
         *has_next_out = 1;
     } else {
         *has_next_out = 0;
     }
     null_mut()
 }
 
 /// # Safety
 ///
-/// * `reader_in` must point to a valid non-null reader, allocated by [`arrow_odbc_reader_make`].
-///   This function takes ownership of reader_in and will free the associated resources, even in
-///   case of error. After the function call `reader_in` is invalid and must not be dereferenced.
-/// * `reader_out` In case another result set exists, `reader_out` will point to a valid instance of
-///   [`ArrowOdbcReader`]. Otherwise, it will point to `NULL`.
+/// * `reader` must point to a valid non-null reader, allocated by [`arrow_odbc_reader_make`].
+/// * `has_more_results` must point to a valid boolean.
 #[no_mangle]
 pub unsafe extern "C" fn arrow_odbc_reader_more_results(
-    reader_in: NonNull<ArrowOdbcReader>,
-    reader_out: *mut *mut ArrowOdbcReader,
+    mut reader: NonNull<ArrowOdbcReader>,
+    has_more_results: *mut bool,
     batch_size: usize,
     max_text_size: usize,
     max_binary_size: usize,
     fallibale_allocations: bool,
 ) -> *mut ArrowOdbcError {
-    // In case we return early, we want the caller to know that reader_out is invalid.
-    *reader_out = null_mut();
-
-    // Dereference reader and take ownership of it.
-    let reader = Box::from_raw(reader_in.as_ptr()).0;
-
+    let buffer_allocation_options =
+        alloc_opts_from_c_args(max_text_size, max_binary_size, fallibale_allocations);
     // Move cursor to the next result set.
-    let cursor = try_!(reader.into_cursor());
-    let next = try_!(cursor.more_results());
-
-    if let Some(cursor) = next {
-        // There is another result set. Let us create an new reader
-        let max_text_size = if max_text_size == 0 {
-            None
-        } else {
-            Some(max_text_size)
-        };
-        let max_binary_size = if max_binary_size == 0 {
-            None
-        } else {
-            Some(max_binary_size)
-        };
-        let buffer_allocation_options = BufferAllocationOptions {
-            max_text_size,
-            max_binary_size,
-            fallibale_allocations,
-        };
-
-        let reader = try_!(OdbcReader::with(
-            cursor,
-            batch_size,
-            None,
-            buffer_allocation_options
-        ));
-        let reader = ArrowOdbcReader(reader);
-        *reader_out = Box::into_raw(Box::new(reader));
-    }
-
+    *has_more_results = try_!(reader.as_mut().more_results(batch_size, buffer_allocation_options));
     null_mut()
 }
 
 /// Retrieve the associated schema from a reader.
 #[no_mangle]
 pub unsafe extern "C" fn arrow_odbc_reader_schema(
-    mut reader: NonNull<ArrowOdbcReader>,
+    reader: NonNull<ArrowOdbcReader>,
     out_schema: *mut c_void,
 ) -> *mut ArrowOdbcError {
-    let out_schema: *mut FFI_ArrowSchema = out_schema as *mut FFI_ArrowSchema;
+    let out_schema = out_schema as *mut FFI_ArrowSchema;
 
-    let reader = &mut reader.as_mut().0;
-    let schema_ref = reader.schema();
-    let schema = &*schema_ref;
-    let schema_ffi = try_!(schema.try_into());
+    let schema_ffi = try_!(reader.as_ref().schema());
     *out_schema = schema_ffi;
     null_mut()
 }
+
+fn alloc_opts_from_c_args(
+    max_text_size: usize,
+    max_binary_size: usize,
+    fallibale_allocations: bool,
+) -> BufferAllocationOptions {
+    let max_text_size = if max_text_size == 0 {
+        None
+    } else {
+        Some(max_text_size)
+    };
+    let max_binary_size = if max_binary_size == 0 {
+        None
+    } else {
+        Some(max_binary_size)
+    };
+    BufferAllocationOptions {
+        max_text_size,
+        max_binary_size,
+        fallibale_allocations,
+    }
+}
```

### Comparing `arrow_odbc-1.0.0/src/writer.rs` & `arrow_odbc-1.0.1/src/writer.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.0/tests/iris.csv` & `arrow_odbc-1.0.1/tests/iris.csv`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.0/tests/iris.parquet` & `arrow_odbc-1.0.1/tests/iris.parquet`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.0/tests/test_arrow_odbc.py` & `arrow_odbc-1.0.1/tests/test_arrow_odbc.py`

 * *Files 0% similar despite different names*

```diff
@@ -514,15 +514,15 @@
         yield pa.RecordBatch.from_arrays([pa.array([(1, 1)])], schema=schema)
 
     reader = pa.RecordBatchReader.from_batches(schema, iter_record_batches())
 
     # When / Then
     with raises(
         Error,
-        match="The arrow data type Dictionary\(Int32, Int32\) is not supported for insertion.",
+        match=r"The arrow data type Dictionary\(Int32, Int32\) is not supported for insertion.",
     ):
         insert_into_table(
             connection_string=MSSQL,
             chunk_size=20,
             table="MyTable",
             reader=reader,
         )
```

### Comparing `arrow_odbc-1.0.0/Cargo.lock` & `arrow_odbc-1.0.1/Cargo.lock`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.0/PKG-INFO` & `arrow_odbc-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Metadata-Version: 2.1
 Name: arrow-odbc
-Version: 1.0.0
+Version: 1.0.1
 Requires-Dist: cffi
 Requires-Dist: pyarrow
 Requires-Dist: pytest < 8.0.0; extra == 'test'
 Provides-Extra: test
 License-File: LICENSE
 Summary: Read the data of an ODBC data source as sequence of Apache Arrow record batches.
 Author: Markus Klein
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: repository, https://github.com/pacman82/arrow-odbc-py
 Project-URL: changelog, https://github.com/pacman82/arrow-odbc-py/blob/main/Changelog.md
+Project-URL: repository, https://github.com/pacman82/arrow-odbc-py
 
 # arrow-odbc-py
 
 [![Licence](https://img.shields.io/crates/l/arrow-odbc)](https://github.com/pacman82/arrow-odbc-py/blob/master/License)
 [![PyPI version](https://badge.fury.io/py/arrow-odbc.svg)](https://pypi.org/project/arrow-odbc/)
 [![Documentation Status](https://readthedocs.org/projects/arrow-odbc/badge/?version=latest)](https://arrow-odbc.readthedocs.io/en/latest/?badge=latest)
 
 Fill Apache Arrow arrays from ODBC data sources. This package is build on top of the [`pyarrow`](https://pypi.org/project/arrow/) Python package and [`arrow-odbc`](https://crates.io/crates/arrow-odbc) Rust crate and enables you to read the data of an ODBC data source as sequence of Apache Arrow record batches.
 
-This package can also be used to insert data in Arrow record batches to database tables.
-
-This package has been designed to be easily deployable, so it provides a prebuild many linux wheel which is independent of the specific version of your Python interpreter and the specific Arrow Version you want to use. It will dynamically link against the ODBC driver manager provided by your system.
-
-Users looking for more features than just bulk fetching/inserting data from/into ODBC data sources in Python should also take a look at [`turbodbc`](https://github.com/blue-yonder/turbodbc) which has a helpful community and seen a lot of battle testing. This Python package is more narrow in Scope (which is a fancy way of saying it has less features), as it is only concerned with bulk fetching Arrow Arrays. `arrow-odbc` may have less features than `turbodbc`, but it is easier to install and more resilient to version changes in `pyarrow`, since it is independent of C++ ABI, system dependencies (with the exeception of your ODBC driver manager of course) and your specific Python ABI. It also offers pre build wheels windows, linux and OS-X on [`pypi`](https://pypi.org/project/arrow-odbc/). In addition to that there is also a conda-forge recipie (thanks to @timkpaine).
+* **Fast**. Makes efficient use of ODBC bulk reads and writes, to lower IO overhead.
+* **Flexible**. Query any ODBC data source you have a driver for. MySQL, MS SQL, Excel, ...
+* **Portable**. Easy to install and update dependencies. No binary dependency to specific implemenations of Python interpreter, Arrow or ODBC driver manager.
 
 ## About Arrow
 
 > [Apache Arrow](https://arrow.apache.org/) defines a language-independent columnar memory format for flat and hierarchical data, organized for efficient analytic operations on modern hardware like CPUs and GPUs. The Arrow memory format also supports zero-copy reads for lightning-fast data access without serialization overhead.
 
 ## About ODBC
 
@@ -99,30 +97,47 @@
 
 You can use homebrew to install UnixODBC
 
 ```shell
 brew install unixodbc
 ```
 
-### Installing Rust toolchain
-
-Note: **Only required if building from source**
-
-To build from source you need to install the Rust toolchain. Installation instruction can be found here: <https://www.rust-lang.org/tools/install>
-
 ### Installing the wheel
 
-Wheels have been uploaded to [PyPi](https://pypi.org) and can be installed using pip. The wheel (including the manylinux wheel) will link against the your system ODBC driver manager at runtime. If there are no prebuild wheels for your platform, you can build the wheel from source. For this the rust toolchain must be installed.
+This package has been designed to be easily deployable, so it provides a prebuild many linux wheel which is independent of the specific version of your Python interpreter and the specific Arrow Version you want to use. It will dynamically link against the ODBC driver manager provided by your system.
+
+Wheels have been uploaded to [`PyPi`](https://pypi.org/project/arrow-odbc/) and can be installed using pip. The wheel (including the manylinux wheel) will link against the your system ODBC driver manager at runtime. If there are no prebuild wheels for your platform, you can build the wheel from source. For this the rust toolchain must be installed.
 
 ```shell
 pip install arrow-odbc
 ```
 
 `arrow-odbc` utilizes `cffi` and the Arrow C-Interface to glue Rust and Python code together. Therefore the wheel does not need to be build against the precise version either of Python or Arrow.
 
+### Installing with conda
+
+```shell
+conda install -c conda-forge turbodbc
+```
+
+Thanks to @timkpaine for maintaining the recipie!
+
+### Building wheel from source
+
+There is no ready made wheel for the platform you want to target? Do not worry, you can probably build it from source.
+
+* To build from source you need to install the Rust toolchain. Installation instruction can be found here: <https://www.rust-lang.org/tools/install>
+* Install ODBC driver manager. See above.
+* Build wheel
+
+  ```shell
+  python -m pip install build
+  python -m build
+  ```
+
 ## Matching of ODBC to Arrow types then querying
 
 | ODBC                     | Arrow                |
 | ------------------------ | -------------------- |
 | Numeric(p <= 38)         | Decimal128           |
 | Decimal(p <= 38, s >= 0) | Decimal128           |
 | Integer                  | Int32                |
@@ -172,7 +187,12 @@
 | Time32 ms             | VarChar(12)        |
 | Time64 us             | VarChar(15)        |
 | Time64 ns             | VarChar(16)        |
 | Binary                | Varbinary          |
 | FixedBinary(l)        | Varbinary(l)       |
 | All others            | Unsupported        |
 
+## Comparision to other Python ODBC bindings
+
+* [`pyodbc`](https://github.com/mkleehammer/pyodbc) - General purpose ODBC python bindings. In contrast `arrow-odbc` is specifically concerned with bulk reads and writes to arrow arrays.
+* [`turbodbc`](https://github.com/blue-yonder/turbodbc) - Complies with the Python Database API Specification 2.0 (PEP 249) which `arrow-odbc` does not aim to do. Like `arrow-odbc` bulk read and writes is the strong point of `turbodbc`. `turbodbc` has more system dependencies, which can make it cumbersome to install if not using conda. `turbodbc` is build against the C++ implementation of Arrow, which implies it is only compatible with matching version of `pyarrow`.
+
```

