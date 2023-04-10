# Comparing `tmp/python-project-structure-0.8.4b0.tar.gz` & `tmp/python-project-structure-0.8.4b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-project-structure-0.8.4b0.tar", last modified: Sun Apr  9 23:42:31 2023, max compression
+gzip compressed data, was "python-project-structure-0.8.4b1.tar", last modified: Mon Apr 10 18:57:17 2023, max compression
```

## Comparing `python-project-structure-0.8.4b0.tar` & `python-project-structure-0.8.4b1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.512361 python-project-structure-0.8.4b0/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      543 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/.dir-locals.el.in
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/.dockerignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      687 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/.env.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.497359 python-project-structure-0.8.4b0/.github/
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.503360 python-project-structure-0.8.4b0/.github/workflows/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4593 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/.github/workflows/build-test.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3704 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/.gitlab-ci.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      779 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/.pre-commit-config.yaml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2377 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/.prospector.yaml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3931 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/CONTRIBUTING.rst
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2519 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/Dockerfile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2859 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/Dockerfile.devel
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1081 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/LICENSE
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    56333 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/Makefile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2704 2023-04-09 23:42:20.000000 python-project-structure-0.8.4b0/NEWS.rst
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13177 2023-04-09 23:42:31.512361 python-project-structure-0.8.4b0/PKG-INFO
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    12114 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/README.rst
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2744 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/TODO.rst
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.504360 python-project-structure-0.8.4b0/bin/
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2792 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/bin/cz-check-bump
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      977 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/bin/entrypoint
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     1101 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/bin/get-base-version
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      321 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/bin/hadolint
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.506360 python-project-structure-0.8.4b0/build-host/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2092 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/build-host/Dockerfile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1438 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/build-host/Makefile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      746 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/build-host/README.rst
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.506360 python-project-structure-0.8.4b0/build-host/bin/
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2058 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/build-host/bin/entrypoint
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      731 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/build-host/requirements-py310.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      674 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/build-host/requirements-py311.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      948 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/build-host/requirements-py37.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/build-host/requirements-py38.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/build-host/requirements-py39.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)        4 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/build-host/requirements.txt.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.506360 python-project-structure-0.8.4b0/dist/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      122 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/dist/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4396 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/docker-compose.override.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      650 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/docker-compose.yml
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.506360 python-project-structure-0.8.4b0/home/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       64 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/home/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      327 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/home/.pypirc.in
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2624 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/pyproject.toml
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.507361 python-project-structure-0.8.4b0/requirements/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      578 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/requirements/build.txt.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.507361 python-project-structure-0.8.4b0/requirements/py310/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/requirements/py310/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4945 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/requirements/py310/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/requirements/py310/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.508361 python-project-structure-0.8.4b0/requirements/py311/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/requirements/py311/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4696 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/requirements/py311/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/requirements/py311/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.508361 python-project-structure-0.8.4b0/requirements/py37/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2645 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/requirements/py37/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5416 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/requirements/py37/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      406 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/requirements/py37/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.509361 python-project-structure-0.8.4b0/requirements/py38/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2515 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/requirements/py38/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4985 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/requirements/py38/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/requirements/py38/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.510361 python-project-structure-0.8.4b0/requirements/py39/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2412 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/requirements/py39/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4972 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/requirements/py39/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/requirements/py39/user.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1701 2023-04-09 23:42:31.513361 python-project-structure-0.8.4b0/setup.cfg
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.499360 python-project-structure-0.8.4b0/src/
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.511361 python-project-structure-0.8.4b0/src/python_project_structure.egg-info/
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13177 2023-04-09 23:42:31.000000 python-project-structure-0.8.4b0/src/python_project_structure.egg-info/PKG-INFO
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)     1768 2023-04-09 23:42:31.000000 python-project-structure-0.8.4b0/src/python_project_structure.egg-info/SOURCES.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)        1 2023-04-09 23:42:31.000000 python-project-structure-0.8.4b0/src/python_project_structure.egg-info/dependency_links.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       73 2023-04-09 23:42:31.000000 python-project-structure-0.8.4b0/src/python_project_structure.egg-info/entry_points.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      146 2023-04-09 23:42:31.000000 python-project-structure-0.8.4b0/src/python_project_structure.egg-info/requires.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       23 2023-04-09 23:42:31.000000 python-project-structure-0.8.4b0/src/python_project_structure.egg-info/top_level.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.512361 python-project-structure-0.8.4b0/src/pythonprojectstructure/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4262 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/src/pythonprojectstructure/__init__.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      201 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/src/pythonprojectstructure/__main__.py
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.512361 python-project-structure-0.8.4b0/src/pythonprojectstructure/newsfragments/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       91 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/src/pythonprojectstructure/newsfragments/.gitignore
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.512361 python-project-structure-0.8.4b0/src/pythonprojectstructure/tests/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       72 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/src/pythonprojectstructure/tests/__init__.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4438 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/src/pythonprojectstructure/tests/test_cli.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      395 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/src/pythonprojectstructure/utils.py
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      162 2023-04-09 23:42:31.000000 python-project-structure-0.8.4b0/src/pythonprojectstructure/version.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3443 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/tox.ini
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 18:57:17.031834 python-project-structure-0.8.4b1/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      543 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/.dir-locals.el.in
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/.dockerignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      687 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/.env.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 18:57:17.016844 python-project-structure-0.8.4b1/.github/
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 18:57:17.022840 python-project-structure-0.8.4b1/.github/workflows/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4593 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/.github/workflows/build-test.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4148 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/.gitlab-ci.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      779 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/.pre-commit-config.yaml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2377 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/.prospector.yaml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3931 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/CONTRIBUTING.rst
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2519 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/Dockerfile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2859 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/Dockerfile.devel
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1081 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/LICENSE
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    56184 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/Makefile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2930 2023-04-10 18:57:04.000000 python-project-structure-0.8.4b1/NEWS.rst
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13204 2023-04-10 18:57:17.031834 python-project-structure-0.8.4b1/PKG-INFO
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    12141 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/README.rst
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2744 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/TODO.rst
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 18:57:17.023839 python-project-structure-0.8.4b1/bin/
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2792 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/bin/cz-check-bump
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      977 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/bin/entrypoint
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     1101 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/bin/get-base-version
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      321 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/bin/hadolint
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 18:57:17.024838 python-project-structure-0.8.4b1/build-host/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2092 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/build-host/Dockerfile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1438 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/build-host/Makefile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      746 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/build-host/README.rst
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 18:57:17.025838 python-project-structure-0.8.4b1/build-host/bin/
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2058 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/build-host/bin/entrypoint
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      731 2023-04-10 18:57:07.000000 python-project-structure-0.8.4b1/build-host/requirements-py310.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      674 2023-04-10 18:57:07.000000 python-project-structure-0.8.4b1/build-host/requirements-py311.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      948 2023-04-10 18:57:07.000000 python-project-structure-0.8.4b1/build-host/requirements-py37.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-10 18:57:07.000000 python-project-structure-0.8.4b1/build-host/requirements-py38.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-10 18:57:07.000000 python-project-structure-0.8.4b1/build-host/requirements-py39.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)        4 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/build-host/requirements.txt.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 18:57:17.025838 python-project-structure-0.8.4b1/dist/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      122 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/dist/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4400 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/docker-compose.override.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      651 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/docker-compose.yml
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 18:57:17.025838 python-project-structure-0.8.4b1/home/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       64 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/home/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      327 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/home/.pypirc.in
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2624 2023-04-10 18:57:06.000000 python-project-structure-0.8.4b1/pyproject.toml
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 18:57:17.025838 python-project-structure-0.8.4b1/requirements/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      578 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/requirements/build.txt.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 18:57:17.026837 python-project-structure-0.8.4b1/requirements/py310/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/requirements/py310/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4945 2023-04-10 18:57:07.000000 python-project-structure-0.8.4b1/requirements/py310/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-10 18:57:07.000000 python-project-structure-0.8.4b1/requirements/py310/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 18:57:17.026837 python-project-structure-0.8.4b1/requirements/py311/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/requirements/py311/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4696 2023-04-10 18:57:07.000000 python-project-structure-0.8.4b1/requirements/py311/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-10 18:57:07.000000 python-project-structure-0.8.4b1/requirements/py311/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 18:57:17.027836 python-project-structure-0.8.4b1/requirements/py37/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2645 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/requirements/py37/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5416 2023-04-10 18:57:07.000000 python-project-structure-0.8.4b1/requirements/py37/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      406 2023-04-10 18:57:07.000000 python-project-structure-0.8.4b1/requirements/py37/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 18:57:17.028836 python-project-structure-0.8.4b1/requirements/py38/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2515 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/requirements/py38/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4985 2023-04-10 18:57:07.000000 python-project-structure-0.8.4b1/requirements/py38/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-10 18:57:07.000000 python-project-structure-0.8.4b1/requirements/py38/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 18:57:17.028836 python-project-structure-0.8.4b1/requirements/py39/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2412 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/requirements/py39/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4972 2023-04-10 18:57:07.000000 python-project-structure-0.8.4b1/requirements/py39/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-10 18:57:07.000000 python-project-structure-0.8.4b1/requirements/py39/user.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1701 2023-04-10 18:57:17.032833 python-project-structure-0.8.4b1/setup.cfg
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 18:57:17.018843 python-project-structure-0.8.4b1/src/
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 18:57:17.029835 python-project-structure-0.8.4b1/src/python_project_structure.egg-info/
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13204 2023-04-10 18:57:16.000000 python-project-structure-0.8.4b1/src/python_project_structure.egg-info/PKG-INFO
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)     1768 2023-04-10 18:57:17.000000 python-project-structure-0.8.4b1/src/python_project_structure.egg-info/SOURCES.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)        1 2023-04-10 18:57:16.000000 python-project-structure-0.8.4b1/src/python_project_structure.egg-info/dependency_links.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       73 2023-04-10 18:57:16.000000 python-project-structure-0.8.4b1/src/python_project_structure.egg-info/entry_points.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      146 2023-04-10 18:57:16.000000 python-project-structure-0.8.4b1/src/python_project_structure.egg-info/requires.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       23 2023-04-10 18:57:16.000000 python-project-structure-0.8.4b1/src/python_project_structure.egg-info/top_level.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 18:57:17.030834 python-project-structure-0.8.4b1/src/pythonprojectstructure/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4262 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/src/pythonprojectstructure/__init__.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      201 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/src/pythonprojectstructure/__main__.py
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 18:57:17.030834 python-project-structure-0.8.4b1/src/pythonprojectstructure/newsfragments/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       91 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/src/pythonprojectstructure/newsfragments/.gitignore
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 18:57:17.031834 python-project-structure-0.8.4b1/src/pythonprojectstructure/tests/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       72 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/src/pythonprojectstructure/tests/__init__.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4438 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/src/pythonprojectstructure/tests/test_cli.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      395 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/src/pythonprojectstructure/utils.py
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      162 2023-04-10 18:57:16.000000 python-project-structure-0.8.4b1/src/pythonprojectstructure/version.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3443 2023-04-10 18:55:20.000000 python-project-structure-0.8.4b1/tox.ini
```

### Comparing `python-project-structure-0.8.4b0/.dir-locals.el.in` & `python-project-structure-0.8.4b1/.dir-locals.el.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/.dockerignore` & `python-project-structure-0.8.4b1/.dockerignore`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/.env.in` & `python-project-structure-0.8.4b1/.env.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/.github/workflows/build-test.yml` & `python-project-structure-0.8.4b1/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/.gitignore` & `python-project-structure-0.8.4b1/.gitignore`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/.gitlab-ci.yml` & `python-project-structure-0.8.4b1/.gitlab-ci.yml`

 * *Files 7% similar despite different names*

```diff
@@ -7,21 +7,25 @@
 #   A Docker Hub Personal Access Token
 # - `GPG_PASSPHRASE`:
 #   See the comments towards the bottom of the `./Makefile`
 # - `GPG_SIGNING_PRIVATE_KEY`:
 #   See the comments towards the bottom of the `./Makefile`
 # - `PROJECT_GITHUB_PAT`:
 #   A GitHub "Classic" Personal Access Token with scopes: `repo`, `workflow`,
