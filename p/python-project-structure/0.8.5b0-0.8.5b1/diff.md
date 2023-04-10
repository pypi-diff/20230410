# Comparing `tmp/python-project-structure-0.8.5b0.tar.gz` & `tmp/python-project-structure-0.8.5b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-project-structure-0.8.5b0.tar", last modified: Mon Apr 10 19:50:07 2023, max compression
+gzip compressed data, was "python-project-structure-0.8.5b1.tar", last modified: Mon Apr 10 20:13:59 2023, max compression
```

## Comparing `python-project-structure-0.8.5b0.tar` & `python-project-structure-0.8.5b1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 19:50:07.842652 python-project-structure-0.8.5b0/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      543 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/.dir-locals.el.in
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/.dockerignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      687 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/.env.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 19:50:07.827651 python-project-structure-0.8.5b0/.github/
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 19:50:07.833652 python-project-structure-0.8.5b0/.github/workflows/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4593 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/.github/workflows/build-test.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4152 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/.gitlab-ci.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      779 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/.pre-commit-config.yaml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2377 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/.prospector.yaml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3931 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/CONTRIBUTING.rst
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2519 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/Dockerfile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2859 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/Dockerfile.devel
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1081 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/LICENSE
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    56729 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/Makefile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3045 2023-04-10 19:49:56.000000 python-project-structure-0.8.5b0/NEWS.rst
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-10 19:50:07.842652 python-project-structure-0.8.5b0/PKG-INFO
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    12157 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/README.rst
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2744 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/TODO.rst
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 19:50:07.834652 python-project-structure-0.8.5b0/bin/
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2792 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/bin/cz-check-bump
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      977 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/bin/entrypoint
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     1101 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/bin/get-base-version
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      321 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/bin/hadolint
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 19:50:07.836652 python-project-structure-0.8.5b0/build-host/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2092 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/build-host/Dockerfile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1438 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/build-host/Makefile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      746 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/build-host/README.rst
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 19:50:07.836652 python-project-structure-0.8.5b0/build-host/bin/
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2058 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/build-host/bin/entrypoint
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      731 2023-04-10 19:49:58.000000 python-project-structure-0.8.5b0/build-host/requirements-py310.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      674 2023-04-10 19:49:58.000000 python-project-structure-0.8.5b0/build-host/requirements-py311.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      948 2023-04-10 19:49:58.000000 python-project-structure-0.8.5b0/build-host/requirements-py37.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-10 19:49:58.000000 python-project-structure-0.8.5b0/build-host/requirements-py38.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-10 19:49:58.000000 python-project-structure-0.8.5b0/build-host/requirements-py39.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)        4 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/build-host/requirements.txt.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 19:50:07.836652 python-project-structure-0.8.5b0/dist/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      122 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/dist/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4400 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/docker-compose.override.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      651 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/docker-compose.yml
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 19:50:07.836652 python-project-structure-0.8.5b0/home/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       64 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/home/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      327 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/home/.pypirc.in
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2624 2023-04-10 19:49:57.000000 python-project-structure-0.8.5b0/pyproject.toml
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 19:50:07.837652 python-project-structure-0.8.5b0/requirements/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      578 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/requirements/build.txt.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 19:50:07.837652 python-project-structure-0.8.5b0/requirements/py310/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/requirements/py310/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4945 2023-04-10 19:49:58.000000 python-project-structure-0.8.5b0/requirements/py310/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-10 19:49:58.000000 python-project-structure-0.8.5b0/requirements/py310/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 19:50:07.838652 python-project-structure-0.8.5b0/requirements/py311/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/requirements/py311/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4696 2023-04-10 19:49:58.000000 python-project-structure-0.8.5b0/requirements/py311/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-10 19:49:58.000000 python-project-structure-0.8.5b0/requirements/py311/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 19:50:07.838652 python-project-structure-0.8.5b0/requirements/py37/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2645 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/requirements/py37/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5416 2023-04-10 19:49:58.000000 python-project-structure-0.8.5b0/requirements/py37/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      406 2023-04-10 19:49:58.000000 python-project-structure-0.8.5b0/requirements/py37/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 19:50:07.839652 python-project-structure-0.8.5b0/requirements/py38/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2515 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/requirements/py38/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4985 2023-04-10 19:49:58.000000 python-project-structure-0.8.5b0/requirements/py38/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-10 19:49:58.000000 python-project-structure-0.8.5b0/requirements/py38/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 19:50:07.839652 python-project-structure-0.8.5b0/requirements/py39/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2412 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/requirements/py39/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4972 2023-04-10 19:49:58.000000 python-project-structure-0.8.5b0/requirements/py39/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-10 19:49:58.000000 python-project-structure-0.8.5b0/requirements/py39/user.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1701 2023-04-10 19:50:07.843652 python-project-structure-0.8.5b0/setup.cfg
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 19:50:07.829651 python-project-structure-0.8.5b0/src/
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 19:50:07.841652 python-project-structure-0.8.5b0/src/python_project_structure.egg-info/
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-10 19:50:07.000000 python-project-structure-0.8.5b0/src/python_project_structure.egg-info/PKG-INFO
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)     1768 2023-04-10 19:50:07.000000 python-project-structure-0.8.5b0/src/python_project_structure.egg-info/SOURCES.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)        1 2023-04-10 19:50:07.000000 python-project-structure-0.8.5b0/src/python_project_structure.egg-info/dependency_links.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       73 2023-04-10 19:50:07.000000 python-project-structure-0.8.5b0/src/python_project_structure.egg-info/entry_points.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      146 2023-04-10 19:50:07.000000 python-project-structure-0.8.5b0/src/python_project_structure.egg-info/requires.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       23 2023-04-10 19:50:07.000000 python-project-structure-0.8.5b0/src/python_project_structure.egg-info/top_level.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 19:50:07.841652 python-project-structure-0.8.5b0/src/pythonprojectstructure/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4262 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/src/pythonprojectstructure/__init__.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      201 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/src/pythonprojectstructure/__main__.py
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 19:50:07.842652 python-project-structure-0.8.5b0/src/pythonprojectstructure/newsfragments/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       91 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/src/pythonprojectstructure/newsfragments/.gitignore
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 19:50:07.842652 python-project-structure-0.8.5b0/src/pythonprojectstructure/tests/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       72 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/src/pythonprojectstructure/tests/__init__.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4438 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/src/pythonprojectstructure/tests/test_cli.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      395 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/src/pythonprojectstructure/utils.py
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      162 2023-04-10 19:50:07.000000 python-project-structure-0.8.5b0/src/pythonprojectstructure/version.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3443 2023-04-10 19:48:11.000000 python-project-structure-0.8.5b0/tox.ini
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:13:59.883664 python-project-structure-0.8.5b1/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      543 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/.dir-locals.el.in
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/.dockerignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      687 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/.env.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:13:59.868663 python-project-structure-0.8.5b1/.github/
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:13:59.874663 python-project-structure-0.8.5b1/.github/workflows/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4593 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/.github/workflows/build-test.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4157 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/.gitlab-ci.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      779 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/.pre-commit-config.yaml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2377 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/.prospector.yaml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3931 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/CONTRIBUTING.rst
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2519 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/Dockerfile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2859 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/Dockerfile.devel
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1081 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/LICENSE
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    56729 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/Makefile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3198 2023-04-10 20:13:47.000000 python-project-structure-0.8.5b1/NEWS.rst
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-10 20:13:59.883664 python-project-structure-0.8.5b1/PKG-INFO
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    12157 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/README.rst
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2744 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/TODO.rst
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:13:59.875664 python-project-structure-0.8.5b1/bin/
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2792 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/bin/cz-check-bump
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      977 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/bin/entrypoint
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     1101 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/bin/get-base-version
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      321 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/bin/hadolint
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:13:59.877664 python-project-structure-0.8.5b1/build-host/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2092 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/build-host/Dockerfile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1438 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/build-host/Makefile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      746 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/build-host/README.rst
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:13:59.877664 python-project-structure-0.8.5b1/build-host/bin/
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2058 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/build-host/bin/entrypoint
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      731 2023-04-10 20:13:50.000000 python-project-structure-0.8.5b1/build-host/requirements-py310.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      674 2023-04-10 20:13:50.000000 python-project-structure-0.8.5b1/build-host/requirements-py311.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      948 2023-04-10 20:13:50.000000 python-project-structure-0.8.5b1/build-host/requirements-py37.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-10 20:13:50.000000 python-project-structure-0.8.5b1/build-host/requirements-py38.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-10 20:13:50.000000 python-project-structure-0.8.5b1/build-host/requirements-py39.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)        4 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/build-host/requirements.txt.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:13:59.877664 python-project-structure-0.8.5b1/dist/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      122 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/dist/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4400 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/docker-compose.override.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      651 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/docker-compose.yml
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:13:59.877664 python-project-structure-0.8.5b1/home/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       64 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/home/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      327 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/home/.pypirc.in
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2624 2023-04-10 20:13:49.000000 python-project-structure-0.8.5b1/pyproject.toml
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:13:59.877664 python-project-structure-0.8.5b1/requirements/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      578 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/requirements/build.txt.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:13:59.878664 python-project-structure-0.8.5b1/requirements/py310/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/requirements/py310/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4945 2023-04-10 20:13:50.000000 python-project-structure-0.8.5b1/requirements/py310/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-10 20:13:50.000000 python-project-structure-0.8.5b1/requirements/py310/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:13:59.879664 python-project-structure-0.8.5b1/requirements/py311/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/requirements/py311/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4696 2023-04-10 20:13:50.000000 python-project-structure-0.8.5b1/requirements/py311/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-10 20:13:50.000000 python-project-structure-0.8.5b1/requirements/py311/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:13:59.879664 python-project-structure-0.8.5b1/requirements/py37/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2645 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/requirements/py37/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5416 2023-04-10 20:13:50.000000 python-project-structure-0.8.5b1/requirements/py37/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      406 2023-04-10 20:13:50.000000 python-project-structure-0.8.5b1/requirements/py37/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:13:59.880664 python-project-structure-0.8.5b1/requirements/py38/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2515 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/requirements/py38/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4985 2023-04-10 20:13:50.000000 python-project-structure-0.8.5b1/requirements/py38/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-10 20:13:50.000000 python-project-structure-0.8.5b1/requirements/py38/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:13:59.880664 python-project-structure-0.8.5b1/requirements/py39/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2412 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/requirements/py39/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4972 2023-04-10 20:13:50.000000 python-project-structure-0.8.5b1/requirements/py39/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-10 20:13:50.000000 python-project-structure-0.8.5b1/requirements/py39/user.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1701 2023-04-10 20:13:59.884664 python-project-structure-0.8.5b1/setup.cfg
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:13:59.870663 python-project-structure-0.8.5b1/src/
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:13:59.881664 python-project-structure-0.8.5b1/src/python_project_structure.egg-info/
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-10 20:13:59.000000 python-project-structure-0.8.5b1/src/python_project_structure.egg-info/PKG-INFO
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)     1768 2023-04-10 20:13:59.000000 python-project-structure-0.8.5b1/src/python_project_structure.egg-info/SOURCES.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)        1 2023-04-10 20:13:59.000000 python-project-structure-0.8.5b1/src/python_project_structure.egg-info/dependency_links.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       73 2023-04-10 20:13:59.000000 python-project-structure-0.8.5b1/src/python_project_structure.egg-info/entry_points.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      146 2023-04-10 20:13:59.000000 python-project-structure-0.8.5b1/src/python_project_structure.egg-info/requires.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       23 2023-04-10 20:13:59.000000 python-project-structure-0.8.5b1/src/python_project_structure.egg-info/top_level.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:13:59.882664 python-project-structure-0.8.5b1/src/pythonprojectstructure/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4262 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/src/pythonprojectstructure/__init__.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      201 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/src/pythonprojectstructure/__main__.py
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:13:59.882664 python-project-structure-0.8.5b1/src/pythonprojectstructure/newsfragments/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       91 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/src/pythonprojectstructure/newsfragments/.gitignore
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:13:59.883664 python-project-structure-0.8.5b1/src/pythonprojectstructure/tests/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       72 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/src/pythonprojectstructure/tests/__init__.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4438 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/src/pythonprojectstructure/tests/test_cli.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      395 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/src/pythonprojectstructure/utils.py
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      162 2023-04-10 20:13:59.000000 python-project-structure-0.8.5b1/src/pythonprojectstructure/version.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3443 2023-04-10 20:12:00.000000 python-project-structure-0.8.5b1/tox.ini
```

### Comparing `python-project-structure-0.8.5b0/.dir-locals.el.in` & `python-project-structure-0.8.5b1/.dir-locals.el.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/.dockerignore` & `python-project-structure-0.8.5b1/.dockerignore`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/.env.in` & `python-project-structure-0.8.5b1/.env.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/.github/workflows/build-test.yml` & `python-project-structure-0.8.5b1/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/.gitignore` & `python-project-structure-0.8.5b1/.gitignore`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/.gitlab-ci.yml` & `python-project-structure-0.8.5b1/.gitlab-ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
   # https://docs.gitlab.com/ee/ci/yaml/#dependencies
   dependencies: []
   variables:
     DOCKER_BUILD_PULL: "true"
   rules:
     - if: >-
         $CI_COMMIT_TAG ||
