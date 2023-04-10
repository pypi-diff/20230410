# Comparing `tmp/linesieve-1.0a9.tar.gz` & `tmp/linesieve-1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linesieve-1.0a9.tar", last modified: Sun Apr  3 11:52:41 2022, max compression
+gzip compressed data, was "linesieve-1.0b1.tar", last modified: Mon Apr 10 15:49:57 2023, max compression
```

## Comparing `linesieve-1.0a9.tar` & `linesieve-1.0b1.tar`

### file list

```diff
@@ -1,77 +1,121 @@
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2022-04-03 11:52:41.510002 linesieve-1.0a9/
--rw-r--r--   0 lemon      (501) staff       (20)     1475 2022-01-09 19:58:47.000000 linesieve-1.0a9/LICENSE
--rw-r--r--   0 lemon      (501) staff       (20)       67 2022-01-09 21:07:30.000000 linesieve-1.0a9/MANIFEST.in
--rw-r--r--   0 lemon      (501) staff       (20)     6040 2022-04-03 11:52:41.510372 linesieve-1.0a9/PKG-INFO
--rw-r--r--   0 lemon      (501) staff       (20)     4802 2022-04-03 11:48:57.000000 linesieve-1.0a9/README.md
--rw-r--r--   0 lemon      (501) staff       (20)       90 2022-01-09 20:00:51.000000 linesieve-1.0a9/pyproject.toml
--rw-r--r--   0 lemon      (501) staff       (20)     1591 2022-04-03 11:52:41.512414 linesieve-1.0a9/setup.cfg
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2022-04-03 11:52:41.482058 linesieve-1.0a9/src/
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2022-04-03 11:52:41.485849 linesieve-1.0a9/src/linesieve/
--rw-r--r--   0 lemon      (501) staff       (20)      622 2022-04-03 11:50:44.000000 linesieve-1.0a9/src/linesieve/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)       72 2022-01-11 21:44:18.000000 linesieve-1.0a9/src/linesieve/__main__.py
--rw-r--r--   0 lemon      (501) staff       (20)    24284 2022-04-03 11:49:31.000000 linesieve-1.0a9/src/linesieve/cli.py
--rw-r--r--   0 lemon      (501) staff       (20)     7116 2022-04-02 11:27:30.000000 linesieve-1.0a9/src/linesieve/parsing.py
--rw-r--r--   0 lemon      (501) staff       (20)     2822 2022-01-13 22:48:38.000000 linesieve-1.0a9/src/linesieve/paths.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2022-04-03 11:52:41.487920 linesieve-1.0a9/src/linesieve.egg-info/
--rw-r--r--   0 lemon      (501) staff       (20)     6040 2022-04-03 11:52:40.000000 linesieve-1.0a9/src/linesieve.egg-info/PKG-INFO
--rw-r--r--   0 lemon      (501) staff       (20)     1969 2022-04-03 11:52:41.000000 linesieve-1.0a9/src/linesieve.egg-info/SOURCES.txt
--rw-r--r--   0 lemon      (501) staff       (20)        1 2022-04-03 11:52:40.000000 linesieve-1.0a9/src/linesieve.egg-info/dependency_links.txt
--rw-r--r--   0 lemon      (501) staff       (20)       48 2022-04-03 11:52:41.000000 linesieve-1.0a9/src/linesieve.egg-info/entry_points.txt
--rw-r--r--   0 lemon      (501) staff       (20)       83 2022-04-03 11:52:41.000000 linesieve-1.0a9/src/linesieve.egg-info/requires.txt
--rw-r--r--   0 lemon      (501) staff       (20)       10 2022-04-03 11:52:41.000000 linesieve-1.0a9/src/linesieve.egg-info/top_level.txt
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2022-04-03 11:52:41.488564 linesieve-1.0a9/tests/
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2022-04-03 11:52:41.509487 linesieve-1.0a9/tests/data/
--rw-r--r--   0 lemon      (501) staff       (20)      180 2022-02-08 11:00:54.000000 linesieve-1.0a9/tests/data/full.in
--rw-r--r--   0 lemon      (501) staff       (20)       38 2022-01-03 23:32:14.000000 linesieve-1.0a9/tests/data/full.out
--rw-r--r--   0 lemon      (501) staff       (20)      161 2022-02-07 20:40:20.000000 linesieve-1.0a9/tests/data/head.in
--rw-r--r--   0 lemon      (501) staff       (20)       34 2022-02-01 21:43:16.000000 linesieve-1.0a9/tests/data/head.out
--rw-r--r--   0 lemon      (501) staff       (20)       58 2022-04-02 11:38:11.000000 linesieve-1.0a9/tests/data/iter-line-filter.in
--rw-r--r--   0 lemon      (501) staff       (20)        8 2022-04-02 11:24:05.000000 linesieve-1.0a9/tests/data/iter-line-filter.out
--rw-r--r--   0 lemon      (501) staff       (20)       23 2022-02-07 20:39:24.000000 linesieve-1.0a9/tests/data/marker-failure-only-not-found.in
--rw-r--r--   0 lemon      (501) staff       (20)       29 2022-01-09 16:03:21.000000 linesieve-1.0a9/tests/data/marker-failure-only-not-found.out
--rw-r--r--   0 lemon      (501) staff       (20)       74 2022-02-07 20:39:21.000000 linesieve-1.0a9/tests/data/marker-failure-only.in
--rw-r--r--   0 lemon      (501) staff       (20)       14 2022-01-09 16:04:44.000000 linesieve-1.0a9/tests/data/marker-failure-only.out
--rw-r--r--   0 lemon      (501) staff       (20)       85 2022-02-07 20:39:15.000000 linesieve-1.0a9/tests/data/marker-failure.in
--rw-r--r--   0 lemon      (501) staff       (20)       14 2022-01-09 15:57:16.000000 linesieve-1.0a9/tests/data/marker-failure.out
--rw-r--r--   0 lemon      (501) staff       (20)       38 2022-02-07 20:39:11.000000 linesieve-1.0a9/tests/data/marker-none.in
--rw-r--r--   0 lemon      (501) staff       (20)       12 2022-01-09 16:07:42.000000 linesieve-1.0a9/tests/data/marker-none.out
--rw-r--r--   0 lemon      (501) staff       (20)       21 2022-02-07 20:39:07.000000 linesieve-1.0a9/tests/data/marker-success-only-not-found.in
--rw-r--r--   0 lemon      (501) staff       (20)       29 2022-01-09 16:02:21.000000 linesieve-1.0a9/tests/data/marker-success-only-not-found.out
--rw-r--r--   0 lemon      (501) staff       (20)       20 2022-02-07 20:39:04.000000 linesieve-1.0a9/tests/data/marker-success-only.in
--rw-r--r--   0 lemon      (501) staff       (20)        3 2022-01-09 16:01:29.000000 linesieve-1.0a9/tests/data/marker-success-only.out
--rw-r--r--   0 lemon      (501) staff       (20)       70 2022-02-07 20:39:01.000000 linesieve-1.0a9/tests/data/marker-success.in
--rw-r--r--   0 lemon      (501) staff       (20)        7 2022-01-09 16:06:40.000000 linesieve-1.0a9/tests/data/marker-success.out
--rw-r--r--   0 lemon      (501) staff       (20)       70 2022-02-07 20:38:57.000000 linesieve-1.0a9/tests/data/marker-unexpected-end-no-section.in
--rw-r--r--   0 lemon      (501) staff       (20)       41 2022-01-09 15:59:34.000000 linesieve-1.0a9/tests/data/marker-unexpected-end-no-section.out
--rw-r--r--   0 lemon      (501) staff       (20)       80 2022-02-07 20:38:52.000000 linesieve-1.0a9/tests/data/marker-unexpected-end.in
--rw-r--r--   0 lemon      (501) staff       (20)       35 2022-01-09 15:55:12.000000 linesieve-1.0a9/tests/data/marker-unexpected-end.out
--rw-r--r--   0 lemon      (501) staff       (20)       31 2022-02-07 20:38:46.000000 linesieve-1.0a9/tests/data/match-invert.in
--rw-r--r--   0 lemon      (501) staff       (20)       10 2022-01-09 15:18:57.000000 linesieve-1.0a9/tests/data/match-invert.out
--rw-r--r--   0 lemon      (501) staff       (20)       50 2022-02-07 20:38:42.000000 linesieve-1.0a9/tests/data/match-only.in
--rw-r--r--   0 lemon      (501) staff       (20)       12 2022-01-09 15:18:42.000000 linesieve-1.0a9/tests/data/match-only.out
--rw-r--r--   0 lemon      (501) staff       (20)     1215 2022-04-03 10:44:21.000000 linesieve-1.0a9/tests/data/match-span.in
--rw-r--r--   0 lemon      (501) staff       (20)      352 2022-04-03 09:40:21.000000 linesieve-1.0a9/tests/data/match-span.out
--rw-r--r--   0 lemon      (501) staff       (20)       32 2022-02-07 20:38:37.000000 linesieve-1.0a9/tests/data/match.in
--rw-r--r--   0 lemon      (501) staff       (20)        8 2022-01-18 21:41:40.000000 linesieve-1.0a9/tests/data/match.out
--rw-r--r--   0 lemon      (501) staff       (20)      102 2022-02-07 20:40:20.000000 linesieve-1.0a9/tests/data/per-section.in
--rw-r--r--   0 lemon      (501) staff       (20)       29 2022-01-09 15:18:07.000000 linesieve-1.0a9/tests/data/per-section.out
--rw-r--r--   0 lemon      (501) staff       (20)       49 2022-02-07 20:38:17.000000 linesieve-1.0a9/tests/data/show-all-data.in
--rw-r--r--   0 lemon      (501) staff       (20)       22 2022-01-09 15:16:18.000000 linesieve-1.0a9/tests/data/show-all-data.out
--rw-r--r--   0 lemon      (501) staff       (20)       41 2022-02-07 20:38:13.000000 linesieve-1.0a9/tests/data/show-all-empty.in
--rw-r--r--   0 lemon      (501) staff       (20)       14 2022-01-09 15:15:45.000000 linesieve-1.0a9/tests/data/show-all-empty.out
--rw-r--r--   0 lemon      (501) staff       (20)       50 2022-02-07 20:38:10.000000 linesieve-1.0a9/tests/data/show-first-section-only.in
--rw-r--r--   0 lemon      (501) staff       (20)        5 2022-01-14 17:27:09.000000 linesieve-1.0a9/tests/data/show-first-section-only.out
--rw-r--r--   0 lemon      (501) staff       (20)       65 2022-02-07 20:38:07.000000 linesieve-1.0a9/tests/data/show-nothing.in
--rw-r--r--   0 lemon      (501) staff       (20)        4 2022-01-09 15:14:48.000000 linesieve-1.0a9/tests/data/show-nothing.out
--rw-r--r--   0 lemon      (501) staff       (20)       51 2022-02-07 20:38:01.000000 linesieve-1.0a9/tests/data/single.in
--rw-r--r--   0 lemon      (501) staff       (20)       10 2022-01-03 23:31:35.000000 linesieve-1.0a9/tests/data/single.out
--rw-r--r--   0 lemon      (501) staff       (20)      147 2022-02-07 20:40:20.000000 linesieve-1.0a9/tests/data/split-max.in
--rw-r--r--   0 lemon      (501) staff       (20)       39 2022-02-05 09:50:09.000000 linesieve-1.0a9/tests/data/split-max.out
--rw-r--r--   0 lemon      (501) staff       (20)      209 2022-02-07 20:40:20.000000 linesieve-1.0a9/tests/data/split.in
--rw-r--r--   0 lemon      (501) staff       (20)       68 2022-02-04 21:15:05.000000 linesieve-1.0a9/tests/data/split.out
--rw-r--r--   0 lemon      (501) staff       (20)       37 2022-02-07 20:37:13.000000 linesieve-1.0a9/tests/data/sub-to-empty-line.in
--rw-r--r--   0 lemon      (501) staff       (20)        9 2022-01-09 15:13:27.000000 linesieve-1.0a9/tests/data/sub-to-empty-line.out
--rw-r--r--   0 lemon      (501) staff       (20)      161 2022-02-07 20:40:20.000000 linesieve-1.0a9/tests/data/tail.in
--rw-r--r--   0 lemon      (501) staff       (20)       34 2022-02-01 21:42:04.000000 linesieve-1.0a9/tests/data/tail.out
--rw-r--r--   0 lemon      (501) staff       (20)     5982 2022-04-02 11:52:29.000000 linesieve-1.0a9/tests/test_cli.py
--rw-r--r--   0 lemon      (501) staff       (20)     1495 2022-01-12 23:19:46.000000 linesieve-1.0a9/tests/test_paths.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.894449 linesieve-1.0b1/
+-rw-r--r--   0 lemon      (501) staff       (20)     1475 2023-04-10 15:23:48.000000 linesieve-1.0b1/LICENSE
+-rw-r--r--   0 lemon      (501) staff       (20)      172 2023-04-10 15:23:48.000000 linesieve-1.0b1/MANIFEST.in
+-rw-r--r--   0 lemon      (501) staff       (20)    14355 2023-04-10 15:49:57.894786 linesieve-1.0b1/PKG-INFO
+-rw-r--r--   0 lemon      (501) staff       (20)    13050 2023-04-10 15:45:50.000000 linesieve-1.0b1/README.rst
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.748155 linesieve-1.0b1/docs/
+-rw-r--r--   0 lemon      (501) staff       (20)      634 2023-04-10 15:23:48.000000 linesieve-1.0b1/docs/Makefile
+-rw-r--r--   0 lemon      (501) staff       (20)      115 2023-04-10 15:23:48.000000 linesieve-1.0b1/docs/cli.rst
+-rw-r--r--   0 lemon      (501) staff       (20)     1552 2023-04-10 15:23:48.000000 linesieve-1.0b1/docs/conf.py
+-rw-r--r--   0 lemon      (501) staff       (20)      133 2023-04-10 15:23:48.000000 linesieve-1.0b1/docs/examples.rst
+-rw-r--r--   0 lemon      (501) staff       (20)      358 2023-04-10 15:44:42.000000 linesieve-1.0b1/docs/index.rst
+-rw-r--r--   0 lemon      (501) staff       (20)      800 2023-04-10 15:23:48.000000 linesieve-1.0b1/docs/make.bat
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.757811 linesieve-1.0b1/examples/
+-rw-r--r--   0 lemon      (501) staff       (20)      580 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/ant-test-single-compile-error.diff
+-rw-r--r--   0 lemon      (501) staff       (20)      855 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/ant-test-single-compile-error.txt
+-rw-r--r--   0 lemon      (501) staff       (20)      633 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/ant-test-single-failure.diff
+-rw-r--r--   0 lemon      (501) staff       (20)     8340 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/ant-test-single-failure.txt
+-rw-r--r--   0 lemon      (501) staff       (20)     4878 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/ant-test-single-success.txt
+-rwxr-xr-x   0 lemon      (501) staff       (20)     1140 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/ant-wrapper.sh
+-rw-r--r--   0 lemon      (501) staff       (20)      376 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/git-options.sh
+-rw-r--r--   0 lemon      (501) staff       (20)      607 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/java-traceback.sh
+-rw-r--r--   0 lemon      (501) staff       (20)    10527 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/java-traceback.txt
+-rw-r--r--   0 lemon      (501) staff       (20)      163 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/simple.sh
+-rw-r--r--   0 lemon      (501) staff       (20)       46 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/simple.txt
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.734660 linesieve-1.0b1/examples/src/
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.734976 linesieve-1.0b1/examples/src/com/
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.735240 linesieve-1.0b1/examples/src/com/example/
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.735599 linesieve-1.0b1/examples/src/com/example/someproject/
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.758578 linesieve-1.0b1/examples/src/com/example/someproject/somepackage/
+-rw-r--r--   0 lemon      (501) staff       (20)        0 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/src/com/example/someproject/somepackage/ThingDoer.java
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.736292 linesieve-1.0b1/examples/tst/
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.736468 linesieve-1.0b1/examples/tst/com/
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.736636 linesieve-1.0b1/examples/tst/com/example/
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.736829 linesieve-1.0b1/examples/tst/com/example/someproject/
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.759350 linesieve-1.0b1/examples/tst/com/example/someproject/somepackage/
+-rw-r--r--   0 lemon      (501) staff       (20)        0 2023-04-10 15:23:48.000000 linesieve-1.0b1/examples/tst/com/example/someproject/somepackage/ThingDoerTest.java
+-rw-r--r--   0 lemon      (501) staff       (20)       90 2023-04-10 15:23:48.000000 linesieve-1.0b1/pyproject.toml
+-rwxr-xr-x   0 lemon      (501) staff       (20)      544 2023-04-10 15:23:48.000000 linesieve-1.0b1/run.sh
+-rw-r--r--   0 lemon      (501) staff       (20)     1713 2023-04-10 15:49:57.896685 linesieve-1.0b1/setup.cfg
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.737577 linesieve-1.0b1/src/
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.763480 linesieve-1.0b1/src/linesieve/
+-rw-r--r--   0 lemon      (501) staff       (20)      735 2023-04-10 15:48:55.000000 linesieve-1.0b1/src/linesieve/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)       28 2023-04-10 15:23:48.000000 linesieve-1.0b1/src/linesieve/__main__.py
+-rw-r--r--   0 lemon      (501) staff       (20)    28501 2023-04-10 15:43:13.000000 linesieve-1.0b1/src/linesieve/cli.py
+-rw-r--r--   0 lemon      (501) staff       (20)     7116 2023-04-10 15:23:48.000000 linesieve-1.0b1/src/linesieve/parsing.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2820 2023-04-10 15:23:48.000000 linesieve-1.0b1/src/linesieve/paths.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.775789 linesieve-1.0b1/src/linesieve.egg-info/
+-rw-r--r--   0 lemon      (501) staff       (20)    14355 2023-04-10 15:49:57.000000 linesieve-1.0b1/src/linesieve.egg-info/PKG-INFO
+-rw-r--r--   0 lemon      (501) staff       (20)     2791 2023-04-10 15:49:57.000000 linesieve-1.0b1/src/linesieve.egg-info/SOURCES.txt
+-rw-r--r--   0 lemon      (501) staff       (20)        1 2023-04-10 15:49:57.000000 linesieve-1.0b1/src/linesieve.egg-info/dependency_links.txt
+-rw-r--r--   0 lemon      (501) staff       (20)       48 2023-04-10 15:49:57.000000 linesieve-1.0b1/src/linesieve.egg-info/entry_points.txt
+-rw-r--r--   0 lemon      (501) staff       (20)      128 2023-04-10 15:49:57.000000 linesieve-1.0b1/src/linesieve.egg-info/requires.txt
+-rw-r--r--   0 lemon      (501) staff       (20)       10 2023-04-10 15:49:57.000000 linesieve-1.0b1/src/linesieve.egg-info/top_level.txt
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.778272 linesieve-1.0b1/tests/
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-04-10 15:49:57.893871 linesieve-1.0b1/tests/data/
+-rw-r--r--   0 lemon      (501) staff       (20)       20 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/exec.in
+-rw-r--r--   0 lemon      (501) staff       (20)       48 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/exec.out
+-rw-r--r--   0 lemon      (501) staff       (20)      180 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/full.in
+-rw-r--r--   0 lemon      (501) staff       (20)       38 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/full.out
+-rw-r--r--   0 lemon      (501) staff       (20)      161 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/head.in
+-rw-r--r--   0 lemon      (501) staff       (20)       34 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/head.out
+-rw-r--r--   0 lemon      (501) staff       (20)       58 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/iter-line-filter.in
+-rw-r--r--   0 lemon      (501) staff       (20)        8 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/iter-line-filter.out
+-rw-r--r--   0 lemon      (501) staff       (20)       23 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-failure-only-not-found.in
+-rw-r--r--   0 lemon      (501) staff       (20)       40 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-failure-only-not-found.out
+-rw-r--r--   0 lemon      (501) staff       (20)       74 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-failure-only.in
+-rw-r--r--   0 lemon      (501) staff       (20)       14 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-failure-only.out
+-rw-r--r--   0 lemon      (501) staff       (20)       85 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-failure.in
+-rw-r--r--   0 lemon      (501) staff       (20)       14 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-failure.out
+-rw-r--r--   0 lemon      (501) staff       (20)       38 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-none.in
+-rw-r--r--   0 lemon      (501) staff       (20)       12 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-none.out
+-rw-r--r--   0 lemon      (501) staff       (20)       21 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-success-only-not-found.in
+-rw-r--r--   0 lemon      (501) staff       (20)       40 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-success-only-not-found.out
+-rw-r--r--   0 lemon      (501) staff       (20)       20 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-success-only.in
+-rw-r--r--   0 lemon      (501) staff       (20)        3 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-success-only.out
+-rw-r--r--   0 lemon      (501) staff       (20)       70 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-success.in
+-rw-r--r--   0 lemon      (501) staff       (20)        7 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-success.out
+-rw-r--r--   0 lemon      (501) staff       (20)       70 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-unexpected-end-no-section.in
+-rw-r--r--   0 lemon      (501) staff       (20)       52 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-unexpected-end-no-section.out
+-rw-r--r--   0 lemon      (501) staff       (20)       80 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-unexpected-end.in
+-rw-r--r--   0 lemon      (501) staff       (20)       46 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/marker-unexpected-end.out
+-rw-r--r--   0 lemon      (501) staff       (20)       31 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/match-invert.in
+-rw-r--r--   0 lemon      (501) staff       (20)       10 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/match-invert.out
+-rw-r--r--   0 lemon      (501) staff       (20)       50 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/match-only.in
+-rw-r--r--   0 lemon      (501) staff       (20)       12 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/match-only.out
+-rw-r--r--   0 lemon      (501) staff       (20)       32 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/match.in
+-rw-r--r--   0 lemon      (501) staff       (20)        8 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/match.out
+-rw-r--r--   0 lemon      (501) staff       (20)      102 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/per-section.in
+-rw-r--r--   0 lemon      (501) staff       (20)       29 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/per-section.out
+-rw-r--r--   0 lemon      (501) staff       (20)       38 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/pop-all-empty.in
+-rw-r--r--   0 lemon      (501) staff       (20)        4 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/pop-all-empty.out
+-rw-r--r--   0 lemon      (501) staff       (20)      143 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/pop-all.in
+-rw-r--r--   0 lemon      (501) staff       (20)       53 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/pop-all.out
+-rw-r--r--   0 lemon      (501) staff       (20)       32 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/pop-empty.in
+-rw-r--r--   0 lemon      (501) staff       (20)       91 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/pop-empty.out
+-rw-r--r--   0 lemon      (501) staff       (20)      117 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/pop.in
+-rw-r--r--   0 lemon      (501) staff       (20)       36 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/pop.out
+-rw-r--r--   0 lemon      (501) staff       (20)      103 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/push.in
+-rw-r--r--   0 lemon      (501) staff       (20)       30 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/push.out
+-rw-r--r--   0 lemon      (501) staff       (20)       49 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/show-all-data.in
+-rw-r--r--   0 lemon      (501) staff       (20)       22 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/show-all-data.out
+-rw-r--r--   0 lemon      (501) staff       (20)       41 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/show-all-empty.in
+-rw-r--r--   0 lemon      (501) staff       (20)       14 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/show-all-empty.out
+-rw-r--r--   0 lemon      (501) staff       (20)       50 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/show-first-section-only.in
+-rw-r--r--   0 lemon      (501) staff       (20)        5 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/show-first-section-only.out
+-rw-r--r--   0 lemon      (501) staff       (20)       65 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/show-nothing.in
+-rw-r--r--   0 lemon      (501) staff       (20)        4 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/show-nothing.out
+-rw-r--r--   0 lemon      (501) staff       (20)       51 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/single.in
+-rw-r--r--   0 lemon      (501) staff       (20)       10 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/single.out
+-rw-r--r--   0 lemon      (501) staff       (20)     1125 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/span.in
+-rw-r--r--   0 lemon      (501) staff       (20)      352 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/span.out
+-rw-r--r--   0 lemon      (501) staff       (20)      147 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/split-max.in
+-rw-r--r--   0 lemon      (501) staff       (20)       39 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/split-max.out
+-rw-r--r--   0 lemon      (501) staff       (20)      209 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/split.in
+-rw-r--r--   0 lemon      (501) staff       (20)       68 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/split.out
+-rw-r--r--   0 lemon      (501) staff       (20)       37 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/sub-to-empty-line.in
+-rw-r--r--   0 lemon      (501) staff       (20)        9 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/sub-to-empty-line.out
+-rw-r--r--   0 lemon      (501) staff       (20)      161 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/tail.in
+-rw-r--r--   0 lemon      (501) staff       (20)       34 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/data/tail.out
+-rw-r--r--   0 lemon      (501) staff       (20)     5982 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/test_cli.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1495 2023-04-10 15:23:48.000000 linesieve-1.0b1/tests/test_paths.py
```

### Comparing `linesieve-1.0a9/LICENSE` & `linesieve-1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `linesieve-1.0a9/setup.cfg` & `linesieve-1.0b1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [metadata]
 name = linesieve
 version = attr: linesieve.__version__
 author = lemon24
 description = An unholy blend of grep, sed, awk, and Python.
-long_description = file: README.md
-long_description_content_type = text/markdown
+long_description = file: README.rst
+long_description_content_type = text/x-rst
 url = https://github.com/lemon24/linesieve
 license = BSD-3-Clause
 project_urls = 
-	Code = https://github.com/lemon24/linesieve
-	Issue tracker = https://github.com/lemon24/linesieve/issues
+	Documentation = https://linesieve.readthedocs.io/
+	Issue Tracker = https://github.com/lemon24/linesieve/issues
+	Source Code = https://github.com/lemon24/linesieve
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Console
 	Intended Audience :: Developers
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
@@ -36,25 +37,30 @@
 	click >= 8
 	braceexpand >= 0.1
 
 [options.extras_require]
 tests = 
 	pytest
 	pytest-cov
+docs = 
+	sphinx
+	sphinx-rtd-theme
+	sphinx-click
 dev = 
 	pre-commit
 	build
 	twine
 
 [options.entry_points]
 console_scripts = 
 	linesieve = linesieve.cli:cli
 
 [tool:pytest]
 addopts = --doctest-modules
+testpaths = tests
 
 [coverage:run]
 branch = true
 source = 
 	linesieve
 	tests
```

