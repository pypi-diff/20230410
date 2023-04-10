# Comparing `tmp/dramatiq_mongodb-0.7.0.tar.gz` & `tmp/dramatiq_mongodb-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dramatiq_mongodb-0.7.0.tar", max compression
+gzip compressed data, was "dramatiq_mongodb-0.7.1.tar", max compression
```

## Comparing `dramatiq_mongodb-0.7.0.tar` & `dramatiq_mongodb-0.7.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     5258 2022-12-27 21:14:44.077488 dramatiq_mongodb-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0     1071 2022-12-27 21:13:59.768914 dramatiq_mongodb-0.7.0/LICENSE
--rw-r--r--   0        0        0     2096 2022-12-27 21:13:59.768914 dramatiq_mongodb-0.7.0/README.md
--rw-r--r--   0        0        0     2556 2022-12-27 21:14:44.085488 dramatiq_mongodb-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      172 2022-12-27 21:14:44.085488 dramatiq_mongodb-0.7.0/src/dramatiq_mongodb/__init__.py
--rw-r--r--   0        0        0     5962 2022-12-27 21:13:59.772914 dramatiq_mongodb-0.7.0/src/dramatiq_mongodb/backend.py
--rw-r--r--   0        0        0     7758 2022-12-27 21:13:59.772914 dramatiq_mongodb-0.7.0/src/dramatiq_mongodb/broker.py
--rw-r--r--   0        0        0      181 2022-12-27 21:13:59.772914 dramatiq_mongodb-0.7.0/src/dramatiq_mongodb/state.py
--rw-r--r--   0        0        0     2933 1970-01-01 00:00:00.000000 dramatiq_mongodb-0.7.0/setup.py
--rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 dramatiq_mongodb-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     5488 2023-04-10 16:15:22.136869 dramatiq_mongodb-0.7.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2023-04-10 16:14:50.232860 dramatiq_mongodb-0.7.1/LICENSE
+-rw-r--r--   0        0        0     2096 2023-04-10 16:14:50.232860 dramatiq_mongodb-0.7.1/README.md
+-rw-r--r--   0        0        0     2556 2023-04-10 16:15:22.144869 dramatiq_mongodb-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-04-10 16:15:22.144869 dramatiq_mongodb-0.7.1/src/dramatiq_mongodb/__init__.py
+-rw-r--r--   0        0        0     6300 2023-04-10 16:14:50.232860 dramatiq_mongodb-0.7.1/src/dramatiq_mongodb/backend.py
+-rw-r--r--   0        0        0     8224 2023-04-10 16:14:50.232860 dramatiq_mongodb-0.7.1/src/dramatiq_mongodb/broker.py
+-rw-r--r--   0        0        0      181 2023-04-10 16:14:50.232860 dramatiq_mongodb-0.7.1/src/dramatiq_mongodb/state.py
+-rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 dramatiq_mongodb-0.7.1/PKG-INFO
```

### Comparing `dramatiq_mongodb-0.7.0/CHANGELOG.md` & `dramatiq_mongodb-0.7.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.7.1 (2023-04-10)
+### Fix
+* Add exception logging to any mongodb update failure to catch non-atomic operations ([`b5355d6`](https://github.com/obscuritylabs/dramatiq-mongodb/commit/b5355d6b5d93a14393e86b73a1df9df8dec519bf))
+
 ## v0.7.0 (2022-12-27)
 ### Feature
 * Add python 3.11 support to CI ([`3744ad8`](https://github.com/obscuritylabs/dramatiq-mongodb/commit/3744ad8bf0b33fc5f44cd73d980324c33e1defc1))
 
 ## v0.6.3 (2022-08-22)
 ### Fix
 * Close mongo client connection when broker is closed ([`263ef66`](https://github.com/obscuritylabs/dramatiq-mongodb/commit/263ef6656e437e109c3faabba8e87ebd64fcef3c))
```

### Comparing `dramatiq_mongodb-0.7.0/LICENSE` & `dramatiq_mongodb-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dramatiq_mongodb-0.7.0/README.md` & `dramatiq_mongodb-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `dramatiq_mongodb-0.7.0/pyproject.toml` & `dramatiq_mongodb-0.7.1/pyproject.toml`

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
-version = "0.7.0"
+version = "0.7.1"
 
 [tool.poetry.dependencies]
 dramatiq = "^1.12.1"
 pymongo = ">=4.1,<5"
 python = ">=3.7,<4"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `dramatiq_mongodb-0.7.0/src/dramatiq_mongodb/backend.py` & `dramatiq_mongodb-0.7.1/src/dramatiq_mongodb/backend.py`

 * *Files 5% similar despite different names*

```diff
@@ -141,26 +141,32 @@
         Args:
             message (Message): Message to store results for.
             result (Result): Result of successful processing.
             ttl (int): Not currently used.
         """
         ttl = ttl  # Ugly hack to get argument checker to let me leave this in.
         collection, message_key = self.build_message_key(message)
-        collection.update_one(
+        results = collection.update_one(
             filter={"_id": message_key},
             update={"$set": {"result": wrap_result(result)}},
         )
 
+        if results.matched_count != 1 or results.modified_count != 1:
+            self.logger.exception(f"Failed to store results for {message.message_id}")
+
     def store_exception(self: MongoDBBackend, message: Message, exception: Exception, ttl: Optional[int]) -> None:
         """Store result for a failed message as a serialized exception.
 
         Args:
             message (Message): Message to store results for.
             exception (Exception): Exception during processing.
             ttl (int): Not currently used.
         """
         ttl = ttl  # Ugly hack to get argument checker to let me leave this in.
         collection, message_key = self.build_message_key(message)
-        collection.update_one(
+        results = collection.update_one(
             filter={"_id": message_key},
             update={"$set": {"exception": wrap_exception(exception)}},
         )
+
+        if results.matched_count != 1 or results.modified_count != 1:
+            self.logger.exception(f"Failed to store exception for {message.message_id}")
```

### Comparing `dramatiq_mongodb-0.7.0/src/dramatiq_mongodb/broker.py` & `dramatiq_mongodb-0.7.1/src/dramatiq_mongodb/broker.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,19 +103,21 @@
         queue_name = message.queue_name
         self.logger.debug(f"Enqueueing message {message.message_id} on queue {queue_name}")
         if delay:
             message = message.copy(options={"eta": current_millis() + delay})
 
         document = {"msg": message.asdict(), "state": State.QUEUED}
         collection = self.queues[queue_name]
-        collection.replace_one(
+        results = collection.replace_one(
             filter={"_id": UUID(message.message_id)},
             replacement=document,
             upsert=True,
         )
+        if results.matched_count != 1 or results.modified_count != 1:
+            self.logger.exception(f"Failed to enqueue {message.message_id}")
         self.emit_after("enqueue", message, delay)
         return message
 
     def flush(self: MongoDBBroker, queue_name: str) -> None:
         """Drop collection that the queue resides in.
 
         Args:
@@ -184,30 +186,36 @@
 
     def ack(self: _MongoDBConsumer, message: MessageProxy) -> None:
         """Acknowledge a message as being processed.
 
         Args:
             message (MessageProxy): The message to ack.
         """
-        self.queue.update_one(
+        results = self.queue.update_one(
             filter={"_id": UUID(message.message_id), "state": State.CONSUMED},
             update={"$set": {"state": State.DONE}},
         )
 
+        if results.matched_count != 1 or results.modified_count != 1:
+            self.logger.exception(f"Failed to ack {message.message_id}")
+
     def nack(self: _MongoDBConsumer, message: MessageProxy) -> None:
         """Non-Acknowledge a message as having been rejected.
 
         Args:
             message (MessageProxy): The message to nack.
         """
-        self.queue.update_one(
+        results = self.queue.update_one(
             filter={"_id": UUID(message.message_id), "state": State.CONSUMED},
             update={"$set": {"state": State.REJECTED}},
         )
 
+        if results.matched_count != 1 or results.modified_count != 1:
+            self.logger.exception(f"Failed to nack {message.message_id}")
+
     def requeue(self: _MongoDBConsumer, messages: List[MessageProxy]) -> None:
         """Requeue all messaged that have been claimed but not acked or nacked.
 
         Args:
             messages (List[MessageProxy]): The list of messages to requeue.
         """
         for message in messages:
```

### Comparing `dramatiq_mongodb-0.7.0/setup.py` & `dramatiq_mongodb-0.7.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,72 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: dramatiq-mongodb
+Version: 0.7.1
+Summary: Dramatiq-Mongodb Broker and Results Backend for Dramatiq
+Home-page: https://github.com/obscuritylabs/dramatiq-mongodb
+License: MIT
+Author: Tory Clasen
+Author-email: ToryClasen@Gmail.com
+Requires-Python: >=3.7,<4
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: dramatiq (>=1.12.1,<2.0.0)
+Requires-Dist: pymongo (>=4.1,<5)
+Project-URL: Repository, https://github.com/obscuritylabs/dramatiq-mongodb
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# Dramatiq-Mongodb Broker and Results Backend for Dramatiq
 
-packages = \
-['dramatiq_mongodb']
+| :exclamation: _WARNING_ This is very early beta software that has not yet been proven to work. :exclamation: |
+| ------------------------------------------------------------------------------------------------------------ |
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['dramatiq>=1.12.1,<2.0.0', 'pymongo>=4.1,<5']
-
-setup_kwargs = {
-    'name': 'dramatiq-mongodb',
-    'version': '0.7.0',
-    'description': 'Dramatiq-Mongodb Broker and Results Backend for Dramatiq',
-    'long_description': "# Dramatiq-Mongodb Broker and Results Backend for Dramatiq\n\n| :exclamation: _WARNING_ This is very early beta software that has not yet been proven to work. :exclamation: |\n| ------------------------------------------------------------------------------------------------------------ |\n\n![CI/CD Pipeline](https://img.shields.io/github/actions/workflow/status/obscuritylabs/dramatiq-mongodb/ci-cd.yaml)\n\n![Latest SEMVER](https://img.shields.io/github/v/tag/obscuritylabs/dramatiq-mongodb)\n\n## Usage Instructions\n\n## Development Instructions\n\n### Configure development environment\n\nInstall Development Dependencies using Poetry:\n\n```shell\npoetry install\n```\n\nInstall githooks to automate quality checks locally:\n\n```shell\npoetry run pre-commit install --install-hooks -t pre-commit -t commit-msg\n```\n\n### Run code quality checks locally\n\nAll code quality checks are performed using the Makefile at the root of the repository. You can execute individual steps by name or execute all steps by omitting a target using `make` or specifying `make all`:\n\n```shell\nmake all\n```\n\nIf you want to purge the repo of all ignore files include the embedded virtual environment then run all tests in a fresh environment you can run:\n\n```shell\nmake clean all\n```\n\nChangelog and semantic version are automated using [Semantic-Release](https://python-semantic-release.readthedocs.io/en/latest/) during the CD process. To accomplish this, this repository makes heavy use of [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/), thought this isn't strictly enforced on the server side at this time until 1.0 is released, but the githooks will lint your commits.\n\n### Start a local MongoDB\n\n```shell\ndocker run -d -p 27017:27017 --name mongo -e MONGO_INITDB_ROOT_USERNAME=username -e MONGO_INITDB_ROOT_PASSWORD=password mongo\n```\n\nOnce the mongodb server is up and running you can create a pymongo client and pass it either into a MongoDBBroker or a MongoDBBackend to test the code locally. Otherwise everything should behave in accordance with the documentation for [Dramatiq](https://dramatiq.io/).\n",
-    'author': 'Tory Clasen',
-    'author_email': 'ToryClasen@Gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/obscuritylabs/dramatiq-mongodb',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4',
-}
+![CI/CD Pipeline](https://img.shields.io/github/actions/workflow/status/obscuritylabs/dramatiq-mongodb/ci-cd.yaml)
 
+![Latest SEMVER](https://img.shields.io/github/v/tag/obscuritylabs/dramatiq-mongodb)
+
+## Usage Instructions
+
+## Development Instructions
+
+### Configure development environment
+
+Install Development Dependencies using Poetry:
+
+```shell
+poetry install
+```
+
+Install githooks to automate quality checks locally:
+
+```shell
+poetry run pre-commit install --install-hooks -t pre-commit -t commit-msg
+```
+
+### Run code quality checks locally
+
+All code quality checks are performed using the Makefile at the root of the repository. You can execute individual steps by name or execute all steps by omitting a target using `make` or specifying `make all`:
+
+```shell
+make all
+```
+
+If you want to purge the repo of all ignore files include the embedded virtual environment then run all tests in a fresh environment you can run:
+
+```shell
+make clean all
+```
+
+Changelog and semantic version are automated using [Semantic-Release](https://python-semantic-release.readthedocs.io/en/latest/) during the CD process. To accomplish this, this repository makes heavy use of [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/), thought this isn't strictly enforced on the server side at this time until 1.0 is released, but the githooks will lint your commits.
+
+### Start a local MongoDB
+
+```shell
+docker run -d -p 27017:27017 --name mongo -e MONGO_INITDB_ROOT_USERNAME=username -e MONGO_INITDB_ROOT_PASSWORD=password mongo
+```
+
+Once the mongodb server is up and running you can create a pymongo client and pass it either into a MongoDBBroker or a MongoDBBackend to test the code locally. Otherwise everything should behave in accordance with the documentation for [Dramatiq](https://dramatiq.io/).
 
-setup(**setup_kwargs)
```

