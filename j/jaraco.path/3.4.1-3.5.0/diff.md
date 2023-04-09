# Comparing `tmp/jaraco.path-3.4.1.tar.gz` & `tmp/jaraco.path-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.path-3.4.1.tar", last modified: Fri Feb 17 02:50:01 2023, max compression
+gzip compressed data, was "jaraco.path-3.5.0.tar", last modified: Sun Apr  9 22:27:02 2023, max compression
```

## Comparing `jaraco.path-3.4.1.tar` & `jaraco.path-3.5.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 02:50:01.378318 jaraco.path-3.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-17 02:49:39.000000 jaraco.path-3.4.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-02-17 02:49:39.000000 jaraco.path-3.4.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-02-17 02:49:39.000000 jaraco.path-3.4.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 02:50:01.374318 jaraco.path-3.4.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-02-17 02:49:39.000000 jaraco.path-3.4.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 02:50:01.374318 jaraco.path-3.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-02-17 02:49:39.000000 jaraco.path-3.4.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-17 02:49:39.000000 jaraco.path-3.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-02-17 02:49:39.000000 jaraco.path-3.4.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-02-17 02:49:39.000000 jaraco.path-3.4.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-02-17 02:49:39.000000 jaraco.path-3.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-02-17 02:50:01.378318 jaraco.path-3.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-02-17 02:49:39.000000 jaraco.path-3.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 02:50:01.374318 jaraco.path-3.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-02-17 02:49:39.000000 jaraco.path-3.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-17 02:49:39.000000 jaraco.path-3.4.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-02-17 02:49:39.000000 jaraco.path-3.4.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 02:50:01.374318 jaraco.path-3.4.1/jaraco/
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-02-17 02:49:39.000000 jaraco.path-3.4.1/jaraco/path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 02:50:01.374318 jaraco.path-3.4.1/jaraco.path.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-02-17 02:50:01.000000 jaraco.path-3.4.1/jaraco.path.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-02-17 02:50:01.000000 jaraco.path-3.4.1/jaraco.path.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 02:50:01.000000 jaraco.path-3.4.1/jaraco.path.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-02-17 02:50:01.000000 jaraco.path-3.4.1/jaraco.path.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-17 02:50:01.000000 jaraco.path-3.4.1/jaraco.path.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-02-17 02:49:39.000000 jaraco.path-3.4.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-02-17 02:49:39.000000 jaraco.path-3.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-02-17 02:49:39.000000 jaraco.path-3.4.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-02-17 02:50:01.378318 jaraco.path-3.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 02:50:01.378318 jaraco.path-3.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-02-17 02:49:39.000000 jaraco.path-3.4.1/tests/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-02-17 02:49:39.000000 jaraco.path-3.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 22:27:02.481495 jaraco.path-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 22:27:02.477495 jaraco.path-3.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 22:27:02.477495 jaraco.path-3.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-09 22:27:02.481495 jaraco.path-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 22:27:02.477495 jaraco.path-3.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 22:27:02.477495 jaraco.path-3.5.0/jaraco/
+-rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/jaraco/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 22:27:02.481495 jaraco.path-3.5.0/jaraco.path.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-09 22:27:02.000000 jaraco.path-3.5.0/jaraco.path.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-09 22:27:02.000000 jaraco.path-3.5.0/jaraco.path.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 22:27:02.000000 jaraco.path-3.5.0/jaraco.path.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-09 22:27:02.000000 jaraco.path-3.5.0/jaraco.path.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-09 22:27:02.000000 jaraco.path-3.5.0/jaraco.path.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-09 22:27:02.481495 jaraco.path-3.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 22:27:02.481495 jaraco.path-3.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/tests/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/tox.ini
```

### Comparing `jaraco.path-3.4.1/.github/workflows/main.yml` & `jaraco.path-3.5.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `jaraco.path-3.4.1/CHANGES.rst` & `jaraco.path-3.5.0/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v3.5.0
+======
+
+Introduced ``Recording`` object and ``TreeMaker`` protocol,
+with ``build()`` now explicitly accepting any ``TreeMaker``.
+
 v3.4.1
 ======
 
 Fixed EncodingWarnings and ResourceWarnings.
 
 v3.4.0
 ======
```

