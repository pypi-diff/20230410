# Comparing `tmp/dramatiq_mongodb-0.7.1.tar.gz` & `tmp/dramatiq_mongodb-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dramatiq_mongodb-0.7.1.tar", max compression
+gzip compressed data, was "dramatiq_mongodb-0.8.0.tar", max compression
```

## Comparing `dramatiq_mongodb-0.7.1.tar` & `dramatiq_mongodb-0.8.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     5488 2023-04-10 16:15:22.136869 dramatiq_mongodb-0.7.1/CHANGELOG.md
--rw-r--r--   0        0        0     1071 2023-04-10 16:14:50.232860 dramatiq_mongodb-0.7.1/LICENSE
--rw-r--r--   0        0        0     2096 2023-04-10 16:14:50.232860 dramatiq_mongodb-0.7.1/README.md
--rw-r--r--   0        0        0     2556 2023-04-10 16:15:22.144869 dramatiq_mongodb-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      172 2023-04-10 16:15:22.144869 dramatiq_mongodb-0.7.1/src/dramatiq_mongodb/__init__.py
--rw-r--r--   0        0        0     6300 2023-04-10 16:14:50.232860 dramatiq_mongodb-0.7.1/src/dramatiq_mongodb/backend.py
--rw-r--r--   0        0        0     8224 2023-04-10 16:14:50.232860 dramatiq_mongodb-0.7.1/src/dramatiq_mongodb/broker.py
--rw-r--r--   0        0        0      181 2023-04-10 16:14:50.232860 dramatiq_mongodb-0.7.1/src/dramatiq_mongodb/state.py
--rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 dramatiq_mongodb-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     5838 2023-04-10 18:52:33.777534 dramatiq_mongodb-0.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2023-04-10 18:51:48.456620 dramatiq_mongodb-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2096 2023-04-10 18:51:48.456620 dramatiq_mongodb-0.8.0/README.md
+-rw-r--r--   0        0        0     2556 2023-04-10 18:52:33.789534 dramatiq_mongodb-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-04-10 18:52:33.789534 dramatiq_mongodb-0.8.0/src/dramatiq_mongodb/__init__.py
+-rw-r--r--   0        0        0     6538 2023-04-10 18:51:48.460620 dramatiq_mongodb-0.8.0/src/dramatiq_mongodb/backend.py
+-rw-r--r--   0        0        0     8442 2023-04-10 18:51:48.460620 dramatiq_mongodb-0.8.0/src/dramatiq_mongodb/broker.py
+-rw-r--r--   0        0        0      181 2023-04-10 18:51:48.460620 dramatiq_mongodb-0.8.0/src/dramatiq_mongodb/state.py
+-rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 dramatiq_mongodb-0.8.0/PKG-INFO
```

### Comparing `dramatiq_mongodb-0.7.1/CHANGELOG.md` & `dramatiq_mongodb-0.8.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.8.0 (2023-04-10)
+### Feature
+* Bump dramatic version ([`5235637`](https://github.com/obscuritylabs/dramatiq-mongodb/commit/5235637d64edb0caa63a4890d8ce6f3acd17b99a))
+
+### Fix
+* Resolve typing issues from updating dramatiq version ([`5039aca`](https://github.com/obscuritylabs/dramatiq-mongodb/commit/5039aca9e80345ce5e0873010decbd9a1a23f35b))
+
 ## v0.7.1 (2023-04-10)
 ### Fix
 * Add exception logging to any mongodb update failure to catch non-atomic operations ([`b5355d6`](https://github.com/obscuritylabs/dramatiq-mongodb/commit/b5355d6b5d93a14393e86b73a1df9df8dec519bf))
 
 ## v0.7.0 (2022-12-27)
 ### Feature
 * Add python 3.11 support to CI ([`3744ad8`](https://github.com/obscuritylabs/dramatiq-mongodb/commit/3744ad8bf0b33fc5f44cd73d980324c33e1defc1))
```

### Comparing `dramatiq_mongodb-0.7.1/LICENSE` & `dramatiq_mongodb-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dramatiq_mongodb-0.7.1/README.md` & `dramatiq_mongodb-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `dramatiq_mongodb-0.7.1/pyproject.toml` & `dramatiq_mongodb-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -56,33 +56,33 @@
 authors = ["Tory Clasen <ToryClasen@Gmail.com>"]
 description = "Dramatiq-Mongodb Broker and Results Backend for Dramatiq"
 include = ["CHANGELOG.md"]
 license = "MIT"
 name = "dramatiq-mongodb"
 readme = "README.md"
 repository = "https://github.com/obscuritylabs/dramatiq-mongodb"
-version = "0.7.1"
+version = "0.8.0"
 
 [tool.poetry.dependencies]
-dramatiq = "^1.12.1"
+dramatiq = "^1.14.2"
 pymongo = ">=4.1,<5"
 python = ">=3.7,<4"
 
 [tool.poetry.group.dev.dependencies]
 autoflake = "^1.4"
 black = "^22.3.0"
 commitizen = "^2.23.0"
 darglint = "^1.8.1"
 dlint = "^0.12.0"
 dramatiq = {extras = ["watch"], version = "^1.13.0"}
 flake8-bugbear = "^22.3.23"
 flake8-docstrings = "^1.6.0"
 flake8-pep518 = "^0.1.0"
 isort = "^5.10.1"
-mypy = "^0.942"
+mypy = "^1.2.0"
 pre-commit = "^2.17.0"
 pytest = "^7.1.1"
 pytest-clarity = "^1.0.1"
 pytest-cov = "^3.0.0"
 pytest-sugar = "^0.9.4"
 pytest-xdist = "^3.1.0"
 python-semantic-release = "^7.27.0"
```

### Comparing `dramatiq_mongodb-0.7.1/src/dramatiq_mongodb/backend.py` & `dramatiq_mongodb-0.8.0/src/dramatiq_mongodb/backend.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import time
+from logging import Logger
 from typing import Any
 from typing import Dict
 from typing import Optional
-from typing import Tuple
 from uuid import UUID
 
 from bson.binary import UuidRepresentation
 from bson.codec_options import CodecOptions
 from dramatiq.common import compute_backoff
 from dramatiq.encoder import Encoder
 from dramatiq.logging import get_logger
@@ -26,15 +26,15 @@
 #: The default timeout for blocking get operations in milliseconds.
 DEFAULT_TIMEOUT = 10000
 
 #: The minimum amount of time in ms to wait between polls.
 BACKOFF_FACTOR = 100
 
 
-class MongoDBBackend(ResultBackend):  # type: ignore
+class MongoDBBackend(ResultBackend):
     """Results Backend for MongoDB."""
 
     def __init__(
         self: MongoDBBackend,
         *,
         database: Database[Any],
         collection_prefix: Optional[str] = "",
@@ -53,120 +53,122 @@
             namespace = "dramatiq-results"
 
         super().__init__(namespace=namespace, encoder=encoder)
 
         if collection_prefix:
             collection_prefix = collection_prefix.rstrip("_") + "_"
 
-        self._collection_prefix = collection_prefix
+        self._collection_prefix = collection_prefix or ""
 
-        self.logger = get_logger(__name__, type(self))
+        self.logger: Logger = get_logger(__name__, type(self))  # type: ignore
         self.database = database
 
-    def build_message_key(self: MongoDBBackend, message: Message) -> Tuple[Collection[Any], UUID]:
+    def build_message_key(self: MongoDBBackend, message: Message[Any]) -> str:
         """Extract the MongoDB Collection name and UUID used for documents from messae.
 
         Args:
-            message (Message): The message with which to extract information from.
+            message (Message[Any]): The message with which to extract information from.
 
         Returns:
-            Tuple[Collection, UUID]: MongoDB Collection and UUID of document in it.
+            str: Message ID in str format.
         """
-        return (
-            self.get_collection(message),
-            UUID(message.message_id),
-        )
+        return message.message_id
 
-    def get_collection(self: MongoDBBackend, message: Message) -> Collection[Any]:
+    def get_collection(self: MongoDBBackend, message: Message[Any]) -> Collection[Any]:
         """Return handle to collection based on metadata in message.
 
         Args:
-            message (Message): Message containing queue name.
+            message (Message[Any]): Message[Any] containing queue name.
 
         Returns:
             Collection: Collection handle to use for results.
         """
         std_opts = CodecOptions(uuid_representation=UuidRepresentation.STANDARD)  # type: ignore
         return self.database.get_collection(self._collection_prefix + message.queue_name, codec_options=std_opts)
 
     def get_result(
         self: MongoDBBackend,
-        message: Message,
+        message: Message[Any],
         *,
         block: Optional[bool] = False,
         timeout: Optional[int] = None,
     ) -> Dict[Any, Any]:
         """Return results from a task.
 
         Args:
-            message (Message): The message to retrieve results for.
+            message (Message[Any]): The message to retrieve results for.
             block (bool, optional): Block process flow until result is available. Defaults to False.
             timeout (int, optional): Milliseconds to wait for a result to become available. Defaults to None.
 
         Raises:
             ResultTimeout: No result was available within timeout period.
             ResultMissing: No result was found.
 
         Returns:
             Result:
         """
         if timeout is None:
             timeout = DEFAULT_TIMEOUT
 
         end_time = time.monotonic() + timeout / 1000
-        collection, message_key = self.build_message_key(message)
+        collection = self.get_collection(message)
+        message_key = UUID(self.build_message_key(message))
         attempts = 0
 
         while True:
-            attempts, delay = compute_backoff(attempts, factor=BACKOFF_FACTOR)
+            attempts, delay = compute_backoff(attempts, factor=BACKOFF_FACTOR)  # type: ignore
             delay /= 1000
             time_expired = time.monotonic() + delay > end_time
 
             document = collection.find_one(filter={"_id": message_key, "state": State.DONE})
 
             if document:
-                result: Dict[Any, Any] = self.unwrap_result(document["result"])
+                result: Dict[Any, Any] = self.unwrap_result(document["result"])  # type: ignore
                 return result
 
             elif not block:
-                raise ResultMissing(message)
+                raise ResultMissing(message)  # type: ignore
 
             elif time_expired:
-                raise ResultTimeout(message)
+                raise ResultTimeout(message)  # type: ignore
 
             time.sleep(delay)
 
-    def store_result(self: MongoDBBackend, message: Message, result: Dict[Any, Any], ttl: Optional[int]) -> None:
+    def store_result(self: MongoDBBackend, message: Message[Any], result: Dict[Any, Any], ttl: Optional[int]) -> None:
         """Store result for a successful message.
 
         Args:
-            message (Message): Message to store results for.
+            message (Message[Any]): Message[Any] to store results for.
             result (Result): Result of successful processing.
             ttl (int): Not currently used.
         """
         ttl = ttl  # Ugly hack to get argument checker to let me leave this in.
-        collection, message_key = self.build_message_key(message)
+        collection = self.get_collection(message)
+        message_key = UUID(self.build_message_key(message))
+        res: dict[Any, Any] = wrap_result(result)  # type: ignore
         results = collection.update_one(
             filter={"_id": message_key},
-            update={"$set": {"result": wrap_result(result)}},
+            update={"$set": {"result": res}},
         )
 
         if results.matched_count != 1 or results.modified_count != 1:
             self.logger.exception(f"Failed to store results for {message.message_id}")
 
-    def store_exception(self: MongoDBBackend, message: Message, exception: Exception, ttl: Optional[int]) -> None:
+    def store_exception(self: MongoDBBackend, message: Message[Any], exception: Exception, ttl: Optional[int]) -> None:
         """Store result for a failed message as a serialized exception.
 
         Args:
-            message (Message): Message to store results for.
+            message (Message[Any]): Message[Any] to store results for.
             exception (Exception): Exception during processing.
             ttl (int): Not currently used.
         """
         ttl = ttl  # Ugly hack to get argument checker to let me leave this in.
-        collection, message_key = self.build_message_key(message)
+        collection = self.get_collection(message)
+        message_key = UUID(self.build_message_key(message))
+        exc: dict[str, Any] = wrap_exception(exception)  # type: ignore
         results = collection.update_one(
             filter={"_id": message_key},
-            update={"$set": {"exception": wrap_exception(exception)}},
+            update={"$set": {"exception": exc}},
         )
 
         if results.matched_count != 1 or results.modified_count != 1:
             self.logger.exception(f"Failed to store exception for {message.message_id}")
```

### Comparing `dramatiq_mongodb-0.7.1/src/dramatiq_mongodb/broker.py` & `dramatiq_mongodb-0.8.0/src/dramatiq_mongodb/broker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from collections import deque
+from logging import Logger
 from typing import Any
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
 from uuid import UUID
 
@@ -20,15 +21,15 @@
 from dramatiq.message import Message
 from pymongo.collection import Collection
 from pymongo.database import Database
 
 from dramatiq_mongodb.state import State
 
 
-class MongoDBBroker(Broker):  # type: ignore
+class MongoDBBroker(Broker):
     """A broker that can be used with MongoDB."""
 
     def __init__(
         self: MongoDBBroker,
         *,
         database: Database[Any],
         collection_prefix: Optional[str] = "",
@@ -37,17 +38,17 @@
         """Initialize a new MongoDB Broker.
 
         Args:
             database (Database): The database to create collections in
             collection_prefix (str, optional): Prefix for all newly created collections. Defaults to "".
             middleware (Optional[List[Middleware]], optional): Middlware to pass to Dramatiq. Defaults to None.
         """
-        super().__init__(middleware=middleware)
+        super().__init__(middleware=middleware)  # type: ignore
 
-        self.logger = get_logger(__name__, type(self))
+        self.logger: Logger = get_logger(__name__, type(self))  # type: ignore
         self.database = database
 
         self._collection_prefix = ""
 
         if collection_prefix:
             self._collection_prefix = collection_prefix.rstrip("_") + "_"
 
@@ -80,45 +81,46 @@
 
         Args:
             queue_name (str): Name of queue to pull tasks from.
         """
         if queue_name not in self.queues:
             collection_name = self._collection_prefix + queue_name
             self.logger.debug(f"Creating queue ({queue_name}) which will have a collection name of {collection_name}")
-            self.emit_before("declare_queue", queue_name)
+            self.emit_before("declare_queue", queue_name)  # type: ignore
             std_opts = CodecOptions[Any](uuid_representation=UuidRepresentation.STANDARD)
             self.queues[queue_name] = self.database.get_collection(collection_name, codec_options=std_opts)
-            self.emit_after("declare_queue", queue_name)
+            self.emit_after("declare_queue", queue_name)  # type: ignore
 
-    def enqueue(self: MongoDBBroker, message: Message, *, delay: Optional[int] = None) -> Message:
+    def enqueue(self: MongoDBBroker, message: Message[Any], *, delay: Optional[int] = None) -> Message[Any]:
         """Enqueue a new message on the designated queue.
 
         Args:
-            message (Message): The message to enqueue
+            message (Message[Any]): The message to enqueue
             delay (Optional[int], optional): Milliseconds until message should br processed. Defaults to None.
 
         Returns:
-            Message: The message that was enqueued.
+            Message[Any]: The message that was enqueued.
         """
-        self.emit_before("enqueue", message, delay)
+        self.emit_before("enqueue", message, delay)  # type: ignore
         queue_name = message.queue_name
         self.logger.debug(f"Enqueueing message {message.message_id} on queue {queue_name}")
         if delay:
-            message = message.copy(options={"eta": current_millis() + delay})
+            millis: int = current_millis()  # type: ignore
+            message = message.copy(options={"eta": millis + delay})
 
         document = {"msg": message.asdict(), "state": State.QUEUED}
         collection = self.queues[queue_name]
         results = collection.replace_one(
             filter={"_id": UUID(message.message_id)},
             replacement=document,
             upsert=True,
         )
         if results.matched_count != 1 or results.modified_count != 1:
             self.logger.exception(f"Failed to enqueue {message.message_id}")
-        self.emit_after("enqueue", message, delay)
+        self.emit_after("enqueue", message, delay)  # type: ignore
         return message
 
     def flush(self: MongoDBBroker, queue_name: str) -> None:
         """Drop collection that the queue resides in.
 
         Args:
             queue_name (str): name of the collection to drop.
@@ -136,15 +138,15 @@
 
         Returns:
             Iterable[str]: List of all queues on the broker.
         """
         return set(self.queues.keys())
 
 
-class _MongoDBConsumer(Consumer):  # type: ignore
+class _MongoDBConsumer(Consumer):
     def __init__(
         self: _MongoDBConsumer,
         broker: MongoDBBroker,
         queue: Collection[Any],
         prefetch: Optional[int],
         timeout: Optional[int],
     ) -> None:
@@ -152,18 +154,18 @@
 
         Args:
             broker (MongoDBBroker): The broker this consumer is attached to.
             queue (Collection): The queue to consume messages from.
             prefetch (Optional[int]): Not currently used.
             timeout (Optional[int]): Not currently used.
         """
-        self.logger = get_logger(__name__, type(self))
+        self.logger: Logger = get_logger(__name__, type(self))  # type: ignore
         self.broker = broker
         self.queue: Collection[Any] = queue
-        self.messages: deque[Message] = deque()
+        self.messages: deque[Message[Any]] = deque()
         self.prefetch = prefetch
         self.timeout = timeout
 
     def __next__(self: _MongoDBConsumer) -> Optional[MessageProxy]:
         """Next item in the queue to be processed.
 
         Returns:
@@ -174,15 +176,15 @@
                 "state": State.QUEUED,
             },
             update={"$set": {"state": State.CONSUMED}},
             sort=[("timestamp", pymongo.ASCENDING)],
         )
         try:
             if document:
-                return MessageProxy(Message(**document["msg"]))
+                return MessageProxy(Message[Any](**document["msg"]))  # type: ignore
             return None
         except Exception as e:
             self.logger.exception(f"Failed to decode message: {document}. Error is: {e}")
             return None
 
     def ack(self: _MongoDBConsumer, message: MessageProxy) -> None:
         """Acknowledge a message as being processed.
```

### Comparing `dramatiq_mongodb-0.7.1/PKG-INFO` & `dramatiq_mongodb-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: dramatiq-mongodb
-Version: 0.7.1
+Version: 0.8.0
 Summary: Dramatiq-Mongodb Broker and Results Backend for Dramatiq
 Home-page: https://github.com/obscuritylabs/dramatiq-mongodb
 License: MIT
 Author: Tory Clasen
 Author-email: ToryClasen@Gmail.com
 Requires-Python: >=3.7,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: dramatiq (>=1.12.1,<2.0.0)
+Requires-Dist: dramatiq (>=1.14.2,<2.0.0)
 Requires-Dist: pymongo (>=4.1,<5)
 Project-URL: Repository, https://github.com/obscuritylabs/dramatiq-mongodb
 Description-Content-Type: text/markdown
 
 # Dramatiq-Mongodb Broker and Results Backend for Dramatiq
 
 | :exclamation: _WARNING_ This is very early beta software that has not yet been proven to work. :exclamation: |
```

