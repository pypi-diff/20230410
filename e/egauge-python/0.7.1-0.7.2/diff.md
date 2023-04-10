# Comparing `tmp/egauge-python-0.7.1.tar.gz` & `tmp/egauge-python-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "egauge-python-0.7.1.tar", last modified: Fri Dec 16 04:56:13 2022, max compression
+gzip compressed data, was "egauge-python-0.7.2.tar", last modified: Mon Apr 10 19:10:39 2023, max compression
```

## Comparing `egauge-python-0.7.1.tar` & `egauge-python-0.7.2.tar`

### file list

```diff
@@ -1,48 +1,54 @@
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2022-12-16 04:56:13.607626 egauge-python-0.7.1/
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1122 2020-03-06 20:34:10.000000 egauge-python-0.7.1/LICENSE
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     2520 2022-12-16 04:56:13.607626 egauge-python-0.7.1/PKG-INFO
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     1893 2022-05-10 23:00:26.000000 egauge-python-0.7.1/README.rst
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2022-12-16 04:56:13.603626 egauge-python-0.7.1/egauge/
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2022-12-16 04:56:13.603626 egauge-python-0.7.1/egauge/ctid/
--rw-rw-r--   0 davidm    (1000) davidm    (1000)       71 2022-05-10 19:26:55.000000 egauge-python-0.7.1/egauge/ctid/__init__.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     2234 2022-04-22 23:39:14.000000 egauge-python-0.7.1/egauge/ctid/bit_stuffer.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    29354 2022-05-14 04:25:32.000000 egauge-python-0.7.1/egauge/ctid/ctid.py
--rwxrwxr-x   0 davidm    (1000) davidm    (1000)    12370 2022-05-14 04:25:14.000000 egauge-python-0.7.1/egauge/ctid/encoder.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     8791 2022-05-10 19:45:02.000000 egauge-python-0.7.1/egauge/ctid/waveform.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2022-12-16 04:56:13.603626 egauge-python-0.7.1/egauge/pyside2/
--rw-r--r--   0 davidm    (1000) davidm    (1000)        0 2020-03-06 20:43:49.000000 egauge-python-0.7.1/egauge/pyside2/__init__.py
--rw-r--r--   0 davidm    (1000) davidm    (1000)     3643 2022-04-22 23:39:14.000000 egauge-python-0.7.1/egauge/pyside2/ansi2html.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    10640 2022-04-22 23:39:14.000000 egauge-python-0.7.1/egauge/pyside2/terminal.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2022-12-16 04:56:13.607626 egauge-python-0.7.1/egauge/webapi/
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1346 2020-07-16 19:02:13.000000 egauge-python-0.7.1/egauge/webapi/__init__.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     8335 2022-05-04 18:07:16.000000 egauge-python-0.7.1/egauge/webapi/auth.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2022-12-16 04:56:13.607626 egauge-python-0.7.1/egauge/webapi/cloud/
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1293 2020-03-12 14:56:16.000000 egauge-python-0.7.1/egauge/webapi/cloud/__init__.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     4069 2022-05-04 18:28:54.000000 egauge-python-0.7.1/egauge/webapi/cloud/credentials.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2022-12-16 04:56:13.607626 egauge-python-0.7.1/egauge/webapi/cloud/gui/
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     3950 2022-04-22 23:52:29.000000 egauge-python-0.7.1/egauge/webapi/cloud/gui/credentials_dialog.py
--rw-r--r--   0 davidm    (1000) davidm    (1000)     7561 2022-05-05 19:36:33.000000 egauge-python-0.7.1/egauge/webapi/cloud/serial_number.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2022-12-16 04:56:13.607626 egauge-python-0.7.1/egauge/webapi/device/
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     1502 2022-09-27 04:23:24.000000 egauge-python-0.7.1/egauge/webapi/device/__init__.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    13784 2022-12-14 04:58:25.000000 egauge-python-0.7.1/egauge/webapi/device/capture.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    16279 2022-04-22 23:39:14.000000 egauge-python-0.7.1/egauge/webapi/device/ctid_info.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     6980 2022-09-27 04:23:24.000000 egauge-python-0.7.1/egauge/webapi/device/device.py
--rw-r--r--   0 davidm    (1000) davidm    (1000)     5461 2022-04-22 23:39:14.000000 egauge-python-0.7.1/egauge/webapi/device/local.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    12412 2022-09-27 04:23:24.000000 egauge-python-0.7.1/egauge/webapi/device/physical_quantity.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    14201 2022-09-27 04:23:24.000000 egauge-python-0.7.1/egauge/webapi/device/physical_units.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     9065 2022-09-19 15:49:48.000000 egauge-python-0.7.1/egauge/webapi/device/register.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     4461 2022-09-19 15:50:04.000000 egauge-python-0.7.1/egauge/webapi/device/register_row.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    30705 2022-09-17 23:27:52.000000 egauge-python-0.7.1/egauge/webapi/device/register_type.py
--rw-r--r--   0 davidm    (1000) davidm    (1000)     9237 2022-09-17 21:07:00.000000 egauge-python-0.7.1/egauge/webapi/device/virtual_register.py
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1405 2022-04-22 23:39:14.000000 egauge-python-0.7.1/egauge/webapi/error.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     7690 2022-04-28 23:10:14.000000 egauge-python-0.7.1/egauge/webapi/json_api.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2022-12-16 04:56:13.607626 egauge-python-0.7.1/egauge_python.egg-info/
--rw-r--r--   0 davidm    (1000) davidm    (1000)     2520 2022-12-16 04:56:13.000000 egauge-python-0.7.1/egauge_python.egg-info/PKG-INFO
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1103 2022-12-16 04:56:13.000000 egauge-python-0.7.1/egauge_python.egg-info/SOURCES.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)        1 2022-12-16 04:56:13.000000 egauge-python-0.7.1/egauge_python.egg-info/dependency_links.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)       59 2022-12-16 04:56:13.000000 egauge-python-0.7.1/egauge_python.egg-info/entry_points.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)       57 2022-12-16 04:56:13.000000 egauge-python-0.7.1/egauge_python.egg-info/requires.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)       12 2022-12-16 04:56:13.000000 egauge-python-0.7.1/egauge_python.egg-info/top_level.txt
--rw-rw-r--   0 davidm    (1000) davidm    (1000)       55 2022-05-11 01:22:07.000000 egauge-python-0.7.1/pyproject.toml
--rw-rw-r--   0 davidm    (1000) davidm    (1000)       38 2022-12-16 04:56:13.607626 egauge-python-0.7.1/setup.cfg
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     1309 2022-12-16 04:54:50.000000 egauge-python-0.7.1/setup.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-10 19:10:39.893046 egauge-python-0.7.2/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1090 2023-02-23 18:58:55.000000 egauge-python-0.7.2/LICENSE
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     2956 2023-04-10 19:10:39.893046 egauge-python-0.7.2/PKG-INFO
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     2301 2023-04-10 19:09:39.000000 egauge-python-0.7.2/README.md
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-10 19:10:39.717049 egauge-python-0.7.2/egauge/
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-10 19:10:39.753048 egauge-python-0.7.2/egauge/ctid/
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)       71 2022-05-10 19:26:55.000000 egauge-python-0.7.2/egauge/ctid/__init__.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     2234 2022-04-22 23:39:14.000000 egauge-python-0.7.2/egauge/ctid/bit_stuffer.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    29354 2022-05-14 04:25:32.000000 egauge-python-0.7.2/egauge/ctid/ctid.py
+-rwxrwxr-x   0 davidm    (1000) davidm    (1000)    12370 2022-05-14 04:25:14.000000 egauge-python-0.7.2/egauge/ctid/encoder.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     8791 2022-05-10 19:45:02.000000 egauge-python-0.7.2/egauge/ctid/waveform.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-10 19:10:39.765048 egauge-python-0.7.2/egauge/pyside2/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)        0 2020-03-06 20:43:49.000000 egauge-python-0.7.2/egauge/pyside2/__init__.py
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     3643 2022-04-22 23:39:14.000000 egauge-python-0.7.2/egauge/pyside2/ansi2html.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    10640 2022-04-22 23:39:14.000000 egauge-python-0.7.2/egauge/pyside2/terminal.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-10 19:10:39.781048 egauge-python-0.7.2/egauge/webapi/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1346 2020-07-16 19:02:13.000000 egauge-python-0.7.2/egauge/webapi/__init__.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     8335 2022-05-04 18:07:16.000000 egauge-python-0.7.2/egauge/webapi/auth.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-10 19:10:39.793048 egauge-python-0.7.2/egauge/webapi/cloud/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1293 2020-03-12 14:56:16.000000 egauge-python-0.7.2/egauge/webapi/cloud/__init__.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     4069 2022-05-04 18:28:54.000000 egauge-python-0.7.2/egauge/webapi/cloud/credentials.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-10 19:10:39.797047 egauge-python-0.7.2/egauge/webapi/cloud/gui/
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     3950 2022-04-22 23:52:29.000000 egauge-python-0.7.2/egauge/webapi/cloud/gui/credentials_dialog.py
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     7561 2022-05-05 19:36:33.000000 egauge-python-0.7.2/egauge/webapi/cloud/serial_number.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-10 19:10:39.841047 egauge-python-0.7.2/egauge/webapi/device/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1502 2022-09-19 21:16:17.000000 egauge-python-0.7.2/egauge/webapi/device/__init__.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    13955 2023-03-01 22:13:47.000000 egauge-python-0.7.2/egauge/webapi/device/capture.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    16279 2023-03-18 20:49:18.000000 egauge-python-0.7.2/egauge/webapi/device/ctid_info.py
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     7379 2023-02-23 18:36:07.000000 egauge-python-0.7.2/egauge/webapi/device/device.py
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     6603 2023-03-01 22:14:28.000000 egauge-python-0.7.2/egauge/webapi/device/local.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    12412 2022-09-20 20:05:39.000000 egauge-python-0.7.2/egauge/webapi/device/physical_quantity.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    14201 2022-09-20 18:48:03.000000 egauge-python-0.7.2/egauge/webapi/device/physical_units.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     9065 2022-09-19 15:49:48.000000 egauge-python-0.7.2/egauge/webapi/device/register.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     5356 2023-03-02 00:28:30.000000 egauge-python-0.7.2/egauge/webapi/device/register_row.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    30705 2023-02-23 21:18:54.000000 egauge-python-0.7.2/egauge/webapi/device/register_type.py
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     9308 2023-03-01 22:33:44.000000 egauge-python-0.7.2/egauge/webapi/device/virtual_register.py
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1405 2022-04-22 23:39:14.000000 egauge-python-0.7.2/egauge/webapi/error.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     9209 2023-04-10 18:59:44.000000 egauge-python-0.7.2/egauge/webapi/json_api.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-10 19:10:39.869046 egauge-python-0.7.2/egauge_python.egg-info/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     2956 2023-04-10 19:10:39.000000 egauge-python-0.7.2/egauge_python.egg-info/PKG-INFO
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1222 2023-04-10 19:10:39.000000 egauge-python-0.7.2/egauge_python.egg-info/SOURCES.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)        1 2023-04-10 19:10:39.000000 egauge-python-0.7.2/egauge_python.egg-info/dependency_links.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)       59 2023-04-10 19:10:39.000000 egauge-python-0.7.2/egauge_python.egg-info/entry_points.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)       94 2023-04-10 19:10:39.000000 egauge-python-0.7.2/egauge_python.egg-info/requires.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)       21 2023-04-10 19:10:39.000000 egauge-python-0.7.2/egauge_python.egg-info/top_level.txt
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-10 19:10:39.889046 egauge-python-0.7.2/examples/
+-rwxrwxr-x   0 davidm    (1000) davidm    (1000)     2224 2023-03-10 21:32:59.000000 egauge-python-0.7.2/examples/test_capture.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)      716 2023-03-02 01:05:11.000000 egauge-python-0.7.2/examples/test_common.py
+-rwxrwxr-x   0 davidm    (1000) davidm    (1000)     2236 2023-03-10 21:33:26.000000 egauge-python-0.7.2/examples/test_ctid.py
+-rwxrwxr-x   0 davidm    (1000) davidm    (1000)     4775 2023-03-10 20:47:54.000000 egauge-python-0.7.2/examples/test_local.py
+-rwxrwxr-x   0 davidm    (1000) davidm    (1000)     3214 2023-03-10 22:06:39.000000 egauge-python-0.7.2/examples/test_register.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)       55 2022-05-11 01:22:07.000000 egauge-python-0.7.2/pyproject.toml
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)       38 2023-04-10 19:10:39.893046 egauge-python-0.7.2/setup.cfg
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     1440 2023-04-10 19:10:03.000000 egauge-python-0.7.2/setup.py
```

### Comparing `egauge-python-0.7.1/LICENSE` & `egauge-python-0.7.2/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2015 David Mosberger <davidm@egauge.net>, eGauge Systems LLC
+Copyright (c) 2015-2023 eGauge Systems LLC
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
```

### Comparing `egauge-python-0.7.1/PKG-INFO` & `egauge-python-0.7.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,88 +1,85 @@
 Metadata-Version: 2.1
 Name: egauge-python
