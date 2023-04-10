# Comparing `tmp/flake8_functions-0.0.7.tar.gz` & `tmp/flake8_functions-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_functions-0.0.7.tar", last modified: Thu Feb 24 10:34:10 2022, max compression
+gzip compressed data, was "flake8_functions-0.0.8.tar", last modified: Mon Apr 10 15:53:13 2023, max compression
```

## Comparing `flake8_functions-0.0.7.tar` & `flake8_functions-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 10:34:10.479140 flake8_functions-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-02-24 10:33:51.000000 flake8_functions-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4322 2022-02-24 10:34:10.479140 flake8_functions-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3382 2022-02-24 10:33:51.000000 flake8_functions-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 10:34:10.479140 flake8_functions-0.0.7/flake8_functions/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-02-24 10:33:51.000000 flake8_functions-0.0.7/flake8_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2795 2022-02-24 10:33:51.000000 flake8_functions-0.0.7/flake8_functions/checker.py
--rw-r--r--   0 runner    (1001) docker     (121)      854 2022-02-24 10:33:51.000000 flake8_functions-0.0.7/flake8_functions/function_arguments_amount.py
--rw-r--r--   0 runner    (1001) docker     (121)     1350 2022-02-24 10:33:51.000000 flake8_functions-0.0.7/flake8_functions/function_lenght.py
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-02-24 10:33:51.000000 flake8_functions-0.0.7/flake8_functions/function_purity.py
--rw-r--r--   0 runner    (1001) docker     (121)      864 2022-02-24 10:33:51.000000 flake8_functions-0.0.7/flake8_functions/function_returns_amount.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 10:34:10.479140 flake8_functions-0.0.7/flake8_functions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4322 2022-02-24 10:34:10.000000 flake8_functions-0.0.7/flake8_functions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-02-24 10:34:10.000000 flake8_functions-0.0.7/flake8_functions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-24 10:34:10.000000 flake8_functions-0.0.7/flake8_functions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-02-24 10:34:10.000000 flake8_functions-0.0.7/flake8_functions.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-24 10:34:10.000000 flake8_functions-0.0.7/flake8_functions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-02-24 10:34:10.000000 flake8_functions-0.0.7/flake8_functions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-02-24 10:34:10.000000 flake8_functions-0.0.7/flake8_functions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      571 2022-02-24 10:34:10.479140 flake8_functions-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1744 2022-02-24 10:33:51.000000 flake8_functions-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:53:13.846435 flake8_functions-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-10 15:52:47.000000 flake8_functions-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-10 15:53:13.846435 flake8_functions-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-04-10 15:52:47.000000 flake8_functions-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:53:13.842435 flake8_functions-0.0.8/flake8_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 15:52:47.000000 flake8_functions-0.0.8/flake8_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-10 15:52:47.000000 flake8_functions-0.0.8/flake8_functions/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-10 15:52:47.000000 flake8_functions-0.0.8/flake8_functions/function_arguments_amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-10 15:52:47.000000 flake8_functions-0.0.8/flake8_functions/function_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-10 15:52:47.000000 flake8_functions-0.0.8/flake8_functions/function_purity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-10 15:52:47.000000 flake8_functions-0.0.8/flake8_functions/function_returns_amount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:53:13.846435 flake8_functions-0.0.8/flake8_functions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-10 15:53:13.000000 flake8_functions-0.0.8/flake8_functions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-10 15:53:13.000000 flake8_functions-0.0.8/flake8_functions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:53:13.000000 flake8_functions-0.0.8/flake8_functions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-10 15:53:13.000000 flake8_functions-0.0.8/flake8_functions.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:53:13.000000 flake8_functions-0.0.8/flake8_functions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-10 15:53:13.000000 flake8_functions-0.0.8/flake8_functions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-10 15:53:13.000000 flake8_functions-0.0.8/flake8_functions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-10 15:53:13.846435 flake8_functions-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-10 15:52:47.000000 flake8_functions-0.0.8/setup.py
```

### Comparing `flake8_functions-0.0.7/LICENSE` & `flake8_functions-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_functions-0.0.7/PKG-INFO` & `flake8_functions-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: flake8_functions
-Version: 0.0.7
+Version: 0.0.8
 Summary: A flake8 extension that checks functions
 Home-page: https://github.com/best-doctor/flake8-functions
 Author: Valery Pavlov
 Author-email: lerikpav@gmail.com
 License: MIT
 Keywords: flake8
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Framework :: Flake8
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Programming Language :: Python
@@ -119,9 +118,7 @@
 Here are useful tips:
 
 * You can run all checks and tests with `make check`.
   Please do it before TravisCI does.
 * We use [BestDoctor python styleguide](https://github.com/best-doctor/guides/blob/master/guides/en/python_styleguide.md).
 * We respect [Django CoC](https://www.djangoproject.com/conduct/).
   Make soft, not bullshit.
-
-
```

### Comparing `flake8_functions-0.0.7/README.md` & `flake8_functions-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `flake8_functions-0.0.7/flake8_functions/checker.py` & `flake8_functions-0.0.8/flake8_functions/checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import ast
 import functools
 from typing import Generator, Tuple, Union, List
 
 from flake8_functions import __version__ as version
 from flake8_functions.function_purity import check_purity_of_functions
-from flake8_functions.function_lenght import get_length_errors
+from flake8_functions.function_length import get_length_errors
 from flake8_functions.function_arguments_amount import get_arguments_amount_error
 from flake8_functions.function_returns_amount import get_returns_amount_error
 
 AnyFuncdef = Union[ast.FunctionDef, ast.AsyncFunctionDef]
 
 
 class FunctionChecker:
```

### Comparing `flake8_functions-0.0.7/flake8_functions/function_arguments_amount.py` & `flake8_functions-0.0.8/flake8_functions/function_arguments_amount.py`

 * *Files identical despite different names*

### Comparing `flake8_functions-0.0.7/flake8_functions/function_lenght.py` & `flake8_functions-0.0.8/flake8_functions/function_length.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     return function_last_line
 
 
 def get_length_errors(func_def: AnyFuncdef, max_function_length: int) -> Tuple[int, int, str]:
     function_start_row = get_function_start_row(func_def)
     function_last_row = get_function_last_row(func_def)
-    function_lenght = function_last_row - function_start_row + 1
-    if function_lenght > max_function_length:
+    function_length = function_last_row - function_start_row + 1
+    if function_length > max_function_length:
         return (
             func_def.lineno,
             func_def.col_offset,
-            f'CFQ001 Function {func_def.name} has length {function_lenght}'
+            f'CFQ001 Function {func_def.name} has length {function_length}'
             f' that exceeds max allowed length {max_function_length}',
         )
```

### Comparing `flake8_functions-0.0.7/flake8_functions/function_returns_amount.py` & `flake8_functions-0.0.8/flake8_functions/function_returns_amount.py`

 * *Files identical despite different names*

### Comparing `flake8_functions-0.0.7/flake8_functions.egg-info/PKG-INFO` & `flake8_functions-0.0.8/flake8_functions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: flake8-functions
-Version: 0.0.7
+Version: 0.0.8
 Summary: A flake8 extension that checks functions
 Home-page: https://github.com/best-doctor/flake8-functions
 Author: Valery Pavlov
 Author-email: lerikpav@gmail.com
 License: MIT
 Keywords: flake8
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Framework :: Flake8
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Programming Language :: Python
@@ -119,9 +118,7 @@
 Here are useful tips:
 
 * You can run all checks and tests with `make check`.
   Please do it before TravisCI does.
 * We use [BestDoctor python styleguide](https://github.com/best-doctor/guides/blob/master/guides/en/python_styleguide.md).
 * We respect [Django CoC](https://www.djangoproject.com/conduct/).
   Make soft, not bullshit.
-
-
```

### Comparing `flake8_functions-0.0.7/flake8_functions.egg-info/SOURCES.txt` & `flake8_functions-0.0.8/flake8_functions.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 flake8_functions/__init__.py
 flake8_functions/checker.py
 flake8_functions/function_arguments_amount.py
-flake8_functions/function_lenght.py
+flake8_functions/function_length.py
 flake8_functions/function_purity.py
 flake8_functions/function_returns_amount.py
 flake8_functions.egg-info/PKG-INFO
 flake8_functions.egg-info/SOURCES.txt
 flake8_functions.egg-info/dependency_links.txt
 flake8_functions.egg-info/entry_points.txt
 flake8_functions.egg-info/not-zip-safe
```

### Comparing `flake8_functions-0.0.7/setup.cfg` & `flake8_functions-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `flake8_functions-0.0.7/setup.py` & `flake8_functions-0.0.8/setup.py`

 * *Files identical despite different names*

