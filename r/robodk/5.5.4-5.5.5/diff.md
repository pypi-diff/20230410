# Comparing `tmp/robodk-5.5.4-py2.py3-none-any.whl.zip` & `tmp/robodk-5.5.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 112201 bytes, number of entries: 15
+Zip file size: 112526 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-02 02:24 pylint_robodk/__init__.py
 -rw-rw-rw-  2.0 fat     1551 b- defN 22-Feb-02 02:24 pylint_robodk/pylint_robodk.py
--rw-rw-rw-  2.0 fat     1516 b- defN 22-Sep-14 12:27 robodk/__init__.py
--rw-rw-rw-  2.0 fat    52103 b- defN 23-Feb-09 17:37 robodk/roboapps.py
--rw-rw-rw-  2.0 fat    45346 b- defN 22-Dec-20 17:55 robodk/robodialogs.py
--rw-rw-rw-  2.0 fat    12497 b- defN 22-Oct-14 18:41 robodk/robofileio.py
--rw-rw-rw-  2.0 fat   325446 b- defN 22-Dec-14 18:28 robodk/robolink.py
--rw-rw-rw-  2.0 fat    10017 b- defN 22-Nov-03 14:49 robodk/robolinkutils.py
--rw-rw-rw-  2.0 fat    68433 b- defN 23-Feb-03 13:35 robodk/robomath.py
+-rw-rw-rw-  2.0 fat     1516 b- defN 23-Mar-09 14:20 robodk/__init__.py
+-rw-rw-rw-  2.0 fat    52619 b- defN 23-Mar-28 13:48 robodk/roboapps.py
+-rw-rw-rw-  2.0 fat    45464 b- defN 23-Mar-28 13:48 robodk/robodialogs.py
+-rw-rw-rw-  2.0 fat    12502 b- defN 23-Mar-09 14:20 robodk/robofileio.py
+-rw-rw-rw-  2.0 fat   326660 b- defN 23-Mar-28 14:43 robodk/robolink.py
+-rw-rw-rw-  2.0 fat    10012 b- defN 23-Apr-06 17:28 robodk/robolinkutils.py
+-rw-rw-rw-  2.0 fat    68442 b- defN 23-Mar-27 23:23 robodk/robomath.py
 -rw-rw-rw-  2.0 fat     1210 b- defN 22-Feb-02 02:29 robolink/__init__.py
--rw-rw-rw-  2.0 fat      587 b- defN 23-Feb-09 17:49 robodk-5.5.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    12419 b- defN 23-Feb-09 17:49 robodk-5.5.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Feb-09 17:49 robodk-5.5.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       30 b- defN 23-Feb-09 17:49 robodk-5.5.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1167 b- defN 23-Feb-09 17:49 robodk-5.5.4.dist-info/RECORD
-15 files, 532432 bytes uncompressed, 110309 bytes compressed:  79.3%
+-rw-rw-rw-  2.0 fat      587 b- defN 23-Apr-10 19:34 robodk-5.5.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    12710 b- defN 23-Apr-10 19:34 robodk-5.5.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-10 19:34 robodk-5.5.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       30 b- defN 23-Apr-10 19:34 robodk-5.5.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1167 b- defN 23-Apr-10 19:34 robodk-5.5.5.dist-info/RECORD
+15 files, 534580 bytes uncompressed, 110634 bytes compressed:  79.3%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: robodk/robomath.py
 Comment: 
 
 Filename: robolink/__init__.py
 Comment: 
 
-Filename: robodk-5.5.4.dist-info/LICENSE
+Filename: robodk-5.5.5.dist-info/LICENSE
 Comment: 
 
-Filename: robodk-5.5.4.dist-info/METADATA
+Filename: robodk-5.5.5.dist-info/METADATA
 Comment: 
 
-Filename: robodk-5.5.4.dist-info/WHEEL
+Filename: robodk-5.5.5.dist-info/WHEEL
 Comment: 
 
-Filename: robodk-5.5.4.dist-info/top_level.txt
+Filename: robodk-5.5.5.dist-info/top_level.txt
 Comment: 
 
-Filename: robodk-5.5.4.dist-info/RECORD
+Filename: robodk-5.5.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## robodk/roboapps.py

