# Comparing `tmp/communica-0.1.4.tar.gz` & `tmp/communica-0.1.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "communica-0.1.4.tar", last modified: Mon Apr 10 08:11:55 2023, max compression
+gzip compressed data, was "communica-0.1.4.post1.tar", last modified: Mon Apr 10 08:34:40 2023, max compression
```

## Comparing `communica-0.1.4.tar` & `communica-0.1.4.post1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 08:11:55.834890 communica-0.1.4/
--rw-rw-rw-   0        0        0      568 2023-03-25 20:48:52.000000 communica-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0     2184 2023-04-10 08:11:55.833891 communica-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1456 2023-04-04 20:46:58.000000 communica-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 08:11:55.817381 communica-0.1.4/communica/
--rw-rw-rw-   0        0        0      101 2023-02-15 13:48:00.000000 communica-0.1.4/communica/__init__.py
--rw-rw-rw-   0        0        0      130 2023-03-19 21:29:46.000000 communica-0.1.4/communica/clients.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:11:55.824897 communica-0.1.4/communica/connectors/
--rw-rw-rw-   0        0        0      170 2023-03-31 19:34:58.000000 communica-0.1.4/communica/connectors/__init__.py
--rw-rw-rw-   0        0        0     2803 2023-03-24 12:30:50.000000 communica-0.1.4/communica/connectors/_stream_local.py
--rw-rw-rw-   0        0        0     5358 2023-03-30 10:48:08.000000 communica-0.1.4/communica/connectors/base.py
--rw-rw-rw-   0        0        0    22199 2023-04-10 08:11:15.000000 communica-0.1.4/communica/connectors/rabbitmq.py
--rw-rw-rw-   0        0        0     9243 2023-03-30 11:38:51.000000 communica-0.1.4/communica/connectors/stream.py
--rw-rw-rw-   0        0        0      468 2023-03-19 11:58:01.000000 communica-0.1.4/communica/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:11:55.827892 communica-0.1.4/communica/pairs/
--rw-rw-rw-   0        0        0      223 2023-03-19 15:01:07.000000 communica-0.1.4/communica/pairs/__init__.py
--rw-rw-rw-   0        0        0     2667 2023-03-21 21:55:22.000000 communica-0.1.4/communica/pairs/base.py
--rw-rw-rw-   0        0        0    10308 2023-04-08 12:28:56.000000 communica-0.1.4/communica/pairs/route.py
--rw-rw-rw-   0        0        0    15514 2023-04-10 08:02:57.000000 communica-0.1.4/communica/pairs/simple.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:11:55.831891 communica-0.1.4/communica/serializers/
--rw-rw-rw-   0        0        0      176 2023-03-19 20:57:46.000000 communica-0.1.4/communica/serializers/__init__.py
--rw-rw-rw-   0        0        0      657 2023-03-18 18:41:17.000000 communica-0.1.4/communica/serializers/base.py
--rw-rw-rw-   0        0        0      315 2023-03-18 19:40:10.000000 communica-0.1.4/communica/serializers/json.py
--rw-rw-rw-   0        0        0      128 2023-03-19 21:29:36.000000 communica-0.1.4/communica/servers.py
--rw-rw-rw-   0        0        0     3077 2023-04-04 16:50:40.000000 communica-0.1.4/communica/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:11:55.821380 communica-0.1.4/communica.egg-info/
--rw-rw-rw-   0        0        0     2184 2023-04-10 08:11:55.000000 communica-0.1.4/communica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      716 2023-04-10 08:11:55.000000 communica-0.1.4/communica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 08:11:55.000000 communica-0.1.4/communica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-04-10 08:11:55.000000 communica-0.1.4/communica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-10 08:11:55.000000 communica-0.1.4/communica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1050 2023-04-10 08:11:31.000000 communica-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-10 08:11:55.834890 communica-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-10 08:11:55.833891 communica-0.1.4/tests/
--rw-rw-rw-   0        0        0     1040 2023-04-01 18:26:37.000000 communica-0.1.4/tests/test_connectors.py
--rw-rw-rw-   0        0        0     2940 2023-04-08 16:43:45.000000 communica-0.1.4/tests/test_entities.py
+drwxrwxrwx   0        0        0        0 2023-04-10 08:34:40.256314 communica-0.1.4.post1/
+-rw-rw-rw-   0        0        0      568 2023-03-25 20:48:52.000000 communica-0.1.4.post1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2190 2023-04-10 08:34:40.256314 communica-0.1.4.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2023-04-04 20:46:58.000000 communica-0.1.4.post1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 08:34:40.238315 communica-0.1.4.post1/communica/
+-rw-rw-rw-   0        0        0      101 2023-02-15 13:48:00.000000 communica-0.1.4.post1/communica/__init__.py
+-rw-rw-rw-   0        0        0      130 2023-03-19 21:29:46.000000 communica-0.1.4.post1/communica/clients.py
+drwxrwxrwx   0        0        0        0 2023-04-10 08:34:40.248315 communica-0.1.4.post1/communica/connectors/
+-rw-rw-rw-   0        0        0      170 2023-03-31 19:34:58.000000 communica-0.1.4.post1/communica/connectors/__init__.py
+-rw-rw-rw-   0        0        0     2803 2023-03-24 12:30:50.000000 communica-0.1.4.post1/communica/connectors/_stream_local.py
+-rw-rw-rw-   0        0        0     5358 2023-03-30 10:48:08.000000 communica-0.1.4.post1/communica/connectors/base.py
+-rw-rw-rw-   0        0        0    22199 2023-04-10 08:11:15.000000 communica-0.1.4.post1/communica/connectors/rabbitmq.py
+-rw-rw-rw-   0        0        0     9243 2023-03-30 11:38:51.000000 communica-0.1.4.post1/communica/connectors/stream.py
+-rw-rw-rw-   0        0        0      468 2023-03-19 11:58:01.000000 communica-0.1.4.post1/communica/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-10 08:34:40.251314 communica-0.1.4.post1/communica/pairs/
+-rw-rw-rw-   0        0        0      223 2023-03-19 15:01:07.000000 communica-0.1.4.post1/communica/pairs/__init__.py
+-rw-rw-rw-   0        0        0     2667 2023-03-21 21:55:22.000000 communica-0.1.4.post1/communica/pairs/base.py
+-rw-rw-rw-   0        0        0    10308 2023-04-10 08:23:55.000000 communica-0.1.4.post1/communica/pairs/route.py
+-rw-rw-rw-   0        0        0    15514 2023-04-10 08:02:57.000000 communica-0.1.4.post1/communica/pairs/simple.py
+drwxrwxrwx   0        0        0        0 2023-04-10 08:34:40.253315 communica-0.1.4.post1/communica/serializers/
+-rw-rw-rw-   0        0        0      176 2023-03-19 20:57:46.000000 communica-0.1.4.post1/communica/serializers/__init__.py
+-rw-rw-rw-   0        0        0      657 2023-03-18 18:41:17.000000 communica-0.1.4.post1/communica/serializers/base.py
+-rw-rw-rw-   0        0        0      315 2023-03-18 19:40:10.000000 communica-0.1.4.post1/communica/serializers/json.py
+-rw-rw-rw-   0        0        0      128 2023-03-19 21:29:36.000000 communica-0.1.4.post1/communica/servers.py
+-rw-rw-rw-   0        0        0     3077 2023-04-04 16:50:40.000000 communica-0.1.4.post1/communica/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 08:34:40.243316 communica-0.1.4.post1/communica.egg-info/
+-rw-rw-rw-   0        0        0     2190 2023-04-10 08:34:40.000000 communica-0.1.4.post1/communica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      716 2023-04-10 08:34:40.000000 communica-0.1.4.post1/communica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 08:34:40.000000 communica-0.1.4.post1/communica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-04-10 08:34:40.000000 communica-0.1.4.post1/communica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-10 08:34:40.000000 communica-0.1.4.post1/communica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1056 2023-04-10 08:33:32.000000 communica-0.1.4.post1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-10 08:34:40.256314 communica-0.1.4.post1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-10 08:34:40.255314 communica-0.1.4.post1/tests/
+-rw-rw-rw-   0        0        0     1040 2023-04-01 18:26:37.000000 communica-0.1.4.post1/tests/test_connectors.py
+-rw-rw-rw-   0        0        0     2940 2023-04-08 16:43:45.000000 communica-0.1.4.post1/tests/test_entities.py
```

### Comparing `communica-0.1.4/LICENSE.txt` & `communica-0.1.4.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `communica-0.1.4/PKG-INFO` & `communica-0.1.4.post1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: communica
-Version: 0.1.4
+Version: 0.1.4.post1
 Summary: Easy to use IPC library
 Author-email: Elchin Sarkarov <elchin751@gmail.com>
 Project-URL: Homepage, https://github.com/elchinchel/communica-py
 Project-URL: Bug Tracker, https://github.com/elchinchel/communica-py/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `communica-0.1.4/README.md` & `communica-0.1.4.post1/README.md`

 * *Files identical despite different names*

### Comparing `communica-0.1.4/communica/connectors/_stream_local.py` & `communica-0.1.4.post1/communica/connectors/_stream_local.py`

 * *Files identical despite different names*

### Comparing `communica-0.1.4/communica/connectors/base.py` & `communica-0.1.4.post1/communica/connectors/base.py`

 * *Files identical despite different names*

### Comparing `communica-0.1.4/communica/connectors/rabbitmq.py` & `communica-0.1.4.post1/communica/connectors/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `communica-0.1.4/communica/connectors/stream.py` & `communica-0.1.4.post1/communica/connectors/stream.py`

 * *Files identical despite different names*

