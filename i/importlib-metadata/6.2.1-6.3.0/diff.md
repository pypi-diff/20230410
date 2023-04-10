# Comparing `tmp/importlib_metadata-6.2.1.tar.gz` & `tmp/importlib_metadata-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "importlib_metadata-6.2.1.tar", last modified: Sun Apr  9 15:29:34 2023, max compression
+gzip compressed data, was "importlib_metadata-6.3.0.tar", last modified: Mon Apr 10 02:27:32 2023, max compression
```

## Comparing `importlib_metadata-6.2.1.tar` & `importlib_metadata-6.3.0.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.870788 importlib_metadata-6.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.862788 importlib_metadata-6.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.862788 importlib_metadata-6.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20500 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-09 15:29:34.870788 importlib_metadata-6.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.862788 importlib_metadata-6.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/docs/migration.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13802 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/docs/using.rst
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/exercises.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.866788 importlib_metadata-6.2.1/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    26608 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/importlib_metadata/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/importlib_metadata/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/importlib_metadata/_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/importlib_metadata/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/importlib_metadata/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/importlib_metadata/_py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/importlib_metadata/_text.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/importlib_metadata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.866788 importlib_metadata-6.2.1/importlib_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-09 15:29:34.000000 importlib_metadata-6.2.1/importlib_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-09 15:29:34.000000 importlib_metadata-6.2.1/importlib_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 15:29:34.000000 importlib_metadata-6.2.1/importlib_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-09 15:29:34.000000 importlib_metadata-6.2.1/importlib_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-09 15:29:34.000000 importlib_metadata-6.2.1/importlib_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.858788 importlib_metadata-6.2.1/prepare/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.866788 importlib_metadata-6.2.1/prepare/example/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.866788 importlib_metadata-6.2.1/prepare/example/example/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/prepare/example/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/prepare/example/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.870788 importlib_metadata-6.2.1/prepare/example2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.870788 importlib_metadata-6.2.1/prepare/example2/example2/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/prepare/example2/example2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/prepare/example2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-09 15:29:34.870788 importlib_metadata-6.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.870788 importlib_metadata-6.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.870788 importlib_metadata-6.2.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tests/data/example-21.12-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tests/data/example-21.12-py3.6.egg
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tests/data/example2-1.0.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tests/py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tests/test_py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tests/test_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.096812 importlib_metadata-6.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.092812 importlib_metadata-6.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.092812 importlib_metadata-6.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20599 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-10 02:27:32.096812 importlib_metadata-6.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.092812 importlib_metadata-6.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/docs/migration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13802 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/docs/using.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/exercises.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.092812 importlib_metadata-6.3.0/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    28576 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/importlib_metadata/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/importlib_metadata/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/importlib_metadata/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/importlib_metadata/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/importlib_metadata/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/importlib_metadata/_py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/importlib_metadata/_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/importlib_metadata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.092812 importlib_metadata-6.3.0/importlib_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-10 02:27:32.000000 importlib_metadata-6.3.0/importlib_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-10 02:27:32.000000 importlib_metadata-6.3.0/importlib_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 02:27:32.000000 importlib_metadata-6.3.0/importlib_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-10 02:27:32.000000 importlib_metadata-6.3.0/importlib_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-10 02:27:32.000000 importlib_metadata-6.3.0/importlib_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.088812 importlib_metadata-6.3.0/prepare/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.092812 importlib_metadata-6.3.0/prepare/example/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.092812 importlib_metadata-6.3.0/prepare/example/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/prepare/example/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/prepare/example/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.092812 importlib_metadata-6.3.0/prepare/example2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.092812 importlib_metadata-6.3.0/prepare/example2/example2/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/prepare/example2/example2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/prepare/example2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-10 02:27:32.096812 importlib_metadata-6.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.096812 importlib_metadata-6.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:32.096812 importlib_metadata-6.3.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/data/example-21.12-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/data/example-21.12-py3.6.egg
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/data/example2-1.0.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/test_py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tests/test_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-10 02:27:13.000000 importlib_metadata-6.3.0/tox.ini
```

### Comparing `importlib_metadata-6.2.1/.github/workflows/main.yml` & `importlib_metadata-6.3.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.1/CHANGES.rst` & `importlib_metadata-6.3.0/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v6.3.0
+======
+
+* #115: Support ``installed-files.txt`` for ``Distribution.files``
+  when present.
+
 v6.2.1
 ======
 
 * #442: Fixed issue introduced in v6.1.0 where non-importable
   names (metadata dirs) began appearing in
   ``packages_distributions``.
