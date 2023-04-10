# Comparing `tmp/neapolitan-23.2.tar.gz` & `tmp/neapolitan-23.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neapolitan-23.2.tar", last modified: Mon Apr 10 08:09:37 2023, max compression
+gzip compressed data, was "neapolitan-23.3.tar", last modified: Mon Apr 10 08:28:02 2023, max compression
```

## Comparing `neapolitan-23.2.tar` & `neapolitan-23.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       59 2023-04-08 15:53:57.994299 neapolitan-23.2/.gitignore
--rw-r--r--   0        0        0     1081 2023-04-08 09:37:37.437304 neapolitan-23.2/LICENSE
--rw-r--r--   0        0        0      794 2023-04-08 13:24:51.718365 neapolitan-23.2/Notes.txt
--rw-r--r--   0        0        0      942 2023-04-08 15:11:04.794396 neapolitan-23.2/README.rst
--rw-r--r--   0        0        0      638 2023-04-08 10:32:21.337055 neapolitan-23.2/docs/Makefile
--rw-r--r--   0        0        0      804 2023-04-08 10:32:21.337901 neapolitan-23.2/docs/make.bat
--rw-r--r--   0        0        0      943 2023-04-08 13:11:08.113103 neapolitan-23.2/docs/source/conf.py
--rw-r--r--   0        0        0     1162 2023-04-08 15:11:01.258471 neapolitan-23.2/docs/source/index.rst
--rw-r--r--   0        0        0      213 2023-04-08 15:52:45.220880 neapolitan-23.2/justfile
--rw-r--r--   0        0        0      636 2023-04-08 16:03:01.424054 neapolitan-23.2/pyproject.toml
--rw-r--r--   0        0        0      948 2023-04-10 08:08:56.237996 neapolitan-23.2/src/neapolitan/__init__.py
--rw-r--r--   0        0        0      273 2023-01-30 10:02:57.766415 neapolitan-23.2/src/neapolitan/templates/neapolitan/object_confirm_delete.html
--rw-r--r--   0        0        0      149 2023-02-03 20:19:46.419308 neapolitan-23.2/src/neapolitan/templates/neapolitan/object_detail.html
--rw-r--r--   0        0        0      349 2023-01-30 14:23:01.301967 neapolitan-23.2/src/neapolitan/templates/neapolitan/object_form.html
--rw-r--r--   0        0        0      264 2023-04-08 14:09:43.805065 neapolitan-23.2/src/neapolitan/templates/neapolitan/object_list.html
--rw-r--r--   0        0        0      131 2023-01-30 15:27:46.386717 neapolitan-23.2/src/neapolitan/templates/neapolitan/partial/detail.html
--rw-r--r--   0        0        0      313 2023-01-30 19:42:10.115831 neapolitan-23.2/src/neapolitan/templates/neapolitan/partial/list.html
--rw-r--r--   0        0        0        0 2023-01-30 15:19:09.531163 neapolitan-23.2/src/neapolitan/templatetags/__init__.py
--rw-r--r--   0        0        0     1263 2023-04-08 14:11:26.730590 neapolitan-23.2/src/neapolitan/templatetags/neapolitan.py
--rw-r--r--   0        0        0    16307 2023-04-10 08:05:59.241948 neapolitan-23.2/src/neapolitan/views.py
--rw-r--r--   0        0        0        0 2023-04-08 09:49:24.396767 neapolitan-23.2/tests/__init__.py
--rw-r--r--   0        0        0      773 2023-04-08 13:50:59.822848 neapolitan-23.2/tests/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-04-08 09:49:24.398351 neapolitan-23.2/tests/migrations/__init__.py
--rw-r--r--   0        0        0      185 2023-04-08 13:28:20.101701 neapolitan-23.2/tests/models.py
--rw-r--r--   0        0        0     1411 2023-04-08 16:03:51.880684 neapolitan-23.2/tests/settings.py
--rw-r--r--   0        0        0      181 2023-04-08 16:13:55.492481 neapolitan-23.2/tests/templates/base.html
--rw-r--r--   0        0        0     2199 2023-04-10 08:07:43.532742 neapolitan-23.2/tests/tests.py
--rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 neapolitan-23.2/PKG-INFO
+-rw-r--r--   0        0        0       59 2023-04-08 15:53:57.994299 neapolitan-23.3/.gitignore
+-rw-r--r--   0        0        0     1081 2023-04-08 09:37:37.437304 neapolitan-23.3/LICENSE
+-rw-r--r--   0        0        0      794 2023-04-08 13:24:51.718365 neapolitan-23.3/Notes.txt
+-rw-r--r--   0        0        0      942 2023-04-08 15:11:04.794396 neapolitan-23.3/README.rst
+-rw-r--r--   0        0        0      638 2023-04-08 10:32:21.337055 neapolitan-23.3/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-04-08 10:32:21.337901 neapolitan-23.3/docs/make.bat
+-rw-r--r--   0        0        0      943 2023-04-08 13:11:08.113103 neapolitan-23.3/docs/source/conf.py
+-rw-r--r--   0        0        0     1162 2023-04-08 15:11:01.258471 neapolitan-23.3/docs/source/index.rst
+-rw-r--r--   0        0        0      213 2023-04-08 15:52:45.220880 neapolitan-23.3/justfile
+-rw-r--r--   0        0        0      636 2023-04-08 16:03:01.424054 neapolitan-23.3/pyproject.toml
+-rw-r--r--   0        0        0      948 2023-04-10 08:27:34.286190 neapolitan-23.3/src/neapolitan/__init__.py
+-rw-r--r--   0        0        0      273 2023-01-30 10:02:57.766415 neapolitan-23.3/src/neapolitan/templates/neapolitan/object_confirm_delete.html
+-rw-r--r--   0        0        0      149 2023-02-03 20:19:46.419308 neapolitan-23.3/src/neapolitan/templates/neapolitan/object_detail.html
+-rw-r--r--   0        0        0      349 2023-01-30 14:23:01.301967 neapolitan-23.3/src/neapolitan/templates/neapolitan/object_form.html
+-rw-r--r--   0        0        0      264 2023-04-08 14:09:43.805065 neapolitan-23.3/src/neapolitan/templates/neapolitan/object_list.html
+-rw-r--r--   0        0        0      131 2023-01-30 15:27:46.386717 neapolitan-23.3/src/neapolitan/templates/neapolitan/partial/detail.html
+-rw-r--r--   0        0        0      313 2023-01-30 19:42:10.115831 neapolitan-23.3/src/neapolitan/templates/neapolitan/partial/list.html
+-rw-r--r--   0        0        0        0 2023-01-30 15:19:09.531163 neapolitan-23.3/src/neapolitan/templatetags/__init__.py
+-rw-r--r--   0        0        0     1263 2023-04-08 14:11:26.730590 neapolitan-23.3/src/neapolitan/templatetags/neapolitan.py
+-rw-r--r--   0        0        0    16076 2023-04-10 08:25:25.914919 neapolitan-23.3/src/neapolitan/views.py
+-rw-r--r--   0        0        0        0 2023-04-08 09:49:24.396767 neapolitan-23.3/tests/__init__.py
+-rw-r--r--   0        0        0      773 2023-04-08 13:50:59.822848 neapolitan-23.3/tests/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-04-08 09:49:24.398351 neapolitan-23.3/tests/migrations/__init__.py
+-rw-r--r--   0        0        0      185 2023-04-08 13:28:20.101701 neapolitan-23.3/tests/models.py
+-rw-r--r--   0        0        0     1411 2023-04-08 16:03:51.880684 neapolitan-23.3/tests/settings.py
+-rw-r--r--   0        0        0      181 2023-04-08 16:13:55.492481 neapolitan-23.3/tests/templates/base.html
+-rw-r--r--   0        0        0     2642 2023-04-10 08:12:45.985067 neapolitan-23.3/tests/tests.py
+-rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 neapolitan-23.3/PKG-INFO
```

### Comparing `neapolitan-23.2/LICENSE` & `neapolitan-23.3/LICENSE`

 * *Files identical despite different names*

### Comparing `neapolitan-23.2/Notes.txt` & `neapolitan-23.3/Notes.txt`

 * *Files identical despite different names*

### Comparing `neapolitan-23.2/README.rst` & `neapolitan-23.3/README.rst`

 * *Files identical despite different names*

### Comparing `neapolitan-23.2/docs/Makefile` & `neapolitan-23.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `neapolitan-23.2/docs/make.bat` & `neapolitan-23.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `neapolitan-23.2/docs/source/conf.py` & `neapolitan-23.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.2/docs/source/index.rst` & `neapolitan-23.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `neapolitan-23.2/pyproject.toml` & `neapolitan-23.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neapolitan-23.2/src/neapolitan/__init__.py` & `neapolitan-23.3/src/neapolitan/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 
 Where you take your app after that is up to you. But Neapolitan will get you
 started.
 
 Let's go! 🚀
 """
 
-__version__ = "23.2"
+__version__ = "23.3"
```

