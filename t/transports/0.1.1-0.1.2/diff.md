# Comparing `tmp/transports-0.1.1.tar.gz` & `tmp/transports-0.1.2.tar.gz`

## Comparing `transports-0.1.1.tar` & `transports-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 transports-0.1.1/local_dependencies/transports/Cargo.toml
--rw-r--r--   0      501       20    11352 2023-04-06 03:00:24.000000 transports-0.1.1/local_dependencies/transports/LICENSE
--rw-r--r--   0      501       20     1652 2023-04-06 03:00:24.000000 transports-0.1.1/local_dependencies/transports/Makefile
--rw-r--r--   0      501       20      663 2023-04-06 03:00:24.000000 transports-0.1.1/local_dependencies/transports/README.md
--rw-r--r--   0      501       20       31 2023-04-06 03:00:24.000000 transports-0.1.1/local_dependencies/transports/src/lib.rs
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 transports-0.1.1/Cargo.toml
--rw-r--r--   0      501       20    11352 2023-04-06 03:00:24.000000 transports-0.1.1/LICENSE
--rw-r--r--   0      501       20      942 2023-04-06 03:00:38.000000 transports-0.1.1/Makefile
--rw-r--r--   0      501       20      663 2023-04-06 03:00:24.000000 transports-0.1.1/README.md
--rw-r--r--   0      501       20     1649 2023-04-06 03:01:24.000000 transports-0.1.1/pyproject.toml
--rw-r--r--   0      501       20      216 2023-04-06 03:00:24.000000 transports-0.1.1/src/lib.rs
--rw-r--r--   0      501       20      569 2023-04-06 03:01:24.000000 transports-0.1.1/transports/__init__.py
--rw-r--r--   0      501       20     1497 2023-04-06 03:00:24.000000 transports-0.1.1/transports/client.py
--rw-r--r--   0      501       20     1774 2023-04-06 03:00:24.000000 transports-0.1.1/transports/connection.py
--rw-r--r--   0      501       20       45 2023-04-06 03:00:24.000000 transports-0.1.1/transports/exceptions.py
--rw-r--r--   0      501       20       99 2023-04-06 03:00:24.000000 transports-0.1.1/transports/handlers/__init__.py
--rw-r--r--   0      501       20     1288 2023-04-06 03:00:24.000000 transports-0.1.1/transports/handlers/aiohttp_client.py
--rw-r--r--   0      501       20     1863 2023-04-06 03:00:24.000000 transports-0.1.1/transports/handlers/starlette.py
--rw-r--r--   0      501       20     2686 2023-04-06 03:00:24.000000 transports-0.1.1/transports/json.py
--rw-r--r--   0      501       20     5850 2023-04-06 03:00:24.000000 transports-0.1.1/transports/model.py
--rw-r--r--   0      501       20     1839 2023-04-06 03:00:24.000000 transports-0.1.1/transports/server.py
--rw-r--r--   0      501       20     2049 2023-04-06 03:00:24.000000 transports-0.1.1/transports/tests/test_transport.py
--rw-r--r--   0      501       20     6188 2023-04-06 03:00:24.000000 transports-0.1.1/transports/transport.py
--rw-r--r--   0      501       20     2146 2023-04-06 03:00:24.000000 transports-0.1.1/transports/update.py
--rw-r--r--   0      501       20      261 2023-04-06 03:00:24.000000 transports-0.1.1/transports/utils.py
--rw-r--r--   0      501       20    18688 2023-04-06 03:03:46.000000 transports-0.1.1/Cargo.lock
--rw-r--r--   0        0        0     2342 1970-01-01 00:00:00.000000 transports-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 transports-0.1.2/local_dependencies/transports/Cargo.toml
+-rw-r--r--   0      501       20    11352 2023-04-06 03:00:24.000000 transports-0.1.2/local_dependencies/transports/LICENSE
+-rw-r--r--   0      501       20     1476 2023-04-09 22:30:35.000000 transports-0.1.2/local_dependencies/transports/Makefile
+-rw-r--r--   0      501       20      680 2023-04-07 23:26:41.000000 transports-0.1.2/local_dependencies/transports/README.md
+-rw-r--r--   0      501       20       31 2023-04-06 03:00:24.000000 transports-0.1.2/local_dependencies/transports/src/lib.rs
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 transports-0.1.2/Cargo.toml
+-rw-r--r--   0      501       20    11352 2023-04-06 03:00:24.000000 transports-0.1.2/LICENSE
+-rw-r--r--   0      501       20     1387 2023-04-09 22:56:11.000000 transports-0.1.2/Makefile
+-rw-r--r--   0      501       20      680 2023-04-07 23:26:41.000000 transports-0.1.2/README.md
+-rw-r--r--   0      501       20     1667 2023-04-09 22:52:30.000000 transports-0.1.2/pyproject.toml
+-rw-r--r--   0      501       20      216 2023-04-06 03:00:24.000000 transports-0.1.2/src/lib.rs
+-rw-r--r--   0      501       20      569 2023-04-09 22:52:30.000000 transports-0.1.2/transports/__init__.py
+-rw-r--r--   0      501       20     1497 2023-04-06 03:00:24.000000 transports-0.1.2/transports/client.py
+-rw-r--r--   0      501       20     1774 2023-04-06 03:00:24.000000 transports-0.1.2/transports/connection.py
+-rw-r--r--   0      501       20       45 2023-04-06 03:00:24.000000 transports-0.1.2/transports/exceptions.py
+-rw-r--r--   0      501       20       99 2023-04-06 03:00:24.000000 transports-0.1.2/transports/handlers/__init__.py
+-rw-r--r--   0      501       20     1288 2023-04-06 03:00:24.000000 transports-0.1.2/transports/handlers/aiohttp_client.py
+-rw-r--r--   0      501       20     1863 2023-04-06 03:00:24.000000 transports-0.1.2/transports/handlers/starlette.py
+-rw-r--r--   0      501       20     2686 2023-04-06 03:00:24.000000 transports-0.1.2/transports/json.py
+-rw-r--r--   0      501       20     5850 2023-04-06 03:00:24.000000 transports-0.1.2/transports/model.py
+-rw-r--r--   0      501       20     1839 2023-04-06 03:00:24.000000 transports-0.1.2/transports/server.py
+-rw-r--r--   0      501       20     2049 2023-04-06 03:00:24.000000 transports-0.1.2/transports/tests/test_transport.py
+-rw-r--r--   0      501       20     6188 2023-04-06 03:00:24.000000 transports-0.1.2/transports/transport.py
+-rw-r--r--   0      501       20     2146 2023-04-06 03:00:24.000000 transports-0.1.2/transports/update.py
+-rw-r--r--   0      501       20      261 2023-04-06 03:00:24.000000 transports-0.1.2/transports/utils.py
+-rw-r--r--   0      501       20    20619 2023-04-09 22:56:20.000000 transports-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0     2385 1970-01-01 00:00:00.000000 transports-0.1.2/PKG-INFO
```

### Comparing `transports-0.1.1/local_dependencies/transports/LICENSE` & `transports-0.1.2/local_dependencies/transports/LICENSE`

 * *Files identical despite different names*

### Comparing `transports-0.1.1/local_dependencies/transports/Makefile` & `transports-0.1.2/local_dependencies/transports/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .DEFAULT_GOAL := help
-.PHONY: dev build lint fix check tests tests-ci-run tests-ci-gha tests-ci-jenkins develop test format checks help
+.PHONY: dev build lint fix check tests tests-ci develop test format checks help
 
 dev:  ## Install required dev dependencies
 	rustup component add rustfmt
 	rustup component add clippy
 	cargo install cargo2junit
 	cargo install grcov
 	cargo install -f wasm-bindgen-cli
