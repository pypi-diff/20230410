# Comparing `tmp/dcicsnovault-7.9.9.0b2.tar.gz` & `tmp/dcicsnovault-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicsnovault-7.9.9.0b2.tar", max compression
+gzip compressed data, was "dcicsnovault-8.0.0.tar", max compression
```

## Comparing `dcicsnovault-7.9.9.0b2.tar` & `dcicsnovault-8.0.0.tar`

### file list

```diff
@@ -1,124 +1,123 @@
--rw-r--r--   0        0        0     1135 2020-04-22 15:19:59.681690 dcicsnovault-7.9.9.0b2/LICENSE.txt
--rw-r--r--   0        0        0     6407 2023-02-08 18:10:49.791837 dcicsnovault-7.9.9.0b2/README.rst
--rw-r--r--   0        0        0     5583 2023-03-14 20:43:04.860678 dcicsnovault-7.9.9.0b2/pyproject.toml
--rw-r--r--   0        0        0     4460 2023-03-13 18:29:23.858548 dcicsnovault-7.9.9.0b2/snovault/__init__.py
--rw-r--r--   0        0        0     1942 2023-02-08 18:10:49.809612 dcicsnovault-7.9.9.0b2/snovault/aggregated_items.py
--rw-r--r--   0        0        0     8207 2023-02-08 18:10:49.814590 dcicsnovault-7.9.9.0b2/snovault/app.py
--rw-r--r--   0        0        0    11879 2023-02-08 18:10:49.815230 dcicsnovault-7.9.9.0b2/snovault/attachment.py
--rw-r--r--   0        0        0     6670 2023-02-08 18:10:49.815747 dcicsnovault-7.9.9.0b2/snovault/batchupgrade.py
--rw-r--r--   0        0        0     1902 2020-04-22 15:19:59.997364 dcicsnovault-7.9.9.0b2/snovault/cache.py
--rw-r--r--   0        0        0     6461 2020-10-21 18:02:06.878589 dcicsnovault-7.9.9.0b2/snovault/calculated.py
--rw-r--r--   0        0        0       10 2020-04-22 15:19:59.995285 dcicsnovault-7.9.9.0b2/snovault/commands/__init__.py
--rw-r--r--   0        0        0     3416 2020-09-15 14:05:58.054812 dcicsnovault-7.9.9.0b2/snovault/commands/check_rendering.py
--rw-r--r--   0        0        0     1608 2023-02-08 18:10:49.821555 dcicsnovault-7.9.9.0b2/snovault/commands/es_index_data.py
--rw-r--r--   0        0        0     1644 2020-04-22 15:19:59.991754 dcicsnovault-7.9.9.0b2/snovault/commands/jsonld_rdf.py
--rw-r--r--   0        0        0     4350 2023-02-08 18:10:49.822376 dcicsnovault-7.9.9.0b2/snovault/commands/profile.py
--rw-r--r--   0        0        0      909 2023-02-08 18:10:49.823005 dcicsnovault-7.9.9.0b2/snovault/commands/wipe_test_indices.py
--rw-r--r--   0        0        0     4183 2023-02-08 18:10:49.823623 dcicsnovault-7.9.9.0b2/snovault/config.py
--rw-r--r--   0        0        0     6352 2023-02-08 18:10:49.824292 dcicsnovault-7.9.9.0b2/snovault/connection.py
--rw-r--r--   0        0        0    14815 2023-02-08 18:10:49.829933 dcicsnovault-7.9.9.0b2/snovault/crud_views.py
--rw-r--r--   0        0        0     4282 2023-02-08 18:10:49.830617 dcicsnovault-7.9.9.0b2/snovault/elasticsearch/__init__.py
--rw-r--r--   0        0        0     4727 2023-02-08 18:10:49.835624 dcicsnovault-7.9.9.0b2/snovault/elasticsearch/cached_views.py
--rw-r--r--   0        0        0    60967 2023-03-13 18:29:27.179039 dcicsnovault-7.9.9.0b2/snovault/elasticsearch/create_mapping.py
--rw-r--r--   0        0        0     7939 2023-02-08 18:10:49.846547 dcicsnovault-7.9.9.0b2/snovault/elasticsearch/es_index_listener.py
--rw-r--r--   0        0        0    18572 2023-02-08 18:10:49.851730 dcicsnovault-7.9.9.0b2/snovault/elasticsearch/esstorage.py
--rw-r--r--   0        0        0    24353 2023-02-08 18:10:49.858087 dcicsnovault-7.9.9.0b2/snovault/elasticsearch/indexer.py
--rw-r--r--   0        0        0    31356 2023-02-08 18:10:49.863845 dcicsnovault-7.9.9.0b2/snovault/elasticsearch/indexer_queue.py
--rw-r--r--   0        0        0    20947 2023-02-08 18:10:49.871835 dcicsnovault-7.9.9.0b2/snovault/elasticsearch/indexer_utils.py
--rw-r--r--   0        0        0      349 2021-08-12 19:39:17.751212 dcicsnovault-7.9.9.0b2/snovault/elasticsearch/interfaces.py
--rw-r--r--   0        0        0    10164 2023-02-08 18:10:49.877388 dcicsnovault-7.9.9.0b2/snovault/elasticsearch/mpindexer.py
--rw-r--r--   0        0        0     8249 2021-08-12 19:39:17.757097 dcicsnovault-7.9.9.0b2/snovault/embed.py
--rw-r--r--   0        0        0     1061 2023-02-08 18:10:49.878124 dcicsnovault-7.9.9.0b2/snovault/etag.py
--rw-r--r--   0        0        0    10835 2023-02-08 18:10:49.886932 dcicsnovault-7.9.9.0b2/snovault/indexing_views.py
--rw-r--r--   0        0        0      774 2020-04-22 15:19:59.962133 dcicsnovault-7.9.9.0b2/snovault/interfaces.py
--rw-r--r--   0        0        0     2229 2023-02-08 18:10:49.892547 dcicsnovault-7.9.9.0b2/snovault/invalidation.py
--rw-r--r--   0        0        0     1639 2023-02-08 18:10:49.897621 dcicsnovault-7.9.9.0b2/snovault/json_renderer.py
--rw-r--r--   0        0        0     2292 2020-09-15 14:05:58.093412 dcicsnovault-7.9.9.0b2/snovault/jsongraph.py
--rw-r--r--   0        0        0     9713 2023-02-08 18:10:49.904627 dcicsnovault-7.9.9.0b2/snovault/jsonld_context.py
--rw-r--r--   0        0        0      846 2020-04-22 15:19:59.956023 dcicsnovault-7.9.9.0b2/snovault/predicates.py
--rw-r--r--   0        0        0       95 2023-03-13 18:29:23.865837 dcicsnovault-7.9.9.0b2/snovault/redis/README.rst
--rw-r--r--   0        0        0       90 2023-03-13 18:29:23.872277 dcicsnovault-7.9.9.0b2/snovault/redis/__init__.py
--rw-r--r--   0        0        0       15 2023-03-13 18:29:23.877586 dcicsnovault-7.9.9.0b2/snovault/redis/interfaces.py
--rw-r--r--   0        0        0     4106 2023-03-15 14:15:35.750621 dcicsnovault-7.9.9.0b2/snovault/redis/redis_connection.py
--rw-r--r--   0        0        0     6495 2023-02-08 18:10:49.909627 dcicsnovault-7.9.9.0b2/snovault/renderers.py
--rw-r--r--   0        0        0    11201 2023-02-08 18:10:49.914597 dcicsnovault-7.9.9.0b2/snovault/resource_views.py
--rw-r--r--   0        0        0    21863 2023-03-15 13:51:18.841427 dcicsnovault-7.9.9.0b2/snovault/resources.py
--rw-r--r--   0        0        0     3450 2023-02-08 18:10:49.920477 dcicsnovault-7.9.9.0b2/snovault/schema_graph.py
--rw-r--r--   0        0        0    16947 2023-02-08 18:10:49.925687 dcicsnovault-7.9.9.0b2/snovault/schema_utils.py
--rw-r--r--   0        0        0     4359 2020-04-22 15:19:59.946631 dcicsnovault-7.9.9.0b2/snovault/schema_views.py
--rw-r--r--   0        0        0      522 2023-02-08 18:10:49.926443 dcicsnovault-7.9.9.0b2/snovault/settings.py
--rw-r--r--   0        0        0     1498 2021-08-12 19:39:17.787731 dcicsnovault-7.9.9.0b2/snovault/standalone_dev.py
--rw-r--r--   0        0        0     4383 2023-02-08 18:10:49.931408 dcicsnovault-7.9.9.0b2/snovault/stats.py
--rw-r--r--   0        0        0    34236 2023-03-13 18:29:27.179813 dcicsnovault-7.9.9.0b2/snovault/storage.py
--rw-r--r--   0        0        0      330 2020-04-22 15:19:59.941685 dcicsnovault-7.9.9.0b2/snovault/test_schemas/AbstractItemTestSecondSubItem.json
--rw-r--r--   0        0        0      300 2020-04-22 15:19:59.940748 dcicsnovault-7.9.9.0b2/snovault/test_schemas/AbstractItemTestSubItem.json
--rw-r--r--   0        0        0     2467 2023-02-08 18:10:49.937350 dcicsnovault-7.9.9.0b2/snovault/test_schemas/EmbeddingTest.json
--rw-r--r--   0        0        0      446 2021-08-12 19:39:17.798764 dcicsnovault-7.9.9.0b2/snovault/test_schemas/NestedEmbeddingContainer.json
--rw-r--r--   0        0        0      883 2021-08-12 19:39:17.803883 dcicsnovault-7.9.9.0b2/snovault/test_schemas/NestedObjectLinkTarget.json
--rw-r--r--   0        0        0      473 2021-08-12 19:39:17.810025 dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingBiogroupSno.json
--rw-r--r--   0        0        0      968 2023-02-08 18:10:49.943722 dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingBiosampleSno.json
--rw-r--r--   0        0        0     1082 2021-08-12 19:39:17.820805 dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingBiosourceSno.json
--rw-r--r--   0        0        0      894 2020-09-25 18:48:35.851983 dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingCalculatedProperties.json
--rw-r--r--   0        0        0      276 2020-04-22 15:19:59.938605 dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingDependencies.json
--rw-r--r--   0        0        0      577 2020-04-22 15:19:59.937715 dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingDownload.json
--rw-r--r--   0        0        0      555 2021-08-12 19:39:17.826025 dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingIndividualSno.json
--rw-r--r--   0        0        0      730 2020-04-22 15:19:59.936694 dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingLinkAggregateSno.json
--rw-r--r--   0        0        0      697 2021-08-12 19:39:17.831918 dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingLinkSourceSno.json
--rw-r--r--   0        0        0      472 2021-08-12 19:39:17.838406 dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingLinkTargetElasticSearch.json
--rw-r--r--   0        0        0      292 2020-04-22 15:19:59.934939 dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingLinkTargetSno.json
--rw-r--r--   0        0        0      311 2020-09-25 18:48:35.858197 dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingMixins.json
--rw-r--r--   0        0        0      845 2021-08-12 19:39:18.009063 dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingNestedEnabled.json
--rw-r--r--   0        0        0     3721 2023-02-08 18:10:49.949847 dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingNoteSno.json
--rw-r--r--   0        0        0     1622 2021-08-12 19:39:17.850333 dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingPostPutPatchSno.json
--rw-r--r--   0        0        0      576 2020-04-22 15:19:59.932932 dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingServerDefault.json
--rw-r--r--   0        0        0      417 2020-09-25 18:48:35.864539 dcicsnovault-7.9.9.0b2/snovault/test_schemas/mixins.json
--rw-r--r--   0        0        0        0 2023-02-08 18:10:49.950317 dcicsnovault-7.9.9.0b2/snovault/tests/__init__.py
--rw-r--r--   0        0        0     9899 2023-02-08 18:10:49.951886 dcicsnovault-7.9.9.0b2/snovault/tests/authentication.py
--rw-r--r--   0        0        0     2068 2020-09-15 14:05:58.153546 dcicsnovault-7.9.9.0b2/snovault/tests/authorization.py
--rw-r--r--   0        0        0     2216 2023-02-08 18:10:49.952416 dcicsnovault-7.9.9.0b2/snovault/tests/conftest.py
--rw-r--r--   0        0        0      100 2023-02-08 18:10:49.952678 dcicsnovault-7.9.9.0b2/snovault/tests/conftest_settings.py
--rw-r--r--   0        0        0     3086 2023-02-08 18:10:49.957620 dcicsnovault-7.9.9.0b2/snovault/tests/elasticsearch_fixture.py
--rw-r--r--   0        0        0     3921 2020-09-15 14:05:58.160270 dcicsnovault-7.9.9.0b2/snovault/tests/postgresql_fixture.py
--rw-r--r--   0        0        0      864 2021-08-12 19:39:17.864425 dcicsnovault-7.9.9.0b2/snovault/tests/pyramidfixtures.py
--rw-r--r--   0        0        0     3007 2020-09-15 14:05:58.161510 dcicsnovault-7.9.9.0b2/snovault/tests/root.py
--rw-r--r--   0        0        0    59212 2023-02-08 18:10:49.963341 dcicsnovault-7.9.9.0b2/snovault/tests/search.py
--rw-r--r--   0        0        0    17315 2023-03-13 18:29:27.180569 dcicsnovault-7.9.9.0b2/snovault/tests/serverfixtures.py
--rw-r--r--   0        0        0     1857 2020-04-22 15:19:59.922938 dcicsnovault-7.9.9.0b2/snovault/tests/snowflake_hash.py
--rw-r--r--   0        0        0    20291 2023-02-08 18:10:49.970172 dcicsnovault-7.9.9.0b2/snovault/tests/test_attachment.py
--rw-r--r--   0        0        0     3932 2020-04-22 15:19:59.920849 dcicsnovault-7.9.9.0b2/snovault/tests/test_authentication.py
--rw-r--r--   0        0        0     1370 2021-08-12 19:39:17.883512 dcicsnovault-7.9.9.0b2/snovault/tests/test_calculated.py
--rw-r--r--   0        0        0     8984 2023-02-08 18:10:49.975775 dcicsnovault-7.9.9.0b2/snovault/tests/test_create_mapping.py
--rw-r--r--   0        0        0     7458 2023-02-08 18:10:49.976460 dcicsnovault-7.9.9.0b2/snovault/tests/test_embed_utils.py
--rw-r--r--   0        0        0     8823 2023-03-13 18:29:27.181151 dcicsnovault-7.9.9.0b2/snovault/tests/test_embedding.py
--rw-r--r--   0        0        0    10024 2020-04-22 15:19:59.916562 dcicsnovault-7.9.9.0b2/snovault/tests/test_es_permissions.py
--rw-r--r--   0        0        0    95147 2023-03-13 18:29:27.182098 dcicsnovault-7.9.9.0b2/snovault/tests/test_indexing.py
--rw-r--r--   0        0        0    28258 2023-02-08 18:10:49.984723 dcicsnovault-7.9.9.0b2/snovault/tests/test_invalidation_scope.py
--rw-r--r--   0        0        0     2147 2023-02-08 18:10:49.985400 dcicsnovault-7.9.9.0b2/snovault/tests/test_key.py
--rw-r--r--   0        0        0     2458 2020-04-22 15:19:59.908101 dcicsnovault-7.9.9.0b2/snovault/tests/test_link.py
--rw-r--r--   0        0        0     5316 2023-02-08 18:10:49.991255 dcicsnovault-7.9.9.0b2/snovault/tests/test_logging.py
--rw-r--r--   0        0        0     1134 2023-03-13 18:29:27.182699 dcicsnovault-7.9.9.0b2/snovault/tests/test_misc.py
--rw-r--r--   0        0        0      373 2020-09-25 18:48:35.895147 dcicsnovault-7.9.9.0b2/snovault/tests/test_mixins.py
--rw-r--r--   0        0        0    13660 2023-02-08 18:10:49.997635 dcicsnovault-7.9.9.0b2/snovault/tests/test_post_put_patch.py
--rw-r--r--   0        0        0     1570 2023-02-08 18:10:50.005697 dcicsnovault-7.9.9.0b2/snovault/tests/test_postgresql_fixture.py
--rw-r--r--   0        0        0     1194 2021-08-12 19:39:17.921857 dcicsnovault-7.9.9.0b2/snovault/tests/test_schemas.py
--rw-r--r--   0        0        0      952 2023-02-08 18:10:50.011548 dcicsnovault-7.9.9.0b2/snovault/tests/test_serverfixtures.py
--rw-r--r--   0        0        0      484 2020-09-15 14:05:58.201112 dcicsnovault-7.9.9.0b2/snovault/tests/test_snowflake_hash.py
--rw-r--r--   0        0        0     4267 2021-08-12 19:39:17.928403 dcicsnovault-7.9.9.0b2/snovault/tests/test_standalone_dev.py
--rw-r--r--   0        0        0     2211 2023-02-08 18:10:50.016544 dcicsnovault-7.9.9.0b2/snovault/tests/test_stats.py
--rw-r--r--   0        0        0    13222 2023-03-13 18:29:27.183158 dcicsnovault-7.9.9.0b2/snovault/tests/test_storage.py
--rw-r--r--   0        0        0     1291 2020-04-22 15:19:59.901514 dcicsnovault-7.9.9.0b2/snovault/tests/test_upgrader.py
--rw-r--r--   0        0        0     6635 2023-02-08 18:10:50.017803 dcicsnovault-7.9.9.0b2/snovault/tests/test_util.py
--rw-r--r--   0        0        0    18612 2023-02-08 18:10:50.023759 dcicsnovault-7.9.9.0b2/snovault/tests/test_views.py
--rw-r--r--   0        0        0     4621 2023-02-08 18:10:50.029803 dcicsnovault-7.9.9.0b2/snovault/tests/testappfixtures.py
--rw-r--r--   0        0        0      688 2020-09-15 14:05:58.215074 dcicsnovault-7.9.9.0b2/snovault/tests/testing_key.py
--rw-r--r--   0        0        0      677 2020-09-15 14:05:58.215585 dcicsnovault-7.9.9.0b2/snovault/tests/testing_upgrader.py
--rw-r--r--   0        0        0    26232 2023-02-08 18:10:50.036243 dcicsnovault-7.9.9.0b2/snovault/tests/testing_views.py
--rw-r--r--   0        0        0     1342 2020-09-15 14:05:58.228484 dcicsnovault-7.9.9.0b2/snovault/tests/toolfixtures.py
--rw-r--r--   0        0        0     3394 2023-03-13 18:29:27.183332 dcicsnovault-7.9.9.0b2/snovault/tools.py
--rw-r--r--   0        0        0     7605 2021-08-12 19:39:17.963916 dcicsnovault-7.9.9.0b2/snovault/typeinfo.py
--rw-r--r--   0        0        0     8124 2023-02-08 18:10:50.037173 dcicsnovault-7.9.9.0b2/snovault/upgrader.py
--rw-r--r--   0        0        0    45963 2023-03-13 18:29:27.184109 dcicsnovault-7.9.9.0b2/snovault/util.py
--rw-r--r--   0        0        0     5460 2023-02-08 18:10:50.039101 dcicsnovault-7.9.9.0b2/snovault/validation.py
--rw-r--r--   0        0        0     5718 2023-02-08 18:10:50.044485 dcicsnovault-7.9.9.0b2/snovault/validators.py
--rw-r--r--   0        0        0     8781 1970-01-01 00:00:00.000000 dcicsnovault-7.9.9.0b2/setup.py
--rw-r--r--   0        0        0     9056 1970-01-01 00:00:00.000000 dcicsnovault-7.9.9.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1135 2023-04-10 00:41:47.965637 dcicsnovault-8.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     6407 2023-04-10 00:41:47.965637 dcicsnovault-8.0.0/README.rst
+-rw-r--r--   0        0        0     5556 2023-04-10 00:41:47.969637 dcicsnovault-8.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4460 2023-04-10 00:41:47.969637 dcicsnovault-8.0.0/snovault/__init__.py
+-rw-r--r--   0        0        0     1942 2023-04-10 00:41:47.969637 dcicsnovault-8.0.0/snovault/aggregated_items.py
+-rw-r--r--   0        0        0     8799 2023-04-10 00:41:47.969637 dcicsnovault-8.0.0/snovault/app.py
+-rw-r--r--   0        0        0    11879 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/attachment.py
+-rw-r--r--   0        0        0     6670 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/batchupgrade.py
+-rw-r--r--   0        0        0     1902 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/cache.py
+-rw-r--r--   0        0        0     6461 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/calculated.py
+-rw-r--r--   0        0        0       10 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/commands/__init__.py
+-rw-r--r--   0        0        0     3416 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/commands/check_rendering.py
+-rw-r--r--   0        0        0     1608 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/commands/es_index_data.py
+-rw-r--r--   0        0        0     1644 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/commands/jsonld_rdf.py
+-rw-r--r--   0        0        0     4350 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/commands/profile.py
+-rw-r--r--   0        0        0      909 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/commands/wipe_test_indices.py
+-rw-r--r--   0        0        0     4183 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/config.py
+-rw-r--r--   0        0        0     6352 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/connection.py
+-rw-r--r--   0        0        0    14815 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/crud_views.py
+-rw-r--r--   0        0        0     4282 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     4727 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/elasticsearch/cached_views.py
+-rw-r--r--   0        0        0    61320 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/elasticsearch/create_mapping.py
+-rw-r--r--   0        0        0     7939 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/elasticsearch/es_index_listener.py
+-rw-r--r--   0        0        0    18572 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/elasticsearch/esstorage.py
+-rw-r--r--   0        0        0    24405 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/elasticsearch/indexer.py
+-rw-r--r--   0        0        0    31356 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/elasticsearch/indexer_queue.py
+-rw-r--r--   0        0        0    20947 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/elasticsearch/indexer_utils.py
+-rw-r--r--   0        0        0      349 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/elasticsearch/interfaces.py
+-rw-r--r--   0        0        0    10190 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/elasticsearch/mpindexer.py
+-rw-r--r--   0        0        0     8249 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/embed.py
+-rw-r--r--   0        0        0     1061 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/etag.py
+-rw-r--r--   0        0        0    10835 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/indexing_views.py
+-rw-r--r--   0        0        0      774 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/interfaces.py
+-rw-r--r--   0        0        0     2229 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/invalidation.py
+-rw-r--r--   0        0        0     1639 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/json_renderer.py
+-rw-r--r--   0        0        0     2292 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/jsongraph.py
+-rw-r--r--   0        0        0     9713 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/jsonld_context.py
+-rw-r--r--   0        0        0      846 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/predicates.py
+-rw-r--r--   0        0        0       95 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/redis/README.rst
+-rw-r--r--   0        0        0       90 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/redis/__init__.py
+-rw-r--r--   0        0        0       16 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/redis/interfaces.py
+-rw-r--r--   0        0        0     4106 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/redis/redis_connection.py
+-rw-r--r--   0        0        0     6495 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/renderers.py
+-rw-r--r--   0        0        0    11201 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/resource_views.py
+-rw-r--r--   0        0        0    21863 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/resources.py
+-rw-r--r--   0        0        0     3450 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/schema_graph.py
+-rw-r--r--   0        0        0    16947 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/schema_utils.py
+-rw-r--r--   0        0        0     4359 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/schema_views.py
+-rw-r--r--   0        0        0      522 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/settings.py
+-rw-r--r--   0        0        0     1498 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/standalone_dev.py
+-rw-r--r--   0        0        0     4383 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/stats.py
+-rw-r--r--   0        0        0    34435 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/storage.py
+-rw-r--r--   0        0        0      330 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/AbstractItemTestSecondSubItem.json
+-rw-r--r--   0        0        0      300 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/AbstractItemTestSubItem.json
+-rw-r--r--   0        0        0     2467 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/EmbeddingTest.json
+-rw-r--r--   0        0        0      446 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/NestedEmbeddingContainer.json
+-rw-r--r--   0        0        0      883 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/NestedObjectLinkTarget.json
+-rw-r--r--   0        0        0      473 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingBiogroupSno.json
+-rw-r--r--   0        0        0      968 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingBiosampleSno.json
+-rw-r--r--   0        0        0     1082 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingBiosourceSno.json
+-rw-r--r--   0        0        0      894 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingCalculatedProperties.json
+-rw-r--r--   0        0        0      276 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingDependencies.json
+-rw-r--r--   0        0        0      577 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingDownload.json
+-rw-r--r--   0        0        0      555 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingIndividualSno.json
+-rw-r--r--   0        0        0      730 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingLinkAggregateSno.json
+-rw-r--r--   0        0        0      697 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingLinkSourceSno.json
+-rw-r--r--   0        0        0      472 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingLinkTargetElasticSearch.json
+-rw-r--r--   0        0        0      292 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingLinkTargetSno.json
+-rw-r--r--   0        0        0      311 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingMixins.json
+-rw-r--r--   0        0        0      845 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingNestedEnabled.json
+-rw-r--r--   0        0        0     3721 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingNoteSno.json
+-rw-r--r--   0        0        0     1622 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingPostPutPatchSno.json
+-rw-r--r--   0        0        0      576 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/TestingServerDefault.json
+-rw-r--r--   0        0        0      417 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/test_schemas/mixins.json
+-rw-r--r--   0        0        0        0 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/tests/__init__.py
+-rw-r--r--   0        0        0     9899 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/tests/authentication.py
+-rw-r--r--   0        0        0     2068 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/tests/authorization.py
+-rw-r--r--   0        0        0     2210 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/tests/conftest.py
+-rw-r--r--   0        0        0      100 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/tests/conftest_settings.py
+-rw-r--r--   0        0        0     3086 2023-04-10 00:41:47.973637 dcicsnovault-8.0.0/snovault/tests/elasticsearch_fixture.py
+-rw-r--r--   0        0        0     3921 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/postgresql_fixture.py
+-rw-r--r--   0        0        0      852 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/pyramidfixtures.py
+-rw-r--r--   0        0        0     3007 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/root.py
+-rw-r--r--   0        0        0    59212 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/search.py
+-rw-r--r--   0        0        0    17312 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/serverfixtures.py
+-rw-r--r--   0        0        0     1857 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/snowflake_hash.py
+-rw-r--r--   0        0        0    20291 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_attachment.py
+-rw-r--r--   0        0        0     3932 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_authentication.py
+-rw-r--r--   0        0        0     1370 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_calculated.py
+-rw-r--r--   0        0        0     8984 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_create_mapping.py
+-rw-r--r--   0        0        0     7458 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_embed_utils.py
+-rw-r--r--   0        0        0     8823 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_embedding.py
+-rw-r--r--   0        0        0    10024 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_es_permissions.py
+-rw-r--r--   0        0        0    97497 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_indexing.py
+-rw-r--r--   0        0        0    28258 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_invalidation_scope.py
+-rw-r--r--   0        0        0     2147 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_key.py
+-rw-r--r--   0        0        0     2458 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_link.py
+-rw-r--r--   0        0        0     5316 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_logging.py
+-rw-r--r--   0        0        0     1134 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_misc.py
+-rw-r--r--   0        0        0      373 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_mixins.py
+-rw-r--r--   0        0        0    13660 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_post_put_patch.py
+-rw-r--r--   0        0        0     1570 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_postgresql_fixture.py
+-rw-r--r--   0        0        0     1194 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_schemas.py
+-rw-r--r--   0        0        0      952 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_serverfixtures.py
+-rw-r--r--   0        0        0      484 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_snowflake_hash.py
+-rw-r--r--   0        0        0     4267 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_standalone_dev.py
+-rw-r--r--   0        0        0     2211 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_stats.py
+-rw-r--r--   0        0        0    13062 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_storage.py
+-rw-r--r--   0        0        0     1291 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_upgrader.py
+-rw-r--r--   0        0        0     6635 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_util.py
+-rw-r--r--   0        0        0    18612 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/test_views.py
+-rw-r--r--   0        0        0     4621 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/testappfixtures.py
+-rw-r--r--   0        0        0      688 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/testing_key.py
+-rw-r--r--   0        0        0      677 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/testing_upgrader.py
+-rw-r--r--   0        0        0    26232 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/testing_views.py
+-rw-r--r--   0        0        0     1342 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tests/toolfixtures.py
+-rw-r--r--   0        0        0     4031 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/tools.py
+-rw-r--r--   0        0        0     7605 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/typeinfo.py
+-rw-r--r--   0        0        0     8124 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/upgrader.py
+-rw-r--r--   0        0        0    45963 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/util.py
+-rw-r--r--   0        0        0     5460 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/validation.py
+-rw-r--r--   0        0        0     5718 2023-04-10 00:41:47.977637 dcicsnovault-8.0.0/snovault/validators.py
+-rw-r--r--   0        0        0     9042 1970-01-01 00:00:00.000000 dcicsnovault-8.0.0/PKG-INFO
```

### Comparing `dcicsnovault-7.9.9.0b2/LICENSE.txt` & `dcicsnovault-8.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/README.rst` & `dcicsnovault-8.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/pyproject.toml` & `dcicsnovault-8.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicsnovault"
-version = "7.9.9.0b2"  # first redis version
+version = "8.0.0"
 description = "Storage support for 4DN Data Portals."
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/snovault"
 repository = "https://github.com/4dn-dcic/snovault"
 documentation = "https://github.com/4dn-dcic/snovault"
