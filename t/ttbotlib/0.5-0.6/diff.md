# Comparing `tmp/ttbotlib-0.5.tar.gz` & `tmp/ttbotlib-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttbotlib-0.5.tar", last modified: Thu Feb 16 14:22:37 2023, max compression
+gzip compressed data, was "ttbotlib-0.6.tar", last modified: Mon Apr 10 17:01:42 2023, max compression
```

## Comparing `ttbotlib-0.5.tar` & `ttbotlib-0.6.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxr-xr-x   0 scailer   (1000) users      (985)        0 2023-02-16 14:22:37.052533 ttbotlib-0.5/
--rw-r--r--   0 scailer   (1000) users      (985)     1070 2020-01-16 11:25:02.000000 ttbotlib-0.5/LICENSE.md
--rw-r--r--   0 scailer   (1000) users      (985)      750 2023-02-16 14:22:37.052533 ttbotlib-0.5/PKG-INFO
--rw-r--r--   0 scailer   (1000) users      (985)     2548 2023-02-16 13:57:02.000000 ttbotlib-0.5/README.md
--rw-r--r--   0 scailer   (1000) users      (985)     1648 2023-02-16 14:22:37.052533 ttbotlib-0.5/setup.cfg
--rw-r--r--   0 scailer   (1000) users      (985)      788 2023-02-15 15:22:13.000000 ttbotlib-0.5/setup.py
-drwxr-xr-x   0 scailer   (1000) users      (985)        0 2023-02-16 14:22:37.052533 ttbotlib-0.5/tests/
--rw-r--r--   0 scailer   (1000) users      (985)     1442 2023-02-16 13:17:00.000000 ttbotlib-0.5/tests/test_client.py
--rw-r--r--   0 scailer   (1000) users      (985)     4629 2023-02-16 13:31:45.000000 ttbotlib-0.5/tests/test_server.py
-drwxr-xr-x   0 scailer   (1000) users      (985)        0 2023-02-16 14:22:37.052533 ttbotlib-0.5/ttbot/
--rw-r--r--   0 scailer   (1000) users      (985)      179 2023-02-16 13:51:15.000000 ttbotlib-0.5/ttbot/__init__.py
--rw-r--r--   0 scailer   (1000) users      (985)     1120 2023-02-16 13:17:44.000000 ttbotlib-0.5/ttbot/client.py
--rw-r--r--   0 scailer   (1000) users      (985)     6081 2023-02-16 13:40:13.000000 ttbotlib-0.5/ttbot/server.py
--rw-r--r--   0 scailer   (1000) users      (985)      632 2023-02-06 12:20:18.000000 ttbotlib-0.5/ttbot/types.py
-drwxr-xr-x   0 scailer   (1000) users      (985)        0 2023-02-16 14:22:37.052533 ttbotlib-0.5/ttbotlib.egg-info/
--rw-r--r--   0 scailer   (1000) users      (985)      750 2023-02-16 14:22:36.000000 ttbotlib-0.5/ttbotlib.egg-info/PKG-INFO
--rw-r--r--   0 scailer   (1000) users      (985)      305 2023-02-16 14:22:37.000000 ttbotlib-0.5/ttbotlib.egg-info/SOURCES.txt
--rw-r--r--   0 scailer   (1000) users      (985)        1 2023-02-16 14:22:36.000000 ttbotlib-0.5/ttbotlib.egg-info/dependency_links.txt
--rw-r--r--   0 scailer   (1000) users      (985)       26 2023-02-16 14:22:36.000000 ttbotlib-0.5/ttbotlib.egg-info/requires.txt
--rw-r--r--   0 scailer   (1000) users      (985)        6 2023-02-16 14:22:36.000000 ttbotlib-0.5/ttbotlib.egg-info/top_level.txt
+drwxr-xr-x   0 scailer   (1000) users      (985)        0 2023-04-10 17:01:42.950729 ttbotlib-0.6/
+-rw-r--r--   0 scailer   (1000) users      (985)     1070 2020-01-16 11:25:02.000000 ttbotlib-0.6/LICENSE.md
+-rw-r--r--   0 scailer   (1000) users      (985)     3317 2023-04-10 17:01:42.950729 ttbotlib-0.6/PKG-INFO
+-rw-r--r--   0 scailer   (1000) users      (985)     2548 2023-02-16 14:30:46.000000 ttbotlib-0.6/README.md
+drwxr-xr-x   0 scailer   (1000) users      (985)        0 2023-04-10 17:01:42.947396 ttbotlib-0.6/example/
+-rw-r--r--   0 scailer   (1000) users      (985)     1664 2023-02-16 14:30:46.000000 ttbotlib-0.6/example/app.py
+-rw-r--r--   0 scailer   (1000) users      (985)     2290 2023-04-10 17:01:27.000000 ttbotlib-0.6/pyproject.toml
+-rw-r--r--   0 scailer   (1000) users      (985)       63 2023-04-10 17:01:42.950729 ttbotlib-0.6/setup.cfg
+-rw-r--r--   0 scailer   (1000) users      (985)       38 2023-04-10 17:01:27.000000 ttbotlib-0.6/setup.py
+drwxr-xr-x   0 scailer   (1000) users      (985)        0 2023-04-10 17:01:42.950729 ttbotlib-0.6/tests/
+-rw-r--r--   0 scailer   (1000) users      (985)     1442 2023-02-16 14:30:46.000000 ttbotlib-0.6/tests/test_client.py
+-rw-r--r--   0 scailer   (1000) users      (985)     4590 2023-04-10 17:01:27.000000 ttbotlib-0.6/tests/test_server.py
+drwxr-xr-x   0 scailer   (1000) users      (985)        0 2023-04-10 17:01:42.950729 ttbotlib-0.6/ttbot/
+-rw-r--r--   0 scailer   (1000) users      (985)      179 2023-04-10 17:01:27.000000 ttbotlib-0.6/ttbot/__init__.py
+-rw-r--r--   0 scailer   (1000) users      (985)     1120 2023-02-16 14:30:46.000000 ttbotlib-0.6/ttbot/client.py
+-rw-r--r--   0 scailer   (1000) users      (985)        0 2023-04-10 17:01:27.000000 ttbotlib-0.6/ttbot/py.typed
+-rw-r--r--   0 scailer   (1000) users      (985)     8065 2023-04-10 17:01:27.000000 ttbotlib-0.6/ttbot/server.py
+-rw-r--r--   0 scailer   (1000) users      (985)      632 2023-02-16 14:30:46.000000 ttbotlib-0.6/ttbot/types.py
+drwxr-xr-x   0 scailer   (1000) users      (985)        0 2023-04-10 17:01:42.950729 ttbotlib-0.6/ttbotlib.egg-info/
+-rw-r--r--   0 scailer   (1000) users      (985)     3317 2023-04-10 17:01:42.000000 ttbotlib-0.6/ttbotlib.egg-info/PKG-INFO
+-rw-r--r--   0 scailer   (1000) users      (985)      350 2023-04-10 17:01:42.000000 ttbotlib-0.6/ttbotlib.egg-info/SOURCES.txt
+-rw-r--r--   0 scailer   (1000) users      (985)        1 2023-04-10 17:01:42.000000 ttbotlib-0.6/ttbotlib.egg-info/dependency_links.txt
+-rw-r--r--   0 scailer   (1000) users      (985)      204 2023-04-10 17:01:42.000000 ttbotlib-0.6/ttbotlib.egg-info/requires.txt
+-rw-r--r--   0 scailer   (1000) users      (985)       14 2023-04-10 17:01:42.000000 ttbotlib-0.6/ttbotlib.egg-info/top_level.txt
```

### Comparing `ttbotlib-0.5/LICENSE.md` & `ttbotlib-0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ttbotlib-0.5/README.md` & `ttbotlib-0.6/README.md`

 * *Files identical despite different names*

### Comparing `ttbotlib-0.5/tests/test_client.py` & `ttbotlib-0.6/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `ttbotlib-0.5/tests/test_server.py` & `ttbotlib-0.6/tests/test_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,17 +128,15 @@
 
 async def test_unknown_ok(server):
     send = AsyncMock()
     receive = AsyncMock(return_value={'body': b''})
 
     await server({'type': 'http', 'method': 'POST', 'path': '/qwe'}, receive, send)
 
-    assert send.call_args_list[1][0][0] == {
-        'type': 'http.response.body', 'body': b'{"error":"unknown path"}'
-    }
+    assert send.call_args_list[1][0][0] == {'type': 'http.response.body', 'body': ''}
 
 
 async def test_shell_ok(server):  # not ready
     receive = AsyncMock(return_value={'body': b'{"q":1}'})
     send = AsyncMock()
 
     await server({'type': 'websocket', 'path': '/shell'}, receive, send)
```

