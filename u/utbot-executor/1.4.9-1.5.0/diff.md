# Comparing `tmp/utbot_executor-1.4.9.tar.gz` & `tmp/utbot_executor-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utbot_executor-1.4.9.tar", max compression
+gzip compressed data, was "utbot_executor-1.5.0.tar", max compression
```

## Comparing `utbot_executor-1.4.9.tar` & `utbot_executor-1.5.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1076 2022-10-03 19:39:38.276000 utbot_executor-1.4.9/LICENSE
--rw-r--r--   0        0        0     1058 2023-02-27 11:20:59.630921 utbot_executor-1.4.9/README.md
--rw-r--r--   0        0        0      451 2023-03-29 13:33:46.633533 utbot_executor-1.4.9/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-17 06:22:44.305237 utbot_executor-1.4.9/utbot_executor/__init__.py
--rw-r--r--   0        0        0     1039 2023-03-27 09:02:56.888080 utbot_executor-1.4.9/utbot_executor/__main__.py
--rw-r--r--   0        0        0        0 2023-02-21 06:50:17.028607 utbot_executor-1.4.9/utbot_executor/deep_serialization/__init__.py
--rw-r--r--   0        0        0     1607 2023-03-29 06:28:35.883102 utbot_executor-1.4.9/utbot_executor/deep_serialization/deep_serialization.py
--rw-r--r--   0        0        0     1469 2023-03-27 12:33:21.420322 utbot_executor-1.4.9/utbot_executor/deep_serialization/example.py
--rw-r--r--   0        0        0     8932 2023-03-29 13:33:04.920744 utbot_executor-1.4.9/utbot_executor/deep_serialization/json_converter.py
--rw-r--r--   0        0        0     9039 2023-03-27 12:12:38.796607 utbot_executor-1.4.9/utbot_executor/deep_serialization/memory_objects.py
--rw-r--r--   0        0        0     3866 2023-03-27 12:33:44.948384 utbot_executor-1.4.9/utbot_executor/deep_serialization/test_json.json
--rw-r--r--   0        0        0     3705 2023-03-27 11:08:26.478081 utbot_executor-1.4.9/utbot_executor/deep_serialization/utils.py
--rw-r--r--   0        0        0     6785 2023-03-29 13:33:34.972753 utbot_executor-1.4.9/utbot_executor/executor.py
--rw-r--r--   0        0        0     3192 2023-03-02 10:22:46.865281 utbot_executor-1.4.9/utbot_executor/listener.py
--rw-r--r--   0        0        0     2452 2023-03-29 07:11:21.770939 utbot_executor-1.4.9/utbot_executor/parser.py
--rw-r--r--   0        0        0      288 2023-03-23 15:10:03.405564 utbot_executor-1.4.9/utbot_executor/utils.py
--rw-r--r--   0        0        0     1803 1970-01-01 00:00:00.000000 utbot_executor-1.4.9/setup.py
--rw-r--r--   0        0        0     1566 1970-01-01 00:00:00.000000 utbot_executor-1.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1076 2022-10-03 19:39:38.276000 utbot_executor-1.5.0/LICENSE
+-rw-r--r--   0        0        0     1058 2023-02-27 11:20:59.630921 utbot_executor-1.5.0/README.md
+-rw-r--r--   0        0        0      401 2023-04-10 11:40:47.733758 utbot_executor-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-17 06:22:44.305237 utbot_executor-1.5.0/utbot_executor/__init__.py
+-rw-r--r--   0        0        0     1039 2023-03-27 09:02:56.888080 utbot_executor-1.5.0/utbot_executor/__main__.py
+-rw-r--r--   0        0        0        0 2023-02-21 06:50:17.028607 utbot_executor-1.5.0/utbot_executor/deep_serialization/__init__.py
+-rw-r--r--   0        0        0     2090 2023-03-30 13:06:09.660414 utbot_executor-1.5.0/utbot_executor/deep_serialization/deep_serialization.py
+-rw-r--r--   0        0        0     1469 2023-04-10 11:40:28.069963 utbot_executor-1.5.0/utbot_executor/deep_serialization/example.py
+-rw-r--r--   0        0        0     8799 2023-04-10 11:38:19.700259 utbot_executor-1.5.0/utbot_executor/deep_serialization/json_converter.py
+-rw-r--r--   0        0        0     9805 2023-04-10 11:38:19.706926 utbot_executor-1.5.0/utbot_executor/deep_serialization/memory_objects.py
+-rw-r--r--   0        0        0     5777 2023-04-10 11:34:06.200767 utbot_executor-1.5.0/utbot_executor/deep_serialization/test_json.json
+-rw-r--r--   0        0        0     3871 2023-04-10 11:32:19.241414 utbot_executor-1.5.0/utbot_executor/deep_serialization/utils.py
+-rw-r--r--   0        0        0     7975 2023-03-30 13:06:09.677079 utbot_executor-1.5.0/utbot_executor/executor.py
+-rw-r--r--   0        0        0     3192 2023-03-02 10:22:46.865281 utbot_executor-1.5.0/utbot_executor/listener.py
+-rw-r--r--   0        0        0      568 2023-03-30 11:31:56.729251 utbot_executor-1.5.0/utbot_executor/memory_compressor.py
+-rw-r--r--   0        0        0     2578 2023-03-30 11:31:56.739251 utbot_executor-1.5.0/utbot_executor/parser.py
+-rw-r--r--   0        0        0      288 2023-03-23 15:10:03.405564 utbot_executor-1.5.0/utbot_executor/utils.py
+-rw-r--r--   0        0        0     1803 1970-01-01 00:00:00.000000 utbot_executor-1.5.0/setup.py
+-rw-r--r--   0        0        0     1516 1970-01-01 00:00:00.000000 utbot_executor-1.5.0/PKG-INFO
```

### Comparing `utbot_executor-1.4.9/LICENSE` & `utbot_executor-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.4.9/README.md` & `utbot_executor-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.4.9/utbot_executor/__main__.py` & `utbot_executor-1.5.0/utbot_executor/__main__.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.4.9/utbot_executor/deep_serialization/deep_serialization.py` & `utbot_executor-1.5.0/utbot_executor/deep_serialization/deep_serialization.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,30 @@
     ids = [
         serializer.write_object_to_memory(obj)
         for obj in objs
     ]
     return ids, serialize_memory_dump(serializer.memory)
 
 
