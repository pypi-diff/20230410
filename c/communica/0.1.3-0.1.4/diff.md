# Comparing `tmp/communica-0.1.3.tar.gz` & `tmp/communica-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "communica-0.1.3.tar", last modified: Tue Apr  4 19:35:59 2023, max compression
+gzip compressed data, was "communica-0.1.4.tar", last modified: Mon Apr 10 08:11:55 2023, max compression
```

## Comparing `communica-0.1.3.tar` & `communica-0.1.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 19:35:59.356384 communica-0.1.3/
--rw-rw-rw-   0        0        0      568 2023-03-25 20:48:52.000000 communica-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0     2185 2023-04-04 19:35:59.356384 communica-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1457 2023-04-04 17:16:21.000000 communica-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 19:35:59.330756 communica-0.1.3/communica/
--rw-rw-rw-   0        0        0      101 2023-02-15 13:48:00.000000 communica-0.1.3/communica/__init__.py
--rw-rw-rw-   0        0        0      130 2023-03-19 21:29:46.000000 communica-0.1.3/communica/clients.py
-drwxrwxrwx   0        0        0        0 2023-04-04 19:35:59.342383 communica-0.1.3/communica/connectors/
--rw-rw-rw-   0        0        0      170 2023-03-31 19:34:58.000000 communica-0.1.3/communica/connectors/__init__.py
--rw-rw-rw-   0        0        0     2803 2023-03-24 12:30:50.000000 communica-0.1.3/communica/connectors/_stream_local.py
--rw-rw-rw-   0        0        0     5358 2023-03-30 10:48:08.000000 communica-0.1.3/communica/connectors/base.py
--rw-rw-rw-   0        0        0    21025 2023-04-04 17:17:48.000000 communica-0.1.3/communica/connectors/rabbitmq.py
--rw-rw-rw-   0        0        0     9243 2023-03-30 11:38:51.000000 communica-0.1.3/communica/connectors/stream.py
--rw-rw-rw-   0        0        0      468 2023-03-19 11:58:01.000000 communica-0.1.3/communica/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-04 19:35:59.347384 communica-0.1.3/communica/pairs/
--rw-rw-rw-   0        0        0      223 2023-03-19 15:01:07.000000 communica-0.1.3/communica/pairs/__init__.py
--rw-rw-rw-   0        0        0     2667 2023-03-21 21:55:22.000000 communica-0.1.3/communica/pairs/base.py
--rw-rw-rw-   0        0        0     9553 2023-04-04 19:35:19.000000 communica-0.1.3/communica/pairs/route.py
--rw-rw-rw-   0        0        0    15234 2023-03-25 13:33:16.000000 communica-0.1.3/communica/pairs/simple.py
-drwxrwxrwx   0        0        0        0 2023-04-04 19:35:59.352384 communica-0.1.3/communica/serializers/
--rw-rw-rw-   0        0        0      176 2023-03-19 20:57:46.000000 communica-0.1.3/communica/serializers/__init__.py
--rw-rw-rw-   0        0        0      657 2023-03-18 18:41:17.000000 communica-0.1.3/communica/serializers/base.py
--rw-rw-rw-   0        0        0      315 2023-03-18 19:40:10.000000 communica-0.1.3/communica/serializers/json.py
--rw-rw-rw-   0        0        0      128 2023-03-19 21:29:36.000000 communica-0.1.3/communica/servers.py
--rw-rw-rw-   0        0        0     3077 2023-04-04 16:50:40.000000 communica-0.1.3/communica/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-04 19:35:59.337753 communica-0.1.3/communica.egg-info/
--rw-rw-rw-   0        0        0     2185 2023-04-04 19:35:59.000000 communica-0.1.3/communica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      716 2023-04-04 19:35:59.000000 communica-0.1.3/communica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 19:35:59.000000 communica-0.1.3/communica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-04-04 19:35:59.000000 communica-0.1.3/communica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-04 19:35:59.000000 communica-0.1.3/communica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1050 2023-04-04 19:34:50.000000 communica-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-04 19:35:59.356384 communica-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-04 19:35:59.355384 communica-0.1.3/tests/
--rw-rw-rw-   0        0        0     1040 2023-04-01 18:26:37.000000 communica-0.1.3/tests/test_connectors.py
--rw-rw-rw-   0        0        0     4440 2023-03-31 20:39:07.000000 communica-0.1.3/tests/test_entities.py
+drwxrwxrwx   0        0        0        0 2023-04-10 08:11:55.834890 communica-0.1.4/
+-rw-rw-rw-   0        0        0      568 2023-03-25 20:48:52.000000 communica-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     2184 2023-04-10 08:11:55.833891 communica-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2023-04-04 20:46:58.000000 communica-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 08:11:55.817381 communica-0.1.4/communica/
+-rw-rw-rw-   0        0        0      101 2023-02-15 13:48:00.000000 communica-0.1.4/communica/__init__.py
+-rw-rw-rw-   0        0        0      130 2023-03-19 21:29:46.000000 communica-0.1.4/communica/clients.py
+drwxrwxrwx   0        0        0        0 2023-04-10 08:11:55.824897 communica-0.1.4/communica/connectors/
+-rw-rw-rw-   0        0        0      170 2023-03-31 19:34:58.000000 communica-0.1.4/communica/connectors/__init__.py
+-rw-rw-rw-   0        0        0     2803 2023-03-24 12:30:50.000000 communica-0.1.4/communica/connectors/_stream_local.py
+-rw-rw-rw-   0        0        0     5358 2023-03-30 10:48:08.000000 communica-0.1.4/communica/connectors/base.py
+-rw-rw-rw-   0        0        0    22199 2023-04-10 08:11:15.000000 communica-0.1.4/communica/connectors/rabbitmq.py
+-rw-rw-rw-   0        0        0     9243 2023-03-30 11:38:51.000000 communica-0.1.4/communica/connectors/stream.py
+-rw-rw-rw-   0        0        0      468 2023-03-19 11:58:01.000000 communica-0.1.4/communica/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-10 08:11:55.827892 communica-0.1.4/communica/pairs/
+-rw-rw-rw-   0        0        0      223 2023-03-19 15:01:07.000000 communica-0.1.4/communica/pairs/__init__.py
+-rw-rw-rw-   0        0        0     2667 2023-03-21 21:55:22.000000 communica-0.1.4/communica/pairs/base.py
+-rw-rw-rw-   0        0        0    10308 2023-04-08 12:28:56.000000 communica-0.1.4/communica/pairs/route.py
+-rw-rw-rw-   0        0        0    15514 2023-04-10 08:02:57.000000 communica-0.1.4/communica/pairs/simple.py
+drwxrwxrwx   0        0        0        0 2023-04-10 08:11:55.831891 communica-0.1.4/communica/serializers/
+-rw-rw-rw-   0        0        0      176 2023-03-19 20:57:46.000000 communica-0.1.4/communica/serializers/__init__.py
+-rw-rw-rw-   0        0        0      657 2023-03-18 18:41:17.000000 communica-0.1.4/communica/serializers/base.py
+-rw-rw-rw-   0        0        0      315 2023-03-18 19:40:10.000000 communica-0.1.4/communica/serializers/json.py
+-rw-rw-rw-   0        0        0      128 2023-03-19 21:29:36.000000 communica-0.1.4/communica/servers.py
+-rw-rw-rw-   0        0        0     3077 2023-04-04 16:50:40.000000 communica-0.1.4/communica/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 08:11:55.821380 communica-0.1.4/communica.egg-info/
+-rw-rw-rw-   0        0        0     2184 2023-04-10 08:11:55.000000 communica-0.1.4/communica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      716 2023-04-10 08:11:55.000000 communica-0.1.4/communica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 08:11:55.000000 communica-0.1.4/communica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-04-10 08:11:55.000000 communica-0.1.4/communica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-10 08:11:55.000000 communica-0.1.4/communica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1050 2023-04-10 08:11:31.000000 communica-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-10 08:11:55.834890 communica-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-10 08:11:55.833891 communica-0.1.4/tests/
+-rw-rw-rw-   0        0        0     1040 2023-04-01 18:26:37.000000 communica-0.1.4/tests/test_connectors.py
+-rw-rw-rw-   0        0        0     2940 2023-04-08 16:43:45.000000 communica-0.1.4/tests/test_entities.py
```

### Comparing `communica-0.1.3/LICENSE.txt` & `communica-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `communica-0.1.3/PKG-INFO` & `communica-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: communica
-Version: 0.1.3
+Version: 0.1.4
 Summary: Easy to use IPC library
 Author-email: Elchin Sarkarov <elchin751@gmail.com>
 Project-URL: Homepage, https://github.com/elchinchel/communica-py
 Project-URL: Bug Tracker, https://github.com/elchinchel/communica-py/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,15 +16,15 @@
 Provides-Extra: orjson
 Provides-Extra: pydantic
 Provides-Extra: rabbitmq
 License-File: LICENSE.txt
 
 # Easy to use IPC library
 
-    This library is not ready yet as i imagine it.
+    This library is still in development process.
     There will be added Pub/Sub entities and data validation in
     serializers with pydantic and dataclass-factory libraries.
 
     Stream connectors has no acknowledgements at the moment,
     so messages on service restart will be lost
     (they will be lost anyway on restarting side, but with acks loss can be less)
```

