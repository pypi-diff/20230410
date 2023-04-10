# Comparing `tmp/trilogy-public-models-0.0.4.tar.gz` & `tmp/trilogy-public-models-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trilogy-public-models-0.0.4.tar", last modified: Sun Mar 12 15:18:37 2023, max compression
+gzip compressed data, was "trilogy-public-models-0.0.6.tar", last modified: Mon Apr 10 01:29:06 2023, max compression
```

## Comparing `trilogy-public-models-0.0.4.tar` & `trilogy-public-models-0.0.6.tar`

### file list

```diff
@@ -1,36 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 15:18:37.638703 trilogy-public-models-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-03-12 15:18:37.634703 trilogy-public-models-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-12 15:18:29.000000 trilogy-public-models-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-12 15:18:37.638703 trilogy-public-models-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-03-12 15:18:29.000000 trilogy-public-models-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 15:18:37.634703 trilogy-public-models-0.0.4/trilogy_public_models/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-12 15:18:29.000000 trilogy-public-models-0.0.4/trilogy_public_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 15:18:37.634703 trilogy-public-models-0.0.4/trilogy_public_models/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 15:18:29.000000 trilogy-public-models-0.0.4/trilogy_public_models/bigquery/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 15:18:37.634703 trilogy-public-models-0.0.4/trilogy_public_models/bigquery/github/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-12 15:18:29.000000 trilogy-public-models-0.0.4/trilogy_public_models/bigquery/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-03-12 15:18:29.000000 trilogy-public-models-0.0.4/trilogy_public_models/bigquery/github/commits.preql
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 15:18:29.000000 trilogy-public-models-0.0.4/trilogy_public_models/bigquery/github/contents.preql
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-12 15:18:29.000000 trilogy-public-models-0.0.4/trilogy_public_models/bigquery/github/datasources.preql
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-12 15:18:29.000000 trilogy-public-models-0.0.4/trilogy_public_models/bigquery/github/entrypoint.preql
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 15:18:29.000000 trilogy-public-models-0.0.4/trilogy_public_models/bigquery/github/files.preql
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-12 15:18:29.000000 trilogy-public-models-0.0.4/trilogy_public_models/bigquery/github/language.preql
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 15:18:29.000000 trilogy-public-models-0.0.4/trilogy_public_models/bigquery/github/licenses.preql
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-12 15:18:29.000000 trilogy-public-models-0.0.4/trilogy_public_models/bigquery/github/repo.preql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 15:18:37.634703 trilogy-public-models-0.0.4/trilogy_public_models/bigquery/stack_overflow/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-12 15:18:29.000000 trilogy-public-models-0.0.4/trilogy_public_models/bigquery/stack_overflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-03-12 15:18:29.000000 trilogy-public-models-0.0.4/trilogy_public_models/bigquery/stack_overflow/answer.preql
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-03-12 15:18:29.000000 trilogy-public-models-0.0.4/trilogy_public_models/bigquery/stack_overflow/badge.preql
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-12 15:18:29.000000 trilogy-public-models-0.0.4/trilogy_public_models/bigquery/stack_overflow/entrypoint.preql
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-03-12 15:18:29.000000 trilogy-public-models-0.0.4/trilogy_public_models/bigquery/stack_overflow/question.preql
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-12 15:18:29.000000 trilogy-public-models-0.0.4/trilogy_public_models/bigquery/stack_overflow/tag.preql
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-03-12 15:18:29.000000 trilogy-public-models-0.0.4/trilogy_public_models/bigquery/stack_overflow/user.preql
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-12 15:18:29.000000 trilogy-public-models-0.0.4/trilogy_public_models/bigquery/stack_overflow/user_metrics.preql
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-12 15:18:29.000000 trilogy-public-models-0.0.4/trilogy_public_models/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-03-12 15:18:29.000000 trilogy-public-models-0.0.4/trilogy_public_models/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 15:18:37.634703 trilogy-public-models-0.0.4/trilogy_public_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-03-12 15:18:37.000000 trilogy-public-models-0.0.4/trilogy_public_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-03-12 15:18:37.000000 trilogy-public-models-0.0.4/trilogy_public_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 15:18:37.000000 trilogy-public-models-0.0.4/trilogy_public_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-12 15:18:37.000000 trilogy-public-models-0.0.4/trilogy_public_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-12 15:18:37.000000 trilogy-public-models-0.0.4/trilogy_public_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:29:06.244178 trilogy-public-models-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-10 01:29:06.244178 trilogy-public-models-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 01:29:06.244178 trilogy-public-models-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:29:06.240178 trilogy-public-models-0.0.6/trilogy_public_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:29:06.240178 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:29:06.240178 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/github/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/github/commits.preql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/github/contents.preql
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/github/datasources.preql
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/github/entrypoint.preql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/github/files.preql
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/github/language.preql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/github/licenses.preql
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/github/repo.preql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:29:06.240178 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/google_search_trends/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/google_search_trends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/google_search_trends/entrypoint.preql
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/google_search_trends/trends.preql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:29:06.240178 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/conference.preql
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/datasources.preql
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/division.preql
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/entrypoint.preql
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/game.preql
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/game_event.preql
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/league.preql
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/player.preql
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/team.preql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:29:06.240178 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/new_york_citibike/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/new_york_citibike/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/new_york_citibike/bikes.preql
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/new_york_citibike/entrypoint.preql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/new_york_citibike/riders.preql
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/new_york_citibike/stations.preql
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/new_york_citibike/trips.preql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:29:06.244178 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/stack_overflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/stack_overflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/stack_overflow/answer.preql
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/stack_overflow/badge.preql
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/stack_overflow/entrypoint.preql
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/stack_overflow/question.preql
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/stack_overflow/tag.preql
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/stack_overflow/user.preql
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/stack_overflow/user_metrics.preql
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:29:06.240178 trilogy-public-models-0.0.6/trilogy_public_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-10 01:29:06.000000 trilogy-public-models-0.0.6/trilogy_public_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-10 01:29:06.000000 trilogy-public-models-0.0.6/trilogy_public_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 01:29:06.000000 trilogy-public-models-0.0.6/trilogy_public_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-10 01:29:06.000000 trilogy-public-models-0.0.6/trilogy_public_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 01:29:06.000000 trilogy-public-models-0.0.6/trilogy_public_models.egg-info/top_level.txt
```

### Comparing `trilogy-public-models-0.0.4/setup.py` & `trilogy-public-models-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     author="",
     author_email="preql-community@gmail.com",
     description="Public trilogy/preql models.",
     long_description=open("README.md").read(),
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(exclude=["dist", "build", "*.tests", "*.tests.*", "tests.*", "tests", "docs", ".github", "", "examples"]),
     package_data={
-        "": ["*.preql"],
+        "": ["*.preql", "py.typed"],
     },
     install_requires=install_requires,
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

