# Comparing `tmp/admin_tool_button-1.0.1a0.tar.gz` & `tmp/admin_tool_button-1.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "admin_tool_button-1.0.1a0.tar", last modified: Mon Apr 10 10:59:23 2023, max compression
+gzip compressed data, was "admin_tool_button-1.0.2a0.tar", last modified: Mon Apr 10 11:09:44 2023, max compression
```

## Comparing `admin_tool_button-1.0.1a0.tar` & `admin_tool_button-1.0.2a0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxr-x   0 bram      (1000) bram      (1000)        0 2023-04-10 10:59:23.362105 admin_tool_button-1.0.1a0/
--rw-rw-r--   0 bram      (1000) bram      (1000)      992 2023-04-10 10:59:23.362105 admin_tool_button-1.0.1a0/PKG-INFO
--rw-rw-r--   0 bram      (1000) bram      (1000)      642 2023-04-09 19:07:21.000000 admin_tool_button-1.0.1a0/README.md
-drwxrwxr-x   0 bram      (1000) bram      (1000)        0 2023-04-10 10:59:23.362105 admin_tool_button-1.0.1a0/admin_tool_button/
--rw-rw-r--   0 bram      (1000) bram      (1000)        1 2023-04-08 20:06:04.000000 admin_tool_button-1.0.1a0/admin_tool_button/__init__.py
--rw-rw-r--   0 bram      (1000) bram      (1000)      266 2023-04-08 20:06:04.000000 admin_tool_button-1.0.1a0/admin_tool_button/version.py
-drwxrwxr-x   0 bram      (1000) bram      (1000)        0 2023-04-10 10:59:23.362105 admin_tool_button-1.0.1a0/admin_tool_button.egg-info/
--rw-rw-r--   0 bram      (1000) bram      (1000)      992 2023-04-10 10:59:23.000000 admin_tool_button-1.0.1a0/admin_tool_button.egg-info/PKG-INFO
--rw-rw-r--   0 bram      (1000) bram      (1000)      321 2023-04-10 10:59:23.000000 admin_tool_button-1.0.1a0/admin_tool_button.egg-info/SOURCES.txt
--rw-rw-r--   0 bram      (1000) bram      (1000)        1 2023-04-10 10:59:23.000000 admin_tool_button-1.0.1a0/admin_tool_button.egg-info/dependency_links.txt
--rw-rw-r--   0 bram      (1000) bram      (1000)        1 2023-04-09 17:15:25.000000 admin_tool_button-1.0.1a0/admin_tool_button.egg-info/not-zip-safe
--rw-rw-r--   0 bram      (1000) bram      (1000)       51 2023-04-10 10:59:23.000000 admin_tool_button-1.0.1a0/admin_tool_button.egg-info/requires.txt
--rw-rw-r--   0 bram      (1000) bram      (1000)       18 2023-04-10 10:59:23.000000 admin_tool_button-1.0.1a0/admin_tool_button.egg-info/top_level.txt
--rw-rw-r--   0 bram      (1000) bram      (1000)       38 2023-04-10 10:59:23.362105 admin_tool_button-1.0.1a0/setup.cfg
--rw-rw-r--   0 bram      (1000) bram      (1000)      720 2023-04-10 10:58:46.000000 admin_tool_button-1.0.1a0/setup.py
+drwxrwxr-x   0 bram      (1000) bram      (1000)        0 2023-04-10 11:09:44.239140 admin_tool_button-1.0.2a0/
+-rw-rw-r--   0 bram      (1000) bram      (1000)      935 2023-04-10 11:09:44.239140 admin_tool_button-1.0.2a0/PKG-INFO
+-rw-rw-r--   0 bram      (1000) bram      (1000)      585 2023-04-10 11:05:04.000000 admin_tool_button-1.0.2a0/README.md
+drwxrwxr-x   0 bram      (1000) bram      (1000)        0 2023-04-10 11:09:44.235140 admin_tool_button-1.0.2a0/admin_tool_button/
+-rw-rw-r--   0 bram      (1000) bram      (1000)        1 2023-04-08 20:06:04.000000 admin_tool_button-1.0.2a0/admin_tool_button/__init__.py
+drwxrwxr-x   0 bram      (1000) bram      (1000)        0 2023-04-10 11:09:44.239140 admin_tool_button-1.0.2a0/admin_tool_button/contrib/
+-rw-rw-r--   0 bram      (1000) bram      (1000)        1 2023-04-08 20:06:04.000000 admin_tool_button-1.0.2a0/admin_tool_button/contrib/__init__.py
+-rw-rw-r--   0 bram      (1000) bram      (1000)     1488 2023-04-09 16:46:09.000000 admin_tool_button-1.0.2a0/admin_tool_button/contrib/admin.py
+-rw-rw-r--   0 bram      (1000) bram      (1000)      266 2023-04-08 20:06:04.000000 admin_tool_button-1.0.2a0/admin_tool_button/version.py
+drwxrwxr-x   0 bram      (1000) bram      (1000)        0 2023-04-10 11:09:44.239140 admin_tool_button-1.0.2a0/admin_tool_button.egg-info/
+-rw-rw-r--   0 bram      (1000) bram      (1000)      935 2023-04-10 11:09:44.000000 admin_tool_button-1.0.2a0/admin_tool_button.egg-info/PKG-INFO
+-rw-rw-r--   0 bram      (1000) bram      (1000)      394 2023-04-10 11:09:44.000000 admin_tool_button-1.0.2a0/admin_tool_button.egg-info/SOURCES.txt
+-rw-rw-r--   0 bram      (1000) bram      (1000)        1 2023-04-10 11:09:44.000000 admin_tool_button-1.0.2a0/admin_tool_button.egg-info/dependency_links.txt
+-rw-rw-r--   0 bram      (1000) bram      (1000)        1 2023-04-09 17:15:25.000000 admin_tool_button-1.0.2a0/admin_tool_button.egg-info/not-zip-safe
+-rw-rw-r--   0 bram      (1000) bram      (1000)       51 2023-04-10 11:09:44.000000 admin_tool_button-1.0.2a0/admin_tool_button.egg-info/requires.txt
+-rw-rw-r--   0 bram      (1000) bram      (1000)       18 2023-04-10 11:09:44.000000 admin_tool_button-1.0.2a0/admin_tool_button.egg-info/top_level.txt
+-rw-rw-r--   0 bram      (1000) bram      (1000)       38 2023-04-10 11:09:44.239140 admin_tool_button-1.0.2a0/setup.cfg
+-rw-rw-r--   0 bram      (1000) bram      (1000)      811 2023-04-10 11:09:02.000000 admin_tool_button-1.0.2a0/setup.py
```

### Comparing `admin_tool_button-1.0.1a0/PKG-INFO` & `admin_tool_button-1.0.2a0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: admin_tool_button
-Version: 1.0.1a0
+Version: 1.0.2a0
 Summary: Extra tool buttons for Django admin
 Home-page: https://github.com/bboogaard/admin_tool_button
 Author: Bram Boogaard
 Author-email: padawan@hetnet.nl
 License: MIT License
 Keywords: Django Admin
 Classifier: Development Status :: 3 - Alpha
