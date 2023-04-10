# Comparing `tmp/mofdb_client-0.8.0.tar.gz` & `tmp/mofdb_client-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mofdb_client-0.8.0.tar", last modified: Sun Dec 11 21:10:23 2022, max compression
+gzip compressed data, was "mofdb_client-0.9.0.tar", last modified: Wed Jan  4 23:42:35 2023, max compression
```

## Comparing `mofdb_client-0.8.0.tar` & `mofdb_client-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 n8ta       (501) staff       (20)        0 2022-12-11 21:10:23.241784 mofdb_client-0.8.0/
--rw-r--r--   0 n8ta       (501) staff       (20)     1062 2022-11-22 20:30:19.000000 mofdb_client-0.8.0/LICENSE
--rw-r--r--   0 n8ta       (501) staff       (20)     4389 2022-12-11 21:10:23.242248 mofdb_client-0.8.0/PKG-INFO
--rw-r--r--   0 n8ta       (501) staff       (20)     3704 2022-12-11 21:06:18.000000 mofdb_client-0.8.0/README.md
--rw-r--r--   0 n8ta       (501) staff       (20)       84 2022-11-22 20:30:19.000000 mofdb_client-0.8.0/pyproject.toml
--rw-r--r--   0 n8ta       (501) staff       (20)      932 2022-12-11 21:10:23.243790 mofdb_client-0.8.0/setup.cfg
-drwxr-xr-x   0 n8ta       (501) staff       (20)        0 2022-12-11 21:10:23.233127 mofdb_client-0.8.0/src/
-drwxr-xr-x   0 n8ta       (501) staff       (20)        0 2022-12-11 21:10:23.238199 mofdb_client-0.8.0/src/mofdb_client/
--rw-r--r--   0 n8ta       (501) staff       (20)       36 2022-11-25 07:26:42.000000 mofdb_client-0.8.0/src/mofdb_client/__init__.py
--rw-r--r--   0 n8ta       (501) staff       (20)      361 2022-11-22 20:30:19.000000 mofdb_client-0.8.0/src/mofdb_client/adsorbate.py
--rw-r--r--   0 n8ta       (501) staff       (20)      185 2022-11-22 20:30:19.000000 mofdb_client-0.8.0/src/mofdb_client/adsorbent.py
--rw-r--r--   0 n8ta       (501) staff       (20)      318 2022-11-22 20:30:19.000000 mofdb_client-0.8.0/src/mofdb_client/element.py
--rw-r--r--   0 n8ta       (501) staff       (20)     1495 2022-11-22 20:30:19.000000 mofdb_client-0.8.0/src/mofdb_client/isotherm.py
--rw-r--r--   0 n8ta       (501) staff       (20)     6172 2022-12-11 21:06:58.000000 mofdb_client-0.8.0/src/mofdb_client/main.py
--rw-r--r--   0 n8ta       (501) staff       (20)     1698 2022-11-23 06:40:10.000000 mofdb_client-0.8.0/src/mofdb_client/mof.py
--rw-r--r--   0 n8ta       (501) staff       (20)      992 2022-11-22 20:30:19.000000 mofdb_client-0.8.0/src/mofdb_client/temperature_point.py
-drwxr-xr-x   0 n8ta       (501) staff       (20)        0 2022-12-11 21:10:23.241118 mofdb_client-0.8.0/src/mofdb_client.egg-info/
--rw-r--r--   0 n8ta       (501) staff       (20)     4389 2022-12-11 21:10:23.000000 mofdb_client-0.8.0/src/mofdb_client.egg-info/PKG-INFO
--rw-r--r--   0 n8ta       (501) staff       (20)      474 2022-12-11 21:10:23.000000 mofdb_client-0.8.0/src/mofdb_client.egg-info/SOURCES.txt
--rw-r--r--   0 n8ta       (501) staff       (20)        1 2022-12-11 21:10:23.000000 mofdb_client-0.8.0/src/mofdb_client.egg-info/dependency_links.txt
--rw-r--r--   0 n8ta       (501) staff       (20)       77 2022-12-11 21:10:23.000000 mofdb_client-0.8.0/src/mofdb_client.egg-info/requires.txt
--rw-r--r--   0 n8ta       (501) staff       (20)       13 2022-12-11 21:10:23.000000 mofdb_client-0.8.0/src/mofdb_client.egg-info/top_level.txt
+drwxr-xr-x   0 n8ta       (501) staff       (20)        0 2023-01-04 23:42:35.497630 mofdb_client-0.9.0/
+-rw-r--r--   0 n8ta       (501) staff       (20)     1062 2022-11-22 20:30:19.000000 mofdb_client-0.9.0/LICENSE
+-rw-r--r--   0 n8ta       (501) staff       (20)     4563 2023-01-04 23:42:35.497852 mofdb_client-0.9.0/PKG-INFO
+-rw-r--r--   0 n8ta       (501) staff       (20)     3878 2023-01-04 23:42:22.000000 mofdb_client-0.9.0/README.md
+-rw-r--r--   0 n8ta       (501) staff       (20)       84 2022-11-22 20:30:19.000000 mofdb_client-0.9.0/pyproject.toml
+-rw-r--r--   0 n8ta       (501) staff       (20)      932 2023-01-04 23:42:35.498773 mofdb_client-0.9.0/setup.cfg
+drwxr-xr-x   0 n8ta       (501) staff       (20)        0 2023-01-04 23:42:35.488958 mofdb_client-0.9.0/src/
+drwxr-xr-x   0 n8ta       (501) staff       (20)        0 2023-01-04 23:42:35.495201 mofdb_client-0.9.0/src/mofdb_client/
+-rw-r--r--   0 n8ta       (501) staff       (20)       36 2022-11-25 07:26:42.000000 mofdb_client-0.9.0/src/mofdb_client/__init__.py
+-rw-r--r--   0 n8ta       (501) staff       (20)      361 2022-11-22 20:30:19.000000 mofdb_client-0.9.0/src/mofdb_client/adsorbate.py
+-rw-r--r--   0 n8ta       (501) staff       (20)      185 2022-11-22 20:30:19.000000 mofdb_client-0.9.0/src/mofdb_client/adsorbent.py
+-rw-r--r--   0 n8ta       (501) staff       (20)      318 2022-11-22 20:30:19.000000 mofdb_client-0.9.0/src/mofdb_client/element.py
+-rw-r--r--   0 n8ta       (501) staff       (20)     1495 2022-11-22 20:30:19.000000 mofdb_client-0.9.0/src/mofdb_client/isotherm.py
+-rw-r--r--   0 n8ta       (501) staff       (20)     6291 2023-01-04 23:41:40.000000 mofdb_client-0.9.0/src/mofdb_client/main.py
+-rw-r--r--   0 n8ta       (501) staff       (20)     1698 2022-11-23 06:40:10.000000 mofdb_client-0.9.0/src/mofdb_client/mof.py
+-rw-r--r--   0 n8ta       (501) staff       (20)      992 2022-11-22 20:30:19.000000 mofdb_client-0.9.0/src/mofdb_client/temperature_point.py
+drwxr-xr-x   0 n8ta       (501) staff       (20)        0 2023-01-04 23:42:35.497234 mofdb_client-0.9.0/src/mofdb_client.egg-info/
+-rw-r--r--   0 n8ta       (501) staff       (20)     4563 2023-01-04 23:42:35.000000 mofdb_client-0.9.0/src/mofdb_client.egg-info/PKG-INFO
+-rw-r--r--   0 n8ta       (501) staff       (20)      474 2023-01-04 23:42:35.000000 mofdb_client-0.9.0/src/mofdb_client.egg-info/SOURCES.txt
+-rw-r--r--   0 n8ta       (501) staff       (20)        1 2023-01-04 23:42:35.000000 mofdb_client-0.9.0/src/mofdb_client.egg-info/dependency_links.txt
+-rw-r--r--   0 n8ta       (501) staff       (20)       77 2023-01-04 23:42:35.000000 mofdb_client-0.9.0/src/mofdb_client.egg-info/requires.txt
+-rw-r--r--   0 n8ta       (501) staff       (20)       13 2023-01-04 23:42:35.000000 mofdb_client-0.9.0/src/mofdb_client.egg-info/top_level.txt
```

### Comparing `mofdb_client-0.8.0/LICENSE` & `mofdb_client-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mofdb_client-0.8.0/PKG-INFO` & `mofdb_client-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mofdb_client
-Version: 0.8.0
+Version: 0.9.0
 Summary: Simple client for fetching data from mofdb
 Home-page: https://github.com/n8ta/mofdb-client
 Author: Nathaniel Tracy-Amoroso
 Author-email: n8@u.northwestern.edu
 Maintainer: Nathaniel Tracy-Amoroso
 Maintainer-email: n8@u.northwestern.edu
 License: MIT License
