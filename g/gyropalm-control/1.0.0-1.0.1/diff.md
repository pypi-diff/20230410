# Comparing `tmp/gyropalm_control-1.0.0.tar.gz` & `tmp/gyropalm_control-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gyropalm_control-1.0.0.tar", last modified: Mon Apr 10 12:52:54 2023, max compression
+gzip compressed data, was "dist\gyropalm_control-1.0.1.tar", last modified: Mon Apr 10 13:16:44 2023, max compression
```

## Comparing `gyropalm_control-1.0.0.tar` & `gyropalm_control-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 12:52:54.101909 gyropalm_control-1.0.0/
--rw-rw-rw-   0        0        0      247 2023-04-10 12:52:54.099908 gyropalm_control-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2473 2023-04-10 12:13:53.000000 gyropalm_control-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 12:52:54.060880 gyropalm_control-1.0.0/gyropalm_control/
--rw-rw-rw-   0        0        0        0 2023-04-10 12:25:26.000000 gyropalm_control-1.0.0/gyropalm_control/__init__.py
--rw-rw-rw-   0        0        0     5863 2023-04-10 12:26:37.000000 gyropalm_control-1.0.0/gyropalm_control/gp_driving.py
--rw-rw-rw-   0        0        0     3517 2023-04-10 12:26:22.000000 gyropalm_control-1.0.0/gyropalm_control/gp_realtime.py
-drwxrwxrwx   0        0        0        0 2023-04-10 12:52:54.091901 gyropalm_control-1.0.0/gyropalm_control.egg-info/
--rw-rw-rw-   0        0        0      247 2023-04-10 12:52:53.000000 gyropalm_control-1.0.0/gyropalm_control.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2023-04-10 12:52:54.000000 gyropalm_control-1.0.0/gyropalm_control.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 12:52:53.000000 gyropalm_control-1.0.0/gyropalm_control.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-10 12:52:53.000000 gyropalm_control-1.0.0/gyropalm_control.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-10 12:52:53.000000 gyropalm_control-1.0.0/gyropalm_control.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 12:52:54.105912 gyropalm_control-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      296 2023-04-10 12:28:22.000000 gyropalm_control-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 13:16:44.649242 gyropalm_control-1.0.1/
+-rw-rw-rw-   0        0        0     3008 2023-04-10 13:16:44.645239 gyropalm_control-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2473 2023-04-10 12:13:53.000000 gyropalm_control-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 13:16:44.597205 gyropalm_control-1.0.1/gyropalm_control/
+-rw-rw-rw-   0        0        0        0 2023-04-10 12:25:26.000000 gyropalm_control-1.0.1/gyropalm_control/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 13:16:44.640236 gyropalm_control-1.0.1/gyropalm_control/examples/
+-rw-rw-rw-   0        0        0     2161 2023-04-10 13:10:13.000000 gyropalm_control-1.0.1/gyropalm_control/examples/driving_test.py
+-rw-rw-rw-   0        0        0      880 2023-04-10 13:10:07.000000 gyropalm_control-1.0.1/gyropalm_control/examples/realtime_test.py
+-rw-rw-rw-   0        0        0     5863 2023-04-10 12:26:37.000000 gyropalm_control-1.0.1/gyropalm_control/gp_driving.py
+-rw-rw-rw-   0        0        0     3517 2023-04-10 12:26:22.000000 gyropalm_control-1.0.1/gyropalm_control/gp_realtime.py
+drwxrwxrwx   0        0        0        0 2023-04-10 13:16:44.627226 gyropalm_control-1.0.1/gyropalm_control.egg-info/
+-rw-rw-rw-   0        0        0     3008 2023-04-10 13:16:44.000000 gyropalm_control-1.0.1/gyropalm_control.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-04-10 13:16:44.000000 gyropalm_control-1.0.1/gyropalm_control.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 13:16:44.000000 gyropalm_control-1.0.1/gyropalm_control.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-10 13:16:44.000000 gyropalm_control-1.0.1/gyropalm_control.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-10 13:16:44.000000 gyropalm_control-1.0.1/gyropalm_control.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 13:16:44.657248 gyropalm_control-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      701 2023-04-10 13:16:40.000000 gyropalm_control-1.0.1/setup.py
```

### Comparing `gyropalm_control-1.0.0/README.md` & `gyropalm_control-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `gyropalm_control-1.0.0/gyropalm_control/gp_driving.py` & `gyropalm_control-1.0.1/gyropalm_control/gp_driving.py`

 * *Files identical despite different names*

### Comparing `gyropalm_control-1.0.0/gyropalm_control/gp_realtime.py` & `gyropalm_control-1.0.1/gyropalm_control/gp_realtime.py`

 * *Files identical despite different names*

