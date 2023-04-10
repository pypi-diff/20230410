# Comparing `tmp/moarc-framework-0.9.4.tar.gz` & `tmp/moarc-framework-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\moarc-framework-0.9.4.tar", last modified: Tue Sep 13 04:01:59 2022, max compression
+gzip compressed data, was "dist\moarc-framework-0.9.5.tar", last modified: Mon Apr 10 02:57:24 2023, max compression
```

## Comparing `moarc-framework-0.9.4.tar` & `moarc-framework-0.9.5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2022-09-13 04:01:59.423576 moarc-framework-0.9.4/
--rw-rw-rw-   0        0        0     1596 2022-02-20 16:21:00.000000 moarc-framework-0.9.4/LICENSE
--rw-rw-rw-   0        0        0      142 2022-09-13 03:58:24.000000 moarc-framework-0.9.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1754 2022-09-13 04:01:59.423576 moarc-framework-0.9.4/PKG-INFO
--rw-rw-rw-   0        0        0      609 2022-02-20 16:18:57.000000 moarc-framework-0.9.4/README.rst
-drwxrwxrwx   0        0        0        0 2022-09-13 04:01:59.399576 moarc-framework-0.9.4/moarc_framework.egg-info/
--rw-rw-rw-   0        0        0     1754 2022-09-13 04:01:59.000000 moarc-framework-0.9.4/moarc_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1309 2022-09-13 04:01:59.000000 moarc-framework-0.9.4/moarc_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-13 04:01:59.000000 moarc-framework-0.9.4/moarc_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2022-09-13 04:01:59.000000 moarc-framework-0.9.4/moarc_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-09-13 04:01:59.000000 moarc-framework-0.9.4/moarc_framework.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-09-13 04:01:59.402577 moarc-framework-0.9.4/moarcframework/
--rw-rw-rw-   0        0        0       25 2022-02-20 16:14:26.000000 moarc-framework-0.9.4/moarcframework/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-13 04:01:59.405576 moarc-framework-0.9.4/moarcframework/helpers/
--rw-rw-rw-   0        0        0       25 2022-02-20 03:31:52.000000 moarc-framework-0.9.4/moarcframework/helpers/__init__.py
--rw-rw-rw-   0        0        0      200 2022-05-11 22:13:28.000000 moarc-framework-0.9.4/moarcframework/helpers/auth.py
--rw-rw-rw-   0        0        0     2314 2022-05-21 15:36:43.000000 moarc-framework-0.9.4/moarcframework/helpers/paginator.py
-drwxrwxrwx   0        0        0        0 2022-09-13 04:01:59.408581 moarc-framework-0.9.4/moarcframework/http/
--rw-rw-rw-   0        0        0       25 2022-02-20 01:02:24.000000 moarc-framework-0.9.4/moarcframework/http/__init__.py
--rw-rw-rw-   0        0        0      764 2022-05-18 22:46:28.000000 moarc-framework-0.9.4/moarcframework/http/decorators.py
--rw-rw-rw-   0        0        0      191 2022-02-20 15:42:53.000000 moarc-framework-0.9.4/moarcframework/http/generic_serializer.py
--rw-rw-rw-   0        0        0     1089 2022-05-25 03:31:33.000000 moarc-framework-0.9.4/moarcframework/http/http.py
-drwxrwxrwx   0        0        0        0 2022-09-13 04:01:59.409576 moarc-framework-0.9.4/moarcframework/management/
--rw-rw-rw-   0        0        0        0 2020-08-29 16:49:19.000000 moarc-framework-0.9.4/moarcframework/management/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-13 04:01:59.410576 moarc-framework-0.9.4/moarcframework/management/commands/
--rw-rw-rw-   0        0        0        0 2020-08-29 16:49:19.000000 moarc-framework-0.9.4/moarcframework/management/commands/__init__.py
--rw-rw-rw-   0        0        0      511 2020-08-29 16:49:19.000000 moarc-framework-0.9.4/moarcframework/management/commands/clean_migrations.py
--rw-rw-rw-   0        0        0      692 2022-02-20 03:39:41.000000 moarc-framework-0.9.4/moarcframework/management/commands/refresh_template.py
-drwxrwxrwx   0        0        0        0 2022-09-13 04:01:59.412576 moarc-framework-0.9.4/moarcframework/middleware/
--rw-rw-rw-   0        0        0       25 2022-02-20 03:32:40.000000 moarc-framework-0.9.4/moarcframework/middleware/__init__.py
--rw-rw-rw-   0        0        0     1388 2020-08-29 16:49:21.000000 moarc-framework-0.9.4/moarcframework/middleware/thread_local_user_middleware.py
-drwxrwxrwx   0        0        0        0 2022-09-13 04:01:59.415577 moarc-framework-0.9.4/moarcframework/migrations/
--rw-rw-rw-   0        0        0     9620 2022-05-11 22:37:17.000000 moarc-framework-0.9.4/moarcframework/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      598 2022-05-25 02:27:59.000000 moarc-framework-0.9.4/moarcframework/migrations/0002_menu_permission.py
--rw-rw-rw-   0        0        0        0 2022-05-11 22:32:56.000000 moarc-framework-0.9.4/moarcframework/migrations/__init__.py
--rw-rw-rw-   0        0        0     9264 2022-09-13 03:58:24.000000 moarc-framework-0.9.4/moarcframework/models.py
-drwxrwxrwx   0        0        0        0 2022-09-13 04:01:59.417576 moarc-framework-0.9.4/moarcframework/orm/
--rw-rw-rw-   0        0        0       25 2022-02-20 00:41:47.000000 moarc-framework-0.9.4/moarcframework/orm/__init__.py
--rw-rw-rw-   0        0        0     9330 2022-09-11 14:11:40.000000 moarc-framework-0.9.4/moarcframework/orm/base_model.py
--rw-rw-rw-   0        0        0     2628 2022-02-20 03:41:43.000000 moarc-framework-0.9.4/moarcframework/orm/fields.py
-drwxrwxrwx   0        0        0        0 2022-09-13 04:01:59.419582 moarc-framework-0.9.4/moarcframework/templatetags/
--rw-rw-rw-   0        0        0       25 2021-12-05 04:03:37.000000 moarc-framework-0.9.4/moarcframework/templatetags/__init__.py
--rw-rw-rw-   0        0        0      339 2021-12-23 00:32:40.000000 moarc-framework-0.9.4/moarcframework/templatetags/custom_tags.py
-drwxrwxrwx   0        0        0        0 2022-09-13 04:01:59.422576 moarc-framework-0.9.4/moarcframework/ui/
--rw-rw-rw-   0        0        0       25 2022-02-20 00:41:55.000000 moarc-framework-0.9.4/moarcframework/ui/__init__.py
--rw-rw-rw-   0        0        0     4200 2021-12-24 19:18:04.000000 moarc-framework-0.9.4/moarcframework/ui/form.html
--rw-rw-rw-   0        0        0     3525 2021-12-24 19:15:05.000000 moarc-framework-0.9.4/moarcframework/ui/import.html
--rw-rw-rw-   0        0        0     1921 2021-12-24 19:13:19.000000 moarc-framework-0.9.4/moarcframework/ui/table.html
--rw-rw-rw-   0        0        0      968 2022-05-11 17:38:21.000000 moarc-framework-0.9.4/moarcframework/urls.py
--rw-rw-rw-   0        0        0      445 2022-05-11 22:59:46.000000 moarc-framework-0.9.4/moarcframework/views.py
--rw-rw-rw-   0        0        0        0 2022-02-20 16:22:45.000000 moarc-framework-0.9.4/pyproject.toml
--rw-rw-rw-   0        0        0      908 2022-09-13 04:01:59.424576 moarc-framework-0.9.4/setup.cfg
--rw-rw-rw-   0        0        0      141 2022-06-09 04:50:44.000000 moarc-framework-0.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 02:57:23.996766 moarc-framework-0.9.5/
+-rw-rw-rw-   0        0        0     1596 2022-02-20 16:21:00.000000 moarc-framework-0.9.5/LICENSE
+-rw-rw-rw-   0        0        0      142 2022-09-13 03:58:24.000000 moarc-framework-0.9.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1754 2023-04-10 02:57:23.996766 moarc-framework-0.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2022-02-20 16:18:57.000000 moarc-framework-0.9.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-10 02:57:23.968812 moarc-framework-0.9.5/moarc_framework.egg-info/
+-rw-rw-rw-   0        0        0     1754 2023-04-10 02:57:23.000000 moarc-framework-0.9.5/moarc_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1309 2023-04-10 02:57:23.000000 moarc-framework-0.9.5/moarc_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 02:57:23.000000 moarc-framework-0.9.5/moarc_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-10 02:57:23.000000 moarc-framework-0.9.5/moarc_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-10 02:57:23.000000 moarc-framework-0.9.5/moarc_framework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 02:57:23.973766 moarc-framework-0.9.5/moarcframework/
+-rw-rw-rw-   0        0        0       25 2022-02-20 16:14:26.000000 moarc-framework-0.9.5/moarcframework/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 02:57:23.975766 moarc-framework-0.9.5/moarcframework/helpers/
+-rw-rw-rw-   0        0        0       25 2022-02-20 03:31:52.000000 moarc-framework-0.9.5/moarcframework/helpers/__init__.py
+-rw-rw-rw-   0        0        0      200 2022-05-11 22:13:28.000000 moarc-framework-0.9.5/moarcframework/helpers/auth.py
+-rw-rw-rw-   0        0        0     2314 2022-05-21 15:36:43.000000 moarc-framework-0.9.5/moarcframework/helpers/paginator.py
+drwxrwxrwx   0        0        0        0 2023-04-10 02:57:23.978795 moarc-framework-0.9.5/moarcframework/http/
+-rw-rw-rw-   0        0        0       25 2022-02-20 01:02:24.000000 moarc-framework-0.9.5/moarcframework/http/__init__.py
+-rw-rw-rw-   0        0        0      764 2022-05-18 22:46:28.000000 moarc-framework-0.9.5/moarcframework/http/decorators.py
+-rw-rw-rw-   0        0        0      191 2022-02-20 15:42:53.000000 moarc-framework-0.9.5/moarcframework/http/generic_serializer.py
+-rw-rw-rw-   0        0        0     1089 2022-05-25 03:31:33.000000 moarc-framework-0.9.5/moarcframework/http/http.py
+drwxrwxrwx   0        0        0        0 2023-04-10 02:57:23.979766 moarc-framework-0.9.5/moarcframework/management/
+-rw-rw-rw-   0        0        0        0 2020-08-29 16:49:19.000000 moarc-framework-0.9.5/moarcframework/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 02:57:23.981766 moarc-framework-0.9.5/moarcframework/management/commands/
+-rw-rw-rw-   0        0        0        0 2020-08-29 16:49:19.000000 moarc-framework-0.9.5/moarcframework/management/commands/__init__.py
+-rw-rw-rw-   0        0        0      511 2020-08-29 16:49:19.000000 moarc-framework-0.9.5/moarcframework/management/commands/clean_migrations.py
+-rw-rw-rw-   0        0        0      692 2022-02-20 03:39:41.000000 moarc-framework-0.9.5/moarcframework/management/commands/refresh_template.py
+drwxrwxrwx   0        0        0        0 2023-04-10 02:57:23.983769 moarc-framework-0.9.5/moarcframework/middleware/
+-rw-rw-rw-   0        0        0       25 2022-02-20 03:32:40.000000 moarc-framework-0.9.5/moarcframework/middleware/__init__.py
+-rw-rw-rw-   0        0        0     1388 2020-08-29 16:49:21.000000 moarc-framework-0.9.5/moarcframework/middleware/thread_local_user_middleware.py
+drwxrwxrwx   0        0        0        0 2023-04-10 02:57:23.986770 moarc-framework-0.9.5/moarcframework/migrations/
+-rw-rw-rw-   0        0        0     9620 2022-05-11 22:37:17.000000 moarc-framework-0.9.5/moarcframework/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      598 2022-05-25 02:27:59.000000 moarc-framework-0.9.5/moarcframework/migrations/0002_menu_permission.py
+-rw-rw-rw-   0        0        0        0 2022-05-11 22:32:56.000000 moarc-framework-0.9.5/moarcframework/migrations/__init__.py
+-rw-rw-rw-   0        0        0    10799 2023-04-10 02:57:05.000000 moarc-framework-0.9.5/moarcframework/models.py
+drwxrwxrwx   0        0        0        0 2023-04-10 02:57:23.989766 moarc-framework-0.9.5/moarcframework/orm/
+-rw-rw-rw-   0        0        0       25 2022-02-20 00:41:47.000000 moarc-framework-0.9.5/moarcframework/orm/__init__.py
+-rw-rw-rw-   0        0        0     9330 2022-09-11 14:11:40.000000 moarc-framework-0.9.5/moarcframework/orm/base_model.py
+-rw-rw-rw-   0        0        0     2628 2022-02-20 03:41:43.000000 moarc-framework-0.9.5/moarcframework/orm/fields.py
+drwxrwxrwx   0        0        0        0 2023-04-10 02:57:23.991766 moarc-framework-0.9.5/moarcframework/templatetags/
+-rw-rw-rw-   0        0        0       25 2021-12-05 04:03:37.000000 moarc-framework-0.9.5/moarcframework/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      339 2021-12-23 00:32:40.000000 moarc-framework-0.9.5/moarcframework/templatetags/custom_tags.py
+drwxrwxrwx   0        0        0        0 2023-04-10 02:57:23.995766 moarc-framework-0.9.5/moarcframework/ui/
+-rw-rw-rw-   0        0        0       25 2022-02-20 00:41:55.000000 moarc-framework-0.9.5/moarcframework/ui/__init__.py
+-rw-rw-rw-   0        0        0     4200 2021-12-24 19:18:04.000000 moarc-framework-0.9.5/moarcframework/ui/form.html
+-rw-rw-rw-   0        0        0     3525 2021-12-24 19:15:05.000000 moarc-framework-0.9.5/moarcframework/ui/import.html
+-rw-rw-rw-   0        0        0     1921 2021-12-24 19:13:19.000000 moarc-framework-0.9.5/moarcframework/ui/table.html
+-rw-rw-rw-   0        0        0      968 2022-05-11 17:38:21.000000 moarc-framework-0.9.5/moarcframework/urls.py
+-rw-rw-rw-   0        0        0      445 2022-05-11 22:59:46.000000 moarc-framework-0.9.5/moarcframework/views.py
+-rw-rw-rw-   0        0        0        0 2022-02-20 16:22:45.000000 moarc-framework-0.9.5/pyproject.toml
+-rw-rw-rw-   0        0        0      908 2023-04-10 02:57:23.998766 moarc-framework-0.9.5/setup.cfg
+-rw-rw-rw-   0        0        0      141 2022-06-09 04:50:44.000000 moarc-framework-0.9.5/setup.py
```

### Comparing `moarc-framework-0.9.4/LICENSE` & `moarc-framework-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.4/PKG-INFO` & `moarc-framework-0.9.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moarc-framework
-Version: 0.9.4
+Version: 0.9.5
 Summary: A Django app Moarc Framework.
 Home-page: https://www.example.com/
 Author: Eduardo Moron
 Author-email: danix799@gmail.com
 License: BSD-3-Clause
 Description: =====
         Moarc Framework
