# Comparing `tmp/in-dbt-spark-1.2.507.tar.gz` & `tmp/in-dbt-spark-1.2.509.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "in-dbt-spark-1.2.507.tar", last modified: Mon Mar 27 17:05:00 2023, max compression
+gzip compressed data, was "in-dbt-spark-1.2.509.tar", last modified: Mon Apr 10 21:15:53 2023, max compression
```

## Comparing `in-dbt-spark-1.2.507.tar` & `in-dbt-spark-1.2.509.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:05:00.800980 in-dbt-spark-1.2.507/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-03-27 17:05:00.796980 in-dbt-spark-1.2.507/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:05:00.788979 in-dbt-spark-1.2.507/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:05:00.788979 in-dbt-spark-1.2.507/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:05:00.792979 in-dbt-spark-1.2.507/dbt/adapters/setu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/adapters/setu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/adapters/setu/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/adapters/setu/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/adapters/setu/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/adapters/setu/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/adapters/setu/session_cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/adapters/setu/session_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/adapters/setu/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/adapters/setu/setu_session_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/adapters/setu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:05:00.792979 in-dbt-spark-1.2.507/dbt/adapters/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/adapters/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/adapters/spark/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/adapters/spark/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    24727 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/adapters/spark/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    21688 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/adapters/spark/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/adapters/spark/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/adapters/spark/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/adapters/spark/spark_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:05:00.788979 in-dbt-spark-1.2.507/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:05:00.792979 in-dbt-spark-1.2.507/dbt/include/spark/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/include/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/include/spark/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:05:00.796980 in-dbt-spark-1.2.507/dbt/include/spark/macros/
--rw-r--r--   0 runner    (1001) docker     (123)    13436 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/include/spark/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/include/spark/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/include/spark/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:05:00.796980 in-dbt-spark-1.2.507/dbt/include/spark/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:05:00.796980 in-dbt-spark-1.2.507/dbt/include/spark/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/include/spark/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/include/spark/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/include/spark/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/include/spark/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/include/spark/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/include/spark/macros/materializations/validate.sql
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/include/spark/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:05:00.796980 in-dbt-spark-1.2.507/dbt/include/spark/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/include/spark/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/include/spark/macros/utils/assert_not_null.sql
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/include/spark/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/include/spark/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/include/spark/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/include/spark/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/include/spark/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/include/spark/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/dbt/include/spark/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:05:00.796980 in-dbt-spark-1.2.507/in_dbt_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-03-27 17:05:00.000000 in-dbt-spark-1.2.507/in_dbt_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-03-27 17:05:00.000000 in-dbt-spark-1.2.507/in_dbt_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 17:05:00.000000 in-dbt-spark-1.2.507/in_dbt_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 17:05:00.000000 in-dbt-spark-1.2.507/in_dbt_spark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-27 17:05:00.000000 in-dbt-spark-1.2.507/in_dbt_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-27 17:05:00.000000 in-dbt-spark-1.2.507/in_dbt_spark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 17:05:00.800980 in-dbt-spark-1.2.507/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-03-27 17:04:44.000000 in-dbt-spark-1.2.507/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:53.323069 in-dbt-spark-1.2.509/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-10 21:15:53.323069 in-dbt-spark-1.2.509/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:53.315069 in-dbt-spark-1.2.509/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:53.315069 in-dbt-spark-1.2.509/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:53.315069 in-dbt-spark-1.2.509/dbt/adapters/setu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/setu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/setu/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/setu/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/setu/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/setu/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/setu/session_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/setu/session_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12139 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/setu/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/setu/setu_session_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/setu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:53.319069 in-dbt-spark-1.2.509/dbt/adapters/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/spark/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/spark/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24727 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/spark/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21731 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/spark/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/spark/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/spark/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/adapters/spark/spark_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:53.315069 in-dbt-spark-1.2.509/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:53.319069 in-dbt-spark-1.2.509/dbt/include/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:53.319069 in-dbt-spark-1.2.509/dbt/include/spark/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/apply_retention.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:53.319069 in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:53.319069 in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/validate.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:53.323069 in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/assert_not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/dbt/include/spark/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:15:53.323069 in-dbt-spark-1.2.509/in_dbt_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-10 21:15:53.000000 in-dbt-spark-1.2.509/in_dbt_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-10 21:15:53.000000 in-dbt-spark-1.2.509/in_dbt_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 21:15:53.000000 in-dbt-spark-1.2.509/in_dbt_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 21:15:53.000000 in-dbt-spark-1.2.509/in_dbt_spark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-10 21:15:53.000000 in-dbt-spark-1.2.509/in_dbt_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-10 21:15:53.000000 in-dbt-spark-1.2.509/in_dbt_spark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 21:15:53.323069 in-dbt-spark-1.2.509/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-10 21:15:40.000000 in-dbt-spark-1.2.509/setup.py
```

### Comparing `in-dbt-spark-1.2.507/PKG-INFO` & `in-dbt-spark-1.2.509/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: in-dbt-spark
-Version: 1.2.507
+Version: 1.2.509
 Summary: Release for LinkedIn's changes to dbt-spark.
 Home-page: https://github.com/linkedin/in-dbt-spark
 Author: LinkedIn DBT Team
 Author-email: dbt-dev@linkedin.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.2.507 Summary: Release for
+Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.2.509 Summary: Release for
 LinkedIn's changes to dbt-spark. Home-page: https://github.com/linkedin/in-dbt-
 spark Author: LinkedIn DBT Team Author-email: dbt-dev@linkedin.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `in-dbt-spark-1.2.507/README.md` & `in-dbt-spark-1.2.509/README.md`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.507/dbt/adapters/setu/client.py` & `in-dbt-spark-1.2.509/dbt/adapters/setu/client.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.507/dbt/adapters/setu/constants.py` & `in-dbt-spark-1.2.509/dbt/adapters/setu/constants.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.507/dbt/adapters/setu/models.py` & `in-dbt-spark-1.2.509/dbt/adapters/setu/models.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.507/dbt/adapters/setu/session.py` & `in-dbt-spark-1.2.509/dbt/adapters/setu/session.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,19 @@
         session = self.client.get_session(session_id=self.session_id)
         logger.info("SETU session INFO = {} ".format(session))
 
     def wait_till_ready(self) -> None:
         """Wait for the session to be ready."""
         intervals = polling_intervals([1, 2, 3, 5], 10)
         while self.state in SESSION_STATE_NOT_READY:
-            time.sleep(next(intervals))
+            interval = next(intervals)
+            logger.info(
+                f"Waiting to get spark resources for setu session - {self.session_id} .. Sleeping for {interval} seconds.."
+            )
+            time.sleep(interval)
         self.print_session_details()
 
     @property
     def state(self) -> SessionState:
         """The state of the managed SETU session."""
         session = self.client.get_session(self.session_id)
         if session is None:
```

### Comparing `in-dbt-spark-1.2.507/dbt/adapters/setu/session_cursor.py` & `in-dbt-spark-1.2.509/dbt/adapters/setu/session_cursor.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.507/dbt/adapters/setu/session_handler.py` & `in-dbt-spark-1.2.509/dbt/adapters/setu/session_handler.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.507/dbt/adapters/setu/session_manager.py` & `in-dbt-spark-1.2.509/dbt/adapters/setu/session_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,14 +202,15 @@
         with cls.session_lock:
             with SetuClient(url, auth, verify) as client:
                 session = client.get_session(cls.session_id)
                 if session is not None:
                     client.cancel_session(cls.session_id)
                     cls.session_id = None
                     logger.info(f"cancelled session : {cls.session_id}")
