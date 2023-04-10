# Comparing `tmp/relation_validator-0.1.0.tar.gz` & `tmp/relation_validator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relation_validator-0.1.0.tar", max compression
+gzip compressed data, was "relation_validator-0.2.0.tar", max compression
```

## Comparing `relation_validator-0.1.0.tar` & `relation_validator-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-03-25 20:00:56.444020 relation_validator-0.1.0/LICENSE
--rw-r--r--   0        0        0       25 2023-03-25 20:05:25.603143 relation_validator-0.1.0/README.md
--rw-r--r--   0        0        0      607 2023-03-26 13:31:36.366140 relation_validator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-23 22:40:04.740921 relation_validator-0.1.0/src/relation_validator/__init__.py
--rw-r--r--   0        0        0      428 2023-03-26 12:17:32.595706 relation_validator-0.1.0/src/relation_validator/__main__.py
--rw-r--r--   0        0        0        0 2023-03-26 11:57:02.725073 relation_validator-0.1.0/src/relation_validator/utils/__init__.py
--rw-r--r--   0        0        0     1694 2023-03-25 19:06:29.408779 relation_validator-0.1.0/src/relation_validator/utils/utils.py
--rw-r--r--   0        0        0     1004 2023-03-26 12:18:50.431033 relation_validator-0.1.0/src/relation_validator/validator.py
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 relation_validator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-25 20:00:56.444020 relation_validator-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2089 2023-04-10 20:51:03.249986 relation_validator-0.2.0/README.md
+-rw-r--r--   0        0        0      594 2023-04-10 21:06:57.907532 relation_validator-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-23 22:40:04.740921 relation_validator-0.2.0/src/relation_validator/__init__.py
+-rw-r--r--   0        0        0     1457 2023-04-01 21:51:21.270341 relation_validator-0.2.0/src/relation_validator/__main__.py
+-rw-r--r--   0        0        0        0 2023-03-26 11:57:02.725073 relation_validator-0.2.0/src/relation_validator/utils/__init__.py
+-rw-r--r--   0        0        0     2403 2023-04-01 21:33:44.672394 relation_validator-0.2.0/src/relation_validator/utils/utils.py
+-rw-r--r--   0        0        0      768 2023-04-01 21:39:21.268624 relation_validator-0.2.0/src/relation_validator/validator.py
+-rw-r--r--   0        0        0     2880 1970-01-01 00:00:00.000000 relation_validator-0.2.0/PKG-INFO
```

### Comparing `relation_validator-0.1.0/LICENSE` & `relation_validator-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `relation_validator-0.1.0/pyproject.toml` & `relation_validator-0.2.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "relation-validator"
-version = "0.1.0"
+version = "0.2.0"
 description = "This package validates a list of relationships between two terms against the specified ontologies."
-authors = ["Anita Caron <anitacaron@users.noreply.github.com>"]
+authors = ["Anita Caron <anitac@ebi.ac.uk>"]
 readme = "README.md"
-packages = [{include = "relation_validator", from="src"}]
+repository = "https://github.com/anitacaron/relation-validator"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-oaklib = "0.1.73"
 pyaml = "^21.10.1"
 ruamel-yaml = "^0.17.21"
 pandas = "^1.5.3"
+oaklib = "^0.5.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
```

### Comparing `relation_validator-0.1.0/src/relation_validator/utils/utils.py` & `relation_validator-0.2.0/src/relation_validator/utils/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,34 @@
 import os
 import logging
 from ruamel.yaml import YAML, YAMLError
 
+from oaklib.implementations.ubergraph import UbergraphImplementation
+
 QUERY = """
    VALUES (?subject ?object) {{
       {pairs}
     }}
     ?subject {property} ?object .
 """
 
+def query_ubergraph(query):
+  oi = UbergraphImplementation()
+  prefixes = get_prefixes(query, oi.prefix_map().keys())
+  
+  res = oi.query(query=query, prefixes=prefixes)
+  
+  return [r for r in res]
+
+def get_pairs(data):
+  pairs = set()
+  for _, row in data.iterrows():
+    pairs.add(f"({row['s']} {row['o']})")
+  return pairs
+
 def chunks(lst, n):
   for i in range(0, len(lst), n):
       yield lst[i:i + n]
 
 def transform_to_str(list):
   terms_pairs = set()
 
@@ -31,21 +47,21 @@
 
   return terms_s, terms_o
 
 def extract_results(list):
   return set((r["subject"], r["object"]) for r in list)
 
 
-def verify_relationship(query_ubergraph, prefixes, terms_pairs, relationship):
+def verify_relationship(terms_pairs, relationship):
   valid_relationship = set()
   if len(terms_pairs) > 90:
     for chunk in chunks(list(terms_pairs), 90):
-      valid_relationship = valid_relationship.union(extract_results(query_ubergraph(QUERY.format(pairs=" ".join(chunk), property=relationship), prefixes)))
+      valid_relationship = valid_relationship.union(extract_results(query_ubergraph(QUERY.format(pairs=" ".join(chunk), property=relationship))))
   else:
-    valid_relationship = extract_results(query_ubergraph(QUERY.format(pairs=" ".join(list(terms_pairs)), property=relationship), prefixes))
+    valid_relationship = extract_results(query_ubergraph(QUERY.format(pairs=" ".join(list(terms_pairs)), property=relationship)))
   
   non_valid_relationship = terms_pairs - transform_to_str(valid_relationship)
 
   return valid_relationship, non_valid_relationship
 
 
 def get_config(input) -> dict:
@@ -57,8 +73,24 @@
         config = ryaml.load(f)
       except YAMLError as exc:
         logging.info(f'Failed to load config: {config}')
     return config
   else:
     logging.error("Given path has unsupported file extension.")
     return False
-  
+
+def get_prefixes(text, prefix_map):
+  prefixes = []
+  for prefix in prefix_map:
+    if prefix in text:
+      prefixes.append(prefix)
+
+  return prefixes
+
+def get_ontologies_version():
+  QUERY_VERSION = """
+    ?ontology a owl:Ontology .
+    OPTIONAL { ?ontology owl:versionIRI ?version . }
+  """
+  
+  response = query_ubergraph(QUERY_VERSION)
+  return response
```

