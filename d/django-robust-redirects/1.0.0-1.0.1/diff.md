# Comparing `tmp/django-robust-redirects-1.0.0.tar.gz` & `tmp/django-robust-redirects-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-robust-redirects-1.0.0.tar", last modified: Thu Apr 28 23:15:01 2022, max compression
+gzip compressed data, was "django-robust-redirects-1.0.1.tar", last modified: Mon Apr 10 16:02:11 2023, max compression
```

## Comparing `django-robust-redirects-1.0.0.tar` & `django-robust-redirects-1.0.1.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxr-xr-x   0 larrykiss   (501) staff       (20)        0 2022-04-28 23:15:01.000000 django-robust-redirects-1.0.0/
-drwxr-xr-x   0 larrykiss   (501) staff       (20)        0 2022-04-28 23:15:01.000000 django-robust-redirects-1.0.0/django_robust_redirects.egg-info/
--rw-r--r--   0 larrykiss   (501) staff       (20)      673 2022-04-28 23:15:00.000000 django-robust-redirects-1.0.0/django_robust_redirects.egg-info/PKG-INFO
--rw-r--r--   0 larrykiss   (501) staff       (20)        1 2022-04-28 23:15:00.000000 django-robust-redirects-1.0.0/django_robust_redirects.egg-info/not-zip-safe
--rw-r--r--   0 larrykiss   (501) staff       (20)     1136 2022-04-28 23:15:00.000000 django-robust-redirects-1.0.0/django_robust_redirects.egg-info/SOURCES.txt
--rw-r--r--   0 larrykiss   (501) staff       (20)       30 2022-04-28 23:15:00.000000 django-robust-redirects-1.0.0/django_robust_redirects.egg-info/requires.txt
--rw-r--r--   0 larrykiss   (501) staff       (20)       16 2022-04-28 23:15:00.000000 django-robust-redirects-1.0.0/django_robust_redirects.egg-info/top_level.txt
--rw-r--r--   0 larrykiss   (501) staff       (20)        1 2022-04-28 23:15:00.000000 django-robust-redirects-1.0.0/django_robust_redirects.egg-info/dependency_links.txt
--rw-r--r--   0 larrykiss   (501) staff       (20)      673 2022-04-28 23:15:01.000000 django-robust-redirects-1.0.0/PKG-INFO
--rw-r--r--   0 larrykiss   (501) staff       (20)      154 2021-11-23 17:18:38.000000 django-robust-redirects-1.0.0/MANIFEST.in
-drwxr-xr-x   0 larrykiss   (501) staff       (20)        0 2022-04-28 23:15:01.000000 django-robust-redirects-1.0.0/robustredirects/
--rw-r--r--   0 larrykiss   (501) staff       (20)       95 2022-04-28 23:12:43.000000 django-robust-redirects-1.0.0/robustredirects/dynamic_urls.py
-drwxr-xr-x   0 larrykiss   (501) staff       (20)        0 2022-04-28 23:15:01.000000 django-robust-redirects-1.0.0/robustredirects/locale/
-drwxr-xr-x   0 larrykiss   (501) staff       (20)        0 2022-04-28 23:15:01.000000 django-robust-redirects-1.0.0/robustredirects/locale/ru/
-drwxr-xr-x   0 larrykiss   (501) staff       (20)        0 2022-04-28 23:15:01.000000 django-robust-redirects-1.0.0/robustredirects/locale/ru/LC_MESSAGES/
--rw-r--r--   0 larrykiss   (501) staff       (20)     1974 2021-11-23 17:18:38.000000 django-robust-redirects-1.0.0/robustredirects/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 larrykiss   (501) staff       (20)     2479 2021-11-23 17:18:38.000000 django-robust-redirects-1.0.0/robustredirects/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 larrykiss   (501) staff       (20)        0 2022-04-28 23:15:01.000000 django-robust-redirects-1.0.0/robustredirects/locale/uk/
-drwxr-xr-x   0 larrykiss   (501) staff       (20)        0 2022-04-28 23:15:01.000000 django-robust-redirects-1.0.0/robustredirects/locale/uk/LC_MESSAGES/
--rw-r--r--   0 larrykiss   (501) staff       (20)     1944 2021-11-23 17:18:38.000000 django-robust-redirects-1.0.0/robustredirects/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 larrykiss   (501) staff       (20)     2446 2021-11-23 17:18:38.000000 django-robust-redirects-1.0.0/robustredirects/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 larrykiss   (501) staff       (20)        0 2022-04-28 23:15:01.000000 django-robust-redirects-1.0.0/robustredirects/locale/en/
-drwxr-xr-x   0 larrykiss   (501) staff       (20)        0 2022-04-28 23:15:01.000000 django-robust-redirects-1.0.0/robustredirects/locale/en/LC_MESSAGES/
--rw-r--r--   0 larrykiss   (501) staff       (20)     1497 2021-11-23 17:18:38.000000 django-robust-redirects-1.0.0/robustredirects/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 larrykiss   (501) staff       (20)     2429 2022-04-28 23:12:43.000000 django-robust-redirects-1.0.0/robustredirects/models.py
-drwxr-xr-x   0 larrykiss   (501) staff       (20)        0 2022-04-28 23:15:01.000000 django-robust-redirects-1.0.0/robustredirects/management/
--rw-r--r--   0 larrykiss   (501) staff       (20)        0 2021-11-23 17:18:38.000000 django-robust-redirects-1.0.0/robustredirects/management/__init__.py
-drwxr-xr-x   0 larrykiss   (501) staff       (20)        0 2022-04-28 23:15:01.000000 django-robust-redirects-1.0.0/robustredirects/management/__pycache__/
--rw-r--r--   0 larrykiss   (501) staff       (20)      172 2021-11-23 17:38:28.000000 django-robust-redirects-1.0.0/robustredirects/management/__pycache__/__init__.cpython-36.pyc
-drwxr-xr-x   0 larrykiss   (501) staff       (20)        0 2022-04-28 23:15:01.000000 django-robust-redirects-1.0.0/robustredirects/management/commands/
--rw-r--r--   0 larrykiss   (501) staff       (20)        0 2021-11-23 17:18:38.000000 django-robust-redirects-1.0.0/robustredirects/management/commands/__init__.py
-drwxr-xr-x   0 larrykiss   (501) staff       (20)        0 2022-04-28 23:15:01.000000 django-robust-redirects-1.0.0/robustredirects/management/commands/__pycache__/
--rw-r--r--   0 larrykiss   (501) staff       (20)      181 2021-11-23 18:06:01.000000 django-robust-redirects-1.0.0/robustredirects/management/commands/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 larrykiss   (501) staff       (20)     1053 2022-04-28 23:12:43.000000 django-robust-redirects-1.0.0/robustredirects/management/commands/convert_redirects.py
--rw-r--r--   0 larrykiss   (501) staff       (20)        0 2022-04-25 18:52:47.000000 django-robust-redirects-1.0.0/robustredirects/__init__.py
--rw-r--r--   0 larrykiss   (501) staff       (20)      143 2022-04-28 23:12:43.000000 django-robust-redirects-1.0.0/robustredirects/apps.py
--rw-r--r--   0 larrykiss   (501) staff       (20)     2638 2022-04-28 23:12:43.000000 django-robust-redirects-1.0.0/robustredirects/admin.py
--rw-r--r--   0 larrykiss   (501) staff       (20)     1816 2022-04-28 23:12:43.000000 django-robust-redirects-1.0.0/robustredirects/utils.py
-drwxr-xr-x   0 larrykiss   (501) staff       (20)        0 2022-04-28 23:15:01.000000 django-robust-redirects-1.0.0/robustredirects/templates/
--rw-r--r--   0 larrykiss   (501) staff       (20)     1598 2021-11-23 17:18:38.000000 django-robust-redirects-1.0.0/robustredirects/templates/change_form.html
--rw-r--r--   0 larrykiss   (501) staff       (20)     5964 2022-04-28 23:12:43.000000 django-robust-redirects-1.0.0/robustredirects/tests.py
--rw-r--r--   0 larrykiss   (501) staff       (20)       14 2021-11-23 17:18:38.000000 django-robust-redirects-1.0.0/robustredirects/urls.py
--rw-r--r--   0 larrykiss   (501) staff       (20)     3512 2022-04-28 23:12:43.000000 django-robust-redirects-1.0.0/robustredirects/middleware.py
--rw-r--r--   0 larrykiss   (501) staff       (20)     1493 2022-04-28 23:12:43.000000 django-robust-redirects-1.0.0/robustredirects/views.py
--rw-r--r--   0 larrykiss   (501) staff       (20)     1709 2022-04-28 23:12:43.000000 django-robust-redirects-1.0.0/README.md
--rw-r--r--   0 larrykiss   (501) staff       (20)      912 2022-04-28 23:12:43.000000 django-robust-redirects-1.0.0/setup.py
--rw-r--r--   0 larrykiss   (501) staff       (20)       38 2022-04-28 23:15:01.000000 django-robust-redirects-1.0.0/setup.cfg
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:02:11.712317 django-robust-redirects-1.0.1/
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1719 2023-03-21 14:42:59.000000 django-robust-redirects-1.0.1/LICENSE
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)      170 2023-04-10 14:42:46.000000 django-robust-redirects-1.0.1/MANIFEST.in
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)      639 2023-04-10 16:02:11.712180 django-robust-redirects-1.0.1/PKG-INFO
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1425 2023-04-08 00:10:15.000000 django-robust-redirects-1.0.1/README.md
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:02:11.707090 django-robust-redirects-1.0.1/django_robust_redirects.egg-info/
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)      639 2023-04-10 16:02:11.000000 django-robust-redirects-1.0.1/django_robust_redirects.egg-info/PKG-INFO
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1048 2023-04-10 16:02:11.000000 django-robust-redirects-1.0.1/django_robust_redirects.egg-info/SOURCES.txt
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)        1 2023-04-10 16:02:11.000000 django-robust-redirects-1.0.1/django_robust_redirects.egg-info/dependency_links.txt
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)        1 2023-04-10 14:47:42.000000 django-robust-redirects-1.0.1/django_robust_redirects.egg-info/not-zip-safe
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)       27 2023-04-10 16:02:11.000000 django-robust-redirects-1.0.1/django_robust_redirects.egg-info/requires.txt
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)       16 2023-04-10 16:02:11.000000 django-robust-redirects-1.0.1/django_robust_redirects.egg-info/top_level.txt
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:02:11.709813 django-robust-redirects-1.0.1/robustredirects/
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)        0 2023-03-21 14:42:59.000000 django-robust-redirects-1.0.1/robustredirects/__init__.py
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     2638 2023-04-10 15:09:01.000000 django-robust-redirects-1.0.1/robustredirects/admin.py
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)      143 2023-04-10 15:09:01.000000 django-robust-redirects-1.0.1/robustredirects/apps.py
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)       95 2023-03-21 14:42:59.000000 django-robust-redirects-1.0.1/robustredirects/dynamic_urls.py
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:02:11.704628 django-robust-redirects-1.0.1/robustredirects/locale/
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:02:11.704331 django-robust-redirects-1.0.1/robustredirects/locale/en/
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:02:11.710066 django-robust-redirects-1.0.1/robustredirects/locale/en/LC_MESSAGES/
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1497 2023-03-21 14:42:59.000000 django-robust-redirects-1.0.1/robustredirects/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:02:11.704494 django-robust-redirects-1.0.1/robustredirects/locale/ru/
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:02:11.710614 django-robust-redirects-1.0.1/robustredirects/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1974 2023-03-21 14:42:59.000000 django-robust-redirects-1.0.1/robustredirects/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     2479 2023-03-21 14:42:59.000000 django-robust-redirects-1.0.1/robustredirects/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:02:11.704692 django-robust-redirects-1.0.1/robustredirects/locale/uk/
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:02:11.711101 django-robust-redirects-1.0.1/robustredirects/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1944 2023-03-21 14:42:59.000000 django-robust-redirects-1.0.1/robustredirects/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     2446 2023-03-21 14:42:59.000000 django-robust-redirects-1.0.1/robustredirects/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:02:11.711310 django-robust-redirects-1.0.1/robustredirects/management/
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)        0 2023-03-21 14:42:59.000000 django-robust-redirects-1.0.1/robustredirects/management/__init__.py
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:02:11.711560 django-robust-redirects-1.0.1/robustredirects/management/commands/
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)        0 2023-03-21 14:42:59.000000 django-robust-redirects-1.0.1/robustredirects/management/commands/__init__.py
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1053 2023-04-10 15:09:01.000000 django-robust-redirects-1.0.1/robustredirects/management/commands/convert_redirects.py
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     3479 2023-04-10 15:09:01.000000 django-robust-redirects-1.0.1/robustredirects/middleware.py
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:02:11.711830 django-robust-redirects-1.0.1/robustredirects/migrations/
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)        0 2023-03-21 14:42:59.000000 django-robust-redirects-1.0.1/robustredirects/migrations/__init__.py
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     2429 2023-04-10 15:09:01.000000 django-robust-redirects-1.0.1/robustredirects/models.py
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:02:11.711952 django-robust-redirects-1.0.1/robustredirects/templates/
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1598 2023-03-21 14:42:59.000000 django-robust-redirects-1.0.1/robustredirects/templates/change_form.html
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     6054 2023-04-10 15:09:01.000000 django-robust-redirects-1.0.1/robustredirects/tests.py
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)       14 2023-04-10 15:09:01.000000 django-robust-redirects-1.0.1/robustredirects/urls.py
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1823 2023-04-10 15:09:01.000000 django-robust-redirects-1.0.1/robustredirects/utils.py
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1493 2023-04-10 15:09:01.000000 django-robust-redirects-1.0.1/robustredirects/views.py
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)       38 2023-04-10 16:02:11.712363 django-robust-redirects-1.0.1/setup.cfg
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)      945 2023-04-10 15:09:01.000000 django-robust-redirects-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-robust-redirects-1.0.0/django_robust_redirects.egg-info/PKG-INFO` & `django-robust-redirects-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: django-robust-redirects
-Version: 1.0.0
+Version: 1.0.1
 Summary: A more robust and feature full django redirect package
 Home-page: http://github.com/spothero/django-robust-redirects
