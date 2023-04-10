# Comparing `tmp/tap-pendo-0.6.1.tar.gz` & `tmp/tap-pendo-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-pendo-0.6.1.tar", last modified: Thu Apr  6 10:00:10 2023, max compression
+gzip compressed data, was "tap-pendo-0.6.2.tar", last modified: Mon Apr 10 13:43:38 2023, max compression
```

## Comparing `tap-pendo-0.6.1.tar` & `tap-pendo-0.6.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-06 10:00:10.365226 tap-pendo-0.6.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32387 2022-12-05 18:24:04.000000 tap-pendo-0.6.1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       89 2022-12-05 18:24:04.000000 tap-pendo-0.6.1/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      314 2023-04-06 10:00:10.365226 tap-pendo-0.6.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15851 2023-03-30 16:00:02.000000 tap-pendo-0.6.1/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-04-06 10:00:10.365226 tap-pendo-0.6.1/setup.cfg
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      916 2023-04-06 09:57:08.000000 tap-pendo-0.6.1/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-06 10:00:10.361226 tap-pendo-0.6.1/tap_pendo/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5901 2023-03-27 07:58:13.000000 tap-pendo-0.6.1/tap_pendo/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5091 2023-03-29 08:01:30.000000 tap-pendo-0.6.1/tap_pendo/discover.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-06 10:00:10.365226 tap-pendo-0.6.1/tap_pendo/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      922 2022-12-05 18:24:04.000000 tap-pendo-0.6.1/tap_pendo/schemas/accounts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      987 2022-12-05 18:24:04.000000 tap-pendo-0.6.1/tap_pendo/schemas/events.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      838 2022-12-05 18:24:04.000000 tap-pendo-0.6.1/tap_pendo/schemas/feature_events.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4166 2022-12-05 18:24:04.000000 tap-pendo-0.6.1/tap_pendo/schemas/features.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1598 2023-03-30 15:54:59.000000 tap-pendo-0.6.1/tap_pendo/schemas/guide_events.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5944 2022-12-05 18:24:04.000000 tap-pendo-0.6.1/tap_pendo/schemas/guides.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      530 2022-12-05 18:24:04.000000 tap-pendo-0.6.1/tap_pendo/schemas/metadata_accounts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1087 2022-12-05 18:24:04.000000 tap-pendo-0.6.1/tap_pendo/schemas/metadata_visitors.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      923 2023-03-30 15:54:59.000000 tap-pendo-0.6.1/tap_pendo/schemas/page_events.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3657 2022-12-05 18:24:04.000000 tap-pendo-0.6.1/tap_pendo/schemas/pages.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1330 2022-12-05 18:24:04.000000 tap-pendo-0.6.1/tap_pendo/schemas/poll_events.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-06 10:00:10.365226 tap-pendo-0.6.1/tap_pendo/schemas/shared/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      684 2022-12-05 18:24:04.000000 tap-pendo-0.6.1/tap_pendo/schemas/shared/metadata.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2022-12-05 18:24:04.000000 tap-pendo-0.6.1/tap_pendo/schemas/track_events.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2327 2022-12-05 18:24:04.000000 tap-pendo-0.6.1/tap_pendo/schemas/track_types.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1262 2022-12-05 18:24:04.000000 tap-pendo-0.6.1/tap_pendo/schemas/visitor_history.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1931 2022-12-05 18:24:04.000000 tap-pendo-0.6.1/tap_pendo/schemas/visitors.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    58754 2023-04-06 09:57:08.000000 tap-pendo-0.6.1/tap_pendo/streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4201 2023-04-04 11:36:09.000000 tap-pendo-0.6.1/tap_pendo/sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2439 2022-12-05 18:24:04.000000 tap-pendo-0.6.1/tap_pendo/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-06 10:00:10.361226 tap-pendo-0.6.1/tap_pendo.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      314 2023-04-06 10:00:10.000000 tap-pendo-0.6.1/tap_pendo.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      910 2023-04-06 10:00:10.000000 tap-pendo-0.6.1/tap_pendo.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-06 10:00:10.000000 tap-pendo-0.6.1/tap_pendo.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       56 2023-04-06 10:00:10.000000 tap-pendo-0.6.1/tap_pendo.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2023-04-06 10:00:10.000000 tap-pendo-0.6.1/tap_pendo.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2023-04-06 10:00:10.000000 tap-pendo-0.6.1/tap_pendo.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-10 13:43:38.070166 tap-pendo-0.6.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32387 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       89 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      280 2023-04-10 13:43:38.070166 tap-pendo-0.6.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15851 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-04-10 13:43:38.070166 tap-pendo-0.6.2/setup.cfg
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      916 2023-04-10 13:35:39.000000 tap-pendo-0.6.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-10 13:43:38.054166 tap-pendo-0.6.2/tap_pendo/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5901 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5091 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/discover.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-10 13:43:38.066166 tap-pendo-0.6.2/tap_pendo/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      922 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/accounts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      987 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      838 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/feature_events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4166 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/features.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1598 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/guide_events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5944 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/guides.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      530 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/metadata_accounts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1087 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/metadata_visitors.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      923 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/page_events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3657 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/pages.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1330 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/poll_events.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-10 13:43:38.066166 tap-pendo-0.6.2/tap_pendo/schemas/shared/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      684 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/shared/metadata.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/track_events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2327 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/track_types.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1262 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/visitor_history.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1931 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/visitors.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    58745 2023-04-10 13:35:39.000000 tap-pendo-0.6.2/tap_pendo/streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4201 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2439 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-10 13:43:38.054166 tap-pendo-0.6.2/tap_pendo.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      280 2023-04-10 13:43:38.000000 tap-pendo-0.6.2/tap_pendo.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      910 2023-04-10 13:43:38.000000 tap-pendo-0.6.2/tap_pendo.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-10 13:43:38.000000 tap-pendo-0.6.2/tap_pendo.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       45 2023-04-10 13:43:38.000000 tap-pendo-0.6.2/tap_pendo.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2023-04-10 13:43:38.000000 tap-pendo-0.6.2/tap_pendo.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2023-04-10 13:43:38.000000 tap-pendo-0.6.2/tap_pendo.egg-info/top_level.txt
```

### Comparing `tap-pendo-0.6.1/LICENSE` & `tap-pendo-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.1/README.md` & `tap-pendo-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.1/setup.py` & `tap-pendo-0.6.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="tap-pendo",
-    version="0.6.1",
+    version="0.6.2",
     description="Singer.io tap for extracting data",
     author="Stitch",
     url="https://github.com/singer-io/tap-pendo",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     py_modules=["tap_pendo"],
     install_requires=[
         'singer-python==5.13.0',
```

### Comparing `tap-pendo-0.6.1/tap_pendo/__init__.py` & `tap-pendo-0.6.2/tap_pendo/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.1/tap_pendo/discover.py` & `tap-pendo-0.6.2/tap_pendo/discover.py`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.1/tap_pendo/schemas/accounts.json` & `tap-pendo-0.6.2/tap_pendo/schemas/accounts.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.1/tap_pendo/schemas/events.json` & `tap-pendo-0.6.2/tap_pendo/schemas/events.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.1/tap_pendo/schemas/feature_events.json` & `tap-pendo-0.6.2/tap_pendo/schemas/feature_events.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.1/tap_pendo/schemas/features.json` & `tap-pendo-0.6.2/tap_pendo/schemas/features.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.1/tap_pendo/schemas/guide_events.json` & `tap-pendo-0.6.2/tap_pendo/schemas/guide_events.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.1/tap_pendo/schemas/guides.json` & `tap-pendo-0.6.2/tap_pendo/schemas/guides.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.1/tap_pendo/schemas/metadata_accounts.json` & `tap-pendo-0.6.2/tap_pendo/schemas/metadata_accounts.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.1/tap_pendo/schemas/metadata_visitors.json` & `tap-pendo-0.6.2/tap_pendo/schemas/metadata_visitors.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.1/tap_pendo/schemas/page_events.json` & `tap-pendo-0.6.2/tap_pendo/schemas/page_events.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.1/tap_pendo/schemas/pages.json` & `tap-pendo-0.6.2/tap_pendo/schemas/pages.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.1/tap_pendo/schemas/poll_events.json` & `tap-pendo-0.6.2/tap_pendo/schemas/poll_events.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.1/tap_pendo/schemas/shared/metadata.json` & `tap-pendo-0.6.2/tap_pendo/schemas/shared/metadata.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.1/tap_pendo/schemas/track_events.json` & `tap-pendo-0.6.2/tap_pendo/schemas/track_events.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.1/tap_pendo/schemas/track_types.json` & `tap-pendo-0.6.2/tap_pendo/schemas/track_types.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.1/tap_pendo/schemas/visitor_history.json` & `tap-pendo-0.6.2/tap_pendo/schemas/visitor_history.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.1/tap_pendo/schemas/visitors.json` & `tap-pendo-0.6.2/tap_pendo/schemas/visitors.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.1/tap_pendo/streams.py` & `tap-pendo-0.6.2/tap_pendo/streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -677,17 +677,18 @@
 
         update_currently_syncing(state, None)
         return (self.stream, stream_records), loop_for_records
 
     def lookback_window(self):
         # Get lookback window from config and verify value
         lookback_window = self.config.get('lookback_window') or '0'
-        if not lookback_window.isdigit():
+        try:
+            return int(lookback_window)
+        except:
             raise TypeError(f"lookback_window '{lookback_window}' is not numeric. Check your configuration")
-        return int(lookback_window)
 
 
 class LazyAggregationStream(Stream):
     def send_request_get_results(self, req, endpoint, params, count, **kwargs):
         # Set request timeout to config param `request_timeout` value.
         # If value is 0,"0", "" or None then it will set default to default to 300.0 seconds if not passed in config.
         try:
```

### Comparing `tap-pendo-0.6.1/tap_pendo/sync.py` & `tap-pendo-0.6.2/tap_pendo/sync.py`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.1/tap_pendo/utils.py` & `tap-pendo-0.6.2/tap_pendo/utils.py`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.1/tap_pendo.egg-info/SOURCES.txt` & `tap-pendo-0.6.2/tap_pendo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

