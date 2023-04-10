# Comparing `tmp/antelope_core-0.2.0.tar.gz` & `tmp/antelope_core-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antelope_core-0.2.0.tar", last modified: Fri Apr  7 05:30:44 2023, max compression
+gzip compressed data, was "antelope_core-0.2.1.tar", last modified: Mon Apr 10 21:44:38 2023, max compression
```

## Comparing `antelope_core-0.2.0.tar` & `antelope_core-0.2.1.tar`

### file list

```diff
@@ -1,185 +1,183 @@
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.113020 antelope_core-0.2.0/
--rw-r--r--   0 b          (500) b          (506)     1520 2020-09-25 22:29:55.000000 antelope_core-0.2.0/LICENSE
--rw-r--r--   0 b          (500) b          (506)      335 2021-10-30 03:39:36.000000 antelope_core-0.2.0/MANIFEST.in
--rw-r--r--   0 b          (500) b          (506)    14232 2023-04-07 05:30:44.113020 antelope_core-0.2.0/PKG-INFO
--rw-r--r--   0 b          (500) b          (506)    13586 2022-04-09 17:53:42.000000 antelope_core-0.2.0/README.md
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.106353 antelope_core-0.2.0/antelope_core/
--rw-r--r--   0 b          (500) b          (506)     3177 2022-09-10 06:13:58.000000 antelope_core-0.2.0/antelope_core/__init__.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.106353 antelope_core-0.2.0/antelope_core/archives/
--rw-r--r--   0 b          (500) b          (506)     4518 2022-12-31 00:11:14.000000 antelope_core-0.2.0/antelope_core/archives/__init__.py
--rw-r--r--   0 b          (500) b          (506)     2364 2021-09-21 18:51:48.000000 antelope_core-0.2.0/antelope_core/archives/archive_index.py
--rw-r--r--   0 b          (500) b          (506)    19334 2022-12-31 00:11:14.000000 antelope_core-0.2.0/antelope_core/archives/basic_archive.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.106353 antelope_core-0.2.0/antelope_core/archives/data/
--rw-r--r--   0 b          (500) b          (506)    27863 2023-02-01 20:12:07.000000 antelope_core-0.2.0/antelope_core/archives/data/elcd_reference_quantities.json
--rw-r--r--   0 b          (500) b          (506)    28771 2023-02-05 06:57:15.000000 antelope_core-0.2.0/antelope_core/archives/entity_store.py
--rw-r--r--   0 b          (500) b          (506)     6288 2022-04-09 17:53:42.000000 antelope_core-0.2.0/antelope_core/archives/lc_archive.py
--rw-r--r--   0 b          (500) b          (506)     5741 2022-12-31 00:11:14.000000 antelope_core-0.2.0/antelope_core/archives/quantity_manager.py
--rw-r--r--   0 b          (500) b          (506)    42836 2023-04-05 08:32:36.000000 antelope_core-0.2.0/antelope_core/archives/term_manager.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.106353 antelope_core-0.2.0/antelope_core/archives/tests/
--rw-r--r--   0 b          (500) b          (506)       54 2019-02-15 00:01:58.000000 antelope_core-0.2.0/antelope_core/archives/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     8577 2020-03-30 08:22:53.000000 antelope_core-0.2.0/antelope_core/archives/tests/test_base.py
--rw-r--r--   0 b          (500) b          (506)     3557 2021-09-21 18:51:48.000000 antelope_core-0.2.0/antelope_core/archives/tests/test_basic_archive.py
--rw-r--r--   0 b          (500) b          (506)     1802 2022-04-09 17:53:42.000000 antelope_core-0.2.0/antelope_core/archives/tests/test_entity_store.py
--rw-r--r--   0 b          (500) b          (506)     4143 2019-04-05 22:10:51.000000 antelope_core-0.2.0/antelope_core/archives/tests/test_json.json
--rw-r--r--   0 b          (500) b          (506)     2287 2021-10-30 03:39:36.000000 antelope_core-0.2.0/antelope_core/archives/tests/test_qdb.py
--rw-r--r--   0 b          (500) b          (506)     3044 2022-04-09 17:53:42.000000 antelope_core-0.2.0/antelope_core/archives/tests/test_quantity_manager.py
--rw-r--r--   0 b          (500) b          (506)     2286 2023-01-12 08:08:59.000000 antelope_core-0.2.0/antelope_core/archives/tests/test_quantity_relation.py
--rw-r--r--   0 b          (500) b          (506)     3013 2023-01-30 19:03:06.000000 antelope_core-0.2.0/antelope_core/archives/tests/test_term_manager.py
--rw-r--r--   0 b          (500) b          (506)     4545 2023-03-30 22:16:32.000000 antelope_core-0.2.0/antelope_core/auth.py
--rw-r--r--   0 b          (500) b          (506)     2170 2020-04-03 08:54:47.000000 antelope_core-0.2.0/antelope_core/autorange.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.106353 antelope_core-0.2.0/antelope_core/catalog/
--rw-r--r--   0 b          (500) b          (506)       70 2021-09-21 18:51:48.000000 antelope_core-0.2.0/antelope_core/catalog/__init__.py
--rw-r--r--   0 b          (500) b          (506)    18441 2023-01-29 07:23:50.000000 antelope_core-0.2.0/antelope_core/catalog/catalog.py
--rw-r--r--   0 b          (500) b          (506)      628 2020-11-05 08:47:12.000000 antelope_core-0.2.0/antelope_core/catalog/catalog_root.py
--rw-r--r--   0 b          (500) b          (506)     6104 2022-04-09 17:53:42.000000 antelope_core-0.2.0/antelope_core/catalog/configurator.py
--rw-r--r--   0 b          (500) b          (506)    18476 2023-02-02 08:06:37.000000 antelope_core-0.2.0/antelope_core/catalog/lc_catalog.py
--rw-r--r--   0 b          (500) b          (506)     8782 2023-01-12 00:22:51.000000 antelope_core-0.2.0/antelope_core/catalog/lc_resolver.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.106353 antelope_core-0.2.0/antelope_core/catalog/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2018-07-26 08:24:01.000000 antelope_core-0.2.0/antelope_core/catalog/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     5139 2022-12-31 00:11:14.000000 antelope_core-0.2.0/antelope_core/catalog/tests/test_catalogs.py
--rw-r--r--   0 b          (500) b          (506)     2316 2022-12-31 00:11:14.000000 antelope_core-0.2.0/antelope_core/catalog/tests/test_process_ref.py
--rw-r--r--   0 b          (500) b          (506)     1624 2022-04-09 17:53:42.000000 antelope_core-0.2.0/antelope_core/catalog/tests/test_quantity_refs.py
--rw-r--r--   0 b          (500) b          (506)    12623 2023-02-03 00:08:39.000000 antelope_core-0.2.0/antelope_core/catalog_query.py
--rw-r--r--   0 b          (500) b          (506)    10710 2022-04-09 17:53:42.000000 antelope_core-0.2.0/antelope_core/characterizations.py
--rw-r--r--   0 b          (500) b          (506)    15445 2022-04-09 17:53:42.000000 antelope_core-0.2.0/antelope_core/contexts.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.106353 antelope_core-0.2.0/antelope_core/data_sources/
--rw-r--r--   0 b          (500) b          (506)        0 2018-10-26 21:44:35.000000 antelope_core-0.2.0/antelope_core/data_sources/__init__.py
--rw-r--r--   0 b          (500) b          (506)     3851 2022-04-09 17:53:42.000000 antelope_core-0.2.0/antelope_core/data_sources/data_source.py
--rw-r--r--   0 b          (500) b          (506)     7497 2022-08-22 21:21:17.000000 antelope_core-0.2.0/antelope_core/data_sources/ecoinvent.py
--rw-r--r--   0 b          (500) b          (506)     1741 2022-08-22 21:21:17.000000 antelope_core-0.2.0/antelope_core/data_sources/ecoinvent_lcia.py
--rw-r--r--   0 b          (500) b          (506)     1303 2022-08-22 21:21:17.000000 antelope_core-0.2.0/antelope_core/data_sources/gwp_ipcc_2007.py
--rw-r--r--   0 b          (500) b          (506)     4614 2020-11-05 09:30:15.000000 antelope_core-0.2.0/antelope_core/data_sources/local.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.109687 antelope_core-0.2.0/antelope_core/data_sources/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2018-10-26 21:44:35.000000 antelope_core-0.2.0/antelope_core/data_sources/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     4152 2022-04-09 17:53:42.000000 antelope_core-0.2.0/antelope_core/data_sources/tests/test_aa_local.py
--rw-r--r--   0 b          (500) b          (506)     1541 2022-04-09 17:53:42.000000 antelope_core-0.2.0/antelope_core/data_sources/tests/test_ecoinvent.py
--rw-r--r--   0 b          (500) b          (506)     7319 2021-07-08 16:41:41.000000 antelope_core-0.2.0/antelope_core/data_sources/tests/test_ecoinvent_lci.py
--rw-r--r--   0 b          (500) b          (506)      815 2022-04-09 17:53:42.000000 antelope_core-0.2.0/antelope_core/data_sources/tests/test_ipcc2007.py
--rw-r--r--   0 b          (500) b          (506)     7263 2023-04-05 08:53:20.000000 antelope_core-0.2.0/antelope_core/data_sources/tests/test_uslci.py
--rw-r--r--   0 b          (500) b          (506)     2438 2022-08-22 21:21:17.000000 antelope_core-0.2.0/antelope_core/data_sources/traci.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.109687 antelope_core-0.2.0/antelope_core/data_sources/uslci/
--rw-r--r--   0 b          (500) b          (506)       31 2020-12-29 09:58:58.000000 antelope_core-0.2.0/antelope_core/data_sources/uslci/__init__.py
--rw-r--r--   0 b          (500) b          (506)     6168 2022-08-22 21:21:17.000000 antelope_core-0.2.0/antelope_core/data_sources/uslci/uslci.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.109687 antelope_core-0.2.0/antelope_core/entities/
--rw-r--r--   0 b          (500) b          (506)      181 2022-04-09 17:53:42.000000 antelope_core-0.2.0/antelope_core/entities/__init__.py
--rw-r--r--   0 b          (500) b          (506)    11169 2022-04-09 17:53:42.000000 antelope_core-0.2.0/antelope_core/entities/entities.py
--rw-r--r--   0 b          (500) b          (506)     4408 2023-03-29 00:53:52.000000 antelope_core-0.2.0/antelope_core/entities/flows.py
--rw-r--r--   0 b          (500) b          (506)    24934 2023-02-24 05:55:04.000000 antelope_core-0.2.0/antelope_core/entities/processes.py
--rw-r--r--   0 b          (500) b          (506)     7804 2023-02-06 19:33:10.000000 antelope_core-0.2.0/antelope_core/entities/quantities.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.109687 antelope_core-0.2.0/antelope_core/entities/tests/
--rw-r--r--   0 b          (500) b          (506)       62 2019-02-15 00:01:58.000000 antelope_core-0.2.0/antelope_core/entities/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     1065 2021-01-07 23:11:04.000000 antelope_core-0.2.0/antelope_core/entities/tests/base_testclass.py
--rw-r--r--   0 b          (500) b          (506)    99142 2019-03-19 20:06:35.000000 antelope_core-0.2.0/antelope_core/entities/tests/test_archive.json
--rw-r--r--   0 b          (500) b          (506)     1019 2020-03-30 08:22:53.000000 antelope_core-0.2.0/antelope_core/entities/tests/test_entities.py
--rw-r--r--   0 b          (500) b          (506)      850 2020-12-29 09:58:58.000000 antelope_core-0.2.0/antelope_core/entities/tests/test_entity_refs.py
--rw-r--r--   0 b          (500) b          (506)      291 2020-03-30 08:22:53.000000 antelope_core-0.2.0/antelope_core/entities/tests/test_flows.py
--rw-r--r--   0 b          (500) b          (506)     1538 2020-03-30 08:22:53.000000 antelope_core-0.2.0/antelope_core/entities/tests/test_processes.py
--rw-r--r--   0 b          (500) b          (506)     1565 2020-09-29 22:38:38.000000 antelope_core-0.2.0/antelope_core/entities/tests/test_quantities.py
--rw-r--r--   0 b          (500) b          (506)    18234 2022-06-13 20:26:37.000000 antelope_core-0.2.0/antelope_core/entities/xlsx_editor.py
--rw-r--r--   0 b          (500) b          (506)    22640 2022-04-09 17:53:42.000000 antelope_core-0.2.0/antelope_core/exchanges.py
--rw-r--r--   0 b          (500) b          (506)     6756 2023-01-11 07:42:19.000000 antelope_core-0.2.0/antelope_core/file_accessor.py
--rw-r--r--   0 b          (500) b          (506)     1137 2021-09-21 18:51:48.000000 antelope_core-0.2.0/antelope_core/from_json.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.109687 antelope_core-0.2.0/antelope_core/implementations/
--rw-r--r--   0 b          (500) b          (506)      333 2021-09-21 18:51:48.000000 antelope_core-0.2.0/antelope_core/implementations/__init__.py
--rw-r--r--   0 b          (500) b          (506)     7347 2023-04-05 07:40:09.000000 antelope_core-0.2.0/antelope_core/implementations/background.py
--rw-r--r--   0 b          (500) b          (506)     5772 2023-03-30 22:45:32.000000 antelope_core-0.2.0/antelope_core/implementations/basic.py
--rw-r--r--   0 b          (500) b          (506)     9856 2022-04-09 17:53:42.000000 antelope_core-0.2.0/antelope_core/implementations/configure.py
--rw-r--r--   0 b          (500) b          (506)     2812 2022-04-09 17:53:42.000000 antelope_core-0.2.0/antelope_core/implementations/exchange.py
--rw-r--r--   0 b          (500) b          (506)     6064 2022-04-09 17:53:42.000000 antelope_core-0.2.0/antelope_core/implementations/index.py
--rw-r--r--   0 b          (500) b          (506)    32779 2023-03-29 00:46:54.000000 antelope_core-0.2.0/antelope_core/implementations/quantity.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.109687 antelope_core-0.2.0/antelope_core/implementations/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2018-09-13 20:45:30.000000 antelope_core-0.2.0/antelope_core/implementations/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     2056 2022-04-09 17:53:42.000000 antelope_core-0.2.0/antelope_core/implementations/tests/test_quantity.py
--rw-r--r--   0 b          (500) b          (506)    16474 2022-12-31 00:11:14.000000 antelope_core-0.2.0/antelope_core/lc_resource.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.109687 antelope_core-0.2.0/antelope_core/lcia_engine/
--rw-r--r--   0 b          (500) b          (506)     5632 2023-02-02 21:42:48.000000 antelope_core-0.2.0/antelope_core/lcia_engine/__init__.py
--rw-r--r--   0 b          (500) b          (506)     8163 2022-04-09 17:53:42.000000 antelope_core-0.2.0/antelope_core/lcia_engine/clookup.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.109687 antelope_core-0.2.0/antelope_core/lcia_engine/data/
--rw-r--r--   0 b          (500) b          (506)     8420 2022-08-27 07:18:09.000000 antelope_core-0.2.0/antelope_core/lcia_engine/data/contexts.json
--rw-r--r--   0 b          (500) b          (506)   383481 2020-03-30 08:22:53.000000 antelope_core-0.2.0/antelope_core/lcia_engine/data/flowables.json
--rw-r--r--   0 b          (500) b          (506)    30980 2021-01-07 00:24:41.000000 antelope_core-0.2.0/antelope_core/lcia_engine/data/ipcc_2007_gwp.json
--rw-r--r--   0 b          (500) b          (506)    18298 2023-04-05 08:32:36.000000 antelope_core-0.2.0/antelope_core/lcia_engine/lcia_engine.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.109687 antelope_core-0.2.0/antelope_core/lcia_engine/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2020-03-30 08:22:53.000000 antelope_core-0.2.0/antelope_core/lcia_engine/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     1513 2023-03-29 01:25:13.000000 antelope_core-0.2.0/antelope_core/lcia_engine/tests/test_biogenic_co2.py
--rw-r--r--   0 b          (500) b          (506)     2559 2020-03-30 08:22:53.000000 antelope_core-0.2.0/antelope_core/lcia_engine/tests/test_clookup.py
--rw-r--r--   0 b          (500) b          (506)      924 2020-09-29 22:38:38.000000 antelope_core-0.2.0/antelope_core/lcia_engine/tests/test_ipcc.py
--rw-r--r--   0 b          (500) b          (506)     2981 2021-10-30 03:39:36.000000 antelope_core-0.2.0/antelope_core/lcia_engine/tests/test_lcia_engine.py
--rw-r--r--   0 b          (500) b          (506)    41768 2023-04-04 03:19:24.000000 antelope_core-0.2.0/antelope_core/lcia_results.py
--rw-r--r--   0 b          (500) b          (506)    16203 2023-04-05 07:40:09.000000 antelope_core-0.2.0/antelope_core/models.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.109687 antelope_core-0.2.0/antelope_core/providers/
--rw-r--r--   0 b          (500) b          (506)     4617 2022-11-07 09:16:47.000000 antelope_core-0.2.0/antelope_core/providers/__init__.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.109687 antelope_core-0.2.0/antelope_core/providers/data/
--rw-r--r--   0 b          (500) b          (506)       57 2019-02-15 00:01:58.000000 antelope_core-0.2.0/antelope_core/providers/data/__init__.py
--rw-r--r--   0 b          (500) b          (506)    39336 2018-07-26 08:24:01.000000 antelope_core-0.2.0/antelope_core/providers/data/list_of_methods_and_indicators_ecoinvent_v3.2.xlsx
--rw-r--r--   0 b          (500) b          (506)    95429 2019-02-15 00:01:58.000000 antelope_core-0.2.0/antelope_core/providers/data/traci_2_1_2014_dec_10_0_test.xlsx
--rw-r--r--   0 b          (500) b          (506)     9551 2022-08-01 22:59:24.000000 antelope_core-0.2.0/antelope_core/providers/ecoinvent_lcia.py
--rw-r--r--   0 b          (500) b          (506)    11083 2022-04-09 17:53:42.000000 antelope_core-0.2.0/antelope_core/providers/ecospold.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.113020 antelope_core-0.2.0/antelope_core/providers/ecospold2/
--rw-r--r--   0 b          (500) b          (506)       41 2018-07-26 08:24:01.000000 antelope_core-0.2.0/antelope_core/providers/ecospold2/__init__.py
--rw-r--r--   0 b          (500) b          (506)    24560 2022-08-23 23:02:58.000000 antelope_core-0.2.0/antelope_core/providers/ecospold2/ecospold2.py
--rw-r--r--   0 b          (500) b          (506)      564 2020-10-18 05:43:46.000000 antelope_core-0.2.0/antelope_core/providers/ecospold2/ecospold2_index.py
--rw-r--r--   0 b          (500) b          (506)     2134 2020-03-30 08:22:53.000000 antelope_core-0.2.0/antelope_core/providers/ecospold2/master_data.py
--rw-r--r--   0 b          (500) b          (506)    10917 2023-02-02 16:59:51.000000 antelope_core-0.2.0/antelope_core/providers/file_store.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.113020 antelope_core-0.2.0/antelope_core/providers/ilcd/
--rw-r--r--   0 b          (500) b          (506)       78 2018-07-26 08:24:01.000000 antelope_core-0.2.0/antelope_core/providers/ilcd/__init__.py
--rw-r--r--   0 b          (500) b          (506)    17683 2022-04-09 17:53:42.000000 antelope_core-0.2.0/antelope_core/providers/ilcd/ilcd.py
--rw-r--r--   0 b          (500) b          (506)     2314 2018-07-26 08:24:01.000000 antelope_core-0.2.0/antelope_core/providers/ilcd/ilcd_flowables.py
--rw-r--r--   0 b          (500) b          (506)     5806 2022-04-09 17:53:42.000000 antelope_core-0.2.0/antelope_core/providers/ilcd/ilcd_lcia.py
--rw-r--r--   0 b          (500) b          (506)      314 2020-09-29 23:36:41.000000 antelope_core-0.2.0/antelope_core/providers/ilcd/index.py
--rw-r--r--   0 b          (500) b          (506)     3177 2021-09-21 18:51:48.000000 antelope_core-0.2.0/antelope_core/providers/ilcd/quantity.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.113020 antelope_core-0.2.0/antelope_core/providers/ilcd/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2021-01-07 00:24:41.000000 antelope_core-0.2.0/antelope_core/providers/ilcd/tests/__init__.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.106353 antelope_core-0.2.0/antelope_core/providers/ilcd/tests/data/
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.106353 antelope_core-0.2.0/antelope_core/providers/ilcd/tests/data/ilcd_test/
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.106353 antelope_core-0.2.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.113020 antelope_core-0.2.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/
--rw-r--r--   0 b          (500) b          (506)     2712 2019-02-15 00:01:58.000000 antelope_core-0.2.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-11da-a746-0800200b9a66.xml
--rw-r--r--   0 b          (500) b          (506)     2738 2019-02-15 00:01:58.000000 antelope_core-0.2.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-11da-a746-0800200c9a66.xml
--rw-r--r--   0 b          (500) b          (506)     2734 2019-02-15 00:01:58.000000 antelope_core-0.2.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-13da-a746-0800200c9a66.xml
--rw-r--r--   0 b          (500) b          (506)     2716 2019-02-15 00:01:58.000000 antelope_core-0.2.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-22da-a746-0800200c9a66.xml
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.113020 antelope_core-0.2.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flows/
--rw-r--r--   0 b          (500) b          (506)     5078 2019-02-15 00:01:58.000000 antelope_core-0.2.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flows/f579de8c-8897-4bdb-9a0a-b36f8b13282e.xml
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.113020 antelope_core-0.2.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/
--rw-r--r--   0 b          (500) b          (506)     2503 2019-02-15 00:01:58.000000 antelope_core-0.2.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/1ff9a08c-6fc1-4509-8bcd-a5404c598755.xml
--rw-r--r--   0 b          (500) b          (506)     3551 2019-02-15 00:01:58.000000 antelope_core-0.2.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/ad38d542-3fe9-439d-9b95-2f5f7752acaf.xml
--rw-r--r--   0 b          (500) b          (506)     3344 2019-02-15 00:01:58.000000 antelope_core-0.2.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/cd950537-0a98-4044-9ba7-9f9a68d0a504.xml
--rw-r--r--   0 b          (500) b          (506)     4443 2019-02-15 00:01:58.000000 antelope_core-0.2.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/de5104d8-3de0-4218-a29d-b7123ce9ca3c.xml
--rw-r--r--   0 b          (500) b          (506)      932 2021-01-07 00:24:41.000000 antelope_core-0.2.0/antelope_core/providers/ilcd/tests/test_ilcd.py
--rw-r--r--   0 b          (500) b          (506)    21764 2023-02-24 05:50:36.000000 antelope_core-0.2.0/antelope_core/providers/openlca_jsonld.py
--rw-r--r--   0 b          (500) b          (506)      729 2021-10-30 03:39:36.000000 antelope_core-0.2.0/antelope_core/providers/parse_math.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.113020 antelope_core-0.2.0/antelope_core/providers/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2018-07-26 08:24:01.000000 antelope_core-0.2.0/antelope_core/providers/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)      569 2020-09-29 23:35:54.000000 antelope_core-0.2.0/antelope_core/providers/tests/test_ecospold.py
--rw-r--r--   0 b          (500) b          (506)     4110 2018-07-26 08:24:01.000000 antelope_core-0.2.0/antelope_core/providers/tests/test_xml_widgets.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.113020 antelope_core-0.2.0/antelope_core/providers/traci/
--rw-r--r--   0 b          (500) b          (506)       50 2018-07-26 08:24:01.000000 antelope_core-0.2.0/antelope_core/providers/traci/__init__.py
--rw-r--r--   0 b          (500) b          (506)      653 2020-09-29 23:35:54.000000 antelope_core-0.2.0/antelope_core/providers/traci/index.py
--rw-r--r--   0 b          (500) b          (506)     3441 2019-01-17 18:55:10.000000 antelope_core-0.2.0/antelope_core/providers/traci/q_info.py
--rw-r--r--   0 b          (500) b          (506)     2076 2020-09-29 23:35:54.000000 antelope_core-0.2.0/antelope_core/providers/traci/quantity.py
--rw-r--r--   0 b          (500) b          (506)     1648 2020-03-30 08:22:53.000000 antelope_core-0.2.0/antelope_core/providers/traci/test_traci.py
--rw-r--r--   0 b          (500) b          (506)     6687 2022-04-09 17:53:42.000000 antelope_core-0.2.0/antelope_core/providers/traci/traci_2_1_spreadsheet.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.113020 antelope_core-0.2.0/antelope_core/providers/xdb_client/
--rw-r--r--   0 b          (500) b          (506)       33 2022-11-14 22:48:38.000000 antelope_core-0.2.0/antelope_core/providers/xdb_client/__init__.py
--rw-r--r--   0 b          (500) b          (506)    13740 2023-04-06 23:18:11.000000 antelope_core-0.2.0/antelope_core/providers/xdb_client/implementation.py
--rw-r--r--   0 b          (500) b          (506)     3693 2023-04-06 23:16:32.000000 antelope_core-0.2.0/antelope_core/providers/xdb_client/requester.py
--rw-r--r--   0 b          (500) b          (506)     5391 2023-02-01 00:30:59.000000 antelope_core-0.2.0/antelope_core/providers/xdb_client/rest_client.py
--rw-r--r--   0 b          (500) b          (506)     5787 2022-12-31 00:11:14.000000 antelope_core-0.2.0/antelope_core/providers/xdb_client/xdb_client.py
--rw-r--r--   0 b          (500) b          (506)     2917 2022-12-31 00:11:14.000000 antelope_core-0.2.0/antelope_core/providers/xdb_client/xdb_entities.py
--rw-r--r--   0 b          (500) b          (506)     2316 2022-08-01 23:00:27.000000 antelope_core-0.2.0/antelope_core/providers/xl_dict.py
--rw-r--r--   0 b          (500) b          (506)     1676 2020-03-30 08:22:53.000000 antelope_core-0.2.0/antelope_core/providers/xml_widgets.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.113020 antelope_core-0.2.0/antelope_core/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2018-07-26 08:24:01.000000 antelope_core-0.2.0/antelope_core/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)      972 2020-09-29 22:38:38.000000 antelope_core-0.2.0/antelope_core/tests/test_autorange.py
--rw-r--r--   0 b          (500) b          (506)    12509 2022-04-09 17:53:42.000000 antelope_core-0.2.0/antelope_core/tests/test_contexts.py
--rw-r--r--   0 b          (500) b          (506)     5637 2020-12-29 09:58:58.000000 antelope_core-0.2.0/antelope_core/tests/test_exchanges.py
--rw-r--r--   0 b          (500) b          (506)      500 2020-12-29 09:58:58.000000 antelope_core-0.2.0/antelope_core/tests/test_lcia_results.py
--rw-r--r--   0 b          (500) b          (506)     1162 2020-09-30 00:02:12.000000 antelope_core-0.2.0/antelope_core/tests/test_resources.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:44.106353 antelope_core-0.2.0/antelope_core.egg-info/
--rw-r--r--   0 b          (500) b          (506)    14232 2023-04-07 05:30:44.000000 antelope_core-0.2.0/antelope_core.egg-info/PKG-INFO
--rw-r--r--   0 b          (500) b          (506)     6778 2023-04-07 05:30:44.000000 antelope_core-0.2.0/antelope_core.egg-info/SOURCES.txt
--rw-r--r--   0 b          (500) b          (506)        1 2023-04-07 05:30:44.000000 antelope_core-0.2.0/antelope_core.egg-info/dependency_links.txt
--rw-r--r--   0 b          (500) b          (506)      169 2023-04-07 05:30:44.000000 antelope_core-0.2.0/antelope_core.egg-info/requires.txt
--rw-r--r--   0 b          (500) b          (506)       14 2023-04-07 05:30:44.000000 antelope_core-0.2.0/antelope_core.egg-info/top_level.txt
--rw-r--r--   0 b          (500) b          (506)       38 2023-04-07 05:30:44.113020 antelope_core-0.2.0/setup.cfg
--rw-r--r--   0 b          (500) b          (506)     3362 2023-04-07 05:28:35.000000 antelope_core-0.2.0/setup.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.534934 antelope_core-0.2.1/
+-rw-r--r--   0 b          (500) b          (506)     1520 2020-09-25 22:29:55.000000 antelope_core-0.2.1/LICENSE
+-rw-r--r--   0 b          (500) b          (506)      335 2021-10-30 03:39:36.000000 antelope_core-0.2.1/MANIFEST.in
+-rw-r--r--   0 b          (500) b          (506)    14232 2023-04-10 21:44:38.534934 antelope_core-0.2.1/PKG-INFO
+-rw-r--r--   0 b          (500) b          (506)    13586 2022-04-09 17:53:42.000000 antelope_core-0.2.1/README.md
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.518267 antelope_core-0.2.1/antelope_core/
+-rw-r--r--   0 b          (500) b          (506)     3177 2022-09-10 06:13:58.000000 antelope_core-0.2.1/antelope_core/__init__.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.521600 antelope_core-0.2.1/antelope_core/archives/
+-rw-r--r--   0 b          (500) b          (506)     4518 2022-12-31 00:11:14.000000 antelope_core-0.2.1/antelope_core/archives/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     2364 2021-09-21 18:51:48.000000 antelope_core-0.2.1/antelope_core/archives/archive_index.py
+-rw-r--r--   0 b          (500) b          (506)    19334 2022-12-31 00:11:14.000000 antelope_core-0.2.1/antelope_core/archives/basic_archive.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.521600 antelope_core-0.2.1/antelope_core/archives/data/
+-rw-r--r--   0 b          (500) b          (506)    27863 2023-02-01 20:12:07.000000 antelope_core-0.2.1/antelope_core/archives/data/elcd_reference_quantities.json
+-rw-r--r--   0 b          (500) b          (506)    28771 2023-02-05 06:57:15.000000 antelope_core-0.2.1/antelope_core/archives/entity_store.py
+-rw-r--r--   0 b          (500) b          (506)     6288 2022-04-09 17:53:42.000000 antelope_core-0.2.1/antelope_core/archives/lc_archive.py
+-rw-r--r--   0 b          (500) b          (506)     5741 2022-12-31 00:11:14.000000 antelope_core-0.2.1/antelope_core/archives/quantity_manager.py
+-rw-r--r--   0 b          (500) b          (506)    42836 2023-04-07 07:09:29.000000 antelope_core-0.2.1/antelope_core/archives/term_manager.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.521600 antelope_core-0.2.1/antelope_core/archives/tests/
+-rw-r--r--   0 b          (500) b          (506)       54 2019-02-15 00:01:58.000000 antelope_core-0.2.1/antelope_core/archives/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     8577 2020-03-30 08:22:53.000000 antelope_core-0.2.1/antelope_core/archives/tests/test_base.py
+-rw-r--r--   0 b          (500) b          (506)     3557 2021-09-21 18:51:48.000000 antelope_core-0.2.1/antelope_core/archives/tests/test_basic_archive.py
+-rw-r--r--   0 b          (500) b          (506)     1802 2022-04-09 17:53:42.000000 antelope_core-0.2.1/antelope_core/archives/tests/test_entity_store.py
+-rw-r--r--   0 b          (500) b          (506)     4143 2019-04-05 22:10:51.000000 antelope_core-0.2.1/antelope_core/archives/tests/test_json.json
+-rw-r--r--   0 b          (500) b          (506)     2287 2021-10-30 03:39:36.000000 antelope_core-0.2.1/antelope_core/archives/tests/test_qdb.py
+-rw-r--r--   0 b          (500) b          (506)     3044 2022-04-09 17:53:42.000000 antelope_core-0.2.1/antelope_core/archives/tests/test_quantity_manager.py
+-rw-r--r--   0 b          (500) b          (506)     2286 2023-01-12 08:08:59.000000 antelope_core-0.2.1/antelope_core/archives/tests/test_quantity_relation.py
+-rw-r--r--   0 b          (500) b          (506)     3013 2023-01-30 19:03:06.000000 antelope_core-0.2.1/antelope_core/archives/tests/test_term_manager.py
+-rw-r--r--   0 b          (500) b          (506)     2170 2020-04-03 08:54:47.000000 antelope_core-0.2.1/antelope_core/autorange.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.521600 antelope_core-0.2.1/antelope_core/catalog/
+-rw-r--r--   0 b          (500) b          (506)       70 2021-09-21 18:51:48.000000 antelope_core-0.2.1/antelope_core/catalog/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    18441 2023-01-29 07:23:50.000000 antelope_core-0.2.1/antelope_core/catalog/catalog.py
+-rw-r--r--   0 b          (500) b          (506)      628 2020-11-05 08:47:12.000000 antelope_core-0.2.1/antelope_core/catalog/catalog_root.py
+-rw-r--r--   0 b          (500) b          (506)     6104 2022-04-09 17:53:42.000000 antelope_core-0.2.1/antelope_core/catalog/configurator.py
+-rw-r--r--   0 b          (500) b          (506)    18804 2023-04-10 21:01:45.000000 antelope_core-0.2.1/antelope_core/catalog/lc_catalog.py
+-rw-r--r--   0 b          (500) b          (506)     8782 2023-01-12 00:22:51.000000 antelope_core-0.2.1/antelope_core/catalog/lc_resolver.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.521600 antelope_core-0.2.1/antelope_core/catalog/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2018-07-26 08:24:01.000000 antelope_core-0.2.1/antelope_core/catalog/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     5139 2022-12-31 00:11:14.000000 antelope_core-0.2.1/antelope_core/catalog/tests/test_catalogs.py
+-rw-r--r--   0 b          (500) b          (506)     2316 2022-12-31 00:11:14.000000 antelope_core-0.2.1/antelope_core/catalog/tests/test_process_ref.py
+-rw-r--r--   0 b          (500) b          (506)     1624 2022-04-09 17:53:42.000000 antelope_core-0.2.1/antelope_core/catalog/tests/test_quantity_refs.py
+-rw-r--r--   0 b          (500) b          (506)    12623 2023-04-08 00:59:41.000000 antelope_core-0.2.1/antelope_core/catalog_query.py
+-rw-r--r--   0 b          (500) b          (506)    10710 2022-04-09 17:53:42.000000 antelope_core-0.2.1/antelope_core/characterizations.py
+-rw-r--r--   0 b          (500) b          (506)    15445 2022-04-09 17:53:42.000000 antelope_core-0.2.1/antelope_core/contexts.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.524933 antelope_core-0.2.1/antelope_core/data_sources/
+-rw-r--r--   0 b          (500) b          (506)        0 2018-10-26 21:44:35.000000 antelope_core-0.2.1/antelope_core/data_sources/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     3851 2022-04-09 17:53:42.000000 antelope_core-0.2.1/antelope_core/data_sources/data_source.py
+-rw-r--r--   0 b          (500) b          (506)     7497 2022-08-22 21:21:17.000000 antelope_core-0.2.1/antelope_core/data_sources/ecoinvent.py
+-rw-r--r--   0 b          (500) b          (506)     1741 2022-08-22 21:21:17.000000 antelope_core-0.2.1/antelope_core/data_sources/ecoinvent_lcia.py
+-rw-r--r--   0 b          (500) b          (506)     1303 2022-08-22 21:21:17.000000 antelope_core-0.2.1/antelope_core/data_sources/gwp_ipcc_2007.py
+-rw-r--r--   0 b          (500) b          (506)     4614 2020-11-05 09:30:15.000000 antelope_core-0.2.1/antelope_core/data_sources/local.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.524933 antelope_core-0.2.1/antelope_core/data_sources/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2018-10-26 21:44:35.000000 antelope_core-0.2.1/antelope_core/data_sources/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     4152 2022-04-09 17:53:42.000000 antelope_core-0.2.1/antelope_core/data_sources/tests/test_aa_local.py
+-rw-r--r--   0 b          (500) b          (506)     1541 2022-04-09 17:53:42.000000 antelope_core-0.2.1/antelope_core/data_sources/tests/test_ecoinvent.py
+-rw-r--r--   0 b          (500) b          (506)     7319 2021-07-08 16:41:41.000000 antelope_core-0.2.1/antelope_core/data_sources/tests/test_ecoinvent_lci.py
+-rw-r--r--   0 b          (500) b          (506)      815 2022-04-09 17:53:42.000000 antelope_core-0.2.1/antelope_core/data_sources/tests/test_ipcc2007.py
+-rw-r--r--   0 b          (500) b          (506)     7231 2023-04-08 03:20:33.000000 antelope_core-0.2.1/antelope_core/data_sources/tests/test_uslci.py
+-rw-r--r--   0 b          (500) b          (506)     2438 2022-08-22 21:21:17.000000 antelope_core-0.2.1/antelope_core/data_sources/traci.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.524933 antelope_core-0.2.1/antelope_core/data_sources/uslci/
+-rw-r--r--   0 b          (500) b          (506)       31 2020-12-29 09:58:58.000000 antelope_core-0.2.1/antelope_core/data_sources/uslci/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     6168 2022-08-22 21:21:17.000000 antelope_core-0.2.1/antelope_core/data_sources/uslci/uslci.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.524933 antelope_core-0.2.1/antelope_core/entities/
+-rw-r--r--   0 b          (500) b          (506)      181 2022-04-09 17:53:42.000000 antelope_core-0.2.1/antelope_core/entities/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    11169 2022-04-09 17:53:42.000000 antelope_core-0.2.1/antelope_core/entities/entities.py
+-rw-r--r--   0 b          (500) b          (506)     4408 2023-04-07 06:21:46.000000 antelope_core-0.2.1/antelope_core/entities/flows.py
+-rw-r--r--   0 b          (500) b          (506)    24934 2023-02-24 05:55:04.000000 antelope_core-0.2.1/antelope_core/entities/processes.py
+-rw-r--r--   0 b          (500) b          (506)     7804 2023-02-06 19:33:10.000000 antelope_core-0.2.1/antelope_core/entities/quantities.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.524933 antelope_core-0.2.1/antelope_core/entities/tests/
+-rw-r--r--   0 b          (500) b          (506)       62 2019-02-15 00:01:58.000000 antelope_core-0.2.1/antelope_core/entities/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     1065 2021-01-07 23:11:04.000000 antelope_core-0.2.1/antelope_core/entities/tests/base_testclass.py
+-rw-r--r--   0 b          (500) b          (506)    99142 2019-03-19 20:06:35.000000 antelope_core-0.2.1/antelope_core/entities/tests/test_archive.json
+-rw-r--r--   0 b          (500) b          (506)     1019 2020-03-30 08:22:53.000000 antelope_core-0.2.1/antelope_core/entities/tests/test_entities.py
+-rw-r--r--   0 b          (500) b          (506)      850 2020-12-29 09:58:58.000000 antelope_core-0.2.1/antelope_core/entities/tests/test_entity_refs.py
+-rw-r--r--   0 b          (500) b          (506)      291 2020-03-30 08:22:53.000000 antelope_core-0.2.1/antelope_core/entities/tests/test_flows.py
+-rw-r--r--   0 b          (500) b          (506)     1538 2020-03-30 08:22:53.000000 antelope_core-0.2.1/antelope_core/entities/tests/test_processes.py
+-rw-r--r--   0 b          (500) b          (506)     1565 2020-09-29 22:38:38.000000 antelope_core-0.2.1/antelope_core/entities/tests/test_quantities.py
+-rw-r--r--   0 b          (500) b          (506)    18234 2022-06-13 20:26:37.000000 antelope_core-0.2.1/antelope_core/entities/xlsx_editor.py
+-rw-r--r--   0 b          (500) b          (506)    22640 2022-04-09 17:53:42.000000 antelope_core-0.2.1/antelope_core/exchanges.py
+-rw-r--r--   0 b          (500) b          (506)     6756 2023-01-11 07:42:19.000000 antelope_core-0.2.1/antelope_core/file_accessor.py
+-rw-r--r--   0 b          (500) b          (506)     1137 2021-09-21 18:51:48.000000 antelope_core-0.2.1/antelope_core/from_json.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.528267 antelope_core-0.2.1/antelope_core/implementations/
+-rw-r--r--   0 b          (500) b          (506)      333 2021-09-21 18:51:48.000000 antelope_core-0.2.1/antelope_core/implementations/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     8780 2023-04-10 06:04:23.000000 antelope_core-0.2.1/antelope_core/implementations/background.py
+-rw-r--r--   0 b          (500) b          (506)     5772 2023-04-08 06:49:08.000000 antelope_core-0.2.1/antelope_core/implementations/basic.py
+-rw-r--r--   0 b          (500) b          (506)     9856 2022-04-09 17:53:42.000000 antelope_core-0.2.1/antelope_core/implementations/configure.py
+-rw-r--r--   0 b          (500) b          (506)     2812 2022-04-09 17:53:42.000000 antelope_core-0.2.1/antelope_core/implementations/exchange.py
+-rw-r--r--   0 b          (500) b          (506)     6064 2022-04-09 17:53:42.000000 antelope_core-0.2.1/antelope_core/implementations/index.py
+-rw-r--r--   0 b          (500) b          (506)    32779 2023-04-07 06:21:46.000000 antelope_core-0.2.1/antelope_core/implementations/quantity.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.528267 antelope_core-0.2.1/antelope_core/implementations/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2018-09-13 20:45:30.000000 antelope_core-0.2.1/antelope_core/implementations/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     2056 2022-04-09 17:53:42.000000 antelope_core-0.2.1/antelope_core/implementations/tests/test_quantity.py
+-rw-r--r--   0 b          (500) b          (506)    16474 2022-12-31 00:11:14.000000 antelope_core-0.2.1/antelope_core/lc_resource.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.528267 antelope_core-0.2.1/antelope_core/lcia_engine/
+-rw-r--r--   0 b          (500) b          (506)     5632 2023-02-02 21:42:48.000000 antelope_core-0.2.1/antelope_core/lcia_engine/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     8163 2022-04-09 17:53:42.000000 antelope_core-0.2.1/antelope_core/lcia_engine/clookup.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.528267 antelope_core-0.2.1/antelope_core/lcia_engine/data/
+-rw-r--r--   0 b          (500) b          (506)     8420 2022-08-27 07:18:09.000000 antelope_core-0.2.1/antelope_core/lcia_engine/data/contexts.json
+-rw-r--r--   0 b          (500) b          (506)   383481 2020-03-30 08:22:53.000000 antelope_core-0.2.1/antelope_core/lcia_engine/data/flowables.json
+-rw-r--r--   0 b          (500) b          (506)    30980 2021-01-07 00:24:41.000000 antelope_core-0.2.1/antelope_core/lcia_engine/data/ipcc_2007_gwp.json
+-rw-r--r--   0 b          (500) b          (506)    18298 2023-04-07 07:51:58.000000 antelope_core-0.2.1/antelope_core/lcia_engine/lcia_engine.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.528267 antelope_core-0.2.1/antelope_core/lcia_engine/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2020-03-30 08:22:53.000000 antelope_core-0.2.1/antelope_core/lcia_engine/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     1513 2023-04-07 06:21:46.000000 antelope_core-0.2.1/antelope_core/lcia_engine/tests/test_biogenic_co2.py
+-rw-r--r--   0 b          (500) b          (506)     2559 2020-03-30 08:22:53.000000 antelope_core-0.2.1/antelope_core/lcia_engine/tests/test_clookup.py
+-rw-r--r--   0 b          (500) b          (506)      924 2020-09-29 22:38:38.000000 antelope_core-0.2.1/antelope_core/lcia_engine/tests/test_ipcc.py
+-rw-r--r--   0 b          (500) b          (506)     2981 2021-10-30 03:39:36.000000 antelope_core-0.2.1/antelope_core/lcia_engine/tests/test_lcia_engine.py
+-rw-r--r--   0 b          (500) b          (506)    41768 2023-04-07 07:51:58.000000 antelope_core-0.2.1/antelope_core/lcia_results.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.528267 antelope_core-0.2.1/antelope_core/providers/
+-rw-r--r--   0 b          (500) b          (506)     4617 2022-11-07 09:16:47.000000 antelope_core-0.2.1/antelope_core/providers/__init__.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.531600 antelope_core-0.2.1/antelope_core/providers/data/
+-rw-r--r--   0 b          (500) b          (506)       57 2019-02-15 00:01:58.000000 antelope_core-0.2.1/antelope_core/providers/data/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    39336 2018-07-26 08:24:01.000000 antelope_core-0.2.1/antelope_core/providers/data/list_of_methods_and_indicators_ecoinvent_v3.2.xlsx
+-rw-r--r--   0 b          (500) b          (506)    95429 2019-02-15 00:01:58.000000 antelope_core-0.2.1/antelope_core/providers/data/traci_2_1_2014_dec_10_0_test.xlsx
+-rw-r--r--   0 b          (500) b          (506)     9551 2022-08-01 22:59:24.000000 antelope_core-0.2.1/antelope_core/providers/ecoinvent_lcia.py
+-rw-r--r--   0 b          (500) b          (506)    11083 2022-04-09 17:53:42.000000 antelope_core-0.2.1/antelope_core/providers/ecospold.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.531600 antelope_core-0.2.1/antelope_core/providers/ecospold2/
+-rw-r--r--   0 b          (500) b          (506)       41 2018-07-26 08:24:01.000000 antelope_core-0.2.1/antelope_core/providers/ecospold2/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    24560 2022-08-23 23:02:58.000000 antelope_core-0.2.1/antelope_core/providers/ecospold2/ecospold2.py
+-rw-r--r--   0 b          (500) b          (506)      564 2020-10-18 05:43:46.000000 antelope_core-0.2.1/antelope_core/providers/ecospold2/ecospold2_index.py
+-rw-r--r--   0 b          (500) b          (506)     2134 2020-03-30 08:22:53.000000 antelope_core-0.2.1/antelope_core/providers/ecospold2/master_data.py
+-rw-r--r--   0 b          (500) b          (506)    10917 2023-02-02 16:59:51.000000 antelope_core-0.2.1/antelope_core/providers/file_store.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.531600 antelope_core-0.2.1/antelope_core/providers/ilcd/
+-rw-r--r--   0 b          (500) b          (506)       78 2018-07-26 08:24:01.000000 antelope_core-0.2.1/antelope_core/providers/ilcd/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    17683 2022-04-09 17:53:42.000000 antelope_core-0.2.1/antelope_core/providers/ilcd/ilcd.py
+-rw-r--r--   0 b          (500) b          (506)     2314 2018-07-26 08:24:01.000000 antelope_core-0.2.1/antelope_core/providers/ilcd/ilcd_flowables.py
+-rw-r--r--   0 b          (500) b          (506)     5806 2022-04-09 17:53:42.000000 antelope_core-0.2.1/antelope_core/providers/ilcd/ilcd_lcia.py
+-rw-r--r--   0 b          (500) b          (506)      314 2020-09-29 23:36:41.000000 antelope_core-0.2.1/antelope_core/providers/ilcd/index.py
+-rw-r--r--   0 b          (500) b          (506)     3177 2021-09-21 18:51:48.000000 antelope_core-0.2.1/antelope_core/providers/ilcd/quantity.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.531600 antelope_core-0.2.1/antelope_core/providers/ilcd/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2021-01-07 00:24:41.000000 antelope_core-0.2.1/antelope_core/providers/ilcd/tests/__init__.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.514933 antelope_core-0.2.1/antelope_core/providers/ilcd/tests/data/
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.514933 antelope_core-0.2.1/antelope_core/providers/ilcd/tests/data/ilcd_test/
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.514933 antelope_core-0.2.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.531600 antelope_core-0.2.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/
+-rw-r--r--   0 b          (500) b          (506)     2712 2019-02-15 00:01:58.000000 antelope_core-0.2.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-11da-a746-0800200b9a66.xml
+-rw-r--r--   0 b          (500) b          (506)     2738 2019-02-15 00:01:58.000000 antelope_core-0.2.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-11da-a746-0800200c9a66.xml
+-rw-r--r--   0 b          (500) b          (506)     2734 2019-02-15 00:01:58.000000 antelope_core-0.2.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-13da-a746-0800200c9a66.xml
+-rw-r--r--   0 b          (500) b          (506)     2716 2019-02-15 00:01:58.000000 antelope_core-0.2.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-22da-a746-0800200c9a66.xml
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.531600 antelope_core-0.2.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flows/
+-rw-r--r--   0 b          (500) b          (506)     5078 2019-02-15 00:01:58.000000 antelope_core-0.2.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flows/f579de8c-8897-4bdb-9a0a-b36f8b13282e.xml
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.531600 antelope_core-0.2.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/
+-rw-r--r--   0 b          (500) b          (506)     2503 2019-02-15 00:01:58.000000 antelope_core-0.2.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/1ff9a08c-6fc1-4509-8bcd-a5404c598755.xml
+-rw-r--r--   0 b          (500) b          (506)     3551 2019-02-15 00:01:58.000000 antelope_core-0.2.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/ad38d542-3fe9-439d-9b95-2f5f7752acaf.xml
+-rw-r--r--   0 b          (500) b          (506)     3344 2019-02-15 00:01:58.000000 antelope_core-0.2.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/cd950537-0a98-4044-9ba7-9f9a68d0a504.xml
+-rw-r--r--   0 b          (500) b          (506)     4443 2019-02-15 00:01:58.000000 antelope_core-0.2.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/de5104d8-3de0-4218-a29d-b7123ce9ca3c.xml
+-rw-r--r--   0 b          (500) b          (506)      932 2021-01-07 00:24:41.000000 antelope_core-0.2.1/antelope_core/providers/ilcd/tests/test_ilcd.py
+-rw-r--r--   0 b          (500) b          (506)    21764 2023-02-24 05:50:36.000000 antelope_core-0.2.1/antelope_core/providers/openlca_jsonld.py
+-rw-r--r--   0 b          (500) b          (506)      729 2021-10-30 03:39:36.000000 antelope_core-0.2.1/antelope_core/providers/parse_math.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.531600 antelope_core-0.2.1/antelope_core/providers/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2018-07-26 08:24:01.000000 antelope_core-0.2.1/antelope_core/providers/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)      569 2020-09-29 23:35:54.000000 antelope_core-0.2.1/antelope_core/providers/tests/test_ecospold.py
+-rw-r--r--   0 b          (500) b          (506)     4110 2018-07-26 08:24:01.000000 antelope_core-0.2.1/antelope_core/providers/tests/test_xml_widgets.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.534934 antelope_core-0.2.1/antelope_core/providers/traci/
+-rw-r--r--   0 b          (500) b          (506)       50 2018-07-26 08:24:01.000000 antelope_core-0.2.1/antelope_core/providers/traci/__init__.py
+-rw-r--r--   0 b          (500) b          (506)      653 2020-09-29 23:35:54.000000 antelope_core-0.2.1/antelope_core/providers/traci/index.py
+-rw-r--r--   0 b          (500) b          (506)     3441 2019-01-17 18:55:10.000000 antelope_core-0.2.1/antelope_core/providers/traci/q_info.py
+-rw-r--r--   0 b          (500) b          (506)     2076 2020-09-29 23:35:54.000000 antelope_core-0.2.1/antelope_core/providers/traci/quantity.py
+-rw-r--r--   0 b          (500) b          (506)     1648 2020-03-30 08:22:53.000000 antelope_core-0.2.1/antelope_core/providers/traci/test_traci.py
+-rw-r--r--   0 b          (500) b          (506)     6687 2022-04-09 17:53:42.000000 antelope_core-0.2.1/antelope_core/providers/traci/traci_2_1_spreadsheet.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.534934 antelope_core-0.2.1/antelope_core/providers/xdb_client/
+-rw-r--r--   0 b          (500) b          (506)       33 2022-11-14 22:48:38.000000 antelope_core-0.2.1/antelope_core/providers/xdb_client/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    16345 2023-04-10 21:06:08.000000 antelope_core-0.2.1/antelope_core/providers/xdb_client/implementation.py
+-rw-r--r--   0 b          (500) b          (506)     3987 2023-04-08 06:34:47.000000 antelope_core-0.2.1/antelope_core/providers/xdb_client/requester.py
+-rw-r--r--   0 b          (500) b          (506)     6873 2023-04-10 21:41:48.000000 antelope_core-0.2.1/antelope_core/providers/xdb_client/rest_client.py
+-rw-r--r--   0 b          (500) b          (506)     5746 2023-04-07 19:16:29.000000 antelope_core-0.2.1/antelope_core/providers/xdb_client/xdb_client.py
+-rw-r--r--   0 b          (500) b          (506)     2912 2023-04-07 19:16:29.000000 antelope_core-0.2.1/antelope_core/providers/xdb_client/xdb_entities.py
+-rw-r--r--   0 b          (500) b          (506)     2316 2022-08-01 23:00:27.000000 antelope_core-0.2.1/antelope_core/providers/xl_dict.py
+-rw-r--r--   0 b          (500) b          (506)     1676 2020-03-30 08:22:53.000000 antelope_core-0.2.1/antelope_core/providers/xml_widgets.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.534934 antelope_core-0.2.1/antelope_core/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2018-07-26 08:24:01.000000 antelope_core-0.2.1/antelope_core/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)      972 2020-09-29 22:38:38.000000 antelope_core-0.2.1/antelope_core/tests/test_autorange.py
+-rw-r--r--   0 b          (500) b          (506)    12509 2022-04-09 17:53:42.000000 antelope_core-0.2.1/antelope_core/tests/test_contexts.py
+-rw-r--r--   0 b          (500) b          (506)     5637 2020-12-29 09:58:58.000000 antelope_core-0.2.1/antelope_core/tests/test_exchanges.py
+-rw-r--r--   0 b          (500) b          (506)      500 2020-12-29 09:58:58.000000 antelope_core-0.2.1/antelope_core/tests/test_lcia_results.py
+-rw-r--r--   0 b          (500) b          (506)     1162 2020-09-30 00:02:12.000000 antelope_core-0.2.1/antelope_core/tests/test_resources.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:44:38.518267 antelope_core-0.2.1/antelope_core.egg-info/
+-rw-r--r--   0 b          (500) b          (506)    14232 2023-04-10 21:44:38.000000 antelope_core-0.2.1/antelope_core.egg-info/PKG-INFO
+-rw-r--r--   0 b          (500) b          (506)     6732 2023-04-10 21:44:38.000000 antelope_core-0.2.1/antelope_core.egg-info/SOURCES.txt
+-rw-r--r--   0 b          (500) b          (506)        1 2023-04-10 21:44:38.000000 antelope_core-0.2.1/antelope_core.egg-info/dependency_links.txt
+-rw-r--r--   0 b          (500) b          (506)      169 2023-04-10 21:44:38.000000 antelope_core-0.2.1/antelope_core.egg-info/requires.txt
+-rw-r--r--   0 b          (500) b          (506)       14 2023-04-10 21:44:38.000000 antelope_core-0.2.1/antelope_core.egg-info/top_level.txt
+-rw-r--r--   0 b          (500) b          (506)       38 2023-04-10 21:44:38.534934 antelope_core-0.2.1/setup.cfg
+-rw-r--r--   0 b          (500) b          (506)     3544 2023-04-10 21:37:42.000000 antelope_core-0.2.1/setup.py
```

### Comparing `antelope_core-0.2.0/LICENSE` & `antelope_core-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/PKG-INFO` & `antelope_core-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antelope_core
-Version: 0.2.0
+Version: 0.2.1
 Home-page: https://github.com/AntelopeLCA/core
 Author: Brandon Kuczenski
 Author-email: bkuczenski@ucsb.edu
 License: BSD 3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `antelope_core-0.2.0/README.md` & `antelope_core-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/__init__.py` & `antelope_core-0.2.1/antelope_core/__init__.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/archives/__init__.py` & `antelope_core-0.2.1/antelope_core/archives/__init__.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/archives/archive_index.py` & `antelope_core-0.2.1/antelope_core/archives/archive_index.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/archives/basic_archive.py` & `antelope_core-0.2.1/antelope_core/archives/basic_archive.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/archives/data/elcd_reference_quantities.json` & `antelope_core-0.2.1/antelope_core/archives/data/elcd_reference_quantities.json`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/archives/entity_store.py` & `antelope_core-0.2.1/antelope_core/archives/entity_store.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/archives/lc_archive.py` & `antelope_core-0.2.1/antelope_core/archives/lc_archive.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/archives/quantity_manager.py` & `antelope_core-0.2.1/antelope_core/archives/quantity_manager.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/archives/term_manager.py` & `antelope_core-0.2.1/antelope_core/archives/term_manager.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/archives/tests/test_base.py` & `antelope_core-0.2.1/antelope_core/archives/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/archives/tests/test_basic_archive.py` & `antelope_core-0.2.1/antelope_core/archives/tests/test_basic_archive.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/archives/tests/test_entity_store.py` & `antelope_core-0.2.1/antelope_core/archives/tests/test_entity_store.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/archives/tests/test_json.json` & `antelope_core-0.2.1/antelope_core/archives/tests/test_json.json`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/archives/tests/test_qdb.py` & `antelope_core-0.2.1/antelope_core/archives/tests/test_qdb.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/archives/tests/test_quantity_manager.py` & `antelope_core-0.2.1/antelope_core/archives/tests/test_quantity_manager.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/archives/tests/test_quantity_relation.py` & `antelope_core-0.2.1/antelope_core/archives/tests/test_quantity_relation.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/archives/tests/test_term_manager.py` & `antelope_core-0.2.1/antelope_core/archives/tests/test_term_manager.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/autorange.py` & `antelope_core-0.2.1/antelope_core/autorange.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/catalog/catalog.py` & `antelope_core-0.2.1/antelope_core/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/catalog/catalog_root.py` & `antelope_core-0.2.1/antelope_core/catalog/catalog_root.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/catalog/configurator.py` & `antelope_core-0.2.1/antelope_core/catalog/configurator.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/catalog/lc_catalog.py` & `antelope_core-0.2.1/antelope_core/catalog/lc_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,40 +202,45 @@
         :param store: [True] if False, don't save the record - use it for this session only
         :param kwargs:
         :return:
         """
         res = LcResource.from_archive(archive, interfaces, source=self._localize_source(archive.source), **kwargs)
         self._resolver.add_resource(res, store=store)
 
-    def blackbook_authenticate(self, blackbook_url, username=None, password=None, token=None):
+    def blackbook_authenticate(self, blackbook_url=None, username=None, password=None, token=None, save_credentials=True):
         """
         Opens an authenticated session with the designated blackbook server.  Credentials can either be provided to the
         method as arguments, or if omitted, they can be obtained through a form.  If a token is provided, it is
         used in lieu of a password workflow
         :param blackbook_url:
         :param username:
         :param password:
         :param token:
         :return:
         """
         if self._blackbook_client:
+            if blackbook_url is None:
+                self._blackbook_client.reauthenticate()  # or raise NoCredentials
+                return
             self._blackbook_client.close()
+        elif blackbook_url is None:
+            raise ValueError('Must provide a URL')
         if token is None:
-            client = RestClient(blackbook_url, auth_route='auth/token')
+            client = RestClient(blackbook_url, auth_route='auth/token', save_credentials=save_credentials)
             if username is None:
                 username = input('Enter username to access blackbook server at %s: ' % blackbook_url)
             if password is None:
                 password = getpass.getpass('Enter password to access blackbook server at %s: ' % blackbook_url)
             try:
                 client.authenticate(username, password)
             except HTTPError:
                 client.close()
                 raise
         else:
-            client = RestClient(blackbook_url, token=token, auth_route='auth/token')
+            client = RestClient(blackbook_url, token=token, auth_route='auth/token', save_credentials=save_credentials)
         self._blackbook_client = client
 
     def get_blackbook_resources(self, origin):
         """
         Use a blackbook server to obtain resources for a given origin.
         :param origin:
         :return:
```

