# Comparing `tmp/dbis-relational-calculus-1.0.2.tar.gz` & `tmp/dbis-relational-calculus-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbis-relational-calculus-1.0.2.tar", last modified: Mon Apr 10 11:23:01 2023, max compression
+gzip compressed data, was "dbis-relational-calculus-1.0.3.tar", last modified: Mon Apr 10 12:11:58 2023, max compression
```

## Comparing `dbis-relational-calculus-1.0.2.tar` & `dbis-relational-calculus-1.0.3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.403341 dbis-relational-calculus-1.0.2/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11357 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/LICENSE
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11837 2023-04-10 11:23:01.403341 dbis-relational-calculus-1.0.2/PKG-INFO
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11343 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/README.md
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.401341 dbis-relational-calculus-1.0.2/dbis_relational_calculus.egg-info/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11837 2023-04-10 11:23:01.000000 dbis-relational-calculus-1.0.2/dbis_relational_calculus.egg-info/PKG-INFO
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2739 2023-04-10 11:23:01.000000 dbis-relational-calculus-1.0.2/dbis_relational_calculus.egg-info/SOURCES.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        1 2023-04-10 11:23:01.000000 dbis-relational-calculus-1.0.2/dbis_relational_calculus.egg-info/dependency_links.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       32 2023-04-10 11:23:01.000000 dbis-relational-calculus-1.0.2/dbis_relational_calculus.egg-info/requires.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       20 2023-04-10 11:23:01.000000 dbis-relational-calculus-1.0.2/dbis_relational_calculus.egg-info/top_level.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      709 2023-04-10 11:22:50.000000 dbis-relational-calculus-1.0.2/pyproject.toml
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.401341 dbis-relational-calculus-1.0.2/relational_calculus/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.401341 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6442 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/DomainCalculus.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      728 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/Result.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      320 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/Variable.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1358 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.401341 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8294 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/Formula.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4420 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/Tuple.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.402341 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/atoms/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2674 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/atoms/Equals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2512 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/atoms/GreaterEquals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2503 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/atoms/GreaterThan.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2506 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/atoms/LessEquals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2497 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/atoms/LessThan.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/atoms/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.402341 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/connectives/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6785 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/connectives/And.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3258 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/connectives/Not.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6768 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/connectives/Or.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/connectives/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.402341 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/quantifiers/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4548 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/quantifiers/Exists.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4412 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/quantifiers/Forall.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/quantifiers/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.402341 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      956 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/Result.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3462 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/TupleCalculus.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1281 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.402341 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    10704 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/Formula.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2120 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/Variable.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.402341 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/atoms/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3914 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/atoms/Equals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3760 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/atoms/GreaterEquals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3753 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/atoms/GreaterThan.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3757 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/atoms/LessEquals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3747 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/atoms/LessThan.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/atoms/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.402341 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/connectives/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    12145 2023-04-10 11:15:31.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/connectives/And.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4573 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/connectives/Not.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    12108 2023-04-10 11:15:31.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/connectives/Or.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/connectives/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.403341 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/quantifiers/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8551 2023-04-10 11:15:31.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/quantifiers/Exists.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8300 2023-04-10 11:15:31.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/quantifiers/Forall.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/quantifiers/__init__.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       38 2023-04-10 11:23:01.403341 dbis-relational-calculus-1.0.2/setup.cfg
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:23:01.403341 dbis-relational-calculus-1.0.2/tests/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4425 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/tests/test_domain_calculus_sql.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      580 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/tests/test_domain_calculus_validity.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3100 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/tests/test_tuple_calculus_attribute_access.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4388 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/tests/test_tuple_calculus_sql.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      733 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.2/tests/test_tuple_calculus_validity.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.171054 dbis-relational-calculus-1.0.3/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11357 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/LICENSE
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11837 2023-04-10 12:11:58.171054 dbis-relational-calculus-1.0.3/PKG-INFO
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11343 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/README.md
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.169054 dbis-relational-calculus-1.0.3/dbis_relational_calculus.egg-info/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11837 2023-04-10 12:11:58.000000 dbis-relational-calculus-1.0.3/dbis_relational_calculus.egg-info/PKG-INFO
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2739 2023-04-10 12:11:58.000000 dbis-relational-calculus-1.0.3/dbis_relational_calculus.egg-info/SOURCES.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        1 2023-04-10 12:11:58.000000 dbis-relational-calculus-1.0.3/dbis_relational_calculus.egg-info/dependency_links.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       32 2023-04-10 12:11:58.000000 dbis-relational-calculus-1.0.3/dbis_relational_calculus.egg-info/requires.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       20 2023-04-10 12:11:58.000000 dbis-relational-calculus-1.0.3/dbis_relational_calculus.egg-info/top_level.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      709 2023-04-10 12:11:51.000000 dbis-relational-calculus-1.0.3/pyproject.toml
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.169054 dbis-relational-calculus-1.0.3/relational_calculus/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.169054 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6442 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/DomainCalculus.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      728 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/Result.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      320 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/Variable.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1358 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.169054 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8294 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/Formula.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4400 2023-04-10 12:11:51.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/Tuple.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.170054 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/atoms/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2674 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/atoms/Equals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2512 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/atoms/GreaterEquals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2503 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/atoms/GreaterThan.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2506 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/atoms/LessEquals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2497 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/atoms/LessThan.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/atoms/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.170054 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/connectives/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6785 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/connectives/And.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3258 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/connectives/Not.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6768 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/connectives/Or.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/connectives/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.170054 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/quantifiers/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4543 2023-04-10 12:11:51.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/quantifiers/Exists.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4407 2023-04-10 12:11:51.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/quantifiers/Forall.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/quantifiers/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.170054 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      956 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/Result.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3462 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/TupleCalculus.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1281 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.170054 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    10704 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/Formula.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2120 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/Variable.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.170054 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/atoms/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3914 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/atoms/Equals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3760 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/atoms/GreaterEquals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3753 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/atoms/GreaterThan.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3757 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/atoms/LessEquals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3747 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/atoms/LessThan.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/atoms/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.171054 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/connectives/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    12145 2023-04-10 11:15:31.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/connectives/And.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4573 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/connectives/Not.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    12108 2023-04-10 11:15:31.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/connectives/Or.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/connectives/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.171054 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/quantifiers/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8541 2023-04-10 12:11:51.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/quantifiers/Exists.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8290 2023-04-10 12:11:51.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/quantifiers/Forall.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/quantifiers/__init__.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       38 2023-04-10 12:11:58.171054 dbis-relational-calculus-1.0.3/setup.cfg
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.171054 dbis-relational-calculus-1.0.3/tests/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4425 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/tests/test_domain_calculus_sql.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      580 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/tests/test_domain_calculus_validity.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3100 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/tests/test_tuple_calculus_attribute_access.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4388 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/tests/test_tuple_calculus_sql.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      733 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/tests/test_tuple_calculus_validity.py
```

### Comparing `dbis-relational-calculus-1.0.2/LICENSE` & `dbis-relational-calculus-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/PKG-INFO` & `dbis-relational-calculus-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-relational-calculus
-Version: 1.0.2
+Version: 1.0.3
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: Til Mohr <til.mohr@rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis-relational-calculus
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-relational-calculus-1.0.2/README.md` & `dbis-relational-calculus-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/dbis_relational_calculus.egg-info/PKG-INFO` & `dbis-relational-calculus-1.0.3/dbis_relational_calculus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-relational-calculus
-Version: 1.0.2
+Version: 1.0.3
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: Til Mohr <til.mohr@rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis-relational-calculus
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-relational-calculus-1.0.2/dbis_relational_calculus.egg-info/SOURCES.txt` & `dbis-relational-calculus-1.0.3/dbis_relational_calculus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/pyproject.toml` & `dbis-relational-calculus-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbis-relational-calculus"
-version = "1.0.2"
+version = "1.0.3"
 description = "RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme"
 authors = [
 	{ name = "Til Mohr", email = "til.mohr@rwth-aachen.de" },
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/DomainCalculus.py` & `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/DomainCalculus.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/Result.py` & `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/Result.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/__init__.py` & `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/__init__.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/Formula.py` & `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/Formula.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/Tuple.py` & `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/Tuple.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                 )
             else:
                 formula = dc.Exists(new_var, formula)
         return formula
 
     @typechecked
     def contains_variable(self, variable: dc.Variable) -> bool:
-        return any(var == variable for var in self.variables)
+        return variable in self.variables
 
     @typechecked
     def contains_variable_typing(self, variable: dc.Variable) -> bool:
         return self.contains_variable(variable)
 
     @typechecked
     def contains_variable_quantification(self, variable: dc.Variable) -> bool:
```

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/atoms/Equals.py` & `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/atoms/Equals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/atoms/GreaterEquals.py` & `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/atoms/GreaterEquals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/atoms/GreaterThan.py` & `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/atoms/GreaterThan.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/atoms/LessEquals.py` & `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/atoms/LessEquals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/atoms/LessThan.py` & `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/atoms/LessThan.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/connectives/And.py` & `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/connectives/And.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/connectives/Not.py` & `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/connectives/Not.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/connectives/Or.py` & `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/connectives/Or.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/quantifiers/Exists.py` & `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/quantifiers/Exists.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                 formula = Exists(var, formula)
             return formula
         return Exists(self.variable, self.children[0]._to_normal_form())
 
     @typechecked
     def contains_variable(self, variable: dc.Variable) -> bool:
         return (
-            any(self.variable == variable)
+            variable in self.variable
             if isinstance(self.variable, set)
             else self.variable == variable
         ) or self.children[0].contains_variable(variable)
 
     @typechecked
     def contains_variable_typing(self, variable: dc.Variable) -> bool:
         return False
```

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/domain_calculus/formulas/quantifiers/Forall.py` & `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/quantifiers/Forall.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                 formula = Forall(var, formula)
             return formula
         return Forall(self.variable, self.children[0]._to_normal_form())
 
     @typechecked
     def contains_variable(self, variable: dc.Variable) -> bool:
         return (
-            any(self.variable == variable)
+            variable in self.variable
             if isinstance(self.variable, set)
             else self.variable == variable
         ) or self.children[0].contains_variable(variable)
 
     @typechecked
     def contains_variable_typing(self, variable: dc.Variable) -> bool:
         return False
