# Comparing `tmp/python-project-structure-0.8.3.tar.gz` & `tmp/python-project-structure-0.8.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-project-structure-0.8.3.tar", last modified: Fri Dec  9 23:23:16 2022, max compression
+gzip compressed data, was "python-project-structure-0.8.4b0.tar", last modified: Sun Apr  9 23:42:31 2023, max compression
```

## Comparing `python-project-structure-0.8.3.tar` & `python-project-structure-0.8.4b0.tar`

### file list

```diff
@@ -1,49 +1,87 @@
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2022-12-09 23:23:16.116452 python-project-structure-0.8.3/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      324 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/.dir-locals.el.in
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1499 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/.dockerignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      447 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/.env.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2022-12-09 23:23:16.107452 python-project-structure-0.8.3/.github/
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2022-12-09 23:23:16.112452 python-project-structure-0.8.3/.github/workflows/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4364 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/.github/workflows/ci-cd.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1499 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2915 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/.gitlab-ci.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      555 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/.pre-commit-config.yaml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1822 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/Dockerfile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1029 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/Dockerfile.devel
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1081 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/LICENSE
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    21891 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/Makefile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5163 2022-12-09 23:21:24.000000 python-project-structure-0.8.3/NEWS.rst
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)     8282 2022-12-09 23:23:16.116452 python-project-structure-0.8.3/PKG-INFO
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     7474 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/README.rst
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1760 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/TODO.rst
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2022-12-09 23:23:16.113452 python-project-structure-0.8.3/bin/
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      936 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/bin/entrypoint
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2728 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/docker-compose.override.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      611 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/docker-compose.yml
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2022-12-09 23:23:16.113452 python-project-structure-0.8.3/home/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       65 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/home/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      327 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/home/.pypirc.in
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2043 2022-12-09 23:21:24.000000 python-project-structure-0.8.3/pyproject.toml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2961 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/requirements-build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      812 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/requirements-build.txt.in
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2914 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/requirements-devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      186 2022-12-09 23:21:25.000000 python-project-structure-0.8.3/requirements.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1429 2022-12-09 23:23:16.117452 python-project-structure-0.8.3/setup.cfg
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2022-12-09 23:23:16.107452 python-project-structure-0.8.3/src/
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2022-12-09 23:23:16.114452 python-project-structure-0.8.3/src/python_project_structure.egg-info/
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)     8282 2022-12-09 23:23:16.000000 python-project-structure-0.8.3/src/python_project_structure.egg-info/PKG-INFO
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      979 2022-12-09 23:23:16.000000 python-project-structure-0.8.3/src/python_project_structure.egg-info/SOURCES.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)        1 2022-12-09 23:23:16.000000 python-project-structure-0.8.3/src/python_project_structure.egg-info/dependency_links.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       73 2022-12-09 23:23:16.000000 python-project-structure-0.8.3/src/python_project_structure.egg-info/entry_points.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      105 2022-12-09 23:23:16.000000 python-project-structure-0.8.3/src/python_project_structure.egg-info/requires.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       23 2022-12-09 23:23:16.000000 python-project-structure-0.8.3/src/python_project_structure.egg-info/top_level.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2022-12-09 23:23:16.115452 python-project-structure-0.8.3/src/pythonprojectstructure/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3395 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/src/pythonprojectstructure/__init__.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      223 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/src/pythonprojectstructure/__main__.py
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2022-12-09 23:23:16.115452 python-project-structure-0.8.3/src/pythonprojectstructure/newsfragments/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       91 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/src/pythonprojectstructure/newsfragments/.gitignore
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2022-12-09 23:23:16.116452 python-project-structure-0.8.3/src/pythonprojectstructure/tests/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       72 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/src/pythonprojectstructure/tests/__init__.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3875 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/src/pythonprojectstructure/tests/test_cli.py
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      176 2022-12-09 23:23:16.000000 python-project-structure-0.8.3/src/pythonprojectstructure/version.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2036 2022-12-09 23:20:50.000000 python-project-structure-0.8.3/tox.ini
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.512361 python-project-structure-0.8.4b0/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      543 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/.dir-locals.el.in
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/.dockerignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      687 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/.env.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.497359 python-project-structure-0.8.4b0/.github/
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.503360 python-project-structure-0.8.4b0/.github/workflows/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4593 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/.github/workflows/build-test.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3704 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/.gitlab-ci.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      779 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/.pre-commit-config.yaml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2377 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/.prospector.yaml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3931 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/CONTRIBUTING.rst
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2519 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/Dockerfile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2859 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/Dockerfile.devel
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1081 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/LICENSE
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    56333 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/Makefile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2704 2023-04-09 23:42:20.000000 python-project-structure-0.8.4b0/NEWS.rst
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13177 2023-04-09 23:42:31.512361 python-project-structure-0.8.4b0/PKG-INFO
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    12114 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/README.rst
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2744 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/TODO.rst
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.504360 python-project-structure-0.8.4b0/bin/
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2792 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/bin/cz-check-bump
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      977 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/bin/entrypoint
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     1101 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/bin/get-base-version
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      321 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/bin/hadolint
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.506360 python-project-structure-0.8.4b0/build-host/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2092 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/build-host/Dockerfile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1438 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/build-host/Makefile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      746 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/build-host/README.rst
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.506360 python-project-structure-0.8.4b0/build-host/bin/
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2058 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/build-host/bin/entrypoint
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      731 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/build-host/requirements-py310.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      674 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/build-host/requirements-py311.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      948 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/build-host/requirements-py37.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/build-host/requirements-py38.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/build-host/requirements-py39.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)        4 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/build-host/requirements.txt.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.506360 python-project-structure-0.8.4b0/dist/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      122 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/dist/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4396 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/docker-compose.override.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      650 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/docker-compose.yml
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.506360 python-project-structure-0.8.4b0/home/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       64 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/home/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      327 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/home/.pypirc.in
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2624 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/pyproject.toml
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.507361 python-project-structure-0.8.4b0/requirements/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      578 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/requirements/build.txt.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.507361 python-project-structure-0.8.4b0/requirements/py310/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/requirements/py310/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4945 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/requirements/py310/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/requirements/py310/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.508361 python-project-structure-0.8.4b0/requirements/py311/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/requirements/py311/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4696 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/requirements/py311/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/requirements/py311/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.508361 python-project-structure-0.8.4b0/requirements/py37/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2645 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/requirements/py37/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5416 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/requirements/py37/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      406 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/requirements/py37/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.509361 python-project-structure-0.8.4b0/requirements/py38/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2515 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/requirements/py38/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4985 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/requirements/py38/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/requirements/py38/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.510361 python-project-structure-0.8.4b0/requirements/py39/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2412 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/requirements/py39/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4972 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/requirements/py39/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-09 23:42:22.000000 python-project-structure-0.8.4b0/requirements/py39/user.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1701 2023-04-09 23:42:31.513361 python-project-structure-0.8.4b0/setup.cfg
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.499360 python-project-structure-0.8.4b0/src/
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.511361 python-project-structure-0.8.4b0/src/python_project_structure.egg-info/
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13177 2023-04-09 23:42:31.000000 python-project-structure-0.8.4b0/src/python_project_structure.egg-info/PKG-INFO
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)     1768 2023-04-09 23:42:31.000000 python-project-structure-0.8.4b0/src/python_project_structure.egg-info/SOURCES.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)        1 2023-04-09 23:42:31.000000 python-project-structure-0.8.4b0/src/python_project_structure.egg-info/dependency_links.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       73 2023-04-09 23:42:31.000000 python-project-structure-0.8.4b0/src/python_project_structure.egg-info/entry_points.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      146 2023-04-09 23:42:31.000000 python-project-structure-0.8.4b0/src/python_project_structure.egg-info/requires.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       23 2023-04-09 23:42:31.000000 python-project-structure-0.8.4b0/src/python_project_structure.egg-info/top_level.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.512361 python-project-structure-0.8.4b0/src/pythonprojectstructure/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4262 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/src/pythonprojectstructure/__init__.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      201 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/src/pythonprojectstructure/__main__.py
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.512361 python-project-structure-0.8.4b0/src/pythonprojectstructure/newsfragments/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       91 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/src/pythonprojectstructure/newsfragments/.gitignore
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-09 23:42:31.512361 python-project-structure-0.8.4b0/src/pythonprojectstructure/tests/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       72 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/src/pythonprojectstructure/tests/__init__.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4438 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/src/pythonprojectstructure/tests/test_cli.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      395 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/src/pythonprojectstructure/utils.py
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      162 2023-04-09 23:42:31.000000 python-project-structure-0.8.4b0/src/pythonprojectstructure/version.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3443 2023-04-09 23:40:37.000000 python-project-structure-0.8.4b0/tox.ini
```

### Comparing `python-project-structure-0.8.3/.dockerignore` & `python-project-structure-0.8.4b0/.dockerignore`

 * *Files 8% similar despite different names*

```diff
@@ -17,24 +17,22 @@
 **/.so
 
 # Distribution / packaging
 .Python
 env/
 build/
 develop-eggs/