+def serialize_objects_dump(objs: List[Any], clear_visited: bool = False) -> Tuple[List[PythonId], MemoryDump, str]:
+    """
+    Serialize objects with shared memory.
+    Returns list of object ids and memory dump.
+    """
+
+    serializer = PythonSerializer()
+    if clear_visited:
+        serializer.clear_visited()
+    ids = [
+        serializer.write_object_to_memory(obj)
+        for obj in objs
+    ]
+    return ids, serializer.memory, serialize_memory_dump(serializer.memory)
+
+
 def deserialize_objects(ids: List[str], memory: str, imports: List[str]) -> Dict[str, object]:
     """
     Deserialize objects from shared memory.
     Returns dictionary where keys are ID and values are deserialized objects.
     """
 
     memory_dump = deserialize_memory_objects(memory)
```

### Comparing `utbot_executor-1.4.9/utbot_executor/deep_serialization/example.py` & `utbot_executor-1.5.0/utbot_executor/deep_serialization/example.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.4.9/utbot_executor/deep_serialization/json_converter.py` & `utbot_executor-1.5.0/utbot_executor/deep_serialization/json_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,23 +129,14 @@
                 new_memory_object.args = self.dump_id_to_real_id[new_memory_object.args]
                 new_memory_object.state = self.dump_id_to_real_id[new_memory_object.state]
                 new_memory_object.listitems = self.dump_id_to_real_id[new_memory_object.listitems]
                 new_memory_object.dictitems = self.dump_id_to_real_id[new_memory_object.dictitems]
             new_memory_objects[self.dump_id_to_real_id[id_]] = new_memory_object
         return MemoryDump(new_memory_objects)
 
-    def update_states(self, memory_dump: MemoryDump) -> MemoryDump:
-        for id_, obj in memory_dump.objects.items():
-            if isinstance(obj, ReduceMemoryObject):
-                memory_object = self.memory[id_]
-                if isinstance(memory_object, ReduceMemoryObject):
-                    obj.state = memory_object.state
-                    obj.listitems = memory_object.listitems
-                    obj.dictitems = memory_object.dictitems
-
     @staticmethod
     def add_syspaths(syspaths: Iterable[str]):
         for path in syspaths:
             if path not in sys.path:
                 sys.path.insert(0, path)
 
     @staticmethod