@@ -40,15 +40,15 @@
 # TODO: This is a backport of Python's statistics library for versions earlier than Python 3.4,
 #       so may no longer be needed. Something to investigate later. -kmp 20-Feb-2020
 # "backports.statistics" = "0.1.0"
 botocore = ">=1.27.36"  # no particular version required, but this speeds up search
 boto3 = ">=1.24.36"  # no particular version required, but this speeds up search
 elasticsearch = "7.13.4"  # versions >= 7.14.0 lock out AWS ES
 elasticsearch_dsl = "^7.4.0"
-dcicutils = "^6.9.9.0b0"
+dcicutils = "^7.0.0"
 future = ">=0.15.2,<1"
 html5lib = ">=1.1"  # experimental, should be OK now that we're not using moto server
 humanfriendly = "^1.44.9"
 jsonschema_serialize_fork = "^2.1.1"
 netaddr = ">=0.8.0,<1"
 passlib = "^1.7.4"
 psutil = "^5.9.0"
@@ -77,15 +77,15 @@
 # TODO: Investigate whether a major version upgrade is allowable for 'venusian'.
 venusian = "^1.2.0"
 WebOb = "^1.8.7"
 WebTest = "^2.0.35"
 WSGIProxy2 = "0.4.2"
 xlrd = "^1.0.0"
 "zope.deprecation" = "^4.4.0"
