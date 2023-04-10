# Comparing `tmp/gwosc-0.6.1.tar.gz` & `tmp/gwosc-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwosc-0.6.1.tar", last modified: Thu Aug 12 20:54:03 2021, max compression
+gzip compressed data, was "gwosc-0.7.0.tar", last modified: Mon Apr 10 14:32:53 2023, max compression
```

## Comparing `gwosc-0.6.1.tar` & `gwosc-0.7.0.tar`

### file list

```diff
@@ -1,65 +1,67 @@
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2021-08-12 20:54:03.567932 gwosc-0.6.1/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      441 2021-05-12 10:53:16.000000 gwosc-0.6.1/.codeclimate.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)       55 2020-07-27 09:48:35.000000 gwosc-0.6.1/.codecov.yml
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2021-08-12 20:54:03.507933 gwosc-0.6.1/.github/
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2021-08-12 20:54:03.527933 gwosc-0.6.1/.github/workflows/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3136 2021-05-19 09:56:23.000000 gwosc-0.6.1/.github/workflows/build.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1332 2021-05-12 10:53:16.000000 gwosc-0.6.1/.github/workflows/docs.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1090 2021-05-12 10:53:16.000000 gwosc-0.6.1/.github/workflows/lint.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)    12287 2021-08-10 13:21:34.000000 gwosc-0.6.1/.github/workflows/packaging.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)      474 2021-05-12 10:53:16.000000 gwosc-0.6.1/.gitignore
--rw-r--r--   0 duncan    (1000) duncan    (1000)       44 2020-07-27 09:48:35.000000 gwosc-0.6.1/.pep8speaks.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1081 2020-07-27 09:48:35.000000 gwosc-0.6.1/LICENSE
--rw-r--r--   0 duncan    (1000) duncan    (1000)      112 2021-05-12 10:53:16.000000 gwosc-0.6.1/MANIFEST.in
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7133 2021-08-12 20:54:03.567932 gwosc-0.6.1/PKG-INFO
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4806 2021-05-12 10:53:16.000000 gwosc-0.6.1/README.md
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1274 2020-07-27 09:48:35.000000 gwosc-0.6.1/RELEASE.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2021-08-12 20:54:03.527933 gwosc-0.6.1/debian/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2790 2021-08-12 20:53:42.000000 gwosc-0.6.1/debian/changelog
--rw-r--r--   0 duncan    (1000) duncan    (1000)        2 2020-07-27 09:48:35.000000 gwosc-0.6.1/debian/compat
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1032 2021-05-12 10:53:16.000000 gwosc-0.6.1/debian/control
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1299 2020-07-27 09:48:35.000000 gwosc-0.6.1/debian/copyright
--rwxr-xr-x   0 duncan    (1000) duncan    (1000)      500 2021-05-12 10:53:16.000000 gwosc-0.6.1/debian/rules
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2021-08-12 20:54:03.527933 gwosc-0.6.1/debian/source/
--rw-r--r--   0 duncan    (1000) duncan    (1000)       12 2020-07-27 09:48:35.000000 gwosc-0.6.1/debian/source/format
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2021-08-12 20:54:03.537932 gwosc-0.6.1/docs/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      605 2021-08-10 13:21:34.000000 gwosc-0.6.1/docs/Makefile
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2021-08-12 20:54:03.537932 gwosc-0.6.1/docs/_static/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      463 2020-07-27 09:48:35.000000 gwosc-0.6.1/docs/_static/gwosc.css
--rw-r--r--   0 duncan    (1000) duncan    (1000)      169 2020-08-28 15:29:11.000000 gwosc-0.6.1/docs/api.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3786 2021-05-12 10:53:16.000000 gwosc-0.6.1/docs/conf.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      238 2020-07-27 09:48:35.000000 gwosc-0.6.1/docs/datasets.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)      533 2020-07-27 09:48:35.000000 gwosc-0.6.1/docs/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)      211 2020-07-27 09:48:35.000000 gwosc-0.6.1/docs/locate.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)      209 2020-07-27 09:48:35.000000 gwosc-0.6.1/docs/timeline.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2021-08-12 20:54:03.557932 gwosc-0.6.1/gwosc/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      371 2021-05-12 10:53:16.000000 gwosc-0.6.1/gwosc/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      142 2021-08-12 20:54:02.000000 gwosc-0.6.1/gwosc/_version.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     9651 2021-08-12 20:53:42.000000 gwosc-0.6.1/gwosc/api.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1817 2021-05-12 10:53:16.000000 gwosc-0.6.1/gwosc/catalog.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    15144 2021-08-10 13:21:34.000000 gwosc-0.6.1/gwosc/datasets.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7967 2021-08-10 13:21:34.000000 gwosc-0.6.1/gwosc/locate.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2021-08-12 20:54:03.567932 gwosc-0.6.1/gwosc/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      188 2021-05-12 10:53:16.000000 gwosc-0.6.1/gwosc/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1408 2021-05-12 10:53:16.000000 gwosc-0.6.1/gwosc/tests/conftest.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4742 2021-08-12 20:53:42.000000 gwosc-0.6.1/gwosc/tests/test_api.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1046 2021-05-12 10:53:16.000000 gwosc-0.6.1/gwosc/tests/test_catalog.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6257 2021-08-10 13:21:34.000000 gwosc-0.6.1/gwosc/tests/test_datasets.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2628 2021-05-12 10:53:16.000000 gwosc-0.6.1/gwosc/tests/test_locate.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1361 2021-05-12 10:53:16.000000 gwosc-0.6.1/gwosc/tests/test_timeline.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1646 2021-08-10 13:21:34.000000 gwosc-0.6.1/gwosc/tests/test_urls.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1371 2021-05-12 10:53:16.000000 gwosc-0.6.1/gwosc/tests/test_utils.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2429 2021-08-10 13:21:34.000000 gwosc-0.6.1/gwosc/timeline.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5236 2021-08-10 13:21:34.000000 gwosc-0.6.1/gwosc/urls.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2600 2021-05-12 10:53:16.000000 gwosc-0.6.1/gwosc/utils.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2021-08-12 20:54:03.557932 gwosc-0.6.1/gwosc.egg-info/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7133 2021-08-12 20:54:02.000000 gwosc-0.6.1/gwosc.egg-info/PKG-INFO
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1027 2021-08-12 20:54:02.000000 gwosc-0.6.1/gwosc.egg-info/SOURCES.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)        1 2021-08-12 20:54:02.000000 gwosc-0.6.1/gwosc.egg-info/dependency_links.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)      134 2021-08-12 20:54:02.000000 gwosc-0.6.1/gwosc.egg-info/requires.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)        6 2021-08-12 20:54:02.000000 gwosc-0.6.1/gwosc.egg-info/top_level.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3693 2021-08-12 20:53:42.000000 gwosc-0.6.1/gwosc.spec
--rw-r--r--   0 duncan    (1000) duncan    (1000)      409 2021-08-10 13:21:34.000000 gwosc-0.6.1/pyproject.toml
--rw-r--r--   0 duncan    (1000) duncan    (1000)       61 2020-07-27 09:48:35.000000 gwosc-0.6.1/readthedocs.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1699 2021-08-12 20:54:03.567932 gwosc-0.6.1/setup.cfg
--rwxr-xr-x   0 duncan    (1000) duncan    (1000)      192 2021-05-12 10:53:16.000000 gwosc-0.6.1/setup.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-10 14:32:52.995620 gwosc-0.7.0/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1054 2022-10-21 10:12:50.000000 gwosc-0.7.0/.appveyor.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      407 2022-10-21 10:12:50.000000 gwosc-0.7.0/.flake8
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      474 2022-05-16 13:55:13.000000 gwosc-0.7.0/.gitignore
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-10 14:32:52.945620 gwosc-0.7.0/.gitlab/
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-10 14:32:52.965620 gwosc-0.7.0/.gitlab/ci/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1105 2023-03-21 17:33:53.000000 gwosc-0.7.0/.gitlab/ci/analysis.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3605 2023-04-10 14:14:53.000000 gwosc-0.7.0/.gitlab/ci/debian.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      624 2022-10-21 10:12:50.000000 gwosc-0.7.0/.gitlab/ci/dist.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      729 2022-10-21 10:12:50.000000 gwosc-0.7.0/.gitlab/ci/docs.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1525 2023-04-10 13:21:39.000000 gwosc-0.7.0/.gitlab/ci/python.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3272 2022-10-21 10:12:50.000000 gwosc-0.7.0/.gitlab/ci/rhel.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1458 2022-10-21 10:12:50.000000 gwosc-0.7.0/.gitlab/ci/test.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      445 2022-10-21 10:12:50.000000 gwosc-0.7.0/.gitlab-ci.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       44 2020-07-27 09:48:35.000000 gwosc-0.7.0/.pep8speaks.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1081 2020-07-27 09:48:35.000000 gwosc-0.7.0/LICENSE
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      112 2022-05-16 13:55:13.000000 gwosc-0.7.0/MANIFEST.in
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5931 2023-04-10 14:32:52.995620 gwosc-0.7.0/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4580 2022-10-21 10:12:50.000000 gwosc-0.7.0/README.md
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4899 2023-01-09 14:57:56.000000 gwosc-0.7.0/RELEASE.md
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-10 14:32:52.975620 gwosc-0.7.0/debian/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2929 2023-04-10 14:14:53.000000 gwosc-0.7.0/debian/changelog
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        2 2020-07-27 09:48:35.000000 gwosc-0.7.0/debian/compat
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1040 2022-10-21 10:12:50.000000 gwosc-0.7.0/debian/control
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1299 2020-07-27 09:48:35.000000 gwosc-0.7.0/debian/copyright
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)      284 2022-10-21 10:12:50.000000 gwosc-0.7.0/debian/rules
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-10 14:32:52.975620 gwosc-0.7.0/debian/source/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       12 2020-07-27 09:48:35.000000 gwosc-0.7.0/debian/source/format
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-10 14:32:52.975620 gwosc-0.7.0/docs/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      605 2022-05-16 13:55:13.000000 gwosc-0.7.0/docs/Makefile
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-10 14:32:52.975620 gwosc-0.7.0/docs/_static/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      463 2020-07-27 09:48:35.000000 gwosc-0.7.0/docs/_static/gwosc.css
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      169 2021-10-13 10:04:46.000000 gwosc-0.7.0/docs/api.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3786 2022-05-16 13:55:13.000000 gwosc-0.7.0/docs/conf.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      238 2020-07-27 09:48:35.000000 gwosc-0.7.0/docs/datasets.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      533 2020-07-27 09:48:35.000000 gwosc-0.7.0/docs/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      211 2020-07-27 09:48:35.000000 gwosc-0.7.0/docs/locate.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      209 2020-07-27 09:48:35.000000 gwosc-0.7.0/docs/timeline.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-10 14:32:52.985620 gwosc-0.7.0/gwosc/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      371 2022-05-16 13:55:13.000000 gwosc-0.7.0/gwosc/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      160 2023-04-10 14:32:52.000000 gwosc-0.7.0/gwosc/_version.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    12698 2023-04-10 13:21:39.000000 gwosc-0.7.0/gwosc/api.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    16728 2023-03-21 17:33:53.000000 gwosc-0.7.0/gwosc/datasets.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7611 2023-01-09 14:57:42.000000 gwosc-0.7.0/gwosc/locate.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-10 14:32:52.995620 gwosc-0.7.0/gwosc/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      188 2022-05-16 13:55:13.000000 gwosc-0.7.0/gwosc/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1408 2022-05-16 13:55:13.000000 gwosc-0.7.0/gwosc/tests/conftest.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6498 2023-04-10 13:21:39.000000 gwosc-0.7.0/gwosc/tests/test_api.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7364 2023-03-21 17:33:53.000000 gwosc-0.7.0/gwosc/tests/test_datasets.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2403 2022-10-21 10:12:50.000000 gwosc-0.7.0/gwosc/tests/test_locate.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1361 2023-01-09 14:57:53.000000 gwosc-0.7.0/gwosc/tests/test_timeline.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1646 2022-05-16 13:55:13.000000 gwosc-0.7.0/gwosc/tests/test_urls.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1371 2022-05-16 13:55:13.000000 gwosc-0.7.0/gwosc/tests/test_utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2429 2023-01-09 14:57:53.000000 gwosc-0.7.0/gwosc/timeline.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5236 2022-05-16 13:55:13.000000 gwosc-0.7.0/gwosc/urls.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2600 2022-05-16 13:55:13.000000 gwosc-0.7.0/gwosc/utils.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-10 14:32:52.985620 gwosc-0.7.0/gwosc.egg-info/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5931 2023-04-10 14:32:52.000000 gwosc-0.7.0/gwosc.egg-info/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1022 2023-04-10 14:32:52.000000 gwosc-0.7.0/gwosc.egg-info/SOURCES.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        1 2023-04-10 14:32:52.000000 gwosc-0.7.0/gwosc.egg-info/dependency_links.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      171 2023-04-10 14:32:52.000000 gwosc-0.7.0/gwosc.egg-info/requires.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        6 2023-04-10 14:32:52.000000 gwosc-0.7.0/gwosc.egg-info/top_level.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3837 2023-04-10 14:14:53.000000 gwosc-0.7.0/gwosc.spec
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      626 2022-10-21 10:12:50.000000 gwosc-0.7.0/pyproject.toml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       61 2020-07-27 09:48:35.000000 gwosc-0.7.0/readthedocs.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1508 2023-04-10 14:32:52.995620 gwosc-0.7.0/setup.cfg
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)      192 2022-05-16 13:55:13.000000 gwosc-0.7.0/setup.py
```

### Comparing `gwosc-0.6.1/LICENSE` & `gwosc-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gwosc-0.6.1/PKG-INFO` & `gwosc-0.7.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,147 +1,20 @@
 Metadata-Version: 2.1
 Name: gwosc
