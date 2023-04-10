# Comparing `tmp/gptcache-0.1.6.tar.gz` & `tmp/gptcache-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptcache-0.1.6.tar", last modified: Mon Apr 10 10:20:04 2023, max compression
+gzip compressed data, was "gptcache-0.1.7.tar", last modified: Mon Apr 10 15:01:21 2023, max compression
```

## Comparing `gptcache-0.1.6.tar` & `gptcache-0.1.7.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:20:04.453627 gptcache-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-04-10 10:19:55.000000 gptcache-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    16700 2023-04-10 10:20:04.453627 gptcache-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    16162 2023-04-10 10:19:55.000000 gptcache-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:20:04.441627 gptcache-0.1.6/gptcache/
--rw-r--r--   0 runner    (1001) docker     (122)     5999 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:20:04.445627 gptcache-0.1.6/gptcache/adapter/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3936 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/adapter/adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/adapter/langchain_llms.py
--rw-r--r--   0 runner    (1001) docker     (122)     2789 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/adapter/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:20:04.445627 gptcache-0.1.6/gptcache/embedding/
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/embedding/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1768 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/embedding/cohere.py
--rw-r--r--   0 runner    (1001) docker     (122)     1663 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/embedding/fasttext.py
--rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/embedding/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/embedding/onnx.py
--rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/embedding/openai.py
--rw-r--r--   0 runner    (1001) docker     (122)     1542 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/embedding/sbert.py
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/embedding/string.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:20:04.449627 gptcache-0.1.6/gptcache/manager/
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5132 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/eviction.py
--rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:20:04.449627 gptcache-0.1.6/gptcache/manager/scalar_data/
--rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/scalar_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      919 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/scalar_data/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/scalar_data/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     5200 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/scalar_data/sqlalchemy.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:20:04.449627 gptcache-0.1.6/gptcache/manager/vector_data/
--rw-r--r--   0 runner    (1001) docker     (122)     1479 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/vector_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      601 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/vector_data/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1598 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/vector_data/chroma.py
--rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/vector_data/faiss.py
--rw-r--r--   0 runner    (1001) docker     (122)     3100 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/vector_data/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     4936 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/vector_data/milvus.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:20:04.449627 gptcache-0.1.6/gptcache/processor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/processor/post.py
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/processor/pre.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:20:04.453627 gptcache-0.1.6/gptcache/similarity_evaluation/
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/similarity_evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/similarity_evaluation/distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/similarity_evaluation/exact_match.py
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/similarity_evaluation/np.py
--rw-r--r--   0 runner    (1001) docker     (122)     4633 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/similarity_evaluation/onnx.py
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/similarity_evaluation/similarity_evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:20:04.453627 gptcache-0.1.6/gptcache/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     2001 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      536 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/utils/dependency_control.py
--rw-r--r--   0 runner    (1001) docker     (122)      552 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/utils/lazy_import.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:20:04.445627 gptcache-0.1.6/gptcache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    16700 2023-04-10 10:20:04.000000 gptcache-0.1.6/gptcache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1570 2023-04-10 10:20:04.000000 gptcache-0.1.6/gptcache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 10:20:04.000000 gptcache-0.1.6/gptcache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-10 10:20:04.000000 gptcache-0.1.6/gptcache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-10 10:20:04.000000 gptcache-0.1.6/gptcache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-10 10:20:04.453627 gptcache-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-04-10 10:19:55.000000 gptcache-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:21.880425 gptcache-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-04-10 15:01:12.000000 gptcache-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    16700 2023-04-10 15:01:21.880425 gptcache-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    16162 2023-04-10 15:01:12.000000 gptcache-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:21.872425 gptcache-0.1.7/gptcache/
+-rw-r--r--   0 runner    (1001) docker     (122)     5999 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:21.876425 gptcache-0.1.7/gptcache/adapter/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3957 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/adapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/adapter/langchain_llms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2789 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/adapter/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:21.876425 gptcache-0.1.7/gptcache/embedding/
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/embedding/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1768 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/embedding/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1663 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/embedding/fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/embedding/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/embedding/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/embedding/openai.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1542 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/embedding/sbert.py
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/embedding/string.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:21.876425 gptcache-0.1.7/gptcache/manager/
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5132 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/eviction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:21.876425 gptcache-0.1.7/gptcache/manager/scalar_data/
+-rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/scalar_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      919 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/scalar_data/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/scalar_data/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5200 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/scalar_data/sqlalchemy.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:21.876425 gptcache-0.1.7/gptcache/manager/vector_data/
+-rw-r--r--   0 runner    (1001) docker     (122)     1479 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/vector_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      601 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/vector_data/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1598 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/vector_data/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/vector_data/faiss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3100 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/vector_data/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4936 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/manager/vector_data/milvus.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:21.876425 gptcache-0.1.7/gptcache/processor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/processor/post.py
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/processor/pre.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:21.880425 gptcache-0.1.7/gptcache/similarity_evaluation/
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/similarity_evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/similarity_evaluation/distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/similarity_evaluation/exact_match.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/similarity_evaluation/np.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4633 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/similarity_evaluation/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/similarity_evaluation/similarity_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:21.880425 gptcache-0.1.7/gptcache/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     2001 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/utils/dependency_control.py
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-04-10 15:01:12.000000 gptcache-0.1.7/gptcache/utils/lazy_import.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:01:21.872425 gptcache-0.1.7/gptcache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    16700 2023-04-10 15:01:21.000000 gptcache-0.1.7/gptcache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1570 2023-04-10 15:01:21.000000 gptcache-0.1.7/gptcache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 15:01:21.000000 gptcache-0.1.7/gptcache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-10 15:01:21.000000 gptcache-0.1.7/gptcache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-10 15:01:21.000000 gptcache-0.1.7/gptcache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-10 15:01:21.880425 gptcache-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-04-10 15:01:12.000000 gptcache-0.1.7/setup.py
```

### Comparing `gptcache-0.1.6/LICENSE` & `gptcache-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/PKG-INFO` & `gptcache-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptcache
-Version: 0.1.6
+Version: 0.1.7
 Summary: GPT Cache, a powerful caching library that can be used to speed up and lower the cost of chat applications that rely on the LLM service. GPT Cache works as a memcache for AIGC applications, similar to how Redis works for traditional applications.
 Home-page: https://github.com/zilliztech/GPTCache
 Author: SimFG
 Author-email: bang.fu@zilliz.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