-#   `packages`, and `project`
+#   `packages`, and `project`. If using both GitLab CI/CD for releases and GitHub
+#   Actions as duplicate CI for tests, then configure repository mirroring in your
+#   GitLab project -> Settings -> Repository using the same token.
 # - `PYPI_PASSWORD`:
 #   A PyPI API token
 # - `TEST_PYPI_PASSWORD`:
 #   A PyPI API token
 # - `VCS_REMOTE_PUSH_URL`:
-#   See the comments towards the bottom of the `./Makefile`
+#   A GitLab Personal or Project Access Token formatted as an HTTP authentication prefix
+#   to the hostname, e.g.:
+#     https://token-name:token-value@gitlab.com/rpatterson/python-project-structure.git
 
 default:
   image:
     name: "$CI_TEMPLATE_REGISTRY_HOST/rpatterson/$CI_PROJECT_NAME:build-host"
     entrypoint:
       - "docker-entrypoint.sh"
   services:
@@ -45,15 +49,16 @@
   - "release"
   - "scheduled"
 
 build-test:
   stage: "build-test"
   rules:
     - if: >-
-        $CI_COMMIT_TAG
+        $CI_COMMIT_TAG ||
+        $CI_COMMIT_MESSAGE =~ "^\[ci skip\]$"
       when: "never"
     - if: >-
         $CI_PIPELINE_SOURCE != "schedule"
   interruptible: true
   parallel:
     matrix:
       - PYTHON_MINORS:
@@ -94,15 +99,16 @@
   # Avoid unnecessary artifact downloads:
   # https://docs.gitlab.com/ee/ci/yaml/#dependencies
   dependencies: []
   variables:
     DOCKER_BUILD_PULL: "true"
   rules:
     - if: >-
-        $CI_COMMIT_TAG
+        $CI_COMMIT_TAG ||
+        $CI_COMMIT_MESSAGE =~ "^\[ci skip\]$"
       when: "never"
     - if: >-
         $CI_PROJECT_NAMESPACE == "rpatterson"
         && $CI_COMMIT_BRANCH != null
         && $CI_COMMIT_BRANCH =~ "^(develop|master)$"
         && $CI_PIPELINE_SOURCE != "schedule"
   script:
```

### Comparing `python-project-structure-0.8.4b0/.pre-commit-config.yaml` & `python-project-structure-0.8.4b1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/.prospector.yaml` & `python-project-structure-0.8.4b1/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/CONTRIBUTING.rst` & `python-project-structure-0.8.4b1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/Dockerfile` & `python-project-structure-0.8.4b1/Dockerfile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/Dockerfile.devel` & `python-project-structure-0.8.4b1/Dockerfile.devel`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/LICENSE` & `python-project-structure-0.8.4b1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/Makefile` & `python-project-structure-0.8.4b1/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -186,14 +186,17 @@
 CI_TEMPLATE_REGISTRY_HOST=registry.gitlab.com
 CI_REGISTRY=$(CI_TEMPLATE_REGISTRY_HOST)/$(CI_PROJECT_NAMESPACE)
 CI_REGISTRY_IMAGE=$(CI_REGISTRY)/$(CI_PROJECT_NAME)
 DOCKER_COMPOSE_RUN_ARGS=--rm
 ifneq ($(CI),true)
 DOCKER_COMPOSE_RUN_ARGS+= --quiet-pull
 endif
+ifeq ($(shell tty),not a tty)
+DOCKER_COMPOSE_RUN_ARGS+= -T
+endif
 DOCKER_BUILD_ARGS=
 DOCKER_REGISTRIES=DOCKER GITLAB GITHUB
 export DOCKER_REGISTRY=$(firstword $(DOCKER_REGISTRIES))
 DOCKER_IMAGE_DOCKER=$(DOCKER_USER)/$(CI_PROJECT_NAME)
 DOCKER_IMAGE_GITLAB=$(CI_REGISTRY_IMAGE)
 DOCKER_IMAGE_GITHUB=ghcr.io/$(CI_PROJECT_NAMESPACE)/$(CI_PROJECT_NAME)
 DOCKER_IMAGE=$(DOCKER_IMAGE_$(DOCKER_REGISTRY))
@@ -347,23 +350,22 @@
 build-pkgs: ./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) \
 		./var/docker/$(PYTHON_ENV)/log/build-devel.log build-docker-volumes-$(PYTHON_ENV)
 # Defined as a .PHONY recipe so that multiple targets can depend on this as a
 # pre-requisite and it will only be run once per invocation.
 	rm -vf ./dist/*
 # Build Python packages/distributions from the development Docker container for
 # consistency/reproducibility.
-	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) -T \
-	    python-project-structure-devel tox run -e "$(PYTHON_ENV)" --pkg-only
+	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) python-project-structure-devel \
+	    tox run -e "$(PYTHON_ENV)" --pkg-only
 # Copy the wheel to a location accessible to all containers:
 	cp -lfv "$$(
 	    ls -t ./var/docker/$(PYTHON_ENV)/.tox/.pkg/dist/*.whl | head -n 1
 	)" "./dist/"
 # Also build the source distribution:
-	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) -T \
-	    python-project-structure-devel \
+	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) python-project-structure-devel \
 	    tox run -e "$(PYTHON_ENV)" --override "testenv.package=sdist" --pkg-only
 	cp -lfv "$$(
 	    ls -t ./var/docker/$(PYTHON_ENV)/.tox/.pkg/dist/*.tar.gz | head -n 1
 	)" "./dist/"
 
 .PHONY: $(PYTHON_ENVS:%=build-requirements-%)
 ### Compile fixed/pinned dependency versions if necessary.
@@ -444,17 +446,16 @@
 .PHONY: $(PYTHON_MINORS:%=build-docker-requirements-%)
 ### Pull container images and compile fixed/pinned dependency versions if necessary.
 $(PYTHON_MINORS:%=build-docker-requirements-%): ./.env
 	export PYTHON_MINOR="$(@:build-docker-requirements-%=%)"
 	export PYTHON_ENV="py$(subst .,,$(@:build-docker-requirements-%=%))"
 	$(MAKE) -e build-docker-volumes-$${PYTHON_ENV} \
 	    "./var/docker/$(PYTHON_ENV)/log/build-devel.log"
-	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) -T \
-	    python-project-structure-devel make -e \
-	    PYTHON_MINORS="$(@:build-docker-requirements-%=%)" \
+	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) python-project-structure-devel \
+	    make -e PYTHON_MINORS="$(@:build-docker-requirements-%=%)" \
 	    PIP_COMPILE_ARGS="$(PIP_COMPILE_ARGS)" \
 	    build-requirements-py$(subst .,,$(@:build-docker-requirements-%=%))
 
 .PHONY: $(PYTHON_ENVS:%=build-docker-volumes-%)
 ### Ensure access permissions to build artifacts in Python version container volumes.
 # If created by `# dockerd`, they end up owned by `root`.
 $(PYTHON_ENVS:%=build-docker-volumes-%): \
