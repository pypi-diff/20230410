# Comparing `tmp/dramatiq_mongodb-0.8.0.tar.gz` & `tmp/dramatiq_mongodb-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dramatiq_mongodb-0.8.0.tar", max compression
+gzip compressed data, was "dramatiq_mongodb-0.8.1.tar", max compression
```

## Comparing `dramatiq_mongodb-0.8.0.tar` & `dramatiq_mongodb-0.8.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     5838 2023-04-10 18:52:33.777534 dramatiq_mongodb-0.8.0/CHANGELOG.md
--rw-r--r--   0        0        0     1071 2023-04-10 18:51:48.456620 dramatiq_mongodb-0.8.0/LICENSE
--rw-r--r--   0        0        0     2096 2023-04-10 18:51:48.456620 dramatiq_mongodb-0.8.0/README.md
--rw-r--r--   0        0        0     2556 2023-04-10 18:52:33.789534 dramatiq_mongodb-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      172 2023-04-10 18:52:33.789534 dramatiq_mongodb-0.8.0/src/dramatiq_mongodb/__init__.py
--rw-r--r--   0        0        0     6538 2023-04-10 18:51:48.460620 dramatiq_mongodb-0.8.0/src/dramatiq_mongodb/backend.py
--rw-r--r--   0        0        0     8442 2023-04-10 18:51:48.460620 dramatiq_mongodb-0.8.0/src/dramatiq_mongodb/broker.py
--rw-r--r--   0        0        0      181 2023-04-10 18:51:48.460620 dramatiq_mongodb-0.8.0/src/dramatiq_mongodb/state.py
--rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 dramatiq_mongodb-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     6011 2023-04-10 20:09:40.601507 dramatiq_mongodb-0.8.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2023-04-10 20:09:01.765417 dramatiq_mongodb-0.8.1/LICENSE
+-rw-r--r--   0        0        0     2096 2023-04-10 20:09:01.765417 dramatiq_mongodb-0.8.1/README.md
+-rw-r--r--   0        0        0     2556 2023-04-10 20:09:40.609507 dramatiq_mongodb-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-04-10 20:09:40.609507 dramatiq_mongodb-0.8.1/src/dramatiq_mongodb/__init__.py
+-rw-r--r--   0        0        0     6538 2023-04-10 20:09:01.769417 dramatiq_mongodb-0.8.1/src/dramatiq_mongodb/backend.py
+-rw-r--r--   0        0        0     8260 2023-04-10 20:09:01.769417 dramatiq_mongodb-0.8.1/src/dramatiq_mongodb/broker.py
+-rw-r--r--   0        0        0      181 2023-04-10 20:09:01.769417 dramatiq_mongodb-0.8.1/src/dramatiq_mongodb/state.py
+-rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 dramatiq_mongodb-0.8.1/PKG-INFO
```

### Comparing `dramatiq_mongodb-0.8.0/CHANGELOG.md` & `dramatiq_mongodb-0.8.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.8.1 (2023-04-10)
+### Fix
+* Convert enqueue to insert ([`25a4f71`](https://github.com/obscuritylabs/dramatiq-mongodb/commit/25a4f719f51867b011865d32f14acdcfa1265bc9))
+
 ## v0.8.0 (2023-04-10)
 ### Feature
 * Bump dramatic version ([`5235637`](https://github.com/obscuritylabs/dramatiq-mongodb/commit/5235637d64edb0caa63a4890d8ce6f3acd17b99a))
 
 ### Fix
 * Resolve typing issues from updating dramatiq version ([`5039aca`](https://github.com/obscuritylabs/dramatiq-mongodb/commit/5039aca9e80345ce5e0873010decbd9a1a23f35b))
```

### Comparing `dramatiq_mongodb-0.8.0/LICENSE` & `dramatiq_mongodb-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dramatiq_mongodb-0.8.0/README.md` & `dramatiq_mongodb-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `dramatiq_mongodb-0.8.0/pyproject.toml` & `dramatiq_mongodb-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 authors = ["Tory Clasen <ToryClasen@Gmail.com>"]
 description = "Dramatiq-Mongodb Broker and Results Backend for Dramatiq"
 include = ["CHANGELOG.md"]
 license = "MIT"
 name = "dramatiq-mongodb"
 readme = "README.md"
 repository = "https://github.com/obscuritylabs/dramatiq-mongodb"
-version = "0.8.0"
+version = "0.8.1"
 
 [tool.poetry.dependencies]
 dramatiq = "^1.14.2"
 pymongo = ">=4.1,<5"
 python = ">=3.7,<4"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `dramatiq_mongodb-0.8.0/src/dramatiq_mongodb/backend.py` & `dramatiq_mongodb-0.8.1/src/dramatiq_mongodb/backend.py`

 * *Files identical despite different names*

### Comparing `dramatiq_mongodb-0.8.0/src/dramatiq_mongodb/broker.py` & `dramatiq_mongodb-0.8.1/src/dramatiq_mongodb/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,23 +103,22 @@
         self.emit_before("enqueue", message, delay)  # type: ignore
         queue_name = message.queue_name
         self.logger.debug(f"Enqueueing message {message.message_id} on queue {queue_name}")
         if delay:
             millis: int = current_millis()  # type: ignore
             message = message.copy(options={"eta": millis + delay})
 
-        document = {"msg": message.asdict(), "state": State.QUEUED}
+        document = {
+            "_id": UUID(message.message_id),
+            "msg": message.asdict(),
+            "state": State.QUEUED,
+        }
         collection = self.queues[queue_name]
-        results = collection.replace_one(
-            filter={"_id": UUID(message.message_id)},
-            replacement=document,
-            upsert=True,
-        )
-        if results.matched_count != 1 or results.modified_count != 1:
-            self.logger.exception(f"Failed to enqueue {message.message_id}")
+        collection.insert_one(document=document)
+
         self.emit_after("enqueue", message, delay)  # type: ignore
         return message
 
     def flush(self: MongoDBBroker, queue_name: str) -> None:
         """Drop collection that the queue resides in.
 
         Args:
```

### Comparing `dramatiq_mongodb-0.8.0/PKG-INFO` & `dramatiq_mongodb-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dramatiq-mongodb
-Version: 0.8.0
+Version: 0.8.1
 Summary: Dramatiq-Mongodb Broker and Results Backend for Dramatiq
 Home-page: https://github.com/obscuritylabs/dramatiq-mongodb
 License: MIT
 Author: Tory Clasen
 Author-email: ToryClasen@Gmail.com
 Requires-Python: >=3.7,<4
 Classifier: License :: OSI Approved :: MIT License
```

