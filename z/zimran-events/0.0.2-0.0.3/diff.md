# Comparing `tmp/zimran-events-0.0.2.tar.gz` & `tmp/zimran-events-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zimran-events-0.0.2.tar", last modified: Mon Apr 10 10:36:22 2023, max compression
+gzip compressed data, was "zimran-events-0.0.3.tar", last modified: Mon Apr 10 11:00:05 2023, max compression
```

## Comparing `zimran-events-0.0.2.tar` & `zimran-events-0.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:36:22.623407 zimran-events-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-10 10:36:14.000000 zimran-events-0.0.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-10 10:36:14.000000 zimran-events-0.0.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-10 10:36:14.000000 zimran-events-0.0.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:36:22.611407 zimran-events-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:36:22.615407 zimran-events-0.0.2/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-04-10 10:36:14.000000 zimran-events-0.0.2/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:36:22.615407 zimran-events-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-10 10:36:14.000000 zimran-events-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-10 10:36:14.000000 zimran-events-0.0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-04-10 10:36:14.000000 zimran-events-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-10 10:36:14.000000 zimran-events-0.0.2/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-10 10:36:14.000000 zimran-events-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-04-10 10:36:22.623407 zimran-events-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-10 10:36:14.000000 zimran-events-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-10 10:36:14.000000 zimran-events-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-10 10:36:14.000000 zimran-events-0.0.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 10:36:22.623407 zimran-events-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:36:22.611407 zimran-events-0.0.2/zimran/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:36:22.619407 zimran-events-0.0.2/zimran/events/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-10 10:36:14.000000 zimran-events-0.0.2/zimran/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-10 10:36:14.000000 zimran-events-0.0.2/zimran/events/_abstracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-10 10:36:14.000000 zimran-events-0.0.2/zimran/events/_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-04-10 10:36:14.000000 zimran-events-0.0.2/zimran/events/_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-10 10:36:14.000000 zimran-events-0.0.2/zimran/events/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-10 10:36:14.000000 zimran-events-0.0.2/zimran/events/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-10 10:36:14.000000 zimran-events-0.0.2/zimran/events/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-10 10:36:14.000000 zimran-events-0.0.2/zimran/events/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:36:22.623407 zimran-events-0.0.2/zimran_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-04-10 10:36:22.000000 zimran-events-0.0.2/zimran_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-10 10:36:22.000000 zimran-events-0.0.2/zimran_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 10:36:22.000000 zimran-events-0.0.2/zimran_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-10 10:36:22.000000 zimran-events-0.0.2/zimran_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-10 10:36:22.000000 zimran-events-0.0.2/zimran_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:00:05.478657 zimran-events-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-10 10:59:56.000000 zimran-events-0.0.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-10 10:59:56.000000 zimran-events-0.0.3/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-10 10:59:56.000000 zimran-events-0.0.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:00:05.470657 zimran-events-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:00:05.474657 zimran-events-0.0.3/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-04-10 10:59:56.000000 zimran-events-0.0.3/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:00:05.474657 zimran-events-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-10 10:59:56.000000 zimran-events-0.0.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-10 10:59:56.000000 zimran-events-0.0.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-04-10 10:59:56.000000 zimran-events-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-10 10:59:56.000000 zimran-events-0.0.3/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-10 10:59:56.000000 zimran-events-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-04-10 11:00:05.478657 zimran-events-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-10 10:59:56.000000 zimran-events-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-10 10:59:56.000000 zimran-events-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-10 10:59:56.000000 zimran-events-0.0.3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 11:00:05.478657 zimran-events-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:00:05.470657 zimran-events-0.0.3/zimran/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:00:05.474657 zimran-events-0.0.3/zimran/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-10 10:59:56.000000 zimran-events-0.0.3/zimran/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-10 10:59:56.000000 zimran-events-0.0.3/zimran/events/_abstracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-10 10:59:56.000000 zimran-events-0.0.3/zimran/events/_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-04-10 10:59:56.000000 zimran-events-0.0.3/zimran/events/_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-10 10:59:56.000000 zimran-events-0.0.3/zimran/events/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-10 10:59:56.000000 zimran-events-0.0.3/zimran/events/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-10 10:59:56.000000 zimran-events-0.0.3/zimran/events/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-10 10:59:56.000000 zimran-events-0.0.3/zimran/events/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:00:05.478657 zimran-events-0.0.3/zimran_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-04-10 11:00:05.000000 zimran-events-0.0.3/zimran_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-10 11:00:05.000000 zimran-events-0.0.3/zimran_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 11:00:05.000000 zimran-events-0.0.3/zimran_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-10 11:00:05.000000 zimran-events-0.0.3/zimran_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-10 11:00:05.000000 zimran-events-0.0.3/zimran_events.egg-info/top_level.txt
```

### Comparing `zimran-events-0.0.2/.github/scripts/release.py` & `zimran-events-0.0.3/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.0.2/.gitignore` & `zimran-events-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `zimran-events-0.0.2/LICENSE` & `zimran-events-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zimran-events-0.0.2/PKG-INFO` & `zimran-events-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimran-events
-Version: 0.0.2
+Version: 0.0.3
 Summary: The zimran-events provides amqp interface
 Author-email: Talgat Abdraimov <abdraimov.talga@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Talgat Abdraimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zimran-events-0.0.2/README.md` & `zimran-events-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `zimran-events-0.0.2/pyproject.toml` & `zimran-events-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zimran-events"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Talgat Abdraimov", email="abdraimov.talga@gmail.com" },
 ]
 description = "The zimran-events provides amqp interface"
 readme = "README.md"
 requires-python = ">=3.10"
 license = { file = "LICENSE" }
