# Comparing `tmp/best-sort-0.0.5.tar.gz` & `tmp/best-sort-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "best-sort-0.0.5.tar", last modified: Fri Mar 31 02:25:17 2023, max compression
+gzip compressed data, was "best-sort-0.0.6.tar", last modified: Mon Apr 10 05:03:38 2023, max compression
```

## Comparing `best-sort-0.0.5.tar` & `best-sort-0.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      130 2023-03-17 22:46:27.922581 best-sort-0.0.5/README.md
--rw-r--r--   0        0        0      722 2023-03-31 02:24:13.575453 best-sort-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       25 2023-03-18 04:22:23.338540 best-sort-0.0.5/src/best_sort/__init__.py
--rw-r--r--   0        0        0       60 2023-03-31 01:47:42.618759 best-sort-0.0.5/src/best_sort/sort_algos/__init__.py
--rw-r--r--   0        0        0     1060 2023-03-23 02:30:20.768607 best-sort-0.0.5/src/best_sort/sort_algos/bubble_sort.py
--rw-r--r--   0        0        0     1086 2023-03-31 02:22:50.498076 best-sort-0.0.5/src/best_sort/sort_algos/insertion_sort.py
--rw-r--r--   0        0        0     1017 2023-03-18 01:53:58.571909 best-sort-0.0.5/src/best_sort/sort_algos/selection_sort.py
--rw-r--r--   0        0        0      752 1970-01-01 00:00:00.000000 best-sort-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      130 2023-03-17 22:46:27.922581 best-sort-0.0.6/README.md
+-rw-r--r--   0        0        0      722 2023-04-10 04:40:05.083403 best-sort-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       25 2023-03-18 04:22:23.338540 best-sort-0.0.6/src/best_sort/__init__.py
+-rw-r--r--   0        0        0       62 2023-04-09 18:27:39.497791 best-sort-0.0.6/src/best_sort/sort_algos/__init__.py
+-rw-r--r--   0        0        0     1060 2023-03-23 02:30:20.768607 best-sort-0.0.6/src/best_sort/sort_algos/bubble_sort.py
+-rw-r--r--   0        0        0     1086 2023-03-31 02:22:50.498076 best-sort-0.0.6/src/best_sort/sort_algos/insertion_sort.py
+-rw-r--r--   0        0        0     1017 2023-04-06 00:41:43.248019 best-sort-0.0.6/src/best_sort/sort_algos/selection_sort.py
+-rw-r--r--   0        0        0      752 1970-01-01 00:00:00.000000 best-sort-0.0.6/PKG-INFO
```

### Comparing `best-sort-0.0.5/pyproject.toml` & `best-sort-0.0.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "best-sort"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Joey Wheeler", email="joewheeler2048@gmail.com" },
 ]
 description = "A package to find the best sorting algorithm for given data."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `best-sort-0.0.5/src/best_sort/sort_algos/bubble_sort.py` & `best-sort-0.0.6/src/best_sort/sort_algos/bubble_sort.py`

 * *Files identical despite different names*

### Comparing `best-sort-0.0.5/src/best_sort/sort_algos/insertion_sort.py` & `best-sort-0.0.6/src/best_sort/sort_algos/insertion_sort.py`

 * *Files identical despite different names*

### Comparing `best-sort-0.0.5/src/best_sort/sort_algos/selection_sort.py` & `best-sort-0.0.6/src/best_sort/sort_algos/selection_sort.py`

 * *Files identical despite different names*

### Comparing `best-sort-0.0.5/PKG-INFO` & `best-sort-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: best-sort
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package to find the best sorting algorithm for given data.
 Keywords: sorting algorithm,sorting,best algorithm
 Author-email: Joey Wheeler <joewheeler2048@gmail.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

