# Comparing `tmp/dtumathtools-1.0.3.tar.gz` & `tmp/dtumathtools-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtumathtools-1.0.3.tar", last modified: Sun Mar 19 14:11:50 2023, max compression
+gzip compressed data, was "dtumathtools-1.0.4.tar", last modified: Mon Apr 10 14:20:52 2023, max compression
```

## Comparing `dtumathtools-1.0.3.tar` & `dtumathtools-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-03-19 14:11:50.753266 dtumathtools-1.0.3/
--rw-rw-rw-   0        0        0     1471 2023-01-29 21:40:49.000000 dtumathtools-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     3541 2023-03-19 14:11:50.752264 dtumathtools-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2635 2023-01-29 21:46:36.000000 dtumathtools-1.0.3/README.md
--rw-rw-rw-   0        0        0     1162 2023-03-19 12:19:26.000000 dtumathtools-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-19 14:11:50.754264 dtumathtools-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-19 14:11:50.698384 dtumathtools-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-03-19 14:11:50.713348 dtumathtools-1.0.3/src/dtumathtools/
--rw-rw-rw-   0        0        0       84 2023-01-30 09:29:20.000000 dtumathtools-1.0.3/src/dtumathtools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:11:50.743267 dtumathtools-1.0.3/src/dtumathtools/dtuplot/
--rw-rw-rw-   0        0        0      162 2023-03-19 12:43:03.000000 dtumathtools-1.0.3/src/dtumathtools/dtuplot/__init__.py
--rw-rw-rw-   0        0        0     6322 2022-12-23 22:17:04.000000 dtumathtools-1.0.3/src/dtumathtools/dtuplot/quiverplot.py
--rw-rw-rw-   0        0        0     2643 2022-12-23 23:07:43.000000 dtumathtools-1.0.3/src/dtumathtools/dtuplot/scatterplot.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:11:50.745267 dtumathtools-1.0.3/src/dtumathtools/dtutools/
--rw-rw-rw-   0        0        0       56 2023-01-30 09:30:16.000000 dtumathtools-1.0.3/src/dtumathtools/dtutools/__init__.py
--rw-rw-rw-   0        0        0     1891 2023-03-19 12:10:52.000000 dtumathtools-1.0.3/src/dtumathtools/dtutools/helpers.py
-drwxrwxrwx   0        0        0        0 2023-03-19 14:11:50.738267 dtumathtools-1.0.3/src/dtumathtools.egg-info/
--rw-rw-rw-   0        0        0     3541 2023-03-19 14:11:50.000000 dtumathtools-1.0.3/src/dtumathtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-03-19 14:11:50.000000 dtumathtools-1.0.3/src/dtumathtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-19 14:11:50.000000 dtumathtools-1.0.3/src/dtumathtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-03-19 14:11:50.000000 dtumathtools-1.0.3/src/dtumathtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-19 14:11:50.000000 dtumathtools-1.0.3/src/dtumathtools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-19 14:11:50.751266 dtumathtools-1.0.3/tests/
--rw-rw-rw-   0        0        0        0 2023-03-19 12:45:23.000000 dtumathtools-1.0.3/tests/test_dtuplot.py
--rw-rw-rw-   0        0        0     1802 2023-03-19 14:08:01.000000 dtumathtools-1.0.3/tests/test_dtutools.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:20:52.551698 dtumathtools-1.0.4/
+-rw-rw-rw-   0        0        0     1471 2023-01-29 21:40:49.000000 dtumathtools-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3541 2023-04-10 14:20:52.550698 dtumathtools-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2635 2023-01-29 21:46:36.000000 dtumathtools-1.0.4/README.md
+-rw-rw-rw-   0        0        0     1162 2023-04-10 14:05:44.000000 dtumathtools-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-10 14:20:52.551698 dtumathtools-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-10 14:20:52.500700 dtumathtools-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-10 14:20:52.513696 dtumathtools-1.0.4/src/dtumathtools/
+-rw-rw-rw-   0        0        0       84 2023-01-30 09:29:20.000000 dtumathtools-1.0.4/src/dtumathtools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:20:52.541695 dtumathtools-1.0.4/src/dtumathtools/dtuplot/
+-rw-rw-rw-   0        0        0      162 2023-03-19 12:43:03.000000 dtumathtools-1.0.4/src/dtumathtools/dtuplot/__init__.py
+-rw-rw-rw-   0        0        0     6322 2022-12-23 22:17:04.000000 dtumathtools-1.0.4/src/dtumathtools/dtuplot/quiverplot.py
+-rw-rw-rw-   0        0        0     2643 2022-12-23 23:07:43.000000 dtumathtools-1.0.4/src/dtumathtools/dtuplot/scatterplot.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:20:52.546699 dtumathtools-1.0.4/src/dtumathtools/dtutools/
+-rw-rw-rw-   0        0        0       73 2023-04-10 14:03:03.000000 dtumathtools-1.0.4/src/dtumathtools/dtutools/__init__.py
+-rw-rw-rw-   0        0        0     3091 2023-04-10 14:15:11.000000 dtumathtools-1.0.4/src/dtumathtools/dtutools/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:20:52.536710 dtumathtools-1.0.4/src/dtumathtools.egg-info/
+-rw-rw-rw-   0        0        0     3541 2023-04-10 14:20:52.000000 dtumathtools-1.0.4/src/dtumathtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2023-04-10 14:20:52.000000 dtumathtools-1.0.4/src/dtumathtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 14:20:52.000000 dtumathtools-1.0.4/src/dtumathtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-04-10 14:20:52.000000 dtumathtools-1.0.4/src/dtumathtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-10 14:20:52.000000 dtumathtools-1.0.4/src/dtumathtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 14:20:52.548696 dtumathtools-1.0.4/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-10 14:01:29.000000 dtumathtools-1.0.4/tests/test_dtuplot.py
+-rw-rw-rw-   0        0        0     1802 2023-03-19 14:08:01.000000 dtumathtools-1.0.4/tests/test_dtutools.py
```

### Comparing `dtumathtools-1.0.3/LICENSE` & `dtumathtools-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dtumathtools-1.0.3/PKG-INFO` & `dtumathtools-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtumathtools
-Version: 1.0.3
+Version: 1.0.4
 Summary: A plotting package for the 01005 Mathematics 1 course at the Technical University of Denmark
 Author-email: Christian Mikkelstrup <s194345@student.dtu.dk>, Hans Henrik Hermansen <s194042@student.dtu.dk>
 License: BSD License (BSD)
 Project-URL: Homepage, https://github.com/Chrillebon/DTUMathTools
 Project-URL: Mathematics 1 homepage, https://01005.compute.dtu.dk/
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dtumathtools-1.0.3/README.md` & `dtumathtools-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dtumathtools-1.0.3/pyproject.toml` & `dtumathtools-1.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dtumathtools"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
     {name = "Christian Mikkelstrup", email = "s194345@student.dtu.dk"},
     {name = "Hans Henrik Hermansen", email = "s194042@student.dtu.dk"},
 ]
 description = "A plotting package for the 01005 Mathematics 1 course at the Technical University of Denmark"
 readme = "README.md"
 license = {'text' = "BSD License (BSD)"}
