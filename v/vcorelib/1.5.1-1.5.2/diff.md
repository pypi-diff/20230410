# Comparing `tmp/vcorelib-1.5.1.tar.gz` & `tmp/vcorelib-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcorelib-1.5.1.tar", last modified: Sun Apr  9 04:27:39 2023, max compression
+gzip compressed data, was "vcorelib-1.5.2.tar", last modified: Mon Apr 10 05:37:49 2023, max compression
```

## Comparing `vcorelib-1.5.1.tar` & `vcorelib-1.5.2.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:27:39.181969 vcorelib-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-09 04:25:55.000000 vcorelib-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-09 04:27:39.181969 vcorelib-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-09 04:25:55.000000 vcorelib-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-09 04:25:55.000000 vcorelib-1.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 04:27:39.181969 vcorelib-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-09 04:25:55.000000 vcorelib-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:27:39.169968 vcorelib-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-09 04:25:55.000000 vcorelib-1.5.1/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-09 04:25:55.000000 vcorelib-1.5.1/tests/test_namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:27:39.169968 vcorelib-1.5.1/vcorelib/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:27:39.169968 vcorelib-1.5.1/vcorelib/args/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/args/newline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:27:39.173968 vcorelib-1.5.1/vcorelib/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/asyncio/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/asyncio/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:27:39.173968 vcorelib-1.5.1/vcorelib/dict/
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/dict/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/dict/codec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/dict/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/dict/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:27:39.173968 vcorelib-1.5.1/vcorelib/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/graph/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/graph/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/graph/port.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:27:39.173968 vcorelib-1.5.1/vcorelib/io/
--rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/io/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:27:39.173968 vcorelib-1.5.1/vcorelib/io/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/io/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/io/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/io/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/io/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/io/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:27:39.173968 vcorelib-1.5.1/vcorelib/math/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/math/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:27:39.177968 vcorelib-1.5.1/vcorelib/math/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/math/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/math/analysis/average.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:27:39.177968 vcorelib-1.5.1/vcorelib/math/analysis/rate/
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/math/analysis/rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/math/analysis/rate/limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/math/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:27:39.177968 vcorelib-1.5.1/vcorelib/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/paths/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/paths/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/paths/info_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:27:39.177968 vcorelib-1.5.1/vcorelib/platform/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:27:39.177968 vcorelib-1.5.1/vcorelib/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/schemas/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/schemas/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:27:39.177968 vcorelib-1.5.1/vcorelib/script/
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:27:39.177968 vcorelib-1.5.1/vcorelib/target/
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/target/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/target/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/target/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/target/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:27:39.177968 vcorelib-1.5.1/vcorelib/task/
--rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:27:39.177968 vcorelib-1.5.1/vcorelib/task/dict/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/task/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/task/dict/melder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/task/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:27:39.181969 vcorelib-1.5.1/vcorelib/task/subprocess/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/task/subprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/task/subprocess/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:27:39.181969 vcorelib-1.5.1/vcorelib/task/time/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/task/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-09 04:25:55.000000 vcorelib-1.5.1/vcorelib/task/time/sleep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:27:39.169968 vcorelib-1.5.1/vcorelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-09 04:27:39.000000 vcorelib-1.5.1/vcorelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-09 04:27:39.000000 vcorelib-1.5.1/vcorelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 04:27:39.000000 vcorelib-1.5.1/vcorelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-09 04:27:39.000000 vcorelib-1.5.1/vcorelib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-09 04:27:39.000000 vcorelib-1.5.1/vcorelib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.056496 vcorelib-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-10 05:36:30.000000 vcorelib-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-10 05:37:49.056496 vcorelib-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-10 05:36:30.000000 vcorelib-1.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-10 05:36:30.000000 vcorelib-1.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 05:37:49.056496 vcorelib-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-10 05:36:30.000000 vcorelib-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.036496 vcorelib-1.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-10 05:36:30.000000 vcorelib-1.5.2/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-10 05:36:30.000000 vcorelib-1.5.2/tests/test_namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.036496 vcorelib-1.5.2/vcorelib/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.040495 vcorelib-1.5.2/vcorelib/args/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/args/newline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.040495 vcorelib-1.5.2/vcorelib/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/asyncio/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/asyncio/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.044495 vcorelib-1.5.2/vcorelib/dict/
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/dict/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/dict/codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/dict/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/dict/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.044495 vcorelib-1.5.2/vcorelib/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/graph/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/graph/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/graph/port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.044495 vcorelib-1.5.2/vcorelib/io/
+-rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/io/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.044495 vcorelib-1.5.2/vcorelib/io/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/io/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/io/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/io/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/io/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/io/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.048495 vcorelib-1.5.2/vcorelib/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/math/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.048495 vcorelib-1.5.2/vcorelib/math/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/math/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/math/analysis/average.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.048495 vcorelib-1.5.2/vcorelib/math/analysis/rate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/math/analysis/rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/math/analysis/rate/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/math/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.048495 vcorelib-1.5.2/vcorelib/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/paths/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/paths/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/paths/info_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.048495 vcorelib-1.5.2/vcorelib/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.052496 vcorelib-1.5.2/vcorelib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/schemas/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/schemas/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.052496 vcorelib-1.5.2/vcorelib/script/
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.052496 vcorelib-1.5.2/vcorelib/target/
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/target/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/target/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/target/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/target/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.052496 vcorelib-1.5.2/vcorelib/task/
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.052496 vcorelib-1.5.2/vcorelib/task/dict/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/task/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/task/dict/melder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/task/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.052496 vcorelib-1.5.2/vcorelib/task/subprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/task/subprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/task/subprocess/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.056496 vcorelib-1.5.2/vcorelib/task/time/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/task/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-10 05:36:30.000000 vcorelib-1.5.2/vcorelib/task/time/sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:37:49.040495 vcorelib-1.5.2/vcorelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-10 05:37:49.000000 vcorelib-1.5.2/vcorelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-10 05:37:49.000000 vcorelib-1.5.2/vcorelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 05:37:49.000000 vcorelib-1.5.2/vcorelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-10 05:37:49.000000 vcorelib-1.5.2/vcorelib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 05:37:49.000000 vcorelib-1.5.2/vcorelib.egg-info/top_level.txt
```

### Comparing `vcorelib-1.5.1/LICENSE` & `vcorelib-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/PKG-INFO` & `vcorelib-1.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 1.5.1
+Version: 1.5.2
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=20d293956056ae6ed7f6904fc221a589
+    hash=4f5dac9c4ed3066040913d4d4437e4bf
     =====================================
 -->
 
