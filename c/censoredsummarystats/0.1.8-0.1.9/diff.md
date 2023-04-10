# Comparing `tmp/censoredsummarystats-0.1.8.tar.gz` & `tmp/censoredsummarystats-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censoredsummarystats-0.1.8.tar", max compression
+gzip compressed data, was "censoredsummarystats-0.1.9.tar", max compression
```

## Comparing `censoredsummarystats-0.1.8.tar` & `censoredsummarystats-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      588 2023-04-10 04:15:16.014879 censoredsummarystats-0.1.8/censoredsummarystats/__init__.py
--rw-r--r--   0        0        0    52645 2023-04-09 06:25:41.657236 censoredsummarystats-0.1.8/censoredsummarystats/censoredsummarystats.py
--rw-r--r--   0        0        0    11558 2023-03-12 00:39:53.769556 censoredsummarystats-0.1.8/LICENSE
--rw-r--r--   0        0        0      534 2023-04-10 04:16:51.797277 censoredsummarystats-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      112 2023-03-12 00:39:53.771555 censoredsummarystats-0.1.8/README.md
--rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 censoredsummarystats-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      588 2023-04-10 04:15:16.014879 censoredsummarystats-0.1.9/censoredsummarystats/__init__.py
+-rw-r--r--   0        0        0    52645 2023-04-09 06:25:41.657236 censoredsummarystats-0.1.9/censoredsummarystats/censoredsummarystats.py
+-rw-r--r--   0        0        0    11558 2023-03-12 00:39:53.769556 censoredsummarystats-0.1.9/LICENSE
+-rw-r--r--   0        0        0      534 2023-04-10 04:33:32.221568 censoredsummarystats-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-03-12 00:39:53.771555 censoredsummarystats-0.1.9/README.md
+-rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 censoredsummarystats-0.1.9/PKG-INFO
```

### Comparing `censoredsummarystats-0.1.8/censoredsummarystats/__init__.py` & `censoredsummarystats-0.1.9/censoredsummarystats/__init__.py`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.1.8/censoredsummarystats/censoredsummarystats.py` & `censoredsummarystats-0.1.9/censoredsummarystats/censoredsummarystats.py`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.1.8/LICENSE` & `censoredsummarystats-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.1.8/pyproject.toml` & `censoredsummarystats-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "censoredsummarystats"
-version = "0.1.8"
+version = "0.1.9"
 description = "A python package for calculating summary stats on censored data (data that contains < and > symbols)."
 authors = ["Kurt van Ness <vanness.kurt@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/kurtvanness/CensoredSummaryStats"
 packages = [{include = "censoredsummarystats"}]
 
 [tool.poetry.dependencies]
```

### Comparing `censoredsummarystats-0.1.8/PKG-INFO` & `censoredsummarystats-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censoredsummarystats
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python package for calculating summary stats on censored data (data that contains < and > symbols).
 Home-page: https://github.com/kurtvanness/CensoredSummaryStats
 Author: Kurt van Ness
 Author-email: vanness.kurt@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