-"zope.interface" = "^4.7.2"
+"zope.interface" = ">=4.7.2,<6"
 "zope.sqlalchemy" = "1.6"
 pytest-redis = "^2.0.0"
 redis = "^4.5.1"
 
 [tool.poetry.dev-dependencies]
 botocore-stubs = ">=1.27.36"  # no particular version required, but this speeds up search
 boto3-stubs = ">=1.24.36"  # no particular version required, but this speeds up search
```

### Comparing `dcicsnovault-7.9.9.0b2/snovault/__init__.py` & `dcicsnovault-8.0.0/snovault/__init__.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/aggregated_items.py` & `dcicsnovault-8.0.0/snovault/aggregated_items.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/app.py` & `dcicsnovault-8.0.0/snovault/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,25 +57,36 @@
         timeout = settings.get('postgresql.statement_timeout')
         if timeout:
             timeout = int(timeout) * 1000
             set_postgresql_statement_timeout(engine, timeout)
     return engine
 
 
-def set_postgresql_statement_timeout(engine, timeout=20 * 1000):
+def set_postgresql_statement_timeout(engine, timeout: int = 20 * 1000):
     """
     Prevent Postgres waiting indefinitely for a lock.
+
+    :param engine: a database engine
+    :param timeout: a number of milliseconds to set for as statement_timeout
     """
 
     @event.listens_for(engine, 'connect')
     def connect(dbapi_connection, connection_record):
         ignored(connection_record)
+        timeout_ms = timeout
+        if not isinstance(timeout_ms, int):
+            # This coercion will truncate 3.5 to 3, but so would the %d below,
+            # and we have long used that. But the real purpose of introducing
+            # this coercion is to get a ValueError if a string other than a
+            # representation of a number slips through, to seal out accidental injection.
+            # -kmp 6-Apr-2023
+            timeout_ms = int(timeout_ms)
         cursor = dbapi_connection.cursor()
         try:
-            cursor.execute("SET statement_timeout TO %d" % timeout)
+            cursor.execute("SET statement_timeout TO %d" % timeout_ms)
         except psycopg2.Error:
             dbapi_connection.rollback()
         finally:
             cursor.close()
             dbapi_connection.commit()
```

### Comparing `dcicsnovault-7.9.9.0b2/snovault/attachment.py` & `dcicsnovault-8.0.0/snovault/attachment.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/batchupgrade.py` & `dcicsnovault-8.0.0/snovault/batchupgrade.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/cache.py` & `dcicsnovault-8.0.0/snovault/cache.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/calculated.py` & `dcicsnovault-8.0.0/snovault/calculated.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/commands/check_rendering.py` & `dcicsnovault-8.0.0/snovault/commands/check_rendering.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/commands/es_index_data.py` & `dcicsnovault-8.0.0/snovault/commands/es_index_data.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/commands/jsonld_rdf.py` & `dcicsnovault-8.0.0/snovault/commands/jsonld_rdf.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/commands/profile.py` & `dcicsnovault-8.0.0/snovault/commands/profile.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/commands/wipe_test_indices.py` & `dcicsnovault-8.0.0/snovault/commands/wipe_test_indices.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/config.py` & `dcicsnovault-8.0.0/snovault/config.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/connection.py` & `dcicsnovault-8.0.0/snovault/connection.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/crud_views.py` & `dcicsnovault-8.0.0/snovault/crud_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/elasticsearch/__init__.py` & `dcicsnovault-8.0.0/snovault/elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/elasticsearch/cached_views.py` & `dcicsnovault-8.0.0/snovault/elasticsearch/cached_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/elasticsearch/create_mapping.py` & `dcicsnovault-8.0.0/snovault/elasticsearch/create_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,31 +11,32 @@
 import datetime
 import json
 import logging
 import structlog
 import time
 
 from collections import OrderedDict
-from dcicutils.misc_utils import ignored
+from dcicutils.misc_utils import ignored  # , VirtualApp
 from elasticsearch.exceptions import (
     TransportError,
     RequestError,
     ConnectionTimeout
 )
 from elasticsearch.helpers import scan
 from elasticsearch_dsl import Search
 from functools import reduce
 from itertools import chain
 from pyramid.paster import get_app
 from timeit import default_timer as timer
 from ..interfaces import COLLECTIONS, TYPES
 from dcicutils.log_utils import set_logging
 from dcicutils.misc_utils import as_seconds
-from ..commands.es_index_data import run as run_index_data
+# from ..commands.es_index_data import run as run_index_data
 from ..schema_utils import combine_schemas