```diff
@@ -19,21 +19,28 @@
 #     https://robodk.com/doc/en/RoboDK-API.html
 #     https://robodk.com/doc/en/PythonAPI/index.html
 # --------------------------------------------
 
 import sys
 import time
 
-if 'ENABLE_TK' not in globals():
-    global ENABLE_TK
-    ENABLE_TK = True
-
-if 'ENABLE_QT' not in globals():
-    global ENABLE_QT
-    ENABLE_QT = True
+from robodk import robodialogs
+
+if robodialogs.ENABLE_QT:
+    from PySide2 import QtWidgets, QtCore, QtGui
+
+if robodialogs.ENABLE_TK:
+    if sys.version_info[0] < 3:
+        import Tkinter as tkinter
+        import tkFileDialog as filedialog
+        import tkMessageBox as messagebox
+    else:
+        import tkinter
+        from tkinter import filedialog
+        from tkinter import messagebox
 """
 App/actions control utilities.
 
 Use these to control your App's actions: run on click, run while checked, do not kill, etc.
 """
 
 
@@ -116,15 +123,15 @@
 
     return False
 
 
 def Checked():
     """
     Verify if the command "Checked" is present. In this case it means the action was just checked from RoboDK (applicable to checkable actions only).
-    
+
     Example for a 'Checkable Action':
 
     .. code-block:: python
 
         def runmain():
             if roboapps.Unchecked():
                 ActionUnchecked()
@@ -162,15 +169,15 @@
     sys.stdout.flush()
 
 
 def SkipKill():
     """
     For Checkable actions, this setting will tell RoboDK App loader to not kill the process a few seconds after the terminate function is called.
     This is needed if we want the user input to save the file. For example: The Record action from the Record App.
-    
+
     Example for a 'Momentary Action':
 
     .. code-block:: python
 
         def runmain():
             if roboapps.Unchecked():
                 roboapps.Exit()  # or sys.exit()
@@ -314,15 +321,15 @@
     :param parent: Parent of the widget (Qt/Tkinter)
 
     :return: (widget, funcs) the widget, and a list of 'get' functions to retrieve the value of the widget
     :rtype: tuple of widget (Qt/Tkinter), callable
 
     .. seealso:: :func:`~robodk.roboapps.widget_to_value`
     """
-    if ENABLE_QT:
+    if robodialogs.ENABLE_QT:
         return value_to_qt_widget(value, parent)
     else:
         return value_to_tk_widget(value, parent)
 
 
 def widget_to_value(funcs, original_value):
     """
@@ -438,30 +445,25 @@
     return themes[int(theme_idx)]
 
 
 """
 PySide2 / Qt utilities
 """
 
-if ENABLE_QT:
-    try:
-        from robodk.robolink import import_install
-        import_install("PySide2", "PySide2==5.15.*")
-        from PySide2 import QtCore, QtGui, QtWidgets
-    except:
-        ENABLE_QT = False
+if robodialogs.ENABLE_QT:
 
-if ENABLE_QT:
-
-    def get_qt_app(robodk_icon=True, robodk_theme=True):
+    def get_qt_app(robodk_icon=True, robodk_theme=True, RDK=None):
         """
         Get the QApplication instance.
 
+        Note: If RoboDK is not running, The RoboDK theme is not applied.
+
         :param bool robodk_icon: Applies the RoboDK logo, defaults to True
         :param bool robodk_theme: Applies the current RoboDK theme, defaults to True
+        :param robolink.Robolink RDK: Link to the running RoboDK instance for the theme, defaults to None
 
         :return: The QApplication instance
         :rtype: :class:`PySide2.QtWidgets.QApplication`
         """
 
         app = QtWidgets.QApplication.instance()
         if app is None:
@@ -470,23 +472,28 @@
             app = QtWidgets.QApplication([])
 
         if robodk_icon:
             from robodk import robolink
             icon_path = robolink.getPathIcon()
             from os import path
             if path.exists(icon_path):
-                import sys
                 if sys.platform.startswith('win'):
                     import ctypes
                     ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(str(app))  # Enable the taskbar icon
                 app_icon = QtGui.QIcon(icon_path)
                 app.setWindowIcon(app_icon)
 
         if robodk_theme:
-            set_qt_theme(app)
+            if RDK is None:
+                RDK = robolink.Robolink(robodk_path='')  # If no running instance of RoboDK is found, do not instantiate RoboDK
+            try:
+                if RDK._is_connected():
+                    set_qt_theme(app, RDK)
+            except:
+                pass
 
         return app
 
     def set_qt_theme(app, RDK=None):
         """Set a Qt application theme to match RoboDK's theme.
 
         :param app: The QApplication
@@ -549,18 +556,18 @@
 
         .. seealso:: :func:`~robodk.roboapps.get_qt_robodk_icons`
         """
         if RDK is None:
             from robodk.robolink import Robolink
             RDK = Robolink()
 
-        #if 'OK' != RDK.Command('PluginLoad', 'App Loader'):  # Ensure the plugin is loaded
-        #    return None
-
-        img_hex = RDK.PluginCommand('App Loader', 'IconGet', icon_name)
+        if 'Addin Manager' in RDK.Command('PluginsList'):
+            img_hex = RDK.PluginCommand('Addin Manager', 'IconGet', icon_name)
+        else:
+            img_hex = RDK.PluginCommand('App Loader', 'IconGet', icon_name)
         if type(img_hex) is not str or img_hex == '':
             return None
 
         byte_array = QtCore.QByteArray.fromHex(img_hex.encode())
         image = QtGui.QImage()  # QImage does not require a QApplication instance, as appose to QPixmap
         if not image.loadFromData(byte_array):
             return None
@@ -801,37 +808,23 @@
         return widget, func
 
 
 """
 Tkinter utilities
 """
 
-if ENABLE_TK:
-    import sys
-    if sys.version_info[0] < 3:
-        # Python 2.X only:
-        try:
-            import Tkinter as tkinter
-        except:
-            ENABLE_TK = False
-    else:
-        # Python 3.x only
-        try:
-            import tkinter
-        except:
-            ENABLE_TK = False
-
-if ENABLE_TK:
+if robodialogs.ENABLE_TK:
 
-    def get_tk_app(robodk_icon=True, robodk_theme=True):
+    def get_tk_app(robodk_icon=True, robodk_theme=True, RDK=None):
         """
         Get the QApplication instance.
 
         :param bool robodk_icon: Applies the RoboDK logo, defaults to True
         :param bool robodk_theme: Applies the current RoboDK theme, defaults to True
+        :param robolink.Robolink RDK: Link to the running RoboDK instance for the theme, defaults to None
 
         :return: The QApplication instance
         :rtype: :class:`PySide2.QtWidgets.QApplication`
         """
 
         app = tkinter.Tk()
         app.withdraw()  # Use app.deiconify() to show the app, if needed
@@ -844,15 +837,14 @@
         app.update_idletasks()
 
         if robodk_icon:
             from robodk import robolink
             icon_path = robolink.getPathIcon()
             from os import path
             if path.exists(icon_path):
-                import sys
                 if sys.platform.startswith('win'):
                     import ctypes
                     ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(str(app))  # Enable the taskbar icon
                 app.iconbitmap(default=icon_path)
 
         if robodk_theme:
             pass  # TODO: Use tkk to apply styling globally
@@ -951,28 +943,28 @@
     Generic application settings class to save and load settings to a RoboDK station with a built-in UI.
 
     :param str settings_param: RoboDK parameter used to store this app settings. It should be unique if you have more than one App setting.
 
     Example:
 
         .. code-block:: python
-        
+
             class Settings(AppSettings):
 
                 def __init__(self, settings_param='My-App-Settings'):
                     super().__init__(settings_param=settings_param)
 
                     # List the variable names you would like to save and their default values.
                     # Variables that start with underscore (_) will not be saved.
                     self.BOOL = True
                     self.INT = 123456
                     self.FLOAT = 0.123456789
                     self.STRING = 'Text'
-                    self.INT_LIST = [1, 2, 3]  
-                    self.FLOAT_LIST = [1.0, 2.0, 3.0]  
+                    self.INT_LIST = [1, 2, 3]
+                    self.FLOAT_LIST = [1.0, 2.0, 3.0]
                     self.STRING_LIST = ['First line', 'Second line', 'Third line']
                     self.MIXED_LIST = [False, 1, '2']
                     self.INT_TUPLE = (1, 2, 3)
                     self.DROPDOWN = [1, ['First line', 'Second line', 'Third line']]
                     self.DICT = {'This is a string': 'Text', 'This is a float': 0.0}
 
                     # Variable names when displayed on the user interface (detailed descriptions).
@@ -1045,15 +1037,15 @@
                 defaults[a] = getattr(base, a)
         return defaults
 
     def getAttribs(self):
         """
         Get the list of all attributes (settings).
         Attributes that starts with '_' are ignored.
-        
+
         :return: all attributes
         :rtype: list of str
         """
         return [a for a in dir(self) if (not callable(getattr(self, a)) and not a.startswith("_"))]
 
     def _getAttribsSave(self):
         """
@@ -1139,15 +1131,15 @@
             rdk.setParam(param_val, bytes_data)
             rdk.setParam(param_backup, b'')
 
     def Load(self, rdk=None):
         """
         Load the class attributes from a RoboDK binary parameter.
         If the station is not provided, it uses the active station.
-        
+
         :param rdk: Station to load from, defaults to None
         :type rdk: Robolink, optional
 
         :return: True if it succeeds, else false.
         """
         # Use a dictionary and the str/eval buit-in conversion
         attribs_list = self._getAttribsSave()
@@ -1256,14 +1248,17 @@
         if fields_value is None:
             # User cancelled
             return False
 
         # Apply the new values
         desc_value_inv = {v: k for k, v in attrib_desc.items()}
         for desc, value in fields_value.items():
+            if desc.endswith('$') and desc.startswith('$'):
+                # Section header
+                continue
             attrib = desc_value_inv[desc]
             setattr(self, attrib, value)
 
         # And store them to the station
         self.Save()
         return True
 
@@ -1335,14 +1330,17 @@
 
                     icon_window = QtWidgets.QDialog()
                     icon_window.setWindowTitle('RoboDK Icons')
                     icon_window.setWindowFlag(QtCore.Qt.WindowType.WindowStaysOnTopHint, True)
                     icon_window.setLayout(QtWidgets.QVBoxLayout())
                     icon_window.layout().addWidget(scroll_widget)
                     icon_window.exec_()
+                else:
+                    from robodk import robodialogs
+                    robodialogs.ShowMessage('No icons to display! Is the plug-in enabled?')
 
             actions = [("Show a Yes/No Message", showMessage), ("Show RoboDK Icons", showIcons)]
 
             return super(SettingsExample, self).ShowUI(actions=actions, *args, **kwargs)
 
     S = SettingsExample()
     S.Load()  # Load previously stored settings in the station
@@ -1350,16 +1348,14 @@
     S.INT = -123456  # Manually change a value
     S.Save()  # Manually save it
     S.Erase()  # Remove all data from the station
 
 
 def runmain():
 
-    from robodk import robodialogs
-
     ShowExample()
 
     if robodialogs.ENABLE_QT:
         robodialogs.ENABLE_QT = False
         ShowExample()
```

