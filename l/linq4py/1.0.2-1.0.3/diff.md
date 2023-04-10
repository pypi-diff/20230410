# Comparing `tmp/linq4py-1.0.2.tar.gz` & `tmp/linq4py-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linq4py-1.0.2.tar", last modified: Sat Apr  8 12:55:29 2023, max compression
+gzip compressed data, was "linq4py-1.0.3.tar", max compression
```

## Comparing `linq4py-1.0.2.tar` & `linq4py-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 12:55:29.918977 linq4py-1.0.2/
--rw-rw-rw-   0        0        0     1095 2023-04-08 11:12:41.000000 linq4py-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1851 2023-04-08 12:55:29.918476 linq4py-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1540 2023-04-08 12:15:42.000000 linq4py-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 12:55:29.906975 linq4py-1.0.2/linq4py/
--rw-rw-rw-   0        0        0       28 2023-04-08 12:55:20.000000 linq4py-1.0.2/linq4py/__init__.py
--rw-rw-rw-   0        0        0    36286 2023-04-08 12:55:02.000000 linq4py-1.0.2/linq4py/linq4py.py
-drwxrwxrwx   0        0        0        0 2023-04-08 12:55:29.916977 linq4py-1.0.2/linq4py.egg-info/
--rw-rw-rw-   0        0        0     1851 2023-04-08 12:55:29.000000 linq4py-1.0.2/linq4py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-04-08 12:55:29.000000 linq4py-1.0.2/linq4py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 12:55:29.000000 linq4py-1.0.2/linq4py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-08 12:55:29.000000 linq4py-1.0.2/linq4py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      423 2023-04-08 12:36:20.000000 linq4py-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-08 12:55:29.918977 linq4py-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      980 2023-04-08 12:51:50.000000 linq4py-1.0.2/setup.py
+-rw-r--r--   0        0        0     1095 2023-04-08 11:12:41.897031 linq4py-1.0.3/LICENSE
+-rw-r--r--   0        0        0       28 2023-04-08 12:55:20.756205 linq4py-1.0.3/linq4py/__init__.py
+-rw-r--r--   0        0        0     4241 2023-04-10 01:00:21.734794 linq4py-1.0.3/linq4py/core.py
+-rw-r--r--   0        0        0      220 2023-04-10 00:58:06.718825 linq4py-1.0.3/linq4py/exceptions.py
+-rw-r--r--   0        0        0    32067 2023-04-10 01:00:19.025581 linq4py-1.0.3/linq4py/linq4py.py
+-rw-r--r--   0        0        0      423 2023-04-10 01:00:49.877240 linq4py-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1540 2023-04-08 12:15:42.402975 linq4py-1.0.3/README.md
+-rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 linq4py-1.0.3/setup.py
+-rw-r--r--   0        0        0     1862 1970-01-01 00:00:00.000000 linq4py-1.0.3/PKG-INFO
```

### Comparing `linq4py-1.0.2/LICENSE` & `linq4py-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `linq4py-1.0.2/PKG-INFO` & `linq4py-1.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,58 +1,59 @@
-Metadata-Version: 2.1
-Name: linq4py
-Version: 1.0.2
-Summary: a python package for linq 
-Author: six006
-Author-email: six006@126.com
-License: MIT
-Keywords: python,linq for python,chain call
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# Linq for Python
-
-像C#或JavaScript一样链式写python
-
-## 1 代码说明
-代码Fork `https://pypi.org/project/py-linq/`
-
-## 2 新增功能
-- 新增：`filter`,`map`,`find`等类似于JavaScript`filter`,`map`,`find`
-- 使用函数式入口来初始化列表`linq4py.array()`
-
-## 3 举例
-
-```
-import linq4py as lp
-
-origin_items = [
-    {'id': '1', 'parent_id': '', 'name': 'indicator 1', 'weight': 1, 'has_child': True},
-    {'id': '2', 'parent_id': '1', 'name': 'indicator 2', 'weight': 0.6, 'has_child': True},
-    {'id': '3', 'parent_id': '1', 'name': 'indicator 3', 'weight': 0.4, 'has_child': True},
-    {'id': '4', 'parent_id': '2', 'name': 'indicator 4', 'weight': 0.5, 'has_child': False},
-    {'id': '5', 'parent_id': '2', 'name': 'indicator 5', 'weight': 0.8, 'has_child': False},
-    {'id': '6', 'parent_id': '3', 'name': 'indicator 6', 'weight': 0.8, 'has_child': False},
-    {'id': '7', 'parent_id': '3', 'name': 'indicator 7', 'weight': 0.8, 'has_child': False},
-]
-
-
-# count demo
-count = lp.array(origin_items).count(lambda item: item['has_child'])
-print(count)
-
-# filter,order_by_descending map demo
-items = lp.array(origin_items).filter(lambda item: item["has_child"]).order_by_descending(
-    lambda item: item['weight']).map(lambda item: (item['id'], item['name']))
-print(items)
-
-# find demo
-result = lp.array(origin_items).find(lambda item: item['weight'] > 0.3)
-print(result)
-
-```
-
-## 4 修改日志
-
-- 2023-04-08 重新打包
-- 2023-04-08 Fork项目并新增相关功能
+Metadata-Version: 2.1
+Name: linq4py
+Version: 1.0.3
+Summary: Linq for python
+Keywords: LINQ,linq for python
+Author: six006
+Author-email: six006@126.com
+Requires-Python: >=3.10
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+
+# Linq for Python
+
+像C#或JavaScript一样链式写python
+
+## 1 代码说明
+代码Fork `https://pypi.org/project/py-linq/`
+
+## 2 新增功能
+- 新增：`filter`,`map`,`find`等类似于JavaScript`filter`,`map`,`find`
+- 使用函数式入口来初始化列表`linq4py.array()`
+
+## 3 举例
+
+```
+import linq4py as lp
+
+origin_items = [
+    {'id': '1', 'parent_id': '', 'name': 'indicator 1', 'weight': 1, 'has_child': True},
+    {'id': '2', 'parent_id': '1', 'name': 'indicator 2', 'weight': 0.6, 'has_child': True},
+    {'id': '3', 'parent_id': '1', 'name': 'indicator 3', 'weight': 0.4, 'has_child': True},
+    {'id': '4', 'parent_id': '2', 'name': 'indicator 4', 'weight': 0.5, 'has_child': False},
+    {'id': '5', 'parent_id': '2', 'name': 'indicator 5', 'weight': 0.8, 'has_child': False},
+    {'id': '6', 'parent_id': '3', 'name': 'indicator 6', 'weight': 0.8, 'has_child': False},
+    {'id': '7', 'parent_id': '3', 'name': 'indicator 7', 'weight': 0.8, 'has_child': False},
+]
+
+
+# count demo
+count = lp.array(origin_items).count(lambda item: item['has_child'])
+print(count)
+
+# filter,order_by_descending map demo
+items = lp.array(origin_items).filter(lambda item: item["has_child"]).order_by_descending(
+    lambda item: item['weight']).map(lambda item: (item['id'], item['name']))
+print(items)
+
+# find demo
+result = lp.array(origin_items).find(lambda item: item['weight'] > 0.3)
+print(result)
+
+```
+
+## 4 修改日志
+
+- 2023-04-08 重新打包
+- 2023-04-08 Fork项目并新增相关功能
```

### Comparing `linq4py-1.0.2/README.md` & `linq4py-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `linq4py-1.0.2/linq4py/linq4py.py` & `linq4py-1.0.3/linq4py/linq4py.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,173 +5,25 @@
     TypeVar,
     Union,
     Optional,
     Callable,
 )
 
 from builtins import range
-import inspect
-from dataclasses import dataclass
+
+from linq4py.core import RepeatableIterable, OrderingDirection, Key, Node
+from linq4py.exceptions import NullArgumentError, NoMatchingElement, MoreThanOneMatchingElement, NoElementsError
 
 TEnumerable = TypeVar("TEnumerable", bound="Enumerable")
 TGrouping = TypeVar("TGrouping", bound="Grouping")
 TSortedEnumerable = TypeVar("TSortedEnumerable", bound="SortedEnumerable")
 TGroupedEnumerable = TypeVar("TGroupedEnumerable", bound="GroupedEnumerable")
 Number = Union[float, int]
 # core
 
-TNode = TypeVar("TNode", bound="Node")
-
-
-@dataclass
-class Node(object):
-    """
-    Node for linked list
-    """
-
-    value: Any
-    next: Optional[TNode] = None
-
-
-class Key(object):
-    def __init__(self, key, **kwargs):
-        """
-        Constructor for Key class. Autogenerates key properties in object
-        given dict or kwargs
-        :param key: dict of name-values
-        :param kwargs: optional keyword arguments
-        :return: void
-        """
-        key = key if key is not None else kwargs
-        self.__dict__.update(key)
-
-    def __repr__(self):
-        return self.__dict__.__repr__()
-
-
-class OrderingDirection(object):
-    def __init__(self, key, reverse):
-        """
-        A container to hold the lambda key and sorting direction
-        :param key: lambda function
-        :param reverse: boolean. True for reverse sort
-        """
-        self.key = key
-        self.descending = reverse
-
-
-class RepeatableIterable(object):
-    def __init__(self, data: Iterable[Any] = None):
-        """
-        Constructor. Pretty straight forward except for the is_generator check. This is so we
-        can detect when a function that generates data is passed as a datasource. In this case we
-        need to exhaust the values in the function generator
-        """
-        if data is None:
-            data = []
-        if not hasattr(data, "__iter__"):
-            raise TypeError(
-                u"RepeatableIterable must be instantiated with an iterable object"
-            )
-        self._data: Iterable[Any] = data
-        self._len = None
-        self._root: TNode = None
-        self._current: TNode = None
-
-    def __len__(self):
-        if self._len is None:
-            self._len = sum(1 for item in iter(self))
-        return self._len
-
-    def __reversed__(self) -> Any:
-        if inspect.isgenerator(self._data) or isinstance(self._data, itertools.chain):
-            # We need to collect the data from a generator since reversing a generator
-            # is not possible
-            self._data = list(self._data)
-        if self._root is None:
-            i = 0
-            for index, item in enumerate(reversed(self._data)):
-                node = Node(value=item)
-                if index == 0:
-                    self._root = node
-                    self._current = self._root
-                else:
-                    self._current.next = node
-                    self._current = self._current.next
-                yield node.value
-                i += 1
-            self._len = i
-        else:
-            while self._current is not None:
-                yield self._current.value
-                self._current = self._current.next
-        self._current = self._root
-
-    def __iter__(self) -> Any:
-        if self._root is None:
-            i = 0
-            for index, item in enumerate(self._data):
-                node = Node(value=item)
-                if index == 0:
-                    self._root = node
-                    self._current = self._root
-                else:
-                    self._current.next = node
-                    self._current = self._current.next
-                yield node.value
-                i += 1
-            self._len = i
-        else:
-            while self._current is not None:
-                yield self._current.value
-                self._current = self._current.next
-        self._current = self._root
-
-    def __next__(self):
-        if self._current.next is None:
-            self._current = self._root
-            raise StopIteration
-        self._current = self._current.next
-        return self._current.value
-
-    @property
-    def current(self) -> Optional[TNode]:
-        return self._current
-
-    @current.setter
-    def current(self, node: TNode) -> None:
-        self._current = node
-
-    @property
-    def head(self) -> Optional[TNode]:
-        return self._root
-
-    @head.setter
-    def head(self, node: TNode) -> None:
-        self._root = node
-
-    def next(self):
-        return self.__next__()
-
-
-# exception
-class NoElementsError(Exception):
-    pass
-
-
-class NullArgumentError(Exception):
-    pass
-
-
-class NoMatchingElement(Exception):
-    pass
-
-
-class MoreThanOneMatchingElement(Exception):
-    pass
 
 
 class Enumerable(object):
     def __init__(self, data=None):
         """
         Constructor
         ** Note: no type checking of the data elements are performed during
```