### Comparing `trilogy-public-models-0.0.4/trilogy_public_models/__init__.py` & `trilogy-public-models-0.0.6/trilogy_public_models/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from preql import Environment
 from typing import Dict
 from os.path import dirname
 import sys
 
 models: Dict["str", Environment] = {}
 
-__version__ = "0.0.4"
+__version__ = "0.0.6"
 
 for loader, module_name, is_pkg in pkgutil.walk_packages([dirname(__file__)]):
     module = loader.find_module(module_name)  # type: ignore
     if not module:
         continue
     _module = module.load_module(module_name)
     try:
```

### Comparing `trilogy-public-models-0.0.4/trilogy_public_models/bigquery/github/datasources.preql` & `trilogy-public-models-0.0.6/trilogy_public_models/bigquery/github/datasources.preql`

 * *Files identical despite different names*

### Comparing `trilogy-public-models-0.0.4/trilogy_public_models/bigquery/stack_overflow/answer.preql` & `trilogy-public-models-0.0.6/trilogy_public_models/bigquery/stack_overflow/answer.preql`

 * *Files identical despite different names*

### Comparing `trilogy-public-models-0.0.4/trilogy_public_models/bigquery/stack_overflow/question.preql` & `trilogy-public-models-0.0.6/trilogy_public_models/bigquery/stack_overflow/question.preql`

 * *Files identical despite different names*

### Comparing `trilogy-public-models-0.0.4/trilogy_public_models/inventory.py` & `trilogy-public-models-0.0.6/trilogy_public_models/inventory.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 from preql.parser import parse
 
 
 def parse_initial_models(fpath: str) -> Environment:
     files = listdir(dirname(fpath))
 
     for file in files:
-        path = Path(file)
         if file.endswith("entrypoint.preql"):
             with open(join(dirname(fpath), file), "r", encoding="utf-8") as f:
                 contents = f.read()
                 env = Environment(working_path=dirname(fpath))
                 environment, statements = parse(contents, environment=env)
                 return environment
+    raise ValueError("Missing entrypoint.preql")
```

### Comparing `trilogy-public-models-0.0.4/trilogy_public_models/validator.py` & `trilogy-public-models-0.0.6/trilogy_public_models/validator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from preql import Environment
-from preql.core.query_processor import get_datasource_by_concept_and_grain
 from preql.core.models import Grain, Concept, Datasource
 from preql.executor import Executor
 from preql.parser import parse_text
