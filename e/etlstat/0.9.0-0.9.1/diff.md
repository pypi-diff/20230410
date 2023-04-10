# Comparing `tmp/etlstat-0.9.0.tar.gz` & `tmp/etlstat-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etlstat-0.9.0.tar", last modified: Thu Feb 16 14:06:51 2023, max compression
+gzip compressed data, was "etlstat-0.9.1.tar", last modified: Mon Apr 10 07:59:28 2023, max compression
```

## Comparing `etlstat-0.9.0.tar` & `etlstat-0.9.1.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-02-16 14:06:51.413562 etlstat-0.9.0/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     8667 2021-05-12 11:14:17.000000 etlstat-0.9.0/.pylintrc
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      384 2022-07-14 07:12:25.000000 etlstat-0.9.0/.travis.yml
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1324 2023-02-16 13:55:59.000000 etlstat-0.9.0/CHANGELOG.txt
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    11323 2021-05-12 11:14:17.000000 etlstat-0.9.0/LICENSE.txt
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      907 2021-10-18 11:25:24.000000 etlstat-0.9.0/MANIFEST.in
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1134 2023-02-16 14:06:51.413562 etlstat-0.9.0/PKG-INFO
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1305 2023-02-16 13:48:24.000000 etlstat-0.9.0/Pipfile
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    56446 2023-02-16 13:49:01.000000 etlstat-0.9.0/Pipfile.lock
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      266 2021-05-12 11:14:17.000000 etlstat-0.9.0/README.rst
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-02-16 14:06:51.381562 etlstat-0.9.0/docs/
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-02-16 14:06:51.389562 etlstat-0.9.0/docs/source/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     7782 2021-10-18 11:25:24.000000 etlstat-0.9.0/docs/source/conf.py
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      494 2021-05-12 11:14:17.000000 etlstat-0.9.0/docs/source/index.rst
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      225 2021-05-12 11:14:17.000000 etlstat-0.9.0/docs/source/modules.rst
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-02-16 14:06:51.389562 etlstat-0.9.0/etlstat/
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/__init__.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-02-16 14:06:51.393562 etlstat-0.9.0/etlstat/database/
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     4639 2021-10-28 13:02:54.000000 etlstat-0.9.0/etlstat/database/README.rst
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/database/__init__.py
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    11111 2023-02-16 13:39:52.000000 etlstat-0.9.0/etlstat/database/mysql.py
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    10583 2023-02-16 11:50:51.000000 etlstat-0.9.0/etlstat/database/oracle.py
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3946 2023-02-16 11:51:00.000000 etlstat-0.9.0/etlstat/database/postgresql.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-02-16 14:06:51.393562 etlstat-0.9.0/etlstat/database/test/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1846 2021-10-18 11:25:24.000000 etlstat-0.9.0/etlstat/database/test/22350.px
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/database/test/__init__.py
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1079 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/database/test/pmh.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      503 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/database/test/pmh_update.csv
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     1271 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/database/test/px_01001.csv
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    15093 2023-02-16 13:39:31.000000 etlstat-0.9.0/etlstat/database/test/test_mysql.py
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     8709 2023-02-16 13:38:55.000000 etlstat-0.9.0/etlstat/database/test/test_oracle.py
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3249 2021-10-28 13:02:54.000000 etlstat-0.9.0/etlstat/database/test/test_postgresql.py
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     2640 2023-02-16 13:37:38.000000 etlstat-0.9.0/etlstat/database/test/test_sqlloader.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-02-16 14:06:51.393562 etlstat-0.9.0/etlstat/extractor/
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      332 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/README.rst
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/__init__.py
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    18326 2021-10-29 06:18:59.000000 etlstat-0.9.0/etlstat/extractor/extractor.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-02-16 14:06:51.393562 etlstat-0.9.0/etlstat/extractor/test/
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/__init__.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-02-16 14:06:51.381562 etlstat-0.9.0/etlstat/extractor/test/data/
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-02-16 14:06:51.397562 etlstat-0.9.0/etlstat/extractor/test/data/csv/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      503 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/csv/AEREO_SER_06_15.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      503 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/csv/AEREO_SER_06_15.txt
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1514 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/csv/AGENV_SER_06_15.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1875 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/csv/ALOJ_SER_06_15.csv
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-02-16 14:06:51.397562 etlstat-0.9.0/etlstat/extractor/test/data/excel/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    86016 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/excel/excel_prueba.xls
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    86016 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/excel/prueba_excel.xls
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-02-16 14:06:51.401562 etlstat-0.9.0/etlstat/extractor/test/data/positional/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      588 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/AEREO_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     2982 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/AGENV_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3476 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/ALOJ_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     4994 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/AUDIOV_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    38412 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/CONS_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    26514 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/INFOR_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    24900 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/JURID_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    16986 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/LIMPI_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)   259350 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/MAYOR_COM_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)   534625 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/MENOR_COM_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      560 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/OPIN_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     5865 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/PERSON_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     7680 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/POST_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    11275 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/PUBLI_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3699 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/SSCC_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    52216 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/TEC_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      612 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/TFERR_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1412 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/TMAR_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    87580 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/TMER_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     6120 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/TUI_SER_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    52920 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/VEHIC_COM_06_15.TXT
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)       36 2021-10-29 06:18:59.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/WHITE_SPACES.TXT
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-02-16 14:06:51.405562 etlstat-0.9.0/etlstat/extractor/test/data/positional/format/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      588 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/format/AEREO_SER_formato.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      629 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/format/AGENV_SER_formato.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      451 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/format/ALOJ_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      371 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/format/AUDIOV_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      567 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/format/CONS_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      983 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/format/INFOR_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      605 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/format/JURID_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      428 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/format/LIMPI_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      989 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/format/MAYOR_COM.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1487 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/format/MENOR_COM.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      382 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/format/OPIN_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      575 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/format/PERSON_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1082 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/format/POST_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      581 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/format/PUBLI_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      502 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/format/SSCC_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      686 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/format/TEC_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      639 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/format/TFERR_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      506 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/format/TMAR_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1139 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/format/TMER_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      592 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/format/TUI_SER.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      743 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/format/VEHIC_COM.csv
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)       72 2021-10-29 06:18:59.000000 etlstat-0.9.0/etlstat/extractor/test/data/positional/format/WHITE_SPACES.csv
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-02-16 14:06:51.405562 etlstat-0.9.0/etlstat/extractor/test/data/px/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    18192 2021-10-29 06:18:59.000000 etlstat-0.9.0/etlstat/extractor/test/data/px/o20012.px
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    13264 2021-10-29 06:18:59.000000 etlstat-0.9.0/etlstat/extractor/test/data/px/o20013.px
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      166 2023-02-16 13:50:14.000000 etlstat-0.9.0/etlstat/extractor/test/data/px/pcaxis_urls.csv
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-02-16 14:06:51.405562 etlstat-0.9.0/etlstat/extractor/test/data/px_file/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)   768984 2021-10-18 11:25:24.000000 etlstat-0.9.0/etlstat/extractor/test/data/px_file/27066.px
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-02-16 14:06:51.409561 etlstat-0.9.0/etlstat/extractor/test/data/sql/
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     1583 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/sql/afiliados.sql
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     3024 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/sql/contratos.sql
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    13618 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/sql/ratios.sql
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-02-16 14:06:51.409561 etlstat-0.9.0/etlstat/extractor/test/data/xml/
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    28811 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/xml/Comex.kjb
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    26043 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/xml/Ec_SE_BalanzaCom.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24654 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/xml/Ec_SE_IEFAD.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    26252 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/xml/Ec_SE_IEFAE.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24666 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/xml/Ec_SE_IEFAZ.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24501 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/xml/Ec_SE_IEFDZ.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24796 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/xml/Ec_SE_IEFPZ.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    26158 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/xml/Ec_SE_IEFSC.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    26697 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/xml/Ec_SE_IEFSEC.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24643 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/xml/Ec_SE_IEFTZ.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)   192858 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/extractor/test/data/xml/Ec_SE_IndPosComPreCon99_hechos_v.2.ktr
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    12422 2021-10-29 06:18:59.000000 etlstat-0.9.0/etlstat/extractor/test/test_extractor.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-02-16 14:06:51.409561 etlstat-0.9.0/etlstat/log/
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      112 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/log/README.rst
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       23 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/log/__init__.py
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      739 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/log/logging.py
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      683 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/log/timing.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-02-16 14:06:51.409561 etlstat-0.9.0/etlstat/text/
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      316 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/text/README.rst
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/text/__init__.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-02-16 14:06:51.409561 etlstat-0.9.0/etlstat/text/test/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/text/test/__init__.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-02-16 14:06:51.385562 etlstat-0.9.0/etlstat/text/test/data/
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-02-16 14:06:51.413562 etlstat-0.9.0/etlstat/text/test/data/jobs/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    13315 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/text/test/data/jobs/TODAS_Uso de Comercio Electrónico.kjb
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      522 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/text/test/data/jobs/Uso com_elec.csv
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-02-16 14:06:51.413562 etlstat-0.9.0/etlstat/text/test/data/output/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)    13001 2023-02-16 13:50:15.000000 etlstat-0.9.0/etlstat/text/test/data/output/TODAS_Uso de Comercio Electrónico.kjb
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1621 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/text/test/test_utils.py
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3998 2021-05-12 11:14:17.000000 etlstat-0.9.0/etlstat/text/utils.py
-drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-02-16 14:06:51.393562 etlstat-0.9.0/etlstat.egg-info/
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1134 2023-02-16 14:06:51.000000 etlstat-0.9.0/etlstat.egg-info/PKG-INFO
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     5186 2023-02-16 14:06:51.000000 etlstat-0.9.0/etlstat.egg-info/SOURCES.txt
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)        1 2023-02-16 14:06:51.000000 etlstat-0.9.0/etlstat.egg-info/dependency_links.txt
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)      450 2023-02-16 14:06:51.000000 etlstat-0.9.0/etlstat.egg-info/requires.txt
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)        8 2023-02-16 14:06:51.000000 etlstat-0.9.0/etlstat.egg-info/top_level.txt
--rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1279 2023-02-16 13:56:35.000000 etlstat-0.9.0/requirements.txt
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      204 2023-02-16 14:06:51.413562 etlstat-0.9.0/setup.cfg
--rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     1870 2023-02-16 14:06:27.000000 etlstat-0.9.0/setup.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.264006 etlstat-0.9.1/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     8667 2021-05-12 11:14:17.000000 etlstat-0.9.1/.pylintrc
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      384 2022-07-14 07:12:25.000000 etlstat-0.9.1/.travis.yml
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1356 2023-04-10 07:56:32.000000 etlstat-0.9.1/CHANGELOG.txt
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    11323 2021-05-12 11:14:17.000000 etlstat-0.9.1/LICENSE.txt
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      907 2023-04-10 07:49:18.000000 etlstat-0.9.1/MANIFEST.in
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1134 2023-04-10 07:59:28.264006 etlstat-0.9.1/PKG-INFO
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1305 2023-02-16 13:48:24.000000 etlstat-0.9.1/Pipfile
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    57266 2023-04-10 07:46:25.000000 etlstat-0.9.1/Pipfile.lock
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      266 2021-05-12 11:14:17.000000 etlstat-0.9.1/README.rst
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.208006 etlstat-0.9.1/docs/
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.224005 etlstat-0.9.1/docs/source/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     7782 2021-10-18 11:25:24.000000 etlstat-0.9.1/docs/source/conf.py
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      494 2021-05-12 11:14:17.000000 etlstat-0.9.1/docs/source/index.rst
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      225 2021-05-12 11:14:17.000000 etlstat-0.9.1/docs/source/modules.rst
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.224005 etlstat-0.9.1/etlstat/
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/__init__.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.224005 etlstat-0.9.1/etlstat/database/
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     4639 2021-10-28 13:02:54.000000 etlstat-0.9.1/etlstat/database/README.rst
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/database/__init__.py
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    11111 2023-02-16 13:39:52.000000 etlstat-0.9.1/etlstat/database/mysql.py
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    10583 2023-02-16 11:50:51.000000 etlstat-0.9.1/etlstat/database/oracle.py
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3946 2023-02-16 11:51:00.000000 etlstat-0.9.1/etlstat/database/postgresql.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.228006 etlstat-0.9.1/etlstat/database/test/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1846 2021-10-18 11:25:24.000000 etlstat-0.9.1/etlstat/database/test/22350.px
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/database/test/__init__.py
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1079 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/database/test/pmh.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      503 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/database/test/pmh_update.csv
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     1271 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/database/test/px_01001.csv
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    15093 2023-02-16 13:39:31.000000 etlstat-0.9.1/etlstat/database/test/test_mysql.py
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     8709 2023-02-16 13:38:55.000000 etlstat-0.9.1/etlstat/database/test/test_oracle.py
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3249 2021-10-28 13:02:54.000000 etlstat-0.9.1/etlstat/database/test/test_postgresql.py
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     2640 2023-02-16 13:37:38.000000 etlstat-0.9.1/etlstat/database/test/test_sqlloader.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.228006 etlstat-0.9.1/etlstat/extractor/
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      332 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/README.rst
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/__init__.py
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    18326 2021-10-29 06:18:59.000000 etlstat-0.9.1/etlstat/extractor/extractor.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.228006 etlstat-0.9.1/etlstat/extractor/test/
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/__init__.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.212005 etlstat-0.9.1/etlstat/extractor/test/data/
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.228006 etlstat-0.9.1/etlstat/extractor/test/data/csv/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      503 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/csv/AEREO_SER_06_15.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      503 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/csv/AEREO_SER_06_15.txt
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1514 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/csv/AGENV_SER_06_15.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1875 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/csv/ALOJ_SER_06_15.csv
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.228006 etlstat-0.9.1/etlstat/extractor/test/data/excel/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    86016 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/excel/excel_prueba.xls
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    86016 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/excel/prueba_excel.xls
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.236005 etlstat-0.9.1/etlstat/extractor/test/data/positional/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      588 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/AEREO_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     2982 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/AGENV_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3476 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/ALOJ_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     4994 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/AUDIOV_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    38412 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/CONS_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    26514 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/INFOR_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    24900 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/JURID_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    16986 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/LIMPI_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)   259350 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/MAYOR_COM_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)   534625 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/MENOR_COM_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      560 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/OPIN_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     5865 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/PERSON_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     7680 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/POST_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    11275 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/PUBLI_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3699 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/SSCC_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    52216 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/TEC_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      612 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/TFERR_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1412 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/TMAR_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    87580 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/TMER_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     6120 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/TUI_SER_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    52920 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/VEHIC_COM_06_15.TXT
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)       36 2021-10-29 06:18:59.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/WHITE_SPACES.TXT
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.240005 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      588 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/AEREO_SER_formato.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      629 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/AGENV_SER_formato.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      451 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/ALOJ_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      371 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/AUDIOV_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      567 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/CONS_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      983 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/INFOR_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      605 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/JURID_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      428 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/LIMPI_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      989 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/MAYOR_COM.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1487 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/MENOR_COM.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      382 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/OPIN_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      575 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/PERSON_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1082 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/POST_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      581 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/PUBLI_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      502 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/SSCC_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      686 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/TEC_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      639 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/TFERR_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      506 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/TMAR_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1139 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/TMER_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      592 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/TUI_SER.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      743 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/VEHIC_COM.csv
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)       72 2021-10-29 06:18:59.000000 etlstat-0.9.1/etlstat/extractor/test/data/positional/format/WHITE_SPACES.csv
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.240005 etlstat-0.9.1/etlstat/extractor/test/data/px/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    18192 2021-10-29 06:18:59.000000 etlstat-0.9.1/etlstat/extractor/test/data/px/o20012.px
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    13264 2021-10-29 06:18:59.000000 etlstat-0.9.1/etlstat/extractor/test/data/px/o20013.px
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      166 2023-02-16 13:50:14.000000 etlstat-0.9.1/etlstat/extractor/test/data/px/pcaxis_urls.csv
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.260005 etlstat-0.9.1/etlstat/extractor/test/data/px_file/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)   768984 2021-10-18 11:25:24.000000 etlstat-0.9.1/etlstat/extractor/test/data/px_file/27066.px
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.260005 etlstat-0.9.1/etlstat/extractor/test/data/sql/
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     1583 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/sql/afiliados.sql
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     3024 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/sql/contratos.sql
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    13618 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/sql/ratios.sql
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.264006 etlstat-0.9.1/etlstat/extractor/test/data/xml/
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    28811 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/xml/Comex.kjb
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    26043 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_BalanzaCom.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24654 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFAD.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    26252 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFAE.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24666 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFAZ.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24501 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFDZ.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24796 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFPZ.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    26158 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFSC.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    26697 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFSEC.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    24643 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFTZ.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)   192858 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IndPosComPreCon99_hechos_v.2.ktr
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)    12422 2021-10-29 06:18:59.000000 etlstat-0.9.1/etlstat/extractor/test/test_extractor.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.264006 etlstat-0.9.1/etlstat/log/
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      112 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/log/README.rst
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)       23 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/log/__init__.py
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      739 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/log/logging.py
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      683 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/log/timing.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.264006 etlstat-0.9.1/etlstat/text/
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      316 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/text/README.rst
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/text/__init__.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.264006 etlstat-0.9.1/etlstat/text/test/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)       24 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/text/test/__init__.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.212005 etlstat-0.9.1/etlstat/text/test/data/
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.264006 etlstat-0.9.1/etlstat/text/test/data/jobs/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    13315 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/text/test/data/jobs/TODAS_Uso de Comercio Electrónico.kjb
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      522 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/text/test/data/jobs/Uso com_elec.csv
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.264006 etlstat-0.9.1/etlstat/text/test/data/output/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)    13001 2023-02-16 13:50:15.000000 etlstat-0.9.1/etlstat/text/test/data/output/TODAS_Uso de Comercio Electrónico.kjb
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1621 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/text/test/test_utils.py
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     3998 2021-05-12 11:14:17.000000 etlstat-0.9.1/etlstat/text/utils.py
+drwxr-xr-x   0 arc17854  (1000) arc17854  (1000)        0 2023-04-10 07:59:28.224005 etlstat-0.9.1/etlstat.egg-info/
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1134 2023-04-10 07:59:28.000000 etlstat-0.9.1/etlstat.egg-info/PKG-INFO
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     5186 2023-04-10 07:59:28.000000 etlstat-0.9.1/etlstat.egg-info/SOURCES.txt
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)        1 2023-04-10 07:59:28.000000 etlstat-0.9.1/etlstat.egg-info/dependency_links.txt
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)      448 2023-04-10 07:59:28.000000 etlstat-0.9.1/etlstat.egg-info/requires.txt
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)        8 2023-04-10 07:59:28.000000 etlstat-0.9.1/etlstat.egg-info/top_level.txt
+-rw-r--r--   0 arc17854  (1000) arc17854  (1000)     1271 2023-04-10 07:50:08.000000 etlstat-0.9.1/requirements.txt
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)      204 2023-04-10 07:59:28.268005 etlstat-0.9.1/setup.cfg
+-rwxr-xr-x   0 arc17854  (1000) arc17854  (1000)     1867 2023-04-10 07:56:04.000000 etlstat-0.9.1/setup.py
```

### Comparing `etlstat-0.9.0/.pylintrc` & `etlstat-0.9.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/CHANGELOG.txt` & `etlstat-0.9.1/CHANGELOG.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+v0.9.1:
+    - Fix dependencies.
 v0.9.0:
     - Add management for database exceptions.
     - Update dependencies.
 v0.8.2:
     - fix dependencies.
 v0.8.1:
     - fix dependencies.