+Download-URL: http://github.com/spothero/django-robust-redirects/tarball/0.10.0
 Author: SpotHero
 Author-email: pypi@spothero.com
-License: UNKNOWN
-Download-URL: http://github.com/spothero/django-robust-redirects/tarball/0.10.0
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3.6
+License-File: LICENSE
```

### Comparing `django-robust-redirects-1.0.0/django_robust_redirects.egg-info/SOURCES.txt` & `django-robust-redirects-1.0.1/django_robust_redirects.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 django_robust_redirects.egg-info/PKG-INFO
 django_robust_redirects.egg-info/SOURCES.txt
 django_robust_redirects.egg-info/dependency_links.txt
 django_robust_redirects.egg-info/not-zip-safe
@@ -19,12 +20,11 @@
 robustredirects/views.py
 robustredirects/locale/en/LC_MESSAGES/django.po
 robustredirects/locale/ru/LC_MESSAGES/django.mo
 robustredirects/locale/ru/LC_MESSAGES/django.po
 robustredirects/locale/uk/LC_MESSAGES/django.mo
 robustredirects/locale/uk/LC_MESSAGES/django.po
 robustredirects/management/__init__.py
-robustredirects/management/__pycache__/__init__.cpython-36.pyc
 robustredirects/management/commands/__init__.py
 robustredirects/management/commands/convert_redirects.py
