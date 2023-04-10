# Comparing `tmp/hx_requests-0.7.0.tar.gz` & `tmp/hx_requests-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hx_requests-0.7.0.tar", max compression
+gzip compressed data, was "hx_requests-0.7.1.tar", max compression
```

## Comparing `hx_requests-0.7.0.tar` & `hx_requests-0.7.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1073 2023-04-09 22:37:27.568819 hx_requests-0.7.0/LICENSE
--rw-r--r--   0        0        0     6283 2023-04-09 22:37:27.568819 hx_requests-0.7.0/README.md
--rw-r--r--   0        0        0     1799 2023-04-09 22:37:27.568819 hx_requests-0.7.0/hx_requests/.gitignore
--rw-r--r--   0        0        0       22 2023-04-09 22:37:52.793101 hx_requests-0.7.0/hx_requests/__init__.py
--rw-r--r--   0        0        0      153 2023-04-09 22:37:27.568819 hx_requests-0.7.0/hx_requests/apps.py
--rw-r--r--   0        0        0     1336 2023-04-09 22:37:27.568819 hx_requests-0.7.0/hx_requests/hx_messages.py
--rw-r--r--   0        0        0    10847 2023-04-09 22:37:27.568819 hx_requests-0.7.0/hx_requests/hx_requests.py
--rw-r--r--   0        0        0     1156 2023-04-09 22:37:27.568819 hx_requests-0.7.0/hx_requests/templates/hx_requests/modal.html
--rw-r--r--   0        0        0        0 2023-04-09 22:37:27.568819 hx_requests-0.7.0/hx_requests/templatetags/__init__.py
--rw-r--r--   0        0        0      620 2023-04-09 22:37:27.568819 hx_requests-0.7.0/hx_requests/templatetags/hx_tags.py
--rw-r--r--   0        0        0     1374 2023-04-09 22:37:27.568819 hx_requests-0.7.0/hx_requests/utils.py
--rw-r--r--   0        0        0     2985 2023-04-09 22:37:27.568819 hx_requests-0.7.0/hx_requests/views.py
--rw-r--r--   0        0        0     1435 2023-04-09 22:37:52.805101 hx_requests-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     7500 1970-01-01 00:00:00.000000 hx_requests-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-10 00:17:54.286103 hx_requests-0.7.1/LICENSE
+-rw-r--r--   0        0        0     6283 2023-04-10 00:17:54.286103 hx_requests-0.7.1/README.md
+-rw-r--r--   0        0        0     1799 2023-04-10 00:17:54.286103 hx_requests-0.7.1/hx_requests/.gitignore
+-rw-r--r--   0        0        0       22 2023-04-10 00:18:19.674009 hx_requests-0.7.1/hx_requests/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-10 00:17:54.286103 hx_requests-0.7.1/hx_requests/apps.py
+-rw-r--r--   0        0        0     1336 2023-04-10 00:17:54.286103 hx_requests-0.7.1/hx_requests/hx_messages.py
+-rw-r--r--   0        0        0    10857 2023-04-10 00:17:54.286103 hx_requests-0.7.1/hx_requests/hx_requests.py
+-rw-r--r--   0        0        0     1173 2023-04-10 00:17:54.286103 hx_requests-0.7.1/hx_requests/templates/hx_requests/modal.html
+-rw-r--r--   0        0        0        0 2023-04-10 00:17:54.286103 hx_requests-0.7.1/hx_requests/templatetags/__init__.py
+-rw-r--r--   0        0        0      620 2023-04-10 00:17:54.286103 hx_requests-0.7.1/hx_requests/templatetags/hx_tags.py
+-rw-r--r--   0        0        0     1374 2023-04-10 00:17:54.286103 hx_requests-0.7.1/hx_requests/utils.py
+-rw-r--r--   0        0        0     2985 2023-04-10 00:17:54.286103 hx_requests-0.7.1/hx_requests/views.py
+-rw-r--r--   0        0        0     1435 2023-04-10 00:18:19.686009 hx_requests-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     7500 1970-01-01 00:00:00.000000 hx_requests-0.7.1/PKG-INFO
```

### Comparing `hx_requests-0.7.0/LICENSE` & `hx_requests-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hx_requests-0.7.0/README.md` & `hx_requests-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `hx_requests-0.7.0/hx_requests/.gitignore` & `hx_requests-0.7.1/hx_requests/.gitignore`

 * *Files identical despite different names*