### Comparing `communica-0.1.3/README.md` & `communica-0.1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Easy to use IPC library
 
-    This library is not ready yet as i imagine it.
+    This library is still in development process.
     There will be added Pub/Sub entities and data validation in
     serializers with pydantic and dataclass-factory libraries.
 
     Stream connectors has no acknowledgements at the moment,
     so messages on service restart will be lost
     (they will be lost anyway on restarting side, but with acks loss can be less)
```

### Comparing `communica-0.1.3/communica/connectors/_stream_local.py` & `communica-0.1.4/communica/connectors/_stream_local.py`

 * *Files identical despite different names*

### Comparing `communica-0.1.3/communica/connectors/base.py` & `communica-0.1.4/communica/connectors/base.py`

 * *Files identical despite different names*

### Comparing `communica-0.1.3/communica/connectors/rabbitmq.py` & `communica-0.1.4/communica/connectors/rabbitmq.py`

 * *Files 5% similar despite different names*

```diff
@@ -193,14 +193,15 @@
             await self._rmq_chan.basic_ack(message.delivery_tag)
 
         waiter = await MessageWaiter.new(self._rmq_chan,
                                          self._recv_queue, no_ack=False)
 
         while not self._rmq_chan.is_closed:
             message = await waiter.wait()
+            print(message.header.properties.message_type)
 
             if message.header.properties.message_type == _MessageType.MESSAGE:
                 null_pos = message.body.find(NULL_CHAR)
                 if null_pos == -1:
                     await ack_message(message)
                     await self._close(True)
                     raise ValueError('Got message without metadata separator')