+from ..tools import make_indexer_testapp
 from ..util import (
     add_default_embeds, IndexSettings,
     NUM_SHARDS, NUM_REPLICAS, SEARCH_MAX, KW_IGNORE_ABOVE, MIN_NGRAM,
     MAX_NGRAM, NESTED_ENABLED, REFRESH_INTERVAL
 )
 from .indexer_utils import (
     get_namespaced_index,
@@ -1165,22 +1166,23 @@
         return res
 
     # use type_sort_key fxn to sort + flatten uuids_to_index
     for itype in sorted(uuids_to_index.keys(), key=type_sort_key):
         to_index_list.extend(uuids_to_index[itype])
     return to_index_list
 
-
-def run_indexing(app, indexing_uuids):
-    """
-    indexing_uuids is a set of uuids that should be reindexed. If global args
-    are available, then this will spawn a new process to run indexing with.
-    Otherwise, run with the current INDEXER
-    """
-    run_index_data(app, uuids=indexing_uuids)
+# Will thinks this is no longer needed. -kmp 11-Mar-2023
+#
+# def run_indexing(app, indexing_uuids):
+#     """
+#     indexing_uuids is a set of uuids that should be reindexed. If global args
+#     are available, then this will spawn a new process to run indexing with.
+#     Otherwise, run with the current INDEXER
+#     """
+#     run_index_data(app, uuids=indexing_uuids)
 
 
 def run(app, collections=None, dry_run=False, check_first=False, skip_indexing=False,
         index_diff=False, strict=False, sync_index=False, print_count_only=False,
         purge_queue=False, item_order=None):
     """
     Run create_mapping. Has the following options:
@@ -1333,17 +1335,22 @@
                         ))
                         # NOTE: invalidation scope computation not possible here since there is no set of diffs
                         all_assc_uuids, _ = find_uuids_for_indexing(registry, all_uuids_to_index, i_type)
                         uuids_to_index[i_type] = all_assc_uuids - to_subtract
                 log.error('___SYNC INDEXING WITH STRICT=FALSE MAY CAUSE REV_LINK INCONSISTENCY___')
             # sort by-type uuids into one list and index synchronously
             to_index_list = flatten_and_sort_uuids(app.registry, uuids_to_index, item_order)
-            log.info('\n___UUIDS TO INDEX (SYNC)___: %s\n' % len(to_index_list),
+            log.info(f'\n___UUIDS TO INDEX (SYNC)___: {to_index_list}\n',
                      cat='uuids to index', count=len(to_index_list))
-            run_indexing(app, to_index_list)
+
+            # Will suggested this substitute way to implement this indexing action. -kmp 11-Mar-2023
+            vapp = make_indexer_testapp(app)
+            vapp.post_json('/index', {'record': True, 'uuids': to_index_list})
+            # run_indexing(app, to_index_list)
+
         else:
             # if non-strict and attempting to reindex a ton, it is faster
             # just to strictly reindex all items
             use_strict = strict or total_reindex
             if len_all_uuids > 50000 and not use_strict:
                 log.warning('___MAPPING ALL ITEMS WITH STRICT=TRUE TO SAVE TIME___')
                 # get all the uuids from EVERY item type
```

### Comparing `dcicsnovault-7.9.9.0b2/snovault/elasticsearch/es_index_listener.py` & `dcicsnovault-8.0.0/snovault/elasticsearch/es_index_listener.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/elasticsearch/esstorage.py` & `dcicsnovault-8.0.0/snovault/elasticsearch/esstorage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/elasticsearch/indexer.py` & `dcicsnovault-8.0.0/snovault/elasticsearch/indexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from dcicutils.misc_utils import ignorable, ignored
 from elasticsearch.exceptions import (
     ConflictError,
     ConnectionError,
     TransportError,
 )
 from pyramid.view import view_config
+from sqlalchemy import text as psql_text
 from timeit import default_timer as timer
 from urllib3.exceptions import ReadTimeoutError
 from ..interfaces import (
     DBSESSION,
     STORAGE
 )
 from .indexer_utils import get_namespaced_index, find_uuids_for_indexing, filter_invalidation_scope
@@ -172,15 +173,15 @@
         """
         Top level routing between `Indexer.update_objects_sync` (synchronous)
         and `Indexer.update_objects_queue` (asynchronous, usually used).
         Also sets isolation level for the DB connection
         """
         session = request.registry[DBSESSION]()
         connection = session.connection()
-        connection.execute('SET TRANSACTION ISOLATION LEVEL REPEATABLE READ READ ONLY')
+        connection.execute(psql_text('SET TRANSACTION ISOLATION LEVEL REPEATABLE READ READ ONLY'))
 
         # indexing is either run with sync uuids passed through the request
         # (which is synchronous) OR uuids from the queue
         sync_uuids = request.json.get('uuids', None)
 
         # actually index
         if sync_uuids:
```

### Comparing `dcicsnovault-7.9.9.0b2/snovault/elasticsearch/indexer_queue.py` & `dcicsnovault-8.0.0/snovault/elasticsearch/indexer_queue.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/elasticsearch/indexer_utils.py` & `dcicsnovault-8.0.0/snovault/elasticsearch/indexer_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/elasticsearch/mpindexer.py` & `dcicsnovault-8.0.0/snovault/elasticsearch/mpindexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from dcicutils.log_utils import set_logging
 from dcicutils.misc_utils import ignored
 from functools import partial
 from multiprocessing import get_context, cpu_count
 from multiprocessing.pool import Pool
 from pyramid.request import apply_request_extensions
 from pyramid.threadlocal import get_current_request, manager
-from sqlalchemy import orm
+from sqlalchemy import orm, text as psql_text
 
 from ..app import configure_engine
 from ..interfaces import DBSESSION
 from ..storage import register_storage, RDBStorage
 
 from .indexer import INDEXER, Indexer
 from .interfaces import APP_FACTORY
@@ -30,30 +30,30 @@
         return
     config.registry[INDEXER] = MPIndexer(config.registry)
 
 
 # ===== Running in subprocess =====
 
 app = None
+db_engine = None
 
 
 def initializer(app_factory, settings):
     """
     Need to initialize the app for the subprocess.
     As part of this, configue a new database engine and set logging
     """
     signal.signal(signal.SIGINT, signal.SIG_IGN)
 
     # set up global variables to use throughout subprocess
-    global db_engine
-    db_engine = None
     atexit.register(clear_manager_and_dispose_engine)
 
     global app
     app = app_factory(settings, indexer_worker=True, create_tables=False)
+    global db_engine
     db_engine = configure_engine(settings)
 
     # Use `es_server=app.registry.settings.get('elasticsearch.server')` when ES logging is working
     set_logging(in_prod=app.registry.settings.get('production'))
     global log
     log = structlog.get_logger(__name__)
 
@@ -80,15 +80,15 @@
     # configure a sqlalchemy session and set isolation level
     DBSession = orm.scoped_session(orm.sessionmaker(bind=db_engine))
     request.registry[DBSESSION] = DBSession
     # configue RDBStorage. Overide write storage to use new DBSession
     register_storage(request.registry, write_override=RDBStorage(DBSession))
     zope.sqlalchemy.register(DBSession)
     connection = DBSession().connection()
-    connection.execute('SET TRANSACTION ISOLATION LEVEL REPEATABLE READ READ ONLY')
+    connection.execute(psql_text('SET TRANSACTION ISOLATION LEVEL REPEATABLE READ READ ONLY'))
 
     # add the newly created request to the pyramid threadlocal manager
     manager.push({'request': request, 'registry': registry})
     yield
     # remove the session when leaving contextmanager
     request.registry[DBSESSION].remove()
```

### Comparing `dcicsnovault-7.9.9.0b2/snovault/embed.py` & `dcicsnovault-8.0.0/snovault/embed.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/etag.py` & `dcicsnovault-8.0.0/snovault/etag.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/indexing_views.py` & `dcicsnovault-8.0.0/snovault/indexing_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/interfaces.py` & `dcicsnovault-8.0.0/snovault/interfaces.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/invalidation.py` & `dcicsnovault-8.0.0/snovault/invalidation.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/json_renderer.py` & `dcicsnovault-8.0.0/snovault/json_renderer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/jsongraph.py` & `dcicsnovault-8.0.0/snovault/jsongraph.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/jsonld_context.py` & `dcicsnovault-8.0.0/snovault/jsonld_context.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/predicates.py` & `dcicsnovault-8.0.0/snovault/predicates.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/redis/redis_connection.py` & `dcicsnovault-8.0.0/snovault/redis/redis_connection.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/renderers.py` & `dcicsnovault-8.0.0/snovault/renderers.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/resource_views.py` & `dcicsnovault-8.0.0/snovault/resource_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/resources.py` & `dcicsnovault-8.0.0/snovault/resources.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/schema_graph.py` & `dcicsnovault-8.0.0/snovault/schema_graph.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/schema_utils.py` & `dcicsnovault-8.0.0/snovault/schema_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/schema_views.py` & `dcicsnovault-8.0.0/snovault/schema_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/settings.py` & `dcicsnovault-8.0.0/snovault/settings.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/standalone_dev.py` & `dcicsnovault-8.0.0/snovault/standalone_dev.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/stats.py` & `dcicsnovault-8.0.0/snovault/stats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/storage.py` & `dcicsnovault-8.0.0/snovault/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,18 @@
     blob_bucket = registry.settings.get('blob_bucket', None)
     s3_encrypt_key_id = registry.settings.get('s3_encrypt_key_id', None)  # TODO: refactor SettingsKey
     registry[BLOBS] = (S3BlobStorage(blob_bucket, kms_key_id=s3_encrypt_key_id)
                        if blob_bucket
                        else RDBBlobStorage(registry[DBSESSION]))
 
 
+# These 3 versions are known to be compatible, older versions should not be
+# used, odds are 14 can be used as well - Will Sept 13 2022
+POSTGRES_COMPATIBLE_MAJOR_VERSIONS = ['11', '12', '13', '14']
+
 Base = declarative_base()
 
 # baked queries allow for caching of query construction to save Python overhead
 bakery = baked.bakery()
 baked_query_resource = bakery(lambda session: session.query(Resource))
 baked_query_unique_key = bakery(
     lambda session: session.query(Key).options(
```

### Comparing `dcicsnovault-7.9.9.0b2/snovault/test_schemas/EmbeddingTest.json` & `dcicsnovault-8.0.0/snovault/test_schemas/EmbeddingTest.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/test_schemas/NestedObjectLinkTarget.json` & `dcicsnovault-8.0.0/snovault/test_schemas/NestedObjectLinkTarget.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingBiosampleSno.json` & `dcicsnovault-8.0.0/snovault/test_schemas/TestingBiosampleSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingBiosourceSno.json` & `dcicsnovault-8.0.0/snovault/test_schemas/TestingBiosourceSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingCalculatedProperties.json` & `dcicsnovault-8.0.0/snovault/test_schemas/TestingCalculatedProperties.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingDownload.json` & `dcicsnovault-8.0.0/snovault/test_schemas/TestingDownload.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingIndividualSno.json` & `dcicsnovault-8.0.0/snovault/test_schemas/TestingIndividualSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingLinkAggregateSno.json` & `dcicsnovault-8.0.0/snovault/test_schemas/TestingLinkAggregateSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingLinkSourceSno.json` & `dcicsnovault-8.0.0/snovault/test_schemas/TestingLinkSourceSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingNestedEnabled.json` & `dcicsnovault-8.0.0/snovault/test_schemas/TestingNestedEnabled.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingNoteSno.json` & `dcicsnovault-8.0.0/snovault/test_schemas/TestingNoteSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingPostPutPatchSno.json` & `dcicsnovault-8.0.0/snovault/test_schemas/TestingPostPutPatchSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/test_schemas/TestingServerDefault.json` & `dcicsnovault-8.0.0/snovault/test_schemas/TestingServerDefault.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/authentication.py` & `dcicsnovault-8.0.0/snovault/tests/authentication.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/authorization.py` & `dcicsnovault-8.0.0/snovault/tests/authorization.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/conftest.py` & `dcicsnovault-8.0.0/snovault/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 #         if 'Running' in out.decode('utf-8'):
 #             return True
 #         tries -= 1
 #         time.sleep(1)  # give it a sec
 #     return False
 #
 #
-# @pytest.yield_fixture(scope='session', autouse=True)
+# @pytest.fixture(scope='session', autouse=True)
 # def start_moto_server_sqs():
 #     """
 #     Spins off a moto server running sqs, yields to the tests and cleans up.
 #     """
 #     delete_sqs_url = 'SQS_URL' not in os.environ
 #     old_sqs_url = os.environ.get('SQS_URL', None)
 #     server_output = tempfile.TemporaryFile()
```

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/elasticsearch_fixture.py` & `dcicsnovault-8.0.0/snovault/tests/elasticsearch_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/postgresql_fixture.py` & `dcicsnovault-8.0.0/snovault/tests/postgresql_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/pyramidfixtures.py` & `dcicsnovault-8.0.0/snovault/tests/pyramidfixtures.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 from dcicutils.qa_utils import notice_pytest_fixtures
 from pyramid.request import apply_request_extensions
 from pyramid.testing import setUp, tearDown
 from pyramid.threadlocal import manager
 
 
-@pytest.yield_fixture
+@pytest.fixture
 def config():
     yield setUp()
     tearDown()
 
 
-@pytest.yield_fixture
+@pytest.fixture
 def threadlocals(request, dummy_request, registry):
     notice_pytest_fixtures(request, dummy_request, registry)
     manager.push({'request': dummy_request, 'registry': registry})
     yield manager.get()
     manager.pop()
```

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/root.py` & `dcicsnovault-8.0.0/snovault/tests/root.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/search.py` & `dcicsnovault-8.0.0/snovault/tests/search.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/serverfixtures.py` & `dcicsnovault-8.0.0/snovault/tests/serverfixtures.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import webtest
 import webtest.http
 import zope.sqlalchemy
 
 from contextlib import contextmanager
 from dcicutils.misc_utils import ignored, environ_bool
 from dcicutils.qa_utils import notice_pytest_fixtures
+from sqlalchemy import text as psql_text
 from transaction.interfaces import ISynchronizer
 from zope.interface import implementer
 
 from ..app import configure_engine
 from ..storage import Base
 from .elasticsearch_fixture import server_process as elasticsearch_server_process
 from .postgresql_fixture import (
@@ -40,15 +41,15 @@
                 record.msg = record.msg[:self.max_len] + '...'
             return True
 
     logging.getLogger('sqlalchemy.engine.base.Engine').addFilter(Shorten())
 
 
 @pytest.mark.fixture_cost(10)
-@pytest.yield_fixture(scope='session')
+@pytest.fixture(scope='session')
 def engine_url(tmpdir_factory):
     if NO_SERVER_FIXTURES:
         yield 'NO_SERVER_FIXTURES'
         return
 
     notice_pytest_fixtures(tmpdir_factory)
 
@@ -62,15 +63,15 @@
 
     if process.poll() is None:
         process.terminate()
         process.wait()
 
 
 @pytest.mark.fixture_cost(10)
-@pytest.yield_fixture(scope='session')
+@pytest.fixture(scope='session')
 def postgresql_server(tmpdir_factory):
     if NO_SERVER_FIXTURES:
         yield 'NO_SERVER_FIXTURES'
         return
 
     notice_pytest_fixtures(tmpdir_factory)
     tmpdir = tmpdir_factory.mktemp('postgresql', numbered=True)
@@ -92,15 +93,15 @@
 
 @pytest.fixture(scope='session')
 def elasticsearch_server_dir(tmpdir_factory):
     return str(tmpdir_factory.mktemp('elasticsearch', numbered=True))
 
 
 @pytest.mark.fixture_cost(10)
-@pytest.yield_fixture(scope='session')
+@pytest.fixture(scope='session')
 def elasticsearch_server(elasticsearch_server_dir, elasticsearch_host_port, remote_es):
     if NO_SERVER_FIXTURES:
         yield 'NO_SERVER_FIXTURES'
         return
 
     notice_pytest_fixtures(elasticsearch_host_port, remote_es)
     if not remote_es:
@@ -117,15 +118,15 @@
         yield remote_es
 
 
 # http://docs.sqlalchemy.org/en/rel_0_8/orm/session.html#joining-a-session-into-an-external-transaction
 # By binding the SQLAlchemy Session to an external transaction multiple testapp
 # requests can be rolled back at the end of the test.
 
-@pytest.yield_fixture(scope='session')
+@pytest.fixture(scope='session')
 def engine(engine_url):
     if NO_SERVER_FIXTURES:
         yield 'NO_SERVER_FIXTURES'
         return
 
     notice_pytest_fixtures(engine_url)
     engine_settings = {
@@ -135,15 +136,15 @@
         }
     }
 
     engine = configure_engine(engine_settings)
     yield engine
 
 
-@pytest.yield_fixture(scope='session')
+@pytest.fixture(scope='session')
 def conn(engine):
     if NO_SERVER_FIXTURES:
         yield 'NO_SERVER_FIXTURES'
         return
 
     notice_pytest_fixtures(engine)
     conn = engine.connect()
@@ -174,15 +175,15 @@
     if NO_SERVER_FIXTURES:
         return 'NO_SERVER_FIXTURES'
 
     notice_pytest_fixtures(zsa_savepoints, check_constraints)
     return _DBSession
 
 
-@pytest.yield_fixture
+@pytest.fixture
 def external_tx(request, conn):
     if NO_SERVER_FIXTURES:
         yield 'NO_SERVER_FIXTURES'
         return
 
     notice_pytest_fixtures(request)
     # print('BEGIN external_tx')
@@ -204,15 +205,15 @@
 
     notice_pytest_fixtures(request, external_tx, zsa_savepoints, check_constraints)
     transaction_management.begin()
     request.addfinalizer(transaction_management.abort)
     return transaction_management
 
 
-@pytest.yield_fixture(scope='session')
+@pytest.fixture(scope='session')
 def zsa_savepoints(conn):
     """ Place a savepoint at the start of the zope transaction
 
     This means failed requests rollback to the db state when they began rather
     than that at the start of the test.
     """
     notice_pytest_fixtures(conn)
@@ -270,15 +271,15 @@
     if NO_SERVER_FIXTURES:
         return 'NO_SERVER_FIXTURES'
 
     notice_pytest_fixtures(transaction, DBSession)
     return DBSession()
 
 
-@pytest.yield_fixture(scope='session')
+@pytest.fixture(scope='session')
 def check_constraints(conn, _DBSession):
     """
     Check deferred constraints on zope transaction commit.
 
     Deferred foreign key constraints are only checked at the outer transaction
     boundary, not at a savepoint. With the Pyramid transaction bound to a
     subtransaction check them manually.
@@ -306,20 +307,20 @@
             @transaction.addBeforeCommitHook
             def set_constraints():
                 self.state = 'checking'
                 session = _DBSession()
                 session.flush()
                 sp = self.conn.begin_nested()
                 try:
-                    self.conn.execute('SET CONSTRAINTS ALL IMMEDIATE')
+                    self.conn.execute(psql_text('SET CONSTRAINTS ALL IMMEDIATE'))
                 except BaseException:  # even things like keyboard interrupt
                     sp.rollback()
                     raise
                 else:
-                    self.conn.execute('SET CONSTRAINTS ALL DEFERRED')
+                    self.conn.execute(psql_text('SET CONSTRAINTS ALL DEFERRED'))
                 finally:
                     sp.commit()
                     self.state = None
 
     check_constraints = CheckConstraints(conn)
 
     transaction_management.manager.registerSynch(check_constraints)
@@ -392,15 +393,15 @@
         assert counted_events == expected_count, (
                 f"Counter mismatch. Expected {expected_count} but got {counted_events}:\n"
                 + '\n'.join([f"{'*' if ae['counted'] else ' '} {ae['event']}"
                             for ae in annotated_events]))
         self._active = False
 
 
-@pytest.yield_fixture
+@pytest.fixture
 def execute_counter(conn, zsa_savepoints, check_constraints, filter=None):
     """
     This fixture gives you a context manager that can be used to count calls to the SQLAlchemy 'execute' operation.
 
     Using this allows you to find out how many queries are needed to do a particular inquiry or set of inquiries
     using the ORM. Such a test is by nature a bit fragile, since it is bypassing abstraction boundaries, but I think
     the intent is to let the caller check whether joins are happening correctly. If they are not, the likely result
@@ -448,15 +449,15 @@
             })
 
     yield watcher
 
     sqlalchemy.event.remove(conn, 'after_cursor_execute', after_cursor_execute)
 
 
