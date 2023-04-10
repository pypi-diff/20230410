# Comparing `tmp/muffin-grpc-0.5.0.tar.gz` & `tmp/muffin_grpc-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin-grpc-0.5.0.tar", last modified: Sat Mar  4 11:55:11 2023, max compression
+gzip compressed data, was "muffin_grpc-0.5.1.tar", max compression
```

## Comparing `muffin-grpc-0.5.0.tar` & `muffin_grpc-0.5.1.tar`

### file list

```diff
@@ -1,19 +1,7 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 11:55:11.353492 muffin-grpc-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-04 11:54:58.000000 muffin-grpc-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-03-04 11:55:11.353492 muffin-grpc-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-03-04 11:54:58.000000 muffin-grpc-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 11:55:11.353492 muffin-grpc-0.5.0/muffin_grpc/
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-03-04 11:54:58.000000 muffin-grpc-0.5.0/muffin_grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-03-04 11:54:58.000000 muffin-grpc-0.5.0/muffin_grpc/proto3.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 11:54:58.000000 muffin-grpc-0.5.0/muffin_grpc/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-04 11:54:58.000000 muffin-grpc-0.5.0/muffin_grpc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 11:55:11.353492 muffin-grpc-0.5.0/muffin_grpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-03-04 11:55:11.000000 muffin-grpc-0.5.0/muffin_grpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-04 11:55:11.000000 muffin-grpc-0.5.0/muffin_grpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 11:55:11.000000 muffin-grpc-0.5.0/muffin_grpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-04 11:55:11.000000 muffin-grpc-0.5.0/muffin_grpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-04 11:55:11.000000 muffin-grpc-0.5.0/muffin_grpc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-03-04 11:54:58.000000 muffin-grpc-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-04 11:55:11.353492 muffin-grpc-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 11:55:11.353492 muffin-grpc-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-03-04 11:54:58.000000 muffin-grpc-0.5.0/tests/test_base.py
+-rw-r--r--   0        0        0     6014 2023-04-10 11:59:59.534705 muffin_grpc-0.5.1/README.rst
+-rw-r--r--   0        0        0     6875 2023-04-10 11:59:59.534705 muffin_grpc-0.5.1/muffin_grpc/__init__.py
+-rw-r--r--   0        0        0    11986 2023-04-10 11:59:59.534705 muffin_grpc-0.5.1/muffin_grpc/proto3.py
+-rw-r--r--   0        0        0        0 2023-04-10 11:59:59.534705 muffin_grpc-0.5.1/muffin_grpc/py.typed
+-rw-r--r--   0        0        0     1420 2023-04-10 11:59:59.534705 muffin_grpc-0.5.1/muffin_grpc/utils.py
+-rw-r--r--   0        0        0     1957 2023-04-10 11:59:59.538705 muffin_grpc-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     7241 1970-01-01 00:00:00.000000 muffin_grpc-0.5.1/PKG-INFO
```

### Comparing `muffin-grpc-0.5.0/PKG-INFO` & `muffin_grpc-0.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: muffin-grpc
-Version: 0.5.0
+Version: 0.5.1
 Summary: GRPC support for Muffin framework.
-Author-email: Kirill Klenov <horneds@gmail.com>
-License: MIT License
-Project-URL: homepage, https://github.com/klen/muffin-grpc
-Project-URL: repository, https://github.com/klen/muffin-grpc
+Home-page: https://github.com/klen/muffin-grpc
+License: MIT
 Keywords: grpc,muffin,asyncio,asgi,web
+Author: Kirill Klenov
+Author-email: horneds@gmail.com
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Framework :: AsyncIO
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: grpcio (>=1,<2)
+Requires-Dist: grpcio-tools (>=1,<2)
+Requires-Dist: muffin (>=0,<1)
+Requires-Dist: parsy
+Project-URL: Repository, https://github.com/klen/muffin-grpc
 Description-Content-Type: text/x-rst
-Provides-Extra: tests
-Provides-Extra: dev
-Provides-Extra: yaml
-Provides-Extra: example
 
 Muffin-GRPC
 ############
 
 .. _description:
 
 Muffin-GRPC -- GRPC support for Muffin_ framework.
@@ -52,15 +58,15 @@
 .. contents::
 
 .. _requirements:
 
 Requirements
 =============
 
-- python >= 3.7
+- python >= 3.8
 
 .. note:: The plugin supports only asyncio evenloop (not trio)
 
 .. _installation:
 
 Installation
 =============
@@ -175,26 +181,26 @@
 The ``/`` endpoint will make a request to the GRPC server and return a message
 from the server.
 
 
 Configuration options
 ----------------------
 
-=========================== ======================================= =========================== 
+=========================== ======================================= ===========================
 Name                        Default value                           Desctiption
 --------------------------- --------------------------------------- ---------------------------
 **build_dir**               ``None``                                A directory to build proto files
 **server_listen**           ``"[::]:50051"``                        Server address
 **ssl_server**              ``False``                               Enable SSL for server
 **ssl_server_params**       ``None``                                SSL Server Params
 **ssl_client**              ``False``                               Enable SSL for client
 **ssl_client_params**       ``None``                                SSL Client Params
 **default_channel**         ``localhost:50051``                     Default Client Channel Address
 **default_channel_options** ``{}``                                  GRPC options for the default channel
-=========================== ======================================= =========================== 
+=========================== ======================================= ===========================
 
 You are able to provide the options when you are initiliazing the plugin:
 
 .. code-block:: python
 
     grpc.setup(app, server_listen='localhost:40000')
 