## robodk/robodialogs.py

```diff
@@ -17,21 +17,42 @@
 #
 # More information about the RoboDK API for Python here:
 #     https://robodk.com/doc/en/RoboDK-API.html
 #     https://robodk.com/doc/en/PythonAPI/index.html
 #
 # --------------------------------------------
 
-if 'ENABLE_TK' not in globals():
-    global ENABLE_TK
-    ENABLE_TK = True
+import sys
 
-if 'ENABLE_QT' not in globals():
-    global ENABLE_QT
+# robodialogs is compatible with PySide2 and tkinter. At least one must be present.
+ENABLE_QT = False
+try:
+    from PySide2 import QtWidgets, QtCore
     ENABLE_QT = True
+except:
+    pass
+
+ENABLE_TK = False
+try:
+    if sys.version_info[0] < 3:
+        import Tkinter as tkinter
+        import tkFileDialog as filedialog
+        import tkMessageBox as messagebox
+    else:
+        import tkinter
+        from tkinter import filedialog
+        from tkinter import messagebox
+    ENABLE_TK = True
+except:
+    pass
+
+if not ENABLE_TK and not ENABLE_QT:
+    s = 'PySide2 and/or tkinter is not present on the system. Please install PySide2: "python -m pip install PySide2" or "python -m pip install robodk[apps]"'
+    print(s)
+    #raise ImportError(s)
 
 FILE_TYPES_ALL = ('All Files', '.*')  #: File type filter for all files
 FILE_TYPES_ROBODK = ('RoboDK Files', '.sld .rdk .robot .tool .rdka .rdkbak .rdkp .py')  #: File type filter for RoboDK files
 FILE_TYPES_3D_OBJECT = ('3D Object Files', '.sld .stl .iges .igs .step .stp .obj .slp .3ds .dae .blend .wrl .wrml')  #: File type filter for 3D object files
 FILE_TYPES_TEXT = ('Text Files', '.txt .csv')  #: File type filter for text files
 FILE_TYPES_IMG = ('Image Files', '.png .jpg')  #: File type filter for image files
 FILE_TYPES_CAM = ('CAM Files', '.cnc .nc .apt .gcode .ngc .nci .anc .dxf .aptsource .cls .acl .cl .clt .ncl .knc')  #: File type filter for CAD/CAM files
@@ -358,125 +379,106 @@
 
 
 def _message_to_window_title(message):
     return message.split('\n', 1)[0].split('.', 1)[0].split(':', 1)[0]
 
 
 if ENABLE_TK:
-    import sys
-    if sys.version_info[0] < 3:
-        # Python 2.X only:
-        try:
-            import Tkinter as tkinter
-            import tkFileDialog as filedialog
-            import tkMessageBox as messagebox
-        except:
-            ENABLE_TK = False
-    else:
-        # Python 3.x only
-        try:
-            import tkinter
-            from tkinter import filedialog
-            from tkinter import messagebox
-        except:
-            ENABLE_TK = False
-
-if ENABLE_TK:
 
     from robodk.roboapps import get_tk_app, value_to_tk_widget, widget_to_value
 
     class DialogsTk:
 
         @staticmethod
         def getOpenFile(path_preference=DEFAULT_FOLDER, strfile='', strtitle='Open File', defaultextension=DEFAULT_FILE_EXT, filetypes=DEFAULT_FILE_TYPES):
             options = {}
             options['initialdir'] = path_preference
             options['title'] = strtitle
             options['defaultextension'] = defaultextension
             options['filetypes'] = filetypes
             options['initialfile'] = strfile
-            root = get_tk_app()
+            root = get_tk_app(robodk_theme=False)
             root.withdraw()
             root.attributes("-topmost", True)
             file_path = filedialog.askopenfile(**options)
             return file_path
 
         @staticmethod
         def getSaveFile(path_preference=DEFAULT_FOLDER, strfile='', strtitle='Save As', defaultextension=DEFAULT_FILE_EXT, filetypes=DEFAULT_FILE_TYPES):
             options = {}
             options['initialdir'] = path_preference
             options['title'] = strtitle
             options['defaultextension'] = defaultextension
             options['filetypes'] = filetypes
             options['initialfile'] = strfile
-            root = get_tk_app()
+            root = get_tk_app(robodk_theme=False)
             root.withdraw()
             root.attributes("-topmost", True)
             file_path = filedialog.asksaveasfile(**options)
             return file_path
 
         @staticmethod
         def getOpenFileName(path_preference=DEFAULT_FOLDER, strfile='', strtitle='Open File', defaultextension=DEFAULT_FILE_EXT, filetypes=DEFAULT_FILE_TYPES):
             options = {}
             options['initialdir'] = path_preference
             options['title'] = strtitle
             options['defaultextension'] = defaultextension
             options['filetypes'] = filetypes
             options['initialfile'] = strfile
-            root = get_tk_app()
+            root = get_tk_app(robodk_theme=False)
             root.withdraw()
             root.attributes("-topmost", True)
             file_path = filedialog.askopenfilename(**options)
             return file_path
 
         @staticmethod
         def getOpenFileNames(path_preference=DEFAULT_FOLDER, strfile='', strtitle='Open File(s)', defaultextension=DEFAULT_FILE_EXT, filetypes=DEFAULT_FILE_TYPES):
             options = {}
             options['initialdir'] = path_preference
             options['title'] = strtitle
             options['defaultextension'] = defaultextension
             options['filetypes'] = filetypes
             options['initialfile'] = strfile
-            root = get_tk_app()
+            root = get_tk_app(robodk_theme=False)
             root.withdraw()
             root.attributes("-topmost", True)
             file_path = filedialog.askopenfilenames(**options)
             return file_path
 
         @staticmethod
         def getSaveFileName(path_preference=DEFAULT_FOLDER, strfile='', strtitle='Save As', defaultextension=DEFAULT_FILE_EXT, filetypes=DEFAULT_FILE_TYPES):
             options = {}
             options['initialdir'] = path_preference
             options['title'] = strtitle
             options['defaultextension'] = defaultextension
             options['filetypes'] = filetypes
             options['initialfile'] = strfile
-            root = get_tk_app()
+            root = get_tk_app(robodk_theme=False)
             root.withdraw()
             root.attributes("-topmost", True)
             file_path = filedialog.asksaveasfilename(**options)
             return file_path
 
         @staticmethod
         def getOpenFolder(path_preference=DEFAULT_FOLDER, strtitle='Open Folder'):
             options = {}
             options['title'] = strtitle
             options['initialdir'] = path_preference
-            root = get_tk_app()
+            root = get_tk_app(robodk_theme=False)
             root.withdraw()
             root.attributes("-topmost", True)
             file_path = filedialog.askdirectory(**options)
             return file_path
 
         @staticmethod
         def getSaveFolder(path_preference=DEFAULT_FOLDER, strtitle='Save to Folder'):
             options = {}
             options['title'] = strtitle
             options['initialdir'] = path_preference
-            root = get_tk_app()
+            root = get_tk_app(robodk_theme=False)
             root.withdraw()
             root.attributes("-topmost", True)
             file_path = filedialog.askdirectory(**options)
             return file_path
 
         @staticmethod
         def ShowMessage(msg, title=None):
@@ -747,22 +749,14 @@
             msgbox.root.mainloop()
             # the function pauses here until the mainloop is quit
             msgbox.root.destroy()
             return msgbox.returning
 
 
 if ENABLE_QT:
-    try:
-        from robodk.robolink import import_install
-        import_install("PySide2", "PySide2==5.15.*")
-        from PySide2 import QtCore, QtWidgets
-    except:
-        ENABLE_QT = False
-
-if ENABLE_QT:
 
     from robodk.roboapps import get_qt_app, value_to_qt_widget, widget_to_value
 
     class DialogsQt:
 
         @staticmethod
         def convert_filetypes(filetypes, defaultextension=None):
@@ -779,42 +773,42 @@
                 if defaultextension in exts:
                     defaultextension_qt = f
 
             return ';;'.join(filetypes_qt), defaultextension_qt
 
         @staticmethod
         def getOpenFileName(path_preference=DEFAULT_FOLDER, strfile='', strtitle='Open File', defaultextension=DEFAULT_FILE_EXT, filetypes=DEFAULT_FILE_TYPES):
-            app = get_qt_app()
+            app = get_qt_app(robodk_theme=False)
             filetypes, defaultextension = DialogsQt.convert_filetypes(filetypes, defaultextension)
             file, ext = QtWidgets.QFileDialog.getOpenFileName(None, strtitle, path_preference if not strfile else path_preference + "/" + strfile, filetypes, defaultextension)
             return file if file else None
 
         @staticmethod
         def getOpenFileNames(path_preference=DEFAULT_FOLDER, strfile='', strtitle='Open File(s)', defaultextension=DEFAULT_FILE_EXT, filetypes=DEFAULT_FILE_TYPES):
-            app = get_qt_app()
+            app = get_qt_app(robodk_theme=False)
             filetypes, defaultextension = DialogsQt.convert_filetypes(filetypes, defaultextension)
             file, ext = QtWidgets.QFileDialog.getOpenFileNames(None, strtitle, path_preference if not strfile else path_preference + "/" + strfile, filetypes, defaultextension)
             return file if file else None
 
         @staticmethod
         def getSaveFileName(path_preference=DEFAULT_FOLDER, strfile='', strtitle='Save As', defaultextension=DEFAULT_FILE_EXT, filetypes=DEFAULT_FILE_TYPES):
-            app = get_qt_app()
+            app = get_qt_app(robodk_theme=False)
             filetypes, defaultextension = DialogsQt.convert_filetypes(filetypes, defaultextension)
             file, ext = QtWidgets.QFileDialog.getSaveFileName(None, strtitle, path_preference if not strfile else path_preference + "/" + strfile, filetypes, defaultextension)
             return file if file else None
 
         @staticmethod
         def getOpenFolder(path_preference=DEFAULT_FOLDER, strtitle='Open Folder'):
-            app = get_qt_app()
+            app = get_qt_app(robodk_theme=False)
             file = QtWidgets.QFileDialog.getExistingDirectory(None, strtitle, path_preference, QtWidgets.QFileDialog.ShowDirsOnly)
             return file if file else None
 
         @staticmethod
         def getSaveFolder(path_preference=DEFAULT_FOLDER, strtitle='Save to Folder'):
-            app = get_qt_app()
+            app = get_qt_app(robodk_theme=False)
             file = QtWidgets.QFileDialog.getExistingDirectory(None, strtitle, path_preference, QtWidgets.QFileDialog.ShowDirsOnly)
             return file if file else None
 
         @staticmethod
         def ShowMessage(msg, title=None):
             print(msg)
             if title is None:
```

