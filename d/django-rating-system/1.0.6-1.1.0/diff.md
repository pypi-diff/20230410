# Comparing `tmp/django-rating-system-1.0.6.tar.gz` & `tmp/django-rating-system-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-rating-system-1.0.6.tar", last modified: Mon Mar 27 19:49:54 2023, max compression
+gzip compressed data, was "django-rating-system-1.1.0.tar", last modified: Mon Apr 10 08:54:45 2023, max compression
```

## Comparing `django-rating-system-1.0.6.tar` & `django-rating-system-1.1.0.tar`

### file list

```diff
@@ -1,51 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:49:54.126343 django-rating-system-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-03-27 19:49:54.126343 django-rating-system-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:49:54.126343 django-rating-system-1.0.6/django_rating_system.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-27 19:49:54.000000 django-rating-system-1.0.6/django_rating_system.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:49:54.122343 django-rating-system-1.0.6/rating/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:49:54.122343 django-rating-system-1.0.6/rating/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/migrations/0002_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:49:54.118343 django-rating-system-1.0.6/rating/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:49:54.118343 django-rating-system-1.0.6/rating/static/rating/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:49:54.122343 django-rating-system-1.0.6/rating/static/rating/css/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/static/rating/css/style.css
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/static/rating/css/style.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:49:54.122343 django-rating-system-1.0.6/rating/static/rating/img/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/static/rating/img/heart.svg
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/static/rating/img/star.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:49:54.122343 django-rating-system-1.0.6/rating/static/rating/js/
--rw-r--r--   0 runner    (1001) docker     (123)    89574 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/static/rating/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/static/rating/js/rating.js
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/static/rating/js/rating.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:49:54.118343 django-rating-system-1.0.6/rating/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:49:54.122343 django-rating-system-1.0.6/rating/templates/rating/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:49:54.122343 django-rating-system-1.0.6/rating/templates/rating/info/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/templates/rating/info/info_base.html
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/templates/rating/info/info_extender.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:49:54.122343 django-rating-system-1.0.6/rating/templates/rating/rating/
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/templates/rating/rating/rating.html
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/templates/rating/rating/rating_info.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:49:54.126343 django-rating-system-1.0.6/rating/templates/rating/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/templates/rating/utils/IMPORTS.html
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/templates/rating/utils/SCRIPTS.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:49:54.126343 django-rating-system-1.0.6/rating/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/templatetags/rating_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/rating/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-03-27 19:49:54.126343 django-rating-system-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 19:49:49.000000 django-rating-system-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.552947 django-rating-system-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-04-10 08:54:45.552947 django-rating-system-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.552947 django-rating-system-1.1.0/django_rating_system.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-10 08:54:45.000000 django-rating-system-1.1.0/django_rating_system.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.548946 django-rating-system-1.1.0/rating/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.548946 django-rating-system-1.1.0/rating/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/migrations/0002_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.544947 django-rating-system-1.1.0/rating/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.544947 django-rating-system-1.1.0/rating/static/rating/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.548946 django-rating-system-1.1.0/rating/static/rating/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/static/rating/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/static/rating/css/style.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.548946 django-rating-system-1.1.0/rating/static/rating/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/static/rating/img/heart.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/static/rating/img/star.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.548946 django-rating-system-1.1.0/rating/static/rating/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/static/rating/js/rating.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/static/rating/js/rating.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.548946 django-rating-system-1.1.0/rating/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.548946 django-rating-system-1.1.0/rating/templates/rating/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.552947 django-rating-system-1.1.0/rating/templates/rating/info/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/templates/rating/info/info_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/templates/rating/info/info_extender.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.552947 django-rating-system-1.1.0/rating/templates/rating/rating/
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/templates/rating/rating/rating.html
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/templates/rating/rating/rating_info.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.552947 django-rating-system-1.1.0/rating/templates/rating/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/templates/rating/utils/IMPORTS.html
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/templates/rating/utils/SCRIPTS.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:45.552947 django-rating-system-1.1.0/rating/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/templatetags/rating_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/rating/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-10 08:54:45.552947 django-rating-system-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 08:54:42.000000 django-rating-system-1.1.0/setup.py
```

### Comparing `django-rating-system-1.0.6/LICENSE` & `django-rating-system-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.0.6/PKG-INFO` & `django-rating-system-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rating-system
-Version: 1.0.6
+Version: 1.1.0
 Summary: Django rating System, It can be associated with any given model.
 Home-page: https://github.com/mahyar-amiri/django-rating-system
 Author: Mahyar Amiri
 Author-email: mmaahhyyaarr@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/mahyar-amiri/django-rating-system/README.md
 Project-URL: Source Code, https://github.com/mahyar-amiri/django-rating-system