```

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/Result.py` & `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/Result.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/TupleCalculus.py` & `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/TupleCalculus.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/__init__.py` & `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/__init__.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/Formula.py` & `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/Formula.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/Variable.py` & `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/Variable.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/atoms/Equals.py` & `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/atoms/Equals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/atoms/GreaterEquals.py` & `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/atoms/GreaterEquals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/atoms/GreaterThan.py` & `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/atoms/GreaterThan.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/atoms/LessEquals.py` & `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/atoms/LessEquals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/atoms/LessThan.py` & `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/atoms/LessThan.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/connectives/And.py` & `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/connectives/And.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/connectives/Not.py` & `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/connectives/Not.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/connectives/Or.py` & `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/connectives/Or.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/quantifiers/Exists.py` & `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/quantifiers/Exists.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,23 +169,23 @@
                 formula = Exists(var, formula)
             return formula
         return Exists(self.variable, self.children[0]._to_normal_form())
 
     @typechecked
     def contains_variable(self, variable: tc.Variable) -> bool:
         return (
-            any(self.variable == variable)
+            variable in self.variable
             if isinstance(self.variable, set)
             else self.variable == variable
         ) or self.children[0].contains_variable(variable)
 
     @typechecked
     def contains_variable_typing(self, variable: tc.Variable) -> bool:
         return (
-            any(self.variable == variable)
+            variable in self.variable
             if isinstance(self.variable, set)
             else self.variable == variable
         ) or self.children[0].contains_variable_typing(variable)
 
     @typechecked
     def _rename_variable(
         self, old_variable: tc.Variable, new_variable: tc.Variable
```

### Comparing `dbis-relational-calculus-1.0.2/relational_calculus/tuple_calculus/formulas/quantifiers/Forall.py` & `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/quantifiers/Forall.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,23 +164,23 @@
                 formula = Forall(var, formula)
             return formula
         return Forall(self.variable, self.children[0]._to_normal_form())
 
     @typechecked
     def contains_variable(self, variable: tc.Variable) -> bool:
         return (
-            any(self.variable == variable)
+            variable in self.variable
             if isinstance(self.variable, set)
             else self.variable == variable
         ) or self.children[0].contains_variable(variable)
 
     @typechecked
     def contains_variable_typing(self, variable: tc.Variable) -> bool:
         return (
-            any(self.variable == variable)
+            variable in self.variable
             if isinstance(self.variable, set)
             else self.variable == variable
         ) or self.children[0].contains_variable_typing(variable)
 
     @typechecked
     def _rename_variable(
         self, old_variable: tc.Variable, new_variable: tc.Variable
```

### Comparing `dbis-relational-calculus-1.0.2/tests/test_domain_calculus_sql.py` & `dbis-relational-calculus-1.0.3/tests/test_domain_calculus_sql.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/tests/test_domain_calculus_validity.py` & `dbis-relational-calculus-1.0.3/tests/test_domain_calculus_validity.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/tests/test_tuple_calculus_attribute_access.py` & `dbis-relational-calculus-1.0.3/tests/test_tuple_calculus_attribute_access.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/tests/test_tuple_calculus_sql.py` & `dbis-relational-calculus-1.0.3/tests/test_tuple_calculus_sql.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.2/tests/test_tuple_calculus_validity.py` & `dbis-relational-calculus-1.0.3/tests/test_tuple_calculus_validity.py`

 * *Files identical despite different names*

