# Comparing `tmp/lessweb-1.0.5.tar.gz` & `tmp/lessweb-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lessweb-1.0.5.tar", last modified: Wed Feb 15 00:23:11 2023, max compression
+gzip compressed data, was "lessweb-1.0.6.tar", last modified: Mon Apr 10 03:57:05 2023, max compression
```

## Comparing `lessweb-1.0.5.tar` & `lessweb-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-02-15 00:23:11.651720 lessweb-1.0.5/
--rw-r--r--   0 zhangji    (501) staff       (20)      556 2022-11-14 08:34:51.000000 lessweb-1.0.5/LICENSE.txt
--rw-r--r--   0 zhangji    (501) staff       (20)      356 2023-02-15 00:23:11.650536 lessweb-1.0.5/PKG-INFO
--rw-r--r--   0 zhangji    (501) staff       (20)     1649 2022-12-06 09:47:53.000000 lessweb-1.0.5/README.md
-drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-02-15 00:23:11.641257 lessweb-1.0.5/lessweb/
--rw-r--r--   0 zhangji    (501) staff       (20)      255 2023-02-15 00:22:25.000000 lessweb-1.0.5/lessweb/__init__.py
--rw-r--r--   0 zhangji    (501) staff       (20)    14160 2023-02-15 00:22:05.000000 lessweb-1.0.5/lessweb/bridge.py
--rw-r--r--   0 zhangji    (501) staff       (20)        0 2023-01-14 08:15:49.000000 lessweb-1.0.5/lessweb/py.typed
--rw-r--r--   0 zhangji    (501) staff       (20)     7860 2023-01-14 07:25:23.000000 lessweb-1.0.5/lessweb/typecast.py
-drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-02-15 00:23:11.649796 lessweb-1.0.5/lessweb.egg-info/
--rw-r--r--   0 zhangji    (501) staff       (20)      356 2023-02-15 00:23:11.000000 lessweb-1.0.5/lessweb.egg-info/PKG-INFO
--rw-r--r--   0 zhangji    (501) staff       (20)      293 2023-02-15 00:23:11.000000 lessweb-1.0.5/lessweb.egg-info/SOURCES.txt
--rw-r--r--   0 zhangji    (501) staff       (20)        1 2023-02-15 00:23:11.000000 lessweb-1.0.5/lessweb.egg-info/dependency_links.txt
--rw-r--r--   0 zhangji    (501) staff       (20)       20 2023-02-15 00:23:11.000000 lessweb-1.0.5/lessweb.egg-info/entry_points.txt
--rw-r--r--   0 zhangji    (501) staff       (20)       43 2023-02-15 00:23:11.000000 lessweb-1.0.5/lessweb.egg-info/requires.txt
--rw-r--r--   0 zhangji    (501) staff       (20)        8 2023-02-15 00:23:11.000000 lessweb-1.0.5/lessweb.egg-info/top_level.txt
--rw-r--r--   0 zhangji    (501) staff       (20)       38 2023-02-15 00:23:11.652693 lessweb-1.0.5/setup.cfg
--rw-r--r--   0 zhangji    (501) staff       (20)     1124 2023-01-14 09:41:41.000000 lessweb-1.0.5/setup.py
+drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-04-10 03:57:05.473904 lessweb-1.0.6/
+-rw-r--r--   0 zhangji    (501) staff       (20)      556 2022-11-14 08:34:51.000000 lessweb-1.0.6/LICENSE.txt
+-rw-r--r--   0 zhangji    (501) staff       (20)      356 2023-04-10 03:57:05.473427 lessweb-1.0.6/PKG-INFO
+-rw-r--r--   0 zhangji    (501) staff       (20)     1649 2022-12-06 09:47:53.000000 lessweb-1.0.6/README.md
+drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-04-10 03:57:05.464688 lessweb-1.0.6/lessweb/
+-rw-r--r--   0 zhangji    (501) staff       (20)      255 2023-04-10 02:14:16.000000 lessweb-1.0.6/lessweb/__init__.py
+-rw-r--r--   0 zhangji    (501) staff       (20)    14482 2023-04-10 03:54:50.000000 lessweb-1.0.6/lessweb/bridge.py
+-rw-r--r--   0 zhangji    (501) staff       (20)        0 2023-01-14 08:15:49.000000 lessweb-1.0.6/lessweb/py.typed
+-rw-r--r--   0 zhangji    (501) staff       (20)     7860 2023-01-14 07:25:23.000000 lessweb-1.0.6/lessweb/typecast.py
+drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-04-10 03:57:05.472151 lessweb-1.0.6/lessweb.egg-info/
+-rw-r--r--   0 zhangji    (501) staff       (20)      356 2023-04-10 03:57:05.000000 lessweb-1.0.6/lessweb.egg-info/PKG-INFO
+-rw-r--r--   0 zhangji    (501) staff       (20)      293 2023-04-10 03:57:05.000000 lessweb-1.0.6/lessweb.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangji    (501) staff       (20)        1 2023-04-10 03:57:05.000000 lessweb-1.0.6/lessweb.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangji    (501) staff       (20)       20 2023-04-10 03:57:05.000000 lessweb-1.0.6/lessweb.egg-info/entry_points.txt
+-rw-r--r--   0 zhangji    (501) staff       (20)       43 2023-04-10 03:57:05.000000 lessweb-1.0.6/lessweb.egg-info/requires.txt
+-rw-r--r--   0 zhangji    (501) staff       (20)        8 2023-04-10 03:57:05.000000 lessweb-1.0.6/lessweb.egg-info/top_level.txt
+-rw-r--r--   0 zhangji    (501) staff       (20)       38 2023-04-10 03:57:05.474050 lessweb-1.0.6/setup.cfg
+-rw-r--r--   0 zhangji    (501) staff       (20)     1124 2023-01-14 09:41:41.000000 lessweb-1.0.6/setup.py
```

### Comparing `lessweb-1.0.5/LICENSE.txt` & `lessweb-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lessweb-1.0.5/README.md` & `lessweb-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `lessweb-1.0.5/lessweb/bridge.py` & `lessweb-1.0.6/lessweb/bridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from aiohttp.web import Request, Application, Response, middleware, HTTPBadRequest, HTTPError, Type, run_app
+from aiohttp.web import Request, Application, Response, middleware, HTTPBadRequest, HTTPError, run_app
 from aiohttp.typedefs import LooseHeaders
 from dataclasses import dataclass
 import importlib
 import inspect
 import logging
 from logging.handlers import TimedRotatingFileHandler
 import orjson
@@ -267,21 +267,23 @@
     return aio_endpoint
 
 
 @dataclass
 class Route:
     method: str
     path: str
+    paths: Optional[list]
     handler: Any
 
 
-def rest_mapping(method: str, path: str):
+def rest_mapping(method: str, path: str, paths: list=None):
     def g(sp_endpoint) -> Route:
         handler = make_router(sp_endpoint)
-        route = Route(method=method.upper(), path=path, handler=handler)
+        assert bool(path) ^ bool(paths), 'Only one of path and paths must be non-empty value.'
+        route = Route(method=method.upper(), path=path, paths=paths, handler=handler)
         route.__doc__ = inspect.getdoc(sp_endpoint)
         return route
 
     return g
 
 
 def get_mapping(path: str):
@@ -406,15 +408,19 @@
 
         self.app.cleanup_ctx.append(aio_handler)
 
     def add_on_shutdown(self, handler):
         self.app.on_shutdown.append(make_app_signal(handler))
 
     def add_route(self, route):
-        self.app.router.add_route(method=route.method, path=route.path, handler=route.handler)
+        if route.paths:
+            for path in route.paths:
+                self.app.router.add_route(method=route.method, path=path, handler=route.handler)
+        else:
+            self.app.router.add_route(method=route.method, path=route.path, handler=route.handler)
 
     def add_route_scan(self, endpoint_package: str):
         endpoint_mdl = importlib.import_module(endpoint_package)
         for filename in listdir(endpoint_mdl.__spec__.submodule_search_locations[0]):
             if filename.endswith('.py'):
                 sub_mdl = importlib.import_module(f'{endpoint_package}.{filename[:-3]}')
                 for item in sub_mdl.__dict__.values():
```

### Comparing `lessweb-1.0.5/lessweb/typecast.py` & `lessweb-1.0.6/lessweb/typecast.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.0.5/setup.py` & `lessweb-1.0.6/setup.py`

 * *Files identical despite different names*