## robodk/robofileio.py

```diff
@@ -22,15 +22,15 @@
 # --------------------------------------------
 
 import sys
 import time
 import os.path
 import time
 
-from . import robomath
+from robodk import robomath
 
 #----------------------------------------------------
 #--------      Generic file usage     ---------------
 
 
 def searchfiles(pattern='C:\\RoboDK\\Library\\*.rdk'):
     """List the files in a directory with a given extension"""
```

## robodk/robolink.py

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015-2022 - RoboDK Inc. - https://robodk.com/
+# Copyright 2015-2023 - RoboDK Inc. - https://robodk.com/
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 # http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
@@ -480,15 +480,15 @@
     iconpath = getPathRoboDK()
     if iconpath.endswith(".exe"):
         iconpath = iconpath[:-4]
     iconpath = iconpath + '.ico'
     return iconpath
 
 
-def import_install(module_name, pip_name=None, rdk=None, upgrade_pip=True):
+def import_install(module_name, pip_name=None, rdk=None, upgrade_pip=False):
     """Import a module by first installing it if the corresponding package is not available. If the module name does not match the pip install command, provide the pip_name for install purposes.
     Optionally, you can pass the RoboDK API Robolink object to see install progress in RoboDK's status bar.
 
     .. code-block:: python
 
         # If you want to install opencv for Python and pyserial you should use:
         import_install("opencv", "opencv-python", RDK)
@@ -504,15 +504,14 @@
 
     """
     try:
         exec('import ' + module_name, globals())
         return
 
     except ModuleNotFoundError:
