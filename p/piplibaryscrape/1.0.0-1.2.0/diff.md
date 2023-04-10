# Comparing `tmp/piplibaryscrape-1.0.0.tar.gz` & `tmp/piplibaryscrape-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piplibaryscrape-1.0.0.tar", last modified: Thu Apr  6 20:31:31 2023, max compression
+gzip compressed data, was "piplibaryscrape-1.2.0.tar", last modified: Mon Apr 10 17:23:34 2023, max compression
```

## Comparing `piplibaryscrape-1.0.0.tar` & `piplibaryscrape-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:31:31.178062 piplibaryscrape-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      309 2023-04-06 20:31:31.178062 piplibaryscrape-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:31:31.178062 piplibaryscrape-1.0.0/piplibaryscrape/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-06 20:31:30.000000 piplibaryscrape-1.0.0/piplibaryscrape/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:31:31.178062 piplibaryscrape-1.0.0/piplibaryscrape.egg-info/
--rw-r--r--   0 root         (0) root         (0)      309 2023-04-06 20:31:31.000000 piplibaryscrape-1.0.0/piplibaryscrape.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      192 2023-04-06 20:31:31.000000 piplibaryscrape-1.0.0/piplibaryscrape.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 20:31:31.000000 piplibaryscrape-1.0.0/piplibaryscrape.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-06 20:31:31.000000 piplibaryscrape-1.0.0/piplibaryscrape.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-06 20:31:31.178062 piplibaryscrape-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      522 2023-04-06 20:31:30.000000 piplibaryscrape-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 17:23:34.570668 piplibaryscrape-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-04-10 17:23:34.570668 piplibaryscrape-1.2.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 17:23:34.570668 piplibaryscrape-1.2.0/piplibaryscrape/
+-rw-r--r--   0 root         (0) root         (0)    70957 2023-04-10 17:23:33.000000 piplibaryscrape-1.2.0/piplibaryscrape/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 17:23:34.570668 piplibaryscrape-1.2.0/piplibaryscrape.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-04-10 17:23:34.000000 piplibaryscrape-1.2.0/piplibaryscrape.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      192 2023-04-10 17:23:34.000000 piplibaryscrape-1.2.0/piplibaryscrape.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 17:23:34.000000 piplibaryscrape-1.2.0/piplibaryscrape.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-10 17:23:34.000000 piplibaryscrape-1.2.0/piplibaryscrape.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 17:23:34.570668 piplibaryscrape-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      628 2023-04-10 17:23:33.000000 piplibaryscrape-1.2.0/setup.py
```

