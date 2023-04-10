# Comparing `tmp/dkist_fits_specifications-3.4.0.tar.gz` & `tmp/dkist_fits_specifications-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_fits_specifications-3.4.0.tar", last modified: Wed Mar 15 19:59:29 2023, max compression
+gzip compressed data, was "dkist_fits_specifications-3.5.0.tar", last modified: Mon Apr 10 15:34:50 2023, max compression
```

## Comparing `dkist_fits_specifications-3.4.0.tar` & `dkist_fits_specifications-3.5.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:59:29.524880 dkist_fits_specifications-3.4.0/
--rw-rw-rw-   0 root         (0) root         (0)     3334 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      676 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)     3955 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     6506 2023-03-15 19:59:29.524880 dkist_fits_specifications-3.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6089 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2283 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:59:29.512880 dkist_fits_specifications-3.4.0/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/changelog/.gitempty
--rwxrwxrwx   0 root         (0) root         (0)      346 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:59:29.512880 dkist_fits_specifications-3.4.0/dkist_fits_specifications/
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/py.typed
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:59:29.516880 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/
--rw-rw-rw-   0 root         (0) root         (0)     3584 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:59:29.516880 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/
--rw-rw-rw-   0 root         (0) root         (0)      715 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/ao.yml
--rw-rw-rw-   0 root         (0) root         (0)     2951 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/camera.yml
--rw-rw-rw-   0 root         (0) root         (0)      477 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/compression.yml
--rw-rw-rw-   0 root         (0) root         (0)    10244 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/cryonirsp.yml
--rw-rw-rw-   0 root         (0) root         (0)     1466 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/dkist-dkist.yml
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/dkist-id.yml
--rw-rw-rw-   0 root         (0) root         (0)     4395 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/dlnirsp.yml
--rw-rw-rw-   0 root         (0) root         (0)     1709 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/fits.yml
--rw-rw-rw-   0 root         (0) root         (0)     1934 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/pac.yml
--rw-rw-rw-   0 root         (0) root         (0)     2653 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/telescope.yml
--rw-rw-rw-   0 root         (0) root         (0)      930 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/vbi.yml
--rw-rw-rw-   0 root         (0) root         (0)     3047 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/visp.yml
--rw-rw-rw-   0 root         (0) root         (0)     2299 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/vtf.yml
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/wfc.yml
--rw-rw-rw-   0 root         (0) root         (0)      703 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/ws.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:59:29.516880 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/
--rw-rw-rw-   0 root         (0) root         (0)    11708 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3117 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/level0.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:59:29.520880 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/
--rw-rw-rw-   0 root         (0) root         (0)     1811 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/ao.yml
--rw-rw-rw-   0 root         (0) root         (0)     5886 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/camera.yml
--rw-rw-rw-   0 root         (0) root         (0)     6341 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/compression.yml
--rw-rw-rw-   0 root         (0) root         (0)    13479 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/cryonirsp.yml
--rw-rw-rw-   0 root         (0) root         (0)     3736 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/datacenter.yml
--rw-rw-rw-   0 root         (0) root         (0)     4144 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/dataset.yml
--rw-rw-rw-   0 root         (0) root         (0)     2429 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/dkist-id.yml
--rw-rw-rw-   0 root         (0) root         (0)     1567 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/dkist-op.yml
--rw-rw-rw-   0 root         (0) root         (0)     8355 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/dlnirsp.yml
--rw-rw-rw-   0 root         (0) root         (0)     7276 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/fits.yml
--rw-rw-rw-   0 root         (0) root         (0)     2304 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/pac.yml
--rw-rw-rw-   0 root         (0) root         (0)      778 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/stats.yml
--rw-rw-rw-   0 root         (0) root         (0)     7410 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/telescope.yml
--rw-rw-rw-   0 root         (0) root         (0)     1913 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/vbi.yml
--rw-rw-rw-   0 root         (0) root         (0)     2939 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/visp.yml
--rw-rw-rw-   0 root         (0) root         (0)     3660 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/vtf.yml
--rw-rw-rw-   0 root         (0) root         (0)     1483 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/wfc.yml
--rw-rw-rw-   0 root         (0) root         (0)     1310 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/ws.yml
--rw-rw-rw-   0 root         (0) root         (0)     1001 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/spec214_full_schema.yml
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec_validation_schema.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:59:29.520880 dkist_fits_specifications-3.4.0/dkist_fits_specifications/tests/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1044 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/tests/test_122.py
--rw-rw-rw-   0 root         (0) root         (0)     2687 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/tests/test_214.py
--rw-rw-rw-   0 root         (0) root         (0)     2808 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/tests/test_expansions.py
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/tests/test_level0_214.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:59:29.520880 dkist_fits_specifications-3.4.0/dkist_fits_specifications/utils/
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3374 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/utils/formatter.py
--rw-rw-rw-   0 root         (0) root         (0)     1222 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/utils/frozendict.py
--rw-rw-rw-   0 root         (0) root         (0)     4782 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/utils/spec.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:59:29.520880 dkist_fits_specifications-3.4.0/dkist_fits_specifications/utils/sphinx/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/utils/sphinx/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8553 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/utils/sphinx/spec_table.py
--rw-rw-rw-   0 root         (0) root         (0)      345 2023-03-15 19:59:29.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:59:29.516880 dkist_fits_specifications-3.4.0/dkist_fits_specifications.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     6506 2023-03-15 19:59:29.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3341 2023-03-15 19:59:29.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-15 19:59:29.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-15 19:59:29.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-03-15 19:59:29.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-03-15 19:59:29.000000 dkist_fits_specifications-3.4.0/dkist_fits_specifications.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:59:29.524880 dkist_fits_specifications-3.4.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      872 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     1092 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3424 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/docs/level_one.rst
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/docs/reference.rst
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/docs/release_history.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:59:29.524880 dkist_fits_specifications-3.4.0/docs/specs/
--rw-rw-rw-   0 root         (0) root         (0)     1463 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/docs/specs/spec-122.rst
--rw-rw-rw-   0 root         (0) root         (0)     2668 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/docs/specs/spec-214.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:59:29.524880 dkist_fits_specifications-3.4.0/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1480 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/licenses/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1659 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/licenses/TEMPLATE_LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2030 2023-03-15 19:59:29.524880 dkist_fits_specifications-3.4.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      612 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1327 2023-03-15 19:59:02.000000 dkist_fits_specifications-3.4.0/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 15:34:50.477600 dkist_fits_specifications-3.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)     3334 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      676 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4276 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     6506 2023-04-10 15:34:50.477600 dkist_fits_specifications-3.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6089 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2283 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 15:34:50.465600 dkist_fits_specifications-3.5.0/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/changelog/.gitempty
+-rwxrwxrwx   0 root         (0) root         (0)      346 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 15:34:50.469600 dkist_fits_specifications-3.5.0/dkist_fits_specifications/
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/py.typed
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 15:34:50.469600 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/
+-rw-rw-rw-   0 root         (0) root         (0)     3584 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 15:34:50.473600 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)      715 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/ao.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2951 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/camera.yml
+-rw-rw-rw-   0 root         (0) root         (0)      477 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/compression.yml
+-rw-rw-rw-   0 root         (0) root         (0)    10244 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/cryonirsp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/dkist-dkist.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/dkist-id.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4395 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/dlnirsp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1709 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/fits.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1934 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/pac.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2653 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/telescope.yml
+-rw-rw-rw-   0 root         (0) root         (0)      930 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/vbi.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/visp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2299 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/vtf.yml
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/wfc.yml
+-rw-rw-rw-   0 root         (0) root         (0)      703 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/ws.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 15:34:50.473600 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/
+-rw-rw-rw-   0 root         (0) root         (0)    11880 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3117 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/level0.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 15:34:50.477600 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)     1811 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/ao.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5886 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/camera.yml
+-rw-rw-rw-   0 root         (0) root         (0)     6341 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/compression.yml
+-rw-rw-rw-   0 root         (0) root         (0)    13479 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/cryonirsp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3955 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/datacenter.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4144 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/dataset.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/dkist-id.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/dkist-op.yml
+-rw-rw-rw-   0 root         (0) root         (0)     8355 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/dlnirsp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     7276 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/fits.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2304 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/pac.yml
+-rw-rw-rw-   0 root         (0) root         (0)      778 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/stats.yml
+-rw-rw-rw-   0 root         (0) root         (0)     7410 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/telescope.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1913 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/vbi.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2939 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/visp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3660 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/vtf.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1483 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/wfc.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/ws.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/spec214_full_schema.yml
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec_validation_schema.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 15:34:50.477600 dkist_fits_specifications-3.5.0/dkist_fits_specifications/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1044 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/tests/test_122.py
+-rw-rw-rw-   0 root         (0) root         (0)     2687 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/tests/test_214.py
+-rw-rw-rw-   0 root         (0) root         (0)     2808 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/tests/test_expansions.py
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/tests/test_level0_214.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 15:34:50.477600 dkist_fits_specifications-3.5.0/dkist_fits_specifications/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3374 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/utils/formatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1222 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/utils/frozendict.py
+-rw-rw-rw-   0 root         (0) root         (0)     4782 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/utils/spec.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 15:34:50.477600 dkist_fits_specifications-3.5.0/dkist_fits_specifications/utils/sphinx/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/utils/sphinx/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8553 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/utils/sphinx/spec_table.py
+-rw-rw-rw-   0 root         (0) root         (0)      345 2023-04-10 15:34:50.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 15:34:50.469600 dkist_fits_specifications-3.5.0/dkist_fits_specifications.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6506 2023-04-10 15:34:50.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3341 2023-04-10 15:34:50.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-10 15:34:50.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-10 15:34:50.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-04-10 15:34:50.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-10 15:34:50.000000 dkist_fits_specifications-3.5.0/dkist_fits_specifications.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 15:34:50.477600 dkist_fits_specifications-3.5.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      872 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3424 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/docs/level_one.rst
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/docs/reference.rst
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/docs/release_history.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 15:34:50.477600 dkist_fits_specifications-3.5.0/docs/specs/
+-rw-rw-rw-   0 root         (0) root         (0)     1463 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/docs/specs/spec-122.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2668 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/docs/specs/spec-214.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 15:34:50.477600 dkist_fits_specifications-3.5.0/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/licenses/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2030 2023-04-10 15:34:50.481600 dkist_fits_specifications-3.5.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      612 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1327 2023-04-10 15:34:28.000000 dkist_fits_specifications-3.5.0/tox.ini
```

### Comparing `dkist_fits_specifications-3.4.0/.gitignore` & `dkist_fits_specifications-3.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/.pre-commit-config.yaml` & `dkist_fits_specifications-3.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/CHANGELOG.rst` & `dkist_fits_specifications-3.5.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v3.5.0 (2023-04-10)
+===================
+
+Backwards Compatible Changes to the Specification
+-------------------------------------------------
+
+- Added `NSPECLNS` and `SPECLN<sl>` keys to support inclusion of spectral line information. (`#34 <https://bitbucket.org/dkistdc/dkist-fits-specifications/pull-requests/34>`__)
+
+
 v3.4.0 (2023-03-15)
 ===================
 
 Backwards Compatible Changes to the Specification
 -------------------------------------------------
 
 - Add CRYO-NIRSP keys for tracking number of map scans. (`#32 <https://bitbucket.org/dkistdc/dkist-fits-specifications/pull-requests/32>`__)
