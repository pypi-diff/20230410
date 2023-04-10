# Comparing `tmp/django-htmx-viewsets-0.0.6.tar.gz` & `tmp/django-htmx-viewsets-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-htmx-viewsets-0.0.6.tar", last modified: Sun Apr  9 08:37:49 2023, max compression
+gzip compressed data, was "django-htmx-viewsets-0.0.7.tar", last modified: Mon Apr 10 10:06:11 2023, max compression
```

## Comparing `django-htmx-viewsets-0.0.6.tar` & `django-htmx-viewsets-0.0.7.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.212925 django-htmx-viewsets-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-04-09 08:37:49.212925 django-htmx-viewsets-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-09 08:37:39.000000 django-htmx-viewsets-0.0.6/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 08:37:49.212925 django-htmx-viewsets-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.196925 django-htmx-viewsets-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.200925 django-htmx-viewsets-0.0.6/src/django_htmx_viewsets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-04-09 08:37:49.000000 django-htmx-viewsets-0.0.6/src/django_htmx_viewsets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-04-09 08:37:49.000000 django-htmx-viewsets-0.0.6/src/django_htmx_viewsets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 08:37:49.000000 django-htmx-viewsets-0.0.6/src/django_htmx_viewsets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-09 08:37:49.000000 django-htmx-viewsets-0.0.6/src/django_htmx_viewsets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-09 08:37:49.000000 django-htmx-viewsets-0.0.6/src/django_htmx_viewsets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.204925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-09 08:37:39.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)    20012 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.200925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.196925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.204925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/bootstrap/5.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)   194901 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    60404 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.196925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/datatables/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.204925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/datatables/1.13.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18721 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    87108 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.196925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.200925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.204925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/css/
--rw-r--r--   0 runner    (1001) docker     (123)   102025 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/css/all.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.208925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   187208 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   108020 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    63952 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   394628 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150124 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.200925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/htmx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.208925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/htmx/1.8.6/
--rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/htmx/1.8.6/htmx.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.200925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/jquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.208925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/jquery/3.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)    89795 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/jquery/3.6.4/jquery-3.6.4.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.200925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/select2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.208925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/select2/4.1.0-rc.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    73163 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.208925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.200925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.212925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/chart.html
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/delete.html
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/dispatch.html
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/form.html
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/full.html
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.212925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/modal/
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/modal/formset.html
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/modal.html
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/partial.html
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/table.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:49.212925 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/templatetags/htmx_viewsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-04-09 08:37:27.000000 django-htmx-viewsets-0.0.6/src/htmx_viewsets/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.794651 django-htmx-viewsets-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-04-10 10:06:11.794651 django-htmx-viewsets-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 10:06:03.000000 django-htmx-viewsets-0.0.7/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 10:06:11.794651 django-htmx-viewsets-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.770650 django-htmx-viewsets-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.778651 django-htmx-viewsets-0.0.7/src/django_htmx_viewsets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-04-10 10:06:11.000000 django-htmx-viewsets-0.0.7/src/django_htmx_viewsets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-04-10 10:06:11.000000 django-htmx-viewsets-0.0.7/src/django_htmx_viewsets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 10:06:11.000000 django-htmx-viewsets-0.0.7/src/django_htmx_viewsets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-10 10:06:11.000000 django-htmx-viewsets-0.0.7/src/django_htmx_viewsets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-10 10:06:11.000000 django-htmx-viewsets-0.0.7/src/django_htmx_viewsets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.782651 django-htmx-viewsets-0.0.7/src/htmx_viewsets/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 10:06:03.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20056 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.774650 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.774650 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.782651 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/bootstrap/5.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)   194901 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    60404 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.774650 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/datatables/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.786651 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/datatables/1.13.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18721 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    87108 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.774650 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.774650 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.786651 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   102025 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/css/all.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.790651 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   187208 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   108020 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    63952 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   394628 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150124 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.774650 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/htmx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.790651 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/htmx/1.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/htmx/1.8.6/htmx.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.774650 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.790651 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/jquery/3.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    89795 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/jquery/3.6.4/jquery-3.6.4.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.774650 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/select2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.790651 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/select2/4.1.0-rc.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    73163 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.794651 django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.774650 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.794651 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/chart.html
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/dispatch.html
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/full.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.794651 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/modal/
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/modal/formset.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/partial.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/table.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:06:11.794651 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/templatetags/htmx_viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-04-10 10:05:51.000000 django-htmx-viewsets-0.0.7/src/htmx_viewsets/viewsets.py
```

### Comparing `django-htmx-viewsets-0.0.6/LICENSE` & `django-htmx-viewsets-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/setup.py` & `django-htmx-viewsets-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/django_htmx_viewsets.egg-info/SOURCES.txt` & `django-htmx-viewsets-0.0.7/src/django_htmx_viewsets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/chart.py` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/chart.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,22 +17,23 @@
     Variance: {'hidden': True},
     StdDev: {'hidden': True},
 }
 
 
 class Dataset(dict):
     def __init__(self, field, data):
-        self.field                  = field
+        self.field = field
         self.update({
             'type': 'line',
             'label': field.verbose_name or field.name.title(),
             'data': [*data],
             'color': field.color,
             'borderColor': field.color,
             'backgroundColor': field.color,
+            'hidden': True,
         })
 
 
 class ChartDatasets:
     dataset_options = DATASET_OPTIONS
     data_fields: Iterable[ViewsetModelField]
 
@@ -56,29 +57,27 @@
         names = [field.name for field in fields]
         return queryset.values_list(*names, named=True)
 
     def get_dataset(self, field):
         return Dataset(field)
 
     def get_datasets(self):
-        for i, field in enumerate(self.data_fields):
-            data = (x[i] for x in self.values_list)
+        for field in self.data_fields:
+            data = (getattr(x, field.name) for x in self.values_list)
             yield Dataset(field, data)
 
     @property
     def labels(self):
         return self.get_labels()
 
     def get_labels(self):
         return [str(x[0]) for x in self.values_list]
 
 
 class ChartBase(ChartDatasets):
-    #label_field: Optional[str] = None
-    #data_fields: Optional[Iterable[str]] = None
     type = None  # May be set on subclass
     options = {
         'interaction': {
             'intersect': False,
             'mode': 'index',
         },
     }
```

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/color.py` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/color.py`

 * *Files 0% similar despite different names*

