# Comparing `tmp/Flask-BigApp-2023.1.8.4.tar.gz` & `tmp/Flask-BigApp-2023.1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-BigApp-2023.1.8.4.tar", last modified: Sun Apr  9 21:19:28 2023, max compression
+gzip compressed data, was "Flask-BigApp-2023.1.8.5.tar", last modified: Mon Apr 10 19:03:26 2023, max compression
```

## Comparing `Flask-BigApp-2023.1.8.4.tar` & `Flask-BigApp-2023.1.8.5.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-09 21:19:28.034354 Flask-BigApp-2023.1.8.4/
--rw-rw-r--   0 david     (1000) david     (1000)    25342 2022-11-24 21:56:54.000000 Flask-BigApp-2023.1.8.4/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)       60 2023-01-08 16:44:01.000000 Flask-BigApp-2023.1.8.4/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)     1701 2023-04-09 21:19:28.034354 Flask-BigApp-2023.1.8.4/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      554 2023-04-01 10:35:56.000000 Flask-BigApp-2023.1.8.4/README.md
--rw-rw-r--   0 david     (1000) david     (1000)      271 2022-09-20 09:41:33.000000 Flask-BigApp-2023.1.8.4/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)      174 2023-04-09 21:19:28.034354 Flask-BigApp-2023.1.8.4/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)     1631 2023-04-09 20:57:18.000000 Flask-BigApp-2023.1.8.4/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-09 21:19:28.026354 Flask-BigApp-2023.1.8.4/src/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-09 21:19:28.026354 Flask-BigApp-2023.1.8.4/src/Flask_BigApp.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     1701 2023-04-09 21:19:28.000000 Flask-BigApp-2023.1.8.4/src/Flask_BigApp.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     1827 2023-04-09 21:19:28.000000 Flask-BigApp-2023.1.8.4/src/Flask_BigApp.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-04-09 21:19:28.000000 Flask-BigApp-2023.1.8.4/src/Flask_BigApp.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       54 2023-04-09 21:19:28.000000 Flask-BigApp-2023.1.8.4/src/Flask_BigApp.egg-info/entry_points.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-01-08 17:03:33.000000 Flask-BigApp-2023.1.8.4/src/Flask_BigApp.egg-info/not-zip-safe
--rw-rw-r--   0 david     (1000) david     (1000)      101 2023-04-09 21:19:28.000000 Flask-BigApp-2023.1.8.4/src/Flask_BigApp.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)       30 2023-04-09 21:19:28.000000 Flask-BigApp-2023.1.8.4/src/Flask_BigApp.egg-info/top_level.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-09 21:19:28.030354 Flask-BigApp-2023.1.8.4/src/flask_bigapp/
--rw-rw-r--   0 david     (1000) david     (1000)      305 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    10308 2023-04-05 11:13:29.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp/auth.py
--rw-rw-r--   0 david     (1000) david     (1000)    11872 2023-04-05 10:53:55.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp/bigapp.py
--rw-rw-r--   0 david     (1000) david     (1000)     6465 2023-03-31 22:32:21.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp/blueprint.py
--rw-rw-r--   0 david     (1000) david     (1000)     4958 2023-04-01 16:09:06.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp/helpers.py
--rw-rw-r--   0 david     (1000) david     (1000)      916 2023-03-31 22:01:28.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp/objects.py
--rw-rw-r--   0 david     (1000) david     (1000)     1659 2023-04-01 10:10:00.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp/resources.py
--rw-rw-r--   0 david     (1000) david     (1000)     7648 2023-04-09 21:03:21.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp/security.py
--rw-rw-r--   0 david     (1000) david     (1000)     3093 2023-03-31 22:23:19.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp/utilities.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-09 21:19:28.030354 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/
--rw-rw-r--   0 david     (1000) david     (1000)       46 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-09 21:19:28.026354 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-09 21:19:28.030354 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/builtins/
--rw-rw-r--   0 david     (1000) david     (1000)      360 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/builtins/context_processors.py
--rw-rw-r--   0 david     (1000) david     (1000)      915 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-09 21:19:28.026354 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/static/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-09 21:19:28.030354 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/static/css/
--rw-rw-r--   0 david     (1000) david     (1000)       45 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/static/css/example__css.css
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-09 21:19:28.030354 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/static/img/
--rw-rw-r--   0 david     (1000) david     (1000)    28469 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-09 21:19:28.030354 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/static/js/
--rw-rw-r--   0 david     (1000) david     (1000)      119 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/static/js/example__js.js
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-09 21:19:28.026354 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-09 21:19:28.026354 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-09 21:19:28.030354 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/
--rw-rw-r--   0 david     (1000) david     (1000)      268 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/400.html
--rw-rw-r--   0 david     (1000) david     (1000)      315 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/401.html
--rw-rw-r--   0 david     (1000) david     (1000)      261 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/403.html
--rw-rw-r--   0 david     (1000) david     (1000)      281 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/404.html
--rw-rw-r--   0 david     (1000) david     (1000)      302 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/405.html
--rw-rw-r--   0 david     (1000) david     (1000)      278 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/500.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-09 21:19:28.030354 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/
--rw-rw-r--   0 david     (1000) david     (1000)      766 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-09 21:19:28.030354 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/
--rw-rw-r--   0 david     (1000) david     (1000)       13 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/footer.html
--rw-rw-r--   0 david     (1000) david     (1000)       11 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/menu.html
--rw-rw-r--   0 david     (1000) david     (1000)     9883 2023-04-01 00:04:55.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/cli.py
--rw-rw-r--   0 david     (1000) david     (1000)      992 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/resources.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-09 21:19:28.030354 Flask-BigApp-2023.1.8.4/tests/
--rw-rw-r--   0 david     (1000) david     (1000)     1592 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.4/tests/test_group.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-10 19:03:26.323540 Flask-BigApp-2023.1.8.5/
+-rw-rw-r--   0 david     (1000) david     (1000)    25342 2022-11-24 21:56:54.000000 Flask-BigApp-2023.1.8.5/LICENSE
+-rw-rw-r--   0 david     (1000) david     (1000)       60 2023-01-08 16:44:01.000000 Flask-BigApp-2023.1.8.5/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)     1701 2023-04-10 19:03:26.323540 Flask-BigApp-2023.1.8.5/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      554 2023-04-01 10:35:56.000000 Flask-BigApp-2023.1.8.5/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)      271 2023-04-10 18:03:50.000000 Flask-BigApp-2023.1.8.5/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)      174 2023-04-10 19:03:26.327540 Flask-BigApp-2023.1.8.5/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)     1631 2023-04-10 18:05:04.000000 Flask-BigApp-2023.1.8.5/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-10 19:03:26.319540 Flask-BigApp-2023.1.8.5/src/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-10 19:03:26.323540 Flask-BigApp-2023.1.8.5/src/Flask_BigApp.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     1701 2023-04-10 19:03:26.000000 Flask-BigApp-2023.1.8.5/src/Flask_BigApp.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     1851 2023-04-10 19:03:26.000000 Flask-BigApp-2023.1.8.5/src/Flask_BigApp.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-04-10 19:03:26.000000 Flask-BigApp-2023.1.8.5/src/Flask_BigApp.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       54 2023-04-10 19:03:26.000000 Flask-BigApp-2023.1.8.5/src/Flask_BigApp.egg-info/entry_points.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-01-08 17:03:33.000000 Flask-BigApp-2023.1.8.5/src/Flask_BigApp.egg-info/not-zip-safe
+-rw-rw-r--   0 david     (1000) david     (1000)      101 2023-04-10 19:03:26.000000 Flask-BigApp-2023.1.8.5/src/Flask_BigApp.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       30 2023-04-10 19:03:26.000000 Flask-BigApp-2023.1.8.5/src/Flask_BigApp.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-10 19:03:26.323540 Flask-BigApp-2023.1.8.5/src/flask_bigapp/
+-rw-rw-r--   0 david     (1000) david     (1000)      305 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10308 2023-04-05 11:13:29.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp/auth.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11872 2023-04-05 10:53:55.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp/bigapp.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6465 2023-03-31 22:32:21.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp/blueprint.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4958 2023-04-01 16:09:06.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp/helpers.py
+-rw-rw-r--   0 david     (1000) david     (1000)      916 2023-03-31 22:01:28.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp/objects.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4878 2023-04-10 19:02:07.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp/orm.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1659 2023-04-01 10:10:00.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp/resources.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7663 2023-04-09 22:17:36.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp/security.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3093 2023-03-31 22:23:19.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp/utilities.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-10 19:03:26.323540 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/
+-rw-rw-r--   0 david     (1000) david     (1000)       46 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-10 19:03:26.319540 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-10 19:03:26.323540 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/builtins/
+-rw-rw-r--   0 david     (1000) david     (1000)      360 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/builtins/context_processors.py
+-rw-rw-r--   0 david     (1000) david     (1000)      915 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-10 19:03:26.319540 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/static/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-10 19:03:26.323540 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/static/css/
+-rw-rw-r--   0 david     (1000) david     (1000)       45 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/static/css/example__css.css
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-10 19:03:26.323540 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/static/img/
+-rw-rw-r--   0 david     (1000) david     (1000)    28469 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-10 19:03:26.323540 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/static/js/
+-rw-rw-r--   0 david     (1000) david     (1000)      119 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/static/js/example__js.js
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-10 19:03:26.319540 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-10 19:03:26.319540 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-10 19:03:26.323540 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/
+-rw-rw-r--   0 david     (1000) david     (1000)      268 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/400.html
+-rw-rw-r--   0 david     (1000) david     (1000)      315 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/401.html
+-rw-rw-r--   0 david     (1000) david     (1000)      261 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/403.html
+-rw-rw-r--   0 david     (1000) david     (1000)      281 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/404.html
+-rw-rw-r--   0 david     (1000) david     (1000)      302 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/405.html
+-rw-rw-r--   0 david     (1000) david     (1000)      278 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/500.html
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-10 19:03:26.323540 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/
+-rw-rw-r--   0 david     (1000) david     (1000)      766 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-10 19:03:26.323540 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/
+-rw-rw-r--   0 david     (1000) david     (1000)       13 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/footer.html
+-rw-rw-r--   0 david     (1000) david     (1000)       11 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/menu.html
+-rw-rw-r--   0 david     (1000) david     (1000)     9883 2023-04-01 00:04:55.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/cli.py
+-rw-rw-r--   0 david     (1000) david     (1000)      992 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/resources.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-10 19:03:26.323540 Flask-BigApp-2023.1.8.5/tests/
+-rw-rw-r--   0 david     (1000) david     (1000)     1792 2023-04-10 18:58:43.000000 Flask-BigApp-2023.1.8.5/tests/test_group.py
```

### Comparing `Flask-BigApp-2023.1.8.4/LICENSE` & `Flask-BigApp-2023.1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.4/PKG-INFO` & `Flask-BigApp-2023.1.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Flask-BigApp
-Version: 2023.1.8.4
+Version: 2023.1.8.5
 Summary: A Flask auto importer that allows your Flask apps to grow big.
