# Comparing `tmp/exotx-0.6.1.tar.gz` & `tmp/exotx-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exotx-0.6.1.tar", last modified: Sun Feb 26 19:04:46 2023, max compression
+gzip compressed data, was "exotx-0.6.3.tar", last modified: Mon Apr 10 16:58:51 2023, max compression
```

## Comparing `exotx-0.6.1.tar` & `exotx-0.6.3.tar`

### file list

```diff
@@ -1,58 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:04:46.940189 exotx-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-02-26 19:04:46.940189 exotx-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-02-26 19:04:36.000000 exotx-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:04:46.932189 exotx-0.6.1/exotx/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:04:46.932189 exotx-0.6.1/exotx/data/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/data/marketdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:04:46.936189 exotx-0.6.1/exotx/data/static/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/data/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/data/static/calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/data/static/calendars.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/data/static/conventions.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/data/static/daycounters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/data/staticdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:04:46.936189 exotx-0.6.1/exotx/instruments/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/instruments/asian_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/instruments/autocallable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/instruments/average_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/instruments/barrier_option.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/instruments/instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/instruments/option_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/instruments/vanilla_option.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:04:46.936189 exotx-0.6.1/exotx/models/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/models/blackscholesmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/models/hestonmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:04:46.936189 exotx-0.6.1/exotx/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:04:46.936189 exotx-0.6.1/exotx/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/tests/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:04:46.936189 exotx-0.6.1/exotx/tests/data/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/tests/data/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/tests/data/static/test_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/tests/data/test_marketdata.py
--rw-r--r--   0 runner    (1001) docker     (123)    12408 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/tests/data/test_staticdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:04:46.940189 exotx-0.6.1/exotx/tests/instruments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/tests/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/tests/instruments/test_asian_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/tests/instruments/test_autocallable_bs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/tests/instruments/test_autocallable_heston.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/tests/instruments/test_barrier_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/tests/instruments/test_vanilla_option.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:04:46.940189 exotx-0.6.1/exotx/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-02-26 19:04:36.000000 exotx-0.6.1/exotx/tests/models/test_hestonmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:04:46.932189 exotx-0.6.1/exotx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-02-26 19:04:46.000000 exotx-0.6.1/exotx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-02-26 19:04:46.000000 exotx-0.6.1/exotx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-26 19:04:46.000000 exotx-0.6.1/exotx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-26 19:04:46.000000 exotx-0.6.1/exotx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-26 19:04:46.000000 exotx-0.6.1/exotx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-26 19:04:36.000000 exotx-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-26 19:04:46.940189 exotx-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-02-26 19:04:36.000000 exotx-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:51.049523 exotx-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-10 16:58:51.049523 exotx-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-10 16:58:40.000000 exotx-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:51.041523 exotx-0.6.3/exotx/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:51.045524 exotx-0.6.3/exotx/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/data/marketdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:51.045524 exotx-0.6.3/exotx/data/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/data/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/data/static/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/data/static/calendars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/data/static/conventions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/data/static/daycounters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/data/staticdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:51.045524 exotx-0.6.3/exotx/instruments/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/instruments/asian_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/instruments/autocallable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/instruments/average_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/instruments/average_convention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/instruments/average_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/instruments/barrier_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/instruments/basket_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/instruments/basket_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/instruments/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/instruments/option_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/instruments/vanilla_option.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:51.045524 exotx-0.6.3/exotx/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/models/blackscholesmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/models/hestonmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:51.045524 exotx-0.6.3/exotx/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:51.045524 exotx-0.6.3/exotx/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:51.045524 exotx-0.6.3/exotx/tests/data/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/data/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/data/static/test_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/data/test_marketdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/data/test_staticdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:51.049523 exotx-0.6.3/exotx/tests/instruments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/instruments/test_asian_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/instruments/test_autocallable_bs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/instruments/test_autocallable_heston.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/instruments/test_barrier_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/instruments/test_basket_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/instruments/test_vanilla_option.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:51.049523 exotx-0.6.3/exotx/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/models/test_hestonmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:51.045524 exotx-0.6.3/exotx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-10 16:58:51.000000 exotx-0.6.3/exotx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-10 16:58:51.000000 exotx-0.6.3/exotx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:58:51.000000 exotx-0.6.3/exotx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 16:58:51.000000 exotx-0.6.3/exotx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 16:58:51.000000 exotx-0.6.3/exotx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-10 16:58:40.000000 exotx-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-10 16:58:51.049523 exotx-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-10 16:58:40.000000 exotx-0.6.3/setup.py
```

### Comparing `exotx-0.6.1/PKG-INFO` & `exotx-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exotx
-Version: 0.6.1
+Version: 0.6.3
 Summary: Python library for pricing autocallables
 Home-page: https://github.com/SebastienEveno/exotx
 Author: Sebastien Eveno
 Author-email: sebastien.louis.eveno@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -16,98 +16,113 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.10.2, <4
 Description-Content-Type: text/markdown
 
 # exotx
+
 <p align="center">
     <img src="https://github.com/SebastienEveno/exotx/actions/workflows/python-package.yml/badge.svg?branch=master" />
     <a href="https://pypi.org/project/exotx" alt="Python Versions">
         <img src="https://img.shields.io/pypi/pyversions/exotx.svg?logo=python&logoColor=white" /></a>
     <a href="https://pypi.org/project/exotx" alt="PyPi">
         <img src="https://img.shields.io/pypi/v/exotx" /></a>
     <a href="https://pepy.tech/project/exotx" alt="Downloads">
         <img src="https://pepy.tech/badge/exotx" /></a>
 </p>
 