-        $CI_COMMIT_MESSAGE =~ ".*\[ci skip\].*"
+        $CI_COMMIT_MESSAGE =~ "(?mi).*\[ci skip\].*"
       when: "never"
     - if: >-
         $CI_PROJECT_NAMESPACE == "rpatterson"
         && $CI_COMMIT_BRANCH != null
         && $CI_COMMIT_BRANCH =~ "^(develop|master)$"
         && $CI_PIPELINE_SOURCE != "schedule"
   script:
```

### Comparing `python-project-structure-0.8.5b0/.pre-commit-config.yaml` & `python-project-structure-0.8.5b1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/.prospector.yaml` & `python-project-structure-0.8.5b1/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/CONTRIBUTING.rst` & `python-project-structure-0.8.5b1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/Dockerfile` & `python-project-structure-0.8.5b1/Dockerfile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/Dockerfile.devel` & `python-project-structure-0.8.5b1/Dockerfile.devel`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/LICENSE` & `python-project-structure-0.8.5b1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/Makefile` & `python-project-structure-0.8.5b1/Makefile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/NEWS.rst` & `python-project-structure-0.8.5b1/NEWS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+python-project-structure 0.8.5b1 (2023-04-10)
+=============================================
+
+Bugfixes
+--------
+
+- Simulate a patch release. (simulate)
+
+
 python-project-structure 0.8.5b0 (2023-04-10)
 =============================================
 
 Bugfixes
 --------
 
 - Upgrade all requirements to the latest versions as of Mon Apr 10 06:25:02 PM UTC 2023. (upgrade-requirements)
```

