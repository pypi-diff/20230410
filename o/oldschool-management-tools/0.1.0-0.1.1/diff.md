# Comparing `tmp/oldschool_management_tools-0.1.0.tar.gz` & `tmp/oldschool_management_tools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oldschool_management_tools-0.1.0.tar", max compression
+gzip compressed data, was "oldschool_management_tools-0.1.1.tar", max compression
```

## Comparing `oldschool_management_tools-0.1.0.tar` & `oldschool_management_tools-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       96 2023-04-10 12:05:51.622779 oldschool_management_tools-0.1.0/oldschool_management_tools/__init__.py
--rw-r--r--   0        0        0     1063 2022-11-05 13:50:02.083491 oldschool_management_tools-0.1.0/oldschool_management_tools/calendar_items/calendar_item.py
--rw-r--r--   0        0        0      565 2023-04-10 12:03:47.257190 oldschool_management_tools-0.1.0/oldschool_management_tools/mgmt_tools_cmd.py
--rw-r--r--   0        0        0     2041 2023-04-10 12:05:13.986985 oldschool_management_tools-0.1.0/oldschool_management_tools/oldschool_management_tools.py
--rw-r--r--   0        0        0      352 2023-04-10 12:00:27.263061 oldschool_management_tools-0.1.0/oldschool_management_tools/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-10 12:00:27.259073 oldschool_management_tools-0.1.0/oldschool_management_tools/README.md
--rw-r--r--   0        0        0      698 2022-11-06 16:58:42.825790 oldschool_management_tools-0.1.0/oldschool_management_tools/special_prompts/special_prompts.py
--rw-r--r--   0        0        0        0 2023-04-10 12:00:27.259073 oldschool_management_tools-0.1.0/oldschool_management_tools/tests/__init__.py
--rw-r--r--   0        0        0      447 2023-04-09 07:24:56.391208 oldschool_management_tools-0.1.0/oldschool_management_tools/testy.py
--rw-r--r--   0        0        0      440 2023-04-10 12:03:11.141215 oldschool_management_tools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        4 2022-10-15 13:56:15.832011 oldschool_management_tools-0.1.0/README.md
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 oldschool_management_tools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       96 2023-04-10 12:05:51.622779 oldschool_management_tools-0.1.1/oldschool_management_tools/__init__.py
+-rw-r--r--   0        0        0     1063 2022-11-05 13:50:02.083491 oldschool_management_tools-0.1.1/oldschool_management_tools/calendar_items/calendar_item.py
+-rw-r--r--   0        0        0      565 2023-04-10 12:03:47.257190 oldschool_management_tools-0.1.1/oldschool_management_tools/mgmt_tools_cmd.py
+-rw-r--r--   0        0        0     2041 2023-04-10 12:05:13.986985 oldschool_management_tools-0.1.1/oldschool_management_tools/oldschool_management_tools.py
+-rw-r--r--   0        0        0      352 2023-04-10 12:00:27.263061 oldschool_management_tools-0.1.1/oldschool_management_tools/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 12:00:27.259073 oldschool_management_tools-0.1.1/oldschool_management_tools/README.md
+-rw-r--r--   0        0        0      698 2022-11-06 16:58:42.825790 oldschool_management_tools-0.1.1/oldschool_management_tools/special_prompts/special_prompts.py
+-rw-r--r--   0        0        0        0 2023-04-10 12:00:27.259073 oldschool_management_tools-0.1.1/oldschool_management_tools/tests/__init__.py
+-rw-r--r--   0        0        0      447 2023-04-09 07:24:56.391208 oldschool_management_tools-0.1.1/oldschool_management_tools/testy.py
+-rw-r--r--   0        0        0      436 2023-04-10 12:20:22.624588 oldschool_management_tools-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        4 2022-10-15 13:56:15.832011 oldschool_management_tools-0.1.1/README.md
+-rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 oldschool_management_tools-0.1.1/PKG-INFO
```

### Comparing `oldschool_management_tools-0.1.0/oldschool_management_tools/calendar_items/calendar_item.py` & `oldschool_management_tools-0.1.1/oldschool_management_tools/calendar_items/calendar_item.py`

 * *Files identical despite different names*

### Comparing `oldschool_management_tools-0.1.0/oldschool_management_tools/mgmt_tools_cmd.py` & `oldschool_management_tools-0.1.1/oldschool_management_tools/mgmt_tools_cmd.py`

 * *Files identical despite different names*

### Comparing `oldschool_management_tools-0.1.0/oldschool_management_tools/oldschool_management_tools.py` & `oldschool_management_tools-0.1.1/oldschool_management_tools/oldschool_management_tools.py`

 * *Files identical despite different names*

### Comparing `oldschool_management_tools-0.1.0/oldschool_management_tools/special_prompts/special_prompts.py` & `oldschool_management_tools-0.1.1/oldschool_management_tools/special_prompts/special_prompts.py`

 * *Files identical despite different names*

