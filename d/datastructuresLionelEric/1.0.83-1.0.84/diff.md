# Comparing `tmp/datastructuresLionelEric-1.0.83.tar.gz` & `tmp/datastructuresLionelEric-1.0.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datastructuresLionelEric-1.0.83.tar", last modified: Sun Apr  9 22:26:47 2023, max compression
+gzip compressed data, was "datastructuresLionelEric-1.0.84.tar", last modified: Sun Apr  9 22:28:00 2023, max compression
```

## Comparing `datastructuresLionelEric-1.0.83.tar` & `datastructuresLionelEric-1.0.84.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:26:47.344836 datastructuresLionelEric-1.0.83/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-03-29 13:29:16.000000 datastructuresLionelEric-1.0.83/.DS_Store
--rw-r--r--   0 lionelhasan   (501) staff       (20)      152 2023-04-09 22:26:47.344666 datastructuresLionelEric-1.0.83/PKG-INFO
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:26:47.344395 datastructuresLionelEric-1.0.83/datastructuresLionelEric.egg-info/
--rw-r--r--   0 lionelhasan   (501) staff       (20)      152 2023-04-09 22:26:47.000000 datastructuresLionelEric-1.0.83/datastructuresLionelEric.egg-info/PKG-INFO
--rw-r--r--   0 lionelhasan   (501) staff       (20)      210 2023-04-09 22:26:47.000000 datastructuresLionelEric-1.0.83/datastructuresLionelEric.egg-info/SOURCES.txt
--rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-09 22:26:47.000000 datastructuresLionelEric-1.0.83/datastructuresLionelEric.egg-info/dependency_links.txt
--rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-09 22:26:47.000000 datastructuresLionelEric-1.0.83/datastructuresLionelEric.egg-info/top_level.txt
--rw-r--r--   0 lionelhasan   (501) staff       (20)       38 2023-04-09 22:26:47.344893 datastructuresLionelEric-1.0.83/setup.cfg
--rw-r--r--   0 lionelhasan   (501) staff       (20)      230 2023-04-09 22:26:40.000000 datastructuresLionelEric-1.0.83/setup.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:28:00.677659 datastructuresLionelEric-1.0.84/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-03-29 13:29:16.000000 datastructuresLionelEric-1.0.84/.DS_Store
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      162 2023-04-09 22:28:00.677503 datastructuresLionelEric-1.0.84/PKG-INFO
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:28:00.677305 datastructuresLionelEric-1.0.84/datastructuresLionelEric.egg-info/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      162 2023-04-09 22:28:00.000000 datastructuresLionelEric-1.0.84/datastructuresLionelEric.egg-info/PKG-INFO
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      210 2023-04-09 22:28:00.000000 datastructuresLionelEric-1.0.84/datastructuresLionelEric.egg-info/SOURCES.txt
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-09 22:28:00.000000 datastructuresLionelEric-1.0.84/datastructuresLionelEric.egg-info/dependency_links.txt
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-09 22:28:00.000000 datastructuresLionelEric-1.0.84/datastructuresLionelEric.egg-info/top_level.txt
+-rw-r--r--   0 lionelhasan   (501) staff       (20)       38 2023-04-09 22:28:00.677702 datastructuresLionelEric-1.0.84/setup.cfg
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      240 2023-04-09 22:27:57.000000 datastructuresLionelEric-1.0.84/setup.py
```

### Comparing `datastructuresLionelEric-1.0.83/.DS_Store` & `datastructuresLionelEric-1.0.84/.DS_Store`

 * *Files identical despite different names*

