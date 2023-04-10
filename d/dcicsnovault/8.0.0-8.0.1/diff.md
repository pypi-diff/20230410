# Comparing `tmp/dcicsnovault-8.0.0.tar.gz` & `tmp/dcicsnovault-8.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicsnovault-8.0.0.tar", max compression
+gzip compressed data, was "dcicsnovault-8.0.1.tar", max compression
```

## Comparing `dcicsnovault-8.0.0.tar` & `dcicsnovault-8.0.1.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0     1135 2023-04-10 00:41:47.965637 dcicsnovault-8.0.0/LICENSE.txt
--rw-r--r--   0        0        0     6407 2023-04-10 00:41:47.965637 dcicsnovault-8.0.0/README.rst
--rw-r--r--   0        0        0     5556 2023-04-10 00:41:47.969637 dcicsnovault-8.0.0/pyproject.toml
--rw-r--r--   0        0        0     4460 2023-04-10 00:41:47.969637 dcicsnovault-8.0.0/snovault/__init__.py
--rw-r--r--   0        0        0     1942 2023-04-10 00:41:47.969637 dcicsnovault-8.0.0/snovault/aggregated_items.py
--rw-r--r--   0        0        0     8799 2023-04-10 00:41:47.969637 dcicsnovault-8.0.0/snovault/app.py
--rw-r--r--   0        0        0    11879 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/attachment.py
--rw-r--r--   0        0        0     6670 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/batchupgrade.py
--rw-r--r--   0        0        0     1902 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/cache.py
--rw-r--r--   0        0        0     6461 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/calculated.py
--rw-r--r--   0        0        0       10 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/commands/__init__.py
--rw-r--r--   0        0        0     3416 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/commands/check_rendering.py
--rw-r--r--   0        0        0     1608 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/commands/es_index_data.py
--rw-r--r--   0        0        0     1644 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/commands/jsonld_rdf.py
--rw-r--r--   0        0        0     4350 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/commands/profile.py
--rw-r--r--   0        0        0      909 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/commands/wipe_test_indices.py
--rw-r--r--   0        0        0     4183 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/config.py
--rw-r--r--   0        0        0     6352 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/connection.py
--rw-r--r--   0        0        0    14815 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/crud_views.py
--rw-r--r--   0        0        0     4282 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/elasticsearch/__init__.py
--rw-r--r--   0        0        0     4727 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/elasticsearch/cached_views.py
--rw-r--r--   0        0        0    61320 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/elasticsearch/create_mapping.py
--rw-r--r--   0        0        0     7939 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/elasticsearch/es_index_listener.py
--rw-r--r--   0        0        0    18572 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/elasticsearch/esstorage.py
--rw-r--r--   0        0        0    24405 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/elasticsearch/indexer.py
--rw-r--r--   0        0        0    31356 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/elasticsearch/indexer_queue.py
--rw-r--r--   0        0        0    20947 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/elasticsearch/indexer_utils.py
--rw-r--r--   0        0        0      349 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/elasticsearch/interfaces.py
--rw-r--r--   0        0        0    10190 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/elasticsearch/mpindexer.py
--rw-r--r--   0        0        0     8249 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/embed.py
--rw-r--r--   0        0        0     1061 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/etag.py
--rw-r--r--   0        0        0    10835 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/indexing_views.py
--rw-r--r--   0        0        0      774 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/interfaces.py
--rw-r--r--   0        0        0     2229 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/invalidation.py
--rw-r--r--   0        0        0     1639 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/json_renderer.py
--rw-r--r--   0        0        0     2292 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/jsongraph.py
--rw-r--r--   0        0        0     9713 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/jsonld_context.py
--rw-r--r--   0        0        0      846 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/predicates.py
--rw-r--r--   0        0        0       95 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/redis/README.rst
--rw-r--r--   0        0        0       90 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/redis/__init__.py
--rw-r--r--   0        0        0       16 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/redis/interfaces.py
--rw-r--r--   0        0        0     4106 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/redis/redis_connection.py
--rw-r--r--   0        0        0     6495 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/renderers.py
--rw-r--r--   0        0        0    11201 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/resource_views.py
--rw-r--r--   0        0        0    21863 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/resources.py
--rw-r--r--   0        0        0     3450 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/schema_graph.py
--rw-r--r--   0        0        0    16947 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/schema_utils.py
--rw-r--r--   0        0        0     4359 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/schema_views.py
--rw-r--r--   0        0        0      522 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/settings.py
--rw-r--r--   0        0        0     1498 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/standalone_dev.py
--rw-r--r--   0        0        0     4383 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/stats.py
--rw-r--r--   0        0        0    34435 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/storage.py
--rw-r--r--   0        0        0      330 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/AbstractItemTestSecondSubItem.json
--rw-r--r--   0        0        0      300 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/AbstractItemTestSubItem.json
--rw-r--r--   0        0        0     2467 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/EmbeddingTest.json
--rw-r--r--   0        0        0      446 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/NestedEmbeddingContainer.json
--rw-r--r--   0        0        0      883 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/NestedObjectLinkTarget.json
--rw-r--r--   0        0        0      473 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingBiogroupSno.json
--rw-r--r--   0        0        0      968 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingBiosampleSno.json
--rw-r--r--   0        0        0     1082 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingBiosourceSno.json
--rw-r--r--   0        0        0      894 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingCalculatedProperties.json
--rw-r--r--   0        0        0      276 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingDependencies.json
--rw-r--r--   0        0        0      577 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingDownload.json
--rw-r--r--   0        0        0      555 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingIndividualSno.json
--rw-r--r--   0        0        0      730 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingLinkAggregateSno.json
--rw-r--r--   0        0        0      697 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingLinkSourceSno.json
--rw-r--r--   0        0        0      472 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingLinkTargetElasticSearch.json
--rw-r--r--   0        0        0      292 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingLinkTargetSno.json
--rw-r--r--   0        0        0      311 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingMixins.json
--rw-r--r--   0        0        0      845 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingNestedEnabled.json
--rw-r--r--   0        0        0     3721 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingNoteSno.json
--rw-r--r--   0        0        0     1622 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingPostPutPatchSno.json
--rw-r--r--   0        0        0      576 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingServerDefault.json
--rw-r--r--   0        0        0      417 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/mixins.json
--rw-r--r--   0        0        0        0 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/tests/__init__.py
--rw-r--r--   0        0        0     9899 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/tests/authentication.py
--rw-r--r--   0        0        0     2068 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/tests/authorization.py
--rw-r--r--   0        0        0     2210 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/tests/conftest.py
--rw-r--r--   0        0        0      100 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/tests/conftest_settings.py
--rw-r--r--   0        0        0     3086 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/tests/elasticsearch_fixture.py
--rw-r--r--   0        0        0     3921 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/postgresql_fixture.py
--rw-r--r--   0        0        0      852 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/pyramidfixtures.py
--rw-r--r--   0        0        0     3007 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/root.py
--rw-r--r--   0        0        0    59212 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/search.py
--rw-r--r--   0        0        0    17312 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/serverfixtures.py
--rw-r--r--   0        0        0     1857 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/snowflake_hash.py
--rw-r--r--   0        0        0    20291 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_attachment.py
--rw-r--r--   0        0        0     3932 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_authentication.py
--rw-r--r--   0        0        0     1370 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_calculated.py
--rw-r--r--   0        0        0     8984 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_create_mapping.py
--rw-r--r--   0        0        0     7458 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_embed_utils.py
--rw-r--r--   0        0        0     8823 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_embedding.py
--rw-r--r--   0        0        0    10024 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_es_permissions.py
--rw-r--r--   0        0        0    97497 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_indexing.py
--rw-r--r--   0        0        0    28258 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_invalidation_scope.py
--rw-r--r--   0        0        0     2147 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_key.py
--rw-r--r--   0        0        0     2458 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_link.py
--rw-r--r--   0        0        0     5316 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_logging.py
--rw-r--r--   0        0        0     1134 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_misc.py
--rw-r--r--   0        0        0      373 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_mixins.py
--rw-r--r--   0        0        0    13660 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_post_put_patch.py
--rw-r--r--   0        0        0     1570 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_postgresql_fixture.py
--rw-r--r--   0        0        0     1194 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_schemas.py
--rw-r--r--   0        0        0      952 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_serverfixtures.py
--rw-r--r--   0        0        0      484 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_snowflake_hash.py
--rw-r--r--   0        0        0     4267 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_standalone_dev.py
--rw-r--r--   0        0        0     2211 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_stats.py
--rw-r--r--   0        0        0    13062 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_storage.py
--rw-r--r--   0        0        0     1291 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_upgrader.py
--rw-r--r--   0        0        0     6635 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_util.py
--rw-r--r--   0        0        0    18612 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_views.py
--rw-r--r--   0        0        0     4621 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/testappfixtures.py
--rw-r--r--   0        0        0      688 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/testing_key.py
--rw-r--r--   0        0        0      677 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/testing_upgrader.py
--rw-r--r--   0        0        0    26232 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/testing_views.py
--rw-r--r--   0        0        0     1342 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/toolfixtures.py
--rw-r--r--   0        0        0     4031 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tools.py
--rw-r--r--   0        0        0     7605 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/typeinfo.py
--rw-r--r--   0        0        0     8124 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/upgrader.py
--rw-r--r--   0        0        0    45963 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/util.py
--rw-r--r--   0        0        0     5460 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/validation.py
--rw-r--r--   0        0        0     5718 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/validators.py
--rw-r--r--   0        0        0     9042 1970-01-01 00:00:00.000000 dcicsnovault-8.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1135 2023-04-10 18:53:44.992983 dcicsnovault-8.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     6407 2023-04-10 18:53:44.992983 dcicsnovault-8.0.1/README.rst
+-rw-r--r--   0        0        0     5556 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4460 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/__init__.py
+-rw-r--r--   0        0        0     1942 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/aggregated_items.py
+-rw-r--r--   0        0        0     8799 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/app.py
+-rw-r--r--   0        0        0    11879 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/attachment.py
+-rw-r--r--   0        0        0     6670 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/batchupgrade.py
+-rw-r--r--   0        0        0     1902 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/cache.py
+-rw-r--r--   0        0        0     6461 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/calculated.py
+-rw-r--r--   0        0        0       10 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/commands/__init__.py
+-rw-r--r--   0        0        0     3416 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/commands/check_rendering.py
+-rw-r--r--   0        0        0     1608 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/commands/es_index_data.py
+-rw-r--r--   0        0        0     1644 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/commands/jsonld_rdf.py
+-rw-r--r--   0        0        0     4350 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/commands/profile.py
+-rw-r--r--   0        0        0      909 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/commands/wipe_test_indices.py
+-rw-r--r--   0        0        0     4183 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/config.py
+-rw-r--r--   0        0        0     6352 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/connection.py
+-rw-r--r--   0        0        0    14815 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/crud_views.py
+-rw-r--r--   0        0        0     4282 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     4727 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/elasticsearch/cached_views.py
+-rw-r--r--   0        0        0    61320 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/elasticsearch/create_mapping.py
+-rw-r--r--   0        0        0     7939 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/elasticsearch/es_index_listener.py
+-rw-r--r--   0        0        0    18572 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/elasticsearch/esstorage.py
+-rw-r--r--   0        0        0    24405 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/elasticsearch/indexer.py
+-rw-r--r--   0        0        0    31356 2023-04-10 18:53:44.996983 dcicsnovault-8.0.1/snovault/elasticsearch/indexer_queue.py
+-rw-r--r--   0        0        0    20947 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/elasticsearch/indexer_utils.py
+-rw-r--r--   0        0        0      349 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/elasticsearch/interfaces.py
+-rw-r--r--   0        0        0    10190 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/elasticsearch/mpindexer.py
+-rw-r--r--   0        0        0     8249 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/embed.py
+-rw-r--r--   0        0        0     1061 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/etag.py
+-rw-r--r--   0        0        0    10835 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/indexing_views.py
+-rw-r--r--   0        0        0      774 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/interfaces.py
+-rw-r--r--   0        0        0     2229 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/invalidation.py
+-rw-r--r--   0        0        0     1639 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/json_renderer.py
+-rw-r--r--   0        0        0     2292 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/jsongraph.py
+-rw-r--r--   0        0        0     9713 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/jsonld_context.py
+-rw-r--r--   0        0        0      846 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/predicates.py
+-rw-r--r--   0        0        0       95 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/redis/README.rst
+-rw-r--r--   0        0        0       90 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/redis/__init__.py
+-rw-r--r--   0        0        0       16 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/redis/interfaces.py
+-rw-r--r--   0        0        0     4106 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/redis/redis_connection.py
+-rw-r--r--   0        0        0     6495 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/renderers.py
+-rw-r--r--   0        0        0    11201 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/resource_views.py
+-rw-r--r--   0        0        0    21863 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/resources.py
+-rw-r--r--   0        0        0     3450 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/schema_graph.py
+-rw-r--r--   0        0        0    16947 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/schema_utils.py
+-rw-r--r--   0        0        0     4359 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/schema_views.py
+-rw-r--r--   0        0        0      522 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/settings.py
+-rw-r--r--   0        0        0     1498 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/standalone_dev.py
+-rw-r--r--   0        0        0     4383 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/stats.py
+-rw-r--r--   0        0        0    34834 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/storage.py
+-rw-r--r--   0        0        0      330 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/AbstractItemTestSecondSubItem.json
+-rw-r--r--   0        0        0      300 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/AbstractItemTestSubItem.json
+-rw-r--r--   0        0        0     2467 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/EmbeddingTest.json
+-rw-r--r--   0        0        0      446 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/NestedEmbeddingContainer.json
+-rw-r--r--   0        0        0      883 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/NestedObjectLinkTarget.json
+-rw-r--r--   0        0        0      473 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingBiogroupSno.json
+-rw-r--r--   0        0        0      968 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingBiosampleSno.json
+-rw-r--r--   0        0        0     1082 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingBiosourceSno.json
+-rw-r--r--   0        0        0      894 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingCalculatedProperties.json
+-rw-r--r--   0        0        0      276 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingDependencies.json
+-rw-r--r--   0        0        0      577 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingDownload.json
+-rw-r--r--   0        0        0      555 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingIndividualSno.json
+-rw-r--r--   0        0        0      730 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingLinkAggregateSno.json
+-rw-r--r--   0        0        0      697 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingLinkSourceSno.json
+-rw-r--r--   0        0        0      472 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingLinkTargetElasticSearch.json
+-rw-r--r--   0        0        0      292 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingLinkTargetSno.json
+-rw-r--r--   0        0        0      311 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingMixins.json
+-rw-r--r--   0        0        0      845 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingNestedEnabled.json
+-rw-r--r--   0        0        0     3721 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingNoteSno.json
+-rw-r--r--   0        0        0     1622 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingPostPutPatchSno.json
+-rw-r--r--   0        0        0      576 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/TestingServerDefault.json
+-rw-r--r--   0        0        0      417 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/test_schemas/mixins.json
+-rw-r--r--   0        0        0        0 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/__init__.py
+-rw-r--r--   0        0        0     9899 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/authentication.py
+-rw-r--r--   0        0        0     2068 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/authorization.py
+-rw-r--r--   0        0        0     2210 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/conftest.py
+-rw-r--r--   0        0        0      100 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/conftest_settings.py
+-rw-r--r--   0        0        0     3086 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/elasticsearch_fixture.py
+-rw-r--r--   0        0        0     3921 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/postgresql_fixture.py
+-rw-r--r--   0        0        0      852 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/pyramidfixtures.py
+-rw-r--r--   0        0        0     3007 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/root.py
+-rw-r--r--   0        0        0    59212 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/search.py
+-rw-r--r--   0        0        0    17312 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/serverfixtures.py
+-rw-r--r--   0        0        0     1857 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/snowflake_hash.py
+-rw-r--r--   0        0        0    20332 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_attachment.py
+-rw-r--r--   0        0        0     3932 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_authentication.py
+-rw-r--r--   0        0        0     1370 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_calculated.py
+-rw-r--r--   0        0        0     8984 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_create_mapping.py
+-rw-r--r--   0        0        0     7458 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_embed_utils.py
+-rw-r--r--   0        0        0     8823 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_embedding.py
+-rw-r--r--   0        0        0    10024 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_es_permissions.py
+-rw-r--r--   0        0        0    97622 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_indexing.py
+-rw-r--r--   0        0        0    28258 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_invalidation_scope.py
+-rw-r--r--   0        0        0     2147 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_key.py
+-rw-r--r--   0        0        0     2458 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_link.py
+-rw-r--r--   0        0        0     5316 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_logging.py
+-rw-r--r--   0        0        0     1134 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_misc.py
+-rw-r--r--   0        0        0      373 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_mixins.py
+-rw-r--r--   0        0        0    13660 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_post_put_patch.py
+-rw-r--r--   0        0        0     1570 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_postgresql_fixture.py
+-rw-r--r--   0        0        0     1194 2023-04-10 18:53:45.000983 dcicsnovault-8.0.1/snovault/tests/test_schemas.py
+-rw-r--r--   0        0        0      952 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/test_serverfixtures.py
+-rw-r--r--   0        0        0      484 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/test_snowflake_hash.py
+-rw-r--r--   0        0        0     4267 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/test_standalone_dev.py
+-rw-r--r--   0        0        0     2211 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/test_stats.py
+-rw-r--r--   0        0        0    13182 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/test_storage.py
+-rw-r--r--   0        0        0     1291 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/test_upgrader.py
+-rw-r--r--   0        0        0     6635 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/test_util.py
+-rw-r--r--   0        0        0    18612 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/test_views.py
+-rw-r--r--   0        0        0     4621 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/testappfixtures.py
+-rw-r--r--   0        0        0      688 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/testing_key.py
+-rw-r--r--   0        0        0      677 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/testing_upgrader.py
+-rw-r--r--   0        0        0    26232 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/testing_views.py
+-rw-r--r--   0        0        0     1342 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tests/toolfixtures.py
+-rw-r--r--   0        0        0     4031 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/tools.py
+-rw-r--r--   0        0        0     7605 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/typeinfo.py
+-rw-r--r--   0        0        0     8124 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/upgrader.py
+-rw-r--r--   0        0        0    45963 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/util.py
+-rw-r--r--   0        0        0     5460 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/validation.py
+-rw-r--r--   0        0        0     5718 2023-04-10 18:53:45.004983 dcicsnovault-8.0.1/snovault/validators.py
+-rw-r--r--   0        0        0     9042 1970-01-01 00:00:00.000000 dcicsnovault-8.0.1/PKG-INFO
```

### Comparing `dcicsnovault-8.0.0/LICENSE.txt` & `dcicsnovault-8.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/README.rst` & `dcicsnovault-8.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/pyproject.toml` & `dcicsnovault-8.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicsnovault"
-version = "8.0.0"
+version = "8.0.1"
 description = "Storage support for 4DN Data Portals."
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/snovault"
 repository = "https://github.com/4dn-dcic/snovault"
 documentation = "https://github.com/4dn-dcic/snovault"
