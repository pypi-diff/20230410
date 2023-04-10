# Comparing `tmp/circuitpython-async-button-1.2.0.tar.gz` & `tmp/circuitpython-async-button-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-async-button-1.2.0.tar", last modified: Mon Apr 10 19:25:31 2023, max compression
+gzip compressed data, was "circuitpython-async-button-1.2.1.tar", last modified: Mon Apr 10 19:57:58 2023, max compression
```

## Comparing `circuitpython-async-button-1.2.0.tar` & `circuitpython-async-button-1.2.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:31.368247 circuitpython-async-button-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:31.360247 circuitpython-async-button-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:31.360247 circuitpython-async-button-1.2.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:31.364247 circuitpython-async-button-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:31.364247 circuitpython-async-button-1.2.0/.reuse/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:31.364247 circuitpython-async-button-1.2.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-04-10 19:25:31.368247 circuitpython-async-button-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-04-10 19:25:21.000000 circuitpython-async-button-1.2.0/async_button.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:31.364247 circuitpython-async-button-1.2.0/circuitpython_async_button.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-04-10 19:25:31.000000 circuitpython-async-button-1.2.0/circuitpython_async_button.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-10 19:25:31.000000 circuitpython-async-button-1.2.0/circuitpython_async_button.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:25:31.000000 circuitpython-async-button-1.2.0/circuitpython_async_button.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-10 19:25:31.000000 circuitpython-async-button-1.2.0/circuitpython_async_button.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-10 19:25:31.000000 circuitpython-async-button-1.2.0/circuitpython_async_button.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:31.368247 circuitpython-async-button-1.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:31.368247 circuitpython-async-button-1.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/events.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/events.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/timing_double.json
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/timing_long.json
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/timing_single.json
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/docs/timing_triple.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:31.368247 circuitpython-async-button-1.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-10 19:25:21.000000 circuitpython-async-button-1.2.0/examples/async_button_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-10 19:25:21.000000 circuitpython-async-button-1.2.0/examples/async_multibutton_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-10 19:25:21.000000 circuitpython-async-button-1.2.0/examples/async_simplebutton_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-10 19:25:21.000000 circuitpython-async-button-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-10 19:25:10.000000 circuitpython-async-button-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 19:25:31.368247 circuitpython-async-button-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:31.368247 circuitpython-async-button-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:21.000000 circuitpython-async-button-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-04-10 19:25:21.000000 circuitpython-async-button-1.2.0/tests/test_async_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-10 19:25:21.000000 circuitpython-async-button-1.2.0/tests/test_async_multi_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-10 19:25:21.000000 circuitpython-async-button-1.2.0/tests/test_async_simple_button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:57:58.071371 circuitpython-async-button-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:57:58.063371 circuitpython-async-button-1.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:57:58.067371 circuitpython-async-button-1.2.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:57:58.067371 circuitpython-async-button-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:57:58.067371 circuitpython-async-button-1.2.1/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:57:58.067371 circuitpython-async-button-1.2.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-04-10 19:57:58.071371 circuitpython-async-button-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-04-10 19:57:50.000000 circuitpython-async-button-1.2.1/async_button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:57:58.067371 circuitpython-async-button-1.2.1/circuitpython_async_button.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-04-10 19:57:58.000000 circuitpython-async-button-1.2.1/circuitpython_async_button.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-10 19:57:58.000000 circuitpython-async-button-1.2.1/circuitpython_async_button.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:57:58.000000 circuitpython-async-button-1.2.1/circuitpython_async_button.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-10 19:57:58.000000 circuitpython-async-button-1.2.1/circuitpython_async_button.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-10 19:57:58.000000 circuitpython-async-button-1.2.1/circuitpython_async_button.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:57:58.071371 circuitpython-async-button-1.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:57:58.071371 circuitpython-async-button-1.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/events.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/events.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/timing_double.json
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/timing_long.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/timing_single.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/timing_triple.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:57:58.071371 circuitpython-async-button-1.2.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-10 19:57:50.000000 circuitpython-async-button-1.2.1/examples/async_button_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-10 19:57:50.000000 circuitpython-async-button-1.2.1/examples/async_multibutton_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-10 19:57:50.000000 circuitpython-async-button-1.2.1/examples/async_simplebutton_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-10 19:57:50.000000 circuitpython-async-button-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 19:57:58.071371 circuitpython-async-button-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:57:58.071371 circuitpython-async-button-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:57:50.000000 circuitpython-async-button-1.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-04-10 19:57:50.000000 circuitpython-async-button-1.2.1/tests/test_async_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-10 19:57:50.000000 circuitpython-async-button-1.2.1/tests/test_async_multi_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-10 19:57:50.000000 circuitpython-async-button-1.2.1/tests/test_async_simple_button.py
```

### Comparing `circuitpython-async-button-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-async-button-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.0/.gitignore` & `circuitpython-async-button-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.0/.pre-commit-config.yaml` & `circuitpython-async-button-1.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.0/.pylintrc` & `circuitpython-async-button-1.2.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.0/CODE_OF_CONDUCT.md` & `circuitpython-async-button-1.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.0/LICENSE` & `circuitpython-async-button-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.0/LICENSES/CC-BY-4.0.txt` & `circuitpython-async-button-1.2.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.0/LICENSES/MIT.txt` & `circuitpython-async-button-1.2.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.0/LICENSES/Unlicense.txt` & `circuitpython-async-button-1.2.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.0/PKG-INFO` & `circuitpython-async-button-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-async-button
-Version: 1.2.0
+Version: 1.2.1
 Summary: a library for reading buttons using asyncio
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/furbrain/CircuitPython_async_button
 Keywords: adafruit,blinka,circuitpython,micropython,async_button,async,asyncio,countio,keypad,button,press
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-async-button-1.2.0/README.rst` & `circuitpython-async-button-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.0/async_button.py` & `circuitpython-async-button-1.2.1/async_button.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   https://github.com/adafruit/Adafruit_CircuitPython_asyncio
 
 * CircuitPython ticks module:
   https://github.com/adafruit/Adafruit_CircuitPython_Ticks
 """
 
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 __repo__ = "https://github.com/furbrain/CircuitPython_async_button.git"
 
 import asyncio
 from asyncio import Task, Event
 
 from adafruit_ticks import ticks_add, ticks_less, ticks_ms
```

### Comparing `circuitpython-async-button-1.2.0/circuitpython_async_button.egg-info/PKG-INFO` & `circuitpython-async-button-1.2.1/circuitpython_async_button.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-async-button
-Version: 1.2.0
+Version: 1.2.1
 Summary: a library for reading buttons using asyncio
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/furbrain/CircuitPython_async_button
 Keywords: adafruit,blinka,circuitpython,micropython,async_button,async,asyncio,countio,keypad,button,press
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-async-button-1.2.0/circuitpython_async_button.egg-info/SOURCES.txt` & `circuitpython-async-button-1.2.1/circuitpython_async_button.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.0/docs/_static/favicon.ico` & `circuitpython-async-button-1.2.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.0/docs/conf.py` & `circuitpython-async-button-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.0/docs/events.rst` & `circuitpython-async-button-1.2.1/docs/events.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.0/docs/index.rst` & `circuitpython-async-button-1.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.0/docs/timing_double.json` & `circuitpython-async-button-1.2.1/docs/timing_double.json`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.0/docs/timing_long.json` & `circuitpython-async-button-1.2.1/docs/timing_long.json`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.0/docs/timing_single.json` & `circuitpython-async-button-1.2.1/docs/timing_single.json`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.0/docs/timing_triple.json` & `circuitpython-async-button-1.2.1/docs/timing_triple.json`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.0/examples/async_button_test.py` & `circuitpython-async-button-1.2.1/examples/async_button_test.py`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.0/examples/async_multibutton_test.py` & `circuitpython-async-button-1.2.1/examples/async_multibutton_test.py`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.0/examples/async_simplebutton_test.py` & `circuitpython-async-button-1.2.1/examples/async_simplebutton_test.py`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.0/pyproject.toml` & `circuitpython-async-button-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-async-button"
 description = "a library for reading buttons using asyncio"
-version = "1.2.0"
+version = "1.2.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/furbrain/CircuitPython_async_button"}
 keywords = [
     "adafruit",
```

### Comparing `circuitpython-async-button-1.2.0/tests/test_async_button.py` & `circuitpython-async-button-1.2.1/tests/test_async_button.py`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.0/tests/test_async_multi_button.py` & `circuitpython-async-button-1.2.1/tests/test_async_multi_button.py`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.0/tests/test_async_simple_button.py` & `circuitpython-async-button-1.2.1/tests/test_async_simple_button.py`

 * *Files identical despite different names*

