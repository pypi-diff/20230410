# Comparing `tmp/circuitpython-async-button-1.1.0.tar.gz` & `tmp/circuitpython-async-button-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-async-button-1.1.0.tar", last modified: Tue Jan 17 15:10:41 2023, max compression
+gzip compressed data, was "circuitpython-async-button-1.2.0.tar", last modified: Mon Apr 10 19:25:31 2023, max compression
```

## Comparing `circuitpython-async-button-1.1.0.tar` & `circuitpython-async-button-1.2.0.tar`

### file list

```diff
@@ -1,60 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:41.211791 circuitpython-async-button-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:41.203791 circuitpython-async-button-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:41.203791 circuitpython-async-button-1.1.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:41.207791 circuitpython-async-button-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:41.207791 circuitpython-async-button-1.1.0/.reuse/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:41.207791 circuitpython-async-button-1.1.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-01-17 15:10:41.207791 circuitpython-async-button-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)    11810 2023-01-17 15:10:34.000000 circuitpython-async-button-1.1.0/async_button.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:41.207791 circuitpython-async-button-1.1.0/circuitpython_async_button.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-01-17 15:10:41.000000 circuitpython-async-button-1.1.0/circuitpython_async_button.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-01-17 15:10:41.000000 circuitpython-async-button-1.1.0/circuitpython_async_button.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 15:10:41.000000 circuitpython-async-button-1.1.0/circuitpython_async_button.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-17 15:10:41.000000 circuitpython-async-button-1.1.0/circuitpython_async_button.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-17 15:10:41.000000 circuitpython-async-button-1.1.0/circuitpython_async_button.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:41.207791 circuitpython-async-button-1.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:41.207791 circuitpython-async-button-1.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/docs/events.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/docs/events.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/docs/timing_double.json
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/docs/timing_long.json
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/docs/timing_single.json
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/docs/timing_triple.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:41.207791 circuitpython-async-button-1.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-01-17 15:10:34.000000 circuitpython-async-button-1.1.0/examples/async_button_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-01-17 15:10:34.000000 circuitpython-async-button-1.1.0/examples/async_simplebutton_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-01-17 15:10:34.000000 circuitpython-async-button-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-01-17 15:10:27.000000 circuitpython-async-button-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 15:10:41.211791 circuitpython-async-button-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:41.207791 circuitpython-async-button-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:34.000000 circuitpython-async-button-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11513 2023-01-17 15:10:34.000000 circuitpython-async-button-1.1.0/tests/test_async_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-01-17 15:10:34.000000 circuitpython-async-button-1.1.0/tests/test_async_simple_button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:31.368247 circuitpython-async-button-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:31.360247 circuitpython-async-button-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:31.360247 circuitpython-async-button-1.2.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:31.364247 circuitpython-async-button-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:31.364247 circuitpython-async-button-1.2.0/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:31.364247 circuitpython-async-button-1.2.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-04-10 19:25:31.368247 circuitpython-async-button-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-04-10 19:25:21.000000 circuitpython-async-button-1.2.0/async_button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:31.364247 circuitpython-async-button-1.2.0/circuitpython_async_button.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-04-10 19:25:31.000000 circuitpython-async-button-1.2.0/circuitpython_async_button.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-10 19:25:31.000000 circuitpython-async-button-1.2.0/circuitpython_async_button.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:25:31.000000 circuitpython-async-button-1.2.0/circuitpython_async_button.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-10 19:25:31.000000 circuitpython-async-button-1.2.0/circuitpython_async_button.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-10 19:25:31.000000 circuitpython-async-button-1.2.0/circuitpython_async_button.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:31.368247 circuitpython-async-button-1.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:31.368247 circuitpython-async-button-1.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/events.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/events.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/timing_double.json
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/timing_long.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/timing_single.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/timing_triple.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:31.368247 circuitpython-async-button-1.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-10 19:25:21.000000 circuitpython-async-button-1.2.0/examples/async_button_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-10 19:25:21.000000 circuitpython-async-button-1.2.0/examples/async_multibutton_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-10 19:25:21.000000 circuitpython-async-button-1.2.0/examples/async_simplebutton_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-10 19:25:21.000000 circuitpython-async-button-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 19:25:31.368247 circuitpython-async-button-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:31.368247 circuitpython-async-button-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:21.000000 circuitpython-async-button-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-04-10 19:25:21.000000 circuitpython-async-button-1.2.0/tests/test_async_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-10 19:25:21.000000 circuitpython-async-button-1.2.0/tests/test_async_multi_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-10 19:25:21.000000 circuitpython-async-button-1.2.0/tests/test_async_simple_button.py
```

### Comparing `circuitpython-async-button-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-async-button-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.1.0/.gitignore` & `circuitpython-async-button-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.1.0/.pre-commit-config.yaml` & `circuitpython-async-button-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.1.0/.pylintrc` & `circuitpython-async-button-1.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.1.0/CODE_OF_CONDUCT.md` & `circuitpython-async-button-1.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.1.0/LICENSE` & `circuitpython-async-button-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.1.0/LICENSES/CC-BY-4.0.txt` & `circuitpython-async-button-1.2.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.1.0/LICENSES/MIT.txt` & `circuitpython-async-button-1.2.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.1.0/LICENSES/Unlicense.txt` & `circuitpython-async-button-1.2.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.1.0/PKG-INFO` & `circuitpython-async-button-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-async-button
-Version: 1.1.0
+Version: 1.2.0
 Summary: a library for reading buttons using asyncio
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/furbrain/CircuitPython_async_button
 Keywords: adafruit,blinka,circuitpython,micropython,async_button,async,asyncio,countio,keypad,button,press
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-async-button-1.1.0/README.rst` & `circuitpython-async-button-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.1.0/async_button.py` & `circuitpython-async-button-1.2.0/async_button.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,23 +23,24 @@
   https://github.com/adafruit/Adafruit_CircuitPython_asyncio
 
 * CircuitPython ticks module:
   https://github.com/adafruit/Adafruit_CircuitPython_Ticks
 """
 
 
-__version__ = "1.1.0"
+__version__ = "1.2.0"
 __repo__ = "https://github.com/furbrain/CircuitPython_async_button.git"
 
 import asyncio
+from asyncio import Task, Event
 
 from adafruit_ticks import ticks_add, ticks_less, ticks_ms
 
 try:
-    from typing import Dict, Sequence, Awaitable
+    from typing import Dict, Sequence, Awaitable, Any, Union
 except ImportError:
     pass
 
 import digitalio
 import keypad
 from microcontroller import Pin
 import countio
@@ -96,14 +97,60 @@
         with countio.Counter(self.pin, edge=edge, pull=self.pull) as counter:
             while True:
                 if counter.count > 0:
                     return
                 await asyncio.sleep(self.interval)
 
 
+class TaskWrapper:
+    """
+    Create a task to run coro, then trigger event when finished
+    Shouldn't really need this but CircuitPython does not have asyncio.wait or Task.result()
+    """
+
+    def __init__(self, coro: Awaitable, event: Event):
+        """
+        :param Awaitable coro: coroutine to run
+        :param asyncio.Event event:
+        """
+        self._result = None
+        self.coro = coro
+        self.event = event
+        self.task = asyncio.create_task(self._wait())
+
+    async def _wait(self):
+        self._result = await self.coro
+        self.event.set()
+
+    def done(self):
+        """
+        Check whether task has completed
+
+        :return: True if task has completed
+        """
+        return self.task.done()
+
+    def result(self):
+        """
+        Get return value from task
+
+        :return: Whatever the task returned.
+        """
+        if not self.done():
+            raise AssertionError("Task has not yet completed")
+        return self._result
+
+    def cancel(self):
+        """
+        Cancel the task
+        :return:
+        """
+        self.task.cancel()
+
+
 class Button:
     """
     This object will monitor the specified pin for changes and will report
     single, double, triple and long_clicks. It creates a background `asyncio` process
     that will monitor the button. The `events` chapter in the documentation shows when the
     various events are triggered
     """
@@ -247,44 +294,45 @@
             self.last_click = self.SINGLE
 
     def _trigger(self, event: int):
         evt = self.events[event]
         evt.set()
         evt.clear()
 
-    @staticmethod
-    async def _set_event_when_done(coro: Awaitable, event: asyncio.Event):
-        await coro
-        event.set()
-
-    async def wait(self, click_types: Sequence[int] = ALL_EVENTS):
+    async def wait(self, click_types: Union[int, Sequence[int]] = ALL_EVENTS):
         """
         Wait for the first of the specified events.
 