-Version: 0.7.1
+Version: 0.7.2
 Summary: .
 Home-page: https://bitbucket.org/egauge/python/
 Author: David Mosberger-Tang
 Author-email: davidm@egauge.net
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
+Provides-Extra: examples
 License-File: LICENSE
 
-eGauge open source Python code
-******************************
+# eGauge open source Python code
 
 This repository is a collection of Python packages that have been
 released by eGauge Systems LLC as open source (MIT license).  These
 are released in the hope that they may be useful for other developers.
 Please see LICENSE for details.  eGauge Systems LLC also reserved the
 rights to add, modify, or remove code from this repository or the
 entire repository without notice.
 
-|
+## Example Programs
 
-Overview of available modules
-=============================
+Example programs can be found in the `examples` subdirectory.  If you
+want to run these programs, ensure that all dependencies are installed
+by running the command:
 
-|
+```sh
+pip install egauge-python[examples]
+```
 
-egauge.webapi
--------------
+Before running these programs, set the following environment variables
+for your preferred test device:
+
+ * EGDEV: URL of the test device (e.g., "http://eGaugeXXXXX.local" or
+   "http://eGaugeXXXX.d.egauge.net")
+ * EGUSR: Username to authenticate with (e.g., "owner")
+ * EGPWD: Password to authenticate with (e.g., "super-secret-pw")
+
+## Overview of available modules
+
+### egauge.webapi
 
 The classes in this module provide access to eGauge web services.  The
 APIs may be available on eGauge devices and/or as cloud-based web
 services.
 
