# Comparing `tmp/novadata_utils-0.2.tar.gz` & `tmp/novadata_utils-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novadata_utils-0.2.tar", last modified: Tue Apr  4 13:09:41 2023, max compression
+gzip compressed data, was "novadata_utils-0.2.1.tar", last modified: Mon Apr 10 15:01:26 2023, max compression
```

## Comparing `novadata_utils-0.2.tar` & `novadata_utils-0.2.1.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-04 13:09:41.861808 novadata_utils-0.2/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1066 2023-04-04 12:57:52.000000 novadata_utils-0.2/LICENSE
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1045 2023-04-04 13:09:41.861808 novadata_utils-0.2/PKG-INFO
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      602 2023-04-04 12:57:52.000000 novadata_utils-0.2/README.md
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-04 13:09:41.857809 novadata_utils-0.2/novadata_utils/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       60 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-04 13:09:41.857809 novadata_utils-0.2/novadata_utils/admin/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       92 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/admin/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     2829 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/admin/novadata_model_admin.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      219 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/apps.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-04 13:09:41.857809 novadata_utils-0.2/novadata_utils/auth/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       92 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/auth/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      729 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/auth/login_username_email.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-04 13:09:41.857809 novadata_utils-0.2/novadata_utils/forms/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/forms/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-04 13:09:41.857809 novadata_utils-0.2/novadata_utils/functions/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       60 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/functions/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     2150 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/functions/get_prop.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-04 13:09:41.857809 novadata_utils-0.2/novadata_utils/managers/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/managers/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-04 13:09:41.857809 novadata_utils-0.2/novadata_utils/middlewares/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/middlewares/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-04 13:09:41.857809 novadata_utils-0.2/novadata_utils/migrations/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1232 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/migrations/0001_initial.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)        0 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/migrations/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-04 13:09:41.857809 novadata_utils-0.2/novadata_utils/models/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       76 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/models/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1188 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/models/novadata_model.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-04 13:09:41.861808 novadata_utils-0.2/novadata_utils/redirect/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       87 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/redirect/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1130 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/redirect/reverse_lazy_plus.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-04 13:09:41.861808 novadata_utils-0.2/novadata_utils/save/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      130 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/save/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1749 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/save/create_logs.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     2152 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/save/get_changes.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-04 13:09:41.861808 novadata_utils-0.2/novadata_utils/serializers/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      107 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/serializers/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      880 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/serializers/novadata_model_serializer.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-04 13:09:41.861808 novadata_utils-0.2/novadata_utils/signals/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/signals/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-04 13:09:41.861808 novadata_utils-0.2/novadata_utils/templatetags/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)        0 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/templatetags/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-04 13:09:41.861808 novadata_utils-0.2/novadata_utils/tests/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)        0 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/tests/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       58 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/urls.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-04 13:09:41.861808 novadata_utils-0.2/novadata_utils/views/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/views/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-04 13:09:41.861808 novadata_utils-0.2/novadata_utils/viewsets/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       98 2023-04-04 12:57:52.000000 novadata_utils-0.2/novadata_utils/viewsets/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     4830 2023-04-04 13:09:11.000000 novadata_utils-0.2/novadata_utils/viewsets/novadata_model_viewset.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-04 13:09:41.857809 novadata_utils-0.2/novadata_utils.egg-info/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1045 2023-04-04 13:09:41.000000 novadata_utils-0.2/novadata_utils.egg-info/PKG-INFO
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1283 2023-04-04 13:09:41.000000 novadata_utils-0.2/novadata_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 flavio    (1000) flavio    (1000)        1 2023-04-04 13:09:41.000000 novadata_utils-0.2/novadata_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       70 2023-04-04 13:09:41.000000 novadata_utils-0.2/novadata_utils.egg-info/requires.txt
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       15 2023-04-04 13:09:41.000000 novadata_utils-0.2/novadata_utils.egg-info/top_level.txt
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       38 2023-04-04 13:09:41.861808 novadata_utils-0.2/setup.cfg
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      801 2023-04-04 13:09:40.000000 novadata_utils-0.2/setup.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:01:26.483634 novadata_utils-0.2.1/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1066 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/LICENSE
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1088 2023-04-10 15:01:26.483634 novadata_utils-0.2.1/PKG-INFO
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      643 2023-04-10 13:10:00.000000 novadata_utils-0.2.1/README.md
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:01:26.479634 novadata_utils-0.2.1/novadata_utils/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       60 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/novadata_utils/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:01:26.479634 novadata_utils-0.2.1/novadata_utils/admin/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       92 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/novadata_utils/admin/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     4353 2023-04-10 14:26:47.000000 novadata_utils-0.2.1/novadata_utils/admin/novadata_model_admin.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      219 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/novadata_utils/apps.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:01:26.479634 novadata_utils-0.2.1/novadata_utils/auth/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       92 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/novadata_utils/auth/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      729 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/novadata_utils/auth/login_username_email.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:01:26.479634 novadata_utils-0.2.1/novadata_utils/forms/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/novadata_utils/forms/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:01:26.479634 novadata_utils-0.2.1/novadata_utils/functions/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      126 2023-04-10 14:20:05.000000 novadata_utils-0.2.1/novadata_utils/functions/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     3573 2023-04-10 14:19:03.000000 novadata_utils-0.2.1/novadata_utils/functions/get_prop.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      416 2023-04-10 14:19:49.000000 novadata_utils-0.2.1/novadata_utils/functions/transform_field.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:01:26.479634 novadata_utils-0.2.1/novadata_utils/managers/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/novadata_utils/managers/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:01:26.479634 novadata_utils-0.2.1/novadata_utils/middlewares/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/novadata_utils/middlewares/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:01:26.479634 novadata_utils-0.2.1/novadata_utils/migrations/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1232 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/novadata_utils/migrations/0001_initial.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)        0 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/novadata_utils/migrations/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:01:26.479634 novadata_utils-0.2.1/novadata_utils/models/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       76 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/novadata_utils/models/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1188 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/novadata_utils/models/novadata_model.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:01:26.479634 novadata_utils-0.2.1/novadata_utils/redirect/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       87 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/novadata_utils/redirect/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1130 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/novadata_utils/redirect/reverse_lazy_plus.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:01:26.483634 novadata_utils-0.2.1/novadata_utils/save/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      130 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/novadata_utils/save/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1749 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/novadata_utils/save/create_logs.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     2152 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/novadata_utils/save/get_changes.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:01:26.483634 novadata_utils-0.2.1/novadata_utils/serializers/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      107 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/novadata_utils/serializers/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      880 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/novadata_utils/serializers/novadata_model_serializer.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:01:26.483634 novadata_utils-0.2.1/novadata_utils/signals/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/novadata_utils/signals/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:01:26.483634 novadata_utils-0.2.1/novadata_utils/templatetags/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)        0 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/novadata_utils/templatetags/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:01:26.483634 novadata_utils-0.2.1/novadata_utils/tests/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)        0 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/novadata_utils/tests/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       58 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/novadata_utils/urls.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:01:26.483634 novadata_utils-0.2.1/novadata_utils/views/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/novadata_utils/views/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:01:26.483634 novadata_utils-0.2.1/novadata_utils/viewsets/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       98 2023-04-04 12:57:52.000000 novadata_utils-0.2.1/novadata_utils/viewsets/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     4830 2023-04-04 13:09:11.000000 novadata_utils-0.2.1/novadata_utils/viewsets/novadata_model_viewset.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:01:26.479634 novadata_utils-0.2.1/novadata_utils.egg-info/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1088 2023-04-10 15:01:26.000000 novadata_utils-0.2.1/novadata_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1327 2023-04-10 15:01:26.000000 novadata_utils-0.2.1/novadata_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)        1 2023-04-10 15:01:26.000000 novadata_utils-0.2.1/novadata_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      111 2023-04-10 15:01:26.000000 novadata_utils-0.2.1/novadata_utils.egg-info/requires.txt
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       15 2023-04-10 15:01:26.000000 novadata_utils-0.2.1/novadata_utils.egg-info/top_level.txt
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       38 2023-04-10 15:01:26.483634 novadata_utils-0.2.1/setup.cfg
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      855 2023-04-10 14:47:35.000000 novadata_utils-0.2.1/setup.py
```

### Comparing `novadata_utils-0.2/LICENSE` & `novadata_utils-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2/PKG-INFO` & `novadata_utils-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: novadata_utils
-Version: 0.2
+Version: 0.2.1
 Summary: novadata utils
 Home-page: https://github.com/TimeNovaData/novadata_utils/
 Author: Flávio Silva
 Author-email: flavio.nogueira.profissional@gmail.com
 License: MIT License
 Project-URL: GitHub, https://github.com/TimeNovaData/novadata_utils/
 Keywords: Django,utils,ndt,novadata,nova data,nova,data
