# Comparing `tmp/on_rails-2.1.0.tar.gz` & `tmp/on_rails-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "on_rails-2.1.0.tar", max compression
+gzip compressed data, was "on_rails-3.0.0.tar", max compression
```

## Comparing `on_rails-2.1.0.tar` & `on_rails-3.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    35149 2023-04-07 20:45:45.970074 on_rails-2.1.0/LICENSE
--rw-r--r--   0        0        0    14163 2023-04-07 20:45:45.970074 on_rails-2.1.0/README.md
--rw-r--r--   0        0        0    19087 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/Result.py
--rw-r--r--   0        0        0     2866 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetail.py
--rw-r--r--   0        0        0     1504 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/ErrorDetail.py
--rw-r--r--   0        0        0      808 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Errors/BadRequestError.py
--rw-r--r--   0        0        0      819 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Errors/ConflictError.py
--rw-r--r--   0        0        0      840 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Errors/ExceptionError.py
--rw-r--r--   0        0        0      728 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Errors/ForbiddenError.py
--rw-r--r--   0        0        0      726 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Errors/InternalError.py
--rw-r--r--   0        0        0     1227 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Errors/NotFoundError.py
--rw-r--r--   0        0        0      880 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Errors/UnauthorizedError.py
--rw-r--r--   0        0        0      753 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Errors/ValidationError.py
--rw-r--r--   0        0        0      474 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Errors/__init__.py
--rw-r--r--   0        0        0      573 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Success/CreatedDetail.py
--rw-r--r--   0        0        0      629 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Success/NotModifiedDetail.py
--rw-r--r--   0        0        0      831 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Success/PartialContentDetail.py
--rw-r--r--   0        0        0      188 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Success/__init__.py
--rw-r--r--   0        0        0     1034 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/SuccessDetail.py
--rw-r--r--   0        0        0      100 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/__init__.py
--rw-r--r--   0        0        0       99 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/__init__.py
--rw-r--r--   0        0        0     3337 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/_utility.py
--rw-r--r--   0        0        0     1585 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/decorator.py
--rw-r--r--   0        0        0      722 2023-04-07 20:45:45.970074 on_rails-2.1.0/pyproject.toml
--rw-r--r--   0        0        0    14790 1970-01-01 00:00:00.000000 on_rails-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-10 18:02:38.936610 on_rails-3.0.0/LICENSE
+-rw-r--r--   0        0        0    14186 2023-04-10 18:02:38.936610 on_rails-3.0.0/README.md
+-rw-r--r--   0        0        0    37998 2023-04-10 18:02:38.936610 on_rails-3.0.0/on_rails/Result.py
+-rw-r--r--   0        0        0     2866 2023-04-10 18:02:38.936610 on_rails-3.0.0/on_rails/ResultDetail.py
+-rw-r--r--   0        0        0     1504 2023-04-10 18:02:38.936610 on_rails-3.0.0/on_rails/ResultDetails/ErrorDetail.py
+-rw-r--r--   0        0        0      808 2023-04-10 18:02:38.936610 on_rails-3.0.0/on_rails/ResultDetails/Errors/BadRequestError.py
+-rw-r--r--   0        0        0      819 2023-04-10 18:02:38.936610 on_rails-3.0.0/on_rails/ResultDetails/Errors/ConflictError.py
+-rw-r--r--   0        0        0      840 2023-04-10 18:02:38.936610 on_rails-3.0.0/on_rails/ResultDetails/Errors/ExceptionError.py
+-rw-r--r--   0        0        0      728 2023-04-10 18:02:38.936610 on_rails-3.0.0/on_rails/ResultDetails/Errors/ForbiddenError.py
+-rw-r--r--   0        0        0      726 2023-04-10 18:02:38.936610 on_rails-3.0.0/on_rails/ResultDetails/Errors/InternalError.py
+-rw-r--r--   0        0        0     1227 2023-04-10 18:02:38.936610 on_rails-3.0.0/on_rails/ResultDetails/Errors/NotFoundError.py
+-rw-r--r--   0        0        0      880 2023-04-10 18:02:38.936610 on_rails-3.0.0/on_rails/ResultDetails/Errors/UnauthorizedError.py
+-rw-r--r--   0        0        0      753 2023-04-10 18:02:38.936610 on_rails-3.0.0/on_rails/ResultDetails/Errors/ValidationError.py
+-rw-r--r--   0        0        0      474 2023-04-10 18:02:38.936610 on_rails-3.0.0/on_rails/ResultDetails/Errors/__init__.py
+-rw-r--r--   0        0        0      573 2023-04-10 18:02:38.936610 on_rails-3.0.0/on_rails/ResultDetails/Success/CreatedDetail.py
+-rw-r--r--   0        0        0      629 2023-04-10 18:02:38.936610 on_rails-3.0.0/on_rails/ResultDetails/Success/NotModifiedDetail.py
+-rw-r--r--   0        0        0      831 2023-04-10 18:02:38.936610 on_rails-3.0.0/on_rails/ResultDetails/Success/PartialContentDetail.py
+-rw-r--r--   0        0        0      188 2023-04-10 18:02:38.936610 on_rails-3.0.0/on_rails/ResultDetails/Success/__init__.py
+-rw-r--r--   0        0        0     1034 2023-04-10 18:02:38.936610 on_rails-3.0.0/on_rails/ResultDetails/SuccessDetail.py
+-rw-r--r--   0        0        0      100 2023-04-10 18:02:38.936610 on_rails-3.0.0/on_rails/ResultDetails/__init__.py
+-rw-r--r--   0        0        0       99 2023-04-10 18:02:38.936610 on_rails-3.0.0/on_rails/__init__.py
+-rw-r--r--   0        0        0     4780 2023-04-10 18:02:38.936610 on_rails-3.0.0/on_rails/_utility.py
+-rw-r--r--   0        0        0     1760 2023-04-10 18:02:38.936610 on_rails-3.0.0/on_rails/decorator.py
+-rw-r--r--   0        0        0      722 2023-04-10 18:02:38.936610 on_rails-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0    14813 1970-01-01 00:00:00.000000 on_rails-3.0.0/PKG-INFO
```

### Comparing `on_rails-2.1.0/LICENSE` & `on_rails-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `on_rails-2.1.0/README.md` & `on_rails-3.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 by using functional programming concepts, developers can write code that is easier to reason about and understand, which
 can lead to faster development cycles and better quality code.
 
 ## Getting Started
 
 Use `pip` to install package:
 
-`pip install on_rails`
+`pip install on_rails --upgrade`
 
 ## Usage
 
 ### Sample 1
 
 ```python
 from on_rails import Result, def_result
