# Comparing `tmp/python-sotools-0.1.2.tar.gz` & `tmp/python-sotools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sotools-0.1.2.tar", last modified: Fri Apr  7 21:23:00 2023, max compression
+gzip compressed data, was "python-sotools-0.1.3.tar", last modified: Mon Apr 10 17:05:57 2023, max compression
```

## Comparing `python-sotools-0.1.2.tar` & `python-sotools-0.1.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-07 21:23:00.840027 python-sotools-0.1.2/
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       51 2022-02-24 21:18:50.000000 python-sotools-0.1.2/.coveragerc
-drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-07 21:23:00.826693 python-sotools-0.1.2/.github/
-drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-07 21:23:00.830027 python-sotools-0.1.2/.github/workflows/
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      623 2022-02-24 21:25:31.000000 python-sotools-0.1.2/.github/workflows/coverage.yml
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      603 2022-02-24 21:28:59.000000 python-sotools-0.1.2/.github/workflows/lint.yml
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      647 2022-02-24 22:27:09.000000 python-sotools-0.1.2/.github/workflows/test.yml
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       77 2023-03-06 17:24:24.000000 python-sotools-0.1.2/.gitignore
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      788 2023-04-07 21:20:55.000000 python-sotools-0.1.2/HISTORY
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     2058 2023-04-07 21:23:00.840027 python-sotools-0.1.2/PKG-INFO
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1548 2023-03-06 16:40:47.000000 python-sotools-0.1.2/README.md
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      926 2023-03-06 17:06:41.000000 python-sotools-0.1.2/pyproject.toml
-drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-07 21:23:00.833360 python-sotools-0.1.2/python_sotools.egg-info/
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     2058 2023-04-07 21:23:00.000000 python-sotools-0.1.2/python_sotools.egg-info/PKG-INFO
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1188 2023-04-07 21:23:00.000000 python-sotools-0.1.2/python_sotools.egg-info/SOURCES.txt
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)        1 2023-04-07 21:23:00.000000 python-sotools-0.1.2/python_sotools.egg-info/dependency_links.txt
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       91 2023-04-07 21:23:00.000000 python-sotools-0.1.2/python_sotools.egg-info/entry_points.txt
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       11 2023-04-07 21:23:00.000000 python-sotools-0.1.2/python_sotools.egg-info/requires.txt
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)        8 2023-04-07 21:23:00.000000 python-sotools-0.1.2/python_sotools.egg-info/top_level.txt
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       38 2023-04-07 21:23:00.840027 python-sotools-0.1.2/setup.cfg
-drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-07 21:23:00.833360 python-sotools-0.1.2/sotools/
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     2286 2023-03-06 16:46:09.000000 python-sotools-0.1.2/sotools/__init__.py
-drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-07 21:23:00.833360 python-sotools-0.1.2/sotools/dl_cache/
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     6434 2022-06-02 20:48:51.000000 python-sotools-0.1.2/sotools/dl_cache/__init__.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     2338 2022-06-02 20:48:51.000000 python-sotools-0.1.2/sotools/dl_cache/dl_cache.py
-drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-07 21:23:00.836694 python-sotools-0.1.2/sotools/dl_cache/extensions/
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1003 2022-06-02 20:48:51.000000 python-sotools-0.1.2/sotools/dl_cache/extensions/__init__.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      718 2022-06-02 20:48:51.000000 python-sotools-0.1.2/sotools/dl_cache/extensions/generator.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1922 2022-06-02 20:48:51.000000 python-sotools-0.1.2/sotools/dl_cache/extensions/hwcaps.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     3466 2022-06-02 20:48:51.000000 python-sotools-0.1.2/sotools/dl_cache/flags.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     3376 2022-06-02 20:48:51.000000 python-sotools-0.1.2/sotools/dl_cache/structure.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      455 2023-03-06 16:40:47.000000 python-sotools-0.1.2/sotools/ldd.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)    11541 2023-03-06 16:54:57.000000 python-sotools-0.1.2/sotools/libraryset.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     3870 2023-04-07 20:58:44.000000 python-sotools-0.1.2/sotools/linker.py
-drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-07 21:23:00.836694 python-sotools-0.1.2/sotools/scripts/
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)        0 2023-03-06 16:40:47.000000 python-sotools-0.1.2/sotools/scripts/__init__.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1664 2023-03-06 16:40:47.000000 python-sotools-0.1.2/sotools/scripts/ldconfig.py
--rwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)     1194 2023-03-06 16:40:47.000000 python-sotools-0.1.2/sotools/scripts/ldd.py
--rwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)     1074 2023-03-06 16:40:47.000000 python-sotools-0.1.2/sotools/scripts/sowhich.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      124 2022-01-31 23:30:48.000000 python-sotools-0.1.2/sotools/util.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      160 2023-04-07 21:23:00.000000 python-sotools-0.1.2/sotools/version.py
-drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-07 21:23:00.836694 python-sotools-0.1.2/tests/
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       68 2023-04-07 20:45:59.000000 python-sotools-0.1.2/tests/__init__.py
-drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-07 21:23:00.836694 python-sotools-0.1.2/tests/assets/
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)    11236 2022-03-08 17:17:01.000000 python-sotools-0.1.2/tests/assets/embedded.so.cache
--rwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)    14736 2023-04-07 20:12:33.000000 python-sotools-0.1.2/tests/assets/libmakebelieve.so.0
--rwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)    14736 2023-04-07 20:12:33.000000 python-sotools-0.1.2/tests/assets/libmakebelieve.so.0.0
--rwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)    14736 2023-04-07 20:12:33.000000 python-sotools-0.1.2/tests/assets/libmakebelieve.so.0.0.1
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       36 2023-04-07 20:12:32.000000 python-sotools-0.1.2/tests/assets/make-believe.c
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)    16847 2022-03-08 17:17:01.000000 python-sotools-0.1.2/tests/assets/modern.so.cache
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)    66251 2022-06-02 20:48:51.000000 python-sotools-0.1.2/tests/assets/with_hwcaps.so.cache
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)    10077 2023-04-07 19:26:28.000000 python-sotools-0.1.2/tests/test_dl_cache.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1018 2022-03-08 21:55:56.000000 python-sotools-0.1.2/tests/test_libraries.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     4389 2022-03-08 21:22:29.000000 python-sotools-0.1.2/tests/test_libraries_set.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1749 2023-04-07 21:15:26.000000 python-sotools-0.1.2/tests/test_linker.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1062 2022-06-02 20:48:51.000000 python-sotools-0.1.2/tests/test_tools.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      497 2023-04-07 19:13:50.000000 python-sotools-0.1.2/tox.ini
+drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-10 17:05:57.075430 python-sotools-0.1.3/
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       51 2022-02-24 21:18:50.000000 python-sotools-0.1.3/.coveragerc
+drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-10 17:05:57.065429 python-sotools-0.1.3/.github/
+drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-10 17:05:57.068763 python-sotools-0.1.3/.github/workflows/
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      623 2022-02-24 21:25:31.000000 python-sotools-0.1.3/.github/workflows/coverage.yml
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      603 2022-02-24 21:28:59.000000 python-sotools-0.1.3/.github/workflows/lint.yml
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      647 2022-02-24 22:27:09.000000 python-sotools-0.1.3/.github/workflows/test.yml
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       83 2023-04-10 17:03:30.000000 python-sotools-0.1.3/.gitignore
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      907 2023-04-10 17:04:48.000000 python-sotools-0.1.3/HISTORY
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     2058 2023-04-10 17:05:57.075430 python-sotools-0.1.3/PKG-INFO
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1548 2023-03-06 16:40:47.000000 python-sotools-0.1.3/README.md
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      926 2023-03-06 17:06:41.000000 python-sotools-0.1.3/pyproject.toml
+drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-10 17:05:57.068763 python-sotools-0.1.3/python_sotools.egg-info/
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     2058 2023-04-10 17:05:57.000000 python-sotools-0.1.3/python_sotools.egg-info/PKG-INFO
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1188 2023-04-10 17:05:57.000000 python-sotools-0.1.3/python_sotools.egg-info/SOURCES.txt
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)        1 2023-04-10 17:05:57.000000 python-sotools-0.1.3/python_sotools.egg-info/dependency_links.txt
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       91 2023-04-10 17:05:57.000000 python-sotools-0.1.3/python_sotools.egg-info/entry_points.txt
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       11 2023-04-10 17:05:57.000000 python-sotools-0.1.3/python_sotools.egg-info/requires.txt
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)        8 2023-04-10 17:05:57.000000 python-sotools-0.1.3/python_sotools.egg-info/top_level.txt
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       38 2023-04-10 17:05:57.075430 python-sotools-0.1.3/setup.cfg
+drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-10 17:05:57.072096 python-sotools-0.1.3/sotools/
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     2286 2023-03-06 16:46:09.000000 python-sotools-0.1.3/sotools/__init__.py
+drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-10 17:05:57.072096 python-sotools-0.1.3/sotools/dl_cache/
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     6434 2022-06-02 20:48:51.000000 python-sotools-0.1.3/sotools/dl_cache/__init__.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     2338 2022-06-02 20:48:51.000000 python-sotools-0.1.3/sotools/dl_cache/dl_cache.py
+drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-10 17:05:57.072096 python-sotools-0.1.3/sotools/dl_cache/extensions/
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1003 2022-06-02 20:48:51.000000 python-sotools-0.1.3/sotools/dl_cache/extensions/__init__.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      718 2022-06-02 20:48:51.000000 python-sotools-0.1.3/sotools/dl_cache/extensions/generator.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1922 2022-06-02 20:48:51.000000 python-sotools-0.1.3/sotools/dl_cache/extensions/hwcaps.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     3466 2022-06-02 20:48:51.000000 python-sotools-0.1.3/sotools/dl_cache/flags.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     3376 2022-06-02 20:48:51.000000 python-sotools-0.1.3/sotools/dl_cache/structure.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      455 2023-03-06 16:40:47.000000 python-sotools-0.1.3/sotools/ldd.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)    11541 2023-03-06 16:54:57.000000 python-sotools-0.1.3/sotools/libraryset.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     3897 2023-04-10 16:56:21.000000 python-sotools-0.1.3/sotools/linker.py
+drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-10 17:05:57.072096 python-sotools-0.1.3/sotools/scripts/
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)        0 2023-03-06 16:40:47.000000 python-sotools-0.1.3/sotools/scripts/__init__.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1664 2023-03-06 16:40:47.000000 python-sotools-0.1.3/sotools/scripts/ldconfig.py
+-rwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)     1194 2023-03-06 16:40:47.000000 python-sotools-0.1.3/sotools/scripts/ldd.py
+-rwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)     1074 2023-03-06 16:40:47.000000 python-sotools-0.1.3/sotools/scripts/sowhich.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      124 2022-01-31 23:30:48.000000 python-sotools-0.1.3/sotools/util.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      160 2023-04-10 17:05:56.000000 python-sotools-0.1.3/sotools/version.py
+drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-10 17:05:57.075430 python-sotools-0.1.3/tests/
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       68 2023-04-07 20:45:59.000000 python-sotools-0.1.3/tests/__init__.py
+drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-10 17:05:57.075430 python-sotools-0.1.3/tests/assets/
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)    11236 2022-03-08 17:17:01.000000 python-sotools-0.1.3/tests/assets/embedded.so.cache
+-rwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)    14736 2023-04-07 20:12:33.000000 python-sotools-0.1.3/tests/assets/libmakebelieve.so.0
+-rwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)    14736 2023-04-07 20:12:33.000000 python-sotools-0.1.3/tests/assets/libmakebelieve.so.0.0
+-rwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)    14736 2023-04-07 20:12:33.000000 python-sotools-0.1.3/tests/assets/libmakebelieve.so.0.0.1
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       36 2023-04-07 20:12:32.000000 python-sotools-0.1.3/tests/assets/make-believe.c
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)    16847 2022-03-08 17:17:01.000000 python-sotools-0.1.3/tests/assets/modern.so.cache
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)    66251 2022-06-02 20:48:51.000000 python-sotools-0.1.3/tests/assets/with_hwcaps.so.cache
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)    10077 2023-04-07 19:26:28.000000 python-sotools-0.1.3/tests/test_dl_cache.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1018 2022-03-08 21:55:56.000000 python-sotools-0.1.3/tests/test_libraries.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     4389 2022-03-08 21:22:29.000000 python-sotools-0.1.3/tests/test_libraries_set.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1749 2023-04-07 21:15:26.000000 python-sotools-0.1.3/tests/test_linker.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1062 2022-06-02 20:48:51.000000 python-sotools-0.1.3/tests/test_tools.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      497 2023-04-07 19:13:50.000000 python-sotools-0.1.3/tox.ini
```

### Comparing `python-sotools-0.1.2/.github/workflows/coverage.yml` & `python-sotools-0.1.3/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/.github/workflows/lint.yml` & `python-sotools-0.1.3/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/.github/workflows/test.yml` & `python-sotools-0.1.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/HISTORY` & `python-sotools-0.1.3/HISTORY`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+0.1.4
+
+0.1.3 (10-04-2023)
+------------------
+
+- Fix resolving using LD_LIBRARY_PATH working for first invokation only
+
 0.1.2 (07-04-2023)
 ------------------
 
 - Added conditional flag on linker.resolve to choose for paths to be resolved
 
 
 0.1.1 (06-03-2023)
```

