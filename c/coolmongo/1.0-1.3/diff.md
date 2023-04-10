# Comparing `tmp/coolmongo-1.0.tar.gz` & `tmp/coolmongo-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolmongo-1.0.tar", last modified: Thu Mar 16 14:45:54 2023, max compression
+gzip compressed data, was "coolmongo-1.3.tar", last modified: Mon Apr 10 14:25:12 2023, max compression
```

## Comparing `coolmongo-1.0.tar` & `coolmongo-1.3.tar`

### file list

```diff
@@ -1,9 +1,5 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmongo-1.0/LICENSE
--rw-r--r--   0        0        0    11357 2022-11-17 21:35:25.000000 coolmongo-1.0/Licenses of dependent packages/pymongo-LICENSE
--rw-r--r--   0        0        0     6269 2023-03-15 17:16:31.975165 coolmongo-1.0/README.md
--rw-r--r--   0        0        0       24 2022-11-24 13:50:36.000000 coolmongo-1.0/__init__.py
--rw-r--r--   0        0        0      147 2023-02-25 07:43:51.350884 coolmongo-1.0/coolmongo/__init__.py
--rw-r--r--   0        0        0    20928 2023-03-09 15:03:44.333455 coolmongo-1.0/coolmongo/_coolmongo.py
--rw-r--r--   0        0        0      616 2023-03-15 15:26:29.929323 coolmongo-1.0/pyproject.toml
--rw-r--r--   0        0        0    12822 2023-03-12 03:59:13.692662 coolmongo-1.0/test.py
--rw-r--r--   0        0        0     6566 1970-01-01 00:00:00.000000 coolmongo-1.0/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmongo-1.3/LICENSE
+-rw-r--r--   0        0        0     5124 2023-04-09 11:28:09.647580 coolmongo-1.3/README.md
+-rw-r--r--   0        0        0       29 2023-04-10 03:54:46.072863 coolmongo-1.3/coolmongo.py
+-rw-r--r--   0        0        0      566 2023-04-10 09:20:09.279348 coolmongo-1.3/pyproject.toml
+-rw-r--r--   0        0        0     5382 1970-01-01 00:00:00.000000 coolmongo-1.3/PKG-INFO
```

### Comparing `coolmongo-1.0/LICENSE` & `coolmongo-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `coolmongo-1.0/pyproject.toml` & `coolmongo-1.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "coolmongo"
-version = "1.0"
-description = "The most elegant MongoDB ORM in history"
-dependencies = ["pymongo", "vtype"]
+version = "1.3"
+description = "史上最优雅的 MongoDB ORM"
+dependencies = ["lccpy >=1.3"]
 keywords = ["coolmongo", "pymongo", "mongodb"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
+requires-python = ">=3.7"
 
 [project.urls]
-Documentation = "https://www.yuque.com/lcctoor/lccpy/coolmongo"
-Source = "https://github.com/lcctoor/lccpy/tree/main/coolmongo"
+HomePage = "https://github.com/lcctoor/lccpy/tree/main/coolmongo"
```

