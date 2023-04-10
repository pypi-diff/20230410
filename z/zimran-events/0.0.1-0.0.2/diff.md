# Comparing `tmp/zimran-events-0.0.1.tar.gz` & `tmp/zimran-events-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zimran-events-0.0.1.tar", last modified: Fri Apr  7 21:15:30 2023, max compression
+gzip compressed data, was "zimran-events-0.0.2.tar", last modified: Mon Apr 10 10:36:22 2023, max compression
```

## Comparing `zimran-events-0.0.1.tar` & `zimran-events-0.0.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:15:30.754470 zimran-events-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-07 21:15:22.000000 zimran-events-0.0.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-07 21:15:22.000000 zimran-events-0.0.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-07 21:15:22.000000 zimran-events-0.0.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:15:30.746470 zimran-events-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:15:30.750470 zimran-events-0.0.1/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-04-07 21:15:22.000000 zimran-events-0.0.1/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:15:30.750470 zimran-events-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-07 21:15:22.000000 zimran-events-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-07 21:15:22.000000 zimran-events-0.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-04-07 21:15:22.000000 zimran-events-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-07 21:15:22.000000 zimran-events-0.0.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-07 21:15:22.000000 zimran-events-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-04-07 21:15:30.754470 zimran-events-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-07 21:15:22.000000 zimran-events-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-07 21:15:22.000000 zimran-events-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-07 21:15:22.000000 zimran-events-0.0.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 21:15:30.754470 zimran-events-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:15:30.746470 zimran-events-0.0.1/zimran/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:15:30.750470 zimran-events-0.0.1/zimran/events/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-07 21:15:22.000000 zimran-events-0.0.1/zimran/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-07 21:15:22.000000 zimran-events-0.0.1/zimran/events/_abstracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-07 21:15:22.000000 zimran-events-0.0.1/zimran/events/_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-04-07 21:15:22.000000 zimran-events-0.0.1/zimran/events/_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-07 21:15:22.000000 zimran-events-0.0.1/zimran/events/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-07 21:15:22.000000 zimran-events-0.0.1/zimran/events/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-07 21:15:22.000000 zimran-events-0.0.1/zimran/events/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:15:30.754470 zimran-events-0.0.1/zimran_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-04-07 21:15:30.000000 zimran-events-0.0.1/zimran_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-07 21:15:30.000000 zimran-events-0.0.1/zimran_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 21:15:30.000000 zimran-events-0.0.1/zimran_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-07 21:15:30.000000 zimran-events-0.0.1/zimran_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-07 21:15:30.000000 zimran-events-0.0.1/zimran_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:36:22.623407 zimran-events-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-10 10:36:14.000000 zimran-events-0.0.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-10 10:36:14.000000 zimran-events-0.0.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-10 10:36:14.000000 zimran-events-0.0.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:36:22.611407 zimran-events-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:36:22.615407 zimran-events-0.0.2/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-04-10 10:36:14.000000 zimran-events-0.0.2/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:36:22.615407 zimran-events-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-10 10:36:14.000000 zimran-events-0.0.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-10 10:36:14.000000 zimran-events-0.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-04-10 10:36:14.000000 zimran-events-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-10 10:36:14.000000 zimran-events-0.0.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-10 10:36:14.000000 zimran-events-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-04-10 10:36:22.623407 zimran-events-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-10 10:36:14.000000 zimran-events-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-10 10:36:14.000000 zimran-events-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-10 10:36:14.000000 zimran-events-0.0.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 10:36:22.623407 zimran-events-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:36:22.611407 zimran-events-0.0.2/zimran/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:36:22.619407 zimran-events-0.0.2/zimran/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-10 10:36:14.000000 zimran-events-0.0.2/zimran/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-10 10:36:14.000000 zimran-events-0.0.2/zimran/events/_abstracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-10 10:36:14.000000 zimran-events-0.0.2/zimran/events/_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-04-10 10:36:14.000000 zimran-events-0.0.2/zimran/events/_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-10 10:36:14.000000 zimran-events-0.0.2/zimran/events/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-10 10:36:14.000000 zimran-events-0.0.2/zimran/events/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-10 10:36:14.000000 zimran-events-0.0.2/zimran/events/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-10 10:36:14.000000 zimran-events-0.0.2/zimran/events/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:36:22.623407 zimran-events-0.0.2/zimran_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-04-10 10:36:22.000000 zimran-events-0.0.2/zimran_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-10 10:36:22.000000 zimran-events-0.0.2/zimran_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 10:36:22.000000 zimran-events-0.0.2/zimran_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-10 10:36:22.000000 zimran-events-0.0.2/zimran_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-10 10:36:22.000000 zimran-events-0.0.2/zimran_events.egg-info/top_level.txt
```

### Comparing `zimran-events-0.0.1/.github/scripts/release.py` & `zimran-events-0.0.2/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.0.1/.gitignore` & `zimran-events-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `zimran-events-0.0.1/LICENSE` & `zimran-events-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zimran-events-0.0.1/PKG-INFO` & `zimran-events-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimran-events
-Version: 0.0.1
+Version: 0.0.2
 Summary: The zimran-events provides amqp interface
 Author-email: Talgat Abdraimov <abdraimov.talga@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Talgat Abdraimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zimran-events-0.0.1/README.md` & `zimran-events-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `zimran-events-0.0.1/pyproject.toml` & `zimran-events-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zimran-events"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Talgat Abdraimov", email="abdraimov.talga@gmail.com" },
 ]
 description = "The zimran-events provides amqp interface"
 readme = "README.md"
 requires-python = ">=3.10"
 license = { file = "LICENSE" }