### Comparing `python-sotools-0.1.2/PKG-INFO` & `python-sotools-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sotools
-Version: 0.1.2
+Version: 0.1.3
 Summary: Collection of dynamic linking tools
 Author-email: Jean-Baptiste Skutnik <jb.skutnik@gmail.com>
 License: BSD-3-Clause
 Keywords: elf,linking,linux,libraries,system
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `python-sotools-0.1.2/README.md` & `python-sotools-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/pyproject.toml` & `python-sotools-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/python_sotools.egg-info/PKG-INFO` & `python-sotools-0.1.3/python_sotools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sotools
-Version: 0.1.2
+Version: 0.1.3
 Summary: Collection of dynamic linking tools
 Author-email: Jean-Baptiste Skutnik <jb.skutnik@gmail.com>
 License: BSD-3-Clause
 Keywords: elf,linking,linux,libraries,system
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `python-sotools-0.1.2/python_sotools.egg-info/SOURCES.txt` & `python-sotools-0.1.3/python_sotools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/sotools/__init__.py` & `python-sotools-0.1.3/sotools/__init__.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/sotools/dl_cache/__init__.py` & `python-sotools-0.1.3/sotools/dl_cache/__init__.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/sotools/dl_cache/dl_cache.py` & `python-sotools-0.1.3/sotools/dl_cache/dl_cache.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/sotools/dl_cache/extensions/__init__.py` & `python-sotools-0.1.3/sotools/dl_cache/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/sotools/dl_cache/extensions/generator.py` & `python-sotools-0.1.3/sotools/dl_cache/extensions/generator.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/sotools/dl_cache/extensions/hwcaps.py` & `python-sotools-0.1.3/sotools/dl_cache/extensions/hwcaps.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/sotools/dl_cache/flags.py` & `python-sotools-0.1.3/sotools/dl_cache/flags.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/sotools/dl_cache/structure.py` & `python-sotools-0.1.3/sotools/dl_cache/structure.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/sotools/libraryset.py` & `python-sotools-0.1.3/sotools/libraryset.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/sotools/linker.py` & `python-sotools-0.1.3/sotools/linker.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,18 +24,19 @@
 
 @lru_cache()
 def _linker_path() -> Tuple[List[str], List[str]]:
     """
     Return linker search paths, in order
     Sourced from `man ld.so`
     """