@@ -160,17 +151,17 @@
             return self.memory[self.dump_id_to_real_id[python_id]]
 
         dump_object = self.memory_dump.objects[python_id]
         real_object: object
         if isinstance(dump_object, ReprMemoryObject):
             real_object = eval(dump_object.value)
         elif isinstance(dump_object, ListMemoryObject):
-            if dump_object.qualname == 'builtins.set':
+            if dump_object.typeinfo.fullname == 'builtins.set':
                 real_object = set(self.load_object(item) for item in dump_object.items)
-            elif dump_object.qualname == 'builtins.tuple':
+            elif dump_object.typeinfo.fullname == 'builtins.tuple':
                 real_object = tuple(self.load_object(item) for item in dump_object.items)
             else:
                 real_object = [self.load_object(item) for item in dump_object.items]
         elif isinstance(dump_object, DictMemoryObject):
             real_object = {
                     self.load_object(key): self.load_object(value)
                     for key, value in dump_object.items.items()
@@ -181,22 +172,30 @@
             real_object = constructor(*args)
 
             id_ = PythonId(str(id(real_object)))
             self.dump_id_to_real_id[python_id] = id_
             self.memory[id_] = real_object
 
             state = self.load_object(dump_object.state)
-            for field, value in state.items():
-                setattr(real_object, field, value)
+            if isinstance(state, dict):
+                for field, value in state.items():
+                    setattr(real_object, field, value)
+            elif isinstance(state, tuple):
+                if hasattr(real_object, '__setstate__'):
+                    real_object.__setstate__(state)
+
             listitems = self.load_object(dump_object.listitems)
-            for listitem in listitems:
-                real_object.append(listitem)
+            if isinstance(listitems, Iterable):
+                for listitem in listitems:
+                    real_object.append(listitem)
+
             dictitems = self.load_object(dump_object.dictitems)
-            for key, dictitem in dictitems.items():
-                real_object[key] = dictitem
+            if isinstance(dictitems, Dict):
+                for key, dictitem in dictitems.items():
+                    real_object[key] = dictitem
         else:
             raise TypeError(f'Invalid type {dump_object}')
 
         id_ = PythonId(str(id(real_object)))
         self.dump_id_to_real_id[python_id] = id_
         self.memory[id_] = real_object
```

### Comparing `utbot_executor-1.4.9/utbot_executor/deep_serialization/memory_objects.py` & `utbot_executor-1.5.0/utbot_executor/deep_serialization/memory_objects.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from __future__ import annotations
+
+import copyreg
+import logging
+import traceback
 from itertools import zip_longest
 import pickle
-from typing import Any, Callable, Dict, List, Optional, Set, Type
+from typing import Any, Callable, Dict, List, Optional, Set, Type, Final, Iterable
 
 from utbot_executor.deep_serialization.utils import PythonId, get_kind, has_reduce, check_comparability, get_repr, \
     has_repr, TypeInfo, get_constructor_kind
 
+PICKLE_PROTO: Final = 4
+
 
 class MemoryObject:
     strategy: str
     typeinfo: TypeInfo
     comparable: bool
     is_draft: bool
     deserialized_obj: object
@@ -75,14 +81,19 @@
         serializer = PythonSerializer()
 
         for elem in self.obj:
             elem_id = serializer.write_object_to_memory(elem)
             self.items.append(elem_id)
 
         deserialized_obj = [serializer[elem] for elem in self.items]
+        if self.typeinfo.fullname == 'builtins.tuple':
+            deserialized_obj = tuple(deserialized_obj)
+        elif self.typeinfo.fullname == 'builtins.set':
+            deserialized_obj = set(deserialized_obj)
+
         comparable = all(serializer.get_by_id(elem).comparable for elem in self.items)
 
         super()._initialize(deserialized_obj, comparable)
 
     def __repr__(self) -> str:
         if hasattr(self, 'obj'):
             return str(self.obj)
@@ -157,33 +168,48 @@
             self.constructor = TypeInfo('builtins', 'object.__new__')
             self.args = serializer.write_object_to_memory([self.reduce_value[1][0]])
         else:
             callable_constructor = self.reduce_value[0]
             self.constructor = constructor_kind
             self.args = serializer.write_object_to_memory(self.reduce_value[1])
 
-        self.deserialized_obj = callable_constructor(*serializer[self.args])
+        args = serializer[self.args]
+        if isinstance(args, Iterable):
+            self.deserialized_obj = callable_constructor(*args)
 
     def initialize(self) -> None:
         serializer = PythonSerializer()
 
         self.comparable = True  # for recursive objects
         self.state = serializer.write_object_to_memory(self.reduce_value[2])
         self.listitems = serializer.write_object_to_memory(list(self.reduce_value[3]))
         self.dictitems = serializer.write_object_to_memory(dict(self.reduce_value[4]))
 
         deserialized_obj = self.deserialized_obj
-        for key, value in serializer[self.state].items():
-            object.__setattr__(deserialized_obj, key, value)  # TODO: change object.__setattr__ by self.__setattr__?
-        for item in serializer[self.listitems]:
-            deserialized_obj.append(item)
-        for key, value in serializer[self.dictitems].items():
-            deserialized_obj[key] = value
+        state = serializer[self.state]
+        if isinstance(state, dict):
+            for key, value in state.items():
+                setattr(deserialized_obj, key, value)
+        elif hasattr(deserialized_obj, '__setstate__'):
+            deserialized_obj.__setstate__(state)
+
+        items = serializer[self.listitems]
+        if isinstance(items, Iterable):
+            for item in items:
+                deserialized_obj.append(item)
+
+        dictitems = serializer[self.dictitems]
+        if isinstance(dictitems, Dict):
+            for key, value in dictitems.items():
+                deserialized_obj[key] = value
 
-        comparable = self.obj == deserialized_obj
+        if self.typeinfo.fullname == 'numpy.ndarray':
+            comparable = bool((self.obj == deserialized_obj).all())
+        else:
+            comparable = self.obj == deserialized_obj
 
         super()._initialize(deserialized_obj, comparable)
 
 
 class MemoryObjectProvider(object):
     @staticmethod
     def get_serializer(obj: object) -> Optional[Type[MemoryObject]]:
```

### Comparing `utbot_executor-1.4.9/utbot_executor/deep_serialization/utils.py` & `utbot_executor-1.5.0/utbot_executor/deep_serialization/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 
     @property
     def qualname(self):
         if self.module == '' or self.module == 'builtins':
             return self.kind
         return f'{self.module}.{self.kind}'
 
+    @property
+    def fullname(self):
+        if self.module == '':
+            return self.kind
+        return f'{self.module}.{self.kind}'
+
     @staticmethod
     def from_str(representation: str) -> TypeInfo:
         if '.' in representation:
             return TypeInfo(representation.rsplit('.', 1)[0], representation.rsplit('.', 1)[1])
         return TypeInfo('', representation)
 
     def __str__(self):
@@ -55,18 +61,19 @@
         return TypeInfo(py_object.__module__, py_object.__qualname__)
     module = type(py_object).__module__
     qualname = type(py_object).__qualname__
     return TypeInfo(module, qualname)
 
 
 def has_reduce(py_object: object) -> bool:
-    if getattr(py_object, '__reduce__', None) is None:
+    reduce = getattr(py_object, '__reduce__', None)
+    if reduce is None:
         return False
     try:
-        py_object.__reduce__()
+        reduce()
         return True
     except TypeError:
         return False
     except pickle.PicklingError:
         return False
     except Exception:
         return False
@@ -97,14 +104,15 @@
     except Exception:
         return False
 
 
 def has_repr(py_object: object) -> bool:
     reprable_types = [
             type(None),
+            bool,
             int,
             float,
             bytes,
             bytearray,
             str,
             # tuple,
             # list,
```

### Comparing `utbot_executor-1.4.9/utbot_executor/executor.py` & `utbot_executor-1.5.0/utbot_executor/executor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,46 @@
 """Python code executor for UnitTestBot"""
+import copy
 import inspect
 import importlib
 import json
 import logging
 import pathlib
 import sys
 import trace
 import traceback
 from typing import Any, Callable, Dict, Iterable, List, Tuple
 
-from utbot_executor.deep_serialization.deep_serialization import serialize_objects, serialize_memory_dump
+from utbot_executor.deep_serialization.deep_serialization import serialize_objects, serialize_memory_dump, \
+    serialize_objects_dump
 from utbot_executor.deep_serialization.json_converter import DumpLoader, deserialize_memory_objects
-from utbot_executor.deep_serialization.memory_objects import MemoryDump
+from utbot_executor.deep_serialization.memory_objects import MemoryDump, ReduceMemoryObject, PythonSerializer
 from utbot_executor.deep_serialization.utils import PythonId, getattr_by_path
+from utbot_executor.memory_compressor import compress_memory
 from utbot_executor.parser import ExecutionRequest, ExecutionResponse, ExecutionFailResponse, ExecutionSuccessResponse
 from utbot_executor.utils import suppress_stdout as __suppress_stdout
 
 __all__ = ['PythonExecutor']
 
 
+def _update_states(init_memory_dump: MemoryDump, state_before: MemoryDump) -> MemoryDump:
+    for id_, obj in state_before.objects.items():
+        if id_ not in init_memory_dump.objects:
+            init_memory_dump.objects[id_] = obj
+    return init_memory_dump
+
+
+def _load_objects(objs: List[Any]) -> MemoryDump:
+    serializer = PythonSerializer()
+    serializer.clear_visited()
+    for obj in objs:
+        serializer.write_object_to_memory(obj)
+    return serializer.memory
+
+
 class PythonExecutor:
     @staticmethod
     def add_syspaths(syspaths: Iterable[str]):
         for path in syspaths:
             if path not in sys.path:
                 sys.path.insert(0, path)
 
@@ -71,67 +89,70 @@
                         "fail",
                         f"Invalid function path {request.function_module}.{request.function_name}"
                         )
             logging.debug("Function initialized")
             args = [loader.load_object(PythonId(arg_id)) for arg_id in request.arguments_ids]
             logging.debug("Arguments: %s", args)
             kwargs = {name: loader.load_object(PythonId(kwarg_id)) for name, kwarg_id in request.kwarguments_ids.items()}
-        except Exception as ex:
+        except Exception as _:
             logging.debug("Error \n%s", traceback.format_exc())
             return ExecutionFailResponse("fail", traceback.format_exc())
         logging.debug("Arguments have been created")
 
         try:
-            state_before = loader.update_states(loader.reload_id())
+            state_before_memory = _load_objects(args + list(kwargs.values()))
+            init_state_before = _update_states(loader.reload_id(), state_before_memory)
+            serialized_state_init = serialize_memory_dump(init_state_before)
             value = _run_calculate_function_value(
                     function,
                     args,
                     kwargs,
                     request.filepath,
-                    state_before
+                    serialized_state_init
                     )
-        except Exception as ex:
+        except Exception as _:
             logging.debug("Error \n%s", traceback.format_exc())
             return ExecutionFailResponse("fail", traceback.format_exc())
         logging.debug("Value have been calculated: %s", value)
         return value
 
 
 def _serialize_state(
         args: List[Any],
         kwargs: Dict[str, Any],
         result: Any = None,
-        ) -> Tuple[List[PythonId], Dict[str, PythonId], PythonId, str]:
+        ) -> Tuple[List[PythonId], Dict[str, PythonId], PythonId, MemoryDump, str]:
     """Serialize objects from args, kwargs and result.
 
     Returns: tuple of args ids, kwargs ids, result id and serialized memory."""
 
     all_arguments = args + list(kwargs.values()) + [result]
 
