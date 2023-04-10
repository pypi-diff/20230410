# Comparing `tmp/lessweb-1.0.6.tar.gz` & `tmp/lessweb-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lessweb-1.0.6.tar", last modified: Mon Apr 10 03:57:05 2023, max compression
+gzip compressed data, was "lessweb-1.0.7.tar", last modified: Mon Apr 10 04:55:52 2023, max compression
```

## Comparing `lessweb-1.0.6.tar` & `lessweb-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-04-10 03:57:05.473904 lessweb-1.0.6/
--rw-r--r--   0 zhangji    (501) staff       (20)      556 2022-11-14 08:34:51.000000 lessweb-1.0.6/LICENSE.txt
--rw-r--r--   0 zhangji    (501) staff       (20)      356 2023-04-10 03:57:05.473427 lessweb-1.0.6/PKG-INFO
--rw-r--r--   0 zhangji    (501) staff       (20)     1649 2022-12-06 09:47:53.000000 lessweb-1.0.6/README.md
-drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-04-10 03:57:05.464688 lessweb-1.0.6/lessweb/
--rw-r--r--   0 zhangji    (501) staff       (20)      255 2023-04-10 02:14:16.000000 lessweb-1.0.6/lessweb/__init__.py
--rw-r--r--   0 zhangji    (501) staff       (20)    14482 2023-04-10 03:54:50.000000 lessweb-1.0.6/lessweb/bridge.py
--rw-r--r--   0 zhangji    (501) staff       (20)        0 2023-01-14 08:15:49.000000 lessweb-1.0.6/lessweb/py.typed
--rw-r--r--   0 zhangji    (501) staff       (20)     7860 2023-01-14 07:25:23.000000 lessweb-1.0.6/lessweb/typecast.py
-drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-04-10 03:57:05.472151 lessweb-1.0.6/lessweb.egg-info/
--rw-r--r--   0 zhangji    (501) staff       (20)      356 2023-04-10 03:57:05.000000 lessweb-1.0.6/lessweb.egg-info/PKG-INFO
--rw-r--r--   0 zhangji    (501) staff       (20)      293 2023-04-10 03:57:05.000000 lessweb-1.0.6/lessweb.egg-info/SOURCES.txt
--rw-r--r--   0 zhangji    (501) staff       (20)        1 2023-04-10 03:57:05.000000 lessweb-1.0.6/lessweb.egg-info/dependency_links.txt
--rw-r--r--   0 zhangji    (501) staff       (20)       20 2023-04-10 03:57:05.000000 lessweb-1.0.6/lessweb.egg-info/entry_points.txt
--rw-r--r--   0 zhangji    (501) staff       (20)       43 2023-04-10 03:57:05.000000 lessweb-1.0.6/lessweb.egg-info/requires.txt
--rw-r--r--   0 zhangji    (501) staff       (20)        8 2023-04-10 03:57:05.000000 lessweb-1.0.6/lessweb.egg-info/top_level.txt
--rw-r--r--   0 zhangji    (501) staff       (20)       38 2023-04-10 03:57:05.474050 lessweb-1.0.6/setup.cfg
--rw-r--r--   0 zhangji    (501) staff       (20)     1124 2023-01-14 09:41:41.000000 lessweb-1.0.6/setup.py
+drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-04-10 04:55:52.587458 lessweb-1.0.7/
+-rw-r--r--   0 zhangji    (501) staff       (20)      556 2022-11-14 08:34:51.000000 lessweb-1.0.7/LICENSE.txt
+-rw-r--r--   0 zhangji    (501) staff       (20)      356 2023-04-10 04:55:52.586660 lessweb-1.0.7/PKG-INFO
+-rw-r--r--   0 zhangji    (501) staff       (20)     1649 2022-12-06 09:47:53.000000 lessweb-1.0.7/README.md
+drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-04-10 04:55:52.576064 lessweb-1.0.7/lessweb/
+-rw-r--r--   0 zhangji    (501) staff       (20)      255 2023-04-10 04:54:53.000000 lessweb-1.0.7/lessweb/__init__.py
+-rw-r--r--   0 zhangji    (501) staff       (20)    14206 2023-04-10 04:54:53.000000 lessweb-1.0.7/lessweb/bridge.py
+-rw-r--r--   0 zhangji    (501) staff       (20)        0 2023-01-14 08:15:49.000000 lessweb-1.0.7/lessweb/py.typed
+-rw-r--r--   0 zhangji    (501) staff       (20)     7860 2023-01-14 07:25:23.000000 lessweb-1.0.7/lessweb/typecast.py
+drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-04-10 04:55:52.585582 lessweb-1.0.7/lessweb.egg-info/
+-rw-r--r--   0 zhangji    (501) staff       (20)      356 2023-04-10 04:55:52.000000 lessweb-1.0.7/lessweb.egg-info/PKG-INFO
+-rw-r--r--   0 zhangji    (501) staff       (20)      293 2023-04-10 04:55:52.000000 lessweb-1.0.7/lessweb.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangji    (501) staff       (20)        1 2023-04-10 04:55:52.000000 lessweb-1.0.7/lessweb.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangji    (501) staff       (20)       20 2023-04-10 04:55:52.000000 lessweb-1.0.7/lessweb.egg-info/entry_points.txt
+-rw-r--r--   0 zhangji    (501) staff       (20)       43 2023-04-10 04:55:52.000000 lessweb-1.0.7/lessweb.egg-info/requires.txt
+-rw-r--r--   0 zhangji    (501) staff       (20)        8 2023-04-10 04:55:52.000000 lessweb-1.0.7/lessweb.egg-info/top_level.txt
+-rw-r--r--   0 zhangji    (501) staff       (20)       38 2023-04-10 04:55:52.587725 lessweb-1.0.7/setup.cfg
+-rw-r--r--   0 zhangji    (501) staff       (20)     1124 2023-01-14 09:41:41.000000 lessweb-1.0.7/setup.py
```

### Comparing `lessweb-1.0.6/LICENSE.txt` & `lessweb-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lessweb-1.0.6/README.md` & `lessweb-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `lessweb-1.0.6/lessweb/bridge.py` & `lessweb-1.0.7/lessweb/bridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,63 +266,61 @@
 
     return aio_endpoint
 
 
 @dataclass
 class Route:
     method: str
-    path: str
-    paths: Optional[list]
+    paths: list
     handler: Any
 
 
-def rest_mapping(method: str, path: str, paths: list=None):
+def rest_mapping(method: str, paths: list):
     def g(sp_endpoint) -> Route:
         handler = make_router(sp_endpoint)
-        assert bool(path) ^ bool(paths), 'Only one of path and paths must be non-empty value.'
-        route = Route(method=method.upper(), path=path, paths=paths, handler=handler)
+        route = Route(method=method.upper(), paths=paths, handler=handler)
         route.__doc__ = inspect.getdoc(sp_endpoint)
         return route
 
     return g
 
 
 def get_mapping(path: str):
     def g(sp_endpoint) -> Route:
         handler = make_router(sp_endpoint)
-        return rest_mapping(method='GET', path=path)(sp_endpoint)
+        return rest_mapping(method='GET', paths=[path])(sp_endpoint)
 
     return g
 
 
 def post_mapping(path: str):
     def g(sp_endpoint) -> Route:
         handler = make_router(sp_endpoint)
-        return rest_mapping(method='POST', path=path)(sp_endpoint)
+        return rest_mapping(method='POST', paths=[path])(sp_endpoint)
 
     return g
 
 
 def put_mapping(path: str):
     def g(sp_endpoint) -> Route:
-        return rest_mapping(method='PUT', path=path)(sp_endpoint)
+        return rest_mapping(method='PUT', paths=[path])(sp_endpoint)
 
     return g
 
 
 def patch_mapping(path: str):
     def g(sp_endpoint) -> Route:
-        return rest_mapping(method='PATCH', path=path)(sp_endpoint)
+        return rest_mapping(method='PATCH', paths=[path])(sp_endpoint)
 
     return g
 
 
 def delete_mapping(path: str):
     def g(sp_endpoint) -> Route:
-        return rest_mapping(method='DELETE', path=path)(sp_endpoint)
+        return rest_mapping(method='DELETE', paths=[path])(sp_endpoint)
 
     return g
 
 
 class Bridge:
     app: Application
     config: Optional[str]
@@ -408,19 +406,16 @@
 
         self.app.cleanup_ctx.append(aio_handler)
 
     def add_on_shutdown(self, handler):
         self.app.on_shutdown.append(make_app_signal(handler))
 
     def add_route(self, route):
-        if route.paths:
-            for path in route.paths:
-                self.app.router.add_route(method=route.method, path=path, handler=route.handler)
-        else:
-            self.app.router.add_route(method=route.method, path=route.path, handler=route.handler)
+        for path in route.paths:
+            self.app.router.add_route(method=route.method, path=path, handler=route.handler)
 
     def add_route_scan(self, endpoint_package: str):
         endpoint_mdl = importlib.import_module(endpoint_package)
         for filename in listdir(endpoint_mdl.__spec__.submodule_search_locations[0]):
             if filename.endswith('.py'):
                 sub_mdl = importlib.import_module(f'{endpoint_package}.{filename[:-3]}')
                 for item in sub_mdl.__dict__.values():
```

### Comparing `lessweb-1.0.6/lessweb/typecast.py` & `lessweb-1.0.7/lessweb/typecast.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.0.6/setup.py` & `lessweb-1.0.7/setup.py`

 * *Files identical despite different names*

