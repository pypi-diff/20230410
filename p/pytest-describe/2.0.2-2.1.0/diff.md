# Comparing `tmp/pytest-describe-2.0.2.tar.gz` & `tmp/pytest-describe-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-describe-2.0.2.tar", last modified: Sun Apr  9 14:53:32 2023, max compression
+gzip compressed data, was "pytest-describe-2.1.0.tar", last modified: Sun Apr  9 22:52:26 2023, max compression
```

## Comparing `pytest-describe-2.0.2.tar` & `pytest-describe-2.1.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:53:32.356340 pytest-describe-2.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:53:32.356340 pytest-describe-2.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:53:32.356340 pytest-describe-2.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-04-09 14:53:32.356340 pytest-describe-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:53:32.356340 pytest-describe-2.0.2/pytest_describe/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/pytest_describe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/pytest_describe/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/pytest_describe/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:53:32.356340 pytest-describe-2.0.2/pytest_describe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-04-09 14:53:32.000000 pytest-describe-2.0.2/pytest_describe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 14:53:32.000000 pytest-describe-2.0.2/pytest_describe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 14:53:32.000000 pytest-describe-2.0.2/pytest_describe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-09 14:53:32.000000 pytest-describe-2.0.2/pytest_describe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-09 14:53:32.000000 pytest-describe-2.0.2/pytest_describe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-09 14:53:32.000000 pytest-describe-2.0.2/pytest_describe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 14:53:32.356340 pytest-describe-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:53:32.356340 pytest-describe-2.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/test/test_collect.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/test/test_custom_prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/test/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/test/test_marks.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/test/test_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/test/test_shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/test/test_simple_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/test/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 22:52:26.287712 pytest-describe-2.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 22:52:26.283712 pytest-describe-2.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 22:52:26.283712 pytest-describe-2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-09 22:52:22.000000 pytest-describe-2.1.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-09 22:52:22.000000 pytest-describe-2.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-09 22:52:22.000000 pytest-describe-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-09 22:52:22.000000 pytest-describe-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-09 22:52:26.287712 pytest-describe-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-09 22:52:22.000000 pytest-describe-2.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 22:52:26.283712 pytest-describe-2.1.0/pytest_describe/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-09 22:52:22.000000 pytest-describe-2.1.0/pytest_describe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-09 22:52:22.000000 pytest-describe-2.1.0/pytest_describe/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-09 22:52:22.000000 pytest-describe-2.1.0/pytest_describe/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 22:52:26.283712 pytest-describe-2.1.0/pytest_describe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-09 22:52:26.000000 pytest-describe-2.1.0/pytest_describe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-09 22:52:26.000000 pytest-describe-2.1.0/pytest_describe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 22:52:26.000000 pytest-describe-2.1.0/pytest_describe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-09 22:52:26.000000 pytest-describe-2.1.0/pytest_describe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-09 22:52:26.000000 pytest-describe-2.1.0/pytest_describe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-09 22:52:26.000000 pytest-describe-2.1.0/pytest_describe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-09 22:52:26.287712 pytest-describe-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-09 22:52:22.000000 pytest-describe-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 22:52:26.287712 pytest-describe-2.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-09 22:52:22.000000 pytest-describe-2.1.0/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-09 22:52:22.000000 pytest-describe-2.1.0/test/test_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-09 22:52:22.000000 pytest-describe-2.1.0/test/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-09 22:52:22.000000 pytest-describe-2.1.0/test/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-04-09 22:52:22.000000 pytest-describe-2.1.0/test/test_marks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-09 22:52:22.000000 pytest-describe-2.1.0/test/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-09 22:52:22.000000 pytest-describe-2.1.0/test/test_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-04-09 22:52:22.000000 pytest-describe-2.1.0/test/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-09 22:52:22.000000 pytest-describe-2.1.0/test/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-09 22:52:22.000000 pytest-describe-2.1.0/tox.ini
```

### Comparing `pytest-describe-2.0.2/.github/workflows/main.yml` & `pytest-describe-2.1.0/.github/workflows/main.yml`

 * *Files 21% similar despite different names*

```diff
@@ -9,62 +9,66 @@
 
   pull_request:
     branches:
       - main
 
 jobs:
   build:
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-latest
 
     strategy:
       matrix:
-        python: ['3.6', '3.7', '3.8', '3.9', '3.10', 'pypy3.9']
+        python: ['3.7', '3.8', '3.9', '3.10', '3.11', 'pypy3.9']
 
     steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
 
     - name: Set up Python ${{ matrix.python }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python }}
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip setuptools
-        python -m pip install 'tox>=3.28,<4.0'
-
-    - name: Test with Python 3.6
-      if: matrix.python == '3.6'
-      run: tox -e 'py36-pytest{4,50,51,52,53,54,60,61,62,70}'
+        python -m pip install 'tox>=4.4,<5'
 
     - name: Test with Python 3.7
       if: matrix.python == '3.7'
-      run: tox -e 'py37-pytest{4,50,51,52,53,54,60,61,62,70}'
+      run: tox run -x "tox.envlist=py37-pytest{4,5,60,61,62,70,71,72,73}"
 
     - name: Test with Python 3.8
       if: matrix.python == '3.8'
-      run: tox -e 'py38-pytest{4,50,51,52,53,54,60,61,62,70}'
+      run: tox run -x "tox.envlist=py38-pytest{4,5,60,61,62,70,71,72,73}"
 
     - name: Test with Python 3.9
       if: matrix.python == '3.9'
-      run: tox -e 'py39-pytest{4,50,51,52,53,54,60,61,62,70}'
+      run: tox run -x "tox.envlist=py39-pytest{4,5,60,61,62,70,71,72,73}"
 
     - name: Test with Python 3.10
       if: matrix.python == '3.10'
-      run: tox -e 'py310-pytest{62,70}'
+      run: tox run -x "tox.envlist=py310-pytest{62,70,71,72,73}"
+
+    - name: Test with Python 3.11
+      if: matrix.python == '3.11'
+      run: tox run -x "tox.envlist=spy311-pytest{73}"
 
     - name: Test with PyPy 3.9
       if: matrix.python == 'pypy3.9'
-      run: tox -e 'pypy39-pytest{4,50,51,52,53,54,60,61,62,70}'
+      run: tox run -x "tox.envlist=pypy39-pytest{4,5,60,61,62,70,71,72,73}"
 
     - name: Linting with Flake8
-      if: matrix.python == '3.9'
-      run: tox -e flake8
+      if: matrix.python == '3.10'
+      run: tox run -e flake8
+
+    - name: Ensure full coverage
+      if: matrix.python == '3.10'
+      run: tox run -e coverage
 
   deploy:
     if: |
       github.event_name == 'push' &&
       startsWith(github.event.ref, 'refs/tags') &&
       github.repository == 'pytest-dev/pytest-describe'
     runs-on: ubuntu-latest
@@ -72,15 +76,15 @@
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - uses: actions/setup-python@v4
         with:
-          python-version: '3.9'
+          python-version: '3.10'
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install --upgrade wheel setuptools setuptools_scm
 
       - name: Build package
```

### Comparing `pytest-describe-2.0.2/.gitignore` & `pytest-describe-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-describe-2.0.2/LICENSE` & `pytest-describe-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-describe-2.0.2/PKG-INFO` & `pytest-describe-2.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 Metadata-Version: 2.1
 Name: pytest-describe
-Version: 2.0.2
+Version: 2.1.0
 Summary: Describe-style plugin for pytest
 Home-page: https://github.com/pytest-dev/pytest-describe
 Author: Robin Pedersen
 Author-email: robinpeder@gmail.com
 Maintainer: Christoph Zwerschke
 Maintainer-email: cito@online.de
 License: MIT
+Project-URL: Source, https://github.com/pytest-dev/pytest-describe
+Project-URL: Tracker, https://github.com/pytest-dev/pytest-describe/issues
+Keywords: test,unittest,plugin,describe
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Utilities
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://badge.fury.io/py/pytest-describe.svg
     :target: https://pypi.org/project/pytest-describe/
     :alt: PyPI version
```

### Comparing `pytest-describe-2.0.2/README.rst` & `pytest-describe-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-describe-2.0.2/pytest_describe/plugin.py` & `pytest-describe-2.1.0/pytest_describe/plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,83 +1,89 @@
+"""The pytest-describe plugin"""
+
 import sys
 import types
 import pytest
 
 
 PYTEST_GTE_7_0 = getattr(pytest, 'version_tuple', (0, 0)) >= (7, 0)
 PYTEST_GTE_5_4 = PYTEST_GTE_7_0 or hasattr(pytest.Collector, 'from_parent')
 
 
