# Comparing `tmp/dvadmin-third-4.0.0.tar.gz` & `tmp/dvadmin-third-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvadmin-third-4.0.0.tar", last modified: Fri Mar  3 10:49:21 2023, max compression
+gzip compressed data, was "dvadmin-third-4.1.0.tar", last modified: Mon Apr 10 07:42:59 2023, max compression
```

## Comparing `dvadmin-third-4.0.0.tar` & `dvadmin-third-4.1.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-03-03 10:49:21.430493 dvadmin-third-4.0.0/
--rw-rw-rw-   0        0        0       89 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     7539 2023-03-03 10:49:21.430493 dvadmin-third-4.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     6874 2023-03-02 10:37:33.000000 dvadmin-third-4.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-03 10:49:21.383492 dvadmin-third-4.0.0/dvadmin_third/
--rw-rw-rw-   0        0        0        0 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/__init__.py
--rw-rw-rw-   0        0        0       34 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/admin.py
--rw-rw-rw-   0        0        0      198 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/apps.py
-drwxrwxrwx   0        0        0        0 2023-03-03 10:49:21.401489 dvadmin-third-4.0.0/dvadmin_third/fixtures/
--rw-rw-rw-   0        0        0        0 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/fixtures/__init__.py
--rw-rw-rw-   0        0        0     1667 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/fixtures/init_menu.json
--rw-rw-rw-   0        0        0     1413 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/fixtures/init_systemconfig.json
--rw-rw-rw-   0        0        0      892 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/fixtures/initialize.py
-drwxrwxrwx   0        0        0        0 2023-03-03 10:49:21.403491 dvadmin-third-4.0.0/dvadmin_third/migrations/
--rw-rw-rw-   0        0        0     4166 2023-03-02 09:54:56.000000 dvadmin-third-4.0.0/dvadmin_third/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      377 2023-03-03 10:17:22.000000 dvadmin-third-4.0.0/dvadmin_third/migrations/0002_rename_users_thirdusers_user.py
--rw-rw-rw-   0        0        0        0 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/migrations/__init__.py
--rw-rw-rw-   0        0        0     2602 2023-03-03 10:16:53.000000 dvadmin-third-4.0.0/dvadmin_third/models.py
--rw-rw-rw-   0        0        0     9568 2023-03-03 10:40:54.000000 dvadmin-third-4.0.0/dvadmin_third/settings.py
-drwxrwxrwx   0        0        0        0 2023-03-03 10:49:21.375489 dvadmin-third-4.0.0/dvadmin_third/templates/
-drwxrwxrwx   0        0        0        0 2023-03-03 10:49:21.403491 dvadmin-third-4.0.0/dvadmin_third/templates/h5/
--rw-rw-rw-   0        0        0     2794 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/index.html
-drwxrwxrwx   0        0        0        0 2023-03-03 10:49:21.408492 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/
--rw-rw-rw-   0        0        0     4516 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/fail.png
-drwxrwxrwx   0        0        0        0 2023-03-03 10:49:21.408492 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/fonts/
--rw-rw-rw-   0        0        0    35760 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/fonts/uniicons.b6d3756e.ttf
-drwxrwxrwx   0        0        0        0 2023-03-03 10:49:21.410493 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/img/
--rw-rw-rw-   0        0        0     4516 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/img/fail.47f4b282.png
--rw-rw-rw-   0        0        0     4990 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/img/success.d46f6e83.png
--rw-rw-rw-   0        0        0    94257 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/index.2772579d.css
--rw-rw-rw-   0        0        0    96413 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/index.5841170f.css
-drwxrwxrwx   0        0        0        0 2023-03-03 10:49:21.428490 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/
--rw-rw-rw-   0        0        0   704634 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/chunk-vendors.9902d941.js
--rw-rw-rw-   0        0        0   754701 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/chunk-vendors.eca14bfe.js
--rw-rw-rw-   0        0        0   146845 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/index.5bcd04b7.js
--rw-rw-rw-   0        0        0   141283 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/index.5cbd228a.js
--rw-rw-rw-   0        0        0     1338 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-clause-privacy.08668207.js
--rw-rw-rw-   0        0        0     1328 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-clause-privacy.842421f3.js
--rw-rw-rw-   0        0        0     1356 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-clause-termsService.3c6872de.js
--rw-rw-rw-   0        0        0     1348 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-clause-termsService.f239fd83.js
--rw-rw-rw-   0        0        0     5847 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-index-index.15d69ad1.js
--rw-rw-rw-   0        0        0     5797 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-index-index.175865bd.js
--rw-rw-rw-   0        0        0    37917 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-index-index~pages-login-index~pages-scanLogin-index.0f02ccf7.js
--rw-rw-rw-   0        0        0    36983 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-index-index~pages-login-index~pages-scanLogin-index.1aa900d2.js
--rw-rw-rw-   0        0        0    22195 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-index-index~pages-scanLogin-index.0a12dd3f.js
--rw-rw-rw-   0        0        0    21757 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-index-index~pages-scanLogin-index.7c5e3417.js
--rw-rw-rw-   0        0        0    56097 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-login-index.6b42803c.js
--rw-rw-rw-   0        0        0    57597 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-login-index.ce3de6e0.js
--rw-rw-rw-   0        0        0     9109 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-loginstatus-fail.39f81373.js
--rw-rw-rw-   0        0        0     9116 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-loginstatus-invalid.1812d427.js
--rw-rw-rw-   0        0        0     9118 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-loginstatus-pastdue.4066abde.js
--rw-rw-rw-   0        0        0     9121 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-loginstatus-scanned.f6941d45.js
--rw-rw-rw-   0        0        0     9118 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-loginstatus-success.9b20fdf0.js
--rw-rw-rw-   0        0        0     4632 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-scanLogin-index.2f1946d0.js
--rw-rw-rw-   0        0        0     4557 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-scanLogin-index.9a44411b.js
--rw-rw-rw-   0        0        0    32296 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/logo.png
--rw-rw-rw-   0        0        0     4990 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/success.png
--rw-rw-rw-   0        0        0     4660 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/uni.webview.js
--rw-rw-rw-   0        0        0      667 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/urls.py
-drwxrwxrwx   0        0        0        0 2023-03-03 10:49:21.429489 dvadmin-third-4.0.0/dvadmin_third/views/
--rw-rw-rw-   0        0        0        0 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/dvadmin_third/views/__init__.py
--rw-rw-rw-   0        0        0    24358 2023-03-03 10:27:34.000000 dvadmin-third-4.0.0/dvadmin_third/views/third_users.py
-drwxrwxrwx   0        0        0        0 2023-03-03 10:49:21.398489 dvadmin-third-4.0.0/dvadmin_third.egg-info/
--rw-rw-rw-   0        0        0     7539 2023-03-03 10:49:21.000000 dvadmin-third-4.0.0/dvadmin_third.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2937 2023-03-03 10:49:21.000000 dvadmin-third-4.0.0/dvadmin_third.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-03 10:49:21.000000 dvadmin-third-4.0.0/dvadmin_third.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-03-03 10:49:21.000000 dvadmin-third-4.0.0/dvadmin_third.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-03 10:49:21.000000 dvadmin-third-4.0.0/dvadmin_third.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-02-23 03:33:01.000000 dvadmin-third-4.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-03 10:49:21.431492 dvadmin-third-4.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1348 2023-03-03 10:48:40.000000 dvadmin-third-4.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 07:42:59.554339 dvadmin-third-4.1.0/
+-rw-rw-rw-   0        0        0       89 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4641 2023-04-10 07:42:59.554339 dvadmin-third-4.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3978 2023-03-30 10:13:04.000000 dvadmin-third-4.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 07:42:59.513340 dvadmin-third-4.1.0/dvadmin_third/
+-rw-rw-rw-   0        0        0        0 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/__init__.py
+-rw-rw-rw-   0        0        0       34 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/admin.py
+-rw-rw-rw-   0        0        0      198 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-10 07:42:59.529339 dvadmin-third-4.1.0/dvadmin_third/fixtures/
+-rw-rw-rw-   0        0        0        0 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/fixtures/__init__.py
+-rw-rw-rw-   0        0        0     1667 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/fixtures/init_menu.json
+-rw-rw-rw-   0        0        0    13405 2023-03-30 10:30:18.000000 dvadmin-third-4.1.0/dvadmin_third/fixtures/init_systemconfig.json
+-rw-rw-rw-   0        0        0      892 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/fixtures/initialize.py
+drwxrwxrwx   0        0        0        0 2023-04-10 07:42:59.530341 dvadmin-third-4.1.0/dvadmin_third/migrations/
+-rw-rw-rw-   0        0        0     4166 2023-03-02 09:54:56.000000 dvadmin-third-4.1.0/dvadmin_third/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      377 2023-03-03 10:17:22.000000 dvadmin-third-4.1.0/dvadmin_third/migrations/0002_rename_users_thirdusers_user.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2631 2023-03-31 03:30:43.000000 dvadmin-third-4.1.0/dvadmin_third/models.py
+-rw-rw-rw-   0        0        0     1573 2023-03-30 10:15:02.000000 dvadmin-third-4.1.0/dvadmin_third/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-10 07:42:59.506140 dvadmin-third-4.1.0/dvadmin_third/templates/
+drwxrwxrwx   0        0        0        0 2023-04-10 07:42:59.531338 dvadmin-third-4.1.0/dvadmin_third/templates/h5/
+-rw-rw-rw-   0        0        0     2794 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/index.html
+drwxrwxrwx   0        0        0        0 2023-04-10 07:42:59.535339 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/
+-rw-rw-rw-   0        0        0     4516 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/fail.png
+drwxrwxrwx   0        0        0        0 2023-04-10 07:42:59.535339 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/fonts/
+-rw-rw-rw-   0        0        0    35760 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/fonts/uniicons.b6d3756e.ttf
+drwxrwxrwx   0        0        0        0 2023-04-10 07:42:59.536338 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/img/
+-rw-rw-rw-   0        0        0     4516 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/img/fail.47f4b282.png
+-rw-rw-rw-   0        0        0     4990 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/img/success.d46f6e83.png
+-rw-rw-rw-   0        0        0    94257 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/index.2772579d.css
+-rw-rw-rw-   0        0        0    96413 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/index.5841170f.css
+drwxrwxrwx   0        0        0        0 2023-04-10 07:42:59.552339 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/
+-rw-rw-rw-   0        0        0   704634 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/chunk-vendors.9902d941.js
+-rw-rw-rw-   0        0        0   754701 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/chunk-vendors.eca14bfe.js
+-rw-rw-rw-   0        0        0   146845 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/index.5bcd04b7.js
+-rw-rw-rw-   0        0        0   141283 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/index.5cbd228a.js
+-rw-rw-rw-   0        0        0     1338 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-clause-privacy.08668207.js
+-rw-rw-rw-   0        0        0     1328 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-clause-privacy.842421f3.js
+-rw-rw-rw-   0        0        0     1356 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-clause-termsService.3c6872de.js
+-rw-rw-rw-   0        0        0     1348 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-clause-termsService.f239fd83.js
+-rw-rw-rw-   0        0        0     5847 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-index-index.15d69ad1.js
+-rw-rw-rw-   0        0        0     5797 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-index-index.175865bd.js
+-rw-rw-rw-   0        0        0    37917 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-index-index~pages-login-index~pages-scanLogin-index.0f02ccf7.js
+-rw-rw-rw-   0        0        0    36983 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-index-index~pages-login-index~pages-scanLogin-index.1aa900d2.js
+-rw-rw-rw-   0        0        0    22195 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-index-index~pages-scanLogin-index.0a12dd3f.js
+-rw-rw-rw-   0        0        0    21757 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-index-index~pages-scanLogin-index.7c5e3417.js
+-rw-rw-rw-   0        0        0    56097 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-login-index.6b42803c.js
+-rw-rw-rw-   0        0        0    57597 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-login-index.ce3de6e0.js
+-rw-rw-rw-   0        0        0     9109 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-loginstatus-fail.39f81373.js
+-rw-rw-rw-   0        0        0     9116 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-loginstatus-invalid.1812d427.js
+-rw-rw-rw-   0        0        0     9118 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-loginstatus-pastdue.4066abde.js
+-rw-rw-rw-   0        0        0     9121 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-loginstatus-scanned.f6941d45.js
+-rw-rw-rw-   0        0        0     9118 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-loginstatus-success.9b20fdf0.js
+-rw-rw-rw-   0        0        0     4632 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-scanLogin-index.2f1946d0.js
+-rw-rw-rw-   0        0        0     4557 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-scanLogin-index.9a44411b.js
+-rw-rw-rw-   0        0        0    32296 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/logo.png
+-rw-rw-rw-   0        0        0     4990 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/success.png
+-rw-rw-rw-   0        0        0     4660 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/uni.webview.js
+-rw-rw-rw-   0        0        0      667 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-10 07:42:59.553338 dvadmin-third-4.1.0/dvadmin_third/views/
+-rw-rw-rw-   0        0        0        0 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/dvadmin_third/views/__init__.py
+-rw-rw-rw-   0        0        0    29963 2023-03-31 03:19:29.000000 dvadmin-third-4.1.0/dvadmin_third/views/third_users.py
+drwxrwxrwx   0        0        0        0 2023-04-10 07:42:59.527338 dvadmin-third-4.1.0/dvadmin_third.egg-info/
+-rw-rw-rw-   0        0        0     4641 2023-04-10 07:42:59.000000 dvadmin-third-4.1.0/dvadmin_third.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2937 2023-04-10 07:42:59.000000 dvadmin-third-4.1.0/dvadmin_third.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 07:42:59.000000 dvadmin-third-4.1.0/dvadmin_third.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-10 07:42:59.000000 dvadmin-third-4.1.0/dvadmin_third.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-10 07:42:59.000000 dvadmin-third-4.1.0/dvadmin_third.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-02-23 03:33:01.000000 dvadmin-third-4.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-10 07:42:59.554339 dvadmin-third-4.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1348 2023-04-10 07:40:52.000000 dvadmin-third-4.1.0/setup.py
```

### Comparing `dvadmin-third-4.0.0/dvadmin_third/fixtures/init_menu.json` & `dvadmin-third-4.1.0/dvadmin_third/fixtures/init_menu.json`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/fixtures/initialize.py` & `dvadmin-third-4.1.0/dvadmin_third/fixtures/initialize.py`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/migrations/0001_initial.py` & `dvadmin-third-4.1.0/dvadmin_third/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/models.py` & `dvadmin-third-4.1.0/dvadmin_third/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.db import models
 
 from dvadmin.system.models import Users
