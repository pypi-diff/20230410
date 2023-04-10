# Comparing `tmp/th2_data_services_lwdp-2.0.2.0.dev4566564684.tar.gz` & `tmp/th2_data_services_lwdp-2.0.2.0.dev4658647164.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services_lwdp-2.0.2.0.dev4566564684.tar", last modified: Thu Mar 30 16:12:40 2023, max compression
+gzip compressed data, was "dist/th2_data_services_lwdp-2.0.2.0.dev4658647164.tar", last modified: Mon Apr 10 15:16:13 2023, max compression
```

## Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684.tar` & `th2_data_services_lwdp-2.0.2.0.dev4658647164.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 16:12:40.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-03-30 16:12:40.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7699 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-03-30 16:12:17.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-30 16:12:40.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1636 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 16:12:40.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 16:12:40.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 16:12:40.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/
--rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 16:12:40.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/adapters/
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
--rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/adapters/basic_adapters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/adapters/event_adapters.py
--rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/adapters/message_adapters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 16:12:40.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/commands/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    38645 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/commands/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 16:12:40.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/data_source/
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/data_source/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/data_source/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 16:12:40.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/event_tree/
--rw-r--r--   0 runner    (1001) docker     (122)      658 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 16:12:40.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/filters/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/filters/event_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3527 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/filters/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 16:12:40.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/interfaces/filter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/message_response_format.py
--rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/page.py
--rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 16:12:40.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/source_api/
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/source_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16862 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/source_api/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    11129 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/source_api/http.py
--rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/streams.py
--rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 16:12:40.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      671 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-03-30 16:08:58.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 16:12:40.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services_lwdp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-03-30 16:12:40.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services_lwdp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2167 2023-03-30 16:12:40.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services_lwdp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-30 16:12:40.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services_lwdp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-03-30 16:12:40.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services_lwdp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-03-30 16:12:40.000000 th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services_lwdp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7699 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-10 15:15:57.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1636 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/adapters/
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/adapters/basic_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/adapters/event_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/adapters/message_adapters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/commands/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38684 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/commands/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/data_source/
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/data_source/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/data_source/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      658 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/filters/event_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3527 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/filters/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/interfaces/filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/message_response_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/page.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/source_api/
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/source_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16862 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/source_api/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11129 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/source_api/http.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/streams.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      671 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services_lwdp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services_lwdp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2167 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services_lwdp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services_lwdp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services_lwdp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services_lwdp.egg-info/top_level.txt
```

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/PKG-INFO` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services_lwdp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: th2_data_services_lwdp
-Version: 2.0.2.0.dev4566564684
+Name: th2-data-services-lwdp
+Version: 2.0.2.0.dev4658647164
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/README.md` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/setup.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/adapters/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/adapters/adapter_sse.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/adapters/adapter_sse.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/adapters/basic_adapters.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/adapters/basic_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/adapters/event_adapters.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/adapters/event_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/adapters/message_adapters.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/adapters/message_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/commands/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/commands/grpc.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/commands/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/commands/http.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/commands/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -642,15 +642,15 @@
         super().__init__()
         self._id = id
         self._stub_status = use_stub
         self._response_formats = response_formats
 
     def handle(self, data_source: HTTPDataSource) -> dict:  # noqa: D102
         api: HTTPAPI = data_source.source_api
-        if not isinstance(self._response_formats,list):
+        if not isinstance(self._response_formats,list) and self._response_formats is not None:
             raise Exception("response_formats argument should be a list")
         if self._response_formats in [None,["JSON_PARSED","BASE_64"],["BASE_64","JSON_PARSED"]]:
             only_raw = False
         elif self._response_formats in [["BASE_64"]]:
             only_raw = True
         else:
             raise Exception('response_formats takes only values ["BASE_64","JSON_PARSED"] or ["BASE_64"]')
```

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/data_source/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/data_source/grpc.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/data_source/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/data_source/http.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/data_source/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/event_tree/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/filters/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/filters/event_filters.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/filters/event_filters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/filters/filter.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/filters/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/interfaces/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/interfaces/command.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/interfaces/data_source.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/interfaces/filter.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/interfaces/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/interfaces/source_api.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/message_response_format.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/message_response_format.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/page.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/page.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/resolver.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/source_api/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/source_api/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/source_api/grpc.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/source_api/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/source_api/http.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/source_api/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/streams.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/streams.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/struct.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/stub_builder.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/utils/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/utils/json.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/utils/json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services/data_source/lwdp/utils/misc.py` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/utils/misc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services_lwdp.egg-info/PKG-INFO` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: th2-data-services-lwdp
-Version: 2.0.2.0.dev4566564684
+Name: th2_data_services_lwdp
+Version: 2.0.2.0.dev4658647164
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4566564684/th2_data_services_lwdp.egg-info/SOURCES.txt` & `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services_lwdp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

