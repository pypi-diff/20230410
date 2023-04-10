# Comparing `tmp/pygeometa-0.9.0.tar.gz` & `tmp/pygeometa-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pygeometa-0.9.0.tar", last modified: Sun Feb  6 21:23:08 2022, max compression
+gzip compressed data, was "dist/pygeometa-0.9.1.tar", last modified: Tue Mar  1 01:16:35 2022, max compression
```

## Comparing `pygeometa-0.9.0.tar` & `pygeometa-0.9.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-02-06 21:23:08.000000 pygeometa-0.9.0/
--rw-r--r--   0 tomkralidis   (501) staff       (20)     1881 2020-06-11 11:12:37.000000 pygeometa-0.9.0/LICENSE.md
--rw-rw-r--   0 tomkralidis   (501) staff       (20)      101 2021-09-03 15:43:50.000000 pygeometa-0.9.0/MANIFEST.in
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     7772 2022-02-06 21:23:08.000000 pygeometa-0.9.0/PKG-INFO
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     5520 2021-09-03 15:43:50.000000 pygeometa-0.9.0/README.md
-drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-02-06 21:23:08.000000 pygeometa-0.9.0/pygeometa/
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     2454 2022-02-06 21:18:37.000000 pygeometa-0.9.0/pygeometa/__init__.py
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     2805 2022-01-06 15:56:58.000000 pygeometa-0.9.0/pygeometa/cli_options.py
--rw-rw-r--   0 tomkralidis   (501) staff       (20)    16309 2022-01-06 15:56:58.000000 pygeometa-0.9.0/pygeometa/core.py
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     2995 2021-10-14 23:41:51.000000 pygeometa-0.9.0/pygeometa/helpers.py
-drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-02-06 21:23:08.000000 pygeometa-0.9.0/pygeometa/schemas/
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     4213 2021-09-10 22:59:43.000000 pygeometa-0.9.0/pygeometa/schemas/__init__.py
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     3245 2021-10-12 01:33:13.000000 pygeometa-0.9.0/pygeometa/schemas/base.py
-drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-02-06 21:23:08.000000 pygeometa-0.9.0/pygeometa/schemas/common/
--rw-rw-r--   0 tomkralidis   (501) staff       (20)      813 2021-08-26 16:31:02.000000 pygeometa-0.9.0/pygeometa/schemas/common/iso19139-charstring.j2
-drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-02-06 21:23:08.000000 pygeometa-0.9.0/pygeometa/schemas/dcat/
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     8984 2022-01-06 15:56:58.000000 pygeometa-0.9.0/pygeometa/schemas/dcat/__init__.py
-drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-02-06 21:23:08.000000 pygeometa-0.9.0/pygeometa/schemas/iso19139/
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     2403 2021-08-26 16:31:02.000000 pygeometa-0.9.0/pygeometa/schemas/iso19139/__init__.py
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     3897 2021-09-03 15:43:50.000000 pygeometa-0.9.0/pygeometa/schemas/iso19139/contact.j2
--rw-rw-r--   0 tomkralidis   (501) staff       (20)    23253 2022-01-06 15:56:58.000000 pygeometa-0.9.0/pygeometa/schemas/iso19139/main.j2
-drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-02-06 21:23:08.000000 pygeometa-0.9.0/pygeometa/schemas/iso19139_2/
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     2409 2021-08-26 16:31:02.000000 pygeometa-0.9.0/pygeometa/schemas/iso19139_2/__init__.py
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     3897 2021-09-03 15:43:50.000000 pygeometa-0.9.0/pygeometa/schemas/iso19139_2/contact.j2
--rw-rw-r--   0 tomkralidis   (501) staff       (20)    24172 2022-01-06 15:56:58.000000 pygeometa-0.9.0/pygeometa/schemas/iso19139_2/main.j2
-drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-02-06 21:23:08.000000 pygeometa-0.9.0/pygeometa/schemas/iso19139_hnap/
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     2417 2021-08-26 16:31:02.000000 pygeometa-0.9.0/pygeometa/schemas/iso19139_hnap/__init__.py
--rw-rw-r--   0 tomkralidis   (501) staff       (20)      792 2021-08-26 16:31:02.000000 pygeometa-0.9.0/pygeometa/schemas/iso19139_hnap/charstring.j2
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     3205 2021-09-03 15:43:50.000000 pygeometa-0.9.0/pygeometa/schemas/iso19139_hnap/contact.j2
--rw-rw-r--   0 tomkralidis   (501) staff       (20)    32449 2022-01-06 15:56:58.000000 pygeometa-0.9.0/pygeometa/schemas/iso19139_hnap/main.j2
-drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-02-06 21:23:08.000000 pygeometa-0.9.0/pygeometa/schemas/mcf/
--rw-rw-r--   0 tomkralidis   (501) staff       (20)    22163 2022-01-06 15:56:58.000000 pygeometa-0.9.0/pygeometa/schemas/mcf/core.yml
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     1401 2021-09-03 15:43:50.000000 pygeometa-0.9.0/pygeometa/schemas/mcf/iso19139_2.yml
--rw-rw-r--   0 tomkralidis   (501) staff       (20)      795 2021-09-03 15:43:50.000000 pygeometa-0.9.0/pygeometa/schemas/mcf/wmo-cmp.yml
--rw-rw-r--   0 tomkralidis   (501) staff       (20)    15197 2021-09-03 15:43:50.000000 pygeometa-0.9.0/pygeometa/schemas/mcf/wmo-wigos.yml
-drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-02-06 21:23:08.000000 pygeometa-0.9.0/pygeometa/schemas/ogcapi_records/
--rw-rw-r--   0 tomkralidis   (501) staff       (20)    10376 2022-01-06 15:56:58.000000 pygeometa-0.9.0/pygeometa/schemas/ogcapi_records/__init__.py
-drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-02-06 21:23:08.000000 pygeometa-0.9.0/pygeometa/schemas/stac/
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     4979 2022-01-06 15:56:58.000000 pygeometa-0.9.0/pygeometa/schemas/stac/__init__.py
-drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-02-06 21:23:08.000000 pygeometa-0.9.0/pygeometa/schemas/wmo_cmp/
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     2416 2021-08-26 16:31:02.000000 pygeometa-0.9.0/pygeometa/schemas/wmo_cmp/__init__.py
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     3922 2021-09-03 15:43:50.000000 pygeometa-0.9.0/pygeometa/schemas/wmo_cmp/contact.j2
--rw-rw-r--   0 tomkralidis   (501) staff       (20)    23611 2022-01-06 15:56:58.000000 pygeometa-0.9.0/pygeometa/schemas/wmo_cmp/main.j2
-drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-02-06 21:23:08.000000 pygeometa-0.9.0/pygeometa/schemas/wmo_wigos/
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     2404 2021-08-26 16:31:02.000000 pygeometa-0.9.0/pygeometa/schemas/wmo_wigos/__init__.py
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     3914 2021-09-03 15:43:50.000000 pygeometa-0.9.0/pygeometa/schemas/wmo_wigos/contact.j2
--rw-rw-r--   0 tomkralidis   (501) staff       (20)    15110 2021-08-26 16:31:02.000000 pygeometa-0.9.0/pygeometa/schemas/wmo_wigos/main.j2
-drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-02-06 21:23:08.000000 pygeometa-0.9.0/pygeometa.egg-info/
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     7772 2022-02-06 21:23:07.000000 pygeometa-0.9.0/pygeometa.egg-info/PKG-INFO
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     1328 2022-02-06 21:23:07.000000 pygeometa-0.9.0/pygeometa.egg-info/SOURCES.txt
--rw-rw-r--   0 tomkralidis   (501) staff       (20)        1 2022-02-06 21:23:07.000000 pygeometa-0.9.0/pygeometa.egg-info/dependency_links.txt
--rw-rw-r--   0 tomkralidis   (501) staff       (20)       45 2022-02-06 21:23:07.000000 pygeometa-0.9.0/pygeometa.egg-info/entry_points.txt
--rw-rw-r--   0 tomkralidis   (501) staff       (20)       31 2022-02-06 21:23:07.000000 pygeometa-0.9.0/pygeometa.egg-info/requires.txt
--rw-rw-r--   0 tomkralidis   (501) staff       (20)       10 2022-02-06 21:23:07.000000 pygeometa-0.9.0/pygeometa.egg-info/top_level.txt
--rw-rw-r--   0 tomkralidis   (501) staff       (20)       31 2021-09-03 15:43:50.000000 pygeometa-0.9.0/requirements.txt
--rw-rw-r--   0 tomkralidis   (501) staff       (20)       38 2022-02-06 21:23:08.000000 pygeometa-0.9.0/setup.cfg
--rw-r--r--   0 tomkralidis   (501) staff       (20)     4503 2020-06-11 11:12:37.000000 pygeometa-0.9.0/setup.py
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-03-01 01:16:35.000000 pygeometa-0.9.1/
+-rw-r--r--   0 tomkralidis   (501) staff       (20)     1881 2020-06-11 11:12:37.000000 pygeometa-0.9.1/LICENSE.md
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)      101 2021-09-03 15:43:50.000000 pygeometa-0.9.1/MANIFEST.in
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     7772 2022-03-01 01:16:35.000000 pygeometa-0.9.1/PKG-INFO
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     5520 2021-09-03 15:43:50.000000 pygeometa-0.9.1/README.md
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-03-01 01:16:35.000000 pygeometa-0.9.1/pygeometa/
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     2454 2022-03-01 01:14:59.000000 pygeometa-0.9.1/pygeometa/__init__.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     2805 2022-01-06 15:56:58.000000 pygeometa-0.9.1/pygeometa/cli_options.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)    16309 2022-01-06 15:56:58.000000 pygeometa-0.9.1/pygeometa/core.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     2995 2021-10-14 23:41:51.000000 pygeometa-0.9.1/pygeometa/helpers.py
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-03-01 01:16:35.000000 pygeometa-0.9.1/pygeometa/schemas/
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     4213 2021-09-10 22:59:43.000000 pygeometa-0.9.1/pygeometa/schemas/__init__.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     3245 2021-10-12 01:33:13.000000 pygeometa-0.9.1/pygeometa/schemas/base.py
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-03-01 01:16:35.000000 pygeometa-0.9.1/pygeometa/schemas/common/
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)      813 2021-08-26 16:31:02.000000 pygeometa-0.9.1/pygeometa/schemas/common/iso19139-charstring.j2
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-03-01 01:16:35.000000 pygeometa-0.9.1/pygeometa/schemas/dcat/
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     8984 2022-01-06 15:56:58.000000 pygeometa-0.9.1/pygeometa/schemas/dcat/__init__.py
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-03-01 01:16:35.000000 pygeometa-0.9.1/pygeometa/schemas/iso19139/
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     2403 2021-08-26 16:31:02.000000 pygeometa-0.9.1/pygeometa/schemas/iso19139/__init__.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     3897 2021-09-03 15:43:50.000000 pygeometa-0.9.1/pygeometa/schemas/iso19139/contact.j2
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)    23253 2022-01-06 15:56:58.000000 pygeometa-0.9.1/pygeometa/schemas/iso19139/main.j2
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-03-01 01:16:35.000000 pygeometa-0.9.1/pygeometa/schemas/iso19139_2/
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     2409 2021-08-26 16:31:02.000000 pygeometa-0.9.1/pygeometa/schemas/iso19139_2/__init__.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     3897 2021-09-03 15:43:50.000000 pygeometa-0.9.1/pygeometa/schemas/iso19139_2/contact.j2
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)    24172 2022-01-06 15:56:58.000000 pygeometa-0.9.1/pygeometa/schemas/iso19139_2/main.j2
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-03-01 01:16:35.000000 pygeometa-0.9.1/pygeometa/schemas/iso19139_hnap/
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     2417 2021-08-26 16:31:02.000000 pygeometa-0.9.1/pygeometa/schemas/iso19139_hnap/__init__.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)      792 2021-08-26 16:31:02.000000 pygeometa-0.9.1/pygeometa/schemas/iso19139_hnap/charstring.j2
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     3205 2021-09-03 15:43:50.000000 pygeometa-0.9.1/pygeometa/schemas/iso19139_hnap/contact.j2
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)    32449 2022-01-06 15:56:58.000000 pygeometa-0.9.1/pygeometa/schemas/iso19139_hnap/main.j2
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-03-01 01:16:35.000000 pygeometa-0.9.1/pygeometa/schemas/mcf/
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)    22163 2022-01-06 15:56:58.000000 pygeometa-0.9.1/pygeometa/schemas/mcf/core.yml
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     1401 2021-09-03 15:43:50.000000 pygeometa-0.9.1/pygeometa/schemas/mcf/iso19139_2.yml
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)      795 2021-09-03 15:43:50.000000 pygeometa-0.9.1/pygeometa/schemas/mcf/wmo-cmp.yml
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)    15197 2021-09-03 15:43:50.000000 pygeometa-0.9.1/pygeometa/schemas/mcf/wmo-wigos.yml
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-03-01 01:16:35.000000 pygeometa-0.9.1/pygeometa/schemas/ogcapi_records/
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)    10394 2022-03-01 01:12:17.000000 pygeometa-0.9.1/pygeometa/schemas/ogcapi_records/__init__.py
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-03-01 01:16:35.000000 pygeometa-0.9.1/pygeometa/schemas/stac/
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     4979 2022-01-06 15:56:58.000000 pygeometa-0.9.1/pygeometa/schemas/stac/__init__.py
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-03-01 01:16:35.000000 pygeometa-0.9.1/pygeometa/schemas/wmo_cmp/
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     2416 2021-08-26 16:31:02.000000 pygeometa-0.9.1/pygeometa/schemas/wmo_cmp/__init__.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     3922 2021-09-03 15:43:50.000000 pygeometa-0.9.1/pygeometa/schemas/wmo_cmp/contact.j2
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)    23611 2022-01-06 15:56:58.000000 pygeometa-0.9.1/pygeometa/schemas/wmo_cmp/main.j2
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-03-01 01:16:35.000000 pygeometa-0.9.1/pygeometa/schemas/wmo_wigos/
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     2404 2021-08-26 16:31:02.000000 pygeometa-0.9.1/pygeometa/schemas/wmo_wigos/__init__.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     3914 2021-09-03 15:43:50.000000 pygeometa-0.9.1/pygeometa/schemas/wmo_wigos/contact.j2
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)    15110 2021-08-26 16:31:02.000000 pygeometa-0.9.1/pygeometa/schemas/wmo_wigos/main.j2
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2022-03-01 01:16:35.000000 pygeometa-0.9.1/pygeometa.egg-info/
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     7772 2022-03-01 01:16:35.000000 pygeometa-0.9.1/pygeometa.egg-info/PKG-INFO
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     1328 2022-03-01 01:16:35.000000 pygeometa-0.9.1/pygeometa.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)        1 2022-03-01 01:16:35.000000 pygeometa-0.9.1/pygeometa.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)       45 2022-03-01 01:16:35.000000 pygeometa-0.9.1/pygeometa.egg-info/entry_points.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)       31 2022-03-01 01:16:35.000000 pygeometa-0.9.1/pygeometa.egg-info/requires.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)       10 2022-03-01 01:16:35.000000 pygeometa-0.9.1/pygeometa.egg-info/top_level.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)       31 2021-09-03 15:43:50.000000 pygeometa-0.9.1/requirements.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)       38 2022-03-01 01:16:35.000000 pygeometa-0.9.1/setup.cfg
+-rw-r--r--   0 tomkralidis   (501) staff       (20)     4503 2020-06-11 11:12:37.000000 pygeometa-0.9.1/setup.py
```

### Comparing `pygeometa-0.9.0/LICENSE.md` & `pygeometa-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/PKG-INFO` & `pygeometa-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeometa
-Version: 0.9.0
+Version: 0.9.1
 Summary: pygeometa is a Python package to generate metadata for geospatial datasets
 Home-page: https://geopython.github.io/pygeometa
 Author: Meteorological Service of Canada
 Author-email: tom.kralidis@canada.ca
 Maintainer: Meteorological Service of Canada
 Maintainer-email: tom.kralidis@canada.ca
 License: MIT