@@ -23,15 +23,15 @@
 Supports: Python 3.9.
 
 Supports Django Versions: 3.2.
 
 ## Installation
 
 ```shell
-$ pip install https://github.com/bboogaard/admin_tool_button/archive/refs/heads/main.zip
+$ pip install admin_tool_button
 ```
 
 ## Usage
 
 Add `admin_tool_button` to `INSTALLED_APPS`. In your `admin.py` add your custom actions like so:
 
 ```python
```

### Comparing `admin_tool_button-1.0.1a0/admin_tool_button.egg-info/PKG-INFO` & `admin_tool_button-1.0.2a0/admin_tool_button.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: admin-tool-button
-Version: 1.0.1a0
+Version: 1.0.2a0
 Summary: Extra tool buttons for Django admin
 Home-page: https://github.com/bboogaard/admin_tool_button
 Author: Bram Boogaard
 Author-email: padawan@hetnet.nl
 License: MIT License
 Keywords: Django Admin
 Classifier: Development Status :: 3 - Alpha
@@ -23,15 +23,15 @@
 Supports: Python 3.9.
 
 Supports Django Versions: 3.2.
 
 ## Installation
 
 ```shell
-$ pip install https://github.com/bboogaard/admin_tool_button/archive/refs/heads/main.zip
+$ pip install admin_tool_button
 ```
 
 ## Usage
 
 Add `admin_tool_button` to `INSTALLED_APPS`. In your `admin.py` add your custom actions like so:
 
 ```python
```

