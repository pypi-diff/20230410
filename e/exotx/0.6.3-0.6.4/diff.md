# Comparing `tmp/exotx-0.6.3.tar.gz` & `tmp/exotx-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exotx-0.6.3.tar", last modified: Mon Apr 10 16:58:51 2023, max compression
+gzip compressed data, was "exotx-0.6.4.tar", last modified: Mon Apr 10 20:08:31 2023, max compression
```

## Comparing `exotx-0.6.3.tar` & `exotx-0.6.4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:51.049523 exotx-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-10 16:58:51.049523 exotx-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-10 16:58:40.000000 exotx-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:51.041523 exotx-0.6.3/exotx/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:51.045524 exotx-0.6.3/exotx/data/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/data/marketdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:51.045524 exotx-0.6.3/exotx/data/static/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/data/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/data/static/calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/data/static/calendars.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/data/static/conventions.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/data/static/daycounters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/data/staticdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:51.045524 exotx-0.6.3/exotx/instruments/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/instruments/asian_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/instruments/autocallable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/instruments/average_calculation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/instruments/average_convention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/instruments/average_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/instruments/barrier_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/instruments/basket_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/instruments/basket_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/instruments/instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/instruments/option_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/instruments/vanilla_option.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:51.045524 exotx-0.6.3/exotx/models/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/models/blackscholesmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/models/hestonmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:51.045524 exotx-0.6.3/exotx/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:51.045524 exotx-0.6.3/exotx/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:51.045524 exotx-0.6.3/exotx/tests/data/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/data/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/data/static/test_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/data/test_marketdata.py
--rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/data/test_staticdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:51.049523 exotx-0.6.3/exotx/tests/instruments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/instruments/test_asian_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/instruments/test_autocallable_bs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/instruments/test_autocallable_heston.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/instruments/test_barrier_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/instruments/test_basket_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/instruments/test_vanilla_option.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:51.049523 exotx-0.6.3/exotx/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-04-10 16:58:40.000000 exotx-0.6.3/exotx/tests/models/test_hestonmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:51.045524 exotx-0.6.3/exotx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-10 16:58:51.000000 exotx-0.6.3/exotx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-10 16:58:51.000000 exotx-0.6.3/exotx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:58:51.000000 exotx-0.6.3/exotx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 16:58:51.000000 exotx-0.6.3/exotx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 16:58:51.000000 exotx-0.6.3/exotx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-10 16:58:40.000000 exotx-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-10 16:58:51.049523 exotx-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-10 16:58:40.000000 exotx-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:08:31.523830 exotx-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-10 20:08:31.523830 exotx-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-10 20:08:20.000000 exotx-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:08:31.519830 exotx-0.6.4/exotx/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:08:31.519830 exotx-0.6.4/exotx/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/data/marketdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:08:31.519830 exotx-0.6.4/exotx/data/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/data/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/data/static/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/data/static/calendars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/data/static/conventions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/data/static/daycounters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/data/staticdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:08:31.523830 exotx-0.6.4/exotx/instruments/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14077 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/instruments/asian_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/instruments/autocallable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/instruments/average_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/instruments/average_convention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/instruments/average_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/instruments/barrier_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/instruments/basket_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/instruments/basket_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/instruments/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/instruments/option_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/instruments/vanilla_option.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:08:31.523830 exotx-0.6.4/exotx/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/models/blackscholesmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/models/hestonmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:08:31.523830 exotx-0.6.4/exotx/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:08:31.523830 exotx-0.6.4/exotx/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/tests/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:08:31.523830 exotx-0.6.4/exotx/tests/data/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/tests/data/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/tests/data/static/test_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/tests/data/test_marketdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/tests/data/test_staticdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:08:31.523830 exotx-0.6.4/exotx/tests/instruments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/tests/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/tests/instruments/test_asian_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/tests/instruments/test_autocallable_bs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/tests/instruments/test_autocallable_heston.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/tests/instruments/test_barrier_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/tests/instruments/test_basket_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/tests/instruments/test_vanilla_option.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:08:31.523830 exotx-0.6.4/exotx/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-04-10 20:08:20.000000 exotx-0.6.4/exotx/tests/models/test_hestonmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:08:31.519830 exotx-0.6.4/exotx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-10 20:08:31.000000 exotx-0.6.4/exotx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-10 20:08:31.000000 exotx-0.6.4/exotx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:08:31.000000 exotx-0.6.4/exotx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 20:08:31.000000 exotx-0.6.4/exotx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 20:08:31.000000 exotx-0.6.4/exotx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-10 20:08:20.000000 exotx-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-10 20:08:31.527830 exotx-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-10 20:08:20.000000 exotx-0.6.4/setup.py
```

### Comparing `exotx-0.6.3/PKG-INFO` & `exotx-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exotx
-Version: 0.6.3
+Version: 0.6.4
 Summary: Python library for pricing autocallables
 Home-page: https://github.com/SebastienEveno/exotx
 Author: Sebastien Eveno
 Author-email: sebastien.louis.eveno@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: exotx Version: 0.6.3 Summary: Python library for
