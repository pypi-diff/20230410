# Comparing `tmp/python_roborock-0.6.0.tar.gz` & `tmp/python_roborock-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_roborock-0.6.0.tar", max compression
+gzip compressed data, was "python_roborock-0.6.1.tar", max compression
```

## Comparing `python_roborock-0.6.0.tar` & `python_roborock-0.6.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-04-08 14:16:01.154481 python_roborock-0.6.0/LICENSE
--rw-r--r--   0        0        0     2221 2023-04-08 14:16:01.154481 python_roborock-0.6.0/README.md
--rw-r--r--   0        0        0     1175 2023-04-08 14:16:01.842494 python_roborock-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      300 2023-04-08 14:16:01.154481 python_roborock-0.6.0/roborock/__init__.py
--rw-r--r--   0        0        0    17099 2023-04-08 14:16:01.154481 python_roborock-0.6.0/roborock/api.py
--rw-r--r--   0        0        0     3957 2023-04-08 14:16:01.154481 python_roborock-0.6.0/roborock/cli.py
--rw-r--r--   0        0        0     8276 2023-04-08 14:16:01.154481 python_roborock-0.6.0/roborock/cloud_api.py
--rw-r--r--   0        0        0     3704 2023-04-08 14:16:01.154481 python_roborock-0.6.0/roborock/code_mappings.py
--rw-r--r--   0        0        0     9190 2023-04-08 14:16:01.154481 python_roborock-0.6.0/roborock/containers.py
--rw-r--r--   0        0        0     1022 2023-04-08 14:16:01.154481 python_roborock-0.6.0/roborock/exceptions.py
--rw-r--r--   0        0        0     7030 2023-04-08 14:16:01.154481 python_roborock-0.6.0/roborock/local_api.py
--rw-r--r--   0        0        0     1194 2023-04-08 14:16:01.154481 python_roborock-0.6.0/roborock/offline/offline.py
--rw-r--r--   0        0        0     6030 2023-04-08 14:16:01.154481 python_roborock-0.6.0/roborock/roborock_message.py
--rw-r--r--   0        0        0      644 2023-04-08 14:16:01.154481 python_roborock-0.6.0/roborock/roborock_queue.py
--rw-r--r--   0        0        0    12709 2023-04-08 14:16:01.154481 python_roborock-0.6.0/roborock/typing.py
--rw-r--r--   0        0        0      809 2023-04-08 14:16:01.154481 python_roborock-0.6.0/roborock/util.py
--rw-r--r--   0        0        0     3348 1970-01-01 00:00:00.000000 python_roborock-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-10 15:47:18.924247 python_roborock-0.6.1/LICENSE
+-rw-r--r--   0        0        0     2221 2023-04-10 15:47:18.924247 python_roborock-0.6.1/README.md
+-rw-r--r--   0        0        0     1204 2023-04-10 15:47:19.792261 python_roborock-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/__init__.py
+-rw-r--r--   0        0        0    17099 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/api.py
+-rw-r--r--   0        0        0     3957 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/cli.py
+-rw-r--r--   0        0        0     8276 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/cloud_api.py
+-rw-r--r--   0        0        0     3704 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/code_mappings.py
+-rw-r--r--   0        0        0     9190 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/containers.py
+-rw-r--r--   0        0        0     1022 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/exceptions.py
+-rw-r--r--   0        0        0     7030 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/local_api.py
+-rw-r--r--   0        0        0     1194 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/offline/offline.py
+-rw-r--r--   0        0        0     6030 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/roborock_message.py
+-rw-r--r--   0        0        0      644 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/roborock_queue.py
+-rw-r--r--   0        0        0    12709 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/typing.py
+-rw-r--r--   0        0        0      809 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/util.py
+-rw-r--r--   0        0        0     3348 1970-01-01 00:00:00.000000 python_roborock-0.6.1/PKG-INFO
```

### Comparing `python_roborock-0.6.0/LICENSE` & `python_roborock-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.0/README.md` & `python_roborock-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.0/pyproject.toml` & `python_roborock-0.6.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-roborock"
-version = "0.6.0"
+version = "0.6.1"
 description = "A package to control Roborock vacuums."
 authors = ["humbertogontijo <humbertogontijo@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/humbertogontijo/python-roborock"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -36,9 +36,10 @@
 [tool.poetry.dev-dependencies]
 pytest-asyncio = "*"
 pytest = "*"
 
 [tool.semantic_release]
 branch = "main"
 version_source = "tag"
+commit_version_number = true
 version_toml = "pyproject.toml:tool.poetry.version"
 build_command = "pip install poetry && poetry build"
```

### Comparing `python_roborock-0.6.0/roborock/api.py` & `python_roborock-0.6.1/roborock/api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.0/roborock/cli.py` & `python_roborock-0.6.1/roborock/cli.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.0/roborock/cloud_api.py` & `python_roborock-0.6.1/roborock/cloud_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.0/roborock/code_mappings.py` & `python_roborock-0.6.1/roborock/code_mappings.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.0/roborock/containers.py` & `python_roborock-0.6.1/roborock/containers.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.0/roborock/exceptions.py` & `python_roborock-0.6.1/roborock/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.0/roborock/local_api.py` & `python_roborock-0.6.1/roborock/local_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.0/roborock/offline/offline.py` & `python_roborock-0.6.1/roborock/offline/offline.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.0/roborock/roborock_message.py` & `python_roborock-0.6.1/roborock/roborock_message.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.0/roborock/roborock_queue.py` & `python_roborock-0.6.1/roborock/roborock_queue.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.0/roborock/typing.py` & `python_roborock-0.6.1/roborock/typing.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.0/roborock/util.py` & `python_roborock-0.6.1/roborock/util.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.0/PKG-INFO` & `python_roborock-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-roborock
-Version: 0.6.0
+Version: 0.6.1
 Summary: A package to control Roborock vacuums.
 Home-page: https://github.com/humbertogontijo/python-roborock
 License: GPL-3.0-only
 Author: humbertogontijo
 Author-email: humbertogontijo@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-roborock Version: 0.6.0 Summary: A package
+Metadata-Version: 2.1 Name: python-roborock Version: 0.6.1 Summary: A package
 to control Roborock vacuums. Home-page: https://github.com/humbertogontijo/
 python-roborock License: GPL-3.0-only Author: humbertogontijo Author-email:
 humbertogontijo@users.noreply.github.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

