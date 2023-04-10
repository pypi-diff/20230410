# Comparing `tmp/turkle-2.7.0.tar.gz` & `tmp/turkle-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turkle-2.7.0.tar", last modified: Tue Nov  1 19:47:55 2022, max compression
+gzip compressed data, was "turkle-2.7.1.tar", last modified: Mon Apr 10 19:55:30 2023, max compression
```

## Comparing `turkle-2.7.0.tar` & `turkle-2.7.1.tar`

### file list

```diff
@@ -1,160 +1,160 @@
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.511511 turkle-2.7.0/
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1587 2022-04-21 20:58:01.000000 turkle-2.7.0/LICENSE
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)       96 2022-11-01 19:47:17.000000 turkle-2.7.0/MANIFEST.in
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1833 2022-11-01 19:47:55.511511 turkle-2.7.0/PKG-INFO
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1111 2022-04-21 20:58:01.000000 turkle-2.7.0/README.rst
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      133 2022-04-21 20:58:01.000000 turkle-2.7.0/requirements.txt
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      102 2022-11-01 19:47:55.511511 turkle-2.7.0/setup.cfg
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1255 2022-11-01 19:32:31.000000 turkle-2.7.0/setup.py
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.495511 turkle-2.7.0/turkle/
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)       73 2022-11-01 19:42:23.000000 turkle-2.7.0/turkle/__init__.py
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    60267 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/admin.py
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      158 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/apps.py
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.495511 turkle-2.7.0/turkle/management/
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)        0 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/management/__init__.py
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.495511 turkle-2.7.0/turkle/management/commands/
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)        0 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/management/commands/__init__.py
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      608 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/management/commands/expire_assignments.py
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.495511 turkle-2.7.0/turkle/migrations/
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     4597 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/migrations/0001_initial.py
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      512 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/migrations/0002_add_batch_level_permissions.py
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      472 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/migrations/0003_batch_custom_permissions.py
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      479 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/migrations/0004_batch_login_required.py
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      470 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/migrations/0005_batch_published.py
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     2660 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/migrations/0006_copy_can_work_on_permission.py
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      877 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/migrations/0007_auto_20200702_1925.py
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      447 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/migrations/0008_fix_multi_assignment_anonymous_batches.py
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      627 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/migrations/0009_batch_completed.py
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      620 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/migrations/0010_project_allotted_assignment_time.py
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     2964 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/migrations/0011_add_turkle_user_admin_group.py
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      426 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/migrations/0012_auto_20210923_1503.py
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)        0 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/migrations/__init__.py
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    35754 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/models.py
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.495511 turkle-2.7.0/turkle/static/
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.491511 turkle-2.7.0/turkle/static/admin/
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.495511 turkle-2.7.0/turkle/static/admin/css/
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      207 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/admin/css/turkle-admin-theme.css
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.495511 turkle-2.7.0/turkle/static/admin/js/
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      546 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/admin/js/turkle-admin.js
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1740 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/admin/js/turkle-file-upload.js
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      299 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/favicon-16x16.png
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      473 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/favicon-32x32.png
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.499511 turkle-2.7.0/turkle/static/turkle/
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.491511 turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.499511 turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/css/
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    37644 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-grid.css
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    98559 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-grid.css.map
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    28977 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-grid.min.css
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    68241 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-grid.min.css.map
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     4896 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-reboot.css
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    60752 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-reboot.css.map
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     4019 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-reboot.min.css
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    26084 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-reboot.min.css.map
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)   173597 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap.css
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)   430003 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap.css.map
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)   140936 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap.min.css
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)   562427 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap.min.css.map
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.503511 turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/js/
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)   212345 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.bundle.js
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)   358832 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.bundle.js.map
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    70966 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.bundle.min.js
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)   294126 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.bundle.min.js.map
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)   123765 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.js
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)   211967 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.js.map
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    51039 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.min.js
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)   176087 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.min.js.map
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.491511 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.503511 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/css/
--rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    14523 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/css/bootstrap-glyphicons.css
--rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    11830 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/css/bootstrap-glyphicons.min.css
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.491511 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.503511 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/
--rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    98620 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-brands-400.eot
--rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)   507478 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-brands-400.svg
--rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    98384 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-brands-400.ttf
--rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    63712 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-brands-400.woff
--rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    54420 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-brands-400.woff2
--rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    31156 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-regular-400.eot
--rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)   107199 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-regular-400.svg
--rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    30928 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-regular-400.ttf
--rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    14712 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-regular-400.woff
--rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    12220 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-regular-400.woff2
--rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)   102152 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-solid-900.eot
--rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)   378215 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-solid-900.svg
--rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)   101932 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-solid-900.ttf
--rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    48704 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-solid-900.woff
--rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    38784 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-solid-900.woff2
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.507511 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/glyphicons/
--rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    20127 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/glyphicons/glyphicons-halflings-regular.eot
--rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)   108738 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/glyphicons/glyphicons-halflings-regular.svg
--rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    45404 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/glyphicons/glyphicons-halflings-regular.ttf
--rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    23424 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/glyphicons/glyphicons-halflings-regular.woff
--rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    18028 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/glyphicons/glyphicons-halflings-regular.woff2
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.507511 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/maps/
--rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    51062 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/maps/glyphicons-fontawesome.css
--rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    53867 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/maps/glyphicons-fontawesome.less
--rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    42307 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/maps/glyphicons-fontawesome.min.css
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    46370 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/cal-heatmap-3.6.2.min.js
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     2131 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/cal-heatmap.css
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.507511 turkle-2.7.0/turkle/static/turkle/css/
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1472 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/css/admin-turkle.css
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1314 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/css/turkle.css
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)   151725 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/d3-3.5.17.min.js
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.507511 turkle-2.7.0/turkle/static/turkle/datatables-1.10.24/
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     5554 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/datatables-1.10.24/datatables.bootstrap4.min.css
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    91407 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/datatables-1.10.24/datatables.min.js
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    86927 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/jquery-3.3.1.min.js
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    10011 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/jquery.countdown-2.2.0.js
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    42627 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/static/turkle/parsley-2.9.1.min.js
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.491511 turkle-2.7.0/turkle/templates/
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.507511 turkle-2.7.0/turkle/templates/admin/
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1939 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/admin/base_bootcamp.html
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      814 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/admin/base_site.html
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.491511 turkle-2.7.0/turkle/templates/admin/forms/
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.507511 turkle-2.7.0/turkle/templates/admin/forms/widgets/
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      259 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/admin/forms/widgets/custom_button_file_widget.html
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.507511 turkle-2.7.0/turkle/templates/admin/turkle/
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      218 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/admin/turkle/about.html
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.507511 turkle-2.7.0/turkle/templates/admin/turkle/batch/
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1552 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/admin/turkle/batch/change_form.html
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1176 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/admin/turkle/batch/change_list.html
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     6127 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/admin/turkle/batch_stats.html
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.507511 turkle-2.7.0/turkle/templates/admin/turkle/project/
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      581 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/admin/turkle/project/change_form.html
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     7748 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/admin/turkle/project_stats.html
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     2789 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/admin/turkle/review_batch.html
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.507511 turkle-2.7.0/turkle/templates/admin/turkle/taskassignment/
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      611 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/admin/turkle/taskassignment/change_list.html
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.507511 turkle-2.7.0/turkle/templates/registration/
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      386 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/registration/form_field.html
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      363 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/registration/logged_out.html
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     2091 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/registration/login.html
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      376 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/registration/password_change_done.html
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1023 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/registration/password_change_form.html
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      459 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/registration/password_reset_complete.html
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1378 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      624 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/registration/password_reset_done.html
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      540 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/registration/password_reset_email.html
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      883 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/registration/password_reset_form.html
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.511511 turkle-2.7.0/turkle/templates/turkle/
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     2472 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/turkle/base.html
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1395 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/turkle/help.html
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     2194 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/turkle/index.html
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1264 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/turkle/preview.html
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      696 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/turkle/preview_iframe.html
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     3916 2022-11-01 15:37:28.000000 turkle-2.7.0/turkle/templates/turkle/stats.html
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     3190 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/turkle/task_assignment.html
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      704 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/turkle/task_assignment_iframe.html
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      435 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templates/turkle/task_base.html
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.511511 turkle-2.7.0/turkle/templatetags/
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)        0 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templatetags/__init__.py
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      486 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/templatetags/turkle_tags.py
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1870 2022-04-21 20:58:01.000000 turkle-2.7.0/turkle/urls.py
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      884 2022-11-01 15:37:28.000000 turkle-2.7.0/turkle/utils.py
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    23629 2022-11-01 15:50:21.000000 turkle-2.7.0/turkle/views.py
-drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2022-11-01 19:47:55.495511 turkle-2.7.0/turkle.egg-info/
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1833 2022-11-01 19:47:55.000000 turkle-2.7.0/turkle.egg-info/PKG-INFO
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     6507 2022-11-01 19:47:55.000000 turkle-2.7.0/turkle.egg-info/SOURCES.txt
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)        1 2022-11-01 19:47:55.000000 turkle-2.7.0/turkle.egg-info/dependency_links.txt
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      133 2022-11-01 19:47:55.000000 turkle-2.7.0/turkle.egg-info/requires.txt
--rw-rw-r--   0 costecj1  (1000) costecj1  (1000)        7 2022-11-01 19:47:55.000000 turkle-2.7.0/turkle.egg-info/top_level.txt
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.836316 turkle-2.7.1/
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1587 2023-04-10 13:54:30.000000 turkle-2.7.1/LICENSE
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)       96 2023-04-10 13:54:30.000000 turkle-2.7.1/MANIFEST.in
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1870 2023-04-10 19:55:30.836316 turkle-2.7.1/PKG-INFO
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1111 2023-04-10 13:54:30.000000 turkle-2.7.1/README.rst
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      133 2023-04-10 19:47:28.000000 turkle-2.7.1/requirements.txt
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      102 2023-04-10 19:55:30.836316 turkle-2.7.1/setup.cfg
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1303 2023-04-10 13:54:30.000000 turkle-2.7.1/setup.py
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.792316 turkle-2.7.1/turkle/
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)       73 2023-04-10 19:48:43.000000 turkle-2.7.1/turkle/__init__.py
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    60386 2023-04-10 19:47:43.000000 turkle-2.7.1/turkle/admin.py
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      158 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/apps.py
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.796316 turkle-2.7.1/turkle/management/
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/management/__init__.py
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.796316 turkle-2.7.1/turkle/management/commands/
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/management/commands/__init__.py
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      608 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/management/commands/expire_assignments.py
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.800316 turkle-2.7.1/turkle/migrations/
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     4597 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/migrations/0001_initial.py
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      512 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/migrations/0002_add_batch_level_permissions.py
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      472 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/migrations/0003_batch_custom_permissions.py
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      479 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/migrations/0004_batch_login_required.py
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      470 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/migrations/0005_batch_published.py
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     2660 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/migrations/0006_copy_can_work_on_permission.py
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      877 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/migrations/0007_auto_20200702_1925.py
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      447 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/migrations/0008_fix_multi_assignment_anonymous_batches.py
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      627 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/migrations/0009_batch_completed.py
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      620 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/migrations/0010_project_allotted_assignment_time.py
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     2964 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/migrations/0011_add_turkle_user_admin_group.py
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      426 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/migrations/0012_auto_20210923_1503.py
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/migrations/__init__.py
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    35754 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/models.py
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.800316 turkle-2.7.1/turkle/static/
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.788316 turkle-2.7.1/turkle/static/admin/
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.800316 turkle-2.7.1/turkle/static/admin/css/
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      207 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/admin/css/turkle-admin-theme.css
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.800316 turkle-2.7.1/turkle/static/admin/js/
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      546 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/admin/js/turkle-admin.js
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1740 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/admin/js/turkle-file-upload.js
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      299 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/favicon-16x16.png
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      473 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/favicon-32x32.png
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.804316 turkle-2.7.1/turkle/static/turkle/
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.788316 turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.808316 turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/css/
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    37644 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-grid.css
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    98559 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-grid.css.map
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    28977 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-grid.min.css
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    68241 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-grid.min.css.map
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     4896 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-reboot.css
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    60752 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-reboot.css.map
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     4019 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-reboot.min.css
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    26084 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-reboot.min.css.map
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)   173597 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap.css
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)   430003 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap.css.map
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)   140936 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap.min.css
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)   562427 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap.min.css.map
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.812316 turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/js/
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)   212345 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.bundle.js
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)   358832 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.bundle.js.map
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    70966 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.bundle.min.js
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)   294126 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.bundle.min.js.map
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)   123765 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.js
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)   211967 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.js.map
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    51039 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.min.js
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)   176087 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.min.js.map
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.788316 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.816316 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/css/
+-rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    14523 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/css/bootstrap-glyphicons.css
+-rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    11830 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/css/bootstrap-glyphicons.min.css
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.788316 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.820316 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/
+-rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    98620 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-brands-400.eot
+-rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)   507478 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-brands-400.svg
+-rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    98384 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-brands-400.ttf
+-rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    63712 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-brands-400.woff
+-rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    54420 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-brands-400.woff2
+-rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    31156 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-regular-400.eot
+-rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)   107199 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-regular-400.svg
+-rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    30928 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-regular-400.ttf
+-rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    14712 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-regular-400.woff
+-rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    12220 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-regular-400.woff2
+-rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)   102152 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-solid-900.eot
+-rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)   378215 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-solid-900.svg
+-rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)   101932 2023-04-10 13:54:30.000000 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-solid-900.ttf
+-rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    48704 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-solid-900.woff
+-rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    38784 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-solid-900.woff2
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.824316 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/glyphicons/
+-rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    20127 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/glyphicons/glyphicons-halflings-regular.eot
+-rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)   108738 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/glyphicons/glyphicons-halflings-regular.svg
+-rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    45404 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/glyphicons/glyphicons-halflings-regular.ttf
+-rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    23424 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/glyphicons/glyphicons-halflings-regular.woff
+-rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    18028 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/glyphicons/glyphicons-halflings-regular.woff2
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.824316 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/maps/
+-rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    51062 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/maps/glyphicons-fontawesome.css
+-rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    53867 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/maps/glyphicons-fontawesome.less
+-rwxrwxr-x   0 costecj1  (1000) costecj1  (1000)    42307 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/maps/glyphicons-fontawesome.min.css
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    46370 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/static/turkle/cal-heatmap-3.6.2.min.js
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     2131 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/static/turkle/cal-heatmap.css
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.824316 turkle-2.7.1/turkle/static/turkle/css/
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1472 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/static/turkle/css/admin-turkle.css
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1314 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/static/turkle/css/turkle.css
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)   151725 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/static/turkle/d3-3.5.17.min.js
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.828316 turkle-2.7.1/turkle/static/turkle/datatables-1.10.24/
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     5554 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/static/turkle/datatables-1.10.24/datatables.bootstrap4.min.css
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    91407 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/static/turkle/datatables-1.10.24/datatables.min.js
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    86927 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/static/turkle/jquery-3.3.1.min.js
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    10011 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/static/turkle/jquery.countdown-2.2.0.js
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    42627 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/static/turkle/parsley-2.9.1.min.js
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.792316 turkle-2.7.1/turkle/templates/
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.828316 turkle-2.7.1/turkle/templates/admin/
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1939 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/admin/base_bootcamp.html
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      814 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/admin/base_site.html
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.788316 turkle-2.7.1/turkle/templates/admin/forms/
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.828316 turkle-2.7.1/turkle/templates/admin/forms/widgets/
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      259 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/admin/forms/widgets/custom_button_file_widget.html
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.828316 turkle-2.7.1/turkle/templates/admin/turkle/
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      218 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/admin/turkle/about.html
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.828316 turkle-2.7.1/turkle/templates/admin/turkle/batch/
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1552 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/admin/turkle/batch/change_form.html
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1176 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/admin/turkle/batch/change_list.html
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     6127 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/admin/turkle/batch_stats.html
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.828316 turkle-2.7.1/turkle/templates/admin/turkle/project/
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      581 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/admin/turkle/project/change_form.html
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     7748 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/admin/turkle/project_stats.html
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     2789 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/admin/turkle/review_batch.html
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.828316 turkle-2.7.1/turkle/templates/admin/turkle/taskassignment/
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      611 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/admin/turkle/taskassignment/change_list.html
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.832316 turkle-2.7.1/turkle/templates/registration/
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      386 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/registration/form_field.html
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      363 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/registration/logged_out.html
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     2091 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/registration/login.html
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      376 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/registration/password_change_done.html
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1023 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/registration/password_change_form.html
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      459 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/registration/password_reset_complete.html
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1378 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/registration/password_reset_confirm.html
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      624 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/registration/password_reset_done.html
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      540 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/registration/password_reset_email.html
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      883 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/registration/password_reset_form.html
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.832316 turkle-2.7.1/turkle/templates/turkle/
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     2472 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/turkle/base.html
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1395 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/turkle/help.html
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     2194 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/turkle/index.html
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1264 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/turkle/preview.html
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      696 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/turkle/preview_iframe.html
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     3916 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/turkle/stats.html
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     3190 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/turkle/task_assignment.html
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      704 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/turkle/task_assignment_iframe.html
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      435 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templates/turkle/task_base.html
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.832316 turkle-2.7.1/turkle/templatetags/
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templatetags/__init__.py
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      486 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/templatetags/turkle_tags.py
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1870 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/urls.py
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      884 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/utils.py
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)    23629 2023-04-10 13:54:31.000000 turkle-2.7.1/turkle/views.py
+drwxrwxr-x   0 costecj1  (1000) costecj1  (1000)        0 2023-04-10 19:55:30.796316 turkle-2.7.1/turkle.egg-info/
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     1870 2023-04-10 19:55:30.000000 turkle-2.7.1/turkle.egg-info/PKG-INFO
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)     6507 2023-04-10 19:55:30.000000 turkle-2.7.1/turkle.egg-info/SOURCES.txt
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)        1 2023-04-10 19:55:30.000000 turkle-2.7.1/turkle.egg-info/dependency_links.txt
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)      133 2023-04-10 19:55:30.000000 turkle-2.7.1/turkle.egg-info/requires.txt
+-rw-rw-r--   0 costecj1  (1000) costecj1  (1000)        7 2023-04-10 19:55:30.000000 turkle-2.7.1/turkle.egg-info/top_level.txt
```

### Comparing `turkle-2.7.0/LICENSE` & `turkle-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/PKG-INFO` & `turkle-2.7.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turkle
-Version: 2.7.0
+Version: 2.7.1
 Summary: Django-based clone of Amazon's Mechanical Turk service
 Home-page: https://github.com/hltcoe/turkle
 Author: Craig Harman
 Author-email: craig@craigharman.net
 License: BSD
 Project-URL: Documentation, https://turkle.readthedocs.io/
 Keywords: annotation,crowdsourcing,mturk,mechanical turk
