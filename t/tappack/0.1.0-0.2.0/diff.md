# Comparing `tmp/tappack-0.1.0.tar.gz` & `tmp/tappack-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tappack-0.1.0.tar", last modified: Fri Apr  7 14:50:42 2023, max compression
+gzip compressed data, was "tappack-0.2.0.tar", last modified: Mon Apr 10 13:55:34 2023, max compression
```

## Comparing `tappack-0.1.0.tar` & `tappack-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 14:50:42.420867 tappack-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-07 14:50:42.420867 tappack-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-07 14:50:40.000000 tappack-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 14:50:42.420867 tappack-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-07 14:50:36.000000 tappack-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 14:50:42.420867 tappack-0.1.0/tappack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 14:50:36.000000 tappack-0.1.0/tappack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-07 14:50:36.000000 tappack-0.1.0/tappack/autoexec.be.template
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-07 14:50:40.000000 tappack-0.1.0/tappack/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-07 14:50:40.000000 tappack-0.1.0/tappack/packaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-04-07 14:50:40.000000 tappack-0.1.0/tappack/source.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-07 14:50:40.000000 tappack-0.1.0/tappack/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 14:50:42.420867 tappack-0.1.0/tappack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-07 14:50:42.000000 tappack-0.1.0/tappack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-07 14:50:42.000000 tappack-0.1.0/tappack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 14:50:42.000000 tappack-0.1.0/tappack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-07 14:50:42.000000 tappack-0.1.0/tappack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-07 14:50:42.000000 tappack-0.1.0/tappack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-07 14:50:42.000000 tappack-0.1.0/tappack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:55:34.339856 tappack-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-10 13:55:34.339856 tappack-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-04-10 13:55:31.000000 tappack-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 13:55:34.339856 tappack-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-10 13:55:31.000000 tappack-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:55:34.335856 tappack-0.2.0/tappack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 13:55:26.000000 tappack-0.2.0/tappack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-10 13:55:26.000000 tappack-0.2.0/tappack/autoexec.be.template
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-10 13:55:31.000000 tappack-0.2.0/tappack/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-10 13:55:26.000000 tappack-0.2.0/tappack/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-10 13:55:31.000000 tappack-0.2.0/tappack/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-10 13:55:31.000000 tappack-0.2.0/tappack/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-04-10 13:55:31.000000 tappack-0.2.0/tappack/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-10 13:55:31.000000 tappack-0.2.0/tappack/tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 13:55:31.000000 tappack-0.2.0/tappack/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:55:34.339856 tappack-0.2.0/tappack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-10 13:55:34.000000 tappack-0.2.0/tappack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-10 13:55:34.000000 tappack-0.2.0/tappack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 13:55:34.000000 tappack-0.2.0/tappack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 13:55:34.000000 tappack-0.2.0/tappack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-10 13:55:34.000000 tappack-0.2.0/tappack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 13:55:34.000000 tappack-0.2.0/tappack.egg-info/top_level.txt
```

### Comparing `tappack-0.1.0/setup.py` & `tappack-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,20 @@
         name: [f'version', 'autoexec.be.template'],
     },
     install_requires=[
         'requests',
         'click',
         'pyyaml'
     ],
-    extras_require={},
+    extras_require={
+        'server': [
+            'flask',
+            'pyngrok'
+        ]
+    },
     entry_points={
         'console_scripts': [
             f'{name} = {name}.packaging:main',
+            f'{name}-server = {name}.server:main',
         ],
     }
 )
```

### Comparing `tappack-0.1.0/tappack/packaging.py` & `tappack-0.2.0/tappack/packaging.py`

 * *Files identical despite different names*