-    ids, serialized_memory = serialize_objects(all_arguments, True)
+    ids, memory, serialized_memory = serialize_objects_dump(all_arguments, True)
     return (
             ids[:len(args)],
             dict(zip(kwargs.keys(), ids[len(args):len(args)+len(kwargs)])),
             ids[-1],
+            copy.deepcopy(memory),
             serialized_memory,
             )
 
 
 def _run_calculate_function_value(
         function: Callable,
         args: List[Any],
         kwargs: Dict[str, Any],
         fullpath: str,
-        state_before: MemoryDump
+        state_init: str
     ) -> ExecutionResponse:
     """ Calculate function evaluation result.
 
     Return serialized data: status, coverage info, object ids and memory."""
 
-    # _, _, _, state_before = serialize_memory_dump()
+    _, _, _, state_before, serialized_state_before = _serialize_state(args, kwargs)
 
     __is_exception = False
 
     (__sources, __start, ) = inspect.getsourcelines(function)
     __end = __start + len(__sources)
 
     __tracer = trace.Trace(
@@ -153,20 +174,25 @@
     __stmts = [x[1] for x in __tracer.counts if pathlib.PurePath(x[0]) == module_path]
     __stmts_filtered = [x for x in range(__start, __end) if x in __stmts]
     __stmts_filtered_with_def = [__start] + __stmts_filtered
     __missed_filtered = [x for x in range(__start, __end) if x not in __stmts_filtered_with_def]
     logging.debug("Covered lines: %s", __stmts_filtered_with_def)
     logging.debug("Missed lines: %s", __missed_filtered)
 
-    args_ids, kwargs_ids, result_id, state_after = _serialize_state(args, kwargs, __result)
+    args_ids, kwargs_ids, result_id, state_after, serialized_state_after = _serialize_state(args, kwargs, __result)
+    ids = args_ids + list(kwargs_ids.values())
+    # state_before, state_after = compress_memory(ids, state_before, state_after)
+    diff_ids = compress_memory(ids, state_before, state_after)
 
     return ExecutionSuccessResponse(
             status="success",
             is_exception=__is_exception,
             statements=__stmts_filtered_with_def,
             missed_statements=__missed_filtered,
-            state_before=state_before,
-            state_after=state_after,
+            state_init=state_init,
+            state_before=serialized_state_before,
+            state_after=serialized_state_after,
+            diff_ids=diff_ids,
             args_ids=args_ids,
             kwargs_ids=kwargs_ids,
             result_id=result_id,
             )
```

### Comparing `utbot_executor-1.4.9/utbot_executor/listener.py` & `utbot_executor-1.5.0/utbot_executor/listener.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.4.9/utbot_executor/parser.py` & `utbot_executor-1.5.0/utbot_executor/parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,16 +21,18 @@
 
 @dataclasses.dataclass
 class ExecutionSuccessResponse(ExecutionResponse):
     status: str
     is_exception: bool
     statements: List[int]
     missed_statements: List[int]
+    state_init: str
     state_before: str
     state_after: str
+    diff_ids: List[str]
     args_ids: List[str]
     kwargs_ids: Dict[str, str]
     result_id: str
 
 
 @dataclasses.dataclass
 class ExecutionFailResponse(ExecutionResponse):
@@ -70,16 +72,18 @@
     def default(self, o):
         if isinstance(o, ExecutionSuccessResponse):
             return {
                 "status": o.status,
                 "isException": o.is_exception,
                 "statements": o.statements,
                 "missedStatements": o.missed_statements,
+                "stateInit": o.state_init,
                 "stateBefore": o.state_before,
                 "stateAfter": o.state_after,
+                "diffIds": o.diff_ids,
                 "argsIds": o.args_ids,
                 "kwargsIds": o.kwargs_ids,
                 "resultId": o.result_id,
             }
         if isinstance(o, ExecutionFailResponse):
             return {
                 "status": o.status,
```

### Comparing `utbot_executor-1.4.9/setup.py` & `utbot_executor-1.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 entry_points = \
 {'console_scripts': ['utbot-executor = utbot_executor:utbot_executor']}
 
 setup_kwargs = {
     'name': 'utbot-executor',
-    'version': '1.4.9',
+    'version': '1.5.0',
     'description': '',
     'long_description': '# UtBot Executor\n\nUtil for python code execution and state serialization.\n\n## Installation\n\nYou can install module from [PyPI](https://pypi.org/project/utbot-executor/):\n\n```bash\npython -m pip install utbot-executor\n```\n\n## Usage\n\n### From console with socket listener\n\nRun with your `<hostname>` and `<port>` for socket connection\n```bash\n$ python -m utbot_executor <hostname> <port> <logfile> [<loglevel DEBUG | INFO | ERROR>]\n```\n\n### Result format:\n\n```json\n{\n        "status": "success",\n        "isException": bool,\n        "statements": list[int],\n        "missedStatements": list[int],\n        "stateBefore": memory json dump,\n        "stateAfter": memory json dump,\n        "argsIds": list[str],\n        "kwargs": list[str],\n        "resultId": str,\n}\n```\n\nor error format:\n\n```json\n{\n        "status": "fail",\n        "exception": str (traceback),\n}\n```\n\n#### States format\n\nTODO\n\n### Submodule `deep_serialization`\n\nJSON serializer and deserializer for python objects\n\n## Source\n\nGitHub [repository](https://github.com/tamarinvs19/utbot_executor)\n',
     'author': 'Vyacheslav Tamarin',
     'author_email': 'vyacheslav.tamarin@yandex.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `utbot_executor-1.4.9/PKG-INFO` & `utbot_executor-1.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: utbot-executor
-Version: 1.4.9
+Version: 1.5.0
 Summary: 
 Author: Vyacheslav Tamarin
 Author-email: vyacheslav.tamarin@yandex.ru
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # UtBot Executor
```