@@ -26,14 +26,15 @@
 pip install novadata-utils
 ```
 
 Settings.py:
 ```python
 INSTALLED_APPS = [
     ...
+    'django-admin-list-filter-dropdown',
     'django_object_actions',
     'import_export',
     'novadata_utils',
     'rest_framework',
     ...
 ]
 ```
```

### Comparing `novadata_utils-0.2/README.md` & `novadata_utils-0.2.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 pip install novadata-utils
 ```
 
 Settings.py:
 ```python
 INSTALLED_APPS = [
     ...
+    'django-admin-list-filter-dropdown',
     'django_object_actions',
     'import_export',
     'novadata_utils',
     'rest_framework',
     ...
 ]
 ```
```

### Comparing `novadata_utils-0.2/novadata_utils/auth/login_username_email.py` & `novadata_utils-0.2.1/novadata_utils/auth/login_username_email.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2/novadata_utils/migrations/0001_initial.py` & `novadata_utils-0.2.1/novadata_utils/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2/novadata_utils/models/novadata_model.py` & `novadata_utils-0.2.1/novadata_utils/models/novadata_model.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2/novadata_utils/redirect/reverse_lazy_plus.py` & `novadata_utils-0.2.1/novadata_utils/redirect/reverse_lazy_plus.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2/novadata_utils/save/create_logs.py` & `novadata_utils-0.2.1/novadata_utils/save/create_logs.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2/novadata_utils/save/get_changes.py` & `novadata_utils-0.2.1/novadata_utils/save/get_changes.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2/novadata_utils/serializers/novadata_model_serializer.py` & `novadata_utils-0.2.1/novadata_utils/serializers/novadata_model_serializer.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2/novadata_utils/viewsets/novadata_model_viewset.py` & `novadata_utils-0.2.1/novadata_utils/viewsets/novadata_model_viewset.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2/novadata_utils.egg-info/PKG-INFO` & `novadata_utils-0.2.1/novadata_utils.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: novadata-utils
-Version: 0.2
+Version: 0.2.1
 Summary: novadata utils
 Home-page: https://github.com/TimeNovaData/novadata_utils/
 Author: Flávio Silva
 Author-email: flavio.nogueira.profissional@gmail.com
 License: MIT License
 Project-URL: GitHub, https://github.com/TimeNovaData/novadata_utils/
 Keywords: Django,utils,ndt,novadata,nova data,nova,data