+from preql.core.processing.concept_strategies_v2 import source_concepts
 
 
 def validate_dataset(
     dataset: Datasource, environment: Environment, executor: Executor, dry_run_client
 ):
     # TODO: move ths into executor so we don't need this import
     from google.cloud.bigquery import QueryJobConfig
@@ -18,14 +18,15 @@
     try:
         _, parsed = parse_text(validation_query, environment)
         sql = executor.generator.generate_queries(environment, parsed)
     except Exception as e:
         print(validation_query)
         raise e
     for statement in sql:
+        compiled_sql = ""
         # Start the query, passing in the extra configuration.
         try:
             # for UI execution, cap the limit
             compiled_sql = executor.generator.compile_statement(statement)
 
             # TODO: implement this
             # rs = executor.engine.dry_run(compiled_sql)
@@ -42,18 +43,20 @@
         # TODO: do something interesting with cost modeling?
         #
         print(
             "This query will process {} bytes.".format(query_job.total_bytes_processed)
         )
 
 
+def validate_datasource_grain(datasource):
+    pass
+
+
 def validate_concept(concept: Concept, env):
-    get_datasource_by_concept_and_grain(
-        concept, grain=Grain(components=[concept.with_default_grain()]), environment=env
-    )
+    source_concepts([concept], [], environment=env)
 
 
 def validate_model(model: Environment, executor: Executor, dry_run_client):
     for dataset in model.datasources.values():
         validate_dataset(dataset, model, executor, dry_run_client)
     for concept in model.concepts.values():
         validate_concept(concept, model)
```

### Comparing `trilogy-public-models-0.0.4/trilogy_public_models.egg-info/SOURCES.txt` & `trilogy-public-models-0.0.6/trilogy_public_models.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 setup.py
 trilogy_public_models/__init__.py
 trilogy_public_models/inventory.py
+trilogy_public_models/py.typed
 trilogy_public_models/validator.py
 trilogy_public_models.egg-info/PKG-INFO
 trilogy_public_models.egg-info/SOURCES.txt
 trilogy_public_models.egg-info/dependency_links.txt
 trilogy_public_models.egg-info/requires.txt
 trilogy_public_models.egg-info/top_level.txt
 trilogy_public_models/bigquery/__init__.py
@@ -14,14 +15,33 @@
 trilogy_public_models/bigquery/github/contents.preql
 trilogy_public_models/bigquery/github/datasources.preql
 trilogy_public_models/bigquery/github/entrypoint.preql
 trilogy_public_models/bigquery/github/files.preql
 trilogy_public_models/bigquery/github/language.preql
 trilogy_public_models/bigquery/github/licenses.preql
 trilogy_public_models/bigquery/github/repo.preql
+trilogy_public_models/bigquery/google_search_trends/__init__.py
+trilogy_public_models/bigquery/google_search_trends/entrypoint.preql
+trilogy_public_models/bigquery/google_search_trends/trends.preql
+trilogy_public_models/bigquery/ncaa_basketball/__init__.py
+trilogy_public_models/bigquery/ncaa_basketball/conference.preql
+trilogy_public_models/bigquery/ncaa_basketball/datasources.preql
+trilogy_public_models/bigquery/ncaa_basketball/division.preql
+trilogy_public_models/bigquery/ncaa_basketball/entrypoint.preql
+trilogy_public_models/bigquery/ncaa_basketball/game.preql
+trilogy_public_models/bigquery/ncaa_basketball/game_event.preql
+trilogy_public_models/bigquery/ncaa_basketball/league.preql
+trilogy_public_models/bigquery/ncaa_basketball/player.preql
+trilogy_public_models/bigquery/ncaa_basketball/team.preql
+trilogy_public_models/bigquery/new_york_citibike/__init__.py
+trilogy_public_models/bigquery/new_york_citibike/bikes.preql
+trilogy_public_models/bigquery/new_york_citibike/entrypoint.preql
+trilogy_public_models/bigquery/new_york_citibike/riders.preql
+trilogy_public_models/bigquery/new_york_citibike/stations.preql
+trilogy_public_models/bigquery/new_york_citibike/trips.preql
 trilogy_public_models/bigquery/stack_overflow/__init__.py
 trilogy_public_models/bigquery/stack_overflow/answer.preql
 trilogy_public_models/bigquery/stack_overflow/badge.preql
 trilogy_public_models/bigquery/stack_overflow/entrypoint.preql
 trilogy_public_models/bigquery/stack_overflow/question.preql
 trilogy_public_models/bigquery/stack_overflow/tag.preql
 trilogy_public_models/bigquery/stack_overflow/user.preql
```