-def trace_function(funcobj, *args, **kwargs):
-    """Call a function, and return its locals"""
-    funclocals = {}
+def trace_function(func, *args, **kwargs):  # pragma: no-cover
+    """Call a function and return its locals."""
+    f_locals = {}
 
-    def _tracefunc(frame, event, arg):
+    def _trace_func(frame, event, arg):  # pragma: no cover
         # Activate local trace for first call only
-        if frame.f_back.f_locals.get('_tracefunc') == _tracefunc:
-            if event == 'return':
-                funclocals.update(frame.f_locals)
+        if (frame.f_back.f_locals.get('_trace_func') == _trace_func
+                and event == 'return'):
+            f_locals.update(frame.f_locals)
 
-    sys.setprofile(_tracefunc)
+    sys.setprofile(_trace_func)
     try:
-        funcobj(*args, **kwargs)
+        func(*args, **kwargs)
     finally:
         sys.setprofile(None)
 
-    return funclocals
+    return f_locals
 
 
-def make_module_from_function(funcobj):
-    """Evaluates the local scope of a function, as if it was a module"""
-    module = types.ModuleType(funcobj.__name__)
+def make_module_from_function(func):
+    """Evaluate the local scope of a function as if it was a module."""
+    module = types.ModuleType(func.__name__)
 
     # Import shared behaviors into the generated module. We do this before
     # importing the direct children, so that fixtures in the block that's
     # importing the behavior take precedence.
-    for shared_funcobj in getattr(funcobj, '_behaves_like', []):
-        module.__dict__.update(evaluate_shared_behavior(shared_funcobj))
+    for shared_func in getattr(func, '_behaves_like', []):
+        module.__dict__.update(evaluate_shared_behavior(shared_func))
 
     # Import children
-    module.__dict__.update(trace_function(funcobj))
+    module.__dict__.update(trace_function(func))
     return module
 
 
-def evaluate_shared_behavior(funcobj):
-    if not hasattr(funcobj, '_shared_functions'):
-        funcobj._shared_functions = {}
-        for name, obj in trace_function(funcobj).items():
+def evaluate_shared_behavior(func):
+    """Evaluate the local scope of a function."""
+    try:
+        shared_functions = func._shared_functions
+    except AttributeError:
+        shared_functions = {}
+        for name, obj in trace_function(func).items():
             # Only functions are relevant here
             if not isinstance(obj, types.FunctionType):
                 continue
 
             # Mangle names of imported functions, except fixtures because we
             # want fixtures to be overridden in the block that's importing the
             # behavior.
             if not hasattr(obj, '_pytestfixturefunction'):
-                name = obj._mangled_name = f"{funcobj.__name__}::{name}"
+                name = obj._mangled_name = f"{func.__name__}::{name}"
 
-            funcobj._shared_functions[name] = obj
-    return funcobj._shared_functions
+            shared_functions[name] = obj
+        func._shared_functions = shared_functions
+    return shared_functions
 
 
 class DescribeBlock(pytest.Module):
     """Module-like object representing the scope of a describe block"""
 
     @classmethod
     def from_parent(cls, parent, obj):
         """Construct a new node for the describe block"""
         name = getattr(obj, '_mangled_name', obj.__name__)
         nodeid = parent.nodeid + '::' + name
         if PYTEST_GTE_7_0:
             self = super().from_parent(
                 parent=parent, path=parent.path, nodeid=nodeid)
-        elif PYTEST_GTE_5_4:
+        elif PYTEST_GTE_5_4:  # pragma: no cover
             self = super().from_parent(
                 parent=parent, fspath=parent.fspath, nodeid=nodeid)
-        else:
+        else:  # pragma: no cover
             self = cls(parent=parent, fspath=parent.fspath, nodeid=nodeid)
         self.name = name
         self.funcobj = obj
         return self
 
     def collect(self):
         """Get list of children"""
@@ -106,16 +112,18 @@
         return False
 
     def __repr__(self):
         return f"<{self.__class__.__name__} {self.name!r}>"
 
 
 def pytest_pycollect_makeitem(collector, name, obj):
+    """Collector items from describe blocks."""
     if isinstance(obj, types.FunctionType):
         for prefix in collector.config.getini('describe_prefixes'):
             if obj.__name__.startswith(prefix):
                 return DescribeBlock.from_parent(collector, obj)
 
 
 def pytest_addoption(parser):
