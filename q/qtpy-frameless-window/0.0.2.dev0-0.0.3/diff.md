# Comparing `tmp/QtPy-Frameless-Window-0.0.2.dev0.tar.gz` & `tmp/QtPy-Frameless-Window-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QtPy-Frameless-Window-0.0.2.dev0.tar", last modified: Sun Apr  9 15:41:51 2023, max compression
+gzip compressed data, was "QtPy-Frameless-Window-0.0.3.tar", last modified: Mon Apr 10 08:17:36 2023, max compression
```

## Comparing `QtPy-Frameless-Window-0.0.2.dev0.tar` & `QtPy-Frameless-Window-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,19 @@
--rw-r--r--   0        0        0    35823 2023-04-09 13:19:55.238828 QtPy-Frameless-Window-0.0.2.dev0/LICENSE
--rw-r--r--   0        0        0      872 2023-04-09 15:39:35.842902 QtPy-Frameless-Window-0.0.2.dev0/pyproject.toml
--rw-r--r--   0        0        0     1811 2023-04-09 15:30:40.737482 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 13:19:55.243556 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/_rc/__init__.py
--rw-r--r--   0        0        0     2726 2023-04-09 13:19:55.243556 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/_rc/resource.py
--rw-r--r--   0        0        0      135 2023-04-09 13:19:55.244615 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/_rc/resource.qrc
--rw-r--r--   0        0        0     1471 2023-04-09 13:19:55.244615 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/_rc/resource_rc.py
--rw-r--r--   0        0        0      270 2023-04-09 13:19:55.245818 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/_rc/title_bar/close.svg
--rw-r--r--   0        0        0     3107 2023-04-09 15:30:12.853686 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/linux/__init__.py
--rw-r--r--   0        0        0     2920 2023-04-09 15:30:12.854739 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/linux/window_effect.py
--rw-r--r--   0        0        0     3013 2023-04-09 15:30:12.856021 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/mac/__init__.py
--rw-r--r--   0        0        0     4093 2023-04-09 15:30:12.856021 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/mac/window_effect.py
--rw-r--r--   0        0        0     4981 2023-04-09 13:19:55.250827 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/titlebar/__init__.py
--rw-r--r--   0        0        0     9024 2023-04-09 13:19:55.250827 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/titlebar/title_bar_buttons.py
--rw-r--r--   0        0        0      885 2023-04-09 13:19:55.251827 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/utils/__init__.py
--rw-r--r--   0        0        0      457 2023-04-09 15:31:56.716491 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/utils/api_differ.py
--rw-r--r--   0        0        0     5296 2023-04-09 15:30:12.857623 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/utils/linux_utils.py
--rw-r--r--   0        0        0     1848 2023-04-09 15:30:12.858697 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/utils/mac_utils.py
--rw-r--r--   0        0        0     7814 2023-04-09 13:19:55.254337 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/utils/win32_utils.py
--rw-r--r--   0        0        0     8675 2023-04-09 15:30:12.858697 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/windows/__init__.py
--rw-r--r--   0        0        0     4261 2023-04-09 13:19:55.256379 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/windows/c_structures.py
--rw-r--r--   0        0        0     8977 2023-04-09 13:19:55.256379 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/windows/window_effect.py
--rw-r--r--   0        0        0     1858 2023-04-09 15:38:49.563994 QtPy-Frameless-Window-0.0.2.dev0/README.md
--rw-r--r--   0        0        0     2327 1970-01-01 00:00:00.000000 QtPy-Frameless-Window-0.0.2.dev0/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-04-09 05:53:13.370931 QtPy-Frameless-Window-0.0.3/LICENSE
+-rw-r--r--   0        0        0      868 2023-04-10 08:16:15.197846 QtPy-Frameless-Window-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      334 2023-04-10 08:05:24.065036 QtPy-Frameless-Window-0.0.3/qt_api/__init__.py
+-rw-r--r--   0        0        0      500 2023-04-10 07:56:03.491124 QtPy-Frameless-Window-0.0.3/qtframelesswindow/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 04:08:57.987541 QtPy-Frameless-Window-0.0.3/qtframelesswindow/_rc/__init__.py
+-rw-r--r--   0        0        0     2726 2023-04-09 05:54:38.456441 QtPy-Frameless-Window-0.0.3/qtframelesswindow/_rc/resource.py
+-rw-r--r--   0        0        0      135 2023-04-09 04:08:57.987541 QtPy-Frameless-Window-0.0.3/qtframelesswindow/_rc/resource.qrc
+-rw-r--r--   0        0        0     1471 2023-04-10 07:22:02.881400 QtPy-Frameless-Window-0.0.3/qtframelesswindow/_rc/resource_rc.py
+-rw-r--r--   0        0        0      270 2023-04-09 04:08:57.987541 QtPy-Frameless-Window-0.0.3/qtframelesswindow/_rc/title_bar/close.svg
+-rw-r--r--   0        0        0     4981 2023-04-09 05:54:38.598440 QtPy-Frameless-Window-0.0.3/qtframelesswindow/titlebar/__init__.py
+-rw-r--r--   0        0        0     9024 2023-04-09 05:56:24.750554 QtPy-Frameless-Window-0.0.3/qtframelesswindow/titlebar/title_bar_buttons.py
+-rw-r--r--   0        0        0      885 2023-04-09 04:08:57.989541 QtPy-Frameless-Window-0.0.3/qtframelesswindow/utils/__init__.py
+-rw-r--r--   0        0        0      459 2023-04-10 03:39:03.420822 QtPy-Frameless-Window-0.0.3/qtframelesswindow/utils/api_differ.py
+-rw-r--r--   0        0        0     7814 2023-04-09 10:26:41.353848 QtPy-Frameless-Window-0.0.3/qtframelesswindow/utils/win32_utils.py
+-rw-r--r--   0        0        0     8679 2023-04-10 03:39:03.420822 QtPy-Frameless-Window-0.0.3/qtframelesswindow/windows/__init__.py
+-rw-r--r--   0        0        0     4261 2023-04-09 08:44:41.724457 QtPy-Frameless-Window-0.0.3/qtframelesswindow/windows/c_structures.py
+-rw-r--r--   0        0        0     8977 2023-04-09 08:46:42.475612 QtPy-Frameless-Window-0.0.3/qtframelesswindow/windows/window_effect.py
+-rw-r--r--   0        0        0     1993 2023-04-10 08:13:31.126161 QtPy-Frameless-Window-0.0.3/README.md
+-rw-r--r--   0        0        0     2457 1970-01-01 00:00:00.000000 QtPy-Frameless-Window-0.0.3/PKG-INFO
```

### Comparing `QtPy-Frameless-Window-0.0.2.dev0/LICENSE` & `QtPy-Frameless-Window-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2.dev0/pyproject.toml` & `QtPy-Frameless-Window-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 description = "A cross-platform frameless window based on QtPy."
 keywords = [
     "pyqt frameless",
 ]
 name = "QtPy-Frameless-Window"
 readme = "README.md"
 requires-python = ">=3.6"
