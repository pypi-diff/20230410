# Comparing `tmp/pepelimpiezas-0.1.tar.gz` & `tmp/pepelimpiezas-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepelimpiezas-0.1.tar", last modified: Mon Apr 10 19:09:28 2023, max compression
+gzip compressed data, was "pepelimpiezas-0.2.tar", last modified: Mon Apr 10 19:20:14 2023, max compression
```

## Comparing `pepelimpiezas-0.1.tar` & `pepelimpiezas-0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 19:09:27.994462 pepelimpiezas-0.1/
--rw-r--r--   0 root         (0) root         (0)      224 2023-04-10 19:09:27.994462 pepelimpiezas-0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 19:09:27.994462 pepelimpiezas-0.1/pepelimpiezas/
--rw-r--r--   0 root         (0) root         (0)      138 2023-04-10 19:07:08.000000 pepelimpiezas-0.1/pepelimpiezas/copiar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 19:09:27.994462 pepelimpiezas-0.1/pepelimpiezas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      224 2023-04-10 19:09:27.000000 pepelimpiezas-0.1/pepelimpiezas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      180 2023-04-10 19:09:27.000000 pepelimpiezas-0.1/pepelimpiezas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 19:09:27.000000 pepelimpiezas-0.1/pepelimpiezas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 19:09:27.000000 pepelimpiezas-0.1/pepelimpiezas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 19:09:27.994462 pepelimpiezas-0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      338 2023-04-10 19:06:37.000000 pepelimpiezas-0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 19:20:14.482829 pepelimpiezas-0.2/
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-10 19:12:53.000000 pepelimpiezas-0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      224 2023-04-10 19:20:14.482829 pepelimpiezas-0.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 19:20:14.482829 pepelimpiezas-0.2/pepelimpiezas/
+-rw-r--r--   0 root         (0) root         (0)      138 2023-04-10 19:07:08.000000 pepelimpiezas-0.2/pepelimpiezas/copiar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 19:20:14.482829 pepelimpiezas-0.2/pepelimpiezas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      224 2023-04-10 19:20:14.000000 pepelimpiezas-0.2/pepelimpiezas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      192 2023-04-10 19:20:14.000000 pepelimpiezas-0.2/pepelimpiezas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 19:20:14.000000 pepelimpiezas-0.2/pepelimpiezas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 19:20:14.000000 pepelimpiezas-0.2/pepelimpiezas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 19:20:14.482829 pepelimpiezas-0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      338 2023-04-10 19:20:07.000000 pepelimpiezas-0.2/setup.py
```

