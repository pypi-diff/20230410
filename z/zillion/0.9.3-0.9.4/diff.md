# Comparing `tmp/zillion-0.9.3.tar.gz` & `tmp/zillion-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zillion-0.9.3.tar", last modified: Tue Apr  4 15:42:38 2023, max compression
+gzip compressed data, was "zillion-0.9.4.tar", last modified: Mon Apr 10 13:30:56 2023, max compression
```

## Comparing `zillion-0.9.3.tar` & `zillion-0.9.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-04 15:42:38.181033 zillion-0.9.3/
--rw-rw-r--   0 kurt      (1000) kurt      (1000)      297 2022-07-15 16:01:20.000000 zillion-0.9.3/AUTHORS.md
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     7783 2022-07-15 16:01:20.000000 zillion-0.9.3/LICENSE
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    31693 2023-04-04 15:42:38.181033 zillion-0.9.3/PKG-INFO
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    31036 2023-04-04 15:42:18.000000 zillion-0.9.3/README.md
--rw-rw-r--   0 kurt      (1000) kurt      (1000)       38 2023-04-04 15:42:38.181033 zillion-0.9.3/setup.cfg
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     2859 2023-03-31 00:50:17.000000 zillion-0.9.3/setup.py
-drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-04 15:42:38.181033 zillion-0.9.3/zillion/
--rw-rw-r--   0 kurt      (1000) kurt      (1000)      507 2022-07-15 16:01:20.000000 zillion-0.9.3/zillion/__init__.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    51932 2023-03-28 16:19:04.000000 zillion-0.9.3/zillion/configs.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    13415 2023-04-01 17:19:44.000000 zillion-0.9.3/zillion/core.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    69321 2023-04-03 19:42:19.000000 zillion-0.9.3/zillion/datasource.py
-drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-04 15:42:38.181033 zillion-0.9.3/zillion/dialects/
--rw-rw-r--   0 kurt      (1000) kurt      (1000)       91 2023-03-23 18:24:15.000000 zillion-0.9.3/zillion/dialects/__init__.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     6313 2022-07-15 16:01:20.000000 zillion-0.9.3/zillion/dialects/conversions.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     4677 2023-03-24 13:49:53.000000 zillion-0.9.3/zillion/dialects/duckdb.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     3700 2022-07-15 16:01:20.000000 zillion-0.9.3/zillion/dialects/mysql.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     4556 2022-07-15 16:01:20.000000 zillion-0.9.3/zillion/dialects/postgresql.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     4609 2022-07-15 16:01:20.000000 zillion-0.9.3/zillion/dialects/sqlite.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    53505 2023-03-23 18:23:26.000000 zillion-0.9.3/zillion/field.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     1711 2023-04-03 13:02:37.000000 zillion-0.9.3/zillion/model.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    36474 2023-04-04 15:39:51.000000 zillion-0.9.3/zillion/nlp.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    83878 2023-04-03 17:49:18.000000 zillion-0.9.3/zillion/report.py
-drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-04 15:42:38.181033 zillion-0.9.3/zillion/scripts/
--rw-rw-r--   0 kurt      (1000) kurt      (1000)        0 2022-07-15 16:01:20.000000 zillion-0.9.3/zillion/scripts/__init__.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    15096 2023-04-04 14:54:06.000000 zillion-0.9.3/zillion/scripts/bootstrap_datasource_config.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)      121 2022-07-15 16:01:20.000000 zillion-0.9.3/zillion/scripts/json_to_yaml.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     2478 2023-04-04 11:18:20.000000 zillion-0.9.3/zillion/scripts/run_report.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)      109 2022-07-15 16:01:20.000000 zillion-0.9.3/zillion/scripts/yaml_to_json.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    16500 2023-04-03 19:12:41.000000 zillion-0.9.3/zillion/sql_utils.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)       44 2023-04-04 15:42:13.000000 zillion-0.9.3/zillion/version.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    39878 2023-04-04 01:10:26.000000 zillion-0.9.3/zillion/warehouse.py
-drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-04 15:42:38.181033 zillion-0.9.3/zillion.egg-info/
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    31693 2023-04-04 15:42:38.000000 zillion-0.9.3/zillion.egg-info/PKG-INFO
--rw-rw-r--   0 kurt      (1000) kurt      (1000)      737 2023-04-04 15:42:38.000000 zillion-0.9.3/zillion.egg-info/SOURCES.txt
--rw-rw-r--   0 kurt      (1000) kurt      (1000)        1 2023-04-04 15:42:38.000000 zillion-0.9.3/zillion.egg-info/dependency_links.txt
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     1050 2023-04-04 15:42:38.000000 zillion-0.9.3/zillion.egg-info/requires.txt
--rw-rw-r--   0 kurt      (1000) kurt      (1000)        8 2023-04-04 15:42:38.000000 zillion-0.9.3/zillion.egg-info/top_level.txt
+drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-10 13:30:56.819146 zillion-0.9.4/
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)      297 2022-07-15 16:01:20.000000 zillion-0.9.4/AUTHORS.md
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     7783 2022-07-15 16:01:20.000000 zillion-0.9.4/LICENSE
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    31693 2023-04-10 13:30:56.819146 zillion-0.9.4/PKG-INFO
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    31036 2023-04-04 15:42:18.000000 zillion-0.9.4/README.md
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)       38 2023-04-10 13:30:56.819146 zillion-0.9.4/setup.cfg
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     2859 2023-03-31 00:50:17.000000 zillion-0.9.4/setup.py
+drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-10 13:30:56.815146 zillion-0.9.4/zillion/
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)      507 2022-07-15 16:01:20.000000 zillion-0.9.4/zillion/__init__.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    51932 2023-03-28 16:19:04.000000 zillion-0.9.4/zillion/configs.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    13415 2023-04-01 17:19:44.000000 zillion-0.9.4/zillion/core.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    69321 2023-04-03 19:42:19.000000 zillion-0.9.4/zillion/datasource.py
+drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-10 13:30:56.819146 zillion-0.9.4/zillion/dialects/
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)       91 2023-03-23 18:24:15.000000 zillion-0.9.4/zillion/dialects/__init__.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     6313 2022-07-15 16:01:20.000000 zillion-0.9.4/zillion/dialects/conversions.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     4677 2023-03-24 13:49:53.000000 zillion-0.9.4/zillion/dialects/duckdb.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     3700 2022-07-15 16:01:20.000000 zillion-0.9.4/zillion/dialects/mysql.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     4556 2022-07-15 16:01:20.000000 zillion-0.9.4/zillion/dialects/postgresql.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     4609 2022-07-15 16:01:20.000000 zillion-0.9.4/zillion/dialects/sqlite.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    53505 2023-03-23 18:23:26.000000 zillion-0.9.4/zillion/field.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     1718 2023-04-10 13:26:28.000000 zillion-0.9.4/zillion/model.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    36392 2023-04-04 15:47:25.000000 zillion-0.9.4/zillion/nlp.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    83878 2023-04-03 17:49:18.000000 zillion-0.9.4/zillion/report.py
+drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-10 13:30:56.819146 zillion-0.9.4/zillion/scripts/
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)        0 2022-07-15 16:01:20.000000 zillion-0.9.4/zillion/scripts/__init__.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    15096 2023-04-04 14:54:06.000000 zillion-0.9.4/zillion/scripts/bootstrap_datasource_config.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)      121 2022-07-15 16:01:20.000000 zillion-0.9.4/zillion/scripts/json_to_yaml.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     2478 2023-04-04 11:18:20.000000 zillion-0.9.4/zillion/scripts/run_report.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)      109 2022-07-15 16:01:20.000000 zillion-0.9.4/zillion/scripts/yaml_to_json.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    16500 2023-04-03 19:12:41.000000 zillion-0.9.4/zillion/sql_utils.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)       44 2023-04-10 13:30:32.000000 zillion-0.9.4/zillion/version.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    39878 2023-04-04 01:10:26.000000 zillion-0.9.4/zillion/warehouse.py
+drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-10 13:30:56.815146 zillion-0.9.4/zillion.egg-info/
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    31693 2023-04-10 13:30:56.000000 zillion-0.9.4/zillion.egg-info/PKG-INFO
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)      737 2023-04-10 13:30:56.000000 zillion-0.9.4/zillion.egg-info/SOURCES.txt
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)        1 2023-04-10 13:30:56.000000 zillion-0.9.4/zillion.egg-info/dependency_links.txt
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     1050 2023-04-10 13:30:56.000000 zillion-0.9.4/zillion.egg-info/requires.txt
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)        8 2023-04-10 13:30:56.000000 zillion-0.9.4/zillion.egg-info/top_level.txt
```

### Comparing `zillion-0.9.3/LICENSE` & `zillion-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zillion-0.9.3/PKG-INFO` & `zillion-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zillion
-Version: 0.9.3
+Version: 0.9.4
 Summary: Make sense of it all.
 Home-page: https://github.com/totalhack/zillion
 Author: totalhack
 Author-email: none@none.com
 Maintainer: totalhack
 License: LGPLv3
 Platform: UNKNOWN