### Comparing `communica-0.1.4/communica/pairs/base.py` & `communica-0.1.4.post1/communica/pairs/base.py`

 * *Files identical despite different names*

### Comparing `communica-0.1.4/communica/pairs/route.py` & `communica-0.1.4.post1/communica/pairs/route.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -42,25 +42,25 @@
 
     _response_serializers: 'dict[str, BaseSerializer]'
 
     def __init__(self):
         super().__init__()
         self.routes = {}
         self.fallback_task_set = set()
+        self._response_serializers = {}
 
     def update_route(
             self,
             route: str,
             handler: 'SyncHandlerType | AsyncHandlerType',
             serializer: 'BaseSerializer | None'
     ):
         if serializer is None:
             serializer = default_serializer
         self.routes[route] = (RequestHandler(handler), serializer)
-        self._response_serializers = {}
 
     def dispatch(self, metadata: Metadata, raw_data: bytes):
         if metadata['type'] < RequestType.RESP_OK:
             try:
                 route_handle = self.routes[metadata['route']]
                 task_set = route_handle[0].running_tasks
             except KeyError:
```

### Comparing `communica-0.1.4/communica/pairs/simple.py` & `communica-0.1.4.post1/communica/pairs/simple.py`

 * *Files identical despite different names*

### Comparing `communica-0.1.4/communica/serializers/base.py` & `communica-0.1.4.post1/communica/serializers/base.py`

 * *Files identical despite different names*

### Comparing `communica-0.1.4/communica/utils.py` & `communica-0.1.4.post1/communica/utils.py`

 * *Files identical despite different names*

### Comparing `communica-0.1.4/communica.egg-info/PKG-INFO` & `communica-0.1.4.post1/communica.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: communica
-Version: 0.1.4
+Version: 0.1.4.post1
 Summary: Easy to use IPC library
 Author-email: Elchin Sarkarov <elchin751@gmail.com>
 Project-URL: Homepage, https://github.com/elchinchel/communica-py
 Project-URL: Bug Tracker, https://github.com/elchinchel/communica-py/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `communica-0.1.4/communica.egg-info/SOURCES.txt` & `communica-0.1.4.post1/communica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `communica-0.1.4/pyproject.toml` & `communica-0.1.4.post1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "communica"
-version = "0.1.4"
+version = "0.1.4.post1"
 authors = [
   { name="Elchin Sarkarov", email="elchin751@gmail.com" },
 ]
 description = "Easy to use IPC library"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `communica-0.1.4/tests/test_connectors.py` & `communica-0.1.4.post1/tests/test_connectors.py`

 * *Files identical despite different names*

### Comparing `communica-0.1.4/tests/test_entities.py` & `communica-0.1.4.post1/tests/test_entities.py`

 * *Files identical despite different names*

