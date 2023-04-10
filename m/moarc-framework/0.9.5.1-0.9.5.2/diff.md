# Comparing `tmp/moarc-framework-0.9.5.1.tar.gz` & `tmp/moarc-framework-0.9.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\moarc-framework-0.9.5.1.tar", last modified: Mon Apr 10 03:15:40 2023, max compression
+gzip compressed data, was "dist\moarc-framework-0.9.5.2.tar", last modified: Mon Apr 10 03:17:06 2023, max compression
```

## Comparing `moarc-framework-0.9.5.1.tar` & `moarc-framework-0.9.5.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 03:15:40.253497 moarc-framework-0.9.5.1/
--rw-rw-rw-   0        0        0     1596 2022-02-20 16:21:00.000000 moarc-framework-0.9.5.1/LICENSE
--rw-rw-rw-   0        0        0      142 2022-09-13 03:58:24.000000 moarc-framework-0.9.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1756 2023-04-10 03:15:40.254439 moarc-framework-0.9.5.1/PKG-INFO
--rw-rw-rw-   0        0        0      609 2022-02-20 16:18:57.000000 moarc-framework-0.9.5.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-10 03:15:40.227569 moarc-framework-0.9.5.1/moarc_framework.egg-info/
--rw-rw-rw-   0        0        0     1756 2023-04-10 03:15:40.000000 moarc-framework-0.9.5.1/moarc_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1352 2023-04-10 03:15:40.000000 moarc-framework-0.9.5.1/moarc_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 03:15:40.000000 moarc-framework-0.9.5.1/moarc_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-10 03:15:40.000000 moarc-framework-0.9.5.1/moarc_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-10 03:15:40.000000 moarc-framework-0.9.5.1/moarc_framework.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 03:15:40.230566 moarc-framework-0.9.5.1/moarcframework/
--rw-rw-rw-   0        0        0       25 2022-02-20 16:14:26.000000 moarc-framework-0.9.5.1/moarcframework/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 03:15:40.232567 moarc-framework-0.9.5.1/moarcframework/helpers/
--rw-rw-rw-   0        0        0       25 2022-02-20 03:31:52.000000 moarc-framework-0.9.5.1/moarcframework/helpers/__init__.py
--rw-rw-rw-   0        0        0      200 2022-05-11 22:13:28.000000 moarc-framework-0.9.5.1/moarcframework/helpers/auth.py
--rw-rw-rw-   0        0        0     2314 2022-05-21 15:36:43.000000 moarc-framework-0.9.5.1/moarcframework/helpers/paginator.py
-drwxrwxrwx   0        0        0        0 2023-04-10 03:15:40.236603 moarc-framework-0.9.5.1/moarcframework/http/
--rw-rw-rw-   0        0        0       25 2022-02-20 01:02:24.000000 moarc-framework-0.9.5.1/moarcframework/http/__init__.py
--rw-rw-rw-   0        0        0      764 2022-05-18 22:46:28.000000 moarc-framework-0.9.5.1/moarcframework/http/decorators.py
--rw-rw-rw-   0        0        0      191 2022-02-20 15:42:53.000000 moarc-framework-0.9.5.1/moarcframework/http/generic_serializer.py
--rw-rw-rw-   0        0        0     1089 2022-05-25 03:31:33.000000 moarc-framework-0.9.5.1/moarcframework/http/http.py
-drwxrwxrwx   0        0        0        0 2023-04-10 03:15:40.237567 moarc-framework-0.9.5.1/moarcframework/management/
--rw-rw-rw-   0        0        0        0 2020-08-29 16:49:19.000000 moarc-framework-0.9.5.1/moarcframework/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 03:15:40.239566 moarc-framework-0.9.5.1/moarcframework/management/commands/
--rw-rw-rw-   0        0        0        0 2020-08-29 16:49:19.000000 moarc-framework-0.9.5.1/moarcframework/management/commands/__init__.py
--rw-rw-rw-   0        0        0      511 2020-08-29 16:49:19.000000 moarc-framework-0.9.5.1/moarcframework/management/commands/clean_migrations.py
--rw-rw-rw-   0        0        0      692 2022-02-20 03:39:41.000000 moarc-framework-0.9.5.1/moarcframework/management/commands/refresh_template.py
-drwxrwxrwx   0        0        0        0 2023-04-10 03:15:40.240566 moarc-framework-0.9.5.1/moarcframework/middleware/
--rw-rw-rw-   0        0        0       25 2022-02-20 03:32:40.000000 moarc-framework-0.9.5.1/moarcframework/middleware/__init__.py
--rw-rw-rw-   0        0        0     1388 2020-08-29 16:49:21.000000 moarc-framework-0.9.5.1/moarcframework/middleware/thread_local_user_middleware.py
-drwxrwxrwx   0        0        0        0 2023-04-10 03:15:40.244427 moarc-framework-0.9.5.1/moarcframework/migrations/
--rw-rw-rw-   0        0        0     9620 2022-05-11 22:37:17.000000 moarc-framework-0.9.5.1/moarcframework/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      598 2022-05-25 02:27:59.000000 moarc-framework-0.9.5.1/moarcframework/migrations/0002_menu_permission.py
--rw-rw-rw-   0        0        0     2427 2023-04-10 03:14:25.000000 moarc-framework-0.9.5.1/moarcframework/migrations/0003_sequence.py
--rw-rw-rw-   0        0        0        0 2022-05-11 22:32:56.000000 moarc-framework-0.9.5.1/moarcframework/migrations/__init__.py
--rw-rw-rw-   0        0        0    10799 2023-04-10 02:57:05.000000 moarc-framework-0.9.5.1/moarcframework/models.py
-drwxrwxrwx   0        0        0        0 2023-04-10 03:15:40.247436 moarc-framework-0.9.5.1/moarcframework/orm/
--rw-rw-rw-   0        0        0       25 2022-02-20 00:41:47.000000 moarc-framework-0.9.5.1/moarcframework/orm/__init__.py
--rw-rw-rw-   0        0        0     9330 2022-09-11 14:11:40.000000 moarc-framework-0.9.5.1/moarcframework/orm/base_model.py
--rw-rw-rw-   0        0        0     2628 2022-02-20 03:41:43.000000 moarc-framework-0.9.5.1/moarcframework/orm/fields.py
-drwxrwxrwx   0        0        0        0 2023-04-10 03:15:40.248437 moarc-framework-0.9.5.1/moarcframework/templatetags/
--rw-rw-rw-   0        0        0       25 2021-12-05 04:03:37.000000 moarc-framework-0.9.5.1/moarcframework/templatetags/__init__.py
--rw-rw-rw-   0        0        0      339 2021-12-23 00:32:40.000000 moarc-framework-0.9.5.1/moarcframework/templatetags/custom_tags.py
-drwxrwxrwx   0        0        0        0 2023-04-10 03:15:40.253497 moarc-framework-0.9.5.1/moarcframework/ui/
--rw-rw-rw-   0        0        0       25 2022-02-20 00:41:55.000000 moarc-framework-0.9.5.1/moarcframework/ui/__init__.py
--rw-rw-rw-   0        0        0     4200 2021-12-24 19:18:04.000000 moarc-framework-0.9.5.1/moarcframework/ui/form.html
--rw-rw-rw-   0        0        0     3525 2021-12-24 19:15:05.000000 moarc-framework-0.9.5.1/moarcframework/ui/import.html
--rw-rw-rw-   0        0        0     1921 2021-12-24 19:13:19.000000 moarc-framework-0.9.5.1/moarcframework/ui/table.html
--rw-rw-rw-   0        0        0      968 2022-05-11 17:38:21.000000 moarc-framework-0.9.5.1/moarcframework/urls.py
--rw-rw-rw-   0        0        0      445 2022-05-11 22:59:46.000000 moarc-framework-0.9.5.1/moarcframework/views.py
--rw-rw-rw-   0        0        0        0 2022-02-20 16:22:45.000000 moarc-framework-0.9.5.1/pyproject.toml
--rw-rw-rw-   0        0        0      910 2023-04-10 03:15:40.255438 moarc-framework-0.9.5.1/setup.cfg
--rw-rw-rw-   0        0        0      141 2022-06-09 04:50:44.000000 moarc-framework-0.9.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:17:06.863266 moarc-framework-0.9.5.2/
+-rw-rw-rw-   0        0        0     1596 2022-02-20 16:21:00.000000 moarc-framework-0.9.5.2/LICENSE
+-rw-rw-rw-   0        0        0      142 2022-09-13 03:58:24.000000 moarc-framework-0.9.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1756 2023-04-10 03:17:06.863266 moarc-framework-0.9.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2022-02-20 16:18:57.000000 moarc-framework-0.9.5.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-10 03:17:06.836257 moarc-framework-0.9.5.2/moarc_framework.egg-info/
+-rw-rw-rw-   0        0        0     1756 2023-04-10 03:17:06.000000 moarc-framework-0.9.5.2/moarc_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1352 2023-04-10 03:17:06.000000 moarc-framework-0.9.5.2/moarc_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 03:17:06.000000 moarc-framework-0.9.5.2/moarc_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-10 03:17:06.000000 moarc-framework-0.9.5.2/moarc_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-10 03:17:06.000000 moarc-framework-0.9.5.2/moarc_framework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 03:17:06.840255 moarc-framework-0.9.5.2/moarcframework/
+-rw-rw-rw-   0        0        0       25 2022-02-20 16:14:26.000000 moarc-framework-0.9.5.2/moarcframework/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:17:06.843258 moarc-framework-0.9.5.2/moarcframework/helpers/
+-rw-rw-rw-   0        0        0       25 2022-02-20 03:31:52.000000 moarc-framework-0.9.5.2/moarcframework/helpers/__init__.py
+-rw-rw-rw-   0        0        0      200 2022-05-11 22:13:28.000000 moarc-framework-0.9.5.2/moarcframework/helpers/auth.py
+-rw-rw-rw-   0        0        0     2314 2022-05-21 15:36:43.000000 moarc-framework-0.9.5.2/moarcframework/helpers/paginator.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:17:06.846256 moarc-framework-0.9.5.2/moarcframework/http/
+-rw-rw-rw-   0        0        0       25 2022-02-20 01:02:24.000000 moarc-framework-0.9.5.2/moarcframework/http/__init__.py
+-rw-rw-rw-   0        0        0      764 2022-05-18 22:46:28.000000 moarc-framework-0.9.5.2/moarcframework/http/decorators.py
+-rw-rw-rw-   0        0        0      191 2022-02-20 15:42:53.000000 moarc-framework-0.9.5.2/moarcframework/http/generic_serializer.py
+-rw-rw-rw-   0        0        0     1089 2022-05-25 03:31:33.000000 moarc-framework-0.9.5.2/moarcframework/http/http.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:17:06.847257 moarc-framework-0.9.5.2/moarcframework/management/
+-rw-rw-rw-   0        0        0        0 2020-08-29 16:49:19.000000 moarc-framework-0.9.5.2/moarcframework/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:17:06.849255 moarc-framework-0.9.5.2/moarcframework/management/commands/
+-rw-rw-rw-   0        0        0        0 2020-08-29 16:49:19.000000 moarc-framework-0.9.5.2/moarcframework/management/commands/__init__.py
+-rw-rw-rw-   0        0        0      511 2020-08-29 16:49:19.000000 moarc-framework-0.9.5.2/moarcframework/management/commands/clean_migrations.py
+-rw-rw-rw-   0        0        0      692 2022-02-20 03:39:41.000000 moarc-framework-0.9.5.2/moarcframework/management/commands/refresh_template.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:17:06.851257 moarc-framework-0.9.5.2/moarcframework/middleware/
+-rw-rw-rw-   0        0        0       25 2022-02-20 03:32:40.000000 moarc-framework-0.9.5.2/moarcframework/middleware/__init__.py
+-rw-rw-rw-   0        0        0     1388 2020-08-29 16:49:21.000000 moarc-framework-0.9.5.2/moarcframework/middleware/thread_local_user_middleware.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:17:06.854283 moarc-framework-0.9.5.2/moarcframework/migrations/
+-rw-rw-rw-   0        0        0     9620 2022-05-11 22:37:17.000000 moarc-framework-0.9.5.2/moarcframework/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      598 2022-05-25 02:27:59.000000 moarc-framework-0.9.5.2/moarcframework/migrations/0002_menu_permission.py
+-rw-rw-rw-   0        0        0     2078 2023-04-10 03:17:03.000000 moarc-framework-0.9.5.2/moarcframework/migrations/0003_sequence.py
+-rw-rw-rw-   0        0        0        0 2022-05-11 22:32:56.000000 moarc-framework-0.9.5.2/moarcframework/migrations/__init__.py
+-rw-rw-rw-   0        0        0    10799 2023-04-10 02:57:05.000000 moarc-framework-0.9.5.2/moarcframework/models.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:17:06.857267 moarc-framework-0.9.5.2/moarcframework/orm/
+-rw-rw-rw-   0        0        0       25 2022-02-20 00:41:47.000000 moarc-framework-0.9.5.2/moarcframework/orm/__init__.py
+-rw-rw-rw-   0        0        0     9330 2022-09-11 14:11:40.000000 moarc-framework-0.9.5.2/moarcframework/orm/base_model.py
+-rw-rw-rw-   0        0        0     2628 2022-02-20 03:41:43.000000 moarc-framework-0.9.5.2/moarcframework/orm/fields.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:17:06.858267 moarc-framework-0.9.5.2/moarcframework/templatetags/
+-rw-rw-rw-   0        0        0       25 2021-12-05 04:03:37.000000 moarc-framework-0.9.5.2/moarcframework/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      339 2021-12-23 00:32:40.000000 moarc-framework-0.9.5.2/moarcframework/templatetags/custom_tags.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:17:06.862265 moarc-framework-0.9.5.2/moarcframework/ui/
+-rw-rw-rw-   0        0        0       25 2022-02-20 00:41:55.000000 moarc-framework-0.9.5.2/moarcframework/ui/__init__.py
+-rw-rw-rw-   0        0        0     4200 2021-12-24 19:18:04.000000 moarc-framework-0.9.5.2/moarcframework/ui/form.html
+-rw-rw-rw-   0        0        0     3525 2021-12-24 19:15:05.000000 moarc-framework-0.9.5.2/moarcframework/ui/import.html
+-rw-rw-rw-   0        0        0     1921 2021-12-24 19:13:19.000000 moarc-framework-0.9.5.2/moarcframework/ui/table.html
+-rw-rw-rw-   0        0        0      968 2022-05-11 17:38:21.000000 moarc-framework-0.9.5.2/moarcframework/urls.py
+-rw-rw-rw-   0        0        0      445 2022-05-11 22:59:46.000000 moarc-framework-0.9.5.2/moarcframework/views.py
+-rw-rw-rw-   0        0        0        0 2022-02-20 16:22:45.000000 moarc-framework-0.9.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0      910 2023-04-10 03:17:06.864267 moarc-framework-0.9.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      141 2022-06-09 04:50:44.000000 moarc-framework-0.9.5.2/setup.py
```

### Comparing `moarc-framework-0.9.5.1/LICENSE` & `moarc-framework-0.9.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.1/PKG-INFO` & `moarc-framework-0.9.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moarc-framework
-Version: 0.9.5.1
+Version: 0.9.5.2
 Summary: A Django app Moarc Framework.
 Home-page: https://www.example.com/
 Author: Eduardo Moron
 Author-email: danix799@gmail.com
 License: BSD-3-Clause
 Description: =====
         Moarc Framework