-exotx is a Python wrapper for the [QuantLib library](https://www.quantlib.org/), a powerful open-source library for quantitative finance. exotx provides a simple and user-friendly interface for pricing and analyzing financial derivatives using QuantLib's advanced numerical methods.
+exotx is a Python wrapper for the [QuantLib library](https://www.quantlib.org/), a powerful open-source library for
+quantitative finance. exotx provides a simple and user-friendly interface for pricing and analyzing financial
+derivatives using QuantLib's advanced numerical methods.
 
 ## Installation
 
 To install exotx, simply use pip:
+
 ```sh
 pip install exotx
 ```
 
 ## Usage
 
 ### Define the product
+
 ```python
 import exotx
 
 notional = 100
 strike = 100.0
 autocall_barrier_level = 1.0  # 100%
 annual_coupon_value = 0.03  # 3.00%
 coupon_barrier_level = 0.75  # 75%
 protection_barrier_level = 0.75  # 75%
 
 my_autocallable = exotx.Autocallable(notional, strike, autocall_barrier_level, annual_coupon_value, coupon_barrier_level, protection_barrier_level)
 ```
 
 ### Define the static data
+
 The object that represents static data such as the calendar, the day counter or the business day convention used.
 
 #### From the constructor
+
 ```python
 my_static_data = exotx.StaticData(day_counter='Actual360', business_day_convention='ModifiedFollowing')
 ```
 
 #### From JSON
+
 ```python
 my_json = {
     'day_counter': 'Actual360',
     'business_day_convention': 'ModifiedFollowing'
 }
 my_static_data = exotx.StaticData.from_json(my_json)
 ```
 
 ### Define the market data
+
 #### From the constructor
+
 ```python
 reference_date = '2015-11-06'
 spot = 100.0
 risk_free_rate = 0.01
 dividend_rate = 0.0
 black_scholes_volatility = 0.2
 
 my_market_data = exotx.MarketData(reference_date, spot, risk_free_rate, dividend_rate, black_scholes_volatility=black_scholes_volatility)
 ```
+
 #### From JSON
+
 ```python
 my_json = {
     'reference_date': '2015-11-06',
     'spot': 100,
     'risk_free_rate': 0.01,
     'dividend_rate': 0,
     'black_scholes_volatility': 0.2
 }
 my_market_data = exotx.MarketData.from_json(my_json)
 ```
 
 ### Price the product
+
 ```python
 exotx.price(my_autocallable, my_market_data, my_static_data, model='black-scholes')
 ```
+
 ```plaintext
 96.08517973497098
 ```
 
 ## Contributing
 
-We welcome contributions to exotx! If you find a bug or would like to request a new feature, please open an issue on the [Github repository](https://github.com/sebastieneveno/exotx). 
+We welcome contributions to exotx! If you find a bug or would like to request a new feature, please open an issue on
+the [Github repository](https://github.com/sebastieneveno/exotx).
 If you would like to contribute code, please submit a pull request.
 
 ## License
 
 exotx is released under the [MIT License](https://opensource.org/licenses/MIT).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: exotx Version: 0.6.1 Summary: Python library for
+Metadata-Version: 2.1 Name: exotx Version: 0.6.3 Summary: Python library for
 pricing autocallables Home-page: https://github.com/SebastienEveno/exotx
 Author: Sebastien Eveno Author-email: sebastien.louis.eveno@gmail.com License:
 MIT Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.10 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research Classifier: Topic :: Software
```

### Comparing `exotx-0.6.1/README.md` & `exotx-0.6.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,92 +1,107 @@
 # exotx
+
 <p align="center">
     <img src="https://github.com/SebastienEveno/exotx/actions/workflows/python-package.yml/badge.svg?branch=master" />
     <a href="https://pypi.org/project/exotx" alt="Python Versions">
         <img src="https://img.shields.io/pypi/pyversions/exotx.svg?logo=python&logoColor=white" /></a>
     <a href="https://pypi.org/project/exotx" alt="PyPi">
         <img src="https://img.shields.io/pypi/v/exotx" /></a>
     <a href="https://pepy.tech/project/exotx" alt="Downloads">
         <img src="https://pepy.tech/badge/exotx" /></a>
 </p>
 
-exotx is a Python wrapper for the [QuantLib library](https://www.quantlib.org/), a powerful open-source library for quantitative finance. exotx provides a simple and user-friendly interface for pricing and analyzing financial derivatives using QuantLib's advanced numerical methods.
+exotx is a Python wrapper for the [QuantLib library](https://www.quantlib.org/), a powerful open-source library for
+quantitative finance. exotx provides a simple and user-friendly interface for pricing and analyzing financial
+derivatives using QuantLib's advanced numerical methods.
 
 ## Installation
 
 To install exotx, simply use pip:
+
 ```sh
 pip install exotx
 ```
 
 ## Usage
 
 ### Define the product
+
 ```python
 import exotx
 
 notional = 100
 strike = 100.0
 autocall_barrier_level = 1.0  # 100%
 annual_coupon_value = 0.03  # 3.00%
 coupon_barrier_level = 0.75  # 75%
 protection_barrier_level = 0.75  # 75%
 
 my_autocallable = exotx.Autocallable(notional, strike, autocall_barrier_level, annual_coupon_value, coupon_barrier_level, protection_barrier_level)
 ```
 
 ### Define the static data
+
 The object that represents static data such as the calendar, the day counter or the business day convention used.
 
 #### From the constructor
+
 ```python
 my_static_data = exotx.StaticData(day_counter='Actual360', business_day_convention='ModifiedFollowing')
 ```
 
 #### From JSON
+
 ```python
 my_json = {
     'day_counter': 'Actual360',
     'business_day_convention': 'ModifiedFollowing'
 }
 my_static_data = exotx.StaticData.from_json(my_json)
 ```
 
 ### Define the market data
+
 #### From the constructor
+
 ```python
 reference_date = '2015-11-06'
 spot = 100.0
 risk_free_rate = 0.01
 dividend_rate = 0.0
 black_scholes_volatility = 0.2
 
 my_market_data = exotx.MarketData(reference_date, spot, risk_free_rate, dividend_rate, black_scholes_volatility=black_scholes_volatility)
 ```
+
 #### From JSON
+
 ```python
 my_json = {
     'reference_date': '2015-11-06',
     'spot': 100,
     'risk_free_rate': 0.01,
     'dividend_rate': 0,
     'black_scholes_volatility': 0.2
 }
 my_market_data = exotx.MarketData.from_json(my_json)
 ```
 
 ### Price the product
+
 ```python
 exotx.price(my_autocallable, my_market_data, my_static_data, model='black-scholes')
 ```
+
 ```plaintext
 96.08517973497098
 ```
 
 ## Contributing
 
-We welcome contributions to exotx! If you find a bug or would like to request a new feature, please open an issue on the [Github repository](https://github.com/sebastieneveno/exotx). 
+We welcome contributions to exotx! If you find a bug or would like to request a new feature, please open an issue on
+the [Github repository](https://github.com/sebastieneveno/exotx).
 If you would like to contribute code, please submit a pull request.
 
 ## License
 
 exotx is released under the [MIT License](https://opensource.org/licenses/MIT).
```

### Comparing `exotx-0.6.1/exotx/data/marketdata.py` & `exotx-0.6.3/exotx/data/marketdata.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,110 +1,147 @@
 import json
-import QuantLib as ql
 from datetime import datetime
 from typing import List, Union
+
+import QuantLib as ql
 from marshmallow import Schema, fields, post_load
 
 
 class MarketData:
 
     def __init__(self,
-                 spot: float,
+                 underlying_spots: List[float],
                  risk_free_rate: float,
                  dividend_rate: float,
                  reference_date: Union[datetime, str, None] = None,
                  expiration_dates: List[Union[datetime, str]] = None,
                  strikes: List[float] = None,
                  data: List[List[float]] = None,
-                 black_scholes_volatility: float = None) -> None:
+                 underlying_black_scholes_volatilities: List[float] = None,
+                 correlation_matrix: List[List[float]] = None) -> None:
         # set the reference date
         self._set_reference_date(reference_date)
 
-        # set the underlying spot value
-        self._set_underlying_spot(spot)
+        # set underlying spot values
+        self._set_underlying_spots(underlying_spots)
 
         # set market rate curves
         self._set_rate_curves(dividend_rate, risk_free_rate)
 
         # set the volatility surface
-        self._set_volatility_surface(black_scholes_volatility, data, expiration_dates, strikes)
+        self._set_volatility_surface(underlying_black_scholes_volatilities, data, expiration_dates, strikes)
+
+        # set the correlation matrix
+        self._set_correlation_matrix(correlation_matrix)
+
+    # region setters
 
     # TODO: Have a proper rate curves stripper service
-    def _set_rate_curves(self, dividend_rate, risk_free_rate):
+    def _set_rate_curves(self, dividend_rate, risk_free_rate) -> None:
         self.risk_free_rate = risk_free_rate
         self.dividend_rate = dividend_rate
 
     # TODO: Allow for multiple volatility surfaces for each underlying
-    def _set_volatility_surface(self, black_scholes_volatility, data, expiration_dates, strikes):
+    def _set_volatility_surface(self, underlying_black_scholes_volatilities: List[float], data, expiration_dates,
+                                strikes) -> None:
         self.expiration_dates: List[datetime] = []
         if not expiration_dates:
             self.expiration_dates = None
         else:
             for expiration_date in expiration_dates:
                 if isinstance(expiration_date, str):
                     self.expiration_dates.append(datetime.strptime(expiration_date, '%Y-%m-%d'))
                 elif isinstance(expiration_date, datetime):
                     self.expiration_dates.append(expiration_date)
         self.strikes = strikes
         self.data = data
-        self.black_scholes_volatility = black_scholes_volatility
 
-    # TODO: Allow for multiple underlying spots to be defined, may need a proper container class
-    def _set_underlying_spot(self, spot):
-        assert spot > 0
-        self.spot = spot
+        if underlying_black_scholes_volatilities:
+            for vol in underlying_black_scholes_volatilities:
+                assert vol >= 0, f"Invalid volatility: {vol}"
+        self.underlying_black_scholes_volatilities = underlying_black_scholes_volatilities  # set to None if it does not exist, OK
+
+    # TODO: Allow for multiple underlying spots to be defined, may need a proper container class or a dict
+    def _set_underlying_spots(self, underlying_spots: List[float]) -> None:
+        for underlying_spot in underlying_spots:
+            assert underlying_spot > 0, f"Invalid underlying spot {underlying_spot}"
+        self.underlying_spots = underlying_spots
 
-    def _set_reference_date(self, reference_date: Union[datetime, str, None]):
+    def _set_reference_date(self, reference_date: Union[datetime, str, None]) -> None:
         if isinstance(reference_date, str):
             reference_date = datetime.strptime(reference_date, '%Y-%m-%d')
         elif isinstance(reference_date, datetime):
             pass
         else:
             # defaults to today's date
             reference_date = datetime.today()
         self.reference_date: datetime = reference_date
 
+    def _set_correlation_matrix(self, correlation_matrix: Union[List[List[float]], None]) -> None:
+        if correlation_matrix:
+            for rows in correlation_matrix:
+                for rho in rows:
+                    assert 1 >= rho >= -1, "Invalid correlation matrix"
+        self.correlation_matrix = correlation_matrix
+
+    # endregion
+
+    # region getters
     def get_ql_reference_date(self) -> ql.Date:
         return ql.Date().from_date(self.reference_date)
 
+    def get_correlation_matrix(self) -> ql.Matrix:
+        matrix = ql.Matrix(len(self.correlation_matrix), len(self.correlation_matrix))
+        for i in range(len(self.correlation_matrix)):
+            matrix[i][i] = 1.0
+            for j in range(i + 1, len(self.correlation_matrix)):
+                matrix[i][j] = self.correlation_matrix[i][j]
+                matrix[j][i] = self.correlation_matrix[i][j]
+        return matrix
+
     # TODO: Get these from a proper rate curve stripper service
     def get_yield_curve(self, day_counter) -> ql.YieldTermStructureHandle:
         flat_forward = ql.FlatForward(self.get_ql_reference_date(), self.risk_free_rate, day_counter)
         return ql.YieldTermStructureHandle(flat_forward)
 
     def get_dividend_curve(self, day_counter) -> ql.YieldTermStructureHandle:
         flat_forward = ql.FlatForward(self.get_ql_reference_date(), self.dividend_rate, day_counter)
         return ql.YieldTermStructureHandle(flat_forward)
 
+    # endregion
+
+    # region serialization/deserialization
     @classmethod
     def from_json(cls, data: dict):
         schema = MarketDataSchema()
         return schema.load(data)
 
     def to_json(self, format_type: str = "dict"):
         schema = MarketDataSchema()
         my_json = schema.dump(self)
         if format_type == "dict":
             return my_json
         elif format_type == "str":
             return json.dumps(my_json)
         else:
-            raise NotImplemented(f"Invalid format type {format_type} when dumping")
+            raise NotImplementedError(f"Invalid format type {format_type} when dumping")
+    # endregion
 
 
 # region Schema
 
 class MarketDataSchema(Schema):
-    spot = fields.Float(required=True)
+    underlying_spots = fields.List(fields.Float(required=True))
     risk_free_rate = fields.Float(required=True)
     dividend_rate = fields.Float(required=True)
     reference_date = fields.DateTime(format='%Y-%m-%d', allow_none=True)
     expiration_dates = fields.List(fields.DateTime(format='%Y-%m-%d'), allow_none=True)
     strikes = fields.List(fields.Float(), allow_none=True)
     data = fields.List(fields.List(fields.Float), allow_none=True)
-    black_scholes_volatility = fields.Float(allow_none=True)
+    underlying_black_scholes_volatilities = fields.List(fields.Float(allow_none=True))
+    correlation_matrix = fields.List(fields.List(fields.Float()))
 
     @post_load
     def make_market_data(self, data, **kwargs) -> MarketData:
         return MarketData(**data)
 
 # endregion
```

### Comparing `exotx-0.6.1/exotx/data/static/__init__.py` & `exotx-0.6.3/exotx/data/static/__init__.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from exotx.data.static.daycounters import day_counters_to_ql, DayCounter
+from exotx.data.static.calendar import Calendar
 from exotx.data.static.calendars import calendars_to_ql_calendars, CalendarRegion, CalendarMarket, region_to_markets, \
     available_regions
-from exotx.data.static.calendar import Calendar
 from exotx.data.static.conventions import compoundings, frequencies, business_day_conventions_to_ql, \
     BusinessDayConvention
+from exotx.data.static.daycounters import day_counters_to_ql, DayCounter
 
 __all__ = [
     'calendars_to_ql_calendars',
     'day_counters_to_ql',
     'compoundings',
     'frequencies',
     'business_day_conventions_to_ql',
```

### Comparing `exotx-0.6.1/exotx/data/static/calendar.py` & `exotx-0.6.3/exotx/data/static/calendar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Union, Tuple
+
 from marshmallow import Schema, fields, post_load, validates_schema
+
 from exotx.data.static.calendars import CalendarRegion, CalendarMarket, region_to_markets, available_regions
 
 
 class Calendar:
     def __init__(self,
                  region: Union[CalendarRegion, str, None] = None,
                  market: Union[CalendarMarket, str, None] = None):
```

### Comparing `exotx-0.6.1/exotx/data/static/calendars.py` & `exotx-0.6.3/exotx/data/static/calendars.py`

 * *Files identical despite different names*

### Comparing `exotx-0.6.1/exotx/data/static/conventions.py` & `exotx-0.6.3/exotx/data/static/conventions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import enum
+
 import QuantLib as ql
 
 
 # based on https://quantlib-python-docs.readthedocs.io/en/latest/dates.html#conventions
 
 
 # region Compounding
```

### Comparing `exotx-0.6.1/exotx/data/static/daycounters.py` & `exotx-0.6.3/exotx/data/static/daycounters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import enum
+
 import QuantLib as ql
 
 
 # based on https://quantlib-python-docs.readthedocs.io/en/latest/dates.html#daycounter
 
 
 class DayCounter(enum.Enum):
```

### Comparing `exotx-0.6.1/exotx/data/staticdata.py` & `exotx-0.6.3/exotx/data/staticdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import json
-import QuantLib as ql
 from typing import Union
-from exotx.data.static.daycounters import day_counters_to_ql, DayCounter
+
+import QuantLib as ql
+from marshmallow import Schema, fields, post_load, ValidationError
+
 from exotx.data.static.calendar import Calendar, CalendarSchema
 from exotx.data.static.calendars import calendars_to_ql_calendars
 from exotx.data.static.conventions import business_day_conventions_to_ql, BusinessDayConvention
-from marshmallow import Schema, fields, post_load, ValidationError
+from exotx.data.static.daycounters import day_counters_to_ql, DayCounter
 
 
 class StaticData:
     def __init__(self,
                  day_counter: Union[DayCounter, str, None] = None,
                  business_day_convention: Union[BusinessDayConvention, str, None] = None,
                  calendar: Union[Calendar, dict, None] = None) -> None:
@@ -125,15 +127,15 @@
         schema = StaticDataSchema()
         my_json = schema.dump(self)
         if format_type == "dict":
             return my_json
         elif format_type == "str":
             return json.dumps(my_json)
         else:
-            raise NotImplemented(f"Invalid format type {format_type} when dumping")
+            raise NotImplementedError(f"Invalid format type {format_type} when dumping")
 
 
 # region Schema
 
 class BusinessDayConventionField(fields.Field):
     def _serialize(self, value: BusinessDayConvention, attr, obj, **kwargs) -> str:
         return value.name
```

### Comparing `exotx-0.6.1/exotx/instruments/asian_option.py` & `exotx-0.6.3/exotx/instruments/asian_option.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,39 @@
 from datetime import datetime
-from enum import Enum
 from typing import Union, List
 
 import QuantLib as ql
-from marshmallow import Schema, fields, post_load, ValidationError
+from marshmallow import Schema, fields, post_load
 
 from exotx.enums.enums import PricingModel, NumericalMethod
 from exotx.helpers.dates import convert_maturity_to_ql_date
+from exotx.instruments.average_calculation import AverageCalculation, convert_average_calculation, \
+    AverageCalculationField
+from exotx.instruments.average_convention import AverageConvention, convert_average_convention, AverageConventionField
 from exotx.instruments.average_type import AverageTypeField, AverageType, convert_average_type_to_ql
 from exotx.instruments.instrument import Instrument
 from exotx.instruments.option_type import convert_option_type_to_ql, OptionType, OptionTypeField
 from exotx.models.blackscholesmodel import BlackScholesModel
 from exotx.utils.pricing_configuration import PricingConfiguration
 
 
-class AverageCalculation(Enum):
-    CONTINUOUS = 'continuous'
-    DISCRETE = 'discrete'
-
-
-class AverageCalculationField(fields.Field):
-    def _serialize(self, value: AverageCalculation, attr, obj, **kwargs) -> str:
-        return value.name
-
-    def _deserialize(self, value: str, attr, data, **kwargs) -> AverageCalculation:
-        try:
-            return AverageCalculation[value]
-        except KeyError as error:
-            raise ValidationError(
-                f"Invalid average calculation \"{value}\", expected one of {list(AverageCalculation.__members__.keys())}") from error
-
-
 class AsianOption(Instrument):
     def __init__(self,
                  strike: float, maturity: Union[str, datetime], option_type: Union[str, OptionType],
                  average_type: Union[str, AverageType], average_calculation: Union[str, AverageCalculation],
-                 arithmetic_running_accumulator: float = 0.0, geometric_running_accumulator: float = 1.0,
-                 past_fixings: int = 0, future_fixing_dates: List[datetime] = None):
+                 average_convention: Union[str, AverageConvention], arithmetic_running_accumulator: float = 0.0,
+                 geometric_running_accumulator: float = 1.0, past_fixings: int = 0,
+                 future_fixing_dates: List[datetime] = None):
         assert strike >= 0, "Invalid strike: cannot be negative"
         self.strike = strike
         self.maturity = convert_maturity_to_ql_date(maturity)
         self.option_type = convert_option_type_to_ql(option_type)
         self.average_type = convert_average_type_to_ql(average_type)
-        self.average_calculation: AverageCalculation = average_calculation
+        self.average_calculation: AverageCalculation = convert_average_calculation(average_calculation)
+        self.average_convention: AverageConvention = convert_average_convention(average_convention)
         self.arithmetic_running_accumulator = arithmetic_running_accumulator
         self.geometric_running_accumulator = geometric_running_accumulator
         self.past_fixings = past_fixings
         self.future_fixing_dates = None if not future_fixing_dates else [ql.Date().from_date(future_fixing_date)
                                                                          for future_fixing_date in future_fixing_dates]
 
     def price(self, market_data, static_data, pricing_config: PricingConfiguration, seed: int = 1) -> dict:
@@ -95,30 +82,48 @@
     def _get_ql_pricing_engine(self, market_data, static_data, pricing_config: PricingConfiguration, seed: int):
         if self.average_calculation == AverageCalculation.DISCRETE:
             if self.average_type == ql.Average().Geometric:
                 if pricing_config.numerical_method == NumericalMethod.ANALYTIC:
                     # TODO: filter on pricing_config.pricing_model, here we assume black-scholes only
                     bs_model = BlackScholesModel(market_data, static_data)
                     process = bs_model.setup()
-                    return ql.AnalyticDiscreteGeometricAveragePriceAsianEngine(process)
+                    if self.average_convention == AverageConvention.PRICE:
+                        return ql.AnalyticDiscreteGeometricAveragePriceAsianEngine(process)
+                    elif self.average_convention == AverageConvention.STRIKE:
+                        return ql.AnalyticDiscreteGeometricAverageStrikeAsianEngine(process)
+                    else:
+                        raise ValueError(f"Invalid average convention \"{self.average_convention}\"")
                 elif pricing_config.numerical_method == NumericalMethod.MC:
                     # TODO: filter on pricing_config.pricing_model, here we assume black-scholes only
                     bs_model = BlackScholesModel(market_data, static_data)
                     process = bs_model.setup()
-                    # TODO: get the traits parameter (lowdiscrepancy) from the pricing configuration
-                    return ql.MCDiscreteGeometricAPEngine(process, "lowdiscrepancy")
+                    random_number_generator = str(pricing_config.random_number_generator)
+                    if self.average_convention == AverageConvention.PRICE:
+                        return ql.MCDiscreteGeometricAPEngine(process, random_number_generator)
+                    elif self.average_convention == AverageConvention.STRIKE:
+                        return ValueError(
+                            f"No corresponding engine for asian option for numerical method {pricing_config.numerical_method}, "
+                            f"average type {self.average_type}, average calculation {self.average_calculation}, and average convention {self.average_convention}")
+                    else:
+                        raise ValueError(f"Invalid average convention \"{self.average_convention}\"")
                 else:
                     raise ValueError(
                         f"No engine for asian option with numerical method {pricing_config.numerical_method}"
                         f"with average calculation {self.average_calculation} and average type {self.average_type}")
             elif self.average_type == ql.Average().Arithmetic:
                 if pricing_config.numerical_method == NumericalMethod.MC:
                     bs_model = BlackScholesModel(market_data, static_data)
                     process = bs_model.setup()
-                    return ql.MCDiscreteArithmeticAPEngine(process, "lowdiscrepancy")
+                    random_number_generator = str(pricing_config.random_number_generator)
+                    if self.average_convention == AverageConvention.PRICE:
+                        return ql.MCDiscreteArithmeticAPEngine(process, random_number_generator)
+                    elif self.average_convention == AverageConvention.STRIKE:
+                        return ql.MCDiscreteArithmeticASEngine(process, random_number_generator)
+                    else:
+                        raise ValueError(f"Invalid average convention \"{self.average_convention}\"")
             else:
                 raise ValueError(f"Invalid average type {self.average_type}")
         elif self.average_calculation == AverageCalculation.CONTINUOUS:
             if self.average_type == ql.Average().Geometric:
                 if pricing_config.numerical_method == NumericalMethod.ANALYTIC:
                     # TODO: filter on pricing_config.pricing_model, here we assume black-scholes only
                     bs_model = BlackScholesModel(market_data, static_data)
@@ -142,17 +147,20 @@
     def from_json(cls, json_data):
         schema = AsianOptionSchema()
         data = schema.load(json_data)
         return cls(**data)
     # endregion
 
 
+# region Schema
 class AsianOptionSchema(Schema):
     strike = fields.Float()
     maturity = fields.Date(format="%Y-%m-%d")
-    option_type = OptionTypeField(allow_none=False)
-    average_type = AverageTypeField(allow_none=False)
-    average_calculation = AverageCalculationField(allow_none=False)
+    option_type = OptionTypeField()
+    average_type = AverageTypeField()
+    average_calculation = AverageCalculationField()
+    average_convention = AverageConventionField()
 
     @post_load
     def make_asian_option(self, data, **kwargs) -> AsianOption:
         return AsianOption(**data)
+# endregion
```

### Comparing `exotx-0.6.1/exotx/instruments/autocallable.py` & `exotx-0.6.3/exotx/instruments/autocallable.py`

 * *Files identical despite different names*

### Comparing `exotx-0.6.1/exotx/instruments/average_type.py` & `exotx-0.6.3/exotx/instruments/average_type.py`

 * *Files identical despite different names*

### Comparing `exotx-0.6.1/exotx/instruments/barrier_option.py` & `exotx-0.6.3/exotx/instruments/barrier_option.py`

 * *Files identical despite different names*

### Comparing `exotx-0.6.1/exotx/instruments/option_type.py` & `exotx-0.6.3/exotx/instruments/option_type.py`

 * *Files identical despite different names*

### Comparing `exotx-0.6.1/exotx/instruments/vanilla_option.py` & `exotx-0.6.3/exotx/instruments/vanilla_option.py`

 * *Files identical despite different names*

### Comparing `exotx-0.6.1/exotx/models/blackscholesmodel.py` & `exotx-0.6.3/exotx/models/blackscholesmodel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import QuantLib as ql
 import numpy as np
+
 from exotx.data.marketdata import MarketData
 from exotx.data.staticdata import StaticData
 
 
 class BlackScholesModel:
     """Class for the Black-Scholes model."""
 
@@ -13,21 +14,21 @@
         self._reference_date: ql.Date = market_data.get_ql_reference_date()
         self.market_data = market_data
         # set static data
         self._calendar: ql.Calendar = static_data.get_ql_calendar()
         self._day_counter: ql.DayCounter = static_data.get_ql_day_counter()
 
     def setup(self) -> ql.BlackScholesMertonProcess:
-        spot_handle = ql.QuoteHandle(ql.SimpleQuote(self.market_data.spot))
+        spot_handle = ql.QuoteHandle(ql.SimpleQuote(self.market_data.underlying_spots[0]))
         flat_ts = self.market_data.get_yield_curve(self._day_counter)
         dividend_yield = self.market_data.get_dividend_curve(self._day_counter)
         flat_vol_ts = ql.BlackVolTermStructureHandle(
             ql.BlackConstantVol(self._reference_date,
                                 self._calendar,
-                                self.market_data.black_scholes_volatility,
+                                self.market_data.underlying_black_scholes_volatilities[0],
                                 self._day_counter)
         )
         return ql.BlackScholesMertonProcess(spot_handle, dividend_yield, flat_ts, flat_vol_ts)
 
     @staticmethod
     def generate_paths(dates,
                        day_counter: ql.DayCounter,
```

### Comparing `exotx-0.6.1/exotx/models/hestonmodel.py` & `exotx-0.6.3/exotx/models/hestonmodel.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from typing import List, Tuple
+
 import QuantLib as ql
 import numpy as np
 from scipy.optimize import differential_evolution
-from typing import List, Tuple
+
 from exotx.data.marketdata import MarketData
 from exotx.data.staticdata import StaticData
 
 
 class HestonModel:
     """Class for the Heston model."""
 
@@ -31,40 +33,39 @@
         helpers, grid_data = self._setup_helpers(ql_engine)
         cost_function = self._cost_function_generator(model, helpers, norm=True)
         differential_evolution(cost_function, self._bounds, seed=seed, maxiter=100)
         print('Calibrated Heston parameters:', model.params())
 
         return process, model
 
-    def _setup(self, initial_conditions: Tuple[float, ...] = None) -> Tuple[ql.HestonProcess,
-    ql.HestonModel]:
+    def _setup(self, initial_conditions: Tuple[float, ...] = None) -> Tuple[ql.HestonProcess, ql.HestonModel]:
         if initial_conditions:
             theta, kappa, sigma, rho, v0 = initial_conditions
         else:
             theta, kappa, sigma, rho, v0 = self._initial_conditions
 
         process = ql.HestonProcess(self.market_data.get_yield_curve(self._day_counter),
                                    self.market_data.get_dividend_curve(self._day_counter),
-                                   ql.QuoteHandle(ql.SimpleQuote(self.market_data.spot)),
+                                   ql.QuoteHandle(ql.SimpleQuote(self.market_data.underlying_spots[0])),
                                    v0, kappa, theta, sigma, rho)
         model = ql.HestonModel(process)
 
         return process, model
 
-    def _setup_helpers(self, engine: ql.PricingEngine) -> Tuple[List[ql.HestonModelHelper],
-    List[Tuple[ql.Date, float]]]:
+    def _setup_helpers(self, engine: ql.PricingEngine) -> Tuple[
+        List[ql.HestonModelHelper], List[Tuple[ql.Date, float]]]:
         helpers = []
         grid_data = []
         for i, date in enumerate([ql.Date().from_date(date) for date in self.market_data.expiration_dates]):
             for j, strike in enumerate(self.market_data.strikes):
                 t = (date - self._reference_date)
                 p = ql.Period(t, ql.Days)
                 vols = self.market_data.data[i][j]
                 helper = ql.HestonModelHelper(
-                    p, self._calendar, self.market_data.spot, strike,
+                    p, self._calendar, self.market_data.underlying_spots[0], strike,
                     ql.QuoteHandle(ql.SimpleQuote(vols)),
                     self.market_data.get_yield_curve(self._day_counter),
                     self.market_data.get_dividend_curve(self._day_counter))
                 helper.setPricingEngine(engine)
                 helpers.append(helper)
                 grid_data.append((date, strike))
```

### Comparing `exotx-0.6.1/exotx/tests/conftest.py` & `exotx-0.6.3/exotx/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from exotx.data.marketdata import MarketData
 from exotx.data.staticdata import StaticData
 
 
 # Arrange
 @pytest.fixture()
 def my_static_data() -> StaticData:
@@ -13,18 +14,18 @@
     return StaticData.from_json(my_json)
 
 
 @pytest.fixture()
 def my_market_data() -> MarketData:
     my_json = {
         'reference_date': '2015-11-06',
-        'spot': 100,
+        'underlying_spots': [100],
         'risk_free_rate': 0.08,
         'dividend_rate': 0.04,
-        'black_scholes_volatility': 0.25,
+        'underlying_black_scholes_volatilities': [0.25],
         'expiration_dates': [
             '2015-12-06', '2016-01-06', '2016-02-06', '2016-03-06', '2016-04-06', '2016-05-06',
             '2016-06-06', '2016-07-06', '2016-08-06', '2016-09-06', '2016-10-06', '2016-11-06',
             '2016-12-06', '2017-01-06', '2017-02-06', '2017-03-06', '2017-04-06', '2017-05-06',
             '2017-06-06', '2017-07-06', '2017-08-06', '2017-09-06', '2017-10-06', '2017-11-06'
         ],
         'strikes': [
```

### Comparing `exotx-0.6.1/exotx/tests/data/static/test_calendar.py` & `exotx-0.6.3/exotx/tests/data/static/test_calendar.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from typing import Optional, Union
+
 import pytest
+
 from exotx.data.static import Calendar, CalendarRegion, CalendarMarket
-from typing import Optional, Union
 
 
 # region from_json
 @pytest.mark.parametrize('region, market', [
     ('UnitedStates', 'NYSE'),
     (CalendarRegion.UnitedStates, CalendarMarket.NYSE),
     (CalendarRegion.UnitedStates, None)
```

### Comparing `exotx-0.6.1/exotx/tests/data/test_staticdata.py` & `exotx-0.6.3/exotx/tests/data/test_staticdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from typing import Optional, Union
+
 import QuantLib as ql
 import pytest
-from typing import Optional, Union
+
 from exotx.data import StaticData
 from exotx.data.static import Calendar, BusinessDayConvention, DayCounter
 
 
 # Arrange
 def my_default_day_counter_type() -> type:
     my_default_day_counter = StaticData.get_default_day_counter()
```

### Comparing `exotx-0.6.1/exotx/tests/instruments/test_autocallable_bs.py` & `exotx-0.6.3/exotx/tests/instruments/test_autocallable_bs.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 from exotx.instruments.autocallable import Autocallable
 
 
 # Arrange
 @pytest.fixture
 def my_market_data() -> MarketData:
     reference_date = '2015-11-06'
-    spot = 100.0
-    black_scholes_volatility = 0.2
+    underlying_spots = [100.0]
+    underlying_black_scholes_volatilities = [0.2]
     risk_free_rate = 0.01
     dividend_rate = 0.0
 
     return MarketData(reference_date=reference_date,
-                      spot=spot,
+                      underlying_spots=underlying_spots,
                       risk_free_rate=risk_free_rate,
                       dividend_rate=dividend_rate,
-                      black_scholes_volatility=black_scholes_volatility)
+                      underlying_black_scholes_volatilities=underlying_black_scholes_volatilities)
 
 
 @pytest.fixture
 def my_autocallable() -> Autocallable:
     notional = 100
     strike = 100
     autocall_barrier_level = 1.0
```

### Comparing `exotx-0.6.1/exotx/tests/instruments/test_autocallable_heston.py` & `exotx-0.6.3/exotx/tests/instruments/test_autocallable_heston.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from exotx.instruments.autocallable import Autocallable
 
 
 # Arrange
 @pytest.fixture
 def my_market_data() -> MarketData:
     reference_date = '2015-11-06'
-    spot = 100.0
+    underlying_spots = [100.0]
     risk_free_rate = 0.01
     dividend_rate = 0.0
     expiration_dates = ['2015-12-06', '2016-01-06', '2016-02-06', '2016-03-06', '2016-04-06',
                         '2016-05-06', '2016-06-06', '2016-07-06', '2016-08-06', '2016-09-06',
                         '2016-10-06', '2016-11-06', '2016-12-06', '2017-01-06', '2017-02-06',
                         '2017-03-06', '2017-04-06', '2017-05-06', '2017-06-06', '2017-07-06',
                         '2017-08-06', '2017-09-06', '2017-10-06', '2017-11-06']
@@ -42,15 +42,15 @@
         [0.34986, 0.34213, 0.33587, 0.32957, 0.33556, 0.3311, 0.32631, 0.32217],
         [0.34959, 0.34196, 0.33573, 0.32961, 0.3361, 0.33176, 0.32704, 0.32296],
         [0.34934, 0.34181, 0.33561, 0.32964, 0.33658, 0.33235, 0.32769, 0.32368],
         [0.34912, 0.34167, 0.3355, 0.32967, 0.33701, 0.33288, 0.32827, 0.32432],
         [0.34891, 0.34154, 0.33539, 0.3297, 0.33742, 0.33337, 0.32881, 0.32492]]
 
     return MarketData(reference_date=reference_date,
-                      spot=spot,
+                      underlying_spots=underlying_spots,
                       risk_free_rate=risk_free_rate,
                       dividend_rate=dividend_rate,
                       expiration_dates=expiration_dates,
                       strikes=strikes,
                       data=data)
```

### Comparing `exotx-0.6.1/exotx/tests/instruments/test_barrier_option.py` & `exotx-0.6.3/exotx/tests/instruments/test_barrier_option.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,12 +61,13 @@
 
 def test_barrier_option_fd_heston_barrier_engine_constant_vol(my_barrier_option: BarrierOption,
                                                               my_market_data: MarketData,
                                                               my_static_data: StaticData) -> None:
     # Act
     model = 'fd-heston-barrier'
     # test if we retrieve the same price as BS
-    my_market_data.data = [[my_market_data.black_scholes_volatility] * len(i) for i in my_market_data.data]
+    my_market_data.data = [[my_market_data.underlying_black_scholes_volatilities[0]] * len(i) for i in
+                           my_market_data.data]
     pv = price(my_barrier_option, my_market_data, my_static_data, model)
 
     # Assert
     assert pv == pytest.approx(14.114219673481117, abs=1e-8)
```

### Comparing `exotx-0.6.1/exotx/tests/instruments/test_vanilla_option.py` & `exotx-0.6.3/exotx/tests/instruments/test_vanilla_option.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,26 @@
 
 
 # Arrange
 @pytest.fixture
 def my_vanilla_option() -> VanillaOption:
     strike = 90
     maturity = '2016-05-04'
-    exercise = 'european'
     option_type = OptionType.CALL
-    # option_type = 'call'
 
     return VanillaOption(strike, maturity, option_type)
 
 
 @pytest.fixture
 def my_pricing_config() -> PricingConfiguration:
     model = PricingModel.BLACK_SCHOLES
     numerical_method = NumericalMethod.ANALYTIC
     compute_greeks = True
 
-    return PricingConfiguration(model, numerical_method, compute_greeks)
+    return PricingConfiguration(model, numerical_method, compute_greeks=compute_greeks)
 
 
 def test_price_compute_greeks_is_true(my_vanilla_option, my_market_data, my_static_data, my_pricing_config):
     # Act
     result = price(my_vanilla_option, my_market_data, my_static_data, my_pricing_config)
 
     # Assert
```

### Comparing `exotx-0.6.1/exotx/tests/models/test_hestonmodel.py` & `exotx-0.6.3/exotx/tests/models/test_hestonmodel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import pytest
+
 from exotx.data.marketdata import MarketData
+from exotx.data.static.calendar import Calendar
 from exotx.data.staticdata import StaticData
 from exotx.models.hestonmodel import HestonModel
-from exotx.data.static.calendar import Calendar
 
 
 # Arrange
 @pytest.fixture
 def my_static_data() -> StaticData:
     return StaticData(calendar=Calendar(region='UnitedStates'))
 
 
 @pytest.fixture
 def my_market_data() -> MarketData:
     reference_date = '2015-11-06'
-    spot = 659.37
+    underlying_spots = [659.37]
     risk_free_rate = 0.01
     dividend_rate = 0.0
     expiration_dates = ['2015-12-06', '2016-01-06', '2016-02-06', '2016-03-06', '2016-04-06',
                         '2016-05-06', '2016-06-06', '2016-07-06', '2016-08-06', '2016-09-06',
                         '2016-10-06', '2016-11-06', '2016-12-06', '2017-01-06', '2017-02-06',
                         '2017-03-06', '2017-04-06', '2017-05-06', '2017-06-06', '2017-07-06',
                         '2017-08-06', '2017-09-06', '2017-10-06', '2017-11-06']
@@ -46,15 +47,15 @@
         [0.34986, 0.34213, 0.33587, 0.32957, 0.33556, 0.3311, 0.32631, 0.32217],
         [0.34959, 0.34196, 0.33573, 0.32961, 0.3361, 0.33176, 0.32704, 0.32296],
         [0.34934, 0.34181, 0.33561, 0.32964, 0.33658, 0.33235, 0.32769, 0.32368],
         [0.34912, 0.34167, 0.3355, 0.32967, 0.33701, 0.33288, 0.32827, 0.32432],
         [0.34891, 0.34154, 0.33539, 0.3297, 0.33742, 0.33337, 0.32881, 0.32492]]
 
     return MarketData(reference_date=reference_date,
-                      spot=spot,
+                      underlying_spots=underlying_spots,
                       expiration_dates=expiration_dates,
                       strikes=strikes,
                       data=data,
                       risk_free_rate=risk_free_rate,
                       dividend_rate=dividend_rate)
```

### Comparing `exotx-0.6.1/exotx.egg-info/PKG-INFO` & `exotx-0.6.3/exotx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exotx
-Version: 0.6.1
+Version: 0.6.3
 Summary: Python library for pricing autocallables
 Home-page: https://github.com/SebastienEveno/exotx
 Author: Sebastien Eveno
 Author-email: sebastien.louis.eveno@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -16,98 +16,113 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.10.2, <4
 Description-Content-Type: text/markdown
 
 # exotx
+
 <p align="center">
     <img src="https://github.com/SebastienEveno/exotx/actions/workflows/python-package.yml/badge.svg?branch=master" />
     <a href="https://pypi.org/project/exotx" alt="Python Versions">
         <img src="https://img.shields.io/pypi/pyversions/exotx.svg?logo=python&logoColor=white" /></a>
     <a href="https://pypi.org/project/exotx" alt="PyPi">
         <img src="https://img.shields.io/pypi/v/exotx" /></a>
     <a href="https://pepy.tech/project/exotx" alt="Downloads">
         <img src="https://pepy.tech/badge/exotx" /></a>
 </p>
 
-exotx is a Python wrapper for the [QuantLib library](https://www.quantlib.org/), a powerful open-source library for quantitative finance. exotx provides a simple and user-friendly interface for pricing and analyzing financial derivatives using QuantLib's advanced numerical methods.
+exotx is a Python wrapper for the [QuantLib library](https://www.quantlib.org/), a powerful open-source library for
+quantitative finance. exotx provides a simple and user-friendly interface for pricing and analyzing financial
+derivatives using QuantLib's advanced numerical methods.
 
 ## Installation
 
 To install exotx, simply use pip:
+
 ```sh
 pip install exotx
 ```
 
 ## Usage
 
 ### Define the product
+
 ```python
 import exotx
 
 notional = 100
 strike = 100.0
 autocall_barrier_level = 1.0  # 100%
 annual_coupon_value = 0.03  # 3.00%
 coupon_barrier_level = 0.75  # 75%
 protection_barrier_level = 0.75  # 75%
 
 my_autocallable = exotx.Autocallable(notional, strike, autocall_barrier_level, annual_coupon_value, coupon_barrier_level, protection_barrier_level)
 ```
 
 ### Define the static data
+
 The object that represents static data such as the calendar, the day counter or the business day convention used.
 
 #### From the constructor
+
 ```python
 my_static_data = exotx.StaticData(day_counter='Actual360', business_day_convention='ModifiedFollowing')
 ```
 
 #### From JSON
+
 ```python
 my_json = {
     'day_counter': 'Actual360',
     'business_day_convention': 'ModifiedFollowing'
 }
 my_static_data = exotx.StaticData.from_json(my_json)
 ```
 
 ### Define the market data
+
 #### From the constructor
+
 ```python
 reference_date = '2015-11-06'
 spot = 100.0
 risk_free_rate = 0.01
 dividend_rate = 0.0
 black_scholes_volatility = 0.2
 
 my_market_data = exotx.MarketData(reference_date, spot, risk_free_rate, dividend_rate, black_scholes_volatility=black_scholes_volatility)
 ```
+
 #### From JSON
+
 ```python
 my_json = {
     'reference_date': '2015-11-06',
     'spot': 100,
     'risk_free_rate': 0.01,
     'dividend_rate': 0,
     'black_scholes_volatility': 0.2
 }
 my_market_data = exotx.MarketData.from_json(my_json)
 ```
 
 ### Price the product
+
 ```python
 exotx.price(my_autocallable, my_market_data, my_static_data, model='black-scholes')
 ```
+
 ```plaintext
 96.08517973497098
 ```
 
 ## Contributing
 
-We welcome contributions to exotx! If you find a bug or would like to request a new feature, please open an issue on the [Github repository](https://github.com/sebastieneveno/exotx). 
+We welcome contributions to exotx! If you find a bug or would like to request a new feature, please open an issue on
+the [Github repository](https://github.com/sebastieneveno/exotx).
 If you would like to contribute code, please submit a pull request.
 
 ## License
 
 exotx is released under the [MIT License](https://opensource.org/licenses/MIT).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: exotx Version: 0.6.1 Summary: Python library for
+Metadata-Version: 2.1 Name: exotx Version: 0.6.3 Summary: Python library for
 pricing autocallables Home-page: https://github.com/SebastienEveno/exotx
 Author: Sebastien Eveno Author-email: sebastien.louis.eveno@gmail.com License:
 MIT Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.10 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research Classifier: Topic :: Software
```

### Comparing `exotx-0.6.1/exotx.egg-info/SOURCES.txt` & `exotx-0.6.3/exotx.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -16,16 +16,20 @@
 exotx/data/static/calendar.py
 exotx/data/static/calendars.py
 exotx/data/static/conventions.py
 exotx/data/static/daycounters.py
 exotx/instruments/__init__.py
 exotx/instruments/asian_option.py
 exotx/instruments/autocallable.py
+exotx/instruments/average_calculation.py
+exotx/instruments/average_convention.py
 exotx/instruments/average_type.py
 exotx/instruments/barrier_option.py
+exotx/instruments/basket_option.py
+exotx/instruments/basket_type.py
 exotx/instruments/instrument.py
 exotx/instruments/option_type.py
 exotx/instruments/vanilla_option.py
 exotx/models/__init__.py
 exotx/models/blackscholesmodel.py
 exotx/models/hestonmodel.py
 exotx/tests/__init__.py
@@ -36,10 +40,11 @@
 exotx/tests/data/static/__init__.py
 exotx/tests/data/static/test_calendar.py
 exotx/tests/instruments/__init__.py
 exotx/tests/instruments/test_asian_option.py
 exotx/tests/instruments/test_autocallable_bs.py
 exotx/tests/instruments/test_autocallable_heston.py
 exotx/tests/instruments/test_barrier_option.py
+exotx/tests/instruments/test_basket_option.py
 exotx/tests/instruments/test_vanilla_option.py
 exotx/tests/models/__init__.py
 exotx/tests/models/test_hestonmodel.py
```

### Comparing `exotx-0.6.1/setup.py` & `exotx-0.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,19 +25,19 @@
           'plotly>=4.12.0',
           'quantlib>=1.26',
           'pytest>=7.1.3',
           'marshmallow>=3.19.0'
       ],
       python_requires='>=3.10.2, <4',
       classifiers=[
-        'Development Status :: 4 - Beta',
-        'Intended Audience :: Developers',
-        'Intended Audience :: Financial and Insurance Industry',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.10',
-        'Operating System :: OS Independent',
-        'Intended Audience :: Science/Research',
-        'Topic :: Software Development',
-        'Topic :: Office/Business :: Financial',
-        'Topic :: Scientific/Engineering :: Information Analysis'
-        ]
+          'Development Status :: 4 - Beta',
+          'Intended Audience :: Developers',
+          'Intended Audience :: Financial and Insurance Industry',
+          'License :: OSI Approved :: MIT License',
+          'Programming Language :: Python :: 3.10',
+          'Operating System :: OS Independent',
+          'Intended Audience :: Science/Research',
+          'Topic :: Software Development',
+          'Topic :: Office/Business :: Financial',
+          'Topic :: Scientific/Engineering :: Information Analysis'
+      ]
       )
```