@@ -23,15 +23,15 @@
 
 A typed, fast, lightweight, client wrapping the [mofdb api](https://mof.tech.northwestern.edu/api). This client is the fastest way to access
 mofdb since it utilizes the streaming bulk API. Using the regular paginated API will be slow for large page numbers.
 
 ### Installation
 
 ```shell
-python3 -m pip install mofdb_client==0.6.0
+python3 -m pip install mofdb_client==0.9.0
 ```
 
 ### Example
 
 ![Example of mofdb-client IDE autocompletion](assets/screen0.png)
 
 ```python3
@@ -83,15 +83,15 @@
 units/pressures and throw `InvalidUnit` exception.
 
 ### Design Note
 `fetch` is lazy because mofDB is large. Be sure to loop over it with `for mof in fetch()` and NOT `for mof in list(fetch())` since 
 building the list will download all the mofs before it starts processing and this will be very slow and may well run out of memory.
 
 ### Compatibility
-Tested on Python 3.7 to 3.9.
+[Tested](https://app.travis-ci.com/github/n8ta/mofdb-client) on Python 3.7 to 3.11. 
 
 ### Future Enhancements:
 - [ ] Retries for transient network failures with exponential backoff
 - [X] Support for unit conversions
 - [ ] Only download some columns to save time/bandwidth?
 
 ### Telemetry
@@ -113,10 +113,14 @@
 ```
 python3 -m build -n
 python3 -m twine upload dist/*
 ```
 
 ### Change log
 
+
+#### 0.9.0
+Do not report mofdb exceptions like "InvalidUnit" to sentry error monitoring. These indicate user error.
+
 #### 0.8.0
 Fix for crashes on queries returning no mofs. Required a change to mofdb repo as well. Add a 204.response file to zip stream to signal empty response.
```

### Comparing `mofdb_client-0.8.0/README.md` & `mofdb_client-0.9.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 A typed, fast, lightweight, client wrapping the [mofdb api](https://mof.tech.northwestern.edu/api). This client is the fastest way to access
 mofdb since it utilizes the streaming bulk API. Using the regular paginated API will be slow for large page numbers.
 
 ### Installation
 
 ```shell
-python3 -m pip install mofdb_client==0.6.0
+python3 -m pip install mofdb_client==0.9.0
 ```
 
 ### Example
 
 ![Example of mofdb-client IDE autocompletion](assets/screen0.png)
 
 ```python3
@@ -63,15 +63,15 @@
 units/pressures and throw `InvalidUnit` exception.
 
 ### Design Note
 `fetch` is lazy because mofDB is large. Be sure to loop over it with `for mof in fetch()` and NOT `for mof in list(fetch())` since 
 building the list will download all the mofs before it starts processing and this will be very slow and may well run out of memory.
 
 ### Compatibility
-Tested on Python 3.7 to 3.9.
+[Tested](https://app.travis-ci.com/github/n8ta/mofdb-client) on Python 3.7 to 3.11. 
 
 ### Future Enhancements:
 - [ ] Retries for transient network failures with exponential backoff
 - [X] Support for unit conversions
 - [ ] Only download some columns to save time/bandwidth?
 
 ### Telemetry
@@ -93,9 +93,13 @@
 ```
 python3 -m build -n
 python3 -m twine upload dist/*
 ```
 
 ### Change log
 
+
+#### 0.9.0
+Do not report mofdb exceptions like "InvalidUnit" to sentry error monitoring. These indicate user error.
+
 #### 0.8.0
 Fix for crashes on queries returning no mofs. Required a change to mofdb repo as well. Add a 204.response file to zip stream to signal empty response.
```

### Comparing `mofdb_client-0.8.0/setup.cfg` & `mofdb_client-0.9.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mofdb_client
-version = 0.8.0
+version = 0.9.0
 author = Nathaniel Tracy-Amoroso
 author_email = n8@u.northwestern.edu
 maintainer = Nathaniel Tracy-Amoroso
 maintainer_email = n8@u.northwestern.edu
 license = MIT License
 license_file = LICENSE
 description = Simple client for fetching data from mofdb
```

### Comparing `mofdb_client-0.8.0/src/mofdb_client/isotherm.py` & `mofdb_client-0.9.0/src/mofdb_client/isotherm.py`

 * *Files identical despite different names*

### Comparing `mofdb_client-0.8.0/src/mofdb_client/main.py` & `mofdb_client-0.9.0/src/mofdb_client/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,17 +49,20 @@
         data = b""
         for chunk in unzipped_chunks:
             data += chunk
         loaded = json.loads(data)
         yield Mof(loaded)
 
 
-class InvalidUnit(Exception):
+
+class MofdbClientexception(Exception):
     pass
 
+class InvalidUnit(MofdbClientexception):
+    pass
 
 def fetch(mofid: str = None,
           mofkey: str = None,
           vf_min: float = None,
           vf_max: float = None,
           lcd_min: float = None,
           lcd_max: float = None,
@@ -79,14 +82,16 @@
         # Catch, log, and re-raise exceptions in telemetry mode
         try:
             yield from fetch_inner(mofid=mofid, mofkey=mofkey, vf_min=vf_min, vf_max=vf_max, lcd_min=lcd_min,
                                    lcd_max=lcd_max, pld_min=pld_min, pld_max=pld_max, sa_m2g_min=sa_m2g_min,
                                    sa_m2g_max=sa_m2g_max, sa_m2cm3_min=sa_m2cm3_min,
                                    sa_m2cm3_max=sa_m2cm3_max, name=name, pressure_unit=pressure_unit, loading_unit=loading_unit,
                                    limit=limit)
+        except MofdbClientexception as e:
+            pass
         except Exception as e:
             import sentry_sdk
             sentry_sdk.init("https://287d83a67df94a3288777a876182cfcc@o310079.ingest.sentry.io/6290292",
                             traces_sample_rate=0.0)
             sentry_sdk.capture_exception(e)
             raise e
     else:
```

### Comparing `mofdb_client-0.8.0/src/mofdb_client/mof.py` & `mofdb_client-0.9.0/src/mofdb_client/mof.py`

 * *Files identical despite different names*

### Comparing `mofdb_client-0.8.0/src/mofdb_client/temperature_point.py` & `mofdb_client-0.9.0/src/mofdb_client/temperature_point.py`

 * *Files identical despite different names*

### Comparing `mofdb_client-0.8.0/src/mofdb_client.egg-info/PKG-INFO` & `mofdb_client-0.9.0/src/mofdb_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mofdb-client
-Version: 0.8.0
+Version: 0.9.0
 Summary: Simple client for fetching data from mofdb
 Home-page: https://github.com/n8ta/mofdb-client
 Author: Nathaniel Tracy-Amoroso
 Author-email: n8@u.northwestern.edu
 Maintainer: Nathaniel Tracy-Amoroso
 Maintainer-email: n8@u.northwestern.edu
 License: MIT License
@@ -23,15 +23,15 @@
 
 A typed, fast, lightweight, client wrapping the [mofdb api](https://mof.tech.northwestern.edu/api). This client is the fastest way to access
 mofdb since it utilizes the streaming bulk API. Using the regular paginated API will be slow for large page numbers.
 
 ### Installation
 
 ```shell
-python3 -m pip install mofdb_client==0.6.0
+python3 -m pip install mofdb_client==0.9.0
 ```
 
 ### Example
 
 ![Example of mofdb-client IDE autocompletion](assets/screen0.png)
 
 ```python3
@@ -83,15 +83,15 @@
 units/pressures and throw `InvalidUnit` exception.
 
 ### Design Note
 `fetch` is lazy because mofDB is large. Be sure to loop over it with `for mof in fetch()` and NOT `for mof in list(fetch())` since 
 building the list will download all the mofs before it starts processing and this will be very slow and may well run out of memory.
 
 ### Compatibility
-Tested on Python 3.7 to 3.9.
+[Tested](https://app.travis-ci.com/github/n8ta/mofdb-client) on Python 3.7 to 3.11. 
 
 ### Future Enhancements:
 - [ ] Retries for transient network failures with exponential backoff
 - [X] Support for unit conversions
 - [ ] Only download some columns to save time/bandwidth?
 
 ### Telemetry
@@ -113,10 +113,14 @@
 ```
 python3 -m build -n
 python3 -m twine upload dist/*
 ```
 
 ### Change log
 
+
+#### 0.9.0
+Do not report mofdb exceptions like "InvalidUnit" to sentry error monitoring. These indicate user error.
+
 #### 0.8.0
 Fix for crashes on queries returning no mofs. Required a change to mofdb repo as well. Add a 204.response file to zip stream to signal empty response.
```

