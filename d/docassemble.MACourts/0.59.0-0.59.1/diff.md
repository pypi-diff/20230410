# Comparing `tmp/docassemble.MACourts-0.59.0.tar.gz` & `tmp/docassemble.MACourts-0.59.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docassemble.MACourts-0.59.0.tar", last modified: Wed Mar  8 14:12:25 2023, max compression
+gzip compressed data, was "docassemble.MACourts-0.59.1.tar", last modified: Mon Apr 10 20:43:50 2023, max compression
```

## Comparing `docassemble.MACourts-0.59.0.tar` & `docassemble.MACourts-0.59.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 14:12:25.483521 docassemble.MACourts-0.59.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-03-08 14:12:25.483521 docassemble.MACourts-0.59.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      402 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 14:12:25.475521 docassemble.MACourts-0.59.0/docassemble/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 14:12:25.475521 docassemble.MACourts-0.59.0/docassemble/MACourts/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 14:12:25.471521 docassemble.MACourts-0.59.0/docassemble/MACourts/data/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 14:12:25.475521 docassemble.MACourts-0.59.0/docassemble/MACourts/data/questions/
--rw-r--r--   0 runner    (1001) docker     (122)      800 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/data/questions/cache_macourts.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2738 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/data/questions/court_test_bulk.yml
--rw-r--r--   0 runner    (1001) docker     (122)     5093 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/data/questions/courts_tester.yml
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/data/questions/courts_to_xlsx.yml
--rw-r--r--   0 runner    (1001) docker     (122)      657 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/data/questions/test_get_court_by_code.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/data/questions/test_list_ma_courts.yml
--rw-r--r--   0 runner    (1001) docker     (122)      774 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/data/questions/test_local_court_json_files.yml
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/data/questions/test_macourts.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 14:12:25.479521 docassemble.MACourts-0.59.0/docassemble/MACourts/data/sources/
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/data/sources/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1647 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/data/sources/appeals_court.json
--rw-r--r--   0 runner    (1001) docker     (122)     7224 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/data/sources/bmc.json
--rw-r--r--   0 runner    (1001) docker     (122)  2540031 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/data/sources/boston_wards.geojson
--rw-r--r--   0 runner    (1001) docker     (122)    52003 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/data/sources/district_courts.json
--rw-r--r--   0 runner    (1001) docker     (122)    22857 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/data/sources/housing_courts.json
--rw-r--r--   0 runner    (1001) docker     (122)    40742 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/data/sources/juvenile_courts.json
--rw-r--r--   0 runner    (1001) docker     (122)      649 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/data/sources/land_court.json
--rw-r--r--   0 runner    (1001) docker     (122)    15315 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/data/sources/probate_and_family_courts.json
--rw-r--r--   0 runner    (1001) docker     (122)    16321 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/data/sources/superior_courts.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 14:12:25.483521 docassemble.MACourts-0.59.0/docassemble/MACourts/data/static/
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/data/static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 14:12:25.483521 docassemble.MACourts-0.59.0/docassemble/MACourts/data/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/data/templates/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     9103 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/docket_tool.md
--rw-r--r--   0 runner    (1001) docker     (122)    82289 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/macourts.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 14:12:25.483521 docassemble.MACourts-0.59.0/docassemble/MACourts/test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10349 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/test/test_court_finder.py
--rw-r--r--   0 runner    (1001) docker     (122)     3548 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/test/test_docket_numbers.py
--rw-r--r--   0 runner    (1001) docker     (122)      638 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/MACourts/test_local_court_json_files.yml
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/docassemble/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 14:12:25.475521 docassemble.MACourts-0.59.0/docassemble.MACourts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-03-08 14:12:25.000000 docassemble.MACourts-0.59.0/docassemble.MACourts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1797 2023-03-08 14:12:25.000000 docassemble.MACourts-0.59.0/docassemble.MACourts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-08 14:12:25.000000 docassemble.MACourts-0.59.0/docassemble.MACourts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-03-08 14:12:25.000000 docassemble.MACourts-0.59.0/docassemble.MACourts.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-08 14:12:25.000000 docassemble.MACourts-0.59.0/docassemble.MACourts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-03-08 14:12:25.000000 docassemble.MACourts-0.59.0/docassemble.MACourts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-03-08 14:12:25.000000 docassemble.MACourts-0.59.0/docassemble.MACourts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-03-08 14:12:25.483521 docassemble.MACourts-0.59.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2688 2023-03-08 14:12:12.000000 docassemble.MACourts-0.59.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 20:43:50.727256 docassemble.MACourts-0.59.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      558 2023-04-10 20:43:50.727256 docassemble.MACourts-0.59.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      402 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 20:43:50.715256 docassemble.MACourts-0.59.1/docassemble/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 20:43:50.719256 docassemble.MACourts-0.59.1/docassemble/MACourts/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 20:43:50.715256 docassemble.MACourts-0.59.1/docassemble/MACourts/data/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 20:43:50.723256 docassemble.MACourts-0.59.1/docassemble/MACourts/data/questions/
+-rw-r--r--   0 runner    (1001) docker     (122)      800 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/data/questions/cache_macourts.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2738 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/data/questions/court_test_bulk.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     5093 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/data/questions/courts_tester.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/data/questions/courts_to_xlsx.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/data/questions/test_get_court_by_code.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/data/questions/test_list_ma_courts.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/data/questions/test_local_court_json_files.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/data/questions/test_macourts.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 20:43:50.727256 docassemble.MACourts-0.59.1/docassemble/MACourts/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/data/sources/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1647 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/data/sources/appeals_court.json
+-rw-r--r--   0 runner    (1001) docker     (122)     7224 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/data/sources/bmc.json
+-rw-r--r--   0 runner    (1001) docker     (122)  2540031 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/data/sources/boston_wards.geojson
+-rw-r--r--   0 runner    (1001) docker     (122)    52007 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/data/sources/district_courts.json
+-rw-r--r--   0 runner    (1001) docker     (122)    22857 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/data/sources/housing_courts.json
+-rw-r--r--   0 runner    (1001) docker     (122)    40742 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/data/sources/juvenile_courts.json
+-rw-r--r--   0 runner    (1001) docker     (122)      649 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/data/sources/land_court.json
+-rw-r--r--   0 runner    (1001) docker     (122)    15315 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/data/sources/probate_and_family_courts.json
+-rw-r--r--   0 runner    (1001) docker     (122)    16321 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/data/sources/superior_courts.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 20:43:50.727256 docassemble.MACourts-0.59.1/docassemble/MACourts/data/static/
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/data/static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 20:43:50.727256 docassemble.MACourts-0.59.1/docassemble/MACourts/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/data/templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     9103 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/docket_tool.md
+-rw-r--r--   0 runner    (1001) docker     (122)    82323 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/macourts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 20:43:50.727256 docassemble.MACourts-0.59.1/docassemble/MACourts/test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10349 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/test/test_court_finder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3548 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/test/test_docket_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/MACourts/test_local_court_json_files.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/docassemble/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 20:43:50.719256 docassemble.MACourts-0.59.1/docassemble.MACourts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      558 2023-04-10 20:43:50.000000 docassemble.MACourts-0.59.1/docassemble.MACourts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1797 2023-04-10 20:43:50.000000 docassemble.MACourts-0.59.1/docassemble.MACourts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 20:43:50.000000 docassemble.MACourts-0.59.1/docassemble.MACourts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-10 20:43:50.000000 docassemble.MACourts-0.59.1/docassemble.MACourts.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 20:43:50.000000 docassemble.MACourts-0.59.1/docassemble.MACourts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-04-10 20:43:50.000000 docassemble.MACourts-0.59.1/docassemble.MACourts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-10 20:43:50.000000 docassemble.MACourts-0.59.1/docassemble.MACourts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-10 20:43:50.731257 docassemble.MACourts-0.59.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2688 2023-04-10 20:43:40.000000 docassemble.MACourts-0.59.1/setup.py
```

### Comparing `docassemble.MACourts-0.59.0/LICENSE` & `docassemble.MACourts-0.59.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docassemble.MACourts-0.59.0/PKG-INFO` & `docassemble.MACourts-0.59.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docassemble.MACourts
-Version: 0.59.0
+Version: 0.59.1
 Summary: List Massachusetts Courts in Docassemble
 Home-page: https://docassemble.org
 Author: Quinten Steenhuis
 Author-email: qsteenhuis@gbls.org
 License: The MIT License (MIT)
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `docassemble.MACourts-0.59.0/docassemble/MACourts/data/questions/cache_macourts.yml` & `docassemble.MACourts-0.59.1/docassemble/MACourts/data/questions/cache_macourts.yml`

 * *Files identical despite different names*

