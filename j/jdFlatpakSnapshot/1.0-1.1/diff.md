# Comparing `tmp/jdFlatpakSnapshot-1.0.tar.gz` & `tmp/jdFlatpakSnapshot-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdFlatpakSnapshot-1.0.tar", last modified: Mon Apr 10 14:55:25 2023, max compression
+gzip compressed data, was "jdFlatpakSnapshot-1.1.tar", last modified: Mon Apr 10 15:06:34 2023, max compression
```

## Comparing `jdFlatpakSnapshot-1.0.tar` & `jdFlatpakSnapshot-1.1.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-10 14:55:25.858639 jdFlatpakSnapshot-1.0/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     2879 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/BuildBackend.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)    35075 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/LICENSE
--rw-r--r--   0 jakob     (1000) jakob     (1000)      227 2023-04-10 14:55:11.000000 jdFlatpakSnapshot-1.0/MANIFEST.in
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1148 2023-04-10 14:55:25.858639 jdFlatpakSnapshot-1.0/PKG-INFO
--rw-r--r--   0 jakob     (1000) jakob     (1000)       66 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/README.md
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-10 14:55:25.858639 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/
--rw-r--r--   0 jakob     (1000) jakob     (1000)      547 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/AboutDialog.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)      577 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/Constants.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1754 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/Environment.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1359 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/FlatpakHandler.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     2756 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/Functions.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     5611 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/ImportExport.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)    13658 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/MainWindow.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1328 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/ProgressDialog.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1426 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/Settings.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     2726 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/SettingsDialog.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)      263 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/Types.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)      700 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/WelcomeDialog.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1972 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/__init__.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)        2 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/__main__.py
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-10 14:55:25.858639 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/icons/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     3101 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/icons/app-icon.svg
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1181 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/icons/default-icon.svg
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-10 14:55:25.858639 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/translations/
--rw-r--r--   0 jakob     (1000) jakob     (1000)    19882 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_de.ts
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-10 14:55:25.858639 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/ui/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     2287 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/ui/AboutDialog.ui
--rw-r--r--   0 jakob     (1000) jakob     (1000)     5626 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/ui/MainWindow.ui
--rw-r--r--   0 jakob     (1000) jakob     (1000)      880 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/ui/ProgressDialog.ui
--rw-r--r--   0 jakob     (1000) jakob     (1000)     3221 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/ui/SettingsDialog.ui
--rw-r--r--   0 jakob     (1000) jakob     (1000)     3642 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/ui/WelcomeDialog.ui
--rw-r--r--   0 jakob     (1000) jakob     (1000)        3 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/version.txt
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-10 14:55:25.858639 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot.egg-info/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1148 2023-04-10 14:55:25.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot.egg-info/PKG-INFO
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1112 2023-04-10 14:55:25.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot.egg-info/SOURCES.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)        1 2023-04-10 14:55:25.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot.egg-info/dependency_links.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)       57 2023-04-10 14:55:25.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot.egg-info/entry_points.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)       24 2023-04-10 14:55:25.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot.egg-info/requires.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)       18 2023-04-10 14:55:25.000000 jdFlatpakSnapshot-1.0/jdFlatpakSnapshot.egg-info/top_level.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1413 2023-04-10 14:54:24.000000 jdFlatpakSnapshot-1.0/pyproject.toml
--rw-r--r--   0 jakob     (1000) jakob     (1000)       38 2023-04-10 14:55:25.858639 jdFlatpakSnapshot-1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 15:06:34.811073 jdFlatpakSnapshot-1.1/
+-rw-r--r--   0 root         (0) root         (0)     2879 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/BuildBackend.py
+-rw-r--r--   0 root         (0) root         (0)    35075 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      227 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-04-10 15:06:34.811073 jdFlatpakSnapshot-1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       66 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 15:06:34.807073 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/
+-rw-r--r--   0 root         (0) root         (0)      547 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/AboutDialog.py
+-rw-r--r--   0 root         (0) root         (0)      577 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/Constants.py
+-rw-r--r--   0 root         (0) root         (0)     1754 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/Environment.py
+-rw-r--r--   0 root         (0) root         (0)     1359 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/FlatpakHandler.py
+-rw-r--r--   0 root         (0) root         (0)     2756 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/Functions.py
+-rw-r--r--   0 root         (0) root         (0)     5611 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ImportExport.py
+-rw-r--r--   0 root         (0) root         (0)    13658 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/MainWindow.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ProgressDialog.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/Settings.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/SettingsDialog.py
+-rw-r--r--   0 root         (0) root         (0)      263 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/Types.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/WelcomeDialog.py
+-rw-r--r--   0 root         (0) root         (0)     1972 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        2 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 15:06:34.807073 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/icons/
+-rw-r--r--   0 root         (0) root         (0)     3101 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/icons/app-icon.svg
+-rw-r--r--   0 root         (0) root         (0)     1181 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/icons/default-icon.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 15:06:34.807073 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/translations/
+-rw-r--r--   0 root         (0) root         (0)    19882 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_de.ts
+-rw-r--r--   0 root         (0) root         (0)    19670 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_nl.ts
+-rw-r--r--   0 root         (0) root         (0)    19804 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_tr.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 15:06:34.807073 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ui/
+-rw-r--r--   0 root         (0) root         (0)     2287 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ui/AboutDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     5626 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ui/MainWindow.ui
+-rw-r--r--   0 root         (0) root         (0)      880 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ui/ProgressDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     3221 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ui/SettingsDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     3642 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ui/WelcomeDialog.ui
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 15:06:34.807073 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-04-10 15:06:34.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1222 2023-04-10 15:06:34.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 15:06:34.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-04-10 15:06:34.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-10 15:06:34.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-10 15:06:34.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 15:06:34.811073 jdFlatpakSnapshot-1.1/setup.cfg
```

### Comparing `jdFlatpakSnapshot-1.0/BuildBackend.py` & `jdFlatpakSnapshot-1.1/BuildBackend.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.0/LICENSE` & `jdFlatpakSnapshot-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.0/PKG-INFO` & `jdFlatpakSnapshot-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdFlatpakSnapshot
-Version: 1.0
+Version: 1.1
 Summary: A Program to create Snapshots of Flatpak Apps
 Author-email: JakobDev <jakobdev@gmx.de>
 License: GPL-3
 Project-URL: Source, https://codeberg.org/JakobDev/jdFlatpakSnaphot
 Project-URL: Issues, https://codeberg.org/JakobDev/jdFlatpakSnapshot/issues
 Project-URL: Donation, https://ko-fi.com/jakobdev
 Keywords: JakobDev,Linux,Flatpak
