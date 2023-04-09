# Comparing `tmp/taskiq_aio_pika-0.1.1.tar.gz` & `tmp/taskiq_aio_pika-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_aio_pika-0.1.1.tar", max compression
+gzip compressed data, was "taskiq_aio_pika-0.2.0.tar", max compression
```

## Comparing `taskiq_aio_pika-0.1.1.tar` & `taskiq_aio_pika-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3262 2023-03-25 14:33:19.868368 taskiq_aio_pika-0.1.1/README.md
--rw-r--r--   0        0        0     1492 2023-03-25 14:33:19.868368 taskiq_aio_pika-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      118 2023-03-25 14:33:19.868368 taskiq_aio_pika-0.1.1/taskiq_aio_pika/__init__.py
--rw-r--r--   0        0        0     9698 2023-03-25 14:33:19.868368 taskiq_aio_pika-0.1.1/taskiq_aio_pika/broker.py
--rw-r--r--   0        0        0     4381 1970-01-01 00:00:00.000000 taskiq_aio_pika-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3262 2023-04-09 23:57:13.266202 taskiq_aio_pika-0.2.0/README.md
+-rw-r--r--   0        0        0     1492 2023-04-09 23:57:13.266202 taskiq_aio_pika-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-04-09 23:57:13.266202 taskiq_aio_pika-0.2.0/taskiq_aio_pika/__init__.py
+-rw-r--r--   0        0        0     8864 2023-04-09 23:57:13.266202 taskiq_aio_pika-0.2.0/taskiq_aio_pika/broker.py
+-rw-r--r--   0        0        0     4381 1970-01-01 00:00:00.000000 taskiq_aio_pika-0.2.0/PKG-INFO
```

### Comparing `taskiq_aio_pika-0.1.1/README.md` & `taskiq_aio_pika-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `taskiq_aio_pika-0.1.1/pyproject.toml` & `taskiq_aio_pika-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskiq-aio-pika"
-version = "0.1.1"
+version = "0.2.0"
 description = "RabbitMQ broker for taskiq"
 authors = ["Pavel Kirilin <win10@list.ru>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `taskiq_aio_pika-0.1.1/taskiq_aio_pika/broker.py` & `taskiq_aio_pika-0.2.0/taskiq_aio_pika/broker.py`

 * *Files 3% similar despite different names*

```diff
@@ -187,15 +187,15 @@
         :raises ValueError: if startup wasn't called.
         :param message: message to send.
         """
         if self.write_channel is None:
             raise ValueError("Please run startup before kicking.")
         priority = parse_val(int, message.labels.get("priority"))
         rmq_msg = Message(
-            body=message.message.encode(),
+            body=message.message,
             headers={
                 "task_id": message.task_id,
                 "task_name": message.task_name,
                 **message.labels,
             },
             delivery_mode=DeliveryMode.PERSISTENT,
             priority=priority,
@@ -210,15 +210,15 @@
         else:
             rmq_msg.expiration = timedelta(seconds=delay)
             await self.write_channel.default_exchange.publish(
                 rmq_msg,
                 routing_key=self._delay_queue_name,
             )
 
-    async def listen(self) -> AsyncGenerator[BrokerMessage, None]:  # noqa: WPS210
+    async def listen(self) -> AsyncGenerator[bytes, None]:
         """
         Listen to queue.
 
         This function listens to queue and
         yields every new message.
 
         :yields: parsed broker message.
@@ -227,33 +227,15 @@
         if self.read_channel is None:
             raise ValueError("Call startup before starting listening.")
         await self.read_channel.set_qos(prefetch_count=self._qos)
         queue = await self.declare_queues(self.read_channel)
         async with queue.iterator() as iterator:
             async for message in iterator:
                 async with message.process():
-                    headers = {}
-                    for header_name, header_value in message.headers.items():
-                        headers[header_name] = str(header_value)
-                    try:
-                        broker_message = BrokerMessage(
-                            task_id=headers.pop("task_id"),
-                            task_name=headers.pop("task_name"),
-                            message=message.body,
-                            labels=headers,
-                        )
-                    except (ValueError, LookupError) as exc:
-                        logger.warning(
-                            "Cannot read broker message %s",
-                            exc,
-                            exc_info=True,
-                        )
-                        continue
-
-                    yield broker_message
+                    yield message.body
 
     async def shutdown(self) -> None:
         """Close all connections on shutdown."""
         await super().shutdown()
         if self.write_channel:
             await self.write_channel.close()
         if self.read_channel:
```

### Comparing `taskiq_aio_pika-0.1.1/PKG-INFO` & `taskiq_aio_pika-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq-aio-pika
-Version: 0.1.1
+Version: 0.2.0
 Summary: RabbitMQ broker for taskiq
 Home-page: https://github.com/taskiq-python/taskiq-aio-pika
 Keywords: taskiq,tasks,distributed,async,aio-pika
 Author: Pavel Kirilin
 Author-email: win10@list.ru
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python
```