```diff
@@ -591,14 +591,16 @@
 
 
 class Colors:
     COLORS = [
         Color.RED1,
         Color.GREEN1,
         Color.BLUE,
+        Color.YELLOW1,
+        Color.BROWN,
     ]
     def __init__(self):
         self.code_colors = {}
         self.iterator = iter(self)
 
     def __iter__(self):
         self.i = 0
```

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/fields.py` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,24 +84,32 @@
         return str(self.name)
 
     def get_lookups(self, only_groupable=False):
         """
         only_groupable: get only lookups that can be used in group by
         """
         lookups = []
+        verbose_name = self.model_field.verbose_name
+        if only_groupable and not self.model_field.primary_key:
+            lookups.append((
+                self.name,
+                verbose_name,
+            ))
         for name, lookup in self.model_field.get_lookups().items():
             is_groupable = issubclass(lookup, models.lookups.Transform)
-            verbose_name = self.model_field.verbose_name
             if not only_groupable or is_groupable:
-                lookups.append((name, f'{verbose_name}: {lookup.__name__}'))
+                lookups.append((
+                    f'{self.name}__{name}',
+                    f'{verbose_name}: {lookup.__name__}',
+                ))
             if hasattr(lookup, 'get_lookups'):
                 for sub_name, sub_lookup in lookup.get_lookups().items():
                     is_groupable = issubclass(sub_lookup, models.lookups.Transform)
                     if not only_groupable or is_groupable:
                         lookups.append((
-                            f'{name}__{sub_name}',
-                            f'{verbose_name}: {sub_lookup.__name__}'
+                            f'{self.name}__{name}__{sub_name}',
+                            f'{verbose_name}: {sub_lookup.__name__}',
                         ))
         return lookups
 
     def get_group_by_lookups(self):
         return self.get_lookups(only_groupable=True)
```

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/forms.py` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/forms.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.css` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.js` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.css` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.css`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.js` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.js`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/css/all.min.css` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/css/all.min.css`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.ttf` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.woff2` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.ttf` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.woff2` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.ttf` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.woff2` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.ttf` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.woff2` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/htmx/1.8.6/htmx.min.js` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/htmx/1.8.6/htmx.min.js`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/jquery/3.6.4/jquery-3.6.4.min.js` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/jquery/3.6.4/jquery-3.6.4.min.js`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.css` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.css`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.js` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.js`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/action.py` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/action.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/cell.py` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/cell.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/column.py` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/column.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/row.py` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/row.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from django.db.models.base import Model
 
 __all__ = ['Row']
 
 
 class Row:
     """ this is a list of cells """
     def __init__(self, columns, instance, url_names, row_action_classes):
@@ -10,14 +11,16 @@
         self.actions = self.get_actions(row_action_classes, url_names)
         self.cells = self.get_cells(columns)
 
     def get_cells(self, columns):
         return [column.cell_class(self, column) for column in columns]
 
     def get_actions(self, action_classes, url_names):
+        if isinstance(self.instance, dict):
+            return []
         return [cls(self, url_names) for cls in action_classes]
 
     @property
     def data(self):
         return [cell.render() for cell in self.cells]
 
     def __repr__(self):
```

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/table/table.py` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/table/table.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/delete.html` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/delete.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/form.html` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/form.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/list.html` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/list.html`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
       <button class="btn btn-link text-decoration-none" type="button" data-bs-toggle="collapse" data-bs-target="#add-filter-form" aria-expanded="false" aria-controls="add-filter-form">
         &#43; Filter hinzufügen
       </button>
       <div>
         <div class="collapse" id="add-filter-form">
           <div class="card card-body w-100">
             <form id="add-filter-argument-form" method="POST" action="{{ request.path }}?{{ request.GET.urlencode }}">{% csrf_token %}
-              <table>
+              <table class="w-100">
                 {{ add_filter_form.as_table }}
                 <tr>
                   <td>
                   </td>
                   <td>
                     <button class="btn btn-primary" type="submit">Filter hinzufügen</button>
                     <button class="btn btn-secondary" type="reset">Zurücksetzen</button>
@@ -82,14 +82,18 @@
 <div class="row mt-3">
   <div class="col-12">
     <div class="table-responsive">
       {% include table %}{{ table_id }}
     </div>
   </div>
 </div>
+<style>
+  #id_x__value{width: 100%;}
+  #add-filter-argument-form .select2-container{width: 100%!important;}
+</style>
 <script>
     htmx.onLoad(function() {
       $('.modal-close-button').on('click', function () {
           $('#modal').modal('hide');
       });
     });
 	$('#id_x__type').select2({});
```

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/modal/formset.html` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/modal/formset.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/modal.html` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/modal.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/partial.html` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/partial.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/templates/htmx_viewsets/table.html` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/templates/htmx_viewsets/table.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 <table id="{{ table.table_id|safe }}" class="{{ table.table_classes|safe }}" style="{{ table.styles|safe }}">
     <thead>
         <tr>