-# vcorelib ([1.5.1](https://pypi.org/project/vcorelib/))
+# vcorelib ([1.5.2](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-1.5.1/README.md` & `vcorelib-1.5.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=20d293956056ae6ed7f6904fc221a589
+    hash=4f5dac9c4ed3066040913d4d4437e4bf
     =====================================
 -->
 
-# vcorelib ([1.5.1](https://pypi.org/project/vcorelib/))
+# vcorelib ([1.5.2](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-1.5.1/pyproject.toml` & `vcorelib-1.5.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "vcorelib"
-version = "1.5.1"
+version = "1.5.2"
 description = "A collection of core Python utilities."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `vcorelib-1.5.1/setup.py` & `vcorelib-1.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/tests/test_logging.py` & `vcorelib-1.5.2/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/tests/test_namespace.py` & `vcorelib-1.5.2/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/args/__init__.py` & `vcorelib-1.5.2/vcorelib/args/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/args/newline.py` & `vcorelib-1.5.2/vcorelib/args/newline.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/asyncio/__init__.py` & `vcorelib-1.5.2/vcorelib/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/asyncio/cli.py` & `vcorelib-1.5.2/vcorelib/asyncio/cli.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/asyncio/subprocess.py` & `vcorelib-1.5.2/vcorelib/asyncio/subprocess.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/dict/__init__.py` & `vcorelib-1.5.2/vcorelib/dict/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/dict/cache.py` & `vcorelib-1.5.2/vcorelib/dict/cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/dict/codec.py` & `vcorelib-1.5.2/vcorelib/dict/codec.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/dict/config.py` & `vcorelib-1.5.2/vcorelib/dict/config.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/dict/env.py` & `vcorelib-1.5.2/vcorelib/dict/env.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 # internal
 from vcorelib.dict import GenericDict as _GenericDict
 
 GenericList = _List[_Any]
 
 
-def str_resolve_env_var(data: str, env: _Mapping[str, str] = None) -> str:
+def str_resolve_env_var(data: str, env: _Mapping[str, _Any] = None) -> str:
     """
     Convert string data to a resolved environment variable if the string begins
     with '$' and is a key in the environment with a non-empty value.
     """
 
     if env is None:
         env = _environ
```

