# Comparing `tmp/stactools-0.4.5.tar.gz` & `tmp/stactools-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stactools-0.4.5.tar", last modified: Fri Mar 24 16:32:29 2023, max compression
+gzip compressed data, was "stactools-0.4.6.tar", last modified: Mon Apr 10 17:23:34 2023, max compression
```

## Comparing `stactools-0.4.5.tar` & `stactools-0.4.6.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:32:29.711399 stactools-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-24 16:32:08.000000 stactools-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-03-24 16:32:29.711399 stactools-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-03-24 16:32:08.000000 stactools-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-24 16:32:08.000000 stactools-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-03-24 16:32:29.711399 stactools-0.4.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:32:29.691400 stactools-0.4.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:32:29.695400 stactools-0.4.5/src/stactools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:32:29.699400 stactools-0.4.5/src/stactools/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:32:29.703400 stactools-0.4.5/src/stactools/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/cli/commands/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/cli/commands/add_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/cli/commands/add_raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/cli/commands/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/cli/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/cli/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/cli/commands/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/cli/commands/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/cli/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/cli/commands/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/cli/commands/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/cli/commands/update_extent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/cli/commands/update_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/cli/commands/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/cli/commands/version.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/cli/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/cli/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:32:29.707399 stactools-0.4.5/src/stactools/core/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/core/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/core/add_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/core/add_raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/core/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/core/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/core/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:32:29.707399 stactools-0.4.5/src/stactools/core/io/
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/core/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/core/io/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/core/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/core/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/core/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/core/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:32:29.711399 stactools-0.4.5/src/stactools/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/core/utils/antimeridian.py
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/core/utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    40298 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/core/utils/raster_footprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/core/utils/round.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/core/utils/subprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:32:29.711399 stactools-0.4.5/src/stactools/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/testing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/testing/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/testing/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-03-24 16:32:08.000000 stactools-0.4.5/src/stactools/testing/test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:32:29.699400 stactools-0.4.5/src/stactools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-03-24 16:32:29.000000 stactools-0.4.5/src/stactools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-03-24 16:32:29.000000 stactools-0.4.5/src/stactools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 16:32:29.000000 stactools-0.4.5/src/stactools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-24 16:32:29.000000 stactools-0.4.5/src/stactools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 16:32:29.000000 stactools-0.4.5/src/stactools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-24 16:32:29.000000 stactools-0.4.5/src/stactools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-24 16:32:29.000000 stactools-0.4.5/src/stactools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:34.012019 stactools-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-10 17:23:16.000000 stactools-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-04-10 17:23:34.012019 stactools-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-04-10 17:23:16.000000 stactools-0.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-10 17:23:16.000000 stactools-0.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-10 17:23:34.012019 stactools-0.4.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:33.992018 stactools-0.4.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:33.992018 stactools-0.4.6/src/stactools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:34.000018 stactools-0.4.6/src/stactools/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:34.004018 stactools-0.4.6/src/stactools/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/add_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/add_raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/update_extent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/update_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/commands/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/cli/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:34.008019 stactools-0.4.6/src/stactools/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/add_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/add_raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:34.008019 stactools-0.4.6/src/stactools/core/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/io/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:34.012019 stactools-0.4.6/src/stactools/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11624 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/utils/antimeridian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40595 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/utils/raster_footprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/utils/round.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/core/utils/subprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:34.012019 stactools-0.4.6/src/stactools/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/testing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/testing/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/testing/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-10 17:23:16.000000 stactools-0.4.6/src/stactools/testing/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:23:33.996018 stactools-0.4.6/src/stactools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-04-10 17:23:33.000000 stactools-0.4.6/src/stactools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-10 17:23:33.000000 stactools-0.4.6/src/stactools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:23:33.000000 stactools-0.4.6/src/stactools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-10 17:23:33.000000 stactools-0.4.6/src/stactools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:23:33.000000 stactools-0.4.6/src/stactools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-10 17:23:33.000000 stactools-0.4.6/src/stactools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-10 17:23:33.000000 stactools-0.4.6/src/stactools.egg-info/top_level.txt
```

### Comparing `stactools-0.4.5/LICENSE` & `stactools-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/PKG-INFO` & `stactools-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools
-Version: 0.4.5
+Version: 0.4.6
 Summary: Command line tool and Python library for working with STAC
 Home-page: https://github.com/stac-utils/stactools
 Author: stac-utils
 Author-email: stac@radiant.earth
 Project-URL: Documentation, https://stactools.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/stac-utils/stactools/issues
 Keywords: stactools,pystac,imagery,raster,catalog,STAC