@@ -247,14 +248,15 @@
                     routing_key=self._send_queue,
                     properties=aiormq.spec.Basic.Properties(
                         timestamp=datetime.now(),
                         message_type=_MessageType.CLOSE,
                     )
                 )
             await self._rmq_chan.close()
+            await self._connector._check_connection_use()
         except _closed_exceptions():
             return
 
 
 class RmqServer(asyncio.AbstractServer):
     @property
     def exchange(self):
@@ -273,19 +275,21 @@
         self._client_connected_cb = client_connected_cb
 
     def is_serving(self):
         """Return True if the server is accepting connections."""
         return not self._chan.is_closed
 
     def close(self):
-        def del_task(_):
+        async def close_channel():
+            if not self._chan.is_closed:
+                await self._chan.close()
+            await self._connector._check_connection_use()
             del(self._close_task)
 
-        self._close_task = asyncio.create_task(self._chan.close())
-        self._close_task.add_done_callback(del_task)
+        self._close_task = asyncio.create_task(close_channel())
 
     async def wait_closed(self):
         if not hasattr(self, '_close_task'):
             raise RuntimeError('wait_closed() should be '
                                'called right after close() method')
         await self._close_task
 
@@ -385,15 +389,16 @@
 
         Failure to comply with these rules
         leads to unclosed queues growth and message loss.
     """
 
     _TYPE = 'RABBITMQ'
 
-    __slots__ = ('_url', '_address', '_exchange', '_connect_id')
+    __slots__ = ('_url', '_address', '_connect_id',
+                 '_exchange', '_exchange_declared')
 
     @property
     def exchange(self):
         return self._exchange
 
     def __init__(
             self,
@@ -421,14 +426,15 @@
         if connect_id is not None and len(address + connect_id) > 224:
             raise ValueError('Max address + connect_id length is 224 characters')
 
         self._url = URL(url)
         self._address = address
         self._exchange = exchange_name
         self._connect_id = connect_id
+        self._exchange_declared = False
 
     def _get_connect_queue_name(self):
         return self._fmt_queue_name('connect', 'server')
 
     def _get_transport_queue_names(self, connect_id: str):
         return (
             self._fmt_queue_name('toClient', connect_id),
@@ -524,17 +530,26 @@
         if self._connect_id is None:
             raise TypeError('Cannot connect to server. For those, who connect, '
                             'connect_id parameter must be set. '
                             'Check RmqConnector docs for details.')
 
         chan = await self._open_channel()
         try:
+            if not self._exchange_declared:
+                await chan.exchange_declare(
+                    self._exchange,
+                    exchange_type="direct",
+                    durable=True,
+                )
+                self._exchange_declared = True
+
             return await self._client_connect(handshaker, chan)
         except Exception:
-            await chan.close()
+            if not chan.is_closed:
+                await chan.close()
             raise
 
 
     async def cleanup(self):
         """
         Drop all pending messages and
         delete queues with connector's connect_id
