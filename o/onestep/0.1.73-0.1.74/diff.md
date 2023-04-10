# Comparing `tmp/onestep-0.1.73.tar.gz` & `tmp/onestep-0.1.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onestep-0.1.73.tar", max compression
+gzip compressed data, was "onestep-0.1.74.tar", max compression
```

## Comparing `onestep-0.1.73.tar` & `onestep-0.1.74.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1362 2023-04-07 10:01:22.261018 onestep-0.1.73/README.md
--rw-r--r--   0        0        0      704 2023-04-07 10:01:22.265018 onestep-0.1.73/pyproject.toml
--rw-r--r--   0        0        0     1374 2023-04-07 10:01:22.265018 onestep-0.1.73/src/onestep/__init__.py
--rw-r--r--   0        0        0      221 2023-04-07 10:01:22.265018 onestep-0.1.73/src/onestep/broker/__init__.py
--rw-r--r--   0        0        0     4310 2023-04-07 10:01:22.265018 onestep-0.1.73/src/onestep/broker/base.py
--rw-r--r--   0        0        0      957 2023-04-07 10:01:22.265018 onestep-0.1.73/src/onestep/broker/cron.py
--rw-r--r--   0        0        0      151 2023-04-07 10:01:22.265018 onestep-0.1.73/src/onestep/broker/memory.py
--rw-r--r--   0        0        0     1997 2023-04-07 10:01:22.265018 onestep-0.1.73/src/onestep/broker/rabbitmq.py
--rw-r--r--   0        0        0     2144 2023-04-07 10:01:22.265018 onestep-0.1.73/src/onestep/broker/webhook.py
--rw-r--r--   0        0        0      610 2023-04-07 10:01:22.265018 onestep-0.1.73/src/onestep/exception.py
--rw-r--r--   0        0        0     3163 2023-04-07 10:01:22.265018 onestep-0.1.73/src/onestep/message.py
--rw-r--r--   0        0        0      286 2023-04-07 10:01:22.265018 onestep-0.1.73/src/onestep/middleware/__init__.py
--rw-r--r--   0        0        0      521 2023-04-07 10:01:22.265018 onestep-0.1.73/src/onestep/middleware/base.py
--rw-r--r--   0        0        0     2438 2023-04-07 10:01:22.265018 onestep-0.1.73/src/onestep/middleware/config.py
--rw-r--r--   0        0        0     6350 2023-04-07 10:01:22.265018 onestep-0.1.73/src/onestep/onestep.py
--rw-r--r--   0        0        0     2699 2023-04-07 10:01:22.265018 onestep-0.1.73/src/onestep/retry.py
--rw-r--r--   0        0        0      293 2023-04-07 10:01:22.265018 onestep-0.1.73/src/onestep/signal.py
--rw-r--r--   0        0        0      618 2023-04-07 10:01:22.265018 onestep-0.1.73/src/onestep/state.py
--rw-r--r--   0        0        0       36 2023-04-07 10:01:22.265018 onestep-0.1.73/src/onestep/store/__init__.py
--rw-r--r--   0        0        0     4170 2023-04-07 10:01:22.265018 onestep-0.1.73/src/onestep/store/rabbitmq.py
--rw-r--r--   0        0        0     3517 2023-04-07 10:01:22.265018 onestep-0.1.73/src/onestep/worker.py
--rw-r--r--   0        0        0     1993 1970-01-01 00:00:00.000000 onestep-0.1.73/PKG-INFO
+-rw-r--r--   0        0        0     1362 2023-04-10 06:30:32.363794 onestep-0.1.74/README.md
+-rw-r--r--   0        0        0      704 2023-04-10 06:30:32.363794 onestep-0.1.74/pyproject.toml
+-rw-r--r--   0        0        0     1374 2023-04-10 06:30:32.363794 onestep-0.1.74/src/onestep/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-10 06:30:32.363794 onestep-0.1.74/src/onestep/broker/__init__.py
+-rw-r--r--   0        0        0     4310 2023-04-10 06:30:32.363794 onestep-0.1.74/src/onestep/broker/base.py
+-rw-r--r--   0        0        0      957 2023-04-10 06:30:32.363794 onestep-0.1.74/src/onestep/broker/cron.py
+-rw-r--r--   0        0        0      151 2023-04-10 06:30:32.363794 onestep-0.1.74/src/onestep/broker/memory.py
+-rw-r--r--   0        0        0     1997 2023-04-10 06:30:32.363794 onestep-0.1.74/src/onestep/broker/rabbitmq.py
+-rw-r--r--   0        0        0     2144 2023-04-10 06:30:32.363794 onestep-0.1.74/src/onestep/broker/webhook.py
+-rw-r--r--   0        0        0      610 2023-04-10 06:30:32.363794 onestep-0.1.74/src/onestep/exception.py
+-rw-r--r--   0        0        0     3443 2023-04-10 06:30:32.363794 onestep-0.1.74/src/onestep/message.py
+-rw-r--r--   0        0        0      286 2023-04-10 06:30:32.363794 onestep-0.1.74/src/onestep/middleware/__init__.py
+-rw-r--r--   0        0        0      521 2023-04-10 06:30:32.363794 onestep-0.1.74/src/onestep/middleware/base.py
+-rw-r--r--   0        0        0     2438 2023-04-10 06:30:32.363794 onestep-0.1.74/src/onestep/middleware/config.py
+-rw-r--r--   0        0        0     6350 2023-04-10 06:30:32.363794 onestep-0.1.74/src/onestep/onestep.py
+-rw-r--r--   0        0        0     2699 2023-04-10 06:30:32.363794 onestep-0.1.74/src/onestep/retry.py
+-rw-r--r--   0        0        0      293 2023-04-10 06:30:32.363794 onestep-0.1.74/src/onestep/signal.py
+-rw-r--r--   0        0        0      618 2023-04-10 06:30:32.363794 onestep-0.1.74/src/onestep/state.py
+-rw-r--r--   0        0        0       36 2023-04-10 06:30:32.363794 onestep-0.1.74/src/onestep/store/__init__.py
+-rw-r--r--   0        0        0     4170 2023-04-10 06:30:32.363794 onestep-0.1.74/src/onestep/store/rabbitmq.py
+-rw-r--r--   0        0        0     3517 2023-04-10 06:30:32.363794 onestep-0.1.74/src/onestep/worker.py
+-rw-r--r--   0        0        0     1993 1970-01-01 00:00:00.000000 onestep-0.1.74/PKG-INFO
```

### Comparing `onestep-0.1.73/README.md` & `onestep-0.1.74/README.md`

 * *Files identical despite different names*

### Comparing `onestep-0.1.73/pyproject.toml` & `onestep-0.1.74/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onestep"
-version = "0.1.73"
+version = "0.1.74"
 description = ""
 authors = ["miclon <jcnd@163.com>"]
 readme = "README.md"
 packages = [
     { include = 'onestep', from = 'src' }
 ]
