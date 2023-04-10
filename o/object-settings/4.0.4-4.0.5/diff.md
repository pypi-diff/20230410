# Comparing `tmp/object-settings-4.0.4.tar.gz` & `tmp/object-settings-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "object-settings-4.0.4.tar", last modified: Fri Mar 10 16:45:47 2023, max compression
+gzip compressed data, was "object-settings-4.0.5.tar", last modified: Mon Apr 10 16:35:08 2023, max compression
```

## Comparing `object-settings-4.0.4.tar` & `object-settings-4.0.5.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-03-10 16:45:47.332949 object-settings-4.0.4/
--rw-r--r--   0 samu      (1000) samu      (1000)     5602 2023-03-10 16:45:47.331949 object-settings-4.0.4/PKG-INFO
--rw-r--r--   0 samu      (1000) samu      (1000)     4755 2023-03-09 17:49:33.000000 object-settings-4.0.4/README.md
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-03-10 16:45:47.320949 object-settings-4.0.4/object_settings.egg-info/
--rw-r--r--   0 samu      (1000) samu      (1000)     5602 2023-03-10 16:45:47.000000 object-settings-4.0.4/object_settings.egg-info/PKG-INFO
--rw-r--r--   0 samu      (1000) samu      (1000)     1193 2023-03-10 16:45:47.000000 object-settings-4.0.4/object_settings.egg-info/SOURCES.txt
--rw-r--r--   0 samu      (1000) samu      (1000)        1 2023-03-10 16:45:47.000000 object-settings-4.0.4/object_settings.egg-info/dependency_links.txt
--rw-r--r--   0 samu      (1000) samu      (1000)       22 2023-03-10 16:45:47.000000 object-settings-4.0.4/object_settings.egg-info/requires.txt
--rw-r--r--   0 samu      (1000) samu      (1000)       22 2023-03-10 16:45:47.000000 object-settings-4.0.4/object_settings.egg-info/top_level.txt
--rw-r--r--   0 samu      (1000) samu      (1000)     1136 2023-03-10 16:45:28.000000 object-settings-4.0.4/pyproject.toml
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-03-10 16:45:47.321949 object-settings-4.0.4/settings/
--rw-r--r--   0 samu      (1000) samu      (1000)      389 2023-03-04 19:26:29.000000 object-settings-4.0.4/settings/__init__.py
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-03-10 16:45:47.323949 object-settings-4.0.4/settings/backend/
--rw-r--r--   0 samu      (1000) samu      (1000)      114 2023-03-09 16:08:28.000000 object-settings-4.0.4/settings/backend/__init__.py
--rw-r--r--   0 samu      (1000) samu      (1000)     1909 2023-03-09 17:10:15.000000 object-settings-4.0.4/settings/backend/config.py
--rw-r--r--   0 samu      (1000) samu      (1000)      714 2023-03-09 16:38:43.000000 object-settings-4.0.4/settings/backend/datatype_loader.py
--rw-r--r--   0 samu      (1000) samu      (1000)     1494 2023-03-09 16:08:28.000000 object-settings-4.0.4/settings/backend/main.py
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-03-10 16:45:47.325949 object-settings-4.0.4/settings/backend/parsers/
--rw-r--r--   0 samu      (1000) samu      (1000)      235 2023-03-09 16:25:34.000000 object-settings-4.0.4/settings/backend/parsers/__init__.py
--rw-r--r--   0 samu      (1000) samu      (1000)      848 2023-03-09 14:41:43.000000 object-settings-4.0.4/settings/backend/parsers/_template.py
--rw-r--r--   0 samu      (1000) samu      (1000)      839 2023-03-09 16:10:26.000000 object-settings-4.0.4/settings/backend/parsers/cli.py
--rw-r--r--   0 samu      (1000) samu      (1000)      812 2023-03-09 14:41:43.000000 object-settings-4.0.4/settings/backend/parsers/env.py
--rw-r--r--   0 samu      (1000) samu      (1000)     2213 2023-03-10 16:44:26.000000 object-settings-4.0.4/settings/backend/parsers/files.py
--rw-r--r--   0 samu      (1000) samu      (1000)     3373 2023-03-09 17:10:15.000000 object-settings-4.0.4/settings/base.py
--rw-r--r--   0 samu      (1000) samu      (1000)     4411 2023-03-03 16:47:09.000000 object-settings-4.0.4/settings/types.py
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-03-10 16:45:47.326949 object-settings-4.0.4/settings_gui/
--rw-r--r--   0 samu      (1000) samu      (1000)      231 2023-03-04 11:44:09.000000 object-settings-4.0.4/settings_gui/__init__.py
--rw-r--r--   0 samu      (1000) samu      (1000)      338 2022-12-16 13:11:05.000000 object-settings-4.0.4/settings_gui/_tk_abstractor.py
--rw-r--r--   0 samu      (1000) samu      (1000)      279 2023-03-04 22:40:29.000000 object-settings-4.0.4/settings_gui/config.py
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-03-10 16:45:47.327949 object-settings-4.0.4/settings_gui/tkinter/
--rw-r--r--   0 samu      (1000) samu      (1000)      343 2023-03-04 11:44:09.000000 object-settings-4.0.4/settings_gui/tkinter/__init__.py
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-03-10 16:45:47.329949 object-settings-4.0.4/settings_gui/tkinter/icons/
--rw-r--r--   0 samu      (1000) samu      (1000)      206 2015-11-19 10:52:05.000000 object-settings-4.0.4/settings_gui/tkinter/icons/checkmark-black.png
--rw-r--r--   0 samu      (1000) samu      (1000)     4826 2022-10-23 18:33:29.000000 object-settings-4.0.4/settings_gui/tkinter/icons/checkmark-white.png
--rw-r--r--   0 samu      (1000) samu      (1000)      333 2015-11-19 10:51:50.000000 object-settings-4.0.4/settings_gui/tkinter/icons/error.png
--rw-r--r--   0 samu      (1000) samu      (1000)      301 2015-11-21 05:08:04.000000 object-settings-4.0.4/settings_gui/tkinter/icons/folder-black.png
--rw-r--r--   0 samu      (1000) samu      (1000)     5036 2022-10-23 16:12:53.000000 object-settings-4.0.4/settings_gui/tkinter/icons/folder-white.png
--rw-r--r--   0 samu      (1000) samu      (1000)     1417 2023-03-04 11:44:09.000000 object-settings-4.0.4/settings_gui/tkinter/main.py
--rw-r--r--   0 samu      (1000) samu      (1000)      708 2023-03-04 11:44:09.000000 object-settings-4.0.4/settings_gui/tkinter/section_frames.py
--rw-r--r--   0 samu      (1000) samu      (1000)     7619 2023-03-09 14:26:09.000000 object-settings-4.0.4/settings_gui/tkinter/type_frames.py
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-03-10 16:45:47.329949 object-settings-4.0.4/settings_gui/ttk/
--rw-r--r--   0 samu      (1000) samu      (1000)      719 2022-12-16 20:12:38.000000 object-settings-4.0.4/settings_gui/ttk/__init__.py
--rw-r--r--   0 samu      (1000) samu      (1000)       38 2023-03-10 16:45:47.332949 object-settings-4.0.4/setup.cfg
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-03-10 16:45:47.331949 object-settings-4.0.4/tests/
--rw-r--r--   0 samu      (1000) samu      (1000)      923 2023-03-09 16:25:34.000000 object-settings-4.0.4/tests/test_cli.py
--rw-r--r--   0 samu      (1000) samu      (1000)      797 2023-03-09 15:35:21.000000 object-settings-4.0.4/tests/test_datafiles.py
--rw-r--r--   0 samu      (1000) samu      (1000)      821 2023-03-09 16:25:34.000000 object-settings-4.0.4/tests/test_endurance.py
--rw-r--r--   0 samu      (1000) samu      (1000)      830 2023-03-09 14:52:24.000000 object-settings-4.0.4/tests/test_env.py
--rw-r--r--   0 samu      (1000) samu      (1000)     1715 2023-03-04 11:54:10.000000 object-settings-4.0.4/tests/test_gui_(manual).py
--rw-r--r--   0 samu      (1000) samu      (1000)     1108 2022-10-27 17:39:38.000000 object-settings-4.0.4/tests/test_v1_definitions.py
--rw-r--r--   0 samu      (1000) samu      (1000)     1466 2022-11-03 11:24:05.000000 object-settings-4.0.4/tests/test_validation.py
+drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-04-10 16:35:08.766898 object-settings-4.0.5/
+-rw-r--r--   0 samu      (1000) samu      (1000)     5602 2023-04-10 16:35:08.766898 object-settings-4.0.5/PKG-INFO
+-rw-r--r--   0 samu      (1000) samu      (1000)     4755 2023-03-09 17:49:33.000000 object-settings-4.0.5/README.md
+drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-04-10 16:35:08.760898 object-settings-4.0.5/object_settings.egg-info/
+-rw-r--r--   0 samu      (1000) samu      (1000)     5602 2023-04-10 16:35:08.000000 object-settings-4.0.5/object_settings.egg-info/PKG-INFO
+-rw-r--r--   0 samu      (1000) samu      (1000)     1223 2023-04-10 16:35:08.000000 object-settings-4.0.5/object_settings.egg-info/SOURCES.txt
+-rw-r--r--   0 samu      (1000) samu      (1000)        1 2023-04-10 16:35:08.000000 object-settings-4.0.5/object_settings.egg-info/dependency_links.txt
+-rw-r--r--   0 samu      (1000) samu      (1000)       22 2023-04-10 16:35:08.000000 object-settings-4.0.5/object_settings.egg-info/requires.txt
+-rw-r--r--   0 samu      (1000) samu      (1000)       22 2023-04-10 16:35:08.000000 object-settings-4.0.5/object_settings.egg-info/top_level.txt
+-rw-r--r--   0 samu      (1000) samu      (1000)     1136 2023-04-10 16:33:53.000000 object-settings-4.0.5/pyproject.toml
+drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-04-10 16:35:08.760898 object-settings-4.0.5/settings/
+-rw-r--r--   0 samu      (1000) samu      (1000)      389 2023-03-04 19:26:29.000000 object-settings-4.0.5/settings/__init__.py
+drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-04-10 16:35:08.761898 object-settings-4.0.5/settings/backend/
+-rw-r--r--   0 samu      (1000) samu      (1000)      114 2023-03-09 16:08:28.000000 object-settings-4.0.5/settings/backend/__init__.py
+-rw-r--r--   0 samu      (1000) samu      (1000)     1909 2023-03-09 17:10:15.000000 object-settings-4.0.5/settings/backend/config.py
+-rw-r--r--   0 samu      (1000) samu      (1000)      835 2023-04-10 16:29:41.000000 object-settings-4.0.5/settings/backend/datatype_loader.py
+-rw-r--r--   0 samu      (1000) samu      (1000)     1494 2023-03-09 16:08:28.000000 object-settings-4.0.5/settings/backend/main.py
+drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-04-10 16:35:08.762898 object-settings-4.0.5/settings/backend/parsers/
+-rw-r--r--   0 samu      (1000) samu      (1000)      235 2023-03-09 16:25:34.000000 object-settings-4.0.5/settings/backend/parsers/__init__.py
+-rw-r--r--   0 samu      (1000) samu      (1000)      848 2023-03-09 14:41:43.000000 object-settings-4.0.5/settings/backend/parsers/_template.py
+-rw-r--r--   0 samu      (1000) samu      (1000)      839 2023-03-09 16:10:26.000000 object-settings-4.0.5/settings/backend/parsers/cli.py
+-rw-r--r--   0 samu      (1000) samu      (1000)      812 2023-03-09 14:41:43.000000 object-settings-4.0.5/settings/backend/parsers/env.py
+-rw-r--r--   0 samu      (1000) samu      (1000)     2213 2023-03-10 16:44:26.000000 object-settings-4.0.5/settings/backend/parsers/files.py
+-rw-r--r--   0 samu      (1000) samu      (1000)     3373 2023-03-09 17:10:15.000000 object-settings-4.0.5/settings/base.py
+-rw-r--r--   0 samu      (1000) samu      (1000)     4411 2023-03-03 16:47:09.000000 object-settings-4.0.5/settings/types.py
+drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-04-10 16:35:08.762898 object-settings-4.0.5/settings_gui/
+-rw-r--r--   0 samu      (1000) samu      (1000)      231 2023-03-04 11:44:09.000000 object-settings-4.0.5/settings_gui/__init__.py
+-rw-r--r--   0 samu      (1000) samu      (1000)      338 2022-12-16 13:11:05.000000 object-settings-4.0.5/settings_gui/_tk_abstractor.py
+-rw-r--r--   0 samu      (1000) samu      (1000)      279 2023-03-04 22:40:29.000000 object-settings-4.0.5/settings_gui/config.py
+drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-04-10 16:35:08.763898 object-settings-4.0.5/settings_gui/tkinter/
+-rw-r--r--   0 samu      (1000) samu      (1000)      343 2023-03-04 11:44:09.000000 object-settings-4.0.5/settings_gui/tkinter/__init__.py
+drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-04-10 16:35:08.764898 object-settings-4.0.5/settings_gui/tkinter/icons/
+-rw-r--r--   0 samu      (1000) samu      (1000)      206 2015-11-19 10:52:05.000000 object-settings-4.0.5/settings_gui/tkinter/icons/checkmark-black.png
+-rw-r--r--   0 samu      (1000) samu      (1000)     4826 2022-10-23 18:33:29.000000 object-settings-4.0.5/settings_gui/tkinter/icons/checkmark-white.png
+-rw-r--r--   0 samu      (1000) samu      (1000)      333 2015-11-19 10:51:50.000000 object-settings-4.0.5/settings_gui/tkinter/icons/error.png
+-rw-r--r--   0 samu      (1000) samu      (1000)      301 2015-11-21 05:08:04.000000 object-settings-4.0.5/settings_gui/tkinter/icons/folder-black.png
+-rw-r--r--   0 samu      (1000) samu      (1000)     5036 2022-10-23 16:12:53.000000 object-settings-4.0.5/settings_gui/tkinter/icons/folder-white.png
+-rw-r--r--   0 samu      (1000) samu      (1000)     1417 2023-03-04 11:44:09.000000 object-settings-4.0.5/settings_gui/tkinter/main.py
+-rw-r--r--   0 samu      (1000) samu      (1000)      708 2023-03-04 11:44:09.000000 object-settings-4.0.5/settings_gui/tkinter/section_frames.py
+-rw-r--r--   0 samu      (1000) samu      (1000)     7619 2023-03-09 14:26:09.000000 object-settings-4.0.5/settings_gui/tkinter/type_frames.py
+drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-04-10 16:35:08.764898 object-settings-4.0.5/settings_gui/ttk/
+-rw-r--r--   0 samu      (1000) samu      (1000)      719 2022-12-16 20:12:38.000000 object-settings-4.0.5/settings_gui/ttk/__init__.py
+-rw-r--r--   0 samu      (1000) samu      (1000)       38 2023-04-10 16:35:08.766898 object-settings-4.0.5/setup.cfg
+drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-04-10 16:35:08.766898 object-settings-4.0.5/tests/
+-rw-r--r--   0 samu      (1000) samu      (1000)      923 2023-03-09 16:25:34.000000 object-settings-4.0.5/tests/test_cli.py
+-rw-r--r--   0 samu      (1000) samu      (1000)      797 2023-03-09 15:35:21.000000 object-settings-4.0.5/tests/test_datafiles.py
+-rw-r--r--   0 samu      (1000) samu      (1000)      791 2023-04-10 16:31:09.000000 object-settings-4.0.5/tests/test_datatype_loader.py
+-rw-r--r--   0 samu      (1000) samu      (1000)      821 2023-03-09 16:25:34.000000 object-settings-4.0.5/tests/test_endurance.py
+-rw-r--r--   0 samu      (1000) samu      (1000)      830 2023-03-09 14:52:24.000000 object-settings-4.0.5/tests/test_env.py
+-rw-r--r--   0 samu      (1000) samu      (1000)     1715 2023-03-04 11:54:10.000000 object-settings-4.0.5/tests/test_gui_(manual).py
+-rw-r--r--   0 samu      (1000) samu      (1000)     1108 2022-10-27 17:39:38.000000 object-settings-4.0.5/tests/test_v1_definitions.py
+-rw-r--r--   0 samu      (1000) samu      (1000)     1466 2022-11-03 11:24:05.000000 object-settings-4.0.5/tests/test_validation.py
```

### Comparing `object-settings-4.0.4/PKG-INFO` & `object-settings-4.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: object-settings
-Version: 4.0.4
+Version: 4.0.5
 Summary: Simple object-oriented config library, where your settings are objects
 License: MIT License
 Project-URL: Homepage, https://github.com/SamuLumio/object-settings
 Keywords: settings,setting,config,OOP,GUI
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `object-settings-4.0.4/README.md` & `object-settings-4.0.5/README.md`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.4/object_settings.egg-info/PKG-INFO` & `object-settings-4.0.5/object_settings.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: object-settings
-Version: 4.0.4
+Version: 4.0.5
 Summary: Simple object-oriented config library, where your settings are objects
 License: MIT License
 Project-URL: Homepage, https://github.com/SamuLumio/object-settings
 Keywords: settings,setting,config,OOP,GUI
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `object-settings-4.0.4/object_settings.egg-info/SOURCES.txt` & `object-settings-4.0.5/object_settings.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -28,12 +28,13 @@
 settings_gui/tkinter/icons/checkmark-white.png
 settings_gui/tkinter/icons/error.png
 settings_gui/tkinter/icons/folder-black.png
 settings_gui/tkinter/icons/folder-white.png
 settings_gui/ttk/__init__.py
 tests/test_cli.py
 tests/test_datafiles.py
+tests/test_datatype_loader.py
 tests/test_endurance.py
 tests/test_env.py
 tests/test_gui_(manual).py
 tests/test_v1_definitions.py
 tests/test_validation.py
```