-        :param List[int] click_types: One or more events to listen for. Default is to listen
-          for all events
+        :param (List[int] | int) click_types: List of events to listen for. You can also pass a
+          single event type in. Default is to listen for all events.
         :return: A list of the clicks that actually happened.
 
         :example:
           .. code-block:: python
 
             >>> async def get_click():
             >>>     # wait for a double or triple click
             >>>     clicks = await button.wait((Button.DOUBLE, Button.TRIPLE))
             >>>     if Button.DOUBLE in clicks:
             >>>         # do something
 
         """
-        evts: Dict[int, asyncio.Task] = {}
+        if isinstance(click_types, int):
+            click_types = [click_types]
+        # shortcut for efficiency: if only one click type awaited, just await that
+        if len(click_types) == 1:
+            await self.events[click_types[0]].wait()
+            return [click_types[0]]
+
+        # multiple click types - needs more complex algorithm
+        evts: Dict[int, TaskWrapper] = {}
         one_event_done = asyncio.Event()
         for evt_type in click_types:
             coro = self.events[evt_type].wait()
-            evts[evt_type] = asyncio.create_task(
-                self._set_event_when_done(coro, one_event_done)
-            )
+            evts[evt_type] = TaskWrapper(coro, one_event_done)
         await one_event_done.wait()
         if len(evts) > 1:
             await asyncio.sleep(0)  # ensure all event types get an opportunity to run
         results = []
         for evt_type, evt in evts.items():
             if evt.done():
                 results.append(evt_type)
@@ -303,7 +351,62 @@
 
     def deinit(self):
         """
         Deinitialise object and stop the background task
         """
         self.monitor_task.cancel()
         self.keys.deinit()
+
+
+class MultiButton:
+    """
+    This class allows you to await the first click from any of two or more buttons
+    """
+
+    def __init__(self, **kwargs):
+        """
+
+        :param kwargs: pass each button that you want to be able to listen to with its name
+
+        :example:
+          .. code-block:: python
+
+            >>> multi = MultiButton(a = button_a, b=button_b)
+            >>> button, result = await multi.wait(a=Button.SINGLE, b= (Button.DOUBLE, Button.LONG))
+            >>> # Long click on button B
+            >>> print(button, result) # "b", Button.Long
+        """
+        for button in kwargs.values():
+            if not isinstance(button, Button):
+                raise TypeError("Must pass in async_button.Button as parameters")
+        self.buttons: Dict[Any, Button] = kwargs
+
+    async def wait(self, **kwargs):
+        """
+        Wait for any specified clicks
+
+        :param kwargs: pass by keyword what clicks you want to listen for
+        :return: button, click type
+        :example:
+          .. code-block:: python
+
+            >>> multi = MultiButton(a = button_a, b=button_b)
+            >>> button, result = await multi.wait(a=Button.SINGLE, b= (Button.DOUBLE, Button.LONG))
+            >>> # Long click on button B
+            >>> print(button, result) # "b", Button.Long
+        """
+        if len(kwargs) == 1:
+            button = list(kwargs)[0]
+            results = await self.buttons[button].wait(kwargs[button])
+            return button, results[0]
+        tasks: Dict[Any, Task] = {}
+        click_happened = asyncio.Event()
+        for key, value in kwargs.items():
+            tasks[key] = TaskWrapper(self.buttons[key].wait(value), click_happened)
+        await click_happened.wait()
+        result = (None, None)
+        for key, task in tasks.items():
+            if task.done():
+                result = (key, task.result()[0])
+            else:
+                task.cancel()
+        return result
```

### Comparing `circuitpython-async-button-1.1.0/circuitpython_async_button.egg-info/PKG-INFO` & `circuitpython-async-button-1.2.0/circuitpython_async_button.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-async-button
-Version: 1.1.0
+Version: 1.2.0
 Summary: a library for reading buttons using asyncio
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/furbrain/CircuitPython_async_button
 Keywords: adafruit,blinka,circuitpython,micropython,async_button,async,asyncio,countio,keypad,button,press
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-async-button-1.1.0/circuitpython_async_button.egg-info/SOURCES.txt` & `circuitpython-async-button-1.2.0/circuitpython_async_button.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -37,11 +37,13 @@
 docs/timing_double.json
 docs/timing_long.json
 docs/timing_single.json
 docs/timing_triple.json
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/async_button_test.py
+examples/async_multibutton_test.py
 examples/async_simplebutton_test.py
 tests/__init__.py
 tests/test_async_button.py
+tests/test_async_multi_button.py
 tests/test_async_simple_button.py
```

### Comparing `circuitpython-async-button-1.1.0/docs/_static/favicon.ico` & `circuitpython-async-button-1.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.1.0/docs/conf.py` & `circuitpython-async-button-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.1.0/docs/events.rst` & `circuitpython-async-button-1.2.0/docs/events.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.1.0/docs/index.rst` & `circuitpython-async-button-1.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.1.0/docs/timing_double.json` & `circuitpython-async-button-1.2.0/docs/timing_double.json`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.1.0/docs/timing_long.json` & `circuitpython-async-button-1.2.0/docs/timing_long.json`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.1.0/docs/timing_single.json` & `circuitpython-async-button-1.2.0/docs/timing_single.json`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.1.0/docs/timing_triple.json` & `circuitpython-async-button-1.2.0/docs/timing_triple.json`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.1.0/examples/async_button_test.py` & `circuitpython-async-button-1.2.0/examples/async_button_test.py`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.1.0/examples/async_simplebutton_test.py` & `circuitpython-async-button-1.2.0/examples/async_simplebutton_test.py`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.1.0/pyproject.toml` & `circuitpython-async-button-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-async-button"
 description = "a library for reading buttons using asyncio"
-version = "1.1.0"
+version = "1.2.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/furbrain/CircuitPython_async_button"}
 keywords = [
     "adafruit",
```

### Comparing `circuitpython-async-button-1.1.0/tests/test_async_button.py` & `circuitpython-async-button-1.2.0/tests/test_async_button.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,14 +116,20 @@
 
     async def test_single_click(self):
         self.button = FastButton(self.pin, True)
         self.button_timings = [0.10, 0.20]
         await self.wait_event_with_timeout([async_button.Button.SINGLE])
         self.assertAlmostEqual(self.time_count, 0.20, delta=0.1)
 
+    async def test_single_click_specified_without_list(self):
+        self.button = FastButton(self.pin, True)
+        self.button_timings = [0.10, 0.20]
+        await self.wait_event_with_timeout(async_button.Button.SINGLE)
+        self.assertAlmostEqual(self.time_count, 0.20, delta=0.1)
+
     async def test_double_click(self):
         self.button = FastButton(self.pin, True)
         self.button_timings = [0.10, 0.30, 0.5, 0.7]
         await self.wait_event_with_timeout([async_button.Button.DOUBLE])
         self.assertAlmostEqual(self.time_count, 0.70, delta=0.1)
 
     async def test_double_click_not_when_disabled(self):
```

### Comparing `circuitpython-async-button-1.1.0/tests/test_async_simple_button.py` & `circuitpython-async-button-1.2.0/tests/test_async_simple_button.py`

 * *Files identical despite different names*