### Comparing `linesieve-1.0a9/src/linesieve/__init__.py` & `linesieve-1.0b1/src/linesieve/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 """
+An unholy blend of grep, sed, awk, and Python.
+
 Read standard input, process it, and write to standard output.
 
 Split input into sections, and output selected sections.
 Filter output lines, globally or per-section.
 Compress runs of blank lines.
 
 All patterns use the Python regular expression syntax.
 
 Example:
 
 \b
-  $ cat file.txt
-  0
-  one:
-  1...
-  two:
-  2 (two)
-  three:
-  3, three
-  fail
+    $ cat simple.txt
+    0
+    one:
+    1...
+    two:
+    2 (two)
+    three:
+    3, three
+    fail
 
 \b
-  $ cat file.txt | linesieve --section '(\\S+):$' --failure fail \\
-  > show --ignore-case ^O \\
-  > match --section one --only-matching '\\d+' \\
-  > sub '([a-z])' '\\1\\1\\1'
-  d\bone
-  1
-  d\b..
-  d\bthree
-  3, ttthhhrrreeeeee
-  r\bfail
+    $ cat simple.txt \\
+    | linesieve --section '(\\S+):$' --failure fail \\
+      show --ignore-case ^O \\
+      match --section one --only-matching '\\d+' \\
+      sub '([a-z])' '\\1\\1\\1'
+    one  # dim
+    1
+    ..  # dim
+    three  # dim
+    3, ttthhhrrreeeeee
+    fail  # red
 
 """
 
-__version__ = '1.0a9'
+__version__ = '1.0b1'
```

### Comparing `linesieve-1.0a9/src/linesieve/cli.py` & `linesieve-1.0b1/src/linesieve/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,119 +1,62 @@
 import os.path
 import re
 import subprocess
+from contextlib import contextmanager
 from functools import wraps
 
 import click
+from click import BadParameter
 from click import echo
 from click import style
+from click import UsageError
 
 import linesieve
 from .parsing import make_pipeline
 
 
 # references for common command-line option names:
 # https://www.gnu.org/prep/standards/html_node/Option-Table.html
 # http://www.catb.org/~esr/writings/taoup/html/ch10s05.html
 # all the git options, generated with the script in the README
 
 
-def color_help(text):
-
-    KWARGS = {
-        'd': dict(dim=True),
-        'r': dict(fg='red'),
-        'g': dict(fg='green'),
-        'y': dict(fg='yellow'),
-    }
-
-    def repl(match):
-        options, line = match.groups()
-        kwargs = {}
-        for option in options:
-            if option == '\b':
-                continue
-            kwargs.update(KWARGS[option])
-        return style(line, **kwargs)
-
-    return re.sub('([drgy]\b)(.*)', repl, text)
-
-
-def help_all_option():
-    return click.option(
-        "--help-all",
-        is_flag=True,
-        expose_value=False,
-        is_eager=True,
-        help="Show help for all commands and exit.",
-        callback=help_all_callback,
-    )
-
-
-def help_all_callback(ctx, param, value):
-    if not value or ctx.resilient_parsing:
-        return
-
-    formatter = ctx.make_formatter()
-    formatter.indent_increment
-    commands = list_commands_recursive(ctx.command, ctx)
+FURTHER_HELP = """\
+\b
+linesieve help --all
+linesieve COMMAND --help
+https://github.com/lemon24/linesieve
+"""
+
+
+class CLIGroup(click.Group):
+    def format_options(self, ctx, formatter):
+        super().format_options(ctx, formatter)
+        with formatter.section('Further help'):
+            formatter.write_text(FURTHER_HELP)
 
-    for path, command in commands:
-        title = style(path.upper(), bold=True)
-        if command.short_help:
-            short = command.short_help
-            first = short.partition(' ')[0]
-            if first.istitle():
-                short = first.lower() + short[len(first) :]
-            short = short.rstrip('.')
-            title += style(' - ' + short, dim=True)
-
-        formatter.write(title + '\n\n  ')
-
-        with formatter.indentation():
-            if command is ctx.command:
-                format_ctx = ctx
-            else:
-                format_ctx = type(ctx)(command, ctx, command.name)
-            command.format_help(format_ctx, formatter)
-
-        formatter.write('\n')
-
-    click.echo_via_pager(formatter.getvalue(), color=ctx.color)
-    ctx.exit()
-
-
-def list_commands_recursive(self, ctx, path=()):
-    path = path + (self.name,)
-    yield ' '.join(path), self
-    if not hasattr(self, 'list_commands'):
-        return
-    for subcommand in self.list_commands(ctx):
-        cmd = self.get_command(ctx, subcommand)
-        if cmd is None:
-            continue
-        if cmd.hidden:
-            continue
-        yield from list_commands_recursive(cmd, ctx, path)
+    def list_commands(self, ctx):
+        return self.commands
 
 
 @click.group(
     name='linesieve',
     chain=True,
+    cls=CLIGroup,
     invoke_without_command=True,
-    help=color_help(linesieve.__doc__),
-    short_help="An unholy blend of grep, sed, awk, and Python.",
+    no_args_is_help=True,
+    subcommand_metavar='[COMMAND [ARGS]...]... ',
 )
 @click.option(
     '-s',
     '--section',
     metavar='PATTERN',
     help="""
     Consider matching lines the start of a new section.