-dist/
 downloads/
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
 var/
-var-*/
 *.egg-info
 **/*.egg-info
 .installed.cfg
 *.egg
 **/.egg
 /src/*/version.py
 
@@ -50,15 +48,14 @@
 pip-log.txt
 pip-delete-this-directory.txt
 
 # Unit test / coverage reports
 htmlcov/
 .tox
 **/.tox
-.tox-*
 .coverage
 .coverage.*
 coverage.*
 .cache
 **/.cache
 nosetests.xml
 pytest-junit.xml
```

### Comparing `python-project-structure-0.8.3/.github/workflows/ci-cd.yml` & `python-project-structure-0.8.4b0/.github/workflows/build-test.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,120 +1,132 @@
-name: "CI/CD"
+name: "Build and Test"
+
+# TEMPLATE: If using GitHub Actions, then add the following secrets to the project:
+# - `CODECOV_TOKEN`:
+#   Add your project to https://app.codecov.io/gl and use the generated token
+# - `DOCKER_PASS`:
+#   A Docker Hub Personal Access Token
+# - `GPG_PASSPHRASE`:
+#   See the comments towards the bottom of the `./Makefile`
+# - `GPG_SIGNING_PRIVATE_KEY`:
+#   See the comments towards the bottom of the `./Makefile`
+# - `PROJECT_GITHUB_PAT`:
+#   A GitHub "Classic" Personal Access Token with scopes: `repo`, `workflow`,
+#   `packages`, and `project`
+# - `PYPI_PASSWORD`:
+#   A PyPI API token
+# - `TEST_PYPI_PASSWORD`:
+#   A PyPI API token
 
 on:
-  # Only run when branches are pushed, and not when tags are pushed, to allow manual
-  # creation of tags to manually control bumped versions:
+  # Only run on branches, not tags:
   # https://github.com/orgs/community/discussions/25615#discussioncomment-3397691
   push:
     branches:
       - "**"
     tags:
       - "!**"
+      # Also run for open pull requests, including when pushed to:
+  pull_request: {}
 
 jobs:
 
-  ci-cd:
+  build-test:
     runs-on: "ubuntu-latest"
+    container:
+      image: "ghcr.io/rpatterson/python-project-structure:build-host"
+      env:
+        PUID: "1001"
+        PGID: "123"
+        CHECKOUT_DIR: "${{ github.workspace }}"
+        # Requires the secrets to be added to GitHub either through the web UI or the
+        # GitHub CLI tool:
+        # https://docs.github.com/en/actions/security-guides/encrypted-secrets#creating-encrypted-secrets-for-a-repository
+        GPG_PASSPHRASE: "${{ secrets.GPG_PASSPHRASE }}"
+        GPG_SIGNING_PRIVATE_KEY: "${{ secrets.GPG_SIGNING_PRIVATE_KEY }}"
+        DOCKER_PASS: "${{ secrets.DOCKER_PASS }}"
+        # Enable the GitHub CLI
+        PROJECT_GITHUB_PAT: "${{ secrets.PROJECT_GITHUB_PAT }}"
+        # Tell the `./Makefile` about GitHub specific environment details:
+        CI_IS_FORK: >-
+          ${{
+            (
+              (
+                (github.repository_owner != 'rpatterson')
+                || (github.event.pull_request.head.repo.owner.login != 'rpatterson')
+              ) && 'true'
+            ) || 'false'
+          }}
+    permissions:
+      packages: "write"
+      checks: "write"
     strategy:
       matrix:
-        python-version: ["3.10"]
+        PYTHON_MINORS:
+          - "3.11"
+          - "3.10"
+          - "3.9"
+          - "3.8"
+          - "3.7"
+    name: "build-test (python${{ matrix.PYTHON_MINORS }})"
     steps:
 
-      # Global set up
-
+      # Shared/common set up:
       - name: "Checkout source from VCS"
         uses: "actions/checkout@master"
-      # https://github.com/actions/checkout/issues/701#issuecomment-1139627817
-      - name: "Fetch versions from VCS"
-        run: "git fetch --tags origin"
-
-      - name: "Add user installs to PATH"
-        run: |
-          echo "$HOME/.local/bin" >> $GITHUB_PATH
-
-      # Cache build artifacts to speed up CI runs
-
-      - name: "Cache tox virtual environments"
-        if: "github.ref != 'refs/heads/master'"
-        uses: "actions/cache@master"
-        env:
-          # Increment to force clearing the cache
-          cache-name: "tox-v1"
-        with:
-          path: |
-            ~/.local
-            ./.tox
-            ./.tox-*
-            ./var/log
-          # Never get a cache hit to force always caching any upgraded dependencies
-          # Use hashFiles to force venv recreation when dependencies change
-          key: >-
-            ${{ env.cache-name }}-${{ runner.os }}-${{ matrix.python-version }}-${{ hashFiles('pyproject.*') }}-${{ hashFiles('setup.*') }}-${{ hashFiles('tox.ini') }}-${{ github.sha }}
-          # Always re-use the cache and then upgrade
-          restore-keys: >-
-            ${{ env.cache-name }}-${{ runner.os }}-${{ matrix.python-version }}-${{ hashFiles('pyproject.*') }}-${{ hashFiles('setup.*') }}-${{ hashFiles('requirements*.txt') }}-${{ hashFiles('tox.ini') }}-
-
-      # Delegate the rest to the `./Makefile` to keep as much portable between CI
-      # platforms
-
-      - name: "Build the container image in which to run the tests"
-        env:
-          GPG_PASSPHRASE: "${{ secrets.GPG_PASSPHRASE }}"
-          GPG_SIGNING_PRIVATE_KEY: "${{ secrets.GPG_SIGNING_PRIVATE_KEY }}"
-          DOCKER_PASS: "${{ secrets.DOCKER_PASS }}"
-        run: "make -e build-bump build-docker"
-
-      - name: "Run the tests and code checks inside the built container"
-        run: "make test-docker"
+      # TODO: Debug stale venv issues and restore cache once fixed
+      - name: "Change checkout owner"
+        # https://stackoverflow.com/a/58474340/624787
+        run: >-
+          chown -R ${PUID}:${PGID} ./ &&
+          git config --global --add safe.directory
+          /__w/${{ github.event.repository.name }}/${{ github.event.repository.name }}
+
+      # Delegate steps agnostic of the CI/CD platform to the `./Makefile`:
+      - name: "Build image and run tests and checks in a container"
+        run: >-
+          entrypoint make -e PYTHON_MINORS=${{ matrix.PYTHON_MINORS }}
+          test-push build-docker-${{ matrix.PYTHON_MINORS }}
+          test-docker-${{ matrix.PYTHON_MINORS }} test-clean
 
-      # Upload build artifacts
+      # Upload build artifacts:
       # https://github.com/actions/upload-artifact#usage
-
       - name: "Archive test suite reports"
         uses: "actions/upload-artifact@master"
         with:
           name: "test-suite-reports"
           path: |
