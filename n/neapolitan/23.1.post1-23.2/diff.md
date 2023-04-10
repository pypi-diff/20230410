# Comparing `tmp/neapolitan-23.1.post1.tar.gz` & `tmp/neapolitan-23.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neapolitan-23.1.post1.tar", last modified: Sat Apr  8 15:11:43 2023, max compression
+gzip compressed data, was "neapolitan-23.2.tar", last modified: Mon Apr 10 08:09:37 2023, max compression
```

## Comparing `neapolitan-23.1.post1.tar` & `neapolitan-23.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       49 2023-04-08 14:45:43.883877 neapolitan-23.1.post1/.gitignore
--rw-r--r--   0        0        0     1081 2023-04-08 09:37:37.437304 neapolitan-23.1.post1/LICENSE
--rw-r--r--   0        0        0      794 2023-04-08 13:24:51.718365 neapolitan-23.1.post1/Notes.txt
--rw-r--r--   0        0        0      942 2023-04-08 15:11:04.794396 neapolitan-23.1.post1/README.rst
--rw-r--r--   0        0        0      638 2023-04-08 10:32:21.337055 neapolitan-23.1.post1/docs/Makefile
--rw-r--r--   0        0        0      804 2023-04-08 10:32:21.337901 neapolitan-23.1.post1/docs/make.bat
--rw-r--r--   0        0        0      943 2023-04-08 13:11:08.113103 neapolitan-23.1.post1/docs/source/conf.py
--rw-r--r--   0        0        0     1162 2023-04-08 15:11:01.258471 neapolitan-23.1.post1/docs/source/index.rst
--rw-r--r--   0        0        0       70 2023-04-08 10:09:22.500544 neapolitan-23.1.post1/justfile
--rw-r--r--   0        0        0      472 2023-04-08 13:19:11.995123 neapolitan-23.1.post1/pyproject.toml
--rw-r--r--   0        0        0      953 2023-04-08 15:11:24.816613 neapolitan-23.1.post1/src/neapolitan/__init__.py
--rw-r--r--   0        0        0      273 2023-01-30 10:02:57.766415 neapolitan-23.1.post1/src/neapolitan/templates/neapolitan/object_confirm_delete.html
--rw-r--r--   0        0        0      149 2023-02-03 20:19:46.419308 neapolitan-23.1.post1/src/neapolitan/templates/neapolitan/object_detail.html
--rw-r--r--   0        0        0      349 2023-01-30 14:23:01.301967 neapolitan-23.1.post1/src/neapolitan/templates/neapolitan/object_form.html
--rw-r--r--   0        0        0      264 2023-04-08 14:09:43.805065 neapolitan-23.1.post1/src/neapolitan/templates/neapolitan/object_list.html
--rw-r--r--   0        0        0      131 2023-01-30 15:27:46.386717 neapolitan-23.1.post1/src/neapolitan/templates/neapolitan/partial/detail.html
--rw-r--r--   0        0        0      313 2023-01-30 19:42:10.115831 neapolitan-23.1.post1/src/neapolitan/templates/neapolitan/partial/list.html
--rw-r--r--   0        0        0        0 2023-01-30 15:19:09.531163 neapolitan-23.1.post1/src/neapolitan/templatetags/__init__.py
--rw-r--r--   0        0        0     1263 2023-04-08 14:11:26.730590 neapolitan-23.1.post1/src/neapolitan/templatetags/neapolitan.py
--rw-r--r--   0        0        0    16264 2023-04-08 15:06:22.978953 neapolitan-23.1.post1/src/neapolitan/views.py
--rw-r--r--   0        0        0        0 2023-04-08 09:49:24.396767 neapolitan-23.1.post1/tests/__init__.py
--rw-r--r--   0        0        0      773 2023-04-08 13:50:59.822848 neapolitan-23.1.post1/tests/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-04-08 09:49:24.398351 neapolitan-23.1.post1/tests/migrations/__init__.py
--rw-r--r--   0        0        0      185 2023-04-08 13:28:20.101701 neapolitan-23.1.post1/tests/models.py
--rw-r--r--   0        0        0     1384 2023-04-08 14:01:53.085983 neapolitan-23.1.post1/tests/settings.py
--rw-r--r--   0        0        0      190 2023-04-08 13:55:55.998287 neapolitan-23.1.post1/tests/templates/base.html
--rw-r--r--   0        0        0     1249 2023-04-08 14:12:51.663319 neapolitan-23.1.post1/tests/tests.py
--rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 neapolitan-23.1.post1/PKG-INFO
+-rw-r--r--   0        0        0       59 2023-04-08 15:53:57.994299 neapolitan-23.2/.gitignore
+-rw-r--r--   0        0        0     1081 2023-04-08 09:37:37.437304 neapolitan-23.2/LICENSE
+-rw-r--r--   0        0        0      794 2023-04-08 13:24:51.718365 neapolitan-23.2/Notes.txt
+-rw-r--r--   0        0        0      942 2023-04-08 15:11:04.794396 neapolitan-23.2/README.rst
+-rw-r--r--   0        0        0      638 2023-04-08 10:32:21.337055 neapolitan-23.2/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-04-08 10:32:21.337901 neapolitan-23.2/docs/make.bat
+-rw-r--r--   0        0        0      943 2023-04-08 13:11:08.113103 neapolitan-23.2/docs/source/conf.py
+-rw-r--r--   0        0        0     1162 2023-04-08 15:11:01.258471 neapolitan-23.2/docs/source/index.rst
+-rw-r--r--   0        0        0      213 2023-04-08 15:52:45.220880 neapolitan-23.2/justfile
+-rw-r--r--   0        0        0      636 2023-04-08 16:03:01.424054 neapolitan-23.2/pyproject.toml
+-rw-r--r--   0        0        0      948 2023-04-10 08:08:56.237996 neapolitan-23.2/src/neapolitan/__init__.py
+-rw-r--r--   0        0        0      273 2023-01-30 10:02:57.766415 neapolitan-23.2/src/neapolitan/templates/neapolitan/object_confirm_delete.html
+-rw-r--r--   0        0        0      149 2023-02-03 20:19:46.419308 neapolitan-23.2/src/neapolitan/templates/neapolitan/object_detail.html
+-rw-r--r--   0        0        0      349 2023-01-30 14:23:01.301967 neapolitan-23.2/src/neapolitan/templates/neapolitan/object_form.html
+-rw-r--r--   0        0        0      264 2023-04-08 14:09:43.805065 neapolitan-23.2/src/neapolitan/templates/neapolitan/object_list.html
+-rw-r--r--   0        0        0      131 2023-01-30 15:27:46.386717 neapolitan-23.2/src/neapolitan/templates/neapolitan/partial/detail.html
+-rw-r--r--   0        0        0      313 2023-01-30 19:42:10.115831 neapolitan-23.2/src/neapolitan/templates/neapolitan/partial/list.html
+-rw-r--r--   0        0        0        0 2023-01-30 15:19:09.531163 neapolitan-23.2/src/neapolitan/templatetags/__init__.py
+-rw-r--r--   0        0        0     1263 2023-04-08 14:11:26.730590 neapolitan-23.2/src/neapolitan/templatetags/neapolitan.py
+-rw-r--r--   0        0        0    16307 2023-04-10 08:05:59.241948 neapolitan-23.2/src/neapolitan/views.py
+-rw-r--r--   0        0        0        0 2023-04-08 09:49:24.396767 neapolitan-23.2/tests/__init__.py
+-rw-r--r--   0        0        0      773 2023-04-08 13:50:59.822848 neapolitan-23.2/tests/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-04-08 09:49:24.398351 neapolitan-23.2/tests/migrations/__init__.py
+-rw-r--r--   0        0        0      185 2023-04-08 13:28:20.101701 neapolitan-23.2/tests/models.py
+-rw-r--r--   0        0        0     1411 2023-04-08 16:03:51.880684 neapolitan-23.2/tests/settings.py
+-rw-r--r--   0        0        0      181 2023-04-08 16:13:55.492481 neapolitan-23.2/tests/templates/base.html
+-rw-r--r--   0        0        0     2199 2023-04-10 08:07:43.532742 neapolitan-23.2/tests/tests.py
+-rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 neapolitan-23.2/PKG-INFO
```

### Comparing `neapolitan-23.1.post1/LICENSE` & `neapolitan-23.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neapolitan-23.1.post1/Notes.txt` & `neapolitan-23.2/Notes.txt`

 * *Files identical despite different names*

### Comparing `neapolitan-23.1.post1/README.rst` & `neapolitan-23.2/README.rst`

 * *Files identical despite different names*

### Comparing `neapolitan-23.1.post1/docs/Makefile` & `neapolitan-23.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `neapolitan-23.1.post1/docs/make.bat` & `neapolitan-23.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `neapolitan-23.1.post1/docs/source/conf.py` & `neapolitan-23.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.1.post1/docs/source/index.rst` & `neapolitan-23.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `neapolitan-23.1.post1/src/neapolitan/__init__.py` & `neapolitan-23.2/src/neapolitan/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 
 Where you take your app after that is up to you. But Neapolitan will get you
 started.
 
 Let's go! 🚀
 """
 
-__version__ = "23.1post1"
+__version__ = "23.2"
```

