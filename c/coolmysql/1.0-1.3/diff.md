# Comparing `tmp/coolmysql-1.0.tar.gz` & `tmp/coolmysql-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolmysql-1.0.tar", last modified: Thu Mar 16 14:45:14 2023, max compression
+gzip compressed data, was "coolmysql-1.3.tar", last modified: Mon Apr 10 14:26:15 2023, max compression
```

## Comparing `coolmysql-1.0.tar` & `coolmysql-1.3.tar`

### file list

```diff
@@ -1,10 +1,5 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmysql-1.0/LICENSE
--rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 coolmysql-1.0/Licenses of dependent packages/pymysql-LICENSE
--rw-r--r--   0        0        0     5661 2023-03-15 17:16:31.985718 coolmysql-1.0/README.md
--rw-r--r--   0        0        0       24 2022-11-25 13:24:44.000000 coolmysql-1.0/__init__.py
--rw-r--r--   0        0        0       73 2023-02-27 13:47:12.329777 coolmysql-1.0/coolmysql/__init__.py
--rw-r--r--   0        0        0    19839 2023-03-11 05:27:30.756063 coolmysql-1.0/coolmysql/_coolmysql.py
--rw-r--r--   0        0        0      612 2023-03-15 15:27:13.065279 coolmysql-1.0/pyproject.toml
--rw-r--r--   0        0        0    11396 2023-03-12 04:00:08.943260 coolmysql-1.0/test.py
--rw-r--r--   0        0        0     1547 2023-03-04 11:53:07.417341 coolmysql-1.0/希望小学.sql
--rw-r--r--   0        0        0     5937 1970-01-01 00:00:00.000000 coolmysql-1.0/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmysql-1.3/LICENSE
+-rw-r--r--   0        0        0     4351 2023-04-09 11:16:42.051321 coolmysql-1.3/README.md
+-rw-r--r--   0        0        0       29 2023-04-10 03:59:45.387315 coolmysql-1.3/coolmysql.py
+-rw-r--r--   0        0        0      562 2023-04-10 09:20:13.157209 coolmysql-1.3/pyproject.toml
+-rw-r--r--   0        0        0     4603 1970-01-01 00:00:00.000000 coolmysql-1.3/PKG-INFO
```

### Comparing `coolmysql-1.0/LICENSE` & `coolmysql-1.3/LICENSE`

 * *Files identical despite different names*