### Comparing `docassemble.MACourts-0.59.0/docassemble/MACourts/data/questions/court_test_bulk.yml` & `docassemble.MACourts-0.59.1/docassemble/MACourts/data/questions/court_test_bulk.yml`

 * *Files identical despite different names*

### Comparing `docassemble.MACourts-0.59.0/docassemble/MACourts/data/questions/courts_tester.yml` & `docassemble.MACourts-0.59.1/docassemble/MACourts/data/questions/courts_tester.yml`

 * *Files identical despite different names*

### Comparing `docassemble.MACourts-0.59.0/docassemble/MACourts/data/questions/courts_to_xlsx.yml` & `docassemble.MACourts-0.59.1/docassemble/MACourts/data/questions/courts_to_xlsx.yml`

 * *Files identical despite different names*

### Comparing `docassemble.MACourts-0.59.0/docassemble/MACourts/data/questions/test_get_court_by_code.yml` & `docassemble.MACourts-0.59.1/docassemble/MACourts/data/questions/test_get_court_by_code.yml`

 * *Files identical despite different names*

### Comparing `docassemble.MACourts-0.59.0/docassemble/MACourts/data/questions/test_list_ma_courts.yml` & `docassemble.MACourts-0.59.1/docassemble/MACourts/data/questions/test_list_ma_courts.yml`

 * *Files identical despite different names*