-          {% if False and table.row_action_classes %}
-            <th></th>
-          {% endif %}
           {% for column in table.columns %}
             <th style="color: {{ column.field.color }}">{{ column }}</th>
           {% endfor %}
         </tr>
     </thead>
     {% if not table.ajax_url %}
       <tbody>
```

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/templatetags/htmx_viewsets.py` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/templatetags/htmx_viewsets.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/views.py` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,31 +52,33 @@
     select_related:     Iterable[str] = []
 
     # Later: permission_required:Iterable[Permission] = []
     #url_names:          Dict[str, str] = {}
 
     template_name:      str = 'htmx_viewsets/form.html'
     object:             models.Model
-    node_id     : str
-    viewset_class     : 'viewsets.HtmxViewSetBase'
-    viewset     : 'viewsets.HtmxViewSetBase'
+    node_id: str
+    viewset_class: 'viewsets.HtmxViewSetBase'
+    viewset: 'viewsets.HtmxViewSetBase'
     model: models.Model
     base_queryset: QuerySet
     queryset: QuerySet
 
     url_names: Dict
     url_name: str
 
     chart_class: ChartBase
 
     def __new__(cls):
         setattr(cls, 'url_names', cls.viewset_class.url_names)
         return ContextMixin.__new__(cls)
 
     def dispatch(self, request, *args, **kwargs):
+        if not self.has_permission():
+            return self.handle_no_permission()
         self.viewset = self.viewset_class(request)
         self.fields = self.get_fields()
         return super().dispatch(request, *args, **kwargs)
 
     def get_queryset(self):
         return self.viewset.get_queryset()
```

