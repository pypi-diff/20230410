# Comparing `tmp/flask-toolkits-0.7.8.tar.gz` & `tmp/flask-toolkits-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-toolkits-0.7.8.tar", last modified: Wed Mar 29 10:00:35 2023, max compression
+gzip compressed data, was "flask-toolkits-0.7.9.tar", last modified: Mon Apr 10 11:55:34 2023, max compression
```

## Comparing `flask-toolkits-0.7.8.tar` & `flask-toolkits-0.7.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-03-29 10:00:35.388061 flask-toolkits-0.7.8/
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1068 2022-03-24 02:48:15.000000 flask-toolkits-0.7.8/LICENSE
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      107 2022-05-19 03:18:55.000000 flask-toolkits-0.7.8/MANIFEST.in
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)    10332 2023-03-29 10:00:35.388061 flask-toolkits-0.7.8/PKG-INFO
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     9383 2022-11-30 23:32:33.000000 flask-toolkits-0.7.8/README.md
-drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-03-29 10:00:35.371640 flask-toolkits-0.7.8/flask_toolkits/
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      258 2022-08-19 06:08:29.000000 flask-toolkits-0.7.8/flask_toolkits/__init__.py
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      315 2022-08-19 06:08:29.000000 flask-toolkits-0.7.8/flask_toolkits/dependencies.py
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      113 2023-03-29 09:57:24.000000 flask-toolkits-0.7.8/flask_toolkits/exceptions.py
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)    16029 2022-08-19 07:14:58.000000 flask-toolkits-0.7.8/flask_toolkits/fields.py
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       71 2022-08-19 06:08:29.000000 flask-toolkits-0.7.8/flask_toolkits/middleware.py
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      985 2022-08-19 06:08:29.000000 flask-toolkits-0.7.8/flask_toolkits/params.py
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     2966 2022-12-10 03:46:35.000000 flask-toolkits-0.7.8/flask_toolkits/responses.py
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)    32407 2023-03-29 09:57:24.000000 flask-toolkits-0.7.8/flask_toolkits/routing.py
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     2198 2023-03-29 09:58:11.000000 flask-toolkits-0.7.8/flask_toolkits/schemas.py
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     2800 2022-08-19 06:08:29.000000 flask-toolkits-0.7.8/flask_toolkits/security.py
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     2859 2022-08-19 06:08:29.000000 flask-toolkits-0.7.8/flask_toolkits/status.py
-drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-03-29 10:00:35.371640 flask-toolkits-0.7.8/flask_toolkits/swagger/
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1269 2022-08-19 06:08:29.000000 flask-toolkits-0.7.8/flask_toolkits/swagger/__init__.py
-drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-03-29 10:00:35.388061 flask-toolkits-0.7.8/flask_toolkits/swagger/dist/
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      665 2022-08-19 06:08:29.000000 flask-toolkits-0.7.8/flask_toolkits/swagger/dist/favicon-16x16.png
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      628 2022-08-19 06:08:29.000000 flask-toolkits-0.7.8/flask_toolkits/swagger/dist/favicon-32x32.png
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      202 2022-08-19 06:08:29.000000 flask-toolkits-0.7.8/flask_toolkits/swagger/dist/index.css
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      734 2022-08-19 06:08:29.000000 flask-toolkits-0.7.8/flask_toolkits/swagger/dist/index.html
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     2690 2022-08-19 06:08:29.000000 flask-toolkits-0.7.8/flask_toolkits/swagger/dist/oauth2-redirect.html
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      539 2022-08-19 06:08:29.000000 flask-toolkits-0.7.8/flask_toolkits/swagger/dist/swagger-initializer.js
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)  1095130 2022-08-19 06:08:29.000000 flask-toolkits-0.7.8/flask_toolkits/swagger/dist/swagger-ui-bundle.js
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)   406408 2022-08-19 06:08:29.000000 flask-toolkits-0.7.8/flask_toolkits/swagger/dist/swagger-ui-es-bundle-core.js
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)  1094892 2022-08-19 06:08:29.000000 flask-toolkits-0.7.8/flask_toolkits/swagger/dist/swagger-ui-es-bundle.js
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)   339540 2022-08-19 06:08:29.000000 flask-toolkits-0.7.8/flask_toolkits/swagger/dist/swagger-ui-standalone-preset.js
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)   143980 2022-08-19 06:08:29.000000 flask-toolkits-0.7.8/flask_toolkits/swagger/dist/swagger-ui.css
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)   286682 2022-08-19 06:08:29.000000 flask-toolkits-0.7.8/flask_toolkits/swagger/dist/swagger-ui.js
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     3034 2022-08-19 06:08:29.000000 flask-toolkits-0.7.8/flask_toolkits/swagger/flask_swagger_ui.py
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)    18794 2022-11-30 03:16:56.000000 flask-toolkits-0.7.8/flask_toolkits/swagger/swagger.py
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     5776 2022-08-19 06:08:29.000000 flask-toolkits-0.7.8/flask_toolkits/swagger/template.py
-drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-03-29 10:00:35.388061 flask-toolkits-0.7.8/flask_toolkits/swagger/templates/
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     2661 2022-08-19 06:08:29.000000 flask-toolkits-0.7.8/flask_toolkits/swagger/templates/index.template.html
-drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-03-29 10:00:35.371640 flask-toolkits-0.7.8/flask_toolkits.egg-info/
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)    10332 2023-03-29 10:00:35.000000 flask-toolkits-0.7.8/flask_toolkits.egg-info/PKG-INFO
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1297 2023-03-29 10:00:35.000000 flask-toolkits-0.7.8/flask_toolkits.egg-info/SOURCES.txt
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)        1 2023-03-29 10:00:35.000000 flask-toolkits-0.7.8/flask_toolkits.egg-info/dependency_links.txt
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       72 2023-03-29 10:00:35.000000 flask-toolkits-0.7.8/flask_toolkits.egg-info/requires.txt
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       15 2023-03-29 10:00:35.000000 flask-toolkits-0.7.8/flask_toolkits.egg-info/top_level.txt
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       38 2023-03-29 10:00:35.388061 flask-toolkits-0.7.8/setup.cfg
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1499 2023-03-29 09:59:04.000000 flask-toolkits-0.7.8/setup.py
+drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-04-10 11:55:34.805925 flask-toolkits-0.7.9/
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1068 2022-03-24 02:48:15.000000 flask-toolkits-0.7.9/LICENSE
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      107 2022-05-19 03:18:55.000000 flask-toolkits-0.7.9/MANIFEST.in
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)    10332 2023-04-10 11:55:34.805925 flask-toolkits-0.7.9/PKG-INFO
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     9383 2022-11-30 23:32:33.000000 flask-toolkits-0.7.9/README.md
+drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-04-10 11:55:34.653921 flask-toolkits-0.7.9/flask_toolkits/
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      258 2022-08-19 06:08:29.000000 flask-toolkits-0.7.9/flask_toolkits/__init__.py
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      315 2022-08-19 06:08:29.000000 flask-toolkits-0.7.9/flask_toolkits/dependencies.py
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      113 2023-03-29 09:57:24.000000 flask-toolkits-0.7.9/flask_toolkits/exceptions.py
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)    16029 2022-08-19 07:14:58.000000 flask-toolkits-0.7.9/flask_toolkits/fields.py
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       71 2022-08-19 06:08:29.000000 flask-toolkits-0.7.9/flask_toolkits/middleware.py
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      985 2022-08-19 06:08:29.000000 flask-toolkits-0.7.9/flask_toolkits/params.py
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     2966 2022-12-10 03:46:35.000000 flask-toolkits-0.7.9/flask_toolkits/responses.py
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)    32407 2023-03-29 09:57:24.000000 flask-toolkits-0.7.9/flask_toolkits/routing.py
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     2198 2023-03-29 09:58:11.000000 flask-toolkits-0.7.9/flask_toolkits/schemas.py
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     2800 2022-08-19 06:08:29.000000 flask-toolkits-0.7.9/flask_toolkits/security.py
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     2859 2022-08-19 06:08:29.000000 flask-toolkits-0.7.9/flask_toolkits/status.py
+drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-04-10 11:55:34.657921 flask-toolkits-0.7.9/flask_toolkits/swagger/
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1269 2022-08-19 06:08:29.000000 flask-toolkits-0.7.9/flask_toolkits/swagger/__init__.py
+drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-04-10 11:55:34.793924 flask-toolkits-0.7.9/flask_toolkits/swagger/dist/
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      665 2022-08-19 06:08:29.000000 flask-toolkits-0.7.9/flask_toolkits/swagger/dist/favicon-16x16.png
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      628 2022-08-19 06:08:29.000000 flask-toolkits-0.7.9/flask_toolkits/swagger/dist/favicon-32x32.png
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      202 2022-08-19 06:08:29.000000 flask-toolkits-0.7.9/flask_toolkits/swagger/dist/index.css
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      734 2022-08-19 06:08:29.000000 flask-toolkits-0.7.9/flask_toolkits/swagger/dist/index.html
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     2690 2022-08-19 06:08:29.000000 flask-toolkits-0.7.9/flask_toolkits/swagger/dist/oauth2-redirect.html
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      539 2022-08-19 06:08:29.000000 flask-toolkits-0.7.9/flask_toolkits/swagger/dist/swagger-initializer.js
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)  1095130 2022-08-19 06:08:29.000000 flask-toolkits-0.7.9/flask_toolkits/swagger/dist/swagger-ui-bundle.js
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)   406408 2022-08-19 06:08:29.000000 flask-toolkits-0.7.9/flask_toolkits/swagger/dist/swagger-ui-es-bundle-core.js
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)  1094892 2022-08-19 06:08:29.000000 flask-toolkits-0.7.9/flask_toolkits/swagger/dist/swagger-ui-es-bundle.js
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)   339540 2022-08-19 06:08:29.000000 flask-toolkits-0.7.9/flask_toolkits/swagger/dist/swagger-ui-standalone-preset.js
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)   143980 2022-08-19 06:08:29.000000 flask-toolkits-0.7.9/flask_toolkits/swagger/dist/swagger-ui.css
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)   286682 2022-08-19 06:08:29.000000 flask-toolkits-0.7.9/flask_toolkits/swagger/dist/swagger-ui.js
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     3034 2022-08-19 06:08:29.000000 flask-toolkits-0.7.9/flask_toolkits/swagger/flask_swagger_ui.py
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)    18800 2023-04-10 11:55:15.000000 flask-toolkits-0.7.9/flask_toolkits/swagger/swagger.py
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     5776 2022-08-19 06:08:29.000000 flask-toolkits-0.7.9/flask_toolkits/swagger/template.py
+drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-04-10 11:55:34.805925 flask-toolkits-0.7.9/flask_toolkits/swagger/templates/
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     2661 2022-08-19 06:08:29.000000 flask-toolkits-0.7.9/flask_toolkits/swagger/templates/index.template.html
+drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-04-10 11:55:34.653921 flask-toolkits-0.7.9/flask_toolkits.egg-info/
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)    10332 2023-04-10 11:55:34.000000 flask-toolkits-0.7.9/flask_toolkits.egg-info/PKG-INFO
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1297 2023-04-10 11:55:34.000000 flask-toolkits-0.7.9/flask_toolkits.egg-info/SOURCES.txt
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)        1 2023-04-10 11:55:34.000000 flask-toolkits-0.7.9/flask_toolkits.egg-info/dependency_links.txt
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       72 2023-04-10 11:55:34.000000 flask-toolkits-0.7.9/flask_toolkits.egg-info/requires.txt
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       15 2023-04-10 11:55:34.000000 flask-toolkits-0.7.9/flask_toolkits.egg-info/top_level.txt
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       38 2023-04-10 11:55:34.805925 flask-toolkits-0.7.9/setup.cfg
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1499 2023-04-10 11:55:29.000000 flask-toolkits-0.7.9/setup.py
```

### Comparing `flask-toolkits-0.7.8/LICENSE` & `flask-toolkits-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-toolkits-0.7.8/PKG-INFO` & `flask-toolkits-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-toolkits
-Version: 0.7.8
+Version: 0.7.9
 Summary: Flask toolkits to boost your development and simplify flask, its featured with AutoSwagger
 Home-page: https://github.com/Danangjoyoo/flask-toolkits
 Author: danangjoyoo (Agus Danangjoyo)
 Author-email: <agus.danangjoyo.blog@gmail.com>
 Keywords: flask,middleware,http,request,response,swagger,openapi,toolkit
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `flask-toolkits-0.7.8/README.md` & `flask-toolkits-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `flask-toolkits-0.7.8/flask_toolkits/fields.py` & `flask-toolkits-0.7.9/flask_toolkits/fields.py`

 * *Files identical despite different names*

### Comparing `flask-toolkits-0.7.8/flask_toolkits/params.py` & `flask-toolkits-0.7.9/flask_toolkits/params.py`

 * *Files identical despite different names*

### Comparing `flask-toolkits-0.7.8/flask_toolkits/responses.py` & `flask-toolkits-0.7.9/flask_toolkits/responses.py`

 * *Files identical despite different names*

### Comparing `flask-toolkits-0.7.8/flask_toolkits/routing.py` & `flask-toolkits-0.7.9/flask_toolkits/routing.py`

 * *Files identical despite different names*

### Comparing `flask-toolkits-0.7.8/flask_toolkits/schemas.py` & `flask-toolkits-0.7.9/flask_toolkits/schemas.py`

 * *Files identical despite different names*

### Comparing `flask-toolkits-0.7.8/flask_toolkits/security.py` & `flask-toolkits-0.7.9/flask_toolkits/security.py`

 * *Files identical despite different names*

### Comparing `flask-toolkits-0.7.8/flask_toolkits/status.py` & `flask-toolkits-0.7.9/flask_toolkits/status.py`

 * *Files identical despite different names*

### Comparing `flask-toolkits-0.7.8/flask_toolkits/swagger/__init__.py` & `flask-toolkits-0.7.9/flask_toolkits/swagger/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-toolkits-0.7.8/flask_toolkits/swagger/dist/favicon-16x16.png` & `flask-toolkits-0.7.9/flask_toolkits/swagger/dist/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `flask-toolkits-0.7.8/flask_toolkits/swagger/dist/favicon-32x32.png` & `flask-toolkits-0.7.9/flask_toolkits/swagger/dist/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `flask-toolkits-0.7.8/flask_toolkits/swagger/dist/index.html` & `flask-toolkits-0.7.9/flask_toolkits/swagger/dist/index.html`

 * *Files identical despite different names*

### Comparing `flask-toolkits-0.7.8/flask_toolkits/swagger/dist/oauth2-redirect.html` & `flask-toolkits-0.7.9/flask_toolkits/swagger/dist/oauth2-redirect.html`

 * *Files identical despite different names*

### Comparing `flask-toolkits-0.7.8/flask_toolkits/swagger/dist/swagger-initializer.js` & `flask-toolkits-0.7.9/flask_toolkits/swagger/dist/swagger-initializer.js`

 * *Files identical despite different names*

### Comparing `flask-toolkits-0.7.8/flask_toolkits/swagger/dist/swagger-ui-bundle.js` & `flask-toolkits-0.7.9/flask_toolkits/swagger/dist/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-toolkits-0.7.8/flask_toolkits/swagger/dist/swagger-ui-es-bundle-core.js` & `flask-toolkits-0.7.9/flask_toolkits/swagger/dist/swagger-ui-es-bundle-core.js`

 * *Files identical despite different names*

### Comparing `flask-toolkits-0.7.8/flask_toolkits/swagger/dist/swagger-ui-es-bundle.js` & `flask-toolkits-0.7.9/flask_toolkits/swagger/dist/swagger-ui-es-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-toolkits-0.7.8/flask_toolkits/swagger/dist/swagger-ui-standalone-preset.js` & `flask-toolkits-0.7.9/flask_toolkits/swagger/dist/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flask-toolkits-0.7.8/flask_toolkits/swagger/dist/swagger-ui.css` & `flask-toolkits-0.7.9/flask_toolkits/swagger/dist/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flask-toolkits-0.7.8/flask_toolkits/swagger/dist/swagger-ui.js` & `flask-toolkits-0.7.9/flask_toolkits/swagger/dist/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `flask-toolkits-0.7.8/flask_toolkits/swagger/flask_swagger_ui.py` & `flask-toolkits-0.7.9/flask_toolkits/swagger/flask_swagger_ui.py`

 * *Files identical despite different names*