```

### Comparing `dkist_fits_specifications-3.4.0/PKG-INFO` & `dkist_fits_specifications-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist_fits_specifications
-Version: 3.4.0
+Version: 3.5.0
 Summary: Machine readable FITS specifications for DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-fits-specifications/src/main/
 Author: AURA/NSO
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
```

### Comparing `dkist_fits_specifications-3.4.0/README.rst` & `dkist_fits_specifications-3.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/bitbucket-pipelines.yml` & `dkist_fits_specifications-3.5.0/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/__init__.py` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/__init__.py` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/ao.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/ao.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/camera.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/camera.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/cryonirsp.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/cryonirsp.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/dkist-dkist.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/dkist-dkist.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/dkist-id.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/dkist-id.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/dlnirsp.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/dlnirsp.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/fits.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/fits.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/pac.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/pac.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/telescope.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/telescope.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/vbi.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/vbi.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/visp.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/visp.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/vtf.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/vtf.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/wfc.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/wfc.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec122/schemas/ws.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec122/schemas/ws.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/__init__.py` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,14 +289,17 @@
         zval = [k for k in header.keys() if k.startswith("ZVAL")]
         z_max = max([int(k[-1]) for k in zval])
         z_expansion = ExpansionIndex(index="z", size=1, values=range(1, z_max + 1))
         f_expansion = ExpansionIndex(index="f", size=1, values=range(1, header["TFIELDS"] + 1))
         expansion_list.extend([z_expansion, f_expansion])
     pp_expansion = ExpansionIndex(index="pp", size=2, values=[1, 10, 25, 75, 90, 95, 98, 99])
     expansion_list.append(pp_expansion)
+    if "NSPECLNS" in header:
+        sl_expansion = ExpansionIndex(index="sl", size=2, values=range(1, header["NSPECLNS"] + 1))
+        expansion_list.append(sl_expansion)
     return expansion_list
 
 
 def expand_214_schema(
     schema: schema_type_hint, **header: dict[str, Any]
 ) -> dict[str, frozendict[str, Any]]:
     """
```

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/level0.py` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/level0.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/ao.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/ao.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/camera.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/camera.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/compression.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/compression.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/cryonirsp.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/cryonirsp.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/datacenter.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/datacenter.yml`

 * *Files 4% similar despite different names*

