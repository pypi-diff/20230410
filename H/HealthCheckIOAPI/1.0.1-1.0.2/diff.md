# Comparing `tmp/HealthCheckIOAPI-1.0.1.tar.gz` & `tmp/HealthCheckIOAPI-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HealthCheckIOAPI-1.0.1.tar", last modified: Sun Apr  2 13:56:08 2023, max compression
+gzip compressed data, was "HealthCheckIOAPI-1.0.2.tar", last modified: Mon Apr 10 13:49:54 2023, max compression
```

## Comparing `HealthCheckIOAPI-1.0.1.tar` & `HealthCheckIOAPI-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-04-02 13:56:08.198227 HealthCheckIOAPI-1.0.1/
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-04-02 13:56:08.198227 HealthCheckIOAPI-1.0.1/HealthCheckIOAPI.egg-info/
--rw-r--r--   0 felix     (1000) felix     (1000)      280 2023-04-02 13:56:08.000000 HealthCheckIOAPI-1.0.1/HealthCheckIOAPI.egg-info/PKG-INFO
--rw-r--r--   0 felix     (1000) felix     (1000)      300 2023-04-02 13:56:08.000000 HealthCheckIOAPI-1.0.1/HealthCheckIOAPI.egg-info/SOURCES.txt
--rw-r--r--   0 felix     (1000) felix     (1000)        1 2023-04-02 13:56:08.000000 HealthCheckIOAPI-1.0.1/HealthCheckIOAPI.egg-info/dependency_links.txt
--rw-r--r--   0 felix     (1000) felix     (1000)        9 2023-04-02 13:56:08.000000 HealthCheckIOAPI-1.0.1/HealthCheckIOAPI.egg-info/requires.txt
--rw-r--r--   0 felix     (1000) felix     (1000)       14 2023-04-02 13:56:08.000000 HealthCheckIOAPI-1.0.1/HealthCheckIOAPI.egg-info/top_level.txt
--rw-r--r--   0 felix     (1000) felix     (1000)     1069 2023-03-31 22:59:32.000000 HealthCheckIOAPI-1.0.1/LICENSE
--rw-r--r--   0 felix     (1000) felix     (1000)      280 2023-04-02 13:56:08.198227 HealthCheckIOAPI-1.0.1/PKG-INFO
--rw-r--r--   0 felix     (1000) felix     (1000)      951 2023-04-02 13:44:54.000000 HealthCheckIOAPI-1.0.1/README.md
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-04-02 13:56:08.198227 HealthCheckIOAPI-1.0.1/healthcheckio/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2023-03-31 23:02:59.000000 HealthCheckIOAPI-1.0.1/healthcheckio/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2368 2023-04-01 15:34:59.000000 HealthCheckIOAPI-1.0.1/healthcheckio/hc_log.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2853 2023-04-02 12:51:55.000000 HealthCheckIOAPI-1.0.1/healthcheckio/hc_ping.py
--rw-r--r--   0 felix     (1000) felix     (1000)       38 2023-04-02 13:56:08.198227 HealthCheckIOAPI-1.0.1/setup.cfg
--rw-r--r--   0 felix     (1000) felix     (1000)      620 2023-04-02 13:51:36.000000 HealthCheckIOAPI-1.0.1/setup.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-04-10 13:49:54.189880 HealthCheckIOAPI-1.0.2/
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-04-10 13:49:54.189880 HealthCheckIOAPI-1.0.2/HealthCheckIOAPI.egg-info/
+-rw-r--r--   0 felix     (1000) felix     (1000)     1224 2023-04-10 13:49:54.000000 HealthCheckIOAPI-1.0.2/HealthCheckIOAPI.egg-info/PKG-INFO
+-rw-r--r--   0 felix     (1000) felix     (1000)      300 2023-04-10 13:49:54.000000 HealthCheckIOAPI-1.0.2/HealthCheckIOAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)        1 2023-04-10 13:49:54.000000 HealthCheckIOAPI-1.0.2/HealthCheckIOAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)        9 2023-04-10 13:49:54.000000 HealthCheckIOAPI-1.0.2/HealthCheckIOAPI.egg-info/requires.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)       14 2023-04-10 13:49:54.000000 HealthCheckIOAPI-1.0.2/HealthCheckIOAPI.egg-info/top_level.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)     1069 2023-03-31 22:59:32.000000 HealthCheckIOAPI-1.0.2/LICENSE
+-rw-r--r--   0 felix     (1000) felix     (1000)     1224 2023-04-10 13:49:54.189880 HealthCheckIOAPI-1.0.2/PKG-INFO
+-rw-r--r--   0 felix     (1000) felix     (1000)      951 2023-04-02 13:44:54.000000 HealthCheckIOAPI-1.0.2/README.md
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-04-10 13:49:54.189880 HealthCheckIOAPI-1.0.2/healthcheckio/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2023-03-31 23:02:59.000000 HealthCheckIOAPI-1.0.2/healthcheckio/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2368 2023-04-01 15:34:59.000000 HealthCheckIOAPI-1.0.2/healthcheckio/hc_log.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2853 2023-04-02 12:51:55.000000 HealthCheckIOAPI-1.0.2/healthcheckio/hc_ping.py
+-rw-r--r--   0 felix     (1000) felix     (1000)       38 2023-04-10 13:49:54.189880 HealthCheckIOAPI-1.0.2/setup.cfg
+-rw-r--r--   0 felix     (1000) felix     (1000)      629 2023-04-10 13:49:23.000000 HealthCheckIOAPI-1.0.2/setup.py
```

### Comparing `HealthCheckIOAPI-1.0.1/LICENSE` & `HealthCheckIOAPI-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `HealthCheckIOAPI-1.0.1/README.md` & `HealthCheckIOAPI-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `HealthCheckIOAPI-1.0.1/healthcheckio/hc_log.py` & `HealthCheckIOAPI-1.0.2/healthcheckio/hc_log.py`

 * *Files identical despite different names*

### Comparing `HealthCheckIOAPI-1.0.1/healthcheckio/hc_ping.py` & `HealthCheckIOAPI-1.0.2/healthcheckio/hc_ping.py`

 * *Files identical despite different names*