### Comparing `jaraco.path-3.4.1/LICENSE` & `jaraco.path-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.path-3.4.1/PKG-INFO` & `jaraco.path-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.path
-Version: 3.4.1
+Version: 3.5.0
 Summary: miscellaneous path functions
 Home-page: https://github.com/jaraco/jaraco.path
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jaraco.path-3.4.1/README.rst` & `jaraco.path-3.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `jaraco.path-3.4.1/docs/conf.py` & `jaraco.path-3.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.path-3.4.1/jaraco/path.py` & `jaraco.path-3.5.0/jaraco/path.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 import tempfile
 import platform
 import ctypes
 import importlib
 import pathlib
 from typing import Dict, Union
 
+try:
+    from typing import Protocol, runtime_checkable
+except ImportError:  # pragma: no cover
+    # Python 3.7
+    from typing_extensions import Protocol, runtime_checkable  # type: ignore
+
 
 log = logging.getLogger(__name__)
 
 
 def get_unique_pathname(path, root=''):
     """Return a pathname possibly with a number appended to it so that it is
     unique in the directory."""
@@ -277,15 +283,37 @@
     res = url.getResourceValue_forKey_error_(None, Foundation.NSURLIsHiddenKey, None)
     return res[1]
 
 
 FilesSpec = Dict[str, Union[str, bytes, 'FilesSpec']]  # type: ignore
 
 
-def build(spec: FilesSpec, prefix=pathlib.Path()):
+@runtime_checkable
+class TreeMaker(Protocol):
+    def __truediv__(self, *args, **kwargs):
+        ...  # pragma: no cover
+
+    def mkdir(self, **kwargs):
+        ...  # pragma: no cover
+
+    def write_text(self, content, **kwargs):
+        ...  # pragma: no cover
+
+    def write_bytes(self, content):
+        ...  # pragma: no cover
+
+
+def _ensure_tree_maker(obj: Union[str, TreeMaker]) -> TreeMaker:
+    return obj if isinstance(obj, TreeMaker) else pathlib.Path(obj)  # type: ignore
+
+
+def build(
+    spec: FilesSpec,
+    prefix: Union[str, TreeMaker] = pathlib.Path(),  # type: ignore
+):
     """
     Build a set of files/directories, as described by the spec.
 
     Each key represents a pathname, and the value represents
     the content. Content may be a nested directory.
 
     >>> spec = {
@@ -300,15 +328,15 @@
     ... }
     >>> target = getfixture('tmp_path')
     >>> build(spec, target)
     >>> target.joinpath('foo/baz.py').read_text(encoding='utf-8')
     '# Some code'
     """
     for name, contents in spec.items():
-        create(contents, pathlib.Path(prefix) / name)
+        create(contents, _ensure_tree_maker(prefix) / name)
 
 
 @functools.singledispatch
 def create(content: Union[str, bytes, FilesSpec], path):
     path.mkdir(exist_ok=True)
     build(content, prefix=path)  # type: ignore
 
@@ -317,7 +345,33 @@
 def _(content: bytes, path):
     path.write_bytes(content)
 
 
 @create.register
 def _(content: str, path):
     path.write_text(content, encoding='utf-8')
+
+
+class Recording:
+    """
+    A TreeMaker object that records everything that would be written.
+
+    >>> r = Recording()
+    >>> build({'foo': {'foo1.txt': 'yes'}, 'bar.txt': 'abc'}, r)
+    >>> r.record
+    ['foo/foo1.txt', 'bar.txt']
+    """
+
+    def __init__(self, loc=pathlib.PurePosixPath(), record=None):
+        self.loc = loc
+        self.record = record if record is not None else []
+
+    def __truediv__(self, other):
+        return Recording(self.loc / other, self.record)
+
+    def write_text(self, content, **kwargs):
+        self.record.append(str(self.loc))
+
+    write_bytes = write_text
+
+    def mkdir(self, **kwargs):
+        return
```

### Comparing `jaraco.path-3.4.1/jaraco.path.egg-info/PKG-INFO` & `jaraco.path-3.5.0/jaraco.path.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.path
-Version: 3.4.1
+Version: 3.5.0
 Summary: miscellaneous path functions
 Home-page: https://github.com/jaraco/jaraco.path
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jaraco.path-3.4.1/pytest.ini` & `jaraco.path-3.5.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `jaraco.path-3.4.1/setup.cfg` & `jaraco.path-3.5.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 [options]
 packages = find_namespace:
 include_package_data = true
 python_requires = >=3.7
 install_requires = 
 	pyobjc; platform_system == "Darwin" and platform_python_implementation != "PyPy"
+	typing-extensions>=3.6.4; python_version < "3.8"
 
 [options.packages.find]
 exclude = 
 	build*
 	dist*
 	docs*
 	tests*
```

### Comparing `jaraco.path-3.4.1/tests/test_path.py` & `jaraco.path-3.5.0/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `jaraco.path-3.4.1/tox.ini` & `jaraco.path-3.5.0/tox.ini`

 * *Files identical despite different names*

