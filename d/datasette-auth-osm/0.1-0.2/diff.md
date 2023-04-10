# Comparing `tmp/datasette-auth-osm-0.1.tar.gz` & `tmp/datasette-auth-osm-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-auth-osm-0.1.tar", last modified: Mon Apr 10 20:17:21 2023, max compression
+gzip compressed data, was "datasette-auth-osm-0.2.tar", last modified: Mon Apr 10 21:13:31 2023, max compression
```

## Comparing `datasette-auth-osm-0.1.tar` & `datasette-auth-osm-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:17:21.970986 datasette-auth-osm-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 20:17:06.000000 datasette-auth-osm-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-10 20:17:21.970986 datasette-auth-osm-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-10 20:17:06.000000 datasette-auth-osm-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:17:21.966986 datasette-auth-osm-0.1/datasette_auth_osm/
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-04-10 20:17:06.000000 datasette-auth-osm-0.1/datasette_auth_osm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:17:21.966986 datasette-auth-osm-0.1/datasette_auth_osm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-10 20:17:21.000000 datasette-auth-osm-0.1/datasette_auth_osm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-10 20:17:21.000000 datasette-auth-osm-0.1/datasette_auth_osm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:17:21.000000 datasette-auth-osm-0.1/datasette_auth_osm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-10 20:17:21.000000 datasette-auth-osm-0.1/datasette_auth_osm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-10 20:17:21.000000 datasette-auth-osm-0.1/datasette_auth_osm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-10 20:17:21.000000 datasette-auth-osm-0.1/datasette_auth_osm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 20:17:21.970986 datasette-auth-osm-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-10 20:17:06.000000 datasette-auth-osm-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:17:21.966986 datasette-auth-osm-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-04-10 20:17:06.000000 datasette-auth-osm-0.1/tests/test_auth_osm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:13:31.109705 datasette-auth-osm-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 21:13:04.000000 datasette-auth-osm-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-10 21:13:31.109705 datasette-auth-osm-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-10 21:13:04.000000 datasette-auth-osm-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:13:31.109705 datasette-auth-osm-0.2/datasette_auth_osm/
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-04-10 21:13:04.000000 datasette-auth-osm-0.2/datasette_auth_osm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:13:31.109705 datasette-auth-osm-0.2/datasette_auth_osm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-10 21:13:31.000000 datasette-auth-osm-0.2/datasette_auth_osm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-10 21:13:31.000000 datasette-auth-osm-0.2/datasette_auth_osm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 21:13:31.000000 datasette-auth-osm-0.2/datasette_auth_osm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-10 21:13:31.000000 datasette-auth-osm-0.2/datasette_auth_osm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-10 21:13:31.000000 datasette-auth-osm-0.2/datasette_auth_osm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-10 21:13:31.000000 datasette-auth-osm-0.2/datasette_auth_osm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 21:13:31.109705 datasette-auth-osm-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-10 21:13:04.000000 datasette-auth-osm-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:13:31.109705 datasette-auth-osm-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-04-10 21:13:04.000000 datasette-auth-osm-0.2/tests/test_auth_osm.py
```

### Comparing `datasette-auth-osm-0.1/LICENSE` & `datasette-auth-osm-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-auth-osm-0.1/PKG-INFO` & `datasette-auth-osm-0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-auth-osm
-Version: 0.1
+Version: 0.2
 Summary: Datasette plugin that authenticates users against Openstreetmap
 Home-page: https://github.com/mfa/datasette-auth-osm
 Author: Andreas Madsack
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/mfa/datasette-auth-osm/issues
 Project-URL: CI, https://github.com/mfa/datasette-auth-osm/actions
 Classifier: Framework :: Datasette