```

### Comparing `moarc-framework-0.9.5.1/README.rst` & `moarc-framework-0.9.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.1/moarc_framework.egg-info/PKG-INFO` & `moarc-framework-0.9.5.2/moarc_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moarc-framework
-Version: 0.9.5.1
+Version: 0.9.5.2
 Summary: A Django app Moarc Framework.
 Home-page: https://www.example.com/
 Author: Eduardo Moron
 Author-email: danix799@gmail.com
 License: BSD-3-Clause
 Description: =====
         Moarc Framework
```

### Comparing `moarc-framework-0.9.5.1/moarc_framework.egg-info/SOURCES.txt` & `moarc-framework-0.9.5.2/moarc_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.1/moarcframework/helpers/paginator.py` & `moarc-framework-0.9.5.2/moarcframework/helpers/paginator.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.1/moarcframework/http/decorators.py` & `moarc-framework-0.9.5.2/moarcframework/http/decorators.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.1/moarcframework/http/http.py` & `moarc-framework-0.9.5.2/moarcframework/http/http.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.1/moarcframework/management/commands/refresh_template.py` & `moarc-framework-0.9.5.2/moarcframework/management/commands/refresh_template.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.1/moarcframework/middleware/thread_local_user_middleware.py` & `moarc-framework-0.9.5.2/moarcframework/middleware/thread_local_user_middleware.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.1/moarcframework/migrations/0001_initial.py` & `moarc-framework-0.9.5.2/moarcframework/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.1/moarcframework/migrations/0002_menu_permission.py` & `moarc-framework-0.9.5.2/moarcframework/migrations/0002_menu_permission.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.1/moarcframework/migrations/0003_sequence.py` & `moarc-framework-0.9.5.2/moarcframework/migrations/0003_sequence.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Generated by Django 4.0.2 on 2023-04-10 03:14
 
