# Comparing `tmp/smannan_lotr_sdk-4.0.tar.gz` & `tmp/smannan_lotr_sdk-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smannan_lotr_sdk-4.0.tar", last modified: Mon Apr 10 04:22:33 2023, max compression
+gzip compressed data, was "smannan_lotr_sdk-5.0.tar", last modified: Mon Apr 10 04:58:09 2023, max compression
```

## Comparing `smannan_lotr_sdk-4.0.tar` & `smannan_lotr_sdk-5.0.tar`

### file list

```diff
@@ -1,11 +1,18 @@
-drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 04:22:33.388760 smannan_lotr_sdk-4.0/
--rw-r--r--   0 soniamannan   (501) staff       (20)      256 2023-04-10 04:22:33.389252 smannan_lotr_sdk-4.0/PKG-INFO
--rw-r--r--   0 soniamannan   (501) staff       (20)      416 2023-04-10 04:10:34.000000 smannan_lotr_sdk-4.0/README.md
--rw-r--r--   0 soniamannan   (501) staff       (20)       79 2023-04-10 04:22:33.391330 smannan_lotr_sdk-4.0/setup.cfg
--rw-r--r--   0 soniamannan   (501) staff       (20)      334 2023-04-10 04:22:12.000000 smannan_lotr_sdk-4.0/setup.py
-drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 04:22:33.373354 smannan_lotr_sdk-4.0/src/
-drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 04:22:33.387678 smannan_lotr_sdk-4.0/src/smannan_lotr_sdk.egg-info/
--rw-r--r--   0 soniamannan   (501) staff       (20)      256 2023-04-10 04:22:33.000000 smannan_lotr_sdk-4.0/src/smannan_lotr_sdk.egg-info/PKG-INFO
--rw-r--r--   0 soniamannan   (501) staff       (20)      204 2023-04-10 04:22:33.000000 smannan_lotr_sdk-4.0/src/smannan_lotr_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 soniamannan   (501) staff       (20)        1 2023-04-10 04:22:33.000000 smannan_lotr_sdk-4.0/src/smannan_lotr_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 soniamannan   (501) staff       (20)        1 2023-04-10 04:22:33.000000 smannan_lotr_sdk-4.0/src/smannan_lotr_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 04:58:09.900945 smannan_lotr_sdk-5.0/
+-rw-r--r--   0 soniamannan   (501) staff       (20)      256 2023-04-10 04:58:09.901255 smannan_lotr_sdk-5.0/PKG-INFO
+-rw-r--r--   0 soniamannan   (501) staff       (20)      416 2023-04-10 04:10:34.000000 smannan_lotr_sdk-5.0/README.md
+-rw-r--r--   0 soniamannan   (501) staff       (20)       79 2023-04-10 04:58:09.903020 smannan_lotr_sdk-5.0/setup.cfg
+-rw-r--r--   0 soniamannan   (501) staff       (20)      338 2023-04-10 04:57:36.000000 smannan_lotr_sdk-5.0/setup.py
+drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 04:58:09.883199 smannan_lotr_sdk-5.0/src/
+drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 04:58:09.895184 smannan_lotr_sdk-5.0/src/smannan_lotr_sdk/
+-rw-r--r--   0 soniamannan   (501) staff       (20)        0 2023-04-10 04:21:17.000000 smannan_lotr_sdk-5.0/src/smannan_lotr_sdk/__init__.py
+-rw-r--r--   0 soniamannan   (501) staff       (20)      931 2023-04-10 03:44:05.000000 smannan_lotr_sdk-5.0/src/smannan_lotr_sdk/http_service.py
+-rw-r--r--   0 soniamannan   (501) staff       (20)     2131 2023-04-10 03:44:05.000000 smannan_lotr_sdk-5.0/src/smannan_lotr_sdk/lotr_api_client.py
+-rw-r--r--   0 soniamannan   (501) staff       (20)      591 2023-04-10 02:20:34.000000 smannan_lotr_sdk-5.0/src/smannan_lotr_sdk/movie.py
+-rw-r--r--   0 soniamannan   (501) staff       (20)      274 2023-04-10 02:37:32.000000 smannan_lotr_sdk-5.0/src/smannan_lotr_sdk/quote.py
+-rw-r--r--   0 soniamannan   (501) staff       (20)      870 2023-04-10 03:44:05.000000 smannan_lotr_sdk-5.0/src/smannan_lotr_sdk/test_lotr_client.py
+drwxr-xr-x   0 soniamannan   (501) staff       (20)        0 2023-04-10 04:58:09.900156 smannan_lotr_sdk-5.0/src/smannan_lotr_sdk.egg-info/
+-rw-r--r--   0 soniamannan   (501) staff       (20)      256 2023-04-10 04:58:09.000000 smannan_lotr_sdk-5.0/src/smannan_lotr_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 soniamannan   (501) staff       (20)      415 2023-04-10 04:58:09.000000 smannan_lotr_sdk-5.0/src/smannan_lotr_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 soniamannan   (501) staff       (20)        1 2023-04-10 04:58:09.000000 smannan_lotr_sdk-5.0/src/smannan_lotr_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 soniamannan   (501) staff       (20)       17 2023-04-10 04:58:09.000000 smannan_lotr_sdk-5.0/src/smannan_lotr_sdk.egg-info/top_level.txt
```