### Comparing `vcorelib-1.5.1/vcorelib/graph/__init__.py` & `vcorelib-1.5.2/vcorelib/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/graph/abc.py` & `vcorelib-1.5.2/vcorelib/graph/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/graph/edge.py` & `vcorelib-1.5.2/vcorelib/graph/edge.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/graph/node.py` & `vcorelib-1.5.2/vcorelib/graph/node.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/graph/port.py` & `vcorelib-1.5.2/vcorelib/graph/port.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/io/__init__.py` & `vcorelib-1.5.2/vcorelib/io/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/io/abc.py` & `vcorelib-1.5.2/vcorelib/io/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/io/archive/__init__.py` & `vcorelib-1.5.2/vcorelib/io/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/io/cache.py` & `vcorelib-1.5.2/vcorelib/io/cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/io/decode.py` & `vcorelib-1.5.2/vcorelib/io/decode.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/io/encode.py` & `vcorelib-1.5.2/vcorelib/io/encode.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/io/types.py` & `vcorelib-1.5.2/vcorelib/io/types.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/logging.py` & `vcorelib-1.5.2/vcorelib/logging.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/math/__init__.py` & `vcorelib-1.5.2/vcorelib/math/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/math/analysis/average.py` & `vcorelib-1.5.2/vcorelib/math/analysis/average.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/math/analysis/rate/__init__.py` & `vcorelib-1.5.2/vcorelib/math/analysis/rate/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/math/analysis/rate/limiter.py` & `vcorelib-1.5.2/vcorelib/math/analysis/rate/limiter.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/math/time.py` & `vcorelib-1.5.2/vcorelib/math/time.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/namespace.py` & `vcorelib-1.5.2/vcorelib/namespace.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/paths/__init__.py` & `vcorelib-1.5.2/vcorelib/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/paths/context.py` & `vcorelib-1.5.2/vcorelib/paths/context.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/paths/info.py` & `vcorelib-1.5.2/vcorelib/paths/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,22 +100,24 @@
         to_update["size"] = self.size
         to_update["md5_hex"] = self.md5_hex
         to_update["modified_ns"] = self.modified_ns
 
         return data
 
     @staticmethod
-    def from_json(data: _JsonObject) -> _Dict[_Path, "FileInfo"]:
+    def from_json(
+        data: _JsonObject, force: bool = False
+    ) -> _Dict[_Path, "FileInfo"]:
         """Create file info from JSON data."""
 
         result = {}
         for key, info in data.items():
             assert isinstance(info, _Mapping)
             path = _Path(key)
-            if path.is_file():
+            if path.is_file() or force:
                 result[path] = FileInfo(
                     path,
                     _cast(int, info["size"]),
                     _cast(str, info["md5_hex"]),
                     _cast(int, info["modified_ns"]),
                 )
         return result
