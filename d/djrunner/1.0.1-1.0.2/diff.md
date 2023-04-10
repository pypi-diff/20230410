# Comparing `tmp/djrunner-1.0.1.tar.gz` & `tmp/djrunner-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djrunner-1.0.1.tar", last modified: Sat Nov 12 11:12:32 2022, max compression
+gzip compressed data, was "djrunner-1.0.2.tar", last modified: Mon Apr 10 06:30:15 2023, max compression
```

## Comparing `djrunner-1.0.1.tar` & `djrunner-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2022-11-12 11:12:32.797790 djrunner-1.0.1/
--rw-rw-r--   0 dev       (1000) dev       (1000)      746 2021-08-08 06:51:05.000000 djrunner-1.0.1/LICENSE
--rw-rw-r--   0 dev       (1000) dev       (1000)      161 2021-08-08 06:51:05.000000 djrunner-1.0.1/MANIFEST.in
--rw-rw-r--   0 dev       (1000) dev       (1000)      321 2022-11-12 11:12:32.797790 djrunner-1.0.1/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)     2936 2022-04-11 15:09:31.000000 djrunner-1.0.1/README.md
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2022-11-12 11:12:32.797790 djrunner-1.0.1/djrunner/
--rw-rw-r--   0 dev       (1000) dev       (1000)     6086 2022-05-24 13:54:50.000000 djrunner-1.0.1/djrunner/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      424 2021-12-16 06:38:36.000000 djrunner-1.0.1/djrunner/email.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     2878 2022-11-12 11:12:09.000000 djrunner-1.0.1/djrunner/fab.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2022-11-12 11:12:32.797790 djrunner-1.0.1/djrunner.egg-info/
--rw-rw-r--   0 dev       (1000) dev       (1000)      321 2022-11-12 11:12:32.000000 djrunner-1.0.1/djrunner.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)      279 2022-11-12 11:12:32.000000 djrunner-1.0.1/djrunner.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)        1 2022-11-12 11:12:32.000000 djrunner-1.0.1/djrunner.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)      137 2022-11-12 11:12:32.000000 djrunner-1.0.1/djrunner.egg-info/requires.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)        9 2022-11-12 11:12:32.000000 djrunner-1.0.1/djrunner.egg-info/top_level.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)      174 2022-09-07 17:34:29.000000 djrunner-1.0.1/requirements.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       79 2022-11-12 11:12:32.797790 djrunner-1.0.1/setup.cfg
--rw-rw-r--   0 dev       (1000) dev       (1000)      525 2022-11-12 11:12:23.000000 djrunner-1.0.1/setup.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-10 06:30:15.463910 djrunner-1.0.2/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      746 2021-08-08 06:51:05.000000 djrunner-1.0.2/LICENSE
+-rw-rw-r--   0 dev       (1000) dev       (1000)      161 2021-08-08 06:51:05.000000 djrunner-1.0.2/MANIFEST.in
+-rw-rw-r--   0 dev       (1000) dev       (1000)      321 2023-04-10 06:30:15.463910 djrunner-1.0.2/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2937 2023-03-31 16:22:36.000000 djrunner-1.0.2/README.md
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-10 06:30:15.463910 djrunner-1.0.2/djrunner/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     6086 2023-03-31 16:21:37.000000 djrunner-1.0.2/djrunner/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      424 2023-03-31 16:21:37.000000 djrunner-1.0.2/djrunner/email.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-10 06:30:15.463910 djrunner-1.0.2/djrunner.egg-info/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      321 2023-04-10 06:30:15.000000 djrunner-1.0.2/djrunner.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)      263 2023-04-10 06:30:15.000000 djrunner-1.0.2/djrunner.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)        1 2023-04-10 06:30:15.000000 djrunner-1.0.2/djrunner.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)      134 2023-04-10 06:30:15.000000 djrunner-1.0.2/djrunner.egg-info/requires.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)        9 2023-04-10 06:30:15.000000 djrunner-1.0.2/djrunner.egg-info/top_level.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)      171 2023-04-10 06:29:15.000000 djrunner-1.0.2/requirements.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       79 2023-04-10 06:30:15.463910 djrunner-1.0.2/setup.cfg
+-rw-rw-r--   0 dev       (1000) dev       (1000)      525 2023-04-10 05:04:36.000000 djrunner-1.0.2/setup.py
```

### Comparing `djrunner-1.0.1/LICENSE` & `djrunner-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `djrunner-1.0.1/README.md` & `djrunner-1.0.2/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -169,8 +169,8 @@
 
 from django.core.wsgi import get_wsgi_application
 
 os.environ.setdefault("DJANGO_SETTINGS_MODULE", "core.settings")
 
 application = get_wsgi_application()
 
-```
+```
```

### Comparing `djrunner-1.0.1/djrunner/__init__.py` & `djrunner-1.0.2/djrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `djrunner-1.0.1/setup.py` & `djrunner-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 
 with open('requirements.txt') as f:
     requires = f.read().splitlines()
 
 
-version = '1.0.1'
+version = '1.0.2'
 url = 'https://github.com/pmaigutyak/djrunner'
 
 
 setup(
     name='djrunner',
     version=version,
     description='Django run app',
```