-        import os
         import sys
         import subprocess
         import io
 
         def execute(cmd):
             print("Running command:")
             print(cmd)
@@ -1384,21 +1383,25 @@
 
                 elif i == 0:
                     if self.IP != 'localhost':
                         break
 
                     try:
                         if self.APPLICATION_DIR == '':
+                            if self.COM:
+                                self.COM = None
                             connected = 0
                             return connected
                         command = [self.APPLICATION_DIR]
                         if self.ARGUMENTS:
                             command += self.ARGUMENTS
 
                         if not start_robodk(command):
+                            if self.COM:
+                                self.COM = None
                             connected = 0
                             return connected
                         #import time
                         #time.sleep(5) # wait for RoboDK to start and check network license.
                     except Exception as e:
                         print(str(e))
                         raise Exception('Application path is not correct or could not start: ' + self.APPLICATION_DIR)
@@ -3609,17 +3612,15 @@
         .. seealso:: :func:`~robodk.robolink.Robolink.Spray_Add`, :func:`~robodk.robolink.Robolink.Spray_SetState`, :func:`~robodk.robolink.Robolink.Spray_Clear`
         """
         with self._lock:
             self._check_connection()
             command = 'Gun_Stats'
             self._send_line(command)
             self._send_int(id_spray)
-            info = self._rec_line()
-            info.replace('<br>', '\t')
-            print(info)
+            info = self._rec_line().replace('<br>', '\t')
             data = self._rec_matrix()
             self._check_status()
             return info, data
 
     def Spray_Clear(self, id_spray=-1):
         """Stops simulating a spray gun. This will clear the simulated particles.
 
