# Comparing `tmp/django-docrootcms-2.9.tar.gz` & `tmp/django-docrootcms-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-docrootcms-2.9.tar", last modified: Wed Mar  9 23:03:04 2022, max compression
+gzip compressed data, was "dist/django-docrootcms-3.1.tar", last modified: Mon Apr 10 19:49:58 2023, max compression
```

## Comparing `django-docrootcms-2.9.tar` & `django-docrootcms-3.1.tar`

### file list

```diff
@@ -1,207 +1,204 @@
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.160361 django-docrootcms-2.9/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1069 2020-07-05 21:56:33.000000 django-docrootcms-2.9/LICENSE
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      293 2020-10-23 20:58:04.000000 django-docrootcms-2.9/MANIFEST.in
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     9382 2022-03-09 23:03:04.160361 django-docrootcms-2.9/PKG-INFO
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     7158 2022-03-04 20:04:45.000000 django-docrootcms-2.9/README.md
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.140361 django-docrootcms-2.9/django_docrootcms.egg-info/
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     9382 2022-03-09 23:03:04.000000 django-docrootcms-2.9/django_docrootcms.egg-info/PKG-INFO
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     7770 2022-03-09 23:03:04.000000 django-docrootcms-2.9/django_docrootcms.egg-info/SOURCES.txt
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        1 2022-03-09 23:03:04.000000 django-docrootcms-2.9/django_docrootcms.egg-info/dependency_links.txt
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        1 2022-03-09 23:02:54.000000 django-docrootcms-2.9/django_docrootcms.egg-info/not-zip-safe
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        7 2022-03-09 23:03:04.000000 django-docrootcms-2.9/django_docrootcms.egg-info/requires.txt
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       11 2022-03-09 23:03:04.000000 django-docrootcms-2.9/django_docrootcms.egg-info/top_level.txt
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.144361 django-docrootcms-2.9/docrootcms/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)        0 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/__init__.py
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)       63 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/admin.py
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)       88 2021-06-21 23:06:38.000000 django-docrootcms-2.9/docrootcms/apps.py
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.144361 django-docrootcms-2.9/docrootcms/container_scripts/
--rwxr-xr-x   0 sstacha   (1001) sstacha   (1001)     2222 2020-07-06 20:45:16.000000 django-docrootcms-2.9/docrootcms/container_scripts/deploy.sh
--rwxr-xr-x   0 sstacha   (1001) sstacha   (1001)      678 2020-07-06 17:35:02.000000 django-docrootcms-2.9/docrootcms/container_scripts/docker-entrypoint.sh
--rwxrwxr-x   0 sstacha   (1001) sstacha   (1001)      946 2020-07-06 19:27:34.000000 django-docrootcms-2.9/docrootcms/container_scripts/install.sh
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.144361 django-docrootcms-2.9/docrootcms/contrib/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)        0 2020-08-30 19:02:38.000000 django-docrootcms-2.9/docrootcms/contrib/__init__.py
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.144361 django-docrootcms-2.9/docrootcms/contrib/blog/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)        0 2020-08-30 19:02:38.000000 django-docrootcms-2.9/docrootcms/contrib/blog/__init__.py
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      624 2020-08-30 19:02:38.000000 django-docrootcms-2.9/docrootcms/contrib/blog/admin.py
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      101 2021-06-22 00:14:43.000000 django-docrootcms-2.9/docrootcms/contrib/blog/apps.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       27 2020-10-02 21:45:09.000000 django-docrootcms-2.9/docrootcms/contrib/blog/forms.py
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      956 2020-08-30 19:02:38.000000 django-docrootcms-2.9/docrootcms/contrib/blog/middleware.py
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.144361 django-docrootcms-2.9/docrootcms/contrib/blog/migrations/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     5913 2021-08-12 22:10:45.000000 django-docrootcms-2.9/docrootcms/contrib/blog/migrations/0001_initial.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      800 2020-10-02 21:45:09.000000 django-docrootcms-2.9/docrootcms/contrib/blog/migrations/0002_auto_20201002_2035.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1300 2021-08-12 22:13:13.000000 django-docrootcms-2.9/docrootcms/contrib/blog/migrations/0004_bigauto_convert.py
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)        0 2020-08-30 19:02:38.000000 django-docrootcms-2.9/docrootcms/contrib/blog/migrations/__init__.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     9493 2021-08-12 22:39:57.000000 django-docrootcms-2.9/docrootcms/contrib/blog/models.py
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.140361 django-docrootcms-2.9/docrootcms/contrib/blog/templates/
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.144361 django-docrootcms-2.9/docrootcms/contrib/blog/templates/docrootcms_blog/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1211 2020-10-18 17:41:56.000000 django-docrootcms-2.9/docrootcms/contrib/blog/templates/docrootcms_blog/index.html
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      617 2020-10-18 17:43:26.000000 django-docrootcms-2.9/docrootcms/contrib/blog/templates/docrootcms_blog/post_detail.html
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.144361 django-docrootcms-2.9/docrootcms/contrib/blog/templates/markdownx/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      215 2020-08-30 19:02:38.000000 django-docrootcms-2.9/docrootcms/contrib/blog/templates/markdownx/widget.html
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.144361 django-docrootcms-2.9/docrootcms/contrib/blog/templatetags/
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.144361 django-docrootcms-2.9/docrootcms/contrib/blog/templatetags/__pycache__/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1898 2020-08-30 21:38:19.000000 django-docrootcms-2.9/docrootcms/contrib/blog/templatetags/__pycache__/conversions.cpython-38.pyc
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     2288 2020-08-30 19:02:38.000000 django-docrootcms-2.9/docrootcms/contrib/blog/templatetags/conversions.py
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)       60 2020-08-30 19:02:38.000000 django-docrootcms-2.9/docrootcms/contrib/blog/tests.py
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      350 2020-08-30 19:02:38.000000 django-docrootcms-2.9/docrootcms/contrib/blog/urls.py
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      485 2020-09-01 21:53:10.000000 django-docrootcms-2.9/docrootcms/contrib/blog/views.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     4818 2020-10-02 21:45:09.000000 django-docrootcms-2.9/docrootcms/forms.py
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.140361 django-docrootcms-2.9/docrootcms/install/
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.144361 django-docrootcms-2.9/docrootcms/install/files/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     2768 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/favicon.ico
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2993 2020-07-20 01:22:08.000000 django-docrootcms-2.9/docrootcms/install/files/favicon.svg
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.144361 django-docrootcms-2.9/docrootcms/install/files/mdb/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)   258284 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/License.pdf
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      496 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/README.txt
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)   233734 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/Useful_Resources.pdf
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.148361 django-docrootcms-2.9/docrootcms/install/files/mdb/css/
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.148361 django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     4020 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/datatables-select.min.css
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     4581 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/datatables-select.min.css.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     5629 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/datatables-select2.min.css
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     6257 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/datatables-select2.min.css.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     3831 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/datatables.min.css
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     4452 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/datatables.min.css.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     4517 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/datatables2.min.css
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     5254 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/datatables2.min.css.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      299 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/directives.min.css
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      537 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/directives.min.css.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)    18648 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/flag.min.css
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)    22366 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/flag.min.css.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1128 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/jquery.zmd.hierarchical-display.min.css
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1578 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/jquery.zmd.hierarchical-display.min.css.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      334 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/rating.min.css
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      554 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/rating.min.css.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)   198313 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/bootstrap.css
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)   160357 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/bootstrap.min.css
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)   327212 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/mdb.css
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)   249269 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/mdb.lite.css
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)   218494 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/mdb.lite.min.css
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)   249939 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/mdb.lite.min.css.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)   277022 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/mdb.min.css
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)   321252 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/mdb.min.css.map
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.148361 django-docrootcms-2.9/docrootcms/install/files/mdb/css/modules/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)    58590 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/modules/animations-extended.min.css
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)    71539 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/modules/animations-extended.min.css.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)        0 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/css/style.css
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.148361 django-docrootcms-2.9/docrootcms/install/files/mdb/img/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1150 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/img/mdb-favicon.ico
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.148361 django-docrootcms-2.9/docrootcms/install/files/mdb/img/overlays/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      211 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/img/overlays/01.png
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      213 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/img/overlays/02.png
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      209 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/img/overlays/03.png
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      211 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/img/overlays/04.png
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      213 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/img/overlays/05.png
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      211 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/img/overlays/06.png
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      215 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/img/overlays/07.png
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      146 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/img/overlays/08.png
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      137 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/img/overlays/09.png
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.152361 django-docrootcms-2.9/docrootcms/install/files/mdb/img/svg/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      215 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/img/svg/arrow_left.svg
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      214 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/img/svg/arrow_right.svg
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1864 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/index.html
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.152361 django-docrootcms-2.9/docrootcms/install/files/mdb/js/
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.156361 django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)    38807 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/datatables-select.min.js
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)   186340 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/datatables-select.min.js.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)    39368 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/datatables-select2.min.js
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)   188286 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/datatables-select2.min.js.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)   123419 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/datatables.min.js
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)   830500 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/datatables.min.js.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)   123581 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/datatables2.min.js
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)   830628 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/datatables2.min.js.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      981 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/directives.min.js
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     4647 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/directives.min.js.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      975 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/flag.min.js
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     4641 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/flag.min.js.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)    30250 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/imagesloaded.pkgd.min.js
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)   136735 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/imagesloaded.pkgd.min.js.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)    26634 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/jquery.zmd.hierarchical-display.min.js
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)   127037 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/jquery.zmd.hierarchical-display.min.js.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)    53452 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/masonry.pkgd.min.js
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)   206171 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/masonry.pkgd.min.js.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)    12189 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/rating.min.js
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)    54196 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/rating.min.js.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)   136323 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/bootstrap.js
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)    60132 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/bootstrap.min.js
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)   287629 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/jquery.js
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)    89475 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/jquery.min.js
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)   633581 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/mdb.js
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     4638 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/mdb.lite.min.js.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)   288264 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/mdb.min.js
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)  1200188 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/mdb.min.js.map
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.156361 django-docrootcms-2.9/docrootcms/install/files/mdb/js/modules/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      990 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/modules/animations-extended.min.js
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     4657 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/modules/animations-extended.min.js.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)    22101 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/modules/forms-free.min.js
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)   101119 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/modules/forms-free.min.js.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1160 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/modules/scrolling-navbar.min.js
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     5225 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/modules/scrolling-navbar.min.js.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)    12613 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/modules/treeview.min.js
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)    59670 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/modules/treeview.min.js.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)    14184 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/modules/wow.min.js
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)    61630 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/modules/wow.min.js.map
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)    87167 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/popper.js
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)    21003 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/install/files/mdb/js/popper.min.js
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      186 2020-08-18 23:59:58.000000 django-docrootcms-2.9/docrootcms/install/files/robots.txt
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      532 2020-08-18 23:59:58.000000 django-docrootcms-2.9/docrootcms/install/files/robots_staging.txt
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.156361 django-docrootcms-2.9/docrootcms/install/files/test/
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1939 2020-08-21 01:06:35.000000 django-docrootcms-2.9/docrootcms/install/files/test/index.data.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1863 2020-08-21 01:06:35.000000 django-docrootcms-2.9/docrootcms/install/files/test/index.dt
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      361 2020-08-21 01:06:35.000000 django-docrootcms-2.9/docrootcms/install/files/test/test.data.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       30 2020-08-21 01:06:35.000000 django-docrootcms-2.9/docrootcms/install/files/test/test.dt
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       12 2020-08-21 01:06:35.000000 django-docrootcms-2.9/docrootcms/install/files/test/test.txt
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      369 2020-08-21 01:06:35.000000 django-docrootcms-2.9/docrootcms/install/files/test/test_static.data.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       29 2020-08-21 01:06:35.000000 django-docrootcms-2.9/docrootcms/install/files/test/test_static.dt
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.160361 django-docrootcms-2.9/docrootcms/management/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)        0 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/management/__init__.py
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.160361 django-docrootcms-2.9/docrootcms/management/commands/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)        0 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/management/commands/__init__.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)    13003 2020-10-23 20:46:11.000000 django-docrootcms-2.9/docrootcms/management/commands/docrootcms.py
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     3684 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/management/commands/secret_key.py
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     2704 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/middleware.py
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.160361 django-docrootcms-2.9/docrootcms/migrations/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      883 2021-08-12 21:25:07.000000 django-docrootcms-2.9/docrootcms/migrations/0001_initial.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1056 2021-08-12 22:07:45.000000 django-docrootcms-2.9/docrootcms/migrations/0003_bigauto_mysql_fix.py
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)        0 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/migrations/__init__.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2274 2021-08-12 23:01:24.000000 django-docrootcms-2.9/docrootcms/models.py
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.160361 django-docrootcms-2.9/docrootcms/resources/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)        0 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/resources/__init__.py
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     5880 2020-10-02 22:27:34.000000 django-docrootcms-2.9/docrootcms/resources/docroot_settings_append.py
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      994 2020-10-02 23:43:58.000000 django-docrootcms-2.9/docrootcms/resources/docroot_urls_append.py
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.140361 django-docrootcms-2.9/docrootcms/static/
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.160361 django-docrootcms-2.9/docrootcms/static/ckeditor/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1643 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/static/ckeditor/custom_config.js
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.140361 django-docrootcms-2.9/docrootcms/static/ckeditor/plugins/
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.160361 django-docrootcms-2.9/docrootcms/static/ckeditor/plugins/usave/
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.160361 django-docrootcms-2.9/docrootcms/static/ckeditor/plugins/usave/dialogs/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1650 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/static/ckeditor/plugins/usave/dialogs/usave.js
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.160361 django-docrootcms-2.9/docrootcms/static/ckeditor/plugins/usave/icons/
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.160361 django-docrootcms-2.9/docrootcms/static/ckeditor/plugins/usave/icons/hidpi/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     3503 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/static/ckeditor/plugins/usave/icons/hidpi/usave.png
--rwxr-xr-x   0 sstacha   (1001) sstacha   (1001)     1840 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/static/ckeditor/plugins/usave/icons/loader.gif
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1136 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/static/ckeditor/plugins/usave/icons/usave.png
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1511 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/static/ckeditor/plugins/usave/icons/usave_48.png
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)    10501 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/static/ckeditor/plugins/usave/plugin.js
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.140361 django-docrootcms-2.9/docrootcms/static/markdownx/
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.160361 django-docrootcms-2.9/docrootcms/static/markdownx/js/
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)    24404 2020-10-02 21:45:09.000000 django-docrootcms-2.9/docrootcms/static/markdownx/js/markdownx.js
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)    10164 2020-10-02 21:45:09.000000 django-docrootcms-2.9/docrootcms/static/markdownx/js/markdownx.min.js
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.160361 django-docrootcms-2.9/docrootcms/templates/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1655 2020-11-08 23:14:36.000000 django-docrootcms-2.9/docrootcms/templates/_base.dt
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     3046 2020-11-06 21:14:19.000000 django-docrootcms-2.9/docrootcms/templates/_cms.dt
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      230 2020-11-06 22:48:03.000000 django-docrootcms-2.9/docrootcms/templates/_site.dt
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.160361 django-docrootcms-2.9/docrootcms/templates/admin/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1199 2020-08-30 19:02:38.000000 django-docrootcms-2.9/docrootcms/templates/admin/base_site.html
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.160361 django-docrootcms-2.9/docrootcms/templates/auth/
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)      373 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/templates/auth/login.dt
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)     8770 2020-11-06 22:48:03.000000 django-docrootcms-2.9/docrootcms/templates/page.dt
--rw-r--r--   0 sstacha   (1001) sstacha   (1001)       60 2020-07-05 21:56:33.000000 django-docrootcms-2.9/docrootcms/tests.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1293 2020-10-02 21:45:09.000000 django-docrootcms-2.9/docrootcms/urls.py
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2022-03-09 23:03:04.160361 django-docrootcms-2.9/docrootcms/utils/
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        0 2022-03-04 01:18:04.000000 django-docrootcms-2.9/docrootcms/utils/__init__.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)    11069 2022-03-09 22:30:29.000000 django-docrootcms-2.9/docrootcms/utils/convert.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2814 2022-03-04 01:26:18.000000 django-docrootcms-2.9/docrootcms/utils/logging.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)    31131 2020-10-02 21:45:09.000000 django-docrootcms-2.9/docrootcms/views.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       38 2022-03-09 23:03:04.160361 django-docrootcms-2.9/setup.cfg
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1115 2022-03-09 23:02:29.000000 django-docrootcms-2.9/setup.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.130578 django-docrootcms-3.1/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1069 2020-07-05 21:56:33.000000 django-docrootcms-3.1/LICENSE
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      293 2020-10-23 20:58:04.000000 django-docrootcms-3.1/MANIFEST.in
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     9382 2023-04-10 19:49:58.130578 django-docrootcms-3.1/PKG-INFO
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     7158 2022-03-04 20:04:45.000000 django-docrootcms-3.1/README.md
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.102578 django-docrootcms-3.1/django_docrootcms.egg-info/
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     9382 2023-04-10 19:49:58.000000 django-docrootcms-3.1/django_docrootcms.egg-info/PKG-INFO
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     7703 2023-04-10 19:49:58.000000 django-docrootcms-3.1/django_docrootcms.egg-info/SOURCES.txt
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        1 2023-04-10 19:49:58.000000 django-docrootcms-3.1/django_docrootcms.egg-info/dependency_links.txt
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        1 2023-04-10 19:49:45.000000 django-docrootcms-3.1/django_docrootcms.egg-info/not-zip-safe
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       29 2023-04-10 19:49:58.000000 django-docrootcms-3.1/django_docrootcms.egg-info/requires.txt
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       11 2023-04-10 19:49:58.000000 django-docrootcms-3.1/django_docrootcms.egg-info/top_level.txt
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.102578 django-docrootcms-3.1/docrootcms/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)        0 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/__init__.py
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)       63 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/admin.py
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)       88 2021-06-21 23:06:38.000000 django-docrootcms-3.1/docrootcms/apps.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)    24125 2022-08-01 03:42:58.000000 django-docrootcms-3.1/docrootcms/cms.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.102578 django-docrootcms-3.1/docrootcms/container_scripts/
+-rwxr-xr-x   0 sstacha   (1001) sstacha   (1001)     2222 2020-07-06 20:45:16.000000 django-docrootcms-3.1/docrootcms/container_scripts/deploy.sh
+-rwxr-xr-x   0 sstacha   (1001) sstacha   (1001)      678 2020-07-06 17:35:02.000000 django-docrootcms-3.1/docrootcms/container_scripts/docker-entrypoint.sh
+-rwxrwxr-x   0 sstacha   (1001) sstacha   (1001)      946 2020-07-06 19:27:34.000000 django-docrootcms-3.1/docrootcms/container_scripts/install.sh
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.102578 django-docrootcms-3.1/docrootcms/contrib/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)        0 2020-08-30 19:02:38.000000 django-docrootcms-3.1/docrootcms/contrib/__init__.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.102578 django-docrootcms-3.1/docrootcms/contrib/blog/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)        0 2020-08-30 19:02:38.000000 django-docrootcms-3.1/docrootcms/contrib/blog/__init__.py
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      624 2020-08-30 19:02:38.000000 django-docrootcms-3.1/docrootcms/contrib/blog/admin.py
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      101 2021-06-22 00:14:43.000000 django-docrootcms-3.1/docrootcms/contrib/blog/apps.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       27 2020-10-02 21:45:09.000000 django-docrootcms-3.1/docrootcms/contrib/blog/forms.py
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      956 2020-08-30 19:02:38.000000 django-docrootcms-3.1/docrootcms/contrib/blog/middleware.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.106578 django-docrootcms-3.1/docrootcms/contrib/blog/migrations/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     5913 2021-08-12 22:10:45.000000 django-docrootcms-3.1/docrootcms/contrib/blog/migrations/0001_initial.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      800 2020-10-02 21:45:09.000000 django-docrootcms-3.1/docrootcms/contrib/blog/migrations/0002_auto_20201002_2035.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1300 2021-08-12 22:13:13.000000 django-docrootcms-3.1/docrootcms/contrib/blog/migrations/0004_bigauto_convert.py
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)        0 2020-08-30 19:02:38.000000 django-docrootcms-3.1/docrootcms/contrib/blog/migrations/__init__.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     9493 2021-08-12 22:39:57.000000 django-docrootcms-3.1/docrootcms/contrib/blog/models.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.098578 django-docrootcms-3.1/docrootcms/contrib/blog/templates/
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.106578 django-docrootcms-3.1/docrootcms/contrib/blog/templates/docrootcms_blog/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1211 2020-10-18 17:41:56.000000 django-docrootcms-3.1/docrootcms/contrib/blog/templates/docrootcms_blog/index.html
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      617 2020-10-18 17:43:26.000000 django-docrootcms-3.1/docrootcms/contrib/blog/templates/docrootcms_blog/post_detail.html
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.106578 django-docrootcms-3.1/docrootcms/contrib/blog/templates/markdownx/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      215 2020-08-30 19:02:38.000000 django-docrootcms-3.1/docrootcms/contrib/blog/templates/markdownx/widget.html
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.106578 django-docrootcms-3.1/docrootcms/contrib/blog/templatetags/
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.106578 django-docrootcms-3.1/docrootcms/contrib/blog/templatetags/__pycache__/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1898 2020-08-30 21:38:19.000000 django-docrootcms-3.1/docrootcms/contrib/blog/templatetags/__pycache__/conversions.cpython-38.pyc
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     2288 2020-08-30 19:02:38.000000 django-docrootcms-3.1/docrootcms/contrib/blog/templatetags/conversions.py
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)       60 2020-08-30 19:02:38.000000 django-docrootcms-3.1/docrootcms/contrib/blog/tests.py
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      350 2020-08-30 19:02:38.000000 django-docrootcms-3.1/docrootcms/contrib/blog/urls.py
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      485 2020-09-01 21:53:10.000000 django-docrootcms-3.1/docrootcms/contrib/blog/views.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     4818 2020-10-02 21:45:09.000000 django-docrootcms-3.1/docrootcms/forms.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.098578 django-docrootcms-3.1/docrootcms/install/
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.106578 django-docrootcms-3.1/docrootcms/install/files/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     2768 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/favicon.ico
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2993 2020-07-20 01:22:08.000000 django-docrootcms-3.1/docrootcms/install/files/favicon.svg
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.106578 django-docrootcms-3.1/docrootcms/install/files/mdb/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)   258284 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/License.pdf
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      496 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/README.txt
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)   233734 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/Useful_Resources.pdf
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.110578 django-docrootcms-3.1/docrootcms/install/files/mdb/css/
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.110578 django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     4020 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/datatables-select.min.css
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     4581 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/datatables-select.min.css.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     5629 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/datatables-select2.min.css
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     6257 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/datatables-select2.min.css.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     3831 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/datatables.min.css
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     4452 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/datatables.min.css.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     4517 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/datatables2.min.css
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     5254 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/datatables2.min.css.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      299 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/directives.min.css
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      537 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/directives.min.css.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)    18648 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/flag.min.css
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)    22366 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/flag.min.css.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1128 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/jquery.zmd.hierarchical-display.min.css
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1578 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/jquery.zmd.hierarchical-display.min.css.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      334 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/rating.min.css
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      554 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/rating.min.css.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)   198313 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/bootstrap.css
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)   160357 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/bootstrap.min.css
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)   327212 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/mdb.css
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)   249269 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/mdb.lite.css
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)   218494 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/mdb.lite.min.css
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)   249939 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/mdb.lite.min.css.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)   277022 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/mdb.min.css
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)   321252 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/mdb.min.css.map
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.110578 django-docrootcms-3.1/docrootcms/install/files/mdb/css/modules/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)    58590 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/modules/animations-extended.min.css
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)    71539 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/modules/animations-extended.min.css.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)        0 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/css/style.css
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.110578 django-docrootcms-3.1/docrootcms/install/files/mdb/img/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1150 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/img/mdb-favicon.ico
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.114578 django-docrootcms-3.1/docrootcms/install/files/mdb/img/overlays/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      211 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/img/overlays/01.png
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      213 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/img/overlays/02.png
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      209 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/img/overlays/03.png
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      211 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/img/overlays/04.png
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      213 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/img/overlays/05.png
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      211 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/img/overlays/06.png
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      215 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/img/overlays/07.png
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      146 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/img/overlays/08.png
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      137 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/img/overlays/09.png
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.114578 django-docrootcms-3.1/docrootcms/install/files/mdb/img/svg/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      215 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/img/svg/arrow_left.svg
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      214 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/img/svg/arrow_right.svg
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1864 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/index.html
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.118578 django-docrootcms-3.1/docrootcms/install/files/mdb/js/
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.122578 django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)    38807 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/datatables-select.min.js
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)   186340 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/datatables-select.min.js.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)    39368 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/datatables-select2.min.js
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)   188286 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/datatables-select2.min.js.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)   123419 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/datatables.min.js
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)   830500 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/datatables.min.js.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)   123581 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/datatables2.min.js
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)   830628 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/datatables2.min.js.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      981 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/directives.min.js
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     4647 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/directives.min.js.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      975 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/flag.min.js
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     4641 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/flag.min.js.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)    30250 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/imagesloaded.pkgd.min.js
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)   136735 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/imagesloaded.pkgd.min.js.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)    26634 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/jquery.zmd.hierarchical-display.min.js
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)   127037 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/jquery.zmd.hierarchical-display.min.js.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)    53452 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/masonry.pkgd.min.js
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)   206171 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/masonry.pkgd.min.js.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)    12189 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/rating.min.js
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)    54196 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/rating.min.js.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)   136323 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/bootstrap.js
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)    60132 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/bootstrap.min.js
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)   287629 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/jquery.js
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)    89475 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/jquery.min.js
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)   633581 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/mdb.js
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     4638 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/mdb.lite.min.js.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)   288264 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/mdb.min.js
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)  1200188 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/mdb.min.js.map
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.126578 django-docrootcms-3.1/docrootcms/install/files/mdb/js/modules/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      990 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/modules/animations-extended.min.js
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     4657 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/modules/animations-extended.min.js.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)    22101 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/modules/forms-free.min.js
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)   101119 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/modules/forms-free.min.js.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1160 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/modules/scrolling-navbar.min.js
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     5225 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/modules/scrolling-navbar.min.js.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)    12613 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/modules/treeview.min.js
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)    59670 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/modules/treeview.min.js.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)    14184 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/modules/wow.min.js
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)    61630 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/modules/wow.min.js.map
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)    87167 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/popper.js
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)    21003 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/install/files/mdb/js/popper.min.js
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      186 2020-08-18 23:59:58.000000 django-docrootcms-3.1/docrootcms/install/files/robots.txt
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      532 2020-08-18 23:59:58.000000 django-docrootcms-3.1/docrootcms/install/files/robots_staging.txt
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.126578 django-docrootcms-3.1/docrootcms/install/files/test/
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1939 2020-08-21 01:06:35.000000 django-docrootcms-3.1/docrootcms/install/files/test/index.data.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1863 2020-08-21 01:06:35.000000 django-docrootcms-3.1/docrootcms/install/files/test/index.dt
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      361 2020-08-21 01:06:35.000000 django-docrootcms-3.1/docrootcms/install/files/test/test.data.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       30 2020-08-21 01:06:35.000000 django-docrootcms-3.1/docrootcms/install/files/test/test.dt
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       12 2020-08-21 01:06:35.000000 django-docrootcms-3.1/docrootcms/install/files/test/test.txt
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      369 2020-08-21 01:06:35.000000 django-docrootcms-3.1/docrootcms/install/files/test/test_static.data.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       29 2020-08-21 01:06:35.000000 django-docrootcms-3.1/docrootcms/install/files/test/test_static.dt
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.126578 django-docrootcms-3.1/docrootcms/management/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)        0 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/management/__init__.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.126578 django-docrootcms-3.1/docrootcms/management/commands/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)        0 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/management/commands/__init__.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)    13003 2020-10-23 20:46:11.000000 django-docrootcms-3.1/docrootcms/management/commands/docrootcms.py
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     3684 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/management/commands/secret_key.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2737 2022-08-01 02:47:11.000000 django-docrootcms-3.1/docrootcms/middleware.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.126578 django-docrootcms-3.1/docrootcms/migrations/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      883 2021-08-12 21:25:07.000000 django-docrootcms-3.1/docrootcms/migrations/0001_initial.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1056 2021-08-12 22:07:45.000000 django-docrootcms-3.1/docrootcms/migrations/0003_bigauto_mysql_fix.py
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)        0 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/migrations/__init__.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2274 2021-08-12 23:01:24.000000 django-docrootcms-3.1/docrootcms/models.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.126578 django-docrootcms-3.1/docrootcms/resources/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)        0 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/resources/__init__.py
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     6404 2023-03-20 21:05:41.000000 django-docrootcms-3.1/docrootcms/resources/docroot_settings_append.py
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      994 2020-10-02 23:43:58.000000 django-docrootcms-3.1/docrootcms/resources/docroot_urls_append.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.098578 django-docrootcms-3.1/docrootcms/static/
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.126578 django-docrootcms-3.1/docrootcms/static/ckeditor/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1643 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/static/ckeditor/custom_config.js
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.098578 django-docrootcms-3.1/docrootcms/static/ckeditor/plugins/
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.126578 django-docrootcms-3.1/docrootcms/static/ckeditor/plugins/usave/
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.126578 django-docrootcms-3.1/docrootcms/static/ckeditor/plugins/usave/dialogs/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1650 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/static/ckeditor/plugins/usave/dialogs/usave.js
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.126578 django-docrootcms-3.1/docrootcms/static/ckeditor/plugins/usave/icons/
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.126578 django-docrootcms-3.1/docrootcms/static/ckeditor/plugins/usave/icons/hidpi/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     3503 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/static/ckeditor/plugins/usave/icons/hidpi/usave.png
+-rwxr-xr-x   0 sstacha   (1001) sstacha   (1001)     1840 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/static/ckeditor/plugins/usave/icons/loader.gif
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1136 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/static/ckeditor/plugins/usave/icons/usave.png
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1511 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/static/ckeditor/plugins/usave/icons/usave_48.png
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)    10501 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/static/ckeditor/plugins/usave/plugin.js
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.098578 django-docrootcms-3.1/docrootcms/static/markdownx/
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.130578 django-docrootcms-3.1/docrootcms/static/markdownx/js/
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)    24404 2020-10-02 21:45:09.000000 django-docrootcms-3.1/docrootcms/static/markdownx/js/markdownx.js
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)    10164 2020-10-02 21:45:09.000000 django-docrootcms-3.1/docrootcms/static/markdownx/js/markdownx.min.js
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.130578 django-docrootcms-3.1/docrootcms/templates/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1655 2020-11-08 23:14:36.000000 django-docrootcms-3.1/docrootcms/templates/_base.dt
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     3046 2020-11-06 21:14:19.000000 django-docrootcms-3.1/docrootcms/templates/_cms.dt
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      230 2020-11-06 22:48:03.000000 django-docrootcms-3.1/docrootcms/templates/_site.dt
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.130578 django-docrootcms-3.1/docrootcms/templates/admin/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     1199 2020-08-30 19:02:38.000000 django-docrootcms-3.1/docrootcms/templates/admin/base_site.html
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-10 19:49:58.130578 django-docrootcms-3.1/docrootcms/templates/auth/
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)      373 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/templates/auth/login.dt
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)     8770 2020-11-06 22:48:03.000000 django-docrootcms-3.1/docrootcms/templates/page.dt
+-rw-r--r--   0 sstacha   (1001) sstacha   (1001)       60 2020-07-05 21:56:33.000000 django-docrootcms-3.1/docrootcms/tests.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1293 2020-10-02 21:45:09.000000 django-docrootcms-3.1/docrootcms/urls.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)    16201 2022-08-01 02:38:18.000000 django-docrootcms-3.1/docrootcms/views.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       38 2023-04-10 19:49:58.130578 django-docrootcms-3.1/setup.cfg
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1150 2023-04-10 19:24:09.000000 django-docrootcms-3.1/setup.py
```

### Comparing `django-docrootcms-2.9/LICENSE` & `django-docrootcms-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/PKG-INFO` & `django-docrootcms-3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-docrootcms
-Version: 2.9
+Version: 3.1
 Summary: The missing app for developers creating and maintaining websites
 Home-page: http://github.com/sstacha/django-docrootcms
 Author: Steve Stacha
 Author-email: sstacha@gmail.com
 License: MIT
 Description: # django-docrootcms
         Docroot CMS is a django application for developers who build, manage and maintain websites.  This app takes the simplicity of working with a PHP docroot, the fun of working with Python and fully leverages the power of Django for adding website application functionality.