@@ -23,27 +23,24 @@
 check:
 	cargo check --all-features
 
 tests:  ## Run the tests
 	cargo test -- --show-output
 	# cargo test -- -Z unstable-options --format json | cargo2junit > junit.xml
 
-tests-ci-run: $(eval SHELL:=/bin/bash)
+tests-ci: $(eval SHELL:=/bin/bash)
 	{ \
 		export CARGO_INCREMENTAL=0;\
 		export RUSTDOCFLAGS="-Cpanic=abort";\
 		export RUSTFLAGS="-Zprofile -Ccodegen-units=1 -Copt-level=0 -Clink-dead-code -Coverflow-checks=off -Zpanic_abort_tests -Cpanic=abort";\
 		cargo test -- -Z unstable-options --format json | cargo2junit > junit.xml;\
+		grcov . --llvm -s . -t cobertura --branch --ignore-not-existing -o ./coverage.xml;\
 	}
 
-tests-ci-gha: tests-ci-run
-	grcov . --llvm -s . -t lcov --branch --ignore-not-existing -o ./coverage.info;\
 
-tests-ci-jenkins: tests-ci-run
-	grcov . --llvm -s . -t cobertura --branch --ignore-not-existing -o ./coverage.xml;\
 
 # aliases
 develop: dev
 test: tests
 format: fix
 checks: check