-@pytest.yield_fixture
+@pytest.fixture
 def no_deps(conn, DBSession):
     notice_pytest_fixtures(conn, DBSession)
 
     if NO_SERVER_FIXTURES:
         yield 'NO_SERVER_FIXTURES'
         return
 
@@ -498,15 +499,15 @@
     if NO_SERVER_FIXTURES:
         return 'NO_SERVER_FIXTURES'
 
     return app
 
 
 @pytest.mark.fixture_cost(100)
-@pytest.yield_fixture(scope='session')
+@pytest.fixture(scope='session')
 def wsgi_server(request, wsgi_server_app, wsgi_server_host_port):
     notice_pytest_fixtures(request, wsgi_server_app, wsgi_server_host_port)
 
     if NO_SERVER_FIXTURES:
         yield 'NO_SERVER_FIXTURES'
         return
```

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/snowflake_hash.py` & `dcicsnovault-8.0.0/snovault/tests/snowflake_hash.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/test_attachment.py` & `dcicsnovault-8.0.0/snovault/tests/test_attachment.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/test_authentication.py` & `dcicsnovault-8.0.0/snovault/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/test_calculated.py` & `dcicsnovault-8.0.0/snovault/tests/test_calculated.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/test_create_mapping.py` & `dcicsnovault-8.0.0/snovault/tests/test_create_mapping.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/test_embed_utils.py` & `dcicsnovault-8.0.0/snovault/tests/test_embed_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/test_embedding.py` & `dcicsnovault-8.0.0/snovault/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/test_es_permissions.py` & `dcicsnovault-8.0.0/snovault/tests/test_es_permissions.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/test_indexing.py` & `dcicsnovault-8.0.0/snovault/tests/test_indexing.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from datetime import datetime, timedelta
 from dcicutils.lang_utils import n_of
 from dcicutils.misc_utils import ignored, get_error_message, override_dict
 from dcicutils.qa_utils import ControlledTime, Eventually, notice_pytest_fixtures
 from elasticsearch.exceptions import NotFoundError
 from pyramid.traversal import traverse
-from sqlalchemy import MetaData
+from sqlalchemy import MetaData, text as psql_text
 from unittest import mock
 from zope.sqlalchemy import mark_changed
 
 from .. import util  # The filename util.py, not something in __init__.py
 from .. import main  # Function main actually defined in __init__.py (should maybe be defined elsewhere)
 
 from ..elasticsearch import create_mapping, indexer_utils
@@ -41,41 +41,26 @@
 )
 from ..elasticsearch.indexer import check_sid, SidException
 from ..elasticsearch.indexer_queue import QueueManager
 from ..elasticsearch.indexer_utils import compute_invalidation_scope
 from ..elasticsearch.interfaces import ELASTIC_SEARCH, INDEXER_QUEUE, INDEXER_QUEUE_MIRROR
 from ..interfaces import DBSESSION, STORAGE, COLLECTIONS, TYPES
 from ..storage import Base
-from ..tools import index_n_items_for_testing
+from ..tools import index_n_items_for_testing, delay_rerun, make_es_count_checker
 from ..util import INDEXER_NAMESPACE_FOR_TESTING
 
 from .testing_views import TestingLinkSourceSno
 
 
 notice_pytest_fixtures(TestingLinkSourceSno)
 
 
 pytestmark = [pytest.mark.indexing]
 
 
-def delay_rerun(*args):
-    """ Rerun function for flaky """
-    ignored(args)
-    time.sleep(10)
-    return True
-
-
-def make_es_count_checker(n, *, es, namespaced_index):
-    def es_count_checker():
-        indexed_count = es.count(index=namespaced_index).get('count')
-        assert indexed_count == n
-        return n
-    return es_count_checker
-
-
 TEST_COLL = '/testing-post-put-patch-sno/'
 TEST_TYPE = 'testing_post_put_patch_sno'  # use one collection for testing
 
 # we just need single shard for these tests
 # XXX: use new type
 create_mapping.NUM_SHARDS = 1
 
@@ -105,15 +90,15 @@
     INDEXER_APP_PARAMS = [False]
 elif INDEXER_MODE == "BOTH":
     INDEXER_APP_PARAMS = [False, True]
 else:
     raise Exception("Bad value of INDEXER_MODE: %s. Possible values are MPINDEX, INDEX, and BOTH." % INDEXER_MODE)
 
 
-@pytest.yield_fixture(scope='module', params=INDEXER_APP_PARAMS)  # must happen AFTER scope='session' moto setup
+@pytest.fixture(scope='module', params=INDEXER_APP_PARAMS)  # must happen AFTER scope='session' moto setup
 def app(app_settings, request):
     old_mpindexer = app_settings['mpindexer']
     with override_dict(app_settings, mpindexer=old_mpindexer):  # we plan to set it inside here
         if request.param:  # run tests both with and without mpindexer
             print("TEMPORARILY SETTING mpindexer=True in app_settings")
             app_settings['mpindexer'] = True  # This will get cleaned up by the override_dict
         app = main({}, **app_settings)
@@ -126,15 +111,15 @@
         except AttributeError:
             # TODO: The .bind may be a connection, which doesn't have a .pool, so maybe sometime try this instead?
             #       DBSession.bind.engine.pool.dispose()
             pass
 
 # XXX C4-312: refactor tests so this can be module scope.
 # Having to have to drop DB tables and re-run create_mapping for every test is slow.
-@pytest.yield_fixture(scope='function', autouse=True)
+@pytest.fixture(scope='function', autouse=True)
 def setup_and_teardown(app):
     """
     Run create mapping and purge queue before tests and clear out the
     DB tables after the test
     """
     # BEFORE THE TEST - just run CM for the TEST_TYPE by default
     create_mapping.run(app, collections=[TEST_TYPE], skip_indexing=True, purge_queue=True)
@@ -147,23 +132,23 @@
     # The reflect=True argument to MetaData was deprecated. Instead, one is supposed to call the .reflect()
     # method after creation. (This comment is transitional and can go away if things seem to work normally.)
     # -kmp 11-May-2020
     # Ref: https://stackoverflow.com/questions/44193823/get-existing-table-using-sqlalchemy-metadata/44205552
     # meta = MetaData(bind=session.connection())
     # meta.reflect()
     # sqlalchemy 1.4 - use TRUNCATE instead of DELETE
-    connection.execute('TRUNCATE {} RESTART IDENTITY CASCADE;'.format(
-        ','.join(table.name
-                 for table in reversed(Base.metadata.sorted_tables))))
+    table_names = [table.name for table in reversed(Base.metadata.sorted_tables)]
+    table_names_spec = ','.join(table_names)
+    connection.execute(psql_text(f"TRUNCATE {table_names_spec} RESTART IDENTITY CASCADE;"))
     session.flush()
     mark_changed(session())
     transaction_management.commit()
 
 
-@pytest.yield_fixture(scope='function')
+@pytest.fixture(scope='function')
 def es_based_target(app, testapp):
     # must run create mapping BEFORE posting the ES-based item, since it will
     # cause the underlying item properties in the index to be lost
     create_mapping.run(
         app,
         collections=['testing_link_target_elastic_search'],
         skip_indexing=True
@@ -854,15 +839,15 @@
 
     # lastly, test purge_uuid and delete functionality
     with pytest.raises(webtest.AppError) as excinfo:
         testapp.delete_json('/' + source['uuid'] + '/?purge=True')
     assert 'Item status must equal deleted before purging' in str(excinfo.value)
     del_res1 = testapp.delete_json('/' + source['uuid'])
     assert del_res1.json['status'] == 'success'
-    # this item will still have items linking to it indexing occurs
+    # this item will still have items linking to it until indexing occurs
     with pytest.raises(webtest.AppError) as excinfo:
         testapp.delete_json('/' + source['uuid'] + '/?purge=True')
     assert 'Cannot purge item as other items still link to it' in str(excinfo.value)
     # the source should fail due to outdated sids
     # must manually update _sid_cache on dummy_request for source
     src_sid = dummy_request.registry[STORAGE].write.get_by_uuid(source['uuid']).sid
     dummy_request._sid_cache[source['uuid']] = src_sid
@@ -874,47 +859,63 @@
     valid3 = util.validate_es_content(target_ctxt2, dummy_request, tar_es_res_obj, 'object')
     assert valid3 is False
     indexer_testapp.post_json('/index', {'record': True})
     del_res3 = testapp.delete_json('/' + source['uuid'] + '/?purge=True')
     assert del_res3.json['status'] == 'success'
     assert del_res3.json['notification'] == 'Permanently deleted ' + source['uuid']
     time.sleep(3)
-    # make sure everything has updated on ES
-    check_es_source = es.get(index=namespaced_link_source, id=source['uuid'], ignore=[404])
-    assert check_es_source['found'] is False
-    # source uuid removed from the target uuid
-    check_es_target = es.get(index=namespaced_link_target, id=target['uuid'])
-    uuids_linked_emb2 = [link['uuid'] for link in check_es_target['_source']['linked_uuids_embedded']]
-    assert source['uuid'] not in uuids_linked_emb2
+
+    @Eventually.consistent()
+    def await_not_found():
+        # TODO: Will asks "Should a version of this be available generally?" -kmp 29-Mar-2023
+
+        # make sure everything has updated on ES
+        check_es_source = es.get(index=namespaced_link_source, id=source['uuid'], ignore=[404])
+        assert check_es_source['found'] is False
+
+        # source uuid removed from the target uuid
+        check_es_target = es.get(index=namespaced_link_target, id=target['uuid'])
+        uuids_linked_emb2 = [link['uuid'] for link in check_es_target['_source']['linked_uuids_embedded']]
+        assert source['uuid'] not in uuids_linked_emb2
+
+    await_not_found()
+
     # the source is now purged
     testapp.get('/' + source['uuid'], status=404)
     # make sure check_es_and_cache_linked_sids fails for the purged item
     es_res_emb2 = util.check_es_and_cache_linked_sids(source_ctxt, dummy_request, 'embedded')
     assert es_res_emb2 is None
 
 
-@pytest.mark.flaky
+# @pytest.mark.flaky
 def test_indexing_invalid_sid(app, testapp, indexer_testapp):
+    namespaced_test_type = indexer_utils.get_namespaced_index(app, TEST_TYPE)
+    assert namespaced_test_type
     es = app.registry[ELASTIC_SEARCH]
     # post an item, index, then find version (sid)
     res = testapp.post_json(TEST_COLL, {'required': ''})
     test_uuid = res.json['@graph'][0]['uuid']
-    res = indexer_testapp.post_json('/index', {'record': True})
-    assert res.json['indexing_count'] == 1
-    time.sleep(4)
-    namespaced_test_type = indexer_utils.get_namespaced_index(app, TEST_TYPE)
+
+    index_n_items_for_testing(indexer_testapp, 1)
+    # res = indexer_testapp.post_json('/index', {'record': True})
+    # assert res.json['indexing_count'] == 1
+    # time.sleep(4)
+
     es_item = es.get(index=namespaced_test_type, id=test_uuid)
     initial_version = es_item['_version']  # same as sid
     assert es_item['_source']['max_sid'] == initial_version
 
     # now increment the version and check it
     testapp.patch_json(TEST_COLL + test_uuid, {'required': 'meh'})
-    res = indexer_testapp.post_json('/index', {'record': True})
-    assert res.json['indexing_count'] == 1
-    time.sleep(4)
+
+    index_n_items_for_testing(indexer_testapp, 1)
+    # res = indexer_testapp.post_json('/index', {'record': True})
+    # assert res.json['indexing_count'] == 1
+    # time.sleep(4)
+
     es_item = es.get(index=namespaced_test_type, id=test_uuid)
     assert es_item['_version'] == initial_version + 1
     assert es_item['_source']['max_sid'] == initial_version + 1
 
     # manually cause SidException
     max_sid = app.registry[STORAGE].write.get_max_sid()
     with pytest.raises(SidException):
@@ -943,16 +944,20 @@
         'name': 'idx_source',
         'target': target1['uuid'],
         'uuid': str(uuid.uuid4()),
         'status': 'current',
     }
     testapp.post_json('/testing-link-targets-sno/', target1, status=201)
     testapp.post_json('/testing-link-sources-sno/', source, status=201)
-    indexer_testapp.post_json('/index', {'record': True})
-    time.sleep(2)
+
+    index_n_items_for_testing(indexer_testapp, 2)
+
+    # indexer_testapp.post_json('/index', {'record': True})
+    # time.sleep(2)
+
     namespaced_link_target = indexer_utils.get_namespaced_index(app, 'testing_link_target_sno')
     es_item = es.get(index=namespaced_link_target, id=target1['uuid'])
     initial_version = es_item['_version']
 
     # now try to manually bump an invalid version for the queued item
     # expect it to be recycled to the primary queue and not cause any
     # secondary indexing
@@ -961,17 +966,21 @@
         'sid': initial_version + 2,
         'strict': False,
         'timestamp': datetime.utcnow().isoformat()
     }
     indexer_queue.send_messages([to_queue], target_queue='primary')
     received_secondary = indexer_queue.receive_messages(target_queue='secondary')
     assert len(received_secondary) == 0
+
+    # No point to using index_n_items here because 0 is problematic. -kmp 9-Mar-2023
     res = indexer_testapp.post_json('/index', {'record': True})
     time.sleep(4)
     assert res.json['indexing_count'] == 0
+
+    # TODO: This part needs more work
     # make sure nothing is in secondary queue after calling /index
     received_secondary = indexer_queue.receive_messages(target_queue='secondary')
     assert len(received_secondary) == 0
     # remove the message with invalid sid
     received_deferred = indexer_queue.receive_messages(target_queue='primary')
     assert len(received_deferred) == 1
     indexer_queue.delete_messages(received_deferred, target_queue='primary')
@@ -1088,17 +1097,20 @@
 def test_confirm_mapping(app, testapp, indexer_testapp):
     es = app.registry[ELASTIC_SEARCH]
     # make a dynamic mapping
     namespaced_index = indexer_utils.get_namespaced_index(app, TEST_TYPE)
     es.indices.delete(index=namespaced_index)
     time.sleep(2)
     testapp.post_json(TEST_COLL, {'required': ''})
-    res = indexer_testapp.post_json('/index', {'record': True})
-    assert res.json['indexing_count'] == 1
+
+    index_n_items_for_testing(indexer_testapp, 1)
+    # res = indexer_testapp.post_json('/index', {'record': True})
+    # assert res.json['indexing_count'] == 1
     time.sleep(2)
+
     mapping = create_mapping_by_type(TEST_TYPE, app.registry)
     index_record = build_index_record(mapping, TEST_TYPE)
     tries_taken = confirm_mapping(es, namespaced_index, TEST_TYPE, index_record)
     # 3 tries means it failed to correct, 0 means it was unneeded
     assert 0 < tries_taken < 3
     # test against a live mapping to ensure handling of dynamic mapping works
     run(app, collections=[TEST_TYPE], skip_indexing=True)
@@ -1148,76 +1160,104 @@
 
 @pytest.mark.flaky
 def test_es_purge_uuid(app, testapp, indexer_testapp, session):
     indexer_queue = app.registry[INDEXER_QUEUE]
     es = app.registry[ELASTIC_SEARCH]
     # == Adding new test resource to DB ==
     storage = app.registry[STORAGE]
+
     test_body = {'required': '', 'simple1': 'foo', 'simple2': 'bar'}
-    res = testapp.post_json(TEST_COLL, test_body)
-    test_uuid = res.json['@graph'][0]['uuid']
-    check = storage.get_by_uuid(test_uuid)
+    result = testapp.post_json(TEST_COLL, test_body).json
+    #  print(json.dumps(result, indent=2))
+
+    test_uuid = result['@graph'][0]['uuid']
+    print(f"test_uuid={test_uuid}")
 
+    check = storage.get_by_uuid(test_uuid)
     assert str(check.uuid) == test_uuid
 
-    # Then index it:
+    print("Indexing...")
+
+    # TODO: Maybe instead do this? -kmp 10-Mar-2023
+    # index_n_items_for_testing(indexer_testapp, 1, initial_wait_seconds=2)
+
     create_mapping.run(app, collections=[TEST_TYPE], sync_index=True)
     indexer_queue.clear_queue()
-    # time.sleep(4)
+    time.sleep(4)
 
     @Eventually.consistent()
     def ensure_uuid_not_in_es():
+        print("Trying ensure_uuid_not_in_es...")
         # Now ensure that we do have it in ES:
         try:
             namespaced_index = indexer_utils.get_namespaced_index(app, TEST_TYPE)
             es_item = es.get(index=namespaced_index, id=test_uuid)
         except Exception as e:
             raise AssertionError(f"Couldn't find item uuid. {get_error_message(e)}")
         item_uuid = es_item.get('_source', {}).get('uuid')
         assert item_uuid == test_uuid
         return namespaced_index, es_item, item_uuid
 
     namespaced_index, es_item, item_uuid = ensure_uuid_not_in_es()
 
+    print("Indexing complete.")
+
     check_post_from_rdb = storage.write.get_by_uuid(test_uuid)
     assert check_post_from_rdb is not None
 
     assert es_item['_source']['embedded']['simple1'] == test_body['simple1']
     assert es_item['_source']['embedded']['simple2'] == test_body['simple2']
 
+    print("Getting revisions...")
+
     # The actual delete
     revisions = testapp.get('/' + test_uuid + '/@@revision-history').json['revisions']
     assert len(revisions) == 1
-    storage.purge_uuid(test_uuid, TEST_TYPE)
+
+    print("Found 1 revision. Purging...")
+
+    storage.purge_uuid(rid=test_uuid, item_type=TEST_TYPE)
 
     # Riddle me this: above^ delete supposedly fails if the below is not commented out? - Will 04/23/21
     # revisions = testapp.get('/' + test_uuid + '/@@revision-history').json['revisions']
     # assert len(revisions) == 1  # es_items have no revision history
 
+    print("Purge complete. Checking DB...")
+
     @Eventually.consistent()
     def check_rdb_2():
-
+        print("Trying check_rdb_2...")
         check_post_from_rdb_2 = storage.write.get_by_uuid(test_uuid)
         assert check_post_from_rdb_2 is None
 
     check_rdb_2()
 
+    print("DB ok. Checking ES...")
+
     @Eventually.consistent()
     def check_es_2():
+        print("Trying check_es_2...")
         # time.sleep(5)  # Allow time for ES API to send network request to ES server to perform delete.
         check_post_from_es_2 = es.get(index=namespaced_index, id=test_uuid, ignore=[404])
         assert check_post_from_es_2['found'] is False
 
     check_es_2()
 
+    print("Purge results verified for DB and ES. Getting revision history...")
+
     # Now that all the es work is done, test es item revision history
 
     revisions = testapp.get('/' + test_uuid + '/@@revision-history').json['revisions']
     assert len(revisions) == 1  # es_items have no revision history
 
+    print("1 revision found. All good.")
+
+    # TODO: None of these changes are needed, and issues can happen on teardown. Maybe something a commit or abort?
+    # transaction_management.abort()
+
 
 @pytest.mark.flaky
 def test_create_mapping_check_first(app, testapp, indexer_testapp):
     es = app.registry[ELASTIC_SEARCH]
     # get the initial mapping
     mapping = create_mapping_by_type(TEST_TYPE, app.registry)
     index_record = build_index_record(mapping, TEST_TYPE)
@@ -1400,123 +1440,161 @@
     print("Deleting test item via testapp (with purge)")
     testapp.delete_json('/' + test_uuid + '?purge=True')  # purge fully
     print("Checking test item gone from DB.")
     assert not rdbstorage.get_by_uuid(test_uuid)  # should not get now
     print("All done.")
 
 
-@pytest.mark.flaky(max_runs=3, rerun_filter=delay_rerun)
+# @pytest.mark.flaky(max_runs=3, rerun_filter=delay_rerun)
 def test_aggregated_items(app, testapp, indexer_testapp):
     """
     Test that the item aggregation works, which only occurs when indexing
     is actually run. This test does the following:
     - Post a TestingLinkAggregateSno, which links to 2 TestingLinkSourceSno
     - Check aggregated-items view for the item; should be empty before indexing
     - Index and retrieve the TestingLinkAggregateSno from ES
     - Check that the aggregations worked correctly
     - Patch the TestingLinkAggregateSno to only 1 TestingLinkSourceSno, index
     - Ensure that the aggregated_items changed, checking ES
     - Ensure that duplicate aggregated_items are deduplicated
     - Check aggregated-items view; should now match ES results
     """
+
     es = app.registry[ELASTIC_SEARCH]
     # first, run create mapping with the indices we will use
     namespaced_aggregate = indexer_utils.get_namespaced_index(app, 'testing_link_aggregate_sno')
-    create_mapping.run(
-        app,
-        collections=['testing_link_target_sno', 'testing_link_aggregate_sno'],
-        skip_indexing=True
-    )
+
     # generate a uuid for the aggregate item
     agg_res_uuid = str(uuid.uuid4())
-    target1 = {'name': 'one', 'uuid': '775795d3-4410-4114-836b-8eeecf1d0c2f'}
-    target2 = {'name': 'two', 'uuid': '775795d3-4410-4114-836b-8eeecf1daabc'}
+    target_uuid1 = '775795d3-4410-4114-836b-8eeecf1d0c2f'
+    target_uuid2 = '775795d3-4410-4114-836b-8eeecf1daabc'
+    target1 = {'name': 'one', 'uuid': target_uuid1}
+    target2 = {'name': 'two', 'uuid': target_uuid2}
     aggregated = {
         'name': 'A',
         'targets': [
             {
                 'test_description': 'target one',
-                'target': '775795d3-4410-4114-836b-8eeecf1d0c2f'
+                'target': target_uuid1,
             },
             {
                 'test_description': 'target two',
-                'target': '775795d3-4410-4114-836b-8eeecf1daabc'
+                'target': target_uuid2,
             }
         ],
         'uuid': agg_res_uuid,
         'status': 'current'
     }
-    # you can do stuff like this and it will take effect
-    # app.registry['types']['testing_link_aggregate_sno'].aggregated_items['targets'] = (
-    #    ['target.name', 'test_description'])
-    testapp.post_json('/testing-link-targets-sno/', target1, status=201)
-    testapp.post_json('/testing-link-targets-sno/', target2, status=201)
-    agg_res = testapp.post_json('/testing-link-aggregates-sno/', aggregated, status=201)
-    agg_res_atid = agg_res.json['@graph'][0]['@id']
-    # ensure that aggregated-items view shows nothing before indexing
-    pre_agg_view = testapp.get(agg_res_atid + '@@aggregated-items', status=200).json
-    assert pre_agg_view['@id'] == agg_res_atid
-    assert pre_agg_view['aggregated_items'] == {}
-    # wait for the items to index
-    indexer_testapp.post_json('/index', {'record': True})
-    time.sleep(2)
-    # wait for test-link-aggregated item to index
-    doc_count = es.count(index=namespaced_aggregate).get('count')
-    tries = 0
-    while doc_count < 1 and tries < 5:
-        time.sleep(4)
-        doc_count = es.count(index=namespaced_aggregate).get('count')
-        tries += 1
-    assert doc_count == 1
-    es_agg_res = es.get(index=namespaced_aggregate, id=agg_res_uuid)
-    assert 'aggregated_items' in es_agg_res['_source']
-    es_agg_items = es_agg_res['_source']['aggregated_items']
-    assert 'targets' in es_agg_items
-    assert len(es_agg_items['targets']) == 2
-    for idx, target_agg in enumerate(es_agg_items['targets']):
-        # order of targets should be maintained
-        assert target_agg['parent'] == agg_res.json['@graph'][0]['@id']
-        assert target_agg['embedded_path'] == 'targets'
-        if idx == 0:
-            assert target_agg['item']['test_description'] == 'target one'
-            assert target_agg['item']['target']['uuid'] == target1['uuid']
-        else:
-            assert target_agg['item']['test_description'] == 'target two'
-            assert target_agg['item']['target']['uuid'] == target2['uuid']
-    # now make sure they get updated on a patch
-    # use duplicate items, which should be deduplicated if all aggregated
-    # content (including parent) is exactly the same
-    testapp.patch_json(
-        '/testing-link-aggregates-sno/' + aggregated['uuid'],
-        {'targets': [
-            {'test_description': 'target one revised',
-             'target': '775795d3-4410-4114-836b-8eeecf1d0c2f'},
-            {'test_description': 'target one revised',
-             'target': '775795d3-4410-4114-836b-8eeecf1d0c2f'},
-            {'test_description': 'target one revised2',
-             'target': '775795d3-4410-4114-836b-8eeecf1d0c2f'}
-        ]}
-    )
-    indexer_testapp.post_json('/index', {'record': True})
-    time.sleep(10)  # be lazy and just wait a bit
-    es_agg_res = es.get(index=namespaced_aggregate, id=agg_res_uuid)
-    assert 'aggregated_items' in es_agg_res['_source']
-    es_agg_items = es_agg_res['_source']['aggregated_items']
-    assert 'targets' in es_agg_items
-    assert len(es_agg_items['targets']) == 2
-    assert es_agg_items['targets'][0]['item']['test_description'] == 'target one revised'
-    assert es_agg_items['targets'][1]['item']['test_description'] == 'target one revised2'
-    # check that the aggregated-items view now works
-    post_agg_view = testapp.get(agg_res_atid + '@@aggregated-items', status=200).json
-    assert post_agg_view['@id'] == agg_res_atid
-    assert post_agg_view['aggregated_items'] == es_agg_res['_source']['aggregated_items']
-    # clean up the test items
-    testapp.patch_json('/testing-link-aggregates-sno/' + aggregated['uuid'],
-                       {'targets': []})
-    indexer_testapp.post_json('/index', {'record': True})
+
+    try:
+
+        create_mapping.run(
+            app,
+            collections=['testing_link_target_sno', 'testing_link_aggregate_sno'],
+            skip_indexing=True
+        )
+
+        time.sleep(2)
+        # you can do stuff like this and it will take effect
+        # app.registry['types']['testing_link_aggregate_sno'].aggregated_items['targets'] = (
+        #    ['target.name', 'test_description'])
+
+        testapp.post_json('/testing-link-targets-sno/', target1, status=201)
+        testapp.post_json('/testing-link-targets-sno/', target2, status=201)
+        agg_res = testapp.post_json('/testing-link-aggregates-sno/', aggregated, status=201)
+        agg_res_atid = agg_res.json['@graph'][0]['@id']
+
+        # ensure that aggregated-items view shows nothing before indexing
+        pre_agg_view = testapp.get(agg_res_atid + '@@aggregated-items', status=200).json
+        assert pre_agg_view['@id'] == agg_res_atid
+        assert pre_agg_view['aggregated_items'] == {}
+
+        index_n_items_for_testing(indexer_testapp, 3)
+        # wait for the items to index
+        # indexer_testapp.post_json('/index', {'record': True})
+        time.sleep(2)
+
+        # wait for test-link-aggregated item to index
+        # doc_count = es.count(index=namespaced_aggregate).get('count')
+        # tries = 0
+        # while doc_count < 1 and tries < 5:
+        #     time.sleep(4)
+        #     doc_count = es.count(index=namespaced_aggregate).get('count')
+        #     tries += 1
+        # assert doc_count == 1
+        Eventually.call_assertion(make_es_count_checker(1, es=es, namespaced_index=namespaced_aggregate),
+                                  wait_seconds=4)
+
+        @Eventually.consistent()
+        def check_links():
+            es_agg_res = es.get(index=namespaced_aggregate, id=agg_res_uuid)
+            assert 'aggregated_items' in es_agg_res['_source']
+            es_agg_items = es_agg_res['_source']['aggregated_items']
+            assert 'targets' in es_agg_items
+            assert len(es_agg_items['targets']) == 2
+            for idx, target_agg in enumerate(es_agg_items['targets']):
+                # order of targets should be maintained
+                assert target_agg['parent'] == agg_res.json['@graph'][0]['@id']
+                assert target_agg['embedded_path'] == 'targets'
+                if idx == 0:
+                    assert target_agg['item']['test_description'] == 'target one'
+                    assert target_agg['item']['target']['uuid'] == target1['uuid']
+                else:
+                    assert target_agg['item']['test_description'] == 'target two'
+                    assert target_agg['item']['target']['uuid'] == target2['uuid']
+
+        check_links()
+
+        # now make sure they get updated on a patch
+        # use duplicate items, which should be deduplicated if all aggregated
+        # content (including parent) is exactly the same
+        testapp.patch_json(
+            '/testing-link-aggregates-sno/' + aggregated['uuid'],
+            {'targets': [
+                {'test_description': 'target one revised',
+                 'target': target_uuid1},
+                {'test_description': 'target one revised',
+                 'target': target_uuid1},
+                {'test_description': 'target one revised2',
+                 'target': target_uuid1}
+            ]}
+        )
+
+        index_n_items_for_testing(indexer_testapp, 1)
+
+        # indexer_testapp.post_json('/index', {'record': True})
+        # time.sleep(10)  # be lazy and just wait a bit
+
+        @Eventually.consistent()
+        def check_updated_links():
+            es_agg_res = es.get(index=namespaced_aggregate, id=agg_res_uuid)
+            assert 'aggregated_items' in es_agg_res['_source']
+            es_agg_items = es_agg_res['_source']['aggregated_items']
+            assert 'targets' in es_agg_items
+            assert len(es_agg_items['targets']) == 2
+            assert es_agg_items['targets'][0]['item']['test_description'] == 'target one revised'
+            assert es_agg_items['targets'][1]['item']['test_description'] == 'target one revised2'
+            # check that the aggregated-items view now works
+            post_agg_view = testapp.get(agg_res_atid + '@@aggregated-items', status=200).json
+            assert post_agg_view['@id'] == agg_res_atid
+            assert post_agg_view['aggregated_items'] == es_agg_res['_source']['aggregated_items']
+
+        check_updated_links()
+
+    finally:
+
+        # TODO: Will thinks this is not needed and that setup_and_teardown's call to create_mapping is
+        #       enough to assure this will ultimately be reset. I'll leave that to debug another day. -kmp 29-Mar-2023
+
+        # clean up the test items
+        testapp.patch_json('/testing-link-aggregates-sno/' + aggregated['uuid'],
+                           {'targets': []})
+        # indexer_testapp.post_json('/index', {'record': True})
+        index_n_items_for_testing(indexer_testapp, 1)
+        time.sleep(2)  # allow some settling out
 
 
 @pytest.mark.flaky(max_runs=2, rerun_filter=delay_rerun)
 def test_indexing_info(app, testapp, indexer_testapp):
     """
     Test the information on indexing-info for a given uuid and make sure that
     it updates properly following indexing
```

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/test_invalidation_scope.py` & `dcicsnovault-8.0.0/snovault/tests/test_invalidation_scope.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/test_key.py` & `dcicsnovault-8.0.0/snovault/tests/test_key.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/test_link.py` & `dcicsnovault-8.0.0/snovault/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/test_logging.py` & `dcicsnovault-8.0.0/snovault/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/test_misc.py` & `dcicsnovault-8.0.0/snovault/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/test_post_put_patch.py` & `dcicsnovault-8.0.0/snovault/tests/test_post_put_patch.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/test_postgresql_fixture.py` & `dcicsnovault-8.0.0/snovault/tests/test_postgresql_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/test_schemas.py` & `dcicsnovault-8.0.0/snovault/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/test_serverfixtures.py` & `dcicsnovault-8.0.0/snovault/tests/test_serverfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/test_standalone_dev.py` & `dcicsnovault-8.0.0/snovault/tests/test_standalone_dev.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/test_stats.py` & `dcicsnovault-8.0.0/snovault/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/test_storage.py` & `dcicsnovault-8.0.0/snovault/tests/test_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from dcicutils.misc_utils import filtered_warnings
 from pyramid.threadlocal import manager
 from sqlalchemy import func
 from sqlalchemy.exc import IntegrityError
 from ..interfaces import DBSESSION, STORAGE
 from ..storage import (
+    POSTGRES_COMPATIBLE_MAJOR_VERSIONS,
     Blob,
     CurrentPropertySheet,
     Key,
     Link,
     PickStorage,
     PropertySheet,
     RDBStorage,
@@ -22,19 +23,14 @@
     S3BlobStorage,
 )
 from moto import mock_s3
 
 pytestmark = pytest.mark.storage
 
 
