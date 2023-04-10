# Comparing `tmp/logics-1.6.2.tar.gz` & `tmp/logics-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logics-1.6.2.tar", last modified: Fri Mar 17 15:14:37 2023, max compression
+gzip compressed data, was "logics-1.6.3.tar", last modified: Mon Apr 10 16:30:58 2023, max compression
```

## Comparing `logics-1.6.2.tar` & `logics-1.6.3.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:14:37.070790 logics-1.6.2/
--rwxrwxrwx   0 root         (0) root         (0)     1079 2021-03-26 14:06:13.000000 logics-1.6.2/LICENSE.txt
--rwxrwxrwx   0 root         (0) root         (0)    12232 2023-03-17 15:14:37.072222 logics-1.6.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)    11457 2023-03-16 17:08:29.000000 logics-1.6.2/README.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:14:36.579539 logics-1.6.2/logics/
--rwxrwxrwx   0 root         (0) root         (0)       24 2021-01-04 20:43:46.000000 logics-1.6.2/logics/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:14:36.583483 logics-1.6.2/logics/classes/
--rwxrwxrwx   0 root         (0) root         (0)        0 2020-11-23 15:17:26.000000 logics-1.6.2/logics/classes/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2980 2023-03-17 15:04:03.000000 logics-1.6.2/logics/classes/errors.py
--rwxrwxrwx   0 root         (0) root         (0)      919 2020-12-04 15:16:37.000000 logics-1.6.2/logics/classes/exceptions.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:14:36.630702 logics-1.6.2/logics/classes/predicate/
--rwxrwxrwx   0 root         (0) root         (0)      243 2023-02-22 18:26:21.000000 logics-1.6.2/logics/classes/predicate/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    27795 2023-02-23 17:44:50.000000 logics-1.6.2/logics/classes/predicate/formula.py
--rwxrwxrwx   0 root         (0) root         (0)    19794 2023-02-22 18:26:21.000000 logics-1.6.2/logics/classes/predicate/language.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:14:36.651342 logics-1.6.2/logics/classes/predicate/proof_theories/
--rwxrwxrwx   0 root         (0) root         (0)      246 2023-02-22 18:26:21.000000 logics-1.6.2/logics/classes/predicate/proof_theories/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      418 2023-02-22 18:26:21.000000 logics-1.6.2/logics/classes/predicate/proof_theories/derivation.py
--rwxrwxrwx   0 root         (0) root         (0)    12369 2023-03-17 15:08:30.000000 logics-1.6.2/logics/classes/predicate/proof_theories/natural_deduction.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:14:36.655275 logics-1.6.2/logics/classes/predicate/semantics/
--rwxrwxrwx   0 root         (0) root         (0)       72 2021-03-24 14:39:07.000000 logics-1.6.2/logics/classes/predicate/semantics/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    35944 2021-03-25 15:15:23.000000 logics-1.6.2/logics/classes/predicate/semantics/models.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:14:36.706802 logics-1.6.2/logics/classes/propositional/
--rwxrwxrwx   0 root         (0) root         (0)      195 2020-11-21 15:41:12.000000 logics-1.6.2/logics/classes/propositional/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    19235 2023-02-22 18:26:21.000000 logics-1.6.2/logics/classes/propositional/formula.py
--rwxrwxrwx   0 root         (0) root         (0)    22170 2022-09-26 18:39:16.000000 logics-1.6.2/logics/classes/propositional/inference.py
--rwxrwxrwx   0 root         (0) root         (0)    10060 2022-02-03 20:01:19.000000 logics-1.6.2/logics/classes/propositional/language.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:14:36.732161 logics-1.6.2/logics/classes/propositional/proof_theories/
--rwxrwxrwx   0 root         (0) root         (0)      518 2020-11-12 22:59:54.000000 logics-1.6.2/logics/classes/propositional/proof_theories/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    10897 2023-03-17 15:09:33.000000 logics-1.6.2/logics/classes/propositional/proof_theories/axiom_system.py
--rwxrwxrwx   0 root         (0) root         (0)     6040 2021-03-27 16:24:15.000000 logics-1.6.2/logics/classes/propositional/proof_theories/derivation.py
--rwxrwxrwx   0 root         (0) root         (0)    32961 2023-03-17 15:04:03.000000 logics-1.6.2/logics/classes/propositional/proof_theories/natural_deduction.py
--rwxrwxrwx   0 root         (0) root         (0)    67490 2023-03-17 15:11:42.000000 logics-1.6.2/logics/classes/propositional/proof_theories/sequents.py
--rwxrwxrwx   0 root         (0) root         (0)    54616 2023-03-17 15:04:55.000000 logics-1.6.2/logics/classes/propositional/proof_theories/tableaux.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:14:36.744398 logics-1.6.2/logics/classes/propositional/semantics/
--rwxrwxrwx   0 root         (0) root         (0)      156 2020-12-02 15:23:39.000000 logics-1.6.2/logics/classes/propositional/semantics/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    45702 2022-08-29 18:21:06.000000 logics-1.6.2/logics/classes/propositional/semantics/many_valued.py
--rwxrwxrwx   0 root         (0) root         (0)    24328 2021-03-22 18:00:32.000000 logics-1.6.2/logics/classes/propositional/semantics/mapped_logic.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:14:36.758351 logics-1.6.2/logics/instances/
--rwxrwxrwx   0 root         (0) root         (0)        0 2020-11-23 15:17:36.000000 logics-1.6.2/logics/instances/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:14:36.787434 logics-1.6.2/logics/instances/predicate/
--rwxrwxrwx   0 root         (0) root         (0)        0 2020-11-23 15:18:38.000000 logics-1.6.2/logics/instances/predicate/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7074 2023-02-22 18:26:21.000000 logics-1.6.2/logics/instances/predicate/languages.py
--rwxrwxrwx   0 root         (0) root         (0)     5209 2021-03-25 14:49:21.000000 logics-1.6.2/logics/instances/predicate/model_semantics.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:14:36.802054 logics-1.6.2/logics/instances/predicate/model_subclasses/
--rwxrwxrwx   0 root         (0) root         (0)      109 2020-10-16 15:02:56.000000 logics-1.6.2/logics/instances/predicate/model_subclasses/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1606 2020-12-14 17:40:49.000000 logics-1.6.2/logics/instances/predicate/model_subclasses/arithmetic.py
--rwxrwxrwx   0 root         (0) root         (0)     2274 2023-02-22 18:26:21.000000 logics-1.6.2/logics/instances/predicate/natural_deduction.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:14:36.909612 logics-1.6.2/logics/instances/propositional/
--rwxrwxrwx   0 root         (0) root         (0)        0 2020-11-23 15:18:54.000000 logics-1.6.2/logics/instances/propositional/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1022 2020-12-07 15:24:22.000000 logics-1.6.2/logics/instances/propositional/axiom_systems.py
--rwxrwxrwx   0 root         (0) root         (0)     4316 2022-08-29 18:21:06.000000 logics-1.6.2/logics/instances/propositional/languages.py
--rwxrwxrwx   0 root         (0) root         (0)    16665 2022-08-29 18:21:06.000000 logics-1.6.2/logics/instances/propositional/many_valued_semantics.py
--rwxrwxrwx   0 root         (0) root         (0)    12138 2021-03-18 16:02:34.000000 logics-1.6.2/logics/instances/propositional/mapped_logic_semantics.py
--rwxrwxrwx   0 root         (0) root         (0)     5498 2023-02-22 18:26:21.000000 logics-1.6.2/logics/instances/propositional/natural_deduction.py
--rwxrwxrwx   0 root         (0) root         (0)    17155 2022-02-03 19:56:56.000000 logics-1.6.2/logics/instances/propositional/sequents.py
--rwxrwxrwx   0 root         (0) root         (0)    17045 2023-02-28 16:31:49.000000 logics-1.6.2/logics/instances/propositional/tableaux.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:14:36.918416 logics-1.6.2/logics/utils/
--rwxrwxrwx   0 root         (0) root         (0)        0 2020-11-23 15:17:53.000000 logics-1.6.2/logics/utils/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:14:36.928125 logics-1.6.2/logics/utils/formula_generators/
--rwxrwxrwx   0 root         (0) root         (0)        0 2020-11-23 15:19:08.000000 logics-1.6.2/logics/utils/formula_generators/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    24268 2021-03-23 18:12:03.000000 logics-1.6.2/logics/utils/formula_generators/generators_biased.py
--rwxrwxrwx   0 root         (0) root         (0)       85 2021-03-26 15:35:46.000000 logics-1.6.2/logics/utils/formula_generators/generators_unbiased.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:14:36.947706 logics-1.6.2/logics/utils/parsers/
--rwxrwxrwx   0 root         (0) root         (0)      169 2023-03-16 17:08:29.000000 logics-1.6.2/logics/utils/parsers/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    16572 2021-03-25 14:03:02.000000 logics-1.6.2/logics/utils/parsers/parser_utils.py
--rwxrwxrwx   0 root         (0) root         (0)    21937 2023-02-23 18:39:04.000000 logics-1.6.2/logics/utils/parsers/predicate_parser.py
--rwxrwxrwx   0 root         (0) root         (0)    28650 2022-08-29 18:21:06.000000 logics-1.6.2/logics/utils/parsers/standard_parser.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:14:37.042767 logics-1.6.2/logics/utils/solvers/
--rwxrwxrwx   0 root         (0) root         (0)      196 2022-11-15 18:01:45.000000 logics-1.6.2/logics/utils/solvers/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    17735 2023-02-22 18:26:21.000000 logics-1.6.2/logics/utils/solvers/first_order_natural_deduction.py
--rwxrwxrwx   0 root         (0) root         (0)    65608 2023-02-22 18:26:21.000000 logics-1.6.2/logics/utils/solvers/natural_deduction.py
--rwxrwxrwx   0 root         (0) root         (0)    15790 2021-03-16 16:54:50.000000 logics-1.6.2/logics/utils/solvers/sequents.py
--rwxrwxrwx   0 root         (0) root         (0)     9699 2023-02-28 16:31:49.000000 logics-1.6.2/logics/utils/solvers/tableaux.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:14:37.056209 logics-1.6.2/logics/utils/upgrade/
--rwxrwxrwx   0 root         (0) root         (0)       88 2023-02-22 18:26:21.000000 logics-1.6.2/logics/utils/upgrade/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1916 2023-02-22 18:26:21.000000 logics-1.6.2/logics/utils/upgrade/upgrade.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:14:36.582157 logics-1.6.2/logics.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)    12232 2023-03-17 15:14:36.000000 logics-1.6.2/logics.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2630 2023-03-17 15:14:36.000000 logics-1.6.2/logics.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-03-17 15:14:36.000000 logics-1.6.2/logics.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-03-17 15:14:36.000000 logics-1.6.2/logics.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-03-17 15:14:36.000000 logics-1.6.2/logics.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      104 2021-03-26 14:42:28.000000 logics-1.6.2/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)      905 2023-03-17 15:14:37.075812 logics-1.6.2/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 16:30:58.643311 logics-1.6.3/
+-rwxrwxrwx   0 root         (0) root         (0)     1079 2021-03-26 14:06:13.000000 logics-1.6.3/LICENSE.txt
+-rwxrwxrwx   0 root         (0) root         (0)    12232 2023-04-10 16:30:58.643693 logics-1.6.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)    11457 2023-03-16 17:08:29.000000 logics-1.6.3/README.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 16:30:58.386889 logics-1.6.3/logics/
+-rwxrwxrwx   0 root         (0) root         (0)       24 2021-01-04 20:43:46.000000 logics-1.6.3/logics/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 16:30:58.425290 logics-1.6.3/logics/classes/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2020-11-23 15:17:26.000000 logics-1.6.3/logics/classes/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3043 2023-03-17 15:19:26.000000 logics-1.6.3/logics/classes/errors.py
+-rwxrwxrwx   0 root         (0) root         (0)      919 2020-12-04 15:16:37.000000 logics-1.6.3/logics/classes/exceptions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 16:30:58.427598 logics-1.6.3/logics/classes/predicate/
+-rwxrwxrwx   0 root         (0) root         (0)      243 2023-02-22 18:26:21.000000 logics-1.6.3/logics/classes/predicate/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    27795 2023-02-23 17:44:50.000000 logics-1.6.3/logics/classes/predicate/formula.py
+-rwxrwxrwx   0 root         (0) root         (0)    19794 2023-02-22 18:26:21.000000 logics-1.6.3/logics/classes/predicate/language.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 16:30:58.459053 logics-1.6.3/logics/classes/predicate/proof_theories/
+-rwxrwxrwx   0 root         (0) root         (0)      246 2023-02-22 18:26:21.000000 logics-1.6.3/logics/classes/predicate/proof_theories/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      418 2023-02-22 18:26:21.000000 logics-1.6.3/logics/classes/predicate/proof_theories/derivation.py
+-rwxrwxrwx   0 root         (0) root         (0)    12369 2023-03-17 15:15:19.000000 logics-1.6.3/logics/classes/predicate/proof_theories/natural_deduction.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 16:30:58.462176 logics-1.6.3/logics/classes/predicate/semantics/
+-rwxrwxrwx   0 root         (0) root         (0)       72 2021-03-24 14:39:07.000000 logics-1.6.3/logics/classes/predicate/semantics/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    35944 2021-03-25 15:15:23.000000 logics-1.6.3/logics/classes/predicate/semantics/models.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 16:30:58.472129 logics-1.6.3/logics/classes/propositional/
+-rwxrwxrwx   0 root         (0) root         (0)      195 2020-11-21 15:41:12.000000 logics-1.6.3/logics/classes/propositional/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    19235 2023-02-22 18:26:21.000000 logics-1.6.3/logics/classes/propositional/formula.py
+-rwxrwxrwx   0 root         (0) root         (0)    22170 2022-09-26 18:39:16.000000 logics-1.6.3/logics/classes/propositional/inference.py
+-rwxrwxrwx   0 root         (0) root         (0)    10060 2022-02-03 20:01:19.000000 logics-1.6.3/logics/classes/propositional/language.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 16:30:58.489311 logics-1.6.3/logics/classes/propositional/proof_theories/
+-rwxrwxrwx   0 root         (0) root         (0)      518 2020-11-12 22:59:54.000000 logics-1.6.3/logics/classes/propositional/proof_theories/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    10897 2023-03-17 15:15:19.000000 logics-1.6.3/logics/classes/propositional/proof_theories/axiom_system.py
+-rwxrwxrwx   0 root         (0) root         (0)     6040 2021-03-27 16:24:15.000000 logics-1.6.3/logics/classes/propositional/proof_theories/derivation.py
+-rwxrwxrwx   0 root         (0) root         (0)    34808 2023-04-10 16:26:27.000000 logics-1.6.3/logics/classes/propositional/proof_theories/natural_deduction.py
+-rwxrwxrwx   0 root         (0) root         (0)    67490 2023-03-17 15:15:19.000000 logics-1.6.3/logics/classes/propositional/proof_theories/sequents.py
+-rwxrwxrwx   0 root         (0) root         (0)    54616 2023-03-17 15:15:19.000000 logics-1.6.3/logics/classes/propositional/proof_theories/tableaux.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 16:30:58.495082 logics-1.6.3/logics/classes/propositional/semantics/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2020-12-02 15:23:39.000000 logics-1.6.3/logics/classes/propositional/semantics/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    45702 2022-08-29 18:21:06.000000 logics-1.6.3/logics/classes/propositional/semantics/many_valued.py
+-rwxrwxrwx   0 root         (0) root         (0)    24328 2021-03-22 18:00:32.000000 logics-1.6.3/logics/classes/propositional/semantics/mapped_logic.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 16:30:58.511138 logics-1.6.3/logics/instances/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2020-11-23 15:17:36.000000 logics-1.6.3/logics/instances/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 16:30:58.575604 logics-1.6.3/logics/instances/predicate/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2020-11-23 15:18:38.000000 logics-1.6.3/logics/instances/predicate/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7074 2023-02-22 18:26:21.000000 logics-1.6.3/logics/instances/predicate/languages.py
+-rwxrwxrwx   0 root         (0) root         (0)     5209 2021-03-25 14:49:21.000000 logics-1.6.3/logics/instances/predicate/model_semantics.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 16:30:58.579871 logics-1.6.3/logics/instances/predicate/model_subclasses/
+-rwxrwxrwx   0 root         (0) root         (0)      109 2020-10-16 15:02:56.000000 logics-1.6.3/logics/instances/predicate/model_subclasses/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1606 2020-12-14 17:40:49.000000 logics-1.6.3/logics/instances/predicate/model_subclasses/arithmetic.py
+-rwxrwxrwx   0 root         (0) root         (0)     2274 2023-02-22 18:26:21.000000 logics-1.6.3/logics/instances/predicate/natural_deduction.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 16:30:58.618096 logics-1.6.3/logics/instances/propositional/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2020-11-23 15:18:54.000000 logics-1.6.3/logics/instances/propositional/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1022 2020-12-07 15:24:22.000000 logics-1.6.3/logics/instances/propositional/axiom_systems.py
+-rwxrwxrwx   0 root         (0) root         (0)     4316 2022-08-29 18:21:06.000000 logics-1.6.3/logics/instances/propositional/languages.py
+-rwxrwxrwx   0 root         (0) root         (0)    16665 2022-08-29 18:21:06.000000 logics-1.6.3/logics/instances/propositional/many_valued_semantics.py
+-rwxrwxrwx   0 root         (0) root         (0)    12138 2021-03-18 16:02:34.000000 logics-1.6.3/logics/instances/propositional/mapped_logic_semantics.py
+-rwxrwxrwx   0 root         (0) root         (0)     8493 2023-04-10 16:05:04.000000 logics-1.6.3/logics/instances/propositional/natural_deduction.py
+-rwxrwxrwx   0 root         (0) root         (0)    17155 2022-02-03 19:56:56.000000 logics-1.6.3/logics/instances/propositional/sequents.py
+-rwxrwxrwx   0 root         (0) root         (0)    17045 2023-02-28 16:31:49.000000 logics-1.6.3/logics/instances/propositional/tableaux.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 16:30:58.619330 logics-1.6.3/logics/utils/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2020-11-23 15:17:53.000000 logics-1.6.3/logics/utils/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 16:30:58.622553 logics-1.6.3/logics/utils/formula_generators/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2020-11-23 15:19:08.000000 logics-1.6.3/logics/utils/formula_generators/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    24268 2021-03-23 18:12:03.000000 logics-1.6.3/logics/utils/formula_generators/generators_biased.py
+-rwxrwxrwx   0 root         (0) root         (0)       85 2021-03-26 15:35:46.000000 logics-1.6.3/logics/utils/formula_generators/generators_unbiased.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 16:30:58.628533 logics-1.6.3/logics/utils/parsers/
+-rwxrwxrwx   0 root         (0) root         (0)      169 2023-03-16 17:08:29.000000 logics-1.6.3/logics/utils/parsers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    16572 2021-03-25 14:03:02.000000 logics-1.6.3/logics/utils/parsers/parser_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)    21937 2023-02-23 18:39:04.000000 logics-1.6.3/logics/utils/parsers/predicate_parser.py
+-rwxrwxrwx   0 root         (0) root         (0)    28650 2022-08-29 18:21:06.000000 logics-1.6.3/logics/utils/parsers/standard_parser.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 16:30:58.641242 logics-1.6.3/logics/utils/solvers/
+-rwxrwxrwx   0 root         (0) root         (0)      196 2022-11-15 18:01:45.000000 logics-1.6.3/logics/utils/solvers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    17735 2023-02-22 18:26:21.000000 logics-1.6.3/logics/utils/solvers/first_order_natural_deduction.py
+-rwxrwxrwx   0 root         (0) root         (0)    65608 2023-02-22 18:26:21.000000 logics-1.6.3/logics/utils/solvers/natural_deduction.py
+-rwxrwxrwx   0 root         (0) root         (0)    15790 2021-03-16 16:54:50.000000 logics-1.6.3/logics/utils/solvers/sequents.py
+-rwxrwxrwx   0 root         (0) root         (0)     9699 2023-02-28 16:31:49.000000 logics-1.6.3/logics/utils/solvers/tableaux.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 16:30:58.642680 logics-1.6.3/logics/utils/upgrade/
+-rwxrwxrwx   0 root         (0) root         (0)       88 2023-02-22 18:26:21.000000 logics-1.6.3/logics/utils/upgrade/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1916 2023-02-22 18:26:21.000000 logics-1.6.3/logics/utils/upgrade/upgrade.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 16:30:58.421839 logics-1.6.3/logics.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)    12232 2023-04-10 16:30:58.000000 logics-1.6.3/logics.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2630 2023-04-10 16:30:58.000000 logics-1.6.3/logics.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-10 16:30:58.000000 logics-1.6.3/logics.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-04-10 16:30:58.000000 logics-1.6.3/logics.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        7 2023-04-10 16:30:58.000000 logics-1.6.3/logics.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      104 2021-03-26 14:42:28.000000 logics-1.6.3/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)      905 2023-04-10 16:30:58.644669 logics-1.6.3/setup.cfg
```

### Comparing `logics-1.6.2/LICENSE.txt` & `logics-1.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/PKG-INFO` & `logics-1.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logics
-Version: 1.6.2
+Version: 1.6.3
 Summary: Logics is a Python framework for mathematical logic
 Home-page: https://github.com/ariroffe/logics
 Author: Ariel Jonathan Roffé
 Author-email: arielroffe@filo.uba.ar
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `logics-1.6.2/README.rst` & `logics-1.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/classes/errors.py` & `logics-1.6.3/logics/classes/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     # Tableaux
     TBL_PREMISE_NOT_BEGINNING = 301
     TBL_INCORRECT_PREMISE = 302
     TBL_RULE_NOT_APPLIED = 303
     TBL_RULE_INCORRECTLY_APPLIED = 304
     TBL_PREMISE_NOT_PRESENT = 305
     TBL_CONCLUSION_NOT_PRESENT = 306
+    TBL_INCORRECT_INDEX = 307
 
     # Axiom systems
     AX_INCORRECT_PREMISE = 401
     AX_INCORRECT_AXIOM = 402
     AX_RULE_INCORRECTLY_APPLIED = 403
     AX_INCORRECT_JUSTIFICATION = 404
     AX_INCORRECT_CONCLUSION = 405
@@ -59,14 +60,15 @@
     # Tableaux
     301: "TBL: Premise not at the beggining",
     302: "TBL: Incorrect premise",
     303: "TBL: Rule not applied to node",
     304: "TBL: Rule incorrectly applied",
     305: "TBL: Premise not present",
     306: "TBL: Conclusion not present",
+    307: "TBL: Incorrect index",
 
     # Axiom systems
     401: "AX: Incorrect premise",
     402: "AX: Not an axiom instance",
     403: "AX: Rule incorrectly applied",
     404: "AX: Incorrect justification",
     405: "AX: Incorrect conclusion",
```