+Metadata-Version: 2.1 Name: exotx Version: 0.6.4 Summary: Python library for
 pricing autocallables Home-page: https://github.com/SebastienEveno/exotx
 Author: Sebastien Eveno Author-email: sebastien.louis.eveno@gmail.com License:
 MIT Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.10 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research Classifier: Topic :: Software
```

### Comparing `exotx-0.6.3/README.md` & `exotx-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `exotx-0.6.3/exotx/data/marketdata.py` & `exotx-0.6.4/exotx/data/marketdata.py`

 * *Files identical despite different names*

### Comparing `exotx-0.6.3/exotx/data/static/__init__.py` & `exotx-0.6.4/exotx/data/static/__init__.py`

 * *Files identical despite different names*

### Comparing `exotx-0.6.3/exotx/data/static/calendar.py` & `exotx-0.6.4/exotx/data/static/calendar.py`

 * *Files identical despite different names*

### Comparing `exotx-0.6.3/exotx/data/static/calendars.py` & `exotx-0.6.4/exotx/data/static/calendars.py`

 * *Files identical despite different names*

### Comparing `exotx-0.6.3/exotx/data/static/conventions.py` & `exotx-0.6.4/exotx/data/static/conventions.py`

 * *Files identical despite different names*

### Comparing `exotx-0.6.3/exotx/data/static/daycounters.py` & `exotx-0.6.4/exotx/data/static/daycounters.py`

 * *Files identical despite different names*

### Comparing `exotx-0.6.3/exotx/data/staticdata.py` & `exotx-0.6.4/exotx/data/staticdata.py`

 * *Files identical despite different names*

### Comparing `exotx-0.6.3/exotx/instruments/average_calculation.py` & `exotx-0.6.4/exotx/instruments/average_calculation.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,24 +6,45 @@
 
 class AverageCalculation(Enum):
     CONTINUOUS = 'continuous'
     DISCRETE = 'discrete'
 
 
 def convert_average_calculation(average_calculation: Union[str, AverageCalculation]) -> AverageCalculation:
+    """
+    Converts an AverageCalculation enum value or a string representing an average calculation to the corresponding AverageCalculation enum value.
+
+    This function takes an input average_calculation, which can be either an AverageCalculation enum value or a string, and returns the
+    corresponding AverageCalculation enum value. The function raises an error if the input is invalid or not supported.
+
+    :param average_calculation: The input average calculation, either as an AverageCalculation enum value or a string.
+    :type average_calculation: Union[str, AverageCalculation]
+    :return: The corresponding AverageCalculation enum value.
+    :rtype: AverageCalculation
+    :raises ValueError: If the input average calculation is invalid or not supported.
+    :raises Exception: If the input type is not a valid AverageCalculation enum value or a string.
+
+    Example usage:
+
+    >>> convert_average_calculation(AverageCalculation.CONTINUOUS)
+    <AverageCalculation.CONTINUOUS: 'continuous'>
+    >>> convert_average_calculation('discrete')
+    <AverageCalculation.DISCRETE: 'discrete'>
+    """
     if isinstance(average_calculation, str):
         average_calculation = average_calculation.upper()
         if average_calculation not in AverageCalculation.__members__:
             raise ValueError(
                 f"Invalid average calculation \"{average_calculation}\", expected one of {list(AverageCalculation.__members__.keys())}")
         return AverageCalculation[average_calculation]
     elif isinstance(average_calculation, AverageCalculation):
         return average_calculation
     else:
-        raise Exception(f"Invalid average calculation type \"{type(average_calculation)}\"")
+        raise Exception(
+            f"Invalid average calculation type \"{type(average_calculation)}\"")
 
 
 class AverageCalculationField(fields.Field):
     def _serialize(self, value: AverageCalculation, attr, obj, **kwargs) -> str:
         return value.name
 
     def _deserialize(self, value: str, attr, data, **kwargs) -> AverageCalculation:
```

### Comparing `exotx-0.6.3/exotx/instruments/barrier_option.py` & `exotx-0.6.4/exotx/instruments/barrier_option.py`

 * *Files 22% similar despite different names*

```diff
@@ -31,15 +31,31 @@
     ANALYTICBARRIERENGINE = 'analytic'
     FDBLACKSCHOLESBARRIERENGINE = 'fd-bs-barrier'
     FDBLACKSCHOLESREBATEENGINE = 'fd-bs-rebate'
     FDHESTONBARRIERENGINE = 'fd-heston-barrier'
 
 
 class BarrierOption(Instrument):
-    """Class for modeling a barrier option."""
+    """
+    BarrierOption is a class representing a barrier option financial instrument.
+
+    The BarrierOption class provides methods for pricing and analyzing barrier options using various models
+    and pricing engines from the QuantLib library.
+
+    Attributes:
+        barrier_type (BarrierType): The barrier type (Up-and-In, Up-and-Out, Down-and-In, or Down-and-Out).
+        barrier (float): The barrier level.
+        strike (float): The strike price of the option.
+        maturity (ql.Date): The maturity date of the option.
+        exercise (ExerciseType): The exercise style (European or American).
+        option_type (OptionType): The option type (Call or Put).
+        rebate (float): The rebate amount.
+        reference_date (ql.Date): The reference date used for pricing the option.
+        model (str): The pricing model used for the option.
+    """
 
     def __init__(self,
                  barrier_type: str,
                  barrier: float,
                  strike: float,
                  maturity: str,
                  exercise: str = 'european',
@@ -52,25 +68,39 @@
         self.exercise = ExerciseType[exercise.upper()]
         self.option_type = OptionType[option_type.upper()]
         self.rebate = rebate
         self.reference_date = ql.Date().todaysDate()
         self.model = None
 
     def price(self, market_data: MarketData, static_data: StaticData, model: str):
+        """
+        Calculates the price of the barrier option using the given market data, static data, and model.
+
+        :param market_data: The market data used for pricing the option.
+        :type market_data: MarketData
+        :param static_data: The static data used for pricing the option.
+        :type static_data: StaticData
+        :param model: The pricing model used for the option.
+        :type model: str
+        :return: The net present value (NPV) of the option.
+        :rtype: float
+        """
         self.reference_date: ql.Date = market_data.get_ql_reference_date()
         ql.Settings.instance().evaluationDate = self.reference_date
 
         # create product
         ql_barrier_type = self._get_ql_barrier_type()
         ql_payoff = self._get_ql_payoff()
         ql_exercise = self._get_ql_exercise()
-        ql_option = ql.BarrierOption(ql_barrier_type, self.barrier, self.rebate, ql_payoff, ql_exercise)
+        ql_option = ql.BarrierOption(
+            ql_barrier_type, self.barrier, self.rebate, ql_payoff, ql_exercise)
 
         # set pricing engine
-        ql_pricing_engine = self._get_ql_pricing_engine(market_data, static_data, model)
+        ql_pricing_engine = self._get_ql_pricing_engine(
+            market_data, static_data, model)
         ql_option.setPricingEngine(ql_pricing_engine)
 
         return ql_option.NPV()
 
     def _get_ql_barrier_type(self) -> ql.Barrier:
         if self.barrier_type == BarrierType.UPANDIN:
             return ql.Barrier.UpIn
```

### Comparing `exotx-0.6.3/exotx/instruments/basket_option.py` & `exotx-0.6.4/exotx/instruments/basket_option.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,39 +9,83 @@
 from exotx.instruments.basket_type import BasketType, convert_basket_type, BasketTypeField
 from exotx.instruments.instrument import Instrument
 from exotx.instruments.option_type import convert_option_type_to_ql, OptionType, OptionTypeField
 from exotx.utils.pricing_configuration import PricingConfiguration
 
 
 class BasketOption(Instrument):
+    """
+    BasketOption is a class representing a basket option financial instrument.
+
+    A basket option is a financial derivative that derives its value from the weighted sum of several underlying assets.
+    The class inherits from the Instrument abstract base class and implements the price method to calculate the price of
+    the basket option.
+
+    The class also provides methods for converting basket type to the corresponding QuantLib payoff and creating a
+    QuantLib pricing engine for the basket option.
+
+    Attributes:
+    - strike (float): The option's strike price.
+    - maturity (ql.Date): The option's maturity date in QuantLib format.
+    - option_type (ql.Option.Type): The option type (call or put) in QuantLib format.
+    - basket_type (BasketType): The basket type (minbasket, maxbasket, spreadbasket, or averagebasket).
+
+    Example usage:
+
+    >>> basket_option = BasketOption(strike=100.0, maturity='2023-05-10', option_type='call', basket_type='minbasket')
+    >>> price = basket_option.price(market_data, static_data, pricing_config)
+    """
+
     def __init__(self,
                  strike: float,
                  maturity: Union[str, datetime],
                  option_type: Union[str, OptionType],
                  basket_type: Union[str, BasketType]):
         assert strike >= 0, "Invalid strike: cannot be negative"
         self.strike = strike
         self.maturity = convert_maturity_to_ql_date(maturity)
         self.option_type = convert_option_type_to_ql(option_type)
         self.basket_type = convert_basket_type(basket_type)
 
     def price(self, market_data, static_data, pricing_config: PricingConfiguration, seed: int = 1) -> dict:
+        """
+        Calculates the price and optionally the greeks (delta, gamma, and theta) for the basket option using the 
+        provided market data, static data, and pricing configuration.
+
+        :param market_data: Market data object containing relevant market information such as yield curve, dividend curve,
+                            underlying spots, and volatilities.
+        :type market_data: MarketData
+        :param static_data: Static data object containing relevant static information such as calendar and day counter.
+        :type static_data: StaticData
+        :param pricing_config: Pricing configuration object containing pricing settings and whether to compute greeks.
+        :type pricing_config: PricingConfiguration
+        :param seed: Seed for the random number generator used in Monte Carlo pricing engine, defaults to 1.
+        :type seed: int, optional
+        :return: A dictionary containing the price and optionally the greeks (delta, gamma, and theta) of the option.
+        :rtype: dict
+
+        Example usage:
+
+        >>> basket_option.price(market_data, static_data, pricing_config)
+        {'price': 10.1234, 'delta': 0.5678, 'gamma': 0.0123, 'theta': -0.0987}
+        """
         # set the reference date
         reference_date: ql.Date = market_data.get_ql_reference_date()
         ql.Settings.instance().evaluationDate = reference_date
 
         # create the product
         ql_payoff = ql.PlainVanillaPayoff(self.option_type, self.strike)
         ql_exercise = ql.EuropeanExercise(self.maturity)
 
         ql_basket_payoff = self._basket_type_to_payoff(ql_payoff)
         ql_option = ql.BasketOption(ql_basket_payoff, ql_exercise)
 
         # set the pricing engine
-        ql_engine = self._get_ql_pricing_engine(market_data, static_data, pricing_config, seed)
+        ql_engine = self._get_ql_pricing_engine(
+            market_data, static_data, pricing_config, seed)
         ql_option.setPricingEngine(ql_engine)
 
         # price
         price = ql_option.NPV()
         if pricing_config.compute_greeks:
             delta = ql_option.delta()
             gamma = ql_option.gamma()
@@ -104,30 +148,69 @@
         reference_date = market_data.get_ql_reference_date()
 
         # set static data
         calendar = static_data.get_ql_calendar()
         day_counter = static_data.get_ql_day_counter()
 
         processes = [ql.BlackScholesMertonProcess(ql.QuoteHandle(ql.SimpleQuote(x)),
-                                                  market_data.get_dividend_curve(day_counter),
-                                                  market_data.get_yield_curve(day_counter),
+                                                  market_data.get_dividend_curve(
+                                                      day_counter),
+                                                  market_data.get_yield_curve(
+                                                      day_counter),
                                                   ql.BlackVolTermStructureHandle(
                                                       ql.BlackConstantVol(reference_date, calendar, y, day_counter)))
                      for x, y in zip(market_data.underlying_spots, market_data.underlying_black_scholes_volatilities)]
-        multi_processes = ql.StochasticProcessArray(processes, market_data.get_correlation_matrix())
+        multi_processes = ql.StochasticProcessArray(
+            processes, market_data.get_correlation_matrix())
 
         # TODO: Consider different pricing engines based on self.basket_type and/or pricing_config
         return ql.MCEuropeanBasketEngine(multi_processes, RandomNumberGenerator.PSEUDORANDOM.value, timeStepsPerYear=1,
                                          requiredSamples=100000, seed=seed)
 
 
 # region Schema
 class BasketOptionSchema(Schema):
+    """
+    BasketOptionSchema is a Marshmallow schema class for deserializing and validating JSON data into a BasketOption object.
+
+    This schema defines the required fields for a BasketOption object and validates their types and values. It also provides
+    a post_load method to create a BasketOption object after deserialization and validation.
+
+    Fields:
+    - strike (float): The option's strike price.
+    - maturity (date): The option's maturity date in the format "YYYY-MM-DD".
+    - option_type (OptionType): The option type, either "call" or "put".
+    - basket_type (BasketType): The basket type, one of "minbasket", "maxbasket", "spreadbasket", or "averagebasket".
+
+    Example usage:
+
+    >>> basket_option_data = {
+    ...     "strike": 100.0,
+    ...     "maturity": "2023-05-10",
+    ...     "option_type": "call",
+    ...     "basket_type": "minbasket"
+    ... }
+    >>> schema = BasketOptionSchema()
+    >>> result = schema.load(basket_option_data)
+    >>> basket_option = result.data
+    """
     strike = fields.Float()
     maturity = fields.Date(format="%Y-%m-%d")
     option_type = OptionTypeField()
     basket_type = BasketTypeField()
 
     @post_load
     def make_basket_option(self, data, **kwargs) -> BasketOption:
+        """
+        Constructs a BasketOption instance from the deserialized data.
+
+        This method is called by the Marshmallow schema after the input data has been deserialized.
+        It uses the deserialized data to create a new BasketOption instance and returns it.
+
+        :param data: A dictionary containing the deserialized data for the basket option.
+        :type data: dict
+        :param kwargs: Additional keyword arguments.
+        :return: A BasketOption instance created from the deserialized data.
+        :rtype: BasketOption
+        """
         return BasketOption(**data)
 # endregion
```

### Comparing `exotx-0.6.3/exotx/instruments/basket_type.py` & `exotx-0.6.4/exotx/instruments/basket_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,31 @@
     MINBASKET = 'minbasket'
     MAXBASKET = 'maxbasket'
     SPREADBASKET = 'spreadbasket'
     AVERAGEBASKET = 'averagebasket'
 
 
 def convert_basket_type(basket_type: Union[str, BasketType]) -> BasketType:
+    """
+    Converts the input basket_type to a BasketType enumeration value.
+
+    :param basket_type: A string or BasketType instance representing the basket type.
+    :type basket_type: Union[str, BasketType]
+    :return: The corresponding BasketType enumeration value.
+    :rtype: BasketType
+    :raises ValueError: If the input string is not a valid BasketType member.
+    :raises Exception: If the input is neither a string nor a BasketType instance.
+
+    Example usage:
+
+    >>> convert_basket_type("minbasket")
+    <BasketType.MINBASKET: 1>
+    >>> convert_basket_type(BasketType.MINBASKET)
+    <BasketType.MINBASKET: 1>
+    """
     if isinstance(basket_type, str):
         basket_type = basket_type.upper()
         if basket_type not in BasketType.__members__:
             raise ValueError(
                 f"Invalid basket type \"{basket_type}\", expected one of {list(BasketType.__members__.keys())}")
         return BasketType[basket_type]
     elif isinstance(basket_type, BasketType):
```

### Comparing `exotx-0.6.3/exotx/models/blackscholesmodel.py` & `exotx-0.6.4/exotx/models/blackscholesmodel.py`

 * *Files identical despite different names*

### Comparing `exotx-0.6.3/exotx/models/hestonmodel.py` & `exotx-0.6.4/exotx/models/hestonmodel.py`

 * *Files identical despite different names*

### Comparing `exotx-0.6.3/exotx/tests/conftest.py` & `exotx-0.6.4/exotx/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `exotx-0.6.3/exotx/tests/data/static/test_calendar.py` & `exotx-0.6.4/exotx/tests/data/static/test_calendar.py`

 * *Files identical despite different names*

### Comparing `exotx-0.6.3/exotx/tests/data/test_staticdata.py` & `exotx-0.6.4/exotx/tests/data/test_staticdata.py`

 * *Files identical despite different names*

### Comparing `exotx-0.6.3/exotx/tests/instruments/test_asian_option.py` & `exotx-0.6.4/exotx/tests/instruments/test_asian_option.py`

 * *Files identical despite different names*

### Comparing `exotx-0.6.3/exotx/tests/instruments/test_autocallable_bs.py` & `exotx-0.6.4/exotx/tests/instruments/test_autocallable_bs.py`

 * *Files identical despite different names*

### Comparing `exotx-0.6.3/exotx/tests/instruments/test_autocallable_heston.py` & `exotx-0.6.4/exotx/tests/instruments/test_autocallable_heston.py`

 * *Files identical despite different names*

### Comparing `exotx-0.6.3/exotx/tests/instruments/test_barrier_option.py` & `exotx-0.6.4/exotx/tests/instruments/test_barrier_option.py`

 * *Files identical despite different names*

### Comparing `exotx-0.6.3/exotx/tests/instruments/test_basket_option.py` & `exotx-0.6.4/exotx/tests/instruments/test_basket_option.py`

 * *Files identical despite different names*

### Comparing `exotx-0.6.3/exotx/tests/instruments/test_vanilla_option.py` & `exotx-0.6.4/exotx/tests/instruments/test_vanilla_option.py`

 * *Files identical despite different names*

### Comparing `exotx-0.6.3/exotx/tests/models/test_hestonmodel.py` & `exotx-0.6.4/exotx/tests/models/test_hestonmodel.py`

 * *Files identical despite different names*

### Comparing `exotx-0.6.3/exotx.egg-info/PKG-INFO` & `exotx-0.6.4/exotx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exotx
-Version: 0.6.3
+Version: 0.6.4
 Summary: Python library for pricing autocallables
 Home-page: https://github.com/SebastienEveno/exotx
 Author: Sebastien Eveno
 Author-email: sebastien.louis.eveno@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: exotx Version: 0.6.3 Summary: Python library for
+Metadata-Version: 2.1 Name: exotx Version: 0.6.4 Summary: Python library for
 pricing autocallables Home-page: https://github.com/SebastienEveno/exotx
 Author: Sebastien Eveno Author-email: sebastien.louis.eveno@gmail.com License:
 MIT Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.10 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research Classifier: Topic :: Software
```

### Comparing `exotx-0.6.3/exotx.egg-info/SOURCES.txt` & `exotx-0.6.4/exotx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exotx-0.6.3/setup.py` & `exotx-0.6.4/setup.py`

 * *Files identical despite different names*