-Home-page: https://github.com/CheeseCake87/Flask-BigApp
+Home-page: https://github.com/Flask-Planet/Flask-BigApp
 Author: David Carmichael
 Author-email: carmichaelits@gmail.com
 License: GNU Lesser General Public License v2.1
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `Flask-BigApp-2023.1.8.4/README.md` & `Flask-BigApp-2023.1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.4/setup.py` & `Flask-BigApp-2023.1.8.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pathlib
 from setuptools import setup, find_packages
 
 readme = pathlib.Path(pathlib.Path.cwd() / "README.md").read_text()
 
 setup(
     name='Flask-BigApp',
-    version=f'2023.1.8.4',
-    url='https://github.com/CheeseCake87/Flask-BigApp',
+    version=f'2023.1.8.5',
+    url='https://github.com/Flask-Planet/Flask-BigApp',
     license='GNU Lesser General Public License v2.1',
     author='David Carmichael',
     author_email='carmichaelits@gmail.com',
     description='A Flask auto importer that allows your Flask apps to grow big.',
     long_description=f'{readme}',
     long_description_content_type='text/markdown',
     platforms='any',
```

### Comparing `Flask-BigApp-2023.1.8.4/src/Flask_BigApp.egg-info/PKG-INFO` & `Flask-BigApp-2023.1.8.5/src/Flask_BigApp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Flask-BigApp
-Version: 2023.1.8.4
+Version: 2023.1.8.5
 Summary: A Flask auto importer that allows your Flask apps to grow big.