@@ -12,14 +12,15 @@
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Turkle
 ======
 
 Run a clone of Amazon's Mechanical **Turk** service in your **l**\ocal
 **e**\nvironment.
```

### Comparing `turkle-2.7.0/README.rst` & `turkle-2.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/setup.py` & `turkle-2.7.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     requirements = [line.strip() for line in f]
 
 setuptools.setup(
     name="turkle",
     version=ns["__version__"],
     description="Django-based clone of Amazon's Mechanical Turk service",
     long_description=long_description,
+    long_description_content_type="text/x-rst",
     url="https://github.com/hltcoe/turkle",
     project_urls={
         "Documentation": "https://turkle.readthedocs.io/",
     },
     author="Craig Harman",
     author_email="craig@craigharman.net",
     license="BSD",
```

### Comparing `turkle-2.7.0/turkle/admin.py` & `turkle-2.7.1/turkle/admin.py`

 * *Files identical despite different names*

```diff
@@ -1254,22 +1254,26 @@
     def has_change_permission(self, request, obj=None):
         return False
 
     def has_delete_permission(self, request, obj=None):
         return False
 
 
-class TaskAssignmentAdmin(ViewOnlyAdminMixin, admin.ModelAdmin):
+class TaskAssignmentAdmin(admin.ModelAdmin):
     """View for assignments to expire abandoned ones"""
 
     class Media:
         css = {
             'all': ('turkle/css/admin-turkle.css',),
         }
 
+    # this turns off the add button in admin sidebar for task assignments
+    def has_add_permission(self, request):
+        return False
+
     def changelist_view(self, request, extra_context=None):
         num_incomplete_tasks = TaskAssignment.objects.\
             filter(completed=False).\
             count()
         num_expired_tasks = TaskAssignment.objects.\
             filter(completed=False).\
             filter(expires_at__lt=timezone.now()).\
```

### Comparing `turkle-2.7.0/turkle/management/commands/expire_assignments.py` & `turkle-2.7.1/turkle/management/commands/expire_assignments.py`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/migrations/0001_initial.py` & `turkle-2.7.1/turkle/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/migrations/0002_add_batch_level_permissions.py` & `turkle-2.7.1/turkle/migrations/0002_add_batch_level_permissions.py`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/migrations/0006_copy_can_work_on_permission.py` & `turkle-2.7.1/turkle/migrations/0006_copy_can_work_on_permission.py`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/migrations/0007_auto_20200702_1925.py` & `turkle-2.7.1/turkle/migrations/0007_auto_20200702_1925.py`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/migrations/0009_batch_completed.py` & `turkle-2.7.1/turkle/migrations/0009_batch_completed.py`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/migrations/0010_project_allotted_assignment_time.py` & `turkle-2.7.1/turkle/migrations/0010_project_allotted_assignment_time.py`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/migrations/0011_add_turkle_user_admin_group.py` & `turkle-2.7.1/turkle/migrations/0011_add_turkle_user_admin_group.py`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/models.py` & `turkle-2.7.1/turkle/models.py`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/admin/js/turkle-admin.js` & `turkle-2.7.1/turkle/static/admin/js/turkle-admin.js`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/admin/js/turkle-file-upload.js` & `turkle-2.7.1/turkle/static/admin/js/turkle-file-upload.js`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-grid.css` & `turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-grid.css.map` & `turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-grid.min.css` & `turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-grid.min.css.map` & `turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-reboot.css` & `turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-reboot.css.map` & `turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-reboot.min.css` & `turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-reboot.min.css.map` & `turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap.css` & `turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap.css.map` & `turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap.min.css` & `turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap.min.css.map` & `turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.bundle.js` & `turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.bundle.js.map` & `turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.bundle.min.js` & `turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.bundle.min.js.map` & `turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.js` & `turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.js.map` & `turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.min.js` & `turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.min.js.map` & `turkle-2.7.1/turkle/static/turkle/bootstrap-4.1.3/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/css/bootstrap-glyphicons.css` & `turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/css/bootstrap-glyphicons.css`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/css/bootstrap-glyphicons.min.css` & `turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/css/bootstrap-glyphicons.min.css`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-brands-400.eot` & `turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-brands-400.svg` & `turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-brands-400.ttf` & `turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-brands-400.woff` & `turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-brands-400.woff2` & `turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-regular-400.eot` & `turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-regular-400.svg` & `turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-regular-400.ttf` & `turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-regular-400.woff` & `turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-regular-400.woff2` & `turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-solid-900.eot` & `turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-solid-900.svg` & `turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-solid-900.ttf` & `turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-solid-900.woff` & `turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-solid-900.woff2` & `turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/fontawesome/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/glyphicons/glyphicons-halflings-regular.eot` & `turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/glyphicons/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/glyphicons/glyphicons-halflings-regular.svg` & `turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/glyphicons/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/glyphicons/glyphicons-halflings-regular.ttf` & `turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/glyphicons/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/glyphicons/glyphicons-halflings-regular.woff` & `turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/glyphicons/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/fonts/glyphicons/glyphicons-halflings-regular.woff2` & `turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/fonts/glyphicons/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/maps/glyphicons-fontawesome.css` & `turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/maps/glyphicons-fontawesome.css`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/maps/glyphicons-fontawesome.less` & `turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/maps/glyphicons-fontawesome.less`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/bootstrap4-glyphicons/maps/glyphicons-fontawesome.min.css` & `turkle-2.7.1/turkle/static/turkle/bootstrap4-glyphicons/maps/glyphicons-fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/cal-heatmap-3.6.2.min.js` & `turkle-2.7.1/turkle/static/turkle/cal-heatmap-3.6.2.min.js`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/cal-heatmap.css` & `turkle-2.7.1/turkle/static/turkle/cal-heatmap.css`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/css/admin-turkle.css` & `turkle-2.7.1/turkle/static/turkle/css/admin-turkle.css`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/css/turkle.css` & `turkle-2.7.1/turkle/static/turkle/css/turkle.css`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/d3-3.5.17.min.js` & `turkle-2.7.1/turkle/static/turkle/d3-3.5.17.min.js`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/datatables-1.10.24/datatables.bootstrap4.min.css` & `turkle-2.7.1/turkle/static/turkle/datatables-1.10.24/datatables.bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/datatables-1.10.24/datatables.min.js` & `turkle-2.7.1/turkle/static/turkle/datatables-1.10.24/datatables.min.js`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/jquery-3.3.1.min.js` & `turkle-2.7.1/turkle/static/turkle/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/jquery.countdown-2.2.0.js` & `turkle-2.7.1/turkle/static/turkle/jquery.countdown-2.2.0.js`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/static/turkle/parsley-2.9.1.min.js` & `turkle-2.7.1/turkle/static/turkle/parsley-2.9.1.min.js`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/templates/admin/base_bootcamp.html` & `turkle-2.7.1/turkle/templates/admin/base_bootcamp.html`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/templates/admin/base_site.html` & `turkle-2.7.1/turkle/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/templates/admin/turkle/batch/change_form.html` & `turkle-2.7.1/turkle/templates/admin/turkle/batch/change_form.html`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/templates/admin/turkle/batch/change_list.html` & `turkle-2.7.1/turkle/templates/admin/turkle/batch/change_list.html`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/templates/admin/turkle/batch_stats.html` & `turkle-2.7.1/turkle/templates/admin/turkle/batch_stats.html`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/templates/admin/turkle/project/change_form.html` & `turkle-2.7.1/turkle/templates/admin/turkle/project/change_form.html`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/templates/admin/turkle/project_stats.html` & `turkle-2.7.1/turkle/templates/admin/turkle/project_stats.html`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/templates/admin/turkle/review_batch.html` & `turkle-2.7.1/turkle/templates/admin/turkle/review_batch.html`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/templates/admin/turkle/taskassignment/change_list.html` & `turkle-2.7.1/turkle/templates/admin/turkle/taskassignment/change_list.html`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/templates/registration/login.html` & `turkle-2.7.1/turkle/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/templates/registration/password_change_form.html` & `turkle-2.7.1/turkle/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/templates/registration/password_reset_confirm.html` & `turkle-2.7.1/turkle/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/templates/registration/password_reset_done.html` & `turkle-2.7.1/turkle/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/templates/registration/password_reset_email.html` & `turkle-2.7.1/turkle/templates/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/templates/registration/password_reset_form.html` & `turkle-2.7.1/turkle/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/templates/turkle/base.html` & `turkle-2.7.1/turkle/templates/turkle/base.html`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/templates/turkle/help.html` & `turkle-2.7.1/turkle/templates/turkle/help.html`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/templates/turkle/index.html` & `turkle-2.7.1/turkle/templates/turkle/index.html`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/templates/turkle/preview.html` & `turkle-2.7.1/turkle/templates/turkle/preview.html`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/templates/turkle/preview_iframe.html` & `turkle-2.7.1/turkle/templates/turkle/preview_iframe.html`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/templates/turkle/stats.html` & `turkle-2.7.1/turkle/templates/turkle/stats.html`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/templates/turkle/task_assignment.html` & `turkle-2.7.1/turkle/templates/turkle/task_assignment.html`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/templates/turkle/task_assignment_iframe.html` & `turkle-2.7.1/turkle/templates/turkle/task_assignment_iframe.html`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/urls.py` & `turkle-2.7.1/turkle/urls.py`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/utils.py` & `turkle-2.7.1/turkle/utils.py`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle/views.py` & `turkle-2.7.1/turkle/views.py`

 * *Files identical despite different names*

### Comparing `turkle-2.7.0/turkle.egg-info/PKG-INFO` & `turkle-2.7.1/turkle.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turkle
-Version: 2.7.0
+Version: 2.7.1
 Summary: Django-based clone of Amazon's Mechanical Turk service
 Home-page: https://github.com/hltcoe/turkle
 Author: Craig Harman
 Author-email: craig@craigharman.net
 License: BSD
 Project-URL: Documentation, https://turkle.readthedocs.io/
 Keywords: annotation,crowdsourcing,mturk,mechanical turk
@@ -12,14 +12,15 @@
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Turkle
 ======
 
 Run a clone of Amazon's Mechanical **Turk** service in your **l**\ocal
 **e**\nvironment.
```

### Comparing `turkle-2.7.0/turkle.egg-info/SOURCES.txt` & `turkle-2.7.1/turkle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

