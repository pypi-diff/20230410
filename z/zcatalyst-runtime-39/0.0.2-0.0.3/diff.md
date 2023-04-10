# Comparing `tmp/zcatalyst_runtime_39-0.0.2.tar.gz` & `tmp/zcatalyst_runtime_39-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zcatalyst_runtime_39-0.0.2.tar", last modified: Wed Mar 15 09:57:25 2023, max compression
+gzip compressed data, was "zcatalyst_runtime_39-0.0.3.tar", last modified: Fri Apr  7 05:23:18 2023, max compression
```

## Comparing `zcatalyst_runtime_39-0.0.2.tar` & `zcatalyst_runtime_39-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 vignesh-11323 (618215590) domain^users (618136065)        0 2023-03-15 09:57:25.140330 zcatalyst_runtime_39-0.0.2/
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      639 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.2/LICENSE
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      129 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.2/MANIFEST.in
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      879 2023-03-15 09:57:25.140330 zcatalyst_runtime_39-0.0.2/PKG-INFO
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      251 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.2/README.md
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)       38 2023-03-15 09:57:25.140330 zcatalyst_runtime_39-0.0.2/setup.cfg
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1392 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.2/setup.py
-drwxr-xr-x   0 vignesh-11323 (618215590) domain^users (618136065)        0 2023-03-15 09:57:25.140330 zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39/
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)        1 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39/__init__.py
-drwxr-xr-x   0 vignesh-11323 (618215590) domain^users (618136065)        0 2023-03-15 09:57:25.140330 zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39/flavours/
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     2494 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39/flavours/__init__.py
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      306 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39/flavours/applogic.py
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1899 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39/flavours/basicio.py
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1705 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39/flavours/cron.py
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1926 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39/flavours/event.py
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1075 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39/flavours/integration.py
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      744 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39/flavours/utils.py
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1805 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39/init_handler.py
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1829 2023-03-10 07:50:09.000000 zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39/log_handler.py
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     7283 2023-03-15 09:56:42.000000 zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39/main.py
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      271 2023-03-15 09:56:42.000000 zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39/meta.json
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)       25 2023-03-15 09:56:42.000000 zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39/requirements-prod.txt
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)       10 2023-03-15 09:56:42.000000 zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39/requirements.txt
-drwxr-xr-x   0 vignesh-11323 (618215590) domain^users (618136065)        0 2023-03-15 09:57:25.140330 zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39.egg-info/
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      879 2023-03-15 09:57:25.000000 zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39.egg-info/PKG-INFO
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      747 2023-03-15 09:57:25.000000 zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39.egg-info/SOURCES.txt
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)        1 2023-03-15 09:57:25.000000 zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39.egg-info/dependency_links.txt
--rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)       21 2023-03-15 09:57:25.000000 zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39.egg-info/top_level.txt
+drwxr-xr-x   0 vignesh-11323 (618215590) domain^users (618136065)        0 2023-04-07 05:23:18.072115 zcatalyst_runtime_39-0.0.3/
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      639 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.3/LICENSE
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      129 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.3/MANIFEST.in
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      879 2023-04-07 05:23:18.072115 zcatalyst_runtime_39-0.0.3/PKG-INFO
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      251 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.3/README.md
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)       38 2023-04-07 05:23:18.072115 zcatalyst_runtime_39-0.0.3/setup.cfg
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1392 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.3/setup.py
+drwxr-xr-x   0 vignesh-11323 (618215590) domain^users (618136065)        0 2023-04-07 05:23:18.072115 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)        1 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/__init__.py
+drwxr-xr-x   0 vignesh-11323 (618215590) domain^users (618136065)        0 2023-04-07 05:23:18.072115 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     2494 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/__init__.py
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      306 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/applogic.py
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1899 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/basicio.py
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1705 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/cron.py
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1926 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/event.py
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1075 2023-03-07 13:22:44.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/integration.py
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      794 2023-04-07 05:22:03.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/utils.py
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1805 2023-04-06 05:53:57.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/init_handler.py
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     1829 2023-03-10 07:50:09.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/log_handler.py
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)     7283 2023-03-15 09:56:42.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/main.py
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      271 2023-04-07 05:22:03.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/meta.json
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)       25 2023-03-15 09:56:42.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/requirements-prod.txt
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)       10 2023-03-15 09:56:42.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/requirements.txt
+drwxr-xr-x   0 vignesh-11323 (618215590) domain^users (618136065)        0 2023-04-07 05:23:18.072115 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39.egg-info/
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      879 2023-04-07 05:23:18.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39.egg-info/PKG-INFO
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)      747 2023-04-07 05:23:18.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39.egg-info/SOURCES.txt
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)        1 2023-04-07 05:23:18.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39.egg-info/dependency_links.txt
+-rw-r--r--   0 vignesh-11323 (618215590) domain^users (618136065)       21 2023-04-07 05:23:18.000000 zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39.egg-info/top_level.txt
```

### Comparing `zcatalyst_runtime_39-0.0.2/LICENSE` & `zcatalyst_runtime_39-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zcatalyst_runtime_39-0.0.2/PKG-INFO` & `zcatalyst_runtime_39-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: zcatalyst_runtime_39
-Version: 0.0.2
-Summary: Catalyst runtime for Python 3.9-d68ae7e
+Version: 0.0.3
+Summary: Catalyst runtime for Python 3.9-fd917f8
 Home-page: https://catalyst.zoho.com/
 Author: Catalyst by Zoho
 Author-email: support@zohocatalyst.com
 Maintainer: Catalyst by Zoho
 Maintainer-email: support@zohocatalyst.com
 License: Apache 2.0
 Keywords: zcatalyst,zoho,catalyst,serverless
```

### Comparing `zcatalyst_runtime_39-0.0.2/setup.py` & `zcatalyst_runtime_39-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39/flavours/__init__.py` & `zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/__init__.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39/flavours/basicio.py` & `zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/basicio.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39/flavours/cron.py` & `zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/cron.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39/flavours/event.py` & `zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/event.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39/flavours/integration.py` & `zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/integration.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39/flavours/utils.py` & `zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/flavours/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,12 +15,13 @@
     catalyst_body = request.get_data()
     return json.loads(catalyst_body) if catalyst_body else {}
 
 def send_json_response(status_code: int, message: dict = None) -> None:
     g.response.status_code = status_code
 
     if message:
-        g.response.headers.add('Content-Type', 'application/json')
+        g.response.content_type = 'application/json; charset=utf-8'
+        g.response.mimetype = 'application/json'
 
         message_str = json.dumps(message)
         g.response.set_data(message_str)
```

### Comparing `zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39/init_handler.py` & `zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/init_handler.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39/log_handler.py` & `zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/log_handler.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39/main.py` & `zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39/main.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39.egg-info/PKG-INFO` & `zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: zcatalyst-runtime-39
-Version: 0.0.2
-Summary: Catalyst runtime for Python 3.9-d68ae7e
+Version: 0.0.3
+Summary: Catalyst runtime for Python 3.9-fd917f8
 Home-page: https://catalyst.zoho.com/
 Author: Catalyst by Zoho
 Author-email: support@zohocatalyst.com
 Maintainer: Catalyst by Zoho
 Maintainer-email: support@zohocatalyst.com
 License: Apache 2.0
 Keywords: zcatalyst,zoho,catalyst,serverless
```

### Comparing `zcatalyst_runtime_39-0.0.2/zcatalyst_runtime_39.egg-info/SOURCES.txt` & `zcatalyst_runtime_39-0.0.3/zcatalyst_runtime_39.egg-info/SOURCES.txt`

 * *Files identical despite different names*

