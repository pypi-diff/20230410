# Comparing `tmp/sm-search-connector-poc-0.1.0.tar.gz` & `tmp/sm-search-connector-poc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sm-search-connector-poc-0.1.0.tar", last modified: Fri Apr  7 05:32:13 2023, max compression
+gzip compressed data, was "sm-search-connector-poc-0.1.1.tar", last modified: Mon Apr 10 01:22:51 2023, max compression
```

## Comparing `sm-search-connector-poc-0.1.0.tar` & `sm-search-connector-poc-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxr-xr-x   0 shrmitul   (505) staff       (20)        0 2023-04-07 05:32:13.146572 sm-search-connector-poc-0.1.0/
--rw-r--r--   0 shrmitul   (505) staff       (20)      163 2023-04-07 05:32:13.146176 sm-search-connector-poc-0.1.0/PKG-INFO
--rw-r--r--   0 shrmitul   (505) staff       (20)       38 2023-04-07 05:32:13.146686 sm-search-connector-poc-0.1.0/setup.cfg
--rw-r--r--   0 shrmitul   (505) staff       (20)      337 2023-04-07 05:25:03.000000 sm-search-connector-poc-0.1.0/setup.py
-drwxr-xr-x   0 shrmitul   (505) staff       (20)        0 2023-04-07 05:32:13.143599 sm-search-connector-poc-0.1.0/sm-search-connector-poc/
--rw-r--r--   0 shrmitul   (505) staff       (20)       40 2023-04-07 05:27:03.000000 sm-search-connector-poc-0.1.0/sm-search-connector-poc/__init__.py
-drwxr-xr-x   0 shrmitul   (505) staff       (20)        0 2023-04-07 05:32:13.145741 sm-search-connector-poc-0.1.0/sm_search_connector_poc.egg-info/
--rw-r--r--   0 shrmitul   (505) staff       (20)      163 2023-04-07 05:32:13.000000 sm-search-connector-poc-0.1.0/sm_search_connector_poc.egg-info/PKG-INFO
--rw-r--r--   0 shrmitul   (505) staff       (20)      232 2023-04-07 05:32:13.000000 sm-search-connector-poc-0.1.0/sm_search_connector_poc.egg-info/SOURCES.txt
--rw-r--r--   0 shrmitul   (505) staff       (20)        1 2023-04-07 05:32:13.000000 sm-search-connector-poc-0.1.0/sm_search_connector_poc.egg-info/dependency_links.txt
--rw-r--r--   0 shrmitul   (505) staff       (20)       24 2023-04-07 05:32:13.000000 sm-search-connector-poc-0.1.0/sm_search_connector_poc.egg-info/top_level.txt
+drwxr-xr-x   0 shrmitul   (505) staff       (20)        0 2023-04-10 01:22:51.045250 sm-search-connector-poc-0.1.1/
+-rw-r--r--   0 shrmitul   (505) staff       (20)      163 2023-04-10 01:22:51.044824 sm-search-connector-poc-0.1.1/PKG-INFO
+-rw-r--r--   0 shrmitul   (505) staff       (20)       38 2023-04-10 01:22:51.045382 sm-search-connector-poc-0.1.1/setup.cfg
+-rw-r--r--   0 shrmitul   (505) staff       (20)      381 2023-04-10 01:21:49.000000 sm-search-connector-poc-0.1.1/setup.py
+drwxr-xr-x   0 shrmitul   (505) staff       (20)        0 2023-04-10 01:22:51.042414 sm-search-connector-poc-0.1.1/sm-search-connector-poc/
+-rw-r--r--   0 shrmitul   (505) staff       (20)      104 2023-04-10 01:21:22.000000 sm-search-connector-poc-0.1.1/sm-search-connector-poc/__init__.py
+-rw-r--r--   0 shrmitul   (505) staff       (20)      343 2023-04-10 01:19:43.000000 sm-search-connector-poc-0.1.1/sm-search-connector-poc/searchConnectorPoc.py
+drwxr-xr-x   0 shrmitul   (505) staff       (20)        0 2023-04-10 01:22:51.044276 sm-search-connector-poc-0.1.1/sm_search_connector_poc.egg-info/
+-rw-r--r--   0 shrmitul   (505) staff       (20)      163 2023-04-10 01:22:50.000000 sm-search-connector-poc-0.1.1/sm_search_connector_poc.egg-info/PKG-INFO
+-rw-r--r--   0 shrmitul   (505) staff       (20)      324 2023-04-10 01:22:51.000000 sm-search-connector-poc-0.1.1/sm_search_connector_poc.egg-info/SOURCES.txt
+-rw-r--r--   0 shrmitul   (505) staff       (20)        1 2023-04-10 01:22:50.000000 sm-search-connector-poc-0.1.1/sm_search_connector_poc.egg-info/dependency_links.txt
+-rw-r--r--   0 shrmitul   (505) staff       (20)       34 2023-04-10 01:22:50.000000 sm-search-connector-poc-0.1.1/sm_search_connector_poc.egg-info/requires.txt
+-rw-r--r--   0 shrmitul   (505) staff       (20)       24 2023-04-10 01:22:50.000000 sm-search-connector-poc-0.1.1/sm_search_connector_poc.egg-info/top_level.txt
```