@@ -263,7 +269,8 @@
 
 .. _links:
 
 
 .. _klen: https://github.com/klen
 .. _Muffin: https://github.com/klen/muffin
 .. _MIT license: http://opensource.org/licenses/MIT
+
```

### Comparing `muffin-grpc-0.5.0/README.rst` & `muffin_grpc-0.5.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 .. contents::
 
 .. _requirements:
 
 Requirements
 =============
 
-- python >= 3.7
+- python >= 3.8
 
 .. note:: The plugin supports only asyncio evenloop (not trio)
 
 .. _installation:
 
 Installation
 =============
@@ -149,26 +149,26 @@
 The ``/`` endpoint will make a request to the GRPC server and return a message
 from the server.
 
 
 Configuration options
 ----------------------
 
-=========================== ======================================= =========================== 
+=========================== ======================================= ===========================
 Name                        Default value                           Desctiption
 --------------------------- --------------------------------------- ---------------------------
 **build_dir**               ``None``                                A directory to build proto files
 **server_listen**           ``"[::]:50051"``                        Server address
 **ssl_server**              ``False``                               Enable SSL for server
 **ssl_server_params**       ``None``                                SSL Server Params
 **ssl_client**              ``False``                               Enable SSL for client
 **ssl_client_params**       ``None``                                SSL Client Params
 **default_channel**         ``localhost:50051``                     Default Client Channel Address
 **default_channel_options** ``{}``                                  GRPC options for the default channel
-=========================== ======================================= =========================== 
+=========================== ======================================= ===========================
 
 You are able to provide the options when you are initiliazing the plugin:
 
 .. code-block:: python
 
     grpc.setup(app, server_listen='localhost:40000')
```

### Comparing `muffin-grpc-0.5.0/muffin_grpc/__init__.py` & `muffin_grpc-0.5.1/muffin_grpc/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Support GRPC for Muffin Framework."""
 import asyncio
 import logging
 from functools import cached_property
 from importlib import import_module
 from pathlib import Path
 from signal import SIGINT, SIGTERM
-from typing import TYPE_CHECKING, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 import grpc
 from grpc_tools import protoc
 from muffin.plugins import BasePlugin, PluginError
 from pkg_resources import resource_filename
 
 from .utils import _fix_imports, _generate_file, _is_newer, _parse_proto
@@ -37,15 +37,17 @@
         "ssl_server_params": None,
     }
     logger = logging.getLogger("muffin-grpc")
 
     def __init__(self, *args, **kwargs):
         """Initialize the plugin."""
         super(Plugin, self).__init__(*args, **kwargs)
-        self.proto_files = []
+        self.proto_files: List[
+            Tuple[Union[str, Path], Optional[Union[str, Path]], Dict[str, Any]]
+        ] = []
         self.services = []
 
     def setup(self, app: "Application", **options):
         """Setup grpc commands."""
         super(Plugin, self).setup(app, **options)
         self.logger = app.logger
 
@@ -61,17 +63,17 @@
             loop.add_signal_handler(SIGTERM, stop.set)
             await stop.wait()
             await self.server.stop(2)
 
         @app.manage
         async def grpc_build():
             """Build registered proto files."""
-            for path, build_dir in self.proto_files:
+            for path, build_dir, params in self.proto_files:
                 self.logger.warning("Build: %s", path)
-                self.build_proto(path, build_dir=build_dir)
+                self.build_proto(path, build_dir=build_dir, **params)
 
         # TODO: Proto specs
         # -----------------
         #  @app.route('proto/specs')
         #  async def proto_specs(request):
         #      pass
 
@@ -98,18 +100,23 @@
         build_dir: Optional[Union[str, Path]] = None,
         build_package: Optional[str] = None,
         targets: Optional[List[Path]] = None,
     ):
         """Register/build the given proto file."""
         path = Path(path).absolute()
         build_dir = Path(build_dir or self.cfg.build_dir or path.parent)
-        self.proto_files.append((path, build_dir))
+        self.proto_files.append(
+            (path, build_dir, {"build_package": build_package, "targets": targets}),
+        )
         if self.cfg.autobuild:
             return self.build_proto(
-                path, build_dir=build_dir, build_package=build_package, targets=targets,
+                path,
+                build_dir=build_dir,
+                build_package=build_package,
+                targets=targets,
             )
 
     def add_to_server(self, service_cls):
         """Register the given service class to the server."""
         proto_cls = service_cls.mro()[-2]
         proto_module = import_module(proto_cls.__module__)
         register = getattr(proto_module, f"add_{ proto_cls.__name__ }_to_server")
@@ -151,15 +158,16 @@
             build_package = package
 
         targets = targets or []
         targets = targets + [
             target
             for name in imports
             for target in self.build_proto(
-                path.parent / name, build_dir=build_dir / Path(name).parent,
+                path.parent / name,
+                build_dir=build_dir / Path(name).parent,
             )
         ]
 
         args = []
         target_pb2 = build_dir / f"{ path.stem }_pb2.py"
         targets.append(target_pb2)
         if not _is_newer(target_pb2, proto_updated):
```

### Comparing `muffin-grpc-0.5.0/muffin_grpc/proto3.py` & `muffin_grpc-0.5.1/muffin_grpc/proto3.py`

 * *Files identical despite different names*

### Comparing `muffin-grpc-0.5.0/muffin_grpc/utils.py` & `muffin_grpc-0.5.1/muffin_grpc/utils.py`

 * *Files identical despite different names*

