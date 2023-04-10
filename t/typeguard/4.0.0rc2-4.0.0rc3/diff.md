# Comparing `tmp/typeguard-4.0.0rc2.tar.gz` & `tmp/typeguard-4.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typeguard-4.0.0rc2.tar", last modified: Sat Apr  8 11:01:12 2023, max compression
+gzip compressed data, was "typeguard-4.0.0rc3.tar", last modified: Mon Apr 10 16:23:40 2023, max compression
```

## Comparing `typeguard-4.0.0rc2.tar` & `typeguard-4.0.0rc3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:01:12.533336 typeguard-4.0.0rc2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:01:12.521336 typeguard-4.0.0rc2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:01:12.525336 typeguard-4.0.0rc2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/.github/ISSUE_TEMPLATE/features_request.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:01:12.525336 typeguard-4.0.0rc2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-08 11:01:12.533336 typeguard-4.0.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:01:12.525336 typeguard-4.0.0rc2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/docs/extending.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/docs/features.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/docs/userguide.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16916 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/docs/versionhistory.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 11:01:12.533336 typeguard-4.0.0rc2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:01:12.525336 typeguard-4.0.0rc2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:01:12.529336 typeguard-4.0.0rc2/src/typeguard/
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/src/typeguard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25641 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/src/typeguard/_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/src/typeguard/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/src/typeguard/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/src/typeguard/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/src/typeguard/_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/src/typeguard/_importhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/src/typeguard/_memo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/src/typeguard/_pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/src/typeguard/_suppression.py
--rw-r--r--   0 runner    (1001) docker     (123)    38181 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/src/typeguard/_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/src/typeguard/_union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/src/typeguard/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/src/typeguard/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:01:12.533336 typeguard-4.0.0rc2/src/typeguard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-08 11:01:12.000000 typeguard-4.0.0rc2/src/typeguard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-08 11:01:12.000000 typeguard-4.0.0rc2/src/typeguard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 11:01:12.000000 typeguard-4.0.0rc2/src/typeguard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-08 11:01:12.000000 typeguard-4.0.0rc2/src/typeguard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-08 11:01:12.000000 typeguard-4.0.0rc2/src/typeguard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-08 11:01:12.000000 typeguard-4.0.0rc2/src/typeguard.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:01:12.533336 typeguard-4.0.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/tests/dummymodule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:01:12.533336 typeguard-4.0.0rc2/tests/mypy/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/tests/mypy/negative.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/tests/mypy/positive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/tests/mypy/test_type_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)    30979 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/tests/test_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/tests/test_importhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/tests/test_instrumentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/tests/test_suppression.py
--rw-r--r--   0 runner    (1001) docker     (123)    36886 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/tests/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15683 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/tests/test_typechecked.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/tests/test_union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-08 11:01:01.000000 typeguard-4.0.0rc2/tests/test_warn_on_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:40.576764 typeguard-4.0.0rc3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:40.568764 typeguard-4.0.0rc3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:40.568764 typeguard-4.0.0rc3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/.github/ISSUE_TEMPLATE/features_request.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:40.568764 typeguard-4.0.0rc3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-10 16:23:40.576764 typeguard-4.0.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:40.568764 typeguard-4.0.0rc3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/docs/extending.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/docs/features.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/docs/userguide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17085 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/docs/versionhistory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 16:23:40.576764 typeguard-4.0.0rc3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:40.568764 typeguard-4.0.0rc3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:40.572764 typeguard-4.0.0rc3/src/typeguard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25756 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/_importhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/_memo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/_pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38460 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/_union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/src/typeguard/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:40.572764 typeguard-4.0.0rc3/src/typeguard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-10 16:23:40.000000 typeguard-4.0.0rc3/src/typeguard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-10 16:23:40.000000 typeguard-4.0.0rc3/src/typeguard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:23:40.000000 typeguard-4.0.0rc3/src/typeguard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-10 16:23:40.000000 typeguard-4.0.0rc3/src/typeguard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-10 16:23:40.000000 typeguard-4.0.0rc3/src/typeguard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-10 16:23:40.000000 typeguard-4.0.0rc3/src/typeguard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:40.572764 typeguard-4.0.0rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/dummymodule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:23:40.576764 typeguard-4.0.0rc3/tests/mypy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/mypy/negative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/mypy/positive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/mypy/test_type_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30979 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/test_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/test_importhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10861 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/test_instrumentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/test_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36886 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15683 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/test_typechecked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/test_union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-10 16:23:29.000000 typeguard-4.0.0rc3/tests/test_warn_on_error.py
```

### Comparing `typeguard-4.0.0rc2/.github/ISSUE_TEMPLATE/bug_report.yaml` & `typeguard-4.0.0rc3/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/.github/ISSUE_TEMPLATE/features_request.yaml` & `typeguard-4.0.0rc3/.github/ISSUE_TEMPLATE/features_request.yaml`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/.github/workflows/publish.yml` & `typeguard-4.0.0rc3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/.github/workflows/test.yml` & `typeguard-4.0.0rc3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/.pre-commit-config.yaml` & `typeguard-4.0.0rc3/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,18 @@
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
         exclude: "^tests/mypy/negative.py"
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.260
+    rev: v0.0.261
     hooks:
       - id: ruff
         args: [--fix, --show-fixes]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.1.1
+    rev: v1.2.0
     hooks:
       - id: mypy
         additional_dependencies: [ "typing_extensions" ]
         exclude: "^tests/"
```