```

### Comparing `stactools-0.4.5/README.md` & `stactools-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/setup.cfg` & `stactools-0.4.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/cli/__init__.py` & `stactools-0.4.6/src/stactools/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/cli/cli.py` & `stactools-0.4.6/src/stactools/cli/cli.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/cli/commands/add.py` & `stactools-0.4.6/src/stactools/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/cli/commands/add_asset.py` & `stactools-0.4.6/src/stactools/cli/commands/add_asset.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/cli/commands/add_raster.py` & `stactools-0.4.6/src/stactools/cli/commands/add_raster.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/cli/commands/copy.py` & `stactools-0.4.6/src/stactools/cli/commands/copy.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/cli/commands/create.py` & `stactools-0.4.6/src/stactools/cli/commands/create.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/cli/commands/info.py` & `stactools-0.4.6/src/stactools/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/cli/commands/layout.py` & `stactools-0.4.6/src/stactools/cli/commands/layout.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/cli/commands/lint.py` & `stactools-0.4.6/src/stactools/cli/commands/lint.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/cli/commands/merge.py` & `stactools-0.4.6/src/stactools/cli/commands/merge.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/cli/commands/summary.py` & `stactools-0.4.6/src/stactools/cli/commands/summary.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/cli/commands/update_extent.py` & `stactools-0.4.6/src/stactools/cli/commands/update_extent.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/cli/commands/update_geometry.py` & `stactools-0.4.6/src/stactools/cli/commands/update_geometry.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/cli/commands/validate.py` & `stactools-0.4.6/src/stactools/cli/commands/validate.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/cli/commands/version.py` & `stactools-0.4.6/src/stactools/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/cli/registry.py` & `stactools-0.4.6/src/stactools/cli/registry.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/core/__init__.py` & `stactools-0.4.6/src/stactools/core/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     "merge_all_items",
     "merge_items",
     "move_asset_file_to_item",
     "move_assets",
     "move_all_assets",
     "use_fsspec",
 ]
-__version__ = "0.4.5"
+__version__ = "0.4.6"
```

### Comparing `stactools-0.4.5/src/stactools/core/add.py` & `stactools-0.4.6/src/stactools/core/add.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/core/add_asset.py` & `stactools-0.4.6/src/stactools/core/add_asset.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/core/add_raster.py` & `stactools-0.4.6/src/stactools/core/add_raster.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/core/copy.py` & `stactools-0.4.6/src/stactools/core/copy.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/core/create.py` & `stactools-0.4.6/src/stactools/core/create.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/core/geometry.py` & `stactools-0.4.6/src/stactools/core/geometry.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/core/io/__init__.py` & `stactools-0.4.6/src/stactools/core/io/__init__.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/core/io/xml.py` & `stactools-0.4.6/src/stactools/core/io/xml.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/core/layout.py` & `stactools-0.4.6/src/stactools/core/layout.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/core/merge.py` & `stactools-0.4.6/src/stactools/core/merge.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/core/projection.py` & `stactools-0.4.6/src/stactools/core/projection.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/core/utils/__init__.py` & `stactools-0.4.6/src/stactools/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/core/utils/convert.py` & `stactools-0.4.6/src/stactools/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/core/utils/raster_footprint.py` & `stactools-0.4.6/src/stactools/core/utils/raster_footprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import rasterio.features
 from pystac import Item
 from rasterio import Affine, DatasetReader
 from rasterio.crs import CRS
 from rasterio.warp import transform_geom
 from shapely.geometry import mapping, shape
 from shapely.geometry.multipolygon import MultiPolygon
-from shapely.geometry.polygon import Polygon
+from shapely.geometry.polygon import Polygon, orient
 
 logger = logging.getLogger(__name__)
 
 # Roughly 1 centimeter in geodetic coordinates
 DEFAULT_PRECISION = 7
 
 T = TypeVar("T", bound="RasterFootprint")
@@ -45,19 +45,18 @@
 
     Returns:
         List[Tuple[float, float]]: A list of the densified points.
     """  # noqa: E501
     points: Any = np.asarray(point_list)
     densified_number = len(points) * factor
     existing_indices = np.arange(0, densified_number, factor)
-    interp_indices = np.arange(existing_indices[-1])
+    interp_indices = np.arange(existing_indices[-1] + 1)
     interp_x = np.interp(interp_indices, existing_indices, points[:, 0])
     interp_y = np.interp(interp_indices, existing_indices, points[:, 1])
-    densified_points = [(x, y) for x, y in zip(interp_x, interp_y)]
-    return densified_points
+    return [(x, y) for x, y in zip(interp_x, interp_y)]
 
 
 def densify_by_distance(
     point_list: List[Tuple[float, float]], distance: float
 ) -> List[Tuple[float, float]]:
     """Densifies the number of points in a list of points by inserting new
     points at intervals between each set of successive points. For example, if
