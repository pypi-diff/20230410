# Comparing `tmp/lisf-0.1.2.tar.gz` & `tmp/lisf-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lisf-0.1.2.tar", max compression
+gzip compressed data, was "lisf-0.1.3.tar", max compression
```

## Comparing `lisf-0.1.2.tar` & `lisf-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2336 2023-04-09 18:17:29.905578 lisf-0.1.2/lisf.py
--rw-r--r--   0        0        0      424 2023-04-09 18:51:14.046125 lisf-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      532 1970-01-01 00:00:00.000000 lisf-0.1.2/setup.py
--rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 lisf-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2662 2023-04-10 05:46:54.116518 lisf-0.1.3/lisf.py
+-rw-r--r--   0        0        0      405 2023-04-10 05:51:43.589097 lisf-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 lisf-0.1.3/setup.py
+-rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 lisf-0.1.3/PKG-INFO
```

### Comparing `lisf-0.1.2/lisf.py` & `lisf-0.1.3/lisf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,50 @@
+import asyncio
 from contextlib import contextmanager
+from inspect import iscoroutinefunction
 import sys
 import types
-from asgiref import sync
+from functools import partial
+
 
 nothing = object()
 
 
 class Module(types.ModuleType):
     _cache = {}
     _lazy_loaders = {}
 
     def register_loader(self, key, lazy_loader, rewrite=False):
         current_loader = self._lazy_loaders.get(key, None)
         assert callable(lazy_loader)
         assert rewrite is True or current_loader is None
-        if sync.iscoroutinefunction(lazy_loader):
-            lazy_loader = sync.async_to_sync(lazy_loader)
         self._lazy_loaders[key] = lazy_loader
         return current_loader
 
     def get(self, key):
         try:
             value = self._cache[key]
         except KeyError:
             if key in self._lazy_loaders:
                 loader = self._lazy_loaders[key]
-                value = loader()
+                if iscoroutinefunction(loader):
+                    fut = asyncio.ensure_future(loader())
+                    setter = partial(self.set_from_future, key,)
+                    fut.add_done_callback(setter)
+                    value = fut
+                else:
+                    value = loader()
                 self.set(key, value)
             else:
                 raise
         return value
 
+    def set_from_future(self, key, fut: asyncio.Future):
+        self.set(key, fut.result())
+
     def set(self, key, value):
         self._cache[key] = value
         return value
 
     def pop(self, key, default=None):
         result = self._cache.pop(key, default)
         return result
```

