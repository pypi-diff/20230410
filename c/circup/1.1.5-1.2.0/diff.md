# Comparing `tmp/circup-1.1.5.tar.gz` & `tmp/circup-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circup-1.1.5.tar", last modified: Tue Mar 21 00:55:53 2023, max compression
+gzip compressed data, was "circup-1.2.0.tar", last modified: Mon Apr 10 19:30:05 2023, max compression
```

## Comparing `circup-1.1.5.tar` & `circup-1.2.0.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 00:55:53.055857 circup-1.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 00:55:53.051856 circup-1.1.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-03-21 00:55:34.000000 circup-1.1.5/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-03-21 00:55:34.000000 circup-1.1.5/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 00:55:53.051856 circup-1.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-21 00:55:34.000000 circup-1.1.5/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-03-21 00:55:34.000000 circup-1.1.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-03-21 00:55:34.000000 circup-1.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-03-21 00:55:34.000000 circup-1.1.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-03-21 00:55:34.000000 circup-1.1.5/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-03-21 00:55:34.000000 circup-1.1.5/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-21 00:55:34.000000 circup-1.1.5/CODE_OF_CONDUCT.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-03-21 00:55:34.000000 circup-1.1.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-21 00:55:34.000000 circup-1.1.5/CONTRIBUTING.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-21 00:55:34.000000 circup-1.1.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 00:55:53.051856 circup-1.1.5/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-03-21 00:55:34.000000 circup-1.1.5/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-21 00:55:34.000000 circup-1.1.5/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-21 00:55:34.000000 circup-1.1.5/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10910 2023-03-21 00:55:53.055857 circup-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-03-21 00:55:34.000000 circup-1.1.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-21 00:55:34.000000 circup-1.1.5/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 00:55:53.051856 circup-1.1.5/circup/
--rw-r--r--   0 runner    (1001) docker     (123)    60127 2023-03-21 00:55:34.000000 circup-1.1.5/circup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 00:55:53.055857 circup-1.1.5/circup/config/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-21 00:55:34.000000 circup-1.1.5/circup/config/bundle_config.json
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-21 00:55:34.000000 circup-1.1.5/circup/config/bundle_config.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 00:55:53.051856 circup-1.1.5/circup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10910 2023-03-21 00:55:52.000000 circup-1.1.5/circup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-21 00:55:53.000000 circup-1.1.5/circup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 00:55:52.000000 circup-1.1.5/circup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-21 00:55:52.000000 circup-1.1.5/circup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-21 00:55:52.000000 circup-1.1.5/circup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-21 00:55:52.000000 circup-1.1.5/circup.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 00:55:53.055857 circup-1.1.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 00:55:53.055857 circup-1.1.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-21 00:55:34.000000 circup-1.1.5/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-21 00:55:34.000000 circup-1.1.5/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-03-21 00:55:34.000000 circup-1.1.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-21 00:55:34.000000 circup-1.1.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-21 00:55:34.000000 circup-1.1.5/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)    36437 2023-03-21 00:55:34.000000 circup-1.1.5/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-21 00:55:34.000000 circup-1.1.5/docs/logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-21 00:55:34.000000 circup-1.1.5/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-21 00:55:34.000000 circup-1.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-21 00:55:34.000000 circup-1.1.5/requirements.txt.license
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 00:55:53.055857 circup-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-03-21 00:55:34.000000 circup-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 00:55:53.055857 circup-1.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 00:55:34.000000 circup-1.1.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 00:55:53.055857 circup-1.1.5/tests/bad_module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 00:55:34.000000 circup-1.1.5/tests/bad_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-21 00:55:34.000000 circup-1.1.5/tests/bad_module/my_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-21 00:55:34.000000 circup-1.1.5/tests/bundle.json
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-21 00:55:34.000000 circup-1.1.5/tests/bundle.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-21 00:55:34.000000 circup-1.1.5/tests/device.json
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-21 00:55:34.000000 circup-1.1.5/tests/device.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 00:55:53.055857 circup-1.1.5/tests/dir_module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 00:55:34.000000 circup-1.1.5/tests/dir_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-21 00:55:34.000000 circup-1.1.5/tests/dir_module/my_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-21 00:55:34.000000 circup-1.1.5/tests/import_styles.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-21 00:55:34.000000 circup-1.1.5/tests/local_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-21 00:55:34.000000 circup-1.1.5/tests/local_module_cp7.mpy
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-21 00:55:34.000000 circup-1.1.5/tests/local_module_cp7.mpy.license
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-21 00:55:34.000000 circup-1.1.5/tests/mount_exists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-21 00:55:34.000000 circup-1.1.5/tests/mount_exists.txt.license
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-03-21 00:55:34.000000 circup-1.1.5/tests/mount_missing.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-21 00:55:34.000000 circup-1.1.5/tests/mount_missing.txt.license
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-21 00:55:34.000000 circup-1.1.5/tests/remote_module.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-21 00:55:34.000000 circup-1.1.5/tests/test_bundle_config.json
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-21 00:55:34.000000 circup-1.1.5/tests/test_bundle_config.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-21 00:55:34.000000 circup-1.1.5/tests/test_bundle_config_local.json
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-21 00:55:34.000000 circup-1.1.5/tests/test_bundle_config_local.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    39833 2023-03-21 00:55:34.000000 circup-1.1.5/tests/test_circup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-03-21 00:55:34.000000 circup-1.1.5/tests/test_module.mpy
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-21 00:55:34.000000 circup-1.1.5/tests/test_module.mpy.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:05.158273 circup-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:05.150273 circup-1.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-10 19:29:52.000000 circup-1.2.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-10 19:29:52.000000 circup-1.2.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:05.150273 circup-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-10 19:29:52.000000 circup-1.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 19:29:52.000000 circup-1.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-10 19:29:52.000000 circup-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-10 19:29:52.000000 circup-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-04-10 19:29:52.000000 circup-1.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-10 19:29:52.000000 circup-1.2.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 19:29:52.000000 circup-1.2.0/CODE_OF_CONDUCT.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-04-10 19:29:52.000000 circup-1.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 19:29:52.000000 circup-1.2.0/CONTRIBUTING.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-10 19:29:52.000000 circup-1.2.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:05.150273 circup-1.2.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-10 19:29:52.000000 circup-1.2.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-10 19:29:52.000000 circup-1.2.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-10 19:29:52.000000 circup-1.2.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10910 2023-04-10 19:30:05.158273 circup-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-04-10 19:29:52.000000 circup-1.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 19:29:52.000000 circup-1.2.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:05.150273 circup-1.2.0/circup/
+-rw-r--r--   0 runner    (1001) docker     (123)    61068 2023-04-10 19:29:52.000000 circup-1.2.0/circup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:05.154273 circup-1.2.0/circup/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-10 19:29:52.000000 circup-1.2.0/circup/config/bundle_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 19:29:52.000000 circup-1.2.0/circup/config/bundle_config.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:05.154273 circup-1.2.0/circup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10910 2023-04-10 19:30:05.000000 circup-1.2.0/circup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-10 19:30:05.000000 circup-1.2.0/circup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:30:05.000000 circup-1.2.0/circup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-10 19:30:05.000000 circup-1.2.0/circup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-10 19:30:05.000000 circup-1.2.0/circup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-10 19:30:05.000000 circup-1.2.0/circup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:05.154273 circup-1.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:05.154273 circup-1.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-10 19:29:52.000000 circup-1.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-10 19:29:52.000000 circup-1.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-04-10 19:29:52.000000 circup-1.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-10 19:29:52.000000 circup-1.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 19:29:52.000000 circup-1.2.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)    36437 2023-04-10 19:29:52.000000 circup-1.2.0/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 19:29:52.000000 circup-1.2.0/docs/logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-10 19:29:52.000000 circup-1.2.0/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-10 19:29:52.000000 circup-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 19:29:52.000000 circup-1.2.0/requirements.txt.license
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 19:30:05.158273 circup-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-10 19:29:52.000000 circup-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:05.158273 circup-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:29:52.000000 circup-1.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:05.158273 circup-1.2.0/tests/bad_module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:29:52.000000 circup-1.2.0/tests/bad_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-10 19:29:52.000000 circup-1.2.0/tests/bad_module/my_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-10 19:29:52.000000 circup-1.2.0/tests/bad_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-10 19:29:52.000000 circup-1.2.0/tests/bundle.json
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 19:29:52.000000 circup-1.2.0/tests/bundle.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-10 19:29:52.000000 circup-1.2.0/tests/device.json
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 19:29:52.000000 circup-1.2.0/tests/device.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:05.158273 circup-1.2.0/tests/dir_module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:29:52.000000 circup-1.2.0/tests/dir_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-10 19:29:52.000000 circup-1.2.0/tests/dir_module/my_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-10 19:29:52.000000 circup-1.2.0/tests/import_styles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-10 19:29:52.000000 circup-1.2.0/tests/local_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-10 19:29:52.000000 circup-1.2.0/tests/local_module_cp7.mpy
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 19:29:52.000000 circup-1.2.0/tests/local_module_cp7.mpy.license
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-10 19:29:52.000000 circup-1.2.0/tests/mount_exists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 19:29:52.000000 circup-1.2.0/tests/mount_exists.txt.license
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-10 19:29:52.000000 circup-1.2.0/tests/mount_missing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 19:29:52.000000 circup-1.2.0/tests/mount_missing.txt.license
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-10 19:29:52.000000 circup-1.2.0/tests/remote_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-10 19:29:52.000000 circup-1.2.0/tests/test_bundle_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 19:29:52.000000 circup-1.2.0/tests/test_bundle_config.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-10 19:29:52.000000 circup-1.2.0/tests/test_bundle_config_local.json
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 19:29:52.000000 circup-1.2.0/tests/test_bundle_config_local.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    40224 2023-04-10 19:29:52.000000 circup-1.2.0/tests/test_circup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-10 19:29:52.000000 circup-1.2.0/tests/test_module.mpy
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 19:29:52.000000 circup-1.2.0/tests/test_module.mpy.license
```

### Comparing `circup-1.1.5/.github/ISSUE_TEMPLATE.md` & `circup-1.2.0/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `circup-1.1.5/.github/PULL_REQUEST_TEMPLATE.md` & `circup-1.2.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `circup-1.1.5/.github/workflows/build.yml` & `circup-1.2.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circup-1.1.5/.github/workflows/release.yml` & `circup-1.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `circup-1.1.5/.gitignore` & `circup-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `circup-1.1.5/.pylintrc` & `circup-1.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circup-1.1.5/CODE_OF_CONDUCT.rst` & `circup-1.2.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `circup-1.1.5/CONTRIBUTING.rst` & `circup-1.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `circup-1.1.5/LICENSE` & `circup-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circup-1.1.5/LICENSES/CC-BY-4.0.txt` & `circup-1.2.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circup-1.1.5/LICENSES/MIT.txt` & `circup-1.2.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circup-1.1.5/LICENSES/Unlicense.txt` & `circup-1.2.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circup-1.1.5/PKG-INFO` & `circup-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circup
-Version: 1.1.5
+Version: 1.2.0
 Summary: A tool to manage/update libraries on CircuitPython devices.
 Home-page: https://github.com/adafruit/circup
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit,blinka,circuitpython,micropython,libraries
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `circup-1.1.5/README.rst` & `circup-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `circup-1.1.5/circup/__init__.py` & `circup-1.2.0/circup/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1052,15 +1052,23 @@
 def libraries_from_imports(code_py, mod_names):
     """
     Parse the given code.py file and return the imported libraries
 
     :param str code_py: Full path of the code.py file
     :return: sequence of library names
     """
