# Comparing `tmp/gpush-1.1.0.tar.gz` & `tmp/gpush-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpush-1.1.0.tar", last modified: Sun Apr  9 09:17:00 2023, max compression
+gzip compressed data, was "gpush-1.1.1.tar", last modified: Sun Apr  9 20:20:02 2023, max compression
```

## Comparing `gpush-1.1.0.tar` & `gpush-1.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 09:17:00.449565 gpush-1.1.0/
--rw-r--r--   0 root         (0) root         (0)       49 2023-04-09 09:17:00.445564 gpush-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      574 2023-04-09 09:16:57.000000 gpush-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 09:17:00.445564 gpush-1.1.0/gpush.egg-info/
--rw-r--r--   0 root         (0) root         (0)       49 2023-04-09 09:17:00.000000 gpush-1.1.0/gpush.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      158 2023-04-09 09:17:00.000000 gpush-1.1.0/gpush.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 09:17:00.000000 gpush-1.1.0/gpush.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-09 09:17:00.000000 gpush-1.1.0/gpush.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1802 2023-04-09 09:16:57.000000 gpush-1.1.0/gpush.py
--rw-r--r--   0 root         (0) root         (0)      224 2023-04-09 09:16:57.000000 gpush-1.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 09:17:00.449565 gpush-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      144 2023-04-09 09:16:58.000000 gpush-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 20:20:02.354586 gpush-1.1.1/
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-04-09 20:20:02.354586 gpush-1.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1066 2023-04-09 20:19:59.000000 gpush-1.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 20:20:02.354586 gpush-1.1.1/gpush.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-04-09 20:20:02.000000 gpush-1.1.1/gpush.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      158 2023-04-09 20:20:02.000000 gpush-1.1.1/gpush.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 20:20:02.000000 gpush-1.1.1/gpush.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-09 20:20:02.000000 gpush-1.1.1/gpush.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1802 2023-04-09 20:19:59.000000 gpush-1.1.1/gpush.py
+-rw-r--r--   0 root         (0) root         (0)      224 2023-04-09 20:19:59.000000 gpush-1.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 20:20:02.354586 gpush-1.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      343 2023-04-09 20:19:59.000000 gpush-1.1.1/setup.py
```

### Comparing `gpush-1.1.0/gpush.py` & `gpush-1.1.1/gpush.py`

 * *Files identical despite different names*