-Home-page: https://github.com/CheeseCake87/Flask-BigApp
+Home-page: https://github.com/Flask-Planet/Flask-BigApp
 Author: David Carmichael
 Author-email: carmichaelits@gmail.com
 License: GNU Lesser General Public License v2.1
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `Flask-BigApp-2023.1.8.4/src/Flask_BigApp.egg-info/SOURCES.txt` & `Flask-BigApp-2023.1.8.5/src/Flask_BigApp.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 src/Flask_BigApp.egg-info/top_level.txt
 src/flask_bigapp/__init__.py
 src/flask_bigapp/auth.py
 src/flask_bigapp/bigapp.py
 src/flask_bigapp/blueprint.py
 src/flask_bigapp/helpers.py
 src/flask_bigapp/objects.py
+src/flask_bigapp/orm.py
 src/flask_bigapp/resources.py
 src/flask_bigapp/security.py
 src/flask_bigapp/utilities.py
 src/flask_bigapp_cli/__init__.py
 src/flask_bigapp_cli/cli.py
 src/flask_bigapp_cli/resources.py
 src/flask_bigapp_cli/__temp_theme_dir__/builtins/context_processors.py
```

### Comparing `Flask-BigApp-2023.1.8.4/src/flask_bigapp/auth.py` & `Flask-BigApp-2023.1.8.5/src/flask_bigapp/auth.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.4/src/flask_bigapp/bigapp.py` & `Flask-BigApp-2023.1.8.5/src/flask_bigapp/bigapp.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.4/src/flask_bigapp/blueprint.py` & `Flask-BigApp-2023.1.8.5/src/flask_bigapp/blueprint.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.4/src/flask_bigapp/helpers.py` & `Flask-BigApp-2023.1.8.5/src/flask_bigapp/helpers.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.4/src/flask_bigapp/objects.py` & `Flask-BigApp-2023.1.8.5/src/flask_bigapp/objects.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.4/src/flask_bigapp/resources.py` & `Flask-BigApp-2023.1.8.5/src/flask_bigapp/resources.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.4/src/flask_bigapp/security.py` & `Flask-BigApp-2023.1.8.5/src/flask_bigapp/security.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from flask import url_for
 
 
 def login_check(
         bool_session_key: str,
         endpoint_redirect: str,
         redirect_on_value: bool = False,
-        endpoint_kwargs: t.Optional[t.Dict[t.Any, t.Any]] = None,
+        endpoint_kwargs: t.Optional[t.Dict[str, t.Union[str, int]]] = None,
         message: t.Optional[str] = None,
         message_category: str = "message"
 ):
     """
     A decorator that checks if the specified session key exists, redirects to the specified endpoint if it does not
     exist or match the specified value.
 
@@ -67,15 +67,15 @@
     return login_check_wrapper
 
 
 def permission_check(
         iter_session_key: str,
         endpoint_redirect: str,
         redirect_if_no_match: t.Optional[list] = None,
-        endpoint_kwargs: t.Optional[t.Dict[t.Any, t.Any]] = None,
+        endpoint_kwargs: t.Optional[t.Dict[str, t.Union[str, int]]] = None,
         message: t.Optional[str] = None,
         message_category: str = "message"
 ):
     """
     A decorator that checks if the specified session key exists, redirects to the specified endpoint if
     the session key does not exist or if the session key does not contain the specified values.
 
