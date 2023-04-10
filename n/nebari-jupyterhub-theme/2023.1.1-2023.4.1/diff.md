# Comparing `tmp/nebari_jupyterhub_theme-2023.1.1.tar.gz` & `tmp/nebari_jupyterhub_theme-2023.4.1.tar.gz`

## Comparing `nebari_jupyterhub_theme-2023.1.1.tar` & `nebari_jupyterhub_theme-2023.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.1.1/nebari_jupyterhub_theme/__init__.py
--rw-r--r--   0        0        0    54444 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.1.1/nebari_jupyterhub_theme/custom/css/AtkinsonHyperlegible-Bold.ttf
--rw-r--r--   0        0        0    53504 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.1.1/nebari_jupyterhub_theme/custom/css/AtkinsonHyperlegible-Regular.ttf
--rw-r--r--   0        0        0   153944 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.1.1/nebari_jupyterhub_theme/custom/css/Poppins-Bold.ttf
--rw-r--r--   0        0        0   158240 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.1.1/nebari_jupyterhub_theme/custom/css/Poppins-Regular.ttf
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.1.1/nebari_jupyterhub_theme/custom/images/Nebari-Logo-Horizontal-Lockup-White-text.svg
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.1.1/nebari_jupyterhub_theme/custom/images/Nebari-logo-square.svg
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.1.1/nebari_jupyterhub_theme/templates/login.html
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.1.1/nebari_jupyterhub_theme/templates/page.html
--rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.1.1/nebari_jupyterhub_theme/templates/style.css
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.1.1/.gitignore
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.1.1/LICENSE
--rw-r--r--   0        0        0    12426 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.1.1/README.md
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.1.1/pyproject.toml
--rw-r--r--   0        0        0    13236 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.1.1/PKG-INFO
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/__init__.py
+-rw-r--r--   0        0        0    54444 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/custom/css/AtkinsonHyperlegible-Bold.ttf
+-rw-r--r--   0        0        0    53504 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/custom/css/AtkinsonHyperlegible-Regular.ttf
+-rw-r--r--   0        0        0   153944 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/custom/css/Poppins-Bold.ttf
+-rw-r--r--   0        0        0   158240 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/custom/css/Poppins-Regular.ttf
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/custom/images/Nebari-Logo-Horizontal-Lockup-White-text.svg
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/custom/images/Nebari-logo-square.svg
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/templates/login.html
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/templates/page.html
+-rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/templates/style.css
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/.gitignore
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/LICENSE
+-rw-r--r--   0        0        0    12426 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/README.md
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/pyproject.toml
+-rw-r--r--   0        0        0    13236 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/PKG-INFO
```

### Comparing `nebari_jupyterhub_theme-2023.1.1/nebari_jupyterhub_theme/custom/css/AtkinsonHyperlegible-Bold.ttf` & `nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/custom/css/AtkinsonHyperlegible-Bold.ttf`

 * *Files identical despite different names*

### Comparing `nebari_jupyterhub_theme-2023.1.1/nebari_jupyterhub_theme/custom/css/AtkinsonHyperlegible-Regular.ttf` & `nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/custom/css/AtkinsonHyperlegible-Regular.ttf`

 * *Files identical despite different names*

### Comparing `nebari_jupyterhub_theme-2023.1.1/nebari_jupyterhub_theme/custom/css/Poppins-Bold.ttf` & `nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/custom/css/Poppins-Bold.ttf`

 * *Files identical despite different names*

### Comparing `nebari_jupyterhub_theme-2023.1.1/nebari_jupyterhub_theme/custom/css/Poppins-Regular.ttf` & `nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/custom/css/Poppins-Regular.ttf`

 * *Files identical despite different names*

### Comparing `nebari_jupyterhub_theme-2023.1.1/nebari_jupyterhub_theme/custom/images/Nebari-Logo-Horizontal-Lockup-White-text.svg` & `nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/custom/images/Nebari-Logo-Horizontal-Lockup-White-text.svg`

 * *Files identical despite different names*

### Comparing `nebari_jupyterhub_theme-2023.1.1/nebari_jupyterhub_theme/custom/images/Nebari-logo-square.svg` & `nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/custom/images/Nebari-logo-square.svg`

 * *Files identical despite different names*

### Comparing `nebari_jupyterhub_theme-2023.1.1/nebari_jupyterhub_theme/templates/login.html` & `nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/templates/login.html`

 * *Files identical despite different names*

### Comparing `nebari_jupyterhub_theme-2023.1.1/nebari_jupyterhub_theme/templates/page.html` & `nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/templates/page.html`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     <li><a class="dropdown-item" href="{{service.prefix}}">{{service.name}}</a></li>
     {% endfor %}
     </ul>
 </li>
 {% endif %}
 
 <!-- Custom integrations-->
-<li><a href="/auth">User Management</a></li>
+<li><a href="/auth/admin/nebari/console/">User Management</a></li>
 <li><a href="/argo">Argo Workflows</a></li>
 {% if cdsdashboards_enabled %}
     <li><a href="{{ base_url }}dashboards">Dashboards</a></li>
 {% endif %}
 <li><a href="/conda-store">Environment Management</a></li>
 <li><a href="/monitoring">Monitoring</a></li>
```

### Comparing `nebari_jupyterhub_theme-2023.1.1/nebari_jupyterhub_theme/templates/style.css` & `nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/templates/style.css`

 * *Files identical despite different names*

### Comparing `nebari_jupyterhub_theme-2023.1.1/LICENSE` & `nebari_jupyterhub_theme-2023.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nebari_jupyterhub_theme-2023.1.1/README.md` & `nebari_jupyterhub_theme-2023.4.1/README.md`

 * *Files identical despite different names*

### Comparing `nebari_jupyterhub_theme-2023.1.1/pyproject.toml` & `nebari_jupyterhub_theme-2023.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Distributed under the terms of the Modified BSD License.
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "nebari-jupyterhub-theme"
-version = "2023.1.1"
+version = "2023.4.1"
 description = "Nebari JupyterHub theme"
 readme = "README.md"
 license = "BSD-3-Clause"
 requires-python = ">=3.8"
 maintainers = [{ name = "Nebari development team" }]
 keywords = ["jupyterhub", "theme"]
 classifiers = [
```

### Comparing `nebari_jupyterhub_theme-2023.1.1/PKG-INFO` & `nebari_jupyterhub_theme-2023.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nebari-jupyterhub-theme
-Version: 2023.1.1
+Version: 2023.4.1
 Summary: Nebari JupyterHub theme
 Project-URL: Bug Reports, https://github.com/nebari-dev/nebari-jupyterhub-theme/issues
 Project-URL: Homepage, https://nebari.dev
 Project-URL: Source code, https://github.com/nebari-dev/nebari-jupyterhub-theme
 Maintainer: Nebari development team
 License-Expression: BSD-3-Clause
 License-File: LICENSE
```

