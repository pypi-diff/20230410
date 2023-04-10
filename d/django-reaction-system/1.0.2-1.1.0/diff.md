# Comparing `tmp/django-reaction-system-1.0.2.tar.gz` & `tmp/django-reaction-system-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-reaction-system-1.0.2.tar", last modified: Mon Apr  3 07:13:05 2023, max compression
+gzip compressed data, was "django-reaction-system-1.1.0.tar", last modified: Mon Apr 10 11:16:15 2023, max compression
```

## Comparing `django-reaction-system-1.0.2.tar` & `django-reaction-system-1.1.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:13:05.007578 django-reaction-system-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-03 07:13:05.007578 django-reaction-system-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:13:05.007578 django-reaction-system-1.0.2/django_reaction_system.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-03 07:13:04.000000 django-reaction-system-1.0.2/django_reaction_system.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:13:05.003579 django-reaction-system-1.0.2/reaction/
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/reaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/reaction/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/reaction/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:13:05.007578 django-reaction-system-1.0.2/reaction/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/reaction/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/reaction/migrations/0002_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/reaction/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/reaction/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/reaction/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:13:05.003579 django-reaction-system-1.0.2/reaction/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:13:05.003579 django-reaction-system-1.0.2/reaction/static/reaction/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:13:05.007578 django-reaction-system-1.0.2/reaction/static/reaction/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/reaction/static/reaction/css/style.css
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/reaction/static/reaction/css/style.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:13:05.007578 django-reaction-system-1.0.2/reaction/static/reaction/js/
--rw-r--r--   0 runner    (1001) docker     (123)    89574 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/reaction/static/reaction/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/reaction/static/reaction/js/reaction.js
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/reaction/static/reaction/js/reaction.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:13:05.007578 django-reaction-system-1.0.2/reaction/static/reaction/tailwindcss/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/reaction/static/reaction/tailwindcss/style.css
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/reaction/static/reaction/tailwindcss/tailwind.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:13:05.003579 django-reaction-system-1.0.2/reaction/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:13:05.003579 django-reaction-system-1.0.2/reaction/templates/reaction/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:13:05.007578 django-reaction-system-1.0.2/reaction/templates/reaction/reaction/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/reaction/templates/reaction/reaction/reaction.html
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/reaction/templates/reaction/reaction/reaction_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:13:05.007578 django-reaction-system-1.0.2/reaction/templates/reaction/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/reaction/templates/reaction/utils/IMPORTS.html
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/reaction/templates/reaction/utils/SCRIPTS.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:13:05.007578 django-reaction-system-1.0.2/reaction/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/reaction/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/reaction/templatetags/reaction_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/reaction/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/reaction/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/reaction/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-03 07:13:05.007578 django-reaction-system-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 07:13:00.000000 django-reaction-system-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.474034 django-reaction-system-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-10 11:16:15.474034 django-reaction-system-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.474034 django-reaction-system-1.1.0/django_reaction_system.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-10 11:16:15.000000 django-reaction-system-1.1.0/django_reaction_system.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.474034 django-reaction-system-1.1.0/reaction/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.474034 django-reaction-system-1.1.0/reaction/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/migrations/0002_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.470034 django-reaction-system-1.1.0/reaction/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.470034 django-reaction-system-1.1.0/reaction/static/reaction/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.474034 django-reaction-system-1.1.0/reaction/static/reaction/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/static/reaction/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/static/reaction/css/style.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.474034 django-reaction-system-1.1.0/reaction/static/reaction/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    89574 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/static/reaction/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/static/reaction/js/reaction.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/static/reaction/js/reaction.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.474034 django-reaction-system-1.1.0/reaction/static/reaction/tailwindcss/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/static/reaction/tailwindcss/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/static/reaction/tailwindcss/tailwind.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.470034 django-reaction-system-1.1.0/reaction/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.470034 django-reaction-system-1.1.0/reaction/templates/reaction/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.474034 django-reaction-system-1.1.0/reaction/templates/reaction/reaction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/templates/reaction/reaction/reaction.html
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/templates/reaction/reaction/reaction_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.474034 django-reaction-system-1.1.0/reaction/templates/reaction/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/templates/reaction/utils/IMPORTS.html
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/templates/reaction/utils/SCRIPTS.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.474034 django-reaction-system-1.1.0/reaction/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/templatetags/reaction_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-10 11:16:15.478034 django-reaction-system-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/setup.py
```

### Comparing `django-reaction-system-1.0.2/LICENSE` & `django-reaction-system-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-reaction-system-1.0.2/PKG-INFO` & `django-reaction-system-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-reaction-system
-Version: 1.0.2
+Version: 1.1.0
 Summary: Django reaction System, It can be associated with any given model.
 Home-page: https://github.com/mahyar-amiri/django-reaction-system
 Author: Mahyar Amiri
 Author-email: mmaahhyyaarr@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/mahyar-amiri/django-reaction-system/README.md
 Project-URL: Source Code, https://github.com/mahyar-amiri/django-reaction-system