### Comparing `antelope_core-0.2.0/antelope_core/catalog/lc_resolver.py` & `antelope_core-0.2.1/antelope_core/catalog/lc_resolver.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/catalog/tests/test_catalogs.py` & `antelope_core-0.2.1/antelope_core/catalog/tests/test_catalogs.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/catalog/tests/test_process_ref.py` & `antelope_core-0.2.1/antelope_core/catalog/tests/test_process_ref.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/catalog/tests/test_quantity_refs.py` & `antelope_core-0.2.1/antelope_core/catalog/tests/test_quantity_refs.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/catalog_query.py` & `antelope_core-0.2.1/antelope_core/catalog_query.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -267,19 +267,19 @@
                         k = [cf for cf in f._query_ref._chars_seen.keys() if cf[0] is quantity]
                         for cf in k:
                             f._query_ref.pop_char(*cf)
 
     def make_ref(self, entity):
         if isinstance(entity, list):
             return [self.make_ref(k) for k in entity]
+        if entity is None:
+            return None
         if entity.entity_type == 'fragment':
             # TODO: create a new ForegroundQuery to eliminate the need for this hack
             return entity  # don't make references for fragments just now
-        if entity is None:
-            return None
         if entity.is_entity:
             try:
                 e_ref = entity.make_ref(self._grounded_query(entity.origin))
             except UnknownOrigin:
                 e_ref = entity.make_ref(self)
         else:
             e_ref = entity  # already a ref