-    ld_library_path = filter(
-        None,
-        os.environ.get('LD_LIBRARY_PATH', "").split(':'),
-    )
+    ld_library_path = list(
+        filter(
+            None,
+            os.environ.get('LD_LIBRARY_PATH', "").split(':'),
+        ))
 
     return (ld_library_path, DEFAULT_PATHS)
 
 
 def _valid(path: Path) -> bool:
     """Check a path is an existing directory"""
     return path.is_dir()
```

### Comparing `python-sotools-0.1.2/sotools/scripts/ldconfig.py` & `python-sotools-0.1.3/sotools/scripts/ldconfig.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/sotools/scripts/ldd.py` & `python-sotools-0.1.3/sotools/scripts/ldd.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/sotools/scripts/sowhich.py` & `python-sotools-0.1.3/sotools/scripts/sowhich.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/tests/assets/embedded.so.cache` & `python-sotools-0.1.3/tests/assets/embedded.so.cache`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/tests/assets/libmakebelieve.so.0` & `python-sotools-0.1.3/tests/assets/libmakebelieve.so.0`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/tests/assets/libmakebelieve.so.0.0` & `python-sotools-0.1.3/tests/assets/libmakebelieve.so.0.0`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/tests/assets/libmakebelieve.so.0.0.1` & `python-sotools-0.1.3/tests/assets/libmakebelieve.so.0.0.1`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/tests/assets/modern.so.cache` & `python-sotools-0.1.3/tests/assets/modern.so.cache`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/tests/assets/with_hwcaps.so.cache` & `python-sotools-0.1.3/tests/assets/with_hwcaps.so.cache`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/tests/test_dl_cache.py` & `python-sotools-0.1.3/tests/test_dl_cache.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/tests/test_libraries.py` & `python-sotools-0.1.3/tests/test_libraries.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/tests/test_libraries_set.py` & `python-sotools-0.1.3/tests/test_libraries_set.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/tests/test_linker.py` & `python-sotools-0.1.3/tests/test_linker.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.2/tests/test_tools.py` & `python-sotools-0.1.3/tests/test_tools.py`

 * *Files identical despite different names*

