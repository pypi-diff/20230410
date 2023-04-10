# Comparing `tmp/kaflow-0.1.0.tar.gz` & `tmp/kaflow-0.1.1.tar.gz`

## Comparing `kaflow-0.1.0.tar` & `kaflow-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 kaflow-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 kaflow-0.1.0/Makefile
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 kaflow-0.1.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 kaflow-0.1.0/.github/workflows/test.yaml
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/__init__.py
--rw-r--r--   0        0        0     8100 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/_consumer.py
--rw-r--r--   0        0        0    21977 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/applications.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/dependencies.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/exceptions.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/logger.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/message.py
--rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/py.typed
--rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/serializers.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/_utils/__init__.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/_utils/asyncio.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/_utils/inspect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/asyncapi/__init__.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/asyncapi/_builder.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/asyncapi/docs.py
--rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 kaflow-0.1.0/kaflow/asyncapi/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 kaflow-0.1.0/tests/key_value.proto
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 kaflow-0.1.0/tests/key_value_pb2.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 kaflow-0.1.0/tests/key_value_pb2.pyi
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 kaflow-0.1.0/tests/test_application.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 kaflow-0.1.0/tests/test_serializers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.0/tests/_utils/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 kaflow-0.1.0/tests/_utils/test_asyncio.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 kaflow-0.1.0/tests/_utils/test_inspect.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 kaflow-0.1.0/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 kaflow-0.1.0/LICENSE
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 kaflow-0.1.0/README.md
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 kaflow-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 kaflow-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 kaflow-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 kaflow-0.1.1/Makefile
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 kaflow-0.1.1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 kaflow-0.1.1/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/__init__.py
+-rw-r--r--   0        0        0     8100 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/_consumer.py
+-rw-r--r--   0        0        0    21919 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/applications.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/dependencies.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/exceptions.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/logger.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/message.py
+-rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/py.typed
+-rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/serializers.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/_utils/__init__.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/_utils/asyncio.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/_utils/inspect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/asyncapi/__init__.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/asyncapi/_builder.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/asyncapi/docs.py
+-rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 kaflow-0.1.1/kaflow/asyncapi/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 kaflow-0.1.1/tests/key_value.proto
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 kaflow-0.1.1/tests/key_value_pb2.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 kaflow-0.1.1/tests/key_value_pb2.pyi
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 kaflow-0.1.1/tests/test_application.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 kaflow-0.1.1/tests/test_serializers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.1/tests/_utils/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 kaflow-0.1.1/tests/_utils/test_asyncio.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 kaflow-0.1.1/tests/_utils/test_inspect.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 kaflow-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 kaflow-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 kaflow-0.1.1/README.md
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 kaflow-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 kaflow-0.1.1/PKG-INFO
```

### Comparing `kaflow-0.1.0/.github/workflows/release.yaml` & `kaflow-0.1.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.0/.github/workflows/test.yaml` & `kaflow-0.1.1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.0/kaflow/__init__.py` & `kaflow-0.1.1/kaflow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,8 +31,8 @@
     __all__.append("Avro")
 
 if has_protobuf:
     from kaflow.serializers import Protobuf  # noqa: F401
 
     __all__.append("Protobuf")
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

### Comparing `kaflow-0.1.0/kaflow/_consumer.py` & `kaflow-0.1.1/kaflow/_consumer.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.0/kaflow/applications.py` & `kaflow-0.1.1/kaflow/applications.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,14 @@
             sink_topics=sink_topics,
         )
         self._consumers[topic] = topic_processor
 
     def _create_consumer(self) -> AIOKafkaConsumer:
         return AIOKafkaConsumer(
             *self._consumers.keys(),
-            loop=self._loop,
             bootstrap_servers=self.brokers,
             client_id=self.client_id,
             group_id=self.group_id,
             fetch_min_bytes=self.fetch_min_bytes,
             fetch_max_bytes=self.fetch_max_bytes,
             fetch_max_wait_ms=self.fetch_max_wait_ms,
             max_partition_fetch_bytes=self.max_partition_fetch_bytes,
@@ -310,15 +309,14 @@
             sasl_kerberos_domain_name=self.sasl_kerberos_domain_name,
             sasl_kerberos_service_name=self.sasl_kerberos_service_name,
             sasl_oauth_token_provider=self.sasl_oauth_token_provider,
         )
 
     def _create_producer(self) -> AIOKafkaProducer:
         return AIOKafkaProducer(
-            loop=self._loop,
             bootstrap_servers=self.brokers,
             client_id=self.client_id,
             metadata_max_age_ms=self.metadata_max_age_ms,
             request_timeout_ms=self.request_timeout_ms,
             api_version=self.kafka_api_version,
             acks=self.acks,
             compression_type=self.compression_type,
```

### Comparing `kaflow-0.1.0/kaflow/message.py` & `kaflow-0.1.1/kaflow/message.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.0/kaflow/parameters.py` & `kaflow-0.1.1/kaflow/parameters.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.0/kaflow/serializers.py` & `kaflow-0.1.1/kaflow/serializers.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.0/kaflow/_utils/asyncio.py` & `kaflow-0.1.1/kaflow/_utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.0/kaflow/_utils/inspect.py` & `kaflow-0.1.1/kaflow/_utils/inspect.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.0/kaflow/asyncapi/_builder.py` & `kaflow-0.1.1/kaflow/asyncapi/_builder.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.0/kaflow/asyncapi/docs.py` & `kaflow-0.1.1/kaflow/asyncapi/docs.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.0/kaflow/asyncapi/models.py` & `kaflow-0.1.1/kaflow/asyncapi/models.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.0/tests/key_value_pb2.py` & `kaflow-0.1.1/tests/key_value_pb2.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.0/tests/test_serializers.py` & `kaflow-0.1.1/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.0/tests/_utils/test_inspect.py` & `kaflow-0.1.1/tests/_utils/test_inspect.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.0/.gitignore` & `kaflow-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.0/LICENSE` & `kaflow-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.0/README.md` & `kaflow-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.0/pyproject.toml` & `kaflow-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.0/PKG-INFO` & `kaflow-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaflow
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Stream processing backed by Apache Kafka.
 Project-URL: Documentation, https://github.com/gabrielmbmb/kaflow#readme
 Project-URL: Issues, https://github.com/gabrielmbmb/kaflow/issues
 Project-URL: Source, https://github.com/gabrielmbmb/kaflow
 Author-email: Gabriel Martin Blazquez <gmartinbdev@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