-            ./pytest*
+            ./build/*/pytest*
       # https://github.com/marketplace/actions/test-reporter#example
       - name: "Publish test suite report"
         uses: "dorny/test-reporter@main"
-        if: "success() || failure()"    # run this step even if previous step failed
+        # run this step even if previous step failed
+        if: >-
+          (success() || failure())
+          && (
+            (! github.event.pull_request)
+            || ! (
+              (github.repository_owner == 'rpatterson')
+              && (github.event.pull_request.head.repo.owner.login != 'rpatterson')
+            )
+          )
         with:
-          name: "PyTest Test Suite"
-          path: |
-            ./pytest-junit.xml
+          name: "PyTest Test Suite (python${{ matrix.PYTHON_MINORS }})"
+          path: >-
+            ./build/*/pytest-junit.xml,
+            ./build/*/prospector-xunit.xml
           reporter: "java-junit"
-
       - name: "Archive code coverage reports"
         uses: "actions/upload-artifact@master"
         with:
           name: "code-coverage-reports"
           path: |
-            ./coverage*
-            ./htmlcov
-
+            ./build/*/.coverage*
+            ./build/*/coverage*
+            ./build/*/htmlcov*
       - name: "Archive linter reports"
         uses: "actions/upload-artifact@master"
         with:
           name: "linter-reports"
           path: |
-            ./pylint*
-
-      # Release and publish
-
-      - name: "Bump version and publish release artifacts if on `master`/`develop`"
-        env:
-          CODECOV_TOKEN: "${{ secrets.CODECOV_TOKEN }}"
-          # Enable the GitHub CLI
-          GITHUB_TOKEN: "${{ secrets.GITHUB_TOKEN }}"
-          # Requires the secrets to be added to GitHub either through the web UI or the
-          # GitHub CLI tool:
-          # https://docs.github.com/en/actions/security-guides/encrypted-secrets#creating-encrypted-secrets-for-a-repository
-          GPG_PASSPHRASE: "${{ secrets.GPG_PASSPHRASE }}"
-          GPG_SIGNING_PRIVATE_KEY: "${{ secrets.GPG_SIGNING_PRIVATE_KEY }}"
-          PYPI_PASSWORD: "${{ secrets.PYPI_PASSWORD }}"
-          TEST_PYPI_PASSWORD: "${{ secrets.TEST_PYPI_PASSWORD }}"
-          DOCKER_PASS: "${{ secrets.DOCKER_PASS }}"
-        run: "make -e release"
-      # TODO: Push container image to GHCR? I don't currently need this but I can easily
-      #       imagine the value in it.
+            ./build/*/prospector*
+            ./build/*/pylint*
```

### Comparing `python-project-structure-0.8.3/.gitignore` & `python-project-structure-0.8.4b0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -17,24 +17,22 @@
 **/.so
 
 # Distribution / packaging
 .Python
 env/
 build/
 develop-eggs/
-dist/
 downloads/
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
 var/
-var-*/
 *.egg-info
 **/*.egg-info
 .installed.cfg
 *.egg
 **/.egg
 /src/*/version.py
 
@@ -50,15 +48,14 @@
 pip-log.txt
 pip-delete-this-directory.txt
 
 # Unit test / coverage reports
 htmlcov/
 .tox
 **/.tox
-.tox-*
 .coverage
 .coverage.*
 coverage.*
 .cache
 **/.cache
 nosetests.xml
 pytest-junit.xml
```

### Comparing `python-project-structure-0.8.3/Dockerfile` & `python-project-structure-0.8.4b0/build-host/Dockerfile`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,50 @@
-## Container image for use by end users
+## Container image in which to build, test, and release the project
 
-# Stay as close to a vanilla Python environment as possible
-FROM python:3
+# I *want* something to break to let me know if something changes in the latest version
+# of the base image changes something:
+# hadolint ignore=DL3007
+FROM docker:latest
 
-# Put the `ENTRYPOINT` on the `$PATH`
-RUN apt-get update && apt-get install -y gosu && rm -rf /var/lib/apt/lists/*
-COPY [ "./bin/entrypoint", "/usr/local/bin/entrypoint" ]
-
-WORKDIR "/usr/local/src/python-project-structure/"
-# Install dependencies with fixed versions in a separate layer to optimize build times
-# because this step takes the most time and changes the least frequently.
-COPY [ "./requirements.txt", "./" ]
-RUN pip install --no-cache-dir -r "./requirements.txt"
-# Install this package in the most common/standard Python way while still being able to
-# build the image locally.
-RUN --mount=source=./,target=./,rw,type=bind pip install --no-cache-dir "./"
+# Install the minimum OS packages needed to use the `./Makefile`.  Also install any OS
+# packages the `./Makefile` might install to optimize build times.
+# hadolint ignore=DL3018
+RUN \
+    apk add --no-cache \
+    "make" \
+    "bash" \
+    "su-exec" \
+    "git" \
+    "gettext" \
+    "py3-pip" \
+    "gnupg" \
+    "curl" \
+    "tar" \
+    "github-cli" \
+    && rm -rf /var/cache/apk/*
 
 # Find the same home directory even when run as another user, e.g. `root`.
-ENV HOME="/home/python-project-structure"
-WORKDIR "/home/python-project-structure/"
-ENTRYPOINT [ "entrypoint" ]
-CMD [ "python-project-structure" ]
+ENV HOME="/home/runner"
+# Add user installs to PATH
+ENV PATH="${HOME}/.local/bin:${PATH}"
+
+COPY [ "./requirements-py310.txt", "${HOME}/.local/lib/" ]
+RUN mkdir -pv "${HOME}/.local/var/log/" && \
+    pip install --no-cache-dir --user -r "${HOME}/.local/lib/requirements-py310.txt" \
+    >"${HOME}/.local/var/log/python-project-structure-host-install.log"
+
+COPY [ "./bin/entrypoint", "/usr/local/bin/entrypoint" ]
+ENTRYPOINT [ "docker-entrypoint.sh", "entrypoint" ]
+CMD [ "make", "-e", "build-docker" ]
 
 # https://github.com/opencontainers/image-spec/blob/main/annotations.md#pre-defined-annotation-keys
 LABEL org.opencontainers.image.url="https://gitlab.com/rpatterson/python-project-structure"
 LABEL org.opencontainers.image.documentation="https://gitlab.com/rpatterson/python-project-structure"
 LABEL org.opencontainers.image.source="https://gitlab.com/rpatterson/python-project-structure"
-LABEL org.opencontainers.image.title="python-project-structure"
-LABEL org.opencontainers.image.description="Python project structure foundation or template, CLI console scripts."
+LABEL org.opencontainers.image.title="Python Project Structure Build Host"
+LABEL org.opencontainers.image.description="Python project structure foundation or template, build host"
 LABEL org.opencontainers.image.licenses="MIT"
 LABEL org.opencontainers.image.authors="Ross Patterson <me@rpatterson.net>"
 LABEL org.opencontainers.image.vendor="rpatterson.net"
-LABEL org.opencontainers.image.base.name="hub.docker.com/_/python:3"
+LABEL org.opencontainers.image.base.name="docker.io/library/docker:latest"
+# Build-time `LABEL`s
+LABEL org.opencontainers.image.version=0.0.1
```