```

### Comparing `importlib_metadata-6.2.1/LICENSE` & `importlib_metadata-6.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.1/PKG-INFO` & `importlib_metadata-6.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: importlib_metadata
-Version: 6.2.1
+Version: 6.3.0
 Summary: Read metadata from Python packages
 Home-page: https://github.com/python/importlib_metadata
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `importlib_metadata-6.2.1/README.rst` & `importlib_metadata-6.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.1/conftest.py` & `importlib_metadata-6.3.0/conftest.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.1/docs/conf.py` & `importlib_metadata-6.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.1/docs/index.rst` & `importlib_metadata-6.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.1/docs/migration.rst` & `importlib_metadata-6.3.0/docs/migration.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.1/docs/using.rst` & `importlib_metadata-6.3.0/docs/using.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.1/exercises.py` & `importlib_metadata-6.3.0/exercises.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.1/importlib_metadata/__init__.py` & `importlib_metadata-6.3.0/importlib_metadata/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import pathlib
 import operator
 import textwrap
 import warnings
 import functools
 import itertools
 import posixpath
+import contextlib
 import collections
 import inspect
 
 from . import _adapters, _meta, _py39compat
 from ._collections import FreezableDefaultDict, Pair
 from ._compat import (
     NullFinder,
@@ -457,43 +458,86 @@
     @property
     def files(self):
         """Files in this distribution.
 
         :return: List of PackagePath for this distribution or None
 
         Result is `None` if the metadata file that enumerates files
-        (i.e. RECORD for dist-info or SOURCES.txt for egg-info) is
-        missing.
+        (i.e. RECORD for dist-info, or installed-files.txt or
+        SOURCES.txt for egg-info) is missing.
         Result may be empty if the metadata exists but is empty.
         """
 
         def make_file(name, hash=None, size_str=None):
             result = PackagePath(name)
             result.hash = FileHash(hash) if hash else None
             result.size = int(size_str) if size_str else None
             result.dist = self
             return result
 
         @pass_none
         def make_files(lines):
-            return list(starmap(make_file, csv.reader(lines)))
+            return starmap(make_file, csv.reader(lines))
 
-        return make_files(self._read_files_distinfo() or self._read_files_egginfo())
+        @pass_none
+        def skip_missing_files(package_paths):
+            return list(filter(lambda path: path.locate().exists(), package_paths))
+
+        return skip_missing_files(
+            make_files(
+                self._read_files_distinfo()
+                or self._read_files_egginfo_installed()
+                or self._read_files_egginfo_sources()
+            )
+        )
 
     def _read_files_distinfo(self):
         """
         Read the lines of RECORD
         """
         text = self.read_text('RECORD')
         return text and text.splitlines()
 
-    def _read_files_egginfo(self):
+    def _read_files_egginfo_installed(self):
         """
-        SOURCES.txt might contain literal commas, so wrap each line
-        in quotes.
+        Read installed-files.txt and return lines in a similar
+        CSV-parsable format as RECORD: each file must be placed
+        relative to the site-packages directory, and must also be
+        quoted (since file names can contain literal commas).
+
+        This file is written when the package is installed by pip,
+        but it might not be written for other installation methods.
+        Hence, even if we can assume that this file is accurate
+        when it exists, we cannot assume that it always exists.
+        """
+        text = self.read_text('installed-files.txt')
+        # We need to prepend the .egg-info/ subdir to the lines in this file.
+        # But this subdir is only available in the PathDistribution's self._path
+        # which is not easily accessible from this base class...
+        subdir = getattr(self, '_path', None)
+        if not text or not subdir:
+            return
+        with contextlib.suppress(Exception):
+            ret = [
+                str((subdir / line).resolve().relative_to(self.locate_file('')))
+                for line in text.splitlines()
+            ]
+            return map('"{}"'.format, ret)
+
+    def _read_files_egginfo_sources(self):
+        """
+        Read SOURCES.txt and return lines in a similar CSV-parsable
+        format as RECORD: each file name must be quoted (since it
+        might contain literal commas).
+
+        Note that SOURCES.txt is not a reliable source for what
+        files are installed by a package. This file is generated
+        for a source archive, and the files that are present
+        there (e.g. setup.py) may not correctly reflect the files
+        that are present after the package has been installed.
         """
         text = self.read_text('SOURCES.txt')
         return text and map('"{}"'.format, text.splitlines())
 
     @property
     def requires(self):
         """Generated requirements specified for this Distribution"""
```