-|
-
-egauge.webapi.device
---------------------
+### egauge.webapi.device
 
 The classes in this module provide access to APIs implemented on
 eGauge devices.
 
-|
-
-egauge.webapi.cloud
--------------------
+### egauge.webapi.cloud
 
 The classes in this module provide access to APIs implemented by
 eGauge cloud services.
 
-|
-
-egauge.ctid
------------
+### egauge.ctid
 
 The classes in this module support manufacturing CTid® sensors.  CTid®
 is patented technology and shall be used in accordance with the
 licensing agreements governing its use.
 
-|
-
-egauge.pyside2
---------------
+### egauge.pyside2
 
 The classes in this module support QT5-based graphical
 user-interfaces.
 
-|
-
-Source Code Conventions
-=======================
+## Source Code Conventions
 
 Source code should be formatted with ``black`` using a maximum line-length
 of 79 characters.  Black can be installed with ``pip install black``.
 If the resulting output is inadequate for some reason, such as manually
 formatted data tables, you can make judicious use of ``# fmt: off`` and
 ``# fmt: on`` to disable formatting for the relevant lines.
```

### Comparing `egauge-python-0.7.1/egauge/ctid/bit_stuffer.py` & `egauge-python-0.7.2/egauge/ctid/bit_stuffer.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.1/egauge/ctid/ctid.py` & `egauge-python-0.7.2/egauge/ctid/ctid.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.1/egauge/ctid/encoder.py` & `egauge-python-0.7.2/egauge/ctid/encoder.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.1/egauge/ctid/waveform.py` & `egauge-python-0.7.2/egauge/ctid/waveform.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.1/egauge/pyside2/ansi2html.py` & `egauge-python-0.7.2/egauge/pyside2/ansi2html.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.1/egauge/pyside2/terminal.py` & `egauge-python-0.7.2/egauge/pyside2/terminal.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.1/egauge/webapi/__init__.py` & `egauge-python-0.7.2/egauge/webapi/__init__.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.1/egauge/webapi/auth.py` & `egauge-python-0.7.2/egauge/webapi/auth.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.1/egauge/webapi/cloud/__init__.py` & `egauge-python-0.7.2/egauge/webapi/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.1/egauge/webapi/cloud/credentials.py` & `egauge-python-0.7.2/egauge/webapi/cloud/credentials.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.1/egauge/webapi/cloud/gui/credentials_dialog.py` & `egauge-python-0.7.2/egauge/webapi/cloud/gui/credentials_dialog.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.1/egauge/webapi/cloud/serial_number.py` & `egauge-python-0.7.2/egauge/webapi/cloud/serial_number.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.1/egauge/webapi/device/__init__.py` & `egauge-python-0.7.2/egauge/webapi/device/__init__.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.1/egauge/webapi/device/capture.py` & `egauge-python-0.7.2/egauge/webapi/device/capture.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 eGauge Systems LLC
+# Copyright (c) 2022-2023 eGauge Systems LLC
 #       1644 Conestoga St, Suite 2
 #       Boulder, CO 80301
 #       voice: 720-545-9767
 #       email: davidm@egauge.net
 #
 # All rights reserved.
 #
@@ -34,17 +34,18 @@
 from enum import Enum
 from typing import Dict, List, Optional, Union
 
 import time
 
 
 from .device import Device
