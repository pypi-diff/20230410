# Comparing `tmp/coreframe-0.0.1.tar.gz` & `tmp/coreframe-0.1a.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coreframe-0.0.1.tar", last modified: Mon Apr 10 01:50:27 2023, max compression
+gzip compressed data, was "dist/coreframe-0.1a.tar", last modified: Mon Jun 29 22:19:17 2020, max compression
```

## Comparing `coreframe-0.0.1.tar` & `coreframe-0.1a.tar`

### file list

```diff
@@ -1,20 +1,4 @@
-drwxrwxrwx   0 azamat    (1000) azamat    (1000)        0 2023-04-10 01:50:27.197054 coreframe-0.0.1/
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)     1088 2023-04-10 01:42:21.000000 coreframe-0.0.1/LICENSE
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)      668 2023-04-10 01:50:27.195056 coreframe-0.0.1/PKG-INFO
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)       88 2023-02-27 05:49:39.000000 coreframe-0.0.1/README.md
-drwxrwxrwx   0 azamat    (1000) azamat    (1000)        0 2023-04-10 01:50:27.142052 coreframe-0.0.1/coreframe/
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)       96 2023-03-29 04:52:49.000000 coreframe-0.0.1/coreframe/__init__.py
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)    17665 2023-04-07 07:13:09.000000 coreframe-0.0.1/coreframe/coreframe.py
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)      690 2023-02-27 05:27:46.000000 coreframe-0.0.1/coreframe/from_csv.py
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)     1317 2023-03-29 05:02:19.000000 coreframe-0.0.1/coreframe/from_nc.py
-drwxrwxrwx   0 azamat    (1000) azamat    (1000)        0 2023-04-10 01:50:27.187057 coreframe-0.0.1/coreframe.egg-info/
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)      668 2023-04-10 01:50:27.000000 coreframe-0.0.1/coreframe.egg-info/PKG-INFO
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)      317 2023-04-10 01:50:27.000000 coreframe-0.0.1/coreframe.egg-info/SOURCES.txt
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)        1 2023-04-10 01:50:27.000000 coreframe-0.0.1/coreframe.egg-info/dependency_links.txt
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)       18 2023-04-10 01:50:27.000000 coreframe-0.0.1/coreframe.egg-info/requires.txt
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)       10 2023-04-10 01:50:27.000000 coreframe-0.0.1/coreframe.egg-info/top_level.txt
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)       82 2023-02-03 14:00:45.000000 coreframe-0.0.1/pyproject.toml
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)       38 2023-04-10 01:50:27.198053 coreframe-0.0.1/setup.cfg
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)      976 2023-04-10 01:49:50.000000 coreframe-0.0.1/setup.py
-drwxrwxrwx   0 azamat    (1000) azamat    (1000)        0 2023-04-10 01:50:27.191054 coreframe-0.0.1/tests/
--rwxrwxrwx   0 azamat    (1000) azamat    (1000)    12052 2023-03-01 08:53:31.000000 coreframe-0.0.1/tests/test_coreframe.py
+drwxr-xr-x   0 hjkim     (2122) hydrolab  (1000)        0 2020-06-29 22:19:17.000000 coreframe-0.1a/
+-rw-r--r--   0 hjkim     (2122) hydrolab  (1000)      479 2020-06-29 22:19:17.000000 coreframe-0.1a/PKG-INFO
+-rw-r--r--   0 hjkim     (2122) hydrolab  (1000)      959 2015-07-12 00:38:03.000000 coreframe-0.1a/__init__.py
+-rwxr-xr-x   0 hjkim     (2122) hydrolab  (1000)      964 2020-06-29 22:19:01.000000 coreframe-0.1a/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