@@ -532,19 +533,19 @@
 endif
 endif
 
 .PHONY: test-docker-lint
 ### Check the style and content of the `./Dockerfile*` files.
 test-docker-lint: ./.env build-docker-volumes-$(PYTHON_ENV)
 	docker compose pull hadolint
-	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) -T hadolint \
+	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) hadolint \
 	    hadolint "./Dockerfile"
-	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) -T hadolint \
+	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) hadolint \
 	    hadolint "./Dockerfile.devel"
-	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) -T hadolint \
+	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) hadolint \
 	    hadolint "./build-host/Dockerfile"
 
 .PHONY: test-push
 ### Perform any checks that should only be run before pushing.
 test-push: $(VCS_FETCH_TARGETS) \
 		$(HOME)/.local/var/log/python-project-structure-host-install.log \
 		./var/docker/$(PYTHON_ENV)/log/build-devel.log \
@@ -637,14 +638,21 @@
 # https://twine.readthedocs.io/en/latest/#using-twine
 	./.tox/build/bin/twine check ./dist/python?project?structure-*
 # The VCS remote should reflect the release before the release is published to ensure
 # that a published release is never *not* reflected in VCS.  Also ensure the tag is in
 # place on any mirrors, using multiple `pushurl` remotes, for those project hosts as
 # well:
 	$(MAKE) -e test-clean
+ifneq ($(GITHUB_ACTIONS),true)
+ifneq ($(PROJECT_GITHUB_PAT),)
+# Ensure the tag is available for creating the GitHub release below but push *before* to
+# GitLab to avoid a race with repository mirrorying:
+	git push --no-verify --tags "github" "HEAD:$(VCS_BRANCH)"
+endif
+endif
 	git push --no-verify --tags "$(VCS_REMOTE)" "HEAD:$(VCS_BRANCH)"
 	./.tox/build/bin/twine upload -s -r "$(PYPI_REPO)" \
 	    ./dist/python?project?structure-*
 	export VERSION=$$(./.tox/build/bin/cz version --project)
 # Create a GitLab release
 	./.tox/build/bin/twine upload -s -r "gitlab" \
 	    ./dist/python?project?structure-*
@@ -935,15 +943,15 @@
 	export VERSION=$$(./.tox/build/bin/cz version --project)
 ifeq ($(DOCKER_BUILD_PULL),true)
 # Pull the development image and simulate as if it had been built here.
 	if $(MAKE) -e DOCKER_VARIANT="devel" pull-docker
 	then
 	    touch "$(@)" "./var/docker/$(PYTHON_ENV)/log/rebuild.log"
 # Ensure the virtualenv in the volume is also current:
-	    docker compose run $(DOCKER_COMPOSE_RUN_ARGS) -T \
+	    docker compose run $(DOCKER_COMPOSE_RUN_ARGS) \
 	        python-project-structure-devel make -e PYTHON_MINORS="$(PYTHON_MINOR)" \
 	        "./var/log/tox/$(PYTHON_ENV)/build.log"
 	    exit
 	fi
 else
 # https://github.com/moby/moby/issues/39003#issuecomment-879441675
 	docker_build_args="$(DOCKER_BUILD_ARGS) \
@@ -996,17 +1004,16 @@
 	docker push \
 	    "$(DOCKER_IMAGE_GITHUB):devel-$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
 endif
 endif
 	date >>"$(@)"
 # Update the pinned/frozen versions, if needed, using the container.  If changed, then
 # we may need to re-build the container image again to ensure it's current and correct.
-	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) -T \
-	    python-project-structure-devel make -e PYTHON_MINORS="$(PYTHON_MINOR)" \
-	    build-requirements-$(PYTHON_ENV)
+	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) python-project-structure-devel \
+	    make -e PYTHON_MINORS="$(PYTHON_MINOR)" build-requirements-$(PYTHON_ENV)
 ifeq ($(CI),true)
 # On CI, any changes from compiling requirements is a failure so no need to waste time
 # rebuilding images:
 	touch "$(@)"
 else
 	$(MAKE) -e "$(@)"
 endif
@@ -1188,26 +1195,18 @@
 	git config --global user.name "$(USER_FULL_NAME)"
 	git config --global user.email "$(USER_EMAIL)"
 
 ./var/log/git-remotes.log:
 ifeq ($(RELEASE_PUBLISH),true)
 	set +x
 ifneq ($(VCS_REMOTE_PUSH_URL),)