### Comparing `importlib_metadata-6.2.1/importlib_metadata/_adapters.py` & `importlib_metadata-6.3.0/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.1/importlib_metadata/_collections.py` & `importlib_metadata-6.3.0/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.1/importlib_metadata/_compat.py` & `importlib_metadata-6.3.0/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.1/importlib_metadata/_functools.py` & `importlib_metadata-6.3.0/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.1/importlib_metadata/_itertools.py` & `importlib_metadata-6.3.0/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.1/importlib_metadata/_meta.py` & `importlib_metadata-6.3.0/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.1/importlib_metadata/_py39compat.py` & `importlib_metadata-6.3.0/importlib_metadata/_py39compat.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.1/importlib_metadata/_text.py` & `importlib_metadata-6.3.0/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.1/importlib_metadata.egg-info/PKG-INFO` & `importlib_metadata-6.3.0/importlib_metadata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: importlib-metadata
-Version: 6.2.1
+Version: 6.3.0
 Summary: Read metadata from Python packages
 Home-page: https://github.com/python/importlib_metadata
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `importlib_metadata-6.2.1/importlib_metadata.egg-info/SOURCES.txt` & `importlib_metadata-6.3.0/importlib_metadata.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 importlib_metadata.egg-info/requires.txt
 importlib_metadata.egg-info/top_level.txt
 prepare/example/setup.py
 prepare/example/example/__init__.py
 prepare/example2/pyproject.toml
 prepare/example2/example2/__init__.py
 tests/__init__.py
+tests/_path.py
 tests/fixtures.py
 tests/py39compat.py
 tests/test_api.py
 tests/test_integration.py
 tests/test_main.py
 tests/test_py39compat.py
 tests/test_zip.py
```

### Comparing `importlib_metadata-6.2.1/pytest.ini` & `importlib_metadata-6.3.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.1/setup.cfg` & `importlib_metadata-6.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.1/tests/data/example-21.12-py3-none-any.whl` & `importlib_metadata-6.3.0/tests/data/example-21.12-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.1/tests/data/example-21.12-py3.6.egg` & `importlib_metadata-6.3.0/tests/data/example-21.12-py3.6.egg`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.1/tests/data/example2-1.0.0-py3-none-any.whl` & `importlib_metadata-6.3.0/tests/data/example2-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.1/tests/test_api.py` & `importlib_metadata-6.3.0/tests/test_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,17 @@
     with warnings.catch_warnings(record=True) as ctx:
         warnings.simplefilter('default', category=DeprecationWarning)
         yield ctx
 
 
 class APITests(
     fixtures.EggInfoPkg,
+    fixtures.EggInfoPkgPipInstalledNoToplevel,
+    fixtures.EggInfoPkgPipInstalledNoModules,
+    fixtures.EggInfoPkgSourcesFallback,
     fixtures.DistInfoPkg,
     fixtures.DistInfoPkgWithDot,
     fixtures.EggInfoFile,
     unittest.TestCase,
 ):
     version_pattern = r'\d+\.\d+(\.\d)?'
 