+from ..error import Error
 
 
-class Error(Exception):
+class CaptureError(Error):
     """Base exception for all errors raised by this module."""
 
 
 @dataclass
 class ChannelSamples:
     """Each sample is stored as a pair (t,y) where t is the time the
     sample was captured and y is value of the channel at that time.
@@ -202,15 +203,15 @@
     def channel_unit(self, channel_name: str) -> str:
         """Return the physical unit of the channel with name
         `channel_name`.
 
         """
         cinfo = self._dev.channel_info().get(channel_name)
         if cinfo is None:
-            raise Error("Unknown channel.", channel_name)
+            raise CaptureError("Unknown channel.", channel_name)
         return cinfo.unit
 
     def start(self, duration: float = None, **kwargs) -> int:
         """Initiate capturing data for a duration of `duration` seconds.  If
         `duration` is None or unspecified, as much data as possible is
         captured.  Additional keyword arguments are passed along to
         requests.get().  This method returns an integer "cookie" which
@@ -241,44 +242,49 @@
             params += f"&T={1000 * self.trigger_timeout}"
 
         if self.pretrigger is not None:
             params += f"&p={self.pretrigger}"
 
         ret = self._dev.get(f"/capture?{params}", **kwargs)
         if ret.get("error"):
-            raise Error(ret.get("error"))
+            raise CaptureError(ret.get("error"))
 
         if ret["state"] == "available":
-            raise Error("Failed to start capture.", ret["state"])
+            raise CaptureError("Failed to start capture.", ret["state"])
         return ret["cookie"]
 
-    def result(self, cookie: int, **kwargs) -> Union[float, CaptureResult]:
+    def result(
+        self, cookie: int, raw=False, **kwargs
+    ) -> Union[float, CaptureResult]:
         """Return the result of the capture identified by `cookie`, which must
         be a cookie previously returned by a call to Capture.start().
         The method returns a number if the capture is still in
         progress.  If so, the number is from 0 and 1, giving the
         fraction of the total amount of data captured so far.  If all
         the data has been captured, an object of class CaptureResult
         is returned.  If any error occurs, an exception is raised.
 
         """
         params = f"n={cookie}"
 
+        if raw:
+            params += "&r=True"
+
         ret = self._dev.get(f"/capture?{params}", **kwargs)
         if ret.get("error"):
-            raise Error(ret.get("error"))
+            raise CaptureError(ret.get("error"))
 
         if ret["state"] == "available":
-            raise Error("Capture aborted.")  # somebody interfered?
+            raise CaptureError("Capture aborted.")  # somebody interfered?
         if ret["state"] == "armed":
             return 0.0
         if ret["state"] == "capturing":
             return ret["count"] / ret["max_count"]
         if ret["state"] != "full":
-            raise Error("Unknown capture state.", ret["state"])
+            raise CaptureError("Unknown capture state.", ret["state"])
 
         ch_mask = 0
         for n, w in enumerate(ret["ch_mask"]):
             ch_mask |= w << (n * 32)
 
         channel_names = []
         result = CaptureResult()
@@ -356,28 +362,28 @@
 
         """
         params = "R"
         if cookie is not None:
             params = f"n={cookie}"
         ret = self._dev.get(f"/capture?{params}", **kwargs)
         if ret.get("error"):
-            raise Error(ret.get("error"))
+            raise CaptureError(ret.get("error"))
 
         state = ret.get("state")
         if state != "available":
-            raise Error("Unexpected capture state.", state)
+            raise CaptureError("Unexpected capture state.", state)
 
     def _ch_number(self, name: str) -> int:
         """Get the channel number of the channel named `name` or raise an
         exception if the channel name is not known.
 
         """
         cinfo = self._dev.channel_info().get(name)
         if cinfo is None:
-            raise Error("Unknown channel.", name)
+            raise CaptureError("Unknown channel.", name)
         return cinfo.chan
 
     def _ch_name(self, ch: int) -> str:
         """Get the name of the channel with number `ch` or None if there is no
         name for the specified channel number.
 
         """
```

### Comparing `egauge-python-0.7.1/egauge/webapi/device/ctid_info.py` & `egauge-python-0.7.2/egauge/webapi/device/ctid_info.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.1/egauge/webapi/device/device.py` & `egauge-python-0.7.2/egauge/webapi/device/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020, 2022 eGauge Systems LLC
+# Copyright (c) 2020, 2022-2023 eGauge Systems LLC
 #       1644 Conestoga St, Suite 2
 #       Boulder, CO 80301
 #       voice: 720-545-9767
 #       email: davidm@egauge.net
 #
 # All rights reserved.
 #
@@ -33,81 +33,100 @@
 from types import SimpleNamespace
 from typing import List
 
 from .. import json_api
 from ..error import Error
 from .virtual_register import VirtualRegister
 
+
 class DeviceError(Error):
     """Raised if for device related errors."""
 
 
 @dataclass
 class ChannelInfo:
-    chan: int	# the channel number
-    unit: str	# the physical unit of the channel data
+    chan: int  # the channel number
+    unit: str  # the physical unit of the channel data
 
 
 class Device:
     """This class provides access to an eGauge device's JSON WebAPI.
     See "Web API Design" document for details."""
 
-    def __init__(self, dev_uri, auth=None):
+    def __init__(self, dev_uri, auth=None, verify=True):
         """Return a device object that can be used to access the device a
         address DEV_URI.  An example DEV_URI would be
         "http://proto1.egaug.es".  AUTH should be an authentication object
         that provides the credentials to access the device.  Typically,