-robustredirects/management/commands/__pycache__/__init__.cpython-36.pyc
+robustredirects/migrations/__init__.py
 robustredirects/templates/change_form.html
```

### Comparing `django-robust-redirects-1.0.0/PKG-INFO` & `django-robust-redirects-1.0.1/django_robust_redirects.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: django-robust-redirects
-Version: 1.0.0
+Version: 1.0.1
 Summary: A more robust and feature full django redirect package
 Home-page: http://github.com/spothero/django-robust-redirects
+Download-URL: http://github.com/spothero/django-robust-redirects/tarball/0.10.0
 Author: SpotHero
 Author-email: pypi@spothero.com
-License: UNKNOWN
-Download-URL: http://github.com/spothero/django-robust-redirects/tarball/0.10.0
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3.6
+License-File: LICENSE
```

### Comparing `django-robust-redirects-1.0.0/robustredirects/locale/ru/LC_MESSAGES/django.mo` & `django-robust-redirects-1.0.1/robustredirects/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-robust-redirects-1.0.0/robustredirects/locale/ru/LC_MESSAGES/django.po` & `django-robust-redirects-1.0.1/robustredirects/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-robust-redirects-1.0.0/robustredirects/locale/uk/LC_MESSAGES/django.mo` & `django-robust-redirects-1.0.1/robustredirects/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-robust-redirects-1.0.0/robustredirects/locale/uk/LC_MESSAGES/django.po` & `django-robust-redirects-1.0.1/robustredirects/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-robust-redirects-1.0.0/robustredirects/locale/en/LC_MESSAGES/django.po` & `django-robust-redirects-1.0.1/robustredirects/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-robust-redirects-1.0.0/robustredirects/models.py` & `django-robust-redirects-1.0.1/robustredirects/models.py`

 * *Files identical despite different names*

### Comparing `django-robust-redirects-1.0.0/robustredirects/management/commands/convert_redirects.py` & `django-robust-redirects-1.0.1/robustredirects/management/commands/convert_redirects.py`

 * *Files identical despite different names*

### Comparing `django-robust-redirects-1.0.0/robustredirects/admin.py` & `django-robust-redirects-1.0.1/robustredirects/admin.py`

 * *Files identical despite different names*

### Comparing `django-robust-redirects-1.0.0/robustredirects/utils.py` & `django-robust-redirects-1.0.1/robustredirects/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.conf.urls import url
+from django.urls import re_path
 from django.conf import settings
 from robustredirects.models import Redirect
 from robustredirects import views
 
 
 def ignored_url_paths():
     return getattr(settings, "ROBUST_REDIRECTS_IGNORED_PREFIXES", ())
