# Comparing `tmp/QtPy-Frameless-Window-0.0.5.tar.gz` & `tmp/QtPy-Frameless-Window-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QtPy-Frameless-Window-0.0.5.tar", last modified: Mon Apr 10 12:48:05 2023, max compression
+gzip compressed data, was "QtPy-Frameless-Window-0.0.6.tar", last modified: Mon Apr 10 14:24:33 2023, max compression
```

## Comparing `QtPy-Frameless-Window-0.0.5.tar` & `QtPy-Frameless-Window-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    35823 2023-04-09 05:53:13.370931 QtPy-Frameless-Window-0.0.5/LICENSE
--rw-r--r--   0        0        0      868 2023-04-10 12:47:58.146888 QtPy-Frameless-Window-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      334 2023-04-10 12:46:32.973798 QtPy-Frameless-Window-0.0.5/qt_api/__init__.py
--rw-r--r--   0        0        0     1811 2023-04-10 12:46:20.707878 QtPy-Frameless-Window-0.0.5/qtframelesswindow/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 04:08:57.987541 QtPy-Frameless-Window-0.0.5/qtframelesswindow/_rc/__init__.py
--rw-r--r--   0        0        0     2726 2023-04-09 05:54:38.456441 QtPy-Frameless-Window-0.0.5/qtframelesswindow/_rc/resource.py
--rw-r--r--   0        0        0      135 2023-04-09 04:08:57.987541 QtPy-Frameless-Window-0.0.5/qtframelesswindow/_rc/resource.qrc
--rw-r--r--   0        0        0     1471 2023-04-10 12:40:23.394056 QtPy-Frameless-Window-0.0.5/qtframelesswindow/_rc/resource_rc.py
--rw-r--r--   0        0        0      270 2023-04-09 04:08:57.987541 QtPy-Frameless-Window-0.0.5/qtframelesswindow/_rc/title_bar/close.svg
--rw-r--r--   0        0        0     3107 2023-04-10 12:46:20.707878 QtPy-Frameless-Window-0.0.5/qtframelesswindow/linux/__init__.py
--rw-r--r--   0        0        0     2920 2023-04-10 12:46:20.708878 QtPy-Frameless-Window-0.0.5/qtframelesswindow/linux/window_effect.py
--rw-r--r--   0        0        0     3013 2023-04-10 12:46:20.709879 QtPy-Frameless-Window-0.0.5/qtframelesswindow/mac/__init__.py
--rw-r--r--   0        0        0     4093 2023-04-10 12:46:20.709879 QtPy-Frameless-Window-0.0.5/qtframelesswindow/mac/window_effect.py
--rw-r--r--   0        0        0     4981 2023-04-09 05:54:38.598440 QtPy-Frameless-Window-0.0.5/qtframelesswindow/titlebar/__init__.py
--rw-r--r--   0        0        0     9024 2023-04-09 05:56:24.750554 QtPy-Frameless-Window-0.0.5/qtframelesswindow/titlebar/title_bar_buttons.py
--rw-r--r--   0        0        0      885 2023-04-09 04:08:57.989541 QtPy-Frameless-Window-0.0.5/qtframelesswindow/utils/__init__.py
--rw-r--r--   0        0        0      457 2023-04-10 12:46:20.710881 QtPy-Frameless-Window-0.0.5/qtframelesswindow/utils/api_differ.py
--rw-r--r--   0        0        0     5296 2023-04-10 12:46:20.711882 QtPy-Frameless-Window-0.0.5/qtframelesswindow/utils/linux_utils.py
--rw-r--r--   0        0        0     1848 2023-04-10 12:46:20.711882 QtPy-Frameless-Window-0.0.5/qtframelesswindow/utils/mac_utils.py
--rw-r--r--   0        0        0     7814 2023-04-09 10:26:41.353848 QtPy-Frameless-Window-0.0.5/qtframelesswindow/utils/win32_utils.py
--rw-r--r--   0        0        0     8675 2023-04-10 12:46:20.712878 QtPy-Frameless-Window-0.0.5/qtframelesswindow/windows/__init__.py
--rw-r--r--   0        0        0     4261 2023-04-09 08:44:41.724457 QtPy-Frameless-Window-0.0.5/qtframelesswindow/windows/c_structures.py
--rw-r--r--   0        0        0     8977 2023-04-09 08:46:42.475612 QtPy-Frameless-Window-0.0.5/qtframelesswindow/windows/window_effect.py
--rw-r--r--   0        0        0     1866 2023-04-10 12:46:20.703878 QtPy-Frameless-Window-0.0.5/README.md
--rw-r--r--   0        0        0     2330 1970-01-01 00:00:00.000000 QtPy-Frameless-Window-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-04-10 13:55:10.340365 QtPy-Frameless-Window-0.0.6/LICENSE
+-rw-r--r--   0        0        0      868 2023-04-10 14:23:30.646342 QtPy-Frameless-Window-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      334 2023-04-10 13:41:06.835245 QtPy-Frameless-Window-0.0.6/qt_api/__init__.py
+-rw-r--r--   0        0        0     1411 2023-04-10 13:55:10.375881 QtPy-Frameless-Window-0.0.6/qtframelesswindow/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 13:38:09.871612 QtPy-Frameless-Window-0.0.6/qtframelesswindow/_rc/__init__.py
+-rw-r--r--   0        0        0     2726 2023-04-10 13:55:10.375881 QtPy-Frameless-Window-0.0.6/qtframelesswindow/_rc/resource.py
+-rw-r--r--   0        0        0      135 2023-04-10 13:38:09.871612 QtPy-Frameless-Window-0.0.6/qtframelesswindow/_rc/resource.qrc
+-rw-r--r--   0        0        0     1471 2023-04-10 13:55:10.376882 QtPy-Frameless-Window-0.0.6/qtframelesswindow/_rc/resource_rc.py
+-rw-r--r--   0        0        0      270 2023-04-10 13:38:09.871612 QtPy-Frameless-Window-0.0.6/qtframelesswindow/_rc/title_bar/close.svg
+-rw-r--r--   0        0        0      457 2023-04-10 13:56:41.474504 QtPy-Frameless-Window-0.0.6/qtframelesswindow/api_differ/windows.py
+-rw-r--r--   0        0        0    13288 2023-04-10 14:13:36.743103 QtPy-Frameless-Window-0.0.6/qtframelesswindow/linux/__init__.py
+-rw-r--r--   0        0        0     2920 2023-04-10 13:55:10.390882 QtPy-Frameless-Window-0.0.6/qtframelesswindow/linux/window_effect.py
+-rw-r--r--   0        0        0    14832 2023-04-10 14:17:48.095834 QtPy-Frameless-Window-0.0.6/qtframelesswindow/mac/__init__.py
+-rw-r--r--   0        0        0     4093 2023-04-10 13:55:10.391881 QtPy-Frameless-Window-0.0.6/qtframelesswindow/mac/window_effect.py
+-rw-r--r--   0        0        0     4981 2023-04-10 13:55:10.391881 QtPy-Frameless-Window-0.0.6/qtframelesswindow/titlebar/__init__.py
+-rw-r--r--   0        0        0     9024 2023-04-10 13:39:48.695927 QtPy-Frameless-Window-0.0.6/qtframelesswindow/titlebar/title_bar_buttons.py
+-rw-r--r--   0        0        0      885 2023-04-10 14:01:03.589216 QtPy-Frameless-Window-0.0.6/qtframelesswindow/utils/__init__.py
+-rw-r--r--   0        0        0     9302 2023-04-10 14:05:49.422983 QtPy-Frameless-Window-0.0.6/qtframelesswindow/utils/linux_utils.py
+-rw-r--r--   0        0        0     8330 2023-04-10 14:09:51.608296 QtPy-Frameless-Window-0.0.6/qtframelesswindow/utils/mac_utils.py
+-rw-r--r--   0        0        0     7816 2023-04-10 13:57:02.791321 QtPy-Frameless-Window-0.0.6/qtframelesswindow/utils/win32_utils.py
+-rw-r--r--   0        0        0     8675 2023-04-10 13:55:10.394880 QtPy-Frameless-Window-0.0.6/qtframelesswindow/windows/__init__.py
+-rw-r--r--   0        0        0     4261 2023-04-10 13:55:10.394880 QtPy-Frameless-Window-0.0.6/qtframelesswindow/windows/c_structures.py
+-rw-r--r--   0        0        0     8979 2023-04-10 13:57:21.082863 QtPy-Frameless-Window-0.0.6/qtframelesswindow/windows/window_effect.py
+-rw-r--r--   0        0        0     1163 2023-04-10 13:55:10.341348 QtPy-Frameless-Window-0.0.6/README.md
+-rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 QtPy-Frameless-Window-0.0.6/PKG-INFO
```

### Comparing `QtPy-Frameless-Window-0.0.5/LICENSE` & `QtPy-Frameless-Window-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.5/pyproject.toml` & `QtPy-Frameless-Window-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 description = "A cross-platform frameless window based on QtPy."
 keywords = [
     "pyqt frameless",
 ]
 name = "QtPy-Frameless-Window"
 readme = "README.md"
 requires-python = ">=3.6"