-# Requires a Personal or Project Access Token in the GitLab CI/CD Variables.  That
-# variable value should be prefixed with the token name as a HTTP `user:password`
-# authentication string:
-# https://stackoverflow.com/a/73426417/624787
 	git remote set-url --push --add "origin" "$(VCS_REMOTE_PUSH_URL)"
 endif
 ifneq ($(GITHUB_ACTIONS),true)
 ifneq ($(PROJECT_GITHUB_PAT),)
-# Also push to the mirror with the `ci.skip` option to avoid redundant runs on the
-# mirror.
-	git remote set-url --push --add "origin" \
-	    "https://$(PROJECT_GITHUB_PAT)@github.com/$(CI_PROJECT_PATH).git"
 # Also add a fetch remote for the `$ gh ...` CLI tool to detect:
 	git remote add "github" \
 	    "https://$(PROJECT_GITHUB_PAT)@github.com/$(CI_PROJECT_PATH).git"
 else ifneq ($(CI_IS_FORK),true)
 	set +x
 	echo "ERROR: PROJECT_GITHUB_PAT missing from ./.env or CI secrets"
 	false
```

### Comparing `python-project-structure-0.8.4b0/NEWS.rst` & `python-project-structure-0.8.4b1/NEWS.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+python-project-structure 0.8.4b1 (2023-04-10)
+=============================================
+
+Bugfixes
+--------
+
+- Upgrade all requirements to the latest versions as of Mon Apr 10 06:25:02 PM UTC 2023. (upgrade-requirements)
+
+
 python-project-structure 0.8.4b0 (2023-04-09)
 =============================================
 
 Bugfixes
 --------
 
 - Upgrade all requirements to the latest versions as of Sun Apr  9 11:19:15 PM UTC 2023. (upgrade-requirements)
```

### Comparing `python-project-structure-0.8.4b0/PKG-INFO` & `python-project-structure-0.8.4b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-project-structure
-Version: 0.8.4b0
+Version: 0.8.4b1
 Summary: Python project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/python-project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
@@ -62,23 +62,23 @@
 	  :target: https://gitlab.com/rpatterson/python-project-structure
 
      - .. figure:: https://img.shields.io/github/v/release/rpatterson/python-project-structure?logo=github
 	  :alt: GitHub release (latest SemVer)
 	  :target: https://github.com/rpatterson/python-project-structure/releases
        .. figure:: https://github.com/rpatterson/python-project-structure/actions/workflows/ci-cd.yml/badge.svg
           :alt: GitHub Actions status
-          :target: https://github.com/rpatterson/python-project-structure/
-       .. figure:: https://codecov.io/github/rpatterson/python-project-structure/branch/master/graph/badge.svg?token=GNKVQ8VYOU 
+          :target: https://github.com/rpatterson/python-project-structure/actions/workflows/build-test.yml
+       .. figure:: https://github.com/rpatterson/python-project-structure/actions/workflows/build-test.yml/badge.svg
           :alt: Codecov test coverage
 	  :target: https://codecov.io/github/rpatterson/python-project-structure
        .. figure:: https://img.shields.io/github/stars/rpatterson/python-project-structure?logo=github
 	  :alt: GitHub repo stars
 	  :target: https://github.com/rpatterson/python-project-structure/
 
-     - .. figure:: https://img.shields.io/docker/v/merpatterson/python-project-structure?sort=semver&logo=docker
+     - .. figure:: https://img.shields.io/docker/v/merpatterson/python-project-structure/master?sort=semver&logo=docker
           :alt: Docker Hub image version (latest semver)
           :target: https://hub.docker.com/r/merpatterson/python-project-structure
        .. figure:: https://img.shields.io/docker/pulls/merpatterson/python-project-structure?logo=docker
           :alt: Docker Hub image pulls count
           :target: https://hub.docker.com/r/merpatterson/python-project-structure
        .. figure:: https://img.shields.io/docker/stars/merpatterson/python-project-structure?logo=docker
 	  :alt: Docker Hub stars
```

### Comparing `python-project-structure-0.8.4b0/README.rst` & `python-project-structure-0.8.4b1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -34,23 +34,23 @@
 	  :target: https://gitlab.com/rpatterson/python-project-structure
 
      - .. figure:: https://img.shields.io/github/v/release/rpatterson/python-project-structure?logo=github
 	  :alt: GitHub release (latest SemVer)
 	  :target: https://github.com/rpatterson/python-project-structure/releases
        .. figure:: https://github.com/rpatterson/python-project-structure/actions/workflows/ci-cd.yml/badge.svg
           :alt: GitHub Actions status
-          :target: https://github.com/rpatterson/python-project-structure/
-       .. figure:: https://codecov.io/github/rpatterson/python-project-structure/branch/master/graph/badge.svg?token=GNKVQ8VYOU 
+          :target: https://github.com/rpatterson/python-project-structure/actions/workflows/build-test.yml
+       .. figure:: https://github.com/rpatterson/python-project-structure/actions/workflows/build-test.yml/badge.svg
           :alt: Codecov test coverage
 	  :target: https://codecov.io/github/rpatterson/python-project-structure
        .. figure:: https://img.shields.io/github/stars/rpatterson/python-project-structure?logo=github
 	  :alt: GitHub repo stars
 	  :target: https://github.com/rpatterson/python-project-structure/
 
-     - .. figure:: https://img.shields.io/docker/v/merpatterson/python-project-structure?sort=semver&logo=docker
+     - .. figure:: https://img.shields.io/docker/v/merpatterson/python-project-structure/master?sort=semver&logo=docker
           :alt: Docker Hub image version (latest semver)
           :target: https://hub.docker.com/r/merpatterson/python-project-structure
        .. figure:: https://img.shields.io/docker/pulls/merpatterson/python-project-structure?logo=docker
           :alt: Docker Hub image pulls count
           :target: https://hub.docker.com/r/merpatterson/python-project-structure
        .. figure:: https://img.shields.io/docker/stars/merpatterson/python-project-structure?logo=docker
 	  :alt: Docker Hub stars
