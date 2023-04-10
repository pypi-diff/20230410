# Comparing `tmp/dfimagetools-20230409.tar.gz` & `tmp/dfimagetools-20230410.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfimagetools-20230409.tar", last modified: Sun Apr  9 20:55:44 2023, max compression
+gzip compressed data, was "dfimagetools-20230410.tar", last modified: Mon Apr 10 08:01:47 2023, max compression
```

## Comparing `dfimagetools-20230409.tar` & `dfimagetools-20230410.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.132284 dfimagetools-20230409/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:43.984284 dfimagetools-20230409/.github/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.020284 dfimagetools-20230409/.github/workflows/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3653 2023-04-09 14:48:22.000000 dfimagetools-20230409/.github/workflows/test_docker.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1938 2023-04-09 14:48:22.000000 dfimagetools-20230409/.github/workflows/test_docs.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2239 2023-04-09 14:48:22.000000 dfimagetools-20230409/.github/workflows/test_tox.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22101 2023-04-09 14:48:22.000000 dfimagetools-20230409/.pylintrc
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      149 2022-04-30 13:22:39.000000 dfimagetools-20230409/.yamllint.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      479 2022-04-30 13:22:39.000000 dfimagetools-20230409/ACKNOWLEDGEMENTS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      292 2022-04-30 13:22:39.000000 dfimagetools-20230409/AUTHORS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2021-10-31 13:10:45.000000 dfimagetools-20230409/LICENSE
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      608 2022-01-29 19:59:40.000000 dfimagetools-20230409/MANIFEST.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      528 2022-01-29 19:59:40.000000 dfimagetools-20230409/MANIFEST.test_data.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      566 2023-04-09 20:55:44.132284 dfimagetools-20230409/PKG-INFO
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      153 2021-12-26 07:38:07.000000 dfimagetools-20230409/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-04-09 20:52:07.000000 dfimagetools-20230409/appveyor.yml
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:43.984284 dfimagetools-20230409/config/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.020284 dfimagetools-20230409/config/appveyor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2023-04-09 20:52:07.000000 dfimagetools-20230409/config/appveyor/install.ps1
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2023-04-09 14:48:22.000000 dfimagetools-20230409/config/appveyor/install.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2023-04-09 14:48:22.000000 dfimagetools-20230409/config/appveyor/runtests.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.022284 dfimagetools-20230409/config/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      175 2023-04-09 20:52:07.000000 dfimagetools-20230409/config/dpkg/changelog
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       23 2021-12-23 07:30:27.000000 dfimagetools-20230409/config/dpkg/clean
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        2 2023-04-09 14:48:22.000000 dfimagetools-20230409/config/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1798 2023-04-09 14:48:22.000000 dfimagetools-20230409/config/dpkg/control
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      976 2021-12-26 07:38:07.000000 dfimagetools-20230409/config/dpkg/copyright
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        8 2021-12-26 07:38:07.000000 dfimagetools-20230409/config/dpkg/dfimagetools-tools.install
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      105 2021-12-26 07:38:07.000000 dfimagetools-20230409/config/dpkg/python3-dfimagetools.install
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2023-04-09 14:48:22.000000 dfimagetools-20230409/config/dpkg/rules
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.022284 dfimagetools-20230409/config/dpkg/source/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2021-12-23 07:30:27.000000 dfimagetools-20230409/config/dpkg/source/format
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.022284 dfimagetools-20230409/config/pylint/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      229 2021-12-21 12:01:47.000000 dfimagetools-20230409/config/pylint/spelling-private-dict
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5687 2022-09-03 04:58:03.000000 dfimagetools-20230409/dependencies.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.024284 dfimagetools-20230409/dfimagetools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      110 2023-04-09 20:52:07.000000 dfimagetools-20230409/dfimagetools/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4432 2022-10-02 12:20:49.000000 dfimagetools-20230409/dfimagetools/artifact_filters.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9053 2022-10-02 12:20:49.000000 dfimagetools-20230409/dfimagetools/bodyfile.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2022-10-02 12:20:49.000000 dfimagetools-20230409/dfimagetools/data_stream_writer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      710 2022-10-02 12:20:49.000000 dfimagetools-20230409/dfimagetools/decorators.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3493 2022-10-02 12:20:49.000000 dfimagetools-20230409/dfimagetools/environment_variables.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6866 2022-10-02 12:20:49.000000 dfimagetools-20230409/dfimagetools/file_entry_lister.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2022-09-03 04:58:03.000000 dfimagetools-20230409/dfimagetools/helpers.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11121 2022-10-02 12:20:49.000000 dfimagetools-20230409/dfimagetools/path_resolver.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4304 2022-12-26 19:18:50.000000 dfimagetools-20230409/dfimagetools/recursive_hasher.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2362 2022-04-30 13:22:39.000000 dfimagetools-20230409/dfimagetools/resources.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2861 2022-12-26 04:50:18.000000 dfimagetools-20230409/dfimagetools/source_analyzer.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6222 2022-04-30 13:22:39.000000 dfimagetools-20230409/dfimagetools/windows_registry.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.025284 dfimagetools-20230409/dfimagetools.egg-info/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      566 2023-04-09 20:55:42.000000 dfimagetools-20230409/dfimagetools.egg-info/PKG-INFO
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1905 2023-04-09 20:55:43.000000 dfimagetools-20230409/dfimagetools.egg-info/SOURCES.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2023-04-09 20:55:42.000000 dfimagetools-20230409/dfimagetools.egg-info/dependency_links.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      801 2023-04-09 20:55:42.000000 dfimagetools-20230409/dfimagetools.egg-info/requires.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       13 2023-04-09 20:55:42.000000 dfimagetools-20230409/dfimagetools.egg-info/top_level.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      388 2021-12-26 07:38:07.000000 dfimagetools-20230409/dfimagetools.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.036284 dfimagetools-20230409/docs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2023-04-09 14:48:22.000000 dfimagetools-20230409/docs/conf.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      528 2022-11-21 19:36:05.000000 dfimagetools-20230409/docs/index.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      105 2023-04-09 14:48:38.000000 dfimagetools-20230409/docs/requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.053284 dfimagetools-20230409/docs/sources/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2022-12-18 20:43:00.000000 dfimagetools-20230409/docs/sources/Bodyfile-format.md
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.073284 dfimagetools-20230409/docs/sources/api/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2236 2023-04-09 20:52:07.000000 dfimagetools-20230409/docs/sources/api/dfimagetools.rst
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       73 2022-11-21 19:36:05.000000 dfimagetools-20230409/docs/sources/api/modules.rst
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.105284 dfimagetools-20230409/docs/sources/user/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1693 2022-11-21 19:36:05.000000 dfimagetools-20230409/docs/sources/user/Installation-instructions.md
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      296 2022-11-21 19:36:05.000000 dfimagetools-20230409/docs/sources/user/index.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      871 2023-04-09 14:48:22.000000 dfimagetools-20230409/requirements.txt
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1018 2022-10-02 12:20:49.000000 dfimagetools-20230409/run_tests.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1460 2023-04-09 20:55:44.133284 dfimagetools-20230409/setup.cfg
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6828 2023-04-09 14:48:22.000000 dfimagetools-20230409/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 18:36:28.000000 dfimagetools-20230409/test_dependencies.ini
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 14:48:22.000000 dfimagetools-20230409/test_requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.108284 dfimagetools-20230409/tests/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2021-12-21 09:32:11.000000 dfimagetools-20230409/tests/__init__.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7807 2022-04-30 13:22:39.000000 dfimagetools-20230409/tests/artifact_filters.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4034 2022-01-29 19:59:40.000000 dfimagetools-20230409/tests/bodyfile.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2291 2022-04-30 13:22:39.000000 dfimagetools-20230409/tests/environment_variables.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3293 2022-01-29 19:59:40.000000 dfimagetools-20230409/tests/file_entry_lister.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11717 2022-04-30 13:22:39.000000 dfimagetools-20230409/tests/path_resover.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      655 2022-12-23 10:46:53.000000 dfimagetools-20230409/tests/source_analyzer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2273 2022-10-02 12:20:49.000000 dfimagetools-20230409/tests/test_lib.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.122284 dfimagetools-20230409/tools/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       57 2021-12-21 09:32:11.000000 dfimagetools-20230409/tools/__init__.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     8865 2022-10-02 12:20:49.000000 dfimagetools-20230409/tools/extract_data_streams.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     8136 2022-12-18 20:43:00.000000 dfimagetools-20230409/tools/list_file_entries.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     5100 2022-10-02 12:20:49.000000 dfimagetools-20230409/tools/map_extents.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4465 2022-12-26 19:18:50.000000 dfimagetools-20230409/tools/recursive_hasher.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3866 2022-12-25 20:20:03.000000 dfimagetools-20230409/tools/source_analyzer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2023-04-09 14:48:22.000000 dfimagetools-20230409/tox.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 20:55:44.123284 dfimagetools-20230409/utils/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2021-12-21 09:32:11.000000 dfimagetools-20230409/utils/__init__.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2023-04-09 14:48:22.000000 dfimagetools-20230409/utils/check_dependencies.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2023-04-09 14:48:22.000000 dfimagetools-20230409/utils/dependencies.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      655 2022-04-30 13:22:18.000000 dfimagetools-20230409/utils/update_release.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.392297 dfimagetools-20230410/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.172296 dfimagetools-20230410/.github/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.304297 dfimagetools-20230410/.github/workflows/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3653 2023-04-10 06:21:28.000000 dfimagetools-20230410/.github/workflows/test_docker.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1938 2023-04-10 06:21:28.000000 dfimagetools-20230410/.github/workflows/test_docs.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2239 2023-04-10 06:21:28.000000 dfimagetools-20230410/.github/workflows/test_tox.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22101 2023-04-10 06:21:27.000000 dfimagetools-20230410/.pylintrc
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      149 2022-04-30 13:22:39.000000 dfimagetools-20230410/.yamllint.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      479 2022-04-30 13:22:39.000000 dfimagetools-20230410/ACKNOWLEDGEMENTS
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      292 2022-04-30 13:22:39.000000 dfimagetools-20230410/AUTHORS
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2021-10-31 13:10:45.000000 dfimagetools-20230410/LICENSE
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      608 2022-01-29 19:59:40.000000 dfimagetools-20230410/MANIFEST.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      528 2022-01-29 19:59:40.000000 dfimagetools-20230410/MANIFEST.test_data.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      566 2023-04-10 08:01:47.392297 dfimagetools-20230410/PKG-INFO
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      153 2021-12-26 07:38:07.000000 dfimagetools-20230410/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-04-10 06:21:28.000000 dfimagetools-20230410/appveyor.yml
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.173296 dfimagetools-20230410/config/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.305297 dfimagetools-20230410/config/appveyor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2023-04-10 06:21:28.000000 dfimagetools-20230410/config/appveyor/install.ps1
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2023-04-10 06:21:28.000000 dfimagetools-20230410/config/appveyor/install.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2023-04-10 06:21:28.000000 dfimagetools-20230410/config/appveyor/runtests.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.306296 dfimagetools-20230410/config/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      175 2023-04-10 08:00:49.000000 dfimagetools-20230410/config/dpkg/changelog
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       23 2021-12-23 07:30:27.000000 dfimagetools-20230410/config/dpkg/clean
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        2 2023-04-10 06:21:28.000000 dfimagetools-20230410/config/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1798 2023-04-10 06:21:28.000000 dfimagetools-20230410/config/dpkg/control
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      976 2021-12-26 07:38:07.000000 dfimagetools-20230410/config/dpkg/copyright
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        8 2021-12-26 07:38:07.000000 dfimagetools-20230410/config/dpkg/dfimagetools-tools.install
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      105 2021-12-26 07:38:07.000000 dfimagetools-20230410/config/dpkg/python3-dfimagetools.install
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2023-04-10 06:21:28.000000 dfimagetools-20230410/config/dpkg/rules
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.306296 dfimagetools-20230410/config/dpkg/source/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2021-12-23 07:30:27.000000 dfimagetools-20230410/config/dpkg/source/format
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.307297 dfimagetools-20230410/config/pylint/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      229 2021-12-21 12:01:47.000000 dfimagetools-20230410/config/pylint/spelling-private-dict
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5687 2022-09-03 04:58:03.000000 dfimagetools-20230410/dependencies.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.308297 dfimagetools-20230410/dfimagetools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      110 2023-04-10 08:00:49.000000 dfimagetools-20230410/dfimagetools/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4432 2022-10-02 12:20:49.000000 dfimagetools-20230410/dfimagetools/artifact_filters.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9053 2022-10-02 12:20:49.000000 dfimagetools-20230410/dfimagetools/bodyfile.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2022-10-02 12:20:49.000000 dfimagetools-20230410/dfimagetools/data_stream_writer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      710 2022-10-02 12:20:49.000000 dfimagetools-20230410/dfimagetools/decorators.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3493 2022-10-02 12:20:49.000000 dfimagetools-20230410/dfimagetools/environment_variables.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6866 2022-10-02 12:20:49.000000 dfimagetools-20230410/dfimagetools/file_entry_lister.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2022-09-03 04:58:03.000000 dfimagetools-20230410/dfimagetools/helpers.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11121 2022-10-02 12:20:49.000000 dfimagetools-20230410/dfimagetools/path_resolver.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4304 2022-12-26 19:18:50.000000 dfimagetools-20230410/dfimagetools/recursive_hasher.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2362 2022-04-30 13:22:39.000000 dfimagetools-20230410/dfimagetools/resources.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2861 2022-12-26 04:50:18.000000 dfimagetools-20230410/dfimagetools/source_analyzer.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6222 2022-04-30 13:22:39.000000 dfimagetools-20230410/dfimagetools/windows_registry.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.309296 dfimagetools-20230410/dfimagetools.egg-info/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      566 2023-04-10 08:01:46.000000 dfimagetools-20230410/dfimagetools.egg-info/PKG-INFO
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1905 2023-04-10 08:01:47.000000 dfimagetools-20230410/dfimagetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2023-04-10 08:01:46.000000 dfimagetools-20230410/dfimagetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      834 2023-04-10 08:01:46.000000 dfimagetools-20230410/dfimagetools.egg-info/requires.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       13 2023-04-10 08:01:46.000000 dfimagetools-20230410/dfimagetools.egg-info/top_level.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      388 2021-12-26 07:38:07.000000 dfimagetools-20230410/dfimagetools.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.317297 dfimagetools-20230410/docs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2023-04-10 06:21:28.000000 dfimagetools-20230410/docs/conf.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      528 2022-11-21 19:36:05.000000 dfimagetools-20230410/docs/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      105 2023-04-10 06:21:38.000000 dfimagetools-20230410/docs/requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.317297 dfimagetools-20230410/docs/sources/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2022-12-18 20:43:00.000000 dfimagetools-20230410/docs/sources/Bodyfile-format.md
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.348296 dfimagetools-20230410/docs/sources/api/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2236 2023-04-09 20:52:07.000000 dfimagetools-20230410/docs/sources/api/dfimagetools.rst
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       73 2022-11-21 19:36:05.000000 dfimagetools-20230410/docs/sources/api/modules.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.375296 dfimagetools-20230410/docs/sources/user/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1693 2022-11-21 19:36:05.000000 dfimagetools-20230410/docs/sources/user/Installation-instructions.md
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      296 2022-11-21 19:36:05.000000 dfimagetools-20230410/docs/sources/user/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      902 2023-04-10 08:00:49.000000 dfimagetools-20230410/requirements.txt
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1018 2022-10-02 12:20:49.000000 dfimagetools-20230410/run_tests.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1460 2023-04-10 08:01:47.393297 dfimagetools-20230410/setup.cfg
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6828 2023-04-10 06:21:28.000000 dfimagetools-20230410/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 18:36:28.000000 dfimagetools-20230410/test_dependencies.ini
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 06:21:27.000000 dfimagetools-20230410/test_requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.376297 dfimagetools-20230410/tests/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2021-12-21 09:32:11.000000 dfimagetools-20230410/tests/__init__.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7807 2022-04-30 13:22:39.000000 dfimagetools-20230410/tests/artifact_filters.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4034 2022-01-29 19:59:40.000000 dfimagetools-20230410/tests/bodyfile.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2291 2022-04-30 13:22:39.000000 dfimagetools-20230410/tests/environment_variables.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3293 2022-01-29 19:59:40.000000 dfimagetools-20230410/tests/file_entry_lister.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11717 2022-04-30 13:22:39.000000 dfimagetools-20230410/tests/path_resover.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      655 2022-12-23 10:46:53.000000 dfimagetools-20230410/tests/source_analyzer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2273 2022-10-02 12:20:49.000000 dfimagetools-20230410/tests/test_lib.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.391296 dfimagetools-20230410/tools/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       57 2021-12-21 09:32:11.000000 dfimagetools-20230410/tools/__init__.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     8865 2022-10-02 12:20:49.000000 dfimagetools-20230410/tools/extract_data_streams.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     8136 2022-12-18 20:43:00.000000 dfimagetools-20230410/tools/list_file_entries.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     5100 2022-10-02 12:20:49.000000 dfimagetools-20230410/tools/map_extents.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4465 2022-12-26 19:18:50.000000 dfimagetools-20230410/tools/recursive_hasher.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3866 2022-12-25 20:20:03.000000 dfimagetools-20230410/tools/source_analyzer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2023-04-10 06:21:28.000000 dfimagetools-20230410/tox.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.392297 dfimagetools-20230410/utils/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2021-12-21 09:32:11.000000 dfimagetools-20230410/utils/__init__.py
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2023-04-10 06:21:28.000000 dfimagetools-20230410/utils/check_dependencies.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2023-04-10 06:21:28.000000 dfimagetools-20230410/utils/dependencies.py
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      655 2022-04-30 13:22:18.000000 dfimagetools-20230410/utils/update_release.sh
```

### Comparing `dfimagetools-20230409/.github/workflows/test_docker.yml` & `dfimagetools-20230410/.github/workflows/test_docker.yml`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/.github/workflows/test_docs.yml` & `dfimagetools-20230410/.github/workflows/test_docs.yml`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/.github/workflows/test_tox.yml` & `dfimagetools-20230410/.github/workflows/test_tox.yml`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/.pylintrc` & `dfimagetools-20230410/.pylintrc`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/LICENSE` & `dfimagetools-20230410/LICENSE`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/MANIFEST.in` & `dfimagetools-20230410/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/MANIFEST.test_data.in` & `dfimagetools-20230410/MANIFEST.test_data.in`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/PKG-INFO` & `dfimagetools-20230410/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfimagetools
-Version: 20230409
+Version: 20230410
 Summary: Storage media image tools
 Home-page: https://github.com/log2timeline/dfimagetools
 Maintainer: Log2Timeline maintainers
 Maintainer-email: log2timeline-maintainers@googlegroups.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `dfimagetools-20230409/appveyor.yml` & `dfimagetools-20230410/appveyor.yml`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/config/appveyor/install.ps1` & `dfimagetools-20230410/config/appveyor/install.ps1`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/config/appveyor/runtests.sh` & `dfimagetools-20230410/config/appveyor/runtests.sh`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/config/dpkg/control` & `dfimagetools-20230410/config/dpkg/control`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/config/dpkg/copyright` & `dfimagetools-20230410/config/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/dependencies.ini` & `dfimagetools-20230410/dependencies.ini`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/dfimagetools/artifact_filters.py` & `dfimagetools-20230410/dfimagetools/artifact_filters.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/dfimagetools/bodyfile.py` & `dfimagetools-20230410/dfimagetools/bodyfile.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/dfimagetools/data_stream_writer.py` & `dfimagetools-20230410/dfimagetools/data_stream_writer.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/dfimagetools/decorators.py` & `dfimagetools-20230410/dfimagetools/decorators.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/dfimagetools/environment_variables.py` & `dfimagetools-20230410/dfimagetools/environment_variables.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/dfimagetools/file_entry_lister.py` & `dfimagetools-20230410/dfimagetools/file_entry_lister.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/dfimagetools/helpers.py` & `dfimagetools-20230410/dfimagetools/helpers.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/dfimagetools/path_resolver.py` & `dfimagetools-20230410/dfimagetools/path_resolver.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/dfimagetools/recursive_hasher.py` & `dfimagetools-20230410/dfimagetools/recursive_hasher.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/dfimagetools/resources.py` & `dfimagetools-20230410/dfimagetools/resources.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/dfimagetools/source_analyzer.py` & `dfimagetools-20230410/dfimagetools/source_analyzer.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/dfimagetools/windows_registry.py` & `dfimagetools-20230410/dfimagetools/windows_registry.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/dfimagetools.egg-info/PKG-INFO` & `dfimagetools-20230410/dfimagetools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfimagetools
