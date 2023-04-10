# Comparing `tmp/tkreform-0.3.2.tar.gz` & `tmp/tkreform-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkreform-0.3.2.tar", last modified: Mon Apr 10 16:35:05 2023, max compression
+gzip compressed data, was "tkreform-0.3.3.tar", last modified: Mon Apr 10 16:49:41 2023, max compression
```

## Comparing `tkreform-0.3.2.tar` & `tkreform-0.3.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:35:05.297644 tkreform-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-10 16:35:02.000000 tkreform-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-10 16:35:05.297644 tkreform-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-10 16:35:02.000000 tkreform-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 16:35:05.297644 tkreform-0.3.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1035 2023-04-10 16:35:02.000000 tkreform-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:35:05.297644 tkreform-0.3.2/tkreform/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-10 16:35:02.000000 tkreform-0.3.2/tkreform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18527 2023-04-10 16:35:02.000000 tkreform-0.3.2/tkreform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-04-10 16:35:02.000000 tkreform-0.3.2/tkreform/declarative.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-10 16:35:02.000000 tkreform-0.3.2/tkreform/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-10 16:35:02.000000 tkreform-0.3.2/tkreform/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-10 16:35:02.000000 tkreform-0.3.2/tkreform/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-10 16:35:02.000000 tkreform-0.3.2/tkreform/linguist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-10 16:35:02.000000 tkreform-0.3.2/tkreform/menu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:35:05.297644 tkreform-0.3.2/tkreform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-10 16:35:05.000000 tkreform-0.3.2/tkreform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-10 16:35:05.000000 tkreform-0.3.2/tkreform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:35:05.000000 tkreform-0.3.2/tkreform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-10 16:35:05.000000 tkreform-0.3.2/tkreform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 16:35:05.000000 tkreform-0.3.2/tkreform.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:49:41.970293 tkreform-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-10 16:49:36.000000 tkreform-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-10 16:49:41.970293 tkreform-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-10 16:49:36.000000 tkreform-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 16:49:41.970293 tkreform-0.3.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1035 2023-04-10 16:49:36.000000 tkreform-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:49:41.970293 tkreform-0.3.3/tkreform/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-10 16:49:36.000000 tkreform-0.3.3/tkreform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18527 2023-04-10 16:49:36.000000 tkreform-0.3.3/tkreform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-10 16:49:36.000000 tkreform-0.3.3/tkreform/declarative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-10 16:49:36.000000 tkreform-0.3.3/tkreform/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-10 16:49:36.000000 tkreform-0.3.3/tkreform/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-10 16:49:36.000000 tkreform-0.3.3/tkreform/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-10 16:49:36.000000 tkreform-0.3.3/tkreform/linguist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-10 16:49:36.000000 tkreform-0.3.3/tkreform/menu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:49:41.970293 tkreform-0.3.3/tkreform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-10 16:49:41.000000 tkreform-0.3.3/tkreform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-10 16:49:41.000000 tkreform-0.3.3/tkreform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:49:41.000000 tkreform-0.3.3/tkreform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-10 16:49:41.000000 tkreform-0.3.3/tkreform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 16:49:41.000000 tkreform-0.3.3/tkreform.egg-info/top_level.txt
```

### Comparing `tkreform-0.3.2/LICENSE` & `tkreform-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.2/PKG-INFO` & `tkreform-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkreform
-Version: 0.3.2
+Version: 0.3.3
 Summary: Reformed tkinter coding tool.
 Home-page: https://github.com/tkinguist/tkreform
 Author: HivertMoZara
 Author-email: worldmozara@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tkreform-0.3.2/setup.py` & `tkreform-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.2/tkreform/__init__.py` & `tkreform-0.3.3/tkreform/__init__.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.2/tkreform/base.py` & `tkreform-0.3.3/tkreform/base.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.2/tkreform/declarative.py` & `tkreform-0.3.3/tkreform/declarative.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 >>> window.loop()
 """
 
 from dataclasses import dataclass
 import sys
 import tkinter as tk
 from tkinter import ttk, Menu
-from typing import TYPE_CHECKING, Any, Iterable, Optional, Type, Union
+from typing import TYPE_CHECKING, Any, Iterable, Optional, Tuple, Type, Union
 
 from tkreform.menu import MenuItem
 
 if TYPE_CHECKING:
     from tkreform.base import Window
 
 WidgetType = Union[tk.Widget, ttk.Widget]
@@ -37,15 +37,16 @@
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 Direction = Literal["n", "ne", "e", "se", "s", "sw", "w", "nw"]
 Compound = Literal["top", "left", "center", "right", "bottom", "none"]
-
+LiteralFloat = Union[str, float]
+Padding = Union[LiteralFloat, Tuple[LiteralFloat, ...]]
 
 @dataclass
 class Gridder:
     column: Optional[int] = None
     columnspan: Optional[int] = None
     in_: Optional[Union[WidgetType, WindowType]] = None
     ipadx: Optional[int] = None
@@ -92,15 +93,15 @@
     win: Optional["Window"] = None
 
 
 @dataclass
 class NotebookAdder:
     state: Literal["normal", "disabled", "hidden"] = "normal"
     sticky: Optional[Direction] = None
-    padding: ttk._Padding = (0, 0)
+    padding: Padding = (0, 0)
     text: str = ""
     image: Any = None
     compound: Compound = "none"
     underline: int = 0
 
 
 class W:
```

### Comparing `tkreform-0.3.2/tkreform/events.py` & `tkreform-0.3.3/tkreform/events.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.2/tkreform/groups.py` & `tkreform-0.3.3/tkreform/groups.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.2/tkreform/linguist.py` & `tkreform-0.3.3/tkreform/linguist.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.2/tkreform/menu.py` & `tkreform-0.3.3/tkreform/menu.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.2/tkreform.egg-info/PKG-INFO` & `tkreform-0.3.3/tkreform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkreform
-Version: 0.3.2
+Version: 0.3.3
 Summary: Reformed tkinter coding tool.
 Home-page: https://github.com/tkinguist/tkreform
 Author: HivertMoZara
 Author-email: worldmozara@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