@@ -84,21 +84,20 @@
     @bp.route("/admin-page", methods=["GET"])
     @login_check('logged_in', 'blueprint.login_page') <- can be mixed with login_check
     @permission_check('permissions', 'www.index', redirect_if_no_match=['admin'],
                       message="You don't have the correct permissions to view this page.")
     def admin_page():
         ...
 
-
     IF redirect_if_no_match is None, the default value of ['admin'] is set.
 
     :param iter_session_key: The session key to check for.
     :param endpoint_redirect: The endpoint to redirect to if the
-                                session key does not exist or does not contain the
-                                specified values.
+                              session key does not exist or does not contain the
+                              specified values.
     :param redirect_if_no_match: A list of values that the session key must contain.
     :param endpoint_kwargs: A dictionary of keyword arguments to pass to the redirect endpoint.
     :param message: If a message is specified, a flash message is shown.
     :param message_category: The category of the flash message.
     """
 
     if redirect_if_no_match is None:
```

### Comparing `Flask-BigApp-2023.1.8.4/src/flask_bigapp/utilities.py` & `Flask-BigApp-2023.1.8.5/src/flask_bigapp/utilities.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py` & `Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png` & `Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html` & `Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/cli.py` & `Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/cli.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.4/src/flask_bigapp_cli/resources.py` & `Flask-BigApp-2023.1.8.5/src/flask_bigapp_cli/resources.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.4/tests/test_group.py` & `Flask-BigApp-2023.1.8.5/tests/test_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,13 +42,21 @@
     """
     If this test is successful, the database has been dropped and created correctly.
     """
     response = client.get('/tests/database-creation')
     assert b"Database created." in response.data
 
 
+def test_mixin_create(client):
+    """
+    If this test is successful, the mixin is working correctly.
+    """
+    response = client.get('/tests/mixin-add')
+    assert b"MixinTest" in response.data
+
+
 def test_database_population(client):
     """
     If this test is successful, the database has been populated correctly.
     """
     response = client.get('/tests/database-population')
     assert b"David created" in response.data
```