```

### Comparing `zimran-events-0.0.1/zimran/events/_abstracts.py` & `zimran-events-0.0.2/zimran/events/_abstracts.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.0.1/zimran/events/_consumer.py` & `zimran-events-0.0.2/zimran/events/_consumer.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.0.1/zimran/events/_producer.py` & `zimran-events-0.0.2/zimran/events/_producer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import asyncio
 import json
 
 import aio_pika
 import pika
 
+from zimran.events.constants import UNROUTABLE_EXCHANGE_NAME, UNROUTABLE_QUEUE_NAME
 from zimran.events.mixins import EventMixin
-from zimran.events.schemas import ContextScheme
+from zimran.events.schemas import ContextScheme, ExchangeScheme
 
 from ._abstracts import AbstractProducer
 
 
 class AsyncProducer(EventMixin, AbstractProducer):
     def __init__(self, *, broker_url: str, loop=None):
         super().__init__(broker_url=broker_url)
@@ -62,27 +63,37 @@
         channel = await self.channel
 
         if context.exchange is None:
             await channel.default_exchange.publish(message=message, routing_key=routing_key)
             return
 
         self._validate_exchange(context.exchange)
-        exchange = await channel.declare_exchange(**context.exchange.as_dict(exclude_none=True))
+
+        exchange_args = {**context.exchange.arguments, 'alternate-exchange': UNROUTABLE_EXCHANGE_NAME}
+        exchange = await channel.declare_exchange(
+            **context.exchange.as_dict(exclude_none=True, exclude=['arguments']),
+            arguments=exchange_args,
+        )
 
         await exchange.publish(message=message, routing_key=routing_key)
 
     @staticmethod
     def _get_message(context: ContextScheme, payload: dict):
         return aio_pika.Message(
             body=json.dumps(payload, default=str).encode(),
             headers=context.headers,
             content_type='application/json',
             correlation_id=context.correlation_id,
         )
 
+    async def _declare_unroutable_exchange(self, channel: aio_pika.abc.AbstractChannel):
+        exchange = await channel.declare_exchange(UNROUTABLE_EXCHANGE_NAME, type='fanout', durable=True)
+        queue = await channel.declare_queue(UNROUTABLE_QUEUE_NAME, durable=True)
+        await queue.bind(exchange=exchange, routing_key='')
+
 
 class Producer(EventMixin, AbstractProducer):
     def __init__(self, *, broker_url: str):
         super().__init__(broker_url=broker_url)
 
         self._connection = None
         self._channel = None
@@ -127,15 +138,25 @@
             self._validate_context(context)
 
         body = json.dumps(payload, default=str).encode()
         if context.exchange is None:
             self.channel.basic_publish(exchange='', routing_key=routing_key, body=body)
             return
 
+        self._declare_unroutable_queue()
+
         self._validate_exchange(context.exchange)
+
+        exchange_args = {**context.exchange, 'alternate-exchange': UNROUTABLE_EXCHANGE_NAME}
         self.channel.exchange_declare(
             exchange=context.exchange.name,
             exchange_type=context.exchange.type,
-            **context.exchange.as_dict(exclude=['name', 'type', 'timeout'], exclude_none=True),
+            arguments=exchange_args,
+            **context.exchange.as_dict(exclude=['name', 'type', 'timeout', 'arguments'], exclude_none=True),
         )
 
         self.channel.basic_publish(exchange=context.exchange.name, routing_key=routing_key, body=body)
+
+    def _declare_unroutable_queue(self):
+        self.channel.exchange_declare(exchange=UNROUTABLE_EXCHANGE_NAME, exchange_type='fanout', durable=True)
+        self.channel.queue_declare(UNROUTABLE_QUEUE_NAME, durable=True)
+        self.channel.queue_bind(UNROUTABLE_QUEUE_NAME, UNROUTABLE_EXCHANGE_NAME, '')
```

### Comparing `zimran-events-0.0.1/zimran/events/mixins.py` & `zimran-events-0.0.2/zimran/events/mixins.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.0.1/zimran/events/schemas.py` & `zimran-events-0.0.2/zimran/events/schemas.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.0.1/zimran_events.egg-info/PKG-INFO` & `zimran-events-0.0.2/zimran_events.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimran-events
-Version: 0.0.1
+Version: 0.0.2
 Summary: The zimran-events provides amqp interface
 Author-email: Talgat Abdraimov <abdraimov.talga@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Talgat Abdraimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zimran-events-0.0.1/zimran_events.egg-info/SOURCES.txt` & `zimran-events-0.0.2/zimran_events.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 .github/scripts/release.py
 .github/workflows/publish.yml
 .github/workflows/release.yml
 zimran/events/__init__.py
 zimran/events/_abstracts.py
 zimran/events/_consumer.py
 zimran/events/_producer.py
+zimran/events/constants.py
 zimran/events/exceptions.py
 zimran/events/mixins.py
 zimran/events/schemas.py
 zimran_events.egg-info/PKG-INFO
 zimran_events.egg-info/SOURCES.txt
 zimran_events.egg-info/dependency_links.txt
 zimran_events.egg-info/requires.txt
```