-    The section name is one of: the named group 'name',
+    The section name is one of: the named group `name`,
     the first captured group, the entire match.
     """,
 )
 @click.option(
     '--success',
     metavar='PATTERN',
     help="If matched, exit with a status code indicating success.",
@@ -122,31 +65,45 @@
     '--failure',
     metavar='PATTERN',
     help="""
     If matched, exit with a status code indicating failure.
     Before exiting, output the last section if it wasn't already.
     """,
 )
-@help_all_option()
+@click.version_option(linesieve.__version__, message='%(prog)s %(version)s')
 @click.pass_context
 def cli(ctx, **kwargs):
+    """An unholy blend of grep, sed, awk, and Python."""
     # options reserved for future expansion:
     # -s --section --section-start
     # -e --section-end
     # -n --section-name # same as annotate_lines() marker
     ctx.obj = {}
 
 
 @cli.result_callback()
 @click.pass_context
 def process_pipeline(ctx, processors, section, success, failure):
+    if section is not None:
+        with handle_re_error('--section'):
+            section = re.compile(section)
+    if success is not None:
+        with handle_re_error('--success'):
+            success = re.compile(success)
+    if failure is not None:
+        with handle_re_error('--failure'):
+            failure = re.compile(failure)
+
     file = ctx.obj.get('file')
     if not file:
         file = click.get_text_stream('stdin')
 
+    if file.isatty():
+        echo(style("linesieve: reading from terminal", dim=True), err=True)
+
     process = ctx.obj.get('process')
     show = ctx.obj.get('show')
 
     processors = [p for p in processors if p]
 
     status, label = output_sections(
         make_pipeline(file, section, success, failure, show, processors)
@@ -168,66 +125,50 @@
         # failure only          -> end is success (unless returncode says failure)
         # success only          -> end is failure (unless returncode says success)
         # success and failure   -> end is unexpected
 
         label = label or '<no-section>'
         if success is not None and failure is not None:
             message = style(
-                f"unexpected end during {style(label, bold=True)}", fg='red'
+                f"linesieve: unexpected end during {style(label, bold=True)}", fg='red'
             )
             returncode = 1
 
     if message:
         echo(message, err=status not in {True, False})
 
     if process:
         process.wait()
         returncode = process.returncode
         if not message:
             message = style(
-                f"exited with status code {style(str(returncode), bold=True)}",
+                f"linesieve: {process.args[0]} exited with status code "
+                f"{style(str(returncode), bold=True)}",
                 fg=('green' if returncode == 0 else 'red'),
             )
         else:
             message = None
 
     else:
         if not message:
             assert success is None or failure is None, (success, failure)
             if success is not None:
-                message = style("success marker not found", fg='red')
+                message = style("linesieve: success marker not found", fg='red')
                 returncode = 1
             if failure is not None:
-                message = style("failure marker not found", fg='green')
+                message = style("linesieve: failure marker not found", fg='green')
                 returncode = 0
         else:
             message = None
 
     if message:
         echo(message, err=True)
 
     ctx.exit(returncode)
 
-    # TODO before 1.0:
-    # pattern compilation error messages
-    # push --section pattern ... pop
-    # bugbear?
-    # TODO after 1.0:
-    # hide section
-    # match -e pattern -e pattern (hard to do with click while keeping arg)
-    # match-span -s ... -s ..s
-    # print last section without --failure if exec exits with non-zero (how?)
-    # exec time
-    # collapse any repeated lines
-    # runfilter "grep pattern"
-    # short command aliases (four-letter ones)
-    # make dedupe_blank_lines optional
-    # match replace spans of skipped lines with ... (match span already does this)
-    # section -s pattern section --include pattern (tried it, not necessarily better)
-
 
 def output_sections(groups, section_dot='.'):
     """Print (section, lines) pairs in a fancy way.
 
     >>> groups = [('', 'ab'), ('', ''), ('', ''), ('one', 'c'), ('', ''), (True, 'xyz')]
     >>> output_sections(groups)  # doctest: +SKIP
     a