-version = "0.0.5"
+version = "0.0.6"
 
 [project.license]
 text = "GPLv3"
 
 [project.urls]
 Homepage = "https://github.com/TaoChenyue/QtPy-Frameless-Window.git"
```

### Comparing `QtPy-Frameless-Window-0.0.5/qtframelesswindow/__init__.py` & `QtPy-Frameless-Window-0.0.6/qtframelesswindow/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,9 @@
 import os
 import argparse
-def set_qt_api(api:str=None,parse:bool=False):
-    if parse:
-        parser = argparse.ArgumentParser(description='Set Qt API')
-        parser.add_argument('--api', type=str)
-        args = parser.parse_args()
-        if args.api is not None:
-            api=args.api
-        return args
-    if api is None:
-        api="pyqt5"
-    os.environ["QT_API"]=api
-    
-set_qt_api(parse=True)
-
 from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar
 from qtpy.QtWidgets import QDialog,QMainWindow
 import sys
 if sys.platform == "win32":
     from .windows import AcrylicWindow
     from .windows import WindowsFramelessWindow as FramelessWindow
     from .windows import WindowsFramelessMainWindow as FramelessMainWindow
```

### Comparing `QtPy-Frameless-Window-0.0.5/qtframelesswindow/_rc/resource.py` & `QtPy-Frameless-Window-0.0.6/qtframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.5/qtframelesswindow/_rc/resource_rc.py` & `QtPy-Frameless-Window-0.0.6/qtframelesswindow/_rc/resource_rc.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.5/qtframelesswindow/linux/window_effect.py` & `QtPy-Frameless-Window-0.0.6/qtframelesswindow/linux/window_effect.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.5/qtframelesswindow/mac/window_effect.py` & `QtPy-Frameless-Window-0.0.6/qtframelesswindow/mac/window_effect.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.5/qtframelesswindow/titlebar/__init__.py` & `QtPy-Frameless-Window-0.0.6/qtframelesswindow/titlebar/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.5/qtframelesswindow/titlebar/title_bar_buttons.py` & `QtPy-Frameless-Window-0.0.6/qtframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.5/qtframelesswindow/utils/__init__.py` & `QtPy-Frameless-Window-0.0.6/qtframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.5/qtframelesswindow/utils/win32_utils.py` & `QtPy-Frameless-Window-0.0.6/qtframelesswindow/utils/win32_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import win32api
 import win32con
 import win32gui
 from qtpy.QtCore import QOperatingSystemVersion
 from qtpy.QtGui import QGuiApplication
 from win32comext.shell import shellcon
 