@@ -77,22 +76,25 @@
 
     Returns:
         List[Tuple[float, float]]: A list of the densified points.
     """
     points: Any = np.asarray(point_list)
     dxdy = points[1:, :] - points[:-1, :]
     segment_lengths = np.sqrt(np.sum(np.square(dxdy), axis=1))
-    total_length = np.sum(segment_lengths)
-    cum_segment_lengths = np.cumsum(segment_lengths)
-    cum_segment_lengths = np.insert(cum_segment_lengths, 0, [0])
-    cum_interp_lengths = np.arange(0, total_length, distance)
-    cum_interp_lengths = np.append(cum_interp_lengths, [total_length])
-    interp_x = np.interp(cum_interp_lengths, cum_segment_lengths, points[:, 0])
-    interp_y = np.interp(cum_interp_lengths, cum_segment_lengths, points[:, 1])
-    return [(x, y) for x, y in zip(interp_x, interp_y)]
+    steps = segment_lengths / distance
+    coordinate_steps = dxdy / steps.reshape(-1, 1)
+    densified_points = np.empty((len(point_list) - 1,), dtype="O")
+    for index in range(len(point_list) - 1):
+        step = np.arange(steps[index])
+        densified_points[index] = (
+            np.array((step, step)).T * coordinate_steps[index] + points[index]
+        )
+    final_point = points[-1].reshape(1, -1)
+    densified_array = np.concatenate((*densified_points, final_point), axis=0)
+    return [(float(row[0]), float(row[1])) for row in densified_array]
 
 
 def reproject_polygon(
     polygon: Polygon, crs: CRS, precision: Optional[int] = DEFAULT_PRECISION
 ) -> Polygon:
     """Projects a polygon to EPSG 4326 and rounds the projected vertex
     coordinates to ``precision``.
@@ -286,15 +288,15 @@
         if not data_polygons:
             return None
         elif len(data_polygons) == 1:
             polygon = data_polygons[0]
         else:
             polygon = MultiPolygon(data_polygons).convex_hull
 
-        return polygon
+        return orient(polygon)
 
     def densify_polygon(self, polygon: Polygon) -> Polygon:
         """Adds vertices to the footprint polygon in the native CRS using
         either ``self.densification_factor`` or
         ``self.densification_distance``.
 
         Args:
@@ -339,16 +341,18 @@
         Args:
             polygon (Polygon): Polygon to be simplified.
 
         Returns:
             Polygon: Reduced vertex polygon.
         """
         if self.simplify_tolerance is not None:
-            return polygon.simplify(
-                tolerance=self.simplify_tolerance, preserve_topology=False
+            return orient(
+                polygon.simplify(
+                    tolerance=self.simplify_tolerance, preserve_topology=False
+                )
             )
         return polygon
 
     @classmethod
     def from_href(
         cls: Type[T],
         href: str,
@@ -498,14 +502,16 @@
         no_data: Optional[Union[int, float]] = None,
         bands: List[int] = [1],
         skip_errors: bool = True,
     ) -> bool:
         """Accepts an Item and an optional list of asset names within that
         Item, and updates the geometry of that Item in-place with the data
         footprint derived from the first of the assets that exists in the Item.
+        The Item bbox is also updated in-place to bound the new footprint
+        extents.
 
         See :class:`RasterFootprint` for details on the data footprint
         calculation.
 
         Args:
             item (Item): The PySTAC Item to update.
             asset_names (List[str]): The names of the assets for which to attempt to
@@ -557,14 +563,15 @@
                 skip_errors=skip_errors,
             ),
             None,
         )
         if asset_name_and_extent is not None:
             _, extent = asset_name_and_extent
             item.geometry = extent
+            item.bbox = list(shape(extent).bounds)
             return True
         else:
             return False
 
     @classmethod
     def data_footprints_for_data_assets(
         cls,
@@ -672,15 +679,16 @@
 
     .. deprecated:: 0.4.4
         Use :meth:`RasterFootprint.update_geometry_from_asset_footprint`
         instead.
 
     Accepts an Item and an optional list of asset names within that Item, and
     updates the geometry of that Item in-place with the data footprint derived
-    from the first of the assets that exists in the Item.
+    from the first of the assets that exists in the Item. The Item bbox is also
+    updated in-place to bound the new footprint extents.
 
     See :class:`RasterFootprint` for details on the data footprint
     calculation.
 
     Args:
         item (Item): The PySTAC Item to update.
         asset_names (List[str]): The names of the assets for which to attempt to
```

### Comparing `stactools-0.4.5/src/stactools/core/utils/round.py` & `stactools-0.4.6/src/stactools/core/utils/round.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/core/utils/subprocess.py` & `stactools-0.4.6/src/stactools/core/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/testing/cli.py` & `stactools-0.4.6/src/stactools/testing/cli.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/testing/cli_test.py` & `stactools-0.4.6/src/stactools/testing/cli_test.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools/testing/test_data.py` & `stactools-0.4.6/src/stactools/testing/test_data.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.5/src/stactools.egg-info/PKG-INFO` & `stactools-0.4.6/src/stactools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools
-Version: 0.4.5
+Version: 0.4.6
 Summary: Command line tool and Python library for working with STAC
 Home-page: https://github.com/stac-utils/stactools
 Author: stac-utils
 Author-email: stac@radiant.earth
 Project-URL: Documentation, https://stactools.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/stac-utils/stactools/issues
 Keywords: stactools,pystac,imagery,raster,catalog,STAC
```

### Comparing `stactools-0.4.5/src/stactools.egg-info/SOURCES.txt` & `stactools-0.4.6/src/stactools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