-    imports = [info.name.split(".", 1)[0] for info in findimports.find_imports(code_py)]
+    # pylint: disable=broad-except
+    try:
+        found_imports = findimports.find_imports(code_py)
+    except Exception as ex:  # broad exception because anything could go wrong
+        logger.exception(ex)
+        click.secho('Unable to read the auto file: "{}"'.format(str(ex)), fg="red")
+        sys.exit(2)
+    # pylint: enable=broad-except
+    imports = [info.name.split(".", 1)[0] for info in found_imports]
     return [r for r in imports if r in mod_names]
 
 
 def libraries_from_requirements(requirements):
     """
     Clean up supplied requirements.txt and turn into tuple of CP libraries
 
@@ -1286,43 +1294,60 @@
 
 
 # pylint: disable=too-many-arguments,too-many-locals
 @main.command()
 @click.argument(
     "modules", required=False, nargs=-1, shell_complete=completion_for_install
 )
-@click.option("pyext", "--py", is_flag=True)
-@click.option("-r", "--requirement", type=click.Path(exists=True, dir_okay=False))
-@click.option("--auto/--no-auto", "-a/-A")
-@click.option("--auto-file", default="code.py")
+@click.option(
+    "pyext",
+    "--py",
+    is_flag=True,
+    help="Install the .py version of the module(s) instead of the mpy version.",
+)
+@click.option(
+    "-r",
+    "--requirement",
+    type=click.Path(exists=True, dir_okay=False),
+    help="specify a text file to install all modules listed in the text file."
+    " Typically requirements.txt.",
+)
+@click.option("--auto", "-a", help="Install the modules imported in code.py.")
+@click.option(
+    "--auto-file",
+    default=None,
+    help="Specify the name of a file on the board to read for auto install."
+    " Also accepts an absolute path or a local ./ path.",
+)
 @click.pass_context
 def install(ctx, modules, pyext, requirement, auto, auto_file):  # pragma: no cover
     """
     Install a named module(s) onto the device. Multiple modules
     can be installed at once by providing more than one module name, each
     separated by a space.