```

### Comparing `etlstat-0.9.0/LICENSE.txt` & `etlstat-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/MANIFEST.in` & `etlstat-0.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/PKG-INFO` & `etlstat-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etlstat
-Version: 0.9.0
+Version: 0.9.1
 Summary: ETL utils for statistical offices data processing
 Home-page: https://github.com/icane/etlstat.git
 Author: Instituto Cántabro de Estadística
 Author-email: icane@cantabria.es
 License: Apache License 2.0
 Keywords: etl,icane,statistics,utils
 Classifier: Development Status :: 4 - Beta
```

### Comparing `etlstat-0.9.0/Pipfile` & `etlstat-0.9.1/Pipfile`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/Pipfile.lock` & `etlstat-0.9.1/Pipfile.lock`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9641377423389619%*

 * *Differences: {"'default'": "{'beautifulsoup4': {'hashes': "*

 * *              "['sha256:492bbc69dca35d12daac71c4db1bfff0c876c00ef4a2ffacce226d4638eb72da', "*

 * *              "'sha256:bd2520ca0d9d7d12694a53d44ac482d181b4ec1888909b035a3dbf40d0f57d4a'], "*

 * *              "'version': '==4.12.2'}, 'charset-normalizer': {'hashes': "*

 * *              "['sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6', "*

 * *              "'sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1', "*

 * *              "'sha2 […]*

```diff
@@ -14,122 +14,109 @@
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "beautifulsoup4": {
             "hashes": [
-                "sha256:0e79446b10b3ecb499c1556f7e228a53e64a2bfcebd455f370d8927cb5b59e39",
-                "sha256:bc4bdda6717de5a2987436fb8d72f45dc90dd856bdfd512a1314ce90349a0106"
+                "sha256:492bbc69dca35d12daac71c4db1bfff0c876c00ef4a2ffacce226d4638eb72da",
+                "sha256:bd2520ca0d9d7d12694a53d44ac482d181b4ec1888909b035a3dbf40d0f57d4a"
             ],
             "index": "pypi",
-            "version": "==4.11.2",
+            "version": "==4.12.2",
             "version >=": "4.10.*"
         },
         "certifi": {
             "hashes": [
                 "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
                 "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2022.12.7"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:00d3ffdaafe92a5dc603cb9bd5111aaa36dfa187c8285c543be562e61b755f6b",
-                "sha256:024e606be3ed92216e2b6952ed859d86b4cfa52cd5bc5f050e7dc28f9b43ec42",
-                "sha256:0298eafff88c99982a4cf66ba2efa1128e4ddaca0b05eec4c456bbc7db691d8d",
-                "sha256:02a51034802cbf38db3f89c66fb5d2ec57e6fe7ef2f4a44d070a593c3688667b",
-                "sha256:083c8d17153ecb403e5e1eb76a7ef4babfc2c48d58899c98fcaa04833e7a2f9a",
-                "sha256:0a11e971ed097d24c534c037d298ad32c6ce81a45736d31e0ff0ad37ab437d59",
-                "sha256:0bf2dae5291758b6f84cf923bfaa285632816007db0330002fa1de38bfcb7154",
-                "sha256:0c0a590235ccd933d9892c627dec5bc7511ce6ad6c1011fdf5b11363022746c1",
-                "sha256:0f438ae3532723fb6ead77e7c604be7c8374094ef4ee2c5e03a3a17f1fca256c",
-                "sha256:109487860ef6a328f3eec66f2bf78b0b72400280d8f8ea05f69c51644ba6521a",
-                "sha256:11b53acf2411c3b09e6af37e4b9005cba376c872503c8f28218c7243582df45d",
-                "sha256:12db3b2c533c23ab812c2b25934f60383361f8a376ae272665f8e48b88e8e1c6",
-                "sha256:14e76c0f23218b8f46c4d87018ca2e441535aed3632ca134b10239dfb6dadd6b",
-                "sha256:16a8663d6e281208d78806dbe14ee9903715361cf81f6d4309944e4d1e59ac5b",
-                "sha256:292d5e8ba896bbfd6334b096e34bffb56161c81408d6d036a7dfa6929cff8783",
-                "sha256:2c03cc56021a4bd59be889c2b9257dae13bf55041a3372d3295416f86b295fb5",
-                "sha256:2e396d70bc4ef5325b72b593a72c8979999aa52fb8bcf03f701c1b03e1166918",
-                "sha256:2edb64ee7bf1ed524a1da60cdcd2e1f6e2b4f66ef7c077680739f1641f62f555",
-                "sha256:31a9ddf4718d10ae04d9b18801bd776693487cbb57d74cc3458a7673f6f34639",
-                "sha256:356541bf4381fa35856dafa6a965916e54bed415ad8a24ee6de6e37deccf2786",
-                "sha256:358a7c4cb8ba9b46c453b1dd8d9e431452d5249072e4f56cfda3149f6ab1405e",
-                "sha256:37f8febc8ec50c14f3ec9637505f28e58d4f66752207ea177c1d67df25da5aed",
-                "sha256:39049da0ffb96c8cbb65cbf5c5f3ca3168990adf3551bd1dee10c48fce8ae820",
-                "sha256:39cf9ed17fe3b1bc81f33c9ceb6ce67683ee7526e65fde1447c772afc54a1bb8",
-                "sha256:3ae1de54a77dc0d6d5fcf623290af4266412a7c4be0b1ff7444394f03f5c54e3",
-                "sha256:3b590df687e3c5ee0deef9fc8c547d81986d9a1b56073d82de008744452d6541",
-                "sha256:3e45867f1f2ab0711d60c6c71746ac53537f1684baa699f4f668d4c6f6ce8e14",
-                "sha256:3fc1c4a2ffd64890aebdb3f97e1278b0cc72579a08ca4de8cd2c04799a3a22be",
-                "sha256:4457ea6774b5611f4bed5eaa5df55f70abde42364d498c5134b7ef4c6958e20e",
-                "sha256:44ba614de5361b3e5278e1241fda3dc1838deed864b50a10d7ce92983797fa76",
-                "sha256:4a8fcf28c05c1f6d7e177a9a46a1c52798bfe2ad80681d275b10dcf317deaf0b",
-                "sha256:4b0d02d7102dd0f997580b51edc4cebcf2ab6397a7edf89f1c73b586c614272c",
-                "sha256:502218f52498a36d6bf5ea77081844017bf7982cdbe521ad85e64cabee1b608b",
-                "sha256:503e65837c71b875ecdd733877d852adbc465bd82c768a067badd953bf1bc5a3",
-                "sha256:5995f0164fa7df59db4746112fec3f49c461dd6b31b841873443bdb077c13cfc",
-                "sha256:59e5686dd847347e55dffcc191a96622f016bc0ad89105e24c14e0d6305acbc6",
-                "sha256:601f36512f9e28f029d9481bdaf8e89e5148ac5d89cffd3b05cd533eeb423b59",
-                "sha256:608862a7bf6957f2333fc54ab4399e405baad0163dc9f8d99cb236816db169d4",
-                "sha256:62595ab75873d50d57323a91dd03e6966eb79c41fa834b7a1661ed043b2d404d",
-                "sha256:70990b9c51340e4044cfc394a81f614f3f90d41397104d226f21e66de668730d",
-                "sha256:71140351489970dfe5e60fc621ada3e0f41104a5eddaca47a7acb3c1b851d6d3",
-                "sha256:72966d1b297c741541ca8cf1223ff262a6febe52481af742036a0b296e35fa5a",
-                "sha256:74292fc76c905c0ef095fe11e188a32ebd03bc38f3f3e9bcb85e4e6db177b7ea",
-                "sha256:761e8904c07ad053d285670f36dd94e1b6ab7f16ce62b9805c475b7aa1cffde6",
-                "sha256:772b87914ff1152b92a197ef4ea40efe27a378606c39446ded52c8f80f79702e",
-                "sha256:79909e27e8e4fcc9db4addea88aa63f6423ebb171db091fb4373e3312cb6d603",
-                "sha256:7e189e2e1d3ed2f4aebabd2d5b0f931e883676e51c7624826e0a4e5fe8a0bf24",
-                "sha256:7eb33a30d75562222b64f569c642ff3dc6689e09adda43a082208397f016c39a",
-                "sha256:81d6741ab457d14fdedc215516665050f3822d3e56508921cc7239f8c8e66a58",
-                "sha256:8499ca8f4502af841f68135133d8258f7b32a53a1d594aa98cc52013fff55678",
-                "sha256:84c3990934bae40ea69a82034912ffe5a62c60bbf6ec5bc9691419641d7d5c9a",
-                "sha256:87701167f2a5c930b403e9756fab1d31d4d4da52856143b609e30a1ce7160f3c",
-                "sha256:88600c72ef7587fe1708fd242b385b6ed4b8904976d5da0893e31df8b3480cb6",
-                "sha256:8ac7b6a045b814cf0c47f3623d21ebd88b3e8cf216a14790b455ea7ff0135d18",
-                "sha256:8b8af03d2e37866d023ad0ddea594edefc31e827fee64f8de5611a1dbc373174",
-                "sha256:8c7fe7afa480e3e82eed58e0ca89f751cd14d767638e2550c77a92a9e749c317",
-                "sha256:8eade758719add78ec36dc13201483f8e9b5d940329285edcd5f70c0a9edbd7f",
-                "sha256:911d8a40b2bef5b8bbae2e36a0b103f142ac53557ab421dc16ac4aafee6f53dc",
-                "sha256:93ad6d87ac18e2a90b0fe89df7c65263b9a99a0eb98f0a3d2e079f12a0735837",
-                "sha256:95dea361dd73757c6f1c0a1480ac499952c16ac83f7f5f4f84f0658a01b8ef41",
-                "sha256:9ab77acb98eba3fd2a85cd160851816bfce6871d944d885febf012713f06659c",
-                "sha256:9cb3032517f1627cc012dbc80a8ec976ae76d93ea2b5feaa9d2a5b8882597579",
-                "sha256:9cf4e8ad252f7c38dd1f676b46514f92dc0ebeb0db5552f5f403509705e24753",
-                "sha256:9d9153257a3f70d5f69edf2325357251ed20f772b12e593f3b3377b5f78e7ef8",
-                "sha256:a152f5f33d64a6be73f1d30c9cc82dfc73cec6477ec268e7c6e4c7d23c2d2291",
-                "sha256:a16418ecf1329f71df119e8a65f3aa68004a3f9383821edcb20f0702934d8087",
-                "sha256:a60332922359f920193b1d4826953c507a877b523b2395ad7bc716ddd386d866",
-                "sha256:a8d0fc946c784ff7f7c3742310cc8a57c5c6dc31631269876a88b809dbeff3d3",
-                "sha256:ab5de034a886f616a5668aa5d098af2b5385ed70142090e2a31bcbd0af0fdb3d",
-                "sha256:c22d3fe05ce11d3671297dc8973267daa0f938b93ec716e12e0f6dee81591dc1",
-                "sha256:c2ac1b08635a8cd4e0cbeaf6f5e922085908d48eb05d44c5ae9eabab148512ca",
-                "sha256:c512accbd6ff0270939b9ac214b84fb5ada5f0409c44298361b2f5e13f9aed9e",
-                "sha256:c75ffc45f25324e68ab238cb4b5c0a38cd1c3d7f1fb1f72b5541de469e2247db",
-                "sha256:c95a03c79bbe30eec3ec2b7f076074f4281526724c8685a42872974ef4d36b72",
-                "sha256:cadaeaba78750d58d3cc6ac4d1fd867da6fc73c88156b7a3212a3cd4819d679d",
-                "sha256:cd6056167405314a4dc3c173943f11249fa0f1b204f8b51ed4bde1a9cd1834dc",
-                "sha256:db72b07027db150f468fbada4d85b3b2729a3db39178abf5c543b784c1254539",
-                "sha256:df2c707231459e8a4028eabcd3cfc827befd635b3ef72eada84ab13b52e1574d",
-                "sha256:e62164b50f84e20601c1ff8eb55620d2ad25fb81b59e3cd776a1902527a788af",
-                "sha256:e696f0dd336161fca9adbb846875d40752e6eba585843c768935ba5c9960722b",
-                "sha256:eaa379fcd227ca235d04152ca6704c7cb55564116f8bc52545ff357628e10602",
-                "sha256:ebea339af930f8ca5d7a699b921106c6e29c617fe9606fa7baa043c1cdae326f",
-                "sha256:f4c39b0e3eac288fedc2b43055cfc2ca7a60362d0e5e87a637beac5d801ef478",
-                "sha256:f5057856d21e7586765171eac8b9fc3f7d44ef39425f85dbcccb13b3ebea806c",
-                "sha256:f6f45710b4459401609ebebdbcfb34515da4fc2aa886f95107f556ac69a9147e",
-                "sha256:f97e83fa6c25693c7a35de154681fcc257c1c41b38beb0304b9c4d2d9e164479",
-                "sha256:f9d0c5c045a3ca9bedfc35dca8526798eb91a07aa7a2c0fee134c6c6f321cbd7",
-                "sha256:ff6f3db31555657f3163b15a6b7c6938d08df7adbfc9dd13d9d19edad678f1e8"
+                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
+                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
+                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
+                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
+                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
+                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
+                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
+                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
+                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
+                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
+                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
+                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
+                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
+                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
+                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
+                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
+                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
+                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
+                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
+                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
+                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
+                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
+                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
+                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
+                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
+                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
+                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
+                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
+                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
+                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
+                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
+                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
+                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
+                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
+                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
+                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
+                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
+                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
+                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
+                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
+                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
+                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
+                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
+                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
+                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
+                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
+                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
+                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
+                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
+                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
+                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
+                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
+                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
+                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
+                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
+                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
+                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
+                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
+                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
+                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
+                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
+                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
+                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
+                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
+                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
+                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
+                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
+                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
+                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
+                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
+                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
+                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
+                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
+                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
+                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
-            "markers": "python_full_version >= '3.6.0'",
-            "version": "==3.0.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==3.1.0"
         },
         "cx-oracle": {
             "hashes": [
                 "sha256:052cfd1b49ca20265893bad543f2d0755ec5d726f1f9b43b091ccb819a2912ca",
                 "sha256:10379b49b910b475987f771c43a37f7e94f938d4fa7bd8f88d06e7460a5370ae",
                 "sha256:1b519d3435ac1ca8b186e59626351355e24be050b80936a36065cbf5618b9017",
                 "sha256:257f03c19271f023d2720b7600f80cee282725670ce790322c312a1de8b92b2f",
@@ -342,17 +329,17 @@
                 "sha256:3624ac64a5e4187a74daa9b68953ec351440fbdebb32e56bc8f73d32973eb766"
             ],
             "index": "pypi",
             "version": "==0.3.4"
         },
         "pyjstat": {
             "hashes": [
-                "sha256:72034d058bdc7447b21fab2c9c2372250e0065e9bbd20439b05058617fddd50a"
+                "sha256:dd7fc7b4ed0892fb949ff87eeea3e2c838754eef43922b40ba3c38fadfc30795"
             ],
-            "version": "==2.3.0"
+            "version": "==2.4.0"
         },
         "python-dateutil": {
             "hashes": [
                 "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86",
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -363,18 +350,18 @@
                 "sha256:dc2395fbd148a1ab31090dd113c366695934b9e85fe5a4b2a032745efd0346f6"
             ],
             "index": "pypi",
             "version": "==0.12.2"
         },
         "pytz": {
             "hashes": [
-                "sha256:01a0681c4b9684a28304615eba55d1ab31ae00bf68ec157ec3708a8182dbbcd0",
-                "sha256:78f4f37d8198e0627c5f1143240bb0206b8691d8d7ac6d78fee88b78733f8c4a"
+                "sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588",
+                "sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb"
             ],
-            "version": "==2022.7.1"
+            "version": "==2023.3"
         },
         "requests": {
             "hashes": [
                 "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
                 "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
             ],
             "markers": "python_version >= '3.7' and python_version < '4'",
@@ -394,58 +381,58 @@
                 "sha256:e28dba9ca6c7c00173e34e4ba57448f0688bb681b7c5e8bf4971daafc093d69a"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.4"
         },
         "sqlalchemy": {
             "hashes": [
-                "sha256:07e48cbcdda6b8bc7a59d6728bd3f5f574ffe03f2c9fb384239f3789c2d95c2e",
-                "sha256:18cafdb27834fa03569d29f571df7115812a0e59fd6a3a03ccb0d33678ec8420",
-                "sha256:1b1e5e96e2789d89f023d080bee432e2fef64d95857969e70d3cadec80bd26f0",
-                "sha256:315676344e3558f1f80d02535f410e80ea4e8fddba31ec78fe390eff5fb8f466",
-                "sha256:31de1e2c45e67a5ec1ecca6ec26aefc299dd5151e355eb5199cd9516b57340be",
-                "sha256:3d94682732d1a0def5672471ba42a29ff5e21bb0aae0afa00bb10796fc1e28dd",
-                "sha256:3ec187acf85984263299a3f15c34a6c0671f83565d86d10f43ace49881a82718",
-                "sha256:4847f4b1d822754e35707db913396a29d874ee77b9c3c3ef3f04d5a9a6209618",
-                "sha256:4d112b0f3c1bc5ff70554a97344625ef621c1bfe02a73c5d97cac91f8cd7a41e",
-                "sha256:51e1ba2884c6a2b8e19109dc08c71c49530006c1084156ecadfaadf5f9b8b053",
-                "sha256:535377e9b10aff5a045e3d9ada8a62d02058b422c0504ebdcf07930599890eb0",
-                "sha256:5dbf17ac9a61e7a3f1c7ca47237aac93cabd7f08ad92ac5b96d6f8dea4287fc1",
-                "sha256:5f752676fc126edc1c4af0ec2e4d2adca48ddfae5de46bb40adbd3f903eb2120",
-                "sha256:64cb0ad8a190bc22d2112001cfecdec45baffdf41871de777239da6a28ed74b6",
-                "sha256:6913b8247d8a292ef8315162a51931e2b40ce91681f1b6f18f697045200c4a30",
-                "sha256:69fac0a7054d86b997af12dc23f581cf0b25fb1c7d1fed43257dee3af32d3d6d",
-                "sha256:7001f16a9a8e06488c3c7154827c48455d1c1507d7228d43e781afbc8ceccf6d",
-                "sha256:7b81b1030c42b003fc10ddd17825571603117f848814a344d305262d370e7c34",
-                "sha256:7f8267682eb41a0584cf66d8a697fef64b53281d01c93a503e1344197f2e01fe",
-                "sha256:887865924c3d6e9a473dc82b70977395301533b3030d0f020c38fd9eba5419f2",
-                "sha256:9167d4227b56591a4cc5524f1b79ccd7ea994f36e4c648ab42ca995d28ebbb96",
-                "sha256:939f9a018d2ad04036746e15d119c0428b1e557470361aa798e6e7d7f5875be0",
-                "sha256:955162ad1a931fe416eded6bb144ba891ccbf9b2e49dc7ded39274dd9c5affc5",
-                "sha256:984ee13543a346324319a1fb72b698e521506f6f22dc37d7752a329e9cd00a32",
-                "sha256:9883f5fae4fd8e3f875adc2add69f8b945625811689a6c65866a35ee9c0aea23",
-                "sha256:a1ad90c97029cc3ab4ffd57443a20fac21d2ec3c89532b084b073b3feb5abff3",
-                "sha256:a3714e5b33226131ac0da60d18995a102a17dddd42368b7bdd206737297823ad",
-                "sha256:ae067ab639fa499f67ded52f5bc8e084f045d10b5ac7bb928ae4ca2b6c0429a5",
-                "sha256:b33ffbdbbf5446cf36cd4cc530c9d9905d3c2fe56ed09e25c22c850cdb9fac92",
-                "sha256:b6e4cb5c63f705c9d546a054c60d326cbde7421421e2d2565ce3e2eee4e1a01f",
-                "sha256:b7f4b6aa6e87991ec7ce0e769689a977776db6704947e562102431474799a857",
-                "sha256:c04144a24103135ea0315d459431ac196fe96f55d3213bfd6d39d0247775c854",
-                "sha256:c522e496f9b9b70296a7675272ec21937ccfc15da664b74b9f58d98a641ce1b6",
-                "sha256:c5a99282848b6cae0056b85da17392a26b2d39178394fc25700bcf967e06e97a",
-                "sha256:c7a46639ba058d320c9f53a81db38119a74b8a7a1884df44d09fbe807d028aaf",
-                "sha256:d4b1cc7835b39835c75cf7c20c926b42e97d074147c902a9ebb7cf2c840dc4e2",
-                "sha256:d4d164df3d83d204c69f840da30b292ac7dc54285096c6171245b8d7807185aa",
-                "sha256:d61e9ecc849d8d44d7f80894ecff4abe347136e9d926560b818f6243409f3c86",
-                "sha256:d68e1762997bfebf9e5cf2a9fd0bcf9ca2fdd8136ce7b24bbd3bbfa4328f3e4a",
-                "sha256:e3c1808008124850115a3f7e793a975cfa5c8a26ceeeb9ff9cbb4485cac556df",
-                "sha256:f8cb80fe8d14307e4124f6fad64dfd87ab749c9d275f82b8b4ec84c84ecebdbe"
+                "sha256:03be6f3cb66e69fb3a09b5ea89d77e4bc942f3bf84b207dba84666a26799c166",
+                "sha256:048509d7f3ac27b83ad82fd96a1ab90a34c8e906e4e09c8d677fc531d12c23c5",
+                "sha256:07764b240645627bc3e82596435bd1a1884646bfc0721642d24c26b12f1df194",
+                "sha256:0fdbb8e9d4e9003f332a93d6a37bca48ba8095086c97a89826a136d8eddfc455",
+                "sha256:10edbb92a9ef611f01b086e271a9f6c1c3e5157c3b0c5ff62310fb2187acbd4a",
+                "sha256:14a3879853208a242b5913f3a17c6ac0eae9dc210ff99c8f10b19d4a1ed8ed9b",
+                "sha256:16ee6fea316790980779268da47a9260d5dd665c96f225d28e7750b0bb2e2a04",
+                "sha256:1e2a42017984099ef6f56438a6b898ce0538f6fadddaa902870c5aa3e1d82583",
+                "sha256:28297aa29e035f29cba6b16aacd3680fbc6a9db682258d5f2e7b49ec215dbe40",
+                "sha256:28fda5a69d6182589892422c5a9b02a8fd1125787aab1d83f1392aa955bf8d0a",
+                "sha256:299b5c5c060b9fbe51808d0d40d8475f7b3873317640b9b7617c7f988cf59fda",
+                "sha256:2bba39b12b879c7b35cde18b6e14119c5f1a16bd064a48dd2ac62d21366a5e17",
+                "sha256:32ab09f2863e3de51529aa84ff0e4fe89a2cb1bfbc11e225b6dbc60814e44c94",
+                "sha256:45e799c1a41822eba6bee4e59b0e38764e1a1ee69873ab2889079865e9ea0e23",
+                "sha256:511d4abc823152dec49461209607bbfb2df60033c8c88a3f7c93293b8ecbb13d",
+                "sha256:557675e0befafa08d36d7a9284e8761c97490a248474d778373fb96b0d7fd8de",
+                "sha256:6572d7c96c2e3e126d0bb27bfb1d7e2a195b68d951fcc64c146b94f088e5421a",
+                "sha256:684e5c773222781775c7f77231f412633d8af22493bf35b7fa1029fdf8066d10",
+                "sha256:6a94632ba26a666e7be0a7d7cc3f7acab622a04259a3aa0ee50ff6d44ba9df0d",
+                "sha256:6b6d807c76c20b4bc143a49ad47782228a2ac98bdcdcb069da54280e138847fc",
+                "sha256:7120a2f72599d4fed7c001fa1cbbc5b4d14929436135768050e284f53e9fbe5e",
+                "sha256:71d4bf7768169c4502f6c2b0709a02a33703544f611810fb0c75406a9c576ee1",
+                "sha256:795b5b9db573d3ed61fae74285d57d396829e3157642794d3a8f72ec2a5c719b",
+                "sha256:7a4df53472c9030a8ddb1cce517757ba38a7a25699bbcabd57dcc8a5d53f324e",
+                "sha256:8f216a51451a0a0466e082e163591f6dcb2f9ec182adb3f1f4b1fd3688c7582c",
+                "sha256:95fc02f7fc1f3199aaa47a8a757437134cf618e9d994c84effd53f530c38586f",
+                "sha256:989c62b96596b7938cbc032e39431e6c2d81b635034571d6a43a13920852fb65",
+                "sha256:998e782c8d9fd57fa8704d149ccd52acf03db30d7dd76f467fd21c1c21b414fa",
+                "sha256:9a198f690ac12a3a807e03a5a45df6a30cd215935f237a46f4248faed62e69c8",
+                "sha256:a6c3929df5eeaf3867724003d5c19fed3f0c290f3edc7911616616684f200ecf",
+                "sha256:bb2797fee8a7914fb2c3dc7de404d3f96eb77f20fc60e9ee38dc6b0ca720f2c2",
+                "sha256:bd988b3362d7e586ef581eb14771bbb48793a4edb6fcf62da75d3f0f3447060b",
+                "sha256:ca8ab6748e3ec66afccd8b23ec2f92787a58d5353ce9624dccd770427ee67c82",
+                "sha256:dbe57f39f531c5d68d5594ea4613daa60aba33bb51a8cc42f96f17bbd6305e8d",
+                "sha256:dcfb480bfc9e1fab726003ae00a6bfc67a29bad275b63a4e36d17fe7f13a624e",
+                "sha256:dd45c60cc4f6d68c30d5179e2c2c8098f7112983532897566bb69c47d87127d3",
+                "sha256:dde4d02213f1deb49eaaf8be8a6425948963a7af84983b3f22772c63826944de",
+                "sha256:e3b67bda733da1dcdccaf354e71ef01b46db483a4f6236450d3f9a61efdba35a",
+                "sha256:e98ef1babe34f37f443b7211cd3ee004d9577a19766e2dbacf62fce73c76245a",
+                "sha256:f80915681ea9001f19b65aee715115f2ad310730c8043127cf3e19b3009892dd",
+                "sha256:fc700b862e0a859a37faf85367e205e7acaecae5a098794aff52fdd8aea77b12"
             ],
             "index": "pypi",
-            "version": "==1.4.46"
+            "version": "==1.4.47"
         },
         "sqlparse": {
             "hashes": [
                 "sha256:022fb9c87b524d1f7862b3037e541f68597a730a8843245c349fc93e1643dc4e",
                 "sha256:e162203737712307dfe78860cc56c8da8a852ab2ee33750e33aeadf38d12c548"
             ],
             "index": "pypi",
@@ -457,77 +444,69 @@
                 "sha256:a039f89014245e0cad8858976293e23501accc9ff5a7bdbc739a14a2b7b85cdc"
             ],
             "index": "pypi",
             "version": "==1.1.2"
         },
         "urllib3": {
             "hashes": [
-                "sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72",
-                "sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1"
+                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
+                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.14"
+            "version": "==1.26.15"
         },
         "xlrd": {
             "hashes": [
                 "sha256:6a33ee89877bd9abc1158129f6e94be74e2679636b8a205b43b85206c3f0bbdd",
                 "sha256:f72f148f54442c6b056bf931dbc34f986fd0c3b0b6b5a58d013c9aef274d0c88"
             ],
             "index": "pypi",
             "version": "==2.0.1"
         }
     },
     "develop": {
         "astroid": {
             "hashes": [
-                "sha256:0e0e3709d64fbffd3037e4ff403580550f14471fd3eaae9fa11cc9a5c7901153",
-                "sha256:a3cf9f02c53dd259144a7e8f3ccd75d67c9a8c716ef183e0c1f291bc5d7bb3cf"
+                "sha256:6e61b85c891ec53b07471aec5878f4ac6446a41e590ede0f2ce095f39f7d49dd",
+                "sha256:dea89d9f99f491c66ac9c04ebddf91e4acf8bd711722175fe6245c0725cc19bb"
             ],
             "markers": "python_full_version >= '3.7.2'",
-            "version": "==2.14.2"
-        },
-        "attrs": {
-            "hashes": [
-                "sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836",
-                "sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==22.2.0"
+            "version": "==2.15.2"
         },
         "autopep8": {
             "hashes": [
-                "sha256:be5bc98c33515b67475420b7b1feafc8d32c1a69862498eda4983b45bffd2687",
-                "sha256:d27a8929d8dcd21c0f4b3859d2d07c6c25273727b98afc984c039df0f0d86566"
+                "sha256:86e9303b5e5c8160872b2f5ef611161b2893e9bfe8ccc7e2f76385947d57a2f1",
+                "sha256:f9849cdd62108cb739dbcdbfb7fdcc9a30d1b63c4cc3e1c1f893b5360941b61c"
             ],
             "index": "pypi",
-            "version": "==2.0.1"
+            "version": "==2.0.2"
         },
         "bandit": {
             "hashes": [
-                "sha256:2d63a8c573417bae338962d4b9b06fbc6080f74ecd955a092849e1e65c717bd2",
-                "sha256:412d3f259dab4077d0e7f0c11f50f650cc7d10db905d98f6520a95a18049658a"
+                "sha256:75665181dc1e0096369112541a056c59d1c5f66f9bb74a8d686c3c362b83f549",
+                "sha256:bdfc739baa03b880c2d15d0431b31c658ffc348e907fe197e54e0389dd59e11e"
             ],
             "index": "pypi",
-            "version": "==1.7.4"
+            "version": "==1.7.5"
         },
         "dill": {
             "hashes": [
                 "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
                 "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
             ],
             "markers": "python_version < '3.11'",
             "version": "==0.3.6"
         },
         "exceptiongroup": {
             "hashes": [
-                "sha256:327cbda3da756e2de031a3107b81ab7b3770a602c4d16ca618298c526f4bec1e",
-                "sha256:bcb67d800a4497e1b404c2dd44fca47d3b7a5e5433dbab67f96c1a685cdfdf23"
+                "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
+                "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
             ],
             "markers": "python_version < '3.11'",
-            "version": "==1.1.0"
+            "version": "==1.1.1"
         },
         "flake8": {
             "hashes": [
                 "sha256:3833794e27ff64ea4e9cf5d410082a8b97ff1a06c16aa3d2027339cd0f1195c7",
                 "sha256:c61007e76655af75e6785a931f452915b371dc48f56efd765247c8fe68f2b181"
             ],
             "index": "pypi",
@@ -577,19 +556,19 @@
                 "sha256:c286cf298426064079ed96a9e4a9d39e7f3e9bf15ba60701e95f5492f28415c7"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.0.10"
         },
         "gitpython": {
             "hashes": [
-                "sha256:769c2d83e13f5d938b7688479da374c4e3d49f71549aaf462b646db9602ea6f8",
-                "sha256:cd455b0000615c60e286208ba540271af9fe531fa6a87cc590a7298785ab2882"
+                "sha256:8ce3bcf69adfdf7c7d503e78fd3b1c492af782d58893b650adb2ac8912ddd573",
+                "sha256:f04893614f6aa713a60cbbe1e6a97403ef633103cdd0ef5eb6efe0deb98dbe8d"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.1.30"
+            "version": "==3.1.31"
         },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
@@ -641,29 +620,45 @@
                 "sha256:f12ad7126ae0c98d601a7ee504c1122bcef553d1d5e0c3bfa77b16b3968d2734",
                 "sha256:f2457189d8257dd41ae9b434ba33298aec198e30adf2dcdaaa3a28b9994f6adb",
                 "sha256:f699ac1c768270c9e384e4cbd268d6e67aebcfae6cd623b4d7c3bfde5a35db59"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.9.0"
         },
+        "markdown-it-py": {
+            "hashes": [
+                "sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30",
+                "sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==2.2.0"
+        },
         "mccabe": {
             "hashes": [
                 "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325",
                 "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.7.0"
         },
+        "mdurl": {
+            "hashes": [
+                "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8",
+                "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==0.1.2"
+        },
         "more-itertools": {
             "hashes": [
-                "sha256:250e83d7e81d0c87ca6bd942e6aeab8cc9daa6096d12c5308f3f92fa5e5c1f41",
-                "sha256:5a6257e40878ef0520b1803990e3e22303a41b5714006c32a3fd8304b26ea1ab"
+                "sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d",
+                "sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3"
             ],
             "index": "pypi",
-            "version": "==9.0.0"
+            "version": "==9.1.0"
         },
         "packaging": {
             "hashes": [
                 "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
                 "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
             ],
             "markers": "python_version >= '3.7'",
@@ -683,19 +678,19 @@
                 "sha256:fe249b52e20498e59e0b5c5256aa52ee99fc295b26ec9eaa85776ffdb9fe6374"
             ],
             "index": "pypi",
             "version": "==1.7.1"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:8a1228abb1ef82d788f74139988b137e78692984ec7b08eaa6c65f1723af28f9",
-                "sha256:b1d5eb14f221506f50d6604a561f4c5786d9e80355219694a1b244bcd96f4567"
+                "sha256:d5b638ca397f25f979350ff789db335903d7ea010ab28903f57b27e1b16c2b08",
+                "sha256:ebe11c0d7a805086e99506aa331612429a72ca7cd52a1f0d277dc4adc20cb10e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.0.0"
+            "version": "==3.2.0"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
@@ -721,29 +716,37 @@
             "hashes": [
                 "sha256:ec55bf7fe21fff7f1ad2f7da62363d749e2a470500eab1b555334b67aa1ef8cf",
                 "sha256:ec8b276a6b60bd80defed25add7e439881c19e64850afd9b346283d4165fd0fd"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==3.0.1"
         },
+        "pygments": {
+            "hashes": [
+                "sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297",
+                "sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==2.14.0"
+        },
         "pylint": {
             "hashes": [
-                "sha256:13b2c805a404a9bf57d002cd5f054ca4d40b0b87542bdaba5e05321ae8262c84",
-                "sha256:ff22dde9c2128cd257c145cfd51adeff0be7df4d80d669055f24a962b351bbe4"
+                "sha256:001cc91366a7df2970941d7e6bbefcbf98694e00102c1f121c531a814ddc2ea8",
+                "sha256:1b647da5249e7c279118f657ca28b6aaebb299f86bf92affc632acf199f7adbb"
             ],
             "index": "pypi",
-            "version": "==2.16.2"
+            "version": "==2.17.2"
         },
         "pytest": {
             "hashes": [
-                "sha256:c7c6ca206e93355074ae32f7403e8ea12163b1163c976fee7d4d84027c162be5",
-                "sha256:d45e0952f3727241918b8fd0f376f5ff6b301cc0777c6f9a556935c92d8a7d42"
+                "sha256:58ecc27ebf0ea643ebfdf7fb1249335da761a00c9f955bcd922349bcb68ee57d",
+                "sha256:933051fa1bfbd38a21e73c3960cebdad4cf59483ddba7696c48509727e17f201"
             ],
             "index": "pypi",
-            "version": "==7.2.1"
+            "version": "==7.3.0"
         },
         "pyyaml": {
             "hashes": [
                 "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
                 "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
                 "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
                 "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
@@ -783,14 +786,22 @@
                 "sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f",
                 "sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174",
                 "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==6.0"
         },
+        "rich": {
+            "hashes": [
+                "sha256:540c7d6d26a1178e8e8b37e9ba44573a3cd1464ff6348b99ee7061b95d1c6333",
+                "sha256:dc84400a9d842b3a9c5ff74addd8eb798d155f36c1c91303888e0a66850d2a15"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==13.3.3"
+        },
         "smmap": {
             "hashes": [
                 "sha256:2aba19d6a040e78d8b09de5c57e96207b09ed71d8e55ce0959eeee6c8e190d94",
                 "sha256:c840e62059cd3be204b0c9c9f74be2c09d5648eddd4580d9314c3ecde0b30936"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==5.0.0"
@@ -816,93 +827,104 @@
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version < '3.11'",
             "version": "==2.0.1"
         },
         "tomlkit": {
             "hashes": [
-                "sha256:07de26b0d8cfc18f871aec595fda24d95b08fef89d147caa861939f37230bf4b",
-                "sha256:71b952e5721688937fb02cf9d354dbcf0785066149d2855e44531ebdd2b65d73"
+                "sha256:5325463a7da2ef0c6bbfefb62a3dc883aebe679984709aee32a317907d0a8d3c",
+                "sha256:f392ef70ad87a672f02519f99967d28a4d3047133e2d1df936511465fbb3791d"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==0.11.6"
+            "markers": "python_version >= '3.7'",
+            "version": "==0.11.7"
         },
         "typing-extensions": {
             "hashes": [
                 "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
                 "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version < '3.11'",
             "version": "==4.5.0"
         },
         "wrapt": {
             "hashes": [
-                "sha256:00b6d4ea20a906c0ca56d84f93065b398ab74b927a7a3dbd470f6fc503f95dc3",
-                "sha256:01c205616a89d09827986bc4e859bcabd64f5a0662a7fe95e0d359424e0e071b",
-                "sha256:02b41b633c6261feff8ddd8d11c711df6842aba629fdd3da10249a53211a72c4",
-                "sha256:07f7a7d0f388028b2df1d916e94bbb40624c59b48ecc6cbc232546706fac74c2",
-                "sha256:11871514607b15cfeb87c547a49bca19fde402f32e2b1c24a632506c0a756656",
-                "sha256:1b376b3f4896e7930f1f772ac4b064ac12598d1c38d04907e696cc4d794b43d3",
-                "sha256:21ac0156c4b089b330b7666db40feee30a5d52634cc4560e1905d6529a3897ff",
-                "sha256:257fd78c513e0fb5cdbe058c27a0624c9884e735bbd131935fd49e9fe719d310",
-                "sha256:2b39d38039a1fdad98c87279b48bc5dce2c0ca0d73483b12cb72aa9609278e8a",
-                "sha256:2cf71233a0ed05ccdabe209c606fe0bac7379fdcf687f39b944420d2a09fdb57",
-                "sha256:2fe803deacd09a233e4762a1adcea5db5d31e6be577a43352936179d14d90069",
-                "sha256:3232822c7d98d23895ccc443bbdf57c7412c5a65996c30442ebe6ed3df335383",
-                "sha256:34aa51c45f28ba7f12accd624225e2b1e5a3a45206aa191f6f9aac931d9d56fe",
-                "sha256:36f582d0c6bc99d5f39cd3ac2a9062e57f3cf606ade29a0a0d6b323462f4dd87",
-                "sha256:380a85cf89e0e69b7cfbe2ea9f765f004ff419f34194018a6827ac0e3edfed4d",
-                "sha256:40e7bc81c9e2b2734ea4bc1aceb8a8f0ceaac7c5299bc5d69e37c44d9081d43b",
-                "sha256:43ca3bbbe97af00f49efb06e352eae40434ca9d915906f77def219b88e85d907",
-                "sha256:4fcc4649dc762cddacd193e6b55bc02edca674067f5f98166d7713b193932b7f",
-                "sha256:5a0f54ce2c092aaf439813735584b9537cad479575a09892b8352fea5e988dc0",
-                "sha256:5a9a0d155deafd9448baff28c08e150d9b24ff010e899311ddd63c45c2445e28",
-                "sha256:5b02d65b9ccf0ef6c34cba6cf5bf2aab1bb2f49c6090bafeecc9cd81ad4ea1c1",
-                "sha256:60db23fa423575eeb65ea430cee741acb7c26a1365d103f7b0f6ec412b893853",
-                "sha256:642c2e7a804fcf18c222e1060df25fc210b9c58db7c91416fb055897fc27e8cc",
-                "sha256:6a9a25751acb379b466ff6be78a315e2b439d4c94c1e99cb7266d40a537995d3",
-                "sha256:6b1a564e6cb69922c7fe3a678b9f9a3c54e72b469875aa8018f18b4d1dd1adf3",
-                "sha256:6d323e1554b3d22cfc03cd3243b5bb815a51f5249fdcbb86fda4bf62bab9e164",
-                "sha256:6e743de5e9c3d1b7185870f480587b75b1cb604832e380d64f9504a0535912d1",
-                "sha256:709fe01086a55cf79d20f741f39325018f4df051ef39fe921b1ebe780a66184c",
-                "sha256:7b7c050ae976e286906dd3f26009e117eb000fb2cf3533398c5ad9ccc86867b1",
-                "sha256:7d2872609603cb35ca513d7404a94d6d608fc13211563571117046c9d2bcc3d7",
-                "sha256:7ef58fb89674095bfc57c4069e95d7a31cfdc0939e2a579882ac7d55aadfd2a1",
-                "sha256:80bb5c256f1415f747011dc3604b59bc1f91c6e7150bd7db03b19170ee06b320",
-                "sha256:81b19725065dcb43df02b37e03278c011a09e49757287dca60c5aecdd5a0b8ed",
-                "sha256:833b58d5d0b7e5b9832869f039203389ac7cbf01765639c7309fd50ef619e0b1",
-                "sha256:88bd7b6bd70a5b6803c1abf6bca012f7ed963e58c68d76ee20b9d751c74a3248",
-                "sha256:8ad85f7f4e20964db4daadcab70b47ab05c7c1cf2a7c1e51087bfaa83831854c",
-                "sha256:8c0ce1e99116d5ab21355d8ebe53d9460366704ea38ae4d9f6933188f327b456",
-                "sha256:8d649d616e5c6a678b26d15ece345354f7c2286acd6db868e65fcc5ff7c24a77",
-                "sha256:903500616422a40a98a5a3c4ff4ed9d0066f3b4c951fa286018ecdf0750194ef",
-                "sha256:9736af4641846491aedb3c3f56b9bc5568d92b0692303b5a305301a95dfd38b1",
-                "sha256:988635d122aaf2bdcef9e795435662bcd65b02f4f4c1ae37fbee7401c440b3a7",
-                "sha256:9cca3c2cdadb362116235fdbd411735de4328c61425b0aa9f872fd76d02c4e86",
-                "sha256:9e0fd32e0148dd5dea6af5fee42beb949098564cc23211a88d799e434255a1f4",
-                "sha256:9f3e6f9e05148ff90002b884fbc2a86bd303ae847e472f44ecc06c2cd2fcdb2d",
-                "sha256:a85d2b46be66a71bedde836d9e41859879cc54a2a04fad1191eb50c2066f6e9d",
-                "sha256:a9a52172be0b5aae932bef82a79ec0a0ce87288c7d132946d645eba03f0ad8a8",
-                "sha256:aa31fdcc33fef9eb2552cbcbfee7773d5a6792c137b359e82879c101e98584c5",
-                "sha256:b014c23646a467558be7da3d6b9fa409b2c567d2110599b7cf9a0c5992b3b471",
-                "sha256:b21bb4c09ffabfa0e85e3a6b623e19b80e7acd709b9f91452b8297ace2a8ab00",
-                "sha256:b5901a312f4d14c59918c221323068fad0540e34324925c8475263841dbdfe68",
-                "sha256:b9b7a708dd92306328117d8c4b62e2194d00c365f18eff11a9b53c6f923b01e3",
-                "sha256:d1967f46ea8f2db647c786e78d8cc7e4313dbd1b0aca360592d8027b8508e24d",
-                "sha256:d52a25136894c63de15a35bc0bdc5adb4b0e173b9c0d07a2be9d3ca64a332735",
-                "sha256:d77c85fedff92cf788face9bfa3ebaa364448ebb1d765302e9af11bf449ca36d",
-                "sha256:d79d7d5dc8a32b7093e81e97dad755127ff77bcc899e845f41bf71747af0c569",
-                "sha256:dbcda74c67263139358f4d188ae5faae95c30929281bc6866d00573783c422b7",
-                "sha256:ddaea91abf8b0d13443f6dac52e89051a5063c7d014710dcb4d4abb2ff811a59",
-                "sha256:dee0ce50c6a2dd9056c20db781e9c1cfd33e77d2d569f5d1d9321c641bb903d5",
-                "sha256:dee60e1de1898bde3b238f18340eec6148986da0455d8ba7848d50470a7a32fb",
-                "sha256:e2f83e18fe2f4c9e7db597e988f72712c0c3676d337d8b101f6758107c42425b",
-                "sha256:e3fb1677c720409d5f671e39bac6c9e0e422584e5f518bfd50aa4cbbea02433f",
-                "sha256:ee2b1b1769f6707a8a445162ea16dddf74285c3964f605877a20e38545c3c462",
-                "sha256:ee6acae74a2b91865910eef5e7de37dc6895ad96fa23603d1d27ea69df545015",
-                "sha256:ef3f72c9666bba2bab70d2a8b79f2c6d2c1a42a7f7e2b0ec83bb2f9e383950af"
+                "sha256:02fce1852f755f44f95af51f69d22e45080102e9d00258053b79367d07af39c0",
+                "sha256:077ff0d1f9d9e4ce6476c1a924a3332452c1406e59d90a2cf24aeb29eeac9420",
+                "sha256:078e2a1a86544e644a68422f881c48b84fef6d18f8c7a957ffd3f2e0a74a0d4a",
+                "sha256:0970ddb69bba00670e58955f8019bec4a42d1785db3faa043c33d81de2bf843c",
+                "sha256:1286eb30261894e4c70d124d44b7fd07825340869945c79d05bda53a40caa079",
+                "sha256:21f6d9a0d5b3a207cdf7acf8e58d7d13d463e639f0c7e01d82cdb671e6cb7923",
+                "sha256:230ae493696a371f1dbffaad3dafbb742a4d27a0afd2b1aecebe52b740167e7f",
+                "sha256:26458da5653aa5b3d8dc8b24192f574a58984c749401f98fff994d41d3f08da1",
+                "sha256:2cf56d0e237280baed46f0b5316661da892565ff58309d4d2ed7dba763d984b8",
+                "sha256:2e51de54d4fb8fb50d6ee8327f9828306a959ae394d3e01a1ba8b2f937747d86",
+                "sha256:2fbfbca668dd15b744418265a9607baa970c347eefd0db6a518aaf0cfbd153c0",
+                "sha256:38adf7198f8f154502883242f9fe7333ab05a5b02de7d83aa2d88ea621f13364",
+                "sha256:3a8564f283394634a7a7054b7983e47dbf39c07712d7b177b37e03f2467a024e",
+                "sha256:3abbe948c3cbde2689370a262a8d04e32ec2dd4f27103669a45c6929bcdbfe7c",
+                "sha256:3bbe623731d03b186b3d6b0d6f51865bf598587c38d6f7b0be2e27414f7f214e",
+                "sha256:40737a081d7497efea35ab9304b829b857f21558acfc7b3272f908d33b0d9d4c",
+                "sha256:41d07d029dd4157ae27beab04d22b8e261eddfc6ecd64ff7000b10dc8b3a5727",
+                "sha256:46ed616d5fb42f98630ed70c3529541408166c22cdfd4540b88d5f21006b0eff",
+                "sha256:493d389a2b63c88ad56cdc35d0fa5752daac56ca755805b1b0c530f785767d5e",
+                "sha256:4ff0d20f2e670800d3ed2b220d40984162089a6e2c9646fdb09b85e6f9a8fc29",
+                "sha256:54accd4b8bc202966bafafd16e69da9d5640ff92389d33d28555c5fd4f25ccb7",
+                "sha256:56374914b132c702aa9aa9959c550004b8847148f95e1b824772d453ac204a72",
+                "sha256:578383d740457fa790fdf85e6d346fda1416a40549fe8db08e5e9bd281c6a475",
+                "sha256:58d7a75d731e8c63614222bcb21dd992b4ab01a399f1f09dd82af17bbfc2368a",
+                "sha256:5c5aa28df055697d7c37d2099a7bc09f559d5053c3349b1ad0c39000e611d317",
+                "sha256:5fc8e02f5984a55d2c653f5fea93531e9836abbd84342c1d1e17abc4a15084c2",
+                "sha256:63424c681923b9f3bfbc5e3205aafe790904053d42ddcc08542181a30a7a51bd",
+                "sha256:64b1df0f83706b4ef4cfb4fb0e4c2669100fd7ecacfb59e091fad300d4e04640",
+                "sha256:74934ebd71950e3db69960a7da29204f89624dde411afbfb3b4858c1409b1e98",
+                "sha256:75669d77bb2c071333417617a235324a1618dba66f82a750362eccbe5b61d248",
+                "sha256:75760a47c06b5974aa5e01949bf7e66d2af4d08cb8c1d6516af5e39595397f5e",
+                "sha256:76407ab327158c510f44ded207e2f76b657303e17cb7a572ffe2f5a8a48aa04d",
+                "sha256:76e9c727a874b4856d11a32fb0b389afc61ce8aaf281ada613713ddeadd1cfec",
+                "sha256:77d4c1b881076c3ba173484dfa53d3582c1c8ff1f914c6461ab70c8428b796c1",
+                "sha256:780c82a41dc493b62fc5884fb1d3a3b81106642c5c5c78d6a0d4cbe96d62ba7e",
+                "sha256:7dc0713bf81287a00516ef43137273b23ee414fe41a3c14be10dd95ed98a2df9",
+                "sha256:7eebcdbe3677e58dd4c0e03b4f2cfa346ed4049687d839adad68cc38bb559c92",
+                "sha256:896689fddba4f23ef7c718279e42f8834041a21342d95e56922e1c10c0cc7afb",
+                "sha256:96177eb5645b1c6985f5c11d03fc2dbda9ad24ec0f3a46dcce91445747e15094",
+                "sha256:96e25c8603a155559231c19c0349245eeb4ac0096fe3c1d0be5c47e075bd4f46",
+                "sha256:9d37ac69edc5614b90516807de32d08cb8e7b12260a285ee330955604ed9dd29",
+                "sha256:9ed6aa0726b9b60911f4aed8ec5b8dd7bf3491476015819f56473ffaef8959bd",
+                "sha256:a487f72a25904e2b4bbc0817ce7a8de94363bd7e79890510174da9d901c38705",
+                "sha256:a4cbb9ff5795cd66f0066bdf5947f170f5d63a9274f99bdbca02fd973adcf2a8",
+                "sha256:a74d56552ddbde46c246b5b89199cb3fd182f9c346c784e1a93e4dc3f5ec9975",
+                "sha256:a89ce3fd220ff144bd9d54da333ec0de0399b52c9ac3d2ce34b569cf1a5748fb",
+                "sha256:abd52a09d03adf9c763d706df707c343293d5d106aea53483e0ec8d9e310ad5e",
+                "sha256:abd8f36c99512755b8456047b7be10372fca271bf1467a1caa88db991e7c421b",
+                "sha256:af5bd9ccb188f6a5fdda9f1f09d9f4c86cc8a539bd48a0bfdc97723970348418",
+                "sha256:b02f21c1e2074943312d03d243ac4388319f2456576b2c6023041c4d57cd7019",
+                "sha256:b06fa97478a5f478fb05e1980980a7cdf2712015493b44d0c87606c1513ed5b1",
+                "sha256:b0724f05c396b0a4c36a3226c31648385deb6a65d8992644c12a4963c70326ba",
+                "sha256:b130fe77361d6771ecf5a219d8e0817d61b236b7d8b37cc045172e574ed219e6",
+                "sha256:b56d5519e470d3f2fe4aa7585f0632b060d532d0696c5bdfb5e8319e1d0f69a2",
+                "sha256:b67b819628e3b748fd3c2192c15fb951f549d0f47c0449af0764d7647302fda3",
+                "sha256:ba1711cda2d30634a7e452fc79eabcadaffedf241ff206db2ee93dd2c89a60e7",
+                "sha256:bbeccb1aa40ab88cd29e6c7d8585582c99548f55f9b2581dfc5ba68c59a85752",
+                "sha256:bd84395aab8e4d36263cd1b9308cd504f6cf713b7d6d3ce25ea55670baec5416",
+                "sha256:c99f4309f5145b93eca6e35ac1a988f0dc0a7ccf9ccdcd78d3c0adf57224e62f",
+                "sha256:ca1cccf838cd28d5a0883b342474c630ac48cac5df0ee6eacc9c7290f76b11c1",
+                "sha256:cd525e0e52a5ff16653a3fc9e3dd827981917d34996600bbc34c05d048ca35cc",
+                "sha256:cdb4f085756c96a3af04e6eca7f08b1345e94b53af8921b25c72f096e704e145",
+                "sha256:ce42618f67741d4697684e501ef02f29e758a123aa2d669e2d964ff734ee00ee",
+                "sha256:d06730c6aed78cee4126234cf2d071e01b44b915e725a6cb439a879ec9754a3a",
+                "sha256:d5fe3e099cf07d0fb5a1e23d399e5d4d1ca3e6dfcbe5c8570ccff3e9208274f7",
+                "sha256:d6bcbfc99f55655c3d93feb7ef3800bd5bbe963a755687cbf1f490a71fb7794b",
+                "sha256:d787272ed958a05b2c86311d3a4135d3c2aeea4fc655705f074130aa57d71653",
+                "sha256:e169e957c33576f47e21864cf3fc9ff47c223a4ebca8960079b8bd36cb014fd0",
+                "sha256:e20076a211cd6f9b44a6be58f7eeafa7ab5720eb796975d0c03f05b47d89eb90",
+                "sha256:e826aadda3cae59295b95343db8f3d965fb31059da7de01ee8d1c40a60398b29",
+                "sha256:eef4d64c650f33347c1f9266fa5ae001440b232ad9b98f1f43dfe7a79435c0a6",
+                "sha256:f2e69b3ed24544b0d3dbe2c5c0ba5153ce50dcebb576fdc4696d52aa22db6034",
+                "sha256:f87ec75864c37c4c6cb908d282e1969e79763e0d9becdfe9fe5473b7bb1e5f09",
+                "sha256:fbec11614dba0424ca72f4e8ba3c420dba07b4a7c206c8c8e4e73f2e98f4c559",
+                "sha256:fd69666217b62fa5d7c6aa88e507493a34dec4fa20c5bd925e4bc12fce586639"
             ],
             "markers": "python_version < '3.11'",
-            "version": "==1.14.1"
+            "version": "==1.15.0"
         }
     }
 }
```

### Comparing `etlstat-0.9.0/docs/source/conf.py` & `etlstat-0.9.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/database/README.rst` & `etlstat-0.9.1/etlstat/database/README.rst`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/database/mysql.py` & `etlstat-0.9.1/etlstat/database/mysql.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/database/oracle.py` & `etlstat-0.9.1/etlstat/database/oracle.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/database/postgresql.py` & `etlstat-0.9.1/etlstat/database/postgresql.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/database/test/22350.px` & `etlstat-0.9.1/etlstat/database/test/22350.px`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/database/test/pmh.csv` & `etlstat-0.9.1/etlstat/database/test/pmh.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/database/test/px_01001.csv` & `etlstat-0.9.1/etlstat/database/test/px_01001.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/database/test/test_mysql.py` & `etlstat-0.9.1/etlstat/database/test/test_mysql.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/database/test/test_oracle.py` & `etlstat-0.9.1/etlstat/database/test/test_oracle.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/database/test/test_postgresql.py` & `etlstat-0.9.1/etlstat/database/test/test_postgresql.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/database/test/test_sqlloader.py` & `etlstat-0.9.1/etlstat/database/test/test_sqlloader.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/extractor.py` & `etlstat-0.9.1/etlstat/extractor/extractor.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/csv/AGENV_SER_06_15.csv` & `etlstat-0.9.1/etlstat/extractor/test/data/csv/AGENV_SER_06_15.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/csv/ALOJ_SER_06_15.csv` & `etlstat-0.9.1/etlstat/extractor/test/data/csv/ALOJ_SER_06_15.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/excel/excel_prueba.xls` & `etlstat-0.9.1/etlstat/extractor/test/data/excel/excel_prueba.xls`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/excel/prueba_excel.xls` & `etlstat-0.9.1/etlstat/extractor/test/data/excel/prueba_excel.xls`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/AEREO_SER_06_15.TXT` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/AEREO_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/AGENV_SER_06_15.TXT` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/AGENV_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/ALOJ_SER_06_15.TXT` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/ALOJ_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/AUDIOV_SER_06_15.TXT` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/AUDIOV_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/CONS_SER_06_15.TXT` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/CONS_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/INFOR_SER_06_15.TXT` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/INFOR_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/JURID_SER_06_15.TXT` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/JURID_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/LIMPI_SER_06_15.TXT` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/LIMPI_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/MAYOR_COM_06_15.TXT` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/MAYOR_COM_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/MENOR_COM_06_15.TXT` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/MENOR_COM_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/OPIN_SER_06_15.TXT` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/OPIN_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/PERSON_SER_06_15.TXT` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/PERSON_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/POST_SER_06_15.TXT` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/POST_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/PUBLI_SER_06_15.TXT` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/PUBLI_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/SSCC_SER_06_15.TXT` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/SSCC_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/TEC_SER_06_15.TXT` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/TEC_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/TFERR_SER_06_15.TXT` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/TFERR_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/TMAR_SER_06_15.TXT` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/TMAR_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/TMER_SER_06_15.TXT` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/TMER_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/TUI_SER_06_15.TXT` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/TUI_SER_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/VEHIC_COM_06_15.TXT` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/VEHIC_COM_06_15.TXT`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/format/AEREO_SER_formato.csv` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/AEREO_SER_formato.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/format/AGENV_SER_formato.csv` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/AGENV_SER_formato.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/format/CONS_SER.csv` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/CONS_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/format/INFOR_SER.csv` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/INFOR_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/format/JURID_SER.csv` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/JURID_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/format/MAYOR_COM.csv` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/MAYOR_COM.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/format/MENOR_COM.csv` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/MENOR_COM.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/format/PERSON_SER.csv` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/PERSON_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/format/POST_SER.csv` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/POST_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/format/PUBLI_SER.csv` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/PUBLI_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/format/TEC_SER.csv` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/TEC_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/format/TFERR_SER.csv` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/TFERR_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/format/TMER_SER.csv` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/TMER_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/format/TUI_SER.csv` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/TUI_SER.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/positional/format/VEHIC_COM.csv` & `etlstat-0.9.1/etlstat/extractor/test/data/positional/format/VEHIC_COM.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/px/o20012.px` & `etlstat-0.9.1/etlstat/extractor/test/data/px/o20012.px`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/px/o20013.px` & `etlstat-0.9.1/etlstat/extractor/test/data/px/o20013.px`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/px_file/27066.px` & `etlstat-0.9.1/etlstat/extractor/test/data/px_file/27066.px`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/sql/afiliados.sql` & `etlstat-0.9.1/etlstat/extractor/test/data/sql/afiliados.sql`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/sql/contratos.sql` & `etlstat-0.9.1/etlstat/extractor/test/data/sql/contratos.sql`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/sql/ratios.sql` & `etlstat-0.9.1/etlstat/extractor/test/data/sql/ratios.sql`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/xml/Comex.kjb` & `etlstat-0.9.1/etlstat/extractor/test/data/xml/Comex.kjb`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/xml/Ec_SE_BalanzaCom.ktr` & `etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_BalanzaCom.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/xml/Ec_SE_IEFAD.ktr` & `etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFAD.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/xml/Ec_SE_IEFAE.ktr` & `etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFAE.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/xml/Ec_SE_IEFAZ.ktr` & `etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFAZ.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/xml/Ec_SE_IEFDZ.ktr` & `etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFDZ.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/xml/Ec_SE_IEFPZ.ktr` & `etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFPZ.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/xml/Ec_SE_IEFSC.ktr` & `etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFSC.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/xml/Ec_SE_IEFSEC.ktr` & `etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFSEC.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/xml/Ec_SE_IEFTZ.ktr` & `etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IEFTZ.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/data/xml/Ec_SE_IndPosComPreCon99_hechos_v.2.ktr` & `etlstat-0.9.1/etlstat/extractor/test/data/xml/Ec_SE_IndPosComPreCon99_hechos_v.2.ktr`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/extractor/test/test_extractor.py` & `etlstat-0.9.1/etlstat/extractor/test/test_extractor.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/log/logging.py` & `etlstat-0.9.1/etlstat/log/logging.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/log/timing.py` & `etlstat-0.9.1/etlstat/log/timing.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/text/test/data/jobs/TODAS_Uso de Comercio Electrónico.kjb` & `etlstat-0.9.1/etlstat/text/test/data/jobs/TODAS_Uso de Comercio Electrónico.kjb`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/text/test/data/jobs/Uso com_elec.csv` & `etlstat-0.9.1/etlstat/text/test/data/jobs/Uso com_elec.csv`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/text/test/data/output/TODAS_Uso de Comercio Electrónico.kjb` & `etlstat-0.9.1/etlstat/text/test/data/output/TODAS_Uso de Comercio Electrónico.kjb`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/text/test/test_utils.py` & `etlstat-0.9.1/etlstat/text/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat/text/utils.py` & `etlstat-0.9.1/etlstat/text/utils.py`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/etlstat.egg-info/PKG-INFO` & `etlstat-0.9.1/etlstat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etlstat
-Version: 0.9.0
+Version: 0.9.1
 Summary: ETL utils for statistical offices data processing
 Home-page: https://github.com/icane/etlstat.git
 Author: Instituto Cántabro de Estadística
 Author-email: icane@cantabria.es
 License: Apache License 2.0
 Keywords: etl,icane,statistics,utils
 Classifier: Development Status :: 4 - Beta
```

### Comparing `etlstat-0.9.0/etlstat.egg-info/SOURCES.txt` & `etlstat-0.9.1/etlstat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etlstat-0.9.0/requirements.txt` & `etlstat-0.9.1/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,33 +2,34 @@
 # These requirements were autogenerated by pipenv
 # To regenerate from the project's Pipfile, run:
 #
 #    pipenv lock --requirements
 #
 
 -i https://pypi.org/simple
-beautifulsoup4==4.11.2
+beautifulsoup4==4.12.2
 certifi==2022.12.7; python_version >= '3.6'
-charset-normalizer==3.0.1; python_full_version >= '3.6.0'
+charset-normalizer==3.1.0; python_version >= '3.7'
 cx-oracle==7.3.0
 defusedxml==0.6.0
 et-xmlfile==1.1.0; python_version >= '3.6'
 greenlet==2.0.2; python_version >= '3' and platform_machine == 'aarch64' or (platform_machine == 'ppc64le' or (platform_machine == 'x86_64' or (platform_machine == 'amd64' or (platform_machine == 'AMD64' or (platform_machine == 'win32' or platform_machine == 'WIN32')))))
 idna==3.4; python_version >= '3.5'
 mysql-connector==2.2.9
 numpy==1.23.5
 openpyxl==3.0.10
 pandas==1.4.4
 psycopg2==2.8.6
 pyaxis==0.3.4
-pyjstat==2.3.0
+pyjstat==2.4.0
 python-dateutil==2.8.2; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 python-levenshtein==0.12.2
-pytz==2022.7.1
+pytz==2023.3
 requests==2.28.2; python_version >= '3.7' and python_version < '4'
 six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 soupsieve==2.4; python_version >= '3.7'
-sqlalchemy==1.4.46
+sqlalchemy==1.4.47
 sqlparse==0.3.1
 unidecode==1.1.2
-urllib3==1.26.14; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'
+urllib3==1.26.15; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'
 xlrd==2.0.1
+
```

### Comparing `etlstat-0.9.0/setup.py` & `etlstat-0.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 # -*- coding: utf-8 -*-
 from setuptools import find_packages, setup
 
 setup(
     name='etlstat',
-    version='0.9.0',
+    version='0.9.1',
     author='Instituto Cántabro de Estadística',
     author_email='icane@cantabria.es',
     packages=find_packages(),
     url='https://github.com/icane/etlstat.git',
     license='Apache License 2.0',
     description='ETL utils for statistical offices data processing',
     long_description=open('README.rst').read(),
     install_requires=[
-        'beautifulsoup4==4.11.2',
+        'beautifulsoup4==4.12.2',
         'certifi==2022.12.7',
-        'charset-normalizer==3.0.1',
+        'charset-normalizer==3.1.0',
         'cx-oracle==7.3.0',
         'defusedxml==0.6.0',
         'et-xmlfile==1.1.0',
         'greenlet==2.0.2',
         'idna==3.4',
         'mysql-connector==2.2.9',
         'numpy==1.23.5',
         'openpyxl==3.0.10',
         'pandas==1.4.4',
         'psycopg2==2.8.6',
         'pyaxis==0.3.4',
-        'pyjstat==2.3.0',
+        'pyjstat==2.4.0',
         'python-dateutil==2.8.2',
         'python-levenshtein==0.12.2',
-        'pytz==2022.7.1',
+        'pytz==2023.3',
         'requests==2.28.2',
         'six==1.16.0',
         'soupsieve==2.4',
-        'sqlalchemy==1.4.46',
+        'sqlalchemy==1.4.47',
         'sqlparse==0.3.1',
         'unidecode==1.1.2',
-        'urllib3==1.26.14',
-        'xlrd==2.0.1',
+        'urllib3==1.26.15',
+        'xlrd==2.0.1'
     ],
     test_suite='extractor.test, database.test, text.test',
     keywords=['etl', 'icane', 'statistics', 'utils'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Console',
         'Intended Audience :: Developers',
```

