# Comparing `tmp/ork-0.0.1.tar.gz` & `tmp/ork-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ork-0.0.1.tar", last modified: Sun May 30 16:15:01 2021, max compression
+gzip compressed data, was "ork-0.0.2.tar", last modified: Mon Apr 10 18:28:32 2023, max compression
```

## Comparing `ork-0.0.1.tar` & `ork-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-30 16:15:01.877689 ork-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-05-30 16:14:53.000000 ork-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      238 2021-05-30 16:15:01.877689 ork-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      683 2021-05-30 16:14:53.000000 ork-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-30 16:15:01.877689 ork-0.0.1/ork/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-30 16:14:53.000000 ork-0.0.1/ork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12764 2021-05-30 16:14:53.000000 ork-0.0.1/ork/namegen.json
--rw-r--r--   0 runner    (1001) docker     (121)     1015 2021-05-30 16:14:53.000000 ork-0.0.1/ork/namegen.py
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-05-30 16:14:53.000000 ork-0.0.1/ork/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-30 16:15:01.877689 ork-0.0.1/ork.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      238 2021-05-30 16:15:01.000000 ork-0.0.1/ork.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      208 2021-05-30 16:15:01.000000 ork-0.0.1/ork.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-30 16:15:01.000000 ork-0.0.1/ork.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-05-30 16:15:01.000000 ork-0.0.1/ork.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-30 16:15:01.877689 ork-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      315 2021-05-30 16:14:53.000000 ork-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-30 16:15:01.877689 ork-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (121)      524 2021-05-30 16:14:53.000000 ork-0.0.1/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:28:32.922037 ork-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 18:28:22.000000 ork-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-10 18:28:32.922037 ork-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-10 18:28:22.000000 ork-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:28:32.922037 ork-0.0.2/ork/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-10 18:28:22.000000 ork-0.0.2/ork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-04-10 18:28:22.000000 ork-0.0.2/ork/namegen.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-10 18:28:22.000000 ork-0.0.2/ork/namegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-10 18:28:22.000000 ork-0.0.2/ork/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:28:32.922037 ork-0.0.2/ork.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-10 18:28:32.000000 ork-0.0.2/ork.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-10 18:28:32.000000 ork-0.0.2/ork.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:28:32.000000 ork-0.0.2/ork.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-10 18:28:32.000000 ork-0.0.2/ork.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 18:28:32.922037 ork-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-10 18:28:22.000000 ork-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:28:32.922037 ork-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-10 18:28:22.000000 ork-0.0.2/test/test.py
```

### Comparing `ork-0.0.1/LICENSE` & `ork-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ork-0.0.1/ork/namegen.json` & `ork-0.0.2/ork/namegen.json`

 * *Files identical despite different names*

