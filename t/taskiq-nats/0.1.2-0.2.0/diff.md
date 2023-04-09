# Comparing `tmp/taskiq_nats-0.1.2.tar.gz` & `tmp/taskiq_nats-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_nats-0.1.2.tar", max compression
+gzip compressed data, was "taskiq_nats-0.2.0.tar", max compression
```

## Comparing `taskiq_nats-0.1.2.tar` & `taskiq_nats-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1293 2023-03-25 14:34:12.565394 taskiq_nats-0.1.2/README.md
--rw-r--r--   0        0        0     1453 2023-03-25 14:34:12.565394 taskiq_nats-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      171 2023-03-25 14:34:12.565394 taskiq_nats-0.1.2/taskiq_nats/__init__.py
--rw-r--r--   0        0        0     2470 2023-03-25 14:34:12.565394 taskiq_nats-0.1.2/taskiq_nats/broker.py
--rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 taskiq_nats-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1293 2023-04-09 23:53:49.566584 taskiq_nats-0.2.0/README.md
+-rw-r--r--   0        0        0     1453 2023-04-09 23:53:49.566584 taskiq_nats-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      171 2023-04-09 23:53:49.566584 taskiq_nats-0.2.0/taskiq_nats/__init__.py
+-rw-r--r--   0        0        0     2261 2023-04-09 23:53:49.566584 taskiq_nats-0.2.0/taskiq_nats/broker.py
+-rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 taskiq_nats-0.2.0/PKG-INFO
```

### Comparing `taskiq_nats-0.1.2/README.md` & `taskiq_nats-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `taskiq_nats-0.1.2/pyproject.toml` & `taskiq_nats-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskiq-nats"
-version = "0.1.2"
+version = "0.2.0"
 description = "NATS integration for taskiq"
 authors = ["taskiq-team <taskiq@norely.com>"]
 readme = "README.md"
 packages = [{ include = "taskiq_nats" }]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `taskiq_nats-0.1.2/taskiq_nats/broker.py` & `taskiq_nats-0.2.0/taskiq_nats/broker.py`

 * *Files 26% similar despite different names*

```diff
@@ -54,29 +54,25 @@
         """
         Send a message using NATS.
 
         :param message: message to send.
         """
         await self.client.publish(
             self.subject,
-            payload=message.json().encode(),
+            payload=message.message,
             headers=message.labels,
         )
 
-    async def listen(self) -> AsyncGenerator[BrokerMessage, None]:
+    async def listen(self) -> AsyncGenerator[bytes, None]:
         """
         Start listen to new messages.
 
         :yield: incoming messages.
         """
         subscribe = await self.client.subscribe(self.subject, queue=self.queue or "")
         async for message in subscribe.messages:
-            try:
-                yield BrokerMessage.parse_raw(message.data)
-            except ValueError:
-                data = message.data.decode("utf-8")
-                logger.warning(f"Cannot parse message: {data}")
+            yield message.data
 
     async def shutdown(self) -> None:
         """Close connections to NATS."""
         await self.client.close()
         await super().shutdown()
```

### Comparing `taskiq_nats-0.1.2/PKG-INFO` & `taskiq_nats-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq-nats
-Version: 0.1.2
+Version: 0.2.0
 Summary: NATS integration for taskiq
 Home-page: https://github.com/taskiq-python/taskiq-nats
 Keywords: taskiq,tasks,distributed,async,nats,result_backend
 Author: taskiq-team
 Author-email: taskiq@norely.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python
```

