# Comparing `tmp/ssh_zone_handler-0.3.1.tar.gz` & `tmp/ssh_zone_handler-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_zone_handler-0.3.1.tar", max compression
+gzip compressed data, was "ssh_zone_handler-0.3.2.tar", max compression
```

## Comparing `ssh_zone_handler-0.3.1.tar` & `ssh_zone_handler-0.3.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1092 2022-10-29 09:04:45.756448 ssh_zone_handler-0.3.1/LICENSE
--rw-r--r--   0        0        0     2673 2023-04-08 07:21:08.928832 ssh_zone_handler-0.3.1/README.md
--rw-r--r--   0        0        0     1109 2023-04-08 07:45:58.511877 ssh_zone_handler-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      195 2022-10-29 09:04:45.756448 ssh_zone_handler-0.3.1/ssh_zone_handler/__init__.py
--rw-r--r--   0        0        0     6113 2023-04-08 07:45:58.511877 ssh_zone_handler-0.3.1/ssh_zone_handler/base.py
--rw-r--r--   0        0        0     3751 2022-11-26 11:59:52.153894 ssh_zone_handler-0.3.1/ssh_zone_handler/bind.py
--rw-r--r--   0        0        0     2889 2022-11-26 11:59:52.153894 ssh_zone_handler-0.3.1/ssh_zone_handler/cli.py
--rw-r--r--   0        0        0     3048 2022-11-26 11:59:52.153894 ssh_zone_handler-0.3.1/ssh_zone_handler/knot.py
--rw-r--r--   0        0        0      862 2022-10-29 09:04:45.756448 ssh_zone_handler-0.3.1/ssh_zone_handler/static.py
--rw-r--r--   0        0        0     1377 2022-11-26 11:59:52.153894 ssh_zone_handler-0.3.1/ssh_zone_handler/types.py
--rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 ssh_zone_handler-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-10 19:23:17.011134 ssh_zone_handler-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2673 2023-04-10 19:23:17.011134 ssh_zone_handler-0.3.2/README.md
+-rw-r--r--   0        0        0     1109 2023-04-10 19:23:17.015134 ssh_zone_handler-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      195 2023-04-10 19:23:17.015134 ssh_zone_handler-0.3.2/ssh_zone_handler/__init__.py
+-rw-r--r--   0        0        0     6113 2023-04-10 19:23:17.015134 ssh_zone_handler-0.3.2/ssh_zone_handler/base.py
+-rw-r--r--   0        0        0     3751 2023-04-10 19:23:17.015134 ssh_zone_handler-0.3.2/ssh_zone_handler/bind.py
+-rw-r--r--   0        0        0     2889 2023-04-10 19:23:17.015134 ssh_zone_handler-0.3.2/ssh_zone_handler/cli.py
+-rw-r--r--   0        0        0     3048 2023-04-10 19:23:17.015134 ssh_zone_handler-0.3.2/ssh_zone_handler/knot.py
+-rw-r--r--   0        0        0      862 2023-04-10 19:23:17.015134 ssh_zone_handler-0.3.2/ssh_zone_handler/static.py
+-rw-r--r--   0        0        0     1377 2023-04-10 19:23:17.015134 ssh_zone_handler-0.3.2/ssh_zone_handler/types.py
+-rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 ssh_zone_handler-0.3.2/PKG-INFO
```

### Comparing `ssh_zone_handler-0.3.1/LICENSE` & `ssh_zone_handler-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ssh_zone_handler-0.3.1/README.md` & `ssh_zone_handler-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ssh_zone_handler-0.3.1/pyproject.toml` & `ssh_zone_handler-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssh-zone-handler"
-version = "0.3.1"
+version = "0.3.2"
 description = "SSH commands to provide Secondary DNS self-service."
 readme = "README.md"
 license = "MIT"
 authors = ["Andreas Olsson <andreas@arrakis.se>"]
 repository = "https://github.com/andreaso/ssh-zone-handler"
 
 [tool.poetry.dependencies]
```

### Comparing `ssh_zone_handler-0.3.1/ssh_zone_handler/base.py` & `ssh_zone_handler-0.3.2/ssh_zone_handler/base.py`

 * *Files identical despite different names*

### Comparing `ssh_zone_handler-0.3.1/ssh_zone_handler/bind.py` & `ssh_zone_handler-0.3.2/ssh_zone_handler/bind.py`

 * *Files identical despite different names*

### Comparing `ssh_zone_handler-0.3.1/ssh_zone_handler/cli.py` & `ssh_zone_handler-0.3.2/ssh_zone_handler/cli.py`

 * *Files identical despite different names*

### Comparing `ssh_zone_handler-0.3.1/ssh_zone_handler/knot.py` & `ssh_zone_handler-0.3.2/ssh_zone_handler/knot.py`

 * *Files identical despite different names*

### Comparing `ssh_zone_handler-0.3.1/ssh_zone_handler/static.py` & `ssh_zone_handler-0.3.2/ssh_zone_handler/static.py`

 * *Files identical despite different names*

### Comparing `ssh_zone_handler-0.3.1/ssh_zone_handler/types.py` & `ssh_zone_handler-0.3.2/ssh_zone_handler/types.py`

 * *Files identical despite different names*

### Comparing `ssh_zone_handler-0.3.1/PKG-INFO` & `ssh_zone_handler-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh-zone-handler
-Version: 0.3.1
+Version: 0.3.2
 Summary: SSH commands to provide Secondary DNS self-service.
 Home-page: https://github.com/andreaso/ssh-zone-handler
 License: MIT
 Author: Andreas Olsson
 Author-email: andreas@arrakis.se
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