@@ -38,17 +38,17 @@
         extra = {}
         pattern = r'^%s$' % redirect.from_url
 
         extra.update({'url': '%s' % redirect.to_url})
 
         if redirect.http_status == 302:
             extra.update({'permanent': False})
-            url_list.append(url(pattern, views.redirect_to, extra))
+            url_list.append(re_path(pattern, views.redirect_to, extra))
         else:
-            url_list.append(url(pattern, views.redirect_to, extra))
+            url_list.append(re_path(pattern, views.redirect_to, extra))
 
     arg_groups = list(group_arguments(url_list))
     for args in arg_groups:
         url_patterns += list(args)
 
     return url_patterns
```

### Comparing `django-robust-redirects-1.0.0/robustredirects/templates/change_form.html` & `django-robust-redirects-1.0.1/robustredirects/templates/change_form.html`

 * *Files identical despite different names*

### Comparing `django-robust-redirects-1.0.0/robustredirects/tests.py` & `django-robust-redirects-1.0.1/robustredirects/tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,16 +20,19 @@
         clear_url_caches()
         settings.ROBUST_REDIRECTS_IGNORED_URL_PATHS = None
 
     @staticmethod
     def run_redirect(request):
         from robustredirects import dynamic_urls
 
+        def get_response(*args, **kwargs):
+            print("Get Response")
+
         reload_module(dynamic_urls)
