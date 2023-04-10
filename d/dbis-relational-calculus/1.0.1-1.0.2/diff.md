# Comparing `tmp/dbis-relational-calculus-1.0.1.tar.gz` & `tmp/dbis-relational-calculus-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbis-relational-calculus-1.0.1.tar", last modified: Tue Mar 28 20:43:33 2023, max compression
+gzip compressed data, was "dbis-relational-calculus-1.0.2.tar", last modified: Mon Apr 10 11:23:01 2023, max compression
```

## Comparing `dbis-relational-calculus-1.0.1.tar` & `dbis-relational-calculus-1.0.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 20:43:33.683775 dbis-relational-calculus-1.0.1/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11357 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/LICENSE
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11837 2023-03-28 20:43:33.683775 dbis-relational-calculus-1.0.1/PKG-INFO
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11343 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/README.md
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 20:43:33.681774 dbis-relational-calculus-1.0.1/dbis_relational_calculus.egg-info/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11837 2023-03-28 20:43:33.000000 dbis-relational-calculus-1.0.1/dbis_relational_calculus.egg-info/PKG-INFO
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2739 2023-03-28 20:43:33.000000 dbis-relational-calculus-1.0.1/dbis_relational_calculus.egg-info/SOURCES.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        1 2023-03-28 20:43:33.000000 dbis-relational-calculus-1.0.1/dbis_relational_calculus.egg-info/dependency_links.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       32 2023-03-28 20:43:33.000000 dbis-relational-calculus-1.0.1/dbis_relational_calculus.egg-info/requires.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       20 2023-03-28 20:43:33.000000 dbis-relational-calculus-1.0.1/dbis_relational_calculus.egg-info/top_level.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      709 2023-03-28 20:43:17.000000 dbis-relational-calculus-1.0.1/pyproject.toml
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 20:43:33.681774 dbis-relational-calculus-1.0.1/relational_calculus/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/relational_calculus/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 20:43:33.682774 dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6442 2023-03-28 20:43:17.000000 dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/DomainCalculus.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      728 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/Result.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      320 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/Variable.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1358 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 20:43:33.682774 dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8294 2023-03-28 20:43:17.000000 dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/Formula.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4420 2023-03-28 20:43:17.000000 dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/Tuple.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 20:43:33.682774 dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/atoms/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2674 2023-03-28 20:43:17.000000 dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/atoms/Equals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2512 2023-03-28 20:43:17.000000 dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/atoms/GreaterEquals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2503 2023-03-28 20:43:17.000000 dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/atoms/GreaterThan.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2506 2023-03-28 20:43:17.000000 dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/atoms/LessEquals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2497 2023-03-28 20:43:17.000000 dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/atoms/LessThan.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/atoms/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 20:43:33.682774 dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/connectives/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6785 2023-03-28 20:43:17.000000 dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/connectives/And.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3258 2023-03-28 20:43:17.000000 dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/connectives/Not.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6768 2023-03-28 20:43:17.000000 dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/connectives/Or.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/connectives/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 20:43:33.682774 dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/quantifiers/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4548 2023-03-28 20:43:17.000000 dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/quantifiers/Exists.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4412 2023-03-28 20:43:17.000000 dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/quantifiers/Forall.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/quantifiers/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 20:43:33.682774 dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      956 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/Result.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3462 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/TupleCalculus.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1281 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 20:43:33.682774 dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    10704 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/Formula.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2120 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/Variable.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 20:43:33.683775 dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/atoms/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3914 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/atoms/Equals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3760 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/atoms/GreaterEquals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3753 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/atoms/GreaterThan.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3757 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/atoms/LessEquals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3747 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/atoms/LessThan.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/atoms/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 20:43:33.683775 dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/connectives/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    12145 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/connectives/And.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4573 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/connectives/Not.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    12108 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/connectives/Or.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/connectives/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 20:43:33.683775 dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/quantifiers/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8549 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/quantifiers/Exists.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8298 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/quantifiers/Forall.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/quantifiers/__init__.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       38 2023-03-28 20:43:33.683775 dbis-relational-calculus-1.0.1/setup.cfg
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 20:43:33.683775 dbis-relational-calculus-1.0.1/tests/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4425 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/tests/test_domain_calculus_sql.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      580 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/tests/test_domain_calculus_validity.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3100 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/tests/test_tuple_calculus_attribute_access.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4388 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/tests/test_tuple_calculus_sql.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      733 2023-03-28 19:51:35.000000 dbis-relational-calculus-1.0.1/tests/test_tuple_calculus_validity.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.403341 dbis-relational-calculus-1.0.2/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11357 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/LICENSE
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11837 2023-04-10 11:23:01.403341 dbis-relational-calculus-1.0.2/PKG-INFO
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11343 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/README.md
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.401341 dbis-relational-calculus-1.0.2/dbis_relational_calculus.egg-info/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11837 2023-04-10 11:23:01.000000 dbis-relational-calculus-1.0.2/dbis_relational_calculus.egg-info/PKG-INFO
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2739 2023-04-10 11:23:01.000000 dbis-relational-calculus-1.0.2/dbis_relational_calculus.egg-info/SOURCES.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        1 2023-04-10 11:23:01.000000 dbis-relational-calculus-1.0.2/dbis_relational_calculus.egg-info/dependency_links.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       32 2023-04-10 11:23:01.000000 dbis-relational-calculus-1.0.2/dbis_relational_calculus.egg-info/requires.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       20 2023-04-10 11:23:01.000000 dbis-relational-calculus-1.0.2/dbis_relational_calculus.egg-info/top_level.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      709 2023-04-10 11:22:50.000000 dbis-relational-calculus-1.0.2/pyproject.toml
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.401341 dbis-relational-calculus-1.0.2/relational_calculus/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.401341 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6442 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/DomainCalculus.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      728 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/Result.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      320 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/Variable.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1358 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.401341 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8294 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/Formula.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4420 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/Tuple.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.402341 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/atoms/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2674 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/atoms/Equals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2512 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/atoms/GreaterEquals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2503 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/atoms/GreaterThan.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2506 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/atoms/LessEquals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2497 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/atoms/LessThan.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/atoms/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.402341 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/connectives/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6785 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/connectives/And.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3258 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/connectives/Not.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6768 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/connectives/Or.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/connectives/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.402341 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/quantifiers/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4548 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/quantifiers/Exists.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4412 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/quantifiers/Forall.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/quantifiers/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.402341 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      956 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/Result.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3462 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/TupleCalculus.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1281 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.402341 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    10704 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/Formula.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2120 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/Variable.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.402341 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/atoms/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3914 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/atoms/Equals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3760 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/atoms/GreaterEquals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3753 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/atoms/GreaterThan.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3757 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/atoms/LessEquals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3747 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/atoms/LessThan.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/atoms/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.402341 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/connectives/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    12145 2023-04-10 11:15:31.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/connectives/And.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4573 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/connectives/Not.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    12108 2023-04-10 11:15:31.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/connectives/Or.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/connectives/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.403341 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/quantifiers/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8551 2023-04-10 11:15:31.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/quantifiers/Exists.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8300 2023-04-10 11:15:31.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/quantifiers/Forall.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/quantifiers/__init__.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       38 2023-04-10 11:23:01.403341 dbis-relational-calculus-1.0.2/setup.cfg
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.403341 dbis-relational-calculus-1.0.2/tests/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4425 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/tests/test_domain_calculus_sql.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      580 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/tests/test_domain_calculus_validity.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3100 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/tests/test_tuple_calculus_attribute_access.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4388 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/tests/test_tuple_calculus_sql.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      733 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/tests/test_tuple_calculus_validity.py
```

### Comparing `dbis-relational-calculus-1.0.1/LICENSE` & `dbis-relational-calculus-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/PKG-INFO` & `dbis-relational-calculus-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-relational-calculus
-Version: 1.0.1
+Version: 1.0.2
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: Til Mohr <til.mohr@rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis-relational-calculus
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-relational-calculus-1.0.1/README.md` & `dbis-relational-calculus-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/dbis_relational_calculus.egg-info/PKG-INFO` & `dbis-relational-calculus-1.0.2/dbis_relational_calculus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-relational-calculus
-Version: 1.0.1
+Version: 1.0.2
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: Til Mohr <til.mohr@rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis-relational-calculus
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-relational-calculus-1.0.1/dbis_relational_calculus.egg-info/SOURCES.txt` & `dbis-relational-calculus-1.0.2/dbis_relational_calculus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/pyproject.toml` & `dbis-relational-calculus-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbis-relational-calculus"
-version = "1.0.1"
+version = "1.0.2"
 description = "RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme"
 authors = [
 	{ name = "Til Mohr", email = "til.mohr@rwth-aachen.de" },
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/DomainCalculus.py` & `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/DomainCalculus.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/Result.py` & `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/Result.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/__init__.py` & `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/__init__.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/Formula.py` & `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/Formula.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/Tuple.py` & `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/Tuple.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/atoms/Equals.py` & `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/atoms/Equals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/atoms/GreaterEquals.py` & `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/atoms/GreaterEquals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/atoms/GreaterThan.py` & `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/atoms/GreaterThan.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/atoms/LessEquals.py` & `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/atoms/LessEquals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/atoms/LessThan.py` & `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/atoms/LessThan.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/connectives/And.py` & `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/connectives/And.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/connectives/Not.py` & `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/connectives/Not.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/connectives/Or.py` & `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/connectives/Or.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/quantifiers/Exists.py` & `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/quantifiers/Exists.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/domain_calculus/formulas/quantifiers/Forall.py` & `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/quantifiers/Forall.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/Result.py` & `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/Result.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/TupleCalculus.py` & `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/TupleCalculus.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/__init__.py` & `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/__init__.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/Formula.py` & `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/Formula.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/Variable.py` & `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/Variable.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/atoms/Equals.py` & `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/atoms/Equals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/atoms/GreaterEquals.py` & `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/atoms/GreaterEquals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/atoms/GreaterThan.py` & `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/atoms/GreaterThan.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/atoms/LessEquals.py` & `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/atoms/LessEquals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/atoms/LessThan.py` & `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/atoms/LessThan.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/connectives/And.py` & `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/connectives/And.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
                             self.children[0].children[0], self.children[1]
                         )._move_same_type_quantifiers_outwards(
                             move_exists=True, move_forall=False
                         ),
                     )
             if isinstance(self.children[1], tc.Exists):
                 variable = self.children[1].variable