```

### Comparing `onestep-0.1.73/src/onestep/__init__.py` & `onestep-0.1.74/src/onestep/__init__.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.73/src/onestep/broker/base.py` & `onestep-0.1.74/src/onestep/broker/base.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.73/src/onestep/broker/cron.py` & `onestep-0.1.74/src/onestep/broker/cron.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.73/src/onestep/broker/rabbitmq.py` & `onestep-0.1.74/src/onestep/broker/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.73/src/onestep/broker/webhook.py` & `onestep-0.1.74/src/onestep/broker/webhook.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.73/src/onestep/exception.py` & `onestep-0.1.74/src/onestep/exception.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.73/src/onestep/message.py` & `onestep-0.1.74/src/onestep/message.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,119 +5,122 @@
 
 
 class Extra:
     def __init__(self, task_id=None, publish_time=None, failure_count=0):
         self.task_id = task_id or str(uuid.uuid4())
         self.publish_time = publish_time or round(time.time(), 3)
         self.failure_count = failure_count
-
+    
     def to_dict(self):
         return {
             'task_id': self.task_id,
             'publish_time': self.publish_time,
             'failure_count': self.failure_count,
         }
-
+    
     def __str__(self):
         return str(self.to_dict())
-
+    
     def __repr__(self):
         return f"{self.__class__.__name__}({self.task_id}, {self.publish_time}, {self.failure_count})"
 
 
 class Message:
-
+    
     def __init__(
             self,
             body: Optional[Union[dict, Any]] = None,
             extra: Optional[Union[dict, Extra]] = None,
             msg: Optional[Any] = None,
             broker=None
     ):
         self.body = body
         self.extra = self._set_extra(extra)
         self.msg = msg
-
+        
         self.broker = broker
         self._exception = None
-
+    
     @staticmethod
     def _set_extra(extra):
         if isinstance(extra, Extra):
             return extra
         elif isinstance(extra, dict):
             return Extra(**extra)
         else:
             return Extra()
-
+    
     def set_exception(self, exception):
         self.exception = exception
         self.failure_count = self.failure_count + 1
-
+    
     @property
     def exception(self):
         return self._exception
-
+    
     @exception.setter
     def exception(self, value):
         self._exception = value
-
+    
     @property
     def fail(self):
         return self.exception is not None
-
+    
     @property
     def failure_count(self):
         return self.extra.failure_count
-
+    
     @failure_count.setter
     def failure_count(self, value):
         self.extra.failure_count = value
-
+    
     def replace(self, **kwargs):
         """替换当前message的属性"""
         for key, value in kwargs.items():
             if not hasattr(self, key):
                 continue
             if key == 'extra':
                 value = self._set_extra(value)
             setattr(self, key, value)
         return self
-
-    def to_dict(self) -> dict:
-        return {'body': self.body, 'extra': self.extra.to_dict()}
-
-    def to_json(self) -> str:
-        return json.dumps(self.to_dict())
-
+    
+    def to_dict(self, include_exception=False) -> dict:
+        data = {'body': self.body, 'extra': self.extra.to_dict()}
+        if include_exception and self.exception:
+            data['exception'] = str(self.exception)
+        return data
+    
+    def to_json(self, include_exception=False) -> str:
+        return json.dumps(self.to_dict(include_exception))
+    
     def confirm(self):
         """确认消息"""
         if self.broker:
             self.broker.confirm(self)
-
+    
     def reject(self):
         """拒绝消息 （原始状态重入）"""
         if self.broker:
             self.broker.reject(self)
-
+    
     def requeue(self):
         """重发消息 （最新状态重入）"""
         if self.broker:
             self.broker.requeue(self)
-
+    
     def __getattr__(self, item):
         return None
-
+    
     def __delattr__(self, item):
         if hasattr(self, item):
             setattr(self, item, None)
-
+    
     def __str__(self):
         return str(self.to_dict())
-
+    
     def __repr__(self):
         return f"<{self.__class__.__name__} {self.body}>"
 
 
 if __name__ == '__main__':
     msg = Message()
     msg.x = 1
```

### Comparing `onestep-0.1.73/src/onestep/middleware/base.py` & `onestep-0.1.74/src/onestep/middleware/base.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.73/src/onestep/middleware/config.py` & `onestep-0.1.74/src/onestep/middleware/config.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.73/src/onestep/onestep.py` & `onestep-0.1.74/src/onestep/onestep.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.73/src/onestep/retry.py` & `onestep-0.1.74/src/onestep/retry.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.73/src/onestep/state.py` & `onestep-0.1.74/src/onestep/state.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.73/src/onestep/store/rabbitmq.py` & `onestep-0.1.74/src/onestep/store/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.73/src/onestep/worker.py` & `onestep-0.1.74/src/onestep/worker.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.73/PKG-INFO` & `onestep-0.1.74/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onestep
-Version: 0.1.73
+Version: 0.1.74
 Summary: 
 Author: miclon
 Author-email: jcnd@163.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