-version = "0.0.2-dev"
+version = "0.0.3"
 
 [project.license]
 text = "GPLv3"
 
 [project.urls]
 Homepage = "https://github.com/TaoChenyue/QtPy-Frameless-Window.git"
```

### Comparing `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/_rc/resource.py` & `QtPy-Frameless-Window-0.0.3/qtframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/_rc/resource_rc.py` & `QtPy-Frameless-Window-0.0.3/qtframelesswindow/_rc/resource_rc.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/titlebar/__init__.py` & `QtPy-Frameless-Window-0.0.3/qtframelesswindow/titlebar/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/titlebar/title_bar_buttons.py` & `QtPy-Frameless-Window-0.0.3/qtframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/utils/__init__.py` & `QtPy-Frameless-Window-0.0.3/qtframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/utils/win32_utils.py` & `QtPy-Frameless-Window-0.0.3/qtframelesswindow/utils/win32_utils.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/windows/__init__.py` & `QtPy-Frameless-Window-0.0.3/qtframelesswindow/windows/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,16 +184,16 @@
         self.windowEffect.addWindowAnimation(self.winId())
 
         if win_utils.isWin7():
             self.windowEffect.addShadowEffect(self.winId())
             self.windowEffect.setAeroEffect(self.winId())
         else:
             self.windowEffect.setAcrylicEffect(self.winId())
-            if win_utils.isGreaterEqualWin11():
-                self.windowEffect.addShadowEffect(self.winId())
+            # if win_utils.isGreaterEqualWin11():
+            #     self.windowEffect.addShadowEffect(self.winId())
 
         self.setStyleSheet("AcrylicWindow{background:transparent}")
 
     def nativeEvent(self, eventType, message):
         """Handle the Windows message"""
         msg = MSG.from_address(message.__int__())