+    """Add configuration option describe_prefixes."""
     parser.addini("describe_prefixes", type="args", default=("describe",),
                   help="prefixes for Python describe function discovery")
```

### Comparing `pytest-describe-2.0.2/pytest_describe.egg-info/PKG-INFO` & `pytest-describe-2.1.0/pytest_describe.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 Metadata-Version: 2.1
 Name: pytest-describe
-Version: 2.0.2
+Version: 2.1.0
 Summary: Describe-style plugin for pytest
 Home-page: https://github.com/pytest-dev/pytest-describe
 Author: Robin Pedersen
 Author-email: robinpeder@gmail.com
 Maintainer: Christoph Zwerschke
 Maintainer-email: cito@online.de
 License: MIT
+Project-URL: Source, https://github.com/pytest-dev/pytest-describe
+Project-URL: Tracker, https://github.com/pytest-dev/pytest-describe/issues
+Keywords: test,unittest,plugin,describe
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Utilities
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://badge.fury.io/py/pytest-describe.svg
     :target: https://pypi.org/project/pytest-describe/
     :alt: PyPI version
```

### Comparing `pytest-describe-2.0.2/pytest_describe.egg-info/SOURCES.txt` & `pytest-describe-2.1.0/pytest_describe.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 .gitignore
 LICENSE
 MANIFEST.in
 README.rst
+setup.cfg
 setup.py
 tox.ini
 .github/workflows/main.yml
 pytest_describe/__init__.py
 pytest_describe/plugin.py
 pytest_describe/shared.py
 pytest_describe.egg-info/PKG-INFO
 pytest_describe.egg-info/SOURCES.txt
 pytest_describe.egg-info/dependency_links.txt
 pytest_describe.egg-info/entry_points.txt
 pytest_describe.egg-info/requires.txt
 pytest_describe.egg-info/top_level.txt
+test/conftest.py
+test/test_class.py
 test/test_collect.py
-test/test_custom_prefix.py
 test/test_fixtures.py
 test/test_marks.py
 test/test_output.py
+test/test_prefix.py
 test/test_shared.py
-test/test_simple_execution.py
-test/util.py
+test/test_simple.py
```

### Comparing `pytest-describe-2.0.2/test/test_collect.py` & `pytest-describe-2.1.0/test/test_collect.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,13 @@
-import py
-import re
+"""Test collection of test functions"""
 
-from util import assert_outcomes
 