-from ..utils.api_differ import QtWin
+from ..api_differ.windows import QtWin
 
 
 def isMaximized(hWnd):
     """ Determine whether the window is maximized
 
     Parameters
     ----------
```

### Comparing `QtPy-Frameless-Window-0.0.5/qtframelesswindow/windows/__init__.py` & `QtPy-Frameless-Window-0.0.6/qtframelesswindow/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.5/qtframelesswindow/windows/c_structures.py` & `QtPy-Frameless-Window-0.0.6/qtframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.5/qtframelesswindow/windows/window_effect.py` & `QtPy-Frameless-Window-0.0.6/qtframelesswindow/windows/window_effect.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import win32gui
 
 from .c_structures import (ACCENT_POLICY, ACCENT_STATE, DWMNCRENDERINGPOLICY,
                            DWMWINDOWATTRIBUTE, MARGINS,
                            WINDOWCOMPOSITIONATTRIB,
                            WINDOWCOMPOSITIONATTRIBDATA, DWM_BLURBEHIND)
 from ..utils.win32_utils import isGreaterEqualWin10, isGreaterEqualWin11
-from ..utils.api_differ import QtWin
+from ..api_differ.windows import QtWin
 
 
 class WindowsWindowEffect:
     """ Windows window effect """
 
     def __init__(self, window):
         self.window = window
```

### Comparing `QtPy-Frameless-Window-0.0.5/README.md` & `QtPy-Frameless-Window-0.0.6/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -19,42 +19,10 @@
 ```
 Or clone the repo:
 ```shell
 git clone https://github.com/TaoChenyue/QtPy-Frameless-Window.git
 python setup.py install
 ```
 
-## Usage
-you can specify qt api(pyqt5,pyqt6,pyside2,pyside6) like this in the beginning:
-
-```python
-from qtframelesswindow import set_qt_api
-set_qt_api("pyqt5")
-```
-or specify qt api through args
-```sh
-python your-pyscript.py
-# or 
-python your-pyscript.py --api pyside6
-```
-default qt api is pyqt5.
-```python
-from qtframelesswindow import FramelessWindow
-from qtpy.QtWidgets import QApplication
-
-
-class Window(FramelessWindow):
-    def __init__(self, parent=None):
-        super().__init__(parent=parent)
-        self.setWindowTitle("QtPy-Frameless-Window")
-
-
-if __name__ == "__main__":
-    app = QApplication([])
-    demo = Window()
-    demo.show()
-    app.exec_()
-```
-
 ## FQ
 + Q: Why acrylic window response slowly when dragging its edge on Windows platform?<br>
 A: Reference to https://www.cnblogs.com/zhiyiYo/p/14659981.html, change settings.
```

### Comparing `QtPy-Frameless-Window-0.0.5/PKG-INFO` & `QtPy-Frameless-Window-0.0.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QtPy-Frameless-Window
-Version: 0.0.5
+Version: 0.0.6
 Summary: A cross-platform frameless window based on QtPy.
 License: GPLv3
 Keywords: pyqt frameless
 Author-email: TaoChenyue <3038816978@qq.com>
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -33,43 +33,11 @@
 ```
 Or clone the repo:
 ```shell
 git clone https://github.com/TaoChenyue/QtPy-Frameless-Window.git
 python setup.py install
 ```
 
-## Usage
-you can specify qt api(pyqt5,pyqt6,pyside2,pyside6) like this in the beginning:
-
-```python
-from qtframelesswindow import set_qt_api
-set_qt_api("pyqt5")
-```
-or specify qt api through args
-```sh
-python your-pyscript.py
-# or 
-python your-pyscript.py --api pyside6
-```
-default qt api is pyqt5.
-```python
-from qtframelesswindow import FramelessWindow
-from qtpy.QtWidgets import QApplication
-
-
-class Window(FramelessWindow):
-    def __init__(self, parent=None):
-        super().__init__(parent=parent)
-        self.setWindowTitle("QtPy-Frameless-Window")
-
-
-if __name__ == "__main__":
-    app = QApplication([])
-    demo = Window()
-    demo.show()
-    app.exec_()
-```
-
 ## FQ
 + Q: Why acrylic window response slowly when dragging its edge on Windows platform?<br>
 A: Reference to https://www.cnblogs.com/zhiyiYo/p/14659981.html, change settings.
```