### Comparing `django-htmx-viewsets-0.0.6/src/htmx_viewsets/viewsets.py` & `django-htmx-viewsets-0.0.7/src/htmx_viewsets/viewsets.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 from .forms import (FilterForm, AddFilterForm, RemoveFilterForm,
                     GroupByForm)
 from .fields import ViewsetModelField
 from .table import Table
 from .chart import MixedChart
 from . import views
-from django.db.models.expressions import Ref
 
 
 ADDITIONAL_LOOKUPS = {
     DateTimeField: {
         'trunc_year':       TruncYear,
         'trunc_month':      TruncMonth,
         'trunc_week':       TruncWeek,
@@ -46,23 +45,23 @@
         'trunc_minute':     TruncMinute,
         'trunc_second':     TruncSecond,
     },
 }
 
 
 NUMBER_AGGREGATES = {
-    'count':    Count,
     'avg':      Avg,
     'sum':      Sum,
     'min':      Min,
     'max':      Max,
     'variance': Variance,
     'stddev':   StdDev,
 }
 
+
 AGGREGATES = {
     IntegerField: NUMBER_AGGREGATES,
     PositiveBigIntegerField: NUMBER_AGGREGATES,
     PositiveIntegerField: NUMBER_AGGREGATES,
     PositiveSmallIntegerField: NUMBER_AGGREGATES,
     SmallIntegerField: NUMBER_AGGREGATES,
     BigIntegerField: NUMBER_AGGREGATES,
@@ -76,35 +75,76 @@
     node_id:        str
     urls            : Iterable
 
     # Optional:
     master          : Optional = None
     base_template   : Optional[str] = 'htmx_viewsets/full.html'
     charts          : Iterable = []
+    permissions = {
+        'list':     ['{app_label}.view_{model_name}'],
+        'detail':   ['{app_label}.view_{model_name}'],
+        'create':   ['{app_label}.add_{model_name}'],
+        'update':   ['{app_label}.change_{model_name}'],
+        'delete':   ['{app_label}.delete_{model_name}'],
+        'table':    ['{app_label}.view_{model_name}'],
+        'chart':    ['{app_label}.view_{model_name}'],
+    }
 
     @classmethod
     def get_urls(cls):  # @NoSelf
-        return [view.url_path for view in cls.get_views()]
+        return ([view.url_path for view in cls.get_views()], cls.namespace)
 
     @classmethod
     def get_url_names(cls):
         return {code: f'{cls.namespace}:{cls.node_id}-{code}'
                 for code in cls.url_paths.keys()}
 
     @classmethod
     def get_views(cls):
         views = [cls.get_view(code, view_cls) 
                  for code, view_cls in cls.view_classes.items()]
         return views
 
     @classmethod
-    def get_view(cls, code, view_class):
-        view_kwargs = {'viewset_class': cls}
-        new_view_class = type(view_class.__name__, (view_class,), view_kwargs)
+    def format_permission(cls, perm):
+        kwargs = {
+            'app_label': cls.model._meta.app_label,
+            'model_name': cls.model._meta.model_name,
+        }
+        return perm.format(**kwargs)
+
+    @classmethod
+    def get_permissions(cls, view_class):
+        if isinstance(cls.permissions, dict):
+            perms = cls.permissions[view_class.code]
+        else:
+            perms = cls.permissions
 
+        if isinstance(perms, Iterable):
+            perms = cls.permissions
+        else:
+            perms = [perms]
+
+        return [cls.format_permission(perm) for perm in perms]
+
+    @classmethod
+    def get_view(cls, code, view_class):
+        """
+        We need to load the Permission mixin here to avoid Apps not loaded error
+        """
+        from django.contrib.auth.mixins import PermissionRequiredMixin
+        view_kwargs = {
+            'viewset_class': cls,
+            'permission_required': cls.get_permissions(view_class),
+        }
+        new_view_class = type(
+            view_class.__name__,
+            (view_class, PermissionRequiredMixin),
+            view_kwargs
+        )
         url_path = cls.url_paths[code]
         url_name = cls.url_names[code].split(':')[-1]
         setattr(
             new_view_class,
             'url_path',
             path(url_path, new_view_class.as_view(), name=url_name),
         )
@@ -137,29 +177,29 @@
     }
     additional_lookups = ADDITIONAL_LOOKUPS
     default_aggregates = AGGREGATES
     field_class = ViewsetModelField
 
     filter_form_class: Optional[forms.Form] = FilterForm
     add_filter_form_class: Optional[forms.Form] = AddFilterForm
