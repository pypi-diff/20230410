# Comparing `tmp/PyStorCLI2-0.6.0.tar.gz` & `tmp/PyStorCLI2-0.6.1.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyStorCLI2-0.6.0.tar", last modified: Tue Apr  4 12:30:44 2023, max compression
+gzip compressed data, was "PyStorCLI2-0.6.1.dev6.tar", last modified: Mon Apr 10 09:50:00 2023, max compression
```

## Comparing `PyStorCLI2-0.6.0.tar` & `PyStorCLI2-0.6.1.dev6.tar`

### file list

```diff
@@ -1,122 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.762486 PyStorCLI2-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.738486 PyStorCLI2-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.746486 PyStorCLI2-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.746486 PyStorCLI2-0.6.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-04 12:30:44.762486 PyStorCLI2-0.6.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.746486 PyStorCLI2-0.6.0/PyStorCLI2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-04 12:30:44.000000 PyStorCLI2-0.6.0/PyStorCLI2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-04 12:30:44.000000 PyStorCLI2-0.6.0/PyStorCLI2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 12:30:44.000000 PyStorCLI2-0.6.0/PyStorCLI2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-04 12:30:44.000000 PyStorCLI2-0.6.0/PyStorCLI2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-04 12:30:44.000000 PyStorCLI2-0.6.0/PyStorCLI2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-04 12:30:44.000000 PyStorCLI2-0.6.0/PyStorCLI2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.746486 PyStorCLI2-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-04 12:30:09.000000 PyStorCLI2-0.6.0/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (123)   750282 2023-04-04 12:30:09.000000 PyStorCLI2-0.6.0/docs/pystorcli2.html
--rw-r--r--   0 runner    (1001) docker     (123)   329997 2023-04-04 12:30:09.000000 PyStorCLI2-0.6.0/docs/search.js
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.750486 PyStorCLI2-0.6.0/pystorcli/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/pystorcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/pystorcli/cachevault.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/pystorcli/cmdRunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/pystorcli/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/pystorcli/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    26664 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/pystorcli/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/pystorcli/enclosure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/pystorcli/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/pystorcli/storcli.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-04 12:30:44.000000 PyStorCLI2-0.6.0/pystorcli/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/pystorcli/virtualdrive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.750486 PyStorCLI2-0.6.0/pystorcli2/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/pystorcli2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/pystorcli2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.750486 PyStorCLI2-0.6.0/pystorcli2/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/pystorcli2/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5262 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/pystorcli2/bin/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/pystorcli2/cachevault.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/pystorcli2/cmdRunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/pystorcli2/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/pystorcli2/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    26664 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/pystorcli2/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/pystorcli2/enclosure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/pystorcli2/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/pystorcli2/storcli.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-04 12:30:44.000000 PyStorCLI2-0.6.0/pystorcli2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/pystorcli2/virtualdrive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.750486 PyStorCLI2-0.6.0/pystorcli_mirror/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/pystorcli_mirror/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 12:30:44.762486 PyStorCLI2-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.754486 PyStorCLI2-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/baseTest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.742486 PyStorCLI2-0.6.0/tests/datatest/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.738486 PyStorCLI2-0.6.0/tests/datatest/controllerSet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.754486 PyStorCLI2-0.6.0/tests/datatest/controllerSet/test00/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/controllerSet/test00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/controllerSet/test00/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.754486 PyStorCLI2-0.6.0/tests/datatest/controllerSet/test01/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/controllerSet/test01/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/controllerSet/test01/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.754486 PyStorCLI2-0.6.0/tests/datatest/controllerSet/test02/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/controllerSet/test02/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/controllerSet/test02/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.754486 PyStorCLI2-0.6.0/tests/datatest/namedSet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.754486 PyStorCLI2-0.6.0/tests/datatest/namedSet/create_vd_raid0_00/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/create_vd_raid0_00/__c0_add_vd_r0_name=create_vd_raid0_drives=35_12-13_strip=512_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/create_vd_raid0_00/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/create_vd_raid0_00/__c0_v1_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/create_vd_raid0_00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/create_vd_raid0_00/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.758486 PyStorCLI2-0.6.0/tests/datatest/namedSet/create_vd_raid1_00/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/create_vd_raid1_00/__c0_add_vd_r1_name=create_vd_raid1_drives=35_12-13_strip=512_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/create_vd_raid1_00/__c0_add_vd_r1_name=create_vd_raid1_drives=35_12-13_strip=512_PDperArray=2_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/create_vd_raid1_00/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/create_vd_raid1_00/__c0_v1_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/create_vd_raid1_00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/create_vd_raid1_00/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.758486 PyStorCLI2-0.6.0/tests/datatest/namedSet/delete_vd_00/
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/delete_vd_00/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/delete_vd_00/__c0_v1_del_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/delete_vd_00/__c0_v1_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/delete_vd_00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/delete_vd_00/device.json
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.758486 PyStorCLI2-0.6.0/tests/datatest/namedSet/set_state_offline_00/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/set_state_offline_00/__c0_e35_s12_set_offline_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/set_state_offline_00/__c0_e35_s12_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/set_state_offline_00/__c0_e35_sall_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/set_state_offline_00/__c0_e35_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/set_state_offline_00/__c0_eall_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/set_state_offline_00/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/set_state_offline_00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/set_state_offline_00/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.762486 PyStorCLI2-0.6.0/tests/datatest/namedSet/show_events_00/
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/show_events_00/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/show_events_00/__c0_show_events_file=_root_raid_events.log_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/show_events_00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/show_events_00/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.762486 PyStorCLI2-0.6.0/tests/datatest/namedSet/spindown_disk_00/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/spindown_disk_00/__c0_e35_s12_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/spindown_disk_00/__c0_e35_s12_spindown_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/spindown_disk_00/__c0_e35_sall_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/spindown_disk_00/__c0_e35_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/spindown_disk_00/__c0_eall_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/spindown_disk_00/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/spindown_disk_00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/namedSet/spindown_disk_00/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.742486 PyStorCLI2-0.6.0/tests/datatest/storcliSet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.762486 PyStorCLI2-0.6.0/tests/datatest/storcliSet/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/datatest/storcliSet/dummy/device.json
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/storclifile.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/test_controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-04 12:29:51.000000 PyStorCLI2-0.6.0/tests/test_storcli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.841245 PyStorCLI2-0.6.1.dev6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.825245 PyStorCLI2-0.6.1.dev6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.829245 PyStorCLI2-0.6.1.dev6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.829245 PyStorCLI2-0.6.1.dev6/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-10 09:50:00.841245 PyStorCLI2-0.6.1.dev6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.829245 PyStorCLI2-0.6.1.dev6/PyStorCLI2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-10 09:50:00.000000 PyStorCLI2-0.6.1.dev6/PyStorCLI2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-10 09:50:00.000000 PyStorCLI2-0.6.1.dev6/PyStorCLI2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 09:50:00.000000 PyStorCLI2-0.6.1.dev6/PyStorCLI2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-10 09:50:00.000000 PyStorCLI2-0.6.1.dev6/PyStorCLI2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-10 09:50:00.000000 PyStorCLI2-0.6.1.dev6/PyStorCLI2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-10 09:50:00.000000 PyStorCLI2-0.6.1.dev6/PyStorCLI2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.833245 PyStorCLI2-0.6.1.dev6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-10 09:49:34.000000 PyStorCLI2-0.6.1.dev6/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)   751593 2023-04-10 09:49:34.000000 PyStorCLI2-0.6.1.dev6/docs/pystorcli2.html
+-rw-r--r--   0 runner    (1001) docker     (123)   331389 2023-04-10 09:49:34.000000 PyStorCLI2-0.6.1.dev6/docs/search.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.833245 PyStorCLI2-0.6.1.dev6/pystorcli/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli/cachevault.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli/cmdRunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11885 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26664 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli/enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli/storcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-10 09:50:00.000000 PyStorCLI2-0.6.1.dev6/pystorcli/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli/virtualdrive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.833245 PyStorCLI2-0.6.1.dev6/pystorcli2/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.833245 PyStorCLI2-0.6.1.dev6/pystorcli2/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5262 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/bin/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/cachevault.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/cmdRunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11885 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26664 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/storcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-10 09:50:00.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/virtualdrive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.833245 PyStorCLI2-0.6.1.dev6/pystorcli_mirror/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli_mirror/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 09:50:00.841245 PyStorCLI2-0.6.1.dev6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.837245 PyStorCLI2-0.6.1.dev6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/baseTest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.829245 PyStorCLI2-0.6.1.dev6/tests/datatest/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.829245 PyStorCLI2-0.6.1.dev6/tests/datatest/controllerSet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.837245 PyStorCLI2-0.6.1.dev6/tests/datatest/controllerSet/test00/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/controllerSet/test00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/controllerSet/test00/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.837245 PyStorCLI2-0.6.1.dev6/tests/datatest/controllerSet/test01/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/controllerSet/test01/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/controllerSet/test01/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.837245 PyStorCLI2-0.6.1.dev6/tests/datatest/controllerSet/test02/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/controllerSet/test02/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/controllerSet/test02/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.837245 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.837245 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid0_00/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid0_00/__c0_add_vd_r0_name=create_vd_raid0_drives=35_12-13_strip=512_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid0_00/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid0_00/__c0_v1_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid0_00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid0_00/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.837245 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid1_00/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid1_00/__c0_add_vd_r1_name=create_vd_raid1_drives=35_12-13_strip=512_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid1_00/__c0_add_vd_r1_name=create_vd_raid1_drives=35_12-13_strip=512_PDperArray=2_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid1_00/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid1_00/__c0_v1_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid1_00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid1_00/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.837245 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/delete_vd_00/
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/delete_vd_00/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/delete_vd_00/__c0_v1_del_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/delete_vd_00/__c0_v1_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/delete_vd_00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/delete_vd_00/device.json
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.841245 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/__c0_e35_s12_set_offline_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/__c0_e35_s12_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/__c0_e35_sall_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/__c0_e35_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/__c0_eall_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.841245 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/show_events_00/
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/show_events_00/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/show_events_00/__c0_show_events_file=_root_raid_events.log_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/show_events_00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/show_events_00/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.841245 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/__c0_e35_s12_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/__c0_e35_s12_spindown_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/__c0_e35_sall_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/__c0_e35_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/__c0_eall_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.829245 PyStorCLI2-0.6.1.dev6/tests/datatest/storcliSet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.841245 PyStorCLI2-0.6.1.dev6/tests/datatest/storcliSet/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/storcliSet/dummy/device.json
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/storclifile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/test_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/test_storcli.py
```

### Comparing `PyStorCLI2-0.6.0/.github/workflows/check.yml` & `PyStorCLI2-0.6.1.dev6/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/.github/workflows/publish-to-pypi.yml` & `PyStorCLI2-0.6.1.dev6/.github/workflows/publish-to-pypi.yml`

 * *Files 13% similar despite different names*

```diff
@@ -48,11 +48,11 @@
           python -m
           build
           --sdist
           --wheel
           --outdir dist/
           .
       - name: Publish distribution 📦 to PyPI
-        if: startsWith(github.ref, 'refs/tags')
+        if: startsWith(github.ref, 'refs/tags') || github.ref == 'refs/heads/master'
         uses: pypa/gh-action-pypi-publish@master
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `PyStorCLI2-0.6.0/CHANGELOG.md` & `PyStorCLI2-0.6.1.dev6/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Version 0.6.1
+=============
+
+- **New features**:
+  -----------------
+  - [**Controller**]        Added method drives_ids to get all pair of enclosure:drive_id
+
+- **Fixes**:
+  ----------
+  - [**Controller**]        Fixed device count on controller.create_vd. Requested in [#2](https://github.com/Naudit/pystorcli2/issues/2)
+  - [**Controller**]        Fixed default pd on controller.create_vd in some scenarios. Requested in [#2](https://github.com/Naudit/pystorcli2/issues/2)
+
 Version 0.6.0
 =============
 
 - **New features**:
   -----------------
     - Added enclosures, drives and virtualdrives to main __init__.py
     - Increased test coverage
```