### Comparing `logics-1.6.2/logics/classes/exceptions.py` & `logics-1.6.3/logics/classes/exceptions.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/classes/predicate/formula.py` & `logics-1.6.3/logics/classes/predicate/formula.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/classes/predicate/language.py` & `logics-1.6.3/logics/classes/predicate/language.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/classes/predicate/proof_theories/natural_deduction.py` & `logics-1.6.3/logics/classes/predicate/proof_theories/natural_deduction.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/classes/predicate/semantics/models.py` & `logics-1.6.3/logics/classes/predicate/semantics/models.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/classes/propositional/formula.py` & `logics-1.6.3/logics/classes/propositional/formula.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/classes/propositional/inference.py` & `logics-1.6.3/logics/classes/propositional/inference.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/classes/propositional/language.py` & `logics-1.6.3/logics/classes/propositional/language.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/classes/propositional/proof_theories/__init__.py` & `logics-1.6.3/logics/classes/propositional/proof_theories/__init__.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/classes/propositional/proof_theories/axiom_system.py` & `logics-1.6.3/logics/classes/propositional/proof_theories/axiom_system.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/classes/propositional/proof_theories/derivation.py` & `logics-1.6.3/logics/classes/propositional/proof_theories/derivation.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/classes/propositional/proof_theories/natural_deduction.py` & `logics-1.6.3/logics/classes/propositional/proof_theories/natural_deduction.py`

 * *Files 4% similar despite different names*