```

### Comparing `antelope_core-0.2.0/antelope_core/characterizations.py` & `antelope_core-0.2.1/antelope_core/characterizations.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/contexts.py` & `antelope_core-0.2.1/antelope_core/contexts.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/data_sources/data_source.py` & `antelope_core-0.2.1/antelope_core/data_sources/data_source.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/data_sources/ecoinvent.py` & `antelope_core-0.2.1/antelope_core/data_sources/ecoinvent.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/data_sources/ecoinvent_lcia.py` & `antelope_core-0.2.1/antelope_core/data_sources/ecoinvent_lcia.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/data_sources/gwp_ipcc_2007.py` & `antelope_core-0.2.1/antelope_core/data_sources/gwp_ipcc_2007.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/data_sources/local.py` & `antelope_core-0.2.1/antelope_core/data_sources/local.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/data_sources/tests/test_aa_local.py` & `antelope_core-0.2.1/antelope_core/data_sources/tests/test_aa_local.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/data_sources/tests/test_ecoinvent.py` & `antelope_core-0.2.1/antelope_core/data_sources/tests/test_ecoinvent.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/data_sources/tests/test_ecoinvent_lci.py` & `antelope_core-0.2.1/antelope_core/data_sources/tests/test_ecoinvent_lci.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/data_sources/tests/test_ipcc2007.py` & `antelope_core-0.2.1/antelope_core/data_sources/tests/test_ipcc2007.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/data_sources/tests/test_uslci.py` & `antelope_core-0.2.1/antelope_core/data_sources/tests/test_uslci.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
         def _get_fg_test_case_rx(self):
             p = next(self.query.processes(Name='Seedlings, at greenhouse, US PNW'))
             return p.reference()
 
         def _get_fg_test_case_lci(self):
             rx = self._get_fg_test_case_rx()
