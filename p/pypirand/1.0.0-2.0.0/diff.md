# Comparing `tmp/pypirand-1.0.0.tar.gz` & `tmp/pypirand-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypirand-1.0.0.tar", last modified: Sun Apr  9 21:24:27 2023, max compression
+gzip compressed data, was "pypirand-2.0.0.tar", last modified: Mon Apr 10 10:26:25 2023, max compression
```

## Comparing `pypirand-1.0.0.tar` & `pypirand-2.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 21:24:27.456254 pypirand-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      413 2023-04-09 21:24:27.456254 pypirand-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 21:24:27.456254 pypirand-1.0.0/pypirand/
--rw-r--r--   0 root         (0) root         (0)      498 2023-04-09 21:24:26.000000 pypirand-1.0.0/pypirand/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 21:24:27.456254 pypirand-1.0.0/pypirand.egg-info/
--rw-r--r--   0 root         (0) root         (0)      413 2023-04-09 21:24:27.000000 pypirand-1.0.0/pypirand.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      157 2023-04-09 21:24:27.000000 pypirand-1.0.0/pypirand.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 21:24:27.000000 pypirand-1.0.0/pypirand.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-09 21:24:27.000000 pypirand-1.0.0/pypirand.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 21:24:27.456254 pypirand-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      626 2023-04-09 21:24:26.000000 pypirand-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:26:25.719827 pypirand-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)      413 2023-04-10 10:26:25.719827 pypirand-2.0.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:26:25.719827 pypirand-2.0.0/pypirand/
+-rw-r--r--   0 root         (0) root         (0)    81719 2023-04-10 10:26:25.000000 pypirand-2.0.0/pypirand/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:26:25.719827 pypirand-2.0.0/pypirand.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      413 2023-04-10 10:26:25.000000 pypirand-2.0.0/pypirand.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      157 2023-04-10 10:26:25.000000 pypirand-2.0.0/pypirand.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 10:26:25.000000 pypirand-2.0.0/pypirand.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-10 10:26:25.000000 pypirand-2.0.0/pypirand.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 10:26:25.719827 pypirand-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      626 2023-04-10 10:26:24.000000 pypirand-2.0.0/setup.py
```

### Comparing `pypirand-1.0.0/setup.py` & `pypirand-2.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '2.0.0'
 DESCRIPTION = "Package that can generate a random password of any lenght"
 LONG_DESCRIPTION = "Package that can generate a random password of any lenght"
 
 # Setting up
 setup(
     name="pypirand",
     version=VERSION,
```