+                client.close()
 
     @classmethod
     def get_session_if_active(
         cls,
         url: str,
         session_id: str,
         auth: Auth = None,
```

### Comparing `in-dbt-spark-1.2.507/dbt/adapters/setu/setu_session_request.py` & `in-dbt-spark-1.2.509/dbt/adapters/setu/setu_session_request.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.507/dbt/adapters/setu/utils.py` & `in-dbt-spark-1.2.509/dbt/adapters/setu/utils.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.507/dbt/adapters/spark/column.py` & `in-dbt-spark-1.2.509/dbt/adapters/spark/column.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.507/dbt/adapters/spark/connections.py` & `in-dbt-spark-1.2.509/dbt/adapters/spark/connections.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.507/dbt/adapters/spark/impl.py` & `in-dbt-spark-1.2.509/dbt/adapters/spark/impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 
 @dataclass
 class SparkConfig(AdapterConfig):
     file_format: str = "openhouse"
     location_root: Optional[str] = None
     partition_by: Optional[Union[List[str], str]] = None
     partition_granularity: Optional[str] = None
+    retention_period: Optional[str] = None
     clustered_by: Optional[Union[List[str], str]] = None
     buckets: Optional[int] = None
     options: Optional[Dict[str, str]] = None
     merge_update_columns: Optional[str] = None
 
 
 class SparkAdapter(SQLAdapter):
```

### Comparing `in-dbt-spark-1.2.507/dbt/adapters/spark/relation.py` & `in-dbt-spark-1.2.509/dbt/adapters/spark/relation.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.507/dbt/adapters/spark/session.py` & `in-dbt-spark-1.2.509/dbt/adapters/spark/session.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.507/dbt/include/spark/macros/adapters.sql` & `in-dbt-spark-1.2.509/dbt/include/spark/macros/adapters.sql`

 * *Files 6% similar despite different names*

```diff
@@ -142,63 +142,26 @@
     {{ create_temporary_view(relation, sql) }}
   {%- else -%}
     {% if config.get('file_format', validator=validation.any[basestring]) == 'delta' %}
       create or replace table {{ relation }}
     {% else %}
       create table {{ relation }}
     {% endif %}
-    {{ file_format_clause() }}
-    {{ options_clause() }}
-    {{ partition_cols(label="partitioned by") }}
-    {{ clustered_cols(label="clustered by") }}
-    {{ location_clause() }}
-    {{ comment_clause() }}
-    as
-      {{ sql }}
-
-  {%- endif %}
-{%- endmacro -%}
-
-{% macro spark__insert_workaround(relation, sql) -%}
-
-  INSERT INTO {{ relation }}
-  {% if (sql is not none) and (sql.lstrip().lower().startswith('with')) -%}
-    select * from ({{ sql }});
-  {%- else -%}
-    {{ sql }};
-  {%- endif %}
-{%- endmacro -%}
-
-{#-- Temporary workaround for lack of support for CTAS in Openhouse #}
-{% macro spark__create_table_as_limit0(temporary, relation, sql) -%}
-  {% if temporary -%}
-    {{ create_temporary_view(relation, sql) }}
-  {%- else -%}
-    {% set file_format = config.get('file_format', validator=validation.any[basestring]) %}
-
-    {% if file_format == 'delta' %}
-      create or replace table {{ relation }}
-    {% else %}
-      create table {{ relation }}
+    {% if config.get('file_format', validator=validation.any[basestring]) != 'openhouse' %}
+      {{ file_format_clause() }}
     {% endif %}
-
     {{ options_clause() }}
-    {{ comment_clause() }}
     {{ partition_cols(label="partitioned by") }}
-
-    {% if file_format != 'openhouse' %}
-      {{ file_format_clause() }}
+    {% if config.get('file_format', validator=validation.any[basestring]) != 'openhouse' %}
       {{ clustered_cols(label="clustered by") }}
       {{ location_clause() }}
     {% endif %}
+    {{ comment_clause() }}
     as
       {{ sql }}
-    {% if file_format == 'openhouse' %}
-      limit 0
-    {% endif %}
 
   {%- endif %}
 {%- endmacro -%}
 
 {% macro spark__create_view_as(relation, sql) -%}
   create or replace view {{ relation }}
   {{ comment_clause() }}
```

### Comparing `in-dbt-spark-1.2.507/dbt/include/spark/macros/apply_grants.sql` & `in-dbt-spark-1.2.509/dbt/include/spark/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.507/dbt/include/spark/macros/catalog.sql` & `in-dbt-spark-1.2.509/dbt/include/spark/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.507/dbt/include/spark/macros/materializations/incremental/strategies.sql` & `in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.507/dbt/include/spark/macros/materializations/seed.sql` & `in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.507/dbt/include/spark/macros/materializations/snapshot.sql` & `in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.507/dbt/include/spark/macros/materializations/table.sql` & `in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/table.sql`

 * *Files 13% similar despite different names*

```diff
@@ -30,25 +30,20 @@
   -- create or replace table instead of dropping, so we don't have the table unavailable
   {% if old_relation and not (old_relation.is_delta and file_format == 'delta') -%}
     {{ adapter.drop_relation(old_relation) }}
   {%- endif %}
 
   -- build model
   {% call statement('main') -%}
-    {% if file_format == 'openhouse' %}
-      {% do run_query(spark__create_table_as_limit0(False, target_relation, sql)) %}
-      {{ spark__insert_workaround(target_relation, sql) }}
-    {% else %}
-      {{ create_table_as(False, target_relation, sql) }}
-    {% endif %}
+    {{ create_table_as(False, target_relation, sql) }}
   {%- endcall %}
 
   {% set should_revoke = should_revoke(old_relation, full_refresh_mode=True) %}
   {% do apply_grants(target_relation, grant_config, should_revoke) %}
-
+  {% do apply_retention(target_relation) %}
   {% do persist_docs(target_relation, model) %}
 
   {{ run_hooks(post_hooks) }}
 
   {{ return({'relations': [target_relation]})}}
 
 {% endmaterialization %}
```

### Comparing `in-dbt-spark-1.2.507/dbt/include/spark/macros/materializations/validate.sql` & `in-dbt-spark-1.2.509/dbt/include/spark/macros/materializations/validate.sql`

 * *Files 9% similar despite different names*

```diff
@@ -85,11 +85,17 @@
     {%- if grant_config is not none %}
         {%- for privilege in grant_config.keys() %}
           {% if privilege.lower() not in ['select', 'manage grants'] %}
             {% do exceptions.raise_compiler_error("For outputs with file_format = 'openhouse', keys in 'grants' map must be one of ('select', 'manage_grants').") %}
           {% endif %}
         {%- endfor -%}
     {% endif %}
+
+    {% if config.get('retention_period', none) is not none %}
+      {% if config.get('partition_by', none) is none %}
+        {% do exceptions.raise_compiler_error("For tables with file_format = 'openhouse' and 'retention_period', 'partition_by' must be supplied") %}
+      {% endif %}
+    {% endif %}
   {% endif %}
 
   {% do return(file_format) %}
 {% endmacro %}
```

### Comparing `in-dbt-spark-1.2.507/dbt/include/spark/macros/utils/dateadd.sql` & `in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.507/dbt/include/spark/macros/utils/datediff.sql` & `in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.507/dbt/include/spark/macros/utils/listagg.sql` & `in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.507/dbt/include/spark/macros/utils/split_part.sql` & `in-dbt-spark-1.2.509/dbt/include/spark/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.507/dbt/include/spark/profile_template.yml` & `in-dbt-spark-1.2.509/dbt/include/spark/profile_template.yml`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.507/in_dbt_spark.egg-info/PKG-INFO` & `in-dbt-spark-1.2.509/in_dbt_spark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: in-dbt-spark
-Version: 1.2.507
+Version: 1.2.509
 Summary: Release for LinkedIn's changes to dbt-spark.
 Home-page: https://github.com/linkedin/in-dbt-spark
 Author: LinkedIn DBT Team
 Author-email: dbt-dev@linkedin.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.2.507 Summary: Release for
+Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.2.509 Summary: Release for
 LinkedIn's changes to dbt-spark. Home-page: https://github.com/linkedin/in-dbt-
 spark Author: LinkedIn DBT Team Author-email: dbt-dev@linkedin.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `in-dbt-spark-1.2.507/in_dbt_spark.egg-info/SOURCES.txt` & `in-dbt-spark-1.2.509/in_dbt_spark.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 dbt/adapters/spark/session.py
 dbt/adapters/spark/spark_utils.py
 dbt/include/spark/__init__.py
 dbt/include/spark/dbt_project.yml
 dbt/include/spark/profile_template.yml
 dbt/include/spark/macros/adapters.sql
 dbt/include/spark/macros/apply_grants.sql
+dbt/include/spark/macros/apply_retention.sql
 dbt/include/spark/macros/catalog.sql
 dbt/include/spark/macros/materializations/seed.sql
 dbt/include/spark/macros/materializations/snapshot.sql
 dbt/include/spark/macros/materializations/table.sql
 dbt/include/spark/macros/materializations/validate.sql
 dbt/include/spark/macros/materializations/view.sql
 dbt/include/spark/macros/materializations/incremental/incremental.sql
```

### Comparing `in-dbt-spark-1.2.507/setup.py` & `in-dbt-spark-1.2.509/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "in-dbt-spark"
-package_version = "1.2.507"
+package_version = "1.2.509"
 dbt_core_version = _get_dbt_core_version()
 description = """Release for LinkedIn's changes to dbt-spark."""
 
 odbc_extras = ["pyodbc>=4.0.30"]
 pyhive_extras = [
     "PyHive[hive]>=0.6.0,<0.7.0",
     "thrift>=0.11.0,<0.16.0",
```