-            return [x for x in self.query.lci(rx.process.external_ref, rx.flow.external_ref)]
+            return list(rx.process.lci(rx.flow.external_ref))
 
         def _get_fg_test_case_observed(self):
             rx = self._get_fg_test_case_rx()
             return rx.process.exchange_values(self._test_case_observed_flow)
 
         def test_21_exchange_relation(self):
             rx = self._get_fg_test_case_rx()
```

### Comparing `antelope_core-0.2.0/antelope_core/data_sources/traci.py` & `antelope_core-0.2.1/antelope_core/data_sources/traci.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/data_sources/uslci/uslci.py` & `antelope_core-0.2.1/antelope_core/data_sources/uslci/uslci.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/entities/entities.py` & `antelope_core-0.2.1/antelope_core/entities/entities.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/entities/flows.py` & `antelope_core-0.2.1/antelope_core/entities/flows.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/entities/processes.py` & `antelope_core-0.2.1/antelope_core/entities/processes.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/entities/quantities.py` & `antelope_core-0.2.1/antelope_core/entities/quantities.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/entities/tests/base_testclass.py` & `antelope_core-0.2.1/antelope_core/entities/tests/base_testclass.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/entities/tests/test_archive.json` & `antelope_core-0.2.1/antelope_core/entities/tests/test_archive.json`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/entities/tests/test_entities.py` & `antelope_core-0.2.1/antelope_core/entities/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/entities/tests/test_entity_refs.py` & `antelope_core-0.2.1/antelope_core/entities/tests/test_entity_refs.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/entities/tests/test_processes.py` & `antelope_core-0.2.1/antelope_core/entities/tests/test_processes.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/entities/tests/test_quantities.py` & `antelope_core-0.2.1/antelope_core/entities/tests/test_quantities.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/entities/xlsx_editor.py` & `antelope_core-0.2.1/antelope_core/entities/xlsx_editor.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/exchanges.py` & `antelope_core-0.2.1/antelope_core/exchanges.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/file_accessor.py` & `antelope_core-0.2.1/antelope_core/file_accessor.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/from_json.py` & `antelope_core-0.2.1/antelope_core/from_json.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/implementations/background.py` & `antelope_core-0.2.1/antelope_core/implementations/background.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from itertools import chain
 
 from .basic import BasicImplementation
 from antelope import BackgroundInterface, ExteriorFlow, EntityNotFound, comp_dir  # , ProductFlow
 from antelope_core.contexts import Context
 
 
 class NonStaticBackground(Exception):
@@ -201,7 +202,36 @@
         For sys_lci, we should just do the same. yield the supplied demand as a degenerate LCI.
         :param demand:
         :param kwargs:
         :return:
         """
         for y in demand:
             yield y
+
+    def bg_lcia(self, process, query_qty, observed=None, ref_flow=None, **kwargs):
+        """
+        returns an LciaResult object, aggregated as appropriate depending on the interface's privacy level.
+        This is an ensemble function that stitches together bg functions with quantity access.
+
+        :param process:
+        :param query_qty: must be an operable quantity_ref. the process must have exchange access
+        :param observed: iterable of DirectedFlows (flow: FlowSpec, direction: str)
+        :param ref_flow:
+        :param kwargs:
+        :return:
+        """
+        p_ref = self.get(process)  # a ref-- unless this was a basic impl. hrm.
+        if p_ref.is_entity:
+            raise NotImplementedError  # we can't proceed
+        if observed is None:
+            observed = ()
+        obs = set((x.flow.external_ref, x.direction) for x in observed)
+        if len(obs) > 0:
+            exts = chain(p_ref.emissions(ref_flow=ref_flow),
+                         p_ref.cutoffs(ref_flow=ref_flow))
+            incl = (k for k in p_ref.dependencies(ref_flow=ref_flow) if (k.flow.external_ref, k.direction) not in obs)
+            ext = (k for k in exts if (k.flow.external_ref, k.direction) not in obs)
+            lci = chain(self.sys_lci(incl), ext)
+        else:
+            lci = p_ref.lci(ref_flow=ref_flow)
+        # aggregation
+        return query_qty.do_lcia(lci, **kwargs)
```