```

### Comparing `zillion-0.9.3/README.md` & `zillion-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `zillion-0.9.3/setup.py` & `zillion-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.3/zillion/configs.py` & `zillion-0.9.4/zillion/configs.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.3/zillion/core.py` & `zillion-0.9.4/zillion/core.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.3/zillion/datasource.py` & `zillion-0.9.4/zillion/datasource.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.3/zillion/dialects/conversions.py` & `zillion-0.9.4/zillion/dialects/conversions.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.3/zillion/dialects/duckdb.py` & `zillion-0.9.4/zillion/dialects/duckdb.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.3/zillion/dialects/mysql.py` & `zillion-0.9.4/zillion/dialects/mysql.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.3/zillion/dialects/postgresql.py` & `zillion-0.9.4/zillion/dialects/postgresql.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.3/zillion/dialects/sqlite.py` & `zillion-0.9.4/zillion/dialects/sqlite.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.3/zillion/field.py` & `zillion-0.9.4/zillion/field.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.3/zillion/model.py` & `zillion-0.9.4/zillion/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,12 +40,12 @@
 if nlp_installed:
     EmbeddingsCache = sa.Table(
         "embeddings_cache",
         zillion_metadata,
         sa.Column("text_hash", sa.String(100), primary_key=True),
         sa.Column("model", sa.String(100), primary_key=True),
         sa.Column("text", sa.Text, nullable=False),
-        sa.Column("vector", sa.BLOB, nullable=False),
+        sa.Column("vector", sa.LargeBinary, nullable=False),
         sa.Column("created_at", sa.DateTime, server_default=sa.func.NOW()),
     )
 
 zillion_metadata.create_all(zillion_engine)
```