@@ -123,16 +123,16 @@
 
 @def_result()
 def get_number() -> Result:
     number = int(input("Enter number: "))
     return Result.ok(number)
 
 
-get_number()\
-    .on_success(lambda prev: print(f"Number is valid: {prev.value}"))\
+get_number()
+    .on_success(lambda value: print(f"Number is valid: {value}"))
     .on_fail(lambda prev: print(prev.detail))
 ```
 
 Within the `get_number` function, the user is prompted to enter an integer number. If the user enters a valid integer,
 the number is returned as a successful result using `Result.ok()`, otherwise, an error message is returned as a failed
 result.
 
@@ -238,15 +238,15 @@
     return Result.ok(response.json(), detail)
 
 
 def fake_operation():
     return Result.ok()
 
 
-fake_operation().on_success(create_data, num_of_try=5)
+fake_operation().on_success(lambda: create_data(url, data), num_of_try=5)
 
 ```
 
 In the example above, if the request goes wrong, an **exception** will be raised. By setting `num_of_try`, you can
 specify how many times the operation should be repeated in case of an error.
 
 ### Sample 5: Async Decorator
```

### Comparing `on_rails-2.1.0/on_rails/ResultDetail.py` & `on_rails-3.0.0/on_rails/ResultDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.1.0/on_rails/ResultDetails/ErrorDetail.py` & `on_rails-3.0.0/on_rails/ResultDetails/ErrorDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.1.0/on_rails/ResultDetails/Errors/BadRequestError.py` & `on_rails-3.0.0/on_rails/ResultDetails/Errors/BadRequestError.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.1.0/on_rails/ResultDetails/Errors/ConflictError.py` & `on_rails-3.0.0/on_rails/ResultDetails/Errors/ConflictError.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.1.0/on_rails/ResultDetails/Errors/ExceptionError.py` & `on_rails-3.0.0/on_rails/ResultDetails/Errors/ExceptionError.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.1.0/on_rails/ResultDetails/Errors/ForbiddenError.py` & `on_rails-3.0.0/on_rails/ResultDetails/Errors/ForbiddenError.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.1.0/on_rails/ResultDetails/Errors/InternalError.py` & `on_rails-3.0.0/on_rails/ResultDetails/Errors/InternalError.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.1.0/on_rails/ResultDetails/Errors/NotFoundError.py` & `on_rails-3.0.0/on_rails/ResultDetails/Errors/NotFoundError.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.1.0/on_rails/ResultDetails/Errors/UnauthorizedError.py` & `on_rails-3.0.0/on_rails/ResultDetails/Errors/UnauthorizedError.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.1.0/on_rails/ResultDetails/Errors/ValidationError.py` & `on_rails-3.0.0/on_rails/ResultDetails/Errors/ValidationError.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.1.0/on_rails/ResultDetails/Success/CreatedDetail.py` & `on_rails-3.0.0/on_rails/ResultDetails/Success/CreatedDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.1.0/on_rails/ResultDetails/Success/NotModifiedDetail.py` & `on_rails-3.0.0/on_rails/ResultDetails/Success/NotModifiedDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.1.0/on_rails/ResultDetails/Success/PartialContentDetail.py` & `on_rails-3.0.0/on_rails/ResultDetails/Success/PartialContentDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.1.0/on_rails/ResultDetails/SuccessDetail.py` & `on_rails-3.0.0/on_rails/ResultDetails/SuccessDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.1.0/on_rails/_utility.py` & `on_rails-3.0.0/on_rails/_utility.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import inspect
+from asyncio import AbstractEventLoop
 from typing import Any, Coroutine, List
 
 from on_rails.ResultDetails.ErrorDetail import ErrorDetail
 
 
 def get_num_of_function_parameters(func: callable) -> int:
     """
@@ -36,15 +37,15 @@
     returned. If it is not a coroutine, its result will be returned as is.
     :return: Returns the result of the input function `func`. If the result is an instance of
     `Coroutine`, it will be run using the `asyncio` event loop until it completes, and the final result will be returned.
     Otherwise, the original result will be returned.
     """
     result = func()
     if isinstance(result, Coroutine):