@@ -4446,15 +4447,18 @@
                 self.link.COM.flush()
                 return self
 
             self.link._check_status()
             return self
 
     def Pose(self):
-        """Returns the relative pose of an object, target or reference frame. For example, the position of an object, target or reference frame with respect to its parent (the item it is attached to in the tree). For robot items, this function returns the pose of the active tool with respect to the active reference. It returns the pose as :class:`~robodk.robomath.Mat`.
+        """Returns the relative pose of an object, target or reference frame. For example, the position of an object, target or reference frame with respect to its parent (the item it is attached to in the tree).
+        For robot items, this function returns the pose of the active tool with respect to the active reference frame.
+
+        It returns the pose as :class:`~robodk.robomath.Mat`.
 
         Tip: Use a Pose_2_* function from the robodk module (such as :class:`robomath.Pose_2_KUKA`) to convert the pose to XYZABC (XYZ position in mm and ABC orientation in degrees), specific to a robot brand.
 
         Example: :ref:`weldexample`
 
         .. seealso:: :func:`~robodk.robolink.Item.Pose`, :func:`~robodk.robolink.Item.setPose`, :func:`~robodk.robolink.Item.PoseAbs`, :func:`~robodk.robolink.Item.PoseTool`, :func:`~robodk.robolink.Item.PoseFrame`, :func:`~robodk.robolink.Robolink.Item`
         """
@@ -4522,15 +4526,18 @@
                 self.link.COM.flush()
                 return self
 
             self.link._check_status()
             return self
 
     def PoseAbs(self):
-        """Return the pose (:class:`~robodk.robomath.Mat`) of this item with respect to the absolute reference frame (also know as the station reference or world coordinate system -WCS-). For example, the position of an object/frame/target with respect to the origin of the station.
+        """Return the pose (:class:`~robodk.robomath.Mat`) of this item with respect to the absolute reference frame (also know as the station reference or world coordinate system -WCS-).
+        For example, the position of an object/frame/target with respect to the origin of the station.
+
+        For robot items, this returns the pose of the robot base with respect to the origin of the station.
 
         Example:
 
         .. code-block:: python
 
             # Calculate the pose of any object with respect to any reference in RoboDK
             def CalculatePoseFrame2Object(frame, part):
@@ -6991,18 +6998,44 @@
                 command = 'S_ItmDataParam'
                 self.link._send_line(command)
                 self.link._send_item(self)
                 self.link._send_line(str(param))
                 self.link._send_bytes(value)
                 self.link._check_status()
                 return True
+
             elif isinstance(value, Item):
                 value = str(value.item)
+
             elif isinstance(value, bool):
                 value = '1' if value else '0'
+
+            elif isinstance(value, robomath.Mat):
+                # Special 2D matrix write/read
+                self.link._check_connection()
+                command = 'G_Gen_Mat'
+                self.link._send_line(command)
+                self.link._send_item(self)
+                self.link._send_line(str(param))
+                self.link._send_matrix(value)
+                self.link.COM.settimeout(3600)
+                nmats = self.link._rec_int()
+                self.link.COM.settimeout(self.link.TIMEOUT)
+                mat2d_list = []
+                if nmats == 1:
+                    mat2d_list = self.link._rec_matrix()
+                elif nmats == 0:
+                    mat2d_list = None
+                else:
+                    for i in range(nmats):
+                        mat2d_list.append(self.link._rec_matrix())
+
+                self.link._check_status()
+                return mat2d_list
+
             else:
                 value = str(value)
             value = value.replace('\n', '<br>')
 
             self.link._check_connection()
 
             # Skipstatus flag has no effect here
```

## robodk/robolinkutils.py

```diff
@@ -177,25 +177,22 @@
     :return: The pose from the source Item to the second Item
     :rtype: :class:`robomath.Mat`
     """
 
     if item1 == item2:
         return robomath.eye(4)
 