-        middleware = RedirectMiddleware()
+        middleware = RedirectMiddleware(get_response)
         response = HttpResponseNotFound()
         new_response = middleware.process_response(request, response)
         return new_response
 
     def test_redirect_request_permanent(self):
         # Create a redirect
         request = self.factory.get('/test/123/')
```

### Comparing `django-robust-redirects-1.0.0/robustredirects/middleware.py` & `django-robust-redirects-1.0.1/robustredirects/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from django.conf import settings
 from django.contrib.sites.shortcuts import get_current_site
 from django.urls import resolve, Resolver404
 from django.db.models import Q
 from django.http import HttpResponsePermanentRedirect, HttpResponseRedirect, HttpResponseGone
 from robustredirects.models import Redirect
 from robustredirects.utils import ignored_url_paths, replace_partial_url
```

### Comparing `django-robust-redirects-1.0.0/robustredirects/views.py` & `django-robust-redirects-1.0.1/robustredirects/views.py`

 * *Files identical despite different names*

### Comparing `django-robust-redirects-1.0.0/README.md` & `django-robust-redirects-1.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,56 @@
-Django Robust Redirects
-=======================
+# Django Robust Redirects
 
 A more robust django redirect project.
 
 Supports
 
 - Regular expression redirects
 - Ordinary direct redirects
 - Partial path redirects
 - Excluding paths that will never be redirected
 
 
