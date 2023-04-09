# Comparing `tmp/bigbrother-0.1.2.tar.gz` & `tmp/bigbrother-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigbrother-0.1.2.tar", last modified: Fri Apr  7 20:15:46 2023, max compression
+gzip compressed data, was "bigbrother-0.1.3.tar", last modified: Sun Apr  9 22:34:28 2023, max compression
```

## Comparing `bigbrother-0.1.2.tar` & `bigbrother-0.1.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-07 20:15:46.478933 bigbrother-0.1.2/
--rw-r--r--   0 timkpaine   (501) staff       (20)      299 2023-04-07 20:15:44.000000 bigbrother-0.1.2/.bumpversion.cfg
--rw-r--r--   0 timkpaine   (501) staff       (20)     1920 2023-04-06 02:39:34.000000 bigbrother-0.1.2/CONTRIBUTING.md
--rw-r--r--   0 timkpaine   (501) staff       (20)    11352 2023-04-06 02:39:34.000000 bigbrother-0.1.2/LICENSE
--rw-r--r--   0 timkpaine   (501) staff       (20)      509 2023-04-06 02:39:34.000000 bigbrother-0.1.2/MANIFEST.in
--rw-r--r--   0 timkpaine   (501) staff       (20)     3036 2023-04-07 19:12:10.000000 bigbrother-0.1.2/Makefile
--rw-r--r--   0 timkpaine   (501) staff       (20)    15759 2023-04-07 20:15:46.478727 bigbrother-0.1.2/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)     1914 2023-04-07 19:12:14.000000 bigbrother-0.1.2/README.md
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-07 20:15:46.476199 bigbrother-0.1.2/bigbrother/
--rw-r--r--   0 timkpaine   (501) staff       (20)     2355 2023-04-07 20:15:44.000000 bigbrother-0.1.2/bigbrother/__init__.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-07 20:15:46.477305 bigbrother-0.1.2/bigbrother/builtins/
--rw-r--r--   0 timkpaine   (501) staff       (20)      189 2023-04-07 19:12:10.000000 bigbrother-0.1.2/bigbrother/builtins/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2471 2023-04-07 19:12:10.000000 bigbrother-0.1.2/bigbrother/builtins/dict.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3048 2023-04-07 19:12:10.000000 bigbrother-0.1.2/bigbrother/builtins/list.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3048 2023-04-07 19:12:10.000000 bigbrother-0.1.2/bigbrother/builtins/set.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      282 2023-04-07 19:12:10.000000 bigbrother-0.1.2/bigbrother/common.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      126 2023-04-06 02:39:34.000000 bigbrother-0.1.2/bigbrother/generic.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-07 20:15:46.477513 bigbrother-0.1.2/bigbrother/libraries/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-04-06 02:39:34.000000 bigbrother-0.1.2/bigbrother/libraries/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1695 2023-04-07 19:12:10.000000 bigbrother-0.1.2/bigbrother/libraries/pydantic.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-07 20:15:46.477708 bigbrother-0.1.2/bigbrother/tests/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-04-06 02:39:34.000000 bigbrother-0.1.2/bigbrother/tests/__init__.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-07 20:15:46.478152 bigbrother-0.1.2/bigbrother/tests/builtins/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-04-06 02:39:34.000000 bigbrother-0.1.2/bigbrother/tests/builtins/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1348 2023-04-07 19:12:10.000000 bigbrother-0.1.2/bigbrother/tests/builtins/test_dict.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2083 2023-04-07 19:12:10.000000 bigbrother-0.1.2/bigbrother/tests/builtins/test_list.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2088 2023-04-07 19:12:10.000000 bigbrother-0.1.2/bigbrother/tests/builtins/test_set.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      465 2023-04-06 02:39:34.000000 bigbrother-0.1.2/bigbrother/tests/common.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-07 20:15:46.478480 bigbrother-0.1.2/bigbrother/tests/libraries/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-04-06 02:39:34.000000 bigbrother-0.1.2/bigbrother/tests/libraries/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2457 2023-04-07 19:12:10.000000 bigbrother-0.1.2/bigbrother/tests/libraries/test_pydantic.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-07 20:15:46.476846 bigbrother-0.1.2/bigbrother.egg-info/
--rw-r--r--   0 timkpaine   (501) staff       (20)    15759 2023-04-07 20:15:46.000000 bigbrother-0.1.2/bigbrother.egg-info/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)      804 2023-04-07 20:15:46.000000 bigbrother-0.1.2/bigbrother.egg-info/SOURCES.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        1 2023-04-07 20:15:46.000000 bigbrother-0.1.2/bigbrother.egg-info/dependency_links.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)      163 2023-04-07 20:15:46.000000 bigbrother-0.1.2/bigbrother.egg-info/requires.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       11 2023-04-07 20:15:46.000000 bigbrother-0.1.2/bigbrother.egg-info/top_level.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)     2170 2023-04-07 20:15:44.000000 bigbrother-0.1.2/pyproject.toml
--rw-r--r--   0 timkpaine   (501) staff       (20)       38 2023-04-07 20:15:46.478974 bigbrother-0.1.2/setup.cfg
--rw-r--r--   0 timkpaine   (501) staff       (20)       39 2023-04-06 02:39:34.000000 bigbrother-0.1.2/setup.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-09 22:34:28.732664 bigbrother-0.1.3/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      299 2023-04-09 22:33:34.000000 bigbrother-0.1.3/.bumpversion.cfg
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1920 2023-04-06 02:39:34.000000 bigbrother-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0 timkpaine   (501) staff       (20)    11352 2023-04-06 02:39:34.000000 bigbrother-0.1.3/LICENSE
+-rw-r--r--   0 timkpaine   (501) staff       (20)      509 2023-04-06 02:39:34.000000 bigbrother-0.1.3/MANIFEST.in
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3036 2023-04-07 19:12:10.000000 bigbrother-0.1.3/Makefile
+-rw-r--r--   0 timkpaine   (501) staff       (20)    16338 2023-04-09 22:34:28.732486 bigbrother-0.1.3/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2493 2023-04-09 22:33:34.000000 bigbrother-0.1.3/README.md
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-09 22:34:28.729553 bigbrother-0.1.3/bigbrother/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2384 2023-04-09 22:33:34.000000 bigbrother-0.1.3/bigbrother/__init__.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-09 22:34:28.730719 bigbrother-0.1.3/bigbrother/builtins/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      189 2023-04-07 19:12:10.000000 bigbrother-0.1.3/bigbrother/builtins/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2486 2023-04-09 22:33:34.000000 bigbrother-0.1.3/bigbrother/builtins/dict.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3067 2023-04-09 22:33:34.000000 bigbrother-0.1.3/bigbrother/builtins/list.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3059 2023-04-09 22:33:34.000000 bigbrother-0.1.3/bigbrother/builtins/set.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      196 2023-04-09 22:33:34.000000 bigbrother-0.1.3/bigbrother/common.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      126 2023-04-06 02:39:34.000000 bigbrother-0.1.3/bigbrother/generic.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-09 22:34:28.731069 bigbrother-0.1.3/bigbrother/libraries/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-04-06 02:39:34.000000 bigbrother-0.1.3/bigbrother/libraries/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1699 2023-04-09 22:33:34.000000 bigbrother-0.1.3/bigbrother/libraries/pydantic.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-09 22:34:28.731372 bigbrother-0.1.3/bigbrother/tests/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-04-06 02:39:34.000000 bigbrother-0.1.3/bigbrother/tests/__init__.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-09 22:34:28.731989 bigbrother-0.1.3/bigbrother/tests/builtins/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-04-06 02:39:34.000000 bigbrother-0.1.3/bigbrother/tests/builtins/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1603 2023-04-09 22:33:34.000000 bigbrother-0.1.3/bigbrother/tests/builtins/test_dict.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2491 2023-04-09 22:33:34.000000 bigbrother-0.1.3/bigbrother/tests/builtins/test_list.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2496 2023-04-09 22:33:34.000000 bigbrother-0.1.3/bigbrother/tests/builtins/test_set.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      692 2023-04-09 22:33:34.000000 bigbrother-0.1.3/bigbrother/tests/common.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-09 22:34:28.732231 bigbrother-0.1.3/bigbrother/tests/libraries/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-04-06 02:39:34.000000 bigbrother-0.1.3/bigbrother/tests/libraries/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2512 2023-04-09 22:33:34.000000 bigbrother-0.1.3/bigbrother/tests/libraries/test_pydantic.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-09 22:34:28.730166 bigbrother-0.1.3/bigbrother.egg-info/
+-rw-r--r--   0 timkpaine   (501) staff       (20)    16338 2023-04-09 22:34:28.000000 bigbrother-0.1.3/bigbrother.egg-info/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)      804 2023-04-09 22:34:28.000000 bigbrother-0.1.3/bigbrother.egg-info/SOURCES.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        1 2023-04-09 22:34:28.000000 bigbrother-0.1.3/bigbrother.egg-info/dependency_links.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)      163 2023-04-09 22:34:28.000000 bigbrother-0.1.3/bigbrother.egg-info/requires.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       11 2023-04-09 22:34:28.000000 bigbrother-0.1.3/bigbrother.egg-info/top_level.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2170 2023-04-09 22:33:34.000000 bigbrother-0.1.3/pyproject.toml
+-rw-r--r--   0 timkpaine   (501) staff       (20)       38 2023-04-09 22:34:28.732713 bigbrother-0.1.3/setup.cfg
+-rw-r--r--   0 timkpaine   (501) staff       (20)       39 2023-04-06 02:39:34.000000 bigbrother-0.1.3/setup.py
```

### Comparing `bigbrother-0.1.2/CONTRIBUTING.md` & `bigbrother-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bigbrother-0.1.2/LICENSE` & `bigbrother-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bigbrother-0.1.2/Makefile` & `bigbrother-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `bigbrother-0.1.2/PKG-INFO` & `bigbrother-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigbrother
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library for object observability
 Author-email: Tim Paine <t.paine154@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -233,27 +233,43 @@
 ## Overview
 `bigbrother` is a mutation observer library. You can use it to watch your objects for changes. When your object changes, `bigbrother` will trigger your choice of callback. 
 
 
 ```python
 x = {1: "a", 2: "b", 3: "c"}
 
