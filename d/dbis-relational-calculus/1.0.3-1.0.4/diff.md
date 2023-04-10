# Comparing `tmp/dbis-relational-calculus-1.0.3.tar.gz` & `tmp/dbis-relational-calculus-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbis-relational-calculus-1.0.3.tar", last modified: Mon Apr 10 12:11:58 2023, max compression
+gzip compressed data, was "dbis-relational-calculus-1.0.4.tar", last modified: Mon Apr 10 12:19:26 2023, max compression
```

## Comparing `dbis-relational-calculus-1.0.3.tar` & `dbis-relational-calculus-1.0.4.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.171054 dbis-relational-calculus-1.0.3/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11357 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/LICENSE
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11837 2023-04-10 12:11:58.171054 dbis-relational-calculus-1.0.3/PKG-INFO
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11343 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/README.md
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.169054 dbis-relational-calculus-1.0.3/dbis_relational_calculus.egg-info/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11837 2023-04-10 12:11:58.000000 dbis-relational-calculus-1.0.3/dbis_relational_calculus.egg-info/PKG-INFO
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2739 2023-04-10 12:11:58.000000 dbis-relational-calculus-1.0.3/dbis_relational_calculus.egg-info/SOURCES.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        1 2023-04-10 12:11:58.000000 dbis-relational-calculus-1.0.3/dbis_relational_calculus.egg-info/dependency_links.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       32 2023-04-10 12:11:58.000000 dbis-relational-calculus-1.0.3/dbis_relational_calculus.egg-info/requires.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       20 2023-04-10 12:11:58.000000 dbis-relational-calculus-1.0.3/dbis_relational_calculus.egg-info/top_level.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      709 2023-04-10 12:11:51.000000 dbis-relational-calculus-1.0.3/pyproject.toml
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.169054 dbis-relational-calculus-1.0.3/relational_calculus/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.169054 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6442 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/DomainCalculus.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      728 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/Result.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      320 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/Variable.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1358 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.169054 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8294 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/Formula.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4400 2023-04-10 12:11:51.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/Tuple.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.170054 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/atoms/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2674 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/atoms/Equals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2512 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/atoms/GreaterEquals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2503 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/atoms/GreaterThan.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2506 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/atoms/LessEquals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2497 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/atoms/LessThan.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/atoms/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.170054 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/connectives/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6785 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/connectives/And.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3258 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/connectives/Not.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6768 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/connectives/Or.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/connectives/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.170054 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/quantifiers/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4543 2023-04-10 12:11:51.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/quantifiers/Exists.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4407 2023-04-10 12:11:51.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/quantifiers/Forall.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/quantifiers/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.170054 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      956 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/Result.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3462 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/TupleCalculus.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1281 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.170054 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    10704 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/Formula.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2120 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/Variable.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.170054 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/atoms/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3914 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/atoms/Equals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3760 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/atoms/GreaterEquals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3753 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/atoms/GreaterThan.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3757 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/atoms/LessEquals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3747 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/atoms/LessThan.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/atoms/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.171054 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/connectives/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    12145 2023-04-10 11:15:31.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/connectives/And.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4573 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/connectives/Not.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    12108 2023-04-10 11:15:31.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/connectives/Or.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/connectives/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.171054 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/quantifiers/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8541 2023-04-10 12:11:51.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/quantifiers/Exists.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8290 2023-04-10 12:11:51.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/quantifiers/Forall.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/quantifiers/__init__.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       38 2023-04-10 12:11:58.171054 dbis-relational-calculus-1.0.3/setup.cfg
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:11:58.171054 dbis-relational-calculus-1.0.3/tests/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4425 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/tests/test_domain_calculus_sql.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      580 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/tests/test_domain_calculus_validity.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3100 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/tests/test_tuple_calculus_attribute_access.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4388 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/tests/test_tuple_calculus_sql.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      733 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.3/tests/test_tuple_calculus_validity.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:19:26.481855 dbis-relational-calculus-1.0.4/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11357 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/LICENSE
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11837 2023-04-10 12:19:26.481855 dbis-relational-calculus-1.0.4/PKG-INFO
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11343 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/README.md
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:19:26.479855 dbis-relational-calculus-1.0.4/dbis_relational_calculus.egg-info/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11837 2023-04-10 12:19:26.000000 dbis-relational-calculus-1.0.4/dbis_relational_calculus.egg-info/PKG-INFO
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2739 2023-04-10 12:19:26.000000 dbis-relational-calculus-1.0.4/dbis_relational_calculus.egg-info/SOURCES.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        1 2023-04-10 12:19:26.000000 dbis-relational-calculus-1.0.4/dbis_relational_calculus.egg-info/dependency_links.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       32 2023-04-10 12:19:26.000000 dbis-relational-calculus-1.0.4/dbis_relational_calculus.egg-info/requires.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       20 2023-04-10 12:19:26.000000 dbis-relational-calculus-1.0.4/dbis_relational_calculus.egg-info/top_level.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      709 2023-04-10 12:17:37.000000 dbis-relational-calculus-1.0.4/pyproject.toml
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:19:26.479855 dbis-relational-calculus-1.0.4/relational_calculus/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:19:26.479855 dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6442 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/DomainCalculus.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      728 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/Result.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      320 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/Variable.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1358 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:19:26.479855 dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8294 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/Formula.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4400 2023-04-10 12:11:51.000000 dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/Tuple.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:19:26.480855 dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/atoms/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2674 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/atoms/Equals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2512 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/atoms/GreaterEquals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2503 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/atoms/GreaterThan.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2506 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/atoms/LessEquals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2497 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/atoms/LessThan.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/atoms/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:19:26.480855 dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/connectives/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6785 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/connectives/And.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3258 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/connectives/Not.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6768 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/connectives/Or.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/connectives/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:19:26.480855 dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/quantifiers/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4543 2023-04-10 12:11:51.000000 dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/quantifiers/Exists.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4407 2023-04-10 12:11:51.000000 dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/quantifiers/Forall.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/quantifiers/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:19:26.480855 dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      956 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/Result.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3462 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/TupleCalculus.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1281 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:19:26.480855 dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    10704 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/Formula.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2120 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/Variable.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:19:26.480855 dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/atoms/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3914 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/atoms/Equals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3760 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/atoms/GreaterEquals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3753 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/atoms/GreaterThan.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3757 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/atoms/LessEquals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3747 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/atoms/LessThan.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/atoms/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:19:26.480855 dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/connectives/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    12145 2023-04-10 11:15:31.000000 dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/connectives/And.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4573 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/connectives/Not.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    12108 2023-04-10 11:15:31.000000 dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/connectives/Or.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/connectives/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:19:26.481855 dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/quantifiers/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8618 2023-04-10 12:19:02.000000 dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/quantifiers/Exists.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8367 2023-04-10 12:19:02.000000 dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/quantifiers/Forall.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/quantifiers/__init__.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       38 2023-04-10 12:19:26.481855 dbis-relational-calculus-1.0.4/setup.cfg
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 12:19:26.481855 dbis-relational-calculus-1.0.4/tests/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4425 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/tests/test_domain_calculus_sql.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      580 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/tests/test_domain_calculus_validity.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3100 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/tests/test_tuple_calculus_attribute_access.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4388 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/tests/test_tuple_calculus_sql.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      733 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.4/tests/test_tuple_calculus_validity.py
```

### Comparing `dbis-relational-calculus-1.0.3/LICENSE` & `dbis-relational-calculus-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/PKG-INFO` & `dbis-relational-calculus-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-relational-calculus
-Version: 1.0.3
+Version: 1.0.4
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: Til Mohr <til.mohr@rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis-relational-calculus
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-relational-calculus-1.0.3/README.md` & `dbis-relational-calculus-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/dbis_relational_calculus.egg-info/PKG-INFO` & `dbis-relational-calculus-1.0.4/dbis_relational_calculus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-relational-calculus
-Version: 1.0.3
+Version: 1.0.4
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: Til Mohr <til.mohr@rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis-relational-calculus
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-relational-calculus-1.0.3/dbis_relational_calculus.egg-info/SOURCES.txt` & `dbis-relational-calculus-1.0.4/dbis_relational_calculus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/pyproject.toml` & `dbis-relational-calculus-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbis-relational-calculus"
-version = "1.0.3"
+version = "1.0.4"
 description = "RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme"
 authors = [
 	{ name = "Til Mohr", email = "til.mohr@rwth-aachen.de" },
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/DomainCalculus.py` & `dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/DomainCalculus.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/Result.py` & `dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/Result.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/__init__.py` & `dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/__init__.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/Formula.py` & `dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/Formula.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/Tuple.py` & `dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/Tuple.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/atoms/Equals.py` & `dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/atoms/Equals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/atoms/GreaterEquals.py` & `dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/atoms/GreaterEquals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/atoms/GreaterThan.py` & `dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/atoms/GreaterThan.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/atoms/LessEquals.py` & `dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/atoms/LessEquals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/atoms/LessThan.py` & `dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/atoms/LessThan.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/connectives/And.py` & `dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/connectives/And.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/connectives/Not.py` & `dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/connectives/Not.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/connectives/Or.py` & `dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/connectives/Or.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/quantifiers/Exists.py` & `dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/quantifiers/Exists.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/domain_calculus/formulas/quantifiers/Forall.py` & `dbis-relational-calculus-1.0.4/relational_calculus/domain_calculus/formulas/quantifiers/Forall.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/Result.py` & `dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/Result.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/TupleCalculus.py` & `dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/TupleCalculus.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/__init__.py` & `dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/__init__.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/Formula.py` & `dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/Formula.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/Variable.py` & `dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/Variable.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/atoms/Equals.py` & `dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/atoms/Equals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/atoms/GreaterEquals.py` & `dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/atoms/GreaterEquals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/atoms/GreaterThan.py` & `dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/atoms/GreaterThan.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/atoms/LessEquals.py` & `dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/atoms/LessEquals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/atoms/LessThan.py` & `dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/atoms/LessThan.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/connectives/And.py` & `dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/connectives/And.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/connectives/Not.py` & `dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/connectives/Not.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/connectives/Or.py` & `dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/connectives/Or.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/quantifiers/Exists.py` & `dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/quantifiers/Exists.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,20 +52,20 @@
             and self.variable == other.variable
             and self.children[0] == other.children[0]
         )
 
     @typechecked
     def expand_quantifiers(self) -> tc.Formula:
         if isinstance(self.variable, set):