```

### Comparing `dtumathtools-1.0.3/src/dtumathtools/dtuplot/quiverplot.py` & `dtumathtools-1.0.4/src/dtumathtools/dtuplot/quiverplot.py`

 * *Files identical despite different names*

### Comparing `dtumathtools-1.0.3/src/dtumathtools/dtuplot/scatterplot.py` & `dtumathtools-1.0.4/src/dtumathtools/dtuplot/scatterplot.py`

 * *Files identical despite different names*

### Comparing `dtumathtools-1.0.3/src/dtumathtools/dtutools/helpers.py` & `dtumathtools-1.0.4/src/dtumathtools/dtutools/helpers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sympy import *
 from functools import reduce
-
+from typing import Union
 
 def _extract_vars(expr):
     return [e[1] for e in sorted(list(map(lambda x: (str(x),x), expr.free_symbols)))]
 
 
 def taylor(expr, vars, degree):
     if len(vars) != 2 and len(vars) != 4:
@@ -62,7 +62,41 @@
     return Matrix(
         [
             V[2].diff(var[1]) - V[1].diff(var[2]),
             V[0].diff(var[2]) - V[2].diff(var[0]),
             V[1].diff(var[0]) - V[0].diff(var[1]),
         ]
     )
+
+
+def dsolve(ODE: Union[Eq, list, Matrix], ics=None) -> dict:
+    """ A wrapper for the sympy dsolve-function. Instead of a list of equations
+        denoting the solution, this function returns a dictionary of solutions.
+
+        // This makes it easier to substitute solution in the places it's needed
+
+        ## Input:
+            ODE: one or multiple differential equations to be solved by sympy
+
+        ## Returns:
+            sol: a dictionary containing solutions to 'ODE'
+        
+    """
+    
+    # Common problem for people is making an single equation, but with both sides
+    # being Matrices. This alleviates that issue, and lets users think less
+    if type(ODE) == Eq and type(ODE.lhs) == type(ODE.rhs) == Matrix:
+            sol = dsolve(ODE.lhs - ODE.rhs, ics=ics)
+    else:
+        sol = dsolve(ODE, ics=ics)
+
+    return {eq.lhs : eq.rhs for eq in sol}
+
+
+def l2_norm( v: Matrix ):
+    """ Computes the l2-norm for a Matrix-class object, without using
+        absolute values on entries, for easier simplification and integration
+
+        ## Input:
+            v: A sympy Matrix
+    """
+    return sqrt(sum(x**2 for x in v))
```

### Comparing `dtumathtools-1.0.3/src/dtumathtools.egg-info/PKG-INFO` & `dtumathtools-1.0.4/src/dtumathtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtumathtools
-Version: 1.0.3
+Version: 1.0.4
 Summary: A plotting package for the 01005 Mathematics 1 course at the Technical University of Denmark
 Author-email: Christian Mikkelstrup <s194345@student.dtu.dk>, Hans Henrik Hermansen <s194042@student.dtu.dk>
 License: BSD License (BSD)
 Project-URL: Homepage, https://github.com/Chrillebon/DTUMathTools
 Project-URL: Mathematics 1 homepage, https://01005.compute.dtu.dk/
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dtumathtools-1.0.3/tests/test_dtutools.py` & `dtumathtools-1.0.4/tests/test_dtutools.py`

 * *Files identical despite different names*

