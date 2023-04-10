# Comparing `tmp/hx_requests-0.7.2.tar.gz` & `tmp/hx_requests-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hx_requests-0.7.2.tar", max compression
+gzip compressed data, was "hx_requests-0.8.0.tar", max compression
```

## Comparing `hx_requests-0.7.2.tar` & `hx_requests-0.8.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1073 2023-04-10 01:04:34.044628 hx_requests-0.7.2/LICENSE
--rw-r--r--   0        0        0     6283 2023-04-10 01:04:34.044628 hx_requests-0.7.2/README.md
--rw-r--r--   0        0        0     1799 2023-04-10 01:04:34.044628 hx_requests-0.7.2/hx_requests/.gitignore
--rw-r--r--   0        0        0       22 2023-04-10 01:04:58.644938 hx_requests-0.7.2/hx_requests/__init__.py
--rw-r--r--   0        0        0      153 2023-04-10 01:04:34.044628 hx_requests-0.7.2/hx_requests/apps.py
--rw-r--r--   0        0        0     1336 2023-04-10 01:04:34.044628 hx_requests-0.7.2/hx_requests/hx_messages.py
--rw-r--r--   0        0        0    10900 2023-04-10 01:04:34.044628 hx_requests-0.7.2/hx_requests/hx_requests.py
--rw-r--r--   0        0        0     1173 2023-04-10 01:04:34.044628 hx_requests-0.7.2/hx_requests/templates/hx_requests/modal.html
--rw-r--r--   0        0        0        0 2023-04-10 01:04:34.044628 hx_requests-0.7.2/hx_requests/templatetags/__init__.py
--rw-r--r--   0        0        0      620 2023-04-10 01:04:34.044628 hx_requests-0.7.2/hx_requests/templatetags/hx_tags.py
--rw-r--r--   0        0        0     1374 2023-04-10 01:04:34.044628 hx_requests-0.7.2/hx_requests/utils.py
--rw-r--r--   0        0        0     2985 2023-04-10 01:04:34.044628 hx_requests-0.7.2/hx_requests/views.py
--rw-r--r--   0        0        0     1435 2023-04-10 01:04:58.656938 hx_requests-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     7500 1970-01-01 00:00:00.000000 hx_requests-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-10 01:12:24.737968 hx_requests-0.8.0/LICENSE
+-rw-r--r--   0        0        0     6283 2023-04-10 01:12:24.737968 hx_requests-0.8.0/README.md
+-rw-r--r--   0        0        0     1799 2023-04-10 01:12:24.737968 hx_requests-0.8.0/hx_requests/.gitignore
+-rw-r--r--   0        0        0       22 2023-04-10 01:12:59.026013 hx_requests-0.8.0/hx_requests/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-10 01:12:24.737968 hx_requests-0.8.0/hx_requests/apps.py
+-rw-r--r--   0        0        0     1336 2023-04-10 01:12:24.737968 hx_requests-0.8.0/hx_requests/hx_messages.py
+-rw-r--r--   0        0        0    10900 2023-04-10 01:12:24.737968 hx_requests-0.8.0/hx_requests/hx_requests.py
+-rw-r--r--   0        0        0     1173 2023-04-10 01:12:24.737968 hx_requests-0.8.0/hx_requests/templates/hx_requests/modal.html
+-rw-r--r--   0        0        0        0 2023-04-10 01:12:24.737968 hx_requests-0.8.0/hx_requests/templatetags/__init__.py
+-rw-r--r--   0        0        0      620 2023-04-10 01:12:24.737968 hx_requests-0.8.0/hx_requests/templatetags/hx_tags.py
+-rw-r--r--   0        0        0     1374 2023-04-10 01:12:24.737968 hx_requests-0.8.0/hx_requests/utils.py
+-rw-r--r--   0        0        0     3199 2023-04-10 01:12:24.737968 hx_requests-0.8.0/hx_requests/views.py
+-rw-r--r--   0        0        0     1435 2023-04-10 01:12:59.038013 hx_requests-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     7500 1970-01-01 00:00:00.000000 hx_requests-0.8.0/PKG-INFO
```

### Comparing `hx_requests-0.7.2/LICENSE` & `hx_requests-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hx_requests-0.7.2/README.md` & `hx_requests-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `hx_requests-0.7.2/hx_requests/.gitignore` & `hx_requests-0.8.0/hx_requests/.gitignore`

 * *Files identical despite different names*

### Comparing `hx_requests-0.7.2/hx_requests/hx_messages.py` & `hx_requests-0.8.0/hx_requests/hx_messages.py`

 * *Files identical despite different names*

### Comparing `hx_requests-0.7.2/hx_requests/hx_requests.py` & `hx_requests-0.8.0/hx_requests/hx_requests.py`

 * *Files identical despite different names*

### Comparing `hx_requests-0.7.2/hx_requests/templates/hx_requests/modal.html` & `hx_requests-0.8.0/hx_requests/templates/hx_requests/modal.html`

 * *Files identical despite different names*

### Comparing `hx_requests-0.7.2/hx_requests/templatetags/hx_tags.py` & `hx_requests-0.8.0/hx_requests/templatetags/hx_tags.py`

 * *Files identical despite different names*

### Comparing `hx_requests-0.7.2/hx_requests/utils.py` & `hx_requests-0.8.0/hx_requests/utils.py`

 * *Files identical despite different names*

### Comparing `hx_requests-0.7.2/hx_requests/views.py` & `hx_requests-0.8.0/hx_requests/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,19 +41,24 @@
             hx_request.setup_hx_request(request)
             return hx_request.post(request, *args, **kwargs)
         return super().post(request, *args, **kwargs)
 
     def get_hx_request(self, request):
         hx_request_name = request.GET.get("hx_request_name")
         self._get_hx_reqeust_classes()
-        hx_request = next(
-            hx_request
-            for name, hx_request in self.hx_requests.items()
-            if name == hx_request_name
-        )
+        try:
+            hx_request = next(
+                hx_request
+                for name, hx_request in self.hx_requests.items()
+                if name == hx_request_name
+            )
+        except StopIteration:
+            raise Exception(
+                f"No HXRequest found with the name {hx_request_name}. Are you sure it's spelled correctly?"
+            )
         return hx_request()
 
     @classmethod
     def _get_hx_reqeust_classes(cls):
         from .hx_requests import BaseHXRequest
 
         # If the hx_requests are already set don't need to do the whole collection.
```

### Comparing `hx_requests-0.7.2/pyproject.toml` & `hx_requests-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hx-requests"
-version = "0.7.2"
+version = "0.8.0"
 description = "Facilitates the usage of HTMX with Django"
 authors = ["yaakovLowenstein <lowensteinyaakov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/yaakovLowenstein/hx-requests"
 keywords = ["django", "htmx"]
     classifiers=[
```

### Comparing `hx_requests-0.7.2/PKG-INFO` & `hx_requests-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hx-requests
-Version: 0.7.2
+Version: 0.8.0
 Summary: Facilitates the usage of HTMX with Django
 Home-page: https://github.com/yaakovLowenstein/hx-requests
 License: MIT
 Keywords: django,htmx
 Author: yaakovLowenstein
 Author-email: lowensteinyaakov@gmail.com
 Requires-Python: >=3.8,<4.0
```

