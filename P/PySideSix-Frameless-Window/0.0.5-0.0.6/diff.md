# Comparing `tmp/PySideSix-Frameless-Window-0.0.5.tar.gz` & `tmp/PySideSix-Frameless-Window-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySideSix-Frameless-Window-0.0.5.tar", last modified: Tue Mar 28 03:30:55 2023, max compression
+gzip compressed data, was "dist\PySideSix-Frameless-Window-0.0.6.tar", last modified: Mon Apr 10 14:42:55 2023, max compression
```

## Comparing `PySideSix-Frameless-Window-0.0.5.tar` & `PySideSix-Frameless-Window-0.0.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 03:30:55.561923 PySideSix-Frameless-Window-0.0.5/
--rw-rw-rw-   0        0        0     7815 2023-03-28 03:25:25.000000 PySideSix-Frameless-Window-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     5519 2023-03-28 03:30:55.560241 PySideSix-Frameless-Window-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-28 03:30:55.520563 PySideSix-Frameless-Window-0.0.5/PySideSix_Frameless_Window.egg-info/
--rw-rw-rw-   0        0        0     5519 2023-03-28 03:30:55.000000 PySideSix-Frameless-Window-0.0.5/PySideSix_Frameless_Window.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      868 2023-03-28 03:30:55.000000 PySideSix-Frameless-Window-0.0.5/PySideSix_Frameless_Window.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 03:30:55.000000 PySideSix-Frameless-Window-0.0.5/PySideSix_Frameless_Window.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-03-28 03:30:55.000000 PySideSix-Frameless-Window-0.0.5/PySideSix_Frameless_Window.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-03-28 03:30:55.000000 PySideSix-Frameless-Window-0.0.5/PySideSix_Frameless_Window.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4927 2023-03-28 03:28:49.000000 PySideSix-Frameless-Window-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-28 03:30:55.524751 PySideSix-Frameless-Window-0.0.5/qframelesswindow/
--rw-rw-rw-   0        0        0     2280 2023-03-28 03:26:47.000000 PySideSix-Frameless-Window-0.0.5/qframelesswindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:30:55.527909 PySideSix-Frameless-Window-0.0.5/qframelesswindow/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PySideSix-Frameless-Window-0.0.5/qframelesswindow/_rc/__init__.py
--rw-rw-rw-   0        0        0     1477 2023-03-28 03:25:13.000000 PySideSix-Frameless-Window-0.0.5/qframelesswindow/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:30:55.532822 PySideSix-Frameless-Window-0.0.5/qframelesswindow/linux/
--rw-rw-rw-   0        0        0     2878 2023-03-28 03:25:13.000000 PySideSix-Frameless-Window-0.0.5/qframelesswindow/linux/__init__.py
--rw-rw-rw-   0        0        0     2918 2023-03-28 03:25:13.000000 PySideSix-Frameless-Window-0.0.5/qframelesswindow/linux/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:30:55.537214 PySideSix-Frameless-Window-0.0.5/qframelesswindow/mac/
--rw-rw-rw-   0        0        0     3024 2023-03-28 03:25:13.000000 PySideSix-Frameless-Window-0.0.5/qframelesswindow/mac/__init__.py
--rw-rw-rw-   0        0        0     4320 2023-03-28 03:25:13.000000 PySideSix-Frameless-Window-0.0.5/qframelesswindow/mac/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:30:55.541619 PySideSix-Frameless-Window-0.0.5/qframelesswindow/titlebar/
--rw-rw-rw-   0        0        0     5062 2023-03-28 03:25:13.000000 PySideSix-Frameless-Window-0.0.5/qframelesswindow/titlebar/__init__.py
--rw-rw-rw-   0        0        0     9039 2023-03-28 03:25:13.000000 PySideSix-Frameless-Window-0.0.5/qframelesswindow/titlebar/title_bar_buttons.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:30:55.551221 PySideSix-Frameless-Window-0.0.5/qframelesswindow/utils/
--rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PySideSix-Frameless-Window-0.0.5/qframelesswindow/utils/__init__.py
--rw-rw-rw-   0        0        0     1216 2023-03-28 03:25:13.000000 PySideSix-Frameless-Window-0.0.5/qframelesswindow/utils/linux_utils.py
--rw-rw-rw-   0        0        0     1844 2023-03-28 03:25:13.000000 PySideSix-Frameless-Window-0.0.5/qframelesswindow/utils/mac_utils.py
--rw-rw-rw-   0        0        0     7143 2023-03-28 03:25:13.000000 PySideSix-Frameless-Window-0.0.5/qframelesswindow/utils/win32_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:30:55.556591 PySideSix-Frameless-Window-0.0.5/qframelesswindow/windows/
--rw-rw-rw-   0        0        0     6651 2023-03-28 03:25:13.000000 PySideSix-Frameless-Window-0.0.5/qframelesswindow/windows/__init__.py
--rw-rw-rw-   0        0        0     4261 2023-03-28 03:25:13.000000 PySideSix-Frameless-Window-0.0.5/qframelesswindow/windows/c_structures.py
--rw-rw-rw-   0        0        0     8905 2023-03-28 03:25:13.000000 PySideSix-Frameless-Window-0.0.5/qframelesswindow/windows/window_effect.py
--rw-rw-rw-   0        0        0       42 2023-03-28 03:30:55.561923 PySideSix-Frameless-Window-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1003 2023-03-28 03:26:30.000000 PySideSix-Frameless-Window-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:42:55.264169 PySideSix-Frameless-Window-0.0.6/
+-rw-rw-rw-   0        0        0     7815 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     5519 2023-04-10 14:42:55.261655 PySideSix-Frameless-Window-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 14:42:55.216259 PySideSix-Frameless-Window-0.0.6/PySideSix_Frameless_Window.egg-info/
+-rw-rw-rw-   0        0        0     5519 2023-04-10 14:42:54.000000 PySideSix-Frameless-Window-0.0.6/PySideSix_Frameless_Window.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      868 2023-04-10 14:42:55.000000 PySideSix-Frameless-Window-0.0.6/PySideSix_Frameless_Window.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 14:42:54.000000 PySideSix-Frameless-Window-0.0.6/PySideSix_Frameless_Window.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-04-10 14:42:54.000000 PySideSix-Frameless-Window-0.0.6/PySideSix_Frameless_Window.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-10 14:42:54.000000 PySideSix-Frameless-Window-0.0.6/PySideSix_Frameless_Window.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4927 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 14:42:55.223871 PySideSix-Frameless-Window-0.0.6/qframelesswindow/
+-rw-rw-rw-   0        0        0     1614 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:42:55.225068 PySideSix-Frameless-Window-0.0.6/qframelesswindow/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/_rc/__init__.py
+-rw-rw-rw-   0        0        0     1477 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:42:55.231841 PySideSix-Frameless-Window-0.0.6/qframelesswindow/linux/
+-rw-rw-rw-   0        0        0     4320 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/linux/__init__.py
+-rw-rw-rw-   0        0        0     2918 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/linux/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:42:55.231841 PySideSix-Frameless-Window-0.0.6/qframelesswindow/mac/
+-rw-rw-rw-   0        0        0     4529 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/mac/__init__.py
+-rw-rw-rw-   0        0        0     4320 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/mac/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:42:55.240337 PySideSix-Frameless-Window-0.0.6/qframelesswindow/titlebar/
+-rw-rw-rw-   0        0        0     5062 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/titlebar/__init__.py
+-rw-rw-rw-   0        0        0     9039 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/titlebar/title_bar_buttons.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:42:55.247404 PySideSix-Frameless-Window-0.0.6/qframelesswindow/utils/
+-rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/utils/__init__.py
+-rw-rw-rw-   0        0        0     1216 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/utils/linux_utils.py
+-rw-rw-rw-   0        0        0     1844 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/utils/mac_utils.py
+-rw-rw-rw-   0        0        0     7143 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/utils/win32_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:42:55.259186 PySideSix-Frameless-Window-0.0.6/qframelesswindow/windows/
+-rw-rw-rw-   0        0        0     8180 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/windows/__init__.py
+-rw-rw-rw-   0        0        0     4261 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/windows/c_structures.py
+-rw-rw-rw-   0        0        0     8905 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/windows/window_effect.py
+-rw-rw-rw-   0        0        0       42 2023-04-10 14:42:55.264169 PySideSix-Frameless-Window-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/setup.py
```

### Comparing `PySideSix-Frameless-Window-0.0.5/LICENSE` & `PySideSix-Frameless-Window-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.5/PKG-INFO` & `PySideSix-Frameless-Window-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySideSix-Frameless-Window
-Version: 0.0.5
+Version: 0.0.6
 Summary: A cross-platform frameless window based on pyside6, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PySide6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: LGPLv3
 Keywords: pyside6 frameless
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PySideSix-Frameless-Window-0.0.5/PySideSix_Frameless_Window.egg-info/PKG-INFO` & `PySideSix-Frameless-Window-0.0.6/PySideSix_Frameless_Window.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySideSix-Frameless-Window
-Version: 0.0.5
+Version: 0.0.6
 Summary: A cross-platform frameless window based on pyside6, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PySide6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: LGPLv3
 Keywords: pyside6 frameless
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PySideSix-Frameless-Window-0.0.5/PySideSix_Frameless_Window.egg-info/SOURCES.txt` & `PySideSix-Frameless-Window-0.0.6/PySideSix_Frameless_Window.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.5/README.md` & `PySideSix-Frameless-Window-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.5/qframelesswindow/__init__.py` & `PySideSix-Frameless-Window-0.0.6/qframelesswindow/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,67 +8,36 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PySide6/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: LGPLv3, see LICENSE for more details.
 """
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 
 import sys
 
 from PySide6.QtCore import Qt
 from PySide6.QtWidgets import QDialog, QMainWindow
 
 from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar
 
 if sys.platform == "win32":
-    from .windows import AcrylicWindow as AcrylicWindowBase
-    from .windows import WindowsFramelessWindow as FramelessWindowBase
+    from .windows import AcrylicWindow
+    from .windows import WindowsFramelessWindow as FramelessWindow
+    from .windows import WindowsFramelessMainWindow as FramelessMainWindow
+    from .windows import WindowsFramelessDialog as FramelessDialog
     from .windows import WindowsWindowEffect as WindowEffect
 elif sys.platform == "darwin":
-    from .mac import AcrylicWindow as AcrylicWindowBase
-    from .mac import MacFramelessWindow as FramelessWindowBase
+    from .mac import AcrylicWindow
+    from .mac import MacFramelessWindow as FramelessWindow
+    from .mac import MacFramelessMainWindow as FramelessMainWindow
+    from .mac import MacFramelessDialog as FramelessDialog
     from .mac import MacWindowEffect as WindowEffect
 else:
-    from .linux import LinuxFramelessWindow as FramelessWindowBase
+    from .linux import LinuxFramelessWindow as FramelessWindow
+    from .linux import LinuxFramelessMainWindow as FramelessMainWindow
+    from .linux import LinuxFramelessDialog as FramelessDialog
     from .linux import LinuxWindowEffect as WindowEffect
 
-    AcrylicWindowBase = FramelessWindowBase
+    AcrylicWindow = FramelessWindow
 
-
-class FramelessWindow(FramelessWindowBase):
-    """ Frameless window """
-
-    def __init__(self, parent=None):
-        super().__init__(parent=parent)
-        self._initFrameless()
-
-
-class FramelessDialog(QDialog, FramelessWindowBase):
-    """ Frameless dialog """
-
-    def __init__(self, parent=None):
-        super().__init__(parent=parent)
-        self._initFrameless()
-        self.titleBar.minBtn.hide()
-        self.titleBar.maxBtn.hide()
-        self.titleBar.setDoubleClickEnabled(False)
-
-    def resizeEvent(self, e):
-        self.titleBar.resize(self.width(), self.titleBar.height())
-
-
-class FramelessMainWindow(QMainWindow, FramelessWindowBase):
-    """ Frameless main window """
-
-    def __init__(self, parent=None):
-        super().__init__(parent=parent)
-        self._initFrameless()
-
-
-class AcrylicWindow(AcrylicWindowBase):
-    """ Acrylic window """
-
-    def __init__(self, parent=None):
-        super().__init__(parent=parent)
-        self._initFrameless()
```

### Comparing `PySideSix-Frameless-Window-0.0.5/qframelesswindow/_rc/resource.py` & `PySideSix-Frameless-Window-0.0.6/qframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.5/qframelesswindow/linux/window_effect.py` & `PySideSix-Frameless-Window-0.0.6/qframelesswindow/linux/window_effect.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.5/qframelesswindow/mac/window_effect.py` & `PySideSix-Frameless-Window-0.0.6/qframelesswindow/mac/window_effect.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.5/qframelesswindow/titlebar/__init__.py` & `PySideSix-Frameless-Window-0.0.6/qframelesswindow/titlebar/__init__.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.5/qframelesswindow/titlebar/title_bar_buttons.py` & `PySideSix-Frameless-Window-0.0.6/qframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.5/qframelesswindow/utils/__init__.py` & `PySideSix-Frameless-Window-0.0.6/qframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.5/qframelesswindow/utils/linux_utils.py` & `PySideSix-Frameless-Window-0.0.6/qframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.5/qframelesswindow/utils/mac_utils.py` & `PySideSix-Frameless-Window-0.0.6/qframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.5/qframelesswindow/utils/win32_utils.py` & `PySideSix-Frameless-Window-0.0.6/qframelesswindow/utils/win32_utils.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.5/qframelesswindow/windows/__init__.py` & `PySideSix-Frameless-Window-0.0.6/qframelesswindow/windows/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # coding:utf-8
 from ctypes import cast
 from ctypes.wintypes import LPRECT, MSG
 
-import win32api
 import win32con
 import win32gui
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QCloseEvent, QCursor
-from PySide6.QtWidgets import QApplication, QWidget
+from PySide6.QtWidgets import QApplication, QDialog, QWidget, QMainWindow
 
 from ..titlebar import TitleBar
 from ..utils import win32_utils as win_utils
 from ..utils.win32_utils import Taskbar
 from .c_structures import LPNCCALCSIZE_PARAMS
 from .window_effect import WindowsWindowEffect
 
 
-class WindowsFramelessWindow(QWidget):
-    """  Frameless window for Windows system """
+class WindowsFramelessWindowBase:
+    """ Frameless window base class for Windows system """
 
     BORDER_WIDTH = 5
 
+    def __init__(self, *args, **kwargs):
+        pass
+
     def _initFrameless(self):
         self.windowEffect = WindowsWindowEffect(self)
         self.titleBar = TitleBar(self)
         self._isResizeEnabled = True
 
         # remove window border
         if not win_utils.isWin7():
@@ -57,23 +59,19 @@
         self.titleBar.setParent(self)
         self.titleBar.raise_()
 
     def setResizeEnabled(self, isEnabled: bool):
         """ set whether resizing is enabled """
         self._isResizeEnabled = isEnabled
 
-    def resizeEvent(self, e):
-        super().resizeEvent(e)
-        self.titleBar.resize(self.width(), self.titleBar.height())
-
     def nativeEvent(self, eventType, message):
         """ Handle the Windows message """
         msg = MSG.from_address(message.__int__())
         if not msg.hWnd:
-            return super().nativeEvent(eventType, message)
+            return False, 0
 
         if msg.message == win32con.WM_NCHITTEST and self._isResizeEnabled:
             pos = QCursor.pos()
             xPos = pos.x() - self.x()
             yPos = pos.y() - self.y()
             w, h = self.width(), self.height()
             lx = xPos < self.BORDER_WIDTH
@@ -126,21 +124,38 @@
                     rect.left += Taskbar.AUTO_HIDE_THICKNESS
                 elif position == Taskbar.RIGHT:
                     rect.right -= Taskbar.AUTO_HIDE_THICKNESS
 
             result = 0 if not msg.wParam else win32con.WVR_REDRAW
             return True, result
 
-        return super().nativeEvent(eventType, message)
+        return False, 0
 
     def __onScreenChanged(self):
         hWnd = int(self.windowHandle().winId())
         win32gui.SetWindowPos(hWnd, None, 0, 0, 0, 0, win32con.SWP_NOMOVE |
                               win32con.SWP_NOSIZE | win32con.SWP_FRAMECHANGED)
 
+    def resizeEvent(self, e):
+        self.titleBar.resize(self.width(), self.titleBar.height())
+
+
+class WindowsFramelessWindow(QWidget, WindowsFramelessWindowBase):
+    """  Frameless window for Windows system """
+
+    def __init__(self, parent=None):
+        super().__init__(parent=parent)
+        self._initFrameless()
+
+    def resizeEvent(self, e):
+        WindowsFramelessWindowBase.resizeEvent(self, e)
+
+    def nativeEvent(self, eventType, message):
+        return WindowsFramelessWindowBase.nativeEvent(self, eventType, message)
+
 
 class AcrylicWindow(WindowsFramelessWindow):
     """ A frameless window with acrylic effect """
 
     def __init__(self, parent=None):
         super().__init__(parent=parent)
         self.__closedByKey = False
@@ -178,7 +193,39 @@
         if not self.__closedByKey or QApplication.quitOnLastWindowClosed():
             self.__closedByKey = False
             return super().closeEvent(e)
 
         # system tray icon
         self.__closedByKey = False
         self.hide()
+
+
+class WindowsFramelessMainWindow(QMainWindow, WindowsFramelessWindowBase):
+    """ Frameless main window for Windows system """
+
+    def __init__(self, parent=None):
+        super().__init__(parent=parent)
+        self._initFrameless()
+
+    def resizeEvent(self, e):
+        QMainWindow.resizeEvent(self, e)
+        self.titleBar.resize(self.width(), self.titleBar.height())
+
+    def nativeEvent(self, eventType, message):
+        return WindowsFramelessWindowBase.nativeEvent(self, eventType, message)
+
+
+class WindowsFramelessDialog(QDialog, WindowsFramelessWindowBase):
+    """ Frameless dialog for Windows system """
+
+    def __init__(self, parent=None):
+        super().__init__(parent=parent)
+        self._initFrameless()
+        self.titleBar.minBtn.hide()
+        self.titleBar.maxBtn.hide()
+        self.titleBar.setDoubleClickEnabled(False)
+
+    def resizeEvent(self, e):
+        WindowsFramelessWindowBase.resizeEvent(self, e)
+
+    def nativeEvent(self, eventType, message):
+        return WindowsFramelessWindowBase.nativeEvent(self, eventType, message)
```

### Comparing `PySideSix-Frameless-Window-0.0.5/qframelesswindow/windows/c_structures.py` & `PySideSix-Frameless-Window-0.0.6/qframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.5/qframelesswindow/windows/window_effect.py` & `PySideSix-Frameless-Window-0.0.6/qframelesswindow/windows/window_effect.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.5/setup.py` & `PySideSix-Frameless-Window-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PySideSix-Frameless-Window",
-    version="0.0.5",
+    version="0.0.6",
     keywords="pyside6 frameless",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A cross-platform frameless window based on pyside6, support Win32, Linux and macOS.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="LGPLv3",
```