-# These 3 versions are known to be compatible, older versions should not be
-# used, odds are 14 can be used as well - Will Sept 13 2022
-POSTGRES_COMPATIBLE_MAJOR_VERSIONS = ['11', '12', '13', '14']
-
-
 def test_postgres_version(session):
     """ Tests that the local postgres is running one of the compatible versions """
     (version_info,) = session.query(func.version()).one()
     print("version_info=", version_info)
     assert isinstance(version_info, str)
     assert re.match("PostgreSQL (%s)([.][0-9]+)? " % '|'.join(POSTGRES_COMPATIBLE_MAJOR_VERSIONS), version_info)
```

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/test_upgrader.py` & `dcicsnovault-8.0.0/snovault/tests/test_upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/test_util.py` & `dcicsnovault-8.0.0/snovault/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/test_views.py` & `dcicsnovault-8.0.0/snovault/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/testappfixtures.py` & `dcicsnovault-8.0.0/snovault/tests/testappfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/testing_key.py` & `dcicsnovault-8.0.0/snovault/tests/testing_key.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/testing_upgrader.py` & `dcicsnovault-8.0.0/snovault/tests/testing_upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/testing_views.py` & `dcicsnovault-8.0.0/snovault/tests/testing_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tests/toolfixtures.py` & `dcicsnovault-8.0.0/snovault/tests/toolfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/tools.py` & `dcicsnovault-8.0.0/snovault/tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import contextlib
 import json
 import time
 import webtest
 
 from dcicutils.lang_utils import n_of
+from dcicutils.misc_utils import ignored
 from .interfaces import DBSESSION
 from .elasticsearch import create_mapping
 
 
 def make_testapp(app, *, http_accept=None, remote_user=None):
     """
     By default, makes a testapp with environ={"HTTP_ACCEPT": "application/json", "REMOTE_USER": "TEST"}.
@@ -77,19 +78,38 @@
 @contextlib.contextmanager
 def local_collections(*, app, collections):
     with begin_nested(app=app, commit=False):
         create_mapping.run(app, collections=collections, skip_indexing=True, purge_queue=True)
         yield
 
 
-def index_n_items_for_testing(indexer_testapp, n, *, max_tries=10):
+def index_n_items_for_testing(indexer_testapp, n, *, max_tries=10, wait_seconds=1, initial_wait_seconds=None):
     tries_so_far = 0
     total_items_seen = 0
-    while total_items_seen < n:
+    current_wait_seconds = 0.5 * wait_seconds if initial_wait_seconds is None else initial_wait_seconds
+    while True:
+        time.sleep(current_wait_seconds)
         indexing_record = indexer_testapp.post_json('/index', {'record': True}).json
         items_this_time = indexing_record.get('indexing_count')
         assert items_this_time is not None, f"Expected an indexing_record, but got {json.dumps(indexing_record)}."
         total_items_seen += items_this_time
+        if total_items_seen >= n:
+            break
         assert tries_so_far < max_tries, (
             f"Attempt to index {n_of(n, 'item')}. Tried {max_tries} times, but saw only {total_items_seen}.")
         tries_so_far += 1
-        time.sleep(1)
+        current_wait_seconds = wait_seconds
+
+
+def delay_rerun(*args):
+    """ Rerun function for flaky """
+    ignored(args)
+    time.sleep(10)
+    return True
+
+
+def make_es_count_checker(n, *, es, namespaced_index):
+    def es_count_checker():
+        indexed_count = es.count(index=namespaced_index).get('count')
+        assert indexed_count == n
+        return n
+    return es_count_checker
```

