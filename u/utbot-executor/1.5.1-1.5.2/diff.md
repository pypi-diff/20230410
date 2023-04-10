# Comparing `tmp/utbot_executor-1.5.1.tar.gz` & `tmp/utbot_executor-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utbot_executor-1.5.1.tar", max compression
+gzip compressed data, was "utbot_executor-1.5.2.tar", max compression
```

## Comparing `utbot_executor-1.5.1.tar` & `utbot_executor-1.5.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1076 2022-10-03 19:39:38.276000 utbot_executor-1.5.1/LICENSE
--rw-r--r--   0        0        0     1058 2023-02-27 11:20:59.630921 utbot_executor-1.5.1/README.md
--rw-r--r--   0        0        0      419 2023-04-10 14:12:03.413025 utbot_executor-1.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-17 06:22:44.305237 utbot_executor-1.5.1/utbot_executor/__init__.py
--rw-r--r--   0        0        0     1039 2023-03-27 09:02:56.888080 utbot_executor-1.5.1/utbot_executor/__main__.py
--rw-r--r--   0        0        0        0 2023-02-21 06:50:17.028607 utbot_executor-1.5.1/utbot_executor/deep_serialization/__init__.py
--rw-r--r--   0        0        0     2090 2023-03-30 13:06:09.660414 utbot_executor-1.5.1/utbot_executor/deep_serialization/deep_serialization.py
--rw-r--r--   0        0        0     1537 2023-04-10 14:00:00.445575 utbot_executor-1.5.1/utbot_executor/deep_serialization/example.py
--rw-r--r--   0        0        0     8799 2023-04-10 11:38:19.700259 utbot_executor-1.5.1/utbot_executor/deep_serialization/json_converter.py
--rw-r--r--   0        0        0     9807 2023-04-10 14:10:28.050704 utbot_executor-1.5.1/utbot_executor/deep_serialization/memory_objects.py
--rw-r--r--   0        0        0     4300 2023-04-10 14:10:46.157811 utbot_executor-1.5.1/utbot_executor/deep_serialization/test_json.json
--rw-r--r--   0        0        0     3871 2023-04-10 11:32:19.241414 utbot_executor-1.5.1/utbot_executor/deep_serialization/utils.py
--rw-r--r--   0        0        0     7975 2023-03-30 13:06:09.677079 utbot_executor-1.5.1/utbot_executor/executor.py
--rw-r--r--   0        0        0     3192 2023-03-02 10:22:46.865281 utbot_executor-1.5.1/utbot_executor/listener.py
--rw-r--r--   0        0        0      568 2023-03-30 11:31:56.729251 utbot_executor-1.5.1/utbot_executor/memory_compressor.py
--rw-r--r--   0        0        0     2578 2023-03-30 11:31:56.739251 utbot_executor-1.5.1/utbot_executor/parser.py
--rw-r--r--   0        0        0      288 2023-03-23 15:10:03.405564 utbot_executor-1.5.1/utbot_executor/utils.py
--rw-r--r--   0        0        0     1892 1970-01-01 00:00:00.000000 utbot_executor-1.5.1/setup.py
--rw-r--r--   0        0        0     1555 1970-01-01 00:00:00.000000 utbot_executor-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2022-10-03 19:39:38.276000 utbot_executor-1.5.2/LICENSE
+-rw-r--r--   0        0        0     1058 2023-02-27 11:20:59.630921 utbot_executor-1.5.2/README.md
+-rw-r--r--   0        0        0      419 2023-04-10 14:29:44.896576 utbot_executor-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-17 06:22:44.305237 utbot_executor-1.5.2/utbot_executor/__init__.py
+-rw-r--r--   0        0        0     1039 2023-03-27 09:02:56.888080 utbot_executor-1.5.2/utbot_executor/__main__.py
+-rw-r--r--   0        0        0        0 2023-02-21 06:50:17.028607 utbot_executor-1.5.2/utbot_executor/deep_serialization/__init__.py
+-rw-r--r--   0        0        0     2090 2023-03-30 13:06:09.660414 utbot_executor-1.5.2/utbot_executor/deep_serialization/deep_serialization.py
+-rw-r--r--   0        0        0     1528 2023-04-10 14:27:35.374234 utbot_executor-1.5.2/utbot_executor/deep_serialization/example.py
+-rw-r--r--   0        0        0     8799 2023-04-10 11:38:19.700259 utbot_executor-1.5.2/utbot_executor/deep_serialization/json_converter.py
+-rw-r--r--   0        0        0     9940 2023-04-10 14:28:14.324894 utbot_executor-1.5.2/utbot_executor/deep_serialization/memory_objects.py
+-rw-r--r--   0        0        0     5445 2023-04-10 14:28:17.024941 utbot_executor-1.5.2/utbot_executor/deep_serialization/test_json.json
+-rw-r--r--   0        0        0     3871 2023-04-10 11:32:19.241414 utbot_executor-1.5.2/utbot_executor/deep_serialization/utils.py
+-rw-r--r--   0        0        0     7975 2023-03-30 13:06:09.677079 utbot_executor-1.5.2/utbot_executor/executor.py
+-rw-r--r--   0        0        0     3192 2023-03-02 10:22:46.865281 utbot_executor-1.5.2/utbot_executor/listener.py
+-rw-r--r--   0        0        0      568 2023-03-30 11:31:56.729251 utbot_executor-1.5.2/utbot_executor/memory_compressor.py
+-rw-r--r--   0        0        0     2578 2023-03-30 11:31:56.739251 utbot_executor-1.5.2/utbot_executor/parser.py
+-rw-r--r--   0        0        0      288 2023-03-23 15:10:03.405564 utbot_executor-1.5.2/utbot_executor/utils.py
+-rw-r--r--   0        0        0     1892 1970-01-01 00:00:00.000000 utbot_executor-1.5.2/setup.py
+-rw-r--r--   0        0        0     1555 1970-01-01 00:00:00.000000 utbot_executor-1.5.2/PKG-INFO
```

### Comparing `utbot_executor-1.5.1/LICENSE` & `utbot_executor-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.1/README.md` & `utbot_executor-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.1/utbot_executor/__main__.py` & `utbot_executor-1.5.2/utbot_executor/__main__.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.1/utbot_executor/deep_serialization/deep_serialization.py` & `utbot_executor-1.5.2/utbot_executor/deep_serialization/deep_serialization.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.1/utbot_executor/deep_serialization/example.py` & `utbot_executor-1.5.2/utbot_executor/deep_serialization/example.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     # a = [1, 2, float('inf'), "abc", {1: 1}, None, b, c]
     # x = Node("x")
     # y = Node("y")
     # x.children.append(y)
     # y.children.append(x)
     x = numpy.array([101])
     serializer_ = PythonSerializer()