### Comparing `ttbotlib-0.5/ttbot/client.py` & `ttbotlib-0.6/ttbot/client.py`

 * *Files identical despite different names*

### Comparing `ttbotlib-0.5/ttbot/server.py` & `ttbotlib-0.6/ttbot/server.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import base64
 import hmac
 import json
 import logging
 import os
+import mimetypes
+import itertools
 
 from hashlib import sha256
+from pathlib import Path
 from urllib.parse import parse_qs
 
 from ttutils import to_bytes
 
 from .client import Client
 from .types import Action, Post, Receive, Request, Scope, Send
 
@@ -16,39 +19,88 @@
 class Server:
     client: Client
     url_prefix: str
     __secret_bytes__: bytes
 
     log = logging.getLogger('server')
 
-    def __init__(self, secret: str = '') -> None:
+    def __init__(self, secret: str = '', static_path: str = '') -> None:
         secret = secret or os.environ.get('SECRET', '')
         assert secret, 'Set SECRET env'
 
         self.url_prefix = '/' + secret[:8]
         self.client = Client(secret[20:])
         self.__secret_bytes__ = to_bytes(int(secret, 32))
 
+        self._static_files: dict[str, dict] = {}
+        if base_path := os.environ.get('STATIC', static_path):
+            self._load_static_files(base_path)
+
+    def _load_static_files(self, base_path: str) -> None:
+        all_files = itertools.chain(*[
+            [Path(prefix) / Path(fname) for fname in files]
+            for prefix, _, files in os.walk(base_path)
+        ])
+
+        for path in all_files:
+            with open(path, 'rb') as fh:
+                content_length = str(os.fstat(fh.fileno()).st_size)
+                content_type, _ = mimetypes.guess_type(path.name)
+
+                self._static_files[str(path).replace(base_path, '')] = {
+                    'content_length': bytes(content_length, 'utf8'),
+                    'content_type': bytes(content_type or '', 'utf8'),
+                    'body': fh.read(),
+                }
+
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         ''' Main http router '''
         # Remove guard path prefix
         scope['path'] = scope['path'].replace(self.url_prefix, '') or '/'
 
         match scope:
             case {'type': 'http', 'method': 'POST', 'path': '/' | '/bot'}:
                 await self.asgi_call_bot(scope, receive, send)
             case {'type': 'http', 'method': 'POST', 'path': '/act'}:
                 await self.asgi_call_act(scope, receive, send)
             case {'type': 'http', 'path': '/api'}:
                 await self.asgi_call_api(scope, receive, send)
             case {'type': 'websocket', 'path': '/shell'}:
                 await self.asgi_call_shell(scope, receive, send)
