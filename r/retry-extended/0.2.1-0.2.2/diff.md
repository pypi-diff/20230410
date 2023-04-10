# Comparing `tmp/retry_extended-0.2.1.tar.gz` & `tmp/retry_extended-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retry_extended-0.2.1.tar", max compression
+gzip compressed data, was "retry_extended-0.2.2.tar", max compression
```

## Comparing `retry_extended-0.2.1.tar` & `retry_extended-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-04-10 19:08:56.975862 retry_extended-0.2.1/LICENSE
--rw-r--r--   0        0        0     1232 2023-04-10 19:08:56.975862 retry_extended-0.2.1/README.md
--rw-r--r--   0        0        0     1172 2023-04-10 19:09:11.368620 retry_extended-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      252 2023-04-10 19:08:56.975862 retry_extended-0.2.1/retry/__init__.py
--rw-r--r--   0        0        0     7280 2023-04-10 19:08:56.975862 retry_extended-0.2.1/retry/api.py
--rw-r--r--   0        0        0     2429 1970-01-01 00:00:00.000000 retry_extended-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-10 19:27:09.510070 retry_extended-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1232 2023-04-10 19:27:09.510070 retry_extended-0.2.2/README.md
+-rw-r--r--   0        0        0     1172 2023-04-10 19:27:09.510070 retry_extended-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      252 2023-04-10 19:27:09.510070 retry_extended-0.2.2/retry/__init__.py
+-rw-r--r--   0        0        0     7280 2023-04-10 19:27:09.510070 retry_extended-0.2.2/retry/api.py
+-rw-r--r--   0        0        0     2429 1970-01-01 00:00:00.000000 retry_extended-0.2.2/PKG-INFO
```

### Comparing `retry_extended-0.2.1/LICENSE` & `retry_extended-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `retry_extended-0.2.1/README.md` & `retry_extended-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `retry_extended-0.2.1/pyproject.toml` & `retry_extended-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "retry-extended"
-version = "0.2.1"
+version = "0.2.2"
 description = "Retry API compatible extended library"
 authors = ["Strollby Developers <backend.developers@strollby.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/strollby/retry-extended"
 repository = "https://github.com/strollby/retry-extended"
 documentation = "https://github.com/strollby/retry-extended"
```

### Comparing `retry_extended-0.2.1/retry/api.py` & `retry_extended-0.2.2/retry/api.py`

 * *Files identical despite different names*

### Comparing `retry_extended-0.2.1/PKG-INFO` & `retry_extended-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retry-extended
-Version: 0.2.1
+Version: 0.2.2
 Summary: Retry API compatible extended library
 Home-page: https://github.com/strollby/retry-extended
 License: Apache-2.0
 Keywords: retry,retry-extended,python-retry
 Author: Strollby Developers
 Author-email: backend.developers@strollby.com
 Requires-Python: >=3.7,<4.0
```