@@ -550,27 +565,29 @@
                 await chan.queue_purge(queue)
                 await chan.queue_delete(queue)
             except aiormq.exceptions.ChannelNotFoundEntity:
                 # channel will be closed by server if we try to delete unknown queue
                 continue
             await chan.close()
 
+        await self._check_connection_use()
+
     def dump_state(self) -> str:
         """Unsupported for this connector"""
         raise TypeError('This method unsupported cause user and password '
                         'are not encrypted in dump, which is insecure')
 
     @classmethod
     def from_state(cls, state: str) -> Self:
         """Unsupported for this connector"""
         raise TypeError('This method unsupported cause user and password '
                         'are not encrypted in dump, which is insecure')
 
     async def _open_channel(self):
-        # there is two limits for simultaneously opened channels:
+        # there are two limits for simultaneously opened channels:
         # 65k defined by AMQP protocol (channel number range),
         # which cause 'while not (some channel closed)' loop in conn.channel()
         # and 'max-channels' limit set by AMQP server
         # (RabbitMQ 3.11 default is 2047), which cause connection termination
         # it's unlikely to happen, but i'll keep this in mind ( in comment :D )
 
         if (conn := _connections.get(self._url)) is None:
@@ -591,14 +608,29 @@
 
         elif conn.is_closed:
             del(_connections[self._url])
             return await self._open_channel()
 
         return await conn.channel()
 
+    async def _check_connection_use(self):
+        print('check connection called')
+        conn = _connections.get(self._url)
+        if conn is None or isinstance(conn, asyncio.Future):
+            return
+
+        for chan in conn.channels.values():
+            if chan is not None and not chan.is_closed:
+                print(repr(chan), chan.is_closed)
+                return
+        print('deleting')
+        del(_connections[self._url])
+        print(_connections)
+        await conn.close()
+
     async def _queue_declare_and_bind(
             self,
             chan: 'aiormq.abc.AbstractChannel',
             name: str = '',
             **declare_kwargs
     ):
         declare_ok = await chan.queue_declare(queue=name, **declare_kwargs)
```

### Comparing `communica-0.1.3/communica/connectors/stream.py` & `communica-0.1.4/communica/connectors/stream.py`

 * *Files identical despite different names*

### Comparing `communica-0.1.3/communica/pairs/base.py` & `communica-0.1.4/communica/pairs/base.py`

 * *Files identical despite different names*

### Comparing `communica-0.1.3/communica/pairs/route.py` & `communica-0.1.4/communica/pairs/route.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,39 +25,42 @@
 __all__ = (
     'RouteClient',
     'RouteServer'
 )
 
 
 class Metadata(TypedDict):
-    id: int
+    id: str
     type: RequestType
     route: str
 
 
 class RouteMessageFlow(ReqRepMessageFlow):
