# Comparing `tmp/lins_pix-2.0.0.dev3.tar.gz` & `tmp/lins_pix-2.0.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lins_pix-2.0.0.dev3.tar", last modified: Thu Apr  6 19:58:44 2023, max compression
+gzip compressed data, was "dist/lins_pix-2.0.0.dev4.tar", last modified: Mon Apr 10 18:23:48 2023, max compression
```

## Comparing `lins_pix-2.0.0.dev3.tar` & `lins_pix-2.0.0.dev4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:58:44.000000 lins_pix-2.0.0.dev3/
--rw-r--r--   0 root         (0) root         (0)      281 2023-04-06 19:58:44.000000 lins_pix-2.0.0.dev3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3021 2023-04-06 19:58:22.000000 lins_pix-2.0.0.dev3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:58:44.000000 lins_pix-2.0.0.dev3/lins_pix/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-04-06 19:58:22.000000 lins_pix-2.0.0.dev3/lins_pix/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1231 2023-04-06 19:58:22.000000 lins_pix-2.0.0.dev3/lins_pix/log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:58:44.000000 lins_pix-2.0.0.dev3/lins_pix/psp/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-06 19:58:22.000000 lins_pix-2.0.0.dev3/lins_pix/psp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:58:44.000000 lins_pix-2.0.0.dev3/lins_pix/psp/santander/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-06 19:58:22.000000 lins_pix-2.0.0.dev3/lins_pix/psp/santander/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6833 2023-04-06 19:58:22.000000 lins_pix-2.0.0.dev3/lins_pix/psp/santander/autenticacao.py
--rw-rw-rw-   0 root         (0) root         (0)     7688 2023-04-06 19:58:22.000000 lins_pix-2.0.0.dev3/lins_pix/psp/santander/cob.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:58:44.000000 lins_pix-2.0.0.dev3/lins_pix/psp/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-06 19:58:22.000000 lins_pix-2.0.0.dev3/lins_pix/psp/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3868 2023-04-06 19:58:22.000000 lins_pix-2.0.0.dev3/lins_pix/psp/tests/test_api_santander.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-04-06 19:58:22.000000 lins_pix-2.0.0.dev3/lins_pix/qrcode.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2023-04-06 19:58:22.000000 lins_pix-2.0.0.dev3/lins_pix/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      872 2023-04-06 19:58:22.000000 lins_pix-2.0.0.dev3/lins_pix/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:58:44.000000 lins_pix-2.0.0.dev3/lins_pix.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)      281 2023-04-06 19:58:44.000000 lins_pix-2.0.0.dev3/lins_pix.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      473 2023-04-06 19:58:44.000000 lins_pix-2.0.0.dev3/lins_pix.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-06 19:58:44.000000 lins_pix-2.0.0.dev3/lins_pix.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-04-06 19:58:44.000000 lins_pix-2.0.0.dev3/lins_pix.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-04-06 19:58:44.000000 lins_pix-2.0.0.dev3/lins_pix.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-06 19:58:44.000000 lins_pix-2.0.0.dev3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      673 2023-04-06 19:58:22.000000 lins_pix-2.0.0.dev3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 18:23:48.000000 lins_pix-2.0.0.dev4/
+-rw-r--r--   0 root         (0) root         (0)      281 2023-04-10 18:23:48.000000 lins_pix-2.0.0.dev4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3021 2023-04-10 18:23:25.000000 lins_pix-2.0.0.dev4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 18:23:48.000000 lins_pix-2.0.0.dev4/lins_pix/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-04-10 18:23:25.000000 lins_pix-2.0.0.dev4/lins_pix/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1231 2023-04-10 18:23:25.000000 lins_pix-2.0.0.dev4/lins_pix/log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 18:23:48.000000 lins_pix-2.0.0.dev4/lins_pix/psp/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 18:23:25.000000 lins_pix-2.0.0.dev4/lins_pix/psp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 18:23:48.000000 lins_pix-2.0.0.dev4/lins_pix/psp/santander/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 18:23:25.000000 lins_pix-2.0.0.dev4/lins_pix/psp/santander/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6833 2023-04-10 18:23:25.000000 lins_pix-2.0.0.dev4/lins_pix/psp/santander/autenticacao.py
+-rw-rw-rw-   0 root         (0) root         (0)     7688 2023-04-10 18:23:25.000000 lins_pix-2.0.0.dev4/lins_pix/psp/santander/cob.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 18:23:48.000000 lins_pix-2.0.0.dev4/lins_pix/psp/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 18:23:25.000000 lins_pix-2.0.0.dev4/lins_pix/psp/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3868 2023-04-10 18:23:25.000000 lins_pix-2.0.0.dev4/lins_pix/psp/tests/test_api_santander.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-04-10 18:23:25.000000 lins_pix-2.0.0.dev4/lins_pix/qrcode.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2023-04-10 18:23:25.000000 lins_pix-2.0.0.dev4/lins_pix/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      872 2023-04-10 18:23:25.000000 lins_pix-2.0.0.dev4/lins_pix/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 18:23:48.000000 lins_pix-2.0.0.dev4/lins_pix.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)      281 2023-04-10 18:23:48.000000 lins_pix-2.0.0.dev4/lins_pix.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      473 2023-04-10 18:23:48.000000 lins_pix-2.0.0.dev4/lins_pix.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-10 18:23:48.000000 lins_pix-2.0.0.dev4/lins_pix.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-04-10 18:23:48.000000 lins_pix-2.0.0.dev4/lins_pix.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-04-10 18:23:48.000000 lins_pix-2.0.0.dev4/lins_pix.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 18:23:48.000000 lins_pix-2.0.0.dev4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      705 2023-04-10 18:23:25.000000 lins_pix-2.0.0.dev4/setup.py
```

### Comparing `lins_pix-2.0.0.dev3/README.md` & `lins_pix-2.0.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `lins_pix-2.0.0.dev3/lins_pix/log.py` & `lins_pix-2.0.0.dev4/lins_pix/log.py`

 * *Files identical despite different names*

### Comparing `lins_pix-2.0.0.dev3/lins_pix/psp/santander/autenticacao.py` & `lins_pix-2.0.0.dev4/lins_pix/psp/santander/autenticacao.py`

 * *Files identical despite different names*

### Comparing `lins_pix-2.0.0.dev3/lins_pix/psp/santander/cob.py` & `lins_pix-2.0.0.dev4/lins_pix/psp/santander/cob.py`

 * *Files identical despite different names*

### Comparing `lins_pix-2.0.0.dev3/lins_pix/psp/tests/test_api_santander.py` & `lins_pix-2.0.0.dev4/lins_pix/psp/tests/test_api_santander.py`

 * *Files identical despite different names*

### Comparing `lins_pix-2.0.0.dev3/lins_pix/qrcode.py` & `lins_pix-2.0.0.dev4/lins_pix/qrcode.py`

 * *Files identical despite different names*

### Comparing `lins_pix-2.0.0.dev3/lins_pix/settings.py` & `lins_pix-2.0.0.dev4/lins_pix/settings.py`

 * *Files identical despite different names*

### Comparing `lins_pix-2.0.0.dev3/lins_pix/utils.py` & `lins_pix-2.0.0.dev4/lins_pix/utils.py`

 * *Files identical despite different names*

