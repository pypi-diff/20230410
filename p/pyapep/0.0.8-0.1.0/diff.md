# Comparing `tmp/pyapep-0.0.8.tar.gz` & `tmp/pyapep-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyapep-0.0.8.tar", last modified: Thu Nov 18 13:25:25 2021, max compression
+gzip compressed data, was "pyapep-0.1.0.tar", last modified: Mon Apr 10 12:53:37 2023, max compression
```

## Comparing `pyapep-0.0.8.tar` & `pyapep-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2021-11-18 13:25:25.615148 pyapep-0.0.8/
--rw-rw-rw-   0        0        0      399 2021-11-18 13:25:25.614262 pyapep-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1226 2021-11-18 12:00:33.000000 pyapep-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2021-11-18 13:25:25.580263 pyapep-0.0.8/pyapep/
--rw-rw-rw-   0        0        0        0 2021-07-14 09:43:53.000000 pyapep-0.0.8/pyapep/__init__.py
--rw-rw-rw-   0        0        0    24684 2021-11-18 12:33:12.000000 pyapep-0.0.8/pyapep/simsep.py
--rw-rw-rw-   0        0        0     5982 2021-11-18 12:30:00.000000 pyapep-0.0.8/pyapep/simsto.py
-drwxrwxrwx   0        0        0        0 2021-11-18 13:25:25.611177 pyapep-0.0.8/pyapep.egg-info/
--rw-rw-rw-   0        0        0      399 2021-11-18 13:25:25.000000 pyapep-0.0.8/pyapep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2021-11-18 13:25:25.000000 pyapep-0.0.8/pyapep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-11-18 13:25:25.000000 pyapep-0.0.8/pyapep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2021-11-18 13:25:25.000000 pyapep-0.0.8/pyapep.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2021-11-18 13:25:25.000000 pyapep-0.0.8/pyapep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-11-18 13:25:25.616146 pyapep-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      676 2021-11-18 13:25:12.000000 pyapep-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:53:37.013400 pyapep-0.1.0/
+-rw-rw-rw-   0        0        0      352 2023-04-10 12:53:37.012387 pyapep-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2022-05-27 15:52:19.000000 pyapep-0.1.0/README
+drwxrwxrwx   0        0        0        0 2023-04-10 12:53:36.969858 pyapep-0.1.0/pyapep/
+-rw-rw-rw-   0        0        0        0 2022-10-19 06:19:02.000000 pyapep-0.1.0/pyapep/__init__.py
+-rw-rw-rw-   0        0        0    22187 2022-12-20 03:37:29.000000 pyapep-0.1.0/pyapep/isofit.py
+-rw-rw-rw-   0        0        0     8353 2022-05-27 15:52:19.000000 pyapep-0.1.0/pyapep/simide.py
+-rw-rw-rw-   0        0        0    90223 2022-10-19 06:19:02.000000 pyapep-0.1.0/pyapep/simsep.py
+-rw-rw-rw-   0        0        0    87603 2022-10-19 06:19:02.000000 pyapep-0.1.0/pyapep/simsep_backup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:53:37.009477 pyapep-0.1.0/pyapep.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-04-10 12:53:35.000000 pyapep-0.1.0/pyapep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-04-10 12:53:36.000000 pyapep-0.1.0/pyapep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 12:53:35.000000 pyapep-0.1.0/pyapep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-10 12:53:36.000000 pyapep-0.1.0/pyapep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-10 12:53:36.000000 pyapep-0.1.0/pyapep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 12:53:37.014405 pyapep-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      931 2023-04-10 12:52:58.000000 pyapep-0.1.0/setup.py
```