### Comparing `antelope_core-0.2.0/antelope_core/implementations/basic.py` & `antelope_core-0.2.1/antelope_core/implementations/basic.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/implementations/configure.py` & `antelope_core-0.2.1/antelope_core/implementations/configure.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/implementations/exchange.py` & `antelope_core-0.2.1/antelope_core/implementations/exchange.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/implementations/index.py` & `antelope_core-0.2.1/antelope_core/implementations/index.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/implementations/quantity.py` & `antelope_core-0.2.1/antelope_core/implementations/quantity.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/implementations/tests/test_quantity.py` & `antelope_core-0.2.1/antelope_core/implementations/tests/test_quantity.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/lc_resource.py` & `antelope_core-0.2.1/antelope_core/lc_resource.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/lcia_engine/__init__.py` & `antelope_core-0.2.1/antelope_core/lcia_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/lcia_engine/clookup.py` & `antelope_core-0.2.1/antelope_core/lcia_engine/clookup.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/lcia_engine/data/contexts.json` & `antelope_core-0.2.1/antelope_core/lcia_engine/data/contexts.json`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/lcia_engine/data/flowables.json` & `antelope_core-0.2.1/antelope_core/lcia_engine/data/flowables.json`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/lcia_engine/data/ipcc_2007_gwp.json` & `antelope_core-0.2.1/antelope_core/lcia_engine/data/ipcc_2007_gwp.json`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/lcia_engine/lcia_engine.py` & `antelope_core-0.2.1/antelope_core/lcia_engine/lcia_engine.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/lcia_engine/tests/test_biogenic_co2.py` & `antelope_core-0.2.1/antelope_core/lcia_engine/tests/test_biogenic_co2.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/lcia_engine/tests/test_clookup.py` & `antelope_core-0.2.1/antelope_core/lcia_engine/tests/test_clookup.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/lcia_engine/tests/test_ipcc.py` & `antelope_core-0.2.1/antelope_core/lcia_engine/tests/test_ipcc.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/lcia_engine/tests/test_lcia_engine.py` & `antelope_core-0.2.1/antelope_core/lcia_engine/tests/test_lcia_engine.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/lcia_results.py` & `antelope_core-0.2.1/antelope_core/lcia_results.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/__init__.py` & `antelope_core-0.2.1/antelope_core/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/data/list_of_methods_and_indicators_ecoinvent_v3.2.xlsx` & `antelope_core-0.2.1/antelope_core/providers/data/list_of_methods_and_indicators_ecoinvent_v3.2.xlsx`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/data/traci_2_1_2014_dec_10_0_test.xlsx` & `antelope_core-0.2.1/antelope_core/providers/data/traci_2_1_2014_dec_10_0_test.xlsx`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/ecoinvent_lcia.py` & `antelope_core-0.2.1/antelope_core/providers/ecoinvent_lcia.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/ecospold.py` & `antelope_core-0.2.1/antelope_core/providers/ecospold.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/ecospold2/ecospold2.py` & `antelope_core-0.2.1/antelope_core/providers/ecospold2/ecospold2.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/ecospold2/ecospold2_index.py` & `antelope_core-0.2.1/antelope_core/providers/ecospold2/ecospold2_index.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/ecospold2/master_data.py` & `antelope_core-0.2.1/antelope_core/providers/ecospold2/master_data.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/file_store.py` & `antelope_core-0.2.1/antelope_core/providers/file_store.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/ilcd/ilcd.py` & `antelope_core-0.2.1/antelope_core/providers/ilcd/ilcd.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/ilcd/ilcd_flowables.py` & `antelope_core-0.2.1/antelope_core/providers/ilcd/ilcd_flowables.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/ilcd/ilcd_lcia.py` & `antelope_core-0.2.1/antelope_core/providers/ilcd/ilcd_lcia.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/ilcd/quantity.py` & `antelope_core-0.2.1/antelope_core/providers/ilcd/quantity.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-11da-a746-0800200b9a66.xml` & `antelope_core-0.2.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-11da-a746-0800200b9a66.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-11da-a746-0800200c9a66.xml` & `antelope_core-0.2.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-11da-a746-0800200c9a66.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-13da-a746-0800200c9a66.xml` & `antelope_core-0.2.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-13da-a746-0800200c9a66.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-22da-a746-0800200c9a66.xml` & `antelope_core-0.2.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flowproperties/93a60a56-a3c8-22da-a746-0800200c9a66.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flows/f579de8c-8897-4bdb-9a0a-b36f8b13282e.xml` & `antelope_core-0.2.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/flows/f579de8c-8897-4bdb-9a0a-b36f8b13282e.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/1ff9a08c-6fc1-4509-8bcd-a5404c598755.xml` & `antelope_core-0.2.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/1ff9a08c-6fc1-4509-8bcd-a5404c598755.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/ad38d542-3fe9-439d-9b95-2f5f7752acaf.xml` & `antelope_core-0.2.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/ad38d542-3fe9-439d-9b95-2f5f7752acaf.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/cd950537-0a98-4044-9ba7-9f9a68d0a504.xml` & `antelope_core-0.2.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/cd950537-0a98-4044-9ba7-9f9a68d0a504.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/de5104d8-3de0-4218-a29d-b7123ce9ca3c.xml` & `antelope_core-0.2.1/antelope_core/providers/ilcd/tests/data/ilcd_test/ILCD/unitgroups/de5104d8-3de0-4218-a29d-b7123ce9ca3c.xml`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/ilcd/tests/test_ilcd.py` & `antelope_core-0.2.1/antelope_core/providers/ilcd/tests/test_ilcd.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/openlca_jsonld.py` & `antelope_core-0.2.1/antelope_core/providers/openlca_jsonld.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/parse_math.py` & `antelope_core-0.2.1/antelope_core/providers/parse_math.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/tests/test_ecospold.py` & `antelope_core-0.2.1/antelope_core/providers/tests/test_ecospold.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/tests/test_xml_widgets.py` & `antelope_core-0.2.1/antelope_core/providers/tests/test_xml_widgets.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/traci/index.py` & `antelope_core-0.2.1/antelope_core/providers/traci/index.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/traci/q_info.py` & `antelope_core-0.2.1/antelope_core/providers/traci/q_info.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/traci/quantity.py` & `antelope_core-0.2.1/antelope_core/providers/traci/quantity.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/traci/test_traci.py` & `antelope_core-0.2.1/antelope_core/providers/traci/test_traci.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/traci/traci_2_1_spreadsheet.py` & `antelope_core-0.2.1/antelope_core/providers/traci/traci_2_1_spreadsheet.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/xdb_client/implementation.py` & `antelope_core-0.2.1/antelope_core/providers/xdb_client/implementation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from collections import defaultdict
-
+# from collections import defaultdict
+import json
 from antelope import IndexInterface, ExchangeInterface, QuantityInterface, BackgroundInterface