@@ -58,23 +61,36 @@
         prefixes = 'p', 'pkg', 'pkg.'
         for prefix in prefixes:
             with self.subTest(prefix):
                 with self.assertRaises(PackageNotFoundError):
                     distribution(prefix)
 
     def test_for_top_level(self):
-        self.assertEqual(
-            distribution('egginfo-pkg').read_text('top_level.txt').strip(), 'mod'
-        )
+        tests = [
+            ('egginfo-pkg', 'mod'),
+            ('egg_with_no_modules-pkg', ''),
+        ]
+        for pkg_name, expect_content in tests:
+            with self.subTest(pkg_name):
+                self.assertEqual(
+                    distribution(pkg_name).read_text('top_level.txt').strip(),
+                    expect_content,
+                )
 
     def test_read_text(self):
-        top_level = [
-            path for path in files('egginfo-pkg') if path.name == 'top_level.txt'
-        ][0]
-        self.assertEqual(top_level.read_text(), 'mod\n')
+        tests = [
+            ('egginfo-pkg', 'mod\n'),
+            ('egg_with_no_modules-pkg', '\n'),
+        ]
+        for pkg_name, expect_content in tests:
+            with self.subTest(pkg_name):
+                top_level = [
+                    path for path in files(pkg_name) if path.name == 'top_level.txt'
+                ][0]
+                self.assertEqual(top_level.read_text(), expect_content)
 
     def test_entry_points(self):
         eps = entry_points()
         assert 'entries' in eps.groups
         entries = eps.select(group='entries')
         assert 'main' in entries.names
         ep = entries['main']
@@ -180,14 +196,17 @@
         self.assertRegex(repr(util.hash), '<FileHash mode: sha256 value: .*>')
 
     def test_files_dist_info(self):
         self._test_files(files('distinfo-pkg'))
 
     def test_files_egg_info(self):
         self._test_files(files('egginfo-pkg'))
+        self._test_files(files('egg_with_module-pkg'))
+        self._test_files(files('egg_with_no_modules-pkg'))
+        self._test_files(files('sources_fallback-pkg'))
 
     def test_version_egg_info_file(self):
         self.assertEqual(version('egginfo-file'), '0.1')
 
     def test_requires_egg_info_file(self):
         requirements = requires('egginfo-file')
         self.assertIsNone(requirements)
```

### Comparing `importlib_metadata-6.2.1/tests/test_integration.py` & `importlib_metadata-6.3.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.1/tests/test_main.py` & `importlib_metadata-6.3.0/tests/test_main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 import pickle
 import unittest
 import importlib
 import importlib_metadata