```diff
@@ -224,21 +224,58 @@
 
         Notes
         --------
         For rules that have more than one variant (e.g. ``E∧1`` and ``E∧2``) you can omit the number. E.g.:
 
         >>> from logics.utils.parsers import classical_parser
         >>> from logics.instances.propositional.natural_deduction import classical_natural_deduction_system
-        >>> inf = classical_parser.parse('p and q / p')
+        >>> inf = classical_parser.parse('p ∧ q / p')
         >>> deriv = classical_parser.parse_derivation('''
-        ... p and q; premise; []; []
+        ... p ∧ q; premise; []; []
         ... p; E∧; [0]; []''',
         ... natural_deduction=True)
         >>> classical_natural_deduction_system.is_correct_derivation(deriv, inf)
         True
+
+        Also note that ``on_steps`` need to be provided in the order they were specified in the rule. E.g., the
+        conditional elimination rule states:
+
+        >>> cond_elim = NaturalDeductionRule([
+        >>> '(...)',
+        >>> NaturalDeductionStep(Formula(['→', ['A'], ['B']]), open_suppositions=[]),
+        >>> '(...)',
+        >>> NaturalDeductionStep(Formula(['A']), open_suppositions=[]),
+        >>> '(...)',
+        >>> NaturalDeductionStep(Formula(['B']), 'E→', [0, 1], open_suppositions=[])
+        >>> ]),
+
+        So, if we do:
+
+        >>> from logics.utils.parsers import classical_parser
+        >>> from logics.instances.propositional.natural_deduction import classical_natural_deduction_system
+        >>> inf = classical_parser.parse('p → q, p / q')
+        >>> deriv = classical_parser.parse_derivation('''
+        ... p → q; premise; []; []
+        ... p; premise; []; []
+        ... q; E→; [1, 0]; []''',
+        ... natural_deduction=True)
+        >>> classical_natural_deduction_system.is_correct_derivation(deriv, inf)
+        False
+
+        The last step is incorrect because the conditional elimination rule specifies that the first ``on_step`` is the
+        conditional statement and the second is the antecedent.
+
+        If you want to be able to specify them in reverse order, the solution is to add another rule to the system with
+        the ``on_steps`` reversed. There are some predefined systems that do this
+        (for rules that do not involve suppositions), see the Instances below.
+
+        >>> from logics.instances.propositional.natural_deduction import classical_natural_deduction_system_unordered
+        >>> # define the same inference and derivation as in the example above
+        >>> classical_natural_deduction_system_unordered.is_correct_derivation(deriv, inf)
+        True
         """
         error_list = list()
 
         for step_index in range(len(derivation)):
             step = derivation[step_index]
 
             # If the justification is 'premise'
```