-    parents1 = getAncestors(item1)
-    if item2 in parents1:
-        return getAncestorPose(item1, item2)
-
-    parents2 = getAncestors(item2)
-    if item1 in parents2:
-        return getAncestorPose(item2, item1).inv()
-
-    lca = getLowestCommonAncestor(item1, item2)
-    pose1 = getAncestorPose(item1, lca)
-    pose2 = getAncestorPose(item2, lca)
+    pose1 = item1.PoseAbs()
+    pose2 = item2.PoseAbs()
+
+    if item1.Type() in [robolink.ITEM_TYPE_ROBOT, robolink.ITEM_TYPE_TOOL]:
+        pose1 = getAncestorPose(item1, item1.RDK().ActiveStation())
+
+    if item2.Type() in [robolink.ITEM_TYPE_ROBOT, robolink.ITEM_TYPE_TOOL]:
+        pose2 = getAncestorPose(item2, item2.RDK().ActiveStation())
 
     return pose2.inv() * pose1
 
 
 def setPoseAbsIK(item, pose_abs):
     """
     Set the pose of the item with respect to the absolute reference frame, accounting for inverse kinematics.
```

## robodk/robomath.py

```diff
@@ -232,45 +232,48 @@
 
 def point_Xaxis_2_pose(point, xaxis, zaxis_hint1=[0, 0, -1], zaxis_hint2=[0, -1, 0]):
     """Returns a pose given the origin as a point, a X axis and a preferred orientation for the Z axis"""
     pose = eye(4)
     pose.setPos(point)
     pose.setVX(xaxis)
     zaprox = zaxis_hint1
-    if abs(angle3(xaxis, zaprox)) < 0.03 or abs(angle3(xaxis, zaprox)) - pi < 0.03:
+    delta = abs(angle3(xaxis, zaprox))
+    if delta < 0.03 or abs(delta - pi) < 0.03:
         zaprox = zaxis_hint2
     yaxis = normalize3(cross(zaprox, xaxis))
     zaxis = cross(xaxis, yaxis)
     pose.setVY(yaxis)
     pose.setVZ(zaxis)
     return pose
 
 
 def point_Yaxis_2_pose(point, yaxis, zaxis_hint1=[0, 0, -1], zaxis_hint2=[-1, 0, 0]):
     """Returns a pose given the origin as a point, a Y axis and a preferred orientation for the Z axis"""
     pose = eye(4)
     pose.setPos(point)
     pose.setVY(yaxis)
     zaprox = zaxis_hint1
-    if abs(angle3(yaxis, zaprox)) < 0.03 or abs(angle3(yaxis, zaprox)) - pi < 0.03:
+    delta = abs(angle3(yaxis, zaprox))
+    if delta < 0.03 or abs(delta - pi) < 0.03:
         zaprox = zaxis_hint2
     xaxis = normalize3(cross(yaxis, zaprox))
     zaxis = cross(xaxis, yaxis)
     pose.setVX(xaxis)
     pose.setVZ(zaxis)
     return pose
 
 
 def point_Zaxis_2_pose(point, zaxis, yaxis_hint1=[0, 0, 1], yaxis_hint2=[0, 1, 1]):
     """Returns a pose given the origin as a point, a Z axis and a preferred orientation for the Y axis"""
     pose = eye(4)
     pose.setPos(point)
     pose.setVZ(zaxis)
     yaprox = yaxis_hint1
-    if abs(angle3(zaxis, yaprox)) < 0.03 or abs(angle3(zaxis, yaprox)) - pi < 0.03:
+    delta = abs(angle3(zaxis, yaprox))
+    if delta < 0.03 or abs(delta - pi) < 0.03:
         yaprox = yaxis_hint2
     xaxis = normalize3(cross(yaprox, zaxis))
     yaxis = cross(zaxis, xaxis)
     pose.setVX(xaxis)
     pose.setVY(yaxis)
     return pose
```

## Comparing `robodk-5.5.4.dist-info/LICENSE` & `robodk-5.5.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `robodk-5.5.4.dist-info/METADATA` & `robodk-5.5.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robodk
-Version: 5.5.4
+Version: 5.5.5
 Summary: RoboDK tools for simulating and programming industrial robots (implements the RoboDK API)
 Home-page: https://robodk.com/doc/en/PythonAPI/index.html
 Author: RoboDK Inc.
 Author-email: info@robodk.com
 License: Apache Software License
 Keywords: industrial robot,simulation,offline programming,robot programming,robotics,online programming,3D simulator,post processors
 Platform: UNKNOWN
@@ -28,19 +28,25 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: C
 Classifier: Programming Language :: C#
+Classifier: Programming Language :: C++
 Classifier: Programming Language :: Visual Basic
 Description-Content-Type: text/markdown
 Provides-Extra: apps
-Requires-Dist: PySide2 ; extra == 'apps'
+Requires-Dist: PySide2 (==5.15.*) ; extra == 'apps'
 Provides-Extra: cv
 Requires-Dist: opencv-contrib-python ; extra == 'cv'
 Requires-Dist: numpy ; extra == 'cv'
 Provides-Extra: lint
 Requires-Dist: astroid ; extra == 'lint'
 
 RoboDK API for Python
```

## Comparing `robodk-5.5.4.dist-info/RECORD` & `robodk-5.5.5.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 pylint_robodk/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pylint_robodk/pylint_robodk.py,sha256=iYjRh4qyQKnB-lTY_YJuRu8931imrzzKH9JLNwPUC1c,1551
 robodk/__init__.py,sha256=AKKmH90Q2slRJHJwWCjbPMdPDuU1Nm_bBTxH5HXHi18,1516
-robodk/roboapps.py,sha256=UaK7xQc5dEVtUWgSq3_vXd4mZDw86torHMzcaH6RoFk,52103
-robodk/robodialogs.py,sha256=G0BtVQ2U3fkKigNbgF04xVTFLumx9HVBC8Cylkre0Xo,45346
-robodk/robofileio.py,sha256=OGoU0dhoE0ddh86xM192qGBHMp4xHaY9uS9APUuvq2M,12497
-robodk/robolink.py,sha256=ulWqOayOa_V7T-Z0WnB45vYCt5OH7iRHFLLDdR40izs,325446
-robodk/robolinkutils.py,sha256=z6gicRia4KGecFIxxqBUq1E00WAixHCr8bWemZ0kxkI,10017
-robodk/robomath.py,sha256=7DBds7MhGs0sEUoKZsv5b_HqptB-Csa9dvsF6ZvvBKY,68433
+robodk/roboapps.py,sha256=4ASX0n1emCtszBBjVpaehUYwb0SVAbeJi1du2XrmTIs,52619
+robodk/robodialogs.py,sha256=bZbt3iekQpmHHTQDRiEOxm_lOBFBpP4z1INssN5QMIM,45464
+robodk/robofileio.py,sha256=bECjUE05RKE-9uGRexOinYKrOV4dsLrLzPKt4YcLfqg,12502
+robodk/robolink.py,sha256=XicOC2gllTTxzjR5l8wVEtdiMuxjbdGHhO36n7TXgSs,326660
+robodk/robolinkutils.py,sha256=mGfOtayuhnLlFHFy1hvaK52NbeunH-e-MWabKfUrG9M,10012
+robodk/robomath.py,sha256=V_zrtpTaamR9QP1TAgEbL3rInzgDRfx2QgHAzXL-nC8,68442
 robolink/__init__.py,sha256=RqchTjeRBU7Hnko58B9xHigsffzo9R6nlNs83zA5NhU,1210
-robodk-5.5.4.dist-info/LICENSE,sha256=D5sOGFtT_R0frDUaM9bm7RVnQJ_G2ivMdr1DRZCu8WU,587
-robodk-5.5.4.dist-info/METADATA,sha256=hAiz1teX0QmH2UtRljPRfHlTkpP9cAu8HIxxTxQwNO0,12419
-robodk-5.5.4.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-robodk-5.5.4.dist-info/top_level.txt,sha256=3CTL620vD_h4LfM0G4AXCDqkk8qr2UpQZMQU_gYi9Sc,30
-robodk-5.5.4.dist-info/RECORD,,
+robodk-5.5.5.dist-info/LICENSE,sha256=D5sOGFtT_R0frDUaM9bm7RVnQJ_G2ivMdr1DRZCu8WU,587
+robodk-5.5.5.dist-info/METADATA,sha256=CcsHXlrCasL0HJEqvTKfBvkQRy8iMfPoEul2q7j1xuI,12710
+robodk-5.5.5.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+robodk-5.5.5.dist-info/top_level.txt,sha256=3CTL620vD_h4LfM0G4AXCDqkk8qr2UpQZMQU_gYi9Sc,30
+robodk-5.5.5.dist-info/RECORD,,
```

