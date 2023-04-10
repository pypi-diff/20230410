# Comparing `tmp/django_tailwind_cli-1.4.2.tar.gz` & `tmp/django_tailwind_cli-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tailwind_cli-1.4.2.tar", max compression
+gzip compressed data, was "django_tailwind_cli-1.4.3.tar", max compression
```

## Comparing `django_tailwind_cli-1.4.2.tar` & `django_tailwind_cli-1.4.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1071 2023-04-08 16:07:13.819986 django_tailwind_cli-1.4.2/LICENSE
--rw-r--r--   0        0        0     2817 2023-04-08 16:07:13.819986 django_tailwind_cli-1.4.2/README.md
--rw-r--r--   0        0        0     2725 2023-04-08 16:07:13.819986 django_tailwind_cli-1.4.2/pyproject.toml
--rw-r--r--   0        0        0       78 2023-04-08 16:07:13.819986 django_tailwind_cli-1.4.2/src/django_tailwind_cli/__init__.py
--rw-r--r--   0        0        0      168 2023-04-08 16:07:13.819986 django_tailwind_cli-1.4.2/src/django_tailwind_cli/apps.py
--rw-r--r--   0        0        0        0 2023-04-08 16:07:13.819986 django_tailwind_cli-1.4.2/src/django_tailwind_cli/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-08 16:07:13.819986 django_tailwind_cli-1.4.2/src/django_tailwind_cli/management/commands/__init__.py
--rw-r--r--   0        0        0     4712 2023-04-08 16:07:13.819986 django_tailwind_cli-1.4.2/src/django_tailwind_cli/management/commands/tailwind.py
--rw-r--r--   0        0        0        0 2023-04-08 16:07:13.819986 django_tailwind_cli-1.4.2/src/django_tailwind_cli/py.typed
--rw-r--r--   0        0        0       79 2023-04-08 16:07:13.819986 django_tailwind_cli-1.4.2/src/django_tailwind_cli/styles.css
--rw-r--r--   0        0        0      436 2023-04-08 16:07:13.819986 django_tailwind_cli-1.4.2/src/django_tailwind_cli/tailwind.config.js
--rw-r--r--   0        0        0      518 2023-04-08 16:07:13.819986 django_tailwind_cli-1.4.2/src/django_tailwind_cli/templates/tailwind_cli/base.html
--rw-r--r--   0        0        0      257 2023-04-08 16:07:13.819986 django_tailwind_cli-1.4.2/src/django_tailwind_cli/templates/tailwind_cli/tailwind_css.html
--rw-r--r--   0        0        0        0 2023-04-08 16:07:13.819986 django_tailwind_cli-1.4.2/src/django_tailwind_cli/templatetags/__init__.py
--rw-r--r--   0        0        0      463 2023-04-08 16:07:13.819986 django_tailwind_cli-1.4.2/src/django_tailwind_cli/templatetags/tailwind_cli.py
--rw-r--r--   0        0        0     2961 2023-04-08 16:07:13.819986 django_tailwind_cli-1.4.2/src/django_tailwind_cli/utils.py
--rw-r--r--   0        0        0     4304 1970-01-01 00:00:00.000000 django_tailwind_cli-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/LICENSE
+-rw-r--r--   0        0        0     2836 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/README.md
+-rw-r--r--   0        0        0     2725 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/__init__.py
+-rw-r--r--   0        0        0      168 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/apps.py
+-rw-r--r--   0        0        0        0 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/management/commands/__init__.py
+-rw-r--r--   0        0        0     4712 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/management/commands/tailwind.py
+-rw-r--r--   0        0        0        0 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/py.typed
+-rw-r--r--   0        0        0       79 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/styles.css
+-rw-r--r--   0        0        0      436 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/tailwind.config.js
+-rw-r--r--   0        0        0      518 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/templates/tailwind_cli/base.html
+-rw-r--r--   0        0        0      257 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/templates/tailwind_cli/tailwind_css.html
+-rw-r--r--   0        0        0        0 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/templatetags/__init__.py
+-rw-r--r--   0        0        0      463 2023-04-10 14:22:18.821436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/templatetags/tailwind_cli.py
+-rw-r--r--   0        0        0     2961 2023-04-10 14:22:18.821436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/utils.py
+-rw-r--r--   0        0        0     4323 1970-01-01 00:00:00.000000 django_tailwind_cli-1.4.3/PKG-INFO
```

### Comparing `django_tailwind_cli-1.4.2/LICENSE` & `django_tailwind_cli-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-1.4.2/README.md` & `django_tailwind_cli-1.4.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -24,23 +24,23 @@
 
 ## Requirements
 
 Python 3.8 or newer with Django >= 3.2.
 
 ## Documentation
 