### Comparing `docassemble.MACourts-0.59.0/docassemble/MACourts/data/questions/test_local_court_json_files.yml` & `docassemble.MACourts-0.59.1/docassemble/MACourts/data/questions/test_local_court_json_files.yml`

 * *Files identical despite different names*

### Comparing `docassemble.MACourts-0.59.0/docassemble/MACourts/data/sources/appeals_court.json` & `docassemble.MACourts-0.59.1/docassemble/MACourts/data/sources/appeals_court.json`

 * *Files identical despite different names*

### Comparing `docassemble.MACourts-0.59.0/docassemble/MACourts/data/sources/bmc.json` & `docassemble.MACourts-0.59.1/docassemble/MACourts/data/sources/bmc.json`

 * *Files identical despite different names*

### Comparing `docassemble.MACourts-0.59.0/docassemble/MACourts/data/sources/boston_wards.geojson` & `docassemble.MACourts-0.59.1/docassemble/MACourts/data/sources/boston_wards.geojson`

 * *Files identical despite different names*

### Comparing `docassemble.MACourts-0.59.0/docassemble/MACourts/data/sources/district_courts.json` & `docassemble.MACourts-0.59.1/docassemble/MACourts/data/sources/district_courts.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8432795698924738%*

 * *Differences: {'0': "{'ada_coordinators': [OrderedDict([('name', 'Virginia Richardson'), ('phone', '(508) "*

 * *      "222-5900, ext. 313'), ('email', 'virginia.richardson@jud.state.ma.us')])], delete: ['ADA "*

 * *      "Coordinators']}",*

 * * '1': "{'ada_coordinators': [OrderedDict([('name', 'Tina Ramos'), ('phone', '978-772-2100 ext. "*

 * *      "217'), ('email', 'tina.ramos@jud.state.ma.us')])], delete: ['ADA Coordinators']}",*

 * * '10': "{'ada_coordinators': [OrderedDict([('name', 'Eileen M. McDonnell'), ('phone', "*

 * *       "'781-329-477 […]*

```diff
@@ -1,10 +1,10 @@
 [
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "virginia.richardson@jud.state.ma.us",
                 "name": "Virginia Richardson",
                 "phone": "(508) 222-5900, ext. 313"
             }
         ],
         "address": {
@@ -25,15 +25,15 @@
         },
         "name": "Attleboro District Court",
         "phone": "(508) 222-5900 ",
         "tyler_code": "438",
         "tyler_lower_court_code": "1764"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "tina.ramos@jud.state.ma.us",
                 "name": "Tina Ramos",
                 "phone": "978-772-2100 ext. 217"
             }
         ],
         "address": {
@@ -54,15 +54,15 @@
         },
         "name": "Ayer District Court",
         "phone": "(978) 772-2100",
         "tyler_code": "336",
         "tyler_lower_court_code": "1765"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "louise.johnson@jud.state.ma.us",
                 "name": "Louise Johnson",
                 "phone": "(508) 362-0274"
             }
         ],
         "address": {
@@ -83,15 +83,15 @@
         },
         "name": "Barnstable District Court",
         "phone": "(508) 375-6778",
         "tyler_code": "815",
         "tyler_lower_court_code": "1766"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "roderick.wilmore@jud.state.ma.us",
                 "name": "Roderick Wilmore",
                 "phone": "508-897-2717"
             }
         ],
         "address": {
@@ -112,15 +112,15 @@
         },
         "name": "Brockton District Court",
         "phone": "(508) 587-8000",
         "tyler_code": "805",
         "tyler_lower_court_code": "1767"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "kristin.ohara@jud.state.ma.us",
                 "name": "Kristin O'Hara",
                 "phone": "(617) 232-4660 ext. 115"
             },
             {
                 "email": "janice.sennott@jud.state.ma.us",
@@ -146,15 +146,15 @@
         },
         "name": "Brookline District Court",
         "phone": "(617) 232-4660",
         "tyler_code": "506",
         "tyler_lower_court_code": "1768"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "Domenic.strazzullo@jud.state.ma.us",
                 "name": "Domenic Strazzullo",
                 "phone": "(781) 306-2764"
             },
             {
                 "email": "Daniel.tabares@jud.state.ma.us",
@@ -180,15 +180,15 @@
         },
         "name": "Cambridge District Court",
         "phone": "(781) 306-2715",
         "tyler_code": "490",
         "tyler_lower_court_code": "1769"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "carmine.diruzza@jud.state.ma.us",
                 "name": "Carmine DiRuzza",
                 "phone": "617-660-9273"
             }
         ],
         "address": {
@@ -209,15 +209,15 @@
         },
         "name": "Chelsea District Court",
         "phone": "(617) 660-9200",
         "tyler_code": "398",
         "tyler_lower_court_code": "1770"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "carol.diBernardo@jud.state.ma.us",
                 "name": "Carol DiBernardo",
                 "phone": "(413) 598-0099 ext. 209"
             },
             {
                 "email": "barbara.burton@jud.state.ma.us",
@@ -243,15 +243,15 @@
         },
         "name": "Chicopee District Court",
         "phone": "(413) 598-0099",
         "tyler_code": "455",
         "tyler_lower_court_code": "1771"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "mary.rauscher@jud.state.ma.us",
                 "name": "Mary Rauscher",
                 "phone": "978-368-7811 x239"
             }
         ],
         "address": {
@@ -272,15 +272,15 @@
         },
         "name": "Clinton District Court",
         "phone": "(978) 368-7811",
         "tyler_code": "411",
         "tyler_lower_court_code": "1772"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "evan.gilman@jud.state.ma.us",
                 "name": "Evan Gilman",
                 "phone": "(978) 369-0500 ext. 623"
             }
         ],
         "address": {
@@ -301,15 +301,15 @@
         },
         "name": "Concord District Court",
         "phone": "(978) 369-0500",
         "tyler_code": "383",
         "tyler_lower_court_code": "1773"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "eileen.mcdonnell@jud.state.ma.us",
                 "name": "Eileen M. McDonnell",
                 "phone": "781-329-4777 x:303"
             }
         ],
         "address": {
@@ -330,15 +330,15 @@
         },
         "name": "Dedham District Court",
         "phone": "(781) 329-4777",
         "tyler_code": "507",
         "tyler_lower_court_code": "1774"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "joseph.moriarty@jud.state.ma.us",
                 "name": "Joseph Moriarty",
                 "phone": "508-943-7123 x133"
             }
         ],
         "address": {
@@ -359,15 +359,15 @@
         },
         "name": "Dudley District Court",
         "phone": "(508) 943-7123",
         "tyler_code": "447",
         "tyler_lower_court_code": "1775"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "lisa.skutnik@jud.state.ma.us",
                 "name": "Lisa Skutnik",
                 "phone": "508-885-6305 ext. 2711811"
             },
             {
                 "email": "klaudio.tanto@jud.state.ma.us",
@@ -393,15 +393,15 @@
         },
         "name": "East Brookfield District Court",
         "phone": "(508) 885-6305",
         "tyler_code": "449",
         "tyler_lower_court_code": "1776"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "kathleen.mitchell@jud.state.ma.us",
                 "name": "Kathleen Mitchell",
                 "phone": "413-213-7659"
             },
             {
                 "email": "robin.balicki@jud.state.ma.us",
@@ -450,15 +450,15 @@
         },
         "name": "Edgartown District Court",
         "phone": "",
         "tyler_code": "484",
         "tyler_lower_court_code": "1778"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "maura.donovan@jud.state.ma.us",
                 "name": "Maura Donovan",
                 "phone": "508-491-3264"
             }
         ],
         "address": {
@@ -480,15 +480,15 @@
         },
         "name": "Fall River District Court",
         "phone": "",
         "tyler_code": "470",
         "tyler_lower_court_code": "1779"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "tee.sadler@jud.state.ma.us",
                 "name": "Tee Sadler",
                 "phone": "508-495-1500"
             }
         ],
         "address": {
@@ -509,15 +509,15 @@
         },
         "name": "Falmouth District Court",
         "phone": "(508) 495-1500",
         "tyler_code": "486",
         "tyler_lower_court_code": "1780"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "sharon.shosey@jud.state.ma.us",
                 "name": "Sharon Shosey",
                 "phone": "978-345-2111"
             },
             {
                 "email": "denise.vasko@jud.state.ma.us",
@@ -584,18 +584,18 @@
         "location": {
             "latitude": 42.293395,
             "longitude": -71.409619
         },
         "name": "Natick District Court",
         "phone": "(508) 620-9110",
         "tyler_code": "443",
-        "tyler_lower_court_code": ""
+        "tyler_lower_court_code": "1798"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "kimberly.walsh@jud.state.ma.us",
                 "name": "Kimberly A Walsh",
                 "phone": "978-632-2373 x112"
             }
         ],
         "address": {
@@ -616,15 +616,15 @@
         },
         "name": "Gardner District Court",
         "phone": "(978) 632-2373",
         "tyler_code": "422",
         "tyler_lower_court_code": "1783"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "melissa.teixeira@jud.state.ma.us",
                 "name": "Melissa Joy Teixeira",
                 "phone": "978-283-2620 x3007"
             }
         ],
         "address": {
@@ -645,15 +645,15 @@
         },
         "name": "Gloucester District Court",
         "phone": "(978) 283-2620",
         "tyler_code": "389",
         "tyler_lower_court_code": "1784"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "robin.massa@jud.state.ma.us",
                 "name": "Robin Massa",
                 "phone": "413-774-7427"
             }
         ],
         "address": {
@@ -674,15 +674,15 @@
         },
         "name": "Greenfield District Court",
         "phone": "(413) 774-5533",
         "tyler_code": "465",
         "tyler_lower_court_code": "1785"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "katherine.lauranzano@jud.state.ma.us",
                 "name": "Katherine Lauranzano",
                 "phone": "(978) 521-7371"
             },
             {
                 "email": "jennifer.mailhot@jud.state.ma.us",
@@ -708,15 +708,15 @@
         },
         "name": "Haverhill District Court",
         "phone": "(978) 521-7300",
         "tyler_code": "395",
         "tyler_lower_court_code": "1786"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "caroline.field@jud.state.ma.us",
                 "name": "Caroline Field",
                 "phone": "781-749-7000 x201"
             }
         ],
         "address": {
@@ -737,15 +737,15 @@
         },
         "name": "Hingham District Court",
         "phone": "(781) 749-7000",
         "tyler_code": "478",
         "tyler_lower_court_code": "1787"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "azizah.yasin@jud.state.ma.us",
                 "name": "Azizah Yasin",
                 "phone": "(413) 493-0253"
             }
         ],
         "address": {
@@ -766,15 +766,15 @@
         },
         "name": "Holyoke District Court",
         "phone": "(413) 538-9710",
         "tyler_code": "458",
         "tyler_lower_court_code": "1788"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "cara.ring@jud.state.ma.us",
                 "name": "Cara Ring",
                 "phone": "(978) 499-6828"
             }
         ],
         "address": {
@@ -795,15 +795,15 @@
         },
         "name": "Ipswich District Court",
         "phone": "(978) 462-2652",
         "tyler_code": "384",
         "tyler_lower_court_code": "1789"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "nicole.ouelette@jud.state.ma.us",
                 "name": "Nicole Ouelette",
                 "phone": "(978) 687-7184 ext: 5022332"
             }
         ],
         "address": {
@@ -825,15 +825,15 @@
         },
         "name": "Lawrence District Court",
         "phone": "(978) 687-7184",
         "tyler_code": "397",
         "tyler_lower_court_code": "1790"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "sheila.carter@jud.state.ma.us",
                 "name": "Sheila Carter",
                 "phone": "(978) 537-3722  ext. 105"
             },
             {
                 "email": "julie.giusti@jud.state.ma.us",
@@ -859,15 +859,15 @@
         },
         "name": "Leominster District Court",
         "phone": "(978) 537-3722",
         "tyler_code": "424",
         "tyler_lower_court_code": "1791"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "meredith.mingolelli-cotter@jud.state.ma.us",
                 "name": "Meredith Mingolelli Cotter",
                 "phone": "978-442-3268"
             }
         ],
         "address": {
@@ -888,15 +888,15 @@
         },
         "name": "Lowell District Court",
         "phone": "(978) 459-4101",
         "tyler_code": "435",
         "tyler_lower_court_code": "1792"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "paul.hickey@jud.state.ma.us",
                 "name": "Paul Hickey"
             }
         ],
         "address": {
             "address": "580 Essex St.",
@@ -916,15 +916,15 @@
         },
         "name": "Lynn District Court",
         "phone": "(781) 598-5200",
         "tyler_code": "400",
         "tyler_lower_court_code": "1793"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "cynthia.russell@jud.state.ma.us",
                 "name": "Cynthia Russell",
                 "phone": "(781) 322-7500 x219-1408"
             },
             {
                 "email": "alyssa.stewart@jud.state.ma.us",
@@ -950,15 +950,15 @@
         },
         "name": "Malden District Court",
         "phone": "(781) 322-7500",
         "tyler_code": "491",
         "tyler_lower_court_code": "1794"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "james.fahey@jud.state.ma.us",
                 "name": "James Fahey",
                 "phone": "(508) 485-3700 x206"
             },
             {
                 "email": "andrew.souto@jud.state.ma.us",
@@ -984,15 +984,15 @@
         },
         "name": "Marlborough District Court",
         "phone": "(508) 485-3700",
         "tyler_code": "430",
         "tyler_lower_court_code": "1795"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "thomas.carrigan@jud.state.ma.us",
                 "name": "Thomas Carrigan",
                 "phone": "508-473-1260 x110"
             }
         ],
         "address": {
@@ -1013,15 +1013,15 @@
         },
         "name": "Milford District Court",
         "phone": "(508) 473-1260",
         "tyler_code": "431",
         "tyler_lower_court_code": "1796"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "susan.beamish@jud.state.ma.us",
                 "name": "Susan Beamish",
                 "phone": "508-228-2669"
             }
         ],
         "address": {
@@ -1042,15 +1042,15 @@
         },
         "name": "Nantucket District Court",
         "phone": "(508) 228-0460",
         "tyler_code": "487",
         "tyler_lower_court_code": "1797"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "patrick.walsh@jud.state.ma.us",
                 "name": "Patrick Walsh",
                 "phone": "(508) 999-9377"
             },
             {
                 "email": "john.disanto@jud.state.ma.us",
@@ -1076,15 +1076,15 @@
         },
         "name": "New Bedford District Court",
         "phone": "(508) 999-9700",
         "tyler_code": "473",
         "tyler_lower_court_code": "1799"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "cara.ring@jud.state.ma.us",
                 "name": "Cara Ring",
                 "phone": "(978) 499-6828"
             }
         ],
         "address": {
@@ -1105,15 +1105,15 @@
         },
         "name": "Newburyport District Court",
         "phone": "(978) 462-2652",
         "tyler_code": "387",
         "tyler_lower_court_code": "1800"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "kathleen.sheridan@jud.state.ma.us",
                 "name": "Kathleen Sheridan",
                 "phone": "617-243-7206"
             }
         ],
         "address": {
@@ -1134,15 +1134,15 @@
         },
         "name": "Newton District Court",
         "phone": "(617) 244-3600",
         "tyler_code": "493",
         "tyler_lower_court_code": "1801"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "linda.devine@jud.state.ma.us",
                 "name": "Linda Devine",
                 "phone": "413-584-7400 x247"
             }
         ],
         "address": {
@@ -1163,15 +1163,15 @@
         },
         "name": "Northampton District Court",
         "phone": "(413) 584-7400",
         "tyler_code": "462",
         "tyler_lower_court_code": "1802"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "timothy.morey@jud.state.ma.us",
                 "name": "Timothy Morey",
                 "phone": "413-663-5339"
             }
         ],
         "address": {
@@ -1214,15 +1214,15 @@
         },
         "name": "Orange District Court",
         "phone": "(978) 544-8277",
         "tyler_code": "474",
         "tyler_lower_court_code": "1804"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "marion.broidrick@jud.state.ma.us",
                 "name": "Marion Broiderick",
                 "phone": "508-255-4700 x148"
             }
         ],
         "address": {
@@ -1243,15 +1243,15 @@
         },
         "name": "Orleans District Court",
         "phone": "(508) 255-4700",
         "tyler_code": "494",
         "tyler_lower_court_code": "1805"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "yvonne.robinson@jud.state.ma.us",
                 "name": "Yvonne Robinson",
                 "phone": "413-283-8916"
             }
         ],
         "address": {
@@ -1273,15 +1273,15 @@
         },
         "name": "Palmer District Court",
         "phone": "(413) 283-8916",
         "tyler_code": "451",
         "tyler_lower_court_code": "1806"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "rosalind.faretra@jud.state.ma.us",
                 "name": "Rosalind Faretra",
                 "phone": "978-532-3100 x303"
             }
         ],
         "address": {
@@ -1302,15 +1302,15 @@
         },
         "name": "Peabody District Court",
         "phone": "(978) 532-3100",
         "tyler_code": "402",
         "tyler_lower_court_code": "1807"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "shannon.crouse@jud.state.ma.us",
                 "name": "Shannon Crouse",
                 "phone": "413-442-5468"
             }
         ],
         "address": {
@@ -1331,15 +1331,15 @@
         },
         "name": "Pittsfield District Court",
         "phone": "(413) 499-0558",
         "tyler_code": "476",
         "tyler_lower_court_code": "1808"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "angela.martin@jud.state.ma.us",
                 "name": "Angela Martin",
                 "phone": "508-747-8446"
             },
             {
                 "email": "noel.plourde@jud.state.ma.us",
@@ -1365,15 +1365,15 @@
         },
         "name": "Plymouth District Court",
         "phone": "(508) 747-8400",
         "tyler_code": "496",
         "tyler_lower_court_code": "1809"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "rosaria.guarino-galvin@jud.state.ma.us",
                 "name": "Rosanna Guarino",
                 "phone": "(617) 471-1650 x138"
             }
         ],
         "address": {
@@ -1394,15 +1394,15 @@
         },
         "name": "Quincy District Court",
         "phone": "(617) 471-1650",
         "tyler_code": "509",
         "tyler_lower_court_code": "1810"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "andrew.stahnke@jud.state.ma.us",
                 "name": "Andrew Stahnke",
                 "phone": "978-825-3091"
             }
         ],
         "address": {
@@ -1423,15 +1423,15 @@
         },
         "name": "Salem District Court",
         "phone": "(978) 744-1167",
         "tyler_code": "391",
         "tyler_lower_court_code": "1811"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "donna.langill@jud.state.ma.us",
                 "name": "Donna Langill",
                 "phone": "617-666-8000 x758"
             }
         ],
         "address": {
@@ -1452,15 +1452,15 @@
         },
         "name": "Somerville District Court",
         "phone": "(617) 666-8000",
         "tyler_code": "504",
         "tyler_lower_court_code": "1812"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "calandra.austin@jud.state.ma.us",
                 "name": "Calandra Austin",
                 "phone": "413-528-3520 x3"
             }
         ],
         "address": {
@@ -1481,15 +1481,15 @@
         },
         "name": "Southern Berkshire District Court",
         "phone": "(413) 528-3520",
         "tyler_code": "477",
         "tyler_lower_court_code": "1813"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "susanne.moultrie@jud.state.ma.us",
                 "name": "Susanne Moultrie",
                 "phone": "413-748-8643"
             }
         ],
         "address": {
@@ -1510,15 +1510,15 @@
         },
         "name": "Springfield District Court",
         "phone": "(413) 748-8600",
         "tyler_code": "670",
         "tyler_lower_court_code": "1814"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "linda.siegel@jud.state.ma.us",
                 "name": "Linda Siegel",
                 "phone": "781-344-2131 x217"
             }
         ],
         "address": {
@@ -1539,15 +1539,15 @@
         },
         "name": "Stoughton District Court",
         "phone": "(781) 344-2131",
         "tyler_code": "514",
         "tyler_lower_court_code": "1815"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "cheri.sigman@jud.state.ma.us",
                 "name": "Cheri Sigman",
                 "phone": "(508) 977-6159"
             },
             {
                 "email": "melissa.corr@jud.state.ma.us",
@@ -1573,15 +1573,15 @@
         },
         "name": "Taunton District Court",
         "phone": "(508) 977-6000",
         "tyler_code": "480",
         "tyler_lower_court_code": "1816"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "pamela.gervais@jud.state.ma.us",
                 "name": "Pamela Gervais",
                 "phone": "508-278-2454 x115"
             }
         ],
         "address": {
@@ -1602,15 +1602,15 @@
         },
         "name": "Uxbridge District Court",
         "phone": "(508) 278-2454",
         "tyler_code": "433",
         "tyler_lower_court_code": "1817"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "darlene.gambucci@jud.state.ma.us",
                 "name": "Darlene Gambucci",
                 "phone": "781-894-4500 x239"
             }
         ],
         "address": {
@@ -1631,15 +1631,15 @@
         },
         "name": "Waltham District Court",
         "phone": "(781) 894-4500",
         "tyler_code": "502",
         "tyler_lower_court_code": "1818"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "sincere.goodman@jud.state.ma.us",
                 "name": "Sincer\u00e9 Goodman",
                 "phone": "508-295-8300 x315"
             }
         ],
         "address": {
@@ -1660,15 +1660,15 @@
         },
         "name": "Wareham District Court",
         "phone": "(508) 295-8300",
         "tyler_code": "497",
         "tyler_lower_court_code": "1819"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "kimberly.cancelli@jud.state.ma.us",
                 "name": "Kimberly Cancelli",
                 "phone": "(508) 366-8266 ext. 310-2007"
             }
         ],
         "address": {
@@ -1689,15 +1689,15 @@
         },
         "name": "Westborough District Court",
         "phone": "(508) 366-8266",
         "tyler_code": "426",
         "tyler_lower_court_code": "1820"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "robbin.conde@jud.state.ma.us",
                 "name": "Robbin Conde",
                 "phone": "413-568-8946"
             }
         ],
         "address": {
@@ -1718,15 +1718,15 @@
         },
         "name": "Westfield District Court",
         "phone": "(413) 568-8946",
         "tyler_code": "460",
         "tyler_lower_court_code": "1821"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "kimberly.walsh@jud.state.ma.us",
                 "name": "Kimberly A Walsh",
                 "phone": "978-632-2373 x112"
             }
         ],
         "address": {
@@ -1747,15 +1747,15 @@
         },
         "name": "Winchendon District Court",
         "phone": "(978) 632-6326",
         "tyler_code": "437",
         "tyler_lower_court_code": "1822"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "deborah.earl@jud.state.ma.us",
                 "name": "Deborah Earl",
                 "phone": "781-935-4000 x236"
             },
             {
                 "email": "paula.viola@jud.state.ma.us",
@@ -1781,15 +1781,15 @@
         },
         "name": "Woburn District Court",
         "phone": "(781) 935-4000",
         "tyler_code": "588",
         "tyler_lower_court_code": "1823"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "darlene.perro@jud.state.ma.us",
                 "name": "Darlene Perro",
                 "phone": "(508) 831-2040"
             },
             {
                 "email": "k.panagiotou@jud.state.ma.us",
@@ -1815,15 +1815,15 @@
         },
         "name": "Worcester District Court",
         "phone": "(508) 831-2010",
         "tyler_code": "672",
         "tyler_lower_court_code": "1824"
     },
     {
-        "ADA Coordinators": [
+        "ada_coordinators": [
             {
                 "email": "diane.duffey@jud.state.ma.us",
                 "name": "Diane Duffey",
                 "phone": "508-384-3106 ext. 229"
             }
         ],
         "address": {
```

### Comparing `docassemble.MACourts-0.59.0/docassemble/MACourts/data/sources/housing_courts.json` & `docassemble.MACourts-0.59.1/docassemble/MACourts/data/sources/housing_courts.json`

 * *Files identical despite different names*

### Comparing `docassemble.MACourts-0.59.0/docassemble/MACourts/data/sources/juvenile_courts.json` & `docassemble.MACourts-0.59.1/docassemble/MACourts/data/sources/juvenile_courts.json`

 * *Files identical despite different names*

### Comparing `docassemble.MACourts-0.59.0/docassemble/MACourts/data/sources/land_court.json` & `docassemble.MACourts-0.59.1/docassemble/MACourts/data/sources/land_court.json`

 * *Files identical despite different names*

### Comparing `docassemble.MACourts-0.59.0/docassemble/MACourts/data/sources/probate_and_family_courts.json` & `docassemble.MACourts-0.59.1/docassemble/MACourts/data/sources/probate_and_family_courts.json`

 * *Files identical despite different names*

### Comparing `docassemble.MACourts-0.59.0/docassemble/MACourts/data/sources/superior_courts.json` & `docassemble.MACourts-0.59.1/docassemble/MACourts/data/sources/superior_courts.json`

 * *Files identical despite different names*

### Comparing `docassemble.MACourts-0.59.0/docassemble/MACourts/docket_tool.md` & `docassemble.MACourts-0.59.1/docassemble/MACourts/docket_tool.md`

 * *Files identical despite different names*

### Comparing `docassemble.MACourts-0.59.0/docassemble/MACourts/macourts.py` & `docassemble.MACourts-0.59.1/docassemble/MACourts/macourts.py`

 * *Files 0% similar despite different names*

```diff
@@ -778,15 +778,15 @@
         elif address_to_compare.city.lower() in ['attleboro', 'berkley', 'dighton', 'easton', 'mansfield', 'north attleborough', 'norton', 'raynham', 'rehoboth', 'seekonk','taunton']:
             local_housing_court = "Southeast Housing Court - Taunton Session"
         else:
             local_housing_court = ""
         
         # Try one time to match the normalized address instead of the 
         # literal provided address if first match fails
-        if depth == 0 and not local_housing_court:
+        if depth == 0 and not local_housing_court and hasattr(address, "norm_long"):
             return self.matching_housing_court_name(address.norm_long, depth=1)
         return local_housing_court
 
     def matching_bmc(self, address: Address) -> Optional[MACourt]:
         if address.city.lower() in ["winthrop"]:
             # This city is not in Boston but is served by East Boston BMC
             court_name = "East Boston Division, Boston Municipal Court"
```

### Comparing `docassemble.MACourts-0.59.0/docassemble/MACourts/test/test_court_finder.py` & `docassemble.MACourts-0.59.1/docassemble/MACourts/test/test_court_finder.py`

 * *Files identical despite different names*

### Comparing `docassemble.MACourts-0.59.0/docassemble/MACourts/test/test_docket_numbers.py` & `docassemble.MACourts-0.59.1/docassemble/MACourts/test/test_docket_numbers.py`

 * *Files identical despite different names*

### Comparing `docassemble.MACourts-0.59.0/docassemble/MACourts/test_local_court_json_files.yml` & `docassemble.MACourts-0.59.1/docassemble/MACourts/test_local_court_json_files.yml`

 * *Files identical despite different names*

### Comparing `docassemble.MACourts-0.59.0/docassemble.MACourts.egg-info/PKG-INFO` & `docassemble.MACourts-0.59.1/docassemble.MACourts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docassemble.MACourts
-Version: 0.59.0
+Version: 0.59.1
 Summary: List Massachusetts Courts in Docassemble
 Home-page: https://docassemble.org
 Author: Quinten Steenhuis
 Author-email: qsteenhuis@gbls.org
 License: The MIT License (MIT)
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `docassemble.MACourts-0.59.0/docassemble.MACourts.egg-info/SOURCES.txt` & `docassemble.MACourts-0.59.1/docassemble.MACourts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docassemble.MACourts-0.59.0/setup.py` & `docassemble.MACourts-0.59.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                         break
                 if bad_name:
                     continue
                 out.setdefault(package, []).append(prefix+name)
     return out
 
 setup(name='docassemble.MACourts',
-      version='0.59.0',
+      version='0.59.1',
       description=('List Massachusetts Courts in Docassemble'),
       long_description='A utility package that includes JSON files representing all of the courts in Massachusetts.\r\n\r\nCourts automatically scraped from Mass.gov and geocoded with Google Maps.\r\n\r\nIf the court has a PO box, the PO box will be available in court.address.orig_address',
       long_description_content_type='text/markdown',
       author='Quinten Steenhuis',
       author_email='qsteenhuis@gbls.org',
       license='The MIT License (MIT)',
       url='https://docassemble.org',
```