### Comparing `python-project-structure-0.8.5b0/PKG-INFO` & `python-project-structure-0.8.5b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-project-structure
-Version: 0.8.5b0
+Version: 0.8.5b1
 Summary: Python project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/python-project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-project-structure-0.8.5b0/README.rst` & `python-project-structure-0.8.5b1/README.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/TODO.rst` & `python-project-structure-0.8.5b1/TODO.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/bin/cz-check-bump` & `python-project-structure-0.8.5b1/bin/cz-check-bump`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/bin/entrypoint` & `python-project-structure-0.8.5b1/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/bin/get-base-version` & `python-project-structure-0.8.5b1/bin/get-base-version`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/build-host/Dockerfile` & `python-project-structure-0.8.5b1/build-host/Dockerfile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/build-host/Makefile` & `python-project-structure-0.8.5b1/build-host/Makefile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/build-host/README.rst` & `python-project-structure-0.8.5b1/build-host/README.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/build-host/bin/entrypoint` & `python-project-structure-0.8.5b1/build-host/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/build-host/requirements-py310.txt` & `python-project-structure-0.8.5b1/build-host/requirements-py310.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/build-host/requirements-py311.txt` & `python-project-structure-0.8.5b1/build-host/requirements-py311.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/build-host/requirements-py37.txt` & `python-project-structure-0.8.5b1/build-host/requirements-py37.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/build-host/requirements-py38.txt` & `python-project-structure-0.8.5b1/build-host/requirements-py38.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/build-host/requirements-py39.txt` & `python-project-structure-0.8.5b1/build-host/requirements-py39.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/docker-compose.override.yml` & `python-project-structure-0.8.5b1/docker-compose.override.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/docker-compose.yml` & `python-project-structure-0.8.5b1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/pyproject.toml` & `python-project-structure-0.8.5b1/pyproject.toml`

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
-version = "0.8.5b0"
+version = "0.8.5b1"
 tag_format = "v$version"
 annotated_tag = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
 [ci skip]
 """
```