@@ -26,14 +26,15 @@
 pip install novadata-utils
 ```
 
 Settings.py:
 ```python
 INSTALLED_APPS = [
     ...
+    'django-admin-list-filter-dropdown',
     'django_object_actions',
     'import_export',
     'novadata_utils',
     'rest_framework',
     ...
 ]
 ```
```

### Comparing `novadata_utils-0.2/novadata_utils.egg-info/SOURCES.txt` & `novadata_utils-0.2.1/novadata_utils.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 novadata_utils/admin/__init__.py
 novadata_utils/admin/novadata_model_admin.py
 novadata_utils/auth/__init__.py
 novadata_utils/auth/login_username_email.py
 novadata_utils/forms/__init__.py
 novadata_utils/functions/__init__.py
 novadata_utils/functions/get_prop.py
+novadata_utils/functions/transform_field.py
 novadata_utils/managers/__init__.py
 novadata_utils/middlewares/__init__.py
 novadata_utils/migrations/0001_initial.py
 novadata_utils/migrations/__init__.py
 novadata_utils/models/__init__.py
 novadata_utils/models/novadata_model.py
 novadata_utils/redirect/__init__.py
```

### Comparing `novadata_utils-0.2/setup.py` & `novadata_utils-0.2.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     readme = fh.read()
 
 setup(
     name="novadata_utils",
-    version="0.2",
+    version="0.2.1",
     url="https://github.com/TimeNovaData/novadata_utils/",
     license="MIT License",
     author="Flávio Silva",
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email="flavio.nogueira.profissional@gmail.com",
     keywords="Django, utils, ndt, novadata, nova data, nova, data",
     description="novadata utils",
     packages=find_packages(),
     install_requires=[
         "django",
         "djangorestframework",
-        "django-object-actions",
+        "django-admin-list-filter-dropdown",
         "django-import-export",
+        "django-object-actions>=4.0.0",
     ],
     project_urls={
         "GitHub": "https://github.com/TimeNovaData/novadata_utils/",
     },
 )
```

