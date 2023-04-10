# Comparing `tmp/neapolitan-23.3.tar.gz` & `tmp/neapolitan-23.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neapolitan-23.3.tar", last modified: Mon Apr 10 08:28:02 2023, max compression
+gzip compressed data, was "neapolitan-23.4.tar", last modified: Mon Apr 10 10:08:31 2023, max compression
```

## Comparing `neapolitan-23.3.tar` & `neapolitan-23.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       59 2023-04-08 15:53:57.994299 neapolitan-23.3/.gitignore
--rw-r--r--   0        0        0     1081 2023-04-08 09:37:37.437304 neapolitan-23.3/LICENSE
--rw-r--r--   0        0        0      794 2023-04-08 13:24:51.718365 neapolitan-23.3/Notes.txt
--rw-r--r--   0        0        0      942 2023-04-08 15:11:04.794396 neapolitan-23.3/README.rst
--rw-r--r--   0        0        0      638 2023-04-08 10:32:21.337055 neapolitan-23.3/docs/Makefile
--rw-r--r--   0        0        0      804 2023-04-08 10:32:21.337901 neapolitan-23.3/docs/make.bat
--rw-r--r--   0        0        0      943 2023-04-08 13:11:08.113103 neapolitan-23.3/docs/source/conf.py
--rw-r--r--   0        0        0     1162 2023-04-08 15:11:01.258471 neapolitan-23.3/docs/source/index.rst
--rw-r--r--   0        0        0      213 2023-04-08 15:52:45.220880 neapolitan-23.3/justfile
--rw-r--r--   0        0        0      636 2023-04-08 16:03:01.424054 neapolitan-23.3/pyproject.toml
--rw-r--r--   0        0        0      948 2023-04-10 08:27:34.286190 neapolitan-23.3/src/neapolitan/__init__.py
--rw-r--r--   0        0        0      273 2023-01-30 10:02:57.766415 neapolitan-23.3/src/neapolitan/templates/neapolitan/object_confirm_delete.html
--rw-r--r--   0        0        0      149 2023-02-03 20:19:46.419308 neapolitan-23.3/src/neapolitan/templates/neapolitan/object_detail.html
--rw-r--r--   0        0        0      349 2023-01-30 14:23:01.301967 neapolitan-23.3/src/neapolitan/templates/neapolitan/object_form.html
--rw-r--r--   0        0        0      264 2023-04-08 14:09:43.805065 neapolitan-23.3/src/neapolitan/templates/neapolitan/object_list.html
--rw-r--r--   0        0        0      131 2023-01-30 15:27:46.386717 neapolitan-23.3/src/neapolitan/templates/neapolitan/partial/detail.html
--rw-r--r--   0        0        0      313 2023-01-30 19:42:10.115831 neapolitan-23.3/src/neapolitan/templates/neapolitan/partial/list.html
--rw-r--r--   0        0        0        0 2023-01-30 15:19:09.531163 neapolitan-23.3/src/neapolitan/templatetags/__init__.py
--rw-r--r--   0        0        0     1263 2023-04-08 14:11:26.730590 neapolitan-23.3/src/neapolitan/templatetags/neapolitan.py
--rw-r--r--   0        0        0    16076 2023-04-10 08:25:25.914919 neapolitan-23.3/src/neapolitan/views.py
--rw-r--r--   0        0        0        0 2023-04-08 09:49:24.396767 neapolitan-23.3/tests/__init__.py
--rw-r--r--   0        0        0      773 2023-04-08 13:50:59.822848 neapolitan-23.3/tests/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-04-08 09:49:24.398351 neapolitan-23.3/tests/migrations/__init__.py
--rw-r--r--   0        0        0      185 2023-04-08 13:28:20.101701 neapolitan-23.3/tests/models.py
--rw-r--r--   0        0        0     1411 2023-04-08 16:03:51.880684 neapolitan-23.3/tests/settings.py
--rw-r--r--   0        0        0      181 2023-04-08 16:13:55.492481 neapolitan-23.3/tests/templates/base.html
--rw-r--r--   0        0        0     2642 2023-04-10 08:12:45.985067 neapolitan-23.3/tests/tests.py
--rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 neapolitan-23.3/PKG-INFO
+-rw-r--r--   0        0        0       59 2023-04-08 15:53:57.994299 neapolitan-23.4/.gitignore
+-rw-r--r--   0        0        0     1081 2023-04-08 09:37:37.437304 neapolitan-23.4/LICENSE
+-rw-r--r--   0        0        0      837 2023-04-10 08:57:02.274208 neapolitan-23.4/Notes.txt
+-rw-r--r--   0        0        0      942 2023-04-08 15:11:04.794396 neapolitan-23.4/README.rst
+-rw-r--r--   0        0        0      638 2023-04-08 10:32:21.337055 neapolitan-23.4/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-04-08 10:32:21.337901 neapolitan-23.4/docs/make.bat
+-rw-r--r--   0        0        0      943 2023-04-08 13:11:08.113103 neapolitan-23.4/docs/source/conf.py
+-rw-r--r--   0        0        0     1162 2023-04-08 15:11:01.258471 neapolitan-23.4/docs/source/index.rst
+-rw-r--r--   0        0        0      213 2023-04-08 15:52:45.220880 neapolitan-23.4/justfile
+-rw-r--r--   0        0        0      653 2023-04-10 09:35:41.106347 neapolitan-23.4/pyproject.toml
+-rw-r--r--   0        0        0      948 2023-04-10 10:07:28.363677 neapolitan-23.4/src/neapolitan/__init__.py
+-rw-r--r--   0        0        0      273 2023-01-30 10:02:57.766415 neapolitan-23.4/src/neapolitan/templates/neapolitan/object_confirm_delete.html
+-rw-r--r--   0        0        0      149 2023-02-03 20:19:46.419308 neapolitan-23.4/src/neapolitan/templates/neapolitan/object_detail.html
+-rw-r--r--   0        0        0      349 2023-01-30 14:23:01.301967 neapolitan-23.4/src/neapolitan/templates/neapolitan/object_form.html
+-rw-r--r--   0        0        0      264 2023-04-08 14:09:43.805065 neapolitan-23.4/src/neapolitan/templates/neapolitan/object_list.html
+-rw-r--r--   0        0        0      131 2023-01-30 15:27:46.386717 neapolitan-23.4/src/neapolitan/templates/neapolitan/partial/detail.html
+-rw-r--r--   0        0        0      313 2023-01-30 19:42:10.115831 neapolitan-23.4/src/neapolitan/templates/neapolitan/partial/list.html
+-rw-r--r--   0        0        0        0 2023-01-30 15:19:09.531163 neapolitan-23.4/src/neapolitan/templatetags/__init__.py
+-rw-r--r--   0        0        0     1263 2023-04-08 14:11:26.730590 neapolitan-23.4/src/neapolitan/templatetags/neapolitan.py
+-rw-r--r--   0        0        0    16787 2023-04-10 10:04:43.015907 neapolitan-23.4/src/neapolitan/views.py
+-rw-r--r--   0        0        0        0 2023-04-08 09:49:24.396767 neapolitan-23.4/tests/__init__.py
+-rw-r--r--   0        0        0      840 2023-04-10 09:00:23.657242 neapolitan-23.4/tests/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-04-08 09:49:24.398351 neapolitan-23.4/tests/migrations/__init__.py
+-rw-r--r--   0        0        0      236 2023-04-10 08:59:09.860534 neapolitan-23.4/tests/models.py
+-rw-r--r--   0        0        0     1411 2023-04-08 16:03:51.880684 neapolitan-23.4/tests/settings.py
+-rw-r--r--   0        0        0      181 2023-04-08 16:13:55.492481 neapolitan-23.4/tests/templates/base.html
+-rw-r--r--   0        0        0     3850 2023-04-10 09:49:22.975379 neapolitan-23.4/tests/tests.py
+-rw-r--r--   0        0        0     1517 1970-01-01 00:00:00.000000 neapolitan-23.4/PKG-INFO
```

### Comparing `neapolitan-23.3/LICENSE` & `neapolitan-23.4/LICENSE`

 * *Files identical despite different names*

### Comparing `neapolitan-23.3/Notes.txt` & `neapolitan-23.4/Notes.txt`

 * *Files 18% similar despite different names*

```diff
@@ -20,7 +20,11 @@
 
 
 
 
 
 
 .. autoclass:: neapolitan.views.CRUDView