-        return asyncio.get_event_loop().run_until_complete(result)
+        return get_loop().run_until_complete(result)
     return result
 
 
 def generate_error(errors: List[Any], num_of_try: int) -> ErrorDetail:
     """
     This function generates an error detail object with information about the number of attempts made, any errors
     encountered, and whether any of the errors were exceptions.
@@ -65,7 +66,40 @@
         if exception is not None:
             message += "At least one of the errors was an exception type, " \
                        "the first exception being stored in the exception field."
         return ErrorDetail(message=message, exception=exception, more_data=errors)
 
     message += "There is no more information."
     return ErrorDetail(message=message)
+
+
+def is_func_valid(func):
+    """
+    Checks if a given input is a valid callable function or not.
+
+    :param func: The parameter `func` is expected to be a function object. The `is_func_valid` function checks if the `func`
+    parameter is not `None` and is callable (i.e., it can be called as a function). If both conditions are true, it returns
+    `True`
+    :return: Returns a boolean value. It returns `True` if the input `func` is not `None` and
+    is callable (i.e. can be called as a function), and `False` otherwise.
+    """
+    return func is not None and callable(func)
+
+
+def get_loop() -> AbstractEventLoop:
+    """
+    This function returns the current event loop or creates a new one if none exists in the current thread.
+
+    :return: Returns an instance of the `AbstractEventLoop` class, which is the event loop used by
+    asyncio for scheduling and executing coroutines and callbacks. If there is already an event loop running in the current
+    thread, it returns that event loop. Otherwise, it creates a new event loop, sets it as the current event loop for the
+    thread, and returns it.
+    """
+
+    try:
+        return asyncio.get_event_loop()
+    except RuntimeError as e:
+        if str(e).startswith('There is no current event loop in thread'):
+            loop = asyncio.new_event_loop()
+            asyncio.set_event_loop(loop)
+            return loop
+        raise  # pragma: no cover
```

### Comparing `on_rails-2.1.0/on_rails/decorator.py` & `on_rails-3.0.0/on_rails/decorator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Coroutine
 
 from on_rails._utility import await_func
-from on_rails.Result import Result
+from on_rails.Result import BreakRailsException, Result
 from on_rails.ResultDetails.Errors.ExceptionError import ExceptionError
 
 
 def def_result(is_async: bool = False):
     """
     A decorator that converts the output of a function into a Result, and can handle both
     synchronous and asynchronous functions.
