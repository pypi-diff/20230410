# Comparing `tmp/anshudi-0.0.1.tar.gz` & `tmp/anshudi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anshudi-0.0.1.tar", last modified: Mon Apr 10 05:46:53 2023, max compression
+gzip compressed data, was "anshudi-0.0.2.tar", last modified: Mon Apr 10 05:51:19 2023, max compression
```

## Comparing `anshudi-0.0.1.tar` & `anshudi-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 05:46:53.514450 anshudi-0.0.1/
--rw-rw-rw-   0        0        0      138 2023-04-10 05:46:53.505515 anshudi-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 05:46:53.469742 anshudi-0.0.1/anshudi/
--rw-rw-rw-   0        0        0        0 2023-04-10 05:36:11.000000 anshudi-0.0.1/anshudi/__init__.py
--rw-rw-rw-   0        0        0      398 2023-04-10 05:46:05.000000 anshudi-0.0.1/anshudi/anshu.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:46:53.505515 anshudi-0.0.1/anshudi.egg-info/
--rw-rw-rw-   0        0        0      138 2023-04-10 05:46:53.000000 anshudi-0.0.1/anshudi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2023-04-10 05:46:53.000000 anshudi-0.0.1/anshudi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 05:46:53.000000 anshudi-0.0.1/anshudi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-10 05:46:53.000000 anshudi-0.0.1/anshudi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-10 05:46:53.000000 anshudi-0.0.1/anshudi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 05:46:53.515839 anshudi-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-04-10 05:42:54.000000 anshudi-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:51:19.442158 anshudi-0.0.2/
+-rw-rw-rw-   0        0        0      138 2023-04-10 05:51:19.442158 anshudi-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 05:51:19.415536 anshudi-0.0.2/anshudi/
+-rw-rw-rw-   0        0        0        0 2023-04-10 05:36:11.000000 anshudi-0.0.2/anshudi/__init__.py
+-rw-rw-rw-   0        0        0      400 2023-04-10 05:51:02.000000 anshudi-0.0.2/anshudi/anshu.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:51:19.442158 anshudi-0.0.2/anshudi.egg-info/
+-rw-rw-rw-   0        0        0      138 2023-04-10 05:51:19.000000 anshudi-0.0.2/anshudi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2023-04-10 05:51:19.000000 anshudi-0.0.2/anshudi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 05:51:19.000000 anshudi-0.0.2/anshudi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-10 05:51:19.000000 anshudi-0.0.2/anshudi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-10 05:51:19.000000 anshudi-0.0.2/anshudi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 05:51:19.448960 anshudi-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-04-10 05:51:08.000000 anshudi-0.0.2/setup.py
```