-        this should be a JWTAuth object.
+        this should be a JWTAuth object.  VERIFY can be set to False
+        to turn off certificate verification.
 
         """
         self.api_uri = dev_uri + "/api"
         self.auth = auth
-        self._reg_info = None		# cached register info
-        self._chan_info = None		# cached channel info
+        self._reg_info = None  # cached register info
+        self._chan_info = None  # cached channel info
+        self._verify = verify
 
     def get(self, resource, **kwargs):
         """Issue GET request for /api resource RESOURCE and return the parsed
         JSON data or None if the request failed or returned invalid
         JSON data.  Additional keyword arguments are passed on to
         requests.get().
 
         """
-        return json_api.get(self.api_uri + resource, auth=self.auth, **kwargs)
+        return json_api.get(
+            self.api_uri + resource,
+            auth=self.auth,
+            verify=self._verify,
+            **kwargs
+        )
 
     def put(self, resource, json_data, **kwargs):
         """Issue PUT request with JSON_DATA as body to /api resource RESOURCE
         and return parsed JSON reply or None if the request failed or
         returned invalid JSON data.  Additional keyword arguments are
         passed on to requests.put().
 
         """
         return json_api.put(
-            self.api_uri + resource, json_data, auth=self.auth, **kwargs
+            self.api_uri + resource,
+            json_data,
+            auth=self.auth,
+            verify=self._verify,
+            **kwargs
         )
 
     def post(self, resource, json_data, **kwargs):
         """Issue POST request with JSON_DATA as body to /api resource RESOURCE
         and return parsed JSON reply or None if the request failed or
         returned invalid JSON data.  Additional keyword arguments are
         passed on to requests.post().
 
         """
         return json_api.post(
-            self.api_uri + resource, json_data, auth=self.auth, **kwargs
+            self.api_uri + resource,
+            json_data,
+            auth=self.auth,
+            verify=self._verify,
+            **kwargs
         )
 
     def delete(self, resource, **kwargs):
         """Issue DELETE request for /api resource RESOURCE and return parsed
         JSON reply or None if the request failed or returned invalid
         JSON data.  Additional keyword arguments are passed on to
         requests.post().
 
         """
         return json_api.delete(
-            self.api_uri + resource, auth=self.auth, **kwargs
+            self.api_uri + resource,
+            auth=self.auth,
+            verify=self._verify,
+            **kwargs
         )
 
     def _fetch_reg_info(self):
         """Fetch register info, including type and virtual register
         formulas."""
         reply = self.get("/register", params={"virtual": "formula"})
         if reply is None or "registers" not in reply:
```

### Comparing `egauge-python-0.7.1/egauge/webapi/device/local.py` & `egauge-python-0.7.2/egauge/webapi/device/local.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020-2021 eGauge Systems LLC
+# Copyright (c) 2020-2021, 2023 eGauge Systems LLC
 #       1644 Conestoga St, Suite 2
 #       Boulder, CO 80301
 #       voice: 720-545-9767
 #       email: davidm@egauge.net
 #
 # All rights reserved.
 #
@@ -27,45 +27,59 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 import decimal
 import json
 
 from .register_row import RegisterRow
+from .register_type import RegisterType
+
+from ..error import Error
+
+
+class LocalError(Error):
+    """All errors in this module raise this exception."""
 
 
 def sensor_port_name(index):
     """Sensor port name for sensor port with index INDEX, which must be
     in the range from 0..SENSOR_PORT_COUNT-1.
 
     """
-    return "S%u" % (index + 1)
+    sensor = index + 1
+    return f"S{sensor}"
 
 
 class Local:
     """Fetch data from /api/local."""
 
     # Sensor parameter spec strings:
     #   For l=...:
     SPEC_L1 = "L1"
     SPEC_L2 = "L2"
     SPEC_L3 = "L3"
     SPEC_L1_L2 = "L12"
     SPEC_L2_L3 = "L23"
     SPEC_L3_L1 = "L31"
     SPEC_LDC = "Ldc"
+    SPEC_D1 = "D1"
+    SPEC_D2 = "D2"
+    SPEC_D3 = "D3"
 
     # Sensor names as they appear in the output:
     NAME_L1 = "L1"
     NAME_L2 = "L2"
     NAME_L3 = "L3"
     NAME_L1_L2 = "L1-L2"
     NAME_L2_L3 = "L2-L3"
     NAME_L3_L1 = "L3-L1"
     NAME_LDC = "Ldc"
+    NAME_D1 = "D1"
+    NAME_D2 = "D2"
+    NAME_D3 = "D3"
     NAME_TEMP_PCB = "Tpcb"
     NAME_HUMID_PCB = "Hpcb"
 
     METRIC_RATE = "rate"
     METRIC_CUMUL = "cumul"
     METRIC_TYPE = "type"
 
@@ -152,25 +166,45 @@
     ):
         """Return a timestamped row of register data.  By default, the
         cumulative normal values of section "values" is returned.
         Non-default rows can be selected by passing the desired values
         for METRIC, MEASUREMENT, and/or SECTION.
 
         """
+        if metric not in [Local.METRIC_RATE, Local.METRIC_CUMUL]:
+            raise LocalError(
+                "Metric must be one of METRIC_RATE or METRIC_CUMUL", metric
+            )
+
         if self.raw is None:
             return None
-        section = self.raw[section]
         regs = {}
-        for key, metrics in section.items():
-            if metric == Local.METRIC_TYPE:
-                val = metrics[metric]
-            else:
-                val = metrics[metric]
-                if section == Local.SECTION_VALUES:
-                    val = val[measurement]
-                if metric == Local.METRIC_CUMUL:
-                    val = int(val)  # convert from decimal string to integer
+        type_codes = {}
+        is_diff = True
+        if metric == Local.METRIC_CUMUL:
+            is_diff = False
+        for key, metrics in self.raw[section].items():
+            if metric not in metrics:
+                continue
+            val = metrics[metric]
+            if section == Local.SECTION_VALUES:
+                val = val[measurement]
+            if metric == Local.METRIC_CUMUL:
+                val = int(val)  # convert from decimal string to integer
+            regs[key] = val
+            if section == Local.SECTION_ENERGY:
+                # this assumes the sensor pairs measure voltage and current:
+                tc = RegisterType.POWER.value
+            elif section == Local.SECTION_APPARENT:
+                # this assumes the sensor pairs measure voltage and current:
+                tc = RegisterType.APPARENT_POWER.value
+            elif measurement == Local.MEASUREMENT_FREQ:
+                tc = RegisterType.FREQ.value
+            elif Local.METRIC_TYPE in metrics:
+                tc = metrics[Local.METRIC_TYPE]
+
             regs[key] = val
-        return RegisterRow(self.ts(), regs)
+            type_codes[key] = tc
+        return RegisterRow(self.ts(), regs, type_codes, is_diff)
 
     def __str__(self):
         return json.dumps(self.raw)
```

### Comparing `egauge-python-0.7.1/egauge/webapi/device/physical_quantity.py` & `egauge-python-0.7.2/egauge/webapi/device/physical_quantity.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.1/egauge/webapi/device/physical_units.py` & `egauge-python-0.7.2/egauge/webapi/device/physical_units.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.1/egauge/webapi/device/register.py` & `egauge-python-0.7.2/egauge/webapi/device/register.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.1/egauge/webapi/device/register_row.py` & `egauge-python-0.7.2/egauge/webapi/device/register_row.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020, 2022 eGauge Systems LLC
+# Copyright (c) 2020, 2022-2023 eGauge Systems LLC
 #       1644 Conestoga St, Suite 2
 #       Boulder, CO 80301
 #       voice: 720-545-9767
 #       email: davidm@egauge.net
 #
 # All rights reserved.
 #
@@ -33,32 +33,34 @@
 import json
 
 from deprecated import deprecated
 
 from .register_type import Units
 from .physical_quantity import PhysicalQuantity
 
+from ..error import Error
 
-class Error(Exception):
+
+class RegRowError(Error):
     """All errors in this module raise this exception."""
 
 
 class RegisterRow:
     """A row of register data contains a timestamp and the signed 64-bit
     register values for that timestamp.  Subtracing one row from
     another creates a difference row.  On a difference row,
     RegisterRow.pq_accu() can be called to get the amount by which a
     register changed between the two rows.
 
     Similarly, RegisterRow.pq_avg() can be called to calculate the
     average register value that was in effect between the two rows."""
 
-    def __init__(self, ts, regs=None, type_codes=None):
+    def __init__(self, ts, regs=None, type_codes=None, is_diff=False):
         self.ts = ts
-        self.is_diff = False
+        self.is_diff = is_diff
         if regs is None:
             self.regs = {}
         else:
             self.regs = copy.copy(regs)
         if type_codes is None:
             self.type_codes = {}
         else:
@@ -66,14 +68,26 @@
 
     @deprecated(version="0.7.0", reason="use pq_avg() instead")
     def avg(self, regname) -> float:
         """Return the time-average of the register value."""
         self._assert(self.is_diff)
         return self.regs[regname] / self.ts
 
+    def pq_rate(self, regname) -> PhysicalQuantity:
+        """Return register rate of change as a physical quantity in the
+        preferred unit of the default unit system (see
+        PhysicalQuantity.set_unit_system()).
+
+        """
+        self._assert(self.is_diff)
+        val = self.regs[regname]
+        return PhysicalQuantity(
+            val, self.type_codes[regname], is_cumul=False
+        ).to_preferred()
+
     def pq_avg(self, regname) -> PhysicalQuantity:
         """Return the time-average of the register value as a physical
         quantity in the preferred unit of the default unit system
         (see PhysicalQuantity.set_unit_system())."""
         self._assert(self.is_diff)
         ute = Units.table[self.type_codes[regname]]
         val = self.regs[regname] / ute.fix_scale / self.ts
@@ -81,20 +95,25 @@
             val, self.type_codes[regname], is_cumul=False
         ).to_preferred()
 
     def pq_accu(self, regname):
         """Return the accumulated register value as a physical quantity in the
         preferred unit of the default unit system (see
         PhysicalQuantity.set_unit_system())."""
-        self._assert(self.is_diff)
         ute = Units.table[self.type_codes[regname]]
         val = self.regs[regname] * ute.cumul_scale
+
+        # If the row is not a difference row, we cannot convert
+        # between units with additive constants (e.g., °C·d to °F·d).
+        # Set `dt` to None in that case, so those conversions will
+        # fail visibily:
+        dt = self.ts if self.is_diff else None
         return PhysicalQuantity(
             val, self.type_codes[regname], is_cumul=True
-        ).to_preferred(dt=self.ts)
+        ).to_preferred(dt=dt)
 
     def __sub__(self, subtrahend):
         """Subtract two register rows from each other and return the result.
         The SUBTRAHEND must have values for all of the registers in
         the minuend row.
 
         """
@@ -108,12 +127,19 @@
             ret.regs[name] -= subtrahend.regs[name]
         return ret
 
     def _assert(self, cond: bool):
         if cond:
             return
         if self.is_diff:
-            raise Error("It is not possible to subtract a difference row.")
-        raise Error("The row must be a difference.")
+            raise RegRowError("Cannot subtract a difference row.")
+        raise RegRowError("The row must be a difference.")
 
     def __str__(self):
         return f"{self.ts}: {json.dumps(self.regs)}"
+
+    def __iter__(self):
+        """Iterate over cumulative register values.  Each iteration returns
+        one row of data as a RegisterRow.
+
+        """
+        return iter(self.regs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `egauge-python-0.7.1/egauge/webapi/device/register_type.py` & `egauge-python-0.7.2/egauge/webapi/device/register_type.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.1/egauge/webapi/device/virtual_register.py` & `egauge-python-0.7.2/egauge/webapi/device/virtual_register.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 eGauge Systems LLC
+# Copyright (c) 2022-2023 eGauge Systems LLC
 #       1644 Conestoga St, Suite 2
 #       Boulder, CO 80301
 #       voice: 720-545-9767
 #       email: davidm@egauge.net
 #
 # All rights reserved.
 #
@@ -30,19 +30,22 @@
 from dataclasses import dataclass
 from enum import auto, Enum
 from types import SimpleNamespace
 from typing import Callable, List
 
 import re
 
+from ..error import Error
+
+
 ID_PATTERN = re.compile(r"[A-Z]+")
 NUMBER_PATTERN = re.compile(r"(\d+)")
 
 
-class Error(Exception):
+class VirtRegError(Error):
     """Exception raised due to any errors in this module."""
 
 
 class Operator(Enum):
     REG = auto()  # value of a register
     MIN = auto()  # deprecated MIN(reg,c)
     MAX = auto()  # deprecated MAX(reg,c)
@@ -139,15 +142,15 @@
           regname = QUOTED_STRING .
           formula = ('MIN'|'MAX') '(' regname ',' number ')' .
           number = [0-9]+ .
 
         """
 
         def error(reason):