### Comparing `hx_requests-0.7.0/hx_requests/hx_messages.py` & `hx_requests-0.7.1/hx_requests/hx_messages.py`

 * *Files identical despite different names*

### Comparing `hx_requests-0.7.0/hx_requests/hx_requests.py` & `hx_requests-0.7.1/hx_requests/hx_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,23 +256,23 @@
 
 
 class HXModal(HXRequestGET):
     name = "hx_modal"
     modal_template = getattr(
         settings, "HX_REQUSTS_MODAL_TEMPLATE", "hx_requests/modal.html"
     )
-    modal_wrapper_id = getattr(
-        settings, "HX_REQUSTS_MODAL_WRAPPER_ID", "hx_modal_wrapper"
+    modal_container_id = getattr(
+        settings, "HX_REQUSTS_MODAL_CONTAINER_ID", "hx_modal_container"
     )
 
     def get_GET_context_data(self, **kwargs) -> Dict:
         context = super().get_context_data(**kwargs)
         body = kwargs.get("body", self.GET_template)
         context["title"] = kwargs.get("title", self.hx_object)
-        context["modal_wrapper_id"] = self.modal_wrapper_id
+        context["modal_container_id"] = self.modal_container_id
         context["body"] = (
             render_to_string(body, context=context)
             if body.split(".")[-1] == "html"
             else body
         )
         return context
```

### Comparing `hx_requests-0.7.0/hx_requests/templates/hx_requests/modal.html` & `hx_requests-0.7.1/hx_requests/templates/hx_requests/modal.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-<div id="modal-backdrop"
+<div id="hx_modal_backdrop"
      class="modal-backdrop fade show"
      style="display:block"></div>
-<div id="modal"
+<div id="hx_modal"
      class="modal fade show"
      tabindex="-1"
      style="display:block">
     <div class="modal-dialog modal-dialog-centered">
         <div class="modal-content">
             <div class="modal-header">
                 <h5 class="modal-title">{{ title }}</h5>
@@ -17,22 +17,21 @@
                 <button type="button" class="btn btn-secondary" onclick="closeHXModal()">Close</button>
             </div>
         </div>
     </div>
 </div>
 <script>
     function closeHXModal() {
-        const container = document.getElementById('hx_modal_wrapper')
-        const backdrop = document.getElementById("modal-backdrop")
-        const modal = document.getElementById("modal")
+        const container = document.getElementById('{{modal_container_id}}')
+        const backdrop = document.getElementById("hx_modal_backdrop")
+        const modal = document.getElementById("hx_modal")
 
         modal.classList.remove("show")
         backdrop.classList.remove("show")
 
         setTimeout(function () {
             container.innerHTML = ''
         }, 200)
 }
        document.addEventListener('modalFormValid',closeHXModal)
 
-
 </script>
```

### Comparing `hx_requests-0.7.0/hx_requests/templatetags/hx_tags.py` & `hx_requests-0.7.1/hx_requests/templatetags/hx_tags.py`

 * *Files identical despite different names*

### Comparing `hx_requests-0.7.0/hx_requests/utils.py` & `hx_requests-0.7.1/hx_requests/utils.py`

 * *Files identical despite different names*

### Comparing `hx_requests-0.7.0/hx_requests/views.py` & `hx_requests-0.7.1/hx_requests/views.py`

 * *Files identical despite different names*

### Comparing `hx_requests-0.7.0/pyproject.toml` & `hx_requests-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hx-requests"
-version = "0.7.0"
+version = "0.7.1"
 description = "Facilitates the usage of HTMX with Django"
 authors = ["yaakovLowenstein <lowensteinyaakov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/yaakovLowenstein/hx-requests"
 keywords = ["django", "htmx"]
     classifiers=[
```

### Comparing `hx_requests-0.7.0/PKG-INFO` & `hx_requests-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hx-requests
-Version: 0.7.0
+Version: 0.7.1
 Summary: Facilitates the usage of HTMX with Django
 Home-page: https://github.com/yaakovLowenstein/hx-requests
 License: MIT
 Keywords: django,htmx
 Author: yaakovLowenstein
 Author-email: lowensteinyaakov@gmail.com
 Requires-Python: >=3.8,<4.0
```