### Comparing `object-settings-4.0.4/pyproject.toml` & `object-settings-4.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "object-settings"
-version = "4.0.4"
+version = "4.0.5"
 description = "Simple object-oriented config library, where your settings are objects"
 readme = "README.md"
 keywords = ["settings", "setting", "config", "OOP", "GUI"]
 urls = {"Homepage"="https://github.com/SamuLumio/object-settings"}
 license = {text="MIT License"}
 
 dependencies = [
```

### Comparing `object-settings-4.0.4/settings/backend/config.py` & `object-settings-4.0.5/settings/backend/config.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.4/settings/backend/datatype_loader.py` & `object-settings-4.0.5/settings/backend/datatype_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import configparser
 
 str_converter_functions = {
 	str: str,
 	int: int,
 	float: float,
-	bool: lambda string: configparser.ConfigParser.BOOLEAN_STATES[string],
+	bool: lambda string: configparser.ConfigParser.BOOLEAN_STATES[string.lower()],
 	list: lambda string: string.removeprefix("['").removesuffix("']").split("', '")
 }
 
 def get(data, output_type: type[str | int | float | bool | list]):
 	if isinstance(data, output_type):
 		return data
+	elif isinstance(data, float) and output_type == int:
+		return int(data)
 	elif isinstance(data, str) and output_type in str_converter_functions:
 		function = str_converter_functions[output_type]
 		return function(data)
 	else:
-		raise UnsupportedDataError(type(data))
+		raise UnsupportedDataError(type(data), output_type)
 
 
 class UnsupportedDataError(BaseException):
-	def __init__(self, data_type: type):
-		super().__init__(f"loading for source data type {data_type} is unsupported")
+	def __init__(self, data_type: type, wanted_type: type):
+		super().__init__(f"loading {data_type} source data as {wanted_type} is unsupported")
```

### Comparing `object-settings-4.0.4/settings/backend/main.py` & `object-settings-4.0.5/settings/backend/main.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.4/settings/backend/parsers/_template.py` & `object-settings-4.0.5/settings/backend/parsers/_template.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.4/settings/backend/parsers/cli.py` & `object-settings-4.0.5/settings/backend/parsers/cli.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.4/settings/backend/parsers/env.py` & `object-settings-4.0.5/settings/backend/parsers/env.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.4/settings/backend/parsers/files.py` & `object-settings-4.0.5/settings/backend/parsers/files.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.4/settings/base.py` & `object-settings-4.0.5/settings/base.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.4/settings/types.py` & `object-settings-4.0.5/settings/types.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.4/settings_gui/tkinter/icons/checkmark-white.png` & `object-settings-4.0.5/settings_gui/tkinter/icons/checkmark-white.png`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.4/settings_gui/tkinter/icons/folder-white.png` & `object-settings-4.0.5/settings_gui/tkinter/icons/folder-white.png`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.4/settings_gui/tkinter/main.py` & `object-settings-4.0.5/settings_gui/tkinter/main.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.4/settings_gui/tkinter/section_frames.py` & `object-settings-4.0.5/settings_gui/tkinter/section_frames.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.4/settings_gui/tkinter/type_frames.py` & `object-settings-4.0.5/settings_gui/tkinter/type_frames.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.4/settings_gui/ttk/__init__.py` & `object-settings-4.0.5/settings_gui/ttk/__init__.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.4/tests/test_cli.py` & `object-settings-4.0.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.4/tests/test_datafiles.py` & `object-settings-4.0.5/tests/test_datafiles.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.4/tests/test_endurance.py` & `object-settings-4.0.5/tests/test_endurance.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.4/tests/test_env.py` & `object-settings-4.0.5/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.4/tests/test_gui_(manual).py` & `object-settings-4.0.5/tests/test_gui_(manual).py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.4/tests/test_v1_definitions.py` & `object-settings-4.0.5/tests/test_v1_definitions.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.0.4/tests/test_validation.py` & `object-settings-4.0.5/tests/test_validation.py`

 * *Files identical despite different names*

