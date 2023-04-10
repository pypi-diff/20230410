# Comparing `tmp/django-multitenant-3.2.0.tar.gz` & `tmp/django-multitenant-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-multitenant-3.2.0.tar", last modified: Wed Mar 29 12:04:40 2023, max compression
+gzip compressed data, was "django-multitenant-3.2.1.tar", last modified: Sun Apr  2 16:07:24 2023, max compression
```

## Comparing `django-multitenant-3.2.0.tar` & `django-multitenant-3.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 gurkanindibay  (1000) gurkanindibay  (1000)        0 2023-03-29 12:04:40.230000 django-multitenant-3.2.0/
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)     1059 2023-01-18 10:57:53.000000 django-multitenant-3.2.0/LICENSE
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)     9786 2023-03-29 12:04:40.230000 django-multitenant-3.2.0/PKG-INFO
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)     8870 2023-03-01 00:55:27.000000 django-multitenant-3.2.0/README.md
-drwxr-xr-x   0 gurkanindibay  (1000) gurkanindibay  (1000)        0 2023-03-29 12:04:40.220000 django-multitenant-3.2.0/django_multitenant/
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)      394 2023-01-18 10:57:53.000000 django-multitenant-3.2.0/django_multitenant/__init__.py
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)      161 2023-03-23 07:52:16.000000 django-multitenant-3.2.0/django_multitenant/apps.py
-drwxr-xr-x   0 gurkanindibay  (1000) gurkanindibay  (1000)        0 2023-03-29 12:04:40.230000 django-multitenant-3.2.0/django_multitenant/backends/
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)        0 2023-01-18 10:57:53.000000 django-multitenant-3.2.0/django_multitenant/backends/__init__.py
-drwxr-xr-x   0 gurkanindibay  (1000) gurkanindibay  (1000)        0 2023-03-29 12:04:40.230000 django-multitenant-3.2.0/django_multitenant/backends/postgresql/
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)        0 2023-01-18 10:57:53.000000 django-multitenant-3.2.0/django_multitenant/backends/postgresql/__init__.py
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)     5530 2023-03-13 10:02:42.000000 django-multitenant-3.2.0/django_multitenant/backends/postgresql/base.py
-drwxr-xr-x   0 gurkanindibay  (1000) gurkanindibay  (1000)        0 2023-03-29 12:04:40.230000 django-multitenant-3.2.0/django_multitenant/db/
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)        0 2023-01-18 10:57:53.000000 django-multitenant-3.2.0/django_multitenant/db/__init__.py
-drwxr-xr-x   0 gurkanindibay  (1000) gurkanindibay  (1000)        0 2023-03-29 12:04:40.230000 django-multitenant-3.2.0/django_multitenant/db/migrations/
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)       26 2023-01-18 10:57:53.000000 django-multitenant-3.2.0/django_multitenant/db/migrations/__init__.py
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)     3177 2023-01-20 04:55:41.000000 django-multitenant-3.2.0/django_multitenant/db/migrations/distribute.py
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)     1332 2023-01-20 04:55:41.000000 django-multitenant-3.2.0/django_multitenant/deletion.py
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)      279 2023-03-29 11:46:20.000000 django-multitenant-3.2.0/django_multitenant/django_mt_environment.py
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)        0 2023-01-20 04:55:41.000000 django-multitenant-3.2.0/django_multitenant/django_multitenant.py
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)       39 2023-01-18 10:57:53.000000 django-multitenant-3.2.0/django_multitenant/exceptions.py
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)     4159 2023-01-20 04:55:41.000000 django-multitenant-3.2.0/django_multitenant/fields.py
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)      430 2023-03-29 11:46:20.000000 django-multitenant-3.2.0/django_multitenant/middlewares.py
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)     8976 2023-03-29 11:46:20.000000 django-multitenant-3.2.0/django_multitenant/mixins.py
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)      509 2023-03-29 11:46:20.000000 django-multitenant-3.2.0/django_multitenant/models.py
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)     3152 2023-02-23 17:14:43.000000 django-multitenant-3.2.0/django_multitenant/query.py
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)      361 2023-01-18 10:57:53.000000 django-multitenant-3.2.0/django_multitenant/settings.py
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)     4158 2023-03-01 00:55:27.000000 django-multitenant-3.2.0/django_multitenant/utils.py
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)      669 2023-03-29 11:46:20.000000 django-multitenant-3.2.0/django_multitenant/views.py
-drwxr-xr-x   0 gurkanindibay  (1000) gurkanindibay  (1000)        0 2023-03-29 12:04:40.230000 django-multitenant-3.2.0/django_multitenant.egg-info/
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)     9786 2023-03-29 12:04:40.000000 django-multitenant-3.2.0/django_multitenant.egg-info/PKG-INFO
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)      901 2023-03-29 12:04:40.000000 django-multitenant-3.2.0/django_multitenant.egg-info/SOURCES.txt
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)        1 2023-03-29 12:04:40.000000 django-multitenant-3.2.0/django_multitenant.egg-info/dependency_links.txt
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)       19 2023-03-29 12:04:40.000000 django-multitenant-3.2.0/django_multitenant.egg-info/top_level.txt
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)       38 2023-03-29 12:04:40.230000 django-multitenant-3.2.0/setup.cfg
--rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)     1660 2023-03-29 12:01:05.000000 django-multitenant-3.2.0/setup.py
+drwxr-xr-x   0 gurkanindibay  (1000) gurkanindibay  (1000)        0 2023-04-02 16:07:24.136919 django-multitenant-3.2.1/
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)     1059 2023-01-18 10:57:53.000000 django-multitenant-3.2.1/LICENSE
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)     9787 2023-04-02 16:07:24.136919 django-multitenant-3.2.1/PKG-INFO
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)     8871 2023-04-02 15:58:21.000000 django-multitenant-3.2.1/README.md
+drwxr-xr-x   0 gurkanindibay  (1000) gurkanindibay  (1000)        0 2023-04-02 16:07:24.126919 django-multitenant-3.2.1/django_multitenant/
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)      394 2023-01-18 10:57:53.000000 django-multitenant-3.2.1/django_multitenant/__init__.py
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)      161 2023-03-23 07:52:16.000000 django-multitenant-3.2.1/django_multitenant/apps.py
+drwxr-xr-x   0 gurkanindibay  (1000) gurkanindibay  (1000)        0 2023-04-02 16:07:24.126919 django-multitenant-3.2.1/django_multitenant/backends/
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)        0 2023-01-18 10:57:53.000000 django-multitenant-3.2.1/django_multitenant/backends/__init__.py
+drwxr-xr-x   0 gurkanindibay  (1000) gurkanindibay  (1000)        0 2023-04-02 16:07:24.126919 django-multitenant-3.2.1/django_multitenant/backends/postgresql/
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)        0 2023-01-18 10:57:53.000000 django-multitenant-3.2.1/django_multitenant/backends/postgresql/__init__.py
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)     5530 2023-03-13 10:02:42.000000 django-multitenant-3.2.1/django_multitenant/backends/postgresql/base.py
+drwxr-xr-x   0 gurkanindibay  (1000) gurkanindibay  (1000)        0 2023-04-02 16:07:24.136919 django-multitenant-3.2.1/django_multitenant/db/
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)        0 2023-01-18 10:57:53.000000 django-multitenant-3.2.1/django_multitenant/db/__init__.py
+drwxr-xr-x   0 gurkanindibay  (1000) gurkanindibay  (1000)        0 2023-04-02 16:07:24.136919 django-multitenant-3.2.1/django_multitenant/db/migrations/
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)       26 2023-01-18 10:57:53.000000 django-multitenant-3.2.1/django_multitenant/db/migrations/__init__.py
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)     3177 2023-01-20 04:55:41.000000 django-multitenant-3.2.1/django_multitenant/db/migrations/distribute.py
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)     1332 2023-01-20 04:55:41.000000 django-multitenant-3.2.1/django_multitenant/deletion.py
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)      279 2023-03-29 11:46:20.000000 django-multitenant-3.2.1/django_multitenant/django_mt_environment.py
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)        0 2023-01-20 04:55:41.000000 django-multitenant-3.2.1/django_multitenant/django_multitenant.py
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)       39 2023-01-18 10:57:53.000000 django-multitenant-3.2.1/django_multitenant/exceptions.py
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)     4159 2023-01-20 04:55:41.000000 django-multitenant-3.2.1/django_multitenant/fields.py
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)      430 2023-03-29 11:46:20.000000 django-multitenant-3.2.1/django_multitenant/middlewares.py
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)     9030 2023-04-02 15:58:21.000000 django-multitenant-3.2.1/django_multitenant/mixins.py
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)      509 2023-03-29 11:46:20.000000 django-multitenant-3.2.1/django_multitenant/models.py
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)     3152 2023-02-23 17:14:43.000000 django-multitenant-3.2.1/django_multitenant/query.py
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)      361 2023-01-18 10:57:53.000000 django-multitenant-3.2.1/django_multitenant/settings.py
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)     4158 2023-03-01 00:55:27.000000 django-multitenant-3.2.1/django_multitenant/utils.py
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)      669 2023-03-29 11:46:20.000000 django-multitenant-3.2.1/django_multitenant/views.py
+drwxr-xr-x   0 gurkanindibay  (1000) gurkanindibay  (1000)        0 2023-04-02 16:07:24.126919 django-multitenant-3.2.1/django_multitenant.egg-info/
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)     9787 2023-04-02 16:07:24.000000 django-multitenant-3.2.1/django_multitenant.egg-info/PKG-INFO
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)      901 2023-04-02 16:07:24.000000 django-multitenant-3.2.1/django_multitenant.egg-info/SOURCES.txt
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)        1 2023-04-02 16:07:24.000000 django-multitenant-3.2.1/django_multitenant.egg-info/dependency_links.txt
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)       19 2023-04-02 16:07:24.000000 django-multitenant-3.2.1/django_multitenant.egg-info/top_level.txt
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)       38 2023-04-02 16:07:24.136919 django-multitenant-3.2.1/setup.cfg
+-rw-r--r--   0 gurkanindibay  (1000) gurkanindibay  (1000)     1660 2023-04-02 15:59:05.000000 django-multitenant-3.2.1/setup.py
```

### Comparing `django-multitenant-3.2.0/LICENSE` & `django-multitenant-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-multitenant-3.2.0/PKG-INFO` & `django-multitenant-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-multitenant
-Version: 3.2.0
+Version: 3.2.1
 Summary: Django Library to Implement Multi-tenant databases
 Home-page: https://github.com/citusdata/django-multitenant
 Author: Louise Grandjonc
 Author-email: louise.grandjonc@microsoft.com
 Keywords: citus django multi tenantdjango postgres multi-tenant
 Classifier: Development Status :: 5 - Production/Stable 
 Classifier: Topic :: Database