### Comparing `neapolitan-23.1.post1/src/neapolitan/templatetags/neapolitan.py` & `neapolitan-23.2/src/neapolitan/templatetags/neapolitan.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.1.post1/src/neapolitan/views.py` & `neapolitan-23.2/src/neapolitan/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,21 +331,22 @@
         return HttpResponseRedirect(self.get_success_url())
 
     def form_invalid(self, form):
         context = self.get_context_data(form=form)
         return self.render_to_response(context)
 
     def get_success_url(self):
+        success_url = getattr(self, "success_url", False)
         if self.role is Role.DELETE:
-            if not self.success_url:
+            if not success_url:
                 msg = "No URL to redirect to. '%s' must define 'success_url'"
                 raise ImproperlyConfigured(msg % self.__class__.__name__)
-            return self.success_url
+            return success_url
         try:
-            return self.success_url or reverse(
+            return success_url or reverse(
                 f"{self.model._meta.model_name}-detail", kwargs={"pk": self.object.pk}
             )
         except AttributeError:
             msg = "No URL to redirect to. '%s' must provide 'success_url' " "or 'model'"
             raise ImproperlyConfigured(msg % self.__class__.__name__)
 
     def confirm_delete(self, request, *args, **kwargs):
```

### Comparing `neapolitan-23.1.post1/tests/migrations/0001_initial.py` & `neapolitan-23.2/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.1.post1/tests/settings.py` & `neapolitan-23.2/tests/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         "OPTIONS": {
             "context_processors": [
                 "django.template.context_processors.debug",
                 "django.template.context_processors.request",
                 "django.contrib.auth.context_processors.auth",
                 "django.contrib.messages.context_processors.messages",
             ],
+            "debug": True,
         },
     },
 ]
 
 
 INSTALLED_APPS = [
     "django.contrib.admin",
```

### Comparing `neapolitan-23.1.post1/PKG-INFO` & `neapolitan-23.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: neapolitan
-Version: 23.1.post1
+Version: 23.2
 Summary: Neapolitan
 Author-email: Carlton Gibson <carlton.gibson@noumenal.es>
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: Django
 Requires-Dist: Sphinx ; extra == "docs"
-Project-URL: Home, https://noumenal.es/neapolitan/
+Requires-Dist: coverage ; extra == "tests"
+Requires-Dist: django_coverage_plugin ; extra == "tests"
+Project-URL: Docs, https://noumenal.es/neapolitan/
+Project-URL: Repository, https://github.com/carltongibson/neapolitan
 Provides-Extra: docs
+Provides-Extra: tests
 
 ==========
 Neapolitan
 ==========
 
 I have a Django model::
```