```

### Comparing `moarc-framework-0.9.4/README.rst` & `moarc-framework-0.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.4/moarc_framework.egg-info/PKG-INFO` & `moarc-framework-0.9.5/moarc_framework.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moarc-framework
-Version: 0.9.4
+Version: 0.9.5
 Summary: A Django app Moarc Framework.
 Home-page: https://www.example.com/
 Author: Eduardo Moron
 Author-email: danix799@gmail.com
 License: BSD-3-Clause
 Description: =====
         Moarc Framework
```

### Comparing `moarc-framework-0.9.4/moarc_framework.egg-info/SOURCES.txt` & `moarc-framework-0.9.5/moarc_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.4/moarcframework/helpers/paginator.py` & `moarc-framework-0.9.5/moarcframework/helpers/paginator.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.4/moarcframework/http/decorators.py` & `moarc-framework-0.9.5/moarcframework/http/decorators.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.4/moarcframework/http/http.py` & `moarc-framework-0.9.5/moarcframework/http/http.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.4/moarcframework/management/commands/refresh_template.py` & `moarc-framework-0.9.5/moarcframework/management/commands/refresh_template.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.4/moarcframework/middleware/thread_local_user_middleware.py` & `moarc-framework-0.9.5/moarcframework/middleware/thread_local_user_middleware.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.4/moarcframework/migrations/0001_initial.py` & `moarc-framework-0.9.5/moarcframework/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.4/moarcframework/migrations/0002_menu_permission.py` & `moarc-framework-0.9.5/moarcframework/migrations/0002_menu_permission.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.4/moarcframework/models.py` & `moarc-framework-0.9.5/moarcframework/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -243,7 +243,48 @@
         verbose_name = 'Vista UI'
         verbose_name_plural = 'Vistas UI'
 
     name = fields.CharField(verbose_name="Nombre")
     model = fields.CharField(verbose_name="Modelo")
     path = fields.CharField(verbose_name="Ruta")
     content = fields.TextField(verbose_name="Contenido")