```

### Comparing `python-project-structure-0.8.4b0/TODO.rst` & `python-project-structure-0.8.4b1/TODO.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/bin/cz-check-bump` & `python-project-structure-0.8.4b1/bin/cz-check-bump`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/bin/entrypoint` & `python-project-structure-0.8.4b1/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/bin/get-base-version` & `python-project-structure-0.8.4b1/bin/get-base-version`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/build-host/Dockerfile` & `python-project-structure-0.8.4b1/build-host/Dockerfile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/build-host/Makefile` & `python-project-structure-0.8.4b1/build-host/Makefile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/build-host/README.rst` & `python-project-structure-0.8.4b1/build-host/README.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/build-host/bin/entrypoint` & `python-project-structure-0.8.4b1/build-host/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/build-host/requirements-py310.txt` & `python-project-structure-0.8.4b1/build-host/requirements-py310.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/build-host/requirements-py311.txt` & `python-project-structure-0.8.4b1/build-host/requirements-py311.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/build-host/requirements-py37.txt` & `python-project-structure-0.8.4b1/build-host/requirements-py37.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     # via tox
 distlib==0.3.6
     # via virtualenv
 filelock==3.11.0
     # via
     #   tox
     #   virtualenv
-importlib-metadata==6.2.1
+importlib-metadata==6.3.0
     # via
     #   pluggy
     #   tox
     #   virtualenv
 packaging==23.0
     # via
     #   pyproject-api
```

### Comparing `python-project-structure-0.8.4b0/build-host/requirements-py38.txt` & `python-project-structure-0.8.4b1/build-host/requirements-py38.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/build-host/requirements-py39.txt` & `python-project-structure-0.8.4b1/build-host/requirements-py39.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/docker-compose.override.yml` & `python-project-structure-0.8.4b1/docker-compose.override.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # Override `$ docker compose ...` configuration for development or testing here in this
 # repo checkout.  Everything that may be used outside this checkout should be in
 # `./docker-compose.yml`.
 version: "3.8"
 
 services:
 
-  ## Configuration specific to this checkout
+  # Configuration specific to development:
   python-project-structure:
     image: "merpatterson/python-project-structure:${PYTHON_ENV:-py310}-${DOCKER_BRANCH_TAG:-develop}"
     container_name: "python-project-structure-checkout"
     build:
       context: "${CHECKOUT_DIR}/"
       args:
         PYTHON_MINOR: "${PYTHON_MINOR:-3.10}"
         PYTHON_ENV: "${PYTHON_ENV:-py310}"
         VERSION: "${VERSION:-}"
     volumes:
       # Preserve caches caches between container runs
       - "${CHECKOUT_DIR}/home/:/home/python-project-structure/"
 
-  ## Container for use by developers
+  ## Contianers used for development and release:
+
+  # Container for use by developers:
   python-project-structure-devel:
     image: "merpatterson/python-project-structure:devel-${PYTHON_ENV:-py310}-${DOCKER_BRANCH_TAG:-develop}"
     container_name: "python-project-structure-devel"
     build:
       context: "${CHECKOUT_DIR}/"
       dockerfile: "${CHECKOUT_DIR}/Dockerfile.devel"
       args:
@@ -46,16 +48,14 @@
       - "${CHECKOUT_DIR}/home/:/home/python-project-structure/"
       # Avoid any clashes between image variants and/or the local host at both build and
       # run-time.
       - "${CHECKOUT_DIR}/var/docker/${PYTHON_ENV:-py310}/:/usr/local/src/python-project-structure/var/"
       - "${CHECKOUT_DIR}/var/docker/${PYTHON_ENV:-py310}/.tox/:/usr/local/src/python-project-structure/.tox/"
       - "${CHECKOUT_DIR}/var/docker/${PYTHON_ENV:-py310}/python_project_structure.egg-info/:/usr/local/src/python-project-structure/src/python_project_structure.egg-info/"
 
-  ## Contianers during development and release
-
   # https://github.com/hadolint/hadolint#how-to-use
   hadolint:
     image: "hadolint/hadolint"
     environment:
       TZ: "${TZ:-Etc/UTC}"
     volumes:
       - "${CHECKOUT_DIR}/:/usr/local/src/python-project-structure/"
@@ -82,15 +82,24 @@
       DOCKER_PASS: "${DOCKER_PASS}"
     volumes:
       - "${CHECKOUT_DIR}/:/data/"
     command: >-
       --file "/data/README.md" --short "Python project structure foundation or template"
       --debug "merpatterson/python-project-structure"
 
-  ## Container for use by end users
+  gitlab-release-cli:
+    image: "registry.gitlab.com/gitlab-org/release-cli:latest"
+    environment:
+      CI_JOB_TOKEN: "${CI_JOB_TOKEN:-}"
+    volumes:
+      - "./:/usr/local/src/python-project-structure/"
+    working_dir: "/usr/local/src/python-project-structure/"
+
+  ## Containers for simulating CI/CD:
+
   build-host:
     image: "merpatterson/python-project-structure:build-host"
     build: "${CHECKOUT_DIR}/build-host/"
     privileged: true
     volumes:
       - "/var/run/docker.sock:/var/run/docker.sock"
       - "${CHECKOUT_DIR}/:${CHECKOUT_DIR}"
@@ -102,15 +111,7 @@
       TZ: "${TZ:-Etc/UTC}"
       PUID: "${PUID:-1000}"
       PGID: "${DOCKER_GID:-${PGID:-${PUID:-1000}}}"
       # DEBUG: "true"
     working_dir: "${CHECKOUT_DIR}"
     command: >-
       make -e build-docker test-docker release
-
-  gitlab-release-cli:
-    image: "registry.gitlab.com/gitlab-org/release-cli:latest"
-    environment:
-      CI_JOB_TOKEN: "${CI_JOB_TOKEN:-}"
-    volumes:
-      - "./:/usr/local/src/python-project-structure/"
-    working_dir: "/usr/local/src/python-project-structure/"
```

### Comparing `python-project-structure-0.8.4b0/docker-compose.yml` & `python-project-structure-0.8.4b1/docker-compose.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Minimal `$ docker compose ...` configuration to demonstrate the requirements for
 # running python-project-structure in containers.
 version: "3.8"
 
 services:
 