-    __slots__ = ('routes', 'fallback_task_set')
+    __slots__ = ('routes', 'fallback_task_set', '_response_serializers',)
 
     routes: 'dict[str, tuple[RequestHandler, BaseSerializer]]'
     fallback_task_set: 'set[asyncio.Task]'
 
+    _response_serializers: 'dict[str, BaseSerializer]'
+
     def __init__(self):
         super().__init__()
         self.routes = {}
         self.fallback_task_set = set()
 
     def update_route(
             self,
             route: str,
             handler: 'SyncHandlerType | AsyncHandlerType',
             serializer: 'BaseSerializer | None'
     ):
         if serializer is None:
             serializer = default_serializer
         self.routes[route] = (RequestHandler(handler), serializer)
+        self._response_serializers = {}
 
     def dispatch(self, metadata: Metadata, raw_data: bytes):
         if metadata['type'] < RequestType.RESP_OK:
             try:
                 route_handle = self.routes[metadata['route']]
                 task_set = route_handle[0].running_tasks
             except KeyError:
@@ -66,18 +69,21 @@
 
             runner_task = self._get_loop().create_task(
                 self.handle_request(route_handle, metadata, raw_data))
             runner_task.add_done_callback(task_set.discard)
             task_set.add(runner_task)
         else:
             try:
-                _, serializer = self.routes[metadata['route']]
+                serializer = self._response_serializers[metadata['route']]
             except KeyError:
-                logger.critical('Got response with nonexistent '
-                               f'route ({metadata["route"]})')
+                # this is possible, for example, after program restart.
+                # just log and skip, cause we don't have a routine,
+                # waiting for this response
+                logger.warning('Got response with not requested '
+                              f'route ({metadata["route"]})')
                 return
             self._handle_response(serializer, metadata, raw_data)
 
     async def handle_request(
             self,
             route_handle: 'tuple[RequestHandler, BaseSerializer] | None',
             req_meta: Metadata,
@@ -109,29 +115,37 @@
             self,
             route: str,
             serializer: 'BaseSerializer | None',
             data: Any
     ) -> bytes:
         request_id, fut = self.create_response_waiter()
 