```

### Comparing `django-reaction-system-1.0.2/README.md` & `django-reaction-system-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 # Django Reaction System
 
+<p align="center">
+  <img src="image.png" />
+</p>
+
 [![PyPI version](https://img.shields.io/pypi/v/django-reaction-system.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/django-reaction-system)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/django-reaction-system?color=092E20&logo=django)](https://pypi.org/project/django-reaction-system)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/django-reaction-system?color=092E20&logo=django)](https://pypistats.org/packages/django-reaction-system)
 [![GitHub](https://img.shields.io/github/license/mahyar-amiri/django-reaction-system)](LICENSE)
 
+**Here is a [live demo](https://mmaahhyyaarr.pythonanywhere.com/)**
+
 ## Table of Contents
 
 * [Installation](#installation)
 * [Configuration](#configuration)
 * [Usage](#usage)
 * [Settings](#settings)
     * [Global Settings](#global-settings)
     * [Config Settings](#config-settings)
 * [Front-End](#front-end)
+* [Live Demo](https://mmaahhyyaarr.pythonanywhere.com/)
 
 ## Installation
 
 1. Install using pip
 
    ```shell
    python -m pip install django-reaction-system
```

### Comparing `django-reaction-system-1.0.2/README.rst` & `django-reaction-system-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-reaction-system-1.0.2/django_reaction_system.egg-info/SOURCES.txt` & `django-reaction-system-1.1.0/django_reaction_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-reaction-system-1.0.2/reaction/__init__.py` & `django-reaction-system-1.1.0/reaction/__init__.py`

 * *Files identical despite different names*

### Comparing `django-reaction-system-1.0.2/reaction/admin.py` & `django-reaction-system-1.1.0/reaction/admin.py`

 * *Files identical despite different names*

### Comparing `django-reaction-system-1.0.2/reaction/migrations/0001_initial.py` & `django-reaction-system-1.1.0/reaction/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-reaction-system-1.0.2/reaction/migrations/0002_config.py` & `django-reaction-system-1.1.0/reaction/migrations/0002_config.py`

 * *Files identical despite different names*

### Comparing `django-reaction-system-1.0.2/reaction/models.py` & `django-reaction-system-1.1.0/reaction/models.py`

 * *Files identical despite different names*

### Comparing `django-reaction-system-1.0.2/reaction/static/reaction/css/style.css` & `django-reaction-system-1.1.0/reaction/static/reaction/css/style.css`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,18 @@
   height: 1.5rem;
 }
 
 .w-6 {
   width: 1.5rem;
 }
 
+.cursor-pointer {
+  cursor: pointer;
+}
+
 .origin-bottom {
   transform-origin: bottom;
 }
 
 .rounded-full {
   border-radius: 9999px;
 }
```

### Comparing `django-reaction-system-1.0.2/reaction/static/reaction/css/style.min.css` & `django-reaction-system-1.1.0/reaction/static/reaction/css/style.min.css`

 * *Files 8% similar despite different names*

```diff
@@ -1 +1 @@
-.inline{display: inline}.h-12{height: 3rem}.h-6{height: 1.5rem}.w-6{width: 1.5rem}.origin-bottom{transform-origin: bottom}.rounded-full{border-radius: 9999px}.border-2{border-width: 2px}.border-solid{border-style: solid}.border-react-default-border-light{--tw-border-opacity: 1;border-color: rgb(229 231 235 / var(--tw-border-opacity))}.border-react-selected-border-light{--tw-border-opacity: 1;border-color: rgb(191 219 254 / var(--tw-border-opacity))}.bg-react-default-bg-light{--tw-bg-opacity: 1;background-color: rgb(243 244 246 / var(--tw-bg-opacity))}.bg-react-selected-bg-light{--tw-bg-opacity: 1;background-color: rgb(219 234 254 / var(--tw-bg-opacity))}.px-2{padding-left: 0.5rem;padding-right: 0.5rem}.py-2{padding-top: 0.5rem;padding-bottom: 0.5rem}.text-base{font-size: 1rem;line-height: 1.5rem}.text-react-count-text-light{--tw-text-opacity: 1;color: rgb(0 0 0 / var(--tw-text-opacity))}.transition-transform{transition-property: transform;transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);transition-duration: 150ms}.duration-200{transition-duration: 200ms}.group:hover .group-hover\:scale-150{--tw-scale-x: 1.5;--tw-scale-y: 1.5;transform: translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}[dir="ltr"] .ltr\:pr-1{padding-right: 0.25rem}[dir="rtl"] .rtl\:pl-1{padding-left: 0.25rem}[data-mode="dark"] .dark\:border-react-default-border-dark{--tw-border-opacity: 1;border-color: rgb(107 114 128 / var(--tw-border-opacity))}[data-mode="dark"] .dark\:border-react-selected-border-dark{--tw-border-opacity: 1;border-color: rgb(30 41 59 / var(--tw-border-opacity))}[data-mode="dark"] .dark\:bg-react-default-bg-dark{--tw-bg-opacity: 1;background-color: rgb(51 65 85 / var(--tw-bg-opacity))}[data-mode="dark"] .dark\:bg-react-selected-bg-dark{--tw-bg-opacity: 1;background-color: rgb(100 116 139 / var(--tw-bg-opacity))}[data-mode="dark"] .dark\:text-react-count-text-dark{--tw-text-opacity: 1;color: rgb(243 244 246 / var(--tw-text-opacity))}
+.inline{display: inline}.h-12{height: 3rem}.h-6{height: 1.5rem}.w-6{width: 1.5rem}.cursor-pointer{cursor:pointer}.origin-bottom{transform-origin: bottom}.rounded-full{border-radius: 9999px}.border-2{border-width: 2px}.border-solid{border-style: solid}.border-react-default-border-light{--tw-border-opacity: 1;border-color: rgb(229 231 235 / var(--tw-border-opacity))}.border-react-selected-border-light{--tw-border-opacity: 1;border-color: rgb(191 219 254 / var(--tw-border-opacity))}.bg-react-default-bg-light{--tw-bg-opacity: 1;background-color: rgb(243 244 246 / var(--tw-bg-opacity))}.bg-react-selected-bg-light{--tw-bg-opacity: 1;background-color: rgb(219 234 254 / var(--tw-bg-opacity))}.px-2{padding-left: 0.5rem;padding-right: 0.5rem}.py-2{padding-top: 0.5rem;padding-bottom: 0.5rem}.text-base{font-size: 1rem;line-height: 1.5rem}.text-react-count-text-light{--tw-text-opacity: 1;color: rgb(0 0 0 / var(--tw-text-opacity))}.transition-transform{transition-property: transform;transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);transition-duration: 150ms}.duration-200{transition-duration: 200ms}.group:hover .group-hover\:scale-150{--tw-scale-x: 1.5;--tw-scale-y: 1.5;transform: translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}[dir="ltr"] .ltr\:pr-1{padding-right: 0.25rem}[dir="rtl"] .rtl\:pl-1{padding-left: 0.25rem}[data-mode="dark"] .dark\:border-react-default-border-dark{--tw-border-opacity: 1;border-color: rgb(107 114 128 / var(--tw-border-opacity))}[data-mode="dark"] .dark\:border-react-selected-border-dark{--tw-border-opacity: 1;border-color: rgb(30 41 59 / var(--tw-border-opacity))}[data-mode="dark"] .dark\:bg-react-default-bg-dark{--tw-bg-opacity: 1;background-color: rgb(51 65 85 / var(--tw-bg-opacity))}[data-mode="dark"] .dark\:bg-react-selected-bg-dark{--tw-bg-opacity: 1;background-color: rgb(100 116 139 / var(--tw-bg-opacity))}[data-mode="dark"] .dark\:text-react-count-text-dark{--tw-text-opacity: 1;color: rgb(243 244 246 / var(--tw-text-opacity))}
```

### Comparing `django-reaction-system-1.0.2/reaction/static/reaction/js/jquery.min.js` & `django-reaction-system-1.1.0/reaction/static/reaction/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-reaction-system-1.0.2/reaction/static/reaction/tailwindcss/tailwind.config.js` & `django-reaction-system-1.1.0/reaction/static/reaction/tailwindcss/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `django-reaction-system-1.0.2/reaction/templates/reaction/reaction/reaction.html` & `django-reaction-system-1.1.0/reaction/templates/reaction/reaction/reaction.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% load reaction_tags %}
 
 {% for react, count in reacts.items %}
     <button type="button" {% if request.user.is_authenticated %} onclick="React('{{ reaction.urlhash }}', '{{ react.slug }}')" {% endif %}
-            class="group h-12 rounded-full border-solid border-2 py-2 px-2 {% if react == user_react %}border-react-selected-border-light bg-react-selected-bg-light dark:border-react-selected-border-dark dark:bg-react-selected-bg-dark{% else %}border-react-default-border-light bg-react-default-bg-light dark:border-react-default-border-dark dark:bg-react-default-bg-dark{% endif %}">
+            class="group h-12 rounded-full border-solid border-2 py-2 px-2 cursor-pointer {% if react == user_react %}border-react-selected-border-light bg-react-selected-bg-light dark:border-react-selected-border-dark dark:bg-react-selected-bg-dark{% else %}border-react-default-border-light bg-react-default-bg-light dark:border-react-default-border-dark dark:bg-react-default-bg-dark{% endif %}">
         {% if reaction.settings.react_type == 's' and react.source %}
             <img src="{{ react.source.url }}" alt="{{ react.emoji }}" class="w-6 h-6 inline transition-transform duration-200 origin-bottom group-hover:scale-150">
         {% else %}
             <span class="w-6 h-6 inline text-base">{{ react.emoji }}</span>
         {% endif %}
         {% if count %} <span class="ltr:pr-1 rtl:pl-1 text-react-count-text-light dark:text-react-count-text-dark">{{ count|number:0 }}</span>{% endif %}
     </button>
```

### Comparing `django-reaction-system-1.0.2/reaction/templatetags/reaction_tags.py` & `django-reaction-system-1.1.0/reaction/templatetags/reaction_tags.py`

 * *Files identical despite different names*

### Comparing `django-reaction-system-1.0.2/reaction/views.py` & `django-reaction-system-1.1.0/reaction/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import json
+
 from django.contrib.auth.mixins import LoginRequiredMixin
 from django.http import HttpResponse
 from django.shortcuts import render
 from django.views import View
 
 from reaction.models import React, Reaction, UserReaction
 
@@ -18,16 +20,17 @@
             'user_react': user_react,
             'reacts': reacts
         }
         return render(request, 'reaction/reaction/reaction.html', context=context)
 
     def post(self, request, *args, **kwargs):
         user = request.user
-        reaction_urlhash = request.POST.get('urlhash', None)
-        react_slug = request.POST.get('react_slug', None)
+        data = json.loads(request.body)
+        reaction_urlhash = data.get('urlhash', None)
+        react_slug = data.get('react_slug', None)
 
         reaction = UserReaction.objects.filter(user=user, reaction__urlhash=reaction_urlhash).first()
 
         if reaction:  # Update Previous Reaction
             if reaction.react.slug == react_slug:  # Delete Previous Reaction
                 reaction.delete()
             else:  # Change Previous Reaction
```

### Comparing `django-reaction-system-1.0.2/setup.cfg` & `django-reaction-system-1.1.0/setup.cfg`

 * *Files identical despite different names*