```

### Comparing `django-rating-system-1.0.6/README.md` & `django-rating-system-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 # Django Rating System
 
+<p align="center">
+  <img src="image.png" />
+</p>
+
 [![PyPI version](https://img.shields.io/pypi/v/django-rating-system.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/django-rating-system)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/django-rating-system?color=092E20&logo=django)](https://pypi.org/project/django-rating-system)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/django-rating-system?color=092E20&logo=django)](https://pypistats.org/packages/django-rating-system)
 [![GitHub](https://img.shields.io/github/license/mahyar-amiri/django-rating-system)](LICENSE)
 
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
    python -m pip install django-rating-system
```

### Comparing `django-rating-system-1.0.6/README.rst` & `django-rating-system-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.0.6/django_rating_system.egg-info/SOURCES.txt` & `django-rating-system-1.1.0/django_rating_system.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 rating/migrations/0001_initial.py
 rating/migrations/0002_config.py
 rating/migrations/__init__.py
 rating/static/rating/css/style.css
 rating/static/rating/css/style.min.css
 rating/static/rating/img/heart.svg
 rating/static/rating/img/star.svg
-rating/static/rating/js/jquery.min.js
 rating/static/rating/js/rating.js
 rating/static/rating/js/rating.min.js
 rating/templates/rating/info/info_base.html
 rating/templates/rating/info/info_extender.html
 rating/templates/rating/rating/rating.html
 rating/templates/rating/rating/rating_info.html
 rating/templates/rating/utils/IMPORTS.html
```

### Comparing `django-rating-system-1.0.6/rating/__init__.py` & `django-rating-system-1.1.0/rating/__init__.py`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.0.6/rating/admin.py` & `django-rating-system-1.1.0/rating/admin.py`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.0.6/rating/migrations/0001_initial.py` & `django-rating-system-1.1.0/rating/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.0.6/rating/migrations/0002_config.py` & `django-rating-system-1.1.0/rating/migrations/0002_config.py`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.0.6/rating/models.py` & `django-rating-system-1.1.0/rating/models.py`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.0.6/rating/static/rating/css/style.css` & `django-rating-system-1.1.0/rating/static/rating/css/style.css`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.0.6/rating/static/rating/css/style.min.css` & `django-rating-system-1.1.0/rating/static/rating/css/style.min.css`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.0.6/rating/static/rating/img/star.svg` & `django-rating-system-1.1.0/rating/static/rating/img/star.svg`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.0.6/rating/templates/rating/rating/rating.html` & `django-rating-system-1.1.0/rating/templates/rating/rating/rating.html`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.0.6/rating/templates/rating/rating/rating_info.html` & `django-rating-system-1.1.0/rating/templates/rating/rating/rating_info.html`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.0.6/rating/templatetags/rating_tags.py` & `django-rating-system-1.1.0/rating/templatetags/rating_tags.py`

 * *Files identical despite different names*

### Comparing `django-rating-system-1.0.6/rating/views.py` & `django-rating-system-1.1.0/rating/views.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,33 @@
+import json
+import math
 import statistics
 
-import math
 from django.contrib.auth.mixins import LoginRequiredMixin
 from django.contrib.contenttypes.models import ContentType
 from django.http import HttpResponse, HttpResponseBadRequest
 from django.shortcuts import render
 from django.views import View
 
 from rating.models import Rating, RatingSettings, UserRating
 
 
 class UserRatingCreate(View, LoginRequiredMixin):
     def post(self, request, *args, **kwargs):
         try:
-            app_name = request.POST.get('app_name', None)
-            model_name = request.POST.get('model_name', None)
-            object_id = request.POST.get('object_id', None)
+            data = json.loads(request.body)
+            app_name = data.get('app_name', None)
+            model_name = data.get('model_name', None)
+            object_id = data.get('object_id', None)
             content_type = ContentType.objects.get(app_label=app_name, model=model_name.lower())
-            settings_slug = request.POST.get('settings_slug', None)
+            settings_slug = data.get('settings_slug', None)
             rating_settings = RatingSettings.objects.get(slug=settings_slug)
 
             rating = Rating.objects.get_or_create(object_id=object_id, content_type=content_type, settings=rating_settings)[0]
-            rate = int(request.POST.get('rate', None))
+            rate = int(data.get('rate', None))
             if UserRating.objects.filter(user=request.user, rating=rating).exists():
                 user_rating = UserRating.objects.get(user=request.user, rating=rating)
                 if rate == -1:
                     user_rating.delete()
                 else:
                     user_rating.rate = rate / rating_settings.rates
                     user_rating.save()
```

### Comparing `django-rating-system-1.0.6/setup.cfg` & `django-rating-system-1.1.0/setup.cfg`

 * *Files identical despite different names*