-def track_changes(obj, method, *args, **kwargs):
+def track_changes(obj, method, ref, call_args, call_kwargs):
     print(f"method: {method}, args: {args}, kwargs: {kwargs}")
 
 x = watch(x, track_changes)
 
 x[1] = "x"
 
 # prints: method: setitem, args: (1, 'x'), kwargs: {}
 ```
 
 `bigbrother` can also embed itself recursively in your object by passing in argument `deepstate=True`.
 
 
+## Callback
+
+```python
+def callback(obj, method, ref, call_args, call_kwargs):
+    '''Callback called when object is mutated
+
+    Args:
+        obj (Any): The object being mutated via `method`
+        method (str): The method called on the object (dunders removed)
+        ref (Any): Reference object. If callback installed recursively, `ref` will be the entrypoint
+        call_args (Tuple[Any]): Positional arguments that `method` was called with on `obj`
+        call_kwargs (Dict[Any, Any]): Keyword arguments that `method` was called with on `obj`
+    '''
+```
+
+
 ## Supported types
 
 ### Builtins
 Most builtin types are read-only and cannot have their method structure mutated, so we observe via replacement with thin wrappers. 
 
 - `list` via `_ObservedList`
     - `append`
```

### Comparing `bigbrother-0.1.2/README.md` & `bigbrother-0.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -9,27 +9,43 @@
 ## Overview
 `bigbrother` is a mutation observer library. You can use it to watch your objects for changes. When your object changes, `bigbrother` will trigger your choice of callback. 
 
 
 ```python
 x = {1: "a", 2: "b", 3: "c"}
 
-def track_changes(obj, method, *args, **kwargs):
+def track_changes(obj, method, ref, call_args, call_kwargs):
     print(f"method: {method}, args: {args}, kwargs: {kwargs}")
 
 x = watch(x, track_changes)
 
 x[1] = "x"
 
 # prints: method: setitem, args: (1, 'x'), kwargs: {}
 ```
 
 `bigbrother` can also embed itself recursively in your object by passing in argument `deepstate=True`.
 
 