+import itertools
 import pyfakefs.fake_filesystem_unittest as ffs
 
 from . import fixtures
 from importlib_metadata import (
     Distribution,
     EntryPoint,
     PackageNotFoundError,
@@ -166,19 +167,29 @@
 
     def test_metadata_loads_egg_info(self):
         pkg_name = self.pkg_with_non_ascii_description_egg_info(self.site_dir)
         meta = metadata(pkg_name)
         assert meta['Description'] == 'pôrˈtend'
 
 
-class DiscoveryTests(fixtures.EggInfoPkg, fixtures.DistInfoPkg, unittest.TestCase):
+class DiscoveryTests(
+    fixtures.EggInfoPkg,
+    fixtures.EggInfoPkgPipInstalledNoToplevel,
+    fixtures.EggInfoPkgPipInstalledNoModules,
+    fixtures.EggInfoPkgSourcesFallback,
+    fixtures.DistInfoPkg,
+    unittest.TestCase,
+):
     def test_package_discovery(self):
         dists = list(distributions())
         assert all(isinstance(dist, Distribution) for dist in dists)
         assert any(dist.metadata['Name'] == 'egginfo-pkg' for dist in dists)
+        assert any(dist.metadata['Name'] == 'egg_with_module-pkg' for dist in dists)
+        assert any(dist.metadata['Name'] == 'egg_with_no_modules-pkg' for dist in dists)
+        assert any(dist.metadata['Name'] == 'sources_fallback-pkg' for dist in dists)
         assert any(dist.metadata['Name'] == 'distinfo-pkg' for dist in dists)
 
     def test_invalid_usage(self):
         with self.assertRaises(ValueError):
             list(distributions(context='something', name='else'))
 
 
@@ -324,35 +335,77 @@
         packages_distributions()
 
     def test_packages_distributions_all_module_types(self):
         """
         Test top-level modules detected on a package without 'top-level.txt'.
         """
         suffixes = importlib.machinery.all_suffixes()
-        fixtures.build_files(
-            {
-                'all_distributions-1.0.0.dist-info': {
-                    'METADATA': """
-                        Name: all_distributions
-                        Version: 1.0.0
-                    """,
-                    'RECORD': 'all_distributions-1.0.0.dist-info/METADATA\n'
-                    + ''.join(
-                        f'importable-name {i}{suffix},,\n'
-                        f'in_namespace_{i}/mod{suffix},,\n'
-                        f'in_package_{i}/__init__.py,,\n'
-                        f'in_package_{i}/mod{suffix},,\n'
-                        for i, suffix in enumerate(suffixes)
-                    ),
-                },
-            },
-            prefix=self.site_dir,
+        metadata = dict(
+            METADATA="""
+                Name: all_distributions
+                Version: 1.0.0
+                """,
         )
+        files = {
+            'all_distributions-1.0.0.dist-info': metadata,
+        }
+        for i, suffix in enumerate(suffixes):
+            files.update(
+                {
+                    f'importable-name {i}{suffix}': '',
+                    f'in_namespace_{i}': {
+                        f'mod{suffix}': '',
+                    },
+                    f'in_package_{i}': {
+                        '__init__.py': '',
+                        f'mod{suffix}': '',
+                    },
+                }
+            )
+        metadata.update(RECORD=fixtures.build_record(files))
+        fixtures.build_files(files, prefix=self.site_dir)
 
         distributions = packages_distributions()
 
         for i in range(len(suffixes)):
             assert distributions[f'importable-name {i}'] == ['all_distributions']
             assert distributions[f'in_namespace_{i}'] == ['all_distributions']
             assert distributions[f'in_package_{i}'] == ['all_distributions']
 
         assert not any(name.endswith('.dist-info') for name in distributions)
+
+
+class PackagesDistributionsEggTest(
+    fixtures.EggInfoPkg,
+    fixtures.EggInfoPkgPipInstalledNoToplevel,
+    fixtures.EggInfoPkgPipInstalledNoModules,
+    fixtures.EggInfoPkgSourcesFallback,
+    unittest.TestCase,
+):
+    def test_packages_distributions_on_eggs(self):
+        """
+        Test old-style egg packages with a variation of 'top_level.txt',
+        'SOURCES.txt', and 'installed-files.txt', available.
+        """
+        distributions = packages_distributions()
+
+        def import_names_from_package(package_name):
+            return {
+                import_name
+                for import_name, package_names in distributions.items()
+                if package_name in package_names
+            }
+
+        # egginfo-pkg declares one import ('mod') via top_level.txt
+        assert import_names_from_package('egginfo-pkg') == {'mod'}
+
+        # egg_with_module-pkg has one import ('egg_with_module') inferred from
+        # installed-files.txt (top_level.txt is missing)
+        assert import_names_from_package('egg_with_module-pkg') == {'egg_with_module'}
+
+        # egg_with_no_modules-pkg should not be associated with any import names
+        # (top_level.txt is empty, and installed-files.txt has no .py files)
+        assert import_names_from_package('egg_with_no_modules-pkg') == set()
+
+        # sources_fallback-pkg has one import ('sources_fallback') inferred from
+        # SOURCES.txt (top_level.txt and installed-files.txt is missing)
+        assert import_names_from_package('sources_fallback-pkg') == {'sources_fallback'}
```

### Comparing `importlib_metadata-6.2.1/tests/test_py39compat.py` & `importlib_metadata-6.3.0/tests/test_py39compat.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.1/tests/test_zip.py` & `importlib_metadata-6.3.0/tests/test_zip.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.1/tox.ini` & `importlib_metadata-6.3.0/tox.ini`

 * *Files identical despite different names*

