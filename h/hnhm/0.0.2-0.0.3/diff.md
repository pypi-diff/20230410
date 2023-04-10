# Comparing `tmp/hnhm-0.0.2.tar.gz` & `tmp/hnhm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnhm-0.0.2.tar", max compression
+gzip compressed data, was "hnhm-0.0.3.tar", max compression
```

## Comparing `hnhm-0.0.2.tar` & `hnhm-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      707 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/__init__.py
--rw-r--r--   0        0        0     5153 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/cli.py
--rw-r--r--   0        0        0      551 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/core/__init__.py
--rw-r--r--   0        0        0     1084 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/core/attribute.py
--rw-r--r--   0        0        0      554 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/core/entity.py
--rw-r--r--   0        0        0       80 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/core/error.py
--rw-r--r--   0        0        0      311 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/core/group.py
--rw-r--r--   0        0        0      543 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/core/layout.py
--rw-r--r--   0        0        0      654 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/core/link.py
--rw-r--r--   0        0        0     1724 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/core/mutations.py
--rw-r--r--   0        0        0       80 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/core/priority.py
--rw-r--r--   0        0        0      511 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/core/sql.py
--rw-r--r--   0        0        0      621 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/core/storage.py
--rw-r--r--   0        0        0     1545 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/core/tasks.py
--rw-r--r--   0        0        0      564 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/file_storage.py
--rw-r--r--   0        0        0     7561 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/flow.py
--rw-r--r--   0        0        0     9084 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/hnhm.py
--rw-r--r--   0        0        0      902 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/hnhm_attribute.py
--rw-r--r--   0        0        0     3682 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/hnhm_entity.py
--rw-r--r--   0        0        0     2547 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/hnhm_link.py
--rw-r--r--   0        0        0      419 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/hnhm_registry.py
--rw-r--r--   0        0        0        0 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/postgres/__init__.py
--rw-r--r--   0        0        0    12233 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/postgres/sql.py
--rw-r--r--   0        0        0      459 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/postgres/sql_templates/__init__.py
--rw-r--r--   0        0        0      456 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/postgres/sql_templates/create_attribute.py
--rw-r--r--   0        0        0      477 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/postgres/sql_templates/create_group.py
--rw-r--r--   0        0        0      272 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/postgres/sql_templates/create_hub.py
--rw-r--r--   0        0        0      504 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/postgres/sql_templates/create_link.py
--rw-r--r--   0        0        0      228 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/postgres/sql_templates/create_stage.py
--rw-r--r--   0        0        0      425 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/postgres/sql_templates/load_hub.py
--rw-r--r--   0        0        0      905 2023-04-10 21:25:58.157304 hnhm-0.0.2/hnhm/postgres/sql_templates/load_ignore.py
--rw-r--r--   0        0        0     4326 2023-04-10 21:25:58.161304 hnhm-0.0.2/hnhm/postgres/sql_templates/load_new.py
--rw-r--r--   0        0        0     1905 2023-04-10 21:25:58.161304 hnhm-0.0.2/hnhm/postgres/sql_templates/load_update.py
--rw-r--r--   0        0        0      707 2023-04-10 21:25:58.161304 hnhm-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 hnhm-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      707 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/__init__.py
+-rw-r--r--   0        0        0     5189 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/cli.py
+-rw-r--r--   0        0        0      551 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/core/__init__.py
+-rw-r--r--   0        0        0     1084 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/core/attribute.py
+-rw-r--r--   0        0        0      554 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/core/entity.py
+-rw-r--r--   0        0        0       80 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/core/error.py
+-rw-r--r--   0        0        0      311 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/core/group.py
+-rw-r--r--   0        0        0      543 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/core/layout.py
+-rw-r--r--   0        0        0      654 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/core/link.py
+-rw-r--r--   0        0        0     1724 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/core/mutations.py
+-rw-r--r--   0        0        0       80 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/core/priority.py
+-rw-r--r--   0        0        0      511 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/core/sql.py
+-rw-r--r--   0        0        0      621 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/core/storage.py
+-rw-r--r--   0        0        0     1545 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/core/tasks.py
+-rw-r--r--   0        0        0      564 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/file_storage.py
+-rw-r--r--   0        0        0     7561 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/flow.py
+-rw-r--r--   0        0        0     9084 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/hnhm.py
+-rw-r--r--   0        0        0      902 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/hnhm_attribute.py
+-rw-r--r--   0        0        0     3682 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/hnhm_entity.py
+-rw-r--r--   0        0        0     2547 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/hnhm_link.py
+-rw-r--r--   0        0        0      419 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/hnhm_registry.py
+-rw-r--r--   0        0        0        0 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/postgres/__init__.py
+-rw-r--r--   0        0        0    12233 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/postgres/sql.py
+-rw-r--r--   0        0        0      459 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/postgres/sql_templates/__init__.py
+-rw-r--r--   0        0        0      456 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/postgres/sql_templates/create_attribute.py
+-rw-r--r--   0        0        0      477 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/postgres/sql_templates/create_group.py
+-rw-r--r--   0        0        0      272 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/postgres/sql_templates/create_hub.py
+-rw-r--r--   0        0        0      504 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/postgres/sql_templates/create_link.py
+-rw-r--r--   0        0        0      228 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/postgres/sql_templates/create_stage.py
+-rw-r--r--   0        0        0      425 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/postgres/sql_templates/load_hub.py
+-rw-r--r--   0        0        0      905 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/postgres/sql_templates/load_ignore.py
+-rw-r--r--   0        0        0     4326 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/postgres/sql_templates/load_new.py
+-rw-r--r--   0        0        0     1905 2023-04-10 21:36:33.411168 hnhm-0.0.3/hnhm/postgres/sql_templates/load_update.py
+-rw-r--r--   0        0        0      707 2023-04-10 21:36:33.411168 hnhm-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 hnhm-0.0.3/PKG-INFO
```

### Comparing `hnhm-0.0.2/hnhm/__init__.py` & `hnhm-0.0.3/hnhm/__init__.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.2/hnhm/cli.py` & `hnhm-0.0.3/hnhm/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import importlib
 
 import click
 
 from .hnhm import Plan, PlanType
 from .hnhm_registry import HnhmRegistry
 from .core import (
@@ -15,14 +16,15 @@
     RemoveEntity,
     CreateAttribute,
     RemoveAttribute,
 )
 
 
 def import_registry(module: str) -> HnhmRegistry:
+    sys.path.append(".")
     imported_module = importlib.import_module(module)
     registry: HnhmRegistry = getattr(imported_module, "__registry__", None)
     if not registry:
         raise HnhmError(
             f"Failed to import registry from module: '{module}'."
             " Please, specify your registry via __registry__ object in your DWH module."
         )
```

### Comparing `hnhm-0.0.2/hnhm/core/__init__.py` & `hnhm-0.0.3/hnhm/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.2/hnhm/core/attribute.py` & `hnhm-0.0.3/hnhm/core/attribute.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.2/hnhm/core/entity.py` & `hnhm-0.0.3/hnhm/core/entity.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.2/hnhm/core/layout.py` & `hnhm-0.0.3/hnhm/core/layout.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.2/hnhm/core/link.py` & `hnhm-0.0.3/hnhm/core/link.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.2/hnhm/core/mutations.py` & `hnhm-0.0.3/hnhm/core/mutations.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.2/hnhm/core/storage.py` & `hnhm-0.0.3/hnhm/core/storage.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.2/hnhm/core/tasks.py` & `hnhm-0.0.3/hnhm/core/tasks.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.2/hnhm/file_storage.py` & `hnhm-0.0.3/hnhm/file_storage.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.2/hnhm/flow.py` & `hnhm-0.0.3/hnhm/flow.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.2/hnhm/hnhm.py` & `hnhm-0.0.3/hnhm/hnhm.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.2/hnhm/hnhm_attribute.py` & `hnhm-0.0.3/hnhm/hnhm_attribute.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.2/hnhm/hnhm_entity.py` & `hnhm-0.0.3/hnhm/hnhm_entity.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.2/hnhm/hnhm_link.py` & `hnhm-0.0.3/hnhm/hnhm_link.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.2/hnhm/postgres/sql.py` & `hnhm-0.0.3/hnhm/postgres/sql.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.2/hnhm/postgres/sql_templates/load_ignore.py` & `hnhm-0.0.3/hnhm/postgres/sql_templates/load_ignore.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.2/hnhm/postgres/sql_templates/load_new.py` & `hnhm-0.0.3/hnhm/postgres/sql_templates/load_new.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.2/hnhm/postgres/sql_templates/load_update.py` & `hnhm-0.0.3/hnhm/postgres/sql_templates/load_update.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.2/pyproject.toml` & `hnhm-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hnhm"
-version = "0.0.2"
+version = "0.0.3"
 description = "hNhM – highly Normalized hybrid Model."
 authors = ["Arseny Egorov <egoroff-ars@yandex.ru>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "1.10.7"
 click = "8.1.3"
```

