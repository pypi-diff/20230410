# Comparing `tmp/precession-1.0.3.tar.gz` & `tmp/precession-2.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/precession-1.0.3.tar", last modified: Tue Nov  6 22:38:39 2018, max compression
+gzip compressed data, was "precession-2.0.0.dev0.tar", last modified: Mon Apr 10 12:57:13 2023, max compression
```

## Comparing `precession-1.0.3.tar` & `precession-2.0.0.dev0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 dgerosa    (501) staff       (20)        0 2018-11-06 22:38:39.000000 precession-1.0.3/
--rw-r--r--   0 dgerosa    (501) staff       (20)     8290 2018-11-06 22:38:39.000000 precession-1.0.3/PKG-INFO
-drwxr-xr-x   0 dgerosa    (501) staff       (20)        0 2018-11-06 22:38:39.000000 precession-1.0.3/precession.egg-info/
--rw-r--r--   0 dgerosa    (501) staff       (20)     8290 2018-11-06 22:38:39.000000 precession-1.0.3/precession.egg-info/PKG-INFO
--rw-r--r--   0 dgerosa    (501) staff       (20)        1 2017-09-21 16:14:49.000000 precession-1.0.3/precession.egg-info/not-zip-safe
--rw-r--r--   0 dgerosa    (501) staff       (20)      321 2018-11-06 22:38:39.000000 precession-1.0.3/precession.egg-info/SOURCES.txt
--rw-r--r--   0 dgerosa    (501) staff       (20)       37 2018-11-06 22:38:39.000000 precession-1.0.3/precession.egg-info/requires.txt
--rw-r--r--   0 dgerosa    (501) staff       (20)       11 2018-11-06 22:38:39.000000 precession-1.0.3/precession.egg-info/top_level.txt
--rw-r--r--   0 dgerosa    (501) staff       (20)        1 2018-11-06 22:38:39.000000 precession-1.0.3/precession.egg-info/dependency_links.txt
--rw-r--r--   0 dgerosa    (501) staff       (20)     1608 2018-11-06 22:37:31.000000 precession-1.0.3/setup.py
--rw-r--r--   0 dgerosa    (501) staff       (20)       38 2018-11-06 22:38:39.000000 precession-1.0.3/setup.cfg
--rw-r--r--   0 dgerosa    (501) staff       (20)     6313 2018-11-06 22:37:31.000000 precession-1.0.3/README.rst
-drwxr-xr-x   0 dgerosa    (501) staff       (20)        0 2018-11-06 22:38:39.000000 precession-1.0.3/precession/
--rw-r--r--   0 dgerosa    (501) staff       (20)   182279 2018-11-06 22:37:31.000000 precession-1.0.3/precession/precession.py
-drwxr-xr-x   0 dgerosa    (501) staff       (20)        0 2018-11-06 22:38:39.000000 precession-1.0.3/precession/test/
--rw-r--r--   0 dgerosa    (501) staff       (20)       20 2018-11-06 22:37:31.000000 precession-1.0.3/precession/test/__init__.py
--rw-r--r--   0 dgerosa    (501) staff       (20)    25232 2018-11-06 22:37:31.000000 precession-1.0.3/precession/test/test.py
--rw-r--r--   0 dgerosa    (501) staff       (20)      238 2018-11-06 22:37:31.000000 precession-1.0.3/precession/__init__.py
+drwxr-xr-x   0 dgerosa    (501) staff       (20)        0 2023-04-10 12:57:13.897329 precession-2.0.0.dev0/
+-rw-r--r--   0 dgerosa    (501) staff       (20)     1071 2022-02-03 16:32:40.000000 precession-2.0.0.dev0/LICENSE
+-rw-r--r--   0 dgerosa    (501) staff       (20)       24 2023-04-08 16:44:47.000000 precession-2.0.0.dev0/MANIFEST.in
+-rw-r--r--   0 dgerosa    (501) staff       (20)      469 2023-04-10 12:57:13.896834 precession-2.0.0.dev0/PKG-INFO
+-rw-r--r--   0 dgerosa    (501) staff       (20)     2755 2023-04-10 07:58:58.000000 precession-2.0.0.dev0/README.md
+drwxr-xr-x   0 dgerosa    (501) staff       (20)        0 2023-04-10 12:57:13.893781 precession-2.0.0.dev0/precession/
+-rw-r--r--   0 dgerosa    (501) staff       (20)       54 2023-04-08 16:09:00.000000 precession-2.0.0.dev0/precession/__init__.py
+-rw-r--r--   0 dgerosa    (501) staff       (20)      463 2023-04-10 12:56:42.000000 precession-2.0.0.dev0/precession/__version__.py
+-rw-r--r--   0 dgerosa    (501) staff       (20)   226011 2023-04-08 16:08:25.000000 precession-2.0.0.dev0/precession/precession.py
+drwxr-xr-x   0 dgerosa    (501) staff       (20)        0 2023-04-10 12:57:13.896097 precession-2.0.0.dev0/precession.egg-info/
+-rw-r--r--   0 dgerosa    (501) staff       (20)      469 2023-04-10 12:57:13.000000 precession-2.0.0.dev0/precession.egg-info/PKG-INFO
+-rw-r--r--   0 dgerosa    (501) staff       (20)      331 2023-04-10 12:57:13.000000 precession-2.0.0.dev0/precession.egg-info/SOURCES.txt
+-rw-r--r--   0 dgerosa    (501) staff       (20)        1 2023-04-10 12:57:13.000000 precession-2.0.0.dev0/precession.egg-info/dependency_links.txt
+-rw-r--r--   0 dgerosa    (501) staff       (20)        1 2023-04-08 16:11:27.000000 precession-2.0.0.dev0/precession.egg-info/not-zip-safe
+-rw-r--r--   0 dgerosa    (501) staff       (20)       19 2023-04-10 12:57:13.000000 precession-2.0.0.dev0/precession.egg-info/requires.txt
+-rw-r--r--   0 dgerosa    (501) staff       (20)       11 2023-04-10 12:57:13.000000 precession-2.0.0.dev0/precession.egg-info/top_level.txt
+-rw-r--r--   0 dgerosa    (501) staff       (20)       18 2023-04-10 07:39:31.000000 precession-2.0.0.dev0/requirements.txt
+-rw-r--r--   0 dgerosa    (501) staff       (20)       38 2023-04-10 12:57:13.897439 precession-2.0.0.dev0/setup.cfg
+-rw-r--r--   0 dgerosa    (501) staff       (20)      961 2023-04-10 07:58:24.000000 precession-2.0.0.dev0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

