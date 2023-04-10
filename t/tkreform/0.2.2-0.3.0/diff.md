# Comparing `tmp/tkreform-0.2.2.tar.gz` & `tmp/tkreform-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkreform-0.2.2.tar", last modified: Sat Nov 12 10:05:12 2022, max compression
+gzip compressed data, was "tkreform-0.3.0.tar", last modified: Mon Apr 10 15:18:49 2023, max compression
```

## Comparing `tkreform-0.2.2.tar` & `tkreform-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 10:05:12.488796 tkreform-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-11-12 10:05:08.000000 tkreform-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-11-12 10:05:12.488796 tkreform-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-11-12 10:05:08.000000 tkreform-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-12 10:05:12.488796 tkreform-0.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1035 2022-11-12 10:05:08.000000 tkreform-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 10:05:12.488796 tkreform-0.2.2/tkreform/
--rw-r--r--   0 runner    (1001) docker     (121)      966 2022-11-12 10:05:08.000000 tkreform-0.2.2/tkreform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17797 2022-11-12 10:05:08.000000 tkreform-0.2.2/tkreform/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3157 2022-11-12 10:05:08.000000 tkreform-0.2.2/tkreform/declarative.py
--rw-r--r--   0 runner    (1001) docker     (121)     2355 2022-11-12 10:05:08.000000 tkreform-0.2.2/tkreform/events.py
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-11-12 10:05:08.000000 tkreform-0.2.2/tkreform/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2001 2022-11-12 10:05:08.000000 tkreform-0.2.2/tkreform/groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     2266 2022-11-12 10:05:08.000000 tkreform-0.2.2/tkreform/linguist.py
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-11-12 10:05:08.000000 tkreform-0.2.2/tkreform/menu.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 10:05:12.488796 tkreform-0.2.2/tkreform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-11-12 10:05:12.000000 tkreform-0.2.2/tkreform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-11-12 10:05:12.000000 tkreform-0.2.2/tkreform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-12 10:05:12.000000 tkreform-0.2.2/tkreform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-11-12 10:05:12.000000 tkreform-0.2.2/tkreform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-12 10:05:12.000000 tkreform-0.2.2/tkreform.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:49.643422 tkreform-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-10 15:18:46.000000 tkreform-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-10 15:18:49.643422 tkreform-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-10 15:18:46.000000 tkreform-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 15:18:49.643422 tkreform-0.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1035 2023-04-10 15:18:46.000000 tkreform-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:49.639422 tkreform-0.3.0/tkreform/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-10 15:18:46.000000 tkreform-0.3.0/tkreform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18527 2023-04-10 15:18:46.000000 tkreform-0.3.0/tkreform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-10 15:18:46.000000 tkreform-0.3.0/tkreform/declarative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-10 15:18:46.000000 tkreform-0.3.0/tkreform/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-10 15:18:46.000000 tkreform-0.3.0/tkreform/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-10 15:18:46.000000 tkreform-0.3.0/tkreform/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-10 15:18:46.000000 tkreform-0.3.0/tkreform/linguist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-10 15:18:46.000000 tkreform-0.3.0/tkreform/menu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:49.643422 tkreform-0.3.0/tkreform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-10 15:18:49.000000 tkreform-0.3.0/tkreform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-10 15:18:49.000000 tkreform-0.3.0/tkreform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:18:49.000000 tkreform-0.3.0/tkreform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-10 15:18:49.000000 tkreform-0.3.0/tkreform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 15:18:49.000000 tkreform-0.3.0/tkreform.egg-info/top_level.txt
```

### Comparing `tkreform-0.2.2/LICENSE` & `tkreform-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tkreform-0.2.2/PKG-INFO` & `tkreform-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkreform
-Version: 0.2.2
+Version: 0.3.0
 Summary: Reformed tkinter coding tool.
 Home-page: https://github.com/tkinguist/tkreform
 Author: HivertMoZara
 Author-email: worldmozara@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tkreform-0.2.2/setup.py` & `tkreform-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.2.2/tkreform/__init__.py` & `tkreform-0.3.0/tkreform/__init__.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.2.2/tkreform/base.py` & `tkreform-0.3.0/tkreform/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,43 +4,42 @@
 from tkinter import TclError, ttk
 
 from tkreform.exceptions import MessageNotFound, WidgetNotArranged
 from tkreform.linguist import Linguist
 from tkreform.menu import MenuItem
 from . import declarative as dec
 from typing import (
-    Any, Callable, Iterable, List, Optional, Tuple, Type, TypeVar, Union,
+    Any, Callable, Generic, Iterable, List, Optional, Tuple, Type, TypeVar, Union, cast,
     overload
 )
 
 # use Literal type
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 # attempt to use PIL
 try:
-    from PIL.Image import Image
     from PIL.ImageTk import PhotoImage
     HAS_PIL = True
 except ImportError:
     from tkinter import PhotoImage
