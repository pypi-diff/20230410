# Comparing `tmp/smannan_lotr_sdk-3.0.tar.gz` & `tmp/smannan_lotr_sdk-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smannan_lotr_sdk-3.0.tar", last modified: Mon Apr 10 04:08:07 2023, max compression
+gzip compressed data, was "smannan_lotr_sdk-4.0.tar", last modified: Mon Apr 10 04:22:33 2023, max compression
```

## Comparing `smannan_lotr_sdk-3.0.tar` & `smannan_lotr_sdk-4.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 04:08:07.734673 smannan_lotr_sdk-3.0/
--rw-r--r--   0 soniamannan   (501) staff       (20)      256 2023-04-10 04:08:07.734847 smannan_lotr_sdk-3.0/PKG-INFO
--rw-r--r--   0 soniamannan   (501) staff       (20)      415 2023-04-10 03:57:38.000000 smannan_lotr_sdk-3.0/README.md
--rw-r--r--   0 soniamannan   (501) staff       (20)       79 2023-04-10 04:08:07.735854 smannan_lotr_sdk-3.0/setup.cfg
--rw-r--r--   0 soniamannan   (501) staff       (20)      330 2023-04-10 04:07:57.000000 smannan_lotr_sdk-3.0/setup.py
-drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 04:08:07.734199 smannan_lotr_sdk-3.0/smannan_lotr_sdk.egg-info/
--rw-r--r--   0 soniamannan   (501) staff       (20)      256 2023-04-10 04:08:07.000000 smannan_lotr_sdk-3.0/smannan_lotr_sdk.egg-info/PKG-INFO
--rw-r--r--   0 soniamannan   (501) staff       (20)      188 2023-04-10 04:08:07.000000 smannan_lotr_sdk-3.0/smannan_lotr_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 soniamannan   (501) staff       (20)        1 2023-04-10 04:08:07.000000 smannan_lotr_sdk-3.0/smannan_lotr_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 soniamannan   (501) staff       (20)        1 2023-04-10 04:08:07.000000 smannan_lotr_sdk-3.0/smannan_lotr_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 04:22:33.388760 smannan_lotr_sdk-4.0/
+-rw-r--r--   0 soniamannan   (501) staff       (20)      256 2023-04-10 04:22:33.389252 smannan_lotr_sdk-4.0/PKG-INFO
+-rw-r--r--   0 soniamannan   (501) staff       (20)      416 2023-04-10 04:10:34.000000 smannan_lotr_sdk-4.0/README.md
+-rw-r--r--   0 soniamannan   (501) staff       (20)       79 2023-04-10 04:22:33.391330 smannan_lotr_sdk-4.0/setup.cfg
+-rw-r--r--   0 soniamannan   (501) staff       (20)      334 2023-04-10 04:22:12.000000 smannan_lotr_sdk-4.0/setup.py
+drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 04:22:33.373354 smannan_lotr_sdk-4.0/src/
+drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 04:22:33.387678 smannan_lotr_sdk-4.0/src/smannan_lotr_sdk.egg-info/
+-rw-r--r--   0 soniamannan   (501) staff       (20)      256 2023-04-10 04:22:33.000000 smannan_lotr_sdk-4.0/src/smannan_lotr_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 soniamannan   (501) staff       (20)      204 2023-04-10 04:22:33.000000 smannan_lotr_sdk-4.0/src/smannan_lotr_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 soniamannan   (501) staff       (20)        1 2023-04-10 04:22:33.000000 smannan_lotr_sdk-4.0/src/smannan_lotr_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 soniamannan   (501) staff       (20)        1 2023-04-10 04:22:33.000000 smannan_lotr_sdk-4.0/src/smannan_lotr_sdk.egg-info/top_level.txt
```

