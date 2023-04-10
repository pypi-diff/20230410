# Comparing `tmp/tkreform-0.3.0.tar.gz` & `tmp/tkreform-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkreform-0.3.0.tar", last modified: Mon Apr 10 15:18:49 2023, max compression
+gzip compressed data, was "tkreform-0.3.1.tar", last modified: Mon Apr 10 16:27:48 2023, max compression
```

## Comparing `tkreform-0.3.0.tar` & `tkreform-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:49.643422 tkreform-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-10 15:18:46.000000 tkreform-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-10 15:18:49.643422 tkreform-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-10 15:18:46.000000 tkreform-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 15:18:49.643422 tkreform-0.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1035 2023-04-10 15:18:46.000000 tkreform-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:49.639422 tkreform-0.3.0/tkreform/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-10 15:18:46.000000 tkreform-0.3.0/tkreform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18527 2023-04-10 15:18:46.000000 tkreform-0.3.0/tkreform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-10 15:18:46.000000 tkreform-0.3.0/tkreform/declarative.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-10 15:18:46.000000 tkreform-0.3.0/tkreform/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-10 15:18:46.000000 tkreform-0.3.0/tkreform/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-10 15:18:46.000000 tkreform-0.3.0/tkreform/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-10 15:18:46.000000 tkreform-0.3.0/tkreform/linguist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-10 15:18:46.000000 tkreform-0.3.0/tkreform/menu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:49.643422 tkreform-0.3.0/tkreform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-10 15:18:49.000000 tkreform-0.3.0/tkreform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-10 15:18:49.000000 tkreform-0.3.0/tkreform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:18:49.000000 tkreform-0.3.0/tkreform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-10 15:18:49.000000 tkreform-0.3.0/tkreform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 15:18:49.000000 tkreform-0.3.0/tkreform.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:27:48.893890 tkreform-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-10 16:27:43.000000 tkreform-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-10 16:27:48.893890 tkreform-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-10 16:27:43.000000 tkreform-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 16:27:48.893890 tkreform-0.3.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1035 2023-04-10 16:27:43.000000 tkreform-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:27:48.893890 tkreform-0.3.1/tkreform/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-10 16:27:43.000000 tkreform-0.3.1/tkreform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18527 2023-04-10 16:27:43.000000 tkreform-0.3.1/tkreform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-10 16:27:43.000000 tkreform-0.3.1/tkreform/declarative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-10 16:27:43.000000 tkreform-0.3.1/tkreform/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-10 16:27:43.000000 tkreform-0.3.1/tkreform/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-10 16:27:43.000000 tkreform-0.3.1/tkreform/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-10 16:27:43.000000 tkreform-0.3.1/tkreform/linguist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-10 16:27:43.000000 tkreform-0.3.1/tkreform/menu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:27:48.893890 tkreform-0.3.1/tkreform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-10 16:27:48.000000 tkreform-0.3.1/tkreform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-10 16:27:48.000000 tkreform-0.3.1/tkreform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:27:48.000000 tkreform-0.3.1/tkreform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-10 16:27:48.000000 tkreform-0.3.1/tkreform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 16:27:48.000000 tkreform-0.3.1/tkreform.egg-info/top_level.txt
```

### Comparing `tkreform-0.3.0/LICENSE` & `tkreform-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.0/PKG-INFO` & `tkreform-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkreform
-Version: 0.3.0
+Version: 0.3.1
 Summary: Reformed tkinter coding tool.
 Home-page: https://github.com/tkinguist/tkreform
 Author: HivertMoZara
 Author-email: worldmozara@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tkreform-0.3.0/setup.py` & `tkreform-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.0/tkreform/__init__.py` & `tkreform-0.3.1/tkreform/__init__.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.0/tkreform/base.py` & `tkreform-0.3.1/tkreform/base.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.0/tkreform/declarative.py` & `tkreform-0.3.1/tkreform/declarative.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 Direction = Literal["n", "ne", "e", "se", "s", "sw", "w", "nw"]
+Compound = Literal["top", "left", "center", "right", "bottom", "none"]
 
 
 @dataclass
 class Gridder:
     column: Optional[int] = None
     columnspan: Optional[int] = None
     in_: Optional[Union[WidgetType, WindowType]] = None
@@ -94,15 +95,15 @@
 @dataclass
 class NotebookAdder:
     state: Literal["normal", "disabled", "hidden"] = "normal"
     sticky: Optional[Direction] = None
     padding: ttk._Padding = (0, 0)
     text: str = ""
     image: Any = None
-    compound: _Compound = "none"
+    compound: Compound = "none"
     underline: int = 0
 
 
 class W:
     """Widget data pre-storage."""
     def __init__(self, widget: Type[WidgetType], **kwargs: Any) -> None:
         self.widget = widget
```

### Comparing `tkreform-0.3.0/tkreform/events.py` & `tkreform-0.3.1/tkreform/events.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.0/tkreform/groups.py` & `tkreform-0.3.1/tkreform/groups.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.0/tkreform/linguist.py` & `tkreform-0.3.1/tkreform/linguist.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.0/tkreform/menu.py` & `tkreform-0.3.1/tkreform/menu.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.0/tkreform.egg-info/PKG-INFO` & `tkreform-0.3.1/tkreform.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkreform
-Version: 0.3.0
+Version: 0.3.1
 Summary: Reformed tkinter coding tool.
 Home-page: https://github.com/tkinguist/tkreform
 Author: HivertMoZara
 Author-email: worldmozara@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

