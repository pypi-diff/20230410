# Comparing `tmp/mothertongues-0.18.20220503.tar.gz` & `tmp/mothertongues-0.18.20230410.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mothertongues-0.18.20220503.tar", last modified: Tue May  3 21:33:05 2022, max compression
+gzip compressed data, was "mothertongues-0.18.20230410.tar", last modified: Mon Apr 10 20:00:44 2023, max compression
```

## Comparing `mothertongues-0.18.20220503.tar` & `mothertongues-0.18.20230410.tar`

### file list

```diff
@@ -1,196 +1,186 @@
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.643990 mothertongues-0.18.20220503/
--rw-r--r--   0 pinea      (502) staff       (20)      392 2019-09-02 21:21:44.000000 mothertongues-0.18.20220503/MANIFEST.in
--rw-r--r--   0 pinea      (502) staff       (20)     5827 2022-05-03 21:33:05.643677 mothertongues-0.18.20220503/PKG-INFO
--rw-r--r--   0 pinea      (502) staff       (20)     4835 2020-07-28 21:03:13.000000 mothertongues-0.18.20220503/README.md
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.523356 mothertongues-0.18.20220503/mothertongues.egg-info/
--rw-r--r--   0 pinea      (502) staff       (20)     5827 2022-05-03 21:33:05.000000 mothertongues-0.18.20220503/mothertongues.egg-info/PKG-INFO
--rw-r--r--   0 pinea      (502) staff       (20)     5620 2022-05-03 21:33:05.000000 mothertongues-0.18.20220503/mothertongues.egg-info/SOURCES.txt
--rw-r--r--   0 pinea      (502) staff       (20)        1 2022-05-03 21:33:05.000000 mothertongues-0.18.20220503/mothertongues.egg-info/dependency_links.txt
--rw-r--r--   0 pinea      (502) staff       (20)       89 2022-05-03 21:33:05.000000 mothertongues-0.18.20220503/mothertongues.egg-info/entry_points.txt
--rw-r--r--   0 pinea      (502) staff       (20)        1 2018-10-22 01:45:21.000000 mothertongues-0.18.20220503/mothertongues.egg-info/not-zip-safe
--rw-r--r--   0 pinea      (502) staff       (20)      189 2022-05-03 21:33:05.000000 mothertongues-0.18.20220503/mothertongues.egg-info/requires.txt
--rw-r--r--   0 pinea      (502) staff       (20)        4 2022-05-03 21:33:05.000000 mothertongues-0.18.20220503/mothertongues.egg-info/top_level.txt
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.529945 mothertongues-0.18.20220503/mtd/
--rw-r--r--   0 pinea      (502) staff       (20)     1113 2020-04-11 22:02:05.000000 mothertongues-0.18.20220503/mtd/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)       79 2018-10-18 16:51:39.000000 mothertongues-0.18.20220503/mtd/app.py
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.532506 mothertongues-0.18.20220503/mtd/buildtools/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2018-10-18 16:51:09.000000 mothertongues-0.18.20220503/mtd/buildtools/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)     2121 2018-10-24 23:04:11.000000 mothertongues-0.18.20220503/mtd/buildtools/swagger-pre.json
--rw-r--r--   0 pinea      (502) staff       (20)     1555 2018-10-22 03:17:53.000000 mothertongues-0.18.20220503/mtd/buildtools/swagger.json
--rw-r--r--   0 pinea      (502) staff       (20)     2151 2019-01-01 22:26:13.000000 mothertongues-0.18.20220503/mtd/buildtools/write_static.py
--rw-r--r--   0 pinea      (502) staff       (20)    13677 2022-04-02 22:37:16.000000 mothertongues-0.18.20220503/mtd/cli.py
--rw-r--r--   0 pinea      (502) staff       (20)     9751 2022-04-02 22:36:25.000000 mothertongues-0.18.20220503/mtd/dictionary.py
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.532993 mothertongues-0.18.20220503/mtd/exceptions/
--rw-r--r--   0 pinea      (502) staff       (20)     3900 2019-02-01 23:13:23.000000 mothertongues-0.18.20220503/mtd/exceptions/__init__.py
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.534836 mothertongues-0.18.20220503/mtd/languages/
--rw-r--r--   0 pinea      (502) staff       (20)     4206 2022-04-28 23:40:58.000000 mothertongues-0.18.20220503/mtd/languages/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)     2647 2019-10-25 00:07:21.000000 mothertongues-0.18.20220503/mtd/languages/config_schema.json
--rw-r--r--   0 pinea      (502) staff       (20)     6106 2019-08-16 22:04:46.000000 mothertongues-0.18.20220503/mtd/languages/manifest_schema.json
--rw-r--r--   0 pinea      (502) staff       (20)     1044 2020-02-15 18:36:43.000000 mothertongues-0.18.20220503/mtd/languages/suites.py
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.541267 mothertongues-0.18.20220503/mtd/parsers/
--rw-r--r--   0 pinea      (502) staff       (20)     2089 2020-02-15 18:44:30.000000 mothertongues-0.18.20220503/mtd/parsers/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)     1564 2019-09-02 21:07:14.000000 mothertongues-0.18.20220503/mtd/parsers/csv_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)      917 2019-09-02 21:07:03.000000 mothertongues-0.18.20220503/mtd/parsers/dict_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     2011 2019-09-02 21:06:52.000000 mothertongues-0.18.20220503/mtd/parsers/gsheet_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     6481 2020-06-14 19:36:35.000000 mothertongues-0.18.20220503/mtd/parsers/json_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     1329 2019-08-16 21:01:28.000000 mothertongues-0.18.20220503/mtd/parsers/pkl_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     1623 2019-09-02 21:07:38.000000 mothertongues-0.18.20220503/mtd/parsers/psv_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     1654 2019-09-17 03:43:33.000000 mothertongues-0.18.20220503/mtd/parsers/request_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     1610 2019-09-02 21:07:52.000000 mothertongues-0.18.20220503/mtd/parsers/tsv_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     7676 2022-04-28 23:41:31.000000 mothertongues-0.18.20220503/mtd/parsers/utils.py
--rw-r--r--   0 pinea      (502) staff       (20)     2993 2019-10-04 03:51:24.000000 mothertongues-0.18.20220503/mtd/parsers/xlsx_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     4675 2019-09-02 21:08:29.000000 mothertongues-0.18.20220503/mtd/parsers/xml_parser.py
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.543440 mothertongues-0.18.20220503/mtd/processors/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2018-09-22 03:18:01.000000 mothertongues-0.18.20220503/mtd/processors/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)     2366 2020-03-03 01:21:41.000000 mothertongues-0.18.20220503/mtd/processors/sorter.py
--rw-r--r--   0 pinea      (502) staff       (20)    13166 2022-04-02 22:59:06.000000 mothertongues-0.18.20220503/mtd/processors/transducer.py
--rw-r--r--   0 pinea      (502) staff       (20)     2085 2020-02-24 22:56:40.000000 mothertongues-0.18.20220503/mtd/processors/validator.py
--rw-r--r--   0 pinea      (502) staff       (20)     2754 2021-05-27 13:25:57.000000 mothertongues-0.18.20220503/mtd/resources.py
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.545912 mothertongues-0.18.20220503/mtd/static/
--rw-r--r--   0 pinea      (502) staff       (20)     6148 2020-07-11 23:08:12.000000 mothertongues-0.18.20220503/mtd/static/.DS_Store
--rw-r--r--   0 pinea      (502) staff       (20)      332 2019-03-13 05:12:46.000000 mothertongues-0.18.20220503/mtd/static/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)     1270 2022-04-02 23:28:56.000000 mothertongues-0.18.20220503/mtd/static/active.sites.json
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.547275 mothertongues-0.18.20220503/mtd/static/assets/
--rw-r--r--   0 pinea      (502) staff       (20)     6148 2019-09-02 21:17:33.000000 mothertongues-0.18.20220503/mtd/static/assets/.DS_Store
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.549065 mothertongues-0.18.20220503/mtd/static/assets/icon/
--rw-r--r--   0 pinea      (502) staff       (20)     1981 2018-10-19 05:49:00.000000 mothertongues-0.18.20220503/mtd/static/assets/icon/favicon.ico
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.555345 mothertongues-0.18.20220503/mtd/static/assets/js/
--rw-r--r--   0 pinea      (502) staff       (20)     6148 2020-07-11 23:08:21.000000 mothertongues-0.18.20220503/mtd/static/assets/js/.DS_Store
--rw-r--r--   0 pinea      (502) staff       (20)      293 2022-04-02 23:28:56.000000 mothertongues-0.18.20220503/mtd/static/assets/js/config-danish.js
--rw-r--r--   0 pinea      (502) staff       (20)     1500 2020-04-21 08:02:31.000000 mothertongues-0.18.20220503/mtd/static/assets/js/config-h-nq-min-m.js
--rw-r--r--   0 pinea      (502) staff       (20)      388 2022-04-02 23:28:56.000000 mothertongues-0.18.20220503/mtd/static/assets/js/config-test.js
--rw-r--r--   0 pinea      (502) staff       (20)     1195 2022-04-02 23:28:56.000000 mothertongues-0.18.20220503/mtd/static/assets/js/dict_cached-danish.js
--rw-r--r--   0 pinea      (502) staff       (20)   230715 2020-04-21 08:02:31.000000 mothertongues-0.18.20220503/mtd/static/assets/js/dict_cached-h-nq-min-m.js
--rw-r--r--   0 pinea      (502) staff       (20)      129 2022-04-02 23:28:56.000000 mothertongues-0.18.20220503/mtd/static/assets/js/dict_cached-test.js
--rw-r--r--   0 pinea      (502) staff       (20)      266 2018-09-05 18:51:29.000000 mothertongues-0.18.20220503/mtd/static/assets/manifest.json
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.557434 mothertongues-0.18.20220503/mtd/static/css/
--rw-r--r--   0 pinea      (502) staff       (20)     4049 2020-07-27 03:51:38.000000 mothertongues-0.18.20220503/mtd/static/css/custom.css
--rw-r--r--   0 pinea      (502) staff       (20)     7797 2018-10-19 05:49:00.000000 mothertongues-0.18.20220503/mtd/static/css/normalize.css
--rw-r--r--   0 pinea      (502) staff       (20)    11452 2018-10-19 05:49:00.000000 mothertongues-0.18.20220503/mtd/static/css/skeleton.css
--rw-r--r--   0 pinea      (502) staff       (20)      266 2018-10-19 05:49:00.000000 mothertongues-0.18.20220503/mtd/static/manifest.json
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.573866 mothertongues-0.18.20220503/mtd/static/swagger-ui/
--rw-r--r--   0 pinea      (502) staff       (20)      445 2018-08-29 22:23:22.000000 mothertongues-0.18.20220503/mtd/static/swagger-ui/favicon-16x16.png
--rw-r--r--   0 pinea      (502) staff       (20)     1141 2018-08-29 22:23:22.000000 mothertongues-0.18.20220503/mtd/static/swagger-ui/favicon-32x32.png
--rw-r--r--   0 pinea      (502) staff       (20)  1547890 2018-08-29 22:23:22.000000 mothertongues-0.18.20220503/mtd/static/swagger-ui/swagger-ui-bundle.js
--rw-r--r--   0 pinea      (502) staff       (20)   475131 2018-08-29 22:23:22.000000 mothertongues-0.18.20220503/mtd/static/swagger-ui/swagger-ui-standalone-preset.js
--rw-r--r--   0 pinea      (502) staff       (20)   153816 2018-08-29 22:23:22.000000 mothertongues-0.18.20220503/mtd/static/swagger-ui/swagger-ui.css
--rw-r--r--   0 pinea      (502) staff       (20)     1455 2022-04-02 23:28:56.000000 mothertongues-0.18.20220503/mtd/static/swagger.json
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.582319 mothertongues-0.18.20220503/mtd/templates/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2018-10-18 17:28:24.000000 mothertongues-0.18.20220503/mtd/templates/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)     1524 2018-10-22 03:25:21.000000 mothertongues-0.18.20220503/mtd/templates/apidocs.html
--rw-r--r--   0 pinea      (502) staff       (20)     2097 2020-07-27 03:34:32.000000 mothertongues-0.18.20220503/mtd/templates/dictionary.html
--rw-r--r--   0 pinea      (502) staff       (20)     3795 2020-07-27 03:44:13.000000 mothertongues-0.18.20220503/mtd/templates/index.html
--rw-r--r--   0 pinea      (502) staff       (20)   100235 2019-01-12 23:40:47.000000 mothertongues-0.18.20220503/mtd/templates/stats.html
--rw-r--r--   0 pinea      (502) staff       (20)     9074 2018-12-13 20:01:42.000000 mothertongues-0.18.20220503/mtd/templates/validator.html
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.602656 mothertongues-0.18.20220503/mtd/tests/
--rw-r--r--   0 pinea      (502) staff       (20)     4548 2019-02-02 01:33:21.000000 mothertongues-0.18.20220503/mtd/tests/__init__.py
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.605487 mothertongues-0.18.20220503/mtd/tests/integration/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2019-09-17 03:18:37.000000 mothertongues-0.18.20220503/mtd/tests/integration/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)      764 2022-04-02 23:07:08.000000 mothertongues-0.18.20220503/mtd/tests/integration/config_test.json
--rw-r--r--   0 pinea      (502) staff       (20)     3535 2019-09-17 03:17:42.000000 mothertongues-0.18.20220503/mtd/tests/integration/test_api_resources.py
--rw-r--r--   0 pinea      (502) staff       (20)     2551 2019-09-17 03:52:16.000000 mothertongues-0.18.20220503/mtd/tests/integration/test_basic_integration.py
--rw-r--r--   0 pinea      (502) staff       (20)     3515 2019-01-10 01:43:46.000000 mothertongues-0.18.20220503/mtd/tests/integration/test_cli.py
--rw-r--r--   0 pinea      (502) staff       (20)      132 2019-09-17 03:16:43.000000 mothertongues-0.18.20220503/mtd/tests/integration/test_swagger_integration.py
--rw-r--r--   0 pinea      (502) staff       (20)      465 2020-04-11 19:01:54.000000 mothertongues-0.18.20220503/mtd/tests/log.py
--rw-r--r--   0 pinea      (502) staff       (20)     2795 2019-09-17 03:01:54.000000 mothertongues-0.18.20220503/mtd/tests/run.py
--rw-r--r--   0 pinea      (502) staff       (20)     4691 2022-04-02 23:20:17.000000 mothertongues-0.18.20220503/mtd/tests/test_cli.py
--rw-r--r--   0 pinea      (502) staff       (20)     1053 2020-07-12 01:20:42.000000 mothertongues-0.18.20220503/mtd/tests/test_csv_parser.py
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.606896 mothertongues-0.18.20220503/mtd/tests/test_data/
--rw-r--r--   0 pinea      (502) staff       (20)     8196 2019-09-02 21:18:26.000000 mothertongues-0.18.20220503/mtd/tests/test_data/.DS_Store
--rw-r--r--   0 pinea      (502) staff       (20)        0 2018-09-23 03:26:06.000000 mothertongues-0.18.20220503/mtd/tests/test_data/__init__.py
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.608945 mothertongues-0.18.20220503/mtd/tests/test_data/csv/
--rw-r--r--   0 pinea      (502) staff       (20)     6148 2019-01-05 18:19:30.000000 mothertongues-0.18.20220503/mtd/tests/test_data/csv/.DS_Store
--rw-r--r--   0 pinea      (502) staff       (20)        0 2019-01-05 18:37:08.000000 mothertongues-0.18.20220503/mtd/tests/test_data/csv/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)     1244 2019-12-14 18:55:28.000000 mothertongues-0.18.20220503/mtd/tests/test_data/csv/data.csv
--rw-r--r--   0 pinea      (502) staff       (20)     2190 2019-01-07 20:51:43.000000 mothertongues-0.18.20220503/mtd/tests/test_data/csv/manifest.json
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.612769 mothertongues-0.18.20220503/mtd/tests/test_data/json/
--rw-r--r--   0 pinea      (502) staff       (20)     6148 2019-09-02 21:17:27.000000 mothertongues-0.18.20220503/mtd/tests/test_data/json/.DS_Store
--rw-r--r--   0 pinea      (502) staff       (20)        0 2018-09-23 03:59:22.000000 mothertongues-0.18.20220503/mtd/tests/test_data/json/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)       54 2018-09-23 03:27:39.000000 mothertongues-0.18.20220503/mtd/tests/test_data/json/bad.json
--rw-r--r--   0 pinea      (502) staff       (20)     2687 2019-01-07 01:41:22.000000 mothertongues-0.18.20220503/mtd/tests/test_data/json/data.json
--rw-r--r--   0 pinea      (502) staff       (20)     1363 2019-01-07 02:11:15.000000 mothertongues-0.18.20220503/mtd/tests/test_data/json/data_reduced.json
--rw-r--r--   0 pinea      (502) staff       (20)     1766 2019-01-08 18:10:06.000000 mothertongues-0.18.20220503/mtd/tests/test_data/json/dict_manifest.json
--rw-r--r--   0 pinea      (502) staff       (20)     1798 2019-01-07 20:33:34.000000 mothertongues-0.18.20220503/mtd/tests/test_data/json/manifest.json
--rw-r--r--   0 pinea      (502) staff       (20)       39 2018-09-23 03:28:31.000000 mothertongues-0.18.20220503/mtd/tests/test_data/json/missing.json
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.614234 mothertongues-0.18.20220503/mtd/tests/test_data/pkl/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2019-08-16 21:02:59.000000 mothertongues-0.18.20220503/mtd/tests/test_data/pkl/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)     1185 2019-08-16 21:06:33.000000 mothertongues-0.18.20220503/mtd/tests/test_data/pkl/data.pkl
--rw-r--r--   0 pinea      (502) staff       (20)     1798 2019-08-16 21:03:55.000000 mothertongues-0.18.20220503/mtd/tests/test_data/pkl/manifest.json
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.615914 mothertongues-0.18.20220503/mtd/tests/test_data/psv/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2019-01-05 18:37:22.000000 mothertongues-0.18.20220503/mtd/tests/test_data/psv/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)     1244 2019-01-05 18:54:59.000000 mothertongues-0.18.20220503/mtd/tests/test_data/psv/data.psv
--rw-r--r--   0 pinea      (502) staff       (20)     2190 2019-01-07 20:51:28.000000 mothertongues-0.18.20220503/mtd/tests/test_data/psv/manifest.json
--rw-r--r--   0 pinea      (502) staff       (20)        0 2020-02-24 02:54:26.000000 mothertongues-0.18.20220503/mtd/tests/test_data/test.log
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.618688 mothertongues-0.18.20220503/mtd/tests/test_data/test_dictionary/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2019-01-10 00:14:45.000000 mothertongues-0.18.20220503/mtd/tests/test_data/test_dictionary/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)      488 2022-04-02 23:31:51.000000 mothertongues-0.18.20220503/mtd/tests/test_data/test_dictionary/config_0.json
--rw-r--r--   0 pinea      (502) staff       (20)      488 2022-04-02 23:31:51.000000 mothertongues-0.18.20220503/mtd/tests/test_data/test_dictionary/config_1.json
--rw-r--r--   0 pinea      (502) staff       (20)      398 2019-03-13 04:59:15.000000 mothertongues-0.18.20220503/mtd/tests/test_data/test_dictionary/config_2_minimal.json
--rw-r--r--   0 pinea      (502) staff       (20)      153 2022-04-02 23:31:51.000000 mothertongues-0.18.20220503/mtd/tests/test_data/test_dictionary/dictionaries.txt
--rw-r--r--   0 pinea      (502) staff       (20)        0 2020-02-24 02:54:46.000000 mothertongues-0.18.20220503/mtd/tests/test_data/test_dictionary/test.log
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.624386 mothertongues-0.18.20220503/mtd/tests/test_data/transducers/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2019-01-08 23:43:24.000000 mothertongues-0.18.20220503/mtd/tests/test_data/transducers/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)       40 2019-11-02 18:07:53.000000 mothertongues-0.18.20220503/mtd/tests/test_data/transducers/test_composite.json
--rw-r--r--   0 pinea      (502) staff       (20)       71 2020-02-24 00:30:03.000000 mothertongues-0.18.20220503/mtd/tests/test_data/transducers/test_counter_feeding.yaml
--rw-r--r--   0 pinea      (502) staff       (20)        7 2019-01-09 05:48:52.000000 mothertongues-0.18.20220503/mtd/tests/test_data/transducers/test_feeding.csv
--rw-r--r--   0 pinea      (502) staff       (20)        7 2019-02-08 04:41:06.000000 mothertongues-0.18.20220503/mtd/tests/test_data/transducers/test_intermediate_transducer.csv
--rw-r--r--   0 pinea      (502) staff       (20)        8 2019-01-09 00:07:10.000000 mothertongues-0.18.20220503/mtd/tests/test_data/transducers/test_length_transducer.csv
--rw-r--r--   0 pinea      (502) staff       (20)       95 2020-02-24 00:40:06.000000 mothertongues-0.18.20220503/mtd/tests/test_data/transducers/test_length_transducer.yaml
--rw-r--r--   0 pinea      (502) staff       (20)        3 2019-01-08 23:42:54.000000 mothertongues-0.18.20220503/mtd/tests/test_data/transducers/test_transducer.csv
--rw-r--r--   0 pinea      (502) staff       (20)       53 2020-02-24 00:19:43.000000 mothertongues-0.18.20220503/mtd/tests/test_data/transducers/test_transducer.json
--rw-r--r--   0 pinea      (502) staff       (20)       53 2020-04-11 18:31:40.000000 mothertongues-0.18.20220503/mtd/tests/test_data/transducers/test_transducer.yaml
--rw-r--r--   0 pinea      (502) staff       (20)        4 2019-01-09 00:29:53.000000 mothertongues-0.18.20220503/mtd/tests/test_data/transducers/test_transducer_2.csv
--rw-r--r--   0 pinea      (502) staff       (20)       54 2020-04-11 18:32:02.000000 mothertongues-0.18.20220503/mtd/tests/test_data/transducers/test_transducer_2.yaml
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.626341 mothertongues-0.18.20220503/mtd/tests/test_data/tsv/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2019-01-05 18:37:29.000000 mothertongues-0.18.20220503/mtd/tests/test_data/tsv/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)     1244 2019-01-05 18:56:22.000000 mothertongues-0.18.20220503/mtd/tests/test_data/tsv/data.tsv
--rw-r--r--   0 pinea      (502) staff       (20)     2190 2019-01-07 20:51:17.000000 mothertongues-0.18.20220503/mtd/tests/test_data/tsv/manifest.json
--rw-r--r--   0 pinea      (502) staff       (20)     1812 2019-03-05 23:52:45.000000 mothertongues-0.18.20220503/mtd/tests/test_data/whitespace_manifest.json
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.632925 mothertongues-0.18.20220503/mtd/tests/test_data/xlsx/
--rw-r--r--   0 pinea      (502) staff       (20)     6148 2019-02-08 04:59:54.000000 mothertongues-0.18.20220503/mtd/tests/test_data/xlsx/.DS_Store
--rw-r--r--   0 pinea      (502) staff       (20)        0 2019-01-05 18:37:32.000000 mothertongues-0.18.20220503/mtd/tests/test_data/xlsx/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)     4473 2019-02-01 20:46:29.000000 mothertongues-0.18.20220503/mtd/tests/test_data/xlsx/data.xlsx
--rw-r--r--   0 pinea      (502) staff       (20)     2199 2019-01-07 20:52:27.000000 mothertongues-0.18.20220503/mtd/tests/test_data/xlsx/manifest.json
--rw-r--r--   0 pinea      (502) staff       (20)     2199 2019-02-01 20:44:49.000000 mothertongues-0.18.20220503/mtd/tests/test_data/xlsx/manifest.xlsx
--rw-r--r--   0 pinea      (502) staff       (20)     2151 2019-02-01 20:57:18.000000 mothertongues-0.18.20220503/mtd/tests/test_data/xlsx/manifest_alternate.json
--rw-r--r--   0 pinea      (502) staff       (20)     7324 2019-02-08 04:29:14.000000 mothertongues-0.18.20220503/mtd/tests/test_data/xlsx/missing_sheet_data.xlsx
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.635292 mothertongues-0.18.20220503/mtd/tests/test_data/xml/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2019-01-05 18:37:35.000000 mothertongues-0.18.20220503/mtd/tests/test_data/xml/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)    10291 2019-01-06 18:55:29.000000 mothertongues-0.18.20220503/mtd/tests/test_data/xml/data.xml
--rw-r--r--   0 pinea      (502) staff       (20)     9274 2019-01-06 18:56:25.000000 mothertongues-0.18.20220503/mtd/tests/test_data/xml/data_reduced.xml
--rw-r--r--   0 pinea      (502) staff       (20)     1901 2019-01-07 20:46:57.000000 mothertongues-0.18.20220503/mtd/tests/test_data/xml/manifest.json
--rw-r--r--   0 pinea      (502) staff       (20)     1108 2019-03-11 22:05:57.000000 mothertongues-0.18.20220503/mtd/tests/test_data_configuration_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     1693 2020-07-12 01:23:19.000000 mothertongues-0.18.20220503/mtd/tests/test_dict_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     2292 2019-03-13 05:09:30.000000 mothertongues-0.18.20220503/mtd/tests/test_dictionary.py
--rw-r--r--   0 pinea      (502) staff       (20)        0 2019-01-05 19:02:47.000000 mothertongues-0.18.20220503/mtd/tests/test_formatted_export.py
--rw-r--r--   0 pinea      (502) staff       (20)     1643 2020-07-12 01:23:42.000000 mothertongues-0.18.20220503/mtd/tests/test_json_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     1069 2020-07-12 01:22:27.000000 mothertongues-0.18.20220503/mtd/tests/test_pkl_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     1008 2020-07-12 01:22:24.000000 mothertongues-0.18.20220503/mtd/tests/test_psv_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)        0 2019-01-05 19:02:57.000000 mothertongues-0.18.20220503/mtd/tests/test_raw_export.py
--rw-r--r--   0 pinea      (502) staff       (20)     3682 2020-07-12 01:23:55.000000 mothertongues-0.18.20220503/mtd/tests/test_request_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     2702 2019-01-07 21:39:55.000000 mothertongues-0.18.20220503/mtd/tests/test_sorter.py
--rw-r--r--   0 pinea      (502) staff       (20)        0 2019-01-05 19:02:24.000000 mothertongues-0.18.20220503/mtd/tests/test_swagger_spec.py
--rw-r--r--   0 pinea      (502) staff       (20)     9180 2020-04-11 18:51:02.000000 mothertongues-0.18.20220503/mtd/tests/test_transducer.py
--rw-r--r--   0 pinea      (502) staff       (20)     1008 2020-07-12 01:22:18.000000 mothertongues-0.18.20220503/mtd/tests/test_tsv_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)      992 2020-02-23 23:13:47.000000 mothertongues-0.18.20220503/mtd/tests/test_validator.py
--rw-r--r--   0 pinea      (502) staff       (20)     2115 2020-07-12 01:22:08.000000 mothertongues-0.18.20220503/mtd/tests/test_xlsx_parser.py
--rw-r--r--   0 pinea      (502) staff       (20)     1298 2020-07-12 01:21:41.000000 mothertongues-0.18.20220503/mtd/tests/test_xml_parser.py
-drwxr-xr-x   0 pinea      (502) staff       (20)        0 2022-05-03 21:33:05.643057 mothertongues-0.18.20220503/mtd/transducers/
--rw-r--r--   0 pinea      (502) staff       (20)        0 2018-10-11 04:28:00.000000 mothertongues-0.18.20220503/mtd/transducers/__init__.py
--rw-r--r--   0 pinea      (502) staff       (20)      183 2020-02-24 01:57:42.000000 mothertongues-0.18.20220503/mtd/transducers/circumflex_norm.csv
--rw-r--r--   0 pinea      (502) staff       (20)       36 2019-01-02 00:34:27.000000 mothertongues-0.18.20220503/mtd/transducers/combining_comma.csv
--rw-r--r--   0 pinea      (502) staff       (20)       42 2019-01-02 00:34:27.000000 mothertongues-0.18.20220503/mtd/transducers/combining_norm.csv
--rw-r--r--   0 pinea      (502) staff       (20)      941 2020-02-24 22:31:40.000000 mothertongues-0.18.20220503/mtd/transducers/config.yaml
--rw-r--r--   0 pinea      (502) staff       (20)        6 2019-01-02 00:34:27.000000 mothertongues-0.18.20220503/mtd/transducers/digraph_norm.csv
--rw-r--r--   0 pinea      (502) staff       (20)       55 2020-03-26 02:14:20.000000 mothertongues-0.18.20220503/mtd/transducers/dot_below_norm.csv
--rw-r--r--   0 pinea      (502) staff       (20)       87 2020-03-26 02:14:28.000000 mothertongues-0.18.20220503/mtd/transducers/hacek_norm.csv
--rw-r--r--   0 pinea      (502) staff       (20)       64 2019-01-02 00:34:27.000000 mothertongues-0.18.20220503/mtd/transducers/macron_lowline_norm.csv
--rw-r--r--   0 pinea      (502) staff       (20)       40 2020-03-26 02:18:04.000000 mothertongues-0.18.20220503/mtd/transducers/norm.csv
--rw-r--r--   0 pinea      (502) staff       (20)        5 2020-03-26 02:14:38.000000 mothertongues-0.18.20220503/mtd/transducers/slurpy_norm.csv
--rw-r--r--   0 pinea      (502) staff       (20)        6 2019-01-02 00:34:27.000000 mothertongues-0.18.20220503/mtd/transducers/slurpy_to_line_norm.csv
--rw-r--r--   0 pinea      (502) staff       (20)      115 2019-01-02 00:34:27.000000 mothertongues-0.18.20220503/mtd/transducers/underline_norm.csv
--rw-r--r--   0 pinea      (502) staff       (20)       29 2022-05-03 21:33:05.000000 mothertongues-0.18.20220503/mtd/version.py
--rw-r--r--   0 pinea      (502) staff       (20)     2556 2019-07-31 21:49:13.000000 mothertongues-0.18.20220503/mtd/views.py
--rw-r--r--   0 pinea      (502) staff       (20)      189 2021-12-01 06:24:52.000000 mothertongues-0.18.20220503/requirements.txt
--rw-r--r--   0 pinea      (502) staff       (20)       38 2022-05-03 21:33:05.644092 mothertongues-0.18.20220503/setup.cfg
--rw-r--r--   0 pinea      (502) staff       (20)     1214 2019-10-04 04:03:21.000000 mothertongues-0.18.20220503/setup.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.272616 mothertongues-0.18.20230410/
+-rw-r--r--   0 pinea      (502) staff       (20)    34523 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/LICENSE
+-rw-r--r--   0 pinea      (502) staff       (20)      392 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/MANIFEST.in
+-rw-r--r--   0 pinea      (502) staff       (20)     5178 2023-04-10 20:00:44.272427 mothertongues-0.18.20230410/PKG-INFO
+-rw-r--r--   0 pinea      (502) staff       (20)     4835 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/README.md
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.241843 mothertongues-0.18.20230410/mothertongues.egg-info/
+-rw-r--r--   0 pinea      (502) staff       (20)     5178 2023-04-10 20:00:44.000000 mothertongues-0.18.20230410/mothertongues.egg-info/PKG-INFO
+-rw-r--r--   0 pinea      (502) staff       (20)     5248 2023-04-10 20:00:44.000000 mothertongues-0.18.20230410/mothertongues.egg-info/SOURCES.txt
+-rw-r--r--   0 pinea      (502) staff       (20)        1 2023-04-10 20:00:44.000000 mothertongues-0.18.20230410/mothertongues.egg-info/dependency_links.txt
+-rw-r--r--   0 pinea      (502) staff       (20)       64 2023-04-10 20:00:44.000000 mothertongues-0.18.20230410/mothertongues.egg-info/entry_points.txt
+-rw-r--r--   0 pinea      (502) staff       (20)        1 2023-03-10 00:49:13.000000 mothertongues-0.18.20230410/mothertongues.egg-info/not-zip-safe
+-rw-r--r--   0 pinea      (502) staff       (20)      205 2023-04-10 20:00:44.000000 mothertongues-0.18.20230410/mothertongues.egg-info/requires.txt
+-rw-r--r--   0 pinea      (502) staff       (20)        4 2023-04-10 20:00:44.000000 mothertongues-0.18.20230410/mothertongues.egg-info/top_level.txt
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.243375 mothertongues-0.18.20230410/mtd/
+-rw-r--r--   0 pinea      (502) staff       (20)     1113 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)       79 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/app.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.244226 mothertongues-0.18.20230410/mtd/buildtools/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/buildtools/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2121 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/buildtools/swagger-pre.json
+-rw-r--r--   0 pinea      (502) staff       (20)     1555 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/buildtools/swagger.json
+-rw-r--r--   0 pinea      (502) staff       (20)     2151 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/buildtools/write_static.py
+-rw-r--r--   0 pinea      (502) staff       (20)    13677 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/cli.py
+-rw-r--r--   0 pinea      (502) staff       (20)     9751 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/dictionary.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.244430 mothertongues-0.18.20230410/mtd/exceptions/
+-rw-r--r--   0 pinea      (502) staff       (20)     3900 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/exceptions/__init__.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.245059 mothertongues-0.18.20230410/mtd/languages/
+-rw-r--r--   0 pinea      (502) staff       (20)     4206 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/languages/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2647 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/languages/config_schema.json
+-rw-r--r--   0 pinea      (502) staff       (20)     6106 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/languages/manifest_schema.json
+-rw-r--r--   0 pinea      (502) staff       (20)     1044 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/languages/suites.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.247450 mothertongues-0.18.20230410/mtd/parsers/
+-rw-r--r--   0 pinea      (502) staff       (20)     2089 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/parsers/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1564 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/parsers/csv_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)      917 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/parsers/dict_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2011 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/parsers/gsheet_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     6481 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/parsers/json_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1329 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/parsers/pkl_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1623 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/parsers/psv_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1654 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/parsers/request_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1610 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/parsers/tsv_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     7676 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/parsers/utils.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2993 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/parsers/xlsx_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     4675 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/parsers/xml_parser.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.248037 mothertongues-0.18.20230410/mtd/processors/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/processors/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2366 2023-04-10 19:59:43.000000 mothertongues-0.18.20230410/mtd/processors/sorter.py
+-rw-r--r--   0 pinea      (502) staff       (20)    13166 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/processors/transducer.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2085 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/processors/validator.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2754 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/resources.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.248661 mothertongues-0.18.20230410/mtd/static/
+-rw-r--r--   0 pinea      (502) staff       (20)      332 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1270 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/active.sites.json
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.248906 mothertongues-0.18.20230410/mtd/static/assets/
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.249077 mothertongues-0.18.20230410/mtd/static/assets/icon/
+-rw-r--r--   0 pinea      (502) staff       (20)     1981 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/assets/icon/favicon.ico
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.249415 mothertongues-0.18.20230410/mtd/static/assets/js/
+-rw-r--r--   0 pinea      (502) staff       (20)      293 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/assets/js/config-danish.js
+-rw-r--r--   0 pinea      (502) staff       (20)     1195 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/assets/js/dict_cached-danish.js
+-rw-r--r--   0 pinea      (502) staff       (20)      266 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/assets/manifest.json
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.249975 mothertongues-0.18.20230410/mtd/static/css/
+-rw-r--r--   0 pinea      (502) staff       (20)     4049 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/css/custom.css
+-rw-r--r--   0 pinea      (502) staff       (20)     7797 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/css/normalize.css
+-rw-r--r--   0 pinea      (502) staff       (20)    11452 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/css/skeleton.css
+-rw-r--r--   0 pinea      (502) staff       (20)      266 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/manifest.json
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.254371 mothertongues-0.18.20230410/mtd/static/swagger-ui/
+-rw-r--r--   0 pinea      (502) staff       (20)      445 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/swagger-ui/favicon-16x16.png
+-rw-r--r--   0 pinea      (502) staff       (20)     1141 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/swagger-ui/favicon-32x32.png
+-rw-r--r--   0 pinea      (502) staff       (20)  1547890 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/swagger-ui/swagger-ui-bundle.js
+-rw-r--r--   0 pinea      (502) staff       (20)   475131 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/swagger-ui/swagger-ui-standalone-preset.js
+-rw-r--r--   0 pinea      (502) staff       (20)   153816 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/swagger-ui/swagger-ui.css
+-rw-r--r--   0 pinea      (502) staff       (20)     1455 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/static/swagger.json
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.256327 mothertongues-0.18.20230410/mtd/templates/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/templates/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1524 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/templates/apidocs.html
+-rw-r--r--   0 pinea      (502) staff       (20)     2097 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/templates/dictionary.html
+-rw-r--r--   0 pinea      (502) staff       (20)     3795 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/templates/index.html
+-rw-r--r--   0 pinea      (502) staff       (20)   100235 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/templates/stats.html
+-rw-r--r--   0 pinea      (502) staff       (20)     9074 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/templates/validator.html
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.260249 mothertongues-0.18.20230410/mtd/tests/
+-rw-r--r--   0 pinea      (502) staff       (20)     4548 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/__init__.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.261407 mothertongues-0.18.20230410/mtd/tests/integration/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/integration/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)      764 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/integration/config_test.json
+-rw-r--r--   0 pinea      (502) staff       (20)     3535 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/integration/test_api_resources.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2551 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/integration/test_basic_integration.py
+-rw-r--r--   0 pinea      (502) staff       (20)     3515 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/integration/test_cli.py
+-rw-r--r--   0 pinea      (502) staff       (20)      132 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/integration/test_swagger_integration.py
+-rw-r--r--   0 pinea      (502) staff       (20)      465 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/log.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2795 2023-03-09 23:35:38.000000 mothertongues-0.18.20230410/mtd/tests/run.py
+-rw-r--r--   0 pinea      (502) staff       (20)     4691 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_cli.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1053 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_csv_parser.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.261837 mothertongues-0.18.20230410/mtd/tests/test_data/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/__init__.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.262308 mothertongues-0.18.20230410/mtd/tests/test_data/csv/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/csv/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1244 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/csv/data.csv
+-rw-r--r--   0 pinea      (502) staff       (20)     2190 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/csv/manifest.json
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.263506 mothertongues-0.18.20230410/mtd/tests/test_data/json/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/json/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)       54 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/json/bad.json
+-rw-r--r--   0 pinea      (502) staff       (20)     2687 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/json/data.json
+-rw-r--r--   0 pinea      (502) staff       (20)     1363 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/json/data_reduced.json
+-rw-r--r--   0 pinea      (502) staff       (20)     1766 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/json/dict_manifest.json
+-rw-r--r--   0 pinea      (502) staff       (20)     1798 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/json/manifest.json
+-rw-r--r--   0 pinea      (502) staff       (20)       39 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/json/missing.json
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.263994 mothertongues-0.18.20230410/mtd/tests/test_data/pkl/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/pkl/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1185 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/pkl/data.pkl
+-rw-r--r--   0 pinea      (502) staff       (20)     1798 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/pkl/manifest.json
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.264561 mothertongues-0.18.20230410/mtd/tests/test_data/psv/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/psv/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1244 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/psv/data.psv
+-rw-r--r--   0 pinea      (502) staff       (20)     2190 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/psv/manifest.json
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/test.log
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.265803 mothertongues-0.18.20230410/mtd/tests/test_data/test_dictionary/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/test_dictionary/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)      488 2023-03-09 23:36:58.000000 mothertongues-0.18.20230410/mtd/tests/test_data/test_dictionary/config_0.json
+-rw-r--r--   0 pinea      (502) staff       (20)      488 2023-03-09 23:36:58.000000 mothertongues-0.18.20230410/mtd/tests/test_data/test_dictionary/config_1.json
+-rw-r--r--   0 pinea      (502) staff       (20)      398 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/test_dictionary/config_2_minimal.json
+-rw-r--r--   0 pinea      (502) staff       (20)      153 2023-03-09 23:36:58.000000 mothertongues-0.18.20230410/mtd/tests/test_data/test_dictionary/dictionaries.txt
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/test_dictionary/test.log
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.267705 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)       40 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/test_composite.json
+-rw-r--r--   0 pinea      (502) staff       (20)       71 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/test_counter_feeding.yaml
+-rw-r--r--   0 pinea      (502) staff       (20)        7 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/test_feeding.csv
+-rw-r--r--   0 pinea      (502) staff       (20)        7 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/test_intermediate_transducer.csv
+-rw-r--r--   0 pinea      (502) staff       (20)        8 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/test_length_transducer.csv
+-rw-r--r--   0 pinea      (502) staff       (20)       95 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/test_length_transducer.yaml
+-rw-r--r--   0 pinea      (502) staff       (20)        3 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/test_transducer.csv
+-rw-r--r--   0 pinea      (502) staff       (20)       53 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/test_transducer.json
+-rw-r--r--   0 pinea      (502) staff       (20)       53 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/test_transducer.yaml
+-rw-r--r--   0 pinea      (502) staff       (20)        4 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/test_transducer_2.csv
+-rw-r--r--   0 pinea      (502) staff       (20)       54 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/transducers/test_transducer_2.yaml
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.268126 mothertongues-0.18.20230410/mtd/tests/test_data/tsv/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/tsv/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1244 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/tsv/data.tsv
+-rw-r--r--   0 pinea      (502) staff       (20)     2190 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/tsv/manifest.json
+-rw-r--r--   0 pinea      (502) staff       (20)     1812 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/whitespace_manifest.json
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.269065 mothertongues-0.18.20230410/mtd/tests/test_data/xlsx/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/xlsx/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     4473 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/xlsx/data.xlsx
+-rw-r--r--   0 pinea      (502) staff       (20)     2199 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/xlsx/manifest.json
+-rw-r--r--   0 pinea      (502) staff       (20)     2199 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/xlsx/manifest.xlsx
+-rw-r--r--   0 pinea      (502) staff       (20)     2151 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/xlsx/manifest_alternate.json
+-rw-r--r--   0 pinea      (502) staff       (20)     7324 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/xlsx/missing_sheet_data.xlsx
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.269842 mothertongues-0.18.20230410/mtd/tests/test_data/xml/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/xml/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)    10291 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/xml/data.xml
+-rw-r--r--   0 pinea      (502) staff       (20)     9274 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/xml/data_reduced.xml
+-rw-r--r--   0 pinea      (502) staff       (20)     1901 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data/xml/manifest.json
+-rw-r--r--   0 pinea      (502) staff       (20)     1108 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_data_configuration_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1693 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_dict_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2292 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_dictionary.py
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_formatted_export.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1643 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_json_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1069 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_pkl_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1008 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_psv_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_raw_export.py
+-rw-r--r--   0 pinea      (502) staff       (20)     3682 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_request_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2702 2023-04-10 19:59:43.000000 mothertongues-0.18.20230410/mtd/tests/test_sorter.py
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_swagger_spec.py
+-rw-r--r--   0 pinea      (502) staff       (20)     9180 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_transducer.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1008 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_tsv_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)      992 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_validator.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2115 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_xlsx_parser.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1298 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/tests/test_xml_parser.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-04-10 20:00:44.272058 mothertongues-0.18.20230410/mtd/transducers/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)      183 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/circumflex_norm.csv
+-rw-r--r--   0 pinea      (502) staff       (20)       36 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/combining_comma.csv
+-rw-r--r--   0 pinea      (502) staff       (20)       42 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/combining_norm.csv
+-rw-r--r--   0 pinea      (502) staff       (20)      941 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/config.yaml
+-rw-r--r--   0 pinea      (502) staff       (20)        6 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/digraph_norm.csv
+-rw-r--r--   0 pinea      (502) staff       (20)       55 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/dot_below_norm.csv
+-rw-r--r--   0 pinea      (502) staff       (20)       87 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/hacek_norm.csv
+-rw-r--r--   0 pinea      (502) staff       (20)       64 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/macron_lowline_norm.csv
+-rw-r--r--   0 pinea      (502) staff       (20)       40 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/norm.csv
+-rw-r--r--   0 pinea      (502) staff       (20)        5 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/slurpy_norm.csv
+-rw-r--r--   0 pinea      (502) staff       (20)        6 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/slurpy_to_line_norm.csv
+-rw-r--r--   0 pinea      (502) staff       (20)      115 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/transducers/underline_norm.csv
+-rw-r--r--   0 pinea      (502) staff       (20)       29 2023-04-10 20:00:44.000000 mothertongues-0.18.20230410/mtd/version.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2556 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/mtd/views.py
+-rw-r--r--   0 pinea      (502) staff       (20)      205 2023-02-04 19:46:13.000000 mothertongues-0.18.20230410/requirements.txt
+-rw-r--r--   0 pinea      (502) staff       (20)       38 2023-04-10 20:00:44.272664 mothertongues-0.18.20230410/setup.cfg
+-rw-r--r--   0 pinea      (502) staff       (20)     1214 2023-01-31 07:16:30.000000 mothertongues-0.18.20230410/setup.py
```

### Comparing `mothertongues-0.18.20220503/PKG-INFO` & `mothertongues-0.18.20230410/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,92 +1,92 @@
 Metadata-Version: 2.1
 Name: mothertongues