-    Image = object
     HAS_PIL = False
 
 WidgetType = Union[tk.Widget, ttk.Widget]
 WindowType = Union[tk.Tk, tk.Toplevel]
 HasText = Union[tk.Label, tk.Button, ttk.Label, ttk.Button, tk.Message]
 
-_T = TypeVar("_T", WidgetType, WindowType)
-_WidgetT = TypeVar("_WidgetT", tk.Widget, ttk.Widget)
+_T = TypeVar("_T", bound=Union[WidgetType, WindowType])
+_WidgetT = TypeVar("_WidgetT", bound=WidgetType)
+_WindowT = TypeVar("_WindowT", bound=WindowType)
 
 
-class _Base(metaclass=ABCMeta):
+class _Base(Generic[_T], metaclass=ABCMeta):
     def __init__(self, base: _T) -> None:
         """
         Base type of Window / Widget.
 
         - base: `WindowType | WidgetType` - base window / widget type
         """
         self.base = base
@@ -57,14 +56,17 @@
 
     def __getitem__(self, it: Union[int, slice]):
         return self._sub_widget[it]
 
     def __setitem__(self, it: int, val: "Widget"):
         self._sub_widget[it] = val
 
+    def __iter__(self):
+        return iter(self._sub_widget)
+
     def on(self, seq: str, append: bool = False):
         """
         Register response function on event sequence.
 
         - seq: `str` - event sequence
         - append: `bool` - decide to override or append function to target
 
@@ -77,15 +79,15 @@
         ...     ...
         """
         def __wrapper(func: Callable[[tk.Event], Any]):
             self.base.bind(seq, func, append)
             return func
         return __wrapper
 
-    def add_widget(self, sw: Type[WidgetType], *args, **kwargs):
+    def add_widget(self, sw: Type[_WidgetT], *args, **kwargs) -> "Widget[_WidgetT]":
         """
         Add a widget to window / widget.
 
         - sw: `Type[WidgetType]` - type of sub widget
         - *args, **kwargs - arguments for sub widget
 
         Returns: `Widget`
@@ -107,14 +109,20 @@
             else:
                 _widget = self.add_widget(w.widget, **w.kwargs)
                 _widget.linguist = self.linguist
                 if isinstance(self.base, tk.Menu) and isinstance(w, dec.M):
                     self.base.add(w.it.type, menu=_widget.base, **w.it.data)
                 elif isinstance(self.base, tk.PanedWindow):
                     self.base.add(_widget.base)
+                elif isinstance(self.base, ttk.Notebook):
+                    w.controller = cast(dec.NotebookAdder, w.controller)
+                    self.base.add(
+                        _widget.base,
+                        **{k: getattr(w.controller, k) for k in w.controller.__dataclass_fields__}
+                    )
                 _widget.load_sub(w.sub)
                 if w.controller is not None:
                     _widget.apply(w.controller)
 
     def __truediv__(self, other: Iterable[Union[dec.W, MenuItem]]):
         for old in self._sub_widget:
             old.destroy()
@@ -136,18 +144,20 @@
 
     @linguist.setter
     def linguist(self, _l: Optional[Linguist]):
         self._linguist = _l
         self.update_translation()
 
 
-class Widget(_Base):
+class Widget(_Base, Generic[_WidgetT]):
     """
     Reformed Widget type based on `tkinter`.
     """
+    base: _WidgetT
+
     def __init__(self, widget: _WidgetT) -> None:
         # To keep the content image alive, here gives a slot to add a
         # reference to the image so that the image wouldn't be recycled by GC
         # at the moment the image adder finishes its work.
         self._image_slot = None
         super().__init__(widget)
         self.base = widget
@@ -234,15 +244,15 @@
         """
         self.base["command"] = func
         return func
 
     command = callback
 
     def apply(
-        self, geo: Union[dec.Gridder, dec.Packer, dec.Placer, dec.MenuBinder]
+        self, geo: Union[dec.Gridder, dec.Packer, dec.Placer, dec.MenuBinder, dec.NotebookAdder]
     ):
         if isinstance(geo, dec.Gridder):
             self.grid(
                 column=geo.column, columnspan=geo.columnspan,
                 in_=geo.in_, ipadx=geo.ipadx, ipady=geo.ipady,
                 padx=geo.padx, pady=geo.pady,
                 row=geo.row, rowspan=geo.rowspan, sticky=geo.sticky
@@ -260,14 +270,16 @@
                 anchor=geo.anchor, width=geo.width, height=geo.height,
                 relwidth=geo.relwidth, relheight=geo.relheight,
                 bordermode=geo.bordermode, in_=geo.in_
             )
         elif isinstance(geo, dec.MenuBinder):
             if geo.win is not None:
                 geo.win.menu = self.base
+        elif isinstance(geo, dec.NotebookAdder):
+            ...
         else:
             raise WidgetNotArranged(
                 f"widget '{self.base}' has not been arranged by gridder, "
                 "packer or placer."
             )
 
     def sync(self):