-
-    Option --py installs .py version of module(s).
-
-    Option -r allows specifying a text file to install all modules listed in
-    the text file.
-
-    Option -a installs based on the modules imported by code.py
     """
     # TODO: Ensure there's enough space on the device
     available_modules = get_bundle_versions(get_bundles_list())
     mod_names = {}
     for module, metadata in available_modules.items():
         mod_names[module.replace(".py", "").lower()] = metadata
     if requirement:
         with open(requirement, "r", encoding="utf-8") as rfile:
             requirements_txt = rfile.read()
         requested_installs = libraries_from_requirements(requirements_txt)
-    elif auto:
-        auto_file = os.path.join(ctx.obj["DEVICE_PATH"], auto_file)
+    elif auto or auto_file:
+        if auto_file is None:
+            auto_file = "code.py"
+        # pass a local file with "./" or "../"
+        is_relative = auto_file.split(os.sep)[0] in [os.path.curdir, os.path.pardir]
+        if not os.path.isabs(auto_file) and not is_relative:
+            auto_file = os.path.join(ctx.obj["DEVICE_PATH"], auto_file or "code.py")
+        if not os.path.isfile(auto_file):
+            click.secho(f"Auto file not found: {auto_file}", fg="red")
+            sys.exit(1)
         requested_installs = libraries_from_imports(auto_file, mod_names)
     else:
         requested_installs = modules
     requested_installs = sorted(set(requested_installs))
     click.echo(f"Searching for dependencies for: {requested_installs}")
     to_install = get_dependencies(requested_installs, mod_names=mod_names)
     device_modules = get_device_versions(ctx.obj["DEVICE_PATH"])
```

### Comparing `circup-1.1.5/circup.egg-info/PKG-INFO` & `circup-1.2.0/circup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circup
-Version: 1.1.5
+Version: 1.2.0
 Summary: A tool to manage/update libraries on CircuitPython devices.
 Home-page: https://github.com/adafruit/circup
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit,blinka,circuitpython,micropython,libraries
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `circup-1.1.5/circup.egg-info/SOURCES.txt` & `circup-1.2.0/circup.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 docs/index.rst
 docs/index.rst.license
 docs/logo.png
 docs/logo.png.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 tests/__init__.py
+tests/bad_python.py
 tests/bundle.json
 tests/bundle.json.license
 tests/device.json
 tests/device.json.license
 tests/import_styles.py
 tests/local_module.py
 tests/local_module_cp7.mpy
```

### Comparing `circup-1.1.5/docs/_static/favicon.ico` & `circup-1.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circup-1.1.5/docs/conf.py` & `circup-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circup-1.1.5/docs/logo.png` & `circup-1.2.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `circup-1.1.5/requirements.txt` & `circup-1.2.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `circup-1.1.5/setup.py` & `circup-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `circup-1.1.5/tests/bundle.json` & `circup-1.2.0/tests/bundle.json`

 * *Files identical despite different names*

### Comparing `circup-1.1.5/tests/mount_exists.txt` & `circup-1.2.0/tests/mount_exists.txt`

 * *Files identical despite different names*

### Comparing `circup-1.1.5/tests/test_circup.py` & `circup-1.2.0/tests/test_circup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1026,7 +1026,16 @@
     print(result)
     assert result == [
         "adafruit_bus_device",
         "adafruit_button",
         "adafruit_esp32spi",
         "adafruit_hid",
     ]
+
+
+def test_libraries_from_imports_bad():
+    """Ensure that we catch an import error"""
+    TEST_BUNDLE_MODULES = {"one.py": {}, "two.py": {}, "three.py": {}}
+    runner = CliRunner()
+    with mock.patch("circup.get_bundle_versions", return_value=TEST_BUNDLE_MODULES):
+        result = runner.invoke(circup.install, ["--auto-file", "./tests/bad_python.py"])
+    assert result.exit_code == 2
```

### Comparing `circup-1.1.5/tests/test_module.mpy` & `circup-1.2.0/tests/test_module.mpy`

 * *Files identical despite different names*