### Comparing `typeguard-4.0.0rc2/LICENSE` & `typeguard-4.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/PKG-INFO` & `typeguard-4.0.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeguard
-Version: 4.0.0rc2
+Version: 4.0.0rc3
 Summary: Run-time type checker for Python
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://typeguard.readthedocs.io/en/latest/
 Project-URL: Change log, https://typeguard.readthedocs.io/en/latest/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/typeguard
 Project-URL: Issue tracker, https://github.com/agronholm/typeguard/issues
```

### Comparing `typeguard-4.0.0rc2/README.rst` & `typeguard-4.0.0rc3/README.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/docs/api.rst` & `typeguard-4.0.0rc3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/docs/conf.py` & `typeguard-4.0.0rc3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/docs/extending.rst` & `typeguard-4.0.0rc3/docs/extending.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/docs/features.rst` & `typeguard-4.0.0rc3/docs/features.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/docs/userguide.rst` & `typeguard-4.0.0rc3/docs/userguide.rst`

 * *Files 1% similar despite different names*

```diff
@@ -130,16 +130,18 @@
 
 Notes on forward reference handling
 -----------------------------------
 
 The internal type checking functions, injected to instrumented code by either
 :func:`@typechecked <typechecked>` or the import hook, use the "naked" versions of any
 annotations, undoing any quotations in them (and the effects of
-``from __future__ import annotations``). As such, the
-:attr:`~.TypeCheckConfiguration.forward_ref_policy` does not apply to instrumented code.
+``from __future__ import annotations``). As such, in instrumented code, the
+:attr:`~.TypeCheckConfiguration.forward_ref_policy` only applies when using type
+variables containing forward references, or type aliases likewise containing forward
+references.
 
 To facilitate the use of types only available to static type checkers, Typeguard
 recognizes module-level imports guarded by ``if typing.TYPE_CHECKING:`` or
 ``if TYPE_CHECKING:`` (add the appropriate :mod:`typing` imports). Imports made within
 such blocks on the module level will be replaced in calls to internal type checking
 functions with :data:`~typing.Any`.
```

### Comparing `typeguard-4.0.0rc2/docs/versionhistory.rst` & `typeguard-4.0.0rc3/docs/versionhistory.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 Version history
 ===============
 
 This library adheres to `Semantic Versioning 2.0 <https://semver.org/#semantic-versioning-200>`_.
 
+**4.0.0rc3** (2023-04-10)
+
+- Fixed ``typing.Literal`` subscript contents being evaluated as forward references
+- Fixed resolution of forward references in type aliases
+
 **4.0.0rc2** (2023-04-08)
 
 - The ``.pyc`` files now use a version-based optimization suffix in the file names so as
   not to cause the interpreter to load potentially faulty/incompatible cached bytecode
   generated by older versions
 - Fixed typed variable positional and keyword arguments causing compilation errors on
   Python 3.7 and 3.8
```

### Comparing `typeguard-4.0.0rc2/pyproject.toml` & `typeguard-4.0.0rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/src/typeguard/__init__.py` & `typeguard-4.0.0rc3/src/typeguard/__init__.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/src/typeguard/_checkers.py` & `typeguard-4.0.0rc3/src/typeguard/_checkers.py`

 * *Files 2% similar despite different names*

```diff
@@ -441,15 +441,19 @@
     if not isclass(value):
         raise TypeCheckError("is not a class")
 
     # Needed on Python 3.7+
     if not args:
         return
 
-    expected_class = args[0]
+    if isinstance(args[0], ForwardRef):
+        expected_class = evaluate_forwardref(args[0], memo)
+    else:
+        expected_class = args[0]
+
     if expected_class is Any:
         return
     elif getattr(expected_class, "_is_protocol", False):
         check_protocol(value, expected_class, (), memo)
     elif isinstance(expected_class, TypeVar):
         check_typevar(value, expected_class, (), memo, subclass_check=True)
     elif get_origin(expected_class) is Union:
```

### Comparing `typeguard-4.0.0rc2/src/typeguard/_config.py` & `typeguard-4.0.0rc3/src/typeguard/_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,18 +72,14 @@
          Default: ``None`` (the :exc:`~.TypeCheckError` is raised directly)
 
     .. attribute:: forward_ref_policy
        :type: ForwardRefPolicy
 
          Specifies what to do when a forward reference fails to resolve.
 
-         Note that this setting only applies to :func:`.check_type`, as instrumented
-         code eagerly resolves forward references during compilation. See the
-         :ref:`forwardrefs` section in the documentation for further information.
-
          Default: ``WARN``
 
     .. attribute:: collection_check_strategy
        :type: CollectionCheckStrategy
 
          Specifies how thoroughly the contents of collections (list, dict, etc.) are
          type checked.
```

### Comparing `typeguard-4.0.0rc2/src/typeguard/_decorators.py` & `typeguard-4.0.0rc3/src/typeguard/_decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,17 @@
                             kwargs[name] = retval
 
                 setattr(target, key, attr.__class__(**kwargs))
 
         return target
 
     # Find either the first Python wrapper or the actual function
-    wrapper_class: type[classmethod[Any]] | type[staticmethod[Any]] | None = None
+    wrapper_class: type[classmethod[Any, Any, Any]] | type[
+        staticmethod[Any, Any]
+    ] | None = None
     if isinstance(target, (classmethod, staticmethod)):
         wrapper_class = target.__class__
         target = target.__func__
 
     retval = instrument(target)
     if isinstance(retval, str):
         warn(
```

### Comparing `typeguard-4.0.0rc2/src/typeguard/_exceptions.py` & `typeguard-4.0.0rc3/src/typeguard/_exceptions.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/src/typeguard/_functions.py` & `typeguard-4.0.0rc3/src/typeguard/_functions.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/src/typeguard/_importhook.py` & `typeguard-4.0.0rc3/src/typeguard/_importhook.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import sys
 import types
 from collections.abc import Callable, Iterable
 from importlib.abc import MetaPathFinder
 from importlib.machinery import ModuleSpec, SourceFileLoader
 from importlib.util import cache_from_source, decode_source
 from inspect import isclass
+from os import PathLike
 from types import CodeType, ModuleType, TracebackType
 from typing import TYPE_CHECKING, Any, Sequence, TypeVar
 from unittest.mock import patch
 
 from ._config import global_config
 from ._transformer import TypeguardTransformer
 
@@ -62,28 +63,43 @@
         data: bytes
         | bytearray
         | memoryview
         | array[Any]
         | mmap
         | _CData
         | PickleBuffer
-        | str,
-        path: str = "<string>",
+        | str
+        | ast.Module
+        | ast.Expression
+        | ast.Interactive,
+        path: bytes
+        | bytearray
+        | memoryview
+        | array[Any]
+        | mmap
+        | _CData
+        | PickleBuffer
+        | str
+        | PathLike[str] = "<string>",
     ) -> CodeType:
-        if isinstance(data, str):
-            source = data
+        if isinstance(data, (ast.Module, ast.Expression, ast.Interactive)):
+            tree = data
         else:
-            source = decode_source(data)
+            if isinstance(data, str):
+                source = data
+            else:
+                source = decode_source(data)
+
+            tree = _call_with_frames_removed(
+                ast.parse,
+                source,
+                path,
+                "exec",
+            )
 
-        tree = _call_with_frames_removed(
-            ast.parse,
-            source,
-            path,
-            "exec",
-        )
         tree = TypeguardTransformer().visit(tree)
         ast.fix_missing_locations(tree)
 
         if global_config.debug_instrumentation and sys.version_info >= (3, 9):
             print(
                 f"Source code of {path!r} after instrumentation:\n"
                 "----------------------------------------------",
```

### Comparing `typeguard-4.0.0rc2/src/typeguard/_memo.py` & `typeguard-4.0.0rc3/src/typeguard/_memo.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/src/typeguard/_pytest_plugin.py` & `typeguard-4.0.0rc3/src/typeguard/_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/src/typeguard/_suppression.py` & `typeguard-4.0.0rc3/src/typeguard/_suppression.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/src/typeguard/_transformer.py` & `typeguard-4.0.0rc3/src/typeguard/_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,18 @@
     "typing.AsyncGenerator",
     "collections.abc.AsyncGenerator",
 )
 anytype_names = (
     "typing.Any",
     "typing_extensions.Any",
 )