@@ -13,15 +13,14 @@
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # datasette-auth-osm
 
 [![PyPI](https://img.shields.io/pypi/v/datasette-auth-osm.svg)](https://pypi.org/project/datasette-auth-osm/)
-[![Changelog](https://img.shields.io/github/v/release/mfa/datasette-auth-osm?include_prereleases&label=changelog)](https://github.com/mfa/datasette-auth-osm/releases)
 [![Tests](https://github.com/mfa/datasette-auth-osm/workflows/Test/badge.svg)](https://github.com/mfa/datasette-auth-osm/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/mfa/datasette-auth-osm/blob/main/LICENSE)
 
 Datasette plugin that authenticates users against OpenStreetMap
 
 ## Installation
 
@@ -31,29 +30,28 @@
 
 ## Demo
 
 You can try this out at [datasette-auth-osm.madflex.de](https://datasette-auth-osm.madflex.de/) - click on the top right menu icon and select "Sign in with OpenStreetMap".
 
 ## Initial configuration
 
-First, create a new application in Auth0. You will need the domain, client ID and client secret for that application.
+First, create a new application in [Openstreetmap - OAuth2 Applications](https://www.openstreetmap.org/oauth2/applications).
+You will need the client ID and client secret for that application.
 
-The domain should be something like `mysite.us.auth0.com`.
-
-Add `http://127.0.0.1:8001/-/auth0-callback` to the list of Allowed Callback URLs.
+Add `http://127.0.0.1:8001/-/osm-callback` to the list of Allowed Callback URLs.
 
 Then configure these plugin secrets using `metadata.yml`:
 
 ```yaml
 plugins:
-  datasette-auth0:
+  datasette-auth-osm:
     client_id:
-      "$env": AUTH0_CLIENT_ID
+      "$env": OSM_CLIENT_ID
     client_secret:
-      "$env": AUTH0_CLIENT_SECRET
+      "$env": OSM_CLIENT_SECRET
 ```
 
 In development, you can run Datasette and pass in environment variables like this:
 ```
 OSM_CLIENT_ID="...client-id-goes-here..." \
 OSM_CLIENT_SECRET="...secret-goes-here..." \
 datasette -m metadata.yml
@@ -63,15 +61,15 @@
 ```
 datasette publish cloudrun mydatabase.db \
 --install datasette-auth-osm \
 --plugin-secret datasette-auth-osm client_id "your-client-id" \
 --plugin-secret datasette-auth-osm client_secret "your-client-secret" \
 --service datasette-auth-osm-demo
 ```
-Once your Datasette instance is deployed, you will need to add its callback URL to the "Allowed Callback URLs" list your [Oauth2 application](https://www.openstreetmap.org/oauth2/applications) in OpenStreetMap.
+Once your Datasette instance is deployed, you will need to add its callback URL to the "Allowed Callback URLs" list your [OAuth2 application](https://www.openstreetmap.org/oauth2/applications) in OpenStreetMap.
 
 The callback URL should be something like:
 
     https://url-to-your-datasette/-/osm-callback
 
 
 ## Development
```

### Comparing `datasette-auth-osm-0.1/README.md` & `datasette-auth-osm-0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # datasette-auth-osm
 
 [![PyPI](https://img.shields.io/pypi/v/datasette-auth-osm.svg)](https://pypi.org/project/datasette-auth-osm/)
-[![Changelog](https://img.shields.io/github/v/release/mfa/datasette-auth-osm?include_prereleases&label=changelog)](https://github.com/mfa/datasette-auth-osm/releases)
 [![Tests](https://github.com/mfa/datasette-auth-osm/workflows/Test/badge.svg)](https://github.com/mfa/datasette-auth-osm/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/mfa/datasette-auth-osm/blob/main/LICENSE)
 
 Datasette plugin that authenticates users against OpenStreetMap
 
 ## Installation
 
@@ -15,29 +14,28 @@
 
 ## Demo
 
 You can try this out at [datasette-auth-osm.madflex.de](https://datasette-auth-osm.madflex.de/) - click on the top right menu icon and select "Sign in with OpenStreetMap".
 
 ## Initial configuration
 
-First, create a new application in Auth0. You will need the domain, client ID and client secret for that application.
+First, create a new application in [Openstreetmap - OAuth2 Applications](https://www.openstreetmap.org/oauth2/applications).
+You will need the client ID and client secret for that application.
 
-The domain should be something like `mysite.us.auth0.com`.
-
-Add `http://127.0.0.1:8001/-/auth0-callback` to the list of Allowed Callback URLs.
+Add `http://127.0.0.1:8001/-/osm-callback` to the list of Allowed Callback URLs.
 
 Then configure these plugin secrets using `metadata.yml`:
 
 ```yaml
 plugins:
-  datasette-auth0:
+  datasette-auth-osm:
     client_id:
-      "$env": AUTH0_CLIENT_ID
+      "$env": OSM_CLIENT_ID
     client_secret:
-      "$env": AUTH0_CLIENT_SECRET
+      "$env": OSM_CLIENT_SECRET
 ```
 
 In development, you can run Datasette and pass in environment variables like this:
 ```
 OSM_CLIENT_ID="...client-id-goes-here..." \
 OSM_CLIENT_SECRET="...secret-goes-here..." \
 datasette -m metadata.yml
@@ -47,15 +45,15 @@
 ```
 datasette publish cloudrun mydatabase.db \
 --install datasette-auth-osm \
 --plugin-secret datasette-auth-osm client_id "your-client-id" \
 --plugin-secret datasette-auth-osm client_secret "your-client-secret" \
 --service datasette-auth-osm-demo
 ```
-Once your Datasette instance is deployed, you will need to add its callback URL to the "Allowed Callback URLs" list your [Oauth2 application](https://www.openstreetmap.org/oauth2/applications) in OpenStreetMap.
+Once your Datasette instance is deployed, you will need to add its callback URL to the "Allowed Callback URLs" list your [OAuth2 application](https://www.openstreetmap.org/oauth2/applications) in OpenStreetMap.
 
 The callback URL should be something like:
 
     https://url-to-your-datasette/-/osm-callback
 
 
 ## Development
```

### Comparing `datasette-auth-osm-0.1/datasette_auth_osm/__init__.py` & `datasette-auth-osm-0.2/datasette_auth_osm/__init__.py`

 * *Files identical despite different names*

### Comparing `datasette-auth-osm-0.1/datasette_auth_osm.egg-info/PKG-INFO` & `datasette-auth-osm-0.2/datasette_auth_osm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-auth-osm
-Version: 0.1
+Version: 0.2
 Summary: Datasette plugin that authenticates users against Openstreetmap
 Home-page: https://github.com/mfa/datasette-auth-osm
 Author: Andreas Madsack
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/mfa/datasette-auth-osm/issues
 Project-URL: CI, https://github.com/mfa/datasette-auth-osm/actions
 Classifier: Framework :: Datasette
@@ -13,15 +13,14 @@
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # datasette-auth-osm
 
 [![PyPI](https://img.shields.io/pypi/v/datasette-auth-osm.svg)](https://pypi.org/project/datasette-auth-osm/)
-[![Changelog](https://img.shields.io/github/v/release/mfa/datasette-auth-osm?include_prereleases&label=changelog)](https://github.com/mfa/datasette-auth-osm/releases)
 [![Tests](https://github.com/mfa/datasette-auth-osm/workflows/Test/badge.svg)](https://github.com/mfa/datasette-auth-osm/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/mfa/datasette-auth-osm/blob/main/LICENSE)
 
 Datasette plugin that authenticates users against OpenStreetMap
 
 ## Installation
 
@@ -31,29 +30,28 @@
 
 ## Demo
 
 You can try this out at [datasette-auth-osm.madflex.de](https://datasette-auth-osm.madflex.de/) - click on the top right menu icon and select "Sign in with OpenStreetMap".
 
 ## Initial configuration
 
-First, create a new application in Auth0. You will need the domain, client ID and client secret for that application.
+First, create a new application in [Openstreetmap - OAuth2 Applications](https://www.openstreetmap.org/oauth2/applications).
+You will need the client ID and client secret for that application.
 
-The domain should be something like `mysite.us.auth0.com`.
-
-Add `http://127.0.0.1:8001/-/auth0-callback` to the list of Allowed Callback URLs.
+Add `http://127.0.0.1:8001/-/osm-callback` to the list of Allowed Callback URLs.
 
 Then configure these plugin secrets using `metadata.yml`:
 
 ```yaml
 plugins:
-  datasette-auth0:
+  datasette-auth-osm:
     client_id:
-      "$env": AUTH0_CLIENT_ID
+      "$env": OSM_CLIENT_ID
     client_secret:
-      "$env": AUTH0_CLIENT_SECRET
+      "$env": OSM_CLIENT_SECRET
 ```
 
 In development, you can run Datasette and pass in environment variables like this:
 ```
 OSM_CLIENT_ID="...client-id-goes-here..." \
 OSM_CLIENT_SECRET="...secret-goes-here..." \
 datasette -m metadata.yml
@@ -63,15 +61,15 @@
 ```
 datasette publish cloudrun mydatabase.db \
 --install datasette-auth-osm \
 --plugin-secret datasette-auth-osm client_id "your-client-id" \
 --plugin-secret datasette-auth-osm client_secret "your-client-secret" \
 --service datasette-auth-osm-demo
 ```
-Once your Datasette instance is deployed, you will need to add its callback URL to the "Allowed Callback URLs" list your [Oauth2 application](https://www.openstreetmap.org/oauth2/applications) in OpenStreetMap.
+Once your Datasette instance is deployed, you will need to add its callback URL to the "Allowed Callback URLs" list your [OAuth2 application](https://www.openstreetmap.org/oauth2/applications) in OpenStreetMap.
 
 The callback URL should be something like:
 
     https://url-to-your-datasette/-/osm-callback
 
 
 ## Development
```

### Comparing `datasette-auth-osm-0.1/setup.py` & `datasette-auth-osm-0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.1"
+VERSION = "0.2"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `datasette-auth-osm-0.1/tests/test_auth_osm.py` & `datasette-auth-osm-0.2/tests/test_auth_osm.py`

 * *Files identical despite different names*