```

### Comparing `django-docrootcms-2.9/README.md` & `django-docrootcms-3.1/README.md`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/django_docrootcms.egg-info/PKG-INFO` & `django-docrootcms-3.1/django_docrootcms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-docrootcms
-Version: 2.9
+Version: 3.1
 Summary: The missing app for developers creating and maintaining websites
 Home-page: http://github.com/sstacha/django-docrootcms
 Author: Steve Stacha
 Author-email: sstacha@gmail.com
 License: MIT
 Description: # django-docrootcms
         Docroot CMS is a django application for developers who build, manage and maintain websites.  This app takes the simplicity of working with a PHP docroot, the fun of working with Python and fully leverages the power of Django for adding website application functionality.
```

### Comparing `django-docrootcms-2.9/django_docrootcms.egg-info/SOURCES.txt` & `django-docrootcms-3.1/django_docrootcms.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 django_docrootcms.egg-info/dependency_links.txt
 django_docrootcms.egg-info/not-zip-safe
 django_docrootcms.egg-info/requires.txt
 django_docrootcms.egg-info/top_level.txt
 docrootcms/__init__.py
 docrootcms/admin.py
 docrootcms/apps.py
+docrootcms/cms.py
 docrootcms/forms.py
 docrootcms/middleware.py
 docrootcms/models.py
 docrootcms/tests.py
 docrootcms/urls.py
 docrootcms/views.py
 docrootcms/container_scripts/deploy.sh