+## Callback
+
+```python
+def callback(obj, method, ref, call_args, call_kwargs):
+    '''Callback called when object is mutated
+
+    Args:
+        obj (Any): The object being mutated via `method`
+        method (str): The method called on the object (dunders removed)
+        ref (Any): Reference object. If callback installed recursively, `ref` will be the entrypoint
+        call_args (Tuple[Any]): Positional arguments that `method` was called with on `obj`
+        call_kwargs (Dict[Any, Any]): Keyword arguments that `method` was called with on `obj`
+    '''
+```
+
+
 ## Supported types
 
 ### Builtins
 Most builtin types are read-only and cannot have their method structure mutated, so we observe via replacement with thin wrappers. 
 
 - `list` via `_ObservedList`
     - `append`
```

### Comparing `bigbrother-0.1.2/bigbrother/__init__.py` & `bigbrother-0.1.3/bigbrother/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 from types import MethodType
-from typing import Any, Callable, Dict, List, Set, TypeVar
+from typing import Any, Callable, Dict, List, Set, Tuple, TypeVar
 
 from .generic import _replacement_setattr, _replacement_setitem
 from .builtins import (
     _createObservedDict,
     _ObservedDict,
     _createObservedList,
     _ObservedList,
@@ -33,15 +33,15 @@
             kwargs.pop("obj", None)
             kwargs.pop("self", None)
         return watcher(obj, *args, **kwargs)
 
     return _watcher_wrapper
 
 
-def _install_watcher(obj: T, watcher: Callable[[T, str, Any], None], recursive: bool = False) -> T:
+def _install_watcher(obj: T, watcher: Callable[[T, str, T, Tuple, Dict], None], recursive: bool = False) -> T:
     # Standard mutable types
     if isinstance(obj, List) and not isinstance(obj, _ObservedList):
         # can't mutate list so replace with watcher variant
         return _createObservedList(watcher, recursive=recursive, _install_watcher=_install_watcher)(obj)
 
     if isinstance(obj, Set) and not isinstance(obj, _ObservedSet):
         return _createObservedSet(watcher, recursive=recursive, _install_watcher=_install_watcher)(obj)
@@ -71,12 +71,12 @@
     except AttributeError:
         # Ignore
         pass
 
     return obj
 
 
-def watch(obj: T, watcher: Callable[[T, str, Any], None], deepstate: bool = False) -> T:
+def watch(obj: T, watcher: Callable[[T, str, T, Tuple, Dict], None], deepstate: bool = False) -> T:
     return _install_watcher(obj, watcher, recursive=deepstate)
 
 
 __all__ = ["watch", "__version__"]
```

### Comparing `bigbrother-0.1.2/bigbrother/builtins/dict.py` & `bigbrother-0.1.3/bigbrother/builtins/dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             # just defer to my own __setitem__, but without the watcher
             for i, item in self.items():
                 self[i] = item
         object.__setattr__(self, "_watcher_ready", True)
 
     def _notify_watcher(self, method, *args, **kwargs):
         if self._watcher_ready:
-            self.__class__._watcher(self, method, *args, **kwargs)
+            self.__class__._watcher(self, method, self, args, kwargs)
 
     def clear(self, *args, **kwargs):
         self._notify_watcher("clear", *args, **kwargs)
         return super().clear(*args, **kwargs)
 
     def pop(self, *args, **kwargs):
         self._notify_watcher("pop", *args, **kwargs)
@@ -33,26 +33,26 @@
     def popitem(self, *args, **kwargs):
         self._notify_watcher("popitem", *args, **kwargs)
         return super().popitem(*args, **kwargs)
 
     def update(self, __m, **kwargs):
         other = dict(__m, **kwargs)
         if self.__class__._recursive:
-            other = self.__class__._install_watcher(other, watcher=_partial(self.__class__._watcher, self), recursive=self._recursive)
+            other = self.__class__._install_watcher(other, watcher=_partial(self.__class__._watcher, ref=self), recursive=self._recursive)
         self._notify_watcher("update", other)
         return super().update(other)
 
     def __setattr__(self, *args, **kwargs):
         self._notify_watcher("setattr", *args, **kwargs)
         return super().__setattr__(*args, **kwargs)
 
     def __setitem__(self, __key, __value):
         if self._recursive:
-            __key = self.__class__._install_watcher(__key, watcher=_partial(self.__class__._watcher, self), recursive=self._recursive)
-            __value = self.__class__._install_watcher(__value, watcher=_partial(self.__class__._watcher, self), recursive=self._recursive)
+            __key = self.__class__._install_watcher(__key, watcher=_partial(self.__class__._watcher, ref=self), recursive=self._recursive)
+            __value = self.__class__._install_watcher(__value, watcher=_partial(self.__class__._watcher, ref=self), recursive=self._recursive)
         self._notify_watcher("setitem", __key, __value)
         return super().__setitem__(__key, __value)
 
 
 def _create(watcher: Callable[[_ObservedDict, str, Any], None], recursive: bool, _install_watcher: Callable) -> Type[_ObservedDict]:
     return type(
         "_ObservedDict", (_ObservedDict,), {"_watcher": watcher, "_recursive": recursive, "_install_watcher": _install_watcher, "_watcher_ready": False}
```

### Comparing `bigbrother-0.1.2/bigbrother/builtins/list.py` & `bigbrother-0.1.3/bigbrother/builtins/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,36 +16,36 @@
             # just defer to my own __setitem__
             for i, item in enumerate(self):
                 self[i] = item
         object.__setattr__(self, "_watcher_ready", True)
 
     def _notify_watcher(self, method, *args, **kwargs):
         if self._watcher_ready:
-            self.__class__._watcher(self, method, *args, **kwargs)
+            self.__class__._watcher(self, method, self, args, kwargs)
 
     def append(self, __object: Any):
         self._notify_watcher("append", __object)
         if self._recursive:
-            __object = self.__class__._install_watcher(__object, watcher=_partial(self.__class__._watcher, self), recursive=self._recursive)
+            __object = self.__class__._install_watcher(__object, watcher=_partial(self.__class__._watcher, ref=self), recursive=self._recursive)
         return super().append(__object)
 
     def clear(self, *args, **kwargs):
         self._notify_watcher("clear", *args, **kwargs)
         return super().clear(*args, **kwargs)
 
     def extend(self, __iterable):
         self._notify_watcher("extend", __iterable)
         if self._recursive:
-            __iterable = self.__class__._install_watcher(list(__iterable), watcher=_partial(self.__class__._watcher, self), recursive=self._recursive)
+            __iterable = self.__class__._install_watcher(list(__iterable), watcher=_partial(self.__class__._watcher, ref=self), recursive=self._recursive)
         return super().extend(__iterable)
 
     def insert(self, __key: int, __value: Any):
         self._notify_watcher("insert", __key, __value)
         if self._recursive:
-            __value = self.__class__._install_watcher(__value, watcher=_partial(self.__class__._watcher, self), recursive=self._recursive)
+            __value = self.__class__._install_watcher(__value, watcher=_partial(self.__class__._watcher, ref=self), recursive=self._recursive)
         return super().insert(__key, __value)
 
     def pop(self, *args, **kwargs):
         self._notify_watcher("pop", *args, **kwargs)
         return super().pop(*args, **kwargs)
 
     def remove(self, *args, **kwargs):
@@ -59,15 +59,15 @@
     def __setattr__(self, *args, **kwargs):
         self._notify_watcher("setattr", *args, **kwargs)
         return super().__setattr__(*args, **kwargs)
 
     def __setitem__(self, __key: int, __value: Any):
         self._notify_watcher("setitem", __key, __value)
         if self._recursive:
-            __value = self.__class__._install_watcher(__value, watcher=_partial(self.__class__._watcher, self), recursive=self._recursive)
+            __value = self.__class__._install_watcher(__value, watcher=_partial(self.__class__._watcher, ref=self), recursive=self._recursive)
         return super().__setitem__(__key, __value)
 
 
 def _create(watcher: Callable[[_ObservedList, str, Any], None], recursive: bool, _install_watcher: Callable) -> Type[_ObservedList]:
     return type(
         "_ObservedList", (_ObservedList,), {"_watcher": watcher, "_recursive": recursive, "_install_watcher": _install_watcher, "_watcher_ready": False}
     )
```

### Comparing `bigbrother-0.1.2/bigbrother/builtins/set.py` & `bigbrother-0.1.3/bigbrother/builtins/set.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,20 +18,20 @@
             self.clear()
             for i in x:
                 self.add(x)
         object.__setattr__(self, "_watcher_ready", True)
 
     def _notify_watcher(self, method, *args, **kwargs):
         if self._watcher_ready:
-            self.__class__._watcher(self, method, *args, **kwargs)
+            self.__class__._watcher(self, method, self, args, kwargs)
 
     def add(self, __element: Any):
         self._notify_watcher("add", __element)
         if self._recursive:
-            __element = self.__class__._install_watcher(__element, watcher=_partial(self.__class__._watcher, self), recursive=self._recursive)
+            __element = self.__class__._install_watcher(__element, watcher=_partial(self.__class__._watcher, ref=self), recursive=self._recursive)
         return super().add(__element)
 
     def clear(self, *args, **kwargs):
         self._notify_watcher("clear", *args, **kwargs)
         return super().clear(*args, **kwargs)
 
     def difference_update(self, *args, **kwargs):
@@ -61,15 +61,15 @@
         # TODO install watcher on items
         return super().symmetric_difference_update(*args, **kwargs)
 
     def update(self, *args):
         self._notify_watcher("update", *args)
         s = set(*args)
         if self._recursive:
-            s = self._install_watcher(s, watcher=_partial(self.__class__._watcher, self), recursive=self._recursive)
+            s = self._install_watcher(s, watcher=_partial(self.__class__._watcher, ref=self), recursive=self._recursive)
         return super().update(s)
 
     def __setattr__(self, *args, **kwargs):
         self._notify_watcher("setattr", *args, **kwargs)
         return super().__setattr__(*args, **kwargs)
```

### Comparing `bigbrother-0.1.2/bigbrother/libraries/pydantic.py` & `bigbrother-0.1.3/bigbrother/libraries/pydantic.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,9 +22,9 @@
             # for name, field in obj.__fields__.items():
             #     obj.__fields__[name] = _install_watcher_pydantic_field(field=field, watcher=watcher, recursive=recursive, _install_watcher=_install_watcher)
             # TODO but don't want to do this on the dict either
             # for key, value in obj.__dict__.items():
             #     obj.__dict__[key] = _install_watcher(value, watcher, recursive=recursive)
             ...
         # replace dict with watched version
-        object.__setattr__(obj, "__dict__", _install_watcher(obj.__dict__, watcher=_partial(watcher, obj), recursive=recursive))
+        object.__setattr__(obj, "__dict__", _install_watcher(obj.__dict__, watcher=_partial(watcher, ref=obj), recursive=recursive))
         return obj
```

### Comparing `bigbrother-0.1.2/bigbrother/tests/builtins/test_list.py` & `bigbrother-0.1.3/bigbrother/tests/builtins/test_list.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,69 +5,69 @@
 @fixture
 def a_list():
     return [1, 2, 3]
 
 
 class TestList:
     def test_list_append(self, a_list):
-        instance, called = create_tester(a_list, "append", (1,), {})
+        instance, called = create_tester(instance=a_list, method_name="append", expected_args=(1,), expected_kwargs={})
         instance.append(1)
         assert called[0]
         assert len(called) == 1
         assert instance == [1, 2, 3, 1]
 
     def test_list_clear(self, a_list):
-        instance, called = create_tester(a_list, "clear", (), {})
+        instance, called = create_tester(instance=a_list, method_name="clear", expected_args=(), expected_kwargs={})
         instance.clear()
         assert called[0]
         assert len(called) == 1
         assert instance == []
 
     def test_list_extend(self, a_list):
-        instance, called = create_tester(a_list, "extend", ([1, 2, 3],), {})
+        instance, called = create_tester(instance=a_list, method_name="extend", expected_args=([1, 2, 3],), expected_kwargs={})
         instance.extend([1, 2, 3])
         assert called[0]
         assert len(called) == 1
         assert instance == [1, 2, 3, 1, 2, 3]
 
     def test_list_insert(self, a_list):
         instance, called = create_tester(
-            a_list,
-            "insert",
-            (
+            instance=a_list,
+            method_name="insert",
+            expected_args=(
                 0,
                 1,
             ),
-            {},
+            expected_kwargs={},
         )
         instance.insert(0, 1)
         assert called[0]
         assert len(called) == 1
         assert instance == [1, 1, 2, 3]
 
     def test_list_pop(self, a_list):
-        instance, called = create_tester(a_list, "pop", (0,), {})
+        instance, called = create_tester(instance=a_list, method_name="pop", expected_args=(0,), expected_kwargs={})
         instance.pop(0)
         assert called[0]
         assert len(called) == 1
         assert instance == [2, 3]
 
     def test_list_remove(self, a_list):
-        instance, called = create_tester(a_list, "remove", (1,), {})
+        instance, called = create_tester(instance=a_list, method_name="remove", expected_args=(1,), expected_kwargs={})
         instance.remove(1)
         assert called[0]
         assert len(called) == 1
         assert instance == [2, 3]
 
     def test_list_sort(self, a_list):
-        instance, called = create_tester(a_list, "sort", (), {})
+        instance, called = create_tester(instance=a_list, method_name="sort", expected_args=(), expected_kwargs={})
         instance.sort()
         assert called[0]
         assert len(called) == 1
         assert instance == [1, 2, 3]
 
     def test_list___setitem__(self, a_list):
-        instance, called = create_tester(a_list, "setitem", (1, 4), {})
+        instance, called = create_tester(instance=a_list, method_name="setitem", expected_args=(1, 4), expected_kwargs={})
         instance[1] = 4
         assert called[0]
         assert len(called) == 1
         assert instance == [1, 4, 3]
```

### Comparing `bigbrother-0.1.2/bigbrother/tests/builtins/test_set.py` & `bigbrother-0.1.3/bigbrother/tests/builtins/test_set.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,61 +5,61 @@
 @fixture
 def a_set():
     return {1, 2, 3}
 
 
 class TestDict:
     def test_set_add(self, a_set):
-        instance, called = create_tester(a_set, "add", (4,), {})
+        instance, called = create_tester(instance=a_set, method_name="add", expected_args=(4,), expected_kwargs={})
         instance.add(4)
         assert called[0]
         assert len(called) == 1
         assert instance == {1, 2, 3, 4}
 
     def test_set_clear(self, a_set):
-        instance, called = create_tester(a_set, "clear", (), {})
+        instance, called = create_tester(instance=a_set, method_name="clear", expected_args=(), expected_kwargs={})
         instance.clear()
         assert called[0]
         assert len(called) == 1
         assert instance == set()
 
     def test_set_difference_update(self, a_set):
-        instance, called = create_tester(a_set, "difference_update", ({1, 2, 4},), {})
+        instance, called = create_tester(instance=a_set, method_name="difference_update", expected_args=({1, 2, 4},), expected_kwargs={})
         instance.difference_update({1, 2, 4})
         assert called[0]
         assert len(called) == 1
         assert instance == {3}
 
     def test_set_discard(self, a_set):
-        instance, called = create_tester(a_set, "discard", (1,), {})
+        instance, called = create_tester(instance=a_set, method_name="discard", expected_args=(1,), expected_kwargs={})
         instance.discard(1)
         assert called[0]
         assert len(called) == 1
         assert instance == {2, 3}
 
     def test_set_intersection_update(self, a_set):
-        instance, called = create_tester(a_set, "intersection_update", ({1, 3},), {})
+        instance, called = create_tester(instance=a_set, method_name="intersection_update", expected_args=({1, 3},), expected_kwargs={})
         instance.intersection_update({1, 3})
         assert called[0]
         assert len(called) == 1
         assert instance == {1, 3}
 
     def test_set_remove(self, a_set):
-        instance, called = create_tester(a_set, "remove", (1,), {})
+        instance, called = create_tester(instance=a_set, method_name="remove", expected_args=(1,), expected_kwargs={})
         instance.remove(1)
         assert called[0]
         assert len(called) == 1
         assert instance == {2, 3}
 
     def test_set_symmetric_difference_update(self, a_set):
-        instance, called = create_tester(a_set, "intersection_update", ({1, 3},), {})
+        instance, called = create_tester(instance=a_set, method_name="intersection_update", expected_args=({1, 3},), expected_kwargs={})
         instance.intersection_update({1, 3})
         assert called[0]
         assert len(called) == 1
         assert instance == {1, 3}
 
     def test_set_update(self, a_set):
-        instance, called = create_tester(a_set, "update", ({4, 5},), {})
+        instance, called = create_tester(instance=a_set, method_name="update", expected_args=({4, 5},), expected_kwargs={})
         instance.update({4, 5})
         assert called[0]
         assert len(called) == 1
         assert instance == {1, 2, 3, 4, 5}
```

### Comparing `bigbrother-0.1.2/bigbrother/tests/libraries/test_pydantic.py` & `bigbrother-0.1.3/bigbrother/tests/libraries/test_pydantic.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,41 +24,41 @@
 class TestPydantic:
     def test_pydantic_setattr(self):
         my_sub_model = MySubModel()
         my_other_sub_model = MyOtherSubModel()
         x = MyModel(a=my_sub_model, b=my_other_sub_model)
 
         x, called = create_tester(
-            x,
-            "setitem",
-            (
+            instance=x,
+            method_name="setitem",
+            expected_args=(
                 "d",
                 my_sub_model,
             ),
-            {},
+            expected_kwargs={},
         )
         x.d = my_sub_model
 
         assert called[0]
         assert len(called) == 1
         assert x.d == my_sub_model
 
     def test_pydantic_setattr_sub(self):
         my_sub_model = MySubModel()
         my_other_sub_model = MyOtherSubModel()
         x = MyModel(a=my_sub_model, b=my_other_sub_model)
 
         called = []
 
-        instance = x
+        instance = x.d
         method_name = "setitem"
         expected_args = ("x", [1])
         expected_kwargs = {}
 
-        def track_changes(obj, method, *args, **kwargs):
+        def track_changes(obj, method, ref, args, kwargs):
             called.append(True)
             print(f"method: {method} args: {args} kwargs: {kwargs}")
             assert obj == instance
             assert method == method_name
             assert args == expected_args
             assert kwargs == expected_kwargs
```

### Comparing `bigbrother-0.1.2/bigbrother.egg-info/PKG-INFO` & `bigbrother-0.1.3/bigbrother.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigbrother
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library for object observability
 Author-email: Tim Paine <t.paine154@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -233,27 +233,43 @@
 ## Overview
 `bigbrother` is a mutation observer library. You can use it to watch your objects for changes. When your object changes, `bigbrother` will trigger your choice of callback. 
 
 
 ```python
 x = {1: "a", 2: "b", 3: "c"}
 
-def track_changes(obj, method, *args, **kwargs):
+def track_changes(obj, method, ref, call_args, call_kwargs):
     print(f"method: {method}, args: {args}, kwargs: {kwargs}")
 
 x = watch(x, track_changes)
 
 x[1] = "x"
 
 # prints: method: setitem, args: (1, 'x'), kwargs: {}
 ```
 
 `bigbrother` can also embed itself recursively in your object by passing in argument `deepstate=True`.
 
 
+## Callback
+
+```python
+def callback(obj, method, ref, call_args, call_kwargs):
+    '''Callback called when object is mutated
+
+    Args:
+        obj (Any): The object being mutated via `method`
+        method (str): The method called on the object (dunders removed)
+        ref (Any): Reference object. If callback installed recursively, `ref` will be the entrypoint
+        call_args (Tuple[Any]): Positional arguments that `method` was called with on `obj`
+        call_kwargs (Dict[Any, Any]): Keyword arguments that `method` was called with on `obj`
+    '''
+```
+
+
 ## Supported types
 
 ### Builtins
 Most builtin types are read-only and cannot have their method structure mutated, so we observe via replacement with thin wrappers. 
 
 - `list` via `_ObservedList`
     - `append`
```

### Comparing `bigbrother-0.1.2/bigbrother.egg-info/SOURCES.txt` & `bigbrother-0.1.3/bigbrother.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bigbrother-0.1.2/pyproject.toml` & `bigbrother-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [project]
 name = "bigbrother"
 authors = [{name = "Tim Paine", email = "t.paine154@gmail.com"}]
 description="A library for object observability"
 readme = "README.md"
 license = { file = "LICENSE" }
-version = "0.1.2"
+version = "0.1.3"
 requires-python = ">=3.8"
 keywords = ["observer", "observer-pattern"]
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
```