```

### Comparing `gptcache-0.1.6/README.md` & `gptcache-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/__init__.py` & `gptcache-0.1.7/gptcache/__init__.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/adapter/adapter.py` & `gptcache-0.1.7/gptcache/adapter/adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,20 +12,21 @@
     embedding_data = None
     # you want to retry to send the request to chatgpt when the cache is negative
     cache_skip = kwargs.pop("cache_skip", False)
     cache_factor = kwargs.pop("cache_factor", 1.0)
     pre_embedding_data = chat_cache.pre_embedding_func(
         kwargs, extra_param=context.get("pre_embedding_func", None)
     )
-    if cache_enable and not cache_skip:
+    if cache_enable:
         embedding_data = time_cal(
             chat_cache.embedding_func,
             func_name="embedding",
             report_func=chat_cache.report.embedding,
         )(pre_embedding_data, extra_param=context.get("embedding_func", None))
+    if cache_enable and not cache_skip:
         cache_data_list = time_cal(
             chat_cache.data_manager.search,
             func_name="search",
             report_func=chat_cache.report.search,
         )(embedding_data, extra_param=context.get("search_func", None))
         if cache_data_list is None:
             cache_data_list = []
```

### Comparing `gptcache-0.1.6/gptcache/adapter/langchain_llms.py` & `gptcache-0.1.7/gptcache/adapter/langchain_llms.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/adapter/openai.py` & `gptcache-0.1.7/gptcache/adapter/openai.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/embedding/__init__.py` & `gptcache-0.1.7/gptcache/embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/embedding/cohere.py` & `gptcache-0.1.7/gptcache/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/embedding/fasttext.py` & `gptcache-0.1.7/gptcache/embedding/fasttext.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/embedding/huggingface.py` & `gptcache-0.1.7/gptcache/embedding/huggingface.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/embedding/onnx.py` & `gptcache-0.1.7/gptcache/embedding/onnx.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/embedding/openai.py` & `gptcache-0.1.7/gptcache/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/embedding/sbert.py` & `gptcache-0.1.7/gptcache/embedding/sbert.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/manager/data_manager.py` & `gptcache-0.1.7/gptcache/manager/data_manager.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/manager/eviction.py` & `gptcache-0.1.7/gptcache/manager/eviction.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/manager/factory.py` & `gptcache-0.1.7/gptcache/manager/factory.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/manager/scalar_data/__init__.py` & `gptcache-0.1.7/gptcache/manager/scalar_data/__init__.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/manager/scalar_data/base.py` & `gptcache-0.1.7/gptcache/manager/scalar_data/base.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/manager/scalar_data/manager.py` & `gptcache-0.1.7/gptcache/manager/scalar_data/manager.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/manager/scalar_data/sqlalchemy.py` & `gptcache-0.1.7/gptcache/manager/scalar_data/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/manager/vector_data/__init__.py` & `gptcache-0.1.7/gptcache/manager/vector_data/__init__.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/manager/vector_data/base.py` & `gptcache-0.1.7/gptcache/manager/vector_data/base.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/manager/vector_data/chroma.py` & `gptcache-0.1.7/gptcache/manager/vector_data/chroma.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/manager/vector_data/faiss.py` & `gptcache-0.1.7/gptcache/manager/vector_data/faiss.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/manager/vector_data/manager.py` & `gptcache-0.1.7/gptcache/manager/vector_data/manager.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/manager/vector_data/milvus.py` & `gptcache-0.1.7/gptcache/manager/vector_data/milvus.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/similarity_evaluation/__init__.py` & `gptcache-0.1.7/gptcache/similarity_evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/similarity_evaluation/distance.py` & `gptcache-0.1.7/gptcache/similarity_evaluation/distance.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/similarity_evaluation/exact_match.py` & `gptcache-0.1.7/gptcache/similarity_evaluation/exact_match.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/similarity_evaluation/np.py` & `gptcache-0.1.7/gptcache/similarity_evaluation/np.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/similarity_evaluation/onnx.py` & `gptcache-0.1.7/gptcache/similarity_evaluation/onnx.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/utils/__init__.py` & `gptcache-0.1.7/gptcache/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/utils/dependency_control.py` & `gptcache-0.1.7/gptcache/utils/dependency_control.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/utils/error.py` & `gptcache-0.1.7/gptcache/utils/error.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache/utils/lazy_import.py` & `gptcache-0.1.7/gptcache/utils/lazy_import.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/gptcache.egg-info/PKG-INFO` & `gptcache-0.1.7/gptcache.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptcache
-Version: 0.1.6
+Version: 0.1.7
 Summary: GPT Cache, a powerful caching library that can be used to speed up and lower the cost of chat applications that rely on the LLM service. GPT Cache works as a memcache for AIGC applications, similar to how Redis works for traditional applications.
 Home-page: https://github.com/zilliztech/GPTCache
 Author: SimFG
 Author-email: bang.fu@zilliz.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
```

### Comparing `gptcache-0.1.6/gptcache.egg-info/SOURCES.txt` & `gptcache-0.1.7/gptcache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.6/setup.py` & `gptcache-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             if require.strip() and not require.startswith('#')
         ]
 
 
 setuptools.setup(
     name="gptcache",
     packages=find_packages(),
-    version="0.1.6",
+    version="0.1.7",
     author="SimFG",
     author_email="bang.fu@zilliz.com",
     description="GPT Cache, a powerful caching library that can be used to speed up and lower the cost of chat "
                 "applications that rely on the LLM service. GPT Cache works as a memcache for AIGC applications, "
                 "similar to how Redis works for traditional applications.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