-  ## Container for use by end users
+  ## Container for use by end users:
   python-project-structure:
     image: "merpatterson/python-project-structure"
     container_name: "python-project-structure"
     environment:
       TZ: "${TZ:-Etc/UTC}"
       # Make the run-time user configurable in `./.env` to match permissions inside and
       # outside the container.  Default to the common/standard main/first user and group
```

### Comparing `python-project-structure-0.8.4b0/pyproject.toml` & `python-project-structure-0.8.4b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # versin tag should be a major, minor or patch bump and create the VCS tag.  Also
 # provides VCS hooks to enforce that commit messages comply with conventional commits:
 # https://commitizen-tools.github.io/commitizen/
 name = "cz_conventional_commits"
 # TEMPLATE: Update these versions to the latest version for your project and ensure the
 # tag exists both locally and on the project's remote:
 changelog_start_rev = "v0.0.0"
-version = "0.8.4b0"
+version = "0.8.4b1"
 tag_format = "v$version"
 annotated_tag = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
 [ci skip]
 """
```

### Comparing `python-project-structure-0.8.4b0/requirements/build.txt.in` & `python-project-structure-0.8.4b1/requirements/build.txt.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/requirements/py310/build.txt` & `python-project-structure-0.8.4b1/requirements/py310/build.txt`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     # via readme-renderer
 filelock==3.11.0
     # via virtualenv
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==6.2.1
+importlib-metadata==6.3.0
     # via
     #   keyring
     #   twine
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
@@ -68,15 +68,15 @@
     # via virtualenv
 pre-commit==3.2.2
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
-pygments==2.14.0
+pygments==2.15.0
     # via
     #   readme-renderer
     #   rich
 pyyaml==6.0
     # via
     #   commitizen
     #   pre-commit
```

### Comparing `python-project-structure-0.8.4b0/requirements/py310/devel.txt` & `python-project-structure-0.8.4b1/requirements/py310/devel.txt`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 pydocstyle==6.3.0
     # via prospector
 pyflakes==2.5.0
     # via
     #   autoflake
     #   flake8
     #   prospector
-pygments==2.14.0
+pygments==2.15.0
     # via
     #   pyroma
     #   rich
 pylint==2.17.2
     # via
     #   prospector
     #   pylint-celery
```

### Comparing `python-project-structure-0.8.4b0/requirements/py311/build.txt` & `python-project-structure-0.8.4b1/requirements/py311/build.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     # via readme-renderer
 filelock==3.11.0
     # via virtualenv
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==6.2.1
+importlib-metadata==6.3.0
     # via
     #   keyring
     #   twine
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
@@ -68,15 +68,15 @@
     # via virtualenv
 pre-commit==3.2.2
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
-pygments==2.14.0
+pygments==2.15.0
     # via
     #   readme-renderer
     #   rich
 pyyaml==6.0
     # via
     #   commitizen
     #   pre-commit
```

### Comparing `python-project-structure-0.8.4b0/requirements/py311/devel.txt` & `python-project-structure-0.8.4b1/requirements/py311/devel.txt`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 pydocstyle==6.3.0
     # via prospector
 pyflakes==2.5.0
     # via
     #   autoflake
     #   flake8
     #   prospector
-pygments==2.14.0
+pygments==2.15.0
     # via
     #   pyroma
     #   rich
 pylint==2.17.2
     # via
     #   prospector
     #   pylint-celery
```

### Comparing `python-project-structure-0.8.4b0/requirements/py37/build.txt` & `python-project-structure-0.8.4b1/requirements/py38/build.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.7
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py37/build.txt --resolver=backtracking requirements/build.txt.in
+#    pip-compile --output-file=requirements/py38/build.txt --resolver=backtracking requirements/build.txt.in
 #
 argcomplete==2.0.6
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
 certifi==2022.12.7
     # via requests
@@ -32,21 +32,18 @@
     # via readme-renderer
 filelock==3.11.0
     # via virtualenv
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==5.2.0
+importlib-metadata==6.3.0
     # via
-    #   argcomplete
     #   keyring
-    #   pre-commit
     #   twine
-    #   virtualenv
 importlib-resources==5.12.0
     # via keyring
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
@@ -67,21 +64,21 @@
     # via pre-commit
 packaging==23.0
     # via commitizen
 pkginfo==1.9.6
     # via twine
 platformdirs==3.2.0
     # via virtualenv
-pre-commit==2.21.0
+pre-commit==3.2.2
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
-pygments==2.14.0
+pygments==2.15.0
     # via
     #   readme-renderer
     #   rich
 pyyaml==6.0
     # via
     #   commitizen
     #   pre-commit
@@ -108,17 +105,14 @@
 tomlkit==0.11.7
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
 typing-extensions==4.5.0
     # via
     #   commitizen
-    #   importlib-metadata
-    #   markdown-it-py
-    #   platformdirs
     #   rich
 urllib3==1.26.15
     # via
     #   requests
     #   twine
 virtualenv==20.21.0
     # via pre-commit
```

### Comparing `python-project-structure-0.8.4b0/requirements/py37/devel.txt` & `python-project-structure-0.8.4b1/requirements/py37/devel.txt`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 pydocstyle==6.3.0
     # via prospector
 pyflakes==2.5.0
     # via
     #   autoflake
     #   flake8
     #   prospector
-pygments==2.14.0
+pygments==2.15.0
     # via
     #   pyroma
     #   rich
 pylint==2.17.2
     # via
     #   prospector
     #   pylint-celery
```

### Comparing `python-project-structure-0.8.4b0/requirements/py38/build.txt` & `python-project-structure-0.8.4b1/requirements/py37/build.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.7
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py38/build.txt --resolver=backtracking requirements/build.txt.in
+#    pip-compile --output-file=requirements/py37/build.txt --resolver=backtracking requirements/build.txt.in
 #
 argcomplete==2.0.6
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
 certifi==2022.12.7
     # via requests
@@ -32,18 +32,21 @@
     # via readme-renderer
 filelock==3.11.0
     # via virtualenv
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==6.2.1
+importlib-metadata==5.2.0
     # via
+    #   argcomplete
     #   keyring
+    #   pre-commit
     #   twine
+    #   virtualenv
 importlib-resources==5.12.0
     # via keyring
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
@@ -64,21 +67,21 @@
     # via pre-commit
 packaging==23.0
     # via commitizen
 pkginfo==1.9.6
     # via twine
 platformdirs==3.2.0
     # via virtualenv
-pre-commit==3.2.2
+pre-commit==2.21.0
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
-pygments==2.14.0
+pygments==2.15.0
     # via
     #   readme-renderer
     #   rich
 pyyaml==6.0
     # via
     #   commitizen
     #   pre-commit
@@ -105,14 +108,17 @@
 tomlkit==0.11.7
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
 typing-extensions==4.5.0
     # via
     #   commitizen
+    #   importlib-metadata
+    #   markdown-it-py
+    #   platformdirs
     #   rich
 urllib3==1.26.15
     # via
     #   requests
     #   twine
 virtualenv==20.21.0
     # via pre-commit
```

### Comparing `python-project-structure-0.8.4b0/requirements/py38/devel.txt` & `python-project-structure-0.8.4b1/requirements/py38/devel.txt`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 pydocstyle==6.3.0
     # via prospector
 pyflakes==2.5.0
     # via
     #   autoflake
     #   flake8
     #   prospector
-pygments==2.14.0
+pygments==2.15.0
     # via
     #   pyroma
     #   rich
 pylint==2.17.2
     # via
     #   prospector
     #   pylint-celery
```

### Comparing `python-project-structure-0.8.4b0/requirements/py39/build.txt` & `python-project-structure-0.8.4b1/requirements/py39/build.txt`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     # via readme-renderer
 filelock==3.11.0
     # via virtualenv
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==6.2.1
+importlib-metadata==6.3.0
     # via
     #   keyring
     #   twine
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
@@ -68,15 +68,15 @@
     # via virtualenv
 pre-commit==3.2.2
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
-pygments==2.14.0
+pygments==2.15.0
     # via
     #   readme-renderer
     #   rich
 pyyaml==6.0
     # via
     #   commitizen
     #   pre-commit
```

### Comparing `python-project-structure-0.8.4b0/requirements/py39/devel.txt` & `python-project-structure-0.8.4b1/requirements/py39/devel.txt`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 pydocstyle==6.3.0
     # via prospector
 pyflakes==2.5.0
     # via
     #   autoflake
     #   flake8
     #   prospector
-pygments==2.14.0
+pygments==2.15.0
     # via
     #   pyroma
     #   rich
 pylint==2.17.2
     # via
     #   prospector
     #   pylint-celery
```

### Comparing `python-project-structure-0.8.4b0/setup.cfg` & `python-project-structure-0.8.4b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/src/python_project_structure.egg-info/PKG-INFO` & `python-project-structure-0.8.4b1/src/python_project_structure.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-project-structure
-Version: 0.8.4b0
+Version: 0.8.4b1
 Summary: Python project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/python-project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
@@ -62,23 +62,23 @@
 	  :target: https://gitlab.com/rpatterson/python-project-structure
 
      - .. figure:: https://img.shields.io/github/v/release/rpatterson/python-project-structure?logo=github
 	  :alt: GitHub release (latest SemVer)
 	  :target: https://github.com/rpatterson/python-project-structure/releases
        .. figure:: https://github.com/rpatterson/python-project-structure/actions/workflows/ci-cd.yml/badge.svg
           :alt: GitHub Actions status
-          :target: https://github.com/rpatterson/python-project-structure/
-       .. figure:: https://codecov.io/github/rpatterson/python-project-structure/branch/master/graph/badge.svg?token=GNKVQ8VYOU 
+          :target: https://github.com/rpatterson/python-project-structure/actions/workflows/build-test.yml
+       .. figure:: https://github.com/rpatterson/python-project-structure/actions/workflows/build-test.yml/badge.svg
           :alt: Codecov test coverage
 	  :target: https://codecov.io/github/rpatterson/python-project-structure
        .. figure:: https://img.shields.io/github/stars/rpatterson/python-project-structure?logo=github
 	  :alt: GitHub repo stars
 	  :target: https://github.com/rpatterson/python-project-structure/
 
-     - .. figure:: https://img.shields.io/docker/v/merpatterson/python-project-structure?sort=semver&logo=docker
+     - .. figure:: https://img.shields.io/docker/v/merpatterson/python-project-structure/master?sort=semver&logo=docker
           :alt: Docker Hub image version (latest semver)
           :target: https://hub.docker.com/r/merpatterson/python-project-structure
        .. figure:: https://img.shields.io/docker/pulls/merpatterson/python-project-structure?logo=docker
           :alt: Docker Hub image pulls count
           :target: https://hub.docker.com/r/merpatterson/python-project-structure
        .. figure:: https://img.shields.io/docker/stars/merpatterson/python-project-structure?logo=docker
 	  :alt: Docker Hub stars
```

### Comparing `python-project-structure-0.8.4b0/src/python_project_structure.egg-info/SOURCES.txt` & `python-project-structure-0.8.4b1/src/python_project_structure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/src/pythonprojectstructure/__init__.py` & `python-project-structure-0.8.4b1/src/pythonprojectstructure/__init__.py`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/src/pythonprojectstructure/tests/test_cli.py` & `python-project-structure-0.8.4b1/src/pythonprojectstructure/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.4b0/tox.ini` & `python-project-structure-0.8.4b1/tox.ini`

 * *Files identical despite different names*