```

### Comparing `transports-0.1.1/local_dependencies/transports/README.md` & `transports-0.1.2/local_dependencies/transports/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 # transports
 Generic communication library
 
 [![Build Status](https://github.com/timkpaine/transports/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/timkpaine/transports/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/timkpaine/transports/branch/main/graph/badge.svg)](https://codecov.io/gh/timkpaine/transports)
-[![PyPI](https://img.shields.io/pypi/l/transports.svg)](https://pypi.python.org/pypi/transports)
+[![License](https://img.shields.io/github/license/timkpaine/transports)](https://github.com/timkpaine/transports)
 [![PyPI](https://img.shields.io/pypi/v/transports.svg)](https://pypi.python.org/pypi/transports)
 <!-- [![npm](https://img.shields.io/npm/v/transports.svg)](https://www.npmjs.com/package/transports) -->
```

### Comparing `transports-0.1.1/Cargo.toml` & `transports-0.1.2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `transports-0.1.1/LICENSE` & `transports-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `transports-0.1.1/README.md` & `transports-0.1.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 # transports
 Generic communication library
 
 [![Build Status](https://github.com/timkpaine/transports/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/timkpaine/transports/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/timkpaine/transports/branch/main/graph/badge.svg)](https://codecov.io/gh/timkpaine/transports)
-[![PyPI](https://img.shields.io/pypi/l/transports.svg)](https://pypi.python.org/pypi/transports)
+[![License](https://img.shields.io/github/license/timkpaine/transports)](https://github.com/timkpaine/transports)
 [![PyPI](https://img.shields.io/pypi/v/transports.svg)](https://pypi.python.org/pypi/transports)
 <!-- [![npm](https://img.shields.io/npm/v/transports.svg)](https://www.npmjs.com/package/transports) -->
```

### Comparing `transports-0.1.1/pyproject.toml` & `transports-0.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["maturin>=0.13,<0.14"]
 build-backend = "maturin"
 
 [project]
 name = "transports"
 authors = [{name = "Tim Paine", email = "t.paine154@gmail.com"}]
 description="Generic communication library"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
@@ -22,14 +22,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 keywords = []
 dependencies = [
     "aiohttp",
     "aiostream",
+    "bigbrother",
     "orjson",
     "pydantic",
     "starlette",
     "udatetime",
     "uvicorn",
     "websockets",
 ]
```

### Comparing `transports-0.1.1/transports/__init__.py` & `transports-0.1.2/transports/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     # handlers
     StarletteWebSocketServer,
     # clients
     AioHttpWebSocketClient,
 )
 
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 
 __all__ = [
     "__version__",
     "BaseModel",
     "Field",
     "PrivateAttr",
```

### Comparing `transports-0.1.1/transports/client.py` & `transports-0.1.2/transports/client.py`

 * *Files identical despite different names*

### Comparing `transports-0.1.1/transports/connection.py` & `transports-0.1.2/transports/connection.py`

 * *Files identical despite different names*

### Comparing `transports-0.1.1/transports/handlers/aiohttp_client.py` & `transports-0.1.2/transports/handlers/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `transports-0.1.1/transports/handlers/starlette.py` & `transports-0.1.2/transports/handlers/starlette.py`

 * *Files identical despite different names*

### Comparing `transports-0.1.1/transports/json.py` & `transports-0.1.2/transports/json.py`

 * *Files identical despite different names*

### Comparing `transports-0.1.1/transports/model.py` & `transports-0.1.2/transports/model.py`

 * *Files identical despite different names*

### Comparing `transports-0.1.1/transports/server.py` & `transports-0.1.2/transports/server.py`

 * *Files identical despite different names*

### Comparing `transports-0.1.1/transports/tests/test_transport.py` & `transports-0.1.2/transports/tests/test_transport.py`

 * *Files identical despite different names*

### Comparing `transports-0.1.1/transports/transport.py` & `transports-0.1.2/transports/transport.py`

 * *Files identical despite different names*

### Comparing `transports-0.1.1/transports/update.py` & `transports-0.1.2/transports/update.py`

 * *Files identical despite different names*

### Comparing `transports-0.1.1/Cargo.lock` & `transports-0.1.2/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -65,17 +65,17 @@
 dependencies = [
  "termcolor",
  "unicode-width",
 ]
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.3"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
+checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "ctor"
 version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d2301688392eb071b0bf1a37be05c469d3cc4dbbd95df672fe28ab021e6a096"
 dependencies = [
@@ -103,15 +103,15 @@
 dependencies = [
  "cc",
  "codespan-reporting",
  "once_cell",
  "proc-macro2",
  "quote",
  "scratch",
- "syn 2.0.12",
+ "syn 2.0.13",
 ]
 
 [[package]]
 name = "cxxbridge-flags"
 version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7944172ae7e4068c533afbb984114a56c46e9ccddda550499caa222902c7f7bb"
@@ -120,33 +120,33 @@
 name = "cxxbridge-macro"
 version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2345488264226bf682893e25de0769f3360aac9957980ec49361b083ddaa5bc5"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.12",
+ "syn 2.0.13",
 ]
 
 [[package]]
 name = "ghost"
 version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e77ac7b51b8e6313251737fcef4b1c01a2ea102bde68415b62c0ee9268fec357"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.12",
+ "syn 2.0.13",
 ]
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.54"
+version = "0.1.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c17cc76786e99f8d2f055c11159e7f0091c42474dcc3189fbab96072e873e6d"
+checksum = "0722cd7114b7de04316e7ea5456a0bbb20e4adb46fd27a3697adb812cff0f37c"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
  "windows",
@@ -191,17 +191,17 @@
 checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.141"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
 
 [[package]]
 name = "link-cplusplus"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
 dependencies = [
@@ -330,17 +330,17 @@
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.54"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e472a104799c74b514a57226160104aa483546de37e839ec50e3c2e41dd87534"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.16.6"
@@ -450,15 +450,15 @@
 name = "serde_derive"
 version = "1.0.159"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c614d17805b093df4b147b51339e7e44bf05ef59fba1e45d83500bcfb4d8585"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.12",
+ "syn 2.0.13",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d721eca97ac802aa7777b701877c8004d950fc142651367300d21c1cc0194744"
@@ -483,17 +483,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.12"
+version = "2.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "79d9531f94112cfc3e4c8f5f02cb2b58f72c97b7efd85f70203cc6d8efda5927"
+checksum = "4c9da457c5285ac1f936ebd076af6dac17a61cfe7826f2076b4d015cf47bc8ec"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -520,15 +520,15 @@
  "libc",
  "wasi",
  "winapi",
 ]
 
 [[package]]
 name = "transports"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "chrono",
  "num",
  "serde",
  "serde_json",
 ]
 
@@ -647,79 +647,136 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows"
-version = "0.46.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cdacb41e6a96a052c6cb63a144f24900236121c6f63f4f8219fef5977ecb0c25"
+checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.42.2",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+dependencies = [
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+
+[[package]]
 name = "windows_aarch64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
+
+[[package]]
 name = "windows_i686_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+
+[[package]]
 name = "windows_i686_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
+
+[[package]]
 name = "windows_x86_64_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+
+[[package]]
 name = "windows_x86_64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+
+[[package]]
+name = "windows_x86_64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `transports-0.1.1/PKG-INFO` & `transports-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 Metadata-Version: 2.1
 Name: transports
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp
 Requires-Dist: aiostream
+Requires-Dist: bigbrother
 Requires-Dist: orjson
 Requires-Dist: pydantic
 Requires-Dist: starlette
 Requires-Dist: udatetime
 Requires-Dist: uvicorn
 Requires-Dist: websockets
-Requires-Dist: pytest; extra == 'test'
-Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: black>=23; extra == 'develop'
 Requires-Dist: bump2version; extra == 'develop'
 Requires-Dist: check-manifest; extra == 'develop'
 Requires-Dist: maturin; extra == 'develop'
 Requires-Dist: pytest; extra == 'develop'
 Requires-Dist: pytest-cov; extra == 'develop'
 Requires-Dist: ruff; extra == 'develop'
 Requires-Dist: semgrep; extra == 'develop'
 Requires-Dist: twine; extra == 'develop'
 Requires-Dist: wheel; extra == 'develop'
-Provides-Extra: test
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
 Provides-Extra: develop
+Provides-Extra: test
 License-File: LICENSE
 Summary: Generic communication library
 Keywords: 
 Author-email: Tim Paine <t.paine154@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: repository, https://github.com/timkpaine/transports
 Project-URL: homepage, https://github.com/timkpaine/transports
+Project-URL: repository, https://github.com/timkpaine/transports
 
 # transports
 Generic communication library
 
 [![Build Status](https://github.com/timkpaine/transports/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/timkpaine/transports/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/timkpaine/transports/branch/main/graph/badge.svg)](https://codecov.io/gh/timkpaine/transports)
-[![PyPI](https://img.shields.io/pypi/l/transports.svg)](https://pypi.python.org/pypi/transports)
+[![License](https://img.shields.io/github/license/timkpaine/transports)](https://github.com/timkpaine/transports)
 [![PyPI](https://img.shields.io/pypi/v/transports.svg)](https://pypi.python.org/pypi/transports)
 <!-- [![npm](https://img.shields.io/npm/v/transports.svg)](https://www.npmjs.com/package/transports) -->
```