```diff
@@ -227,8 +227,22 @@
 00000e20: 7175 6972 6564 3a20 6661 6c73 650a 574b  quired: false.WK
 00000e30: 464c 5645 5253 3a0a 2020 6465 7363 7269  FLVERS:.  descri
 00000e40: 7074 696f 6e3a 2022 5665 7273 696f 6e20  ption: "Version 
 00000e50: 6f66 2074 6865 2077 6f72 6b66 6c6f 7720  of the workflow 
 00000e60: 7468 6174 2070 726f 6475 6365 6420 7468  that produced th
 00000e70: 6973 2064 6174 612e 220a 2020 7479 7065  is data.".  type
 00000e80: 3a20 7374 720a 2020 7265 7175 6972 6564  : str.  required
-00000e90: 3a20 6661 6c73 650a                      : false.
+00000e90: 3a20 6661 6c73 650a 4e53 5045 434c 4e53  : false.NSPECLNS
+00000ea0: 3a0a 2020 6465 7363 7269 7074 696f 6e3a  :.  description:
+00000eb0: 2022 4e75 6d62 6572 206f 6620 7265 6665   "Number of refe
+00000ec0: 7265 6e63 6520 7370 6563 7472 616c 206c  rence spectral l
+00000ed0: 696e 6573 2070 7265 7365 6e74 2069 6e20  ines present in 
+00000ee0: 7468 6520 6672 616d 652e 220a 2020 7479  the frame.".  ty
+00000ef0: 7065 3a20 696e 740a 2020 7265 7175 6972  pe: int.  requir
+00000f00: 6564 3a20 6661 6c73 650a 5350 4543 4c4e  ed: false.SPECLN
+00000f10: 3c73 6c3e 3a0a 2020 6465 7363 7269 7074  <sl>:.  descript
+00000f20: 696f 6e3a 2022 5265 6665 7265 6e63 6520  ion: "Reference 
+00000f30: 7370 6563 7472 616c 206c 696e 6520 7072  spectral line pr
+00000f40: 6573 656e 7420 696e 2074 6865 2066 7261  esent in the fra
+00000f50: 6d65 2e22 0a20 2074 7970 653a 2073 7472  me.".  type: str
+00000f60: 0a20 2072 6571 7569 7265 643a 2066 616c  .  required: fal
+00000f70: 7365 0a                                  se.
```

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/dataset.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/dataset.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/dkist-id.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/dkist-id.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/dkist-op.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/dkist-op.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/dlnirsp.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/dlnirsp.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/fits.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/fits.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/pac.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/pac.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/stats.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/stats.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/telescope.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/telescope.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/vbi.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/vbi.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/visp.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/visp.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/vtf.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/vtf.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/wfc.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/wfc.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/schemas/ws.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/schemas/ws.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec214/spec214_full_schema.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec214/spec214_full_schema.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/spec_validation_schema.yml` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/spec_validation_schema.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/tests/test_122.py` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/tests/test_122.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/tests/test_214.py` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/tests/test_214.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/tests/test_expansions.py` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/tests/test_expansions.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/utils/formatter.py` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/utils/frozendict.py` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/utils/frozendict.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/utils/spec.py` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/utils/spec.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications/utils/sphinx/spec_table.py` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications/utils/sphinx/spec_table.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications.egg-info/PKG-INFO` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-fits-specifications
-Version: 3.4.0
+Version: 3.5.0
 Summary: Machine readable FITS specifications for DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-fits-specifications/src/main/
 Author: AURA/NSO
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
```

### Comparing `dkist_fits_specifications-3.4.0/dkist_fits_specifications.egg-info/SOURCES.txt` & `dkist_fits_specifications-3.5.0/dkist_fits_specifications.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/docs/Makefile` & `dkist_fits_specifications-3.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/docs/conf.py` & `dkist_fits_specifications-3.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/docs/index.rst` & `dkist_fits_specifications-3.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/docs/level_one.rst` & `dkist_fits_specifications-3.5.0/docs/level_one.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/docs/make.bat` & `dkist_fits_specifications-3.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/docs/specs/spec-122.rst` & `dkist_fits_specifications-3.5.0/docs/specs/spec-122.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/docs/specs/spec-214.rst` & `dkist_fits_specifications-3.5.0/docs/specs/spec-214.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/licenses/LICENSE.rst` & `dkist_fits_specifications-3.5.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/licenses/TEMPLATE_LICENSE.rst` & `dkist_fits_specifications-3.5.0/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/pyproject.toml` & `dkist_fits_specifications-3.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/setup.cfg` & `dkist_fits_specifications-3.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/setup.py` & `dkist_fits_specifications-3.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.4.0/tox.ini` & `dkist_fits_specifications-3.5.0/tox.ini`

 * *Files identical despite different names*