-            raise Error(f"{reason} (rest: '{formula[state.idx:]}')")
+            raise VirtRegError(f"{reason} (rest: '{formula[state.idx:]}')")
 
         def whitespace():
             while state.idx < len(formula) and formula[state.idx] in [
                 " ",
                 "\t",
             ]:
                 state.idx += 1
@@ -272,26 +275,26 @@
         '"Solar"+"Solar"',
         ' - "Grid"	',
         '+"Grid"',
         '"Grid"+MAX("Solar",0)',
     ]:
         try:
             virt = VirtualRegister(formula, lambda reg: regmap[reg])
-        except Error as e:
+        except VirtRegError as e:
             print("Error: Compile failed for formula:", formula)
             print("\t", e)
             continue
         print(
             "formula:",
             formula,
             ">>> compiled: ",
             virt,
             "phys_regs",
             virt.phys_regs,
         )
 
     if virt.calc(lambda reg: [10, 20][reg]) != 30:
-        raise Error("Expected 30")
+        raise VirtRegError("Expected 30")
     if virt.calc(lambda reg: [10, -20][reg]) != 10:
-        raise Error("Expected 10")
+        raise VirtRegError("Expected 10")
     if virt.calc(lambda reg: [-10, -20][reg]) != -10:
-        raise Error("Expected 10")
+        raise VirtRegError("Expected 10")
```

### Comparing `egauge-python-0.7.1/egauge/webapi/error.py` & `egauge-python-0.7.2/egauge/webapi/error.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.1/egauge/webapi/json_api.py` & `egauge-python-0.7.2/egauge/webapi/json_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020-2022 eGauge Systems LLC
+# Copyright (c) 2020-2023 eGauge Systems LLC
 #       1644 Conestoga St, Suite 2
 #       Boulder, CO 80301
 #       voice: 720-545-9767
 #       email: davidm@egauge.net
 #
 # All rights reserved.
 #