-import apps.moarc-framework.moarcframework.orm.fields
+from ..orm import fields
 from django.db import migrations, models
 import django.utils.timezone
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
@@ -17,22 +17,22 @@
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('active', models.BooleanField(default=True)),
                 ('created_date', models.DateTimeField(blank=True, default=django.utils.timezone.now, null=True, verbose_name='Fecha de creación')),
                 ('updated_date', models.DateTimeField(blank=True, null=True, verbose_name='Fecha de actualización')),
                 ('created_by', models.IntegerField(null=True, verbose_name='Creado por')),
                 ('updated_by', models.IntegerField(null=True, verbose_name='Actualizado por')),
-                ('name', apps.moarc-framework.moarcframework.orm.fields.CharField(blank=True, default='', max_length=200, null=True, verbose_name='Nombre')),
-                ('code', apps.moarc-framework.moarcframework.orm.fields.CharField(blank=True, default='', max_length=200, null=True, verbose_name='Código')),
-                ('prefix', apps.moarc-framework.moarcframework.orm.fields.CharField(blank=True, default='', max_length=200, null=True, verbose_name='Prefijo')),
-                ('suffix', apps.moarc-framework.moarcframework.orm.fields.CharField(blank=True, default='', max_length=200, null=True, verbose_name='Sufijo')),
-                ('current_number', apps.moarc-framework.moarcframework.orm.fields.IntegerField(default=1, verbose_name='Número actual')),
-                ('start', apps.moarc-framework.moarcframework.orm.fields.IntegerField(default=1, verbose_name='Inicio')),
-                ('padding', apps.moarc-framework.moarcframework.orm.fields.IntegerField(default=5, verbose_name='Fin')),
-                ('increment', apps.moarc-framework.moarcframework.orm.fields.IntegerField(default=1, verbose_name='Paso')),
+                ('name', fields.CharField(blank=True, default='', max_length=200, null=True, verbose_name='Nombre')),
+                ('code', fields.CharField(blank=True, default='', max_length=200, null=True, verbose_name='Código')),
+                ('prefix', fields.CharField(blank=True, default='', max_length=200, null=True, verbose_name='Prefijo')),
+                ('suffix', fields.CharField(blank=True, default='', max_length=200, null=True, verbose_name='Sufijo')),
+                ('current_number', fields.IntegerField(default=1, verbose_name='Número actual')),
+                ('start', fields.IntegerField(default=1, verbose_name='Inicio')),
+                ('padding', fields.IntegerField(default=5, verbose_name='Fin')),
+                ('increment', fields.IntegerField(default=1, verbose_name='Paso')),
             ],
             options={
                 'verbose_name': 'Secuencia',
                 'verbose_name_plural': 'Secuencias',
                 'db_table': 'base_sequence',
             },
         ),
