# Comparing `tmp/sm-search-connector-poc-interface-0.2.1.tar.gz` & `tmp/sm-search-connector-poc-interface-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sm-search-connector-poc-interface-0.2.1.tar", last modified: Mon Apr 10 00:12:47 2023, max compression
+gzip compressed data, was "sm-search-connector-poc-interface-0.2.2.tar", last modified: Mon Apr 10 01:07:37 2023, max compression
```

## Comparing `sm-search-connector-poc-interface-0.2.1.tar` & `sm-search-connector-poc-interface-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 shrmitul   (505) staff       (20)        0 2023-04-10 00:12:47.711423 sm-search-connector-poc-interface-0.2.1/
--rw-r--r--   0 shrmitul   (505) staff       (20)      187 2023-04-10 00:12:47.711128 sm-search-connector-poc-interface-0.2.1/PKG-INFO
--rw-r--r--   0 shrmitul   (505) staff       (20)       38 2023-04-10 00:12:47.711523 sm-search-connector-poc-interface-0.2.1/setup.cfg
--rw-r--r--   0 shrmitul   (505) staff       (20)      361 2023-04-10 00:06:39.000000 sm-search-connector-poc-interface-0.2.1/setup.py
-drwxr-xr-x   0 shrmitul   (505) staff       (20)        0 2023-04-10 00:12:47.708924 sm-search-connector-poc-interface-0.2.1/sm-search-connector-poc-interface/
--rw-r--r--   0 shrmitul   (505) staff       (20)       44 2023-04-07 16:55:55.000000 sm-search-connector-poc-interface-0.2.1/sm-search-connector-poc-interface/__init__.py
--rw-r--r--   0 shrmitul   (505) staff       (20)      199 2023-04-09 23:58:40.000000 sm-search-connector-poc-interface-0.2.1/sm-search-connector-poc-interface/interface.py
-drwxr-xr-x   0 shrmitul   (505) staff       (20)        0 2023-04-10 00:12:47.710718 sm-search-connector-poc-interface-0.2.1/sm_search_connector_poc_interface.egg-info/
--rw-r--r--   0 shrmitul   (505) staff       (20)      187 2023-04-10 00:12:47.000000 sm-search-connector-poc-interface-0.2.1/sm_search_connector_poc_interface.egg-info/PKG-INFO
--rw-r--r--   0 shrmitul   (505) staff       (20)      329 2023-04-10 00:12:47.000000 sm-search-connector-poc-interface-0.2.1/sm_search_connector_poc_interface.egg-info/SOURCES.txt
--rw-r--r--   0 shrmitul   (505) staff       (20)        1 2023-04-10 00:12:47.000000 sm-search-connector-poc-interface-0.2.1/sm_search_connector_poc_interface.egg-info/dependency_links.txt
--rw-r--r--   0 shrmitul   (505) staff       (20)       34 2023-04-10 00:12:47.000000 sm-search-connector-poc-interface-0.2.1/sm_search_connector_poc_interface.egg-info/top_level.txt
+drwxr-xr-x   0 shrmitul   (505) staff       (20)        0 2023-04-10 01:07:37.053883 sm-search-connector-poc-interface-0.2.2/
+-rw-r--r--   0 shrmitul   (505) staff       (20)      187 2023-04-10 01:07:37.053567 sm-search-connector-poc-interface-0.2.2/PKG-INFO
+-rw-r--r--   0 shrmitul   (505) staff       (20)       38 2023-04-10 01:07:37.053981 sm-search-connector-poc-interface-0.2.2/setup.cfg
+-rw-r--r--   0 shrmitul   (505) staff       (20)      361 2023-04-10 01:07:27.000000 sm-search-connector-poc-interface-0.2.2/setup.py
+drwxr-xr-x   0 shrmitul   (505) staff       (20)        0 2023-04-10 01:07:37.051319 sm-search-connector-poc-interface-0.2.2/sm-search-connector-poc-interface/
+-rw-r--r--   0 shrmitul   (505) staff       (20)       86 2023-04-10 01:04:33.000000 sm-search-connector-poc-interface-0.2.2/sm-search-connector-poc-interface/__init__.py
+-rw-r--r--   0 shrmitul   (505) staff       (20)      199 2023-04-09 23:58:40.000000 sm-search-connector-poc-interface-0.2.2/sm-search-connector-poc-interface/interface.py
+drwxr-xr-x   0 shrmitul   (505) staff       (20)        0 2023-04-10 01:07:37.053171 sm-search-connector-poc-interface-0.2.2/sm_search_connector_poc_interface.egg-info/
+-rw-r--r--   0 shrmitul   (505) staff       (20)      187 2023-04-10 01:07:36.000000 sm-search-connector-poc-interface-0.2.2/sm_search_connector_poc_interface.egg-info/PKG-INFO
+-rw-r--r--   0 shrmitul   (505) staff       (20)      329 2023-04-10 01:07:37.000000 sm-search-connector-poc-interface-0.2.2/sm_search_connector_poc_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 shrmitul   (505) staff       (20)        1 2023-04-10 01:07:36.000000 sm-search-connector-poc-interface-0.2.2/sm_search_connector_poc_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 shrmitul   (505) staff       (20)       34 2023-04-10 01:07:36.000000 sm-search-connector-poc-interface-0.2.2/sm_search_connector_poc_interface.egg-info/top_level.txt
```