### Comparing `python-project-structure-0.8.3/LICENSE` & `python-project-structure-0.8.4b0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.3/bin/entrypoint` & `python-project-structure-0.8.4b0/bin/entrypoint`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 #!/bin/bash
 #
 # Perform any required volatile run-time initialization
 
 set -eu -o pipefail
 shopt -s inherit_errexit
-if [ ! -z "${DEBUG:=}" ]
+if [ "${DEBUG:=false}" = "true" ]
 then
     # Echo commands for easier debugging
-    PS4='$0:$LINENO+'
     set -x
+    PS4='$0:$LINENO+'
 fi
 
 
 main() {
-    if [ ! -z "${PUID}" ]
+    if [ -n "${PUID:-}" ]
     then
 	if (( $(id -u) != 0 ))
 	then
 	    set +x
 	    echo "ERROR: Can't create a user when not run as root" 1>&2
 	    false
 	fi
-	if ! id ${PUID}
+	if ! id "${PUID}" >"/dev/null" 2>&1
 	then
 	    # Add a user to the `passwd` DB so that the `~python-project-structure/`
 	    # HOME directory can be looked up.
 	    adduser --uid "${PUID}" --disabled-password --gecos \
-		    "Python Project Structure,,," "python-project-structure" 1>&2
+		    "Python Project Structure,,," "python-project-structure" \
+		    >"/dev/null"
 	fi
 	# Fix the TTY ownership if the session is interactive
 	if tty_dev=$(tty)
 	then
-	    chown -c "${PUID}" "${tty_dev}"
+	    chown "${PUID}" "${tty_dev}"
 	fi
 	# Delegate the rest to the `CMD`
 	exec gosu "${PUID}:${PGID:-${PUID}}" "${@}"
     fi
 
     # Delegate the rest to the `CMD`
     exec "$@"
 }
 
-
 main "$@"
```

### Comparing `python-project-structure-0.8.3/docker-compose.yml` & `python-project-structure-0.8.4b0/docker-compose.yml`

 * *Files 27% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 # running python-project-structure in containers.
 version: "3.8"
 
 services:
 
   ## Container for use by end users
   python-project-structure:
-    image: "merpatterson/python-project-structure:${VERSION:-latest}"
-    build: "./"
+    image: "merpatterson/python-project-structure"
+    container_name: "python-project-structure"
     environment:
+      TZ: "${TZ:-Etc/UTC}"
       # Make the run-time user configurable in `./.env` to match permissions inside and
       # outside the container.  Default to the common/standard main/first user and group
       # IDs
       PUID: "${PUID:-1000}"
       PGID: "${PGID:-${PUID:-1000}}"
     restart: "unless-stopped"
```

### Comparing `python-project-structure-0.8.3/pyproject.toml` & `python-project-structure-0.8.4b0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -12,33 +12,37 @@
 # local_scheme = "no-local-version"
 [tool.commitizen]
 # Parse commit messages according to conventional commits to decide wether the next
 # versin tag should be a major, minor or patch bump and create the VCS tag.  Also
 # provides VCS hooks to enforce that commit messages comply with conventional commits:
 # https://commitizen-tools.github.io/commitizen/
 name = "cz_conventional_commits"
-version = "0.8.3"
+# TEMPLATE: Update these versions to the latest version for your project and ensure the
+# tag exists both locally and on the project's remote:
+changelog_start_rev = "v0.0.0"
+version = "0.8.4b0"
 tag_format = "v$version"
 annotated_tag = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
