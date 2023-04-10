# Comparing `tmp/percy-selenium-1.0.5.tar.gz` & `tmp/percy-selenium-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "percy-selenium-1.0.5.tar", last modified: Tue Mar 29 18:06:08 2022, max compression
+gzip compressed data, was "percy-selenium-1.1.0.tar", last modified: Mon Apr 10 08:09:16 2023, max compression
```

## Comparing `percy-selenium-1.0.5.tar` & `percy-selenium-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 18:06:08.580127 percy-selenium-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-03-29 18:05:49.000000 percy-selenium-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2672 2022-03-29 18:06:08.580127 percy-selenium-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1901 2022-03-29 18:05:49.000000 percy-selenium-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 18:06:08.576126 percy-selenium-1.0.5/percy/
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-03-29 18:05:49.000000 percy-selenium-1.0.5/percy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3001 2022-03-29 18:05:49.000000 percy-selenium-1.0.5/percy/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-03-29 18:05:49.000000 percy-selenium-1.0.5/percy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 18:06:08.580127 percy-selenium-1.0.5/percy_selenium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2672 2022-03-29 18:06:07.000000 percy-selenium-1.0.5/percy_selenium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      305 2022-03-29 18:06:08.000000 percy-selenium-1.0.5/percy_selenium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-29 18:06:07.000000 percy-selenium-1.0.5/percy_selenium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-29 18:06:07.000000 percy-selenium-1.0.5/percy_selenium.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-03-29 18:06:08.000000 percy-selenium-1.0.5/percy_selenium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-03-29 18:06:08.000000 percy-selenium-1.0.5/percy_selenium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-29 18:06:08.580127 percy-selenium-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-03-29 18:05:49.000000 percy-selenium-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:09:16.050206 percy-selenium-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-10 08:08:48.000000 percy-selenium-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-10 08:09:16.050206 percy-selenium-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-10 08:08:48.000000 percy-selenium-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:09:16.046206 percy-selenium-1.1.0/percy/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-10 08:08:48.000000 percy-selenium-1.1.0/percy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-10 08:08:48.000000 percy-selenium-1.1.0/percy/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 08:08:48.000000 percy-selenium-1.1.0/percy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:09:16.046206 percy-selenium-1.1.0/percy_selenium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-10 08:09:16.000000 percy-selenium-1.1.0/percy_selenium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-10 08:09:16.000000 percy-selenium-1.1.0/percy_selenium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:09:16.000000 percy-selenium-1.1.0/percy_selenium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:09:16.000000 percy-selenium-1.1.0/percy_selenium.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-10 08:09:16.000000 percy-selenium-1.1.0/percy_selenium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 08:09:16.000000 percy-selenium-1.1.0/percy_selenium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 08:09:16.050206 percy-selenium-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-10 08:08:48.000000 percy-selenium-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:09:16.046206 percy-selenium-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-04-10 08:08:48.000000 percy-selenium-1.1.0/tests/test_snapshot.py
```

### Comparing `percy-selenium-1.0.5/LICENSE` & `percy-selenium-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `percy-selenium-1.0.5/PKG-INFO` & `percy-selenium-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: percy-selenium
-Version: 1.0.5
+Version: 1.1.0
 Summary: Python client for visual testing with Percy
 Home-page: https://github.com/percy/percy-selenium-python
 Author: Perceptual Inc.
 Author-email: team@percy.io
 License: MIT
 Keywords: selenium percy visual testing
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -86,9 +85,7 @@
 
 If you have a previous Percy configuration file, migrate it to the newest version with the
 [`config:migrate`](https://github.com/percy/cli/tree/master/packages/cli-config#percy-configmigrate-filepath-output) command:
 
 ```sh-session
 $ percy config:migrate
 ```
-
-
```

### Comparing `percy-selenium-1.0.5/README.md` & `percy-selenium-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `percy-selenium-1.0.5/percy/snapshot.py` & `percy-selenium-1.1.0/percy/snapshot.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # for logging
 LABEL = '[\u001b[35m' + ('percy:python' if PERCY_DEBUG else 'percy') + '\u001b[39m]'
 
 # Check if Percy is enabled, caching the result so it is only checked once
 @lru_cache(maxsize=None)
 def is_percy_enabled():
     try:
-        response = requests.get(f'{PERCY_CLI_API}/percy/healthcheck')
+        response = requests.get(f'{PERCY_CLI_API}/percy/healthcheck', timeout=30)
         response.raise_for_status()
         data = response.json()
 
         if not data['success']: raise Exception(data['error'])
         version = response.headers.get('x-percy-core-version')
 
         if not version:
@@ -45,15 +45,15 @@
         print(f'{LABEL} Percy is not running, disabling snapshots')
         if PERCY_DEBUG: print(f'{LABEL} {e}')
         return False
 
 # Fetch the @percy/dom script, caching the result so it is only fetched once
 @lru_cache(maxsize=None)
 def fetch_percy_dom():
-    response = requests.get(f'{PERCY_CLI_API}/percy/dom.js')
+    response = requests.get(f'{PERCY_CLI_API}/percy/dom.js', timeout=30)
     response.raise_for_status()
     return response.text
 
 # Take a DOM snapshot and post it to the snapshot endpoint
 def percy_snapshot(driver, name, **kwargs):
     if not is_percy_enabled(): return
 
@@ -61,21 +61,21 @@
         # Inject the DOM serialization script
         driver.execute_script(fetch_percy_dom())
 
         # Serialize and capture the DOM
         dom_snapshot = driver.execute_script(f'return PercyDOM.serialize({json.dumps(kwargs)})')
 
         # Post the DOM to the snapshot endpoint with snapshot options and other info
-        response = requests.post(f'{PERCY_CLI_API}/percy/snapshot', json=dict(**kwargs, **{
+        response = requests.post(f'{PERCY_CLI_API}/percy/snapshot', json={**kwargs, **{
             'client_info': CLIENT_INFO,
             'environment_info': ENV_INFO,
             'dom_snapshot': dom_snapshot,
             'url': driver.current_url,
             'name': name
-        }))
+        }}, timeout=30)
 
         # Handle errors
         response.raise_for_status()
         data = response.json()
 
         if not data['success']: raise Exception(data['error'])
     except Exception as e:
```

### Comparing `percy-selenium-1.0.5/percy_selenium.egg-info/PKG-INFO` & `percy-selenium-1.1.0/percy_selenium.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: percy-selenium
-Version: 1.0.5
+Version: 1.1.0
 Summary: Python client for visual testing with Percy
 Home-page: https://github.com/percy/percy-selenium-python
 Author: Perceptual Inc.
 Author-email: team@percy.io
 License: MIT
 Keywords: selenium percy visual testing
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -86,9 +85,7 @@
 
 If you have a previous Percy configuration file, migrate it to the newest version with the
 [`config:migrate`](https://github.com/percy/cli/tree/master/packages/cli-config#percy-configmigrate-filepath-output) command:
 
 ```sh-session
 $ percy config:migrate
 ```
-
-
```

### Comparing `percy-selenium-1.0.5/setup.py` & `percy-selenium-1.1.0/setup.py`

 * *Files identical despite different names*