```

### Comparing `pygeometa-0.9.0/README.md` & `pygeometa-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/__init__.py` & `pygeometa-0.9.1/pygeometa/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 #
 # =================================================================
 
 import click
 
 from pygeometa.core import generate, info, schemas, validate
 
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 
 
 @click.group()
 @click.version_option(version=__version__)
 def cli():
     pass
```

### Comparing `pygeometa-0.9.0/pygeometa/cli_options.py` & `pygeometa-0.9.1/pygeometa/cli_options.py`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/core.py` & `pygeometa-0.9.1/pygeometa/core.py`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/helpers.py` & `pygeometa-0.9.1/pygeometa/helpers.py`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/schemas/__init__.py` & `pygeometa-0.9.1/pygeometa/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/schemas/base.py` & `pygeometa-0.9.1/pygeometa/schemas/base.py`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/schemas/common/iso19139-charstring.j2` & `pygeometa-0.9.1/pygeometa/schemas/common/iso19139-charstring.j2`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/schemas/dcat/__init__.py` & `pygeometa-0.9.1/pygeometa/schemas/dcat/__init__.py`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/schemas/iso19139/__init__.py` & `pygeometa-0.9.1/pygeometa/schemas/iso19139/__init__.py`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/schemas/iso19139/contact.j2` & `pygeometa-0.9.1/pygeometa/schemas/iso19139/contact.j2`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/schemas/iso19139/main.j2` & `pygeometa-0.9.1/pygeometa/schemas/iso19139/main.j2`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/schemas/iso19139_2/__init__.py` & `pygeometa-0.9.1/pygeometa/schemas/iso19139_2/__init__.py`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/schemas/iso19139_2/contact.j2` & `pygeometa-0.9.1/pygeometa/schemas/iso19139_2/contact.j2`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/schemas/iso19139_2/main.j2` & `pygeometa-0.9.1/pygeometa/schemas/iso19139_2/main.j2`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/schemas/iso19139_hnap/__init__.py` & `pygeometa-0.9.1/pygeometa/schemas/iso19139_hnap/__init__.py`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/schemas/iso19139_hnap/charstring.j2` & `pygeometa-0.9.1/pygeometa/schemas/iso19139_hnap/charstring.j2`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/schemas/iso19139_hnap/contact.j2` & `pygeometa-0.9.1/pygeometa/schemas/iso19139_hnap/contact.j2`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/schemas/iso19139_hnap/main.j2` & `pygeometa-0.9.1/pygeometa/schemas/iso19139_hnap/main.j2`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/schemas/mcf/core.yml` & `pygeometa-0.9.1/pygeometa/schemas/mcf/core.yml`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/schemas/mcf/iso19139_2.yml` & `pygeometa-0.9.1/pygeometa/schemas/mcf/iso19139_2.yml`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/schemas/mcf/wmo-cmp.yml` & `pygeometa-0.9.1/pygeometa/schemas/mcf/wmo-cmp.yml`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/schemas/mcf/wmo-wigos.yml` & `pygeometa-0.9.1/pygeometa/schemas/mcf/wmo-wigos.yml`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/schemas/ogcapi_records/__init__.py` & `pygeometa-0.9.1/pygeometa/schemas/ogcapi_records/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,17 +117,17 @@
                 'language': lang1,
                 'type': mcf['metadata']['hierarchylevel'],
                 'extent': {
                     'spatial': {
                         'bbox': [[minx, miny, maxx, maxy]],
                         'crs': 'http://www.opengis.net/def/crs/OGC/1.3/CRS84'  # noqa
                     }
-                }
+                },
+                'associations': []
             },