@@ -239,15 +180,14 @@
     (True, 'x')
 
     """
     prev_section = None
     last_was_dot = False
 
     for section, lines in groups:
-
         if section == '' and prev_section is not None:
             echo(style(section_dot, dim=True), err=True, nl=False)
             last_was_dot = True
         elif last_was_dot:
             echo(err=True)
             last_was_dot = False
 
@@ -269,24 +209,37 @@
 
         for line in lines:
             echo(line)
 
         prev_section = section
 
 
+@contextmanager
+def handle_re_error(param_hint):
+    if isinstance(param_hint, str):
+        param_hint = [param_hint]
+    try:
+        yield
+    except re.error as e:
+        raise BadParameter(f"{e}: {e.pattern!r}", param_hint=param_hint)
+
+
+# INPUT
+
+
 @cli.command(short_help="Read input from file.")
 @click.argument('file', type=click.File('r', lazy=True))
 @click.pass_obj
 def open(obj, file):
     """Read input from FILE instead of standard input.
 
     Roughly equivalent to: cat FILE | linesieve
 
     """
-    assert not obj.get('file')
+    assert not obj.get('file'), "should not be possible for open to follow exec"
     obj['file'] = file
 
 
 @cli.command(short_help="Read input from command.")
 @click.argument('command')
 @click.argument('argument', nargs=-1)
 @click.pass_obj
@@ -294,21 +247,25 @@
     """Execute COMMAND and use its output as input.
 
     Roughly equivalent to: COMMAND | linesieve
 
     If the command finishes, exit with its status code.
 
     """
-    assert not obj.get('file')
-    process = subprocess.Popen(
-        (command,) + argument,
-        text=True,
-        stdout=subprocess.PIPE,
-        stderr=subprocess.STDOUT,
-    )
+    if obj.get('file'):
+        raise UsageError("exec and open are mutually exclusive")
+    try:
+        process = subprocess.Popen(
+            (command,) + argument,
+            text=True,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.STDOUT,
+        )
+    except OSError as e:
+        raise BadParameter(e, param_hint='COMMAND')
     obj['process'] = process
     obj['file'] = process.stdout
 
 
 PATTERN_OPTIONS = [
     click.option(
         '-F',
@@ -335,20 +292,17 @@
 
 
 def pattern_argument(fn):
     @click.argument('pattern')
     @pattern_options
     @wraps(fn)
     def wrapper(*args, pattern, fixed_strings, ignore_case, verbose, **kwargs):
-        return fn(
-            *args,
-            pattern=compile_pattern(pattern, fixed_strings, ignore_case, verbose),
-            fixed_strings=fixed_strings,
-            **kwargs,
-        )
+        with handle_re_error('PATTERN'):
+            pattern_re = compile_pattern(pattern, fixed_strings, ignore_case, verbose)
+        return fn(*args, pattern=pattern_re, fixed_strings=fixed_strings, **kwargs)
 
     return wrapper
 
 
 def compile_pattern(pattern, fixed_strings, ignore_case, verbose):
     if fixed_strings:
         pattern = re.escape(pattern)
@@ -358,68 +312,250 @@
         flags |= re.IGNORECASE
     if verbose:
         flags |= re.VERBOSE
 
     return re.compile(pattern, flags)
 
 
+# SECTION CONTROL
+
+
 @cli.command(short_help="Show selected sections.")
 @pattern_argument
 @click.pass_obj
 def show(obj, pattern, fixed_strings):
     """Output only sections matching PATTERN.
 