@@ -44,20 +44,38 @@
     """
 
 
 class UnauthenticatedError(Error):
     """Raised when a request fails with HTTP status code 401."""
 
 
+def _raw_response(kwargs):
+    """Check for and remove 'raw_response' keyword argument from KWARGS.
+    Returns whether 'raw_response' is True.
+
+    """
+    if "raw_response" in kwargs:
+        raw_response = kwargs["raw_response"]
+        del kwargs["raw_response"]
+        return raw_response is True
+    return False
+
+
 def get(resource, **kwargs):
     """Issue GET request for RESOURCE and return the parsed JSON data or
     None if the request failed or returned invalid JSON data.
+
+    If keyword argument raw_response is True, the raw requests
+    response object is returned.  This is useful, for example, if the
+    caller needs to get a response header.
+
     Additional keyword arguments are passed on to requests.get().
 
     """
+    raw = _raw_response(kwargs)
     try:
         r = requests.get(resource, **kwargs)
     except requests.exceptions.RequestException as e:
         raise JSONAPIError("requests.get exception.", e) from e
     if r.status_code == 401:
         raise UnauthenticatedError(r)
     if r.status_code < 200 or r.status_code > 299:
@@ -66,33 +84,42 @@
                 "HTTP GET status code %s.  Keyword args: %s",
                 r.status_code,
                 kwargs,
             )
         raise JSONAPIError(
             "Unexpected HTTP status code.", r.status_code, r.content
         )
+    if raw:
+        return r
+
     reply = None
     try:
         if r.text:
             reply = r.json()
     except ValueError as e:
         raise JSONAPIError("Invalid JSON data.", r.content) from e
     return reply
 
 
 def patch(resource, json_data, **kwargs):
     """Issue PATCH request with JSON_DATA as body to RESOURCE and return
     parsed JSON reply or None if the request failed or returned
-    invalid JSON data.  Additional keyword arguments are passed on to
-    requests.patch().
+    invalid JSON data.
+
+    If keyword argument raw_response is True, the raw requests
+    response object is returned.  This is useful, for example, if the
+    caller needs to get a response header.
+
+    Additional keyword arguments are passed on to requests.patch().
 
     """
     headers = kwargs.get("headers", {})
     headers["Content-Type"] = "application/json"
     kwargs["headers"] = headers
+    raw = _raw_response(kwargs)
     try:
         r = requests.patch(resource, json=json_data, **kwargs)
     except requests.exceptions.RequestException as e:
         raise JSONAPIError("requests.patch exception.", e) from e
     if r.status_code == 401:
         raise UnauthenticatedError(r)
     if not 200 <= r.status_code <= 299:
@@ -104,33 +131,42 @@
                 resource,
                 json_data,
                 kwargs,
             )
         raise JSONAPIError(
             "Unexpected HTTP status code.", r.status_code, r.content
         )
+    if raw:
+        return r
+
     reply = None
     try:
         if r.text:
             reply = r.json()
     except ValueError as e:
         raise JSONAPIError("Invalid JSON data.", r.content) from e
     return reply
 
 
 def put(resource, json_data, **kwargs):
     """Issue PUT request with JSON_DATA as body to RESOURCE and return
     parsed JSON reply or None if the request failed or returned
-    invalid JSON data.  Additional keyword arguments are passed on to
-    requests.put().
+    invalid JSON data.
+
+    If keyword argument raw_response is True, the raw requests
+    response object is returned.  This is useful, for example, if the
+    caller needs to get a response header.
+
+    Additional keyword arguments are passed on to requests.put().
 
     """
     headers = kwargs.get("headers", {})
     headers["Content-Type"] = "application/json"
     kwargs["headers"] = headers
+    raw = _raw_response(kwargs)
     try:
         r = requests.put(resource, json=json_data, **kwargs)
     except requests.exceptions.RequestException as e:
         raise JSONAPIError("requests.put exception.", e) from e
     if r.status_code == 401:
         raise UnauthenticatedError(r)
     if not 200 <= r.status_code <= 299:
@@ -142,33 +178,42 @@
                 resource,
                 json_data,
                 kwargs,
             )
         raise JSONAPIError(
             "Unexpected HTTP status code.", r.status_code, r.content
         )
+    if raw:
+        return r
+
     reply = None
     try:
         if r.text:
             reply = r.json()
     except ValueError as e:
         raise JSONAPIError("Invalid JSON data.", r.content) from e
     return reply
 
 
 def post(resource, json_data, **kwargs):
     """Issue POST request with JSON_DATA as body to RESOURCE and return
     parsed JSON reply or None if the request failed or returned
