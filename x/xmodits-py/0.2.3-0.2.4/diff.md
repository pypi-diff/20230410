# Comparing `tmp/xmodits_py-0.2.3.tar.gz` & `tmp/xmodits_py-0.2.4.tar.gz`

## Comparing `xmodits_py-0.2.3.tar` & `xmodits_py-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 xmodits_py-0.2.3/Cargo.toml
--rw-r--r--   0     1001      123     2794 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      775 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/.gitignore
--rw-r--r--   0     1001      123    42803 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/LICENSE
--rw-r--r--   0     1001      123     3380 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/README.md
--rw-r--r--   0     1001      123        0 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/examples/example_1.md
--rw-r--r--   0     1001      123      214 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/examples/example_1.py
--rw-r--r--   0     1001      123        0 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/examples/example_2.md
--rw-r--r--   0     1001      123      250 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/examples/example_2.py
--rw-r--r--   0     1001      123        0 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/examples/example_3.md
--rw-r--r--   0     1001      123      253 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/examples/example_3.py
--rw-r--r--   0     1001      123        0 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/examples/example_4.md
--rw-r--r--   0     1001      123      253 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/examples/example_4.py
--rw-r--r--   0     1001      123        0 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/examples/example_5.md
--rw-r--r--   0     1001      123      238 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/examples/example_5.py
--rw-r--r--   0     1001      123        0 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/examples/example_6.md
--rw-r--r--   0     1001      123      504 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/examples/example_6.py
--rw-r--r--   0     1001      123      638 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/pyproject.toml
--rw-r--r--   0     1001      123     1772 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/src/api.rs
--rw-r--r--   0     1001      123     2987 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/src/error.rs
--rw-r--r--   0     1001      123     1179 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/src/lib.rs
--rw-r--r--   0     1001      123    11664 2023-04-08 19:53:35.000000 xmodits_py-0.2.3/Cargo.lock
--rw-r--r--   0        0        0     3934 1970-01-01 00:00:00.000000 xmodits_py-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 xmodits_py-0.2.4/Cargo.toml
+-rw-r--r--   0     1001      123     2794 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      775 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/.gitignore
+-rw-r--r--   0     1001      123    42803 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/LICENSE
+-rw-r--r--   0     1001      123     3380 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/README.md
+-rw-r--r--   0     1001      123        0 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/examples/example_1.md
+-rw-r--r--   0     1001      123      214 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/examples/example_1.py
+-rw-r--r--   0     1001      123        0 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/examples/example_2.md
+-rw-r--r--   0     1001      123      250 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/examples/example_2.py
+-rw-r--r--   0     1001      123        0 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/examples/example_3.md
+-rw-r--r--   0     1001      123      253 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/examples/example_3.py
+-rw-r--r--   0     1001      123        0 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/examples/example_4.md
+-rw-r--r--   0     1001      123      253 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/examples/example_4.py
+-rw-r--r--   0     1001      123        0 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/examples/example_5.md
+-rw-r--r--   0     1001      123      238 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/examples/example_5.py
+-rw-r--r--   0     1001      123        0 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/examples/example_6.md
+-rw-r--r--   0     1001      123      504 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/examples/example_6.py
+-rw-r--r--   0     1001      123      638 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/pyproject.toml
+-rw-r--r--   0     1001      123     1772 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/src/api.rs
+-rw-r--r--   0     1001      123     2987 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/src/error.rs
+-rw-r--r--   0     1001      123     1179 2023-04-10 20:36:29.000000 xmodits_py-0.2.4/src/lib.rs
+-rw-r--r--   0     1001      123    11664 2023-04-10 20:37:42.000000 xmodits_py-0.2.4/Cargo.lock
+-rw-r--r--   0        0        0     3934 1970-01-01 00:00:00.000000 xmodits_py-0.2.4/PKG-INFO
```

### Comparing `xmodits_py-0.2.3/Cargo.toml` & `xmodits_py-0.2.4/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [package]
 name = "xmodits_py"
 authors = ["B0ney - https://github.com/B0ney"]
 description = "Extract samples from tracker modules. Supports IT, XM, S3M, MOD, UMX, MPTM"
-version = "0.2.3"
+version = "0.2.4"
 edition = "2021"
 license = "LGPLv3"
 readme = "README.md"
 repository = "https://github.com/B0ney/xmodits-py"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "xmodits"
 crate-type = ["cdylib"]
 
 [dependencies]
-xmodits-lib = { git = "https://github.com/B0ney/xmodits-lib", rev = "fbaa2bd80e94150e9e8a25e4874fd52c38f785c5"}
+xmodits-lib = { git = "https://github.com/B0ney/xmodits-lib", rev = "2101418bda6a7069a889ffc2d3076d963776e3b2"}
 
 [dependencies.pyo3]
 version = "0.18.1"
 features = ["extension-module", "abi3-py37", "anyhow"]
 
 [profile.release]
 strip = true
```

### Comparing `xmodits_py-0.2.3/.github/workflows/CI.yml` & `xmodits_py-0.2.4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `xmodits_py-0.2.3/.gitignore` & `xmodits_py-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `xmodits_py-0.2.3/LICENSE` & `xmodits_py-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xmodits_py-0.2.3/README.md` & `xmodits_py-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `xmodits_py-0.2.3/pyproject.toml` & `xmodits_py-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xmodits_py-0.2.3/src/api.rs` & `xmodits_py-0.2.4/src/api.rs`

 * *Files identical despite different names*

### Comparing `xmodits_py-0.2.3/src/error.rs` & `xmodits_py-0.2.4/src/error.rs`

 * *Files identical despite different names*

### Comparing `xmodits_py-0.2.3/src/lib.rs` & `xmodits_py-0.2.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `xmodits_py-0.2.3/Cargo.lock` & `xmodits_py-0.2.4/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -418,22 +418,22 @@
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
 name = "xmodits-lib"
 version = "0.6.0"
-source = "git+https://github.com/B0ney/xmodits-lib?rev=fbaa2bd80e94150e9e8a25e4874fd52c38f785c5#fbaa2bd80e94150e9e8a25e4874fd52c38f785c5"
+source = "git+https://github.com/B0ney/xmodits-lib?rev=2101418bda6a7069a889ffc2d3076d963776e3b2#2101418bda6a7069a889ffc2d3076d963776e3b2"
 dependencies = [
  "bytemuck",
  "extended",
  "rubato",
  "thiserror",
 ]
 
 [[package]]
 name = "xmodits_py"
-version = "0.2.3"
+version = "0.2.4"
 dependencies = [
  "pyo3",
  "xmodits-lib",
 ]
```

### Comparing `xmodits_py-0.2.3/PKG-INFO` & `xmodits_py-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmodits_py
-Version: 0.2.3
+Version: 0.2.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Extract samples from tracker modules. Supports IT, XM, S3M, MOD, UMX, MPTM
 Author: B0ney - https://github.com/B0ney
 License: LGPLv3
```

