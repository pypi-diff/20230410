# Comparing `tmp/snapstream-0.0.0.dev2.tar.gz` & `tmp/snapstream-0.0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapstream-0.0.0.dev2.tar", max compression
+gzip compressed data, was "snapstream-0.0.0.dev3.tar", max compression
```

## Comparing `snapstream-0.0.0.dev2.tar` & `snapstream-0.0.0.dev3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-04-02 12:40:11.261286 snapstream-0.0.0.dev2/LICENSE
--rw-r--r--   0        0        0     1178 2023-04-02 12:40:11.261286 snapstream-0.0.0.dev2/README.md
--rw-r--r--   0        0        0     1067 2023-04-02 12:40:30.085418 snapstream-0.0.0.dev2/pyproject.toml
--rw-r--r--   0        0        0     1703 2023-04-02 12:40:11.261286 snapstream-0.0.0.dev2/snapstream/__init__.py
--rw-r--r--   0        0        0     3699 2023-04-02 12:40:11.261286 snapstream-0.0.0.dev2/snapstream/caching.py
--rw-r--r--   0        0        0      663 2023-04-02 12:40:11.261286 snapstream-0.0.0.dev2/snapstream/codecs.py
--rw-r--r--   0        0        0     5719 2023-04-02 12:40:11.261286 snapstream-0.0.0.dev2/snapstream/core.py
--rw-r--r--   0        0        0     1182 2023-04-02 12:40:11.261286 snapstream-0.0.0.dev2/snapstream/utils.py
--rw-r--r--   0        0        0     2009 1970-01-01 00:00:00.000000 snapstream-0.0.0.dev2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-02 14:10:00.628028 snapstream-0.0.0.dev3/LICENSE
+-rw-r--r--   0        0        0     1735 2023-04-02 14:10:00.628028 snapstream-0.0.0.dev3/README.md
+-rw-r--r--   0        0        0     1067 2023-04-02 14:10:12.160111 snapstream-0.0.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0     1703 2023-04-02 14:10:00.628028 snapstream-0.0.0.dev3/snapstream/__init__.py
+-rw-r--r--   0        0        0     3699 2023-04-02 14:10:00.628028 snapstream-0.0.0.dev3/snapstream/caching.py
+-rw-r--r--   0        0        0      663 2023-04-02 14:10:00.628028 snapstream-0.0.0.dev3/snapstream/codecs.py
+-rw-r--r--   0        0        0     5719 2023-04-02 14:10:00.628028 snapstream-0.0.0.dev3/snapstream/core.py
+-rw-r--r--   0        0        0     1182 2023-04-02 14:10:00.628028 snapstream-0.0.0.dev3/snapstream/utils.py
+-rw-r--r--   0        0        0     2566 1970-01-01 00:00:00.000000 snapstream-0.0.0.dev3/PKG-INFO
```

### Comparing `snapstream-0.0.0.dev2/LICENSE` & `snapstream-0.0.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.0.dev2/pyproject.toml` & `snapstream-0.0.0.dev3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snapstream"
-version = "0.0.0.dev2"
+version = "0.0.0.dev3"
 description = "Streamline your Kafka data processing, this tool aims to standardize streaming data from multiple Kafka clusters. With a pub-sub approach, multiple functions can easily subscribe to incoming messages, serialization can be specified per topic, and data is automatically processed by data sink functions."
 authors = ["Menziess <stefan_schenk@hotmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/Menziess/snapstream"
 
 
 [tool.poetry.dependencies]
```

### Comparing `snapstream-0.0.0.dev2/snapstream/__init__.py` & `snapstream-0.0.0.dev3/snapstream/__init__.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.0.dev2/snapstream/caching.py` & `snapstream-0.0.0.dev3/snapstream/caching.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.0.dev2/snapstream/codecs.py` & `snapstream-0.0.0.dev3/snapstream/codecs.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.0.dev2/snapstream/core.py` & `snapstream-0.0.0.dev3/snapstream/core.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.0.dev2/snapstream/utils.py` & `snapstream-0.0.0.dev3/snapstream/utils.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.0.dev2/PKG-INFO` & `snapstream-0.0.0.dev3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapstream
-Version: 0.0.0.dev2
+Version: 0.0.0.dev3
 Summary: Streamline your Kafka data processing, this tool aims to standardize streaming data from multiple Kafka clusters. With a pub-sub approach, multiple functions can easily subscribe to incoming messages, serialization can be specified per topic, and data is automatically processed by data sink functions.
 Home-page: https://github.com/Menziess/snapstream
 Author: Menziess
 Author-email: stefan_schenk@hotmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -12,49 +12,53 @@
 Requires-Dist: confluent-kafka (>=2.0.2,<3.0.0)
 Requires-Dist: pypubsub (>=4.0.3,<5.0.0)
 Requires-Dist: rocksdict (>=0.3.10,<0.4.0)
 Description-Content-Type: text/markdown
 
 # Snapstream
 
-<img src="res/logo.png" width="25%" height="25%" align="right" />
+<img src="https://github.com/Menziess/snapstream/blob/feature/github-actions/res/logo.png?raw=true" width="25%" height="25%" align="right" />
 
-An easy to use, extensible data-flow model, providing sensible defaults to produce and consume to and from kafka, serialize/deserialize messages, and cache large amounts of data.
+A tiny data-flow model with a user-friendly interface that provides sensible defaults for Kafka integration, message serialization/deserialization, and data caching.
+
+In response to a challenge of performing a "merge-as-of", "nearby join", or "merge by key distance" operation on multiple kafka streams while reading topics from separate kafka clusters, this package was born.
+
+No actual stream or external database is required, cached data is persisted to disk using rocksdb, applications using snapstream are more inclined to be; self-contained, easy to extend, less complex, easy to test using regular iterables:
 
 ## Installation
 
 ```sh
 pip install snapstream
 ```
 
 ## Usage
 
 In the example below, `snap` decorates the `handle` function, binding the iterable `range(5)` to it:
 
 ```py
 from snapstream import snap, stream
 
+r = range(5)
 
-@snap(range(5))
-def handle(msg):
-    print('Greetings', msg)
+@snap(r, sink=[print])
+    def handler(msg):
+        return f'Hello {msg}'
 
 stream()
 ```
 
 ```sh
-➜ python main.py
-Greetings 0
-Greetings 1
-Greetings 2
-Greetings 3
-Greetings 4
+Hello 0
+Hello 1
+Hello 2
+Hello 3
+Hello 4
 ```
 
 ## Features
 
-- `snapstream.Topic`: consume from topic (iterable), produce to topic (callable), uses [**confluent-kafka**](https://docs.confluent.io/platform/current/clients/confluent-kafka-python/html/index.html) by default
-- `snapstream.Cache`: persist data, uses [**rocksdict**](https://congyuwang.github.io/RocksDict/rocksdict.html)
-- `snapstream.Conf`: configuration singleton class, manages threads for all streams
-- `snapstream.stream`: start streams
-- `snapstream.snap`: bind streams (iterable) and sinks (callable) to handler functions
+- `snapstream.Topic`: an iterable/callable to consume and produce (default: [**confluent-kafka**](https://docs.confluent.io/platform/current/clients/confluent-kafka-python/html/index.html))
+- `snapstream.Cache`: a callable/dict to persist data (default: [**rocksdict**](https://congyuwang.github.io/RocksDict/rocksdict.html))
+- `snapstream.Conf`: a singleton object, can be used to store common kafka configurations
+- `snapstream.snap`: a function to bind streams (iterables) and sinks (callables) to user defined handler functions
+- `snapstream.stream`: a function to start the streams
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