-from dvadmin.utils.models import CoreModel
+from dvadmin.utils.models import CoreModel, table_prefix
 
-TABLE_PREFIX = 'third_'
+TABLE_PREFIX = table_prefix + 'third_'
 
 
 class ThirdUsers(CoreModel):
     user = models.ForeignKey(to=Users, related_name="third_user", help_text="所属用户", verbose_name="关联用户",
                               on_delete=models.CASCADE, null=True, blank=True, db_constraint=False)
     platform = models.CharField(max_length=50, default="wechat", help_text="应用平台", verbose_name="应用平台")
     open_id = models.CharField(max_length=50, help_text="open_id", verbose_name="open_id")
```

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/index.html` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/index.html`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/fail.png` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/fail.png`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/fonts/uniicons.b6d3756e.ttf` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/fonts/uniicons.b6d3756e.ttf`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/img/fail.47f4b282.png` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/img/fail.47f4b282.png`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/img/success.d46f6e83.png` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/img/success.d46f6e83.png`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/index.2772579d.css` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/index.2772579d.css`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/index.5841170f.css` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/index.5841170f.css`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/chunk-vendors.9902d941.js` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/chunk-vendors.9902d941.js`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/chunk-vendors.eca14bfe.js` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/chunk-vendors.eca14bfe.js`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/index.5bcd04b7.js` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/index.5bcd04b7.js`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/index.5cbd228a.js` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/index.5cbd228a.js`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-clause-privacy.08668207.js` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-clause-privacy.08668207.js`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-clause-privacy.842421f3.js` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-clause-privacy.842421f3.js`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-clause-termsService.3c6872de.js` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-clause-termsService.3c6872de.js`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-clause-termsService.f239fd83.js` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-clause-termsService.f239fd83.js`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-index-index.15d69ad1.js` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-index-index.15d69ad1.js`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-index-index.175865bd.js` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-index-index.175865bd.js`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-index-index~pages-login-index~pages-scanLogin-index.0f02ccf7.js` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-index-index~pages-login-index~pages-scanLogin-index.0f02ccf7.js`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-index-index~pages-login-index~pages-scanLogin-index.1aa900d2.js` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-index-index~pages-login-index~pages-scanLogin-index.1aa900d2.js`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-index-index~pages-scanLogin-index.0a12dd3f.js` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-index-index~pages-scanLogin-index.0a12dd3f.js`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-index-index~pages-scanLogin-index.7c5e3417.js` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-index-index~pages-scanLogin-index.7c5e3417.js`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-login-index.6b42803c.js` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-login-index.6b42803c.js`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-login-index.ce3de6e0.js` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-login-index.ce3de6e0.js`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-loginstatus-fail.39f81373.js` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-loginstatus-fail.39f81373.js`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-loginstatus-invalid.1812d427.js` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-loginstatus-invalid.1812d427.js`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-loginstatus-pastdue.4066abde.js` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-loginstatus-pastdue.4066abde.js`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-loginstatus-scanned.f6941d45.js` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-loginstatus-scanned.f6941d45.js`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-loginstatus-success.9b20fdf0.js` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-loginstatus-success.9b20fdf0.js`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-scanLogin-index.2f1946d0.js` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-scanLogin-index.2f1946d0.js`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/js/pages-scanLogin-index.9a44411b.js` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/js/pages-scanLogin-index.9a44411b.js`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/logo.png` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/logo.png`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/success.png` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/success.png`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/templates/h5/static/uni.webview.js` & `dvadmin-third-4.1.0/dvadmin_third/templates/h5/static/uni.webview.js`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/urls.py` & `dvadmin-third-4.1.0/dvadmin_third/urls.py`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/dvadmin_third/views/third_users.py` & `dvadmin-third-4.1.0/dvadmin_third/views/third_users.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 import mimetypes
 import os
 import traceback
 import uuid
-import socket
 import urllib.parse
 import hashlib
 from wsgiref.util import FileWrapper
 
 from pathlib import Path
 
 import requests
@@ -113,38 +112,52 @@
         # 0 无效，1 未扫，2 已扫，3 扫码完成,并返回token
         cache.set(f"third_login_uid_{login_uid}_state", 1, 12000)
         url = f"api/dvadmin_third/index/#/?t=0login_uid={login_uid}"
         login_type = int(self.request.query_params.get('login_type', 0))
         local_ip = get_local_ip()
         if login_type == 0:
             # 微信扫码登录
-            api_option = settings.THIRD_TYPE_CONFIG["wx"]
-            url = f"http://{local_ip}:{api_option['port']}/api/dvadmin_third/index/?t={login_type}#/?login_uid={login_uid}"
+            addr = dispatch.get_system_config_values("default_scan.backend_address")
+            port = dispatch.get_system_config_values("default_scan.backend_port")
+            url = f"http://{addr}:{port}/api/dvadmin_third/index/?t={login_type}#/?login_uid={login_uid}"
         elif login_type == 1:
             # 微信公众号扫码登录
-            api_option = settings.THIRD_TYPE_CONFIG["wx_official"]
+            api_option = {
+                'api': dispatch.get_system_config_values('wechat_official_scan.api'),
+                'appid': dispatch.get_system_config_values('wechat_official_scan.appid'),
+                'confirm': dispatch.get_system_config_values('wechat_official_scan.confirm'),
+                'scope': dispatch.get_system_config_values('wechat_official_scan.scope')
+            }
             url = api_option["api"].format(
                 appid=api_option["appid"],
                 redirect_uri=urllib.parse.quote(api_option["confirm"].format(local_ip=local_ip).encode('utf-8')),
                 # scope="snsapi_base",
                 # scope="snsapi_userinfo",
                 scope=api_option["scope"],
                 state=login_uid
             )
         elif login_type == 2:
             # 飞书扫码登录
-            api_option = settings.THIRD_TYPE_CONFIG["feishu"]
+            api_option = {
+                'api': dispatch.get_system_config_values('feishu_scan.api'),
+                'appid': dispatch.get_system_config_values('feishu_scan.appid'),
+                'confirm': dispatch.get_system_config_values('feishu_scan.confirm')
+            }
             url = api_option["api"].format(
                 appid=api_option["appid"],
                 redirect_uri=urllib.parse.quote(api_option["confirm"].format(local_ip=local_ip).encode('utf-8')),
                 state=login_uid
             )
         elif login_type == 3:
             # 钉钉扫码登录
-            api_option = settings.THIRD_TYPE_CONFIG["dingtalk"]
+            api_option = {
+                'api': dispatch.get_system_config_values('dingtalk_scan.api'),
+                'appid': dispatch.get_system_config_values('dingtalk_scan.appid'),
+                'confirm': dispatch.get_system_config_values('dingtalk_scan.confirm')
+            }
             url = api_option["api"].format(
                 appid=api_option["appid"],
                 redirect_uri=urllib.parse.quote(api_option["confirm"].format(local_ip=local_ip).encode('utf-8')),
                 state=login_uid
             )
         else:
             pass
@@ -233,15 +246,38 @@
         """
         微信公众号扫码确认
         :param request:
         :return:
         """
         code = self.request.GET.get('code')
         login_uid = self.request.GET.get('state')
-        api_option = settings.THIRD_TYPE_CONFIG["wx_official"]
+        # api_option = settings.THIRD_TYPE_CONFIG["wx_official"]
+        api_option = {
+            'dev': dispatch.get_system_config_values('wechat_official_scan.dev'),
+            'uniapp_address': dispatch.get_system_config_values('wechat_official_scan.uniapp_address'),
+            'token_api': dispatch.get_system_config_values('wechat_official_scan.token_api'),
+            'appid': dispatch.get_system_config_values('wechat_official_scan.appid'),
+            'appsecret': dispatch.get_system_config_values('wechat_official_scan.appsecret'),
+            'userinfo_api': dispatch.get_system_config_values('wechat_official_scan.userinfo_api'),
+            'userinfo_lang': dispatch.get_system_config_values('wechat_official_scan.userinfo_lang'),
+            'loginStatus': {
+                'success': dispatch.get_system_config_values('loginStatus.success'),
+                'fail': dispatch.get_system_config_values('loginStatus.fail'),
+                'invalid': dispatch.get_system_config_values('loginStatus.invalid'),
+                'pastdue': dispatch.get_system_config_values('loginStatus.pastdue'),
+                'scanned': dispatch.get_system_config_values('loginStatus.scanned')
+            },
+            'loginStatusDev': {
+                'success': dispatch.get_system_config_values('loginStatusDev.success'),
+                'fail': dispatch.get_system_config_values('loginStatusDev.fail'),
+                'invalid': dispatch.get_system_config_values('loginStatusDev.invalid'),
+                'pastdue': dispatch.get_system_config_values('loginStatusDev.pastdue'),
+                'scanned': dispatch.get_system_config_values('loginStatusDev.scanned')
+            }
+        }
         login_status_url = api_option["loginStatus"]
         addr = api_option["uniapp_address"]
         if api_option["dev"]:
             login_status_url = api_option["loginStatusDev"]
 
         if not login_uid:
             return redirect(login_status_url["invalid"].format(address=addr))
@@ -341,15 +377,38 @@
         """
         飞书扫码确认
         :param request:
         :return:
         """
         code = self.request.GET.get('code')
         login_uid = self.request.GET.get('state')
-        api_option = settings.THIRD_TYPE_CONFIG["feishu"]
+        # api_option = settings.THIRD_TYPE_CONFIG["feishu"]
+        api_option = {
+            'dev': dispatch.get_system_config_values('feishu_scan.dev'),
+            'uniapp_address': dispatch.get_system_config_values('feishu_scan.uniapp_address'),
+            'token_api': dispatch.get_system_config_values('feishu_scan.token_api'),
+            'appid': dispatch.get_system_config_values('feishu_scan.appid'),
+            'appsecret': dispatch.get_system_config_values('feishu_scan.appsecret'),
+            'confirm': dispatch.get_system_config_values('feishu_scan.confirm'),
+            'userinfo_api': dispatch.get_system_config_values('feishu_scan.userinfo_api'),
+            'loginStatus': {
+                'success': dispatch.get_system_config_values('loginStatus.success'),
+                'fail': dispatch.get_system_config_values('loginStatus.fail'),
+                'invalid': dispatch.get_system_config_values('loginStatus.invalid'),
+                'pastdue': dispatch.get_system_config_values('loginStatus.pastdue'),
+                'scanned': dispatch.get_system_config_values('loginStatus.scanned')
+            },
+            'loginStatusDev': {
+                'success': dispatch.get_system_config_values('loginStatusDev.success'),
+                'fail': dispatch.get_system_config_values('loginStatusDev.fail'),
+                'invalid': dispatch.get_system_config_values('loginStatusDev.invalid'),
+                'pastdue': dispatch.get_system_config_values('loginStatusDev.pastdue'),
+                'scanned': dispatch.get_system_config_values('loginStatusDev.scanned')
+            }
+        }
         login_status_url = api_option["loginStatus"]
         addr = api_option["uniapp_address"]
         if api_option["dev"]:
             login_status_url = api_option["loginStatusDev"]
         local_ip = get_local_ip()
 
         if not login_uid:
@@ -448,20 +507,41 @@
 
     @action(methods=["GET"], detail=False, permission_classes=[])
     def dingtalk_confirm_login(self, request):
         print(self.request.GET)
         code = self.request.GET.get('authCode')
         login_uid = self.request.GET.get('state')
         error = self.request.GET.get('error', None)
-        api_option = settings.THIRD_TYPE_CONFIG["dingtalk"]
+        # api_option = settings.THIRD_TYPE_CONFIG["dingtalk"]
+        api_option = {
+            'dev': dispatch.get_system_config_values('dingtalk_scan.dev'),
+            'uniapp_address': dispatch.get_system_config_values('dingtalk_scan.uniapp_address'),
+            'token_api': dispatch.get_system_config_values('dingtalk_scan.token_api'),
+            'appid': dispatch.get_system_config_values('dingtalk_scan.appid'),
+            'appsecret': dispatch.get_system_config_values('dingtalk_scan.appsecret'),
+            'userinfo_api': dispatch.get_system_config_values('dingtalk_scan.userinfo_api'),
+            'loginStatus': {
+                'success': dispatch.get_system_config_values('loginStatus.success'),
+                'fail': dispatch.get_system_config_values('loginStatus.fail'),
+                'invalid': dispatch.get_system_config_values('loginStatus.invalid'),
+                'pastdue': dispatch.get_system_config_values('loginStatus.pastdue'),
+                'scanned': dispatch.get_system_config_values('loginStatus.scanned')
+            },
+            'loginStatusDev': {
+                'success': dispatch.get_system_config_values('loginStatusDev.success'),
+                'fail': dispatch.get_system_config_values('loginStatusDev.fail'),
+                'invalid': dispatch.get_system_config_values('loginStatusDev.invalid'),
+                'pastdue': dispatch.get_system_config_values('loginStatusDev.pastdue'),
+                'scanned': dispatch.get_system_config_values('loginStatusDev.scanned')
+            }
+        }
         login_status_url = api_option["loginStatus"]
         addr = api_option["uniapp_address"]
         if api_option["dev"]:
             login_status_url = api_option["loginStatusDev"]
-        local_ip = get_local_ip()
 
         if not login_uid:
             return redirect(login_status_url["invalid"].format(address=addr))
         login_state = cache.get(f"third_login_uid_{login_uid}_state")
         if not login_state:
             return redirect(login_status_url["pastdue"].format(address=addr))
         if login_state == 3:
@@ -520,15 +600,15 @@
                         thirduser_data = {
                             "user": user.id,
                             "platform": "dingtalk",
                             "open_id": res_json["openId"],
                             "union_id": res_json["unionId"],
                             "openname": res_json["nick"],
                             "login_ip": ip,
-                            "avatar_url": res_json["avatarUrl"]
+                            "avatar_url": res_json.get("avatarUrl", "")
                         }
                         thirduser_serializer = ThirdUsersSerializer(data=thirduser_data)
                         thirduser_serializer.is_valid(raise_exception=True)
                         thirduser_serializer.save()
 
                     # 登录记录
                     analysis_data['username'] = user.username
```

### Comparing `dvadmin-third-4.0.0/dvadmin_third.egg-info/SOURCES.txt` & `dvadmin-third-4.1.0/dvadmin_third.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvadmin-third-4.0.0/setup.py` & `dvadmin-third-4.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dvadmin-third",
-    version="4.0.0",
+    version="4.1.0",
     author="李强",
     author_email="1206709430@qq.com",
     include_package_data=True,
     description="dvadmin-third 插件是dvadmin的一个第三方用户管理插件，支持微信、企业微信、钉钉、飞书、H5页面扫码登录，支持扩展微信、企业微信、钉钉、飞书等用户信息类，以及SSO单点登录等功能(部分功能开发中)。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/huge-dream/dvadmin-third",
```

