# Comparing `tmp/retry_extended-0.1.1.tar.gz` & `tmp/retry_extended-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retry_extended-0.1.1.tar", max compression
+gzip compressed data, was "retry_extended-0.2.0.tar", max compression
```

## Comparing `retry_extended-0.1.1.tar` & `retry_extended-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,6 @@
--rw-r--r--   0        0        0    11357 2022-11-04 12:50:34.776502 retry_extended-0.1.1/LICENSE
--rw-r--r--   0        0        0      404 2022-11-04 12:50:34.780502 retry_extended-0.1.1/README.md
--rw-r--r--   0        0        0     1080 2022-11-04 12:50:57.008622 retry_extended-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      252 2022-11-04 12:50:34.780502 retry_extended-0.1.1/retry/__init__.py
--rw-r--r--   0        0        0     4632 2022-11-04 12:50:34.780502 retry_extended-0.1.1/retry/api.py
--rw-r--r--   0        0        0      660 2022-11-04 12:50:34.780502 retry_extended-0.1.1/retry/compat.py
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 retry_extended-0.1.1/setup.py
--rw-r--r--   0        0        0     1601 1970-01-01 00:00:00.000000 retry_extended-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-10 18:28:57.429966 retry_extended-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1219 2023-04-10 18:28:57.429966 retry_extended-0.2.0/README.md
+-rw-r--r--   0        0        0     1172 2023-04-10 18:28:57.429966 retry_extended-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      252 2023-04-10 18:28:57.429966 retry_extended-0.2.0/retry/__init__.py
+-rw-r--r--   0        0        0     7264 2023-04-10 18:28:57.429966 retry_extended-0.2.0/retry/api.py
+-rw-r--r--   0        0        0     2416 1970-01-01 00:00:00.000000 retry_extended-0.2.0/PKG-INFO
```

### Comparing `retry_extended-0.1.1/LICENSE` & `retry_extended-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `retry_extended-0.1.1/pyproject.toml` & `retry_extended-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "retry-extended"
-version = "0.1.1"
+version = "0.2.0"
 description = "Retry API compatible extended library"
 authors = ["Strollby Developers <backend.developers@strollby.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/strollby/retry-extended"
 repository = "https://github.com/strollby/retry-extended"
 documentation = "https://github.com/strollby/retry-extended"
@@ -35,7 +35,15 @@
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+
+[tool.black]
+line-length = 120
+target-version = ['py311']
+
+[tool.isort]
+profile = "black"
```