```

### Comparing `dcicsnovault-8.0.0/snovault/__init__.py` & `dcicsnovault-8.0.1/snovault/__init__.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/aggregated_items.py` & `dcicsnovault-8.0.1/snovault/aggregated_items.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/app.py` & `dcicsnovault-8.0.1/snovault/app.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/attachment.py` & `dcicsnovault-8.0.1/snovault/attachment.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/batchupgrade.py` & `dcicsnovault-8.0.1/snovault/batchupgrade.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/cache.py` & `dcicsnovault-8.0.1/snovault/cache.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/calculated.py` & `dcicsnovault-8.0.1/snovault/calculated.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/commands/check_rendering.py` & `dcicsnovault-8.0.1/snovault/commands/check_rendering.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/commands/es_index_data.py` & `dcicsnovault-8.0.1/snovault/commands/es_index_data.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/commands/jsonld_rdf.py` & `dcicsnovault-8.0.1/snovault/commands/jsonld_rdf.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/commands/profile.py` & `dcicsnovault-8.0.1/snovault/commands/profile.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/commands/wipe_test_indices.py` & `dcicsnovault-8.0.1/snovault/commands/wipe_test_indices.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/config.py` & `dcicsnovault-8.0.1/snovault/config.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/connection.py` & `dcicsnovault-8.0.1/snovault/connection.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/crud_views.py` & `dcicsnovault-8.0.1/snovault/crud_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/elasticsearch/__init__.py` & `dcicsnovault-8.0.1/snovault/elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/elasticsearch/cached_views.py` & `dcicsnovault-8.0.1/snovault/elasticsearch/cached_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/elasticsearch/create_mapping.py` & `dcicsnovault-8.0.1/snovault/elasticsearch/create_mapping.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/elasticsearch/es_index_listener.py` & `dcicsnovault-8.0.1/snovault/elasticsearch/es_index_listener.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/elasticsearch/esstorage.py` & `dcicsnovault-8.0.1/snovault/elasticsearch/esstorage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/elasticsearch/indexer.py` & `dcicsnovault-8.0.1/snovault/elasticsearch/indexer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/elasticsearch/indexer_queue.py` & `dcicsnovault-8.0.1/snovault/elasticsearch/indexer_queue.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/elasticsearch/indexer_utils.py` & `dcicsnovault-8.0.1/snovault/elasticsearch/indexer_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/elasticsearch/mpindexer.py` & `dcicsnovault-8.0.1/snovault/elasticsearch/mpindexer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/embed.py` & `dcicsnovault-8.0.1/snovault/embed.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/etag.py` & `dcicsnovault-8.0.1/snovault/etag.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/indexing_views.py` & `dcicsnovault-8.0.1/snovault/indexing_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/interfaces.py` & `dcicsnovault-8.0.1/snovault/interfaces.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/invalidation.py` & `dcicsnovault-8.0.1/snovault/invalidation.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/json_renderer.py` & `dcicsnovault-8.0.1/snovault/json_renderer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/jsongraph.py` & `dcicsnovault-8.0.1/snovault/jsongraph.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/jsonld_context.py` & `dcicsnovault-8.0.1/snovault/jsonld_context.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/predicates.py` & `dcicsnovault-8.0.1/snovault/predicates.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/redis/redis_connection.py` & `dcicsnovault-8.0.1/snovault/redis/redis_connection.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/renderers.py` & `dcicsnovault-8.0.1/snovault/renderers.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/resource_views.py` & `dcicsnovault-8.0.1/snovault/resource_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/resources.py` & `dcicsnovault-8.0.1/snovault/resources.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/schema_graph.py` & `dcicsnovault-8.0.1/snovault/schema_graph.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/schema_utils.py` & `dcicsnovault-8.0.1/snovault/schema_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/schema_views.py` & `dcicsnovault-8.0.1/snovault/schema_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/settings.py` & `dcicsnovault-8.0.1/snovault/settings.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/standalone_dev.py` & `dcicsnovault-8.0.1/snovault/standalone_dev.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/stats.py` & `dcicsnovault-8.0.1/snovault/stats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/storage.py` & `dcicsnovault-8.0.1/snovault/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -371,15 +371,17 @@
 
     def get_by_json(self, key, value, item_type, default=None):
         """ Postgres implementation of get_by_json (used for lookup keys) """
         session = self.DBSession()
         try:
             # baked query seem to not work with json
             query = (session.query(CurrentPropertySheet)
-                     .join(CurrentPropertySheet.propsheet, CurrentPropertySheet.resource)
+                     # Rewrittent to use two separate joins per SQLAlchemy 2.0 requirements. -kmp 10-Apr-2023
+                     .join(CurrentPropertySheet.propsheet)
+                     .join(CurrentPropertySheet.resource)
                      .filter(Resource.item_type == item_type,
                              PropertySheet.properties[key].astext == value)
                      )
             data = query.one()
             return data.resource
         except (NoResultFound, MultipleResultsFound):
             return default