### Comparing `dcicsnovault-7.9.9.0b2/snovault/typeinfo.py` & `dcicsnovault-8.0.0/snovault/typeinfo.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/upgrader.py` & `dcicsnovault-8.0.0/snovault/upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/util.py` & `dcicsnovault-8.0.0/snovault/util.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/validation.py` & `dcicsnovault-8.0.0/snovault/validation.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/snovault/validators.py` & `dcicsnovault-8.0.0/snovault/validators.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-7.9.9.0b2/PKG-INFO` & `dcicsnovault-8.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicsnovault
-Version: 7.9.9.0b2
+Version: 8.0.0
 Summary: Storage support for 4DN Data Portals.
 Home-page: https://github.com/4dn-dcic/snovault
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8.1,<3.9
 Classifier: Development Status :: 4 - Beta
@@ -21,15 +21,15 @@
 Requires-Dist: SQLAlchemy (>=1.4.41,<2.0.0)
 Requires-Dist: WSGIProxy2 (==0.4.2)
 Requires-Dist: WebOb (>=1.8.7,<2.0.0)
 Requires-Dist: WebTest (>=2.0.35,<3.0.0)
 Requires-Dist: aws_requests_auth (>=0.4.1,<0.5.0)
 Requires-Dist: boto3 (>=1.24.36)
 Requires-Dist: botocore (>=1.27.36)