-[actions skip]
+[ci skip]
 """
 [tool.towncrier]
 # https://towncrier.readthedocs.io/en/stable/#quick-start
 package = "pythonprojectstructure"
 package_dir = "src"
+name = "python-project-structure"
 
 [tool.pylint.MASTER]
-# Auto-detect the number of processors available to use from:
-#     $ pylint --generate-rcfile
-jobs = 0
+# Ensure `duplicate-code` and any other errors that depend on not runnining in parallel
+# are reported:
+jobs = 1
 enable-all-extensions = true
-output-format = "colorized,json:pylint.json"
+output-format = "colorized"
 ignore-paths = [
 # Managed by tools, best to use `# pylint: disable=...` inline comments for any other
 # ignores.
     "src/.+/version.py",
     ".*/src/.+/version.py",
 ]
 # Extend linting to usage of trusted extension packages
@@ -46,12 +50,23 @@
 [tool.pylint.TYPECHECK]
 # Ignore false negatives from external packages
 ignored-classes = ["lxml.etree.QName.localname"]
 # Match Black's defaults
 # https://black.readthedocs.io/en/stable/guides/using_black_with_other_tools.html#pylint
 [tool.pylint.format]
 max-line-length = "88"
+[tool.pylint."messages control"]
+# Workaround Prospector bug with PyLint:
+# https://github.com/PyCQA/prospector/issues/596#issue-1592499675
+disable = ["relative-beyond-top-level"]
+[[tool.mypy.overrides]]
+module = ["argcomplete"]
+ignore_missing_imports = true
+
+[tool.vulture]
+# https://github.com/jendrikseipp/vulture#ignoring-files
+exclude = ["src/pythonprojectstructure/version.py"]
 
 [tool.isort]
 # Match Black's defaults
 # https://black.readthedocs.io/en/stable/guides/using_black_with_other_tools.html#isort
 profile = "black"
```

### Comparing `python-project-structure-0.8.3/requirements-build.txt` & `python-project-structure-0.8.4b0/requirements/py310/build.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,154 +1,123 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=./requirements-build.txt --resolver=backtracking ./requirements-build.txt.in
+#    pip-compile --output-file=requirements/py310/build.txt --resolver=backtracking requirements/build.txt.in
 #
-argcomplete==2.0.0
+argcomplete==2.0.6
     # via commitizen
-bleach==5.0.1
+bleach==6.0.0
     # via readme-renderer
-build==0.9.0
-    # via pip-tools
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via cryptography
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==2.1.1
     # via
     #   commitizen
     #   requests
-click==8.1.3
-    # via
-    #   click-default-group
-    #   pip-tools
-    #   towncrier
-click-default-group==1.2.2
-    # via towncrier
 colorama==0.4.6
     # via commitizen
-commitizen==2.37.1
-    # via -r ./requirements-build.txt.in
-commonmark==0.9.1
-    # via rich
-cryptography==38.0.4
+commitizen==2.42.1
+    # via -r requirements/build.txt.in
+cryptography==40.0.1
     # via secretstorage
 decli==0.5.2
     # via commitizen
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via readme-renderer
-filelock==3.8.2
+filelock==3.11.0
     # via virtualenv
-identify==2.5.9
+identify==2.5.22
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==5.1.0
+importlib-metadata==6.2.1
     # via
     #   keyring
     #   twine
-incremental==22.10.0
-    # via towncrier
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
 jinja2==3.1.2
-    # via
-    #   commitizen
-    #   towncrier
-keyring==23.11.0
+    # via commitizen
+keyring==23.13.1
     # via twine
-markupsafe==2.1.1
+markdown-it-py==2.2.0
+    # via rich
+markupsafe==2.1.2
     # via jinja2
-more-itertools==9.0.0
+mdurl==0.1.2
+    # via markdown-it-py
+more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
-packaging==21.3
-    # via
-    #   build
-    #   commitizen
-pep517==0.13.0
-    # via build
-pip-tools==6.11.0
-    # via -r ./requirements-build.txt.in
-pkginfo==1.9.2
+packaging==23.0
+    # via commitizen
+pkginfo==1.9.6
     # via twine
-platformdirs==2.6.0
+platformdirs==3.2.0
     # via virtualenv
-pre-commit==2.20.0
-    # via -r ./requirements-build.txt.in
-prompt-toolkit==3.0.36
+pre-commit==3.2.2
+    # via -r requirements/build.txt.in
+prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
-pygments==2.13.0
+pygments==2.14.0
     # via
     #   readme-renderer
     #   rich
-pyparsing==3.0.9
-    # via packaging
 pyyaml==6.0
     # via
     #   commitizen
     #   pre-commit
 questionary==1.10.0
     # via commitizen
 readme-renderer==37.3
     # via twine
-requests==2.28.1
+requests==2.28.2
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==12.6.0
+rich==13.3.3
     # via twine
 secretstorage==3.3.3
     # via keyring
 six==1.16.0
     # via bleach
-termcolor==2.1.1
+termcolor==2.2.0
     # via commitizen
-toml==0.10.2
-    # via pre-commit
-tomli==2.0.1
-    # via
-    #   build
-    #   pep517
-    #   towncrier
-tomlkit==0.11.6
+tomlkit==0.11.7
     # via commitizen
-towncrier==22.8.0
-    # via -r ./requirements-build.txt.in
 twine==4.0.2
-    # via -r ./requirements-build.txt.in
-typing-extensions==4.4.0
+    # via -r requirements/build.txt.in
+typing-extensions==4.5.0
     # via commitizen
-urllib3==1.26.13
+urllib3==1.26.15
     # via
     #   requests
     #   twine
-virtualenv==20.17.1
+virtualenv==20.21.0
     # via pre-commit
-wcwidth==0.2.5
+wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
-wheel==0.38.4
-    # via pip-tools
-zipp==3.11.0
+zipp==3.15.0
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
-# pip
 # setuptools
```

### Comparing `python-project-structure-0.8.3/setup.cfg` & `python-project-structure-0.8.4b0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,69 @@
 [metadata]
 name = python-project-structure
 version = attr: src.pythonprojectstructure.version
 description = Python project structure foundation or template, CLI console scripts.
 url = https://gitlab.com/rpatterson/python-project-structure
 long_description = file: README.rst
 long_description_content_type = text/x-rst
+keywords = template, structure
 author = Ross Patterson
 author_email = me@rpatterson.net
 license = MIT
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Console
 	Intended Audience :: Developers
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.7
 	Topic :: Utilities
 
 [options]
 package_dir = 
 	=src
 packages = find:
+python_requires = >=3.7
+install_requires = 
+	argcomplete
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	python-project-structure = pythonprojectstructure:main
 
 [options.extras_require]
 devel = 
 	pytest
 	coverage
-	tox
-	pylint
-	flake8
+	prospector[with_everything]
+	xenon
 	rstcheck
-	flake8-black
+	black
 	autoflake
 	autopep8
+	pip-tools
 	setuptools_scm
+	towncrier
 	build
 
 [tool:pytest]
 testpaths = src/pythonprojectstructure
 
 [coverage:run]
-command_line = -m pytest --junit-xml=pytest-junit.xml -s
+command_line = -m pytest --junit-xml=pytest-junit.xml
 branch = True
 source = src
 
 [coverage:report]
 fail_under = 100
 show_missing = True
```

### Comparing `python-project-structure-0.8.3/src/pythonprojectstructure/__init__.py` & `python-project-structure-0.8.4b0/src/pythonprojectstructure/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,21 @@
+# PYTHON_ARGCOMPLETE_OK
 """
 Python project structure foundation or template, top-level package.
 """
 
-import os
+import sys
 import logging
 import argparse
-import pprint
+import json
+import pdb
+
+import argcomplete
+
+from . import utils
 
 logger = logging.getLogger(__name__)
 
 # Manage version through the VCS CI/CD process
 __version__ = None
 try:
     from . import version
@@ -19,69 +25,90 @@
     __version__ = version.version
 
 # Define command line options and arguments
 parser = argparse.ArgumentParser(
     description=__doc__.strip(),
     formatter_class=argparse.ArgumentDefaultsHelpFormatter,
 )
+parser.add_argument(
+    "--log-level",
+    default=argparse.SUPPRESS,
+    # I only wish the `logging` module provided public access to all defined levels
+    choices=logging._nameToLevel,  # pylint: disable=protected-access
+    help="Select logging verbosity. (default: INFO)",
+)
 # Define CLI sub-commands
 subparsers = parser.add_subparsers(
     dest="command",
     required=True,
     help="sub-command",
 )
 
 
+# TEMPLATE: Replace with the sub-commands and arguments your project provides.
 def foobar(quiet=False):
     """
     Run the foobar sub-command from the command line.
     """
     if not quiet:
         return ["foo", "bar"]
     return None
 
 
 parser_foobar = subparsers.add_parser(
     "foobar",
-    help=foobar.__doc__.strip(),
-    description=foobar.__doc__.strip(),
+    help=foobar.__doc__.strip(),  # type: ignore
+    description=foobar.__doc__.strip(),  # type: ignore
 )
 # Make the function for the sub-command specified in the CLI argument available in the
 # argument parser for delegation below.
 parser_foobar.set_defaults(command=foobar)
 parser_foobar.add_argument(
     "-q",
     "--quiet",
     action="store_true",
     help="Suppress reporting results",
 )
 
+# Register shell tab completion
+argcomplete.autocomplete(parser)
+
 
 def config_cli_logging(
-    root_level=logging.INFO, **kwargs
-):  # pylint: disable=unused-argument
+    root_level=logging.INFO,
+    log_level=parser.get_default("--log-level"),
+    **_,
+):
     """