+
+
+class Sequence(BaseModel):
+
+    def _serializer(self):
+        return SequenceSerializer
+
+    class Meta:
+        db_table = 'base_sequence'
+        verbose_name = 'Secuencia'
+        verbose_name_plural = 'Secuencias'
+
+    singular_name = 'sequence'
+    plural_name = 'sequences'
+    search_fields = ['name']
+    list_fields = ['name', 'code', 'prefix', 'suffix']
+
+    name = fields.CharField(verbose_name="Nombre")
+    code = fields.CharField(verbose_name="Código")
+    prefix = fields.CharField(verbose_name="Prefijo", null=True, blank=True)
+    suffix = fields.CharField(verbose_name="Sufijo", null=True, blank=True)
+    current_number = fields.IntegerField(verbose_name="Número actual", default=1)
+    start = fields.IntegerField(verbose_name='Inicio', default=1)
+    padding = fields.IntegerField(verbose_name='Fin', default=5)
+    increment = fields.IntegerField(verbose_name='Paso', default=1)
+
+    @staticmethod
+    def get_next_by_sequence(sequence_code):
+        sequence = Sequence.objects.get(code=sequence_code)
+        number = str(sequence.current_number).zfill(sequence.padding)
+        name_parts = [sequence.prefix, number, sequence.suffix]
+        identifier = "".join([name for name in name_parts if name])
+        sequence.current_number += sequence.increment
+        sequence.save()
+        return identifier
+
+
+class SequenceSerializer(serializers.ModelSerializer):
+    class Meta:
+        model = Sequence
+        fields = ('id', 'name', 'code', 'prefix', 'suffix')
```

### Comparing `moarc-framework-0.9.4/moarcframework/orm/base_model.py` & `moarc-framework-0.9.5/moarcframework/orm/base_model.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.4/moarcframework/orm/fields.py` & `moarc-framework-0.9.5/moarcframework/orm/fields.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.4/moarcframework/ui/form.html` & `moarc-framework-0.9.5/moarcframework/ui/form.html`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.4/moarcframework/ui/import.html` & `moarc-framework-0.9.5/moarcframework/ui/import.html`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.4/moarcframework/ui/table.html` & `moarc-framework-0.9.5/moarcframework/ui/table.html`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.4/moarcframework/urls.py` & `moarc-framework-0.9.5/moarcframework/urls.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.4/setup.cfg` & `moarc-framework-0.9.5/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6f61 7263 2d66 7261 6d65 776f   = moarc-framewo
 00000020: 726b 0d0a 7665 7273 696f 6e20 3d20 302e  rk..version = 0.
-00000030: 392e 340d 0a64 6573 6372 6970 7469 6f6e  9.4..description
+00000030: 392e 350d 0a64 6573 6372 6970 7469 6f6e  9.5..description
 00000040: 203d 2041 2044 6a61 6e67 6f20 6170 7020   = A Django app 
 00000050: 4d6f 6172 6320 4672 616d 6577 6f72 6b2e  Moarc Framework.
 00000060: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
 00000070: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
 00000080: 452e 7273 740d 0a75 726c 203d 2068 7474  E.rst..url = htt
 00000090: 7073 3a2f 2f77 7777 2e65 7861 6d70 6c65  ps://www.example
 000000a0: 2e63 6f6d 2f0d 0a61 7574 686f 7220 3d20  .com/..author =
```