+        serializer = serializer or default_serializer
+        if (saved_serializer := self._response_serializers.get(route)) is None:
+            self._response_serializers[route] = serializer
+        elif saved_serializer != serializer:
+            raise TypeError('You should always use the same serializer for the '
+                           f'same route ({saved_serializer!r} '
+                            'has already been used earlier)')
+
         await self._connection.send(
             Metadata(id=request_id, type=RequestType.REQ_REP, route=route),
-            (serializer or default_serializer).dump(data)
+            serializer.dump(data)
         )
 
         return await fut
 
     async def throw(
             self,
             route: str,
             serializer: 'BaseSerializer | None',
             data: Any
     ) -> None:
         await self._connection.send(
-            Metadata(id=0, type=RequestType.REQ_THROW, route=route),
+            Metadata(id='', type=RequestType.REQ_THROW, route=route),
             (serializer or default_serializer).dump(data)
         )
 
 
 class RouteClient(ReqRepClient):
     """
     Pair for RouteServer.
```

### Comparing `communica-0.1.3/communica/pairs/simple.py` & `communica-0.1.4/communica/pairs/simple.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import asyncio
 
 from abc import abstractmethod
 from enum import Enum
-from uuid import uuid4
+from uuid import uuid4, uuid1
 from typing import TypedDict, Any, cast
 from inspect import iscoroutinefunction
 from traceback import format_exc
 from dataclasses import dataclass
 
 from communica.exceptions import RequesterError, ResponderError
 from communica.serializers import BaseSerializer, default_serializer
@@ -48,15 +48,15 @@
 @dataclass
 class ServerHandshakeOk(HandshakeOk):
     client_id: str
 
 
 class Metadata(TypedDict):
     type: RequestType
-    id: int
+    id: str
 
 
 class RequestHandler:
     __slots__ = ('is_async', 'endpoint', 'running_tasks')
 
     is_async: bool
     endpoint: 'SyncHandlerType | AsyncHandlerType'
@@ -72,29 +72,29 @@
 
 
 class ReqRepMessageFlow(HasLoopMixin):
     __slots__ = (
         '_connection', '_id_counter', '_response_waiters'
     )
 
-    _response_waiters: 'dict[int, asyncio.Future]'
+    _response_waiters: 'dict[str, asyncio.Future]'
 
     def __init__(self):
         self._id_counter = cycle_range(*INT32RANGE)
         self._response_waiters = {}
 
     def update_connection(self, connection: BaseConnection):
         try:
             self._connection.update(connection)
         except AttributeError:
             self._connection = connection
         return self._connection
 
     def create_response_waiter(self):
-        request_id = next(self._id_counter)
+        request_id = uuid1().hex
 
         fut = self._get_loop().create_future()
         self._response_waiters[request_id] = fut
         fut.add_done_callback(lambda _: self._response_waiters.pop(request_id, None))
 
         return request_id, fut
 
@@ -108,15 +108,21 @@
         if fut is None or fut.done():
             logger.warning('Drop response for unknown or expired request')
             return
 
         req_type = metadata['type']
 
         if req_type == RequestType.RESP_OK:
-            fut.set_result(serializer.load(raw_data))
+            try:
+                fut.set_result(serializer.load(raw_data))
+            except Exception as e:
+                # if serializer can't load response, considering this
+                # requester's error, cause responder can't do
+                # anything about it after sending response
+                fut.set_exception(e)
             return
 
         data = default_serializer.load(raw_data)
         if req_type == RequestType.RESP_ERR_REQUESTER:
             fut.set_exception(RequesterError(data['msg']))
         elif req_type == RequestType.RESP_ERR_RESPONDER:
             fut.set_exception(ResponderError(data['msg']))
@@ -200,15 +206,15 @@
             self.serializer.dump(data)
         )
 
         return await fut
 
     async def throw(self, data: Any) -> None:
         await self._connection.send(
-            Metadata(id=0, type=RequestType.REQ_THROW),
+            Metadata(id='', type=RequestType.REQ_THROW),
             self.serializer.dump(data)
         )
 
 
 class ReqRepClient(BaseClient):
     __slots__ = ('_connected_event', '_run_task', '_client_id', '_flow')
 
@@ -241,24 +247,18 @@
         except asyncio.TimeoutError:
             self._run_task.cancel()
             raise
         return self
 
     async def close(self) -> None:
         if self._run_task is not None:
-            self._run_task.cancel()
             await self._flow._connection.close()
+            self._run_task.cancel()
         self.stop()
 
-    # def _on_conn_fail(self, task: asyncio.Task):
-    #     if task.cancelled():
-    #         return
-    #     if (exc := task.exception()):
-    #         logger.error('Unhandled exception in connection runner: {exc!r}')
-
     async def _connection_keeper(self):
         while True:
             try:
                 new_conn = await self.connector.client_connect(self._handshaker)
             except Exception as e:
                 logger.warning('Connect failed: %s', repr(e))
                 await asyncio.sleep(1)
@@ -338,19 +338,21 @@
     async def init(self):
         self._server = await self.connector.server_start(
             self._handshaker, self._on_client_connect)
         return self
 
     async def close(self) -> None:
         for client_id, flow in self._known_clients.items():
-            if (conn_task := self._client_conn_runners.get(client_id)):
-                conn_task.cancel()
             if isinstance(flow, ReqRepMessageFlow):
                 self._cancel_handler_tasks(flow)
                 await flow._connection.close()
+            # XXX: проблемы с RMQ коннектором: отмена conn.close()
+            # вызывает повторную отправку Close фрейма, что ломает соединение
+            if (conn_task := self._client_conn_runners.get(client_id)):
+                conn_task.cancel()
         self._server.close()
         await self._server.wait_closed()
 
     async def _handshaker(self, connection: BaseConnection) -> HandshakeGen:
         server_hello = {
             'hello': 'hello'
         }
```

### Comparing `communica-0.1.3/communica/serializers/base.py` & `communica-0.1.4/communica/serializers/base.py`

 * *Files identical despite different names*

### Comparing `communica-0.1.3/communica/utils.py` & `communica-0.1.4/communica/utils.py`

 * *Files identical despite different names*

### Comparing `communica-0.1.3/communica.egg-info/PKG-INFO` & `communica-0.1.4/communica.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: communica
-Version: 0.1.3
+Version: 0.1.4
 Summary: Easy to use IPC library
 Author-email: Elchin Sarkarov <elchin751@gmail.com>
 Project-URL: Homepage, https://github.com/elchinchel/communica-py
 Project-URL: Bug Tracker, https://github.com/elchinchel/communica-py/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,15 +16,15 @@
 Provides-Extra: orjson
 Provides-Extra: pydantic
 Provides-Extra: rabbitmq
 License-File: LICENSE.txt
 
 # Easy to use IPC library
 
-    This library is not ready yet as i imagine it.
+    This library is still in development process.
     There will be added Pub/Sub entities and data validation in
     serializers with pydantic and dataclass-factory libraries.
 
     Stream connectors has no acknowledgements at the moment,
     so messages on service restart will be lost
     (they will be lost anyway on restarting side, but with acks loss can be less)
```

### Comparing `communica-0.1.3/communica.egg-info/SOURCES.txt` & `communica-0.1.4/communica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `communica-0.1.3/pyproject.toml` & `communica-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "communica"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Elchin Sarkarov", email="elchin751@gmail.com" },
 ]
 description = "Easy to use IPC library"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `communica-0.1.3/tests/test_connectors.py` & `communica-0.1.4/tests/test_connectors.py`

 * *Files identical despite different names*

### Comparing `communica-0.1.3/tests/test_entities.py` & `communica-0.1.4/tests/test_entities.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,64 +6,28 @@
 
 import pytest
 
 from communica.pairs import *
 
 from utils import wait_tasks  # type: ignore
 from simple_entities_for_tests import(
+    CLIENT_ID,
     MessageExistenceChecker, MessageOrderChecker,
     client_to_server_messages, server_to_client_messages,
-    CLIENT_ID
+    run_concurrent_send_with_simples,
+    run_sequential_send_with_simples
 )
 
 
-# class TestSimpleEntities:
-    # @pytest.mark.asyncio
-    # async def test_sequential_send(connector, serializer):
-    #     async def run(entity, messages, done_event):
-    #         async with entity:
-    #             for message in messages:
-    #                 resp = await entity.request(message)
-    #                 assert resp == message, 'Response data must be equal to sent'
-    #             await done_event.wait()
-
-    #     cli_checker = MessageOrderChecker(server_to_client_messages)
-    #     client = SimpleClient(
-    #         connector, cli_checker.handler, serializer, CLIENT_ID)
-
-    #     srv_checker = MessageOrderChecker(client_to_server_messages)
-    #     server = SimpleServer(connector, srv_checker.handler, serializer)
-
-    #     await wait_tasks(
-    #         run(server, server_to_client_messages, srv_checker.done),
-    #         run(client, client_to_server_messages, cli_checker.done),
-    #         timeout=10
-    #     )
-
-
-    # @pytest.mark.asyncio
-    # async def test_concurrent_send(connector, serializer):
-    #     async def run(entity, messages, done_event):
-    #         async with entity:
-    #             calls = [entity.throw(msg) for msg in messages]
-    #             await asyncio.gather(*calls)
-    #             await done_event.wait()
-
-    #     cli_checker = MessageExistenceChecker(server_to_client_messages)
-    #     client = SimpleClient(
-    #         connector, cli_checker.handler, serializer, CLIENT_ID)
-
-    #     srv_checker = MessageExistenceChecker(client_to_server_messages)
-    #     server = SimpleServer(connector, srv_checker.handler, serializer)
-
-    #     await wait_tasks(
-    #         run(server, server_to_client_messages, srv_checker.done),
-    #         run(client, client_to_server_messages, cli_checker.done),
-    #         timeout=10
-    #     )
+class TestSimpleEntities:
+    async def test_sequential_send(self, connector, serializer):
+        await run_sequential_send_with_simples(connector, serializer)
+
+    async def test_concurrent_send(self, connector, serializer):
+        await run_concurrent_send_with_simples(connector, serializer)
 
 
 # class RouteEntitiesTestCase(EntitiesTestCase):
 #     # @pytest.mark.asyncio
 #     # async def test_connect(connector, serializer):
 
 #     #     with pytest.raises(asyncio.TimeoutError):
```