-    '^$' matches the lines before the first section.
-    '$none' matches no section.
+    `^$` matches the lines before the first section.
+    `$none` matches no section.
 
     """
     obj.setdefault('show', []).append(pattern)
 
 
+@cli.command(short_help="Push patterns onto the section stack.")
+@pattern_argument
+@click.pass_obj
+def push(obj, pattern, fixed_strings):
+    """Push a pattern onto the section stack.
+
+    When there are patterns on the section stack,
+    filters apply only to the sections that match
+    any of the patterns in the stack.
+
+    `filter --section PATTERN` is equivalent to
+    `push PATTERN filter pop`.
+
+    """
+    stack = obj.setdefault('section_stack', [])
+    stack.append(pattern)
+
+
+@cli.command(short_help="Pop patterns off the section stack.")
+@click.option(
+    '-a', '--all', is_flag=True, help="Remove all the patterns from the stack."
+)
+@click.pass_obj
+def pop(obj, all):
+    """Pop patterns off the section stack. See 'push' for details.
+
+    With no arguments, removes the top pattern from the stack.
+
+    """
+    stack = obj.setdefault('section_stack', [])
+    if not all:
+        if not stack:
+            raise UsageError('nothing to pop')
+        stack.pop()
+    else:
+        stack.clear()
+
+
 def section_option(fn):
     @click.option(
-        '-s', '--section', metavar='PATTERN', help="Apply only to matching sections."
+        '-s',
+        '--section',
+        metavar='PATTERN',
+        help="""
+        Apply only to matching sections.
+        If there are patterns on the section stack,
+        push the pattern (that is, apply *also* to matching sections).
+        """,
     )
     @wraps(fn)
     def wrapper(*args, section, **kwargs):
         rv = fn(*args, **kwargs)
         if rv is None:
             return None
-        section_re = re.compile(section) if section is not None else None
-        return section_re, rv
+
+        ctx = click.get_current_context()
+        section_res = list(ctx.obj.setdefault('section_stack', []))
+        if section is not None:
+            with handle_re_error('--section'):
+                section_res.append(re.compile(section))
+
+        return section_res, rv
 
     return wrapper
 
 
-@cli.command(short_help="Replace pattern.")
-@pattern_argument
-@click.argument('repl')
-@click.option('-o', '--only-matching', is_flag=True, help="Output only matching lines.")
-@click.option('--color', is_flag=True, help="Color replacements.")
+# LINE RANGES
+
+
+@cli.command(short_help="Output the first part of sections.")
+@click.option(
+    '-n',
+    'count',
+    metavar="COUNT",
+    type=int,
+    default=10,
+    show_default=True,
+    help="Print the first COUNT lines. "
+    "With a leading `-`, print all but the last COUNT lines.",
+)
 @section_option
-def sub(pattern, repl, fixed_strings, only_matching, color):
-    """Replace PATTERN matches with REPL.
+def head(count):
+    """Print the first COUNT lines.
 
-    Roughly equivalent to: sed 's/PATTERN/REPL/g'
+    Roughly equivalent to: head -n COUNT
 
-    Works like re.sub() in Python.
+    """
+    from itertools import islice
+
+    def head(lines):
+        if count >= 0:
+            return islice(lines, count)
+        else:
+            # TODO: don't read in memory, use a temporary file
+            return iter(list(lines)[0:count])
+
+    head.is_iter = True
+    return head
+
+
+def tail_count_int(value):
+    value = value.strip()
+    if value.startswith('+'):
+        rv = int(value) - 1
+    elif value.startswith('-'):
+        rv = int(value)
+    else:
+        rv = -int(value)
+    return rv
+
+
+@cli.command(short_help="Output the last part of sections.")
+@click.option(
+    '-n',
+    'count',
+    metavar="COUNT",
+    type=tail_count_int,
+    default=10,
+    show_default=True,
+    help="Print the last COUNT lines. "
+    "With a leading `+`, print lines starting with line COUNT.",
+)
+@section_option
+def tail(count):
+    """Print the last COUNT lines.
+
+    Roughly equivalent to: tail -n COUNT
 
     """
