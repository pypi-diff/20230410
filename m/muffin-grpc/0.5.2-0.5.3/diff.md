# Comparing `tmp/muffin_grpc-0.5.2.tar.gz` & `tmp/muffin_grpc-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin_grpc-0.5.2.tar", max compression
+gzip compressed data, was "muffin_grpc-0.5.3.tar", max compression
```

## Comparing `muffin_grpc-0.5.2.tar` & `muffin_grpc-0.5.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6014 2023-04-10 12:01:56.214063 muffin_grpc-0.5.2/README.rst
--rw-r--r--   0        0        0     6875 2023-04-10 12:01:56.218063 muffin_grpc-0.5.2/muffin_grpc/__init__.py
--rw-r--r--   0        0        0    11986 2023-04-10 12:01:56.218063 muffin_grpc-0.5.2/muffin_grpc/proto3.py
--rw-r--r--   0        0        0        0 2023-04-10 12:01:56.218063 muffin_grpc-0.5.2/muffin_grpc/py.typed
--rw-r--r--   0        0        0     1420 2023-04-10 12:01:56.218063 muffin_grpc-0.5.2/muffin_grpc/utils.py
--rw-r--r--   0        0        0     1957 2023-04-10 12:01:56.218063 muffin_grpc-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     7241 1970-01-01 00:00:00.000000 muffin_grpc-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     6014 2023-04-10 12:22:51.405689 muffin_grpc-0.5.3/README.rst
+-rw-r--r--   0        0        0     6947 2023-04-10 12:22:51.405689 muffin_grpc-0.5.3/muffin_grpc/__init__.py
+-rw-r--r--   0        0        0    11986 2023-04-10 12:22:51.405689 muffin_grpc-0.5.3/muffin_grpc/proto3.py
+-rw-r--r--   0        0        0        0 2023-04-10 12:22:51.405689 muffin_grpc-0.5.3/muffin_grpc/py.typed
+-rw-r--r--   0        0        0     1420 2023-04-10 12:22:51.405689 muffin_grpc-0.5.3/muffin_grpc/utils.py
+-rw-r--r--   0        0        0     1957 2023-04-10 12:22:51.405689 muffin_grpc-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     7241 1970-01-01 00:00:00.000000 muffin_grpc-0.5.3/PKG-INFO
```

### Comparing `muffin_grpc-0.5.2/README.rst` & `muffin_grpc-0.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `muffin_grpc-0.5.2/muffin_grpc/__init__.py` & `muffin_grpc-0.5.3/muffin_grpc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,17 @@
             return self.build_proto(
                 path,
                 build_dir=build_dir,
                 build_package=build_package,
                 targets=targets,
             )
 
+        else:
+            return [build_dir / f"{ path.stem }_pb2.py"]
+
     def add_to_server(self, service_cls):
         """Register the given service class to the server."""
         proto_cls = service_cls.mro()[-2]
         proto_module = import_module(proto_cls.__module__)
         register = getattr(proto_module, f"add_{ proto_cls.__name__ }_to_server")
         self.services.append((service_cls, register))
```

### Comparing `muffin_grpc-0.5.2/muffin_grpc/proto3.py` & `muffin_grpc-0.5.3/muffin_grpc/proto3.py`

 * *Files identical despite different names*

### Comparing `muffin_grpc-0.5.2/muffin_grpc/utils.py` & `muffin_grpc-0.5.3/muffin_grpc/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_grpc-0.5.2/pyproject.toml` & `muffin_grpc-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin-grpc"
-version = "0.5.2"
+version = "0.5.3"
 description = "GRPC support for Muffin framework."
 readme = "README.rst"
 homepage = "https://github.com/klen/muffin-grpc"
 repository = "https://github.com/klen/muffin-grpc"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["grpc", "muffin", "asyncio", "asgi", "web"]
```

### Comparing `muffin_grpc-0.5.2/PKG-INFO` & `muffin_grpc-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin-grpc
-Version: 0.5.2
+Version: 0.5.3
 Summary: GRPC support for Muffin framework.
 Home-page: https://github.com/klen/muffin-grpc
 License: MIT
 Keywords: grpc,muffin,asyncio,asgi,web
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