```

### Comparing `moarc-framework-0.9.5.1/moarcframework/models.py` & `moarc-framework-0.9.5.2/moarcframework/models.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.1/moarcframework/orm/base_model.py` & `moarc-framework-0.9.5.2/moarcframework/orm/base_model.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.1/moarcframework/orm/fields.py` & `moarc-framework-0.9.5.2/moarcframework/orm/fields.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.1/moarcframework/ui/form.html` & `moarc-framework-0.9.5.2/moarcframework/ui/form.html`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.1/moarcframework/ui/import.html` & `moarc-framework-0.9.5.2/moarcframework/ui/import.html`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.1/moarcframework/ui/table.html` & `moarc-framework-0.9.5.2/moarcframework/ui/table.html`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.1/moarcframework/urls.py` & `moarc-framework-0.9.5.2/moarcframework/urls.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.1/setup.cfg` & `moarc-framework-0.9.5.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6f61 7263 2d66 7261 6d65 776f   = moarc-framewo
 00000020: 726b 0d0a 7665 7273 696f 6e20 3d20 302e  rk..version = 0.
-00000030: 392e 352e 310d 0a64 6573 6372 6970 7469  9.5.1..descripti
+00000030: 392e 352e 320d 0a64 6573 6372 6970 7469  9.5.2..descripti
 00000040: 6f6e 203d 2041 2044 6a61 6e67 6f20 6170  on = A Django ap
 00000050: 7020 4d6f 6172 6320 4672 616d 6577 6f72  p Moarc Framewor
 00000060: 6b2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  k...long_descrip
 00000070: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000080: 444d 452e 7273 740d 0a75 726c 203d 2068  DME.rst..url = h
 00000090: 7474 7073 3a2f 2f77 7777 2e65 7861 6d70  ttps://www.examp
 000000a0: 6c65 2e63 6f6d 2f0d 0a61 7574 686f 7220  le.com/..author
```