-    Configure logging CLI usage first, but also appropriate for writing to log files.
+    Configure logging CLI usage as early as possible to affect all output.
     """
     # Want just our logger's level, not others', to be controlled by options/environment
     logging.basicConfig(level=root_level)
-    if "DEBUG" in os.environ and os.getenv("DEBUG").strip().lower() in {
-        "1",
-        "true",
-        "yes",
-        "on",
-    }:  # pragma: no cover
-        level = logging.DEBUG
-    else:
-        level = logging.INFO
-    logger.setLevel(level)
-    return level
+    # If the CLI option was not specified, fallback to the environment variable
+    if log_level is None:
+        log_level = "INFO"
+        if utils.DEBUG:  # pragma: no cover
+            log_level = "DEBUG"
+    logger.setLevel(getattr(logging, log_level.strip().upper()))
+    return log_level
 
 
 def main(args=None):  # pylint: disable=missing-function-docstring
+    try:
+        _main(args=args)
+    except Exception:  # pragma: no cover
+        if utils.POST_MORTEM:
+            pdb.post_mortem()
+        raise
+
+
+def _main(args=None):
+    """
+    Inner main CLI handler for outer exception handling.
+    """
     # Parse CLI options and positional arguments
     parsed_args = parser.parse_args(args=args)
     # Avoid noisy boilerplate, functions meant to handle CLI usage should accept kwargs
     # that match the defined option and argument names.
     cli_kwargs = dict(vars(parsed_args))
     # Remove any meta options and arguments, those used to direct option and argument
     # handling, that shouldn't be passed onto functions meant to handle CLI usage.  More
@@ -97,18 +124,19 @@
     for dest, value in list(shared_kwargs.items()):
         if dest not in prunerr_dests:  # pragma: no cover
             command_kwargs[dest] = value
             del shared_kwargs[dest]
 
     # Configure logging for CLI usage
     config_cli_logging(**shared_kwargs)
+    shared_kwargs.pop("log_level", None)
 
     # Delegate to the function for the sub-command CLI argument
-    logger.info("Running %r sub-command", parsed_args.command.__name__)
+    logger.debug("Running %r sub-command", parsed_args.command.__name__)
     # Sub-commands may return a result to be pretty printed, or handle output themselves
     # and return nothing.
     result = parsed_args.command(**command_kwargs)
     if result is not None:
-        pprint.pprint(result)
+        json.dump(result, sys.stdout, indent=2)
 
 
 main.__doc__ = __doc__
```

### Comparing `python-project-structure-0.8.3/src/pythonprojectstructure/tests/test_cli.py` & `python-project-structure-0.8.4b0/src/pythonprojectstructure/tests/test_cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Test the python-project-structure Command-Line Interface.
 """
 
 import sys
 import io