-    #add_filter_form_class: Optional[forms.Form] = AddFilterForm
     remove_filter_form_class: Optional[forms.Form] = RemoveFilterForm
     group_by_form_class: forms.Form = GroupByForm
 
     # For Chart
     table_class = Table
     chart_class = MixedChart
 
     fields = True or []
     label_field = None
     data_fields = None
 
     base_queryset: QuerySet
     prefetch_related: Iterable[str] = None
     select_related: Iterable[str] = None
+    aggregate_count_pk = True
 
     def __init__(self, request):
         self.request = request
         self.register_lookups()
 
         # Build forms from annotated QuerySet
         self.add_filter_form = self.add_filter_form_class(
@@ -176,28 +216,27 @@
 
         qs = self.get_queryset()
         self.viewset_fields = self.get_fields(qs)
         self.chart = self.get_chart(qs, self.viewset_fields)
         self.table = self.get_table(qs, self.viewset_fields)
 
     def annotate_aggregates(self, qs):
+        if self.aggregate_count_pk:
+            qs = qs.annotate(Count('pk'))
         for field in qs.query.get_meta().fields:
             aggregates = self.default_aggregates.get(field.__class__, {})
             for name, func in aggregates.items():
                 qs = qs.annotate(**{f'{field.name}__{name}': func(field.name)})
         return qs
 
     def get_lookups(self, qs, only_groupable=False):
         viewset_fields = self.get_fields(qs)
         lookups = []
         for field in viewset_fields:
-            field_lookups = field.get_lookups(only_groupable=only_groupable)
-            for name, verbose_name in field_lookups:
-                #bla =  qs.query.get_lookup(f'{field.name}__{name}')
-                lookups.append((f'{field.name}__{name}', verbose_name))
+            lookups += field.get_lookups(only_groupable=only_groupable)
         return lookups
 
     def get_group_by_lookups(self, qs):
         return self.get_lookups(qs, only_groupable=True)
 
     def register_lookups(self):
         for field_cls, lookups in self.additional_lookups.items():
@@ -258,21 +297,16 @@
             ]
         if isinstance(self.fields, list):
             fields = [field for field in fields if field.name in self.fields]
         return fields
 
     def get_group_by_fields(self, qs):
         fields = OrderedDict()
-        if qs.query.group_by == True:
-            raise
         for expression in qs.query.group_by:
-            if isinstance(expression, Ref):
-                field = copy(expression.output_field)
-            else:
-                field = copy(expression.source_expressions[0].output_field)
+            field = copy(expression.output_field)
             name = self.group_by_form.cleaned_data['group_by']
             setattr(field, 'name', name)
             fields[name] = self.field_class(field, qs)
         return [*fields.values()]
 
     def get_aggregate_fields(self, qs):
         fields = OrderedDict()
@@ -304,24 +338,27 @@
 
     def get_table(self, qs, fields):
         table_id = f'{self.node_id}-table'
         return self.table_class(
             self.request, qs, fields, table_id, self.url_names)
 
 
-def modelviewset_factory(model=None, queryset=None, **kwargs):
-    cls = kwargs.get('viewset', HtmxModelViewSet)
+def modelviewset_factory(model=None, queryset=None, permissions=None, **kwargs):
+    cls = kwargs.get('viewset_class', HtmxModelViewSet)
     assert model or isinstance(queryset, QuerySet)
     model = model or queryset.model
     if not isinstance(queryset, QuerySet):
         queryset = model._default_manager.all()
+    perms = permissions if permissions is not None else cls.permissions
     kwargs.update({
         'model': model,
         'base_queryset': queryset,
         'node_id': model._meta.model_name,
-        'namespace': model.__module__.split('.')[0],
+        'permissions': perms,
     })
+    if 'namespace' not in kwargs:
+        kwargs['namespace'] = f'{model._meta.model_name}_viewset'
     kwargs.update(kwargs)
     cls = type(cls.__name__, (cls,), kwargs)
     setattr(cls, 'url_names', cls.get_url_names())
     setattr(cls, 'urls', cls.get_urls())
     return cls
```