@@ -476,15 +478,16 @@
             session.flush()
         except (IntegrityError, FlushError) as e:
             raw_error_msg = get_error_message(e)
             log.error(raw_error_msg)
             msg = 'Cannot update because of one or more conflicting (or undefined) UUIDs'
             raise HTTPConflict(msg)
         assert unique_keys is not None
-        conflicts = [pk for pk in keys_add if session.query(Key).get(pk) is not None]
+        # Formerly session.query(Key).get(pk), rewritten for SA2.0
+        conflicts = [pk for pk in keys_add if session.get(Key, pk) is not None]
         assert conflicts
         msg = 'Keys conflict: %r' % conflicts
         raise HTTPConflict(msg)
 
     def purge_uuid(self, rid):
         # WARNING USE WITH CARE PERMANENTLY DELETES RESOURCES
         session = self.DBSession()
@@ -520,15 +523,15 @@
         }
 
         to_remove = existing - keys_set
         to_add = keys_set - existing
 
         session = self.DBSession()
         for pk in to_remove:
-            key = session.query(Key).get(pk)
+            key = session.get(Key, pk)  # formerly session.query(Key).get(pk), rewritten for SA2.0
             session.delete(key)
 
         for name, value in to_add:
             key = Key(rid=model.rid, name=name, value=value)
             session.add(key)
 
         return to_add, to_remove