-    if fixed_strings:
-        repl = repl.replace('\\', r'\\')
-    if color:
-        repl = style(repl, fg='red')
+    from itertools import islice
+    from collections import deque
 
-    def sub(line):
-        line, subn = pattern.subn(repl, line)
-        if only_matching and not subn:
-            return None
-        return line
+    def tail(lines):
+        if count <= 0:
+            # TODO: don't read in memory, use a temporary file
+            return iter(deque(lines, maxlen=-count))
+        else:
+            return islice(lines, count, None)
+
+    tail.is_iter = True
+    return tail
+
+
+@cli.command(short_help="Output matching line spans.")
+@click.option(
+    '--start', '--start-with', metavar='PATTERN', help="Span start (inclusive)."
+)
+@click.option('--end', '--end-before', metavar='PATTERN', help="Span end (exclusive).")
+@pattern_options
+@click.option(
+    '-v',
+    '--invert-match',
+    is_flag=True,
+    help="Output only lines *not* between those matching `--start` and `--end`.",
+)
+@click.option(
+    '--repl',
+    '--replacement',
+    help="""
+    Replace non-matching line spans with TEXT.
+    With `--invert-match`, backreferences to captures in `--start` are expanded;
+    without `--invert-match`, only escapes are expanded.
+    """,
+)
+@section_option
+def span(start, end, fixed_strings, ignore_case, verbose, invert_match, repl):
+    """Output only lines between those matching `--start` and `--end`.
+
+    Roughly equivalent to: grep START -A9999 | grep END -B9999 | head -n-1
+
+    """
+
+    # options reserved for future expansion:
+    # --start-after (mutually exclusive with --start-with)
+    # --end-with (mutually exclusive with --end-before)
+
+    # TODO: should start/end be arguments? hard to do if we want them to be optional
+
+    start_re = end_re = None
+    if start:
+        with handle_re_error('--start'):
+            start_re = compile_pattern(start, fixed_strings, ignore_case, verbose)
+    if end:
+        with handle_re_error('--end'):
+            end_re = compile_pattern(end, fixed_strings, ignore_case, verbose)
+
+    empty_match = re.search('.*', '')
+
+    def match_span(lines):
+        in_span = False
+        in_span_changed = True
+
+        for line in lines:
+            start_match = start_re.search(line) if start_re else None
+
+            if start_re and start_match:
+                if not in_span:
+                    in_span = True
+                    in_span_changed = True
+            elif end_re and end_re.search(line):
+                if in_span:
+                    in_span = False
+                    in_span_changed = True
+
+            if invert_match != in_span:
+                yield line
+            elif repl is not None and in_span_changed:
+                if invert_match and start_match:
+                    repl_match = start_match
+                else:
+                    repl_match = empty_match
+
+                yield repl_match.expand(repl)
+                in_span_changed = False
+
+    match_span.is_iter = True
+    return match_span
 