-Version: 20230409
+Version: 20230410
 Summary: Storage media image tools
 Home-page: https://github.com/log2timeline/dfimagetools
 Maintainer: Log2Timeline maintainers
 Maintainer-email: log2timeline-maintainers@googlegroups.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `dfimagetools-20230409/dfimagetools.egg-info/SOURCES.txt` & `dfimagetools-20230410/dfimagetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/dfimagetools.egg-info/requires.txt` & `dfimagetools-20230410/dfimagetools.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -28,8 +28,10 @@
 libsmraw-python>=20140612
 libvhdi-python>=20201014
 libvmdk-python>=20140421
 libvsgpt-python>=20211115
 libvshadow-python>=20160109
 libvslvm-python>=20160109
 pytsk3>=20210419
+
+[:platform_system != "Windows"]
 pyxattr>=0.7.2
```

### Comparing `dfimagetools-20230409/docs/conf.py` & `dfimagetools-20230410/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/docs/index.rst` & `dfimagetools-20230410/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/docs/sources/Bodyfile-format.md` & `dfimagetools-20230410/docs/sources/Bodyfile-format.md`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/docs/sources/api/dfimagetools.rst` & `dfimagetools-20230410/docs/sources/api/dfimagetools.rst`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/docs/sources/user/Installation-instructions.md` & `dfimagetools-20230410/docs/sources/user/Installation-instructions.md`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/requirements.txt` & `dfimagetools-20230410/requirements.txt`

 * *Files 15% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 libsmraw-python >= 20140612
 libvhdi-python >= 20201014
 libvmdk-python >= 20140421
 libvsgpt-python >= 20211115
 libvshadow-python >= 20160109
 libvslvm-python >= 20160109
 pytsk3 >= 20210419
