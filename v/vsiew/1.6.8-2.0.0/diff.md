# Comparing `tmp/vsiew-1.6.8.tar.gz` & `tmp/vsiew-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsiew-1.6.8.tar", last modified: Tue Mar 28 18:21:34 2023, max compression
+gzip compressed data, was "vsiew-2.0.0.tar", last modified: Mon Apr 10 12:00:52 2023, max compression
```

## Comparing `vsiew-1.6.8.tar` & `vsiew-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:21:34.520006 vsiew-1.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-28 18:21:10.000000 vsiew-1.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-28 18:21:34.520006 vsiew-1.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-28 18:21:10.000000 vsiew-1.6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 18:21:34.520006 vsiew-1.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-03-28 18:21:10.000000 vsiew-1.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:21:34.520006 vsiew-1.6.8/vsiew/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-28 18:21:10.000000 vsiew-1.6.8/vsiew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-28 18:21:10.000000 vsiew-1.6.8/vsiew/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-03-28 18:21:10.000000 vsiew-1.6.8/vsiew/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-03-28 18:21:10.000000 vsiew-1.6.8/vsiew/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:21:34.520006 vsiew-1.6.8/vsiew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-28 18:21:34.000000 vsiew-1.6.8/vsiew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-28 18:21:34.000000 vsiew-1.6.8/vsiew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 18:21:34.000000 vsiew-1.6.8/vsiew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-28 18:21:34.000000 vsiew-1.6.8/vsiew.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-28 18:21:34.000000 vsiew-1.6.8/vsiew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-28 18:21:34.000000 vsiew-1.6.8/vsiew.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:00:52.663651 vsiew-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-10 12:00:31.000000 vsiew-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-10 12:00:52.663651 vsiew-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-10 12:00:31.000000 vsiew-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 12:00:52.663651 vsiew-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-10 12:00:31.000000 vsiew-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:00:52.663651 vsiew-2.0.0/vsiew/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-10 12:00:31.000000 vsiew-2.0.0/vsiew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-10 12:00:31.000000 vsiew-2.0.0/vsiew/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-10 12:00:31.000000 vsiew-2.0.0/vsiew/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-10 12:00:31.000000 vsiew-2.0.0/vsiew/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:00:52.663651 vsiew-2.0.0/vsiew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-10 12:00:52.000000 vsiew-2.0.0/vsiew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-10 12:00:52.000000 vsiew-2.0.0/vsiew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 12:00:52.000000 vsiew-2.0.0/vsiew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-10 12:00:52.000000 vsiew-2.0.0/vsiew.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-10 12:00:52.000000 vsiew-2.0.0/vsiew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 12:00:52.000000 vsiew-2.0.0/vsiew.egg-info/top_level.txt
```

### Comparing `vsiew-1.6.8/LICENSE` & `vsiew-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vsiew-1.6.8/PKG-INFO` & `vsiew-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsiew
-Version: 1.6.8
+Version: 2.0.0
 Summary: VapourSynth packages from Irrational Encoding Wizardry
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
@@ -25,7 +25,22 @@
 ## How to install
 
 Install `vsiew` with the following command:
 
 ```sh
 pip install vsiew
 ```
+
+<br>
+
+## How to use
+
+Install all iew packages:
+```sh
+python -m vsiew
+```
+
+Install latest git version of all iew packages:
+```sh
+python -m vsiew latest
+```
+
```

### Comparing `vsiew-1.6.8/setup.py` & `vsiew-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `vsiew-1.6.8/vsiew.egg-info/PKG-INFO` & `vsiew-2.0.0/vsiew.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsiew
-Version: 1.6.8
+Version: 2.0.0
 Summary: VapourSynth packages from Irrational Encoding Wizardry
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
@@ -25,7 +25,22 @@
 ## How to install
 
 Install `vsiew` with the following command:
 
 ```sh
 pip install vsiew
 ```
+
+<br>
+
+## How to use
+
+Install all iew packages:
+```sh
+python -m vsiew
+```
+
+Install latest git version of all iew packages:
+```sh
+python -m vsiew latest
+```
+
```