### Comparing `PyStorCLI2-0.6.0/LICENSE` & `PyStorCLI2-0.6.1.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/PKG-INFO` & `PyStorCLI2-0.6.1.dev6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyStorCLI2
-Version: 0.6.0
+Version: 0.6.1.dev6
 Summary: StorCLI module wrapper 2
 Author-email: Rafael Leira <rafael.leira@naudit.es>, Martin Dojcak <martin.dojcak@lablabs.io>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/Naudit/pystorcli2
 Keywords: storcli,wrapper
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
@@ -23,13 +23,14 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # PyStorCLI2
 
 [![Coverage Status Master](https://coveralls.io/repos/github/Naudit/pystorcli2/badge.svg?branch=master)](https://coveralls.io/github/Naudit/pystorcli2?branch=master)
 ![Coveralls branch](https://img.shields.io/coverallsCoverage/github/Naudit/pystorcli2?branch=develop&label=coverage%20on%20develop&logo=coveralls)
+[![Downloads](https://static.pepy.tech/personalized-badge/pystorcli2?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/month)](https://pepy.tech/project/pystorcli2)
 
 PyStorCLI2 official fork from [pystorcli](https://github.com/Chillisystems/pystorcli).
 
 # How to use PyStorCLI2:
 
 FIXME: create useful readme
```

### Comparing `PyStorCLI2-0.6.0/PyStorCLI2.egg-info/PKG-INFO` & `PyStorCLI2-0.6.1.dev6/PyStorCLI2.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyStorCLI2
-Version: 0.6.0
+Version: 0.6.1.dev6
 Summary: StorCLI module wrapper 2
 Author-email: Rafael Leira <rafael.leira@naudit.es>, Martin Dojcak <martin.dojcak@lablabs.io>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/Naudit/pystorcli2
 Keywords: storcli,wrapper
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
@@ -23,13 +23,14 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # PyStorCLI2
 
 [![Coverage Status Master](https://coveralls.io/repos/github/Naudit/pystorcli2/badge.svg?branch=master)](https://coveralls.io/github/Naudit/pystorcli2?branch=master)
 ![Coveralls branch](https://img.shields.io/coverallsCoverage/github/Naudit/pystorcli2?branch=develop&label=coverage%20on%20develop&logo=coveralls)
+[![Downloads](https://static.pepy.tech/personalized-badge/pystorcli2?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/month)](https://pepy.tech/project/pystorcli2)
 
 PyStorCLI2 official fork from [pystorcli](https://github.com/Chillisystems/pystorcli).
 
 # How to use PyStorCLI2:
 
 FIXME: create useful readme
```

### Comparing `PyStorCLI2-0.6.0/PyStorCLI2.egg-info/SOURCES.txt` & `PyStorCLI2-0.6.1.dev6/PyStorCLI2.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 pystorcli2/bin/__init__.py
 pystorcli2/bin/metrics.py
 pystorcli_mirror/__init__.py
 tests/__init__.py
 tests/baseTest.py
 tests/exceptions.py
 tests/storclifile.py
+tests/test_common.py
 tests/test_controllers.py
 tests/test_operations.py
 tests/test_storcli.py
 tests/datatest/controllerSet/test00/_show_J.json
 tests/datatest/controllerSet/test00/device.json
 tests/datatest/controllerSet/test01/_show_J.json
 tests/datatest/controllerSet/test01/device.json
```

### Comparing `PyStorCLI2-0.6.0/docs/pystorcli2.html` & `PyStorCLI2-0.6.1.dev6/docs/pystorcli2.html`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,17 @@
                         <li>
                                 <a class="variable" href="#Controller.vds">vds</a>
                         </li>
                         <li>
                                 <a class="variable" href="#Controller.encls">encls</a>
                         </li>
                         <li>
+                                <a class="variable" href="#Controller.drives_ids">drives_ids</a>
+                        </li>
+                        <li>
                                 <a class="function" href="#Controller.create_vd">create_vd</a>
                         </li>
                 </ul>
 
             </li>
             <li>
                     <a class="class" href="#Controllers">Controllers</a>
@@ -550,15 +553,15 @@
 </span></pre></div>
 
 
             </section>
                 <section id="__version__">
                     <div class="attr variable">
             <span class="name">__version__</span>        =
-<span class="default_value">&#39;0.6.0&#39;</span>
+<span class="default_value">&#39;0.6.1.dev6&#39;</span>
 
         
     </div>
     <a class="headerlink" href="#__version__"></a>
     
     
 
@@ -1347,67 +1350,77 @@
 </span><span id="Controller-272"><a href="#Controller-272"><span class="linenos">272</span></a>
 </span><span id="Controller-273"><a href="#Controller-273"><span class="linenos">273</span></a>    <span class="nd">@property</span>
 </span><span id="Controller-274"><a href="#Controller-274"><span class="linenos">274</span></a>    <span class="k">def</span> <span class="nf">encls</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
 </span><span id="Controller-275"><a href="#Controller-275"><span class="linenos">275</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;(:obj:enclosure.Enclosures): controller enclosures</span>
 </span><span id="Controller-276"><a href="#Controller-276"><span class="linenos">276</span></a><span class="sd">        &quot;&quot;&quot;</span>
 </span><span id="Controller-277"><a href="#Controller-277"><span class="linenos">277</span></a>        <span class="k">return</span> <span class="n">enclosure</span><span class="o">.</span><span class="n">Enclosures</span><span class="p">(</span><span class="n">ctl_id</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_ctl_id</span><span class="p">,</span> <span class="n">binary</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_binary</span><span class="p">)</span>
 </span><span id="Controller-278"><a href="#Controller-278"><span class="linenos">278</span></a>
-</span><span id="Controller-279"><a href="#Controller-279"><span class="linenos">279</span></a>    <span class="k">def</span> <span class="nf">create_vd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">raid</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">drives</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">strip</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;64&#39;</span><span class="p">,</span> <span class="n">PDperArray</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">int</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Optional</span><span class="p">[</span><span class="n">virtualdrive</span><span class="o">.</span><span class="n">VirtualDrive</span><span class="p">]:</span>
-</span><span id="Controller-280"><a href="#Controller-280"><span class="linenos">280</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Create virtual drive (raid) managed by current controller</span>
-</span><span id="Controller-281"><a href="#Controller-281"><span class="linenos">281</span></a>
-</span><span id="Controller-282"><a href="#Controller-282"><span class="linenos">282</span></a><span class="sd">        Args:</span>
-</span><span id="Controller-283"><a href="#Controller-283"><span class="linenos">283</span></a><span class="sd">            name (str): virtual drive name</span>
-</span><span id="Controller-284"><a href="#Controller-284"><span class="linenos">284</span></a><span class="sd">            raid (str): virtual drive raid level (raid0, raid1, ...)</span>
-</span><span id="Controller-285"><a href="#Controller-285"><span class="linenos">285</span></a><span class="sd">            drives (str): storcli drives expression (e:s|e:s-x|e:s-x,y;e:s-x,y,z)</span>
-</span><span id="Controller-286"><a href="#Controller-286"><span class="linenos">286</span></a><span class="sd">            strip (str, optional): virtual drive raid strip size</span>
+</span><span id="Controller-279"><a href="#Controller-279"><span class="linenos">279</span></a>    <span class="nd">@property</span>
+</span><span id="Controller-280"><a href="#Controller-280"><span class="linenos">280</span></a>    <span class="k">def</span> <span class="nf">drives_ids</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">List</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="Controller-281"><a href="#Controller-281"><span class="linenos">281</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;(list of str): list of drives ids in format (e:s)</span>
+</span><span id="Controller-282"><a href="#Controller-282"><span class="linenos">282</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Controller-283"><a href="#Controller-283"><span class="linenos">283</span></a>        <span class="n">drives</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="Controller-284"><a href="#Controller-284"><span class="linenos">284</span></a>        <span class="k">for</span> <span class="n">encl</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">encls</span><span class="p">:</span>
+</span><span id="Controller-285"><a href="#Controller-285"><span class="linenos">285</span></a>            <span class="k">for</span> <span class="nb">id</span> <span class="ow">in</span> <span class="n">encl</span><span class="o">.</span><span class="n">drives</span><span class="o">.</span><span class="n">ids</span><span class="p">:</span>
+</span><span id="Controller-286"><a href="#Controller-286"><span class="linenos">286</span></a>                <span class="n">drives</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">{enc}</span><span class="s2">:</span><span class="si">{id}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">enc</span><span class="o">=</span><span class="n">encl</span><span class="o">.</span><span class="n">id</span><span class="p">,</span> <span class="nb">id</span><span class="o">=</span><span class="nb">id</span><span class="p">))</span>
 </span><span id="Controller-287"><a href="#Controller-287"><span class="linenos">287</span></a>
-</span><span id="Controller-288"><a href="#Controller-288"><span class="linenos">288</span></a><span class="sd">        Returns:</span>
-</span><span id="Controller-289"><a href="#Controller-289"><span class="linenos">289</span></a><span class="sd">            (None): no virtual drive created with name</span>
-</span><span id="Controller-290"><a href="#Controller-290"><span class="linenos">290</span></a><span class="sd">            (:obj:virtualdrive.VirtualDrive)</span>
-</span><span id="Controller-291"><a href="#Controller-291"><span class="linenos">291</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller-292"><a href="#Controller-292"><span class="linenos">292</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Controller-293"><a href="#Controller-293"><span class="linenos">293</span></a>            <span class="s1">&#39;add&#39;</span><span class="p">,</span>
-</span><span id="Controller-294"><a href="#Controller-294"><span class="linenos">294</span></a>            <span class="s1">&#39;vd&#39;</span><span class="p">,</span>
-</span><span id="Controller-295"><a href="#Controller-295"><span class="linenos">295</span></a>            <span class="s1">&#39;r</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">raid</span><span class="p">),</span>
-</span><span id="Controller-296"><a href="#Controller-296"><span class="linenos">296</span></a>            <span class="s1">&#39;name=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">name</span><span class="p">),</span>
-</span><span id="Controller-297"><a href="#Controller-297"><span class="linenos">297</span></a>            <span class="s1">&#39;drives=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">drives</span><span class="p">),</span>
-</span><span id="Controller-298"><a href="#Controller-298"><span class="linenos">298</span></a>            <span class="s1">&#39;strip=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">strip</span><span class="p">)</span>
-</span><span id="Controller-299"><a href="#Controller-299"><span class="linenos">299</span></a>        <span class="p">]</span>
-</span><span id="Controller-300"><a href="#Controller-300"><span class="linenos">300</span></a>
-</span><span id="Controller-301"><a href="#Controller-301"><span class="linenos">301</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="Controller-302"><a href="#Controller-302"><span class="linenos">302</span></a>            <span class="k">if</span> <span class="nb">int</span><span class="p">(</span><span class="n">raid</span><span class="p">)</span> <span class="o">&gt;=</span> <span class="mi">10</span> <span class="ow">and</span> <span class="n">PDperArray</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Controller-303"><a href="#Controller-303"><span class="linenos">303</span></a>                <span class="c1"># Try to count the number of drives in the array</span>
-</span><span id="Controller-304"><a href="#Controller-304"><span class="linenos">304</span></a>                <span class="c1"># The format of the drives argument is e:s|e:s-x|e:s-x,y;e:s-x,y,z</span>
-</span><span id="Controller-305"><a href="#Controller-305"><span class="linenos">305</span></a>                <span class="c1"># The number of drives is the number of commas plus the dashes intervals</span>
-</span><span id="Controller-306"><a href="#Controller-306"><span class="linenos">306</span></a>
-</span><span id="Controller-307"><a href="#Controller-307"><span class="linenos">307</span></a>                <span class="n">numDrives</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="Controller-308"><a href="#Controller-308"><span class="linenos">308</span></a>                <span class="n">drives2</span> <span class="o">=</span> <span class="n">drives</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s1">&#39;:&#39;</span><span class="p">)</span>
-</span><span id="Controller-309"><a href="#Controller-309"><span class="linenos">309</span></a>                <span class="n">drives2</span> <span class="o">=</span> <span class="n">drives2</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span>
-</span><span id="Controller-310"><a href="#Controller-310"><span class="linenos">310</span></a>                <span class="n">numDrives</span> <span class="o">+=</span> <span class="n">drives2</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="s1">&#39;,&#39;</span><span class="p">)</span><span class="o">+</span><span class="mi">1</span>
-</span><span id="Controller-311"><a href="#Controller-311"><span class="linenos">311</span></a>                <span class="k">for</span> <span class="n">interval</span> <span class="ow">in</span> <span class="n">drives2</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s1">&#39;,&#39;</span><span class="p">):</span>
-</span><span id="Controller-312"><a href="#Controller-312"><span class="linenos">312</span></a>                    <span class="k">if</span> <span class="s1">&#39;-&#39;</span> <span class="ow">in</span> <span class="n">interval</span><span class="p">:</span>
-</span><span id="Controller-313"><a href="#Controller-313"><span class="linenos">313</span></a>                        <span class="n">left</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">interval</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s1">&#39;-&#39;</span><span class="p">)[</span><span class="mi">0</span><span class="p">])</span>
-</span><span id="Controller-314"><a href="#Controller-314"><span class="linenos">314</span></a>                        <span class="n">right</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">interval</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s1">&#39;-&#39;</span><span class="p">)[</span><span class="mi">1</span><span class="p">])</span>
-</span><span id="Controller-315"><a href="#Controller-315"><span class="linenos">315</span></a>                        <span class="n">numDrives</span> <span class="o">+=</span> <span class="n">right</span> <span class="o">-</span> <span class="n">left</span>
+</span><span id="Controller-288"><a href="#Controller-288"><span class="linenos">288</span></a>        <span class="k">return</span> <span class="n">drives</span>
+</span><span id="Controller-289"><a href="#Controller-289"><span class="linenos">289</span></a>
+</span><span id="Controller-290"><a href="#Controller-290"><span class="linenos">290</span></a>    <span class="k">def</span> <span class="nf">create_vd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">raid</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">drives</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">strip</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;64&#39;</span><span class="p">,</span> <span class="n">PDperArray</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">int</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Optional</span><span class="p">[</span><span class="n">virtualdrive</span><span class="o">.</span><span class="n">VirtualDrive</span><span class="p">]:</span>
+</span><span id="Controller-291"><a href="#Controller-291"><span class="linenos">291</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Create virtual drive (raid) managed by current controller</span>
+</span><span id="Controller-292"><a href="#Controller-292"><span class="linenos">292</span></a>
+</span><span id="Controller-293"><a href="#Controller-293"><span class="linenos">293</span></a><span class="sd">        Args:</span>
+</span><span id="Controller-294"><a href="#Controller-294"><span class="linenos">294</span></a><span class="sd">            name (str): virtual drive name</span>
+</span><span id="Controller-295"><a href="#Controller-295"><span class="linenos">295</span></a><span class="sd">            raid (str): virtual drive raid level (raid0, raid1, ...)</span>
+</span><span id="Controller-296"><a href="#Controller-296"><span class="linenos">296</span></a><span class="sd">            drives (str): storcli drives expression (e:s|e:s-x|e:s-x,y;e:s-x,y,z)</span>
+</span><span id="Controller-297"><a href="#Controller-297"><span class="linenos">297</span></a><span class="sd">            strip (str, optional): virtual drive raid strip size</span>
+</span><span id="Controller-298"><a href="#Controller-298"><span class="linenos">298</span></a>
+</span><span id="Controller-299"><a href="#Controller-299"><span class="linenos">299</span></a><span class="sd">        Returns:</span>
+</span><span id="Controller-300"><a href="#Controller-300"><span class="linenos">300</span></a><span class="sd">            (None): no virtual drive created with name</span>
+</span><span id="Controller-301"><a href="#Controller-301"><span class="linenos">301</span></a><span class="sd">            (:obj:virtualdrive.VirtualDrive)</span>
+</span><span id="Controller-302"><a href="#Controller-302"><span class="linenos">302</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Controller-303"><a href="#Controller-303"><span class="linenos">303</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="Controller-304"><a href="#Controller-304"><span class="linenos">304</span></a>            <span class="s1">&#39;add&#39;</span><span class="p">,</span>
+</span><span id="Controller-305"><a href="#Controller-305"><span class="linenos">305</span></a>            <span class="s1">&#39;vd&#39;</span><span class="p">,</span>
+</span><span id="Controller-306"><a href="#Controller-306"><span class="linenos">306</span></a>            <span class="s1">&#39;r</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">raid</span><span class="p">),</span>
+</span><span id="Controller-307"><a href="#Controller-307"><span class="linenos">307</span></a>            <span class="s1">&#39;name=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">name</span><span class="p">),</span>
+</span><span id="Controller-308"><a href="#Controller-308"><span class="linenos">308</span></a>            <span class="s1">&#39;drives=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">drives</span><span class="p">),</span>
+</span><span id="Controller-309"><a href="#Controller-309"><span class="linenos">309</span></a>            <span class="s1">&#39;strip=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">strip</span><span class="p">)</span>
+</span><span id="Controller-310"><a href="#Controller-310"><span class="linenos">310</span></a>        <span class="p">]</span>
+</span><span id="Controller-311"><a href="#Controller-311"><span class="linenos">311</span></a>
+</span><span id="Controller-312"><a href="#Controller-312"><span class="linenos">312</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="Controller-313"><a href="#Controller-313"><span class="linenos">313</span></a>            <span class="k">if</span> <span class="nb">int</span><span class="p">(</span><span class="n">raid</span><span class="p">)</span> <span class="o">&gt;=</span> <span class="mi">10</span> <span class="ow">and</span> <span class="n">PDperArray</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Controller-314"><a href="#Controller-314"><span class="linenos">314</span></a>                <span class="c1"># Try to count the number of drives in the array</span>
+</span><span id="Controller-315"><a href="#Controller-315"><span class="linenos">315</span></a>                <span class="c1"># The format of the drives argument is e:s|e:s-x|e:s-x,y;e:s-x,y,z</span>
 </span><span id="Controller-316"><a href="#Controller-316"><span class="linenos">316</span></a>
-</span><span id="Controller-317"><a href="#Controller-317"><span class="linenos">317</span></a>                <span class="n">PDperArray</span> <span class="o">=</span> <span class="n">numDrives</span><span class="o">//</span><span class="mi">2</span>
-</span><span id="Controller-318"><a href="#Controller-318"><span class="linenos">318</span></a>        <span class="k">except</span> <span class="ne">ValueError</span><span class="p">:</span>
-</span><span id="Controller-319"><a href="#Controller-319"><span class="linenos">319</span></a>            <span class="k">pass</span>
-</span><span id="Controller-320"><a href="#Controller-320"><span class="linenos">320</span></a>
-</span><span id="Controller-321"><a href="#Controller-321"><span class="linenos">321</span></a>        <span class="k">if</span> <span class="n">raid</span> <span class="o">==</span> <span class="s1">&#39;00&#39;</span> <span class="ow">and</span> <span class="n">PDperArray</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Controller-322"><a href="#Controller-322"><span class="linenos">322</span></a>            <span class="n">PDperArray</span> <span class="o">=</span> <span class="mi">1</span>
-</span><span id="Controller-323"><a href="#Controller-323"><span class="linenos">323</span></a>
-</span><span id="Controller-324"><a href="#Controller-324"><span class="linenos">324</span></a>        <span class="k">if</span> <span class="n">PDperArray</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Controller-325"><a href="#Controller-325"><span class="linenos">325</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;PDperArray=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">PDperArray</span><span class="p">))</span>
+</span><span id="Controller-317"><a href="#Controller-317"><span class="linenos">317</span></a>                <span class="n">numDrives</span> <span class="o">=</span> <span class="n">common</span><span class="o">.</span><span class="n">count_drives</span><span class="p">(</span><span class="n">drives</span><span class="p">)</span>
+</span><span id="Controller-318"><a href="#Controller-318"><span class="linenos">318</span></a>
+</span><span id="Controller-319"><a href="#Controller-319"><span class="linenos">319</span></a>                <span class="k">if</span> <span class="n">numDrives</span> <span class="o">%</span> <span class="mi">2</span> <span class="o">!=</span> <span class="mi">0</span> <span class="ow">and</span> <span class="n">numDrives</span> <span class="o">%</span> <span class="mi">3</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="Controller-320"><a href="#Controller-320"><span class="linenos">320</span></a>                    <span class="c1"># In some scenarios, such as 9 drives with raid 60, 3 is a good pd number but 4 is not</span>
+</span><span id="Controller-321"><a href="#Controller-321"><span class="linenos">321</span></a>                    <span class="c1"># Must check for similar scenarios</span>
+</span><span id="Controller-322"><a href="#Controller-322"><span class="linenos">322</span></a>                    <span class="c1"># BTW we don&#39;t clearly understand what PDperArray is for and what exactly it does under the hood. More investigation is needed</span>
+</span><span id="Controller-323"><a href="#Controller-323"><span class="linenos">323</span></a>                    <span class="n">PDperArray</span> <span class="o">=</span> <span class="n">numDrives</span><span class="o">//</span><span class="mi">3</span>
+</span><span id="Controller-324"><a href="#Controller-324"><span class="linenos">324</span></a>                <span class="k">else</span><span class="p">:</span>
+</span><span id="Controller-325"><a href="#Controller-325"><span class="linenos">325</span></a>                    <span class="n">PDperArray</span> <span class="o">=</span> <span class="n">numDrives</span><span class="o">//</span><span class="mi">2</span>
 </span><span id="Controller-326"><a href="#Controller-326"><span class="linenos">326</span></a>
-</span><span id="Controller-327"><a href="#Controller-327"><span class="linenos">327</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="Controller-328"><a href="#Controller-328"><span class="linenos">328</span></a>        <span class="k">for</span> <span class="n">vd</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">vds</span><span class="p">:</span>
-</span><span id="Controller-329"><a href="#Controller-329"><span class="linenos">329</span></a>            <span class="k">if</span> <span class="n">name</span> <span class="o">==</span> <span class="n">vd</span><span class="o">.</span><span class="n">name</span><span class="p">:</span>
-</span><span id="Controller-330"><a href="#Controller-330"><span class="linenos">330</span></a>                <span class="k">return</span> <span class="n">vd</span>
-</span><span id="Controller-331"><a href="#Controller-331"><span class="linenos">331</span></a>        <span class="k">return</span> <span class="kc">None</span>
+</span><span id="Controller-327"><a href="#Controller-327"><span class="linenos">327</span></a>        <span class="k">except</span> <span class="ne">ValueError</span><span class="p">:</span>
+</span><span id="Controller-328"><a href="#Controller-328"><span class="linenos">328</span></a>            <span class="k">pass</span>
+</span><span id="Controller-329"><a href="#Controller-329"><span class="linenos">329</span></a>
+</span><span id="Controller-330"><a href="#Controller-330"><span class="linenos">330</span></a>        <span class="k">finally</span><span class="p">:</span>
+</span><span id="Controller-331"><a href="#Controller-331"><span class="linenos">331</span></a>            <span class="k">if</span> <span class="n">raid</span> <span class="o">==</span> <span class="s1">&#39;00&#39;</span> <span class="ow">and</span> <span class="n">PDperArray</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Controller-332"><a href="#Controller-332"><span class="linenos">332</span></a>                <span class="n">PDperArray</span> <span class="o">=</span> <span class="mi">1</span>
+</span><span id="Controller-333"><a href="#Controller-333"><span class="linenos">333</span></a>
+</span><span id="Controller-334"><a href="#Controller-334"><span class="linenos">334</span></a>        <span class="k">if</span> <span class="n">PDperArray</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Controller-335"><a href="#Controller-335"><span class="linenos">335</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;PDperArray=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">PDperArray</span><span class="p">))</span>
+</span><span id="Controller-336"><a href="#Controller-336"><span class="linenos">336</span></a>
+</span><span id="Controller-337"><a href="#Controller-337"><span class="linenos">337</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="Controller-338"><a href="#Controller-338"><span class="linenos">338</span></a>        <span class="k">for</span> <span class="n">vd</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">vds</span><span class="p">:</span>
+</span><span id="Controller-339"><a href="#Controller-339"><span class="linenos">339</span></a>            <span class="k">if</span> <span class="n">name</span> <span class="o">==</span> <span class="n">vd</span><span class="o">.</span><span class="n">name</span><span class="p">:</span>
+</span><span id="Controller-340"><a href="#Controller-340"><span class="linenos">340</span></a>                <span class="k">return</span> <span class="n">vd</span>
+</span><span id="Controller-341"><a href="#Controller-341"><span class="linenos">341</span></a>        <span class="k">return</span> <span class="kc">None</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>StorCLI Controller</p>
 
 <p>Instance of this class represents controller in StorCLI hierarchy</p>
 
@@ -1537,78 +1550,90 @@
     <a class="headerlink" href="#Controller.encls"></a>
     
             <div class="docstring"><p>(:obj:enclosure.Enclosures): controller enclosures</p>
 </div>
 
 
                             </div>
+                            <div id="Controller.drives_ids" class="classattr">
+                                <div class="attr variable">
+            <span class="name">drives_ids</span><span class="annotation">: List[str]</span>
+
+        
+    </div>
+    <a class="headerlink" href="#Controller.drives_ids"></a>
+    
+            <div class="docstring"><p>(list of str): list of drives ids in format (e:s)</p>
+</div>
+
+
+                            </div>
                             <div id="Controller.create_vd" class="classattr">
                                         <input id="Controller.create_vd-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">create_vd</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">name</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">raid</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">drives</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">strip</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;64&#39;</span>,</span><span class="param">	<span class="n">PDperArray</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">int</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="n">Optional</span><span class="p">[</span><span class="n"><a href="#VirtualDrive">pystorcli2.VirtualDrive</a></span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="Controller.create_vd-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Controller.create_vd"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Controller.create_vd-279"><a href="#Controller.create_vd-279"><span class="linenos">279</span></a>    <span class="k">def</span> <span class="nf">create_vd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">raid</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">drives</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">strip</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;64&#39;</span><span class="p">,</span> <span class="n">PDperArray</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">int</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Optional</span><span class="p">[</span><span class="n">virtualdrive</span><span class="o">.</span><span class="n">VirtualDrive</span><span class="p">]:</span>
-</span><span id="Controller.create_vd-280"><a href="#Controller.create_vd-280"><span class="linenos">280</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Create virtual drive (raid) managed by current controller</span>
-</span><span id="Controller.create_vd-281"><a href="#Controller.create_vd-281"><span class="linenos">281</span></a>
-</span><span id="Controller.create_vd-282"><a href="#Controller.create_vd-282"><span class="linenos">282</span></a><span class="sd">        Args:</span>
-</span><span id="Controller.create_vd-283"><a href="#Controller.create_vd-283"><span class="linenos">283</span></a><span class="sd">            name (str): virtual drive name</span>
-</span><span id="Controller.create_vd-284"><a href="#Controller.create_vd-284"><span class="linenos">284</span></a><span class="sd">            raid (str): virtual drive raid level (raid0, raid1, ...)</span>
-</span><span id="Controller.create_vd-285"><a href="#Controller.create_vd-285"><span class="linenos">285</span></a><span class="sd">            drives (str): storcli drives expression (e:s|e:s-x|e:s-x,y;e:s-x,y,z)</span>
-</span><span id="Controller.create_vd-286"><a href="#Controller.create_vd-286"><span class="linenos">286</span></a><span class="sd">            strip (str, optional): virtual drive raid strip size</span>
-</span><span id="Controller.create_vd-287"><a href="#Controller.create_vd-287"><span class="linenos">287</span></a>
-</span><span id="Controller.create_vd-288"><a href="#Controller.create_vd-288"><span class="linenos">288</span></a><span class="sd">        Returns:</span>
-</span><span id="Controller.create_vd-289"><a href="#Controller.create_vd-289"><span class="linenos">289</span></a><span class="sd">            (None): no virtual drive created with name</span>
-</span><span id="Controller.create_vd-290"><a href="#Controller.create_vd-290"><span class="linenos">290</span></a><span class="sd">            (:obj:virtualdrive.VirtualDrive)</span>
-</span><span id="Controller.create_vd-291"><a href="#Controller.create_vd-291"><span class="linenos">291</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller.create_vd-292"><a href="#Controller.create_vd-292"><span class="linenos">292</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Controller.create_vd-293"><a href="#Controller.create_vd-293"><span class="linenos">293</span></a>            <span class="s1">&#39;add&#39;</span><span class="p">,</span>
-</span><span id="Controller.create_vd-294"><a href="#Controller.create_vd-294"><span class="linenos">294</span></a>            <span class="s1">&#39;vd&#39;</span><span class="p">,</span>
-</span><span id="Controller.create_vd-295"><a href="#Controller.create_vd-295"><span class="linenos">295</span></a>            <span class="s1">&#39;r</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">raid</span><span class="p">),</span>
-</span><span id="Controller.create_vd-296"><a href="#Controller.create_vd-296"><span class="linenos">296</span></a>            <span class="s1">&#39;name=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">name</span><span class="p">),</span>
-</span><span id="Controller.create_vd-297"><a href="#Controller.create_vd-297"><span class="linenos">297</span></a>            <span class="s1">&#39;drives=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">drives</span><span class="p">),</span>
-</span><span id="Controller.create_vd-298"><a href="#Controller.create_vd-298"><span class="linenos">298</span></a>            <span class="s1">&#39;strip=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">strip</span><span class="p">)</span>
-</span><span id="Controller.create_vd-299"><a href="#Controller.create_vd-299"><span class="linenos">299</span></a>        <span class="p">]</span>
-</span><span id="Controller.create_vd-300"><a href="#Controller.create_vd-300"><span class="linenos">300</span></a>
-</span><span id="Controller.create_vd-301"><a href="#Controller.create_vd-301"><span class="linenos">301</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="Controller.create_vd-302"><a href="#Controller.create_vd-302"><span class="linenos">302</span></a>            <span class="k">if</span> <span class="nb">int</span><span class="p">(</span><span class="n">raid</span><span class="p">)</span> <span class="o">&gt;=</span> <span class="mi">10</span> <span class="ow">and</span> <span class="n">PDperArray</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Controller.create_vd-303"><a href="#Controller.create_vd-303"><span class="linenos">303</span></a>                <span class="c1"># Try to count the number of drives in the array</span>
-</span><span id="Controller.create_vd-304"><a href="#Controller.create_vd-304"><span class="linenos">304</span></a>                <span class="c1"># The format of the drives argument is e:s|e:s-x|e:s-x,y;e:s-x,y,z</span>
-</span><span id="Controller.create_vd-305"><a href="#Controller.create_vd-305"><span class="linenos">305</span></a>                <span class="c1"># The number of drives is the number of commas plus the dashes intervals</span>
-</span><span id="Controller.create_vd-306"><a href="#Controller.create_vd-306"><span class="linenos">306</span></a>
-</span><span id="Controller.create_vd-307"><a href="#Controller.create_vd-307"><span class="linenos">307</span></a>                <span class="n">numDrives</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="Controller.create_vd-308"><a href="#Controller.create_vd-308"><span class="linenos">308</span></a>                <span class="n">drives2</span> <span class="o">=</span> <span class="n">drives</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s1">&#39;:&#39;</span><span class="p">)</span>
-</span><span id="Controller.create_vd-309"><a href="#Controller.create_vd-309"><span class="linenos">309</span></a>                <span class="n">drives2</span> <span class="o">=</span> <span class="n">drives2</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span>
-</span><span id="Controller.create_vd-310"><a href="#Controller.create_vd-310"><span class="linenos">310</span></a>                <span class="n">numDrives</span> <span class="o">+=</span> <span class="n">drives2</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="s1">&#39;,&#39;</span><span class="p">)</span><span class="o">+</span><span class="mi">1</span>
-</span><span id="Controller.create_vd-311"><a href="#Controller.create_vd-311"><span class="linenos">311</span></a>                <span class="k">for</span> <span class="n">interval</span> <span class="ow">in</span> <span class="n">drives2</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s1">&#39;,&#39;</span><span class="p">):</span>
-</span><span id="Controller.create_vd-312"><a href="#Controller.create_vd-312"><span class="linenos">312</span></a>                    <span class="k">if</span> <span class="s1">&#39;-&#39;</span> <span class="ow">in</span> <span class="n">interval</span><span class="p">:</span>
-</span><span id="Controller.create_vd-313"><a href="#Controller.create_vd-313"><span class="linenos">313</span></a>                        <span class="n">left</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">interval</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s1">&#39;-&#39;</span><span class="p">)[</span><span class="mi">0</span><span class="p">])</span>
-</span><span id="Controller.create_vd-314"><a href="#Controller.create_vd-314"><span class="linenos">314</span></a>                        <span class="n">right</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">interval</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s1">&#39;-&#39;</span><span class="p">)[</span><span class="mi">1</span><span class="p">])</span>
-</span><span id="Controller.create_vd-315"><a href="#Controller.create_vd-315"><span class="linenos">315</span></a>                        <span class="n">numDrives</span> <span class="o">+=</span> <span class="n">right</span> <span class="o">-</span> <span class="n">left</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Controller.create_vd-290"><a href="#Controller.create_vd-290"><span class="linenos">290</span></a>    <span class="k">def</span> <span class="nf">create_vd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">raid</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">drives</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">strip</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;64&#39;</span><span class="p">,</span> <span class="n">PDperArray</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">int</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Optional</span><span class="p">[</span><span class="n">virtualdrive</span><span class="o">.</span><span class="n">VirtualDrive</span><span class="p">]:</span>
+</span><span id="Controller.create_vd-291"><a href="#Controller.create_vd-291"><span class="linenos">291</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Create virtual drive (raid) managed by current controller</span>
+</span><span id="Controller.create_vd-292"><a href="#Controller.create_vd-292"><span class="linenos">292</span></a>
+</span><span id="Controller.create_vd-293"><a href="#Controller.create_vd-293"><span class="linenos">293</span></a><span class="sd">        Args:</span>
+</span><span id="Controller.create_vd-294"><a href="#Controller.create_vd-294"><span class="linenos">294</span></a><span class="sd">            name (str): virtual drive name</span>
+</span><span id="Controller.create_vd-295"><a href="#Controller.create_vd-295"><span class="linenos">295</span></a><span class="sd">            raid (str): virtual drive raid level (raid0, raid1, ...)</span>
+</span><span id="Controller.create_vd-296"><a href="#Controller.create_vd-296"><span class="linenos">296</span></a><span class="sd">            drives (str): storcli drives expression (e:s|e:s-x|e:s-x,y;e:s-x,y,z)</span>
+</span><span id="Controller.create_vd-297"><a href="#Controller.create_vd-297"><span class="linenos">297</span></a><span class="sd">            strip (str, optional): virtual drive raid strip size</span>
+</span><span id="Controller.create_vd-298"><a href="#Controller.create_vd-298"><span class="linenos">298</span></a>
+</span><span id="Controller.create_vd-299"><a href="#Controller.create_vd-299"><span class="linenos">299</span></a><span class="sd">        Returns:</span>
+</span><span id="Controller.create_vd-300"><a href="#Controller.create_vd-300"><span class="linenos">300</span></a><span class="sd">            (None): no virtual drive created with name</span>
+</span><span id="Controller.create_vd-301"><a href="#Controller.create_vd-301"><span class="linenos">301</span></a><span class="sd">            (:obj:virtualdrive.VirtualDrive)</span>
+</span><span id="Controller.create_vd-302"><a href="#Controller.create_vd-302"><span class="linenos">302</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Controller.create_vd-303"><a href="#Controller.create_vd-303"><span class="linenos">303</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="Controller.create_vd-304"><a href="#Controller.create_vd-304"><span class="linenos">304</span></a>            <span class="s1">&#39;add&#39;</span><span class="p">,</span>
+</span><span id="Controller.create_vd-305"><a href="#Controller.create_vd-305"><span class="linenos">305</span></a>            <span class="s1">&#39;vd&#39;</span><span class="p">,</span>
+</span><span id="Controller.create_vd-306"><a href="#Controller.create_vd-306"><span class="linenos">306</span></a>            <span class="s1">&#39;r</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">raid</span><span class="p">),</span>
+</span><span id="Controller.create_vd-307"><a href="#Controller.create_vd-307"><span class="linenos">307</span></a>            <span class="s1">&#39;name=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">name</span><span class="p">),</span>
+</span><span id="Controller.create_vd-308"><a href="#Controller.create_vd-308"><span class="linenos">308</span></a>            <span class="s1">&#39;drives=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">drives</span><span class="p">),</span>
+</span><span id="Controller.create_vd-309"><a href="#Controller.create_vd-309"><span class="linenos">309</span></a>            <span class="s1">&#39;strip=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">strip</span><span class="p">)</span>
+</span><span id="Controller.create_vd-310"><a href="#Controller.create_vd-310"><span class="linenos">310</span></a>        <span class="p">]</span>
+</span><span id="Controller.create_vd-311"><a href="#Controller.create_vd-311"><span class="linenos">311</span></a>
+</span><span id="Controller.create_vd-312"><a href="#Controller.create_vd-312"><span class="linenos">312</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="Controller.create_vd-313"><a href="#Controller.create_vd-313"><span class="linenos">313</span></a>            <span class="k">if</span> <span class="nb">int</span><span class="p">(</span><span class="n">raid</span><span class="p">)</span> <span class="o">&gt;=</span> <span class="mi">10</span> <span class="ow">and</span> <span class="n">PDperArray</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Controller.create_vd-314"><a href="#Controller.create_vd-314"><span class="linenos">314</span></a>                <span class="c1"># Try to count the number of drives in the array</span>
+</span><span id="Controller.create_vd-315"><a href="#Controller.create_vd-315"><span class="linenos">315</span></a>                <span class="c1"># The format of the drives argument is e:s|e:s-x|e:s-x,y;e:s-x,y,z</span>
 </span><span id="Controller.create_vd-316"><a href="#Controller.create_vd-316"><span class="linenos">316</span></a>
-</span><span id="Controller.create_vd-317"><a href="#Controller.create_vd-317"><span class="linenos">317</span></a>                <span class="n">PDperArray</span> <span class="o">=</span> <span class="n">numDrives</span><span class="o">//</span><span class="mi">2</span>
-</span><span id="Controller.create_vd-318"><a href="#Controller.create_vd-318"><span class="linenos">318</span></a>        <span class="k">except</span> <span class="ne">ValueError</span><span class="p">:</span>
-</span><span id="Controller.create_vd-319"><a href="#Controller.create_vd-319"><span class="linenos">319</span></a>            <span class="k">pass</span>
-</span><span id="Controller.create_vd-320"><a href="#Controller.create_vd-320"><span class="linenos">320</span></a>
-</span><span id="Controller.create_vd-321"><a href="#Controller.create_vd-321"><span class="linenos">321</span></a>        <span class="k">if</span> <span class="n">raid</span> <span class="o">==</span> <span class="s1">&#39;00&#39;</span> <span class="ow">and</span> <span class="n">PDperArray</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Controller.create_vd-322"><a href="#Controller.create_vd-322"><span class="linenos">322</span></a>            <span class="n">PDperArray</span> <span class="o">=</span> <span class="mi">1</span>
-</span><span id="Controller.create_vd-323"><a href="#Controller.create_vd-323"><span class="linenos">323</span></a>
-</span><span id="Controller.create_vd-324"><a href="#Controller.create_vd-324"><span class="linenos">324</span></a>        <span class="k">if</span> <span class="n">PDperArray</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Controller.create_vd-325"><a href="#Controller.create_vd-325"><span class="linenos">325</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;PDperArray=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">PDperArray</span><span class="p">))</span>
+</span><span id="Controller.create_vd-317"><a href="#Controller.create_vd-317"><span class="linenos">317</span></a>                <span class="n">numDrives</span> <span class="o">=</span> <span class="n">common</span><span class="o">.</span><span class="n">count_drives</span><span class="p">(</span><span class="n">drives</span><span class="p">)</span>
+</span><span id="Controller.create_vd-318"><a href="#Controller.create_vd-318"><span class="linenos">318</span></a>
+</span><span id="Controller.create_vd-319"><a href="#Controller.create_vd-319"><span class="linenos">319</span></a>                <span class="k">if</span> <span class="n">numDrives</span> <span class="o">%</span> <span class="mi">2</span> <span class="o">!=</span> <span class="mi">0</span> <span class="ow">and</span> <span class="n">numDrives</span> <span class="o">%</span> <span class="mi">3</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="Controller.create_vd-320"><a href="#Controller.create_vd-320"><span class="linenos">320</span></a>                    <span class="c1"># In some scenarios, such as 9 drives with raid 60, 3 is a good pd number but 4 is not</span>
+</span><span id="Controller.create_vd-321"><a href="#Controller.create_vd-321"><span class="linenos">321</span></a>                    <span class="c1"># Must check for similar scenarios</span>
+</span><span id="Controller.create_vd-322"><a href="#Controller.create_vd-322"><span class="linenos">322</span></a>                    <span class="c1"># BTW we don&#39;t clearly understand what PDperArray is for and what exactly it does under the hood. More investigation is needed</span>
+</span><span id="Controller.create_vd-323"><a href="#Controller.create_vd-323"><span class="linenos">323</span></a>                    <span class="n">PDperArray</span> <span class="o">=</span> <span class="n">numDrives</span><span class="o">//</span><span class="mi">3</span>
+</span><span id="Controller.create_vd-324"><a href="#Controller.create_vd-324"><span class="linenos">324</span></a>                <span class="k">else</span><span class="p">:</span>
+</span><span id="Controller.create_vd-325"><a href="#Controller.create_vd-325"><span class="linenos">325</span></a>                    <span class="n">PDperArray</span> <span class="o">=</span> <span class="n">numDrives</span><span class="o">//</span><span class="mi">2</span>
 </span><span id="Controller.create_vd-326"><a href="#Controller.create_vd-326"><span class="linenos">326</span></a>
-</span><span id="Controller.create_vd-327"><a href="#Controller.create_vd-327"><span class="linenos">327</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="Controller.create_vd-328"><a href="#Controller.create_vd-328"><span class="linenos">328</span></a>        <span class="k">for</span> <span class="n">vd</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">vds</span><span class="p">:</span>
-</span><span id="Controller.create_vd-329"><a href="#Controller.create_vd-329"><span class="linenos">329</span></a>            <span class="k">if</span> <span class="n">name</span> <span class="o">==</span> <span class="n">vd</span><span class="o">.</span><span class="n">name</span><span class="p">:</span>
-</span><span id="Controller.create_vd-330"><a href="#Controller.create_vd-330"><span class="linenos">330</span></a>                <span class="k">return</span> <span class="n">vd</span>
-</span><span id="Controller.create_vd-331"><a href="#Controller.create_vd-331"><span class="linenos">331</span></a>        <span class="k">return</span> <span class="kc">None</span>
+</span><span id="Controller.create_vd-327"><a href="#Controller.create_vd-327"><span class="linenos">327</span></a>        <span class="k">except</span> <span class="ne">ValueError</span><span class="p">:</span>
+</span><span id="Controller.create_vd-328"><a href="#Controller.create_vd-328"><span class="linenos">328</span></a>            <span class="k">pass</span>
+</span><span id="Controller.create_vd-329"><a href="#Controller.create_vd-329"><span class="linenos">329</span></a>
+</span><span id="Controller.create_vd-330"><a href="#Controller.create_vd-330"><span class="linenos">330</span></a>        <span class="k">finally</span><span class="p">:</span>
+</span><span id="Controller.create_vd-331"><a href="#Controller.create_vd-331"><span class="linenos">331</span></a>            <span class="k">if</span> <span class="n">raid</span> <span class="o">==</span> <span class="s1">&#39;00&#39;</span> <span class="ow">and</span> <span class="n">PDperArray</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Controller.create_vd-332"><a href="#Controller.create_vd-332"><span class="linenos">332</span></a>                <span class="n">PDperArray</span> <span class="o">=</span> <span class="mi">1</span>
+</span><span id="Controller.create_vd-333"><a href="#Controller.create_vd-333"><span class="linenos">333</span></a>
+</span><span id="Controller.create_vd-334"><a href="#Controller.create_vd-334"><span class="linenos">334</span></a>        <span class="k">if</span> <span class="n">PDperArray</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Controller.create_vd-335"><a href="#Controller.create_vd-335"><span class="linenos">335</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;PDperArray=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">PDperArray</span><span class="p">))</span>
+</span><span id="Controller.create_vd-336"><a href="#Controller.create_vd-336"><span class="linenos">336</span></a>
+</span><span id="Controller.create_vd-337"><a href="#Controller.create_vd-337"><span class="linenos">337</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="Controller.create_vd-338"><a href="#Controller.create_vd-338"><span class="linenos">338</span></a>        <span class="k">for</span> <span class="n">vd</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">vds</span><span class="p">:</span>
+</span><span id="Controller.create_vd-339"><a href="#Controller.create_vd-339"><span class="linenos">339</span></a>            <span class="k">if</span> <span class="n">name</span> <span class="o">==</span> <span class="n">vd</span><span class="o">.</span><span class="n">name</span><span class="p">:</span>
+</span><span id="Controller.create_vd-340"><a href="#Controller.create_vd-340"><span class="linenos">340</span></a>                <span class="k">return</span> <span class="n">vd</span>
+</span><span id="Controller.create_vd-341"><a href="#Controller.create_vd-341"><span class="linenos">341</span></a>        <span class="k">return</span> <span class="kc">None</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create virtual drive (raid) managed by current controller</p>
 
 <p>Args:
     name (str): virtual drive name
@@ -1631,76 +1656,76 @@
     <span class="def">class</span>
     <span class="name">Controllers</span>:
 
                 <label class="view-source-button" for="Controllers-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Controllers"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Controllers-334"><a href="#Controllers-334"><span class="linenos">334</span></a><span class="k">class</span> <span class="nc">Controllers</span><span class="p">(</span><span class="nb">object</span><span class="p">):</span>
-</span><span id="Controllers-335"><a href="#Controllers-335"><span class="linenos">335</span></a><span class="w">    </span><span class="sd">&quot;&quot;&quot;StorCLI Controllers</span>
-</span><span id="Controllers-336"><a href="#Controllers-336"><span class="linenos">336</span></a>
-</span><span id="Controllers-337"><a href="#Controllers-337"><span class="linenos">337</span></a><span class="sd">    Instance of this class is iterable with :obj:Controller as item</span>
-</span><span id="Controllers-338"><a href="#Controllers-338"><span class="linenos">338</span></a>
-</span><span id="Controllers-339"><a href="#Controllers-339"><span class="linenos">339</span></a><span class="sd">    Args:</span>
-</span><span id="Controllers-340"><a href="#Controllers-340"><span class="linenos">340</span></a><span class="sd">        binary (str): storcli binary or full path to the binary</span>
-</span><span id="Controllers-341"><a href="#Controllers-341"><span class="linenos">341</span></a>
-</span><span id="Controllers-342"><a href="#Controllers-342"><span class="linenos">342</span></a><span class="sd">    Properties:</span>
-</span><span id="Controllers-343"><a href="#Controllers-343"><span class="linenos">343</span></a><span class="sd">        ids (list of str): list of controllers id</span>
-</span><span id="Controllers-344"><a href="#Controllers-344"><span class="linenos">344</span></a>
-</span><span id="Controllers-345"><a href="#Controllers-345"><span class="linenos">345</span></a><span class="sd">    Methods:</span>
-</span><span id="Controllers-346"><a href="#Controllers-346"><span class="linenos">346</span></a><span class="sd">        get_clt (:obj:Controller): return controller object by id</span>
-</span><span id="Controllers-347"><a href="#Controllers-347"><span class="linenos">347</span></a><span class="sd">    &quot;&quot;&quot;</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Controllers-344"><a href="#Controllers-344"><span class="linenos">344</span></a><span class="k">class</span> <span class="nc">Controllers</span><span class="p">(</span><span class="nb">object</span><span class="p">):</span>
+</span><span id="Controllers-345"><a href="#Controllers-345"><span class="linenos">345</span></a><span class="w">    </span><span class="sd">&quot;&quot;&quot;StorCLI Controllers</span>
+</span><span id="Controllers-346"><a href="#Controllers-346"><span class="linenos">346</span></a>
+</span><span id="Controllers-347"><a href="#Controllers-347"><span class="linenos">347</span></a><span class="sd">    Instance of this class is iterable with :obj:Controller as item</span>
 </span><span id="Controllers-348"><a href="#Controllers-348"><span class="linenos">348</span></a>
-</span><span id="Controllers-349"><a href="#Controllers-349"><span class="linenos">349</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">binary</span><span class="o">=</span><span class="s1">&#39;storcli64&#39;</span><span class="p">):</span>
-</span><span id="Controllers-350"><a href="#Controllers-350"><span class="linenos">350</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Constructor - create StorCLI Controllers object</span>
+</span><span id="Controllers-349"><a href="#Controllers-349"><span class="linenos">349</span></a><span class="sd">    Args:</span>
+</span><span id="Controllers-350"><a href="#Controllers-350"><span class="linenos">350</span></a><span class="sd">        binary (str): storcli binary or full path to the binary</span>
 </span><span id="Controllers-351"><a href="#Controllers-351"><span class="linenos">351</span></a>
-</span><span id="Controllers-352"><a href="#Controllers-352"><span class="linenos">352</span></a><span class="sd">        Args:</span>
-</span><span id="Controllers-353"><a href="#Controllers-353"><span class="linenos">353</span></a><span class="sd">            binary (str): storcli binary or full path to the binary</span>
-</span><span id="Controllers-354"><a href="#Controllers-354"><span class="linenos">354</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controllers-355"><a href="#Controllers-355"><span class="linenos">355</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_binary</span> <span class="o">=</span> <span class="n">binary</span>
-</span><span id="Controllers-356"><a href="#Controllers-356"><span class="linenos">356</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_storcli</span> <span class="o">=</span> <span class="n">StorCLI</span><span class="p">(</span><span class="n">binary</span><span class="p">)</span>
-</span><span id="Controllers-357"><a href="#Controllers-357"><span class="linenos">357</span></a>
-</span><span id="Controllers-358"><a href="#Controllers-358"><span class="linenos">358</span></a>    <span class="o">@</span> <span class="nb">property</span>
-</span><span id="Controllers-359"><a href="#Controllers-359"><span class="linenos">359</span></a>    <span class="k">def</span> <span class="nf">_ctl_ids</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">List</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="Controllers-360"><a href="#Controllers-360"><span class="linenos">360</span></a>        <span class="n">out</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_storcli</span><span class="o">.</span><span class="n">run</span><span class="p">([</span><span class="s1">&#39;show&#39;</span><span class="p">])</span>
-</span><span id="Controllers-361"><a href="#Controllers-361"><span class="linenos">361</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">common</span><span class="o">.</span><span class="n">response_data</span><span class="p">(</span><span class="n">out</span><span class="p">)</span>
-</span><span id="Controllers-362"><a href="#Controllers-362"><span class="linenos">362</span></a>
-</span><span id="Controllers-363"><a href="#Controllers-363"><span class="linenos">363</span></a>        <span class="k">if</span> <span class="s2">&quot;Number of Controllers&quot;</span> <span class="ow">in</span> <span class="n">response</span> <span class="ow">and</span> <span class="n">response</span><span class="p">[</span><span class="s2">&quot;Number of Controllers&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="Controllers-364"><a href="#Controllers-364"><span class="linenos">364</span></a>            <span class="k">return</span> <span class="p">[]</span>
-</span><span id="Controllers-365"><a href="#Controllers-365"><span class="linenos">365</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="Controllers-366"><a href="#Controllers-366"><span class="linenos">366</span></a>            <span class="k">return</span> <span class="p">[</span><span class="n">ctl</span><span class="p">[</span><span class="s1">&#39;Ctl&#39;</span><span class="p">]</span> <span class="k">for</span> <span class="n">ctl</span> <span class="ow">in</span> <span class="n">common</span><span class="o">.</span><span class="n">response_data_subkey</span><span class="p">(</span><span class="n">out</span><span class="p">,</span> <span class="p">[</span><span class="s1">&#39;System Overview&#39;</span><span class="p">,</span> <span class="s1">&#39;IT System Overview&#39;</span><span class="p">])]</span>
+</span><span id="Controllers-352"><a href="#Controllers-352"><span class="linenos">352</span></a><span class="sd">    Properties:</span>
+</span><span id="Controllers-353"><a href="#Controllers-353"><span class="linenos">353</span></a><span class="sd">        ids (list of str): list of controllers id</span>
+</span><span id="Controllers-354"><a href="#Controllers-354"><span class="linenos">354</span></a>
+</span><span id="Controllers-355"><a href="#Controllers-355"><span class="linenos">355</span></a><span class="sd">    Methods:</span>
+</span><span id="Controllers-356"><a href="#Controllers-356"><span class="linenos">356</span></a><span class="sd">        get_clt (:obj:Controller): return controller object by id</span>
+</span><span id="Controllers-357"><a href="#Controllers-357"><span class="linenos">357</span></a><span class="sd">    &quot;&quot;&quot;</span>
+</span><span id="Controllers-358"><a href="#Controllers-358"><span class="linenos">358</span></a>
+</span><span id="Controllers-359"><a href="#Controllers-359"><span class="linenos">359</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">binary</span><span class="o">=</span><span class="s1">&#39;storcli64&#39;</span><span class="p">):</span>
+</span><span id="Controllers-360"><a href="#Controllers-360"><span class="linenos">360</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Constructor - create StorCLI Controllers object</span>
+</span><span id="Controllers-361"><a href="#Controllers-361"><span class="linenos">361</span></a>
+</span><span id="Controllers-362"><a href="#Controllers-362"><span class="linenos">362</span></a><span class="sd">        Args:</span>
+</span><span id="Controllers-363"><a href="#Controllers-363"><span class="linenos">363</span></a><span class="sd">            binary (str): storcli binary or full path to the binary</span>
+</span><span id="Controllers-364"><a href="#Controllers-364"><span class="linenos">364</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Controllers-365"><a href="#Controllers-365"><span class="linenos">365</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_binary</span> <span class="o">=</span> <span class="n">binary</span>
+</span><span id="Controllers-366"><a href="#Controllers-366"><span class="linenos">366</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_storcli</span> <span class="o">=</span> <span class="n">StorCLI</span><span class="p">(</span><span class="n">binary</span><span class="p">)</span>
 </span><span id="Controllers-367"><a href="#Controllers-367"><span class="linenos">367</span></a>
 </span><span id="Controllers-368"><a href="#Controllers-368"><span class="linenos">368</span></a>    <span class="o">@</span> <span class="nb">property</span>
-</span><span id="Controllers-369"><a href="#Controllers-369"><span class="linenos">369</span></a>    <span class="k">def</span> <span class="nf">_ctls</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controllers-370"><a href="#Controllers-370"><span class="linenos">370</span></a>        <span class="k">for</span> <span class="n">ctl_id</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_ctl_ids</span><span class="p">:</span>
-</span><span id="Controllers-371"><a href="#Controllers-371"><span class="linenos">371</span></a>            <span class="k">yield</span> <span class="n">Controller</span><span class="p">(</span><span class="n">ctl_id</span><span class="o">=</span><span class="n">ctl_id</span><span class="p">,</span> <span class="n">binary</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_binary</span><span class="p">)</span>
+</span><span id="Controllers-369"><a href="#Controllers-369"><span class="linenos">369</span></a>    <span class="k">def</span> <span class="nf">_ctl_ids</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">List</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="Controllers-370"><a href="#Controllers-370"><span class="linenos">370</span></a>        <span class="n">out</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_storcli</span><span class="o">.</span><span class="n">run</span><span class="p">([</span><span class="s1">&#39;show&#39;</span><span class="p">])</span>
+</span><span id="Controllers-371"><a href="#Controllers-371"><span class="linenos">371</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">common</span><span class="o">.</span><span class="n">response_data</span><span class="p">(</span><span class="n">out</span><span class="p">)</span>
 </span><span id="Controllers-372"><a href="#Controllers-372"><span class="linenos">372</span></a>
-</span><span id="Controllers-373"><a href="#Controllers-373"><span class="linenos">373</span></a>    <span class="k">def</span> <span class="fm">__iter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controllers-374"><a href="#Controllers-374"><span class="linenos">374</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_ctls</span>
-</span><span id="Controllers-375"><a href="#Controllers-375"><span class="linenos">375</span></a>
-</span><span id="Controllers-376"><a href="#Controllers-376"><span class="linenos">376</span></a>    <span class="o">@</span> <span class="nb">property</span>
-</span><span id="Controllers-377"><a href="#Controllers-377"><span class="linenos">377</span></a>    <span class="k">def</span> <span class="nf">ids</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controllers-378"><a href="#Controllers-378"><span class="linenos">378</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;(list of str): controllers id</span>
-</span><span id="Controllers-379"><a href="#Controllers-379"><span class="linenos">379</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controllers-380"><a href="#Controllers-380"><span class="linenos">380</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_ctl_ids</span>
-</span><span id="Controllers-381"><a href="#Controllers-381"><span class="linenos">381</span></a>
-</span><span id="Controllers-382"><a href="#Controllers-382"><span class="linenos">382</span></a>    <span class="k">def</span> <span class="nf">get_ctl</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">ctl_id</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Optional</span><span class="p">[</span><span class="n">Controller</span><span class="p">]:</span>
-</span><span id="Controllers-383"><a href="#Controllers-383"><span class="linenos">383</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Get controller object by id</span>
-</span><span id="Controllers-384"><a href="#Controllers-384"><span class="linenos">384</span></a>
-</span><span id="Controllers-385"><a href="#Controllers-385"><span class="linenos">385</span></a><span class="sd">        Args:</span>
-</span><span id="Controllers-386"><a href="#Controllers-386"><span class="linenos">386</span></a><span class="sd">            ctl_id (str): controller id</span>
-</span><span id="Controllers-387"><a href="#Controllers-387"><span class="linenos">387</span></a>
-</span><span id="Controllers-388"><a href="#Controllers-388"><span class="linenos">388</span></a><span class="sd">        Returns:</span>
-</span><span id="Controllers-389"><a href="#Controllers-389"><span class="linenos">389</span></a><span class="sd">            (None): no controller with id</span>
-</span><span id="Controllers-390"><a href="#Controllers-390"><span class="linenos">390</span></a><span class="sd">            (:obj:Controller): controller object</span>
-</span><span id="Controllers-391"><a href="#Controllers-391"><span class="linenos">391</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controllers-392"><a href="#Controllers-392"><span class="linenos">392</span></a>        <span class="k">for</span> <span class="n">ctl</span> <span class="ow">in</span> <span class="bp">self</span><span class="p">:</span>
-</span><span id="Controllers-393"><a href="#Controllers-393"><span class="linenos">393</span></a>            <span class="k">if</span> <span class="n">ctl</span><span class="o">.</span><span class="n">id</span> <span class="o">==</span> <span class="n">ctl_id</span><span class="p">:</span>
-</span><span id="Controllers-394"><a href="#Controllers-394"><span class="linenos">394</span></a>                <span class="k">return</span> <span class="n">ctl</span>
-</span><span id="Controllers-395"><a href="#Controllers-395"><span class="linenos">395</span></a>        <span class="k">return</span> <span class="kc">None</span>
+</span><span id="Controllers-373"><a href="#Controllers-373"><span class="linenos">373</span></a>        <span class="k">if</span> <span class="s2">&quot;Number of Controllers&quot;</span> <span class="ow">in</span> <span class="n">response</span> <span class="ow">and</span> <span class="n">response</span><span class="p">[</span><span class="s2">&quot;Number of Controllers&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="Controllers-374"><a href="#Controllers-374"><span class="linenos">374</span></a>            <span class="k">return</span> <span class="p">[]</span>
+</span><span id="Controllers-375"><a href="#Controllers-375"><span class="linenos">375</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="Controllers-376"><a href="#Controllers-376"><span class="linenos">376</span></a>            <span class="k">return</span> <span class="p">[</span><span class="n">ctl</span><span class="p">[</span><span class="s1">&#39;Ctl&#39;</span><span class="p">]</span> <span class="k">for</span> <span class="n">ctl</span> <span class="ow">in</span> <span class="n">common</span><span class="o">.</span><span class="n">response_data_subkey</span><span class="p">(</span><span class="n">out</span><span class="p">,</span> <span class="p">[</span><span class="s1">&#39;System Overview&#39;</span><span class="p">,</span> <span class="s1">&#39;IT System Overview&#39;</span><span class="p">])]</span>
+</span><span id="Controllers-377"><a href="#Controllers-377"><span class="linenos">377</span></a>
+</span><span id="Controllers-378"><a href="#Controllers-378"><span class="linenos">378</span></a>    <span class="o">@</span> <span class="nb">property</span>
+</span><span id="Controllers-379"><a href="#Controllers-379"><span class="linenos">379</span></a>    <span class="k">def</span> <span class="nf">_ctls</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Controllers-380"><a href="#Controllers-380"><span class="linenos">380</span></a>        <span class="k">for</span> <span class="n">ctl_id</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_ctl_ids</span><span class="p">:</span>
+</span><span id="Controllers-381"><a href="#Controllers-381"><span class="linenos">381</span></a>            <span class="k">yield</span> <span class="n">Controller</span><span class="p">(</span><span class="n">ctl_id</span><span class="o">=</span><span class="n">ctl_id</span><span class="p">,</span> <span class="n">binary</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_binary</span><span class="p">)</span>
+</span><span id="Controllers-382"><a href="#Controllers-382"><span class="linenos">382</span></a>
+</span><span id="Controllers-383"><a href="#Controllers-383"><span class="linenos">383</span></a>    <span class="k">def</span> <span class="fm">__iter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Controllers-384"><a href="#Controllers-384"><span class="linenos">384</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_ctls</span>
+</span><span id="Controllers-385"><a href="#Controllers-385"><span class="linenos">385</span></a>
+</span><span id="Controllers-386"><a href="#Controllers-386"><span class="linenos">386</span></a>    <span class="o">@</span> <span class="nb">property</span>
+</span><span id="Controllers-387"><a href="#Controllers-387"><span class="linenos">387</span></a>    <span class="k">def</span> <span class="nf">ids</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Controllers-388"><a href="#Controllers-388"><span class="linenos">388</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;(list of str): controllers id</span>
+</span><span id="Controllers-389"><a href="#Controllers-389"><span class="linenos">389</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Controllers-390"><a href="#Controllers-390"><span class="linenos">390</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_ctl_ids</span>
+</span><span id="Controllers-391"><a href="#Controllers-391"><span class="linenos">391</span></a>
+</span><span id="Controllers-392"><a href="#Controllers-392"><span class="linenos">392</span></a>    <span class="k">def</span> <span class="nf">get_ctl</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">ctl_id</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Optional</span><span class="p">[</span><span class="n">Controller</span><span class="p">]:</span>
+</span><span id="Controllers-393"><a href="#Controllers-393"><span class="linenos">393</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Get controller object by id</span>
+</span><span id="Controllers-394"><a href="#Controllers-394"><span class="linenos">394</span></a>
+</span><span id="Controllers-395"><a href="#Controllers-395"><span class="linenos">395</span></a><span class="sd">        Args:</span>
+</span><span id="Controllers-396"><a href="#Controllers-396"><span class="linenos">396</span></a><span class="sd">            ctl_id (str): controller id</span>
+</span><span id="Controllers-397"><a href="#Controllers-397"><span class="linenos">397</span></a>
+</span><span id="Controllers-398"><a href="#Controllers-398"><span class="linenos">398</span></a><span class="sd">        Returns:</span>
+</span><span id="Controllers-399"><a href="#Controllers-399"><span class="linenos">399</span></a><span class="sd">            (None): no controller with id</span>
+</span><span id="Controllers-400"><a href="#Controllers-400"><span class="linenos">400</span></a><span class="sd">            (:obj:Controller): controller object</span>
+</span><span id="Controllers-401"><a href="#Controllers-401"><span class="linenos">401</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Controllers-402"><a href="#Controllers-402"><span class="linenos">402</span></a>        <span class="k">for</span> <span class="n">ctl</span> <span class="ow">in</span> <span class="bp">self</span><span class="p">:</span>
+</span><span id="Controllers-403"><a href="#Controllers-403"><span class="linenos">403</span></a>            <span class="k">if</span> <span class="n">ctl</span><span class="o">.</span><span class="n">id</span> <span class="o">==</span> <span class="n">ctl_id</span><span class="p">:</span>
+</span><span id="Controllers-404"><a href="#Controllers-404"><span class="linenos">404</span></a>                <span class="k">return</span> <span class="n">ctl</span>
+</span><span id="Controllers-405"><a href="#Controllers-405"><span class="linenos">405</span></a>        <span class="k">return</span> <span class="kc">None</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>StorCLI Controllers</p>
 
 <p>Instance of this class is iterable with :obj:Controller as item</p>
 
@@ -1721,22 +1746,22 @@
             
         <span class="name">Controllers</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">binary</span><span class="o">=</span><span class="s1">&#39;storcli64&#39;</span></span>)</span>
 
                 <label class="view-source-button" for="Controllers.__init__-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Controllers.__init__"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Controllers.__init__-349"><a href="#Controllers.__init__-349"><span class="linenos">349</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">binary</span><span class="o">=</span><span class="s1">&#39;storcli64&#39;</span><span class="p">):</span>
-</span><span id="Controllers.__init__-350"><a href="#Controllers.__init__-350"><span class="linenos">350</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Constructor - create StorCLI Controllers object</span>
-</span><span id="Controllers.__init__-351"><a href="#Controllers.__init__-351"><span class="linenos">351</span></a>
-</span><span id="Controllers.__init__-352"><a href="#Controllers.__init__-352"><span class="linenos">352</span></a><span class="sd">        Args:</span>
-</span><span id="Controllers.__init__-353"><a href="#Controllers.__init__-353"><span class="linenos">353</span></a><span class="sd">            binary (str): storcli binary or full path to the binary</span>
-</span><span id="Controllers.__init__-354"><a href="#Controllers.__init__-354"><span class="linenos">354</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controllers.__init__-355"><a href="#Controllers.__init__-355"><span class="linenos">355</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_binary</span> <span class="o">=</span> <span class="n">binary</span>
-</span><span id="Controllers.__init__-356"><a href="#Controllers.__init__-356"><span class="linenos">356</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_storcli</span> <span class="o">=</span> <span class="n">StorCLI</span><span class="p">(</span><span class="n">binary</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Controllers.__init__-359"><a href="#Controllers.__init__-359"><span class="linenos">359</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">binary</span><span class="o">=</span><span class="s1">&#39;storcli64&#39;</span><span class="p">):</span>
+</span><span id="Controllers.__init__-360"><a href="#Controllers.__init__-360"><span class="linenos">360</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Constructor - create StorCLI Controllers object</span>
+</span><span id="Controllers.__init__-361"><a href="#Controllers.__init__-361"><span class="linenos">361</span></a>
+</span><span id="Controllers.__init__-362"><a href="#Controllers.__init__-362"><span class="linenos">362</span></a><span class="sd">        Args:</span>
+</span><span id="Controllers.__init__-363"><a href="#Controllers.__init__-363"><span class="linenos">363</span></a><span class="sd">            binary (str): storcli binary or full path to the binary</span>
+</span><span id="Controllers.__init__-364"><a href="#Controllers.__init__-364"><span class="linenos">364</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Controllers.__init__-365"><a href="#Controllers.__init__-365"><span class="linenos">365</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_binary</span> <span class="o">=</span> <span class="n">binary</span>
+</span><span id="Controllers.__init__-366"><a href="#Controllers.__init__-366"><span class="linenos">366</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_storcli</span> <span class="o">=</span> <span class="n">StorCLI</span><span class="p">(</span><span class="n">binary</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Constructor - create StorCLI Controllers object</p>
 
 <p>Args:
     binary (str): storcli binary or full path to the binary</p>
@@ -1764,28 +1789,28 @@
         <span class="def">def</span>
         <span class="name">get_ctl</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">ctl_id</span><span class="p">:</span> <span class="nb">int</span></span><span class="return-annotation">) -> <span class="n">Optional</span><span class="p">[</span><span class="n"><a href="#Controller">pystorcli2.Controller</a></span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="Controllers.get_ctl-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Controllers.get_ctl"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Controllers.get_ctl-382"><a href="#Controllers.get_ctl-382"><span class="linenos">382</span></a>    <span class="k">def</span> <span class="nf">get_ctl</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">ctl_id</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Optional</span><span class="p">[</span><span class="n">Controller</span><span class="p">]:</span>
-</span><span id="Controllers.get_ctl-383"><a href="#Controllers.get_ctl-383"><span class="linenos">383</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Get controller object by id</span>
-</span><span id="Controllers.get_ctl-384"><a href="#Controllers.get_ctl-384"><span class="linenos">384</span></a>
-</span><span id="Controllers.get_ctl-385"><a href="#Controllers.get_ctl-385"><span class="linenos">385</span></a><span class="sd">        Args:</span>
-</span><span id="Controllers.get_ctl-386"><a href="#Controllers.get_ctl-386"><span class="linenos">386</span></a><span class="sd">            ctl_id (str): controller id</span>
-</span><span id="Controllers.get_ctl-387"><a href="#Controllers.get_ctl-387"><span class="linenos">387</span></a>
-</span><span id="Controllers.get_ctl-388"><a href="#Controllers.get_ctl-388"><span class="linenos">388</span></a><span class="sd">        Returns:</span>
-</span><span id="Controllers.get_ctl-389"><a href="#Controllers.get_ctl-389"><span class="linenos">389</span></a><span class="sd">            (None): no controller with id</span>
-</span><span id="Controllers.get_ctl-390"><a href="#Controllers.get_ctl-390"><span class="linenos">390</span></a><span class="sd">            (:obj:Controller): controller object</span>
-</span><span id="Controllers.get_ctl-391"><a href="#Controllers.get_ctl-391"><span class="linenos">391</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controllers.get_ctl-392"><a href="#Controllers.get_ctl-392"><span class="linenos">392</span></a>        <span class="k">for</span> <span class="n">ctl</span> <span class="ow">in</span> <span class="bp">self</span><span class="p">:</span>
-</span><span id="Controllers.get_ctl-393"><a href="#Controllers.get_ctl-393"><span class="linenos">393</span></a>            <span class="k">if</span> <span class="n">ctl</span><span class="o">.</span><span class="n">id</span> <span class="o">==</span> <span class="n">ctl_id</span><span class="p">:</span>
-</span><span id="Controllers.get_ctl-394"><a href="#Controllers.get_ctl-394"><span class="linenos">394</span></a>                <span class="k">return</span> <span class="n">ctl</span>
-</span><span id="Controllers.get_ctl-395"><a href="#Controllers.get_ctl-395"><span class="linenos">395</span></a>        <span class="k">return</span> <span class="kc">None</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Controllers.get_ctl-392"><a href="#Controllers.get_ctl-392"><span class="linenos">392</span></a>    <span class="k">def</span> <span class="nf">get_ctl</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">ctl_id</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Optional</span><span class="p">[</span><span class="n">Controller</span><span class="p">]:</span>
+</span><span id="Controllers.get_ctl-393"><a href="#Controllers.get_ctl-393"><span class="linenos">393</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Get controller object by id</span>
+</span><span id="Controllers.get_ctl-394"><a href="#Controllers.get_ctl-394"><span class="linenos">394</span></a>
+</span><span id="Controllers.get_ctl-395"><a href="#Controllers.get_ctl-395"><span class="linenos">395</span></a><span class="sd">        Args:</span>
+</span><span id="Controllers.get_ctl-396"><a href="#Controllers.get_ctl-396"><span class="linenos">396</span></a><span class="sd">            ctl_id (str): controller id</span>
+</span><span id="Controllers.get_ctl-397"><a href="#Controllers.get_ctl-397"><span class="linenos">397</span></a>
+</span><span id="Controllers.get_ctl-398"><a href="#Controllers.get_ctl-398"><span class="linenos">398</span></a><span class="sd">        Returns:</span>
+</span><span id="Controllers.get_ctl-399"><a href="#Controllers.get_ctl-399"><span class="linenos">399</span></a><span class="sd">            (None): no controller with id</span>
+</span><span id="Controllers.get_ctl-400"><a href="#Controllers.get_ctl-400"><span class="linenos">400</span></a><span class="sd">            (:obj:Controller): controller object</span>
+</span><span id="Controllers.get_ctl-401"><a href="#Controllers.get_ctl-401"><span class="linenos">401</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Controllers.get_ctl-402"><a href="#Controllers.get_ctl-402"><span class="linenos">402</span></a>        <span class="k">for</span> <span class="n">ctl</span> <span class="ow">in</span> <span class="bp">self</span><span class="p">:</span>
+</span><span id="Controllers.get_ctl-403"><a href="#Controllers.get_ctl-403"><span class="linenos">403</span></a>            <span class="k">if</span> <span class="n">ctl</span><span class="o">.</span><span class="n">id</span> <span class="o">==</span> <span class="n">ctl_id</span><span class="p">:</span>
+</span><span id="Controllers.get_ctl-404"><a href="#Controllers.get_ctl-404"><span class="linenos">404</span></a>                <span class="k">return</span> <span class="n">ctl</span>
+</span><span id="Controllers.get_ctl-405"><a href="#Controllers.get_ctl-405"><span class="linenos">405</span></a>        <span class="k">return</span> <span class="kc">None</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Get controller object by id</p>
 
 <p>Args:
     ctl_id (str): controller id</p>
```

#### html2text {}

```diff
@@ -21,14 +21,15 @@
           o Controller
           o id
           o name
           o facts
           o metrics
           o vds
           o encls
+          o drives_ids
           o create_vd
     * Controllers
           o Controllers
           o ids
           o get_ctl
     * Enclosure
           o Enclosure
@@ -175,15 +176,15 @@
 14from .drive import DriveState, Drive, Drives
 15from .virtualdrive import VirtualDrive, VirtualDrives
 16
 17__all__ = ['__version__', 'StorCLI', 'Controller', 'Controllers',
 18           'Enclosure', 'Enclosures', 'DriveState', 'Drive', 'Drives',
 'VirtualDrive', 'VirtualDrives']
 
-__version__ = '0.6.0'
+__version__ = '0.6.1.dev6'
    ⁰
 class StorCLI: View Source
 _27class StorCLI(object):
 _28    """StorCLI command line wrapper
 _29
 _30    Instance of this class is storcli command line wrapper
 _31
@@ -741,71 +742,82 @@
 273    @property
 274    def encls(self):
 275        """(:obj:enclosure.Enclosures): controller enclosures
 276        """
 277        return enclosure.Enclosures(ctl_id=self._ctl_id,
 binary=self._binary)
 278
-279    def create_vd(self, name: str, raid: str, drives: str, strip: str =
+279    @property
+280    def drives_ids(self) -> List[str]:
+281        """(list of str): list of drives ids in format (e:s)
+282        """
+283        drives = []
+284        for encl in self.encls:
+285            for id in encl.drives.ids:
+286                drives.append("{enc}:{id}".format(enc=encl.id, id=id))
+287
+288        return drives
+289
+290    def create_vd(self, name: str, raid: str, drives: str, strip: str =
 '64', PDperArray: Optional[int] = None) -> Optional[virtualdrive.VirtualDrive]:
-280        """Create virtual drive (raid) managed by current controller
-281
-282        Args:
-283            name (str): virtual drive name
-284            raid (str): virtual drive raid level (raid0, raid1, ...)
-285            drives (str): storcli drives expression (e:s|e:s-x|e:s-x,y;e:s-
+291        """Create virtual drive (raid) managed by current controller
+292
+293        Args:
+294            name (str): virtual drive name
+295            raid (str): virtual drive raid level (raid0, raid1, ...)
+296            drives (str): storcli drives expression (e:s|e:s-x|e:s-x,y;e:s-
 x,y,z)
-286            strip (str, optional): virtual drive raid strip size
-287
-288        Returns:
-289            (None): no virtual drive created with name
-290            (:obj:virtualdrive.VirtualDrive)
-291        """
-292        args = [
-293            'add',
-294            'vd',
-295            'r{0}'.format(raid),
-296            'name={0}'.format(name),
-297            'drives={0}'.format(drives),
-298            'strip={0}'.format(strip)
-299        ]
-300
-301        try:
-302            if int(raid) >= 10 and PDperArray is None:
-303                # Try to count the number of drives in the array
-304                # The format of the drives argument is e:s|e:s-x|e:s-x,y;e:
+297            strip (str, optional): virtual drive raid strip size
+298
+299        Returns:
+300            (None): no virtual drive created with name
+301            (:obj:virtualdrive.VirtualDrive)
+302        """
+303        args = [
+304            'add',
+305            'vd',
+306            'r{0}'.format(raid),
+307            'name={0}'.format(name),
+308            'drives={0}'.format(drives),
+309            'strip={0}'.format(strip)
+310        ]
+311
+312        try:
+313            if int(raid) >= 10 and PDperArray is None:
+314                # Try to count the number of drives in the array
+315                # The format of the drives argument is e:s|e:s-x|e:s-x,y;e:
 s-x,y,z
-305                # The number of drives is the number of commas plus the
-dashes intervals
-306
-307                numDrives = 0
-308                drives2 = drives.split(':')
-309                drives2 = drives2[1]
-310                numDrives += drives2.count(',')+1
-311                for interval in drives2.split(','):
-312                    if '-' in interval:
-313                        left = int(interval.split('-')[0])
-314                        right = int(interval.split('-')[1])
-315                        numDrives += right - left
 316
-317                PDperArray = numDrives//2
-318        except ValueError:
-319            pass
-320
-321        if raid == '00' and PDperArray is None:
-322            PDperArray = 1
-323
-324        if PDperArray is not None:
-325            args.append('PDperArray={0}'.format(PDperArray))
+317                numDrives = common.count_drives(drives)
+318
+319                if numDrives % 2 != 0 and numDrives % 3 == 0:
+320                    # In some scenarios, such as 9 drives with raid 60, 3 is
+a good pd number but 4 is not
+321                    # Must check for similar scenarios
+322                    # BTW we don't clearly understand what PDperArray is for
+and what exactly it does under the hood. More investigation is needed
+323                    PDperArray = numDrives//3
+324                else:
+325                    PDperArray = numDrives//2
 326
-327        self._run(args)
-328        for vd in self.vds:
-329            if name == vd.name:
-330                return vd
-331        return None
+327        except ValueError:
+328            pass
+329
+330        finally:
+331            if raid == '00' and PDperArray is None:
+332                PDperArray = 1
+333
+334        if PDperArray is not None:
+335            args.append('PDperArray={0}'.format(PDperArray))
+336
+337        self._run(args)
+338        for vd in self.vds:
+339            if name == vd.name:
+340                return vd
+341        return None
 StorCLI Controller
 Instance of this class represents controller in StorCLI hierarchy
 Args: ctl_id (str): controller id binary (str): storcli binary or full path to
 the binary
 Properties: id (str): controller id name (str): controller cmd name facts
 (dict): raw controller facts metrics (:obj:ControllerMetrics): controller
 metrics vds (list of :obj:virtualdrive.VirtualDrives): controller virtual
@@ -837,187 +849,189 @@
 (dict): raw controller facts
 metrics
 (:obj:ControllerMetrics): controller metrics
 vds
 (:obj:virtualdrive.VirtualDrives): controllers virtual drives
 encls
 (:obj:enclosure.Enclosures): controller enclosures
+drives_ids: List[str]
+(list of str): list of drives ids in format (e:s)
 ⁰
 def create_vd(
 self,
 name: str,
 raid: str,
 drives: str,
 strip: str = '64',
 PDperArray: Optional[int] = None) -> Optional[pystorcli2.VirtualDrive]: View
 Source
-279    def create_vd(self, name: str, raid: str, drives: str, strip: str =
+290    def create_vd(self, name: str, raid: str, drives: str, strip: str =
 '64', PDperArray: Optional[int] = None) -> Optional[virtualdrive.VirtualDrive]:
-280        """Create virtual drive (raid) managed by current controller
-281
-282        Args:
-283            name (str): virtual drive name
-284            raid (str): virtual drive raid level (raid0, raid1, ...)
-285            drives (str): storcli drives expression (e:s|e:s-x|e:s-x,y;e:s-
+291        """Create virtual drive (raid) managed by current controller
+292
+293        Args:
+294            name (str): virtual drive name
+295            raid (str): virtual drive raid level (raid0, raid1, ...)
+296            drives (str): storcli drives expression (e:s|e:s-x|e:s-x,y;e:s-
 x,y,z)
-286            strip (str, optional): virtual drive raid strip size
-287
-288        Returns:
-289            (None): no virtual drive created with name
-290            (:obj:virtualdrive.VirtualDrive)
-291        """
-292        args = [
-293            'add',
-294            'vd',
-295            'r{0}'.format(raid),
-296            'name={0}'.format(name),
-297            'drives={0}'.format(drives),
-298            'strip={0}'.format(strip)
-299        ]
-300
-301        try:
-302            if int(raid) >= 10 and PDperArray is None:
-303                # Try to count the number of drives in the array
-304                # The format of the drives argument is e:s|e:s-x|e:s-x,y;e:
+297            strip (str, optional): virtual drive raid strip size
+298
+299        Returns:
+300            (None): no virtual drive created with name
+301            (:obj:virtualdrive.VirtualDrive)
+302        """
+303        args = [
+304            'add',
+305            'vd',
+306            'r{0}'.format(raid),
+307            'name={0}'.format(name),
+308            'drives={0}'.format(drives),
+309            'strip={0}'.format(strip)
+310        ]
+311
+312        try:
+313            if int(raid) >= 10 and PDperArray is None:
+314                # Try to count the number of drives in the array
+315                # The format of the drives argument is e:s|e:s-x|e:s-x,y;e:
 s-x,y,z
-305                # The number of drives is the number of commas plus the
-dashes intervals
-306
-307                numDrives = 0
-308                drives2 = drives.split(':')
-309                drives2 = drives2[1]
-310                numDrives += drives2.count(',')+1
-311                for interval in drives2.split(','):
-312                    if '-' in interval:
-313                        left = int(interval.split('-')[0])
-314                        right = int(interval.split('-')[1])
-315                        numDrives += right - left
 316
-317                PDperArray = numDrives//2
-318        except ValueError:
-319            pass
-320
-321        if raid == '00' and PDperArray is None:
-322            PDperArray = 1
-323
-324        if PDperArray is not None:
-325            args.append('PDperArray={0}'.format(PDperArray))
+317                numDrives = common.count_drives(drives)
+318
+319                if numDrives % 2 != 0 and numDrives % 3 == 0:
+320                    # In some scenarios, such as 9 drives with raid 60, 3 is
+a good pd number but 4 is not
+321                    # Must check for similar scenarios
+322                    # BTW we don't clearly understand what PDperArray is for
+and what exactly it does under the hood. More investigation is needed
+323                    PDperArray = numDrives//3
+324                else:
+325                    PDperArray = numDrives//2
 326
-327        self._run(args)
-328        for vd in self.vds:
-329            if name == vd.name:
-330                return vd
-331        return None
+327        except ValueError:
+328            pass
+329
+330        finally:
+331            if raid == '00' and PDperArray is None:
+332                PDperArray = 1
+333
+334        if PDperArray is not None:
+335            args.append('PDperArray={0}'.format(PDperArray))
+336
+337        self._run(args)
+338        for vd in self.vds:
+339            if name == vd.name:
+340                return vd
+341        return None
 Create virtual drive (raid) managed by current controller
 Args: name (str): virtual drive name raid (str): virtual drive raid level
 (raid0, raid1, ...) drives (str): storcli drives expression (e:s|e:s-x|e:s-
 x,y;e:s-x,y,z) strip (str, optional): virtual drive raid strip size
 Returns: (None): no virtual drive created with name (:obj:
 virtualdrive.VirtualDrive)
   ⁰
 class Controllers: View Source
-334class Controllers(object):
-335    """StorCLI Controllers
-336
-337    Instance of this class is iterable with :obj:Controller as item
-338
-339    Args:
-340        binary (str): storcli binary or full path to the binary
-341
-342    Properties:
-343        ids (list of str): list of controllers id
-344
-345    Methods:
-346        get_clt (:obj:Controller): return controller object by id
-347    """
+344class Controllers(object):
+345    """StorCLI Controllers
+346
+347    Instance of this class is iterable with :obj:Controller as item
 348
-349    def __init__(self, binary='storcli64'):
-350        """Constructor - create StorCLI Controllers object
+349    Args:
+350        binary (str): storcli binary or full path to the binary
 351
-352        Args:
-353            binary (str): storcli binary or full path to the binary
-354        """
-355        self._binary = binary
-356        self._storcli = StorCLI(binary)
-357
-358    @ property
-359    def _ctl_ids(self) -> List[str]:
-360        out = self._storcli.run(['show'])
-361        response = common.response_data(out)
-362
-363        if "Number of Controllers" in response and response["Number of
-Controllers"] == 0:
-364            return []
-365        else:
-366            return [ctl['Ctl'] for ctl in common.response_data_subkey(out,
-['System Overview', 'IT System Overview'])]
+352    Properties:
+353        ids (list of str): list of controllers id
+354
+355    Methods:
+356        get_clt (:obj:Controller): return controller object by id
+357    """
+358
+359    def __init__(self, binary='storcli64'):
+360        """Constructor - create StorCLI Controllers object
+361
+362        Args:
+363            binary (str): storcli binary or full path to the binary
+364        """
+365        self._binary = binary
+366        self._storcli = StorCLI(binary)
 367
 368    @ property
-369    def _ctls(self):
-370        for ctl_id in self._ctl_ids:
-371            yield Controller(ctl_id=ctl_id, binary=self._binary)
+369    def _ctl_ids(self) -> List[str]:
+370        out = self._storcli.run(['show'])
+371        response = common.response_data(out)
 372
-373    def __iter__(self):
-374        return self._ctls
-375
-376    @ property
-377    def ids(self):
-378        """(list of str): controllers id
-379        """
-380        return self._ctl_ids
-381
-382    def get_ctl(self, ctl_id: int) -> Optional[Controller]:
-383        """Get controller object by id
-384
-385        Args:
-386            ctl_id (str): controller id
-387
-388        Returns:
-389            (None): no controller with id
-390            (:obj:Controller): controller object
-391        """
-392        for ctl in self:
-393            if ctl.id == ctl_id:
-394                return ctl
-395        return None
+373        if "Number of Controllers" in response and response["Number of
+Controllers"] == 0:
+374            return []
+375        else:
+376            return [ctl['Ctl'] for ctl in common.response_data_subkey(out,
+['System Overview', 'IT System Overview'])]
+377
+378    @ property
+379    def _ctls(self):
+380        for ctl_id in self._ctl_ids:
+381            yield Controller(ctl_id=ctl_id, binary=self._binary)
+382
+383    def __iter__(self):
+384        return self._ctls
+385
+386    @ property
+387    def ids(self):
+388        """(list of str): controllers id
+389        """
+390        return self._ctl_ids
+391
+392    def get_ctl(self, ctl_id: int) -> Optional[Controller]:
+393        """Get controller object by id
+394
+395        Args:
+396            ctl_id (str): controller id
+397
+398        Returns:
+399            (None): no controller with id
+400            (:obj:Controller): controller object
+401        """
+402        for ctl in self:
+403            if ctl.id == ctl_id:
+404                return ctl
+405        return None
 StorCLI Controllers
 Instance of this class is iterable with :obj:Controller as item
 Args: binary (str): storcli binary or full path to the binary
 Properties: ids (list of str): list of controllers id
 Methods: get_clt (:obj:Controller): return controller object by id
 ⁰
 Controllers(binary='storcli64') View Source
-349    def __init__(self, binary='storcli64'):
-350        """Constructor - create StorCLI Controllers object
-351
-352        Args:
-353            binary (str): storcli binary or full path to the binary
-354        """
-355        self._binary = binary
-356        self._storcli = StorCLI(binary)
+359    def __init__(self, binary='storcli64'):
+360        """Constructor - create StorCLI Controllers object
+361
+362        Args:
+363            binary (str): storcli binary or full path to the binary
+364        """
+365        self._binary = binary
+366        self._storcli = StorCLI(binary)
 Constructor - create StorCLI Controllers object
 Args: binary (str): storcli binary or full path to the binary
 ids
 (list of str): controllers id
 ⁰
 def get_ctl(self, ctl_id: int) -> Optional[pystorcli2.Controller]: View Source
-382    def get_ctl(self, ctl_id: int) -> Optional[Controller]:
-383        """Get controller object by id
-384
-385        Args:
-386            ctl_id (str): controller id
-387
-388        Returns:
-389            (None): no controller with id
-390            (:obj:Controller): controller object
-391        """
-392        for ctl in self:
-393            if ctl.id == ctl_id:
-394                return ctl
-395        return None
+392    def get_ctl(self, ctl_id: int) -> Optional[Controller]:
+393        """Get controller object by id
+394
+395        Args:
+396            ctl_id (str): controller id
+397
+398        Returns:
+399            (None): no controller with id
+400            (:obj:Controller): controller object
+401        """
+402        for ctl in self:
+403            if ctl.id == ctl_id:
+404                return ctl
+405        return None
 Get controller object by id
 Args: ctl_id (str): controller id
 Returns: (None): no controller with id (:obj:Controller): controller object
   ⁰
 class Enclosure: View Source
 _20class Enclosure(object):
 _21    """StorCLI enclosure
```

### Comparing `PyStorCLI2-0.6.0/docs/search.js` & `PyStorCLI2-0.6.1.dev6/docs/search.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -863,14 +863,22 @@
                 "pystorcli2.Controller.encls": {
                     "fullname": "pystorcli2.Controller.encls",
                     "modulename": "pystorcli2",
                     "qualname": "Controller.encls",
                     "kind": "variable",
                     "doc": "<p>(:obj:enclosure.Enclosures): controller enclosures</p>\n"
                 },
+                "pystorcli2.Controller.drives_ids": {
+                    "fullname": "pystorcli2.Controller.drives_ids",
+                    "modulename": "pystorcli2",
+                    "qualname": "Controller.drives_ids",
+                    "kind": "variable",
+                    "doc": "<p>(list of str): list of drives ids in format (e:s)</p>\n",
+                    "annotation": ": List[str]"
+                },
                 "pystorcli2.Controller.create_vd": {
                     "fullname": "pystorcli2.Controller.create_vd",
                     "modulename": "pystorcli2",
                     "qualname": "Controller.create_vd",
                     "kind": "function",
                     "doc": "<p>Create virtual drive (raid) managed by current controller</p>\n\n<p>Args:\n    name (str): virtual drive name\n    raid (str): virtual drive raid level (raid0, raid1, ...)\n    drives (str): storcli drives expression (e:s|e:s-x|e:s-x,y;e:s-x,y,z)\n    strip (str, optional): virtual drive raid strip size</p>\n\n<p>Returns:\n    (None): no virtual drive created with name\n    (:obj:virtualdrive.VirtualDrive)</p>\n",
                     "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">name</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"n\">raid</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"n\">drives</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"n\">strip</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;64&#39;</span>,</span><span class=\"param\">\t<span class=\"n\">PDperArray</span><span class=\"p\">:</span> <span class=\"n\">Optional</span><span class=\"p\">[</span><span class=\"nb\">int</span><span class=\"p\">]</span> <span class=\"o\">=</span> <span class=\"kc\">None</span></span><span class=\"return-annotation\">) -> <span class=\"n\">Optional</span><span class=\"p\">[</span><span class=\"n\">pystorcli2</span><span class=\"o\">.</span><span class=\"n\">virtualdrive</span><span class=\"o\">.</span><span class=\"n\">VirtualDrive</span><span class=\"p\">]</span>:</span></span>",
@@ -2060,14 +2068,23 @@
                     "fullname": 3,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 0,
                     "bases": 0,
                     "doc": 8
                 },
+                "pystorcli2.Controller.drives_ids": {
+                    "qualname": 3,
+                    "fullname": 4,
+                    "annotation": 2,
+                    "default_value": 0,
+                    "signature": 0,
+                    "bases": 0,
+                    "doc": 15
+                },
                 "pystorcli2.Controller.create_vd": {
                     "qualname": 3,
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 110,
                     "bases": 0,
@@ -3213,15 +3230,15 @@
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 17,
                     "bases": 0,
                     "doc": 33
                 }
             },
-            "length": 151,
+            "length": 152,
             "save": true
         },
         "index": {
             "qualname": {
                 "root": {
                     "docs": {
                         "pystorcli2.StorCLI.__init__": {
@@ -3764,14 +3781,17 @@
                                 "pystorcli2.VirtualDrives.ctl_id": {
                                     "tf": 1
                                 }
                             },
                             "df": 13,
                             "s": {
                                 "docs": {
+                                    "pystorcli2.Controller.drives_ids": {
+                                        "tf": 1
+                                    },
                                     "pystorcli2.Controllers.ids": {
                                         "tf": 1
                                     },
                                     "pystorcli2.Enclosures.ids": {
                                         "tf": 1
                                     },
                                     "pystorcli2.Drives.ids": {
@@ -3780,15 +3800,15 @@
                                     "pystorcli2.Drives.get_drive_range_ids": {
                                         "tf": 1
                                     },
                                     "pystorcli2.VirtualDrives.ids": {
                                         "tf": 1
                                     }
                                 },
-                                "df": 5
+                                "df": 6
                             }
                         },
                         "o": {
                             "docs": {},
                             "df": 0,
                             "p": {
                                 "docs": {},
@@ -3971,19 +3991,22 @@
                                                                 },
                                                                 "pystorcli2.Controller.vds": {
                                                                     "tf": 1
                                                                 },
                                                                 "pystorcli2.Controller.encls": {
                                                                     "tf": 1
                                                                 },
+                                                                "pystorcli2.Controller.drives_ids": {
+                                                                    "tf": 1
+                                                                },
                                                                 "pystorcli2.Controller.create_vd": {
                                                                     "tf": 1
                                                                 }
                                                             },
-                                                            "df": 9,
+                                                            "df": 10,
                                                             "s": {
                                                                 "docs": {
                                                                     "pystorcli2.StorCLI.controllers": {
                                                                         "tf": 1
                                                                     },
                                                                     "pystorcli2.Controllers": {
                                                                         "tf": 1
@@ -4713,14 +4736,17 @@
                                             "pystorcli2.Drives.get_drive_range": {
                                                 "tf": 1
                                             }
                                         },
                                         "df": 37,
                                         "s": {
                                             "docs": {
+                                                "pystorcli2.Controller.drives_ids": {
+                                                    "tf": 1
+                                                },
                                                 "pystorcli2.Enclosure.has_drives": {
                                                     "tf": 1
                                                 },
                                                 "pystorcli2.Enclosure.drives": {
                                                     "tf": 1
                                                 },
                                                 "pystorcli2.Drives": {
@@ -4753,15 +4779,15 @@
                                                 "pystorcli2.Drives.get_drive_range": {
                                                     "tf": 1
                                                 },
                                                 "pystorcli2.VirtualDrive.drives": {
                                                     "tf": 1
                                                 }
                                             },
-                                            "df": 13,
+                                            "df": 14,
                                             "t": {
                                                 "docs": {},
                                                 "df": 0,
                                                 "a": {
                                                     "docs": {},
                                                     "df": 0,
                                                     "t": {
@@ -6162,14 +6188,17 @@
                                                                 },
                                                                 "pystorcli2.Controller.vds": {
                                                                     "tf": 1
                                                                 },
                                                                 "pystorcli2.Controller.encls": {
                                                                     "tf": 1
                                                                 },
+                                                                "pystorcli2.Controller.drives_ids": {
+                                                                    "tf": 1
+                                                                },
                                                                 "pystorcli2.Controller.create_vd": {
                                                                     "tf": 1
                                                                 },
                                                                 "pystorcli2.Controllers": {
                                                                     "tf": 1
                                                                 },
                                                                 "pystorcli2.Controllers.__init__": {
@@ -6547,15 +6576,15 @@
                                                                 "pystorcli2.VirtualDrives.get_vd": {
                                                                     "tf": 1
                                                                 },
                                                                 "pystorcli2.VirtualDrives.get_named_vd": {
                                                                     "tf": 1
                                                                 }
                                                             },
-                                                            "df": 151
+                                                            "df": 152
                                                         },
                                                         "docs": {},
                                                         "df": 0
                                                     }
                                                 }
                                             }
                                         }
@@ -7202,14 +7231,17 @@
                                 "pystorcli2.VirtualDrives.ctl_id": {
                                     "tf": 1
                                 }
                             },
                             "df": 13,
                             "s": {
                                 "docs": {
+                                    "pystorcli2.Controller.drives_ids": {
+                                        "tf": 1
+                                    },
                                     "pystorcli2.Controllers.ids": {
                                         "tf": 1
                                     },
                                     "pystorcli2.Enclosures.ids": {
                                         "tf": 1
                                     },
                                     "pystorcli2.Drives.ids": {
@@ -7218,15 +7250,15 @@
                                     "pystorcli2.Drives.get_drive_range_ids": {
                                         "tf": 1
                                     },
                                     "pystorcli2.VirtualDrives.ids": {
                                         "tf": 1
                                     }
                                 },
-                                "df": 5
+                                "df": 6
                             }
                         },
                         "o": {
                             "docs": {},
                             "df": 0,
                             "p": {
                                 "docs": {},
@@ -7409,19 +7441,22 @@
                                                                 },
                                                                 "pystorcli2.Controller.vds": {
                                                                     "tf": 1
                                                                 },
                                                                 "pystorcli2.Controller.encls": {
                                                                     "tf": 1
                                                                 },
+                                                                "pystorcli2.Controller.drives_ids": {
+                                                                    "tf": 1
+                                                                },
                                                                 "pystorcli2.Controller.create_vd": {
                                                                     "tf": 1
                                                                 }
                                                             },
-                                                            "df": 9,
+                                                            "df": 10,
                                                             "s": {
                                                                 "docs": {
                                                                     "pystorcli2.StorCLI.controllers": {
                                                                         "tf": 1
                                                                     },
                                                                     "pystorcli2.Controllers": {
                                                                         "tf": 1
@@ -8151,14 +8186,17 @@
                                             "pystorcli2.Drives.get_drive_range": {
                                                 "tf": 1
                                             }
                                         },
                                         "df": 37,
                                         "s": {
                                             "docs": {
+                                                "pystorcli2.Controller.drives_ids": {
+                                                    "tf": 1
+                                                },
                                                 "pystorcli2.Enclosure.has_drives": {
                                                     "tf": 1
                                                 },
                                                 "pystorcli2.Enclosure.drives": {
                                                     "tf": 1
                                                 },
                                                 "pystorcli2.Drives": {
@@ -8191,15 +8229,15 @@
                                                 "pystorcli2.Drives.get_drive_range": {
                                                     "tf": 1
                                                 },
                                                 "pystorcli2.VirtualDrive.drives": {
                                                     "tf": 1
                                                 }
                                             },
-                                            "df": 13,
+                                            "df": 14,
                                             "t": {
                                                 "docs": {},
                                                 "df": 0,
                                                 "a": {
                                                     "docs": {},
                                                     "df": 0,
                                                     "t": {
@@ -9353,14 +9391,17 @@
                         },
                         "pystorcli2.StorCLI.version": {
                             "tf": 1
                         },
                         "pystorcli2.StorCLI.controllers": {
                             "tf": 1
                         },
+                        "pystorcli2.Controller.drives_ids": {
+                            "tf": 1
+                        },
                         "pystorcli2.Enclosure.id": {
                             "tf": 1
                         },
                         "pystorcli2.Enclosure.name": {
                             "tf": 1
                         },
                         "pystorcli2.Enclosure.ctl_id": {
@@ -9393,15 +9434,15 @@
                         "pystorcli2.Drives.ctl_id": {
                             "tf": 1
                         },
                         "pystorcli2.Drives.encl_id": {
                             "tf": 1
                         }
                     },
-                    "df": 16,
+                    "df": 17,
                     "s": {
                         "docs": {},
                         "df": 0,
                         "t": {
                             "docs": {},
                             "df": 0,
                             "r": {
@@ -9518,14 +9559,69 @@
                                             }
                                         }
                                     }
                                 }
                             }
                         }
                     },
+                    "l": {
+                        "docs": {},
+                        "df": 0,
+                        "i": {
+                            "docs": {},
+                            "df": 0,
+                            "s": {
+                                "docs": {},
+                                "df": 0,
+                                "t": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "[": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "s": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "t": {
+                                                "docs": {},
+                                                "df": 0,
+                                                "r": {
+                                                    "docs": {
+                                                        "pystorcli2.Controller.drives_ids": {
+                                                            "tf": 1
+                                                        }
+                                                    },
+                                                    "df": 1
+                                                }
+                                            }
+                                        },
+                                        "i": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "n": {
+                                                "docs": {},
+                                                "df": 0,
+                                                "t": {
+                                                    "docs": {
+                                                        "pystorcli2.Enclosures.ids": {
+                                                            "tf": 1
+                                                        },
+                                                        "pystorcli2.Drives.ids": {
+                                                            "tf": 1
+                                                        }
+                                                    },
+                                                    "df": 2
+                                                }
+                                            }
+                                        }
+                                    }
+                                }
+                            }
+                        }
+                    },
                     "i": {
                         "docs": {},
                         "df": 0,
                         "n": {
                             "docs": {},
                             "df": 0,
                             "t": {
@@ -9621,53 +9717,14 @@
                                             }
                                         }
                                     }
                                 }
                             }
                         }
                     },
-                    "l": {
-                        "docs": {},
-                        "df": 0,
-                        "i": {
-                            "docs": {},
-                            "df": 0,
-                            "s": {
-                                "docs": {},
-                                "df": 0,
-                                "t": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "[": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "i": {
-                                            "docs": {},
-                                            "df": 0,
-                                            "n": {
-                                                "docs": {},
-                                                "df": 0,
-                                                "t": {
-                                                    "docs": {
-                                                        "pystorcli2.Enclosures.ids": {
-                                                            "tf": 1
-                                                        },
-                                                        "pystorcli2.Drives.ids": {
-                                                            "tf": 1
-                                                        }
-                                                    },
-                                                    "df": 2
-                                                }
-                                            }
-                                        }
-                                    }
-                                }
-                            }
-                        }
-                    },
                     "o": {
                         "docs": {},
                         "df": 0,
                         "p": {
                             "docs": {},
                             "df": 0,
                             "t": {
@@ -12869,14 +12926,17 @@
                         },
                         "pystorcli2.Controller.vds": {
                             "tf": 2
                         },
                         "pystorcli2.Controller.encls": {
                             "tf": 2
                         },
+                        "pystorcli2.Controller.drives_ids": {
+                            "tf": 2.23606797749979
+                        },
                         "pystorcli2.Controller.create_vd": {
                             "tf": 3.4641016151377544
                         },
                         "pystorcli2.Controllers": {
                             "tf": 3.605551275463989
                         },
                         "pystorcli2.Controllers.__init__": {
@@ -13254,15 +13314,15 @@
                         "pystorcli2.VirtualDrives.get_vd": {
                             "tf": 3
                         },
                         "pystorcli2.VirtualDrives.get_named_vd": {
                             "tf": 3
                         }
                     },
-                    "df": 151,
+                    "df": 152,
                     "s": {
                         "docs": {
                             "pystorcli2.Drive.erase_start": {
                                 "tf": 1
                             },
                             "pystorcli2.VirtualDrive.erase_start": {
                                 "tf": 1
@@ -13576,14 +13636,17 @@
                                     },
                                     "pystorcli2.Controller.id": {
                                         "tf": 1
                                     },
                                     "pystorcli2.Controller.name": {
                                         "tf": 1
                                     },
+                                    "pystorcli2.Controller.drives_ids": {
+                                        "tf": 1
+                                    },
                                     "pystorcli2.Controller.create_vd": {
                                         "tf": 2
                                     },
                                     "pystorcli2.Controllers": {
                                         "tf": 1.4142135623730951
                                     },
                                     "pystorcli2.Controllers.__init__": {
@@ -13778,15 +13841,15 @@
                                     "pystorcli2.VirtualDrives.get_vd": {
                                         "tf": 1
                                     },
                                     "pystorcli2.VirtualDrives.get_named_vd": {
                                         "tf": 1
                                     }
                                 },
-                                "df": 75,
+                                "df": 76,
                                 "i": {
                                     "docs": {},
                                     "df": 0,
                                     "p": {
                                         "docs": {
                                             "pystorcli2.Controller.create_vd": {
                                                 "tf": 1.4142135623730951
@@ -17154,14 +17217,17 @@
                                         },
                                         "pystorcli2.StorCLI.controllers": {
                                             "tf": 1
                                         },
                                         "pystorcli2.Controller": {
                                             "tf": 1
                                         },
+                                        "pystorcli2.Controller.drives_ids": {
+                                            "tf": 1.4142135623730951
+                                        },
                                         "pystorcli2.Controllers": {
                                             "tf": 1.4142135623730951
                                         },
                                         "pystorcli2.Controllers.ids": {
                                             "tf": 1
                                         },
                                         "pystorcli2.Enclosure": {
@@ -17197,15 +17263,15 @@
                                         "pystorcli2.VirtualDrives": {
                                             "tf": 1.4142135623730951
                                         },
                                         "pystorcli2.VirtualDrives.ids": {
                                             "tf": 1.4142135623730951
                                         }
                                     },
-                                    "df": 18
+                                    "df": 19
                                 }
                             }
                         },
                         "e": {
                             "docs": {},
                             "df": 0,
                             "v": {
@@ -17586,14 +17652,17 @@
                             "docs": {
                                 "pystorcli2.StorCLI.version": {
                                     "tf": 1
                                 },
                                 "pystorcli2.Controller": {
                                     "tf": 1
                                 },
+                                "pystorcli2.Controller.drives_ids": {
+                                    "tf": 1
+                                },
                                 "pystorcli2.Enclosure": {
                                     "tf": 1
                                 },
                                 "pystorcli2.Drive": {
                                     "tf": 1
                                 },
                                 "pystorcli2.Drives": {
@@ -17614,15 +17683,15 @@
                                 "pystorcli2.VirtualDrive.erase_progress": {
                                     "tf": 1.4142135623730951
                                 },
                                 "pystorcli2.VirtualDrive.migrate_start": {
                                     "tf": 1.4142135623730951
                                 }
                             },
-                            "df": 11,
+                            "df": 12,
                             "s": {
                                 "docs": {},
                                 "df": 0,
                                 "t": {
                                     "docs": {},
                                     "df": 0,
                                     "a": {
@@ -18167,28 +18236,31 @@
                                 "pystorcli2.VirtualDrives.get_vd": {
                                     "tf": 2
                                 }
                             },
                             "df": 38,
                             "s": {
                                 "docs": {
+                                    "pystorcli2.Controller.drives_ids": {
+                                        "tf": 1
+                                    },
                                     "pystorcli2.Controllers": {
                                         "tf": 1
                                     },
                                     "pystorcli2.Enclosures": {
                                         "tf": 1
                                     },
                                     "pystorcli2.Drives": {
                                         "tf": 1.7320508075688772
                                     },
                                     "pystorcli2.VirtualDrives": {
                                         "tf": 1
                                     }
                                 },
-                                "df": 4
+                                "df": 5
                             }
                         },
                         "t": {
                             "docs": {
                                 "pystorcli2.Drive.spin": {
                                     "tf": 1
                                 },
@@ -18330,14 +18402,17 @@
                                 },
                                 "pystorcli2.StorCLI.controllers": {
                                     "tf": 1
                                 },
                                 "pystorcli2.Controller": {
                                     "tf": 1.4142135623730951
                                 },
+                                "pystorcli2.Controller.drives_ids": {
+                                    "tf": 1.4142135623730951
+                                },
                                 "pystorcli2.Controllers": {
                                     "tf": 1.7320508075688772
                                 },
                                 "pystorcli2.Controllers.ids": {
                                     "tf": 1
                                 },
                                 "pystorcli2.Enclosure": {
@@ -18415,15 +18490,15 @@
                                 "pystorcli2.VirtualDrives": {
                                     "tf": 1.7320508075688772
                                 },
                                 "pystorcli2.VirtualDrives.ids": {
                                     "tf": 1.4142135623730951
                                 }
                             },
-                            "df": 33,
+                            "df": 34,
                             "f": {
                                 "docs": {
                                     "pystorcli2.VirtualDrive.bootdrive": {
                                         "tf": 1.4142135623730951
                                     },
                                     "pystorcli2.VirtualDrive.pdcache": {
                                         "tf": 1.4142135623730951
@@ -21159,25 +21234,28 @@
                                     "docs": {},
                                     "df": 0,
                                     "a": {
                                         "docs": {},
                                         "df": 0,
                                         "t": {
                                             "docs": {
+                                                "pystorcli2.Controller.drives_ids": {
+                                                    "tf": 1
+                                                },
                                                 "pystorcli2.Drives.get_drive_range_ids": {
                                                     "tf": 1
                                                 },
                                                 "pystorcli2.Drives.get_drive_range": {
                                                     "tf": 1
                                                 },
                                                 "pystorcli2.VirtualDrive.migrate_start": {
                                                     "tf": 1
                                                 }
                                             },
-                                            "df": 3
+                                            "df": 4
                                         }
                                     }
                                 },
                                 "c": {
                                     "docs": {},
                                     "df": 0,
                                     "e": {
@@ -21911,19 +21989,22 @@
                             }
                         },
                         ":": {
                             "docs": {},
                             "df": 0,
                             "s": {
                                 "docs": {
+                                    "pystorcli2.Controller.drives_ids": {
+                                        "tf": 1
+                                    },
                                     "pystorcli2.Controller.create_vd": {
                                         "tf": 1
                                     }
                                 },
-                                "df": 1,
+                                "df": 2,
                                 "|": {
                                     "docs": {},
                                     "df": 0,
                                     "e": {
                                         "docs": {},
                                         "df": 0,
                                         ":": {
@@ -22526,14 +22607,17 @@
                                             "docs": {
                                                 "pystorcli2.Controller": {
                                                     "tf": 1
                                                 },
                                                 "pystorcli2.Controller.vds": {
                                                     "tf": 1
                                                 },
+                                                "pystorcli2.Controller.drives_ids": {
+                                                    "tf": 1
+                                                },
                                                 "pystorcli2.Controller.create_vd": {
                                                     "tf": 1.4142135623730951
                                                 },
                                                 "pystorcli2.Enclosure": {
                                                     "tf": 2
                                                 },
                                                 "pystorcli2.Enclosure.has_drives": {
@@ -22575,15 +22659,15 @@
                                                 "pystorcli2.VirtualDrives.ctl": {
                                                     "tf": 1
                                                 },
                                                 "pystorcli2.VirtualDrives.has_vds": {
                                                     "tf": 1
                                                 }
                                             },
-                                            "df": 18,
+                                            "df": 19,
                                             "t": {
                                                 "docs": {},
                                                 "df": 0,
                                                 "a": {
                                                     "docs": {},
                                                     "df": 0,
                                                     "t": {
```

### Comparing `PyStorCLI2-0.6.0/pyproject.toml` & `PyStorCLI2-0.6.1.dev6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/pystorcli/__init__.py` & `PyStorCLI2-0.6.1.dev6/pystorcli/__init__.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/pystorcli/cachevault.py` & `PyStorCLI2-0.6.1.dev6/pystorcli/cachevault.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/pystorcli/cmdRunner.py` & `PyStorCLI2-0.6.1.dev6/pystorcli/cmdRunner.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/pystorcli/common.py` & `PyStorCLI2-0.6.1.dev6/pystorcli/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -217,7 +217,58 @@
             if range_sep_t == 'end':
                 break
         else:
             # enclosure
             drives.extend(drives_from_expression(expr[pos:]))
             break
     return drives
+
+
+def expand_drive_ids(drives: str) -> str:
+    """Expand drive ids to range if needed
+
+    Args:
+        drives (str): storcli drives expression (e:s|e:s-x|e:s-x,y;e:s-x,y,z)
+
+    Returns:
+        (str): expanded drives expression (without dashes)
+    """
+    drive_list = drives.split(',')
+    output = ""
+
+    for i, drive in enumerate(drive_list):
+        drive = drive.strip()
+        encl, slot = drive.split(':')
+        new_output = drive
+
+        encl = encl.strip()
+        slot = slot.strip()
+
+        if '-' in slot:
+            begin, end = slot.split('-')
+
+            begin = begin.strip()
+            end = end.strip()
+
+            new_output = ','.join(['{0}:{1}'.format(encl, i)
+                                   for i in range(int(begin), int(end)+1)])
+
+        if i > 0:
+            output += ',' + new_output
+        else:
+            output += new_output
+
+    return output
+
+
+def count_drives(drives: str) -> int:
+    """Count number of drives in drives expression
+
+    Args:
+        drives (str): storcli drives expression (e:s|e:s-x|e:s-x,y;e:s-x,y,z)
+
+    Returns:
+        (int): number of drives
+    """
+
+    expanded_drives = expand_drive_ids(drives)
+    return len(expanded_drives.split(','))
```

### Comparing `PyStorCLI2-0.6.0/pystorcli/controller.py` & `PyStorCLI2-0.6.1.dev6/pystorcli/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -271,14 +271,25 @@
 
     @property
     def encls(self):
         """(:obj:enclosure.Enclosures): controller enclosures
         """
         return enclosure.Enclosures(ctl_id=self._ctl_id, binary=self._binary)
 
+    @property
+    def drives_ids(self) -> List[str]:
+        """(list of str): list of drives ids in format (e:s)
+        """
+        drives = []
+        for encl in self.encls:
+            for id in encl.drives.ids:
+                drives.append("{enc}:{id}".format(enc=encl.id, id=id))
+
+        return drives
+
     def create_vd(self, name: str, raid: str, drives: str, strip: str = '64', PDperArray: Optional[int] = None) -> Optional[virtualdrive.VirtualDrive]:
         """Create virtual drive (raid) managed by current controller
 
         Args:
             name (str): virtual drive name
             raid (str): virtual drive raid level (raid0, raid1, ...)
             drives (str): storcli drives expression (e:s|e:s-x|e:s-x,y;e:s-x,y,z)
@@ -297,32 +308,31 @@
             'strip={0}'.format(strip)
         ]
 
         try:
             if int(raid) >= 10 and PDperArray is None:
                 # Try to count the number of drives in the array
                 # The format of the drives argument is e:s|e:s-x|e:s-x,y;e:s-x,y,z
-                # The number of drives is the number of commas plus the dashes intervals
 
-                numDrives = 0
-                drives2 = drives.split(':')
-                drives2 = drives2[1]
-                numDrives += drives2.count(',')+1
-                for interval in drives2.split(','):
-                    if '-' in interval:
-                        left = int(interval.split('-')[0])
-                        right = int(interval.split('-')[1])
-                        numDrives += right - left
+                numDrives = common.count_drives(drives)
+
+                if numDrives % 2 != 0 and numDrives % 3 == 0:
+                    # In some scenarios, such as 9 drives with raid 60, 3 is a good pd number but 4 is not
+                    # Must check for similar scenarios
+                    # BTW we don't clearly understand what PDperArray is for and what exactly it does under the hood. More investigation is needed
+                    PDperArray = numDrives//3
+                else:
+                    PDperArray = numDrives//2
 
-                PDperArray = numDrives//2
         except ValueError:
             pass
 
-        if raid == '00' and PDperArray is None:
-            PDperArray = 1
+        finally:
+            if raid == '00' and PDperArray is None:
+                PDperArray = 1
 
         if PDperArray is not None:
             args.append('PDperArray={0}'.format(PDperArray))
 
         self._run(args)
         for vd in self.vds:
             if name == vd.name:
```

### Comparing `PyStorCLI2-0.6.0/pystorcli/drive.py` & `PyStorCLI2-0.6.1.dev6/pystorcli/drive.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/pystorcli/enclosure.py` & `PyStorCLI2-0.6.1.dev6/pystorcli/enclosure.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/pystorcli/exc.py` & `PyStorCLI2-0.6.1.dev6/pystorcli/exc.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/pystorcli/storcli.py` & `PyStorCLI2-0.6.1.dev6/pystorcli/storcli.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/pystorcli/virtualdrive.py` & `PyStorCLI2-0.6.1.dev6/pystorcli/virtualdrive.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/pystorcli2/__init__.py` & `PyStorCLI2-0.6.1.dev6/pystorcli2/__init__.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/pystorcli2/bin/metrics.py` & `PyStorCLI2-0.6.1.dev6/pystorcli2/bin/metrics.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/pystorcli2/cachevault.py` & `PyStorCLI2-0.6.1.dev6/pystorcli2/cachevault.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/pystorcli2/cmdRunner.py` & `PyStorCLI2-0.6.1.dev6/pystorcli2/cmdRunner.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/pystorcli2/common.py` & `PyStorCLI2-0.6.1.dev6/pystorcli2/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -217,7 +217,58 @@
             if range_sep_t == 'end':
                 break
         else:
             # enclosure
             drives.extend(drives_from_expression(expr[pos:]))
             break
     return drives
+
+
+def expand_drive_ids(drives: str) -> str:
+    """Expand drive ids to range if needed
+
+    Args:
+        drives (str): storcli drives expression (e:s|e:s-x|e:s-x,y;e:s-x,y,z)
+
+    Returns:
+        (str): expanded drives expression (without dashes)
+    """
+    drive_list = drives.split(',')
+    output = ""
+
+    for i, drive in enumerate(drive_list):
+        drive = drive.strip()
+        encl, slot = drive.split(':')
+        new_output = drive
+
+        encl = encl.strip()
+        slot = slot.strip()
+
+        if '-' in slot:
+            begin, end = slot.split('-')
+
+            begin = begin.strip()
+            end = end.strip()
+
+            new_output = ','.join(['{0}:{1}'.format(encl, i)
+                                   for i in range(int(begin), int(end)+1)])
+
+        if i > 0:
+            output += ',' + new_output
+        else:
+            output += new_output
+
+    return output
+
+
+def count_drives(drives: str) -> int:
+    """Count number of drives in drives expression
+
+    Args:
+        drives (str): storcli drives expression (e:s|e:s-x|e:s-x,y;e:s-x,y,z)
+
+    Returns:
+        (int): number of drives
+    """
+
+    expanded_drives = expand_drive_ids(drives)
+    return len(expanded_drives.split(','))
```

### Comparing `PyStorCLI2-0.6.0/pystorcli2/controller.py` & `PyStorCLI2-0.6.1.dev6/pystorcli2/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -271,14 +271,25 @@
 
     @property
     def encls(self):
         """(:obj:enclosure.Enclosures): controller enclosures
         """
         return enclosure.Enclosures(ctl_id=self._ctl_id, binary=self._binary)
 
+    @property
+    def drives_ids(self) -> List[str]:
+        """(list of str): list of drives ids in format (e:s)
+        """
+        drives = []
+        for encl in self.encls:
+            for id in encl.drives.ids:
+                drives.append("{enc}:{id}".format(enc=encl.id, id=id))
+
+        return drives
+
     def create_vd(self, name: str, raid: str, drives: str, strip: str = '64', PDperArray: Optional[int] = None) -> Optional[virtualdrive.VirtualDrive]:
         """Create virtual drive (raid) managed by current controller
 
         Args:
             name (str): virtual drive name
             raid (str): virtual drive raid level (raid0, raid1, ...)
             drives (str): storcli drives expression (e:s|e:s-x|e:s-x,y;e:s-x,y,z)
@@ -297,32 +308,31 @@
             'strip={0}'.format(strip)
         ]
 
         try:
             if int(raid) >= 10 and PDperArray is None:
                 # Try to count the number of drives in the array
                 # The format of the drives argument is e:s|e:s-x|e:s-x,y;e:s-x,y,z
-                # The number of drives is the number of commas plus the dashes intervals
 
-                numDrives = 0
-                drives2 = drives.split(':')
-                drives2 = drives2[1]
-                numDrives += drives2.count(',')+1
-                for interval in drives2.split(','):
-                    if '-' in interval:
-                        left = int(interval.split('-')[0])
-                        right = int(interval.split('-')[1])
-                        numDrives += right - left
+                numDrives = common.count_drives(drives)
+
+                if numDrives % 2 != 0 and numDrives % 3 == 0:
+                    # In some scenarios, such as 9 drives with raid 60, 3 is a good pd number but 4 is not
+                    # Must check for similar scenarios
+                    # BTW we don't clearly understand what PDperArray is for and what exactly it does under the hood. More investigation is needed
+                    PDperArray = numDrives//3
+                else:
+                    PDperArray = numDrives//2
 
-                PDperArray = numDrives//2
         except ValueError:
             pass
 
-        if raid == '00' and PDperArray is None:
-            PDperArray = 1
+        finally:
+            if raid == '00' and PDperArray is None:
+                PDperArray = 1
 
         if PDperArray is not None:
             args.append('PDperArray={0}'.format(PDperArray))
 
         self._run(args)
         for vd in self.vds:
             if name == vd.name:
```

### Comparing `PyStorCLI2-0.6.0/pystorcli2/drive.py` & `PyStorCLI2-0.6.1.dev6/pystorcli2/drive.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/pystorcli2/enclosure.py` & `PyStorCLI2-0.6.1.dev6/pystorcli2/enclosure.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/pystorcli2/exc.py` & `PyStorCLI2-0.6.1.dev6/pystorcli2/exc.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/pystorcli2/storcli.py` & `PyStorCLI2-0.6.1.dev6/pystorcli2/storcli.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/pystorcli2/virtualdrive.py` & `PyStorCLI2-0.6.1.dev6/pystorcli2/virtualdrive.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/pystorcli_mirror/__init__.py` & `PyStorCLI2-0.6.1.dev6/pystorcli_mirror/__init__.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/baseTest.py` & `PyStorCLI2-0.6.1.dev6/tests/baseTest.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/datatest/controllerSet/test01/_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/controllerSet/test01/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/datatest/controllerSet/test02/_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/controllerSet/test02/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/datatest/namedSet/create_vd_raid0_00/__c0_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid0_00/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/datatest/namedSet/create_vd_raid0_00/__c0_v1_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid0_00/__c0_v1_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/datatest/namedSet/create_vd_raid0_00/_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid0_00/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/datatest/namedSet/create_vd_raid1_00/__c0_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid1_00/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/datatest/namedSet/create_vd_raid1_00/__c0_v1_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid1_00/__c0_v1_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/datatest/namedSet/create_vd_raid1_00/_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid1_00/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/datatest/namedSet/delete_vd_00/__c0_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/delete_vd_00/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/datatest/namedSet/delete_vd_00/__c0_v1_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/delete_vd_00/__c0_v1_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/datatest/namedSet/delete_vd_00/_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/delete_vd_00/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/datatest/namedSet/set_state_offline_00/__c0_e35_s12_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/__c0_e35_s12_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/datatest/namedSet/set_state_offline_00/__c0_e35_sall_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/__c0_e35_sall_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/datatest/namedSet/set_state_offline_00/__c0_e35_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/__c0_e35_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/datatest/namedSet/set_state_offline_00/__c0_eall_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/__c0_eall_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/datatest/namedSet/set_state_offline_00/__c0_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/datatest/namedSet/set_state_offline_00/_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/datatest/namedSet/show_events_00/__c0_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/show_events_00/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/datatest/namedSet/show_events_00/_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/show_events_00/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/datatest/namedSet/spindown_disk_00/__c0_e35_s12_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/__c0_e35_s12_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/datatest/namedSet/spindown_disk_00/__c0_e35_sall_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/__c0_e35_sall_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/datatest/namedSet/spindown_disk_00/__c0_e35_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/__c0_e35_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/datatest/namedSet/spindown_disk_00/__c0_eall_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/__c0_eall_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/datatest/namedSet/spindown_disk_00/__c0_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/datatest/namedSet/spindown_disk_00/_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/exceptions.py` & `PyStorCLI2-0.6.1.dev6/tests/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/storclifile.py` & `PyStorCLI2-0.6.1.dev6/tests/storclifile.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/test_controllers.py` & `PyStorCLI2-0.6.1.dev6/tests/test_controllers.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/test_operations.py` & `PyStorCLI2-0.6.1.dev6/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.0/tests/test_storcli.py` & `PyStorCLI2-0.6.1.dev6/tests/test_storcli.py`

 * *Files identical despite different names*