+
+
+
+Filtering and pagination for list view.
```

### Comparing `neapolitan-23.3/README.rst` & `neapolitan-23.4/README.rst`

 * *Files identical despite different names*

### Comparing `neapolitan-23.3/docs/Makefile` & `neapolitan-23.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `neapolitan-23.3/docs/make.bat` & `neapolitan-23.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `neapolitan-23.3/docs/source/conf.py` & `neapolitan-23.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.3/docs/source/index.rst` & `neapolitan-23.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `neapolitan-23.3/src/neapolitan/__init__.py` & `neapolitan-23.4/src/neapolitan/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 
 Where you take your app after that is up to you. But Neapolitan will get you
 started.
 
 Let's go! 🚀
 """
 
-__version__ = "23.3"
+__version__ = "23.4"
```

### Comparing `neapolitan-23.3/src/neapolitan/templatetags/neapolitan.py` & `neapolitan-23.4/src/neapolitan/templatetags/neapolitan.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.3/src/neapolitan/views.py` & `neapolitan-23.4/src/neapolitan/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from django.http import Http404, HttpResponseRedirect
 from django.shortcuts import get_object_or_404
 from django.template.response import TemplateResponse
 from django.urls import path, reverse
 from django.utils.decorators import classonlymethod
 from django.utils.translation import gettext as _
 from django.views.generic import View
+from django_filters.filterset import filterset_factory
 
 
 # A CRUDView is a view that can perform all the CRUD operations on a model. The
 # `role` attribute determines which operations are available for a given
 # as_view() call.
 class Role(enum.Enum):
     LIST = "list"
@@ -90,14 +91,32 @@
     paginate_by = None
     page_kwarg = "page"
     allow_empty = True
 
     # Suffix that should be appended to automatically generated template names.
     template_name_suffix = None
 
