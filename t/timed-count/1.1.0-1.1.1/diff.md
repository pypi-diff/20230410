# Comparing `tmp/timed_count-1.1.0.tar.gz` & `tmp/timed_count-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timed_count-1.1.0.tar", max compression
+gzip compressed data, was "timed_count-1.1.1.tar", max compression
```

## Comparing `timed_count-1.1.0.tar` & `timed_count-1.1.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1065 2022-12-07 14:20:50.209521 timed_count-1.1.0/LICENSE
--rw-r--r--   0        0        0      953 2022-12-29 05:36:21.945442 timed_count-1.1.0/README.md
--rw-r--r--   0        0        0      557 2023-01-06 06:48:12.870545 timed_count-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      134 2022-12-25 10:13:46.883006 timed_count-1.1.0/timed_count/__init__.py
--rw-r--r--   0        0        0     1891 2023-01-06 01:54:34.515018 timed_count-1.1.0/timed_count/cls_timed_count.py
--rw-r--r--   0        0        0     2042 2023-01-06 06:47:08.308334 timed_count-1.1.0/timed_count/timed_count.py
--rw-r--r--   0        0        0     1751 1970-01-01 00:00:00.000000 timed_count-1.1.0/setup.py
--rw-r--r--   0        0        0     1499 1970-01-01 00:00:00.000000 timed_count-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-02-19 06:15:52.878047 timed_count-1.1.1/LICENSE
+-rw-r--r--   0        0        0      953 2023-02-19 06:15:52.878175 timed_count-1.1.1/README.md
+-rw-r--r--   0        0        0      556 2023-04-10 10:35:27.532291 timed_count-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-02-19 06:15:52.879102 timed_count-1.1.1/timed_count/__init__.py
+-rw-r--r--   0        0        0     1891 2023-02-19 06:15:52.879222 timed_count-1.1.1/timed_count/cls_timed_count.py
+-rw-r--r--   0        0        0     2096 2023-04-10 10:30:31.178847 timed_count-1.1.1/timed_count/timed_count.py
+-rw-r--r--   0        0        0     1648 1970-01-01 00:00:00.000000 timed_count-1.1.1/PKG-INFO
```

### Comparing `timed_count-1.1.0/LICENSE` & `timed_count-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `timed_count-1.1.0/README.md` & `timed_count-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `timed_count-1.1.0/pyproject.toml` & `timed_count-1.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "timed-count"
-version = "1.1.0"
+version = "1.1.1"
 description = "timed-count provides an iterator that delays each iteration by a specified time period. It can be used to repeatedly execute code at a precise frequency."
 authors = ["morefigs"]
 homepage = "https://github.com/morefigs/timed-count"
 readme = "README.md"
 packages = [{include = "timed_count"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
-stoppy = "^1.0.4"
+python = "^3.7"
+stoppy = "^1.0.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `timed_count-1.1.0/timed_count/cls_timed_count.py` & `timed_count-1.1.1/timed_count/cls_timed_count.py`

 * *Files identical despite different names*

### Comparing `timed_count-1.1.0/timed_count/timed_count.py` & `timed_count-1.1.1/timed_count/timed_count.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,13 +39,15 @@
 
             count = period * index
 
             # Starts the stopwatch on first call, so first call returns exactly 0
             time_ready = stopwatch.time(True)
 
             # Block the iteration until the next count time
-            while (time := stopwatch.time()) < count:
+            time = stopwatch.time()
+            while time < count:
                 sleep(temporal_resolution)
+                time = stopwatch.time()
 
             yield TimedCount(index, count, time, time_ready, count_dp, time_dp)
 
             index += 1
```

### Comparing `timed_count-1.1.0/PKG-INFO` & `timed_count-1.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: timed-count
-Version: 1.1.0
+Version: 1.1.1
 Summary: timed-count provides an iterator that delays each iteration by a specified time period. It can be used to repeatedly execute code at a precise frequency.
 Home-page: https://github.com/morefigs/timed-count
 Author: morefigs
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: stoppy (>=1.0.4,<2.0.0)
+Requires-Dist: stoppy (>=1.0.5,<2.0.0)
 Description-Content-Type: text/markdown
 
 # timed-count
 
 **timed-count** provides an iterator that delays each iteration by a specified time period. It can be used to repeatedly  execute code at a precise frequency.
 
 **timed-count** is a good replacement for a loop that contains a call to `time.sleep`. It is precise, does not dependent on the loop execution time, and won't accumulate temporal drift.
```