-import subprocess
+import runpy
+import subprocess  # nosec B404
 import contextlib
 import pathlib
 
 import unittest
 
 import pythonprojectstructure
 
@@ -18,46 +19,46 @@
     Test the python-project-structure Command-Line Interface.
     """
 
     def test_importable(self):
         """
         The Python package is on `sys.path` and thus importable.
         """
-        import_process = subprocess.run(
+        import_process = subprocess.run(  # nosec B603
             [sys.executable, "-c", "import pythonprojectstructure"],
             check=False,
         )
         self.assertEqual(
             import_process.returncode,
             0,
             "The Python package not importable",
         )
 
     def get_cli_error_messages(self, args):
         """
         Run the CLI script and return any error messages.
         """
         stderr_file = io.StringIO()
-        with self.assertRaises(SystemExit):
+        with self.assertRaises(SystemExit, msg="CLI didn't exit"):
             with contextlib.redirect_stderr(stderr_file):
                 pythonprojectstructure.main(args=args)
         return stderr_file.getvalue()
 
     def test_cli_help(self):
         """
         The command line script is self-docummenting.
         """
         stdout_file = io.StringIO()
-        with self.assertRaises(SystemExit):
+        with self.assertRaises(SystemExit, msg="CLI didn't exit"):
             with contextlib.redirect_stdout(stdout_file):
                 pythonprojectstructure.main(args=["--help"])
         stdout = stdout_file.getvalue()
         self.assertIn(
             pythonprojectstructure.__doc__.strip(),
-            stdout,
+            stdout.replace("\n", " "),
             "The console script name missing from --help output",
         )
 
     def test_cli_subcommand(self):
         """
         The command line supports sub-commands.
         """
@@ -67,55 +68,67 @@
         )
 
     def test_cli_options(self):
         """
         The command line script accepts options controlling behavior.
         """
         self.assertIsNone(
-            pythonprojectstructure.main(args=["foobar", "-q"]),
+            pythonprojectstructure.main(args=["--log-level", "DEBUG", "foobar", "-q"]),
             "Wrong console script options return value",
         )
 
     def test_cli_option_errors(self):
         """
         The command line script displays useful messages for invalid option values.
         """
         stderr = self.get_cli_error_messages(args=["foobar", "--non-existent-option"])
         self.assertIn(
             "error: unrecognized arguments: --non-existent-option",
             stderr,
             "Wrong invalid option message",
         )
 
-    def test_cli_module_main(self):
+    def test_cli_dash_m_option(self):
         """
-        The package/module supports execution via Python's `-m` option.
+        The package supports execution via Python's `-m` CLI option.
         """
-        module_main_process = subprocess.run(
+        module_main_process = subprocess.run(  # nosec B603
             [sys.executable, "-m", "pythonprojectstructure", "foobar"],
             check=False,
         )
         self.assertEqual(
             module_main_process.returncode,
             0,
             "Running via Python's `-m` option exited with non-zero status code",
         )
 
+    def test_cli_module_main(self):
+        """
+        The package supports execution via Python's `-m` option.
+        """
+        with self.assertRaises(SystemExit, msg="CLI didn't exit") as exc_context:
+            runpy.run_module("pythonprojectstructure")
+        self.assertEqual(
+            exc_context.exception.code,
+            2,
+            "Wrong `runpy` exit status code",
+        )
+
     def test_cli_exit_code(self):
         """
         The command line script exits with status code zero if there are no exceptions.
         """
         # Find the location of the `console_scripts` for this test environment
         prefix_path = pathlib.Path(sys.argv[0]).parent
         while not (prefix_path / "bin").is_dir():
             prefix_path = prefix_path.parent
-            if prefix_path.parent is prefix_path.parents[-1]:  # pragma: no cover
+            if prefix_path.parent is list(prefix_path.parents)[-1]:  # pragma: no cover
                 raise ValueError(f"Could not find script prefix path: {sys.argv[0]}")
 
-        script_process = subprocess.run(
+        script_process = subprocess.run(  # nosec B603
             [prefix_path / "bin" / "python-project-structure", "foobar"],
             check=False,
         )
         self.assertEqual(
             script_process.returncode,
             0,
             "Running the console script exited with non-zero status code",
```