-    pprint(serializer_.write_object_to_memory(x.dot(x.T)))
+    pprint(serializer_.write_object_to_memory(x))
     pprint(serializer_.memory.objects)
     with open('test_json.json', 'w') as fout:
         print(json.dumps({'objects': serializer_.memory}, cls=MemoryDumpEncoder, indent=True), file=fout)
 
 
 def deserialize():
     # run()
```

### Comparing `utbot_executor-1.5.1/utbot_executor/deep_serialization/json_converter.py` & `utbot_executor-1.5.2/utbot_executor/deep_serialization/json_converter.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.1/utbot_executor/deep_serialization/memory_objects.py` & `utbot_executor-1.5.2/utbot_executor/deep_serialization/memory_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,15 +200,18 @@
         dictitems = serializer[self.dictitems]
         if isinstance(dictitems, Dict):
             for key, value in dictitems.items():
                 deserialized_obj[key] = value
 
         comparable = self.obj == deserialized_obj
         if hasattr(type(comparable), '__module__') and type(comparable).__module__ == 'numpy':
-            comparable = comparable.__bool__()
+            if type(comparable).__qualname__ == 'ndarray':
+                comparable = bool(comparable.all())
+            else:
+                comparable = comparable.__bool__()
 
         super()._initialize(deserialized_obj, comparable)
 
 
 class MemoryObjectProvider(object):
     @staticmethod
     def get_serializer(obj: object) -> Optional[Type[MemoryObject]]:
```

### Comparing `utbot_executor-1.5.1/utbot_executor/deep_serialization/utils.py` & `utbot_executor-1.5.2/utbot_executor/deep_serialization/utils.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.1/utbot_executor/executor.py` & `utbot_executor-1.5.2/utbot_executor/executor.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.1/utbot_executor/listener.py` & `utbot_executor-1.5.2/utbot_executor/listener.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.1/utbot_executor/memory_compressor.py` & `utbot_executor-1.5.2/utbot_executor/memory_compressor.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.1/utbot_executor/parser.py` & `utbot_executor-1.5.2/utbot_executor/parser.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.1/setup.py` & `utbot_executor-1.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['numpy>=1.24.2,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['utbot-executor = utbot_executor:utbot_executor']}
 
 setup_kwargs = {
     'name': 'utbot-executor',
-    'version': '1.5.1',
+    'version': '1.5.2',
     'description': '',
     'long_description': '# UtBot Executor\n\nUtil for python code execution and state serialization.\n\n## Installation\n\nYou can install module from [PyPI](https://pypi.org/project/utbot-executor/):\n\n```bash\npython -m pip install utbot-executor\n```\n\n## Usage\n\n### From console with socket listener\n\nRun with your `<hostname>` and `<port>` for socket connection\n```bash\n$ python -m utbot_executor <hostname> <port> <logfile> [<loglevel DEBUG | INFO | ERROR>]\n```\n\n### Result format:\n\n```json\n{\n        "status": "success",\n        "isException": bool,\n        "statements": list[int],\n        "missedStatements": list[int],\n        "stateBefore": memory json dump,\n        "stateAfter": memory json dump,\n        "argsIds": list[str],\n        "kwargs": list[str],\n        "resultId": str,\n}\n```\n\nor error format:\n\n```json\n{\n        "status": "fail",\n        "exception": str (traceback),\n}\n```\n\n#### States format\n\nTODO\n\n### Submodule `deep_serialization`\n\nJSON serializer and deserializer for python objects\n\n## Source\n\nGitHub [repository](https://github.com/tamarinvs19/utbot_executor)\n',
     'author': 'Vyacheslav Tamarin',
     'author_email': 'vyacheslav.tamarin@yandex.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `utbot_executor-1.5.1/PKG-INFO` & `utbot_executor-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utbot-executor
-Version: 1.5.1
+Version: 1.5.2
 Summary: 
 Author: Vyacheslav Tamarin
 Author-email: vyacheslav.tamarin@yandex.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