-from antelope import comp_dir, ExchangeRef, RxRef
+from antelope import ExchangeRef, RxRef, EntityNotFound, comp_dir
+from antelope.models import (OriginCount, Entity, FlowEntity, Exchange, ReferenceExchange, UnallocatedExchange,
+                             DetailedLciaResult, AllocatedExchange, Characterization as CharacterizationModel,
+                             ExchangeValues, DirectedFlow)
+
 from antelope_core.implementations import BasicImplementation
-from antelope_core.models import (OriginCount, Entity, FlowEntity, Exchange, ReferenceExchange, UnallocatedExchange,
-                                  DetailedLciaResult, AllocatedExchange, Characterization as CharacterizationModel,
-                                  ExchangeValues, DirectedFlow)
 from antelope_core.lcia_results import LciaResult
 from antelope_core.characterizations import Characterization, QRResult
 
 from .xdb_entities import XdbEntity
 from requests.exceptions import HTTPError
 
 
@@ -172,27 +173,64 @@
             return list(self._resolve_ex(ex)
                         for ex in self._archive.r.get_many(AllocatedExchange, _ref(node), _ref(ref_flow), 'inventory'))
         elif scenario:
             return list(self._resolve_ex(ex)
                         for ex in self._archive.r.get_many(AllocatedExchange, _ref(node), 'inventory',
                                                            scenario=scenario))
         else:
-            return list(self._resolve_ex(ex) for ex in self._archive.r.get_many(AllocatedExchange, _ref(node), 'inventory'))
+            return list(self._resolve_ex(ex) for ex in self._archive.r.get_many(AllocatedExchange, _ref(node),
+                                                                                'inventory'))
+
+    def dependencies(self, process, ref_flow=None, **kwargs):
+        if ref_flow:
+            # process inventory
+            return list(self._resolve_ex(ex) for ex in self._archive.r.get_many(AllocatedExchange, _ref(process),
+                                                                                _ref(ref_flow), 'dependencies'))
+        else:
+            return list(self._resolve_ex(ex) for ex in self._archive.r.get_many(AllocatedExchange, _ref(process),
+                                                                                'dependencies'))
+
+    def emissions(self, process, ref_flow=None, **kwargs):
+        if ref_flow:
+            # process inventory
+            return list(self._resolve_ex(ex) for ex in self._archive.r.get_many(AllocatedExchange, _ref(process),
+                                                                                _ref(ref_flow), 'emissions'))
+        else:
+            return list(self._resolve_ex(ex) for ex in self._archive.r.get_many(AllocatedExchange, _ref(process),
+                                                                                'emissions'))
+
+    def cutoffs(self, process, ref_flow=None, **kwargs):
+        if ref_flow:
+            # process inventory
+            return list(self._resolve_ex(ex) for ex in self._archive.r.get_many(AllocatedExchange, _ref(process),
+                                                                                _ref(ref_flow), 'cutoffs'))
+        else:
+            return list(self._resolve_ex(ex) for ex in self._archive.r.get_many(AllocatedExchange, _ref(process),
+                                                                                'cutoffs'))
 
     def lci(self, process, ref_flow=None, **kwargs):
         if ref_flow:
             # process inventory
             return list(self._resolve_ex(ex)
                         for ex in self._archive.r.get_many(AllocatedExchange, _ref(process), _ref(ref_flow), 'lci'))
         else:
             return list(self._resolve_ex(ex) for ex in self._archive.r.get_many(AllocatedExchange, _ref(process), 'lci'))
 
+    def _to_exch_ref(self, x):
+        """
+        We can't resolve references from here! something is fucked
+        :param x:
+        :return:
+        """
+        pass
+
     def sys_lci(self, demand, **kwargs):
-        dmd = [UnallocatedExchange.from_exchange(x) for x in demand]
-        return self._archive.r.post_return_many(UnallocatedExchange, dmd, 'sys_lci', **kwargs)
+        dmd = [UnallocatedExchange.from_inv(x).dict() for x in demand]
+        return list(self._resolve_ex(ex)  # DWR! THESE ARE NOT OPERATIONAL EXCHANGES YET!!!
+                    for ex in self._archive.r.post_return_many(dmd, UnallocatedExchange, 'sys_lci', **kwargs))
 
     '''
     qdb routes
     '''
     def get_canonical(self, quantity, **kwargs):
         """
 
@@ -276,30 +314,33 @@
                 cf = QRResult(d.factor.flowable, ex.flow.reference_entity, quantity, ex.termination,
                               d.factor.locale, d.factor.origin, d.factor.value)
                 res.add_score(c.component, ex, cf)
             for s in c.summaries:
                 res.add_summary(c.component, node, s.node_weight, s.unit_score)
         return res
 
-    def _result_from_model(self, process, quantity, res_m: DetailedLciaResult):
+    def _result_from_model(self, process_ref, quantity, res_m: DetailedLciaResult):
         """
         Constructs a Detailed LCIA result from a background LCIA query, when we don't have a list of exchanges
-        :param process:
+        :param process_ref:
         :param quantity:
         :param res_m:
         :return:
         """
         res = LciaResult(quantity, scenario=res_m.scenario, scale=res_m.scale)
+        process = self.get(process_ref)
+        res.add_component(process_ref, entity=process)
         for c in res_m.components:
             for d in c.details:
                 value = d.result / d.factor.value
-                ex = UnallocatedExchange(origin=process.origin, process=process, flow=d.exchange, direction='',
-                                         context=d.exchange.context, value=value)
-                rq = self.get_canonical(ex.flow.quantity_ref)
-                cf = QRResult(d.factor.flowable, rq, quantity, ex.context,
+                cx = self.get_context(d.exchange.context)
+                ex = ExchangeRef(process, self.get(d.exchange.external_ref), comp_dir(cx.sense),
+                                 termination=cx, value=value)
+                rq = self.get_canonical(d.exchange.quantity_ref)
+                cf = QRResult(d.factor.flowable, rq, quantity, cx,
                               d.factor.locale, d.factor.origin, d.factor.value)
                 res.add_score(c.component, ex, cf)
             for s in c.summaries:
                 res.add_summary(c.component, process, s.node_weight, s.unit_score)
         return res
 
     def do_lcia(self, quantity, inventory, locale='GLO', **kwargs):
@@ -312,35 +353,46 @@
         :return:
         """
         exchanges = [UnallocatedExchange.from_inv(x).dict() for x in inventory]
         exch_map = {(x.flow.external_ref, x.term_ref): x for x in inventory}
 
         ress = self._archive.r.qdb_post_return_many(exchanges, DetailedLciaResult, _ref(quantity), 'do_lcia')
         return [self._result_from_exchanges(quantity, exch_map, res) for res in ress]
+        if len(res_out) == 1:
+            return res_out[0]
+        return res_out
 
     def bg_lcia(self, process, query_qty, observed=None, ref_flow=None, **kwargs):
         """
         We want to override the interface implementation and send a simple request to the backend
         :param process:
         :param query_qty:
         :param observed:
         :param ref_flow:
         :param kwargs: locale, quell_biogenic_co2
         :return:
         """
-        if observed:
-            obs_flows = [DirectedFlow.from_exchange(x) for x in observed]
-            if ref_flow:
-                ress = self._archive.r.post_return_many(obs_flows, DetailedLciaResult, _ref(process), _ref(ref_flow),
-                                                        'lcia', _ref(query_qty), **kwargs)
+        obs_flows = ()
+        try:
+            if observed:
+                obs_flows = [DirectedFlow.from_exchange(x).dict() for x in observed]
+            if len(obs_flows) > 0:
+                if ref_flow:
+                    ress = self._archive.r.post_return_many(obs_flows, DetailedLciaResult, _ref(process), _ref(ref_flow),
+                                                            'lcia', _ref(query_qty), **kwargs)
+                else:
+                    ress = self._archive.r.post_return_many(obs_flows, DetailedLciaResult, _ref(process),
+                                                            'lcia', _ref(query_qty), **kwargs)
             else:
-                ress = self._archive.r.post_return_many(obs_flows, DetailedLciaResult, _ref(process),
-                                                        'lcia', _ref(query_qty), **kwargs)
-        else:
-            if ref_flow:
-                ress = self._archive.r.get_many(DetailedLciaResult, _ref(process), _ref(ref_flow),
-                                                'lcia', _ref(query_qty), **kwargs)
+                if ref_flow:
+                    ress = self._archive.r.get_many(DetailedLciaResult, _ref(process), _ref(ref_flow),
+                                                    'lcia', _ref(query_qty), **kwargs)
+                else:
+                    ress = self._archive.r.get_many(DetailedLciaResult, _ref(process),
+                                                    'lcia', _ref(query_qty), **kwargs)
+        except HTTPError as e:
+            if e.args[0] == 404:
+                content = json.loads(e.args[1])
+                raise EntityNotFound(content['detail'])
             else:
-                ress = self._archive.r.get_many(DetailedLciaResult, _ref(process),
-                                                'lcia', _ref(query_qty), **kwargs)
-
+                raise
         return [self._result_from_model(process, query_qty, res) for res in ress]
```

### Comparing `antelope_core-0.2.0/antelope_core/providers/xdb_client/requester.py` & `antelope_core-0.2.1/antelope_core/providers/xdb_client/requester.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from antelope_core.models import ResponseModel, OriginMeta
+from antelope.models import ResponseModel, OriginMeta
 from .rest_client import RestClient
 
 
 class XdbRequester(RestClient):
     """
     A RestClient that encapsulates translating the HTTP responses to Pydantic models
      -get_one
@@ -59,18 +59,18 @@
     def get_many(self, model, *args, **kwargs):
         if issubclass(model, ResponseModel):
             return [model(**k) for k in self._get_endpoint(self._org, *args, **kwargs)]
         else:
             return [model(k) for k in self._get_endpoint(self._org, *args, **kwargs)]
 
     def qdb_get_one(self, model, *args, **kwargs):
-            return model(**self._get_endpoint(self._qdb, *args, **kwargs))
+        return model(**self._get_endpoint(self._qdb, *args, **kwargs))
 
     def qdb_get_many(self, model, *args, **kwargs):
-            return [model(**k) for k in self._get_endpoint(self._qdb, *args, **kwargs)]
+        return [model(**k) for k in self._get_endpoint(self._qdb, *args, **kwargs)]
 
     def _post_qdb(self, postdata, *args, **params):
         return self._post(postdata, self._qdb, *args, **params)
 
     def post_return_one(self, postdata, model, *args, **kwargs):
         if issubclass(model, ResponseModel):
             return model(**self._post(postdata, self._org, *args, **kwargs))
@@ -81,11 +81,16 @@
         if issubclass(model, ResponseModel):
             return model(**self._post_qdb(postdata, *args, **kwargs))
         else:
             return model(self._post_qdb(postdata, *args, **kwargs))
 
     def post_return_many(self, postdata, model, *args, **kwargs):
         if issubclass(model, ResponseModel):
+            return [model(**k) for k in self._post(postdata, self._org, *args, **kwargs)]
+        else:
+            return [model(k) for k in self._post(postdata, self._org, *args, **kwargs)]
+
+    def qdb_post_return_many(self, postdata, model, *args, **kwargs):
+        if issubclass(model, ResponseModel):
             return [model(**k) for k in self._post_qdb(postdata, *args, **kwargs)]
         else:
             return [model(k) for k in self._post_qdb(postdata, *args, **kwargs)]
-
```

### Comparing `antelope_core-0.2.0/antelope_core/providers/xdb_client/rest_client.py` & `antelope_core-0.2.1/antelope_core/providers/xdb_client/xdb_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,165 +1,162 @@
-import requests
+"""
+Client for the xdb Antelope server
+
+The concept here is to pass received requests straight into the Pydantic models, and then use those for easy
+(though manual) deserialization into EntityRefs.
+"""
+from antelope.models import Context as ContextModel, Entity
+from antelope_core.archives import LcArchive, InterfaceError
+from antelope_core.catalog_query import READONLY_INTERFACE_TYPES
+from antelope_core.contexts import ContextManager, NullContext
+
+from .requester import XdbRequester
+from .implementation import XdbImplementation
+from .xdb_entities import XdbEntity
+
 from requests.exceptions import HTTPError
-import json
-from time import time
-from pydantic import BaseModel
 
 
-class OAuthToken(BaseModel):
-    token_type: str
-    access_token: str
+class XdbTermManager(object):
+    def __init__(self, requester: XdbRequester):
+        """
+        The key question here: should I at least cache remote contexts? for now let us cache nothing
 
