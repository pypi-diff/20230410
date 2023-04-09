# Comparing `tmp/taskiq_redis-0.2.3.tar.gz` & `tmp/taskiq_redis-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_redis-0.2.3.tar", max compression
+gzip compressed data, was "taskiq_redis-0.3.0.tar", max compression
```

## Comparing `taskiq_redis-0.2.3.tar` & `taskiq_redis-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2576 2023-03-28 21:06:30.781927 taskiq_redis-0.2.3/README.md
--rw-r--r--   0        0        0     1587 2023-03-28 21:06:30.781927 taskiq_redis-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      257 2023-03-28 21:06:30.781927 taskiq_redis-0.2.3/taskiq_redis/__init__.py
--rw-r--r--   0        0        0      314 2023-03-28 21:06:30.785927 taskiq_redis-0.2.3/taskiq_redis/exceptions.py
--rw-r--r--   0        0        0     4154 2023-03-28 21:06:30.785927 taskiq_redis-0.2.3/taskiq_redis/redis_backend.py
--rw-r--r--   0        0        0     4312 2023-03-28 21:06:30.785927 taskiq_redis-0.2.3/taskiq_redis/redis_broker.py
--rw-r--r--   0        0        0     3699 1970-01-01 00:00:00.000000 taskiq_redis-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     2576 2023-04-09 23:26:16.010239 taskiq_redis-0.3.0/README.md
+-rw-r--r--   0        0        0     1587 2023-04-09 23:26:16.010239 taskiq_redis-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      257 2023-04-09 23:26:16.010239 taskiq_redis-0.3.0/taskiq_redis/__init__.py
+-rw-r--r--   0        0        0      314 2023-04-09 23:26:16.010239 taskiq_redis-0.3.0/taskiq_redis/exceptions.py
+-rw-r--r--   0        0        0     4154 2023-04-09 23:26:16.010239 taskiq_redis-0.3.0/taskiq_redis/redis_backend.py
+-rw-r--r--   0        0        0     4006 2023-04-09 23:26:16.010239 taskiq_redis-0.3.0/taskiq_redis/redis_broker.py
+-rw-r--r--   0        0        0     3699 1970-01-01 00:00:00.000000 taskiq_redis-0.3.0/PKG-INFO
```

### Comparing `taskiq_redis-0.2.3/README.md` & `taskiq_redis-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `taskiq_redis-0.2.3/pyproject.toml` & `taskiq_redis-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskiq-redis"
-version = "0.2.3"
+version = "0.3.0"
 description = "Redis integration for taskiq"
 authors = ["taskiq-team <taskiq@norely.com>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `taskiq_redis-0.2.3/taskiq_redis/redis_backend.py` & `taskiq_redis-0.3.0/taskiq_redis/redis_backend.py`

 * *Files identical despite different names*

### Comparing `taskiq_redis-0.2.3/taskiq_redis/redis_broker.py` & `taskiq_redis-0.3.0/taskiq_redis/redis_broker.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import pickle
-from abc import abstractmethod
 from logging import getLogger
 from typing import Any, AsyncGenerator, Callable, Optional, TypeVar
 
 from redis.asyncio import ConnectionPool, Redis
 from taskiq.abc.broker import AsyncBroker
 from taskiq.abc.result_backend import AsyncResultBackend
 from taskiq.message import BrokerMessage
@@ -48,73 +46,70 @@
         self.queue_name = queue_name
 
     async def shutdown(self) -> None:
         """Closes redis connection pool."""
         await super().shutdown()
         await self.connection_pool.disconnect()
 
-    async def listen(self) -> AsyncGenerator[BrokerMessage, None]:
-        """
-        Listen redis queue for new messages.
 
-        This function listens to the queue
-        and yields new messages if they have BrokerMessage type.
+class PubSubBroker(BaseRedisBroker):
+    """Broker that works with Redis and broadcasts tasks to all workers."""
 
-        :yields: broker messages.
+    async def kick(self, message: BrokerMessage) -> None:
         """
-        async for message in self._listen_to_raw_messages():
-            try:
-                redis_message = pickle.loads(message)
-                if isinstance(redis_message, BrokerMessage):
-                    yield redis_message
-            except (
-                TypeError,
-                AttributeError,
-                pickle.UnpicklingError,
-            ) as exc:
-                logger.debug(
-                    "Cannot read broker message %s",
-                    exc,
-                    exc_info=True,
-                )
+        Publish message over PUBSUB channel.
 
-    @abstractmethod
-    async def _listen_to_raw_messages(self) -> AsyncGenerator[bytes, None]:
+        :param message: message to send.
         """
-        Generator for reading raw data from Redis.
+        async with Redis(connection_pool=self.connection_pool) as redis_conn:
+            await redis_conn.publish(self.queue_name, message.message)
 
-        :yields: raw data.
+    async def listen(self) -> AsyncGenerator[bytes, None]:
         """
-        yield  # type: ignore
-
-
-class PubSubBroker(BaseRedisBroker):
-    """Broker that works with Redis and broadcasts tasks to all workers."""
+        Listen redis queue for new messages.
 
-    async def kick(self, message: BrokerMessage) -> None:  # noqa: D102
-        async with Redis(connection_pool=self.connection_pool) as redis_conn:
-            await redis_conn.publish(self.queue_name, pickle.dumps(message))
+        This function listens to the pubsub channel
+        and yields all messages with proper types.
 
-    async def _listen_to_raw_messages(self) -> AsyncGenerator[bytes, None]:
+        :yields: broker messages.
+        """
         async with Redis(connection_pool=self.connection_pool) as redis_conn:
             redis_pubsub_channel = redis_conn.pubsub()
             await redis_pubsub_channel.subscribe(self.queue_name)
             async for message in redis_pubsub_channel.listen():
                 if not message:
                     continue
+                if message["type"] != "message":
+                    logger.debug("Received non-message from redis: %s", message)
+                    continue
                 yield message["data"]
 
 
 class ListQueueBroker(BaseRedisBroker):
     """Broker that works with Redis and distributes tasks between workers."""
 
-    async def kick(self, message: BrokerMessage) -> None:  # noqa: D102
+    async def kick(self, message: BrokerMessage) -> None:
+        """
+        Put a message in a list.
+
+        This method appends a message to the list of all messages.
+
+        :param message: message to append.
+        """
         async with Redis(connection_pool=self.connection_pool) as redis_conn:
-            await redis_conn.lpush(self.queue_name, pickle.dumps(message))
+            await redis_conn.lpush(self.queue_name, message.message)
+
+    async def listen(self) -> AsyncGenerator[bytes, None]:
+        """
+        Listen redis queue for new messages.
 
-    async def _listen_to_raw_messages(self) -> AsyncGenerator[bytes, None]:
+        This function listens to the queue
+        and yields new messages if they have BrokerMessage type.
+
+        :yields: broker messages.
+        """
         redis_brpop_data_position = 1
         async with Redis(connection_pool=self.connection_pool) as redis_conn:
             while True:  # noqa: WPS457
                 yield (await redis_conn.brpop(self.queue_name))[
                     redis_brpop_data_position
                 ]
```

### Comparing `taskiq_redis-0.2.3/PKG-INFO` & `taskiq_redis-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq-redis
-Version: 0.2.3
+Version: 0.3.0
 Summary: Redis integration for taskiq
 Home-page: https://github.com/taskiq-python/taskiq-redis
 Keywords: taskiq,tasks,distributed,async,redis,result_backend
 Author: taskiq-team
 Author-email: taskiq@norely.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python
```

