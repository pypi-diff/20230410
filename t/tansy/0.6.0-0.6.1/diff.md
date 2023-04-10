# Comparing `tmp/tansy-0.6.0.tar.gz` & `tmp/tansy-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tansy-0.6.0.tar", last modified: Mon Apr 10 18:47:48 2023, max compression
+gzip compressed data, was "tansy-0.6.1.tar", last modified: Mon Apr 10 19:58:43 2023, max compression
```

## Comparing `tansy-0.6.0.tar` & `tansy-0.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:47:48.498643 tansy-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-10 18:47:29.000000 tansy-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-10 18:47:48.498643 tansy-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-10 18:47:29.000000 tansy-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-10 18:47:29.000000 tansy-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 18:47:48.498643 tansy-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-10 18:47:29.000000 tansy-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:47:48.498643 tansy-0.6.0/tansy/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-10 18:47:29.000000 tansy-0.6.0/tansy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-04-10 18:47:29.000000 tansy-0.6.0/tansy/class_slash.py
--rw-r--r--   0 runner    (1001) docker     (123)    20034 2023-04-10 18:47:29.000000 tansy-0.6.0/tansy/slash_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-04-10 18:47:29.000000 tansy-0.6.0/tansy/slash_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-10 18:47:29.000000 tansy-0.6.0/tansy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:47:48.498643 tansy-0.6.0/tansy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-10 18:47:48.000000 tansy-0.6.0/tansy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-10 18:47:48.000000 tansy-0.6.0/tansy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:47:48.000000 tansy-0.6.0/tansy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-10 18:47:48.000000 tansy-0.6.0/tansy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 18:47:48.000000 tansy-0.6.0/tansy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:58:43.764072 tansy-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-10 19:58:30.000000 tansy-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-10 19:58:43.764072 tansy-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-10 19:58:30.000000 tansy-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-10 19:58:30.000000 tansy-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 19:58:43.764072 tansy-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-10 19:58:30.000000 tansy-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:58:43.764072 tansy-0.6.1/tansy/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-10 19:58:30.000000 tansy-0.6.1/tansy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-04-10 19:58:30.000000 tansy-0.6.1/tansy/class_slash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20405 2023-04-10 19:58:30.000000 tansy-0.6.1/tansy/slash_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-04-10 19:58:30.000000 tansy-0.6.1/tansy/slash_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-10 19:58:30.000000 tansy-0.6.1/tansy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:58:43.764072 tansy-0.6.1/tansy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-10 19:58:43.000000 tansy-0.6.1/tansy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-10 19:58:43.000000 tansy-0.6.1/tansy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:58:43.000000 tansy-0.6.1/tansy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-10 19:58:43.000000 tansy-0.6.1/tansy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 19:58:43.000000 tansy-0.6.1/tansy.egg-info/top_level.txt
```

### Comparing `tansy-0.6.0/LICENSE` & `tansy-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tansy-0.6.0/PKG-INFO` & `tansy-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tansy
-Version: 0.6.0
+Version: 0.6.1
 Summary: Unstable experiments with interactions.py.
 Home-page: https://github.com/Astrea49/tansy
 Author: AstreaTSS
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `tansy-0.6.0/README.md` & `tansy-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `tansy-0.6.0/setup.py` & `tansy-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 setup(
     name="tansy",
     description="Unstable experiments with interactions.py.",
     long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type="text/markdown",
     author="AstreaTSS",
     url="https://github.com/Astrea49/tansy",
-    version="0.6.0",
+    version="0.6.1",
     packages=find_packages(),
     python_requires=">=3.10",
     install_requires=requirements,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `tansy-0.6.0/tansy/__init__.py` & `tansy-0.6.1/tansy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Tansy
 Unstable experiments with interactions.py.
 :copyright: (c) 2022-present AstreaTSS
 :license: MIT, see LICENSE for more details.
 """
 
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 
 
 from .class_slash import *
 from .slash_commands import *
 from .slash_param import *
 
 __all__ = (
```

### Comparing `tansy-0.6.0/tansy/class_slash.py` & `tansy-0.6.1/tansy/class_slash.py`

 * *Files identical despite different names*

### Comparing `tansy-0.6.0/tansy/slash_commands.py` & `tansy-0.6.1/tansy/slash_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,30 +103,45 @@
     await new_func("hey!")
     ```
 
     Technically, it is possible to make a wrapper around a function that would handle those
     cases just fine, but that adds a lot of overhead, more than just using `partial` or doing this.
     """
     func_copy = copy.copy(func)
-    old_kwarg_defaults = func.__kwdefaults__ or {}
+    func_to_parse = func_copy
+
+    partial_func = False
+
+    if isinstance(func_copy, functools.partial):
+        func_to_parse = func_copy.func
+        partial_func = True
+
+    old_kwarg_defaults = func_to_parse.__kwdefaults__ or {}
 
     new_defaults = []
     new_kwarg_defaults = {}
 
     for name, default in defaults.items():
         if (
             old_kwarg_defaults.get(name)
             or parameters[name].kind == inspect._ParameterKind.KEYWORD_ONLY
         ):
             new_kwarg_defaults[name] = default
         else:
             new_defaults.append(default)
 
-    func_copy.__defaults__ = tuple(new_defaults) if new_defaults else None
-    func_copy.__kwdefaults__ = new_kwarg_defaults or None
+    func_to_parse.__defaults__ = tuple(new_defaults) if new_defaults else None
+    func_to_parse.__kwdefaults__ = new_kwarg_defaults or None
+
+    if partial_func:
+        func_copy = functools.partial(
+            func_to_parse, *func_copy.args, **func_copy.keywords
+        )
+    else:
+        func_copy = func_to_parse
 
     return func_copy
 
 
 @attrs.define(slots=True)
 class TansySlashCommandParameter:
     """An object representing parameters in a command."""
```

### Comparing `tansy-0.6.0/tansy/slash_param.py` & `tansy-0.6.1/tansy/slash_param.py`

 * *Files identical despite different names*

### Comparing `tansy-0.6.0/tansy/utils.py` & `tansy-0.6.1/tansy/utils.py`

 * *Files identical despite different names*

### Comparing `tansy-0.6.0/tansy.egg-info/PKG-INFO` & `tansy-0.6.1/tansy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tansy
-Version: 0.6.0
+Version: 0.6.1
 Summary: Unstable experiments with interactions.py.
 Home-page: https://github.com/Astrea49/tansy
 Author: AstreaTSS
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