-    return sub
+
+# LINE FILTERS
 
 
 @cli.command(short_help="Search for pattern.")
 @pattern_argument
 @click.option(
     '-o',
     '--only-matching',
@@ -477,160 +613,254 @@
                     lines.append('\t'.join(groups))
                 return '\n'.join(lines)
             return None
 
     return search
 
 
-@cli.command(short_help="Output matching line spans.")
+def split_field_slices(value):
+    rv = []
+    for slice_str in value.split(','):
+        parts = slice_str.split('-')
+
+        if len(parts) == 1:
+            start = stop = int(parts[0])
+        elif len(parts) == 2:
+            start = int(parts[0]) if parts[0] else None
+            stop = int(parts[1]) if parts[1] else None
+        else:
+            raise ValueError
+
+        if start is None and stop is None:
+            raise ValueError
+        if start is not None and stop is not None:
+            if start > stop:
+                raise ValueError
+        if start is not None:
+            if start < 1:
+                raise ValueError
+            start -= 1
+        if stop is not None:
+            if stop < 1:
+                raise ValueError
+
+        rv.append(slice(start, stop))
+
+    return rv
+
+
+@cli.command(short_help="Output selected parts of lines.")
 @click.option(
-    '--start', '--start-with', metavar='PATTERN', help="Span start (inclusive)."
+    '-d',
+    '--delimiter',
+    metavar='PATTERN',
+    help="Use as field delimiter (consecutive delimiters delimit empty strings). "
+    "If not given, use runs of whitespace as a delimiter "
+    "(with leading/trailing whitespace stripped first).",
 )
-@click.option('--end', '--end-before', metavar='PATTERN', help="Span end (exclusive).")
 @pattern_options
 @click.option(
-    '-v',
-    '--invert-match',
-    is_flag=True,
-    help="Output only lines *not* between those matching --start and --end.",
+    '-n',
+    '--max-split',
+    metavar="INTEGER",
+    type=click.IntRange(1),
+    help="Maximum number of splits to do. The default is no limit.",
 )
 @click.option(
-    '--repl',
-    '--replacement',
-    help="""
-    Replace non-matching line spans with TEXT.
-    With --invert-match, backreferences to captures in --start are expanded;
-    without --invert-match, only escapes are expanded.
-    """,
+    '-f',
+    '--fields',
+    type=split_field_slices,
+    metavar='LIST',
+    help="Select only these fields.",
+)
+@click.option(
+    '-D',
+    '--output-delimiter',
+    show_default=True,
+    help="Use as the output field delimiter. "
+    "If not given, and `--delimiter` and `--fixed-strings` are given, "
+    "use the input delimiter. Otherwise, use one tab character.",
 )
 @section_option
-def match_span(start, end, fixed_strings, ignore_case, verbose, invert_match, repl):
-    """Output only lines between those matching --start and --end.
+def split(
+    delimiter, fixed_strings, ignore_case, verbose, max_split, fields, output_delimiter
+):
+    """Print selected parts of lines.
 
-    Roughly equivalent to: grep START -A9999 | grep END -B9999 | head -n-1
+    Roughly equivalent to:
+
+    \b
+        awk '{ print ... }'     (no --delimiter)
+        cut -d delim            (--fixed-strings --delimiter delim)
+
+    Python equivalents:
+
+    \b
+        line.split()            (no --delimiter)
+        line.split(delim)       (--fixed-strings --delimiter delim)
+        re.split(delim, line)   (--delimiter delim)
+
+    `--fields` takes a comma-separated list of ranges, each range one of:
+
+    \b
+        N     Nth field, counted from 1
+        N-    from Nth field to end of line
+        N-M   from Nth to Mth (included) field
+         -M   from first to Mth (included) field
+
+    This is the same as the cut command. Unlike cut,
+    selected fields are printed in the order from the list,
+    and more than once, if repeated.
 
     """
+    if delimiter is None or (fixed_strings and not ignore_case):
+        max_split = max_split or -1
 
-    # options reserved for future expansion:
-    # --start-after (mutually exclusive with --start-with)
-    # --end-with (mutually exclusive with --end-before)
+        def split(line):
+            return line.split(delimiter, max_split)
 
-    # TODO: should start/end be arguments? hard to do if we want them to be optional
+    else:
+        # TODO: optimization: if the pattern is a simple string ("aa"), use str.split()
+        with handle_re_error('--delimiter'):
+            pattern = compile_pattern(delimiter, fixed_strings, ignore_case, verbose)
+        max_split = max_split or 0
 
-    start_re = (
-        compile_pattern(start, fixed_strings, ignore_case, verbose) if start else None
-    )
-    end_re = compile_pattern(end, fixed_strings, ignore_case, verbose) if end else None
+        def split(line):
+            return pattern.split(line, max_split)
 
-    empty_match = re.search('.*', '')
+    if not output_delimiter:
+        if fixed_strings:
+            output_delimiter = delimiter
+        else:
+            output_delimiter = '\t'
 
-    def match_span(lines):
-        in_span = False
-        in_span_changed = True
+    if not fields:
+        join = output_delimiter.join
+    else:
 
-        for line in lines:
-            start_match = start_re.search(line) if start_re else None
+        def join(parts):
+            return output_delimiter.join(
+                p for field_slice in fields for p in parts[field_slice]
+            )
 
-            if start_re and start_match:
-                if not in_span:
-                    in_span = True
-                    in_span_changed = True
-            elif end_re and end_re.search(line):
-                if in_span:
-                    in_span = False
-                    in_span_changed = True
+    def processor(line):
+        return join(split(line))
 
-            if invert_match != in_span:
-                yield line
-            elif repl is not None and in_span_changed:
+    return processor
 
-                if invert_match and start_match:
-                    repl_match = start_match
-                else:
-                    repl_match = empty_match
+    # TODO:
+    # -s, --only-delimited
+    # --output-format '{1}{2!r}'? zero-indexed? 1-indexed?
+    #   ...this requires a custom string.Formatter that coerces string arguments
 
-                yield repl_match.expand(repl)
-                in_span_changed = False
 
-    match_span.is_iter = True
-    return match_span
+@cli.command(short_help="Replace pattern.")
+@pattern_argument
+@click.argument('repl')
+@click.option('-o', '--only-matching', is_flag=True, help="Output only matching lines.")
+@click.option('--color', is_flag=True, help="Color replacements.")
+@section_option
+def sub(pattern, repl, fixed_strings, only_matching, color):
+    """Replace PATTERN matches with REPL.
+
+    Roughly equivalent to: sed 's/PATTERN/REPL/g'
+
+    Works like re.sub() in Python.
+
+    """
+    if fixed_strings:
+        repl = repl.replace('\\', r'\\')
+    if color:
+        repl = style(repl, fg='red')
+
+    def sub(line):
+        line, subn = pattern.subn(repl, line)
+        if only_matching and not subn:
+            return None
+        return line
+
+    return sub
+
+
+# SPECIALIZED FILTERS
 
 
 @cli.command(short_help="Shorten paths of existing files.")
 @click.option(
     '--include',
     multiple=True,
     metavar='GLOB',
     help="""
     Replace the paths of existing files matching this pattern.
     Both recursive globs and brace expansion are supported, e.g.
-    {src,tests}/**/*.py.
+    `{src,tests}/**/*.py`.
     """,
 )
 @click.option('--modules', is_flag=True, help="Also replaced dotted module names.")
 @click.option(
     '--modules-skip',
     type=click.IntRange(0),
     metavar='INTEGER',
-    help="Path levels to skip to obtain module names from paths. Implies --modules.",
+    help="Path levels to skip to obtain module names from paths. Implies `--modules`.",
 )
 @click.option(
     '--modules-recursive',
     is_flag=True,
     help="""
     Consider the parent directories of selected files to be modules too.
-    Implies --modules.
+    Implies `--modules`.
     """,
 )
 @section_option
 def sub_paths(include, modules, modules_skip, modules_recursive):
     """Replace paths of existing files with shorter versions.
 
     The replacement paths are still unique.
 
     For example, given these files are selected:
 
     \b
-      src/one/mod1.py
-      src/one/two/mod2.py
-      tests/test.py
+        src/one/mod1.py
+        src/one/two/mod2.py
+        tests/test.py
 
     Their paths will be replaced with:
 
     \b
-      .../mod1.py
-      .../mod2.py
-      .../test.py
+        .../mod1.py
+        .../mod2.py
+        .../test.py
 
     Dotted module names derived from the selected files can also be shortened.
-    For example, with --modules-skip 1 --modules-recursive, these modules:
+    For example, with `--modules-skip 1 --modules-recursive`, these modules:
 
     \b
-      one.mod1
-      one.two.mod2
-      one.two
+        one.mod1
+        one.two.mod2
+        one.two
 
     Will be replaced with:
 
     \b
-      ..mod1
-      ..mod2
-      ..two
+        ..mod1
+        ..mod2
+        ..two
 
     """
     from glob import glob
-    from braceexpand import braceexpand
+    from braceexpand import braceexpand, UnbalancedBracesError
     from .paths import shorten_paths, paths_to_modules, make_file_paths_re
 
-    paths = [
-        path
-        for unexpanded_pattern in include
-        for pattern in braceexpand(unexpanded_pattern)
-        for path in glob(pattern, recursive=True)
-    ]
+    paths = []
+    try:
+        for unexpanded_pattern in include:
+            for pattern in braceexpand(unexpanded_pattern):
+                paths.extend(glob(pattern, recursive=True))
+    except UnbalancedBracesError as e:
+        raise BadParameter(e, param_hint=['--include'])
 
     replacements = shorten_paths(paths, os.sep, '...')
 
     if modules or modules_recursive or modules_skip is not None:
         modules = paths_to_modules(
             paths, skip=modules_skip or 0, recursive=modules_recursive
         )
@@ -711,214 +941,136 @@
 
     def sub_link(line):
         return pattern_re.sub(repl, line)
 
     return sub_link
 
 
-@cli.command(short_help="Output the first part of sections.")
-@click.option(
-    '-n',
-    'count',
-    metavar="COUNT",
-    type=int,
-    default=10,
-    show_default=True,
-    help="Print the first COUNT lines. "
-    "With a leading '-', print all but the last COUNT lines.",
-)
-@section_option
-def head(count):
-    """Print the first COUNT lines.
-
-    Roughly equivalent to: head -n COUNT
-
-    """
-    from itertools import islice
+# HELP
 
-    def head(lines):
-        if count >= 0:
-            return islice(lines, count)
-        else:
-            # TODO: don't read in memory, use a temporary file
-            return iter(list(lines)[0:count])
 
-    head.is_iter = True
-    return head
-
-
-def tail_count_int(value):
-    value = value.strip()
-    if value.startswith('+'):
-        rv = int(value) - 1
-    elif value.startswith('-'):
-        rv = int(value)
-    else:
-        rv = -int(value)
-    return rv
+@cli.command()
+@click.option('--all', is_flag=True, help="Show help for all commands, man-style.")
+@click.pass_context
+def help(ctx, all):
+    """Show detailed help."""
 
+    ctx = ctx.find_root()
+    original_help = ctx.command.help
+    ctx.command.help = color_help(linesieve.__doc__)
 
-@cli.command(short_help="Output the last part of sections.")
-@click.option(
-    '-n',
-    'count',
-    metavar="COUNT",
-    type=tail_count_int,
-    default=10,
-    show_default=True,
-    help="Print the last COUNT lines. "
-    "With a leading '+', print lines starting with line COUNT.",
-)
-@section_option
-def tail(count):
-    """Print the last COUNT lines.
+    try:
+        if not all:
+            click.echo(ctx.get_help(), color=ctx.color)
+        else:
+            click.echo_via_pager(format_help_all(ctx))
+    finally:
+        ctx.command.help = original_help
 
-    Roughly equivalent to: tail -n COUNT
+    ctx.exit()
 
-    """
-    from itertools import islice
-    from collections import deque
 
-    def tail(lines):
-        if count <= 0:
-            # TODO: don't read in memory, use a temporary file
-            return iter(deque(lines, maxlen=-count))
-        else:
-            return islice(lines, count, None)
+def color_help(text):
+    KWARGS = {
+        'dim': dict(dim=True),
+        'red': dict(fg='red'),
+        'green': dict(fg='green'),
+        'yellow': dict(fg='yellow'),
+    }
 
-    tail.is_iter = True
-    return tail
+    def repl(match):
+        line, options = match.groups()
+        kwargs = {}
+        for option in options.split():
+            kwargs.update(KWARGS[option])
+        return style(line, **kwargs)
 
+    options_re = '|'.join(map(re.escape, KWARGS))
+    line_re = f"(.*)#((?: +(?:{options_re}))+ *)$"
 
-def split_field_slices(value):
-    rv = []
-    for slice_str in value.split(','):
-        parts = slice_str.split('-')
+    return re.sub(line_re, repl, text, flags=re.M)
 
-        if len(parts) == 1:
-            start = stop = int(parts[0])
-        elif len(parts) == 2:
-            start = int(parts[0]) if parts[0] else None
-            stop = int(parts[1]) if parts[1] else None
-        else:
-            raise ValueError
 
-        if start is None and stop is None:
-            raise ValueError
-        if start is not None and stop is not None:
-            if start > stop:
-                raise ValueError
-        if start is not None:
-            if start < 1:
-                raise ValueError
-            start -= 1
-        if stop is not None:
-            if stop < 1:
-                raise ValueError
+class ManFormatter(click.HelpFormatter):
+    def __init__(self):
+        super().__init__(4, max_width=999999)
+        # print(self.width)
 
-        rv.append(slice(start, stop))
+    def write_dl(self, rows, col_max=30, col_spacing=2):
+        """Write the options definition after the term, indented.
 
-    return rv
+        col_max and col_spacing are ignored.
 
+        """
+        # for reasons (click bug?), the original write_dl() will spill over
+        # if indenting more than once (worsened by indent_increment > 2);
+        # this does not happen with our implementation
 
-@cli.command(short_help="Output selected parts of lines.")
-@click.option(
-    '-d',
-    '--delimiter',
-    metavar='PATTERN',
-    help="Use as field delimiter (consecutive delimiters delimit empty strings). "
-    "If not given, use runs of whitespace as a delimiter "
-    "(with leading/trailing whitespace stripped first).",
-)
-@pattern_options
-@click.option(
-    '-n',
-    '--max-split',
-    metavar="INTEGER",
-    type=click.IntRange(1),
-    help="Maximum number of splits to do. The default is no limit.",
-)
-@click.option(
-    '-f',
-    '--fields',
-    type=split_field_slices,
-    metavar='LIST',
-    help="Select only these fields.",
-)
-@click.option(
-    '-D',
-    '--output-delimiter',
-    show_default=True,
-    help="Use as the output field delimiter. "
-    "If not given, and --delimiter and --fixed-strings are given, "
-    "use the input delimiter. Otherwise, use one tab character.",
-)
-@section_option
-def split(
-    delimiter, fixed_strings, ignore_case, verbose, max_split, fields, output_delimiter
-):
-    """Print selected parts of lines.
+        for i, (first, second) in enumerate(rows, 1):
+            self.write_text(first)
+            with self.indentation():
+                self.write_text(second)
+            if i != len(rows):
+                self.write_paragraph()
 
-    Roughly equivalent to:
+    def write_usage(self, prog, args='', prefix='Usage: '):
+        if prefix is not None:
+            prefix = style(prefix, bold=True)
 
-    \b
-      awk '{ print ... }'     (no --delimiter)
-      cut -d delim            (--fixed-strings --delimiter delim)
+        self.write(f"{'':>{self.current_indent}}")
+        super().write_usage(prog, args, prefix)
 
-    Python equivalents:
+    def write_heading(self, heading):
+        heading = style(heading, bold=True)
+        self.write(f"{'':>{self.current_indent}}{heading}\n")
 
-    \b
-      line.split()            (no --delimiter)
-      line.split(delim)       (--fixed-strings --delimiter delim)
-      re.split(delim, line)   (--delimiter delim)
+    @contextmanager
+    def supersection(self, name, short=None):
+        title = style(name.upper(), bold=True)
+        if short:
+            title += style(' - ' + short, dim=True)
 
-    --fields takes a comma-separated list of ranges, each range one of:
+        self.write(title)
+        self.write_paragraph()
+        self.write_paragraph()
 
-    \b
-      N     Nth field, counted from 1
-      N-    from Nth field to end of line
-      N-M   from Nth to Mth (included) field
-       -M   from first to Mth (included) field
+        with self.indentation():
+            yield
 
-    This is the same as the cut command. Unlike cut,
-    selected fields are printed in the order from the list,
-    and more than once, if repeated.
-
-    """
-    if delimiter is None or (fixed_strings and not ignore_case):
-        max_split = max_split or -1
+        self.write_paragraph()
 
-        def split(line):
-            return line.split(delimiter, max_split)
 
-    else:
-        # TODO: optimization: if the pattern is a simple string ("aa"), use str.split()
-        pattern = compile_pattern(delimiter, fixed_strings, ignore_case, verbose)
-        max_split = max_split or 0
+def format_help_all(ctx):
+    formatter = ManFormatter()
+    commands = list_commands_recursive(ctx.command, ctx)
 
-        def split(line):
-            return pattern.split(line, max_split)
+    for path, command in commands:
+        short = command.get_short_help_str(limit=55)
+        if short:
+            first = short.partition(' ')[0]
+            if first.istitle():
+                short = first.lower() + short[len(first) :]
+            short = short.rstrip('.')
 
-    if not output_delimiter:
-        if fixed_strings:
-            output_delimiter = delimiter
+        if command is ctx.command:
+            format_ctx = ctx
         else:
-            output_delimiter = '\t'
+            format_ctx = type(ctx)(command, ctx, command.name)
 
-    if not fields:
-        join = output_delimiter.join
-    else:
-
-        def join(parts):
-            return output_delimiter.join(
-                p for field_slice in fields for p in parts[field_slice]
-            )
+        with formatter.supersection(' '.join(path), short):
+            command.format_help(format_ctx, formatter)
 
-    def processor(line):
-        return join(split(line))
+    return formatter.getvalue()
 
-    return processor
 
-    # TODO:
-    # -s, --only-delimited
-    # --output-format '{1}{2!r}'? zero-indexed? 1-indexed?
-    #   ...this requires a custom string.Formatter that coerces string arguments
+def list_commands_recursive(self, ctx, path=()):
+    path = path + (self.name,)
+    yield path, self
+    if not hasattr(self, 'list_commands'):
+        return
+    for subcommand in self.list_commands(ctx):
+        cmd = self.get_command(ctx, subcommand)
+        if cmd is None:
+            continue
+        if cmd.hidden:
+            continue
+        yield from list_commands_recursive(cmd, ctx, path)
```

### Comparing `linesieve-1.0a9/src/linesieve/parsing.py` & `linesieve-1.0b1/src/linesieve/parsing.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,34 +29,29 @@
 
     end_is_failure = None not in {success_pattern, failure_pattern}
     groups = filter_sections(groups, show_section, end_is_failure)
 
     @lru_cache
     def get_filters(section):
         rv = []
-        for section_re, filter in line_filters:
-            if not section_re or section_re.search(section):
+        for section_res, filter in line_filters:
+            if not section_res or any(r.search(section) for r in section_res):
                 rv.append(filter)
         return rv
 
     groups = filter_lines(groups, get_filters)
     groups = dedupe_blank_lines(groups)
 
     return groups
 
 
-MATCH_NOTHING = '$nothing'
+MATCH_NOTHING_RE = re.compile('$nothing')
 
 
-def annotate_lines(
-    lines,
-    section_pattern=None,
-    success_pattern=None,
-    failure_pattern=None,
-):
+def annotate_lines(lines, section_re=None, success_re=None, failure_re=None):
     """Annotate lines with their corresponding section.
     Stop when encountering a success/failure marker.
 
     The section and success/failure markers are considered to be one line.
 
     Yield (section, line) pairs, one for each content line.
     If a section is empty, yield exactly one (section, None) pair.
@@ -71,24 +66,24 @@
     The section and label are:
 
     * the group named 'name', if any
     * the first captured group, if any
     * the entire match, otherwise
 
     >>> lines = ['0', 'one:', '1', 'two:', 'three:', '3', 'end']
-    >>> list(annotate_lines(lines, '(.*):$', 'end'))
+    >>> list(annotate_lines(lines, re.compile('(.*):$'), re.compile('end')))
     [('', '0'), ('one', '1'), ('two', None), ('three', '3'), (True, 'end')]
 
     >>> list(annotate_lines([]))
     [('', None), (None, None)]
 
     """
     section_re, success_re, failure_re = [
-        re.compile(pattern if pattern is not None else MATCH_NOTHING)
-        for pattern in (section_pattern, success_pattern, failure_pattern)
+        pattern if pattern is not None else MATCH_NOTHING_RE
+        for pattern in (section_re, success_re, failure_re)
     ]
 
     done = False
     ok = None
     section = ''
     yielded_lines = False
     for line in chain(lines, [None]):
```

### Comparing `linesieve-1.0a9/src/linesieve/paths.py` & `linesieve-1.0b1/src/linesieve/paths.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,18 +4,16 @@
 
 def shorten_paths(paths, sep, ellipsis):
     shortened = {path: path.split(sep) for path in paths}
 
     _do_end(shortened.values(), 0, -1)
 
     for original, mask in shortened.items():
-
         path = []
         for ps, ms in zip(original.split(sep), mask):
-
             if ms is None:
                 path.append(ps)
             else:
                 if not path or path[-1] != ellipsis:
                     path.append(ellipsis)
 
         shortened[original] = sep.join(path)
```

### Comparing `linesieve-1.0a9/tests/test_cli.py` & `linesieve-1.0b1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `linesieve-1.0a9/tests/test_paths.py` & `linesieve-1.0b1/tests/test_paths.py`

 * *Files identical despite different names*