@@ -153,11 +154,8 @@
 docrootcms/static/markdownx/js/markdownx.js
 docrootcms/static/markdownx/js/markdownx.min.js
 docrootcms/templates/_base.dt
 docrootcms/templates/_cms.dt
 docrootcms/templates/_site.dt
 docrootcms/templates/page.dt
 docrootcms/templates/admin/base_site.html
-docrootcms/templates/auth/login.dt
-docrootcms/utils/__init__.py
-docrootcms/utils/convert.py
-docrootcms/utils/logging.py
+docrootcms/templates/auth/login.dt
```

### Comparing `django-docrootcms-2.9/docrootcms/container_scripts/deploy.sh` & `django-docrootcms-3.1/docrootcms/container_scripts/deploy.sh`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/container_scripts/docker-entrypoint.sh` & `django-docrootcms-3.1/docrootcms/container_scripts/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/container_scripts/install.sh` & `django-docrootcms-3.1/docrootcms/container_scripts/install.sh`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/contrib/blog/admin.py` & `django-docrootcms-3.1/docrootcms/contrib/blog/admin.py`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/contrib/blog/middleware.py` & `django-docrootcms-3.1/docrootcms/contrib/blog/middleware.py`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/contrib/blog/migrations/0001_initial.py` & `django-docrootcms-3.1/docrootcms/contrib/blog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/contrib/blog/migrations/0002_auto_20201002_2035.py` & `django-docrootcms-3.1/docrootcms/contrib/blog/migrations/0002_auto_20201002_2035.py`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/contrib/blog/migrations/0004_bigauto_convert.py` & `django-docrootcms-3.1/docrootcms/contrib/blog/migrations/0004_bigauto_convert.py`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/contrib/blog/models.py` & `django-docrootcms-3.1/docrootcms/contrib/blog/models.py`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/contrib/blog/templates/docrootcms_blog/index.html` & `django-docrootcms-3.1/docrootcms/contrib/blog/templates/docrootcms_blog/index.html`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/contrib/blog/templates/docrootcms_blog/post_detail.html` & `django-docrootcms-3.1/docrootcms/contrib/blog/templates/docrootcms_blog/post_detail.html`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/contrib/blog/templatetags/__pycache__/conversions.cpython-38.pyc` & `django-docrootcms-3.1/docrootcms/contrib/blog/templatetags/__pycache__/conversions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/contrib/blog/templatetags/conversions.py` & `django-docrootcms-3.1/docrootcms/contrib/blog/templatetags/conversions.py`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/forms.py` & `django-docrootcms-3.1/docrootcms/forms.py`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/favicon.ico` & `django-docrootcms-3.1/docrootcms/install/files/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/favicon.svg` & `django-docrootcms-3.1/docrootcms/install/files/favicon.svg`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/License.pdf` & `django-docrootcms-3.1/docrootcms/install/files/mdb/License.pdf`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/Useful_Resources.pdf` & `django-docrootcms-3.1/docrootcms/install/files/mdb/Useful_Resources.pdf`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/datatables-select.min.css` & `django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/datatables-select.min.css`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/datatables-select.min.css.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/datatables-select.min.css.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/datatables-select2.min.css` & `django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/datatables-select2.min.css`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/datatables-select2.min.css.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/datatables-select2.min.css.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/datatables.min.css` & `django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/datatables.min.css`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/datatables.min.css.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/datatables.min.css.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/datatables2.min.css` & `django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/datatables2.min.css`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/datatables2.min.css.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/datatables2.min.css.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/directives.min.css.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/directives.min.css.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/flag.min.css` & `django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/flag.min.css`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/flag.min.css.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/flag.min.css.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/jquery.zmd.hierarchical-display.min.css` & `django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/jquery.zmd.hierarchical-display.min.css`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/jquery.zmd.hierarchical-display.min.css.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/jquery.zmd.hierarchical-display.min.css.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/css/addons/rating.min.css.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/css/addons/rating.min.css.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/css/bootstrap.css` & `django-docrootcms-3.1/docrootcms/install/files/mdb/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/css/bootstrap.min.css` & `django-docrootcms-3.1/docrootcms/install/files/mdb/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/css/mdb.css` & `django-docrootcms-3.1/docrootcms/install/files/mdb/css/mdb.css`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/css/mdb.lite.css` & `django-docrootcms-3.1/docrootcms/install/files/mdb/css/mdb.lite.css`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/css/mdb.lite.min.css` & `django-docrootcms-3.1/docrootcms/install/files/mdb/css/mdb.lite.min.css`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/css/mdb.lite.min.css.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/css/mdb.lite.min.css.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/css/mdb.min.css` & `django-docrootcms-3.1/docrootcms/install/files/mdb/css/mdb.min.css`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/css/mdb.min.css.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/css/mdb.min.css.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/css/modules/animations-extended.min.css` & `django-docrootcms-3.1/docrootcms/install/files/mdb/css/modules/animations-extended.min.css`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/css/modules/animations-extended.min.css.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/css/modules/animations-extended.min.css.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/img/mdb-favicon.ico` & `django-docrootcms-3.1/docrootcms/install/files/mdb/img/mdb-favicon.ico`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/index.html` & `django-docrootcms-3.1/docrootcms/install/files/mdb/index.html`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/datatables-select.min.js` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/datatables-select.min.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/datatables-select.min.js.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/datatables-select.min.js.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/datatables-select2.min.js` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/datatables-select2.min.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/datatables-select2.min.js.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/datatables-select2.min.js.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/datatables.min.js` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/datatables.min.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/datatables.min.js.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/datatables.min.js.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/datatables2.min.js` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/datatables2.min.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/datatables2.min.js.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/datatables2.min.js.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/directives.min.js` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/directives.min.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/directives.min.js.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/directives.min.js.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/flag.min.js` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/flag.min.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/flag.min.js.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/flag.min.js.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/imagesloaded.pkgd.min.js` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/imagesloaded.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/imagesloaded.pkgd.min.js.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/imagesloaded.pkgd.min.js.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/jquery.zmd.hierarchical-display.min.js` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/jquery.zmd.hierarchical-display.min.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/jquery.zmd.hierarchical-display.min.js.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/jquery.zmd.hierarchical-display.min.js.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/masonry.pkgd.min.js` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/masonry.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/masonry.pkgd.min.js.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/masonry.pkgd.min.js.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/rating.min.js` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/rating.min.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/addons/rating.min.js.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/addons/rating.min.js.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/bootstrap.js` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/bootstrap.min.js` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/jquery.js` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/jquery.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/jquery.min.js` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/mdb.js` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/mdb.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/mdb.lite.min.js.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/mdb.lite.min.js.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/mdb.min.js` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/mdb.min.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/mdb.min.js.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/mdb.min.js.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/modules/animations-extended.min.js` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/modules/animations-extended.min.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/modules/animations-extended.min.js.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/modules/animations-extended.min.js.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/modules/forms-free.min.js` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/modules/forms-free.min.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/modules/forms-free.min.js.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/modules/forms-free.min.js.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/modules/scrolling-navbar.min.js` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/modules/scrolling-navbar.min.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/modules/scrolling-navbar.min.js.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/modules/scrolling-navbar.min.js.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/modules/treeview.min.js` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/modules/treeview.min.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/modules/treeview.min.js.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/modules/treeview.min.js.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/modules/wow.min.js` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/modules/wow.min.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/modules/wow.min.js.map` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/modules/wow.min.js.map`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/popper.js` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/popper.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/mdb/js/popper.min.js` & `django-docrootcms-3.1/docrootcms/install/files/mdb/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/robots_staging.txt` & `django-docrootcms-3.1/docrootcms/install/files/robots_staging.txt`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/test/index.data.py` & `django-docrootcms-3.1/docrootcms/install/files/test/index.data.py`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/install/files/test/index.dt` & `django-docrootcms-3.1/docrootcms/install/files/test/index.dt`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/management/commands/docrootcms.py` & `django-docrootcms-3.1/docrootcms/management/commands/docrootcms.py`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/management/commands/secret_key.py` & `django-docrootcms-3.1/docrootcms/management/commands/secret_key.py`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/middleware.py` & `django-docrootcms-3.1/docrootcms/middleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,22 +30,22 @@
         # code to be executed after the view/next middleware is called
         log.debug("DocrootFallbackMiddleware called: " + request.path_info)
         if response.status_code == 404:
             log.debug("got a response of 404 would have done something for: " + request.path_info)
             # will be called by apache for all 404's;
             # first attempt to load a static file (should we skip this if nginx arleady processed? DEBUG=FALSE?
 