@@ -304,22 +316,16 @@
 
     @property
     def image(self) -> PhotoImage:  # type: ignore
         """The image of the widget."""
         return self.base["image"]
 
     @image.setter
-    def image(self, img: Union[str, Image, PhotoImage]):  # type: ignore
-        _img = (
-            PhotoImage(file=img)
-            if isinstance(img, str) else
-            PhotoImage(img)  # type: ignore
-            if isinstance(img, Image) and HAS_PIL else
-            img
-        )
+    def image(self, img: Union[str, PhotoImage]):  # type: ignore
+        _img = (PhotoImage(file=img) if isinstance(img, str) else img)
         self._image_slot = _img
         self.base["image"] = _img
 
     @property
     def width(self) -> int:
         """The width of the widget."""
         return self.base["width"]
@@ -360,21 +366,21 @@
         return self.base["state"] == "disabled"
 
     @disabled.setter
     def disabled(self, st: bool):
         self.base["state"] = "disabled" if st else "normal"
 
 
-class Window(_Base):
+class Window(_Base, Generic[_WindowT]):
     """
     Reformed Window type based on `tkinter`.
     """
-    base: WindowType
+    base: _WindowT
 
-    def __init__(self, base: WindowType) -> None:
+    def __init__(self, base: _WindowT) -> None:
         """
         Initialize a new window.
 
         - base: `tk.Tk | tk.Toplevel` - base window type
         """
         super().__init__(base)
         self._raw_title = self.title
@@ -387,15 +393,15 @@
 
     def sub_window(self):
         """
         Create a sub window.
 
         Returns: `tk.Toplevel`
         """
-        sub = type(self)(tk.Toplevel(self.base))
+        sub = Window(tk.Toplevel(self.base))
         return sub
 
     def update(self):
         """Update window."""
         self.base.update()
 
     def wmhide(self):
@@ -595,7 +601,17 @@
     @property
     def menu(self):
         return self.base["menu"]
 
     @menu.setter
     def menu(self, m):
         self.base["menu"] = m
+
+
+class Application(Generic[_WindowT], metaclass=ABCMeta):
+    def __init__(self, base: Union[_WindowT, Window[_WindowT]]) -> None:
+        self.win = base if isinstance(base, Window) else Window(base)
+        self.setup()
+
+    @abstractmethod
+    def setup(self) -> None:
+        raise NotImplementedError
```

### Comparing `tkreform-0.2.2/tkreform/declarative.py` & `tkreform-0.3.0/tkreform/declarative.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 >>> window[0][1].callback(window.destroy)
 >>> window.loop()
 """
 
 from dataclasses import dataclass
 import sys
 import tkinter as tk
-from tkinter import ttk, Menu
+from tkinter import _Compound, ttk, Menu
 from typing import TYPE_CHECKING, Any, Iterable, Optional, Type, Union
 
 from tkreform.menu import MenuItem
 
 if TYPE_CHECKING:
     from tkreform.base import Window
 
@@ -87,23 +87,34 @@
 
 
 @dataclass
 class MenuBinder:
     win: Optional["Window"] = None
 
 
+@dataclass
+class NotebookAdder:
+    state: Literal["normal", "disabled", "hidden"] = "normal"
+    sticky: Optional[Direction] = None
+    padding: ttk._Padding = (0, 0)
+    text: str = ""
+    image: Any = None
+    compound: _Compound = "none"
+    underline: int = 0
+
+
 class W:
     """Widget data pre-storage."""
     def __init__(self, widget: Type[WidgetType], **kwargs: Any) -> None:
         self.widget = widget
         self.kwargs = kwargs
         self.controller = None
         self.sub: Iterable[Union["W", MenuItem]] = ()
 
-    def __mul__(self, other: Union[Gridder, Packer, Placer, MenuBinder]):
+    def __mul__(self, other: Union[Gridder, Packer, Placer, MenuBinder, NotebookAdder]):
         self.controller = other
         return self
 
     def __truediv__(self, other: Iterable[Union["W", MenuItem]]):
         self.sub = other
         return self
```

### Comparing `tkreform-0.2.2/tkreform/events.py` & `tkreform-0.3.0/tkreform/events.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.2.2/tkreform/groups.py` & `tkreform-0.3.0/tkreform/groups.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.2.2/tkreform/linguist.py` & `tkreform-0.3.0/tkreform/linguist.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.2.2/tkreform/menu.py` & `tkreform-0.3.0/tkreform/menu.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.2.2/tkreform.egg-info/PKG-INFO` & `tkreform-0.3.0/tkreform.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkreform
-Version: 0.2.2
+Version: 0.3.0
 Summary: Reformed tkinter coding tool.
 Home-page: https://github.com/tkinguist/tkreform
 Author: HivertMoZara
 Author-email: worldmozara@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