@@ -544,15 +547,16 @@
             for link in model.rels
         }
 
         to_remove = existing - rels
         to_add = rels - existing
 
         for rel, target in to_remove:
-            link = session.query(Link).get((source, rel, target))
+            # formerly link = session.query(Link).get((source, rel, target)), rewritten for SA2.0
+            link = session.get(Link, (source, rel, target))
             session.delete(link)
 
         for rel, target in to_add:
             link = Link(source_rid=source, rel=rel, target_rid=target)
             session.add(link)
 
         return to_add, to_remove
@@ -636,15 +640,15 @@
         Returns:
             data from the DB
         """
         blob_id = download_meta['blob_id']
         if isinstance(blob_id, str):
             blob_id = uuid.UUID(blob_id)
         session = self.DBSession()
-        blob = session.query(Blob).get(blob_id)
+        blob = session.get(Blob, blob_id)  # was session.query(Blob).get(blob_id), rewritten for SA2.0
         return blob.data
 
 
 class S3BlobStorage(object):
     """ Handler to blobs we store in S3 """
     def __init__(self, bucket, kms_key_id=None):
         self.bucket = bucket
```

### Comparing `dcicsnovault-8.0.0/snovault/test_schemas/EmbeddingTest.json` & `dcicsnovault-8.0.1/snovault/test_schemas/EmbeddingTest.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/test_schemas/NestedObjectLinkTarget.json` & `dcicsnovault-8.0.1/snovault/test_schemas/NestedObjectLinkTarget.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/test_schemas/TestingBiosampleSno.json` & `dcicsnovault-8.0.1/snovault/test_schemas/TestingBiosampleSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/test_schemas/TestingBiosourceSno.json` & `dcicsnovault-8.0.1/snovault/test_schemas/TestingBiosourceSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/test_schemas/TestingCalculatedProperties.json` & `dcicsnovault-8.0.1/snovault/test_schemas/TestingCalculatedProperties.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/test_schemas/TestingDownload.json` & `dcicsnovault-8.0.1/snovault/test_schemas/TestingDownload.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/test_schemas/TestingIndividualSno.json` & `dcicsnovault-8.0.1/snovault/test_schemas/TestingIndividualSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/test_schemas/TestingLinkAggregateSno.json` & `dcicsnovault-8.0.1/snovault/test_schemas/TestingLinkAggregateSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/test_schemas/TestingLinkSourceSno.json` & `dcicsnovault-8.0.1/snovault/test_schemas/TestingLinkSourceSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/test_schemas/TestingNestedEnabled.json` & `dcicsnovault-8.0.1/snovault/test_schemas/TestingNestedEnabled.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/test_schemas/TestingNoteSno.json` & `dcicsnovault-8.0.1/snovault/test_schemas/TestingNoteSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/test_schemas/TestingPostPutPatchSno.json` & `dcicsnovault-8.0.1/snovault/test_schemas/TestingPostPutPatchSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/test_schemas/TestingServerDefault.json` & `dcicsnovault-8.0.1/snovault/test_schemas/TestingServerDefault.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/authentication.py` & `dcicsnovault-8.0.1/snovault/tests/authentication.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/authorization.py` & `dcicsnovault-8.0.1/snovault/tests/authorization.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/conftest.py` & `dcicsnovault-8.0.1/snovault/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/elasticsearch_fixture.py` & `dcicsnovault-8.0.1/snovault/tests/elasticsearch_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/postgresql_fixture.py` & `dcicsnovault-8.0.1/snovault/tests/postgresql_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/pyramidfixtures.py` & `dcicsnovault-8.0.1/snovault/tests/pyramidfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/root.py` & `dcicsnovault-8.0.1/snovault/tests/root.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/search.py` & `dcicsnovault-8.0.1/snovault/tests/search.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/serverfixtures.py` & `dcicsnovault-8.0.1/snovault/tests/serverfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/snowflake_hash.py` & `dcicsnovault-8.0.1/snovault/tests/snowflake_hash.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/test_attachment.py` & `dcicsnovault-8.0.1/snovault/tests/test_attachment.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,15 @@
     """ TODO: It would be great if this class could be elegantly merged with the previous one.
         Note though that the tests do differ in some subtle ways. For example, when using
         s3blobs, we follow s3 redirects via pre-signed URLs - these URLs are parsed via
         helper function and acquired through boto3 in order to interact through moto. -Will Jan 4 2022
     """
     url = '/testing-downloads/'
 
-    def testing_encrypted_download(self, testapp):
+    def _testing_encrypted_download(self, testapp):  # not a test, just does some setup
         item = {
             'attachment': {
                 'download': 'red-dot.png',
                 'href': RED_DOT,
             },
             'attachment2': {
                 'download': 'blue-dot.png',
@@ -266,32 +266,32 @@
         return res.location
 
     def create_bucket_and_post_download(self, testapp):
         """ Bootstraps moto and creates some data to work with. """
         blob_bucket = 'encoded-4dn-blobs'  # note that this bucket exists but is mocked out here
         conn = boto3.resource('s3', region_name='us-east-1')
         conn.create_bucket(Bucket=blob_bucket)
-        return self.testing_encrypted_download(testapp)
+        return self._testing_encrypted_download(testapp)
 
     @staticmethod
-    def get_attachment_from_s3(client, url):
+    def _get_attachment_from_s3(client, url):
         """ Uses ff_utils.parse_s3_bucket_and_key_url to parse the s3 URL in our data into it's
             bucket, key pairs and acquires/reads the content.
         """
         bucket, key = parse_s3_bucket_and_key_url(url)
         return client.get_object(Bucket=bucket, Key=key)['Body'].read()
 
     def attachment_is_red_dot(self, client, url):
         """ Fails assertion if the url is not the RED_DOT """
-        content = self.get_attachment_from_s3(client, url)
+        content = self._get_attachment_from_s3(client, url)
         assert content == b64decode(RED_DOT.split(',', 1)[1])
 
     def attachment_is_blue_dot(self, client, url):
         """ Fails assertion if the url is not the BLUE_DOT """
-        content = self.get_attachment_from_s3(client, url)
+        content = self._get_attachment_from_s3(client, url)
         assert content == b64decode(BLUE_DOT.split(',', 1)[1])
 
     @mock_s3
     def test_download_create_encrypted(self, encrypted_testapp):
         loc = self.create_bucket_and_post_download(encrypted_testapp)
         res = encrypted_testapp.get(loc)
         attachment = res.json['attachment']
```

### Comparing `dcicsnovault-8.0.0/snovault/tests/test_authentication.py` & `dcicsnovault-8.0.1/snovault/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/test_calculated.py` & `dcicsnovault-8.0.1/snovault/tests/test_calculated.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/test_create_mapping.py` & `dcicsnovault-8.0.1/snovault/tests/test_create_mapping.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/test_embed_utils.py` & `dcicsnovault-8.0.1/snovault/tests/test_embed_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/test_embedding.py` & `dcicsnovault-8.0.1/snovault/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/test_es_permissions.py` & `dcicsnovault-8.0.1/snovault/tests/test_es_permissions.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/test_indexing.py` & `dcicsnovault-8.0.1/snovault/tests/test_indexing.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     # BEFORE THE TEST - just run CM for the TEST_TYPE by default
     create_mapping.run(app, collections=[TEST_TYPE], skip_indexing=True, purge_queue=True)
 
     yield  # run the test
 
     # AFTER THE TEST
     session = app.registry[DBSESSION]
-    connection = session.connection().connect()
+    connection = session.connection()  # was session.connection().connect(), rewritten for SA2.0
     # The reflect=True argument to MetaData was deprecated. Instead, one is supposed to call the .reflect()
     # method after creation. (This comment is transitional and can go away if things seem to work normally.)
     # -kmp 11-May-2020
     # Ref: https://stackoverflow.com/questions/44193823/get-existing-table-using-sqlalchemy-metadata/44205552
     # meta = MetaData(bind=session.connection())
     # meta.reflect()
     # sqlalchemy 1.4 - use TRUNCATE instead of DELETE
@@ -1956,15 +1956,16 @@
 def test_assert_transactions_table_is_gone(app):
     """
     A bit of a strange location for this test, but we need the app and
     serverfixtures to be established (used for indexing)
     """
     session = app.registry[DBSESSION]
     conn = session.connection()
-    conn.connect()
+    # In SQLAlchemy 2.0, it is no longer necessary to explicitly connect.
+    # conn.connect()
     # The reflect=True argument to MetaData was deprecated. Instead, one is supposed to call the .reflect()
     # method after creation. (This comment is transitional and can go away if things seem to work normally.)
     # -kmp 11-May-2020
     # Ref: https://stackoverflow.com/questions/44193823/get-existing-table-using-sqlalchemy-metadata/44205552
     # In SQLAlchemy 1.x, the bind= argument sets a default connectable so that later calls to things like .reflect()
     # don't have to specify it. In SQLAlchemy 2.x, that goes away, and the argument must instead be given explicitly
     # in the .reflect() call. -kmp 8-Mar-2023
```

### Comparing `dcicsnovault-8.0.0/snovault/tests/test_invalidation_scope.py` & `dcicsnovault-8.0.1/snovault/tests/test_invalidation_scope.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/test_key.py` & `dcicsnovault-8.0.1/snovault/tests/test_key.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/test_link.py` & `dcicsnovault-8.0.1/snovault/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/test_logging.py` & `dcicsnovault-8.0.1/snovault/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/test_misc.py` & `dcicsnovault-8.0.1/snovault/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/test_post_put_patch.py` & `dcicsnovault-8.0.1/snovault/tests/test_post_put_patch.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/test_postgresql_fixture.py` & `dcicsnovault-8.0.1/snovault/tests/test_postgresql_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/test_schemas.py` & `dcicsnovault-8.0.1/snovault/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/test_serverfixtures.py` & `dcicsnovault-8.0.1/snovault/tests/test_serverfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/test_standalone_dev.py` & `dcicsnovault-8.0.1/snovault/tests/test_standalone_dev.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/test_stats.py` & `dcicsnovault-8.0.1/snovault/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/test_storage.py` & `dcicsnovault-8.0.1/snovault/tests/test_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,18 +111,19 @@
     resource = session.query(Resource).one()
     props2 = {'foo': 'baz'}
     resource[name] = props2
     session.flush()
     resource = session.query(Resource).one()
     session.flush()
     query = (session.query(CurrentPropertySheet)
-             .join(CurrentPropertySheet.propsheet, CurrentPropertySheet.resource)
+             # Rewrittent to use two separate joins per SQLAlchemy 2.0 requirements. -kmp 10-Apr-2023
+             .join(CurrentPropertySheet.propsheet)
+             .join(CurrentPropertySheet.resource)
              .filter(PropertySheet.properties['foo'].astext == 'baz')
              )
-
     data = query.one()
     assert data.propsheet.properties == props2
 
 
 def test_purge_uuid(session, storage):
     """ Tests full purge of metadata (including revision history). """
     name = 'testdata'
```

### Comparing `dcicsnovault-8.0.0/snovault/tests/test_upgrader.py` & `dcicsnovault-8.0.1/snovault/tests/test_upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/test_util.py` & `dcicsnovault-8.0.1/snovault/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/test_views.py` & `dcicsnovault-8.0.1/snovault/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/testappfixtures.py` & `dcicsnovault-8.0.1/snovault/tests/testappfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/testing_key.py` & `dcicsnovault-8.0.1/snovault/tests/testing_key.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/testing_upgrader.py` & `dcicsnovault-8.0.1/snovault/tests/testing_upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/testing_views.py` & `dcicsnovault-8.0.1/snovault/tests/testing_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tests/toolfixtures.py` & `dcicsnovault-8.0.1/snovault/tests/toolfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/tools.py` & `dcicsnovault-8.0.1/snovault/tools.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/typeinfo.py` & `dcicsnovault-8.0.1/snovault/typeinfo.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/upgrader.py` & `dcicsnovault-8.0.1/snovault/upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/util.py` & `dcicsnovault-8.0.1/snovault/util.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/validation.py` & `dcicsnovault-8.0.1/snovault/validation.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/snovault/validators.py` & `dcicsnovault-8.0.1/snovault/validators.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.0/PKG-INFO` & `dcicsnovault-8.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicsnovault
-Version: 8.0.0
+Version: 8.0.1
 Summary: Storage support for 4DN Data Portals.
 Home-page: https://github.com/4dn-dcic/snovault
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8.1,<3.9
 Classifier: Development Status :: 4 - Beta
```