-            # attempt to load as static file
+            # attempt to load/render as static file
             result = cms_views.static(request)
             if result:
                 log.debug("result is a static file...")
                 response = result
 
             # attempt to load as template
-            if not result:
+            if not result and request.method=='GET':
                 result = cms_views.page(request)
                 if result:
                     log.debug("result is not none so returning it...")
                     response = result
 
             # attempt to load an api (determined by extension [.json, .xml etc])
             if not result:
```

### Comparing `django-docrootcms-2.9/docrootcms/migrations/0001_initial.py` & `django-docrootcms-3.1/docrootcms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/migrations/0003_bigauto_mysql_fix.py` & `django-docrootcms-3.1/docrootcms/migrations/0003_bigauto_mysql_fix.py`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/models.py` & `django-docrootcms-3.1/docrootcms/models.py`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/resources/docroot_settings_append.py` & `django-docrootcms-3.1/docrootcms/resources/docroot_settings_append.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 # ------------------------ DOCROOT CMS SETTINGS ------------------------------------
 # add our different roots for static files to be served up
 import os
+import sys
 import pathlib
 import datetime
+from ubercode.utils.logging import ColorLogger
+from ubercode.utils.environment import Environment
+
+this_module = sys.modules[__name__]
+LOG_IN_COLOR = Environment().override_variable("LOG_IN_COLOR", True)
+settings_logger = ColorLogger("django.settings", color_output=LOG_IN_COLOR)
 
 try:
     STATIC_ROOT
 except NameError:
     STATIC_ROOT = pathlib.Path(BASE_DIR, "static/")
 # IMAGES_ROOT = pathlib.Path(BASE_DIR, "images/")
 # CACHED_ROOT = pathlib.Path(BASE_DIR, "cache/")