### Comparing `python-project-structure-0.8.5b0/requirements/build.txt.in` & `python-project-structure-0.8.5b1/requirements/build.txt.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/requirements/py310/build.txt` & `python-project-structure-0.8.5b1/requirements/py310/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/requirements/py310/devel.txt` & `python-project-structure-0.8.5b1/requirements/py310/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/requirements/py311/build.txt` & `python-project-structure-0.8.5b1/requirements/py311/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/requirements/py311/devel.txt` & `python-project-structure-0.8.5b1/requirements/py311/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/requirements/py37/build.txt` & `python-project-structure-0.8.5b1/requirements/py37/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/requirements/py37/devel.txt` & `python-project-structure-0.8.5b1/requirements/py37/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/requirements/py38/build.txt` & `python-project-structure-0.8.5b1/requirements/py38/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/requirements/py38/devel.txt` & `python-project-structure-0.8.5b1/requirements/py38/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/requirements/py39/build.txt` & `python-project-structure-0.8.5b1/requirements/py39/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/requirements/py39/devel.txt` & `python-project-structure-0.8.5b1/requirements/py39/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/setup.cfg` & `python-project-structure-0.8.5b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/src/python_project_structure.egg-info/PKG-INFO` & `python-project-structure-0.8.5b1/src/python_project_structure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-project-structure
-Version: 0.8.5b0
+Version: 0.8.5b1
 Summary: Python project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/python-project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-project-structure-0.8.5b0/src/python_project_structure.egg-info/SOURCES.txt` & `python-project-structure-0.8.5b1/src/python_project_structure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/src/pythonprojectstructure/__init__.py` & `python-project-structure-0.8.5b1/src/pythonprojectstructure/__init__.py`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/src/pythonprojectstructure/tests/test_cli.py` & `python-project-structure-0.8.5b1/src/pythonprojectstructure/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b0/tox.ini` & `python-project-structure-0.8.5b1/tox.ini`

 * *Files identical despite different names*