```

### Comparing `zimran-events-0.0.2/zimran/events/_abstracts.py` & `zimran-events-0.0.3/zimran/events/_abstracts.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.0.2/zimran/events/_consumer.py` & `zimran-events-0.0.3/zimran/events/_consumer.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.0.2/zimran/events/_producer.py` & `zimran-events-0.0.3/zimran/events/_producer.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
         channel = await self.channel
 
         if context.exchange is None:
             await channel.default_exchange.publish(message=message, routing_key=routing_key)
             return
 
         self._validate_exchange(context.exchange)
+        await self._declare_unroutable_queue(channel)
 
         exchange_args = {**context.exchange.arguments, 'alternate-exchange': UNROUTABLE_EXCHANGE_NAME}
         exchange = await channel.declare_exchange(
             **context.exchange.as_dict(exclude_none=True, exclude=['arguments']),
             arguments=exchange_args,
         )
 
@@ -81,15 +82,15 @@
         return aio_pika.Message(
             body=json.dumps(payload, default=str).encode(),
             headers=context.headers,
             content_type='application/json',
             correlation_id=context.correlation_id,
         )
 
-    async def _declare_unroutable_exchange(self, channel: aio_pika.abc.AbstractChannel):
+    async def _declare_unroutable_queue(self, channel: aio_pika.abc.AbstractChannel):
         exchange = await channel.declare_exchange(UNROUTABLE_EXCHANGE_NAME, type='fanout', durable=True)
         queue = await channel.declare_queue(UNROUTABLE_QUEUE_NAME, durable=True)
         await queue.bind(exchange=exchange, routing_key='')
 
 
 class Producer(EventMixin, AbstractProducer):
     def __init__(self, *, broker_url: str):
```

### Comparing `zimran-events-0.0.2/zimran/events/mixins.py` & `zimran-events-0.0.3/zimran/events/mixins.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.0.2/zimran/events/schemas.py` & `zimran-events-0.0.3/zimran/events/schemas.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.0.2/zimran_events.egg-info/PKG-INFO` & `zimran-events-0.0.3/zimran_events.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimran-events
-Version: 0.0.2
+Version: 0.0.3
 Summary: The zimran-events provides amqp interface
 Author-email: Talgat Abdraimov <abdraimov.talga@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Talgat Abdraimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zimran-events-0.0.2/zimran_events.egg-info/SOURCES.txt` & `zimran-events-0.0.3/zimran_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

