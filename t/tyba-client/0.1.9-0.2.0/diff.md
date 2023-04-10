# Comparing `tmp/tyba-client-0.1.9.tar.gz` & `tmp/tyba_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tyba-client-0.1.9.tar", max compression
+gzip compressed data, was "tyba_client-0.2.0.tar", max compression
```

## Comparing `tyba-client-0.1.9.tar` & `tyba_client-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1079 2021-08-06 03:12:49.175008 tyba-client-0.1.9/LICENSE
--rw-r--r--   0        0        0       18 2021-06-28 22:57:28.079564 tyba-client-0.1.9/README.md
--rw-r--r--   0        0        0      506 2021-08-30 18:48:12.211596 tyba-client-0.1.9/pyproject.toml
--rw-r--r--   0        0        0       22 2021-06-17 20:43:47.679004 tyba-client-0.1.9/tyba_client/__init__.py
--rw-r--r--   0        0        0     1884 2021-08-23 23:02:40.709145 tyba-client-0.1.9/tyba_client/client.py
--rw-r--r--   0        0        0     5998 2021-08-30 18:48:03.389936 tyba-client-0.1.9/tyba_client/models.py
--rw-r--r--   0        0        0      869 2021-06-21 22:50:06.942680 tyba-client-0.1.9/tyba_client/utils.py
--rw-r--r--   0        0        0      748 2021-08-30 18:48:34.974650 tyba-client-0.1.9/setup.py
--rw-r--r--   0        0        0      641 2021-08-30 18:48:34.974938 tyba-client-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1079 2021-11-05 19:13:19.360928 tyba_client-0.2.0/LICENSE
+-rw-r--r--   0        0        0       17 2023-03-20 18:44:14.006817 tyba_client-0.2.0/README.md
+-rw-r--r--   0        0        0      604 2023-04-10 20:10:00.481666 tyba_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2021-11-05 19:13:19.364928 tyba_client-0.2.0/tyba_client/__init__.py
+-rw-r--r--   0        0        0     5000 2023-04-06 20:40:29.569469 tyba_client-0.2.0/tyba_client/client.py
+-rw-r--r--   0        0        0    17644 2023-03-28 18:50:42.287839 tyba_client-0.2.0/tyba_client/models.py
+-rw-r--r--   0        0        0     2037 2021-11-10 00:29:24.081096 tyba_client-0.2.0/tyba_client/utils.py
+-rw-r--r--   0        0        0      827 1970-01-01 00:00:00.000000 tyba_client-0.2.0/setup.py
+-rw-r--r--   0        0        0      845 1970-01-01 00:00:00.000000 tyba_client-0.2.0/PKG-INFO
```

### Comparing `tyba-client-0.1.9/LICENSE` & `tyba_client-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tyba-client-0.1.9/PKG-INFO` & `tyba_client-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: tyba-client
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Python API client for the Tyba Public API
 License: MIT
 Author: Tyler Nisonoff
 Author-email: tyler@tybaenergy.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dataclasses-json (>=0.5.4,<0.6.0)
+Requires-Dist: generation-models (>=0.1.0,<0.2.0)
 Requires-Dist: marshmallow (>=3.12.1,<4.0.0)
 Requires-Dist: pandas (>=1.3.2,<2.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
+Requires-Dist: tyba-financial-model (>=0.1.0,<0.2.0)
 Description-Content-Type: text/markdown
 
 # Tyba API Client
-
```

