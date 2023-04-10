# Comparing `tmp/market_analy-0.2.tar.gz` & `tmp/market_analy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "market_analy-0.2.tar", last modified: Thu Feb 23 19:17:00 2023, max compression
+gzip compressed data, was "market_analy-0.2.3.tar", last modified: Mon Apr 10 11:19:10 2023, max compression
```

## Comparing `market_analy-0.2.tar` & `market_analy-0.2.3.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 19:17:00.153068 market_analy-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-02-23 19:16:44.000000 market_analy-0.2/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-02-23 19:16:44.000000 market_analy-0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-02-23 19:16:44.000000 market_analy-0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-02-23 19:16:44.000000 market_analy-0.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-23 19:16:44.000000 market_analy-0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-23 19:16:44.000000 market_analy-0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-02-23 19:17:00.153068 market_analy-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-02-23 19:16:44.000000 market_analy-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 19:17:00.149068 market_analy-0.2/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 19:17:00.149068 market_analy-0.2/etc/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-02-23 19:16:44.000000 market_analy-0.2/etc/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-02-23 19:16:44.000000 market_analy-0.2/etc/requirements/why_here.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-02-23 19:16:44.000000 market_analy-0.2/etc/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-02-23 19:16:44.000000 market_analy-0.2/etc/requirements_tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-02-23 19:16:44.000000 market_analy-0.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-02-23 19:16:44.000000 market_analy-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-02-23 19:16:44.000000 market_analy-0.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 19:17:00.153068 market_analy-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-02-23 19:16:44.000000 market_analy-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 19:17:00.145068 market_analy-0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 19:17:00.149068 market_analy-0.2/src/market_analy/
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-02-23 19:16:44.000000 market_analy-0.2/src/market_analy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-02-23 19:16:59.000000 market_analy-0.2/src/market_analy/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    42395 2023-02-23 19:16:44.000000 market_analy-0.2/src/market_analy/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    65847 2023-02-23 19:16:44.000000 market_analy-0.2/src/market_analy/charts.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-02-23 19:16:44.000000 market_analy-0.2/src/market_analy/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)    17878 2023-02-23 19:16:44.000000 market_analy-0.2/src/market_analy/gui_parts.py
--rw-r--r--   0 runner    (1001) docker     (123)    55600 2023-02-23 19:16:44.000000 market_analy-0.2/src/market_analy/guis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 19:17:00.153068 market_analy-0.2/src/market_analy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-23 19:16:44.000000 market_analy-0.2/src/market_analy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25901 2023-02-23 19:16:44.000000 market_analy-0.2/src/market_analy/utils/bq_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-02-23 19:16:44.000000 market_analy-0.2/src/market_analy/utils/dict_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    27866 2023-02-23 19:16:44.000000 market_analy-0.2/src/market_analy/utils/ipyvuetify_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14373 2023-02-23 19:16:44.000000 market_analy-0.2/src/market_analy/utils/ipywidgets_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20188 2023-02-23 19:16:44.000000 market_analy-0.2/src/market_analy/utils/list_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-02-23 19:16:44.000000 market_analy-0.2/src/market_analy/utils/maths_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-02-23 19:16:44.000000 market_analy-0.2/src/market_analy/utils/mkt_prices_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-02-23 19:16:44.000000 market_analy-0.2/src/market_analy/utils/pandas_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 19:17:00.153068 market_analy-0.2/src/market_analy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-02-23 19:17:00.000000 market_analy-0.2/src/market_analy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-02-23 19:17:00.000000 market_analy-0.2/src/market_analy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 19:17:00.000000 market_analy-0.2/src/market_analy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-02-23 19:17:00.000000 market_analy-0.2/src/market_analy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-23 19:17:00.000000 market_analy-0.2/src/market_analy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:19:10.189507 market_analy-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-10 11:18:52.000000 market_analy-0.2.3/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-10 11:18:52.000000 market_analy-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-10 11:18:52.000000 market_analy-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-10 11:18:52.000000 market_analy-0.2.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-10 11:18:52.000000 market_analy-0.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-10 11:18:52.000000 market_analy-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-04-10 11:19:10.189507 market_analy-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-04-10 11:18:52.000000 market_analy-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:19:10.185507 market_analy-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    42684 2023-04-10 11:18:52.000000 market_analy-0.2.3/docs/splash.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:19:10.185507 market_analy-0.2.3/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:19:10.185507 market_analy-0.2.3/etc/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-10 11:18:52.000000 market_analy-0.2.3/etc/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-10 11:18:52.000000 market_analy-0.2.3/etc/requirements/why_here.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-10 11:18:52.000000 market_analy-0.2.3/etc/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-10 11:18:52.000000 market_analy-0.2.3/etc/requirements_tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-10 11:18:52.000000 market_analy-0.2.3/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-10 11:18:52.000000 market_analy-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-10 11:18:52.000000 market_analy-0.2.3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 11:19:10.189507 market_analy-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-10 11:18:52.000000 market_analy-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:19:10.181507 market_analy-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:19:10.185507 market_analy-0.2.3/src/market_analy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-10 11:19:09.000000 market_analy-0.2.3/src/market_analy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42395 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66003 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18025 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/gui_parts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56989 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/guis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:19:10.189507 market_analy-0.2.3/src/market_analy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25931 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/utils/bq_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/utils/dict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27860 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/utils/ipyvuetify_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/utils/ipywidgets_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20188 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/utils/list_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/utils/maths_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/utils/mkt_prices_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/utils/pandas_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:19:10.189507 market_analy-0.2.3/src/market_analy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-04-10 11:19:10.000000 market_analy-0.2.3/src/market_analy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-10 11:19:10.000000 market_analy-0.2.3/src/market_analy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 11:19:10.000000 market_analy-0.2.3/src/market_analy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-10 11:19:10.000000 market_analy-0.2.3/src/market_analy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-10 11:19:10.000000 market_analy-0.2.3/src/market_analy.egg-info/top_level.txt
```

### Comparing `market_analy-0.2/.flake8` & `market_analy-0.2.3/.flake8`

 * *Files identical despite different names*

### Comparing `market_analy-0.2/.gitignore` & `market_analy-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `market_analy-0.2/.pre-commit-config.yaml` & `market_analy-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `market_analy-0.2/.pylintrc` & `market_analy-0.2.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `market_analy-0.2/LICENSE.txt` & `market_analy-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `market_analy-0.2/PKG-INFO` & `market_analy-0.2.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: market_analy
-Version: 0.2
+Version: 0.2.3
 Summary: Analysis of exchange-listed financial instruments
 Author: Marcus Read
 Author-email: marcusaread@gmail.com
 License: MIT License
 Project-URL: homepage, https://github.com/maread99/market_analy
 Project-URL: documentation, https://github.com/maread99/market_analy
 Project-URL: Issue Tracker, https://github.com/maread99/market_analy/issues
