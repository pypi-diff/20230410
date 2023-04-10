# Comparing `tmp/kaflow-0.1.1.tar.gz` & `tmp/kaflow-0.1.2.tar.gz`

## Comparing `kaflow-0.1.1.tar` & `kaflow-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 kaflow-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 kaflow-0.1.1/Makefile
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 kaflow-0.1.1/.github/workflows/release.yaml
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 kaflow-0.1.1/.github/workflows/test.yaml
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/__init__.py
--rw-r--r--   0        0        0     8100 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/_consumer.py
--rw-r--r--   0        0        0    21919 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/applications.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/dependencies.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/exceptions.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/logger.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/message.py
--rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/py.typed
--rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/serializers.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/_utils/__init__.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/_utils/asyncio.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/_utils/inspect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/asyncapi/__init__.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/asyncapi/_builder.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/asyncapi/docs.py
--rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/asyncapi/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 kaflow-0.1.1/tests/key_value.proto
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 kaflow-0.1.1/tests/key_value_pb2.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 kaflow-0.1.1/tests/key_value_pb2.pyi
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 kaflow-0.1.1/tests/test_application.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 kaflow-0.1.1/tests/test_serializers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.1/tests/_utils/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 kaflow-0.1.1/tests/_utils/test_asyncio.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 kaflow-0.1.1/tests/_utils/test_inspect.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 kaflow-0.1.1/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 kaflow-0.1.1/LICENSE
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 kaflow-0.1.1/README.md
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 kaflow-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 kaflow-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 kaflow-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 kaflow-0.1.2/Makefile
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 kaflow-0.1.2/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 kaflow-0.1.2/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/__init__.py
+-rw-r--r--   0        0        0     8453 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/_consumer.py
+-rw-r--r--   0        0        0    21832 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/applications.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/dependencies.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/exceptions.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/logger.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/message.py
+-rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/py.typed
+-rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/serializers.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/_utils/__init__.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/_utils/asyncio.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/_utils/inspect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/asyncapi/__init__.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/asyncapi/_builder.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/asyncapi/docs.py
+-rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/asyncapi/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 kaflow-0.1.2/tests/key_value.proto
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 kaflow-0.1.2/tests/key_value_pb2.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 kaflow-0.1.2/tests/key_value_pb2.pyi
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 kaflow-0.1.2/tests/test_application.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 kaflow-0.1.2/tests/test_serializers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.2/tests/_utils/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 kaflow-0.1.2/tests/_utils/test_asyncio.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 kaflow-0.1.2/tests/_utils/test_inspect.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 kaflow-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 kaflow-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 kaflow-0.1.2/README.md
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 kaflow-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 kaflow-0.1.2/PKG-INFO
```

### Comparing `kaflow-0.1.1/.github/workflows/release.yaml` & `kaflow-0.1.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.1/.github/workflows/test.yaml` & `kaflow-0.1.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.1/kaflow/__init__.py` & `kaflow-0.1.2/kaflow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,8 +31,8 @@
     __all__.append("Avro")
 
 if has_protobuf:
     from kaflow.serializers import Protobuf  # noqa: F401
 
     __all__.append("Protobuf")
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

### Comparing `kaflow-0.1.1/kaflow/_consumer.py` & `kaflow-0.1.2/kaflow/_consumer.py`

 * *Files 3% similar despite different names*

```diff
@@ -184,27 +184,38 @@
                 e,
             )
             headers = None
             deserialized
 
         return value, key, headers, deserialized
 
+    def _lookup_exception_handler(
+        self, exc: Exception
+    ) -> Callable[..., Awaitable[None]] | None:
+        for cls in type(exc).__mro__:
+            if cls in self.exception_handlers:
+                return self.exception_handlers[cls]
+        return None
+
     async def _execute_dependent(
         self,
         consumer_state: ScopeState,
         message: ReadMessage,
     ) -> Any:
         try:
             return await self.dependent.execute_async(
                 executor=self.executor,
                 state=consumer_state,
                 values={ReadMessage: message},
             )
         except tuple(self.exception_handlers.keys()) as e:
-            await self.exception_handlers[type(e)](e)
+            handler = self._lookup_exception_handler(e)
+            if not handler:
+                raise e
+            await handler(e)
             return None
 
     async def _publish_messages(self, message: Message) -> None:
         if self.sink_topics:
             await asyncio.gather(
                 *[
                     self.publish_fn(
```