-    @property
-    def auth(self):
-        return '%s %s' % (self.token_type, self.access_token)
+        Except we DO need to cache contexts, or at least create them on the fly (and if we are going to create
+        them, we should cache them) because exterior exchanges need to terminate properly in contexts.
 
+        SO: we will establish the condition that Xdb MUST only use contexts' canonical names, thereby escaping the
+        need for synonym disambiguation in the client.
+        :param requester:
+        """
+        self._requester = requester
+        self._cm = ContextManager()
+        self._bad_contexts = set()
+        self._flows = set()
+        self._quantities = set()
 
-class RestClient(object):
-    """
-    A REST client that uses pydantic models to interpret response data
-    """
+    def update_requester(self, requester):
+        self._requester = requester
+
+    @property
+    def is_lcia_engine(self):
+        return self._requester.is_lcia_engine
 
-    auth_route = 'login'
-    _token = None
+    def _fetch_context_model(self, item):
+        return self._requester.get_one(ContextModel, 'contexts', item)
 
-    def _print(self, *args, cont=False):
-        if not self._quiet:
-            if cont:  # continue the same line
-                print(*args, end=".. ")
+    def _build_context(self, context_model, *args):
+        if context_model.name == 'None':
+            c_actual = NullContext  # maintain singleton status of NullContext
+        else:
+            if context_model.parent is None or context_model.parent == '':
+                parent = None
             else:
-                print(*args)
-
-    def __init__(self, api_root, token=None, quiet=False, auth_route=None):
-        self._s = requests.Session()
-        self._s.headers['Accept'] = "application/json"
-        self._quiet = quiet
-        if auth_route:
-            self.auth_route = auth_route
-        if token:
-            self.set_token(token)
-
-        while api_root[-1] == '/':
-            api_root = api_root[:-1]  # strip trailing /
-
-        self._api_root = api_root
-
-    def close(self):
-        self._s.close()
-
-    def set_token(self, token):
-        """
-        we accept:
-        - a string with a plain token
-        - a string with 'token_type token'
-        - an OauthToken
-        :param token:
+                parent = self.get_context(context_model.parent)
+            c_actual = self._cm.new_entry(context_model.name, *args, parent=parent)
+            if parent is not None and parent.sense is None and context_model.sense is not None:
+                c_actual.sense = context_model.sense
+            c_actual.add_origin(self._requester.origin)  # here we are masquerading all origins back to the requester origin
+        return c_actual
+
+    def add_flow(self, flow, **kwargs):
+        self._flows.add(flow)
+
+    def add_quantity(self, quantity):
+        self._quantities.add(quantity)
+
+    def __getitem__(self, item):
+        if isinstance(item, list):
+            item = tuple(item)
+        if item in self._bad_contexts:
+            return None
+        try:
+            return self._cm[item]
+        except KeyError:
+            try:
+                c_model = self._fetch_context_model(item)
+            except HTTPError as e:
+                if e.args[0] == 404:
+                    self._bad_contexts.add(item)
+                    return None
+                else:
+                    raise
+            c_actual = self._build_context(c_model, item)
+            # this escapes the PROTECTED_TERM restrictions- which is OK because our CM is captive
+            self._cm.add_synonym(c_actual.name, item)
+            return c_actual
+
+    def is_context(self, item):
+        """
+        The only place this is used is in collision checking- therefore this only needs to check if the name is
+        known *locally* as a context (why do an http query for literally every new entity?)
+        :param item:
         :return:
         """
-        if isinstance(token, OAuthToken):
-            self._token = token
-        elif isinstance(token, str):
-            toks = token.split(' ')
-            if len(toks) == 1:
-                self._token = OAuthToken(token_type='bearer', access_token=token)
-            elif len(toks) == 2:
-                self._token = OAuthToken(token_type=toks[0], access_token=toks[1])
-            else:
-                raise ValueError('invalid token specification')
-        else:
-            raise ValueError('Invalid token type')
-        self._s.headers['Authorization'] = self._token.auth
+        try:
+            cx = self._cm[item]
+        except KeyError:
+            return False
+        return cx is not None
 
-    def authenticate(self, username, password, **kwargs):
-        """
-        POSTs an OAuth2-compliant form to obtain a bearer token.
-        Be sure to set the 'auth_route' property either in a subclass or manually (e.g. on init)
-        :param username:
-        :param password:
-        :param kwargs:
-        :return:
+    def get_context(self, item):
+        return self.__getitem__(item) or NullContext
+
+    '''
+    def get_canonical(self, item):
         """
-        data = {
-            "grant_type": "password",
-            "username": username,
-            "password": password,
-        }
-        data.update(kwargs)
-        self.set_token(self.post_return_one(data, OAuthToken, self.auth_route, form=True))
-
-    def _request(self, verb, route, **kwargs):
-        """
-        Returns JSON-translated content
-        :param verb:
-        :param route:
-        :param kwargs:
+        again, to avoid premature optimization, the initial policy is no caching anything
+        :param item:
         :return:
         """
-        url = '/'.join([self._api_root, route])
-        endp = {
-            'GET': self._s.get,
-            'PUT': self._s.put,
-            'POST': self._s.post,
-            'PATCH': self._s.patch,
-            'DELETE': self._s.delete
-        }[verb]
-        self._print('%s %s' % (verb, url), cont=True)
-        t = time()
-        resp = endp(url, **kwargs)
-        el = time() - t
-        self._print('%d [%.2f sec]' % (resp.status_code, el))
-        if resp.status_code >= 400:
-            raise HTTPError(resp.status_code, resp.content)
-        return json.loads(resp.content)
-
-    def _get_endpoint(self, route, *args, **params):
-        url = '/'.join([route, *args])
-        return self._request('GET', url, params=params)
-
-    def get_raw(self, *args, **kwargs):
-        return self._get_endpoint(*args, **kwargs)
-
-    def get_one(self, model, *args, **kwargs):
-        if issubclass(model, BaseModel):
-            return model(**self._get_endpoint(*args, **kwargs))
-        else:
-            return model(self._get_endpoint(*args, **kwargs))
+        try:
+            return self._requester.get_one(Entity, 'quantities', item)
+        except HTTPError as e:
+            if e.args[0] == 404:
+                raise EntityNotFound(item)
+            else:
+                raise e
+    '''
 
-    def get_many(self, model, *args, **kwargs):
-        if issubclass(model, BaseModel):
-            return [model(**k) for k in self._get_endpoint(*args, **kwargs)]
-        else:
-            return [model(k) for k in self._get_endpoint(*args, **kwargs)]
+    def synonyms(self, term):
+        return self._requester.get_many(str, 'synonyms', term=term)
 
-    def _post(self, postdata, route, form=False, *args, **params):
-        url = '/'.join([route, *args])
-        if form:
-            return self._request('POST', url, data=postdata, params=params)
-        else:
-            return self._request('POST', url, json=postdata, params=params)
+    def contexts(self, **kwargs):
+        c_models = self._requester.get_many(ContextModel, 'contexts', **kwargs)
+        for c in c_models:
+            if c.name in self._cm:
+                yield self._cm[c.name]
+            else:
+                yield self._build_context(c)
 
-    def post_return_one(self, postdata, model, *args, **kwargs):
-        if issubclass(model, BaseModel):
-            return model(**self._post(postdata, *args, **kwargs))
-        else:
-            return model(self._post(postdata, *args, **kwargs))
 
-    def post_return_many(self, postdata, model, *args, **kwargs):
-        if issubclass(model, BaseModel):
-            return [model(**k) for k in self._post(postdata, *args, **kwargs)]
-        else:
-            return [model(k) for k in self._post(postdata, *args, **kwargs)]
+class XdbClient(LcArchive):
+    """
+    An XdbClient accesses xdb at a named URL using an access token.
+    """
+    def __init__(self, source, ref=None, token=None):
+        self._requester = XdbRequester(source, ref, token=token)
+        if ref is None:
+            ref = 'qdb'
+        super(XdbClient, self).__init__(source, ref=ref, term_manager=XdbTermManager(self._requester))
+
+    def refresh_token(self, new_token):
+        self._requester.set_token(new_token)
+
+    def refresh_auth(self, new_source, new_token):
+        self._requester = XdbRequester(new_source, new_token)
+        self.tm.update_requester(self._requester)
 
-    def put(self, putdata, model, form=False, *args, **kwargs):
-        url = '/'.join(args)
-        if form:
-            response = self._request('PUT', url, data=putdata, params=kwargs)
-        else:
-            response = self._request('PUT', url, json=putdata, params=kwargs)
-        if issubclass(model, BaseModel):
-            return model(**response)
-        else:
-            return model(response)
+    @property
+    def r(self):
+        return self._requester
 
-    def delete(self, *args, **kwargs):
-        url = '/'.join(args)
-        return self._request('DELETE', url, params=kwargs)
+    def make_interface(self, iface):
+        if iface in READONLY_INTERFACE_TYPES:
+            return XdbImplementation(self)
+        raise InterfaceError(iface)
+
+    def _fetch(self, key, **kwargs):
+        ref = self.query.make_ref(XdbEntity(self._requester.get_one(Entity, key), self))
+        if key not in self._entities:
+            self._entities[key] = ref
+        return ref
```

### Comparing `antelope_core-0.2.0/antelope_core/providers/xdb_client/xdb_entities.py` & `antelope_core-0.2.1/antelope_core/providers/xdb_client/xdb_entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from antelope import BaseEntity, CatalogRef
-from antelope_core.models import Entity, FlowEntity, ReferenceExchange
+from antelope.models import Entity, FlowEntity, ReferenceExchange
 
 
 class XdbReferenceRequired(Exception):
     """
     Straight-up entities have no capabilities
     """
     pass
```

### Comparing `antelope_core-0.2.0/antelope_core/providers/xl_dict.py` & `antelope_core-0.2.1/antelope_core/providers/xl_dict.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/providers/xml_widgets.py` & `antelope_core-0.2.1/antelope_core/providers/xml_widgets.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/tests/test_autorange.py` & `antelope_core-0.2.1/antelope_core/tests/test_autorange.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/tests/test_contexts.py` & `antelope_core-0.2.1/antelope_core/tests/test_contexts.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/tests/test_exchanges.py` & `antelope_core-0.2.1/antelope_core/tests/test_exchanges.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core/tests/test_resources.py` & `antelope_core-0.2.1/antelope_core/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `antelope_core-0.2.0/antelope_core.egg-info/PKG-INFO` & `antelope_core-0.2.1/antelope_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antelope-core
-Version: 0.2.0
+Version: 0.2.1
 Home-page: https://github.com/AntelopeLCA/core
 Author: Brandon Kuczenski
 Author-email: bkuczenski@ucsb.edu
 License: BSD 3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `antelope_core-0.2.0/antelope_core.egg-info/SOURCES.txt` & `antelope_core-0.2.1/antelope_core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 antelope_core/__init__.py
-antelope_core/auth.py
 antelope_core/autorange.py
 antelope_core/catalog_query.py
 antelope_core/characterizations.py
 antelope_core/contexts.py
 antelope_core/exchanges.py
 antelope_core/file_accessor.py
 antelope_core/from_json.py
 antelope_core/lc_resource.py
 antelope_core/lcia_results.py
-antelope_core/models.py
 antelope_core.egg-info/PKG-INFO
 antelope_core.egg-info/SOURCES.txt
 antelope_core.egg-info/dependency_links.txt
 antelope_core.egg-info/requires.txt
 antelope_core.egg-info/top_level.txt
 antelope_core/archives/__init__.py
 antelope_core/archives/archive_index.py
```

### Comparing `antelope_core-0.2.0/setup.py` & `antelope_core-0.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.0'
+VERSION = '0.2.1'
 
 requires = [
     "synonym_dict>=0.2.0",
-    "antelope_interface>=0.2.0",
-    "xlstools>=0.1.0",
+    "antelope_interface>=0.2.1",
+    "xlstools>=0.1.3",
     "python-magic>=0.4.18",
     "requests>=2.25",
     "pydantic>=1.8.2"
 ]
 
 # optional: pylzma
 """
 Version History
+0.2.1   2023-04-10 - xdb passes benchmarks
+                     pydantic models moved into interface
+                     sys_lci and bg_lcia operational, both locally and remotely
+
 0.2.0   2023-04-07 - "release" virtualize branch. 
                    - Add pydantic models for everything
                    - add an XDB client implementation for remote operation
                    - job-related changes to entity handling throughout
 
 0.1.8   2022-04-08 - PyPI release to roll up a few small changes:
  * upgrade ecoinvent_lcia to use xlstools; port 3.8
```