-                if self.children[1].contains_variable(variable):
+                if self.children[0].contains_variable(variable):
                     return And(
                         self.children[0], self.children[1].rename_variable(variable)
                     )._move_same_type_quantifiers_outwards(
                         move_exists=True, move_forall=False
                     )
                 else:
                     return tc.Exists(
@@ -112,15 +112,15 @@
                             self.children[0].children[0], self.children[1]
                         )._move_same_type_quantifiers_outwards(
                             move_exists=False, move_forall=True
                         ),
                     )
             if isinstance(self.children[1], tc.Forall):
                 variable = self.children[1].variable
-                if self.children[1].contains_variable(variable):
+                if self.children[0].contains_variable(variable):
                     return And(
                         self.children[0], self.children[1].rename_variable(variable)
                     )._move_same_type_quantifiers_outwards(
                         move_exists=False, move_forall=True
                     )
                 else:
                     return tc.Forall(
```

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/connectives/Not.py` & `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/connectives/Not.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/connectives/Or.py` & `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/connectives/Or.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
                             self.children[0].children[0], self.children[1]
                         )._move_same_type_quantifiers_outwards(
                             move_exists=True, move_forall=False
                         ),
                     )
             if isinstance(self.children[1], tc.Exists):
                 variable = self.children[1].variable
-                if self.children[1].contains_variable(variable):
+                if self.children[0].contains_variable(variable):
                     return Or(
                         self.children[0], self.children[1].rename_variable(variable)
                     )._move_same_type_quantifiers_outwards(
                         move_exists=True, move_forall=False
                     )
                 else:
                     return tc.Exists(
@@ -120,15 +120,15 @@
                             self.children[0].children[0], self.children[1]
                         )._move_same_type_quantifiers_outwards(
                             move_exists=False, move_forall=True
                         ),
                     )
             if isinstance(self.children[1], tc.Forall):
                 variable = self.children[1].variable
-                if self.children[1].contains_variable(variable):
+                if self.children[0].contains_variable(variable):
                     return Or(
                         self.children[0], self.children[1].rename_variable(variable)
                     )._move_same_type_quantifiers_outwards(
                         move_exists=False, move_forall=True
                     )
                 else:
                     return tc.Forall(
```

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/quantifiers/Exists.py` & `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/quantifiers/Exists.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             type_str = type_str[: -len(" \\land ")]
         else:
             forall_str = self.variable.name
             type_str = (
                 f"\\text{{{self.variable.name}}} \\in \\text{{{self.variable.type}}}"
             )
 
-        return f"\\exists_{{{forall_str}}}(type_str \\land ({self.children[0]}))"
+        return f"\\exists_{{{forall_str}}}({type_str} \\land ({self.children[0]}))"
 
     @typechecked
     def __eq__(self, other) -> bool:
         return (
             isinstance(other, Exists)
             and self.variable == other.variable
             and self.children[0] == other.children[0]
```

### Comparing `dbis-relational-calculus-1.0.1/relational_calculus/tuple_calculus/formulas/quantifiers/Forall.py` & `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/quantifiers/Forall.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             type_str = type_str[: -len(" \\land ")]
         else:
             forall_str = self.variable.name
             type_str = (
                 f"\\text{{{self.variable.name}}} \\in \\text{{{self.variable.type}}}"
             )
 
-        return f"\\forall_{{{forall_str}}}(type_str \\land ({self.children[0]}))"
+        return f"\\forall_{{{forall_str}}}({type_str} \\land ({self.children[0]}))"
 
     @typechecked
     def __eq__(self, other) -> bool:
         return (
             isinstance(other, Forall)
             and self.variable == other.variable
             and self.children[0] == other.children[0]
```

### Comparing `dbis-relational-calculus-1.0.1/tests/test_domain_calculus_sql.py` & `dbis-relational-calculus-1.0.2/tests/test_domain_calculus_sql.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/tests/test_domain_calculus_validity.py` & `dbis-relational-calculus-1.0.2/tests/test_domain_calculus_validity.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/tests/test_tuple_calculus_attribute_access.py` & `dbis-relational-calculus-1.0.2/tests/test_tuple_calculus_attribute_access.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/tests/test_tuple_calculus_sql.py` & `dbis-relational-calculus-1.0.2/tests/test_tuple_calculus_sql.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.1/tests/test_tuple_calculus_validity.py` & `dbis-relational-calculus-1.0.2/tests/test_tuple_calculus_validity.py`

 * *Files identical despite different names*