-            'associations': [],
             'links': []
         }
 
         if 'temporal' in mcf['identification']['extents']:
             begin = mcf['identification']['extents']['temporal'][0]['begin']
             end = mcf['identification']['extents']['temporal'][0]['end']
 
@@ -197,15 +197,15 @@
                 link['title'] = name[0]
             elif name != [None, None]:
                 link['title'] = name[0]
 
             if all(x in value['url'] for x in ['{', '}']):
                 link['templated'] = True
 
-            record['associations'].append(link)
+            record['properties']['associations'].append(link)
 
         if stringify:
             return json.dumps(record, default=json_serial, indent=4)
 
         return record
 
     def generate_responsible_party(self, contact: dict,
```

### Comparing `pygeometa-0.9.0/pygeometa/schemas/stac/__init__.py` & `pygeometa-0.9.1/pygeometa/schemas/stac/__init__.py`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/schemas/wmo_cmp/__init__.py` & `pygeometa-0.9.1/pygeometa/schemas/wmo_cmp/__init__.py`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/schemas/wmo_cmp/contact.j2` & `pygeometa-0.9.1/pygeometa/schemas/wmo_cmp/contact.j2`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/schemas/wmo_cmp/main.j2` & `pygeometa-0.9.1/pygeometa/schemas/wmo_cmp/main.j2`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/schemas/wmo_wigos/__init__.py` & `pygeometa-0.9.1/pygeometa/schemas/wmo_wigos/__init__.py`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/schemas/wmo_wigos/contact.j2` & `pygeometa-0.9.1/pygeometa/schemas/wmo_wigos/contact.j2`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa/schemas/wmo_wigos/main.j2` & `pygeometa-0.9.1/pygeometa/schemas/wmo_wigos/main.j2`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/pygeometa.egg-info/PKG-INFO` & `pygeometa-0.9.1/pygeometa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeometa
-Version: 0.9.0
+Version: 0.9.1
 Summary: pygeometa is a Python package to generate metadata for geospatial datasets
 Home-page: https://geopython.github.io/pygeometa
 Author: Meteorological Service of Canada
 Author-email: tom.kralidis@canada.ca
 Maintainer: Meteorological Service of Canada
 Maintainer-email: tom.kralidis@canada.ca
 License: MIT
```

### Comparing `pygeometa-0.9.0/pygeometa.egg-info/SOURCES.txt` & `pygeometa-0.9.1/pygeometa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygeometa-0.9.0/setup.py` & `pygeometa-0.9.1/setup.py`

 * *Files identical despite different names*