+    # Filtering.
+
+    def get_filterset(self, queryset=None):
+        filterset_class = getattr(self, "filterset_class", None)
+        filterset_fields = getattr(self, "filterset_fields", None)
+
+        if filterset_class is None and filterset_fields:
+            filterset_class = filterset_factory(self.model, fields=filterset_fields)
+
+        if filterset_class is None:
+            return None
+
+        return filterset_class(
+            self.request.GET,
+            queryset=queryset,
+            request=self.request,
+        )
+
     # Queryset and object lookup
 
     def get_object(self):
         """
         Returns the object the view is displaying.
         """
         queryset = self.get_queryset()
@@ -272,19 +291,22 @@
         """
         return TemplateResponse(
             request=self.request, template=self.get_template_names(), context=context
         )
 
     def list(self, request, *args, **kwargs):
         queryset = self.get_queryset()
-        paginate_by = self.get_paginate_by()
+        filterset = self.get_filterset(queryset)
+        if filterset is not None:
+            queryset = filterset.qs
 
         if not self.allow_empty and not queryset.exists():
             raise Http404
 
+        paginate_by = self.get_paginate_by()
         if paginate_by is None:
             # Unpaginated response
             self.object_list = queryset
             context = self.get_context_data(
                 page_obj=None,
                 is_paginated=False,
                 paginator=None,
```

### Comparing `neapolitan-23.3/tests/migrations/0001_initial.py` & `neapolitan-23.4/tests/migrations/0001_initial.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.2 on 2023-04-08 08:50
+# Generated by Django 4.2 on 2023-04-10 04:00
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
     initial = True
 
@@ -20,10 +20,11 @@
                         serialize=False,
                         verbose_name="ID",
                     ),
                 ),
                 ("url", models.URLField(unique=True)),
                 ("title", models.CharField(max_length=255)),
                 ("note", models.TextField(blank=True)),
+                ("favourite", models.BooleanField(default=False)),
             ],
         ),
     ]
```

### Comparing `neapolitan-23.3/tests/settings.py` & `neapolitan-23.4/tests/settings.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.3/tests/tests.py` & `neapolitan-23.4/tests/tests.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,26 +6,30 @@
 
 from .models import Bookmark
 
 
 class BookmarkView(CRUDView):
     model = Bookmark
     fields = ["url", "title", "note"]
+    filterset_fields = [
+        "favourite",
+    ]
 
 
 urlpatterns = [] + BookmarkView.get_urls()
 
 
 class BasicTests(TestCase):
     @classmethod
     def setUpTestData(cls):
         cls.homepage = Bookmark.objects.create(
             url="https://noumenal.es/",
             title="Noumenal • Dr Carlton Gibson",
             note="Carlton Gibson's homepage. Blog, Contact and Project links.",
+            favourite=True,
         )
         cls.github = Bookmark.objects.create(
             url="https://github.com/carltongibson",
             title="Carlton Gibson - GitHub",
             note="Carlton Gibson on GitHub",
         )
         cls.fosstodon = Bookmark.objects.create(
@@ -74,7 +78,38 @@
         response = self.client.get(delete_url)
         self.assertEqual(response.status_code, 200)
 
         # Submit the form.
         response = self.client.post(delete_url, follow=True)
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.resolver_match.url_name, "bookmark-list")
+
+    def test_update(self):
+        update_url = reverse("bookmark-update", args=[self.homepage.pk])
+
+        # Load the form.
+        response = self.client.get(update_url)
+        self.assertEqual(response.status_code, 200)
+
+        # Submit the form.
+        response = self.client.post(
+            update_url,
+            {
+                "url": "https://example.com/",
+                "title": "Example",
+                "note": "Example note",
+            },
+            follow=True,
+        )
+        self.assertEqual(response.status_code, 200)
+        self.assertRedirects(
+            response, reverse("bookmark-detail", args=[self.homepage.pk])
+        )
+        self.assertContains(response, "Example")
+
+    def test_filter(self):
+        response = self.client.get("/bookmark/?favourite=true")
+        self.assertEqual(response.status_code, 200)
+        self.assertSequenceEqual([self.homepage], response.context["bookmark_list"])
+        self.assertContains(response, self.homepage.title)
+        self.assertNotContains(response, self.github.title)
+        self.assertNotContains(response, self.fosstodon.title)
```

### Comparing `neapolitan-23.3/PKG-INFO` & `neapolitan-23.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: neapolitan
-Version: 23.3
+Version: 23.4
 Summary: Neapolitan
 Author-email: Carlton Gibson <carlton.gibson@noumenal.es>
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: Django
+Requires-Dist: django-filter
 Requires-Dist: Sphinx ; extra == "docs"
 Requires-Dist: coverage ; extra == "tests"
 Requires-Dist: django_coverage_plugin ; extra == "tests"
 Project-URL: Docs, https://noumenal.es/neapolitan/
 Project-URL: Repository, https://github.com/carltongibson/neapolitan
 Provides-Extra: docs
 Provides-Extra: tests
```