@@ -30,14 +30,20 @@
 Description-Content-Type: text/markdown
 Provides-Extra: jupyter
 Provides-Extra: tests
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 <!-- NB any links not defined as aboslute will not resolve on PyPI page -->
+<div align="center">
+  <img src="docs/splash.png"><br>
+</div>
+
+-----------------
+
 # market_analy
 
 [![PyPI](https://img.shields.io/pypi/v/market-analy)](https://pypi.org/project/market-analy/) ![Python Support](https://img.shields.io/pypi/pyversions/market-analy) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 A python package to analyse financial instruments.
 
 There's a load of great financial libraries out there for Technical Analysis, Charting, Backtesting, Portfolio Analysis etc. This library isn't reinventing the wheel (not intentionally anyway), rather it provides functions and interactive charting that I think are useful and couldn't find elsewhere. It's not comprehensive, but rather fills some of the gaps.
@@ -102,19 +108,27 @@
 ### `market-prices` dependency
 `market-analy` depends on the [market-prices][market-prices] library for price data. This provides for functionality including:
 * defining analysis periods in terms of number of sessions and trading minutes rather than calendar days and times.
 * complete data sets regardless of liquidity (regular data points during market hours, no data points outside of market hours).
 
 Most of the arguments available to the market-prices `get` function can be passed directly to the `market_analy` functions. See the [market-prices][market-prices] documentation for further info.
 
-## Disclaimers
-`market-analy` should not be assumed sufficiently reliable to undertake analysis intended to inform investment decisions. Users should inspect the source code and the test suite of the library and its dependencies in order to make their own assessment of the packages' suitability for their purposes. **The `market-analy` package is used entirely at the user's own risk.**
+## Release schedule, bugs, development and feedback
+
+The first beta version of `market_analy` was released Feb 2023. It's anticipated that functionality to define and visually interrogate trends will be added later in 2023.
+
+The project is immature. Whilst it's not anticipated that major changes will be made to the existing public side, they could be. All that's under-the-bonnet is subject to change as the project evolves. The `guis` module in particular won't permit much further development without overhauling the current inheritance-based approach to a compositional one.
 
 The test suite is limited. It's pretty much guaranteed that there are bugs. Please raise an [issue](https://github.com/maread99/market_analy/issues) if you find one or come across unexpected behaviour.
 
+Please use [discussions](https://github.com/maread99/market_analy/discussions) to make any suggestions and offer general feedback.
+
+## Disclaimers
+`market-analy` should not be assumed sufficiently reliable to undertake analysis intended to inform investment decisions. Users should inspect the source code and the test suite of the library and its dependencies in order to make their own assessment of the packages' suitability for their purposes. **The `market-analy` package is used entirely at the user's own risk.**
+
 The default `market_prices.PricesYahoo` class gets data from publically available Yahoo APIs. **See the [Disclaimers section of the market-prices README](https://github.com/maread99/market_prices#disclaimers) for conditions of use**, including restrictions.
 
 ## Alternative packages
 
 * [awesome-quant](https://github.com/wilsonfreitas/awesome-quant) offers an extensive listing of libraries for all things finance.
 
 ## License
```

### Comparing `market_analy-0.2/README.md` & `market_analy-0.2.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 <!-- NB any links not defined as aboslute will not resolve on PyPI page -->
+<div align="center">
+  <img src="docs/splash.png"><br>
+</div>
+
+-----------------
+
 # market_analy
 
 [![PyPI](https://img.shields.io/pypi/v/market-analy)](https://pypi.org/project/market-analy/) ![Python Support](https://img.shields.io/pypi/pyversions/market-analy) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 A python package to analyse financial instruments.
 
 There's a load of great financial libraries out there for Technical Analysis, Charting, Backtesting, Portfolio Analysis etc. This library isn't reinventing the wheel (not intentionally anyway), rather it provides functions and interactive charting that I think are useful and couldn't find elsewhere. It's not comprehensive, but rather fills some of the gaps.
@@ -67,19 +73,27 @@
 ### `market-prices` dependency
 `market-analy` depends on the [market-prices][market-prices] library for price data. This provides for functionality including:
 * defining analysis periods in terms of number of sessions and trading minutes rather than calendar days and times.
 * complete data sets regardless of liquidity (regular data points during market hours, no data points outside of market hours).
 
 Most of the arguments available to the market-prices `get` function can be passed directly to the `market_analy` functions. See the [market-prices][market-prices] documentation for further info.
 
-## Disclaimers
-`market-analy` should not be assumed sufficiently reliable to undertake analysis intended to inform investment decisions. Users should inspect the source code and the test suite of the library and its dependencies in order to make their own assessment of the packages' suitability for their purposes. **The `market-analy` package is used entirely at the user's own risk.**
+## Release schedule, bugs, development and feedback
+
+The first beta version of `market_analy` was released Feb 2023. It's anticipated that functionality to define and visually interrogate trends will be added later in 2023.
+
+The project is immature. Whilst it's not anticipated that major changes will be made to the existing public side, they could be. All that's under-the-bonnet is subject to change as the project evolves. The `guis` module in particular won't permit much further development without overhauling the current inheritance-based approach to a compositional one.
 
 The test suite is limited. It's pretty much guaranteed that there are bugs. Please raise an [issue](https://github.com/maread99/market_analy/issues) if you find one or come across unexpected behaviour.
 
+Please use [discussions](https://github.com/maread99/market_analy/discussions) to make any suggestions and offer general feedback.
+
+## Disclaimers
+`market-analy` should not be assumed sufficiently reliable to undertake analysis intended to inform investment decisions. Users should inspect the source code and the test suite of the library and its dependencies in order to make their own assessment of the packages' suitability for their purposes. **The `market-analy` package is used entirely at the user's own risk.**
+
 The default `market_prices.PricesYahoo` class gets data from publically available Yahoo APIs. **See the [Disclaimers section of the market-prices README](https://github.com/maread99/market_prices#disclaimers) for conditions of use**, including restrictions.
 
 ## Alternative packages
 
 * [awesome-quant](https://github.com/wilsonfreitas/awesome-quant) offers an extensive listing of libraries for all things finance.
 
 ## License
```

### Comparing `market_analy-0.2/etc/requirements/requirements.txt` & `market_analy-0.2.3/etc/requirements/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,86 +4,86 @@
 #
 #    pip-compile --output-file=./etc/requirements/requirements.txt pyproject.toml
 #
 asttokens==2.2.1
     # via stack-data
 backcall==0.2.0
     # via ipython
-bqplot==0.12.36
+bqplot==0.12.38
     # via market-analy (pyproject.toml)
 certifi==2022.12.7
     # via requests
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via requests
 colorama==0.4.6
     # via
     #   ipython
     #   tqdm
-comm==0.1.2
+comm==0.1.3
     # via ipykernel
 contourpy==1.0.7
     # via matplotlib
 cycler==0.11.0
     # via matplotlib
-debugpy==1.6.6
+debugpy==1.6.7
     # via ipykernel
 decorator==5.1.1
     # via ipython
-exchange-calendars==4.2.5
+exchange-calendars==4.2.6
     # via
     #   market-analy (pyproject.toml)
     #   market-prices
 executing==1.2.0
     # via stack-data
-fonttools==4.38.0
+fonttools==4.39.3
     # via matplotlib
 idna==3.4
     # via requests
-importlib-metadata==6.0.0
+importlib-metadata==6.3.0
     # via jupyter-client
 importlib-resources==5.12.0
     # via matplotlib
-ipykernel==6.21.2
+ipykernel==6.22.0
     # via ipywidgets
-ipython==8.10.0
+ipython==8.12.0
     # via
     #   ipykernel
     #   ipywidgets
-ipyvue==1.8.0
+ipyvue==1.9.0
     # via ipyvuetify
-ipyvuetify==1.8.4
+ipyvuetify==1.8.5
     # via market-analy (pyproject.toml)
-ipywidgets==8.0.4
+ipywidgets==8.0.6
     # via
     #   bqplot
     #   ipyvue
     #   market-analy (pyproject.toml)
 jedi==0.18.2
     # via ipython
 jinja2==3.1.2
     # via market-analy (pyproject.toml)
-jupyter-client==8.0.3
+jupyter-client==8.1.0
     # via ipykernel
-jupyter-core==5.2.0
+jupyter-core==5.3.0
     # via
     #   ipykernel
     #   jupyter-client
-jupyterlab-widgets==3.0.5
+jupyterlab-widgets==3.0.7
     # via ipywidgets
 kiwisolver==1.4.4
     # via matplotlib
 korean-lunar-calendar==0.3.1
     # via exchange-calendars
 lxml==4.9.2
     # via yahooquery
-market-prices==0.10.1
+market-prices==0.10.2
     # via market-analy (pyproject.toml)
 markupsafe==2.1.2
     # via jinja2
-matplotlib==3.7.0
+matplotlib==3.7.1
     # via market-analy (pyproject.toml)
 matplotlib-inline==0.1.6
     # via
     #   ipykernel
     #   ipython
 nest-asyncio==1.5.6
     # via ipykernel
@@ -96,57 +96,57 @@
     #   market-prices
     #   matplotlib
     #   pandas
 packaging==23.0
     # via
     #   ipykernel
     #   matplotlib
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   bqplot
     #   exchange-calendars
     #   market-analy (pyproject.toml)
     #   market-prices
     #   yahooquery
 parso==0.8.3
     # via jedi
 pickleshare==0.7.5
     # via ipython
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
-platformdirs==3.0.0
+platformdirs==3.2.0
     # via jupyter-core
-prompt-toolkit==3.0.37
+prompt-toolkit==3.0.38
     # via ipython
 psutil==5.9.4
     # via ipykernel
 pure-eval==0.2.2
     # via stack-data
-pydantic==1.10.5
+pydantic==1.10.7
     # via market-prices
 pygments==2.14.0
     # via ipython
-pyluach==2.1.0
+pyluach==2.2.0
     # via exchange-calendars
 pyparsing==3.0.9
     # via matplotlib
 python-dateutil==2.8.2
     # via
     #   exchange-calendars
     #   jupyter-client
     #   matplotlib
     #   pandas
-pytz==2022.7.1
+pytz==2023.3
     # via
     #   exchange-calendars
     #   market-prices
     #   pandas
-# pywin32==315
+# pywin32==306
     # via jupyter-core
-pyzmq==25.0.0
+pyzmq==25.0.2
     # via
     #   ipykernel
     #   jupyter-client
 requests==2.28.2
     # via requests-futures
 requests-futures==1.0.0
     # via yahooquery
@@ -158,15 +158,15 @@
     # via ipython
 toolz==0.12.0
     # via exchange-calendars
 tornado==6.2
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.64.1
+tqdm==4.65.0
     # via yahooquery
 traitlets==5.9.0
     # via
     #   bqplot
     #   comm
     #   ipykernel
     #   ipython
@@ -175,20 +175,24 @@
     #   jupyter-core
     #   market-analy (pyproject.toml)
     #   matplotlib-inline
     #   traittypes
 traittypes==0.2.1
     # via bqplot
 typing-extensions==4.5.0
-    # via pydantic
-urllib3==1.26.14
+    # via
+    #   ipython
+    #   pydantic
+tzdata==2023.3
+    # via pandas
+urllib3==1.26.15
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
-widgetsnbextension==4.0.5
+widgetsnbextension==4.0.7
     # via ipywidgets
-yahooquery==2.3.0
+yahooquery==2.3.1
     # via market-prices
-zipp==3.14.0
+zipp==3.15.0
     # via
     #   importlib-metadata
     #   importlib-resources
```

### Comparing `market_analy-0.2/etc/requirements_dev.txt` & `market_analy-0.2.3/etc/requirements_tests.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,239 +1,192 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --extra=dev --output-file=./etc/requirements_dev.txt pyproject.toml
+#    pip-compile --extra=tests --output-file=./etc/requirements_tests.txt pyproject.toml
 #
-astroid==2.14.2
-    # via pylint
 asttokens==2.2.1
     # via stack-data
-attrs==22.2.0
-    # via pytest
 backcall==0.2.0
     # via ipython
-black==23.1.0
+black==23.3.0
     # via market-analy (pyproject.toml)
-bqplot==0.12.36
+bqplot==0.12.38
     # via market-analy (pyproject.toml)
-build==0.10.0
-    # via pip-tools
 certifi==2022.12.7
     # via requests
-cfgv==3.3.1
-    # via pre-commit
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via requests
 click==8.1.3
-    # via
-    #   black
-    #   pip-tools
+    # via black
 colorama==0.4.6
     # via
-    #   build
     #   click
     #   ipython
-    #   pylint
     #   pytest
     #   tqdm
-comm==0.1.2
+comm==0.1.3
     # via ipykernel
 contourpy==1.0.7
     # via matplotlib
 cycler==0.11.0
     # via matplotlib
-debugpy==1.6.6
+debugpy==1.6.7
     # via ipykernel
 decorator==5.1.1
     # via ipython
-dill==0.3.6
-    # via pylint
-distlib==0.3.6
-    # via virtualenv
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via pytest
-exchange-calendars==4.2.5
+exchange-calendars==4.2.6
     # via
     #   market-analy (pyproject.toml)
     #   market-prices
 executing==1.2.0
     # via stack-data
-filelock==3.9.0
-    # via virtualenv
 flake8==6.0.0
     # via
     #   flake8-docstrings
     #   market-analy (pyproject.toml)
 flake8-docstrings==1.7.0
     # via market-analy (pyproject.toml)
-fonttools==4.38.0
+fonttools==4.39.3
     # via matplotlib
-identify==2.5.18
-    # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==6.0.0
+importlib-metadata==6.3.0
     # via jupyter-client
 importlib-resources==5.12.0
     # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.21.2
+ipykernel==6.22.0
     # via ipywidgets
-ipython==8.10.0
+ipython==8.12.0
     # via
     #   ipykernel
     #   ipywidgets
-ipyvue==1.8.0
+ipyvue==1.9.0
     # via ipyvuetify
-ipyvuetify==1.8.4
+ipyvuetify==1.8.5
     # via market-analy (pyproject.toml)
-ipywidgets==8.0.4
+ipywidgets==8.0.6
     # via
     #   bqplot
     #   ipyvue
     #   market-analy (pyproject.toml)
-isort==5.12.0
-    # via pylint
 jedi==0.18.2
     # via ipython
 jinja2==3.1.2
     # via market-analy (pyproject.toml)
-jupyter-client==8.0.3
+jupyter-client==8.1.0
     # via ipykernel
-jupyter-core==5.2.0
+jupyter-core==5.3.0
     # via
     #   ipykernel
     #   jupyter-client
-jupyterlab-widgets==3.0.5
+jupyterlab-widgets==3.0.7
     # via ipywidgets
 kiwisolver==1.4.4
     # via matplotlib
 korean-lunar-calendar==0.3.1
     # via exchange-calendars
-lazy-object-proxy==1.9.0
-    # via astroid
 lxml==4.9.2
     # via yahooquery
-market-prices==0.10.1
+market-prices==0.10.2
     # via market-analy (pyproject.toml)
 markupsafe==2.1.2
     # via jinja2
-matplotlib==3.7.0
+matplotlib==3.7.1
     # via market-analy (pyproject.toml)
 matplotlib-inline==0.1.6
     # via
     #   ipykernel
     #   ipython
 mccabe==0.7.0
-    # via
-    #   flake8
-    #   pylint
-mypy==1.0.1
-    # via market-analy (pyproject.toml)
+    # via flake8
 mypy-extensions==1.0.0
-    # via
-    #   black
-    #   mypy
+    # via black
 nest-asyncio==1.5.6
     # via ipykernel
-nodeenv==1.7.0
-    # via pre-commit
 numpy==1.24.2
     # via
     #   bqplot
     #   contourpy
     #   exchange-calendars
     #   market-analy (pyproject.toml)
     #   market-prices
     #   matplotlib
     #   pandas
 packaging==23.0
     # via
     #   black
-    #   build
     #   ipykernel
     #   matplotlib
     #   pytest
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   bqplot
     #   exchange-calendars
     #   market-analy (pyproject.toml)
     #   market-prices
     #   yahooquery
-pandas-stubs==1.5.3.230214
-    # via market-analy (pyproject.toml)
 parso==0.8.3
     # via jedi
-pathspec==0.11.0
+pathspec==0.11.1
     # via black
 pickleshare==0.7.5
     # via ipython
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
-pip-tools==6.12.2
-    # via market-analy (pyproject.toml)
-platformdirs==3.0.0
+platformdirs==3.2.0
     # via
     #   black
     #   jupyter-core
-    #   pylint
-    #   virtualenv
 pluggy==1.0.0
     # via pytest
-pre-commit==3.1.0
-    # via market-analy (pyproject.toml)
-prompt-toolkit==3.0.37
+prompt-toolkit==3.0.38
     # via ipython
 psutil==5.9.4
     # via ipykernel
 pure-eval==0.2.2
     # via stack-data
 pycodestyle==2.10.0
     # via flake8
-pydantic==1.10.5
+pydantic==1.10.7
     # via market-prices
 pydocstyle==6.3.0
     # via flake8-docstrings
 pyflakes==3.0.1
     # via flake8
 pygments==2.14.0
     # via ipython
-pylint==2.16.2
-    # via market-analy (pyproject.toml)
-pyluach==2.1.0
+pyluach==2.2.0
     # via exchange-calendars
 pyparsing==3.0.9
     # via matplotlib
-pyproject-hooks==1.0.0
-    # via build
-pytest==7.2.1
+pytest==7.3.0
     # via
     #   market-analy (pyproject.toml)
     #   pytest-mock
 pytest-mock==3.10.0
     # via market-analy (pyproject.toml)
 python-dateutil==2.8.2
     # via
     #   exchange-calendars
     #   jupyter-client
     #   matplotlib
     #   pandas
-pytz==2022.7.1
+pytz==2023.3
     # via
     #   exchange-calendars
     #   market-prices
     #   pandas
-pywin32==305
+# pywin32==306
     # via jupyter-core
-pyyaml==6.0
-    # via pre-commit
-pyzmq==25.0.0
+pyzmq==25.0.2
     # via
     #   ipykernel
     #   jupyter-client
 requests==2.28.2
     # via requests-futures
 requests-futures==1.0.0
     # via yahooquery
@@ -244,28 +197,22 @@
 snowballstemmer==2.2.0
     # via pydocstyle
 stack-data==0.6.2
     # via ipython
 tomli==2.0.1
     # via
     #   black
-    #   build
-    #   mypy
-    #   pylint
-    #   pyproject-hooks
     #   pytest
-tomlkit==0.11.6
-    # via pylint
 toolz==0.12.0
     # via exchange-calendars
 tornado==6.2
     # via
     #   ipykernel
     #   jupyter-client
-tqdm==4.64.1
+tqdm==4.65.0
     # via yahooquery
 traitlets==5.9.0
     # via
     #   bqplot
     #   comm
     #   ipykernel
     #   ipython
@@ -273,40 +220,26 @@
     #   jupyter-client
     #   jupyter-core
     #   market-analy (pyproject.toml)
     #   matplotlib-inline
     #   traittypes
 traittypes==0.2.1
     # via bqplot
-types-pytz==2022.7.1.2
-    # via
-    #   market-analy (pyproject.toml)
-    #   pandas-stubs
 typing-extensions==4.5.0
     # via
-    #   astroid
     #   black
-    #   mypy
+    #   ipython
     #   pydantic
-    #   pylint
-urllib3==1.26.14
+tzdata==2023.3
+    # via pandas
+urllib3==1.26.15
     # via requests
-virtualenv==20.19.0
-    # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
-wheel==0.38.4
-    # via pip-tools
-widgetsnbextension==4.0.5
+widgetsnbextension==4.0.7
     # via ipywidgets
-wrapt==1.14.1
-    # via astroid
-yahooquery==2.3.0
+yahooquery==2.3.1
     # via market-prices
-zipp==3.14.0
+zipp==3.15.0
     # via
     #   importlib-metadata
     #   importlib-resources
-
-# The following packages are considered to be unsafe in a requirements file:
-# pip
-# setuptools
```

### Comparing `market_analy-0.2/pyproject.toml` & `market_analy-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `market_analy-0.2/src/market_analy/__init__.py` & `market_analy-0.2.3/src/market_analy/__init__.py`

 * *Files identical despite different names*

### Comparing `market_analy-0.2/src/market_analy/analysis.py` & `market_analy-0.2.3/src/market_analy/analysis.py`

 * *Files identical despite different names*

### Comparing `market_analy-0.2/src/market_analy/charts.py` & `market_analy-0.2.3/src/market_analy/charts.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,14 +250,15 @@
     @property
     def data(self) -> pd.DataFrame | pd.Series:
         """Chart data."""
         return self._data
 
     @data.setter
     def data(self, data: pd.DataFrame | pd.Series):
+        data = data.copy()
         if isinstance(data.index, pd.IntervalIndex):
             data.index = upd.interval_index_new_tz(data.index, None)
         elif data.index.tz is not None:
             data.index = data.index.tz_localize(None)
         self._data = data
 
     @property
@@ -546,16 +547,16 @@
         """bq.Figure from default kwargs.
 
         Notes
         -----
         Extend on subclass to pass through any additional kwargs. Can
         also pass through +title_style+ to override default value.
         """
-        kwargs["marks"] = [self.mark]
-        kwargs["axes"] = self.axes
+        kwargs.setdefault("marks", [self.mark])
+        kwargs.setdefault("axes", self.axes)
         kwargs.setdefault("background_style", {"fill": "#222222"})
         kwargs.setdefault("title_style", CHART_TITLE_STYLE)
         return bq.Figure(**kwargs)
 
     # TITLE
     @property
     def title(self) -> str | None:
@@ -631,16 +632,16 @@
         """Close all chart widgets."""
         for widget in self._widgets:
             widget.close()
 
     def delete(self):
         """Delete all chart widgets."""
         self.close()
-        for widget in copy(self._widgets):
-            del widget
+        for _ in range(len(self._widgets)):
+            del self._widgets[0]
 
     def display(self):
         """Display chart."""
         IPython.display.display(self.figure)
 
     def _cycle_legend(self):
         """Move legend to next position."""
@@ -1685,15 +1686,14 @@
             x_ticks to initially show on x-axis. None to show all.
 
         max_ticks
             Limit on number of dates to include to x-axis. NB If passed
             together with +visible_x_ticks+ and `visible_x_ticks` is longer
             than max_ticks then `visible_x_ticks` will be curtailed.
 
-
         log_scale
             True to plot prices against a log scale.
 
         display
             True to display created chart.
         """
         super().__init__(prices, title, visible_x_ticks, max_ticks, log_scale, display)
@@ -1708,38 +1708,36 @@
     def _get_mark_y_data(self):
         return self._y_data.values.tolist()
 
     @property
     def MarkCls(self) -> type[bq.Mark]:
         return bq.OHLC
 
-    def _tooltip_value(self, mark, data):
-        i = data["data"]["index"]
+    def _tooltip_value(self, mark: bq.OHLC, event: dict) -> str:
+        i = event["data"]["index"]
         row = self.data.iloc[i]
         color = mark.colors[0] if row.close >= row.open else mark.colors[1]
         style = self._tooltip_style(color=color, line_height=1.3)
         s = f"<p {style}>From: " + formatter_datetime(row.name.left)
         s += f"<br>To: {formatter_datetime(row.name.right)}"
         for line in ["open", "high", "low", "close"]:
             v = getattr(row, line)
             s += "<br>" + line.capitalize() + ": " + FORMATTERS[line](v)
         s += "</p>"
         return s
 
-    def _create_mark(self, **_) -> bq.OHLC:
-        return super()._create_mark(
-            format="ohlc",
-            marker="candle",
-            stroke="white",
-            stroke_width=0.5,
-            colors=["SkyBlue", "DarkOrange"],
-        )
+    def _create_mark(self, **kwargs) -> bq.OHLC:
+        kwargs.setdefault("stroke", "white")
+        kwargs.setdefault("stroke_width", 0.5)
+        kwargs.setdefault("colors", ["SkyBlue", "DarkOrange"])
+        return super()._create_mark(format="ohlc", marker="candle", **kwargs)
 
-    def _create_figure(self, **_) -> bq.Figure:
-        return super()._create_figure(padding_x=0.005)
+    def _create_figure(self, **kwargs) -> bq.Figure:
+        kwargs.setdefault("padding_x", 0.005)
+        return super()._create_figure(**kwargs)
 
     def _update_stroke_width(self):
         mask = self.STYLE.index.contains(len(self.plotted_x_ticks))
         stroke_width = self.STYLE.loc[mask, "stroke_width"].values[0]
         self.mark.stroke_width = stroke_width
 
     def update_presentation(self):
```

### Comparing `market_analy-0.2/src/market_analy/formatters.py` & `market_analy-0.2.3/src/market_analy/formatters.py`

 * *Files identical despite different names*

### Comparing `market_analy-0.2/src/market_analy/gui_parts.py` & `market_analy-0.2.3/src/market_analy/gui_parts.py`

 * *Files 2% similar despite different names*

```diff
@@ -485,15 +485,15 @@
             "names": ["stacked", "grouped"],
             "color": "blue",
             "tooltips": ["stacked", "grouped"],
         }
         super().__init__(**d)
 
 
-def _but(
+def create_icon_but(
     icon_name: str,
     tooltip: str,
     color: str,
     handler: Callable | None = None,
     **kwargs,
 ) -> vu.IconBut:
     """`IconButton` with tooltip and handler.
@@ -513,21 +513,23 @@
         signature:
             handler(widget, event, data)
 
         If not passed then handler can be subsequently set with:
             but.on_event('click', handler)
 
     **kwargs
-        Passed on to `IconBut`. Will not pass on parameters defined by method
-        to maintain legend button style.
+        Passed on to `IconBut`. Will not pass on parameters defined by
+        method to maintain legend button style.
     """
     kwargs["icon_name"] = icon_name
     kwargs["tooltip"] = tooltip
     kwargs["color"] = color
-    tt_kwargs = {"color": color}
+
+    dark = kwargs.get("dark", False) and (dark_color := kwargs.get("dark_color", False))
+    tt_kwargs = {"color": dark_color if dark else color}
     tt_kwargs = set_kwargs_from_dflt(tt_kwargs, TT_KWARGS_DFLT)
     tt_kwargs = set_kwargs_from_dflt(kwargs.pop("tt_kwargs", {}), tt_kwargs, deep=True)
     but = vu.IconBut(tt_kwargs=tt_kwargs, **kwargs)
     if handler is not None:
         but.on_event("click", handler)
     return but
 
@@ -542,15 +544,15 @@
         should have signature:
             handler(widget, event, data)
 
     **kwargs
         Passed on to `IconBut`. Will not pass on parameters defined by
         method to maintain legend button style.
     """
-    return _but(
+    return create_icon_but(
         icon_name="fa-list-alt",
         tooltip="Cycle legend location",
         color="white",
         handler=handler,
         **kwargs,
     )
 
@@ -565,15 +567,15 @@
         should have signature:
             handler(widget, event, data)
 
     **kwargs
         Passed on to `IconBut`. Will not pass on parameters defined by
         method to maintain legend button style.
     """
-    return _but(
+    return create_icon_but(
         icon_name="fa-dot-circle-o",
         tooltip="Rebase prices",
         color="orange",
         handler=handler,
         **kwargs,
     )
```

### Comparing `market_analy-0.2/src/market_analy/guis.py` & `market_analy-0.2.3/src/market_analy/guis.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,18 @@
     Bar chart GUI of precentage changes of multiple instruments.
 """
 
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
 from collections.abc import Callable
-from copy import copy
 from contextlib import contextmanager
 from typing import Literal
 
+import bqplot as bq
 from bqplot.interacts import Selector
 import exchange_calendars as xcals
 import IPython
 import ipyvuetify as v
 import ipywidgets as w
 import market_prices as mp
 from market_prices.intervals import TDInterval, PTInterval, to_ptinterval, ONE_DAY
@@ -188,15 +188,15 @@
         Notes
         -----
         Instance of this class will instantiated by `_create_mark`.
         """
 
     def _create_chart(
         self, data: pd.DataFrame | pd.Series, title: str | None, **kwargs
-    ):
+    ) -> charts.Base:
         """Create chart.
 
         Notes
         -----
         Not intended that subclass extends.
 
         `kwargs` receive kwargs as collected by constructor.
@@ -327,16 +327,16 @@
         for widget in self._widgets:
             widget.close()
 
     def delete(self):
         """Delete all gui widgets."""
         self.close()
         self.chart.delete()
-        for widget in copy(self._widgets):
-            del widget
+        for _ in range(len(self._widgets)):
+            del self._widgets[0]
 
     def display(self):
         """Display gui."""
         IPython.display.display(self._gui)
 
     def _update_chart(self, data: pd.DataFrame | pd.Series, title: str | None = None):
         """Update chart with new data."""
@@ -544,14 +544,15 @@
 
 class BasePrice(BaseVariableDates):
     """Base implementation for GUIs incorporating a price chart.
 
     GUI comprises:
 
     IconRow: Icons to undertake chart operations.
+    w.ToggleButtons: Toggle buttons to select interval (optional)
     Figure: plot
     wu.DateRangeSlider: slider to interactively set chart dates
     HtmlOutput: Housing for html output.
 
     TabsControl: cursor and selector tabs.
         Cursor tab:
             + and - toggle buttons to add or delete crosshairs to the plot.
@@ -576,14 +577,19 @@
 
         _chart_title -> str
 
     In addition, subclasses can optionally extend:
 
         Inherited methods as described by Base documentation.
 
+        The following class attributes introduced by this class:
+            _HAS_INTERVAL_SELECTOR : bool, default: True
+                Set to False on subclass to not include the
+                `w.ToggleButtons` that provides for changing tick interval.
+
         The following properties introduced by this class:
 
             _prices_kwargs -> dict:
                 Immutable chart kwargs. Subclass should extend to override
                 defaults and/or add immutable kwargs specific to
                 `ChartCls`.
 
@@ -608,22 +614,24 @@
         "30T",
         "15T",
         "5T",
         "2T",
         "1T",
     ]
     TICK_INTERVALS_PT = [to_ptinterval(ti) for ti in TICK_INTERVALS]
+    _HAS_INTERVAL_SELECTOR = True
 
     def __init__(
         self,
         analysis: analysis.Analysis,
         interval: mp.intervals.RowInterval | None = None,
         max_ticks: int | None = None,
-        log_scale=True,
-        display=True,
+        log_scale: bool = True,
+        display: bool = True,
+        chart_kwargs: dict | None = None,
         **kwargs,
     ):
         """Create GUI.
 
         Parameters
         ----------
         analysis
@@ -639,32 +647,37 @@
 
         log_scale
             True to chart prices against a log scale.
 
         display
             True to display created GUI.
 
+        chart_kwargs
+            Any kwargs to pass on to the chart class.
+
         **kwargs
             Period for which to plot prices. Passed as period parameters as
             described by market-prices documentation for `PricesCls.get`
             method where `PricesCls` is the class that was passed to
             `PricesCls` parameter of `mkt_anlaysis.Analysis` to intantiate
             `analysis`.
         """
         assert issubclass(self.ChartCls, charts.BasePrice)
+        chart_kwargs = {} if chart_kwargs is None else chart_kwargs
         ptinterval = None if interval is None else to_ptinterval(interval)
         self._analysis = analysis
         self._initial_price_params: dict  # set by _get_initial_prices
         prices = self._get_initial_prices(ptinterval, kwargs)
         super().__init__(
             data=prices,
             title=self._chart_title,
             max_ticks=max_ticks,
             display=display,
             log_scale=log_scale,
+            **chart_kwargs,
         )
 
     @property
     def SelectorCls(self) -> type[FastIntervalSelectorDD]:
         return FastIntervalSelectorDD
 
     @property
@@ -803,15 +816,18 @@
     # GUI BOX
     def _create_gui_parts(self):
         super()._create_gui_parts()
         self._crosshairs = Crosshairs(self.chart.figure)
         self._set_mark_handlers()
         self._icon_row_top: gui_parts.IconRowTop = self._create_icon_row_top()
 
-        if self.chart.tick_interval not in self.TICK_INTERVALS_PT:
+        if (
+            not self._HAS_INTERVAL_SELECTOR
+            or self.chart.tick_interval not in self.TICK_INTERVALS_PT
+        ):
             self._interval_selector: w.ToggleButtons | None = None
         else:
             self._interval_selector = self._create_intrvl_slctr()
 
         self.date_slider: wu.DateRangeSlider = self._create_date_slider()
         self._html_output: w.HTML = self._create_html_output()
         self.tabs_control: gui_parts.TabsControl = self._create_tabs_control()
@@ -924,15 +940,15 @@
     # MAX ADV/DEC
     def _get_max_chg(
         self, direction: Literal["max_adv", "max_dec"], style=False, **kwargs
     ):
         interval = self._operation_interval
         method = getattr(self._analysis, direction)
         return method(
-            interval=self._interval_selector.value,
+            interval=self._tick_interval,
             start=interval.left,
             end=interval.right,
             style=style,
             **kwargs,
         )
 
     def _max_chg_html(self, method_name: Literal["max_adv", "max_dec"]):
@@ -1470,21 +1486,21 @@
 
     def _reset(self):
         super()._reset()
         self.chart.opaque()
 
 
 class ChartOHLC(BasePrice):
-    """GUI to display and interact with a OHLC Chart."""
+    """GUI to display and interact with a OHLC Chart.
 
-    from_breaks = pd.IntervalIndex.from_breaks
-    STYLE = pd.DataFrame(
-        {"stroke_width": [1.0, 0.8, 0.5, 0.3, 0.1]},
-        index=from_breaks([0, 50, 70, 180, 548, 365 * 100], closed="right"),
-    )
+    Properties (in addition to inhertied)
+    ----------
+    last_selected -> pd.Series:
+        Price data row corresponding with most recently clicked bar.
+    """
 
     @property
     def ChartCls(self) -> type[charts.Base]:
         return charts.OHLC
 
     @property
     def _chart_title(self) -> str:
@@ -1511,15 +1527,15 @@
             "color": "white",
             "enable": False,
             "scale": self.chart.scales["x"],
             "figure": self.chart.figure,
         }
         return self.SelectorCls(**kw_args)
 
-    def _add_crosshair_handler(self, mark, event):
+    def _add_crosshair_handler(self, mark: bq.OHLC, event: dict):
         if self.tabs_control.cursor_toggle.selected != "plus":
             return
         index = event["data"]["index"]
         x = self.chart.mark.x[index]
 
         # NOTE suspect this part will be refactored out to somewhere more general.
         higher, lower = False, False
@@ -1531,16 +1547,36 @@
             lower = data[index][2] < data[index - i][2]
             if i == 100:
                 raise StopIteration("breaking infinite loop.")
         y = data[index][1] if higher else data[index][2]
 
         self.add_crosshair(x=x, y=y)
 
+    def _display_mark_data(self, mark: bq.OHLC, event: dict):
+        s = self.chart._tooltip_value(mark, event)
+        self.html_output.display(s)
+
+    @property
+    def last_selected(self) -> pd.Series:
+        """Price data row corresponding with most recently clicked mark."""
+        return self._last_selected
+
+    def _selected_mark_handler(self, mark: bq.OHLC, event: dict):
+        self._display_mark_data(mark, event)
+        i = event["data"]["index"]
+        self._last_selected = self.chart.data.iloc[i]
+
+    def _mark_handler(self, mark: bq.OHLC, event: dict):
+        if self.tabs_control.cursor_toggle.selected == "plus":
+            self._add_crosshair_handler(mark, event)
+        else:
+            self._selected_mark_handler(mark, event)
+
     def _set_mark_handlers(self):
-        self.chart.mark.on_element_click(self._add_crosshair_handler)
+        self.chart.mark.on_element_click(self._mark_handler)
 
 
 class PctChg(BaseVariableDates):
     """GUI for bar chart showing precentage changes of single instrument.
 
     GUI comprises:
 
@@ -1589,15 +1625,15 @@
     def ChartCls(self) -> type[charts.Base]:
         return charts.PctChgBar
 
     @property
     def SelectorCls(self) -> type[Selector] | None:
         return None
 
-    def _create_date_slider(self, **kwargs):
+    def _create_date_slider(self, **_):
         return super()._create_date_slider(layout={"margin": "30px 0 15px 0"})
 
     def _create_gui_parts(self):
         super()._create_gui_parts()
         self._icon_row_top = self._create_icon_row_top()
         if len(self.chart.x_ticks) > self.chart.max_ticks:
             self.date_slider: wu.DateRangeSlider = self._create_date_slider()
```

### Comparing `market_analy-0.2/src/market_analy/utils/bq_utils.py` & `market_analy-0.2.3/src/market_analy/utils/bq_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # Colors for use on charts with dark backgrounds.
 COLORS_DARK_8 = [
     "yellow",
     "springgreen",
     "hotpink",
     "darkorange",
     "lightskyblue",
-    "beige",
+    "burlywood",
     "red",
     "mediumorchid",
 ]
 
 LEGEND_LOCATIONS = [
     "top-left",
     "top",
@@ -55,20 +55,20 @@
 
 def discontinuous_date_to_timestamp(value: np.int64) -> pd.Timestamp:
     """Convert integer representing posix to pd.Timestamp.
 
     Parameters
     ----------
     value
-        Value of an OrdinalScale represtenting a date which require as
+        Value of an OrdinalScale representing a date which require as
         pd.Timestamp.
     """
     # utc version of fromtimestamp ensures that operation is the inverse
     # of dates_to_posix
-    return pd.Timestamp.fromtimestamp(value / 1000)
+    return pd.Timestamp.fromtimestamp(value / 1000, tz="UTC").tz_convert(None)
 
 
 class _LevelLine(Lines):
     """Create line at specific level along a scale.
 
     Creates line on `figure` in `direction` at `level` based on either
     `scale`['y'] or `scale`['x'] (as corresponds with `direction`). (Takes
```

### Comparing `market_analy-0.2/src/market_analy/utils/dict_utils.py` & `market_analy-0.2.3/src/market_analy/utils/dict_utils.py`

 * *Files identical despite different names*

### Comparing `market_analy-0.2/src/market_analy/utils/ipyvuetify_utils.py` & `market_analy-0.2.3/src/market_analy/utils/ipyvuetify_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,46 +213,47 @@
         dark_color=DARK,
         dark=False,
         tooltip: str | None = None,
         tt_kwargs: dict | None = None,
         **kwargs,
     ):
         self.tt: vue.Tooltip
-        self._dark_icon_color = dark_color
-        self._light_icon_color = color
+        self.color_dark = dark_color
+        self.color_light = color
 
         assert "children" not in kwargs
         kwargs.setdefault("height", self.icon_dim)
         kwargs.setdefault("width", self.icon_dim)
         kwargs.setdefault("min_width", self.icon_dim)
         kwargs.setdefault("elevation", 5)
         kwargs.setdefault("class_", self.def_class_)
         kwargs.setdefault("icon", True)
 
-        color = self._dark_icon_color if dark else self._light_icon_color
+        color = self.color_dark if dark else self.color_light
 
         super().__init__(
             children=[vue.Icon(children=[icon_name], small=True, color=color)], **kwargs
         )
 
     @property
     def icon_color(self) -> str:
         return self.children[0].color
 
     @icon_color.setter
     def icon_color(self, color: str):
         self.children[0].color = color
+        self.tt.color = color
 
     def darken(self):
         """Darken icon color."""
-        self.icon_color = self._dark_icon_color
+        self.icon_color = self.color_dark
 
     def lighten(self):
         """Lighten icon color."""
-        self.icon_color = self._light_icon_color
+        self.icon_color = self.color_light
 
 
 class ToggleIcon(IconBut):
     """Selectable `IconBut`.
 
     Clicking `IconBut` toggles selection. Optionally:
         Define selected and unselected icon colors.
```

### Comparing `market_analy-0.2/src/market_analy/utils/ipywidgets_utils.py` & `market_analy-0.2.3/src/market_analy/utils/ipywidgets_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,60 +32,98 @@
 import ipywidgets as w  # type: ignore[import]
 import pandas as pd
 
 
 class Timer:
     """Timer.
 
-    See https://ipywidgets.readthedocs.io/en/latest/examples/Widget%20Events.html#Traitlet-events
+    Ref:
+    https://ipywidgets.readthedocs.io/en/latest/examples/Widget%20Events.html#debouncing
     """
 
     def __init__(self, timeout, callback):
         self._timeout = timeout
         self._callback = callback
-        self._task = asyncio.ensure_future(self._job())
 
     async def _job(self):
         await asyncio.sleep(self._timeout)
         self._callback()
 
+    def start(self):
+        self._task = asyncio.ensure_future(self._job())
+
     def cancel(self):
         self._task.cancel()
 
 
+def debounce(wait):
+    """Decorator to postpone callback.
+
+    Postpones callback until `wait` seconds have elapsed during which the
+    value remains unchanged.
+
+    Ref:
+    https://ipywidgets.readthedocs.io/en/latest/examples/Widget%20Events.html#debouncing
+    """
+
+    def decorator(fn):
+        timer = None
+        timer2 = None
+
+        def debounced(*args, **kwargs):
+            nonlocal timer, timer2
+
+            def call_it():
+                fn(*args, **kwargs)
+
+            if timer is not None:
+                timer.cancel()
+            if timer2 is not None:
+                timer2.cancel()
+            timer = Timer(wait, call_it)
+            timer.start()
+            timer2 = Timer(wait * 2, call_it)
+            timer2.start()
+
+        return debounced
+
+    return decorator
+
+
 def throttle(wait) -> Callable:
     """Decorator to limit callbacks.
 
-    Limits decorated callback to being called no more than once every wait
-    period.
+    Limits decorated callback to being called no more than once every
+    `wait` period.
 
-    See https://ipywidgets.readthedocs.io/en/latest/examples/Widget%20Events.html#Traitlet-events
+    Ref:
+    https://ipywidgets.readthedocs.io/en/latest/examples/Widget%20Events.html#throttling
     """
 
     def decorator(fn: Callable) -> Callable:
         time_of_last_call = 0
-        scheduled = False
+        scheduled, timer = False, None
         new_args, new_kwargs = None, None
 
         def throttled(*args, **kwargs):
-            nonlocal new_args, new_kwargs, time_of_last_call, scheduled
+            nonlocal new_args, new_kwargs, time_of_last_call, scheduled, timer
 
             def call_it():
-                nonlocal new_args, new_kwargs, time_of_last_call, scheduled
+                nonlocal new_args, new_kwargs, time_of_last_call, scheduled, timer
                 time_of_last_call = time()
                 fn(*new_args, **new_kwargs)
                 scheduled = False
 
             time_since_last_call = time() - time_of_last_call
-            new_args = args
-            new_kwargs = kwargs
+            new_args, new_kwargs = args, kwargs
             if not scheduled:
-                new_wait = max(0, wait - time_since_last_call)
-                Timer(new_wait, call_it)
                 scheduled = True
+                new_wait = max(0, wait - time_since_last_call)
+                timer = Timer(new_wait, call_it)
+                timer.start()
 
         return throttled
 
     return decorator
 
 
 class NamedChildren:
```

### Comparing `market_analy-0.2/src/market_analy/utils/list_utils.py` & `market_analy-0.2.3/src/market_analy/utils/list_utils.py`

 * *Files identical despite different names*

### Comparing `market_analy-0.2/src/market_analy/utils/mkt_prices_utils.py` & `market_analy-0.2.3/src/market_analy/utils/mkt_prices_utils.py`

 * *Files identical despite different names*

### Comparing `market_analy-0.2/src/market_analy/utils/pandas_utils.py` & `market_analy-0.2.3/src/market_analy/utils/pandas_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,15 +240,17 @@
     >>> left = pd.date_range(
     ...     '2021-05-01 12:00', periods=5, freq='1H', tz='US/Central'
     ... )
     >>> right = left + pd.Timedelta(30, 'T')
     >>> index = pd.IntervalIndex.from_arrays(left, right)
     >>> index.right.tz
     <DstTzInfo 'US/Central' LMT-1 day, 18:09:00 STD>
-    >>> new_index = interval_index_new_tz(index, tz="UTC")
+    >>> new_index = interval_index_new_tz(index, tz=pytz.UTC)
+    >>> new_index.left.tz == new_index.right.tz == pytz.UTC
+    True
     >>> new_index.left.tz.zone == new_index.right.tz.zone == "UTC"
     True
     >>> tz_naive = interval_index_new_tz(index, tz=None)
     >>> tz_naive[0].left
     Timestamp('2021-05-01 12:00:00')
     """
     indices = []
```

### Comparing `market_analy-0.2/src/market_analy.egg-info/PKG-INFO` & `market_analy-0.2.3/src/market_analy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: market-analy
-Version: 0.2
+Version: 0.2.3
 Summary: Analysis of exchange-listed financial instruments
 Author: Marcus Read
 Author-email: marcusaread@gmail.com
 License: MIT License
 Project-URL: homepage, https://github.com/maread99/market_analy
 Project-URL: documentation, https://github.com/maread99/market_analy
 Project-URL: Issue Tracker, https://github.com/maread99/market_analy/issues
@@ -30,14 +30,20 @@
 Description-Content-Type: text/markdown
 Provides-Extra: jupyter
 Provides-Extra: tests
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 <!-- NB any links not defined as aboslute will not resolve on PyPI page -->
+<div align="center">
+  <img src="docs/splash.png"><br>
+</div>
+
+-----------------
+
 # market_analy
 
 [![PyPI](https://img.shields.io/pypi/v/market-analy)](https://pypi.org/project/market-analy/) ![Python Support](https://img.shields.io/pypi/pyversions/market-analy) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 A python package to analyse financial instruments.
 
 There's a load of great financial libraries out there for Technical Analysis, Charting, Backtesting, Portfolio Analysis etc. This library isn't reinventing the wheel (not intentionally anyway), rather it provides functions and interactive charting that I think are useful and couldn't find elsewhere. It's not comprehensive, but rather fills some of the gaps.
@@ -102,19 +108,27 @@
 ### `market-prices` dependency
 `market-analy` depends on the [market-prices][market-prices] library for price data. This provides for functionality including:
 * defining analysis periods in terms of number of sessions and trading minutes rather than calendar days and times.
 * complete data sets regardless of liquidity (regular data points during market hours, no data points outside of market hours).
 
 Most of the arguments available to the market-prices `get` function can be passed directly to the `market_analy` functions. See the [market-prices][market-prices] documentation for further info.
 
-## Disclaimers
-`market-analy` should not be assumed sufficiently reliable to undertake analysis intended to inform investment decisions. Users should inspect the source code and the test suite of the library and its dependencies in order to make their own assessment of the packages' suitability for their purposes. **The `market-analy` package is used entirely at the user's own risk.**
+## Release schedule, bugs, development and feedback
+
+The first beta version of `market_analy` was released Feb 2023. It's anticipated that functionality to define and visually interrogate trends will be added later in 2023.
+
+The project is immature. Whilst it's not anticipated that major changes will be made to the existing public side, they could be. All that's under-the-bonnet is subject to change as the project evolves. The `guis` module in particular won't permit much further development without overhauling the current inheritance-based approach to a compositional one.
 
 The test suite is limited. It's pretty much guaranteed that there are bugs. Please raise an [issue](https://github.com/maread99/market_analy/issues) if you find one or come across unexpected behaviour.
 
+Please use [discussions](https://github.com/maread99/market_analy/discussions) to make any suggestions and offer general feedback.
+
+## Disclaimers
+`market-analy` should not be assumed sufficiently reliable to undertake analysis intended to inform investment decisions. Users should inspect the source code and the test suite of the library and its dependencies in order to make their own assessment of the packages' suitability for their purposes. **The `market-analy` package is used entirely at the user's own risk.**
+
 The default `market_prices.PricesYahoo` class gets data from publically available Yahoo APIs. **See the [Disclaimers section of the market-prices README](https://github.com/maread99/market_prices#disclaimers) for conditions of use**, including restrictions.
 
 ## Alternative packages
 
 * [awesome-quant](https://github.com/wilsonfreitas/awesome-quant) offers an extensive listing of libraries for all things finance.
 
 ## License
```

### Comparing `market_analy-0.2/src/market_analy.egg-info/SOURCES.txt` & `market_analy-0.2.3/src/market_analy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.py
+docs/splash.png
 etc/requirements_dev.txt
 etc/requirements_tests.txt
 etc/requirements/requirements.txt
 etc/requirements/why_here.txt
 src/market_analy/__init__.py
 src/market_analy/_version.py
 src/market_analy/analysis.py
```

