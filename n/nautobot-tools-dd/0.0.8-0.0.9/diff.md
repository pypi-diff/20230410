# Comparing `tmp/nautobot_tools_dd-0.0.8.tar.gz` & `tmp/nautobot_tools_dd-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_tools_dd-0.0.8.tar", last modified: Sun Feb  5 19:12:24 2023, max compression
+gzip compressed data, was "nautobot_tools_dd-0.0.9.tar", last modified: Sun Feb  5 19:14:16 2023, max compression
```

## Comparing `nautobot_tools_dd-0.0.8.tar` & `nautobot_tools_dd-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxr-x   0 inchidi   (1000) inchidi   (1000)        0 2023-02-05 19:12:24.290961 nautobot_tools_dd-0.0.8/
--rw-rw-r--   0 inchidi   (1000) inchidi   (1000)        0 2022-10-17 20:40:10.000000 nautobot_tools_dd-0.0.8/LICENSE
--rw-rw-r--   0 inchidi   (1000) inchidi   (1000)      276 2023-02-05 19:12:24.290961 nautobot_tools_dd-0.0.8/PKG-INFO
--rwxr-x---   0 inchidi   (1000) inchidi   (1000)        0 2022-09-14 06:16:37.000000 nautobot_tools_dd-0.0.8/README.md
-drwxrwxr-x   0 inchidi   (1000) inchidi   (1000)        0 2023-02-05 19:12:24.286961 nautobot_tools_dd-0.0.8/nautobot_tools/
--rwxr-x---   0 inchidi   (1000) inchidi   (1000)      577 2023-02-05 18:42:12.000000 nautobot_tools_dd-0.0.8/nautobot_tools/__init__.py
--rwxr-x---   0 inchidi   (1000) inchidi   (1000)     3147 2022-12-08 15:53:46.000000 nautobot_tools_dd-0.0.8/nautobot_tools/field_mapping.py
--rwxr-x---   0 inchidi   (1000) inchidi   (1000)     1991 2022-12-08 09:34:19.000000 nautobot_tools_dd-0.0.8/nautobot_tools/model_meta.py
--rwxr-x---   0 inchidi   (1000) inchidi   (1000)       86 2022-11-28 09:30:13.000000 nautobot_tools_dd-0.0.8/nautobot_tools/models.py
-drwxrwxr-x   0 inchidi   (1000) inchidi   (1000)        0 2023-02-05 19:12:24.286961 nautobot_tools_dd-0.0.8/nautobot_tools/network_element/
--rwxr-x---   0 inchidi   (1000) inchidi   (1000)        0 2022-09-15 21:19:00.000000 nautobot_tools_dd-0.0.8/nautobot_tools/network_element/__init__.py
--rwxr-x---   0 inchidi   (1000) inchidi   (1000)    21506 2023-02-05 18:23:38.000000 nautobot_tools_dd-0.0.8/nautobot_tools/serializers.py
--rw-rw-r--   0 inchidi   (1000) inchidi   (1000)      439 2023-02-05 19:06:33.000000 nautobot_tools_dd-0.0.8/nautobot_tools/utils.py
-drwxrwxr-x   0 inchidi   (1000) inchidi   (1000)        0 2023-02-05 19:12:24.290961 nautobot_tools_dd-0.0.8/nautobot_tools_dd.egg-info/
--rw-rw-r--   0 inchidi   (1000) inchidi   (1000)      276 2023-02-05 19:12:24.000000 nautobot_tools_dd-0.0.8/nautobot_tools_dd.egg-info/PKG-INFO
--rw-rw-r--   0 inchidi   (1000) inchidi   (1000)      446 2023-02-05 19:12:24.000000 nautobot_tools_dd-0.0.8/nautobot_tools_dd.egg-info/SOURCES.txt
--rw-rw-r--   0 inchidi   (1000) inchidi   (1000)        1 2023-02-05 19:12:24.000000 nautobot_tools_dd-0.0.8/nautobot_tools_dd.egg-info/dependency_links.txt
--rw-rw-r--   0 inchidi   (1000) inchidi   (1000)       37 2023-02-05 19:12:24.000000 nautobot_tools_dd-0.0.8/nautobot_tools_dd.egg-info/requires.txt
--rw-rw-r--   0 inchidi   (1000) inchidi   (1000)       15 2023-02-05 19:12:24.000000 nautobot_tools_dd-0.0.8/nautobot_tools_dd.egg-info/top_level.txt
--rw-rw-r--   0 inchidi   (1000) inchidi   (1000)      505 2023-02-05 19:12:10.000000 nautobot_tools_dd-0.0.8/pyproject.toml
--rw-rw-r--   0 inchidi   (1000) inchidi   (1000)       38 2023-02-05 19:12:24.290961 nautobot_tools_dd-0.0.8/setup.cfg
+drwxrwxr-x   0 inchidi   (1000) inchidi   (1000)        0 2023-02-05 19:14:16.297771 nautobot_tools_dd-0.0.9/
+-rw-rw-r--   0 inchidi   (1000) inchidi   (1000)        0 2022-10-17 20:40:10.000000 nautobot_tools_dd-0.0.9/LICENSE
+-rw-rw-r--   0 inchidi   (1000) inchidi   (1000)      276 2023-02-05 19:14:16.297771 nautobot_tools_dd-0.0.9/PKG-INFO
+-rwxr-x---   0 inchidi   (1000) inchidi   (1000)        0 2022-09-14 06:16:37.000000 nautobot_tools_dd-0.0.9/README.md
+drwxrwxr-x   0 inchidi   (1000) inchidi   (1000)        0 2023-02-05 19:14:16.297771 nautobot_tools_dd-0.0.9/nautobot_tools/
+-rwxr-x---   0 inchidi   (1000) inchidi   (1000)      577 2023-02-05 18:42:12.000000 nautobot_tools_dd-0.0.9/nautobot_tools/__init__.py
+-rwxr-x---   0 inchidi   (1000) inchidi   (1000)     3147 2022-12-08 15:53:46.000000 nautobot_tools_dd-0.0.9/nautobot_tools/field_mapping.py
+-rwxr-x---   0 inchidi   (1000) inchidi   (1000)     1991 2022-12-08 09:34:19.000000 nautobot_tools_dd-0.0.9/nautobot_tools/model_meta.py
+-rwxr-x---   0 inchidi   (1000) inchidi   (1000)       86 2022-11-28 09:30:13.000000 nautobot_tools_dd-0.0.9/nautobot_tools/models.py
+drwxrwxr-x   0 inchidi   (1000) inchidi   (1000)        0 2023-02-05 19:14:16.297771 nautobot_tools_dd-0.0.9/nautobot_tools/network_element/
+-rwxr-x---   0 inchidi   (1000) inchidi   (1000)        0 2022-09-15 21:19:00.000000 nautobot_tools_dd-0.0.9/nautobot_tools/network_element/__init__.py
+-rwxr-x---   0 inchidi   (1000) inchidi   (1000)    21506 2023-02-05 18:23:38.000000 nautobot_tools_dd-0.0.9/nautobot_tools/serializers.py
+-rw-rw-r--   0 inchidi   (1000) inchidi   (1000)      439 2023-02-05 19:06:33.000000 nautobot_tools_dd-0.0.9/nautobot_tools/utils.py
+drwxrwxr-x   0 inchidi   (1000) inchidi   (1000)        0 2023-02-05 19:14:16.297771 nautobot_tools_dd-0.0.9/nautobot_tools/yang/
+-rw-rw-r--   0 inchidi   (1000) inchidi   (1000)      402 2023-01-27 03:24:46.000000 nautobot_tools_dd-0.0.9/nautobot_tools/yang/dd-nos.yang
+drwxrwxr-x   0 inchidi   (1000) inchidi   (1000)        0 2023-02-05 19:14:16.297771 nautobot_tools_dd-0.0.9/nautobot_tools_dd.egg-info/
+-rw-rw-r--   0 inchidi   (1000) inchidi   (1000)      276 2023-02-05 19:14:16.000000 nautobot_tools_dd-0.0.9/nautobot_tools_dd.egg-info/PKG-INFO
+-rw-rw-r--   0 inchidi   (1000) inchidi   (1000)      478 2023-02-05 19:14:16.000000 nautobot_tools_dd-0.0.9/nautobot_tools_dd.egg-info/SOURCES.txt
+-rw-rw-r--   0 inchidi   (1000) inchidi   (1000)        1 2023-02-05 19:14:16.000000 nautobot_tools_dd-0.0.9/nautobot_tools_dd.egg-info/dependency_links.txt
+-rw-rw-r--   0 inchidi   (1000) inchidi   (1000)       37 2023-02-05 19:14:16.000000 nautobot_tools_dd-0.0.9/nautobot_tools_dd.egg-info/requires.txt
+-rw-rw-r--   0 inchidi   (1000) inchidi   (1000)       15 2023-02-05 19:14:16.000000 nautobot_tools_dd-0.0.9/nautobot_tools_dd.egg-info/top_level.txt
+-rw-rw-r--   0 inchidi   (1000) inchidi   (1000)      494 2023-02-05 19:14:07.000000 nautobot_tools_dd-0.0.9/pyproject.toml
+-rw-rw-r--   0 inchidi   (1000) inchidi   (1000)       38 2023-02-05 19:14:16.297771 nautobot_tools_dd-0.0.9/setup.cfg
```

### Comparing `nautobot_tools_dd-0.0.8/nautobot_tools/__init__.py` & `nautobot_tools_dd-0.0.9/nautobot_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot_tools_dd-0.0.8/nautobot_tools/field_mapping.py` & `nautobot_tools_dd-0.0.9/nautobot_tools/field_mapping.py`

 * *Files identical despite different names*

### Comparing `nautobot_tools_dd-0.0.8/nautobot_tools/model_meta.py` & `nautobot_tools_dd-0.0.9/nautobot_tools/model_meta.py`

 * *Files identical despite different names*

### Comparing `nautobot_tools_dd-0.0.8/nautobot_tools/serializers.py` & `nautobot_tools_dd-0.0.9/nautobot_tools/serializers.py`

 * *Files identical despite different names*