-Installation
-------------
+## Installation
 
 1. Install the package from pip `pip install django-robust-redirects`
 2. Add the following line to your INSTALLED_APPS::
 
-```python
-  INSTALLED_APPS = (
-      ...
-      'robustredirects'
-  )
-```
+    ```python
+      INSTALLED_APPS = (
+          ...
+          'robustredirects'
+      )
+    ```
 
 3. Add the following lines to your middleware::
 
-```python
-  MIDDLEWARE_CLASSES = (
-      ...
-      'robustredirects.middleware.RedirectMiddleware'
-  )
-```
+    ```python
+      MIDDLEWARE_CLASSES = (
+          ...
+          'robustredirects.middleware.RedirectMiddleware'
+      )
+    ```
 
 4. Make and run migrations to add the tables to your database
 
 5. (Optional) Add the following lines to your settings to ignore certain paths::
 
-```python
-  # URL path prefixes that should never be redirected
-  ROBUST_REDIRECTS_IGNORED_PREFIXES = ('/api', '/admin')
-```
+    ```python
+      # URL path prefixes that should never be redirected
+      ROBUST_REDIRECTS_IGNORED_PREFIXES = ('/api', '/admin')
+    ```
 
-Converting from django.contrib.redirects
-----------------------------------------
+## Converting from django.contrib.redirects
 
 Robust redirects comes with a management command that will copy all django redirects over into robust redirects, just
 run `python manage.py convert_redirects`
 
-Changelog
-=========
+## Changelog
 
-1.0.0
------
+See the [CHANGELOG.md](CHANGELOG.md) file
 
-- Dropped support for all Python versions under Python 3.6.
-- Dropped support for Django versions under Django 3.2.
-- No longer using django-nose or nose test runner (ie django_nose.NoseTestSuiteRunner).
-- Added AppConfig.
-
-0.10.0
------
-
-- Add support for excluded URL path prefixes
-- Update for Django 1.9+
-
-0.9.2
------
-
-- Fix typos in the help text.
-- Require Django.
-- Prepend a slash when doing a partial replacement if the resulting url doesn’t have one. This avoid relative redirections.
-- Fix the model admin form and use it in the admin.
+## Running Tests
+1. Change to the `redirecttest` directory
+2. Install the requirements with `pip install -r requirements.txt`
+3. Initialize the database with `python manage.py migrate`
+4. Run the tests with `python manage.py test robustredirects`
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django-robust-redirects-1.0.0/setup.py` & `django-robust-redirects-1.0.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from setuptools import setup
+from setuptools import setup, find_packages
 
 setup(
     name="django-robust-redirects",
-    version="1.0.0",
+    version="1.0.1",
     url="http://github.com/spothero/django-robust-redirects",
     download_url="http://github.com/spothero/django-robust-redirects/tarball/0.10.0",
     description="A more robust and feature full django redirect package",
     author="SpotHero",
     author_email="pypi@spothero.com",
-    packages=["robustredirects"],
+    packages=find_packages(exclude=['redirecttest*']),
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         "Development Status :: 4 - Beta",
         "Framework :: Django",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
     ],
     python_requires=">=3.6",
     install_requires=[
-        "django>=3.2,<4",
+        "django>=3.2",
         "six>=1.12.0,<2"
     ],
 )
```