```

### Comparing `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/windows/c_structures.py` & `QtPy-Frameless-Window-0.0.3/qtframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/windows/window_effect.py` & `QtPy-Frameless-Window-0.0.3/qtframelesswindow/windows/window_effect.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2.dev0/README.md` & `QtPy-Frameless-Window-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -20,41 +20,41 @@
 Or clone the repo:
 ```shell
 git clone https://github.com/TaoChenyue/QtPy-Frameless-Window.git
 python setup.py install
 ```
 
 ## Usage
-you can specify qt api(pyqt5,pyqt6,pyside2,pyside6) like this in the beginning:
+According to QtPy, environment argument ```QT_API``` must be set before import qtpy. Here provides an easy way to set it.
 
 ```python
-from qtframelesswindow import set_qt_api
+from qt_api import set_qt_api
+# set through code
 set_qt_api("pyqt5")
+python examples/demo.py 
+# set through sys.argv
+set_qt_api(parse=True)
+python examples/demo.py --api pyside6
 ```
-or specify qt api through args
-```sh
-python your-pyscript.py
-# or 
-python your-pyscript.py --api pyside6
-```
-default qt api is pyqt5.
+If no QT_API is set, qtpy will use pyqt5 as default.
+
 ```python
-from qtframelesswindow import FramelessWindow
+from qt_api import set_qt_api
+set_qt_api("pyqt5")
 from qtpy.QtWidgets import QApplication
-
+from qtframelesswindow import FramelessWindow
 
 class Window(FramelessWindow):
     def __init__(self, parent=None):
         super().__init__(parent=parent)
         self.setWindowTitle("QtPy-Frameless-Window")
 
-
 if __name__ == "__main__":
     app = QApplication([])
     demo = Window()
     demo.show()
     app.exec_()
 ```
 
 ## FQ
-Q: Why acrylic window response slowly when dragging its edge on Windows platform?
-A: Reference to https://www.cnblogs.com/zhiyiYo/p/14659981.html, change settings.
++ Q: Why acrylic window response slowly when dragging its edge on Windows platform?<br>
+A: Reference to https://www.cnblogs.com/zhiyiYo/p/14659981.html, change settings.
```

### Comparing `QtPy-Frameless-Window-0.0.2.dev0/PKG-INFO` & `QtPy-Frameless-Window-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QtPy-Frameless-Window
-Version: 0.0.2-dev
+Version: 0.0.3
 Summary: A cross-platform frameless window based on QtPy.
 License: GPLv3
 Keywords: pyqt frameless
 Author-email: TaoChenyue <3038816978@qq.com>
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -34,41 +34,42 @@
 Or clone the repo:
 ```shell
 git clone https://github.com/TaoChenyue/QtPy-Frameless-Window.git
 python setup.py install
 ```
 
 ## Usage
-you can specify qt api(pyqt5,pyqt6,pyside2,pyside6) like this in the beginning:
+According to QtPy, environment argument ```QT_API``` must be set before import qtpy. Here provides an easy way to set it.
 
 ```python
-from qtframelesswindow import set_qt_api
+from qt_api import set_qt_api
+# set through code
 set_qt_api("pyqt5")
+python examples/demo.py 
+# set through sys.argv
+set_qt_api(parse=True)
+python examples/demo.py --api pyside6
 ```
-or specify qt api through args
-```sh
-python your-pyscript.py
-# or 
-python your-pyscript.py --api pyside6
-```
-default qt api is pyqt5.
+If no QT_API is set, qtpy will use pyqt5 as default.
+
 ```python
-from qtframelesswindow import FramelessWindow
+from qt_api import set_qt_api
+set_qt_api("pyqt5")
 from qtpy.QtWidgets import QApplication
-
+from qtframelesswindow import FramelessWindow
 
 class Window(FramelessWindow):
     def __init__(self, parent=None):
         super().__init__(parent=parent)
         self.setWindowTitle("QtPy-Frameless-Window")
 
-
 if __name__ == "__main__":
     app = QApplication([])
     demo = Window()
     demo.show()
     app.exec_()
 ```
 
 ## FQ
-Q: Why acrylic window response slowly when dragging its edge on Windows platform?
++ Q: Why acrylic window response slowly when dragging its edge on Windows platform?<br>
 A: Reference to https://www.cnblogs.com/zhiyiYo/p/14659981.html, change settings.
+
```