@@ -126,18 +133,20 @@
         },
     }
 
 # SECURITY WARNING: keep the secret key used in production a secret!
 # NOTE: Recommend using a DOCROOTCMS_SECRET_KEY environment variable which will get replaced at runtime below
 # Replace any DOCROOTCMS_ prefixed environment variables in settings at startup
 # NOTE: used for docker/local machine environment variable loading overrides
-import sys
-this_module = sys.modules[__name__]
 env_prefix = "DOCROOTCMS_"
 for k, v in os.environ.items():
     if k.upper().startswith(env_prefix):
         attr_key = k[len(env_prefix):]
         if attr_key:
             # print (f"attempting to set {attr_key} to [{str(v)}]")
             setattr(this_module, attr_key, v)
 
+# by default override any database environment variables if not specified otherwise
+if not getattr(this_module, "DISABLE_DATABASES_OVERRIDE", False) and hasattr(this_module, "DATABASES"):
+    DATABASES = Environment(logger=settings_logger).override_database_variables(DATABASES)
+
 # ------------------------ DOCROOT CMS SETTINGS ------------------------------------
```

### Comparing `django-docrootcms-2.9/docrootcms/resources/docroot_urls_append.py` & `django-docrootcms-3.1/docrootcms/resources/docroot_urls_append.py`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/static/ckeditor/custom_config.js` & `django-docrootcms-3.1/docrootcms/static/ckeditor/custom_config.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/static/ckeditor/plugins/usave/dialogs/usave.js` & `django-docrootcms-3.1/docrootcms/static/ckeditor/plugins/usave/dialogs/usave.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/static/ckeditor/plugins/usave/icons/hidpi/usave.png` & `django-docrootcms-3.1/docrootcms/static/ckeditor/plugins/usave/icons/hidpi/usave.png`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/static/ckeditor/plugins/usave/icons/loader.gif` & `django-docrootcms-3.1/docrootcms/static/ckeditor/plugins/usave/icons/loader.gif`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/static/ckeditor/plugins/usave/icons/usave.png` & `django-docrootcms-3.1/docrootcms/static/ckeditor/plugins/usave/icons/usave.png`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/static/ckeditor/plugins/usave/icons/usave_48.png` & `django-docrootcms-3.1/docrootcms/static/ckeditor/plugins/usave/icons/usave_48.png`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/static/ckeditor/plugins/usave/plugin.js` & `django-docrootcms-3.1/docrootcms/static/ckeditor/plugins/usave/plugin.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/static/markdownx/js/markdownx.js` & `django-docrootcms-3.1/docrootcms/static/markdownx/js/markdownx.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/static/markdownx/js/markdownx.min.js` & `django-docrootcms-3.1/docrootcms/static/markdownx/js/markdownx.min.js`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/templates/_base.dt` & `django-docrootcms-3.1/docrootcms/templates/_base.dt`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/templates/_cms.dt` & `django-docrootcms-3.1/docrootcms/templates/_cms.dt`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/templates/admin/base_site.html` & `django-docrootcms-3.1/docrootcms/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/templates/page.dt` & `django-docrootcms-3.1/docrootcms/templates/page.dt`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/docrootcms/urls.py` & `django-docrootcms-3.1/docrootcms/urls.py`

 * *Files identical despite different names*

### Comparing `django-docrootcms-2.9/setup.py` & `django-docrootcms-3.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(name='django-docrootcms',
-      version='2.9',
+      version='3.1',
       description='The missing app for developers creating and maintaining websites',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='http://github.com/sstacha/django-docrootcms',
       author='Steve Stacha',
       author_email='sstacha@gmail.com',
       license='MIT',
@@ -24,9 +24,10 @@
         "Framework :: Django :: 3.0",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System",
         "Topic :: Internet :: WWW/HTTP :: Site Management",
       ],
       python_requires='>=3.8',
       install_requires=[
           'django',
+          'python-ubercode-utils',
       ],
 )
```

