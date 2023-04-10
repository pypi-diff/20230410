# Comparing `tmp/mpapi-webui-1.0.0.tar.gz` & `tmp/mpapi-webui-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mpapi-webui-1.0.0.tar", last modified: Mon Apr 10 05:25:00 2023, max compression
+gzip compressed data, was "dist/mpapi-webui-1.1.0.tar", last modified: Mon Apr 10 05:35:33 2023, max compression
```

## Comparing `mpapi-webui-1.0.0.tar` & `mpapi-webui-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 05:25:00.668614 mpapi-webui-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      155 2023-04-10 05:25:00.667614 mpapi-webui-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-10 04:50:06.000000 mpapi-webui-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 05:25:00.667614 mpapi-webui-1.0.0/mpapi-webui/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 05:06:31.000000 mpapi-webui-1.0.0/mpapi-webui/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2909 2023-04-10 04:50:06.000000 mpapi-webui-1.0.0/mpapi-webui/caller.py
--rw-r--r--   0 root         (0) root         (0)     2204 2023-04-10 04:50:06.000000 mpapi-webui-1.0.0/mpapi-webui/mpapi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 05:25:00.667614 mpapi-webui-1.0.0/mpapi_webui.egg-info/
--rw-r--r--   0 root         (0) root         (0)      155 2023-04-10 05:25:00.000000 mpapi-webui-1.0.0/mpapi_webui.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      225 2023-04-10 05:25:00.000000 mpapi-webui-1.0.0/mpapi_webui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 05:25:00.000000 mpapi-webui-1.0.0/mpapi_webui.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-10 05:25:00.000000 mpapi-webui-1.0.0/mpapi_webui.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 05:25:00.668614 mpapi-webui-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      290 2023-04-10 05:24:58.000000 mpapi-webui-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 05:35:33.507403 mpapi-webui-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      155 2023-04-10 05:35:33.507403 mpapi-webui-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-10 04:50:06.000000 mpapi-webui-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 05:35:33.506403 mpapi-webui-1.1.0/mpapi_webui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      155 2023-04-10 05:35:33.000000 mpapi-webui-1.1.0/mpapi_webui.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      213 2023-04-10 05:35:33.000000 mpapi-webui-1.1.0/mpapi_webui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 05:35:33.000000 mpapi-webui-1.1.0/mpapi_webui.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-10 05:35:33.000000 mpapi-webui-1.1.0/mpapi_webui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 05:35:33.507403 mpapi-webui-1.1.0/mpwebui/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 05:06:31.000000 mpapi-webui-1.1.0/mpwebui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2909 2023-04-10 04:50:06.000000 mpapi-webui-1.1.0/mpwebui/caller.py
+-rw-r--r--   0 root         (0) root         (0)     2204 2023-04-10 04:50:06.000000 mpapi-webui-1.1.0/mpwebui/mpapi.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 05:35:33.507403 mpapi-webui-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      290 2023-04-10 05:35:27.000000 mpapi-webui-1.1.0/setup.py
```

### Comparing `mpapi-webui-1.0.0/mpapi-webui/caller.py` & `mpapi-webui-1.1.0/mpwebui/caller.py`

 * *Files identical despite different names*

### Comparing `mpapi-webui-1.0.0/mpapi-webui/mpapi.py` & `mpapi-webui-1.1.0/mpwebui/mpapi.py`

 * *Files identical despite different names*

