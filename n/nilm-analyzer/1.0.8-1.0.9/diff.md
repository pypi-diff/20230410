# Comparing `tmp/nilm_analyzer-1.0.8.tar.gz` & `tmp/nilm_analyzer-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nilm_analyzer-1.0.8.tar", last modified: Mon Feb 27 21:33:50 2023, max compression
+gzip compressed data, was "nilm_analyzer-1.0.9.tar", last modified: Thu Mar  2 15:10:30 2023, max compression
```

## Comparing `nilm_analyzer-1.0.8.tar` & `nilm_analyzer-1.0.9.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:50.746879 nilm_analyzer-1.0.8/
--rw-rw-rw-   0        0        0     1090 2023-02-19 14:22:00.000000 nilm_analyzer-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     1343 2023-02-19 17:43:39.000000 nilm_analyzer-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5984 2023-02-27 21:33:50.731236 nilm_analyzer-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4196 2023-02-27 20:54:44.000000 nilm_analyzer-1.0.8/README2.md
--rw-rw-rw-   0        0        0     1121 2023-02-27 21:32:47.000000 nilm_analyzer-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-27 21:33:50.746879 nilm_analyzer-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:49.412886 nilm_analyzer-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:49.576751 nilm_analyzer-1.0.8/src/nilm_analyzer/
--rw-rw-rw-   0        0        0        0 2023-02-20 09:45:12.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/__init__.py
--rw-rw-rw-   0        0        0    74514 2023-02-24 01:00:46.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/loaders.py
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:49.655337 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/
--rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:49.670959 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/ampds/
--rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/ampds/__init__.py
--rw-rw-rw-   0        0        0     3165 2023-01-17 18:36:04.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/ampds/building1.yaml
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:49.859457 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/deddiag/
--rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/deddiag/__init__.py
--rw-rw-rw-   0        0        0       60 2021-01-19 08:13:42.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/deddiag/house_00.tsv
--rw-rw-rw-   0        0        0      117 2021-01-19 08:25:26.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/deddiag/house_01.tsv
--rw-rw-rw-   0        0        0       87 2021-01-19 08:27:11.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/deddiag/house_02.tsv
--rw-rw-rw-   0        0        0      142 2021-01-19 09:02:35.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/deddiag/house_03.tsv
--rw-rw-rw-   0        0        0      170 2021-01-19 09:49:58.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/deddiag/house_04.tsv
--rw-rw-rw-   0        0        0      193 2021-01-19 10:44:05.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/deddiag/house_05.tsv
--rw-rw-rw-   0        0        0      256 2021-01-19 11:09:17.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/deddiag/house_06.tsv
--rw-rw-rw-   0        0        0      159 2021-01-19 11:25:01.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/deddiag/house_07.tsv
--rw-rw-rw-   0        0        0      408 2021-01-19 11:52:15.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/deddiag/house_08.tsv
--rw-rw-rw-   0        0        0      126 2021-01-19 12:47:33.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/deddiag/house_09.tsv
--rw-rw-rw-   0        0        0      129 2021-01-19 13:18:21.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/deddiag/house_10.tsv
--rw-rw-rw-   0        0        0       47 2021-01-19 13:45:02.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/deddiag/house_11.tsv
--rw-rw-rw-   0        0        0      147 2021-01-19 13:45:16.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/deddiag/house_12.tsv
--rw-rw-rw-   0        0        0      129 2021-01-19 13:49:58.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/deddiag/house_13.tsv
--rw-rw-rw-   0        0        0      121 2021-01-19 14:04:28.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/deddiag/house_14.tsv
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:49.875082 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/
--rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:49.890704 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-01/
--rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-01/__init__.py
--rw-rw-rw-   0        0        0     2057 2021-02-17 14:17:58.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-01/info.json
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:49.913844 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-02/
--rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-02/__init__.py
--rw-rw-rw-   0        0        0     1976 2021-02-17 14:18:33.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-02/info.json
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:49.922360 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-03/
--rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-03/__init__.py
--rw-rw-rw-   0        0        0     1999 2021-02-17 14:19:34.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-03/info.json
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:49.953637 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-04/
--rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-04/__init__.py
--rw-rw-rw-   0        0        0     2051 2021-02-17 14:20:29.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-04/info.json
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:49.969285 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-05/
--rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-05/__init__.py
--rw-rw-rw-   0        0        0     2048 2021-02-17 14:22:18.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-05/info.json
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:49.984879 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-06/
--rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-06/__init__.py
--rw-rw-rw-   0        0        0     2194 2021-02-17 14:23:27.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-06/info.json
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:50.016569 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-07/
--rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-07/__init__.py
--rw-rw-rw-   0        0        0     1985 2021-02-17 14:24:36.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-07/info.json
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:50.032213 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-08/
--rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-08/__init__.py
--rw-rw-rw-   0        0        0     2055 2021-02-17 14:25:41.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-08/info.json
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:50.047838 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-09/
--rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-09/__init__.py
--rw-rw-rw-   0        0        0     2061 2021-02-17 14:27:29.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-09/info.json
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:50.063459 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-10/
--rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-10/__init__.py
--rw-rw-rw-   0        0        0     2058 2021-02-17 14:28:06.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-10/info.json
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:50.079085 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-11/
--rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-11/__init__.py
--rw-rw-rw-   0        0        0     2023 2021-02-17 14:29:09.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-11/info.json
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:50.114351 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-12/
--rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-12/__init__.py
--rw-rw-rw-   0        0        0     2047 2021-02-17 14:30:04.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-12/info.json
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:50.142013 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-13/
--rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-13/__init__.py
--rw-rw-rw-   0        0        0     1979 2021-02-17 14:31:06.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-13/info.json
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:50.157645 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-14/
--rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-14/__init__.py
--rw-rw-rw-   0        0        0     2048 2021-02-17 14:32:13.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-14/info.json
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:50.188890 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-15/
--rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-15/__init__.py
--rw-rw-rw-   0        0        0     2022 2021-02-17 14:33:18.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-15/info.json
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:50.220551 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-16/
--rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-16/__init__.py
--rw-rw-rw-   0        0        0     2017 2021-02-17 14:34:54.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-16/info.json
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:50.236193 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-17/
--rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-17/__init__.py
--rw-rw-rw-   0        0        0     2032 2021-02-17 14:36:00.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-17/info.json
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:50.267453 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-18/
--rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-18/__init__.py
--rw-rw-rw-   0        0        0     1945 2021-02-17 14:36:39.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-18/info.json
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:50.283070 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-19/
--rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-19/__init__.py
--rw-rw-rw-   0        0        0     2089 2021-02-17 14:38:06.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-19/info.json
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:50.314835 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-20/
--rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-20/__init__.py
--rw-rw-rw-   0        0        0     1978 2021-02-17 14:38:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-20/info.json
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:50.338908 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/iawe/
--rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/iawe/__init__.py
--rw-rw-rw-   0        0        0     1322 2023-01-19 11:02:54.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/iawe/building1.yaml
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:50.637080 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/
--rw-rw-rw-   0        0        0        0 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/__init__.py
--rw-rw-rw-   0        0        0     1108 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building1.yaml
--rw-rw-rw-   0        0        0     1033 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building10.yaml
--rw-rw-rw-   0        0        0     1009 2023-01-26 10:56:06.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building11.yaml
--rw-rw-rw-   0        0        0      971 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building12.yaml
--rw-rw-rw-   0        0        0     1004 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building13.yaml
--rw-rw-rw-   0        0        0     1065 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building15.yaml
--rw-rw-rw-   0        0        0     1089 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building16.yaml
--rw-rw-rw-   0        0        0     1026 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building17.yaml
--rw-rw-rw-   0        0        0     1048 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building18.yaml
--rw-rw-rw-   0        0        0     1019 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building19.yaml
--rw-rw-rw-   0        0        0     1005 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building2.yaml
--rw-rw-rw-   0        0        0     1005 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building20.yaml
--rw-rw-rw-   0        0        0     1020 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building21.yaml
--rw-rw-rw-   0        0        0     1012 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building3.yaml
--rw-rw-rw-   0        0        0     1025 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building4.yaml
--rw-rw-rw-   0        0        0     1022 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building5.yaml
--rw-rw-rw-   0        0        0      997 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building6.yaml
--rw-rw-rw-   0        0        0      998 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building7.yaml
--rw-rw-rw-   0        0        0      991 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building8.yaml
--rw-rw-rw-   0        0        0     1037 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building9.yaml
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:50.652707 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/ukdale/
--rw-rw-rw-   0        0        0        0 2023-01-16 15:39:19.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/ukdale/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:50.699592 nilm_analyzer-1.0.8/src/nilm_analyzer/modules/
--rw-rw-rw-   0        0        0        0 2023-01-16 15:39:19.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/modules/__init__.py
--rw-rw-rw-   0        0        0    10214 2023-02-22 17:37:30.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/modules/active_durations.py
--rw-rw-rw-   0        0        0     7214 2023-02-18 15:02:45.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/modules/parser.py
--rw-rw-rw-   0        0        0     3348 2023-01-16 15:39:19.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/modules/validations.py
--rw-rw-rw-   0        0        0     1261 2023-01-21 16:20:02.000000 nilm_analyzer-1.0.8/src/nilm_analyzer/utilities.py
-drwxrwxrwx   0        0        0        0 2023-02-27 21:33:49.639712 nilm_analyzer-1.0.8/src/nilm_analyzer.egg-info/
--rw-rw-rw-   0        0        0     5984 2023-02-27 21:33:49.000000 nilm_analyzer-1.0.8/src/nilm_analyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4597 2023-02-27 21:33:49.000000 nilm_analyzer-1.0.8/src/nilm_analyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-27 21:33:49.000000 nilm_analyzer-1.0.8/src/nilm_analyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-02-27 21:33:49.000000 nilm_analyzer-1.0.8/src/nilm_analyzer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-02-27 21:33:49.000000 nilm_analyzer-1.0.8/src/nilm_analyzer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.761367 nilm_analyzer-1.0.9/
+-rw-rw-rw-   0        0        0     1090 2023-02-19 14:22:00.000000 nilm_analyzer-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1343 2023-02-19 17:43:39.000000 nilm_analyzer-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5984 2023-03-02 15:10:30.761367 nilm_analyzer-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4196 2023-02-27 20:54:44.000000 nilm_analyzer-1.0.9/README2.md
+-rw-rw-rw-   0        0        0     1121 2023-03-02 15:09:23.000000 nilm_analyzer-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-03-02 15:10:30.761367 nilm_analyzer-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.161288 nilm_analyzer-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.221664 nilm_analyzer-1.0.9/src/nilm_analyzer/
+-rw-rw-rw-   0        0        0        0 2023-02-20 09:45:12.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/__init__.py
+-rw-rw-rw-   0        0        0    75144 2023-03-02 14:56:31.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/loaders.py
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.253322 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/
+-rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.261451 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/ampds/
+-rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/ampds/__init__.py
+-rw-rw-rw-   0        0        0     3165 2023-01-17 18:36:04.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/ampds/building1.yaml
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.371256 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/deddiag/
+-rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/deddiag/__init__.py
+-rw-rw-rw-   0        0        0       60 2021-01-19 08:13:42.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/deddiag/house_00.tsv
+-rw-rw-rw-   0        0        0      117 2021-01-19 08:25:26.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/deddiag/house_01.tsv
+-rw-rw-rw-   0        0        0       87 2021-01-19 08:27:11.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/deddiag/house_02.tsv
+-rw-rw-rw-   0        0        0      142 2021-01-19 09:02:35.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/deddiag/house_03.tsv
+-rw-rw-rw-   0        0        0      170 2021-01-19 09:49:58.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/deddiag/house_04.tsv
+-rw-rw-rw-   0        0        0      193 2021-01-19 10:44:05.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/deddiag/house_05.tsv
+-rw-rw-rw-   0        0        0      256 2021-01-19 11:09:17.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/deddiag/house_06.tsv
+-rw-rw-rw-   0        0        0      159 2021-01-19 11:25:01.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/deddiag/house_07.tsv
+-rw-rw-rw-   0        0        0      408 2021-01-19 11:52:15.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/deddiag/house_08.tsv
+-rw-rw-rw-   0        0        0      126 2021-01-19 12:47:33.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/deddiag/house_09.tsv
+-rw-rw-rw-   0        0        0      129 2021-01-19 13:18:21.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/deddiag/house_10.tsv
+-rw-rw-rw-   0        0        0       47 2021-01-19 13:45:02.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/deddiag/house_11.tsv
+-rw-rw-rw-   0        0        0      147 2021-01-19 13:45:16.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/deddiag/house_12.tsv
+-rw-rw-rw-   0        0        0      129 2021-01-19 13:49:58.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/deddiag/house_13.tsv
+-rw-rw-rw-   0        0        0      121 2021-01-19 14:04:28.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/deddiag/house_14.tsv
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.371256 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/
+-rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.381348 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-01/
+-rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-01/__init__.py
+-rw-rw-rw-   0        0        0     2057 2021-02-17 14:17:58.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-01/info.json
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.391589 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-02/
+-rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-02/__init__.py
+-rw-rw-rw-   0        0        0     1976 2021-02-17 14:18:33.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-02/info.json
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.401347 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-03/
+-rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-03/__init__.py
+-rw-rw-rw-   0        0        0     1999 2021-02-17 14:19:34.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-03/info.json
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.412483 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-04/
+-rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-04/__init__.py
+-rw-rw-rw-   0        0        0     2051 2021-02-17 14:20:29.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-04/info.json
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.421166 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-05/
+-rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-05/__init__.py
+-rw-rw-rw-   0        0        0     2048 2021-02-17 14:22:18.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-05/info.json
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.431096 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-06/
+-rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-06/__init__.py
+-rw-rw-rw-   0        0        0     2194 2021-02-17 14:23:27.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-06/info.json
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.441293 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-07/
+-rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-07/__init__.py
+-rw-rw-rw-   0        0        0     1985 2021-02-17 14:24:36.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-07/info.json
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.451366 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-08/
+-rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-08/__init__.py
+-rw-rw-rw-   0        0        0     2055 2021-02-17 14:25:41.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-08/info.json
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.461146 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-09/
+-rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-09/__init__.py
+-rw-rw-rw-   0        0        0     2061 2021-02-17 14:27:29.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-09/info.json
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.475803 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-10/
+-rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-10/__init__.py
+-rw-rw-rw-   0        0        0     2058 2021-02-17 14:28:06.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-10/info.json
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.481325 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-11/
+-rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-11/__init__.py
+-rw-rw-rw-   0        0        0     2023 2021-02-17 14:29:09.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-11/info.json
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.491221 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-12/
+-rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-12/__init__.py
+-rw-rw-rw-   0        0        0     2047 2021-02-17 14:30:04.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-12/info.json
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.507280 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-13/
+-rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-13/__init__.py
+-rw-rw-rw-   0        0        0     1979 2021-02-17 14:31:06.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-13/info.json
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.511324 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-14/
+-rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-14/__init__.py
+-rw-rw-rw-   0        0        0     2048 2021-02-17 14:32:13.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-14/info.json
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.523145 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-15/
+-rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-15/__init__.py
+-rw-rw-rw-   0        0        0     2022 2021-02-17 14:33:18.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-15/info.json
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.541446 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-16/
+-rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-16/__init__.py
+-rw-rw-rw-   0        0        0     2017 2021-02-17 14:34:54.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-16/info.json
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.551043 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-17/
+-rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-17/__init__.py
+-rw-rw-rw-   0        0        0     2032 2021-02-17 14:36:00.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-17/info.json
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.561118 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-18/
+-rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-18/__init__.py
+-rw-rw-rw-   0        0        0     1945 2021-02-17 14:36:39.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-18/info.json
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.561118 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-19/
+-rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-19/__init__.py
+-rw-rw-rw-   0        0        0     2089 2021-02-17 14:38:06.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-19/info.json
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.571429 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-20/
+-rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-20/__init__.py
+-rw-rw-rw-   0        0        0     1978 2021-02-17 14:38:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-20/info.json
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.591410 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/iawe/
+-rw-rw-rw-   0        0        0        0 2022-12-27 12:34:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/iawe/__init__.py
+-rw-rw-rw-   0        0        0     1322 2023-01-19 11:02:54.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/iawe/building1.yaml
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.720524 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/
+-rw-rw-rw-   0        0        0        0 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/__init__.py
+-rw-rw-rw-   0        0        0     1108 2023-03-02 14:41:13.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building1.yaml
+-rw-rw-rw-   0        0        0     1032 2023-03-02 14:41:35.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building10.yaml
+-rw-rw-rw-   0        0        0     1008 2023-03-02 14:41:47.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building11.yaml
+-rw-rw-rw-   0        0        0      971 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building12.yaml
+-rw-rw-rw-   0        0        0     1003 2023-03-02 14:43:30.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building13.yaml
+-rw-rw-rw-   0        0        0     1064 2023-03-02 14:43:32.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building15.yaml
+-rw-rw-rw-   0        0        0     1088 2023-03-02 14:43:34.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building16.yaml
+-rw-rw-rw-   0        0        0     1026 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building17.yaml
+-rw-rw-rw-   0        0        0     1047 2023-03-02 14:43:48.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building18.yaml
+-rw-rw-rw-   0        0        0     1019 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building19.yaml
+-rw-rw-rw-   0        0        0     1004 2023-03-02 14:44:07.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building2.yaml
+-rw-rw-rw-   0        0        0     1004 2023-03-02 14:44:13.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building20.yaml
+-rw-rw-rw-   0        0        0     1019 2023-03-02 14:44:23.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building21.yaml
+-rw-rw-rw-   0        0        0     1011 2023-03-02 14:44:33.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building3.yaml
+-rw-rw-rw-   0        0        0     1025 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building4.yaml
+-rw-rw-rw-   0        0        0     1021 2023-03-02 14:45:25.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building5.yaml
+-rw-rw-rw-   0        0        0      996 2023-03-02 14:45:17.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building6.yaml
+-rw-rw-rw-   0        0        0      997 2023-03-02 14:45:06.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building7.yaml
+-rw-rw-rw-   0        0        0      991 2023-01-06 14:19:03.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building8.yaml
+-rw-rw-rw-   0        0        0     1036 2023-03-02 14:44:55.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building9.yaml
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.721529 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/ukdale/
+-rw-rw-rw-   0        0        0        0 2023-01-16 15:39:19.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/ukdale/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.751372 nilm_analyzer-1.0.9/src/nilm_analyzer/modules/
+-rw-rw-rw-   0        0        0        0 2023-01-16 15:39:19.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/modules/__init__.py
+-rw-rw-rw-   0        0        0    10214 2023-03-02 14:55:59.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/modules/active_durations.py
+-rw-rw-rw-   0        0        0     7214 2023-02-18 15:02:45.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/modules/parser.py
+-rw-rw-rw-   0        0        0     3348 2023-01-16 15:39:19.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/modules/validations.py
+-rw-rw-rw-   0        0        0     1261 2023-01-21 16:20:02.000000 nilm_analyzer-1.0.9/src/nilm_analyzer/utilities.py
+drwxrwxrwx   0        0        0        0 2023-03-02 15:10:30.253322 nilm_analyzer-1.0.9/src/nilm_analyzer.egg-info/
+-rw-rw-rw-   0        0        0     5984 2023-03-02 15:10:30.000000 nilm_analyzer-1.0.9/src/nilm_analyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4597 2023-03-02 15:10:30.000000 nilm_analyzer-1.0.9/src/nilm_analyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-02 15:10:30.000000 nilm_analyzer-1.0.9/src/nilm_analyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-03-02 15:10:30.000000 nilm_analyzer-1.0.9/src/nilm_analyzer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-03-02 15:10:30.000000 nilm_analyzer-1.0.9/src/nilm_analyzer.egg-info/top_level.txt
```

### Comparing `nilm_analyzer-1.0.8/LICENSE` & `nilm_analyzer-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/MANIFEST.in` & `nilm_analyzer-1.0.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/PKG-INFO` & `nilm_analyzer-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nilm_analyzer
-Version: 1.0.8
+Version: 1.0.9
 Summary: A simple python package for easy loading and manipulation of NILM datasets.
 Author-email: Mahnoor Shahid <mahnoor.shahid.shakir@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Mahnoor Shahid
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nilm_analyzer-1.0.8/README2.md` & `nilm_analyzer-1.0.9/README2.md`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/pyproject.toml` & `nilm_analyzer-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nilm_analyzer"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="Mahnoor Shahid", email="mahnoor.shahid.shakir@outlook.com" },
 ]
 description = "A simple python package for easy loading and manipulation of NILM datasets."
 readme = "README2.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9.2"
@@ -25,15 +25,15 @@
 ]
 
 [project.urls]
 repository = "https://github.com/mahnoor-shahid/nilm_analyzer"
 
 
 [tool.bumpver]
-current_version = "1.0.8"
+current_version = "1.0.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/loaders.py` & `nilm_analyzer-1.0.9/src/nilm_analyzer/loaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import numpy as np
 import pandas as pd
 import os, pickle
 from sklearn.preprocessing import StandardScaler, MinMaxScaler, RobustScaler
 import math
 import glob
 from datetime import timedelta
 import dask.dataframe as dd
@@ -164,15 +163,16 @@
             super().__init__()
         
         except Exception as e:
             print("Error occured in initialization of REFIT_Loader class due to ", e)
                 
         finally:
             # self.__config = get_config_from_json(description="refit_loader configuration", config_file='../refit_loader/config.json')
-            self.__config = {'DATA_FOLDER': os.path.join(os.getcwd(), data_path), 'DATA_TYPE':'.csv', 'METADATA': os.path.join(get_module_directory(), 'metadata', 'refit'),
+            self.__config = {'DATA_FOLDER': os.path.join(os.getcwd(), data_path), 'DATA_TYPE':'.csv', 'METADATA': os.path.join(get_module_directory(),
+                                                                                                                               'metadata', 'refit'),
                              'REFIT_HOUSES': [1,2,3,4,5,6,7,8,9,10,11,12,13,15,16,17,18,19,20,21]}
             self.__keys_of_appliances = refit_parser(_buildings=self.__config['REFIT_HOUSES'], _metadata=self.__config['METADATA'])
             self.__collective_dataset = CSV_Loader._load_files_via_dask(_data_folder=self.__config['DATA_FOLDER'],
                                                                 _files_format=self.__config['DATA_TYPE'],
                                                                 _buildings=self.__config['REFIT_HOUSES'])
 
             if self.__collective_dataset:
@@ -304,15 +304,16 @@
         try:
             super().__init__()
 
         except Exception as e:
             print("Error occured in initialization of UKDALE_Loader class due to ", e)
 
         finally:
-            self.__config = {'DATA_FOLDER': os.path.join(os.getcwd(), data_path), 'DATA_TYPE':'.dat', 'METADATA': os.path.join(get_module_directory(), 'metadata', 'ukdale'),
+            self.__config = {'DATA_FOLDER': os.path.join(os.getcwd(), data_path), 'DATA_TYPE':'.dat', 'METADATA': os.path.join(get_module_directory(),
+                                                                                                                               'metadata', 'ukdale'),
                              'UKDALE_HOUSES': [1,2,3,4,5]}
             self.__keys_of_appliances = ukdale_parser(_buildings=self.__config['UKDALE_HOUSES'], _metadata=self.__config['METADATA'])
             self.__collective_dataset = CSV_Loader._load_files_via_dask_channel_wise(_data_folder=self.__config['DATA_FOLDER'],
                                                                         _metadata=self.__keys_of_appliances,
                                                                 _files_format=self.__config['DATA_TYPE'],
                                                                 _buildings=self.__config['UKDALE_HOUSES'],
                                                                                      _dataset='ukdale')
@@ -588,15 +589,16 @@
         try:
             super().__init__()
 
         except Exception as e:
             print("Error occured in initialization of IAWE_Loader class due to ", e)
 
         finally:
-            self.__config = {'DATA_FOLDER': os.path.join(os.getcwd(), data_path), 'DATA_TYPE':'.csv', 'METADATA': os.path.join(get_module_directory(), 'metadata', 'iawe'),
+            self.__config = {'DATA_FOLDER': os.path.join(os.getcwd(), data_path), 'DATA_TYPE':'.csv', 'METADATA': os.path.join(get_module_directory(),
+                                                                                                                               'metadata', 'iawe'),
                              'IAWE_HOUSES': [1]}
             self.__keys_of_appliances = iawe_parser(_buildings=self.__config['IAWE_HOUSES'], _metadata=self.__config['METADATA'])
             self.__collective_dataset = CSV_Loader._load_files_via_dask_channel_wise(_data_folder=self.__config['DATA_FOLDER'],
                                                                         _metadata=self.__keys_of_appliances,
                                                                 _files_format=self.__config['DATA_TYPE'],
                                                                 _buildings=self.__config['IAWE_HOUSES'], _dataset='iawe')
 
@@ -743,15 +745,16 @@
         try:
             super().__init__()
 
         except Exception as e:
             print("Error occured in initialization of DEDDIAG_LOADER class due to ", e)
 
         finally:
-            self.__config = {'DATA_FOLDER': os.path.join(os.getcwd(), data_path), 'DATA_TYPE':'.tsv', 'METADATA': os.path.join(get_module_directory(), 'metadata', 'deddiag'),
+            self.__config = {'DATA_FOLDER': os.path.join(os.getcwd(), data_path), 'DATA_TYPE':'.tsv', 'METADATA': os.path.join(get_module_directory(),
+                                                                                                                               'metadata', 'deddiag'),
                              'DEDDIAG_HOUSES': ['00','01', '02', '03', '04', '05', '06', '07','08', '09', '10', '11', '12', '13', '14']}
             self.__keys_of_appliances = deddiag_parser(_buildings=self.__config['DEDDIAG_HOUSES'], _metadata=self.__config['METADATA'])
             self.__collective_dataset = CSV_Loader._load_files_via_dask_channel_wise(_data_folder=self.__config['DATA_FOLDER'],
                                                                         _metadata=self.__keys_of_appliances,
                                                                 _files_format=self.__config['DATA_TYPE'],
                                                                 _buildings=self.__config['DEDDIAG_HOUSES'], _dataset='deddiag')
 
@@ -888,15 +891,16 @@
         try:
             super().__init__()
 
         except Exception as e:
             print("Error occured in initialization of GELAP_Loader class due to ", e)
 
         finally:
-            self.__config = {'DATA_FOLDER': os.path.join(os.getcwd(), data_path), 'DATA_TYPE':'.csv', 'METADATA': os.path.join(get_module_directory(), 'metadata', 'gelap'),
+            self.__config = {'DATA_FOLDER': os.path.join(os.getcwd(), data_path), 'DATA_TYPE':'.csv', 'METADATA': os.path.join(get_module_directory(),
+                                                                                                                               'metadata', 'gelap'),
                              'GELAP_HOUSES': ['01', '02', '03', '04', '05', '06', '07', '08', '09', '10', '11',
                                                 '12', '13', '14', '15', '16', '17', '18', '19', '20']}
             self.__keys_of_appliances = gelap_parser(_buildings=self.__config['GELAP_HOUSES'], _metadata=self.__config['METADATA'])
             self.__collective_dataset = CSV_Loader._load_files_via_dask_channel_wise(_data_folder=self.__config['DATA_FOLDER'],
                                                                         _metadata=self.__keys_of_appliances,
                                                                 _files_format=self.__config['DATA_TYPE'],
                                                                 _buildings=self.__config['GELAP_HOUSES'],
@@ -1072,18 +1076,18 @@
 
             for house_number in self.data.keys():
                 print(f"Resampling for house number: ", house_number)
 #                     target_appliance = self.data[house_number].columns[-1]
                 appliance_data = self.data[house_number]
                 if sampling_period is None:
                     delta = appliance_data.index[1] - appliance_data.index[0]
-                    self.__sampling_period = str(delta.seconds) + 's'
+                    self.__sampling_period = str(int(delta.seconds)) + 's'
                     self.__window_limit = int((window_limit * 60) / delta.seconds)
                 else:
-                    self.__sampling_period = str(sampling_period) + 's'
+                    self.__sampling_period = str(int(sampling_period)) + 's'
                     self.__window_limit = int((window_limit * 60) / sampling_period)
                 print(f'sampling_period = {self.__sampling_period}, window_limit = {self.__window_limit} samples, fill_value = {self.__fill_value}\n')
                 appliance_data = appliance_data[~appliance_data.index.duplicated(keep='first')]
 #                     appliance_data = appliance_data.resample('1s').mean().dropna()
                 appliance_data = appliance_data.resample('1s').asfreq()
                 appliance_data.fillna(method='ffill', axis=0, inplace=True, limit=self.__window_limit)
                 appliance_data.fillna(axis=0, inplace=True, value=self.__fill_value)
```

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/ampds/building1.yaml` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/ampds/building1.yaml`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-01/info.json` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-01/info.json`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-02/info.json` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-02/info.json`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-03/info.json` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-03/info.json`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-04/info.json` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-04/info.json`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-05/info.json` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-05/info.json`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-06/info.json` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-06/info.json`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-07/info.json` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-07/info.json`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-08/info.json` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-08/info.json`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-09/info.json` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-09/info.json`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-10/info.json` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-10/info.json`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-11/info.json` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-11/info.json`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-12/info.json` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-12/info.json`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-13/info.json` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-13/info.json`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-14/info.json` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-14/info.json`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-15/info.json` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-15/info.json`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-16/info.json` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-16/info.json`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-17/info.json` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-17/info.json`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-18/info.json` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-18/info.json`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-19/info.json` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-19/info.json`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/gelap/hh-20/info.json` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/gelap/hh-20/info.json`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/iawe/building1.yaml` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/iawe/building1.yaml`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building1.yaml` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building1.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -38,16 +38,16 @@
   meters: [5]
   
 - original_name: Washing Machine
   type: washing machine
   instance: 1
   meters: [6]
 
-- original_name: Dishwaser
-  type: dish washer
+- original_name: Dishwasher
+  type: dishwasher
   instance: 1
   meters: [7]
   
 - original_name: Computer
   type: computer
   instance: 1
   meters: [8]
```

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building10.yaml` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building10.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 - original_name: Washing Machine
   type: washing machine
   instance: 1
   meters: [6]
   
 - original_name: Dishwasher
-  type: dish washer
+  type: dishwasher
   instance: 1
   meters: [7]
   
 - original_name: Television Site
   type: television
   instance: 1
   meters: [8]
```

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building11.yaml` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building11.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 - original_name: Washing Machine
   type: washing machine
   instance: 1
   meters: [4]
 
 - original_name: Dishwasher
-  type: dish washer
+  type: dishwasher
   instance: 1
   meters: [5]
 
 - original_name: Computer Site
   type: computer
   instance: 1
   meters: [6]
```

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building12.yaml` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building12.yaml`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building13.yaml` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building13.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 - original_name: Washing Machine
   type: washing machine
   instance: 1
   meters: [4]
 
 - original_name: Dishwasher
-  type: dish washer
+  type: dish asher
   instance: 1
   meters: [5]
 
 - original_name: ???
   type: unknown
   instance: 1
   meters: [6]
```

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building15.yaml` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building15.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 - original_name: Washing Machine
   type: washing machine
   instance: 1
   meters: [4]
 
 - original_name: Dishwasher
-  type: dish washer
+  type: dishwasher
   instance: 1
   meters: [5]
 
 - original_name: Computer Site
   type: computer
   instance: 1
   meters: [6]
```

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building16.yaml` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building16.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 - original_name: Washing Machine
   type: washing machine
   instance: 1
   meters: [6]
   
 - original_name: Dishwasher
-  type: dish washer
+  type: dishwasher
   instance: 1
   meters: [7]
   
 - original_name: Computer Site
   type: computer
   instance: 1
   meters: [8]
```

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building17.yaml` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building17.yaml`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building18.yaml` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building7.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-instance: 17
-original_name: House18
+instance: 7
+original_name: House7
 elec_meters:
   1: &clamp 
     site_meter: true
     device_model: Clamp
   2: &iam
     submeter_of: 0 
     device_model: IAM
@@ -13,51 +13,51 @@
   6: *iam
   7: *iam
   8: *iam
   9: *iam
   10: *iam
 
 appliances:
-- original_name: Fridge(garage)
+- original_name: Fridge
   type: fridge
   instance: 1
   meters: [2]
   
-- original_name: Freezer(garage)
+- original_name: Freezer(1)
   type: freezer
   instance: 1
   meters: [3]
 
-- original_name: Fridge-Freezer
-  type: fridge freezer
-  instance: 1
+- original_name: Freezer(2)
+  type: freezer
+  instance: 2
   meters: [4]
 
-- original_name: Washer Dryer(garage)
-  type: washer dryer
+- original_name: Tumble Dryer
+  type: tumble dryer
   instance: 1
   meters: [5]
 
 - original_name: Washing Machine
   type: washing machine
   instance: 1
   meters: [6]
   
 - original_name: Dishwasher
-  type: dish washer
+  type: dishwasher
   instance: 1
   meters: [7]
   
-- original_name: Desktop Computer
-  type: computer
+- original_name: Television Site
+  type: television
   instance: 1
   meters: [8]
 
-- original_name: Television Site
-  type: television
+- original_name: Toaster
+  type: toaster
   instance: 1
   meters: [9]
   
-- original_name: Microwave
-  type: microwave
+- original_name: Kettle
+  type: kettle
   instance: 1
   meters: [10]
```

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building19.yaml` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building19.yaml`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building2.yaml` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building2.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   
 - original_name: Washing Machine
   type: washing machine
   instance: 1
   meters: [3]
 
 - original_name: Dishwaser
-  type: dish washer
+  type: dishwasher
   instance: 1
   meters: [4]
 
 - original_name: Television Site
   type: television
   instance: 1
   meters: [5]
```

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building20.yaml` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building20.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 - original_name: Washing Machine
   type: washing machine
   instance: 1
   meters: [5]
 
 - original_name: Dishwasher
-  type: dish washer
+  type: dishwasher
   instance: 1
   meters: [6]
   
 - original_name: Computer Site
   type: computer
   instance: 1
   meters: [7]
```

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building21.yaml` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building21.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 - original_name: Washing Machine
   type: washing machine
   instance: 1
   meters: [4]
 
 - original_name: Dishwasher
-  type: dish washer
+  type: dishwasher
   instance: 1
   meters: [5]
 
 - original_name: Food Mixer
   type: food processor
   instance: 1
   meters: [6]
```

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building3.yaml` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building3.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 - original_name: Tumble Dryer
   type: tumble dryer
   instance: 1
   meters: [5]
 
 - original_name: Dishwasher
-  type: dish washer
+  type: dishwasher
   instance: 1
   meters: [6]
   
 - original_name: Washing Machine
   type: washing machine
   instance: 1
   meters: [7]
```

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building4.yaml` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building4.yaml`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building5.yaml` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building5.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 - original_name: Washing Machine
   type: washing machine
   instance: 1
   meters: [4]
 
 - original_name: Dishwasher
-  type: dish washer
+  type: dishwasher
   instance: 1
   meters: [5]
 
 - original_name: Desktop Computer
   type: computer
   instance: 1
   meters: [6]
```

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building6.yaml` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building6.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   
 - original_name: Washing Machine
   type: washing machine
   instance: 1
   meters: [3]
 
 - original_name: Dishwasher
-  type: dish washer
+  type: dishwasher
   instance: 1
   meters: [4]
 
 - original_name: MJY Computer
   type: computer
   instance: 1
   meters: [5]
```

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building7.yaml` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building18.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-instance: 7
-original_name: House7
+instance: 17
+original_name: House18
 elec_meters:
   1: &clamp 
     site_meter: true
     device_model: Clamp
   2: &iam
     submeter_of: 0 
     device_model: IAM
@@ -13,51 +13,51 @@
   6: *iam
   7: *iam
   8: *iam
   9: *iam
   10: *iam
 
 appliances:
-- original_name: Fridge
+- original_name: Fridge(garage)
   type: fridge
   instance: 1
   meters: [2]
   
-- original_name: Freezer(1)
+- original_name: Freezer(garage)
   type: freezer
   instance: 1
   meters: [3]
 
-- original_name: Freezer(2)
-  type: freezer
-  instance: 2
+- original_name: Fridge-Freezer
+  type: fridge freezer
+  instance: 1
   meters: [4]
 
-- original_name: Tumble Dryer
-  type: tumble dryer
+- original_name: Washer Dryer(garage)
+  type: washer dryer
   instance: 1
   meters: [5]
 
 - original_name: Washing Machine
   type: washing machine
   instance: 1
   meters: [6]
   
 - original_name: Dishwasher
-  type: dish washer
+  type: dishwasher
   instance: 1
   meters: [7]
   
-- original_name: Television Site
-  type: television
+- original_name: Desktop Computer
+  type: computer
   instance: 1
   meters: [8]
 
-- original_name: Toaster
-  type: toaster
+- original_name: Television Site
+  type: television
   instance: 1
   meters: [9]
   
-- original_name: Kettle
-  type: kettle
+- original_name: Microwave
+  type: microwave
   instance: 1
   meters: [10]
```

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building8.yaml` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building8.yaml`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/metadata/refit/building9.yaml` & `nilm_analyzer-1.0.9/src/nilm_analyzer/metadata/refit/building9.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 - original_name: Washing Machine
   type: washing machine
   instance: 1
   meters: [4]
 
 - original_name: Dishwasher
-  type: dish washer
+  type: dishwasher
   instance: 1
   meters: [5]
 
 - original_name: Television Site
   type: television
   instance: 1
   meters: [6]
```

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/modules/active_durations.py` & `nilm_analyzer-1.0.9/src/nilm_analyzer/modules/active_durations.py`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/modules/parser.py` & `nilm_analyzer-1.0.9/src/nilm_analyzer/modules/parser.py`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/modules/validations.py` & `nilm_analyzer-1.0.9/src/nilm_analyzer/modules/validations.py`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer/utilities.py` & `nilm_analyzer-1.0.9/src/nilm_analyzer/utilities.py`

 * *Files identical despite different names*

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer.egg-info/PKG-INFO` & `nilm_analyzer-1.0.9/src/nilm_analyzer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nilm-analyzer
-Version: 1.0.8
+Version: 1.0.9
 Summary: A simple python package for easy loading and manipulation of NILM datasets.
 Author-email: Mahnoor Shahid <mahnoor.shahid.shakir@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Mahnoor Shahid
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nilm_analyzer-1.0.8/src/nilm_analyzer.egg-info/SOURCES.txt` & `nilm_analyzer-1.0.9/src/nilm_analyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