### Comparing `neapolitan-23.2/src/neapolitan/templatetags/neapolitan.py` & `neapolitan-23.3/src/neapolitan/templatetags/neapolitan.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.2/src/neapolitan/views.py` & `neapolitan-23.3/src/neapolitan/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,15 +62,14 @@
     """
     CRUDView is Neapolitan's core. It provides the standard list, detail,
     create, edit, and delete views for a model, as well as the hooks you need to
     be able to customise any part of that.
     """
 
     role: Role
-    success_url: str
     model = None
     fields = None  # TODO: handle this being None.
 
     # Object lookup parameters. These are used in the URL kwargs, and when
     # performing the model instance lookup.
     # Note that if unset then `lookup_url_kwarg` defaults to using the same
     # value as `lookup_field`.
@@ -331,27 +330,25 @@
         return HttpResponseRedirect(self.get_success_url())
 
     def form_invalid(self, form):
         context = self.get_context_data(form=form)
         return self.render_to_response(context)
 
     def get_success_url(self):
-        success_url = getattr(self, "success_url", False)
+        assert self.model is not None, (
+            "'%s' must define 'model' or override 'get_success_url()'"
+            % self.__class__.__name__
+        )
         if self.role is Role.DELETE:
-            if not success_url:
-                msg = "No URL to redirect to. '%s' must define 'success_url'"
-                raise ImproperlyConfigured(msg % self.__class__.__name__)
-            return success_url
-        try:
-            return success_url or reverse(
+            success_url = reverse(f"{self.model._meta.model_name}-list")
+        else:
+            success_url = reverse(
                 f"{self.model._meta.model_name}-detail", kwargs={"pk": self.object.pk}
             )
-        except AttributeError:
-            msg = "No URL to redirect to. '%s' must provide 'success_url' " "or 'model'"
-            raise ImproperlyConfigured(msg % self.__class__.__name__)
+        return success_url
 
     def confirm_delete(self, request, *args, **kwargs):
         self.object = self.get_object()
         context = self.get_context_data()
         return self.render_to_response(context)
 
     def process_deletion(self, request, *args, **kwargs):
```

### Comparing `neapolitan-23.2/tests/migrations/0001_initial.py` & `neapolitan-23.3/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.2/tests/settings.py` & `neapolitan-23.3/tests/settings.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.2/tests/tests.py` & `neapolitan-23.3/tests/tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,7 +62,19 @@
                 "title": "Example",
                 "note": "Example note",
             },
             follow=True,
         )
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.resolver_match.url_name, "bookmark-detail")
+
+    def test_delete(self):
+        delete_url = reverse("bookmark-delete", args=[self.homepage.pk])
+
+        # Load the form.
+        response = self.client.get(delete_url)
+        self.assertEqual(response.status_code, 200)
+
+        # Submit the form.
+        response = self.client.post(delete_url, follow=True)
+        self.assertEqual(response.status_code, 200)
+        self.assertEqual(response.resolver_match.url_name, "bookmark-list")
```

### Comparing `neapolitan-23.2/PKG-INFO` & `neapolitan-23.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neapolitan
-Version: 23.2
+Version: 23.3
 Summary: Neapolitan
 Author-email: Carlton Gibson <carlton.gibson@noumenal.es>
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: Django
 Requires-Dist: Sphinx ; extra == "docs"
 Requires-Dist: coverage ; extra == "tests"
```