@@ -40,17 +40,18 @@
 ## Installation:
 1. `pip install  --no-cache-dir django_multitenant`
 
 ## Supported Django versions/Pre-requisites.
 
 | Python                | Django        |Citus          |
 | ----------------------| --------------|---------------|
-| 3.7                   | 3.2           | 10  11        |
-| 3.8 3.9 3.10 3.11     | 4.0           | 10  11        |
 | 3.8 3.9 3.10 3.11     | 4.1           | 11            |
+| 3.8 3.9 3.10 3.11     | 4.0           | 10  11        |
+| 3.7                   | 3.2           | 10  11        |
+
 
 
 
 ## Usage:
 
 In order to use this library you can either use Mixins or have your models inherit from our custom model class.
 
@@ -231,9 +232,9 @@
 
 ## Credits
 
 This library uses similar logic of setting/getting tenant object as in [django-simple-multitenant](https://github.com/pombredanne/django-simple-multitenant). We thank the authors for their efforts.
 
 ## License
 
-Copyright (C) 2018, Citus Data
+Copyright (C) 2023, Citus Data
 Licensed under the MIT license, see LICENSE file for details.
```

### Comparing `django-multitenant-3.2.0/README.md` & `django-multitenant-3.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 ## Installation:
 1. `pip install  --no-cache-dir django_multitenant`
 
 ## Supported Django versions/Pre-requisites.
 
 | Python                | Django        |Citus          |
 | ----------------------| --------------|---------------|
-| 3.7                   | 3.2           | 10  11        |
-| 3.8 3.9 3.10 3.11     | 4.0           | 10  11        |
 | 3.8 3.9 3.10 3.11     | 4.1           | 11            |
+| 3.8 3.9 3.10 3.11     | 4.0           | 10  11        |
+| 3.7                   | 3.2           | 10  11        |
+
 
 
 
 ## Usage:
 
 In order to use this library you can either use Mixins or have your models inherit from our custom model class.
 
@@ -209,9 +210,9 @@
 
 ## Credits
 
 This library uses similar logic of setting/getting tenant object as in [django-simple-multitenant](https://github.com/pombredanne/django-simple-multitenant). We thank the authors for their efforts.
 
 ## License
 
-Copyright (C) 2018, Citus Data
+Copyright (C) 2023, Citus Data
 Licensed under the MIT license, see LICENSE file for details.
```

### Comparing `django-multitenant-3.2.0/django_multitenant/backends/postgresql/base.py` & `django-multitenant-3.2.1/django_multitenant/backends/postgresql/base.py`

 * *Files identical despite different names*

### Comparing `django-multitenant-3.2.0/django_multitenant/db/migrations/distribute.py` & `django-multitenant-3.2.1/django_multitenant/db/migrations/distribute.py`

 * *Files identical despite different names*

### Comparing `django-multitenant-3.2.0/django_multitenant/deletion.py` & `django-multitenant-3.2.1/django_multitenant/deletion.py`

 * *Files identical despite different names*

### Comparing `django-multitenant-3.2.0/django_multitenant/fields.py` & `django-multitenant-3.2.1/django_multitenant/fields.py`

 * *Files identical despite different names*

### Comparing `django-multitenant-3.2.0/django_multitenant/mixins.py` & `django-multitenant-3.2.1/django_multitenant/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     Wraps the add method of many to many field to set tenant_id in through_defaults
     parameter of the add method.
     """
 
     def add(self, *objs, through_defaults=None):
 
         if hasattr(self.through, "tenant_field") and get_current_tenant():
+            through_defaults = through_defaults or {}
             through_defaults[
                 get_tenant_column(self.through)
             ] = get_current_tenant_value()
         return many_related_manager_add(self, *objs, through_defaults=through_defaults)
 
     return add
```

### Comparing `django-multitenant-3.2.0/django_multitenant/query.py` & `django-multitenant-3.2.1/django_multitenant/query.py`

 * *Files identical despite different names*

### Comparing `django-multitenant-3.2.0/django_multitenant/utils.py` & `django-multitenant-3.2.1/django_multitenant/utils.py`

 * *Files identical despite different names*

### Comparing `django-multitenant-3.2.0/django_multitenant/views.py` & `django-multitenant-3.2.1/django_multitenant/views.py`

 * *Files identical despite different names*

### Comparing `django-multitenant-3.2.0/django_multitenant.egg-info/PKG-INFO` & `django-multitenant-3.2.1/django_multitenant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-multitenant
-Version: 3.2.0
+Version: 3.2.1
 Summary: Django Library to Implement Multi-tenant databases
 Home-page: https://github.com/citusdata/django-multitenant
 Author: Louise Grandjonc
 Author-email: louise.grandjonc@microsoft.com
 Keywords: citus django multi tenantdjango postgres multi-tenant
 Classifier: Development Status :: 5 - Production/Stable 
 Classifier: Topic :: Database
@@ -40,17 +40,18 @@
 ## Installation:
 1. `pip install  --no-cache-dir django_multitenant`
 
 ## Supported Django versions/Pre-requisites.
 
 | Python                | Django        |Citus          |
 | ----------------------| --------------|---------------|
-| 3.7                   | 3.2           | 10  11        |
-| 3.8 3.9 3.10 3.11     | 4.0           | 10  11        |
 | 3.8 3.9 3.10 3.11     | 4.1           | 11            |
+| 3.8 3.9 3.10 3.11     | 4.0           | 10  11        |
+| 3.7                   | 3.2           | 10  11        |
+
 
 
 
 ## Usage:
 
 In order to use this library you can either use Mixins or have your models inherit from our custom model class.
 
@@ -231,9 +232,9 @@
 
 ## Credits
 
 This library uses similar logic of setting/getting tenant object as in [django-simple-multitenant](https://github.com/pombredanne/django-simple-multitenant). We thank the authors for their efforts.
 
 ## License
 
-Copyright (C) 2018, Citus Data
+Copyright (C) 2023, Citus Data
 Licensed under the MIT license, see LICENSE file for details.
```

### Comparing `django-multitenant-3.2.0/django_multitenant.egg-info/SOURCES.txt` & `django-multitenant-3.2.1/django_multitenant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-multitenant-3.2.0/setup.py` & `django-multitenant-3.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name="django-multitenant",
-    version="3.2.0",  # Required
+    version="3.2.1",  # Required
     description="Django Library to Implement Multi-tenant databases",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/citusdata/django-multitenant",
     author="Louise Grandjonc",
     author_email="louise.grandjonc@microsoft.com",
     # Classifiers help users find your project by categorizing it.
```

