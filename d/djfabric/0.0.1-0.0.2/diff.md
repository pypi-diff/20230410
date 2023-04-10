# Comparing `tmp/djfabric-0.0.1.tar.gz` & `tmp/djfabric-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djfabric-0.0.1.tar", last modified: Fri Mar 31 16:23:59 2023, max compression
+gzip compressed data, was "djfabric-0.0.2.tar", last modified: Mon Apr 10 06:28:41 2023, max compression
```

## Comparing `djfabric-0.0.1.tar` & `djfabric-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-03-31 16:23:59.059815 djfabric-0.0.1/
--rw-rw-r--   0 dev       (1000) dev       (1000)      746 2021-08-08 06:51:05.000000 djfabric-0.0.1/LICENSE
--rw-rw-r--   0 dev       (1000) dev       (1000)      161 2021-08-08 06:51:05.000000 djfabric-0.0.1/MANIFEST.in
--rw-rw-r--   0 dev       (1000) dev       (1000)      296 2023-03-31 16:23:59.059815 djfabric-0.0.1/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)      346 2023-03-31 16:19:28.000000 djfabric-0.0.1/README.md
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-03-31 16:23:59.059815 djfabric-0.0.1/djfabric/
--rw-rw-r--   0 dev       (1000) dev       (1000)     6086 2023-03-31 16:16:18.000000 djfabric-0.0.1/djfabric/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     2878 2022-11-12 11:12:09.000000 djfabric-0.0.1/djfabric/fab.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-03-31 16:23:59.059815 djfabric-0.0.1/djfabric.egg-info/
--rw-rw-r--   0 dev       (1000) dev       (1000)      296 2023-03-31 16:23:59.000000 djfabric-0.0.1/djfabric.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)      261 2023-03-31 16:23:59.000000 djfabric-0.0.1/djfabric.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)        1 2023-03-31 16:23:59.000000 djfabric-0.0.1/djfabric.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       42 2023-03-31 16:23:59.000000 djfabric-0.0.1/djfabric.egg-info/requires.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)        9 2023-03-31 16:23:59.000000 djfabric-0.0.1/djfabric.egg-info/top_level.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       42 2023-03-31 16:19:28.000000 djfabric-0.0.1/requirements.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       79 2023-03-31 16:23:59.059815 djfabric-0.0.1/setup.cfg
--rw-rw-r--   0 dev       (1000) dev       (1000)      528 2023-03-31 16:22:16.000000 djfabric-0.0.1/setup.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-10 06:28:41.774933 djfabric-0.0.2/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      746 2021-08-08 06:51:05.000000 djfabric-0.0.2/LICENSE
+-rw-rw-r--   0 dev       (1000) dev       (1000)      161 2021-08-08 06:51:05.000000 djfabric-0.0.2/MANIFEST.in
+-rw-rw-r--   0 dev       (1000) dev       (1000)      296 2023-04-10 06:28:41.774933 djfabric-0.0.2/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)      346 2023-03-31 16:19:28.000000 djfabric-0.0.2/README.md
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-10 06:28:41.774933 djfabric-0.0.2/djfabric/
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2023-04-10 06:28:10.000000 djfabric-0.0.2/djfabric/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     7650 2023-04-10 06:28:10.000000 djfabric-0.0.2/djfabric/fab.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-10 06:28:41.774933 djfabric-0.0.2/djfabric.egg-info/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      296 2023-04-10 06:28:41.000000 djfabric-0.0.2/djfabric.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)      261 2023-04-10 06:28:41.000000 djfabric-0.0.2/djfabric.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)        1 2023-04-10 06:28:41.000000 djfabric-0.0.2/djfabric.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       60 2023-04-10 06:28:41.000000 djfabric-0.0.2/djfabric.egg-info/requires.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)        9 2023-04-10 06:28:41.000000 djfabric-0.0.2/djfabric.egg-info/top_level.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       60 2023-04-10 05:02:33.000000 djfabric-0.0.2/requirements.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       79 2023-04-10 06:28:41.774933 djfabric-0.0.2/setup.cfg
+-rw-rw-r--   0 dev       (1000) dev       (1000)      528 2023-04-10 05:04:36.000000 djfabric-0.0.2/setup.py
```

### Comparing `djfabric-0.0.1/LICENSE` & `djfabric-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `djfabric-0.0.1/setup.py` & `djfabric-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 
 with open('requirements.txt') as f:
     requires = f.read().splitlines()
 
 
-version = '0.0.1'
+version = '0.0.2'
 url = 'https://github.com/pmaigutyak/djfabric'
 
 
 setup(
     name='djfabric',
     version=version,
     description='Django deploy app',
```