-pyxattr >= 0.7.2
+pyxattr >= 0.7.2 ; platform_system != "Windows"
```

### Comparing `dfimagetools-20230409/run_tests.py` & `dfimagetools-20230410/run_tests.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/setup.cfg` & `dfimagetools-20230410/setup.cfg`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/setup.py` & `dfimagetools-20230410/setup.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/tests/artifact_filters.py` & `dfimagetools-20230410/tests/artifact_filters.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/tests/bodyfile.py` & `dfimagetools-20230410/tests/bodyfile.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/tests/environment_variables.py` & `dfimagetools-20230410/tests/environment_variables.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/tests/file_entry_lister.py` & `dfimagetools-20230410/tests/file_entry_lister.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/tests/path_resover.py` & `dfimagetools-20230410/tests/path_resover.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/tests/source_analyzer.py` & `dfimagetools-20230410/tests/source_analyzer.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/tests/test_lib.py` & `dfimagetools-20230410/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/tools/extract_data_streams.py` & `dfimagetools-20230410/tools/extract_data_streams.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/tools/list_file_entries.py` & `dfimagetools-20230410/tools/list_file_entries.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/tools/map_extents.py` & `dfimagetools-20230410/tools/map_extents.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/tools/recursive_hasher.py` & `dfimagetools-20230410/tools/recursive_hasher.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/tools/source_analyzer.py` & `dfimagetools-20230410/tools/source_analyzer.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/tox.ini` & `dfimagetools-20230410/tox.ini`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/utils/dependencies.py` & `dfimagetools-20230410/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230409/utils/update_release.sh` & `dfimagetools-20230410/utils/update_release.sh`

 * *Files identical despite different names*

