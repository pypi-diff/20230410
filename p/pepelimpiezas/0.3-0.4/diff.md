# Comparing `tmp/pepelimpiezas-0.3.tar.gz` & `tmp/pepelimpiezas-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepelimpiezas-0.3.tar", last modified: Mon Apr 10 19:27:48 2023, max compression
+gzip compressed data, was "pepelimpiezas-0.4.tar", last modified: Mon Apr 10 19:32:05 2023, max compression
```

## Comparing `pepelimpiezas-0.3.tar` & `pepelimpiezas-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 19:27:48.767515 pepelimpiezas-0.3/
--rw-r--r--   0 root         (0) root         (0)      234 2023-04-10 19:27:48.767515 pepelimpiezas-0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      556 2023-04-10 19:24:43.000000 pepelimpiezas-0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 19:27:48.767515 pepelimpiezas-0.3/pepelimpiezas/
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-10 19:26:36.000000 pepelimpiezas-0.3/pepelimpiezas/__init__.py
--rw-r--r--   0 root         (0) root         (0)       75 2023-04-10 19:27:03.000000 pepelimpiezas-0.3/pepelimpiezas/poc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 19:27:48.767515 pepelimpiezas-0.3/pepelimpiezas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      234 2023-04-10 19:27:48.000000 pepelimpiezas-0.3/pepelimpiezas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      213 2023-04-10 19:27:48.000000 pepelimpiezas-0.3/pepelimpiezas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 19:27:48.000000 pepelimpiezas-0.3/pepelimpiezas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-10 19:27:48.000000 pepelimpiezas-0.3/pepelimpiezas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 19:27:48.767515 pepelimpiezas-0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      244 2023-04-10 19:27:41.000000 pepelimpiezas-0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 19:32:05.292419 pepelimpiezas-0.4/
+-rw-r--r--   0 root         (0) root         (0)      234 2023-04-10 19:32:05.292419 pepelimpiezas-0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      556 2023-04-10 19:24:43.000000 pepelimpiezas-0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 19:32:05.292419 pepelimpiezas-0.4/pepelimpiezas/
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-10 19:26:36.000000 pepelimpiezas-0.4/pepelimpiezas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       97 2023-04-10 19:31:30.000000 pepelimpiezas-0.4/pepelimpiezas/poc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 19:32:05.292419 pepelimpiezas-0.4/pepelimpiezas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      234 2023-04-10 19:32:05.000000 pepelimpiezas-0.4/pepelimpiezas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      213 2023-04-10 19:32:05.000000 pepelimpiezas-0.4/pepelimpiezas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 19:32:05.000000 pepelimpiezas-0.4/pepelimpiezas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-10 19:32:05.000000 pepelimpiezas-0.4/pepelimpiezas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 19:32:05.292419 pepelimpiezas-0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      244 2023-04-10 19:31:56.000000 pepelimpiezas-0.4/setup.py
```

### Comparing `pepelimpiezas-0.3/README.md` & `pepelimpiezas-0.4/README.md`

 * *Files identical despite different names*