### Comparing `kaflow-0.1.1/kaflow/applications.py` & `kaflow-0.1.2/kaflow/applications.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,17 +83,15 @@
         max_poll_interval_ms: int = 300000,
         rebalance_timeout_ms: int | None = None,
         session_timeout_ms: int = 10000,
         heartbeat_interval_ms: int = 3000,
         consumer_timeout_ms: int = 200,
         max_poll_records: int | None = None,
         kafka_api_version: str = "auto",
-        security_protocol: Literal[
-            "PLAINTEXT", "SSL", "SASL_PLAINTEXT", "SASL_SSL"
-        ] = "PLAINTEXT",
+        security_protocol: Literal["PLAINTEXT", "SSL"] = "PLAINTEXT",
         exclude_internal_topics: bool = True,
         connection_max_idle_ms: int = 540000,
         isolation_level: Literal[
             "read_committed", "read_uncommitted"
         ] = "read_committed",
         cafile: str | None = None,
         capath: str | None = None,
@@ -168,15 +166,15 @@
         self.sasl_mechanism = sasl_mechanism
         self.sasl_plain_username = sasl_plain_username
         self.sasl_plain_password = sasl_plain_password
         self.sasl_kerberos_service_name = sasl_kerberos_service_name
         self.sasl_kerberos_domain_name = sasl_kerberos_domain_name
         self.sasl_oauth_token_provider = sasl_oauth_token_provider
 
-        if security_protocol == "SSL" or security_protocol == "SASL_SSL":
+        if security_protocol == "SSL":
             self.ssl_context = create_ssl_context(
                 cafile=cafile,
                 capath=capath,
                 cadata=cadata,
                 certfile=certfile,
                 keyfile=keyfile,
                 password=cert_password,
```

### Comparing `kaflow-0.1.1/kaflow/message.py` & `kaflow-0.1.2/kaflow/message.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.1/kaflow/parameters.py` & `kaflow-0.1.2/kaflow/parameters.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.1/kaflow/serializers.py` & `kaflow-0.1.2/kaflow/serializers.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.1/kaflow/_utils/asyncio.py` & `kaflow-0.1.2/kaflow/_utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.1/kaflow/_utils/inspect.py` & `kaflow-0.1.2/kaflow/_utils/inspect.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.1/kaflow/asyncapi/_builder.py` & `kaflow-0.1.2/kaflow/asyncapi/_builder.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.1/kaflow/asyncapi/docs.py` & `kaflow-0.1.2/kaflow/asyncapi/docs.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.1/kaflow/asyncapi/models.py` & `kaflow-0.1.2/kaflow/asyncapi/models.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.1/tests/key_value_pb2.py` & `kaflow-0.1.2/tests/key_value_pb2.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.1/tests/test_serializers.py` & `kaflow-0.1.2/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.1/tests/_utils/test_inspect.py` & `kaflow-0.1.2/tests/_utils/test_inspect.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.1/.gitignore` & `kaflow-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.1/LICENSE` & `kaflow-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.1/README.md` & `kaflow-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.1/pyproject.toml` & `kaflow-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 keywords = ["kafka", "stream", "processing", "data", "pipeline", "flow"]
 authors = [
   { name = "Gabriel Martin Blazquez", email = "gmartinbdev@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
```

### Comparing `kaflow-0.1.1/PKG-INFO` & `kaflow-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: kaflow
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Stream processing backed by Apache Kafka.
 Project-URL: Documentation, https://github.com/gabrielmbmb/kaflow#readme
 Project-URL: Issues, https://github.com/gabrielmbmb/kaflow/issues
 Project-URL: Source, https://github.com/gabrielmbmb/kaflow
 Author-email: Gabriel Martin Blazquez <gmartinbdev@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: data,flow,kafka,pipeline,processing,stream
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
```