```

### Comparing `jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/AboutDialog.py` & `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/AboutDialog.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/Constants.py` & `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/Constants.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/Environment.py` & `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/Environment.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/FlatpakHandler.py` & `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/FlatpakHandler.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/Functions.py` & `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/Functions.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/ImportExport.py` & `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ImportExport.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/MainWindow.py` & `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/MainWindow.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/ProgressDialog.py` & `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ProgressDialog.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/Settings.py` & `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/Settings.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/SettingsDialog.py` & `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/SettingsDialog.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/WelcomeDialog.py` & `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/WelcomeDialog.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/__init__.py` & `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/__init__.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/icons/app-icon.svg` & `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/icons/app-icon.svg`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/icons/default-icon.svg` & `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/icons/default-icon.svg`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_de.ts` & `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_de.ts`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/ui/AboutDialog.ui` & `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ui/AboutDialog.ui`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/ui/MainWindow.ui` & `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ui/MainWindow.ui`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/ui/ProgressDialog.ui` & `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ui/ProgressDialog.ui`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/ui/SettingsDialog.ui` & `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ui/SettingsDialog.ui`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.0/jdFlatpakSnapshot/ui/WelcomeDialog.ui` & `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ui/WelcomeDialog.ui`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.0/jdFlatpakSnapshot.egg-info/PKG-INFO` & `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdFlatpakSnapshot
-Version: 1.0
+Version: 1.1
 Summary: A Program to create Snapshots of Flatpak Apps
 Author-email: JakobDev <jakobdev@gmx.de>
 License: GPL-3
 Project-URL: Source, https://codeberg.org/JakobDev/jdFlatpakSnaphot
 Project-URL: Issues, https://codeberg.org/JakobDev/jdFlatpakSnapshot/issues
 Project-URL: Donation, https://ko-fi.com/jakobdev
 Keywords: JakobDev,Linux,Flatpak
```

### Comparing `jdFlatpakSnapshot-1.0/jdFlatpakSnapshot.egg-info/SOURCES.txt` & `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -23,12 +23,14 @@
 jdFlatpakSnapshot.egg-info/dependency_links.txt
 jdFlatpakSnapshot.egg-info/entry_points.txt
 jdFlatpakSnapshot.egg-info/requires.txt
 jdFlatpakSnapshot.egg-info/top_level.txt
 jdFlatpakSnapshot/icons/app-icon.svg
 jdFlatpakSnapshot/icons/default-icon.svg
 jdFlatpakSnapshot/translations/jdFlatpakSnapshot_de.ts
+jdFlatpakSnapshot/translations/jdFlatpakSnapshot_nl.ts
+jdFlatpakSnapshot/translations/jdFlatpakSnapshot_tr.ts
 jdFlatpakSnapshot/ui/AboutDialog.ui
 jdFlatpakSnapshot/ui/MainWindow.ui
 jdFlatpakSnapshot/ui/ProgressDialog.ui
 jdFlatpakSnapshot/ui/SettingsDialog.ui
 jdFlatpakSnapshot/ui/WelcomeDialog.ui
```

### Comparing `jdFlatpakSnapshot-1.0/pyproject.toml` & `jdFlatpakSnapshot-1.1/pyproject.toml`

 * *Files identical despite different names*

