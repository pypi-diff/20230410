# Comparing `tmp/pure_math-0.0.1.tar.gz` & `tmp/pure_math-0.0.2.tar.gz`

## Comparing `pure_math-0.0.1.tar` & `pure_math-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,6 @@
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 pure_math-0.0.1/LICENSE
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pure_math-0.0.1/README.md
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 pure_math-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 pure_math-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pure_math-0.0.2/src/pure_math/__init__.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pure_math-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 pure_math-0.0.2/LICENSE
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pure_math-0.0.2/README.md
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 pure_math-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 pure_math-0.0.2/PKG-INFO
```

### Comparing `pure_math-0.0.1/LICENSE` & `pure_math-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_math-0.0.1/pyproject.toml` & `pure_math-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pure_math"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="deerawj", email="deerawj@gmail.com" },
 ]
 description = "pure python implementation of the standard math library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pure_math-0.0.1/PKG-INFO` & `pure_math-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure_math
-Version: 0.0.1
+Version: 0.0.2
 Summary: pure python implementation of the standard math library
 Project-URL: Homepage, https://github.com/deerawj/pure_math
 Author-email: deerawj <deerawj@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