+literal_names = (
+    "typing.Literal",
+    "typing_extensions.Literal",
+)
 ignore_decorators = (
     "typing.no_type_check",
     "typeguard.typeguard_ignore",
 )
 aug_assign_functions = {
     Add: "iadd",
     Sub: "isub",
@@ -363,15 +367,20 @@
             else:
                 return None
 
         return node
 
     def visit_Subscript(self, node: Subscript) -> Any:
         self.level += 1
-        self.generic_visit(node)
+
+        # The subscript of typing(_extensions).Literal can be any arbitrary string, so
+        # don't try to evaluate it as code
+        if not self._memo.name_matches(node.value, *literal_names):
+            self.generic_visit(node)
+
         self.level -= 1
         return node
 
     def visit_Name(self, node: Name) -> Any:
         if self._memo.is_ignored_name(node):
             if self.level > 0:
                 return self.transformer._get_import("typing", "Any")
```

### Comparing `typeguard-4.0.0rc2/src/typeguard/_union_transformer.py` & `typeguard-4.0.0rc3/src/typeguard/_union_transformer.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/src/typeguard/_utils.py` & `typeguard-4.0.0rc3/src/typeguard/_utils.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/src/typeguard.egg-info/PKG-INFO` & `typeguard-4.0.0rc3/src/typeguard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeguard
-Version: 4.0.0rc2
+Version: 4.0.0rc3
 Summary: Run-time type checker for Python
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://typeguard.readthedocs.io/en/latest/
 Project-URL: Change log, https://typeguard.readthedocs.io/en/latest/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/typeguard
 Project-URL: Issue tracker, https://github.com/agronholm/typeguard/issues
```

### Comparing `typeguard-4.0.0rc2/src/typeguard.egg-info/SOURCES.txt` & `typeguard-4.0.0rc3/src/typeguard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/tests/__init__.py` & `typeguard-4.0.0rc3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/tests/conftest.py` & `typeguard-4.0.0rc3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/tests/dummymodule.py` & `typeguard-4.0.0rc3/tests/dummymodule.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,16 @@
     AsyncGenerator,
     Callable,
     Dict,
     Generator,
     List,
     Sequence,
     Tuple,
+    Type,
+    TypeVar,
     Union,
     no_type_check,
     no_type_check_decorator,
     overload,
 )
 
 if sys.version_info >= (3, 10):
@@ -33,14 +35,15 @@
     typechecked,
     typeguard_ignore,
 )
 
 if TYPE_CHECKING:
     from nonexistent import Imaginary
 
+T = TypeVar("T", bound="DummyClass")
 P = ParamSpec("P")
 
 
 @no_type_check_decorator
 def dummy_decorator(func):
     return func
 
@@ -312,7 +315,18 @@
     return args, kwargs
 
 
 @typechecked
 def guarded_type_hint(x: "Imaginary") -> "Imaginary":
     y: Imaginary = x
     return y
+
+
+@typechecked
+def literal(x: Literal["foo"]) -> Literal["foo"]:
+    y: Literal["foo"] = x
+    return y
+
+
+@typechecked
+def typevar_forwardref(x: Type[T]) -> T:
+    return x()
```

### Comparing `typeguard-4.0.0rc2/tests/mypy/negative.py` & `typeguard-4.0.0rc3/tests/mypy/negative.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/tests/mypy/positive.py` & `typeguard-4.0.0rc3/tests/mypy/positive.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/tests/mypy/test_type_annotations.py` & `typeguard-4.0.0rc3/tests/mypy/test_type_annotations.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/tests/test_checkers.py` & `typeguard-4.0.0rc3/tests/test_checkers.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/tests/test_importhook.py` & `typeguard-4.0.0rc3/tests/test_importhook.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/tests/test_instrumentation.py` & `typeguard-4.0.0rc3/tests/test_instrumentation.py`

 * *Files 4% similar despite different names*

```diff
@@ -330,7 +330,16 @@
             r"instance of int",
         ):
             dummymodule.typed_variable_args("foo", "bar", a="baz")
 
 
 def test_guarded_type(dummymodule):
     assert dummymodule.guarded_type_hint("foo") == "foo"
+
+
+def test_literal(dummymodule):
+    assert dummymodule.literal("foo") == "foo"
+
+
+def test_typevar_forwardref(dummymodule):
+    instance = dummymodule.typevar_forwardref(dummymodule.DummyClass)
+    assert isinstance(instance, dummymodule.DummyClass)
```

### Comparing `typeguard-4.0.0rc2/tests/test_plugins.py` & `typeguard-4.0.0rc3/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/tests/test_suppression.py` & `typeguard-4.0.0rc3/tests/test_suppression.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/tests/test_transformer.py` & `typeguard-4.0.0rc3/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/tests/test_typechecked.py` & `typeguard-4.0.0rc3/tests/test_typechecked.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/tests/test_union_transformer.py` & `typeguard-4.0.0rc3/tests/test_union_transformer.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/tests/test_utils.py` & `typeguard-4.0.0rc3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc2/tests/test_warn_on_error.py` & `typeguard-4.0.0rc3/tests/test_warn_on_error.py`

 * *Files identical despite different names*