### Comparing `flask-toolkits-0.7.8/flask_toolkits/swagger/swagger.py` & `flask-toolkits-0.7.9/flask_toolkits/swagger/swagger.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
 
     def generate_parameter_schema(self, paired_params: Dict[str, ParamSignature]):
         schemas = []
         definitions = {}
         for k, p in paired_params.items():
             po = p.param_object
             k = p.param_object.alias or k
-            if type(po) in [Header, Path, Query]:
+            if type(po) in [Form, Header, Path, Query]:
                 sub_schema = self.generate_parameter_sub_schema(k, po)
                 schema = {
                     "name": k,
                     "in": po._type.value
                 }
                 if po.default == ... or isinstance(po, Path):
                     schema["required"] = True
```

### Comparing `flask-toolkits-0.7.8/flask_toolkits/swagger/template.py` & `flask-toolkits-0.7.9/flask_toolkits/swagger/template.py`

 * *Files identical despite different names*

### Comparing `flask-toolkits-0.7.8/flask_toolkits/swagger/templates/index.template.html` & `flask-toolkits-0.7.9/flask_toolkits/swagger/templates/index.template.html`

 * *Files identical despite different names*

### Comparing `flask-toolkits-0.7.8/flask_toolkits.egg-info/PKG-INFO` & `flask-toolkits-0.7.9/flask_toolkits.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-toolkits
-Version: 0.7.8
+Version: 0.7.9
 Summary: Flask toolkits to boost your development and simplify flask, its featured with AutoSwagger
 Home-page: https://github.com/Danangjoyoo/flask-toolkits
 Author: danangjoyoo (Agus Danangjoyo)
 Author-email: <agus.danangjoyo.blog@gmail.com>
 Keywords: flask,middleware,http,request,response,swagger,openapi,toolkit
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `flask-toolkits-0.7.8/flask_toolkits.egg-info/SOURCES.txt` & `flask-toolkits-0.7.9/flask_toolkits.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask-toolkits-0.7.8/setup.py` & `flask-toolkits-0.7.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = "0.7.8"
+VERSION = "0.7.9"
 DESCRIPTION = "Flask toolkits to boost your development and simplify flask, its featured with AutoSwagger"
 
 # Setting up
 setup(
     name="flask-toolkits",
     version=VERSION,
     author="danangjoyoo (Agus Danangjoyo)",
```