-    invalid JSON data.  Additional keyword arguments are passed on to
-    requests.post().
+    invalid JSON data.
+
+    If keyword argument raw_response is True, the raw requests
+    response object is returned.  This is useful, for example, if the
+    caller needs to get a response header.
+
+    Additional keyword arguments are passed on to requests.post().
 
     """
     headers = kwargs.get("headers", {})
     headers["Content-Type"] = "application/json"
     kwargs["headers"] = headers
+    raw = _raw_response(kwargs)
     try:
         r = requests.post(resource, json=json_data, **kwargs)
     except requests.exceptions.RequestException as e:
         raise JSONAPIError("requests.post exception.", e) from e
     if r.status_code == 401:
         raise UnauthenticatedError(r)
     if not 200 <= r.status_code <= 299:
@@ -180,29 +225,38 @@
                 resource,
                 json_data,
                 kwargs,
             )
         raise JSONAPIError(
             "Unexpected HTTP status code.", r.status_code, r.content
         )
+    if raw:
+        return r
+
     reply = None
     try:
         if r.text:
             reply = r.json()
     except ValueError as e:
         raise JSONAPIError("Invalid JSON data.", r.content) from e
     return reply
 
 
 def delete(resource, **kwargs):
     """Issue DELETE request for RESOURCE and return the parsed JSON data
     or None if the request failed or returned invalid JSON data.
+
+    If keyword argument raw_response is True, the raw requests
+    response object is returned.  This is useful, for example, if the
+    caller needs to get a response header.
+
     Additional keyword arguments are passed on to requests.delete().
 
     """
+    raw = _raw_response(kwargs)
     try:
         r = requests.delete(resource, **kwargs)
     except requests.exceptions.RequestException as e:
         raise JSONAPIError("requests.delete exception.", e) from e
     if r.status_code == 401:
         raise UnauthenticatedError(r)
     if r.status_code < 200 or r.status_code > 299:
@@ -211,14 +265,17 @@
                 "HTTP DELETE status code %s.  Keyword args: %s",
                 r.status_code,
                 kwargs,
             )
         raise JSONAPIError(
             "Unexpected HTTP status code.", r.status_code, r.content
         )
+    if raw:
+        return r
+
     reply = None
     try:
         if r.text:
             reply = r.json()
     except ValueError as e:
         raise JSONAPIError("Invalid JSON data.", r.content) from e
     return reply
```

### Comparing `egauge-python-0.7.1/egauge_python.egg-info/PKG-INFO` & `egauge-python-0.7.2/egauge_python.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,88 +1,85 @@
 Metadata-Version: 2.1
 Name: egauge-python
-Version: 0.7.1
+Version: 0.7.2
 Summary: .
 Home-page: https://bitbucket.org/egauge/python/
 Author: David Mosberger-Tang
 Author-email: davidm@egauge.net
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
+Provides-Extra: examples
 License-File: LICENSE
 
-eGauge open source Python code
-******************************
+# eGauge open source Python code
 
 This repository is a collection of Python packages that have been
 released by eGauge Systems LLC as open source (MIT license).  These
 are released in the hope that they may be useful for other developers.
 Please see LICENSE for details.  eGauge Systems LLC also reserved the
 rights to add, modify, or remove code from this repository or the
 entire repository without notice.
 
-|
+## Example Programs
 
-Overview of available modules
-=============================
+Example programs can be found in the `examples` subdirectory.  If you
+want to run these programs, ensure that all dependencies are installed
+by running the command:
 
-|
+```sh
+pip install egauge-python[examples]
+```
 
-egauge.webapi
--------------
+Before running these programs, set the following environment variables
+for your preferred test device:
+
+ * EGDEV: URL of the test device (e.g., "http://eGaugeXXXXX.local" or
+   "http://eGaugeXXXX.d.egauge.net")
+ * EGUSR: Username to authenticate with (e.g., "owner")
+ * EGPWD: Password to authenticate with (e.g., "super-secret-pw")
+
+## Overview of available modules
+
+### egauge.webapi
 
 The classes in this module provide access to eGauge web services.  The
 APIs may be available on eGauge devices and/or as cloud-based web
 services.
 
-|
-
-egauge.webapi.device
---------------------
+### egauge.webapi.device
 
 The classes in this module provide access to APIs implemented on
 eGauge devices.
 
-|
-
-egauge.webapi.cloud
--------------------
+### egauge.webapi.cloud
 
 The classes in this module provide access to APIs implemented by
 eGauge cloud services.
 
-|
-
-egauge.ctid
------------
+### egauge.ctid
 
 The classes in this module support manufacturing CTid® sensors.  CTid®
 is patented technology and shall be used in accordance with the
 licensing agreements governing its use.
 
-|
-
-egauge.pyside2
---------------
+### egauge.pyside2
 
 The classes in this module support QT5-based graphical
 user-interfaces.
 
-|
-
-Source Code Conventions
-=======================
+## Source Code Conventions
 
 Source code should be formatted with ``black`` using a maximum line-length
 of 79 characters.  Black can be installed with ``pip install black``.
 If the resulting output is inadequate for some reason, such as manually
 formatted data tables, you can make judicious use of ``# fmt: off`` and
 ``# fmt: on`` to disable formatting for the relevant lines.
```

### Comparing `egauge-python-0.7.1/setup.py` & `egauge-python-0.7.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 import os
 import setuptools
 
-with open(os.path.join(os.path.dirname(__file__), "README.rst")) as readme:
+with open(os.path.join(os.path.dirname(__file__), "README.md")) as readme:
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setuptools.setup(
     name="egauge-python",
-    version="0.7.1",
+    version="0.7.2",
     packages=setuptools.find_namespace_packages(include="egauge.*"),
     install_requires=[
         "crcmod",
         "deprecated",
         "intelhex",
         "wheel",
         "pexpect",
         "requests>=2.4.2",
     ],
+    extras_require={
+        "examples": [
+            "matplotlib",
+            "pytz",
+            "readchar"
+        ]
+    },
     include_package_data=True,
     entry_points={
         "console_scripts": ["ctid-encoder = egauge.ctid.encoder:main"]
     },
     license="MIT License",  # example license
     description=".",
     long_description=README,
-    long_description_content_type="text/x-rst",
+    long_description_content_type="text/markdown",
     url="https://bitbucket.org/egauge/python/",
     author="David Mosberger-Tang",
     author_email="davidm@egauge.net",
     python_requires=">=3.6",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
```