### Comparing `zillion-0.9.3/zillion/nlp.py` & `zillion-0.9.4/zillion/nlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,14 @@
                 self.content_payload_key,
                 self.metadata_payload_key,
             )
 
             start = time.time()
             self.client.upsert(
                 collection_name=self.collection_name,
-                # points=rest.Batch(ids=ids, vectors=vectors, payloads=payloads),
                 points=rest.Batch.construct(
                     ids=ids, vectors=[list(v) for v in vectors], payloads=payloads
                 ),
             )
             info(f"Added {len(texts)} texts to Qdrant in {time.time() - start:.2f}s")
             return ids
```

### Comparing `zillion-0.9.3/zillion/report.py` & `zillion-0.9.4/zillion/report.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.3/zillion/scripts/bootstrap_datasource_config.py` & `zillion-0.9.4/zillion/scripts/bootstrap_datasource_config.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.3/zillion/scripts/run_report.py` & `zillion-0.9.4/zillion/scripts/run_report.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.3/zillion/sql_utils.py` & `zillion-0.9.4/zillion/sql_utils.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.3/zillion/warehouse.py` & `zillion-0.9.4/zillion/warehouse.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.3/zillion.egg-info/PKG-INFO` & `zillion-0.9.4/zillion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zillion
-Version: 0.9.3
+Version: 0.9.4
 Summary: Make sense of it all.
 Home-page: https://github.com/totalhack/zillion
 Author: totalhack
 Author-email: none@none.com
 Maintainer: totalhack
 License: LGPLv3
 Platform: UNKNOWN
```

### Comparing `zillion-0.9.3/zillion.egg-info/SOURCES.txt` & `zillion-0.9.4/zillion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zillion-0.9.3/zillion.egg-info/requires.txt` & `zillion-0.9.4/zillion.egg-info/requires.txt`

 * *Files identical despite different names*