@@ -18,22 +18,26 @@
     """
 
     def inner_decorator(func: callable):
         def wrapper(*args, **kwargs):
             try:
                 result = await_func(lambda: func(*args, **kwargs))
                 return Result.convert_to_result(result)
+            except BreakRailsException as e:
+                return e.result
             except Exception as e:
                 return Result.fail(detail=ExceptionError(message=str(e), exception=e))
 
         async def wrapper_async(*args, **kwargs):
             try:
                 result = func(*args, **kwargs)
                 if isinstance(result, Coroutine):
                     result = await result
                 return Result.convert_to_result(result)
+            except BreakRailsException as e:
+                return e.result
             except Exception as e:
                 return Result.fail(detail=ExceptionError(message=str(e), exception=e))
 
         return wrapper_async if is_async else wrapper
 
     return inner_decorator
```

### Comparing `on_rails-2.1.0/pyproject.toml` & `on_rails-3.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # https://python-poetry.org/docs/pyproject/
 [tool.poetry]
 name = "on_rails"
-version = "2.1.0"
+version = "3.0.0"
 description = "Simple and powerful Railway Oriented library for python"
 authors = ["Payadel <payadelteam@gmail.com>"]
 readme = "README.md"
 license = "GPLV3"
 repository = "https://github.com/Payadel/on_rails"
 keywords = ["railway oriented","functional programming", "error handling"]
 packages = [{ include = "on_rails" }]
```

### Comparing `on_rails-2.1.0/PKG-INFO` & `on_rails-3.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: on-rails
-Version: 2.1.0
+Version: 3.0.0
 Summary: Simple and powerful Railway Oriented library for python
 Home-page: https://github.com/Payadel/on_rails
 License: GPLV3
 Keywords: railway oriented,functional programming,error handling
 Author: Payadel
 Author-email: payadelteam@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -124,15 +124,15 @@
 by using functional programming concepts, developers can write code that is easier to reason about and understand, which
 can lead to faster development cycles and better quality code.
 
 ## Getting Started
 
 Use `pip` to install package:
 
-`pip install on_rails`
+`pip install on_rails --upgrade`
 
 ## Usage
 
 ### Sample 1
 
 ```python
 from on_rails import Result, def_result
@@ -140,16 +140,16 @@
 
 @def_result()
 def get_number() -> Result:
     number = int(input("Enter number: "))
     return Result.ok(number)
 
 
-get_number()\
-    .on_success(lambda prev: print(f"Number is valid: {prev.value}"))\
+get_number()
+    .on_success(lambda value: print(f"Number is valid: {value}"))
     .on_fail(lambda prev: print(prev.detail))
 ```
 
 Within the `get_number` function, the user is prompted to enter an integer number. If the user enters a valid integer,
 the number is returned as a successful result using `Result.ok()`, otherwise, an error message is returned as a failed
 result.
 
@@ -255,15 +255,15 @@
     return Result.ok(response.json(), detail)
 
 
 def fake_operation():
     return Result.ok()
 
 
-fake_operation().on_success(create_data, num_of_try=5)
+fake_operation().on_success(lambda: create_data(url, data), num_of_try=5)
 
 ```
 
 In the example above, if the request goes wrong, an **exception** will be raised. By setting `num_of_try`, you can
 specify how many times the operation should be repeated in case of an error.
 
 ### Sample 5: Async Decorator
```