-pytest_plugins = 'pytester'
-
-
-def test_collect(testdir):
-    a_dir = testdir.mkpydir('a_dir')
-    a_dir.join('test_a.py').write(py.code.Source("""
+def test_collect_only(testdir):
+    testdir.makepyfile(
+        """
         def describe_something():
             def is_foo():
                 pass
             def can_bar():
                 pass
             def _not_a_test():
                 pass
@@ -20,43 +15,44 @@
             def describe_nested():
                 def a_test():
                     pass
         def foo_not_collected():
             pass
         def test_something():
             pass
-    """))
+        """)
 
     result = testdir.runpytest('--collectonly')
+    result.assert_outcomes()
 
-    expected_regex = map(re.compile, [
-        r"collected 4 item(s)?",
-        r"\s*<DescribeBlock '?describe_something'?>",
-        r"\s*<Function '?is_foo'?>",
-        r"\s*<Function '?can_bar'?>",
-        r"\s*<DescribeBlock '?describe_something_else'?>",
-        r"\s*<DescribeBlock '?describe_nested'?>",
-        r"\s*<Function '?a_test'?>",
-        r"\s*<Function '?test_something'?>",
-    ])
-    for line in expected_regex:
-        assert any([line.match(r) is not None for r in result.outlines])
+    output = '\n'.join(filter(None, result.outlines))
+    assert """
+collected 4 items
+<Module test_collect_only.py>
+  <DescribeBlock 'describe_something'>
+    <Function is_foo>
+    <Function can_bar>
+  <DescribeBlock 'describe_something_else'>
+    <DescribeBlock 'describe_nested'>
+      <Function a_test>
+  <Function test_something>
+""" in output
 
 
 def test_describe_evaluated_once(testdir):
-    a_dir = testdir.mkpydir('a_dir')
-    a_dir.join('test_something.py').write(py.code.Source("""
+    testdir.makepyfile(
+        """
         count = 0
         def describe_is_evaluated_only_once():
             global count
             count += 1
             def one():
                 assert count == 1
             def two():
                 assert count == 1
             def describe_nested():
                 def three():
                     assert count == 1
-    """))
+    """)
 
     result = testdir.runpytest('-v')
-    assert_outcomes(result, passed=3)
+    result.assert_outcomes(passed=3)
```

### Comparing `pytest-describe-2.0.2/test/test_marks.py` & `pytest-describe-2.1.0/test/test_marks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,22 @@
-import py
-from util import assert_outcomes
+"""Test mark decorator"""
 
-pytest_plugins = 'pytester'
+
+def assert_outcomes(result, **kwargs):
+    """Get all relevant outcomes"""
+    assert {
+        key: value
+        for key, value in result.parseoutcomes().items()
+        if key != 'seconds'
+    } == kwargs  # pragma: no cover
 
 
 def test_special_marks(testdir):
-    a_dir = testdir.mkpydir('a_dir')
-    a_dir.join('test_a.py').write(py.code.Source("""
+    testdir.makepyfile(
+        """
         import pytest
 
         def describe_marks():
             @pytest.mark.xfail
             def xfails():
                 assert False
 
@@ -21,23 +27,23 @@
             @pytest.mark.skipif("0 < 1")
             def skipped():
                 pass
 
             @pytest.mark.parametrize('foo', (1, 2, 3))
             def isint(foo):
                 assert foo == int(foo)
-    """))
+        """)
 
     result = testdir.runpytest()
-    assert_outcomes(result, passed=3, xfailed=1, xpassed=1, skipped=1)
+    result.assert_outcomes(passed=3, xfailed=1, xpassed=1, skipped=1)
 
 
 def test_multiple_variables_parametrize(testdir):
-    a_dir = testdir.mkpydir('a_dir')
-    a_dir.join('test_a.py').write(py.code.Source("""
+    testdir.makepyfile(
+        """
         import pytest
 
         def describe_marks():
             @pytest.mark.parametrize('foo,bar', [(1, 2), (3, 4)])
             def isint_str_names(foo, bar):
                 assert foo == int(foo)
                 assert bar == int(bar)
@@ -47,41 +53,41 @@
                 assert foo == int(foo)
                 assert bar == int(bar)
 
             @pytest.mark.parametrize(('foo', 'bar'), [(1, 2), (3, 4)])
             def isint_tuple_names(foo, bar):
                 assert foo == int(foo)
                 assert bar == int(bar)
-    """))
+        """)
 
     result = testdir.runpytest()
-    assert_outcomes(result, passed=6)
+    result.assert_outcomes(passed=6)
 
 
 def test_cartesian_parametrize(testdir):
-    a_dir = testdir.mkpydir('a_dir')
-    a_dir.join('test_a.py').write(py.code.Source("""
+    testdir.makepyfile(
+        """
         import pytest
 
         def describe_marks():
 
             @pytest.mark.parametrize('foo', (1, 2, 3))
             @pytest.mark.parametrize('bar', (1, 2, 3))
             def isint(foo, bar):
                 assert foo == int(foo)
                 assert bar == int(bar)
-    """))
+        """)
 
     result = testdir.runpytest()
-    assert_outcomes(result, passed=9)
+    result.assert_outcomes(passed=9)
 
 
 def test_parametrize_applies_to_describe(testdir):
-    a_dir = testdir.mkpydir('a_dir')
-    a_dir.join('test_a.py').write(py.code.Source("""
+    testdir.makepyfile(
+        """
         import pytest
 
         @pytest.mark.parametrize('foo', (1, 2, 3))
         def describe_marks():
 
             @pytest.mark.parametrize('bar', (1, 2, 3))
             def isint(foo, bar):
@@ -90,41 +96,41 @@
 
             def isint2(foo):
                 assert foo == int(foo)
 
             def describe_nested():
                 def isint3(foo):
                     assert foo == int(foo)
-    """))
+        """)
 
     result = testdir.runpytest()
-    assert_outcomes(result, passed=15)
+    result.assert_outcomes(passed=15)
 
 
 def test_cartesian_parametrize_on_describe(testdir):
-    a_dir = testdir.mkpydir('a_dir')
-    a_dir.join('test_a.py').write(py.code.Source("""
+    testdir.makepyfile(
+        """
         import pytest
 
         @pytest.mark.parametrize('foo', (1, 2, 3))
         @pytest.mark.parametrize('bar', (1, 2, 3))
         def describe_marks():
 
             def isint(foo, bar):
                 assert foo == int(foo)
                 assert bar == int(bar)
-    """))
+        """)
 
     result = testdir.runpytest()
-    assert_outcomes(result, passed=9)
+    result.assert_outcomes(passed=9)
 
 
 def test_parametrize_with_shared(testdir):
-    a_dir = testdir.mkpydir('a_dir')
-    a_dir.join('test_a.py').write(py.code.Source("""
+    testdir.makepyfile(
+        """
         import pytest
         from pytest import fixture
         from pytest_describe import behaves_like
 
         def a_duck():
             def it_quacks(sound):
                 assert sound == int(sound)
@@ -139,23 +145,23 @@
 
         @pytest.mark.parametrize('foo', (1, 2, 3))
         @behaves_like(a_duck)
         def describe_something_that_barks():
             @fixture
             def sound(foo):
                 return foo
-    """))
+        """)
 
     result = testdir.runpytest()
-    assert_outcomes(result, passed=6)
+    result.assert_outcomes(passed=6)
 
 
 def test_parametrize_with_shared_but_different_values(testdir):
-    a_dir = testdir.mkpydir('a_dir')
-    a_dir.join('test_a.py').write(py.code.Source("""
+    testdir.makepyfile(
+        """
         import pytest
         from pytest import fixture
         from pytest_describe import behaves_like
 
         def a_duck():
             def it_quacks(sound):
                 assert sound[1] == int(sound[1])
@@ -172,114 +178,126 @@
 
         @pytest.mark.parametrize('foo', (4, 5, 6))
         @behaves_like(a_duck)
         def describe_something_that_barks():
             @fixture
             def sound(foo):
                 return ('bark', foo)
-    """))
+        """)
 
     result = testdir.runpytest()
-    assert_outcomes(result, passed=6)
+    result.assert_outcomes(passed=6)
 
 
 def test_coincident_parametrize_at_top(testdir):
-    a_dir = testdir.mkpydir('a_dir')
-    a_dir.join('test_a.py').write(py.code.Source("""
+    testdir.makepyfile(
+        """
         import pytest
 
         @pytest.mark.parametrize('foo', (1, 2, 3))
         def describe_marks():
 
             @pytest.mark.parametrize('bar', (1, 2, 3))
             def isint(foo, bar):
                 assert foo == int(foo)
                 assert bar == int(bar)
 
         @pytest.mark.parametrize('foo', (1, 2, 3))
         def describe_marks2():
             def isint2(foo):
                 assert foo == int(foo)
-    """))
+        """)
 
     result = testdir.runpytest()
-    assert_outcomes(result, passed=12)
+    result.assert_outcomes(passed=12)
 
 
 def test_keywords(testdir):
-    a_dir = testdir.mkpydir('a_dir')
-    a_dir.join('test_a.py').write(py.code.Source("""
+    testdir.makepyfile(
+        """
         import pytest
         def describe_a():
-            @pytest.mark.foo
             def foo_test():
                 pass
-            @pytest.mark.bar
             def bar_test():
                 pass
-    """))
+        """)
 
     result = testdir.runpytest('-k', 'foo')
-    assert_outcomes(result, passed=1, deselected=1)
-
+    try:
+        result.assert_outcomes(passed=1, deselected=1)
+    except TypeError:  # pragma: no cover pytest < 7.0
+        assert_outcomes(result, passed=1, deselected=1)
+
+
+def test_custom_markers(testdir):
+    testdir.makeini(
+        """
+        [pytest]
+        markers =
+          foo
+          bar
+        """)
 
-def test_marks(testdir):
-    a_dir = testdir.mkpydir('a_dir')
-    a_dir.join('test_a.py').write(py.code.Source("""
+    testdir.makepyfile(
+        """
         import pytest
         def describe_a():
             @pytest.mark.foo
             def foo_test():
                 pass
             @pytest.mark.bar
             def bar_test():
                 pass
-    """))
+        """)
 
     result = testdir.runpytest('-m', 'foo')
-    assert_outcomes(result, passed=1, deselected=1)
+    try:
+        result.assert_outcomes(passed=1, deselected=1)
+    except TypeError:  # pragma: no cover pytest < 7.0
+        assert_outcomes(result, passed=1, deselected=1)
 
 
 def test_module_marks(testdir):
-    a_dir = testdir.mkpydir('a_dir')
-    a_dir.join('test_a.py').write(py.code.Source("""
+    testdir.makepyfile(
+        """
         import pytest
         pytestmark = [ pytest.mark.foo ]
         def describe_a():
             pytestmark = [ pytest.mark.bar ]
             def describe_b():
                 def a_test():
                     pass
-    """))
+        """)
 
     result = testdir.runpytest('-m', 'foo')
-    assert_outcomes(result, passed=1)
+    result.assert_outcomes(passed=1)
 
 
 def test_mark_at_describe_function(testdir):
-    a_dir = testdir.mkpydir('a_dir')
-    a_dir.join('test_a.py').write(py.code.Source("""
+    testdir.makepyfile(
+        """
         import pytest
         @pytest.mark.foo
         def describe_foo():
             def describe_a():
                 def a_test():
                     pass
             @pytest.mark.bar
             def b_test():
                 pass
-    """))
+        """)
 
     result = testdir.runpytest('-m', 'foo')
-    assert_outcomes(result, passed=2)
+    result.assert_outcomes(passed=2)
 
 
 def test_mark_stacking(testdir):
-    a_dir = testdir.mkpydir('a_dir')
-    a_dir.join('test_a.py').write(py.code.Source("""
+    testdir.makepyfile(
+        """
         import pytest
         @pytest.fixture()
         def get_marks(request):
             return [(mark.args[0], node.name) for node, mark
                     in request.node.iter_markers_with_node(name='my_mark')]
 
         @pytest.mark.my_mark('foo')
@@ -290,11 +308,11 @@
             @pytest.mark.my_mark('bar')
             @pytest.mark.my_mark('baz')
             def all_marks_are_chained(get_marks):
                 assert get_marks == [
                     ('baz', 'all_marks_are_chained'),
                     ('bar', 'all_marks_are_chained'),
                     ('foo', 'describe_marks')]
-    """))
+        """)
 
     result = testdir.runpytest()
-    assert_outcomes(result, passed=2)
+    result.assert_outcomes(passed=2)
```

### Comparing `pytest-describe-2.0.2/tox.ini` & `pytest-describe-2.1.0/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 [tox]
-envlist = py{36,37,38,39,py39}-pytest{4,50,51,52,53,54,60,61,62,70},py{310}-pytest{62,70},flake8
+envlist = py{37,38,39,py39}-pytest{4,5,60,61,62,70,71,72,73},py310-pytest{62,70,71,72,73},py311-pytest{73,-latest},flake8,coverage
 
 [testenv]
 basepython =
-    py36: python3.6
     py37: python3.7
     py38: python3.8
     py39: python3.9
     py310: python3.10
+    py311: python3.11
     pypy39: pypy3.9
 deps =
     pytest4: pytest>=4.6,<5.0
-    pytest50: pytest>=5.0,<5.2
-    pytest51: pytest>=5.1,<5.2
-    pytest52: pytest>=5.2,<5.3
-    pytest53: pytest>=5.3,<5.4
-    pytest54: pytest>=5.4,<5.5
+    pytest5: pytest>=5.4,<5.5
     pytest60: pytest>=6.0,<6.1
     pytest61: pytest>=6.1,<6.2
     pytest62: pytest>=6.2,<6.3
     pytest70: pytest>=7.0,<7.1
+    pytest71: pytest>=7.1,<7.2
+    pytest72: pytest>=7.2,<7.3
+    pytest73: pytest>=7.3,<7.4
     pytest-latest: pytest
     pytest-main: git+https://github.com/pytest-dev/pytest.git@main
-commands = pytest -rw {posargs}
+commands = pytest test {posargs}
 
 [testenv:flake8]
-basepython = python3.9
+basepython = python3.10
 deps = flake8>=6,<7
 commands =
     flake8 pytest_describe test setup.py
 
 [testenv:coverage]
-basepython = python3.9
+basepython = python3.10
 deps =
     coverage
     pytest
 commands =
-    coverage run --source=pytest_describe -m pytest
-    coverage report -m
+    coverage run --source=pytest_describe,test -m pytest test {posargs}
+    coverage report -m --fail-under=100
 
 [pytest]
 minversion = 4.6
 filterwarnings =
     ignore:The TerminalReporter\.writer attribute is deprecated, use TerminalReporter\._tw instead at your own risk\.:DeprecationWarning
```