-Version: 0.6.1
+Version: 0.7.0
 Summary: A python interface to the GW Open Science data archive
-Home-page: https://github.com/gwpy/gwosc/
+Home-page: https://git.ligo.org/gwosc/client/
+Download-URL: https://pypi.org/project/gwosc/
 Author: Duncan Macleod
 Author-email: duncan.macleod@ligo.org
 License: MIT
-Download-URL: https://pypi.org/project/gwosc/
-Project-URL: Bug Tracker, https://github.com/gwpy/gwosc/issues
-Project-URL: Discussion Forum, https://gwpy.slack.com
+Project-URL: Bug Tracker, https://git.ligo.org/gwosc/client/-/issues
+Project-URL: Discussion Forum, https://ask.igwn.org
 Project-URL: Documentation, https://gwosc.readthedocs.io
-Project-URL: Source Code, https://github.com/gwpy/gwosc.git
-Description: # `gwosc` client API
-        
-        The `gwosc` package provides an interface to querying the open data
-        releases hosted on <https://gw-openscience.org> from the GEO, LIGO,
-        and Virgo gravitational-wave observatories.
-        
-        ## Release status
-        
-        [![PyPI version](https://badge.fury.io/py/gwosc.svg)](http://badge.fury.io/py/gwosc)
-        [![Conda version](https://img.shields.io/conda/vn/conda-forge/gwosc.svg)](https://anaconda.org/conda-forge/gwosc/)  
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1196306.svg)](https://doi.org/10.5281/zenodo.1196306)
-        [![License](https://img.shields.io/pypi/l/gwosc.svg)](https://choosealicense.com/licenses/mit/)
-        ![Supported Python versions](https://img.shields.io/pypi/pyversions/gwosc.svg)
-        
-        ## Development status
-        
-        [![Build status](https://github.com/gwpy/gwosc/actions/workflows/build.yml/badge.svg)](https://github.com/gwpy/gwosc/actions/workflows/build.yml)
-        [![Codecov](https://codecov.io/gh/gwpy/gwosc/branch/main/graph/badge.svg?token=A0b4PysQYA)](https://codecov.io/gh/gwpy/gwosc)
-        [![Maintainability](https://api.codeclimate.com/v1/badges/234aad1c71f0642d3e60/maintainability)](https://codeclimate.com/github/gwpy/gwosc/maintainability)
-        [![Documentation](https://readthedocs.org/projects/gwosc/badge/?version=latest)](https://gwosc.readthedocs.io/en/latest/?badge=latest)
-        
-        ## Installation
-        
-        To install:
-        
-            conda install -c conda-forge gwosc
-        
-        or
-        
-            pip install gwosc
-        
-        ## Searching for datasets
-        
-        To search for available datasets (correct as of March 14 2018):
-        
-        ```python
-        >>> from gwosc import datasets
-        >>> datasets.find_datasets()
-        ['GW150914', 'GW151226', 'GW170104', 'GW170608', 'GW170814', 'GW170817', 'LVT151012', 'O1', 'S5', 'S6']
-        >>> datasets.find_datasets(detector='V1')
-        ['GW170814', 'GW170817']
-        >>> datasets.find_datasets(type='run')
-        ['O1', 'S5', 'S6']
-        ```
-        
-        To query for the GPS time of an event dataset (or vice-versa):
-        
-        ```python
-        >>> datasets.event_gps('GW170817')
-        1187008882.43
-        >>> datasets.event_at_gps(1187008882)
-        'GW170817'
-        ```
-        
-        Similar queries are available for observing run datasets:
-        
-        ```python
-        >>> datasets.run_segment('O1')
-        (1126051217, 1137254417)
-        >>> datasets.run_at_gps(1135136350)  # event_gps('GW151226')
-        'O1'
-        ```
-        
-        ## Locating data URLs by event name
-        
-        You can search for remote data URLS based on the event name:
-        
-        ```python
-        >>> from gwosc.locate import get_event_urls
-        >>> get_event_urls('GW150914')
-        ['https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/H-H1_GWOSC_4KHZ_R1-1126259447-32.hdf5', 'https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/H-H1_GWOSC_4KHZ_R1-1126257415-4096.hdf5', 'https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126259447-32.hdf5', 'https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126257415-4096.hdf5']
-        ```
-        
-        You can down-select the URLs using keyword arguments:
-        
-        ```python
-        >>> get_event_urls('GW150914', detector='L1', duration=32)
-        ['https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126259447-32.hdf5']
-        ```
-        
-        ## Locating data URLs by GPS interval
-        
-        You can search for remote data URLs based on the GPS time interval as
-        follows:
-        
-        ```python
-        >>> from gwosc.locate import get_urls
-        >>> get_urls('L1', 968650000, 968660000)
-        ['https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968646656-4096.hdf5', 'https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968650752-4096.hdf5', 'https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968654848-4096.hdf5', 'https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968658944-4096.hdf5']
-        ```
-        
-        This arguments for this function are as follows
-        
-        -   `detector` : the prefix of the relevant gravitational-wave
-            interferometer, either `'H1'` for LIGO-Hanford, or `'L1'` for LIGO
-            Livingston,
-        -   `start`: the GPS start time of the interval of interest
-        -   `end`: the GPS end time of the interval of interest
-        
-        By default, this method will return the paths to HDF5 files for the 4
-        kHz sample-rate data, these can be specified as keyword arguments. For
-        full information, run
-        
-        ```python
-        >>> help(get_urls)
-        ```
-        
-        ## Query for Timeline segments
-        
-        You can also search for Timeline segments, based on a flag name, and a
-        GPS time interval as follows:
-        
-        ```python
-        >>> from gwosc.timeline import get_segments
-        >>> get_segments('H1_DATA', 1126051217, 1126151217)
-        [(1126073529, 1126114861), (1126121462, 1126123267), (1126123553, 1126126832), (1126139205, 1126139266), (1126149058, 1126151217)]
-        ```
-        
-        The output is a `list` of `(start, end)` 2-tuples which each represent a
-        semi-open time interval.
-        
-        For documentation on what flags are available, for example for the O1
-        science run, see [the O1 data release page](https://gw-openscience.org/O1/)
-        (*Data Quality*).
-        
-        
-Platform: UNKNOWN
+Project-URL: Source Code, https://git.ligo.org/gwosc/client.git
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -152,7 +25,134 @@
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
+Provides-Extra: lint
+License-File: LICENSE
+
+# `gwosc` client API
+
+The `gwosc` package provides an interface to querying the open data
+releases hosted on <https://gw-openscience.org> from the GEO, LIGO,
+and Virgo gravitational-wave observatories.
+
+## Release status
+
+[![PyPI version](https://badge.fury.io/py/gwosc.svg)](http://badge.fury.io/py/gwosc)
+[![Conda version](https://img.shields.io/conda/vn/conda-forge/gwosc.svg)](https://anaconda.org/conda-forge/gwosc/)  
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1196306.svg)](https://doi.org/10.5281/zenodo.1196306)
+[![License](https://img.shields.io/pypi/l/gwosc.svg)](https://choosealicense.com/licenses/mit/)
+![Supported Python versions](https://img.shields.io/pypi/pyversions/gwosc.svg)
+
+## Development status
+
+[![Build status](https://git.ligo.org/gwosc/client/badges/main/pipeline.svg)](https://git.ligo.org/gwosc/client/-/pipelines)
+![Code coverage](https://git.ligo.org/gwosc/client/badges/main/coverage.svg)
+[![Documentation](https://readthedocs.org/projects/gwosc/badge/?version=latest)](https://gwosc.readthedocs.io/en/latest/?badge=latest)
+
+## Installation
+
+To install:
+
+    conda install -c conda-forge gwosc
+
+or
+
+    pip install gwosc
+
+## Searching for datasets
+
+To search for available datasets (correct as of March 14 2018):
+
+```python
+>>> from gwosc import datasets
+>>> datasets.find_datasets()
+['GW150914', 'GW151226', 'GW170104', 'GW170608', 'GW170814', 'GW170817', 'LVT151012', 'O1', 'S5', 'S6']
+>>> datasets.find_datasets(detector='V1')
+['GW170814', 'GW170817']
+>>> datasets.find_datasets(type='run')
+['O1', 'S5', 'S6']
+```
+
+To query for the GPS time of an event dataset (or vice-versa):
+
+```python
+>>> datasets.event_gps('GW170817')
+1187008882.43
+>>> datasets.event_at_gps(1187008882)
+'GW170817'
+```
+
+Similar queries are available for observing run datasets:
+
+```python
+>>> datasets.run_segment('O1')
+(1126051217, 1137254417)
+>>> datasets.run_at_gps(1135136350)  # event_gps('GW151226')
+'O1'
+```
+
+## Locating data URLs by event name
+
+You can search for remote data URLS based on the event name:
+
+```python
+>>> from gwosc.locate import get_event_urls
+>>> get_event_urls('GW150914')
+['https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/H-H1_GWOSC_4KHZ_R1-1126259447-32.hdf5', 'https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/H-H1_GWOSC_4KHZ_R1-1126257415-4096.hdf5', 'https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126259447-32.hdf5', 'https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126257415-4096.hdf5']
+```
+
+You can down-select the URLs using keyword arguments:
+
+```python
+>>> get_event_urls('GW150914', detector='L1', duration=32)
+['https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126259447-32.hdf5']
+```
+
+## Locating data URLs by GPS interval
+
+You can search for remote data URLs based on the GPS time interval as
+follows:
+
+```python
+>>> from gwosc.locate import get_urls
+>>> get_urls('L1', 968650000, 968660000)
+['https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968646656-4096.hdf5', 'https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968650752-4096.hdf5', 'https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968654848-4096.hdf5', 'https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968658944-4096.hdf5']
+```
+
+This arguments for this function are as follows
+
+-   `detector` : the prefix of the relevant gravitational-wave
+    interferometer, either `'H1'` for LIGO-Hanford, or `'L1'` for LIGO
+    Livingston,
+-   `start`: the GPS start time of the interval of interest
+-   `end`: the GPS end time of the interval of interest
+
+By default, this method will return the paths to HDF5 files for the 4
+kHz sample-rate data, these can be specified as keyword arguments. For
+full information, run
+
+```python
+>>> help(get_urls)
+```
+
+## Query for Timeline segments
+
+You can also search for Timeline segments, based on a flag name, and a
+GPS time interval as follows:
+
+```python
+>>> from gwosc.timeline import get_segments
+>>> get_segments('H1_DATA', 1126051217, 1126151217)
+[(1126073529, 1126114861), (1126121462, 1126123267), (1126123553, 1126126832), (1126139205, 1126139266), (1126149058, 1126151217)]
+```
+
+The output is a `list` of `(start, end)` 2-tuples which each represent a
+semi-open time interval.
+
+For documentation on what flags are available, for example for the O1
+science run, see [the O1 data release page](https://gw-openscience.org/O1/)
+(*Data Quality*).
+
```

### Comparing `gwosc-0.6.1/README.md` & `gwosc-0.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 [![Conda version](https://img.shields.io/conda/vn/conda-forge/gwosc.svg)](https://anaconda.org/conda-forge/gwosc/)  
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1196306.svg)](https://doi.org/10.5281/zenodo.1196306)
 [![License](https://img.shields.io/pypi/l/gwosc.svg)](https://choosealicense.com/licenses/mit/)
 ![Supported Python versions](https://img.shields.io/pypi/pyversions/gwosc.svg)
 
 ## Development status
 
-[![Build status](https://github.com/gwpy/gwosc/actions/workflows/build.yml/badge.svg)](https://github.com/gwpy/gwosc/actions/workflows/build.yml)
-[![Codecov](https://codecov.io/gh/gwpy/gwosc/branch/main/graph/badge.svg?token=A0b4PysQYA)](https://codecov.io/gh/gwpy/gwosc)
-[![Maintainability](https://api.codeclimate.com/v1/badges/234aad1c71f0642d3e60/maintainability)](https://codeclimate.com/github/gwpy/gwosc/maintainability)
+[![Build status](https://git.ligo.org/gwosc/client/badges/main/pipeline.svg)](https://git.ligo.org/gwosc/client/-/pipelines)
+![Code coverage](https://git.ligo.org/gwosc/client/badges/main/coverage.svg)
 [![Documentation](https://readthedocs.org/projects/gwosc/badge/?version=latest)](https://gwosc.readthedocs.io/en/latest/?badge=latest)
 
 ## Installation
 
 To install:
 
     conda install -c conda-forge gwosc
```

### Comparing `gwosc-0.6.1/debian/changelog` & `gwosc-0.7.0/debian/changelog`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+gwosc (0.7.0-1) unstable; urgency=low
+
+  * update to 0.7.0
+
+ -- Duncan Macleod <duncan.macleod@ligo.org>  Mon, 10 Apr 2023 14:23:00 +0100
+
 gwosc (0.6.1-1) unstable; urgency=low
 
   * update to 0.6.1
 
  -- Duncan Macleod <duncan.macleod@ligo.org>  Thu, 12 Aug 2021 21:37:00 +0100
 
 gwosc (0.6.0-1) unstable; urgency=low
```

### Comparing `gwosc-0.6.1/debian/control` & `gwosc-0.7.0/debian/control`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -- gwosc source package ------------------------------------------------------
 
 Source: gwosc
 Homepage: https://gwosc.readthedocs.io
-Vcs-Browser: https://github.com/gwpy/gwosc
-Vcs-Git: https://github.com/gwpy/gwosc.git
+Vcs-Browser: https://git.ligo.org/gwosc/client
+Vcs-Git: https://git.ligo.org/gwosc/client.git
 Maintainer: Duncan Macleod <duncan.macleod@ligo.org>
 Section: python
 Priority: optional
 Standards-Version: 3.9.1
 X-Python3-Version: >= 3.5
 Build-Depends:
   debhelper (>= 9),
```

### Comparing `gwosc-0.6.1/debian/copyright` & `gwosc-0.7.0/debian/copyright`

 * *Files identical despite different names*

### Comparing `gwosc-0.6.1/docs/Makefile` & `gwosc-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gwosc-0.6.1/docs/conf.py` & `gwosc-0.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gwosc-0.6.1/docs/index.rst` & `gwosc-0.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gwosc-0.6.1/gwosc/datasets.py` & `gwosc-0.7.0/gwosc/datasets.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 
 Similar queries are available for observing run datasets:
 
 >>> datasets.run_segment('O1')
 (1126051217, 1137254417)
 >>> datasets.run_at_gps(1135136350)  # event_gps('GW151226')
 'O1'
+
+To run an event query filtered by merger parameters:
+
+>>> from gwosc.datasets import query_events
+>>> query_events(select=["mass-1-source <= 3.0"])
+['GW170817-v3', 'GW190425-v1', 'GW190425-v2', 'GW190425_081805-v3']
 """  # noqa: E501
 
 import re
 import warnings
 
 from . import (
     api,
@@ -586,7 +592,65 @@
     """
     for type_ in ("run", "catalog", "event"):
         if dataset in find_datasets(type=type_, host=host):
             return type_
     raise ValueError(
         "failed to determine type for dataset {0!r}".format(dataset),
     )
+
+
+def query_events(select, host=api.DEFAULT_URL):
+    """Return a list of events filtered by the parameters in `select`
+
+    Parameters
+    ----------
+    select : `list` of `str`
+        A list of strings where each element is a range constrain on the
+        event parameters.
+        All ranges should have inclusive ends (<= and => operators).
+
+    host : `str`, optional
+        the URL of the GWOSC host to query
+
+    Examples
+    --------
+    >>> from gwosc.datasets import query_events
+    >>> query_events(
+    ...     select=[
+    ...         "mass-1-source >= 1.4",
+    ...         "200 >= luminosity-distance >= 100",
+    ...     ]
+    ... )
+    ['GW190425-v1', 'GW190425-v2', 'GW190425_081805-v3']
+
+    Notes
+    -----
+    Operators:
+
+    - `<=` (or `=<`)
+    - `=>` (or `>=`)
+
+    Parameters:
+
+    - ``gps-time`,
+    - ``mass-1-source``,
+    - ``mass-2-source``,
+    - ``network-matched-filter-snr``,
+    - ``luminosity-distance``,
+    - ``chi-eff``,
+    - ``total-mass-source``,
+    - ``chirp-mass``,
+    - ``chirp-mass-source``,
+    - ``redshift``,
+    - ``far``,
+    - ``p-astro``,
+    - ``final-mass-source``
+
+    For a full description of all parameters see
+    https://www.gwosc.org/apidocs/#event5
+    """
+    return list(
+        api.fetch_filtered_events_json(
+            select=select,
+            host=host,
+        )["events"].keys()
+    )
```

### Comparing `gwosc-0.6.1/gwosc/locate.py` & `gwosc-0.7.0/gwosc/locate.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,31 +31,28 @@
  'https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968658944-4096.hdf5']
 
 By default, this method will return the paths to HDF5 files for the 4 kHz
 sample-rate data, these can be specified as keyword arguments.
 For full information, see :func:`get_urls`.
 """  # noqa: E501
 
-import warnings
-
 from . import (
     api,
     datasets,
     urls as lurls,
     utils,
 )
 
 __all__ = ['get_urls', 'get_run_urls', 'get_event_urls']
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 
 
 def get_urls(
         detector, start, end,
         dataset=None,
-        tag=None,
         version=None,
         sample_rate=4096,
         format='hdf5',
         host=api.DEFAULT_URL,
 ):
     """Fetch the URLs from GWOSC regarding a given GPS interval
 
@@ -90,23 +87,14 @@
     urls : `list` of `str`
         the list of remote file URLs that contain data matching the
         relevant parameters
     """
     start = int(start)
     end = int(end)
 
-    if tag is not None:
-        warnings.warn(
-            "the `tag` keyword to get_urls is deprecated, GWOSC no longer "
-            "releases multiple datasets for events, please use the `dataset` "
-            "and `version` keyword arguments to manually select the host "
-            "dataset for URLs",
-            DeprecationWarning,
-        )
-
     for dstype in ("event", "run"):
         dsets = datasets._iter_datasets(
             match=dataset,
             type=dstype,
             detector=detector,
             segment=(start, end),
             version=version,
@@ -130,14 +118,15 @@
                     dst,
                     detector=detector,
                     start=start,
                     end=end,
                     format=format,
                     sample_rate=sample_rate,
                     version=version,
+                    host=host,
                 )
 
             # if full span covered, return now
             if utils.full_coverage(urls, (start, end)):
                 return urls
 
     raise ValueError("Cannot find a GWOSC dataset for %s covering [%d, %d)"
```

### Comparing `gwosc-0.6.1/gwosc/tests/conftest.py` & `gwosc-0.7.0/gwosc/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gwosc-0.6.1/gwosc/tests/test_api.py` & `gwosc-0.7.0/gwosc/tests/test_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,42 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) Cardiff University (2018-2021)
 # SPDX-License-Identifier: MIT
 
 """Tests for :mod:`gwosc.api`
 """
 
-import os.path
 from unittest import mock
 
+from requests import RequestException
+
 import pytest
 
 from .. import api
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 
 
+_ALLOWED_PARAMS = [
+    "gps-time",
+    "mass-1-source",
+    "mass-2-source",
+    "network-matched-filter-snr",
+    "luminosity-distance",
+    "chi-eff",
+    "total-mass-source",
+    "chirp-mass",
+    "chirp-mass-source",
+    "redshift",
+    "far",
+    "p-astro",
+    "final-mass-source",
+]
+
+
 def losc_url(path):
     return '{0}/{1}'.format(api.DEFAULT_URL, path)
 
 
 def check_json_url_list(urllist, keys={'detector', 'format', 'url'}):
     assert isinstance(urllist, list)
     for urld in urllist:
@@ -29,22 +47,23 @@
 @pytest.mark.remote
 def test_fetch_json():
     url = 'https://www.gw-openscience.org/archive/1126257414/1126261510/json/'
     out = api.fetch_json(url)
     assert isinstance(out, dict)
     assert len(out['events']) == 3
     assert sorted(out['events']['GW150914-v1']['detectors']) == ['H1', 'L1']
-    assert {'tenyear', 'O1', 'O1_16KHZ', 'history'}.issubset(set(out['runs']))
+    assert {'O1', 'O1_16KHZ', 'history'}.issubset(set(out['runs']))
+
 
+@pytest.mark.remote
+def test_fetch_json_error():
     # check errors (use legit URL that isn't JSON)
-    url2 = os.path.dirname(os.path.dirname(url))
-    with pytest.raises(ValueError) as exc:
-        api.fetch_json(url2)
-    assert str(exc.value).startswith(
-        "Failed to parse GWOSC JSON from {!r}: ".format(url2))
+    url = 'https://www.gw-openscience.org/archive/1126257414/1126261510/'
+    with pytest.raises((RequestException, ValueError)):
+        api.fetch_json(url)
 
 
 def test_fetch_json_local(requests_mock):
     url = 'http://anything'
     requests_mock.get(
         url,
         json={"key": "value"},
@@ -56,15 +75,15 @@
 
 @pytest.mark.remote
 def test_fetch_dataset_json():
     start = 934000000
     end = 934100000
     out = api.fetch_dataset_json(start, end)
     assert not out['events']
-    assert {"tenyear", "S6", "history"}.issubset(set(out['runs']))
+    assert {"S6", "history"}.issubset(set(out['runs']))
 
 
 @mock.patch('gwosc.api.fetch_json')
 def test_fetch_dataset_json_local(fetch):
     start = 934000000
     end = 934100000
     api.fetch_dataset_json(start, end)
@@ -119,14 +138,64 @@
     api.fetch_catalog_json("GWTC-1-confident")
     fetch.assert_called_with(
         losc_url("eventapi/json/GWTC-1-confident/")
     )
 
 
 @pytest.mark.remote
+def test_fetch_filtered_events_json():
+    out = api.fetch_filtered_events_json(
+        select=["10 <= luminosity-distance <= 200"]
+    )
+    events = out["events"]
+    assert "GW190425-v1" in events
+
+
+@mock.patch(
+    'gwosc.api.fetch_allowed_params_json',
+    mock.MagicMock(return_value=_ALLOWED_PARAMS),
+)
+@mock.patch("gwosc.api.fetch_json")
+@pytest.mark.parametrize("select", [
+    "10 <= luminosity-distance <= 200",
+    "10 =< luminosity-distance <= 200",
+    "200 >= luminosity-distance >= 10",
+    "10 <=  luminosity-distance   =< 200",
+    "10<=luminosity-distance<=200",
+    "  200 >=  luminosity-distance => 10   ",
+    " 200 =>luminosity-distance=>10",
+])
+def test_fetch_filtered_events_json_local(fetch, select):
+    api.fetch_filtered_events_json(select=[select])
+    (called_url,), kwargs = fetch.call_args
+    assert "max-luminosity-distance=200" in called_url
+    assert "min-luminosity-distance=10" in called_url
+
+
+@mock.patch(
+    'gwosc.api.fetch_allowed_params_json',
+    mock.MagicMock(return_value=_ALLOWED_PARAMS),
+)
+@mock.patch("gwosc.api.fetch_json")
+@pytest.mark.parametrize("select", [
+    "100 <= luminosity-distance",
+    "gps-time < 100",
+    "gps-time  = > 100",
+    "unknown-param <= 100",
+    "c0mpl3telyR4nd-m",
+])
+def test_fetch_filtered_events_json_bad_local(fetch, select):
+    with pytest.raises(
+        ValueError,
+        match="Could not parse"
+    ):
+        api.fetch_filtered_events_json(select=[select])
+
+
+@pytest.mark.remote
 def test_fetch_event_json():
     out = api.fetch_event_json("GW150914")
     meta = out["events"]["GW150914-v3"]
     assert int(meta["GPS"]) == 1126259462
     assert meta["version"] == 3
```

### Comparing `gwosc-0.6.1/gwosc/tests/test_datasets.py` & `gwosc-0.7.0/gwosc/tests/test_datasets.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,14 +33,33 @@
                 'OperatingIFOs': "H1 L1",
                 'H1': {},
                 'L1': {},
             },
         },
     }
 }
+EVENT_JSON = {
+    'events': {
+        'mock-event-1': {
+            'GPS': 1240215503.0,
+            'luminosity_distance': 159.0,
+            'mass_1_source': 1.74,
+        },
+        'mock-event-2': {
+            'GPS': 1240215503.0,
+            'luminosity_distance': 160.0,
+            'mass_1_source': 2.0,
+        },
+        'mock-event-3': {
+            'GPS': 1240215503.0,
+            'luminosity_distance': 150.0,
+            'mass_1_source': 2.1,
+        }
+    }
+}
 
 
 @pytest.mark.remote
 def test_find_datasets():
     sets = datasets.find_datasets()
     for dset in ('S6', 'O1', 'GW150914-v1', 'GW170817-v3'):
         assert dset in sets
@@ -58,15 +77,15 @@
 
 
 @pytest.mark.remote
 def test_find_datasets_type():
     runsets = datasets.find_datasets(type='run')
     assert 'O1' in runsets
     run_regex = re.compile(
-        r'\A([OS]\d+([a-z])?|BKGW\d{6})(_\d+KHZ)?(_[RV]\d+)?\Z',
+        r'\A([OS]\d+([a-z]|[A-Z]+)?|BKGW\d{6})(_\d+KHZ)?(_[RV]\d+)?\Z',
     )
     for dset in runsets:
         assert run_regex.match(dset)
 
     assert datasets.find_datasets(type='badtype') == []
 
 
@@ -88,15 +107,15 @@
     sets = datasets.find_datasets(type='event', version=1, detector='L1')
     assert "GW150914-v1" in sets
     assert "GW150914-v3" not in sets  # v3
 
 
 @mock.patch("gwosc.datasets._run_datasets", return_value=[])
 def test_find_datasets_warning(_):
-    with pytest.warns(None):
+    with pytest.warns(UserWarning):
         datasets.find_datasets(type='run', version=1)
 
 
 @pytest.mark.remote
 def test_event_gps():
     assert datasets.event_gps('GW170817') == 1187008882.4
 
@@ -230,7 +249,30 @@
     'gwosc.datasets.find_datasets',
     mock.MagicMock(side_effect=[["testrun"], [], ["testevent"], [], [], []]),
 )
 def test_dataset_type_local():
     assert datasets.dataset_type("testevent") == "event"
     with pytest.raises(ValueError):
         datasets.dataset_type("invalid")
+
+
+@pytest.mark.remote
+def test_query_events():
+    events = datasets.query_events(
+        select=["10 <= luminosity-distance <= 200"]
+    )
+    assert 'GW190425-v1' in events
+    assert 'GW190425-v2' in events
+    assert 'GW190425_081805-v3' in events
+
+
+@mock.patch(
+    'gwosc.api.fetch_filtered_events_json',
+    mock.MagicMock(return_value=EVENT_JSON),
+)
+def test_query_events_local():
+    events = datasets.query_events(
+        select=["mass-1-source >= 1.4", "10 <= luminosity-distance <= 200"]
+    )
+    assert 'mock-event-1' in events
+    assert 'mock-event-2' in events
+    assert 'mock-event-2' in events
```

### Comparing `gwosc-0.6.1/gwosc/tests/test_locate.py` & `gwosc-0.7.0/gwosc/tests/test_locate.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,26 +53,14 @@
     """Regression test against version not being respected in get_urls
     """
     urls = locate.get_urls('L1', 1187008877, 1187008887, version=2)
     assert Path(urls[0]).name == "L-L1_LOSC_CLN_4_V1-1187007040-2048.hdf5"
 
 
 @pytest.mark.remote
-def test_get_urls_deprecated_tag():
-    # test `tag` prints a warning
-    pytest.deprecated_call(
-        locate.get_urls,
-        "L1",
-        1187007040,
-        1187009088,
-        tag="TEST",
-    )
-
-
-@pytest.mark.remote
 def test_get_event_urls():
     urls = locate.get_event_urls("GW150914-v3", sample_rate=4096)
     assert len(urls) == 4
     for url in urls:
         assert "_4KHZ" in url
```

### Comparing `gwosc-0.6.1/gwosc/tests/test_timeline.py` & `gwosc-0.7.0/gwosc/tests/test_timeline.py`

 * *Files identical despite different names*

### Comparing `gwosc-0.6.1/gwosc/tests/test_urls.py` & `gwosc-0.7.0/gwosc/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `gwosc-0.6.1/gwosc/tests/test_utils.py` & `gwosc-0.7.0/gwosc/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwosc-0.6.1/gwosc/timeline.py` & `gwosc-0.7.0/gwosc/timeline.py`

 * *Files identical despite different names*

### Comparing `gwosc-0.6.1/gwosc/urls.py` & `gwosc-0.7.0/gwosc/urls.py`

 * *Files identical despite different names*

### Comparing `gwosc-0.6.1/gwosc/utils.py` & `gwosc-0.7.0/gwosc/utils.py`

 * *Files identical despite different names*

### Comparing `gwosc-0.6.1/gwosc.egg-info/PKG-INFO` & `gwosc-0.7.0/gwosc.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,147 +1,20 @@
 Metadata-Version: 2.1
 Name: gwosc
-Version: 0.6.1
+Version: 0.7.0
 Summary: A python interface to the GW Open Science data archive
-Home-page: https://github.com/gwpy/gwosc/
+Home-page: https://git.ligo.org/gwosc/client/
+Download-URL: https://pypi.org/project/gwosc/
 Author: Duncan Macleod
 Author-email: duncan.macleod@ligo.org
 License: MIT
-Download-URL: https://pypi.org/project/gwosc/
-Project-URL: Bug Tracker, https://github.com/gwpy/gwosc/issues
-Project-URL: Discussion Forum, https://gwpy.slack.com
+Project-URL: Bug Tracker, https://git.ligo.org/gwosc/client/-/issues
+Project-URL: Discussion Forum, https://ask.igwn.org
 Project-URL: Documentation, https://gwosc.readthedocs.io
-Project-URL: Source Code, https://github.com/gwpy/gwosc.git
-Description: # `gwosc` client API
-        
-        The `gwosc` package provides an interface to querying the open data
-        releases hosted on <https://gw-openscience.org> from the GEO, LIGO,
-        and Virgo gravitational-wave observatories.
-        
-        ## Release status
-        
-        [![PyPI version](https://badge.fury.io/py/gwosc.svg)](http://badge.fury.io/py/gwosc)
-        [![Conda version](https://img.shields.io/conda/vn/conda-forge/gwosc.svg)](https://anaconda.org/conda-forge/gwosc/)  
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1196306.svg)](https://doi.org/10.5281/zenodo.1196306)
-        [![License](https://img.shields.io/pypi/l/gwosc.svg)](https://choosealicense.com/licenses/mit/)
-        ![Supported Python versions](https://img.shields.io/pypi/pyversions/gwosc.svg)
-        
-        ## Development status
-        
-        [![Build status](https://github.com/gwpy/gwosc/actions/workflows/build.yml/badge.svg)](https://github.com/gwpy/gwosc/actions/workflows/build.yml)
-        [![Codecov](https://codecov.io/gh/gwpy/gwosc/branch/main/graph/badge.svg?token=A0b4PysQYA)](https://codecov.io/gh/gwpy/gwosc)
-        [![Maintainability](https://api.codeclimate.com/v1/badges/234aad1c71f0642d3e60/maintainability)](https://codeclimate.com/github/gwpy/gwosc/maintainability)
-        [![Documentation](https://readthedocs.org/projects/gwosc/badge/?version=latest)](https://gwosc.readthedocs.io/en/latest/?badge=latest)
-        
-        ## Installation
-        
-        To install:
-        
-            conda install -c conda-forge gwosc
-        
-        or
-        
-            pip install gwosc
-        
-        ## Searching for datasets
-        
-        To search for available datasets (correct as of March 14 2018):
-        
-        ```python
-        >>> from gwosc import datasets
-        >>> datasets.find_datasets()
-        ['GW150914', 'GW151226', 'GW170104', 'GW170608', 'GW170814', 'GW170817', 'LVT151012', 'O1', 'S5', 'S6']
-        >>> datasets.find_datasets(detector='V1')
-        ['GW170814', 'GW170817']
-        >>> datasets.find_datasets(type='run')
-        ['O1', 'S5', 'S6']
-        ```
-        
-        To query for the GPS time of an event dataset (or vice-versa):
-        
-        ```python
-        >>> datasets.event_gps('GW170817')
-        1187008882.43
-        >>> datasets.event_at_gps(1187008882)
-        'GW170817'
-        ```
-        
-        Similar queries are available for observing run datasets:
-        
-        ```python
-        >>> datasets.run_segment('O1')
-        (1126051217, 1137254417)
-        >>> datasets.run_at_gps(1135136350)  # event_gps('GW151226')
-        'O1'
-        ```
-        
-        ## Locating data URLs by event name
-        
-        You can search for remote data URLS based on the event name:
-        
-        ```python
-        >>> from gwosc.locate import get_event_urls
-        >>> get_event_urls('GW150914')
-        ['https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/H-H1_GWOSC_4KHZ_R1-1126259447-32.hdf5', 'https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/H-H1_GWOSC_4KHZ_R1-1126257415-4096.hdf5', 'https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126259447-32.hdf5', 'https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126257415-4096.hdf5']
-        ```
-        
-        You can down-select the URLs using keyword arguments:
-        
-        ```python
-        >>> get_event_urls('GW150914', detector='L1', duration=32)
-        ['https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126259447-32.hdf5']
-        ```
-        
-        ## Locating data URLs by GPS interval
-        
-        You can search for remote data URLs based on the GPS time interval as
-        follows:
-        
-        ```python
-        >>> from gwosc.locate import get_urls
-        >>> get_urls('L1', 968650000, 968660000)
-        ['https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968646656-4096.hdf5', 'https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968650752-4096.hdf5', 'https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968654848-4096.hdf5', 'https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968658944-4096.hdf5']
-        ```
-        
-        This arguments for this function are as follows
-        
-        -   `detector` : the prefix of the relevant gravitational-wave
-            interferometer, either `'H1'` for LIGO-Hanford, or `'L1'` for LIGO
-            Livingston,
-        -   `start`: the GPS start time of the interval of interest
-        -   `end`: the GPS end time of the interval of interest
-        
-        By default, this method will return the paths to HDF5 files for the 4
-        kHz sample-rate data, these can be specified as keyword arguments. For
-        full information, run
-        
-        ```python
-        >>> help(get_urls)
-        ```
-        
-        ## Query for Timeline segments
-        
-        You can also search for Timeline segments, based on a flag name, and a
-        GPS time interval as follows:
-        
-        ```python
-        >>> from gwosc.timeline import get_segments
-        >>> get_segments('H1_DATA', 1126051217, 1126151217)
-        [(1126073529, 1126114861), (1126121462, 1126123267), (1126123553, 1126126832), (1126139205, 1126139266), (1126149058, 1126151217)]
-        ```
-        
-        The output is a `list` of `(start, end)` 2-tuples which each represent a
-        semi-open time interval.
-        
-        For documentation on what flags are available, for example for the O1
-        science run, see [the O1 data release page](https://gw-openscience.org/O1/)
-        (*Data Quality*).
-        
-        
-Platform: UNKNOWN
+Project-URL: Source Code, https://git.ligo.org/gwosc/client.git
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -152,7 +25,134 @@
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
+Provides-Extra: lint
+License-File: LICENSE
+
+# `gwosc` client API
+
+The `gwosc` package provides an interface to querying the open data
+releases hosted on <https://gw-openscience.org> from the GEO, LIGO,
+and Virgo gravitational-wave observatories.
+
+## Release status
+
+[![PyPI version](https://badge.fury.io/py/gwosc.svg)](http://badge.fury.io/py/gwosc)
+[![Conda version](https://img.shields.io/conda/vn/conda-forge/gwosc.svg)](https://anaconda.org/conda-forge/gwosc/)  
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1196306.svg)](https://doi.org/10.5281/zenodo.1196306)
+[![License](https://img.shields.io/pypi/l/gwosc.svg)](https://choosealicense.com/licenses/mit/)
+![Supported Python versions](https://img.shields.io/pypi/pyversions/gwosc.svg)
+
+## Development status
+
+[![Build status](https://git.ligo.org/gwosc/client/badges/main/pipeline.svg)](https://git.ligo.org/gwosc/client/-/pipelines)
+![Code coverage](https://git.ligo.org/gwosc/client/badges/main/coverage.svg)
+[![Documentation](https://readthedocs.org/projects/gwosc/badge/?version=latest)](https://gwosc.readthedocs.io/en/latest/?badge=latest)
+
+## Installation
+
+To install:
+
+    conda install -c conda-forge gwosc
+
+or
+
+    pip install gwosc
+
+## Searching for datasets
+
+To search for available datasets (correct as of March 14 2018):
+
+```python
+>>> from gwosc import datasets
+>>> datasets.find_datasets()
+['GW150914', 'GW151226', 'GW170104', 'GW170608', 'GW170814', 'GW170817', 'LVT151012', 'O1', 'S5', 'S6']
+>>> datasets.find_datasets(detector='V1')
+['GW170814', 'GW170817']
+>>> datasets.find_datasets(type='run')
+['O1', 'S5', 'S6']
+```
+
+To query for the GPS time of an event dataset (or vice-versa):
+
+```python
+>>> datasets.event_gps('GW170817')
+1187008882.43
+>>> datasets.event_at_gps(1187008882)
+'GW170817'
+```
+
+Similar queries are available for observing run datasets:
+
+```python
+>>> datasets.run_segment('O1')
+(1126051217, 1137254417)
+>>> datasets.run_at_gps(1135136350)  # event_gps('GW151226')
+'O1'
+```
+
+## Locating data URLs by event name
+
+You can search for remote data URLS based on the event name:
+
+```python
+>>> from gwosc.locate import get_event_urls
+>>> get_event_urls('GW150914')
+['https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/H-H1_GWOSC_4KHZ_R1-1126259447-32.hdf5', 'https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/H-H1_GWOSC_4KHZ_R1-1126257415-4096.hdf5', 'https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126259447-32.hdf5', 'https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126257415-4096.hdf5']
+```
+
+You can down-select the URLs using keyword arguments:
+
+```python
+>>> get_event_urls('GW150914', detector='L1', duration=32)
+['https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126259447-32.hdf5']
+```
+
+## Locating data URLs by GPS interval
+
+You can search for remote data URLs based on the GPS time interval as
+follows:
+
+```python
+>>> from gwosc.locate import get_urls
+>>> get_urls('L1', 968650000, 968660000)
+['https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968646656-4096.hdf5', 'https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968650752-4096.hdf5', 'https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968654848-4096.hdf5', 'https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968658944-4096.hdf5']
+```
+
+This arguments for this function are as follows
+
+-   `detector` : the prefix of the relevant gravitational-wave
+    interferometer, either `'H1'` for LIGO-Hanford, or `'L1'` for LIGO
+    Livingston,
+-   `start`: the GPS start time of the interval of interest
+-   `end`: the GPS end time of the interval of interest
+
+By default, this method will return the paths to HDF5 files for the 4
+kHz sample-rate data, these can be specified as keyword arguments. For
+full information, run
+
+```python
+>>> help(get_urls)
+```
+
+## Query for Timeline segments
+
+You can also search for Timeline segments, based on a flag name, and a
+GPS time interval as follows:
+
+```python
+>>> from gwosc.timeline import get_segments
+>>> get_segments('H1_DATA', 1126051217, 1126151217)
+[(1126073529, 1126114861), (1126121462, 1126123267), (1126123553, 1126126832), (1126139205, 1126139266), (1126149058, 1126151217)]
+```
+
+The output is a `list` of `(start, end)` 2-tuples which each represent a
+semi-open time interval.
+
+For documentation on what flags are available, for example for the O1
+science run, see [the O1 data release page](https://gw-openscience.org/O1/)
+(*Data Quality*).
+
```

### Comparing `gwosc-0.6.1/gwosc.spec` & `gwosc-0.7.0/gwosc.spec`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 %define name    gwosc
-%define version 0.6.1
+%define version 0.7.0
 %define release 1
 
 Name:      %{name}
 Version:   %{version}
 Release:   %{release}%{?dist}
 Summary:   A python interface to the Gravitational-Wave Open Science Center data archive
 
@@ -41,14 +41,15 @@
 releases hosted on <https://gw-openscience.org> from the GEO, LIGO,
 and Virgo gravitational-wave observatories.
 
 # -- python-3X-gwosc
 
 %package -n python%{python3_pkgversion}-%{name}
 Summary:  %{summary}
+Requires: python%{python3_pkgversion}-requests >= 1.0.0
 %{?python_provide:%python_provide python%{python3_pkgversion}-%{name}}
 %description -n python%{python3_pkgversion}-%{name}
 The `gwosc` package provides an interface to querying the open data
 releases hosted on <https://gw-openscience.org> from the GEO, LIGO,
 and Virgo gravitational-wave observatories.
 
 # -- build steps
@@ -74,14 +75,17 @@
 %license LICENSE
 %doc README.md
 %{python3_sitelib}/*
 
 # -- changelog
 
 %changelog
+* Mon Apr 10 2023 Duncan Macleod <duncan.macleod@ligo.org> - 0.7.0-1
+- update to 0.7.0
+
 * Thu Aug 12 2021 Duncan Macleod <duncan.macleod@ligo.org> - 0.6.1-1
 - update to 0.6.1
 
 * Mon Aug 09 2021 Duncan Macleod <duncan.macleod@ligo.org> - 0.6.0-1
 - update to 0.6.0
 
 * Wed May 19 2021 Duncan Macleod <duncan.macleod@ligo.org> - 0.5.8-1
```

### Comparing `gwosc-0.6.1/setup.cfg` & `gwosc-0.7.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 author = Duncan Macleod
 author_email = duncan.macleod@ligo.org
 description = A python interface to the GW Open Science data archive
 license = MIT
 license_files = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/gwpy/gwosc/
+url = https://git.ligo.org/gwosc/client/
 download_url = https://pypi.org/project/gwosc/
 project_urls = 
-	Bug Tracker = https://github.com/gwpy/gwosc/issues
-	Discussion Forum = https://gwpy.slack.com
+	Bug Tracker = https://git.ligo.org/gwosc/client/-/issues
+	Discussion Forum = https://ask.igwn.org
 	Documentation = https://gwosc.readthedocs.io
-	Source Code = https://github.com/gwpy/gwosc.git
+	Source Code = https://git.ligo.org/gwosc/client.git
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.5
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
@@ -46,36 +46,15 @@
 	pytest-cov
 	pytest-socket
 	requests-mock >= 1.5.0
 docs = 
 	sphinx
 	sphinx-automodapi
 	sphinx_rtd_theme
-
-[coverage:run]
-source = gwosc
-omit = 
-	gwosc/_version.py,
-	setup.py,
-
-[flake8]
-select = 
-	E,
-	F,
-	W,
-ignore = 
-	W503,
-exclude = 
-	__pycache__,
-	.eggs/,
-	.git/,
-	build/,
-	docs/,
-	gwosc/_version.py,
-	venv/,
-per-file-ignores = 
-	__init__.py:F401
+lint = 
+	flake8 < 5.0.0a0
+	flake8-bandit
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