### Comparing `logics-1.6.2/logics/classes/propositional/proof_theories/sequents.py` & `logics-1.6.3/logics/classes/propositional/proof_theories/sequents.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/classes/propositional/proof_theories/tableaux.py` & `logics-1.6.3/logics/classes/propositional/proof_theories/tableaux.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/classes/propositional/semantics/many_valued.py` & `logics-1.6.3/logics/classes/propositional/semantics/many_valued.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/classes/propositional/semantics/mapped_logic.py` & `logics-1.6.3/logics/classes/propositional/semantics/mapped_logic.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/instances/predicate/languages.py` & `logics-1.6.3/logics/instances/predicate/languages.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/instances/predicate/model_semantics.py` & `logics-1.6.3/logics/instances/predicate/model_semantics.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/instances/predicate/model_subclasses/arithmetic.py` & `logics-1.6.3/logics/instances/predicate/model_subclasses/arithmetic.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/instances/predicate/natural_deduction.py` & `logics-1.6.3/logics/instances/predicate/natural_deduction.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/instances/propositional/axiom_systems.py` & `logics-1.6.3/logics/instances/propositional/axiom_systems.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/instances/propositional/languages.py` & `logics-1.6.3/logics/instances/propositional/languages.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/instances/propositional/many_valued_semantics.py` & `logics-1.6.3/logics/instances/propositional/many_valued_semantics.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/instances/propositional/mapped_logic_semantics.py` & `logics-1.6.3/logics/instances/propositional/mapped_logic_semantics.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/instances/propositional/sequents.py` & `logics-1.6.3/logics/instances/propositional/sequents.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/instances/propositional/tableaux.py` & `logics-1.6.3/logics/instances/propositional/tableaux.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/utils/formula_generators/generators_biased.py` & `logics-1.6.3/logics/utils/formula_generators/generators_biased.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/utils/parsers/parser_utils.py` & `logics-1.6.3/logics/utils/parsers/parser_utils.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/utils/parsers/predicate_parser.py` & `logics-1.6.3/logics/utils/parsers/predicate_parser.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/utils/parsers/standard_parser.py` & `logics-1.6.3/logics/utils/parsers/standard_parser.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/utils/solvers/first_order_natural_deduction.py` & `logics-1.6.3/logics/utils/solvers/first_order_natural_deduction.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/utils/solvers/natural_deduction.py` & `logics-1.6.3/logics/utils/solvers/natural_deduction.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/utils/solvers/sequents.py` & `logics-1.6.3/logics/utils/solvers/sequents.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/utils/solvers/tableaux.py` & `logics-1.6.3/logics/utils/solvers/tableaux.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics/utils/upgrade/upgrade.py` & `logics-1.6.3/logics/utils/upgrade/upgrade.py`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/logics.egg-info/PKG-INFO` & `logics-1.6.3/logics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logics
-Version: 1.6.2
+Version: 1.6.3
 Summary: Logics is a Python framework for mathematical logic
 Home-page: https://github.com/ariroffe/logics
 Author: Ariel Jonathan Roffé
 Author-email: arielroffe@filo.uba.ar
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `logics-1.6.2/logics.egg-info/SOURCES.txt` & `logics-1.6.3/logics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logics-1.6.2/setup.cfg` & `logics-1.6.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = logics
-version = 1.6.2
+version = 1.6.3
 author = Ariel Jonathan Roffé
 author_email = arielroffe@filo.uba.ar
 url = https://github.com/ariroffe/logics
 description = Logics is a Python framework for mathematical logic
 license = MIT
 license_file = LICENSE.txt
 long_description = file: README.rst
```