-Version: 0.18.20220503
+Version: 0.18.20230410
 Summary: Mother Tongues Dictionaries dictionary creation tool
 Home-page: https://github.com/roedoejet/mothertongues
 Author: Aidan Pine
 Author-email: info@mothertongues.org
 License: AGPL-3.0
-Description: # Mother Tongues Dictionaries (MTD)
-        
-        [![Coverage Status](https://coveralls.io/repos/github/roedoejet/mothertongues/badge.svg?branch=master)](https://coveralls.io/github/roedoejet/mothertongues?branch=master)
-        [![Build Status](https://travis-ci.org/roedoejet/mothertongues.svg?branch=master)](https://travis-ci.org/roedoejet/mothertongues)
-        [![Documentation Status](https://img.shields.io/badge/-docs-blue)](https://docs.mothertongues.org)
-        [![PyPI package](https://img.shields.io/pypi/v/mothertongues.svg)](https://pypi.org/project/mothertongues/)
-        [![license](https://img.shields.io/github/license/roedoejet/mothertongues.svg)](LICENSE)
-        [![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)
-        
-        MTD is the first of two open-source tools that allow language communities and developers to quickly and inexpensively make their dictionary data digitally accessible. MTD is a tool that parses and prepares your data for being used with an MTD User Interface. Currently [mobile](https://github.com/roedoejet/mothertongues-ui) and [web](https://github.com/MotherTongues/mothertongues-UI-Web) are supported.
-        
-        Please visit the [website](https://www.mothertongues.org) or [docs](https://docs.mothertongues.org) for more information.
-        
-        ## Table of Contents
-        
-        - [Background](#background)
-        - [Install](#install)
-        - [Usage](#usage)
-        - [Contributing](#contributing)
-        - [Acknowledgements](#acknowledgements)
-        - [License](#license)
-        
-        ## Background
-        
-        This project started as just a single dictionary for Gitxsan - a language spoken in Northern British Columbia, but it became quickly apparent that many communities also had the same problem. That is, they had some dictionary data but all of the options for sharing that data online were prohibitively expensive. MTD aims to make it easier to create online digital dictionary resources.
-        
-        **Note** - Just because you _can_ make an online dictionary does _not_ mean you _should_. Before making a dictionary, you must have clear consent from the language community in order to publish a dictionary. For some background on why this is important, please read sections 1 and 2.1 [here](http://oxfordre.com/linguistics/view/10.1093/acrefore/9780199384655.001.0001/acrefore-9780199384655-e-8)
-        
-        ## Install
-        
-        It is recommended to install mothertongues using pip. The package name is `mothertongues`, but it is imported as `mtd` and the CLI can be run using either `mothertongues` or `mtd`.
-        
-        ```
-        pip install mothertongues
-        ```
-        
-        ## Usage
-        
-        In order to create a Mother Tongues Dictionary you will need at least two things:
-        
-        - A configuration file for you language/dictionary
-        - A configuration file for each source of data
-        
-        You can find out more about how to create these files against the MTD configuration schema by visiting the [guides](https://docs.mothertongues.org/docs/mtd-guides)
-        
-        Once you have those files, you can either create a dictionary using the command line interface.
-        
-        The basic workflow for creating a dictionary is as follows:
-        
-        1. Fork and clone the [mtd-starter](https://github.com/roedoejet/mtd-starter)
-        2. [Edit and prepare](https://docs.mothertongues.org/docs/mtd-guides-prepare) the repo using your own data
-        3. [Export your data](https://docs.mothertongues.org/docs/mtd-guides-ui#exporting-your-data) to a format readable by the Mother Tongues User Interfaces
-        4. Chose an interface, either [mobile](https://github.com/roedoejet/mothertongues-ui) or [web](https://github.com/MotherTongues/mothertongues-UI-Web)
-        5. Add your exported data (`config.js` and `dict_cached.js`) from step 3 and then [publish](https://docs.mothertongues.org/docs/mtd-guides-publishing) your dictionary! 🎉
-        
-        
-        ## Contributing
-        
-        If something is not working, or you'd like to see another feature added, feel free to dive in! [Open an issue](https://github.com/roedoejet/mothertongues/issues/new) or submit PRs. Help writing and clarifying documentation is also very welcome.
-        
-        This repo follows the [Contributor Covenant](http://contributor-covenant.org/version/1/3/0/) Code of Conduct.
-        
-        ## Acknowledgements
-        
-        Thank you to both Patrick Littell & Mark Turin for their contributions, guidance and support as well as institutional support from the [First Peoples' Cultural Council](http://www.fpcc.ca/) and SSHRC Insight Grant 435-2016-1694, ‘Enhancing Lexical Resources for BC First Nations Languages’.
-        
-        Thank you to all other contributors for support with improving MotherTongues, finding bugs and writing documentation.
-        
-        ### Contributors
-        
-        This project exists thanks to all the people who contribute. 
-        
-        [@littell](https://github.com/littell).
-        [@markturin](https://github.com/markturin).
-        [@eddieantonio](https://github.com/eddieantonio).
-        [@kavonjon](https://github.com/kavonjon).
-        
-        ## License
-        
-        [AGPL-3 © Aidan Pine.](LICENSE)
-        
-Platform: UNKNOWN
 Requires-Python: >=3.6.2
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Mother Tongues Dictionaries (MTD)
+
+[![Coverage Status](https://coveralls.io/repos/github/roedoejet/mothertongues/badge.svg?branch=master)](https://coveralls.io/github/roedoejet/mothertongues?branch=master)
+[![Build Status](https://travis-ci.org/roedoejet/mothertongues.svg?branch=master)](https://travis-ci.org/roedoejet/mothertongues)
+[![Documentation Status](https://img.shields.io/badge/-docs-blue)](https://docs.mothertongues.org)
+[![PyPI package](https://img.shields.io/pypi/v/mothertongues.svg)](https://pypi.org/project/mothertongues/)
+[![license](https://img.shields.io/github/license/roedoejet/mothertongues.svg)](LICENSE)
+[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)
+
+MTD is the first of two open-source tools that allow language communities and developers to quickly and inexpensively make their dictionary data digitally accessible. MTD is a tool that parses and prepares your data for being used with an MTD User Interface. Currently [mobile](https://github.com/roedoejet/mothertongues-ui) and [web](https://github.com/MotherTongues/mothertongues-UI-Web) are supported.
+
+Please visit the [website](https://www.mothertongues.org) or [docs](https://docs.mothertongues.org) for more information.
+
+## Table of Contents
+
+- [Background](#background)
+- [Install](#install)
+- [Usage](#usage)
+- [Contributing](#contributing)
+- [Acknowledgements](#acknowledgements)
+- [License](#license)
+
+## Background
+
+This project started as just a single dictionary for Gitxsan - a language spoken in Northern British Columbia, but it became quickly apparent that many communities also had the same problem. That is, they had some dictionary data but all of the options for sharing that data online were prohibitively expensive. MTD aims to make it easier to create online digital dictionary resources.
+
+**Note** - Just because you _can_ make an online dictionary does _not_ mean you _should_. Before making a dictionary, you must have clear consent from the language community in order to publish a dictionary. For some background on why this is important, please read sections 1 and 2.1 [here](http://oxfordre.com/linguistics/view/10.1093/acrefore/9780199384655.001.0001/acrefore-9780199384655-e-8)
+
+## Install
+
+It is recommended to install mothertongues using pip. The package name is `mothertongues`, but it is imported as `mtd` and the CLI can be run using either `mothertongues` or `mtd`.
+
+```
+pip install mothertongues
+```
+
+## Usage
+
+In order to create a Mother Tongues Dictionary you will need at least two things:
+
+- A configuration file for you language/dictionary
+- A configuration file for each source of data
+
+You can find out more about how to create these files against the MTD configuration schema by visiting the [guides](https://docs.mothertongues.org/docs/mtd-guides)
+
+Once you have those files, you can either create a dictionary using the command line interface.
+
+The basic workflow for creating a dictionary is as follows:
+
+1. Fork and clone the [mtd-starter](https://github.com/roedoejet/mtd-starter)
+2. [Edit and prepare](https://docs.mothertongues.org/docs/mtd-guides-prepare) the repo using your own data
+3. [Export your data](https://docs.mothertongues.org/docs/mtd-guides-ui#exporting-your-data) to a format readable by the Mother Tongues User Interfaces
+4. Chose an interface, either [mobile](https://github.com/roedoejet/mothertongues-ui) or [web](https://github.com/MotherTongues/mothertongues-UI-Web)
+5. Add your exported data (`config.js` and `dict_cached.js`) from step 3 and then [publish](https://docs.mothertongues.org/docs/mtd-guides-publishing) your dictionary! 🎉
+
+
+## Contributing
+
+If something is not working, or you'd like to see another feature added, feel free to dive in! [Open an issue](https://github.com/roedoejet/mothertongues/issues/new) or submit PRs. Help writing and clarifying documentation is also very welcome.
+
+This repo follows the [Contributor Covenant](http://contributor-covenant.org/version/1/3/0/) Code of Conduct.
+
+## Acknowledgements
+
+Thank you to both Patrick Littell & Mark Turin for their contributions, guidance and support as well as institutional support from the [First Peoples' Cultural Council](http://www.fpcc.ca/) and SSHRC Insight Grant 435-2016-1694, ‘Enhancing Lexical Resources for BC First Nations Languages’.
+
+Thank you to all other contributors for support with improving MotherTongues, finding bugs and writing documentation.
+
+### Contributors
+
+This project exists thanks to all the people who contribute. 
+
+[@littell](https://github.com/littell).
+[@markturin](https://github.com/markturin).
+[@eddieantonio](https://github.com/eddieantonio).
+[@kavonjon](https://github.com/kavonjon).
+
+## License
+
+[AGPL-3 © Aidan Pine.](LICENSE)
```

### Comparing `mothertongues-0.18.20220503/README.md` & `mothertongues-0.18.20230410/README.md`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mothertongues.egg-info/PKG-INFO` & `mothertongues-0.18.20230410/mothertongues.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,92 +1,92 @@
 Metadata-Version: 2.1
 Name: mothertongues
-Version: 0.18.20220503
+Version: 0.18.20230410
 Summary: Mother Tongues Dictionaries dictionary creation tool
 Home-page: https://github.com/roedoejet/mothertongues
 Author: Aidan Pine
 Author-email: info@mothertongues.org
 License: AGPL-3.0
-Description: # Mother Tongues Dictionaries (MTD)
-        
-        [![Coverage Status](https://coveralls.io/repos/github/roedoejet/mothertongues/badge.svg?branch=master)](https://coveralls.io/github/roedoejet/mothertongues?branch=master)
-        [![Build Status](https://travis-ci.org/roedoejet/mothertongues.svg?branch=master)](https://travis-ci.org/roedoejet/mothertongues)
-        [![Documentation Status](https://img.shields.io/badge/-docs-blue)](https://docs.mothertongues.org)
-        [![PyPI package](https://img.shields.io/pypi/v/mothertongues.svg)](https://pypi.org/project/mothertongues/)
-        [![license](https://img.shields.io/github/license/roedoejet/mothertongues.svg)](LICENSE)
-        [![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)
-        
-        MTD is the first of two open-source tools that allow language communities and developers to quickly and inexpensively make their dictionary data digitally accessible. MTD is a tool that parses and prepares your data for being used with an MTD User Interface. Currently [mobile](https://github.com/roedoejet/mothertongues-ui) and [web](https://github.com/MotherTongues/mothertongues-UI-Web) are supported.
-        
-        Please visit the [website](https://www.mothertongues.org) or [docs](https://docs.mothertongues.org) for more information.
-        
-        ## Table of Contents
-        
-        - [Background](#background)
-        - [Install](#install)
-        - [Usage](#usage)
-        - [Contributing](#contributing)
-        - [Acknowledgements](#acknowledgements)
-        - [License](#license)
-        
-        ## Background
-        
-        This project started as just a single dictionary for Gitxsan - a language spoken in Northern British Columbia, but it became quickly apparent that many communities also had the same problem. That is, they had some dictionary data but all of the options for sharing that data online were prohibitively expensive. MTD aims to make it easier to create online digital dictionary resources.
-        
-        **Note** - Just because you _can_ make an online dictionary does _not_ mean you _should_. Before making a dictionary, you must have clear consent from the language community in order to publish a dictionary. For some background on why this is important, please read sections 1 and 2.1 [here](http://oxfordre.com/linguistics/view/10.1093/acrefore/9780199384655.001.0001/acrefore-9780199384655-e-8)
-        
-        ## Install
-        
-        It is recommended to install mothertongues using pip. The package name is `mothertongues`, but it is imported as `mtd` and the CLI can be run using either `mothertongues` or `mtd`.
-        
-        ```
-        pip install mothertongues
-        ```
-        
-        ## Usage
-        
-        In order to create a Mother Tongues Dictionary you will need at least two things:
-        
-        - A configuration file for you language/dictionary
-        - A configuration file for each source of data
-        
-        You can find out more about how to create these files against the MTD configuration schema by visiting the [guides](https://docs.mothertongues.org/docs/mtd-guides)
-        
-        Once you have those files, you can either create a dictionary using the command line interface.
-        
-        The basic workflow for creating a dictionary is as follows:
-        
-        1. Fork and clone the [mtd-starter](https://github.com/roedoejet/mtd-starter)
-        2. [Edit and prepare](https://docs.mothertongues.org/docs/mtd-guides-prepare) the repo using your own data
-        3. [Export your data](https://docs.mothertongues.org/docs/mtd-guides-ui#exporting-your-data) to a format readable by the Mother Tongues User Interfaces
-        4. Chose an interface, either [mobile](https://github.com/roedoejet/mothertongues-ui) or [web](https://github.com/MotherTongues/mothertongues-UI-Web)
-        5. Add your exported data (`config.js` and `dict_cached.js`) from step 3 and then [publish](https://docs.mothertongues.org/docs/mtd-guides-publishing) your dictionary! 🎉
-        
-        
-        ## Contributing
-        
-        If something is not working, or you'd like to see another feature added, feel free to dive in! [Open an issue](https://github.com/roedoejet/mothertongues/issues/new) or submit PRs. Help writing and clarifying documentation is also very welcome.
-        
-        This repo follows the [Contributor Covenant](http://contributor-covenant.org/version/1/3/0/) Code of Conduct.
-        
-        ## Acknowledgements
-        
-        Thank you to both Patrick Littell & Mark Turin for their contributions, guidance and support as well as institutional support from the [First Peoples' Cultural Council](http://www.fpcc.ca/) and SSHRC Insight Grant 435-2016-1694, ‘Enhancing Lexical Resources for BC First Nations Languages’.
-        
-        Thank you to all other contributors for support with improving MotherTongues, finding bugs and writing documentation.
-        
-        ### Contributors
-        
-        This project exists thanks to all the people who contribute. 
-        
-        [@littell](https://github.com/littell).
-        [@markturin](https://github.com/markturin).
-        [@eddieantonio](https://github.com/eddieantonio).
-        [@kavonjon](https://github.com/kavonjon).
-        
-        ## License
-        
-        [AGPL-3 © Aidan Pine.](LICENSE)
-        
-Platform: UNKNOWN
 Requires-Python: >=3.6.2
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Mother Tongues Dictionaries (MTD)
+
+[![Coverage Status](https://coveralls.io/repos/github/roedoejet/mothertongues/badge.svg?branch=master)](https://coveralls.io/github/roedoejet/mothertongues?branch=master)
+[![Build Status](https://travis-ci.org/roedoejet/mothertongues.svg?branch=master)](https://travis-ci.org/roedoejet/mothertongues)
+[![Documentation Status](https://img.shields.io/badge/-docs-blue)](https://docs.mothertongues.org)
+[![PyPI package](https://img.shields.io/pypi/v/mothertongues.svg)](https://pypi.org/project/mothertongues/)
+[![license](https://img.shields.io/github/license/roedoejet/mothertongues.svg)](LICENSE)
+[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)
+
+MTD is the first of two open-source tools that allow language communities and developers to quickly and inexpensively make their dictionary data digitally accessible. MTD is a tool that parses and prepares your data for being used with an MTD User Interface. Currently [mobile](https://github.com/roedoejet/mothertongues-ui) and [web](https://github.com/MotherTongues/mothertongues-UI-Web) are supported.
+
+Please visit the [website](https://www.mothertongues.org) or [docs](https://docs.mothertongues.org) for more information.
+
+## Table of Contents
+
+- [Background](#background)
+- [Install](#install)
+- [Usage](#usage)
+- [Contributing](#contributing)
+- [Acknowledgements](#acknowledgements)
+- [License](#license)
+
+## Background
+
+This project started as just a single dictionary for Gitxsan - a language spoken in Northern British Columbia, but it became quickly apparent that many communities also had the same problem. That is, they had some dictionary data but all of the options for sharing that data online were prohibitively expensive. MTD aims to make it easier to create online digital dictionary resources.
+
+**Note** - Just because you _can_ make an online dictionary does _not_ mean you _should_. Before making a dictionary, you must have clear consent from the language community in order to publish a dictionary. For some background on why this is important, please read sections 1 and 2.1 [here](http://oxfordre.com/linguistics/view/10.1093/acrefore/9780199384655.001.0001/acrefore-9780199384655-e-8)
+
+## Install
+
+It is recommended to install mothertongues using pip. The package name is `mothertongues`, but it is imported as `mtd` and the CLI can be run using either `mothertongues` or `mtd`.
+
+```
+pip install mothertongues
+```
+
+## Usage
+
+In order to create a Mother Tongues Dictionary you will need at least two things:
+
+- A configuration file for you language/dictionary
+- A configuration file for each source of data
+
+You can find out more about how to create these files against the MTD configuration schema by visiting the [guides](https://docs.mothertongues.org/docs/mtd-guides)
+
+Once you have those files, you can either create a dictionary using the command line interface.
+
+The basic workflow for creating a dictionary is as follows:
+
+1. Fork and clone the [mtd-starter](https://github.com/roedoejet/mtd-starter)
+2. [Edit and prepare](https://docs.mothertongues.org/docs/mtd-guides-prepare) the repo using your own data
+3. [Export your data](https://docs.mothertongues.org/docs/mtd-guides-ui#exporting-your-data) to a format readable by the Mother Tongues User Interfaces
+4. Chose an interface, either [mobile](https://github.com/roedoejet/mothertongues-ui) or [web](https://github.com/MotherTongues/mothertongues-UI-Web)
+5. Add your exported data (`config.js` and `dict_cached.js`) from step 3 and then [publish](https://docs.mothertongues.org/docs/mtd-guides-publishing) your dictionary! 🎉
+
+
+## Contributing
+
+If something is not working, or you'd like to see another feature added, feel free to dive in! [Open an issue](https://github.com/roedoejet/mothertongues/issues/new) or submit PRs. Help writing and clarifying documentation is also very welcome.
+
+This repo follows the [Contributor Covenant](http://contributor-covenant.org/version/1/3/0/) Code of Conduct.
+
+## Acknowledgements
+
+Thank you to both Patrick Littell & Mark Turin for their contributions, guidance and support as well as institutional support from the [First Peoples' Cultural Council](http://www.fpcc.ca/) and SSHRC Insight Grant 435-2016-1694, ‘Enhancing Lexical Resources for BC First Nations Languages’.
+
+Thank you to all other contributors for support with improving MotherTongues, finding bugs and writing documentation.
+
+### Contributors
+
+This project exists thanks to all the people who contribute. 
+
+[@littell](https://github.com/littell).
+[@markturin](https://github.com/markturin).
+[@eddieantonio](https://github.com/eddieantonio).
+[@kavonjon](https://github.com/kavonjon).
+
+## License
+
+[AGPL-3 © Aidan Pine.](LICENSE)
```

### Comparing `mothertongues-0.18.20220503/mothertongues.egg-info/SOURCES.txt` & `mothertongues-0.18.20230410/mothertongues.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 mothertongues.egg-info/PKG-INFO
 mothertongues.egg-info/SOURCES.txt
 mothertongues.egg-info/dependency_links.txt
@@ -37,29 +38,22 @@
 mtd/parsers/utils.py
 mtd/parsers/xlsx_parser.py
 mtd/parsers/xml_parser.py
 mtd/processors/__init__.py
 mtd/processors/sorter.py
 mtd/processors/transducer.py
 mtd/processors/validator.py
-mtd/static/.DS_Store
 mtd/static/__init__.py
 mtd/static/active.sites.json
 mtd/static/manifest.json
 mtd/static/swagger.json
-mtd/static/assets/.DS_Store
 mtd/static/assets/manifest.json
 mtd/static/assets/icon/favicon.ico
-mtd/static/assets/js/.DS_Store
 mtd/static/assets/js/config-danish.js
-mtd/static/assets/js/config-h-nq-min-m.js
-mtd/static/assets/js/config-test.js
 mtd/static/assets/js/dict_cached-danish.js
-mtd/static/assets/js/dict_cached-h-nq-min-m.js
-mtd/static/assets/js/dict_cached-test.js
 mtd/static/css/custom.css
 mtd/static/css/normalize.css
 mtd/static/css/skeleton.css
 mtd/static/swagger-ui/favicon-16x16.png
 mtd/static/swagger-ui/favicon-32x32.png
 mtd/static/swagger-ui/swagger-ui-bundle.js
 mtd/static/swagger-ui/swagger-ui-standalone-preset.js
@@ -93,23 +87,20 @@
 mtd/tests/test_xml_parser.py
 mtd/tests/integration/__init__.py
 mtd/tests/integration/config_test.json
 mtd/tests/integration/test_api_resources.py
 mtd/tests/integration/test_basic_integration.py
 mtd/tests/integration/test_cli.py
 mtd/tests/integration/test_swagger_integration.py
-mtd/tests/test_data/.DS_Store
 mtd/tests/test_data/__init__.py
 mtd/tests/test_data/test.log
 mtd/tests/test_data/whitespace_manifest.json
-mtd/tests/test_data/csv/.DS_Store
 mtd/tests/test_data/csv/__init__.py
 mtd/tests/test_data/csv/data.csv
 mtd/tests/test_data/csv/manifest.json
-mtd/tests/test_data/json/.DS_Store
 mtd/tests/test_data/json/__init__.py
 mtd/tests/test_data/json/bad.json
 mtd/tests/test_data/json/data.json
 mtd/tests/test_data/json/data_reduced.json
 mtd/tests/test_data/json/dict_manifest.json
 mtd/tests/test_data/json/manifest.json
 mtd/tests/test_data/json/missing.json
@@ -136,15 +127,14 @@
 mtd/tests/test_data/transducers/test_transducer.json
 mtd/tests/test_data/transducers/test_transducer.yaml
 mtd/tests/test_data/transducers/test_transducer_2.csv
 mtd/tests/test_data/transducers/test_transducer_2.yaml
 mtd/tests/test_data/tsv/__init__.py
 mtd/tests/test_data/tsv/data.tsv
 mtd/tests/test_data/tsv/manifest.json
-mtd/tests/test_data/xlsx/.DS_Store
 mtd/tests/test_data/xlsx/__init__.py
 mtd/tests/test_data/xlsx/data.xlsx
 mtd/tests/test_data/xlsx/manifest.json
 mtd/tests/test_data/xlsx/manifest.xlsx
 mtd/tests/test_data/xlsx/manifest_alternate.json
 mtd/tests/test_data/xlsx/missing_sheet_data.xlsx
 mtd/tests/test_data/xml/__init__.py
```

### Comparing `mothertongues-0.18.20220503/mtd/__init__.py` & `mothertongues-0.18.20230410/mtd/__init__.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/buildtools/swagger-pre.json` & `mothertongues-0.18.20230410/mtd/buildtools/swagger-pre.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/buildtools/swagger.json` & `mothertongues-0.18.20230410/mtd/buildtools/swagger.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/buildtools/write_static.py` & `mothertongues-0.18.20230410/mtd/buildtools/write_static.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/cli.py` & `mothertongues-0.18.20230410/mtd/cli.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/dictionary.py` & `mothertongues-0.18.20230410/mtd/dictionary.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/exceptions/__init__.py` & `mothertongues-0.18.20230410/mtd/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/languages/__init__.py` & `mothertongues-0.18.20230410/mtd/languages/__init__.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/languages/config_schema.json` & `mothertongues-0.18.20230410/mtd/languages/config_schema.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/languages/manifest_schema.json` & `mothertongues-0.18.20230410/mtd/languages/manifest_schema.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/languages/suites.py` & `mothertongues-0.18.20230410/mtd/languages/suites.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/parsers/__init__.py` & `mothertongues-0.18.20230410/mtd/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/parsers/csv_parser.py` & `mothertongues-0.18.20230410/mtd/parsers/csv_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/parsers/dict_parser.py` & `mothertongues-0.18.20230410/mtd/parsers/dict_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/parsers/gsheet_parser.py` & `mothertongues-0.18.20230410/mtd/parsers/gsheet_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/parsers/json_parser.py` & `mothertongues-0.18.20230410/mtd/parsers/json_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/parsers/pkl_parser.py` & `mothertongues-0.18.20230410/mtd/parsers/pkl_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/parsers/psv_parser.py` & `mothertongues-0.18.20230410/mtd/parsers/psv_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/parsers/request_parser.py` & `mothertongues-0.18.20230410/mtd/parsers/request_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/parsers/tsv_parser.py` & `mothertongues-0.18.20230410/mtd/parsers/tsv_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/parsers/utils.py` & `mothertongues-0.18.20230410/mtd/parsers/utils.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/parsers/xlsx_parser.py` & `mothertongues-0.18.20230410/mtd/parsers/xlsx_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/parsers/xml_parser.py` & `mothertongues-0.18.20230410/mtd/parsers/xml_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/processors/sorter.py` & `mothertongues-0.18.20230410/mtd/processors/sorter.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/processors/transducer.py` & `mothertongues-0.18.20230410/mtd/processors/transducer.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/processors/validator.py` & `mothertongues-0.18.20230410/mtd/processors/validator.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/resources.py` & `mothertongues-0.18.20230410/mtd/resources.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/static/active.sites.json` & `mothertongues-0.18.20230410/mtd/static/active.sites.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/static/assets/icon/favicon.ico` & `mothertongues-0.18.20230410/mtd/static/assets/icon/favicon.ico`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/static/assets/js/dict_cached-danish.js` & `mothertongues-0.18.20230410/mtd/static/assets/js/dict_cached-danish.js`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/static/css/custom.css` & `mothertongues-0.18.20230410/mtd/static/css/custom.css`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/static/css/normalize.css` & `mothertongues-0.18.20230410/mtd/static/css/normalize.css`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/static/css/skeleton.css` & `mothertongues-0.18.20230410/mtd/static/css/skeleton.css`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/static/swagger-ui/favicon-32x32.png` & `mothertongues-0.18.20230410/mtd/static/swagger-ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/static/swagger-ui/swagger-ui-bundle.js` & `mothertongues-0.18.20230410/mtd/static/swagger-ui/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/static/swagger-ui/swagger-ui-standalone-preset.js` & `mothertongues-0.18.20230410/mtd/static/swagger-ui/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/static/swagger-ui/swagger-ui.css` & `mothertongues-0.18.20230410/mtd/static/swagger-ui/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/static/swagger.json` & `mothertongues-0.18.20230410/mtd/static/swagger.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/templates/apidocs.html` & `mothertongues-0.18.20230410/mtd/templates/apidocs.html`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/templates/dictionary.html` & `mothertongues-0.18.20230410/mtd/templates/dictionary.html`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/templates/index.html` & `mothertongues-0.18.20230410/mtd/templates/index.html`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/templates/stats.html` & `mothertongues-0.18.20230410/mtd/templates/stats.html`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/templates/validator.html` & `mothertongues-0.18.20230410/mtd/templates/validator.html`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/__init__.py` & `mothertongues-0.18.20230410/mtd/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/integration/config_test.json` & `mothertongues-0.18.20230410/mtd/tests/integration/config_test.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/integration/test_api_resources.py` & `mothertongues-0.18.20230410/mtd/tests/integration/test_api_resources.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/integration/test_basic_integration.py` & `mothertongues-0.18.20230410/mtd/tests/integration/test_basic_integration.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/integration/test_cli.py` & `mothertongues-0.18.20230410/mtd/tests/integration/test_cli.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/run.py` & `mothertongues-0.18.20230410/mtd/tests/run.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_cli.py` & `mothertongues-0.18.20230410/mtd/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_csv_parser.py` & `mothertongues-0.18.20230410/mtd/tests/test_csv_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_data/csv/data.csv` & `mothertongues-0.18.20230410/mtd/tests/test_data/csv/data.csv`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_data/csv/manifest.json` & `mothertongues-0.18.20230410/mtd/tests/test_data/csv/manifest.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_data/json/data.json` & `mothertongues-0.18.20230410/mtd/tests/test_data/json/data.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_data/json/data_reduced.json` & `mothertongues-0.18.20230410/mtd/tests/test_data/json/data_reduced.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_data/json/dict_manifest.json` & `mothertongues-0.18.20230410/mtd/tests/test_data/json/dict_manifest.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_data/json/manifest.json` & `mothertongues-0.18.20230410/mtd/tests/test_data/json/manifest.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_data/pkl/data.pkl` & `mothertongues-0.18.20230410/mtd/tests/test_data/pkl/data.pkl`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_data/pkl/manifest.json` & `mothertongues-0.18.20230410/mtd/tests/test_data/pkl/manifest.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_data/psv/data.psv` & `mothertongues-0.18.20230410/mtd/tests/test_data/psv/data.psv`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_data/psv/manifest.json` & `mothertongues-0.18.20230410/mtd/tests/test_data/psv/manifest.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_data/tsv/data.tsv` & `mothertongues-0.18.20230410/mtd/tests/test_data/tsv/data.tsv`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_data/tsv/manifest.json` & `mothertongues-0.18.20230410/mtd/tests/test_data/tsv/manifest.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_data/whitespace_manifest.json` & `mothertongues-0.18.20230410/mtd/tests/test_data/whitespace_manifest.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_data/xlsx/data.xlsx` & `mothertongues-0.18.20230410/mtd/tests/test_data/xlsx/data.xlsx`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_data/xlsx/manifest.json` & `mothertongues-0.18.20230410/mtd/tests/test_data/xlsx/manifest.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_data/xlsx/manifest.xlsx` & `mothertongues-0.18.20230410/mtd/tests/test_data/xlsx/manifest.xlsx`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_data/xlsx/manifest_alternate.json` & `mothertongues-0.18.20230410/mtd/tests/test_data/xlsx/manifest_alternate.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_data/xlsx/missing_sheet_data.xlsx` & `mothertongues-0.18.20230410/mtd/tests/test_data/xlsx/missing_sheet_data.xlsx`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_data/xml/data.xml` & `mothertongues-0.18.20230410/mtd/tests/test_data/xml/data.xml`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_data/xml/data_reduced.xml` & `mothertongues-0.18.20230410/mtd/tests/test_data/xml/data_reduced.xml`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_data/xml/manifest.json` & `mothertongues-0.18.20230410/mtd/tests/test_data/xml/manifest.json`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_data_configuration_parser.py` & `mothertongues-0.18.20230410/mtd/tests/test_data_configuration_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_dict_parser.py` & `mothertongues-0.18.20230410/mtd/tests/test_dict_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_dictionary.py` & `mothertongues-0.18.20230410/mtd/tests/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_json_parser.py` & `mothertongues-0.18.20230410/mtd/tests/test_json_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_pkl_parser.py` & `mothertongues-0.18.20230410/mtd/tests/test_pkl_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_psv_parser.py` & `mothertongues-0.18.20230410/mtd/tests/test_psv_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_request_parser.py` & `mothertongues-0.18.20230410/mtd/tests/test_request_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_sorter.py` & `mothertongues-0.18.20230410/mtd/tests/test_sorter.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_transducer.py` & `mothertongues-0.18.20230410/mtd/tests/test_transducer.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_tsv_parser.py` & `mothertongues-0.18.20230410/mtd/tests/test_tsv_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_validator.py` & `mothertongues-0.18.20230410/mtd/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_xlsx_parser.py` & `mothertongues-0.18.20230410/mtd/tests/test_xlsx_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/tests/test_xml_parser.py` & `mothertongues-0.18.20230410/mtd/tests/test_xml_parser.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/transducers/config.yaml` & `mothertongues-0.18.20230410/mtd/transducers/config.yaml`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/mtd/views.py` & `mothertongues-0.18.20230410/mtd/views.py`

 * *Files identical despite different names*

### Comparing `mothertongues-0.18.20220503/setup.py` & `mothertongues-0.18.20230410/setup.py`

 * *Files identical despite different names*