-Requires-Dist: dcicutils (>=6.9.9.0b0,<7.0.0.0)
+Requires-Dist: dcicutils (>=7.0.0,<8.0.0)
 Requires-Dist: elasticsearch (==7.13.4)
 Requires-Dist: elasticsearch_dsl (>=7.4.0,<8.0.0)
 Requires-Dist: future (>=0.15.2,<1)
 Requires-Dist: html5lib (>=1.1)
 Requires-Dist: humanfriendly (>=1.44.9,<2.0.0)
 Requires-Dist: jsonschema_serialize_fork (>=2.1.1,<3.0.0)
 Requires-Dist: netaddr (>=0.8.0,<1)
@@ -53,15 +53,15 @@
 Requires-Dist: simplejson (>=3.17.6,<4.0.0)
 Requires-Dist: structlog (>=19.2.0,<20)
 Requires-Dist: subprocess_middleware (>=0.3,<1)
 Requires-Dist: transaction (>=3.0.1,<4.0.0)
 Requires-Dist: venusian (>=1.2.0,<2.0.0)
 Requires-Dist: xlrd (>=1.0.0,<2.0.0)
 Requires-Dist: zope.deprecation (>=4.4.0,<5.0.0)
-Requires-Dist: zope.interface (>=4.7.2,<5.0.0)
+Requires-Dist: zope.interface (>=4.7.2,<6)
 Requires-Dist: zope.sqlalchemy (==1.6)
 Project-URL: Documentation, https://github.com/4dn-dcic/snovault
 Project-URL: Repository, https://github.com/4dn-dcic/snovault
 Description-Content-Type: text/x-rst
 
 =============
 DCIC Snovault
```