-The documentation can be found at <https://django-tailwind-cli.readthedocs.io>.
+The documentation can be found at <https://oliverandrich.github.io/django-tailwind-cli/>.
 
 ## Installation
 
 ```shell
 python -m pip install django-tailwind-cli
 ```
 
-Check the docs for detailed [installation instructions](https://django-tailwind-cli.readthedocs.io/installation/).
+Check the docs for detailed [installation instructions](https://oliverandrich.github.io/django-tailwind-cli/installation/).
 
 ## Bugs and suggestions
 
 In case you have found a bug or have a suggestion, please open a ticket at <https://github.com/oliverandrich/django-tailwind-cli/issues>.
 
 ## License
```

### Comparing `django_tailwind_cli-1.4.2/pyproject.toml` & `django_tailwind_cli-1.4.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-tailwind-cli"
-version = "1.4.2"
+version = "1.4.3"
 description = "Django and Tailwind integration based on the prebuilt Tailwind CSS CLI."
 license = "MIT"
 authors = ["Oliver Andrich <oliver@andrich.me>"]
 readme = "README.md"
 homepage = "https://oliverandrich.github.io/django-tailwind-cli/"
 repository = "https://github.com/oliverandrich/django-tailwind-cli"
 keywords = ["django", "tailwind", "css"]
```

### Comparing `django_tailwind_cli-1.4.2/src/django_tailwind_cli/management/commands/tailwind.py` & `django_tailwind_cli-1.4.3/src/django_tailwind_cli/management/commands/tailwind.py`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-1.4.2/src/django_tailwind_cli/templates/tailwind_cli/base.html` & `django_tailwind_cli-1.4.3/src/django_tailwind_cli/templates/tailwind_cli/base.html`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-1.4.2/src/django_tailwind_cli/utils.py` & `django_tailwind_cli-1.4.3/src/django_tailwind_cli/utils.py`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-1.4.2/PKG-INFO` & `django_tailwind_cli-1.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tailwind-cli
-Version: 1.4.2
+Version: 1.4.3
 Summary: Django and Tailwind integration based on the prebuilt Tailwind CSS CLI.
 Home-page: https://oliverandrich.github.io/django-tailwind-cli/
 License: MIT
 Keywords: django,tailwind,css
 Author: Oliver Andrich
 Author-email: oliver@andrich.me
 Requires-Python: >=3.8.1,<4
@@ -60,23 +60,23 @@
 
 ## Requirements
 
 Python 3.8 or newer with Django >= 3.2.
 
 ## Documentation
 
-The documentation can be found at <https://django-tailwind-cli.readthedocs.io>.
+The documentation can be found at <https://oliverandrich.github.io/django-tailwind-cli/>.
 
 ## Installation
 
 ```shell
 python -m pip install django-tailwind-cli
 ```
 
-Check the docs for detailed [installation instructions](https://django-tailwind-cli.readthedocs.io/installation/).
+Check the docs for detailed [installation instructions](https://oliverandrich.github.io/django-tailwind-cli/installation/).
 
 ## Bugs and suggestions
 
 In case you have found a bug or have a suggestion, please open a ticket at <https://github.com/oliverandrich/django-tailwind-cli/issues>.
 
 ## License
```