+            case {'type': 'http', 'path': path}:
+                if path.startswith('/static'):
+                    await self.lightweight_static(path.replace('/static', ''), send)
+                else:
+                    await self.send_404(send)
             case _:
                 await self._send_json({'error': 'unknown path'}, send)
 
+    async def lightweight_static(self, path: str, send: Send) -> None:
+        if file_data := self._static_files.get(path):
+            await send({
+                'type': 'http.response.start',
+                'status': 200,
+                'headers': [
+                    [b'content-type', file_data['content_type']],
+                    [b'content-length', file_data['content_length']],
+                ]
+            })
+
+            await send({
+                'type': 'http.response.body',
+                'body': file_data['body'],
+            })
+
+        else:
+            await self.send_404(send)
+
+    async def send_404(self, send: Send) -> None:
+        await send({'type': 'http.response.start', 'status': 404})
+        await send({'type': 'http.response.body', 'body': ''})
+
     # ASGI API
     async def asgi_call_api(self, scope: Scope, receive: Receive, send: Send) -> None:
         ''' HTTP API with ASGI interface '''
 
         headers = {
             str(key, 'utf8'): str(val, 'utf8')
             for key, val in scope.get('headers', [])
```

### Comparing `ttbotlib-0.5/ttbot/types.py` & `ttbotlib-0.6/ttbot/types.py`

 * *Files identical despite different names*

