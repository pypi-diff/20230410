# Comparing `tmp/hx_requests-0.7.1.tar.gz` & `tmp/hx_requests-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hx_requests-0.7.1.tar", max compression
+gzip compressed data, was "hx_requests-0.7.2.tar", max compression
```

## Comparing `hx_requests-0.7.1.tar` & `hx_requests-0.7.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1073 2023-04-10 00:17:54.286103 hx_requests-0.7.1/LICENSE
--rw-r--r--   0        0        0     6283 2023-04-10 00:17:54.286103 hx_requests-0.7.1/README.md
--rw-r--r--   0        0        0     1799 2023-04-10 00:17:54.286103 hx_requests-0.7.1/hx_requests/.gitignore
--rw-r--r--   0        0        0       22 2023-04-10 00:18:19.674009 hx_requests-0.7.1/hx_requests/__init__.py
--rw-r--r--   0        0        0      153 2023-04-10 00:17:54.286103 hx_requests-0.7.1/hx_requests/apps.py
--rw-r--r--   0        0        0     1336 2023-04-10 00:17:54.286103 hx_requests-0.7.1/hx_requests/hx_messages.py
--rw-r--r--   0        0        0    10857 2023-04-10 00:17:54.286103 hx_requests-0.7.1/hx_requests/hx_requests.py
--rw-r--r--   0        0        0     1173 2023-04-10 00:17:54.286103 hx_requests-0.7.1/hx_requests/templates/hx_requests/modal.html
--rw-r--r--   0        0        0        0 2023-04-10 00:17:54.286103 hx_requests-0.7.1/hx_requests/templatetags/__init__.py
--rw-r--r--   0        0        0      620 2023-04-10 00:17:54.286103 hx_requests-0.7.1/hx_requests/templatetags/hx_tags.py
--rw-r--r--   0        0        0     1374 2023-04-10 00:17:54.286103 hx_requests-0.7.1/hx_requests/utils.py
--rw-r--r--   0        0        0     2985 2023-04-10 00:17:54.286103 hx_requests-0.7.1/hx_requests/views.py
--rw-r--r--   0        0        0     1435 2023-04-10 00:18:19.686009 hx_requests-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     7500 1970-01-01 00:00:00.000000 hx_requests-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-10 01:04:34.044628 hx_requests-0.7.2/LICENSE
+-rw-r--r--   0        0        0     6283 2023-04-10 01:04:34.044628 hx_requests-0.7.2/README.md
+-rw-r--r--   0        0        0     1799 2023-04-10 01:04:34.044628 hx_requests-0.7.2/hx_requests/.gitignore
+-rw-r--r--   0        0        0       22 2023-04-10 01:04:58.644938 hx_requests-0.7.2/hx_requests/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-10 01:04:34.044628 hx_requests-0.7.2/hx_requests/apps.py
+-rw-r--r--   0        0        0     1336 2023-04-10 01:04:34.044628 hx_requests-0.7.2/hx_requests/hx_messages.py
+-rw-r--r--   0        0        0    10900 2023-04-10 01:04:34.044628 hx_requests-0.7.2/hx_requests/hx_requests.py
+-rw-r--r--   0        0        0     1173 2023-04-10 01:04:34.044628 hx_requests-0.7.2/hx_requests/templates/hx_requests/modal.html
+-rw-r--r--   0        0        0        0 2023-04-10 01:04:34.044628 hx_requests-0.7.2/hx_requests/templatetags/__init__.py
+-rw-r--r--   0        0        0      620 2023-04-10 01:04:34.044628 hx_requests-0.7.2/hx_requests/templatetags/hx_tags.py
+-rw-r--r--   0        0        0     1374 2023-04-10 01:04:34.044628 hx_requests-0.7.2/hx_requests/utils.py
+-rw-r--r--   0        0        0     2985 2023-04-10 01:04:34.044628 hx_requests-0.7.2/hx_requests/views.py
+-rw-r--r--   0        0        0     1435 2023-04-10 01:04:58.656938 hx_requests-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     7500 1970-01-01 00:00:00.000000 hx_requests-0.7.2/PKG-INFO
```

### Comparing `hx_requests-0.7.1/LICENSE` & `hx_requests-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hx_requests-0.7.1/README.md` & `hx_requests-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `hx_requests-0.7.1/hx_requests/.gitignore` & `hx_requests-0.7.2/hx_requests/.gitignore`

 * *Files identical despite different names*

### Comparing `hx_requests-0.7.1/hx_requests/hx_messages.py` & `hx_requests-0.7.2/hx_requests/hx_messages.py`

 * *Files identical despite different names*

### Comparing `hx_requests-0.7.1/hx_requests/hx_requests.py` & `hx_requests-0.7.2/hx_requests/hx_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,20 +178,19 @@
         return self.get_GET_response(**kwargs)
 
     def get_GET_headers(self, **kwargs) -> Dict:
         """
         For when the form is invalid
         """
         headers = super().get_GET_headers()
-        if (
-            self.request.method == "POST"
-            and self._use_hx_messages
-            and self.show_messages
-        ):
-            headers.update(self.get_message_headers(**kwargs))
+        if self.request.method == "POST":
+            if self._use_hx_messages and self.show_messages:
+                headers.update(self.get_message_headers(**kwargs))
+            if self.no_swap:
+                headers["HX-Reswap"] = "none"
         return headers
 
     def get_form_kwargs(self, **kwargs):
         """Return the keyword arguments for instantiating the form."""
         form_kwargs = {"initial": self.get_initial(**kwargs)}
         if self.request.method in ("POST", "PUT"):
             form_kwargs.update(
```

### Comparing `hx_requests-0.7.1/hx_requests/templates/hx_requests/modal.html` & `hx_requests-0.7.2/hx_requests/templates/hx_requests/modal.html`

 * *Files identical despite different names*

### Comparing `hx_requests-0.7.1/hx_requests/templatetags/hx_tags.py` & `hx_requests-0.7.2/hx_requests/templatetags/hx_tags.py`

 * *Files identical despite different names*

### Comparing `hx_requests-0.7.1/hx_requests/utils.py` & `hx_requests-0.7.2/hx_requests/utils.py`

 * *Files identical despite different names*

### Comparing `hx_requests-0.7.1/hx_requests/views.py` & `hx_requests-0.7.2/hx_requests/views.py`

 * *Files identical despite different names*

### Comparing `hx_requests-0.7.1/pyproject.toml` & `hx_requests-0.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hx-requests"
-version = "0.7.1"
+version = "0.7.2"
 description = "Facilitates the usage of HTMX with Django"
 authors = ["yaakovLowenstein <lowensteinyaakov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/yaakovLowenstein/hx-requests"
 keywords = ["django", "htmx"]
     classifiers=[
```

### Comparing `hx_requests-0.7.1/PKG-INFO` & `hx_requests-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hx-requests
-Version: 0.7.1
+Version: 0.7.2
 Summary: Facilitates the usage of HTMX with Django
 Home-page: https://github.com/yaakovLowenstein/hx-requests
 License: MIT
 Keywords: django,htmx
 Author: yaakovLowenstein
 Author-email: lowensteinyaakov@gmail.com
 Requires-Python: >=3.8,<4.0
```