```

### Comparing `vcorelib-1.5.1/vcorelib/paths/info_cache.py` & `vcorelib-1.5.2/vcorelib/paths/info_cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 A module implementing a file-info cache.
 """
 
 # built-in
 from contextlib import contextmanager as _contextmanager
+import logging as _logging
 from pathlib import Path as _Path
 from typing import Callable as _Callable
 from typing import Dict as _Dict
 from typing import Iterator as _Iterator
 from typing import NamedTuple
 from typing import Optional as _Optional
 from typing import Tuple as _Tuple
@@ -53,54 +54,62 @@
     "file_info_cache",
     "FileInfo",
     "FileChangeEvent",
 ]
 
 
 def log_file_change_event(
-    logger: LoggerType, change: FileChanged, base: _Pathlike = None
+    level: int, logger: LoggerType, change: FileChanged, base: _Pathlike = None
 ) -> None:
     """Log information based on a file-change event."""
 
     if change.event is FileChangeEvent.CREATED:
         assert change.new is not None
-        logger.info(
-            "File '%s' is newly created.", _rel(change.new.path, base=base)
+        logger.log(
+            level,
+            "File '%s' is newly created.",
+            _rel(change.new.path, base=base),
         )
     elif change.event is FileChangeEvent.REMOVED:
         assert change.old is not None
-        logger.info("File '%s' was removed.", _rel(change.old.path, base=base))
+        logger.log(
+            level, "File '%s' was removed.", _rel(change.old.path, base=base)
+        )
     else:
         assert change.new is not None
         assert change.old is not None
 
-        logger.info(
+        logger.log(
+            level,
             "File '%s' changed (%d bytes added/removed).",
             change.new.path,
             change.new.size - change.old.size,
         )
 
 
 class FileInfoManager:
     """A class simplifying evaluation of changes to files on disk."""
 
     def __init__(
         self,
         poll_cb: FileChangedCallback,
         initial: _Dict[_Path, FileInfo] = None,
         logger: LoggerType = None,
+        level: int = _logging.DEBUG,
     ) -> None:
         """Initialize this file-info manager."""
 
         self.poll = poll_cb
 
         if initial is None:
             initial = {}
         self.infos = initial
+
         self.logger = logger
+        self.level = level
 
         # If we have initial files, poll them all.
         self.poll_existing()
 
     def _handle_info(self, path: _Path, info: _Optional[FileInfo]) -> None:
         """Update our internal tracking."""
 
@@ -144,26 +153,33 @@
         """
         Call the provided callback with the change event. Log information if
         a logger is provided.
         """
 
         # Log the event, if a logger was provided.
         if self.logger is not None:
-            log_file_change_event(self.logger, change, base=base)
+            log_file_change_event(self.level, self.logger, change, base=base)
 
         return self.poll(change)
 
     def _poll_path(
         self, path: _Path
     ) -> _Tuple[_Optional[FileChangeEvent], _Optional[FileInfo]]:
         """Get information about a file-system path."""
 
+        change = None
+        file_info = None
+
         # If the path isn't in the mapping, it's a new file.
         if path not in self.infos:
-            return FileChangeEvent.CREATED, FileInfo.from_file(path)
+            if path.is_file():
+                change = FileChangeEvent.CREATED
+                file_info = FileInfo.from_file(path)
+
+            return change, file_info
 
         # Determine if the existing file has changed.
         return self.infos[path].poll()
 
     def poll_file(self, path: _Pathlike, base: _Pathlike = None) -> None:
         """Check if a file has changed and invoke the callback if so."""
 
@@ -180,21 +196,26 @@
 
 
 @_contextmanager
 def file_info_cache(
     cache_path: _Pathlike,
     poll_cb: FileChangedCallback,
     logger: LoggerType = None,
+    level: int = _logging.DEBUG,
 ) -> _Iterator[FileInfoManager]:
     """Obtain a file-info manager as a cached context."""
 
     path = _normalize(cache_path)
     assert not path.is_dir(), f"'{path}' is a directory!"
     with FileCache(path).loaded() as data:
         manager = FileInfoManager(
-            poll_cb, FileInfo.from_json(data), logger=logger
+            poll_cb,
+            FileInfo.from_json(data, force=True),
+            logger=logger,
+            level=level,
         )
         yield manager
 
         # Update dictionary data with the current cache contents.
+        data.clear()
         for info in manager.infos.values():
             info.to_json(data)
```

### Comparing `vcorelib-1.5.1/vcorelib/platform/__init__.py` & `vcorelib-1.5.2/vcorelib/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/schemas/__init__.py` & `vcorelib-1.5.2/vcorelib/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/schemas/base.py` & `vcorelib-1.5.2/vcorelib/schemas/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/schemas/json.py` & `vcorelib-1.5.2/vcorelib/schemas/json.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/schemas/mixins.py` & `vcorelib-1.5.2/vcorelib/schemas/mixins.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/script/__init__.py` & `vcorelib-1.5.2/vcorelib/script/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,19 +5,25 @@
 # built-in
 import importlib.machinery
 import importlib.util
 from pathlib import Path as _Path
 from typing import Any as _Any
 from typing import Set as _Set
 
+# internal
+from vcorelib.paths import Pathlike as _Pathlike
+from vcorelib.paths import normalize as _normalize
 
-def invoke_script(script: _Path, method: str, *args, **kwargs) -> _Any:
+
+def invoke_script(script: _Pathlike, method: str, *args, **kwargs) -> _Any:
     """Invoke a method from an external script."""
 
-    loader = importlib.machinery.SourceFileLoader("script", str(script))
+    loader = importlib.machinery.SourceFileLoader(
+        "script", str(_normalize(script))
+    )
     spec = importlib.util.spec_from_loader("script", loader)
     assert spec is not None
     script_module = importlib.util.module_from_spec(spec)
     loader.exec_module(script_module)
 
     # Invoke the script method.
     return getattr(script_module, method)(*args, **kwargs)
```

### Comparing `vcorelib-1.5.1/vcorelib/target/__init__.py` & `vcorelib-1.5.2/vcorelib/target/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/target/evaluation.py` & `vcorelib-1.5.2/vcorelib/target/evaluation.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/target/expression.py` & `vcorelib-1.5.2/vcorelib/target/expression.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/target/resolver.py` & `vcorelib-1.5.2/vcorelib/target/resolver.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/task/__init__.py` & `vcorelib-1.5.2/vcorelib/task/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/task/dict/melder.py` & `vcorelib-1.5.2/vcorelib/task/dict/melder.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/task/manager.py` & `vcorelib-1.5.2/vcorelib/task/manager.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/task/subprocess/run.py` & `vcorelib-1.5.2/vcorelib/task/subprocess/run.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib/task/time/sleep.py` & `vcorelib-1.5.2/vcorelib/task/time/sleep.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.5.1/vcorelib.egg-info/PKG-INFO` & `vcorelib-1.5.2/vcorelib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 1.5.1
+Version: 1.5.2
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=20d293956056ae6ed7f6904fc221a589
+    hash=4f5dac9c4ed3066040913d4d4437e4bf
     =====================================
 -->
 
-# vcorelib ([1.5.1](https://pypi.org/project/vcorelib/))
+# vcorelib ([1.5.2](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-1.5.1/vcorelib.egg-info/SOURCES.txt` & `vcorelib-1.5.2/vcorelib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