-            formula = self.children[0]
+            formula = self.children[0].expand_quantifiers()
             for variable in self.variable:
                 formula = Exists(variable, formula)
             return formula
         else:
-            return self
+            return Exists(self.variable, self.children[0].expand_quantifiers())
 
     @typechecked
     def move_quantifiers_inwards(self) -> tc.Formula:
         assert isinstance(self.variable, tc.Variable)
 
         if not self.children[0].contains_variable(self.variable):
             return self.children[0].move_quantifiers_inwards()
```

### Comparing `dbis-relational-calculus-1.0.3/relational_calculus/tuple_calculus/formulas/quantifiers/Forall.py` & `dbis-relational-calculus-1.0.4/relational_calculus/tuple_calculus/formulas/quantifiers/Forall.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,20 +52,20 @@
             and self.variable == other.variable
             and self.children[0] == other.children[0]
         )
 
     @typechecked
     def expand_quantifiers(self) -> tc.Formula:
         if isinstance(self.variable, set):
-            formula = self.children[0]
+            formula = self.children[0].expand_quantifiers()
             for variable in self.variable:
                 formula = Forall(variable, formula)
             return formula
         else:
-            return self
+            return Forall(self.variable, self.children[0].expand_quantifiers())
 
     @typechecked
     def move_quantifiers_inwards(self) -> tc.Formula:
         assert isinstance(self.variable, tc.Variable)
 
         if not self.children[0].contains_variable(self.variable):
             return self.children[0].move_quantifiers_inwards()
```

### Comparing `dbis-relational-calculus-1.0.3/tests/test_domain_calculus_sql.py` & `dbis-relational-calculus-1.0.4/tests/test_domain_calculus_sql.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/tests/test_domain_calculus_validity.py` & `dbis-relational-calculus-1.0.4/tests/test_domain_calculus_validity.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/tests/test_tuple_calculus_attribute_access.py` & `dbis-relational-calculus-1.0.4/tests/test_tuple_calculus_attribute_access.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/tests/test_tuple_calculus_sql.py` & `dbis-relational-calculus-1.0.4/tests/test_tuple_calculus_sql.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.3/tests/test_tuple_calculus_validity.py` & `dbis-relational-calculus-1.0.4/tests/test_tuple_calculus_validity.py`

 * *Files identical despite different names*

