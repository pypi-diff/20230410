# Comparing `tmp/gptcache-0.1.5.tar.gz` & `tmp/gptcache-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptcache-0.1.5.tar", last modified: Thu Apr  6 12:46:50 2023, max compression
+gzip compressed data, was "gptcache-0.1.6.tar", last modified: Mon Apr 10 10:20:04 2023, max compression
```

## Comparing `gptcache-0.1.5.tar` & `gptcache-0.1.6.tar`

### file list

```diff
@@ -1,60 +1,62 @@
-drwxr-xr-x   0 derek      (501) staff       (20)        0 2023-04-06 12:46:50.546503 gptcache-0.1.5/
--rw-r--r--   0 derek      (501) staff       (20)     1068 2023-04-05 13:14:02.000000 gptcache-0.1.5/LICENSE
--rw-r--r--   0 derek      (501) staff       (20)    15151 2023-04-06 12:46:50.545618 gptcache-0.1.5/PKG-INFO
--rw-r--r--   0 derek      (501) staff       (20)    14613 2023-04-06 12:44:58.000000 gptcache-0.1.5/README.md
-drwxr-xr-x   0 derek      (501) staff       (20)        0 2023-04-06 12:46:50.452518 gptcache-0.1.5/gptcache/
--rw-r--r--   0 derek      (501) staff       (20)     5880 2023-04-06 12:38:32.000000 gptcache-0.1.5/gptcache/__init__.py
-drwxr-xr-x   0 derek      (501) staff       (20)        0 2023-04-06 12:46:50.468557 gptcache-0.1.5/gptcache/adapter/
--rw-r--r--   0 derek      (501) staff       (20)        0 2023-04-01 11:32:02.000000 gptcache-0.1.5/gptcache/adapter/__init__.py
--rw-r--r--   0 derek      (501) staff       (20)     3664 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/adapter/adapter.py
--rw-r--r--   0 derek      (501) staff       (20)      539 2023-04-05 16:49:20.000000 gptcache-0.1.5/gptcache/adapter/langchain_llms.py
--rw-r--r--   0 derek      (501) staff       (20)     2599 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/adapter/openai.py
-drwxr-xr-x   0 derek      (501) staff       (20)        0 2023-04-06 12:46:50.489456 gptcache-0.1.5/gptcache/embedding/
--rw-r--r--   0 derek      (501) staff       (20)     1082 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/embedding/__init__.py
--rw-r--r--   0 derek      (501) staff       (20)      246 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/embedding/base.py
--rw-r--r--   0 derek      (501) staff       (20)     1779 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/embedding/cohere.py
--rw-r--r--   0 derek      (501) staff       (20)     1640 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/embedding/fasttext.py
--rw-r--r--   0 derek      (501) staff       (20)     2412 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/embedding/huggingface.py
--rw-r--r--   0 derek      (501) staff       (20)     2545 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/embedding/onnx.py
--rw-r--r--   0 derek      (501) staff       (20)     1952 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/embedding/openai.py
--rw-r--r--   0 derek      (501) staff       (20)     1527 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/embedding/sbert.py
--rw-r--r--   0 derek      (501) staff       (20)       51 2023-04-04 16:37:34.000000 gptcache-0.1.5/gptcache/embedding/string.py
-drwxr-xr-x   0 derek      (501) staff       (20)        0 2023-04-06 12:46:50.495012 gptcache-0.1.5/gptcache/manager/
--rw-r--r--   0 derek      (501) staff       (20)        0 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/manager/__init__.py
--rw-r--r--   0 derek      (501) staff       (20)     5115 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/manager/data_manager.py
--rw-r--r--   0 derek      (501) staff       (20)     1539 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/manager/eviction.py
--rw-r--r--   0 derek      (501) staff       (20)     5730 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/manager/factory.py
-drwxr-xr-x   0 derek      (501) staff       (20)        0 2023-04-06 12:46:50.498032 gptcache-0.1.5/gptcache/manager/scalar_data/
--rw-r--r--   0 derek      (501) staff       (20)      777 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/manager/scalar_data/__init__.py
--rw-r--r--   0 derek      (501) staff       (20)      978 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/manager/scalar_data/base.py
--rw-r--r--   0 derek      (501) staff       (20)     4400 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/manager/scalar_data/sqlalchemy.py
-drwxr-xr-x   0 derek      (501) staff       (20)        0 2023-04-06 12:46:50.504980 gptcache-0.1.5/gptcache/manager/vector_data/
--rw-r--r--   0 derek      (501) staff       (20)      587 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/manager/vector_data/__init__.py
--rw-r--r--   0 derek      (501) staff       (20)      550 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/manager/vector_data/base.py
--rw-r--r--   0 derek      (501) staff       (20)     1644 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/manager/vector_data/chroma.py
--rw-r--r--   0 derek      (501) staff       (20)     1602 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/manager/vector_data/faiss.py
--rw-r--r--   0 derek      (501) staff       (20)     5869 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/manager/vector_data/milvus.py
-drwxr-xr-x   0 derek      (501) staff       (20)        0 2023-04-06 12:46:50.514004 gptcache-0.1.5/gptcache/processor/
--rw-r--r--   0 derek      (501) staff       (20)        0 2023-04-01 16:45:13.000000 gptcache-0.1.5/gptcache/processor/__init__.py
--rw-r--r--   0 derek      (501) staff       (20)      162 2023-04-04 13:16:14.000000 gptcache-0.1.5/gptcache/processor/post.py
--rw-r--r--   0 derek      (501) staff       (20)      454 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/processor/pre.py
-drwxr-xr-x   0 derek      (501) staff       (20)        0 2023-04-06 12:46:50.527233 gptcache-0.1.5/gptcache/similarity_evaluation/
--rw-r--r--   0 derek      (501) staff       (20)      918 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/similarity_evaluation/__init__.py
--rw-r--r--   0 derek      (501) staff       (20)     1707 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/similarity_evaluation/distance.py
--rw-r--r--   0 derek      (501) staff       (20)     1238 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/similarity_evaluation/exact_match.py
--rw-r--r--   0 derek      (501) staff       (20)     2051 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/similarity_evaluation/np.py
--rw-r--r--   0 derek      (501) staff       (20)     4218 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/similarity_evaluation/onnx.py
--rw-r--r--   0 derek      (501) staff       (20)      235 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/similarity_evaluation/similarity_evaluation.py
-drwxr-xr-x   0 derek      (501) staff       (20)        0 2023-04-06 12:46:50.544009 gptcache-0.1.5/gptcache/utils/
--rw-r--r--   0 derek      (501) staff       (20)     3170 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/utils/__init__.py
--rw-r--r--   0 derek      (501) staff       (20)      382 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/utils/dependency_control.py
--rw-r--r--   0 derek      (501) staff       (20)      508 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/utils/error.py
--rw-r--r--   0 derek      (501) staff       (20)      707 2023-04-06 10:15:14.000000 gptcache-0.1.5/gptcache/utils/lazy_import.py
-drwxr-xr-x   0 derek      (501) staff       (20)        0 2023-04-06 12:46:50.460993 gptcache-0.1.5/gptcache.egg-info/
--rw-r--r--   0 derek      (501) staff       (20)    15151 2023-04-06 12:46:49.000000 gptcache-0.1.5/gptcache.egg-info/PKG-INFO
--rw-r--r--   0 derek      (501) staff       (20)     1490 2023-04-06 12:46:50.000000 gptcache-0.1.5/gptcache.egg-info/SOURCES.txt
--rw-r--r--   0 derek      (501) staff       (20)        1 2023-04-06 12:46:49.000000 gptcache-0.1.5/gptcache.egg-info/dependency_links.txt
--rw-r--r--   0 derek      (501) staff       (20)       24 2023-04-06 12:46:49.000000 gptcache-0.1.5/gptcache.egg-info/requires.txt
--rw-r--r--   0 derek      (501) staff       (20)        9 2023-04-06 12:46:49.000000 gptcache-0.1.5/gptcache.egg-info/top_level.txt
--rw-r--r--   0 derek      (501) staff       (20)       38 2023-04-06 12:46:50.546703 gptcache-0.1.5/setup.cfg
--rw-r--r--   0 derek      (501) staff       (20)     1108 2023-04-06 12:46:42.000000 gptcache-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:20:04.453627 gptcache-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-04-10 10:19:55.000000 gptcache-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    16700 2023-04-10 10:20:04.453627 gptcache-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    16162 2023-04-10 10:19:55.000000 gptcache-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:20:04.441627 gptcache-0.1.6/gptcache/
+-rw-r--r--   0 runner    (1001) docker     (122)     5999 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:20:04.445627 gptcache-0.1.6/gptcache/adapter/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3936 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/adapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/adapter/langchain_llms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2789 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/adapter/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:20:04.445627 gptcache-0.1.6/gptcache/embedding/
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/embedding/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1768 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/embedding/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1663 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/embedding/fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/embedding/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/embedding/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/embedding/openai.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1542 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/embedding/sbert.py
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/embedding/string.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:20:04.449627 gptcache-0.1.6/gptcache/manager/
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5132 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/eviction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:20:04.449627 gptcache-0.1.6/gptcache/manager/scalar_data/
+-rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/scalar_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      919 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/scalar_data/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/scalar_data/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5200 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/scalar_data/sqlalchemy.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:20:04.449627 gptcache-0.1.6/gptcache/manager/vector_data/
+-rw-r--r--   0 runner    (1001) docker     (122)     1479 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/vector_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      601 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/vector_data/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1598 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/vector_data/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/vector_data/faiss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3100 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/vector_data/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4936 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/manager/vector_data/milvus.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:20:04.449627 gptcache-0.1.6/gptcache/processor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/processor/post.py
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/processor/pre.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:20:04.453627 gptcache-0.1.6/gptcache/similarity_evaluation/
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/similarity_evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/similarity_evaluation/distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/similarity_evaluation/exact_match.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/similarity_evaluation/np.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4633 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/similarity_evaluation/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/similarity_evaluation/similarity_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:20:04.453627 gptcache-0.1.6/gptcache/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     2001 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/utils/dependency_control.py
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-04-10 10:19:55.000000 gptcache-0.1.6/gptcache/utils/lazy_import.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:20:04.445627 gptcache-0.1.6/gptcache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    16700 2023-04-10 10:20:04.000000 gptcache-0.1.6/gptcache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1570 2023-04-10 10:20:04.000000 gptcache-0.1.6/gptcache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 10:20:04.000000 gptcache-0.1.6/gptcache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-10 10:20:04.000000 gptcache-0.1.6/gptcache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-10 10:20:04.000000 gptcache-0.1.6/gptcache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-10 10:20:04.453627 gptcache-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-04-10 10:19:55.000000 gptcache-0.1.6/setup.py
```

### Comparing `gptcache-0.1.5/LICENSE` & `gptcache-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.5/PKG-INFO` & `gptcache-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: gptcache
-Version: 0.1.5
+Version: 0.1.6
 Summary: GPT Cache, a powerful caching library that can be used to speed up and lower the cost of chat applications that rely on the LLM service. GPT Cache works as a memcache for AIGC applications, similar to how Redis works for traditional applications.
 Home-page: https://github.com/zilliztech/GPTCache
 Author: SimFG
 Author-email: bang.fu@zilliz.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GPTCache : A Library for Creating Semantic Cache for LLM Queries
 Slash Your LLM API Costs by 10x 💰, Boost Speed by 100x ⚡ 
 
-[![Release](https://img.shields.io/pypi/v/gptcache?label=Release&color)](https://pypi.org/project/gptcache/)
-[![CI](https://github.com/zilliztech/gptcache/actions/workflows/CI_main.yaml/badge.svg)](https://github.com/zilliztech/gptcache/actions/workflows/CI_main.yaml)
-[![pip download](https://img.shields.io/pypi/dm/gptcache.svg?color=bright-green)](https://pypi.org/project/gptcache/)
+[![Release](https://img.shields.io/pypi/v/gptcache?label=Release&color&logo=Python)](https://pypi.org/project/gptcache/)
+[![Pylint](https://img.shields.io/github/actions/workflow/status/zilliztech/GPTCache/pylint.yaml?label=Pylint&logo=Github)](https://github.com/zilliztech/gptcache/actions/workflows/pylint.yaml)
+[![CI](https://img.shields.io/github/actions/workflow/status/zilliztech/GPTCache/unit_test_main.yaml?label=Test&logo=Github)](https://github.com/zilliztech/gptcache/actions/workflows/unit_test_main.yaml)
+[![pip download](https://img.shields.io/pypi/dm/gptcache.svg?color=bright-green&logo=Pypi)](https://pypi.org/project/gptcache/)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/license/mit/)
 [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/zilliz_universe.svg?style=social&label=Follow%20%40Zilliz)](https://twitter.com/zilliz_universe)
 [![Discord](https://dcbadge.vercel.app/api/server/Q8C6WEjSWV?compact=true&style=flat)](https://discord.gg/Q8C6WEjSWV)
 
 Documentation: https://gptcache.readthedocs.io/en/latest/.
 
 Discord: https://discord.gg/Q8C6WEjSWV.
@@ -31,45 +32,30 @@
 
 `pip install gptcache`
 
 ## 🚀 What is GPTCache?
 
 ChatGPT and various large language models (LLMs) boast incredible versatility, enabling the development of a wide range of applications. However, as your application grows in popularity and encounters higher traffic levels, the expenses related to LLM API calls can become substantial. Additionally, LLM services might exhibit slow response times, especially when dealing with a significant number of requests.
 
-To tackle this challenge, we have created GPTCache, a project dedicated to building a semantic cache for storing LLM responses. This library offers the following primary benefits:
-
-1. **Decreased expenses**: Most LLM services charge fees based on a combination of number of requests and [token count](https://openai.com/pricing). By caching query results, GPTCache reduces both the number of requests and the number of tokens sent to the LLM service. This minimizes the overall cost of using the service. 
-2. **Enhanced performance**: LLMs employ generative AI algorithms to generate responses in real-time, a process that can sometimes be time-consuming. However, when a similar query is cached, the response time significantly improves, as the result is fetched directly from the cache, eliminating the need to interact with the LLM service. In most situations, GPTCache can also provide superior query throughput compared to standard LLM services.
-3. **Improved scalability and availability**: LLM services frequently enforce [rate limits](https://platform.openai.com/docs/guides/rate-limits), which are constraints that APIs place on the number of times a user or client can access the server within a given timeframe. Hitting a rate limit means that additional requests will be blocked until a certain period has elapsed, leading to a service outage. With GPTCache, you can easily scale to accommodate an increasing volume of of queries, ensuring consistent performance as your application's user base expands.
-4. **Flexible development environment**: When developing LLM applications, an LLM APIs connection is required to prove concepts. GPTCache offers the same interface as LLM APIs and can store LLM-generated or mocked data. This helps to verify your application's features without connecting to the LLM APIs or even the network.
-
-## 🤔 How does it work?
-
-A good analogy for GptCache is to think of it as a more semantic version of Redis. In GPTCache, hits are not limited to exact matches, but rather also include prompts and context similar to previous queries. We believe that the traditional cache design still works for AIGC applications due to the following reasons:
-
-- Locality is present everywhere. Like traditional application systems, AIGC applications also face similar hot topics. For instance, ChatGPT itself may be a popular topic among programmers.
-- For purpose-built SaaS services, users tend to ask questions within a specific domain, with both temporal and spatial locality.
-- By utilizing vector similarity search, it is possible to find a similarity relationship between questions and answers at a relatively low cost.
-
-We provide [benchmarks](https://github.com/zilliztech/gpt-cache/blob/main/examples/benchmark/benchmark_sqlite_faiss_onnx.py) to illustrate the concept. In semantic caching, there are three key measurement dimensions: false positives, false negatives, and hit latency. With the plugin-style implementation, users can easily tradeoff these three measurements according to their needs.
+To tackle this challenge, we have created GPTCache, a project dedicated to building a semantic cache for storing LLM responses. 
 
 ## 😊 Quick Start
 
 **Note**:
 
 - You can quickly try GPTCache and put it into a production environment without heavy development. However, please note that the repository is still under heavy development.
 - By default, only a limited number of libraries are installed to support the basic cache functionalities. When you need to use additional features, the related libraries will be **automatically installed**.
 - Make sure that the Python version is **3.8.1 or higher**, check: `python --version`
 - If you encounter issues installing a library due to a low pip version, run: `python -m pip install --upgrade pip`.
 
 ### dev install
 
 ```bash
 # clone GPTCache repo
-git clone https://github.com/zilliztech/GPTCache.git
+git clone -b dev https://github.com/zilliztech/GPTCache.git
 cd GPTCache
 
 # install the repo
 pip install -r requirements.txt
 python setup.py install
 ```
 
@@ -169,21 +155,21 @@
 
 def response_text(openai_resp):
     return openai_resp['choices'][0]['message']['content']
 
 from gptcache import cache
 from gptcache.adapter import openai
 from gptcache.embedding import Onnx
-from gptcache.manager.factory import get_data_manager
+from gptcache.manager import CacheBase, VectorBase, get_data_manager
 from gptcache.similarity_evaluation.distance import SearchDistanceEvaluation
 
 print("Cache loading.....")
 
 onnx = Onnx()
-data_manager = get_data_manager("sqlite", "faiss", dimension=onnx.dimension)
+data_manager = get_data_manager(CacheBase("sqlite"), VectorBase("faiss", dimension=onnx.dimension))
 cache.init(
     embedding_func=onnx.to_embeddings,
     data_manager=data_manager,
     similarity_evaluation=SearchDistanceEvaluation(),
     )
 cache.set_openai_key()
 
@@ -224,14 +210,40 @@
 
 More Docs：
 
 - [Usage, how to use GPTCache better](docs/usage.md)
 - [Features, all features currently supported by the cache](docs/feature.md)
 - [Examples, learn better custom caching](examples/README.md)
 
+## 😎 What can this help with?
+GPTCache offers the following primary benefits:
+
+- **Decreased expenses**: Most LLM services charge fees based on a combination of number of requests and [token count](https://openai.com/pricing). By caching query results, GPTCache reduces both the number of requests and the number of tokens sent to the LLM service. This minimizes the overall cost of using the service. 
+- **Enhanced performance**: LLMs employ generative AI algorithms to generate responses in real-time, a process that can sometimes be time-consuming. However, when a similar query is cached, the response time significantly improves, as the result is fetched directly from the cache, eliminating the need to interact with the LLM service. In most situations, GPTCache can also provide superior query throughput compared to standard LLM services.
+- **Improved scalability and availability**: LLM services frequently enforce [rate limits](https://platform.openai.com/docs/guides/rate-limits), which are constraints that APIs place on the number of times a user or client can access the server within a given timeframe. Hitting a rate limit means that additional requests will be blocked until a certain period has elapsed, leading to a service outage. With GPTCache, you can easily scale to accommodate an increasing volume of of queries, ensuring consistent performance as your application's user base expands.
+- **Flexible development environment**: When developing LLM applications, an LLM APIs connection is required to prove concepts. GPTCache offers the same interface as LLM APIs and can store LLM-generated or mocked data. This helps to verify your application's features without connecting to the LLM APIs or even the network.
+
+## 🤔 How does it work?
+
+Online services often exhibit data locality, with users frequently accessing popular or trending content. Cache systems take advantage of this behavior by storing commonly accessed data, which in turn reduces data retrieval time, improves response times, and eases the burden on backend servers. Traditional cache systems typically utilize an exact match between a new query and a cached query to determine if the requested content is available in the cache before fetching the data.
+
+However, using an exact match approach for LLM caches is less effective due to the complexity and variability of LLM queries, resulting in a low cache hit rate. To address this issue, GPTCache adopt alternative strategies like semantic caching. Semantic caching identifies and stores similar or related queries, thereby increasing cache hit probability and enhancing overall caching efficiency. 
+
+GPTCache employs embedding algorithms to convert queries into embeddings and uses a vector store for similarity search on these embeddings. This process allows GPTCache to identify and retrieve similar or related queries from the cache storage, as illustrated in the [Modules section](https://github.com/zilliztech/GPTCache#-modules). 
+
+Featuring a modular design, GPTCache makes it easy for users to customize their own semantic cache. The system offers various implementations for each module, and users can even develop their own implementations to suit their specific needs.
+
+In a semantic cache, false positives can occur during cache hits and false negatives during cache misses. GPTCache provides three metrics to evaluate its performance:
+
+- Precision: the ratio of true positives to the total of true positives and false positives.
+- Recall: the ratio of true positives to the total of true positives and false negatives.
+- Latency: the time required for a query to be processed and the corresponding data to be fetched from the cache.
+
+A [sample benchmark](https://github.com/zilliztech/gpt-cache/blob/main/examples/benchmark/benchmark_sqlite_faiss_onnx.py) is included for users to start with assessing the performance of their semantic cache.
+
 ## 🤗 Modules
 
 ![GPTCache Struct](docs/GPTCacheStructure.png)
 
 - **LLM Adapter**: 
 The LLM Adapter is designed to integrate different LLM models by unifying their APIs and request protocols. GPTCache offers a standardized interface for this purpose, with current support for ChatGPT integration.
   - [x] Support OpenAI ChatGPT API.
@@ -242,51 +254,51 @@
   - [x] Disable embedding. This will turn GPTCache into a keyword-matching cache.
   - [x] Support OpenAI embedding API.
   - [x] Support [ONNX](https://onnx.ai/) with the GPTCache/paraphrase-albert-onnx model.
   - [x] Support [Hugging Face](https://huggingface.co/) embedding API.
   - [x] Support [Cohere](https://docs.cohere.ai/reference/embed) embedding API.
   - [x] Support [fastText](https://fasttext.cc) embedding API.
   - [x] Support [SentenceTransformers](https://www.sbert.net) embedding API.
-  - [ ] Support other embedding apis
+  - [ ] Support other embedding APIs.
 - **Cache Storage**:
 **Cache Storage** is where the response from LLMs, such as ChatGPT, is stored. Cached responses are retrieved to assist in evaluating similarity and are returned to the requester if there is a good semantic match. At present, GPTCache supports SQLite and offers a universally accessible interface for extension of this module.
   - [x] Support [SQLite](https://sqlite.org/docs.html).
   - [x] Support [PostgreSQL](https://www.postgresql.org/).
   - [x] Support [MySQL](https://www.mysql.com/).
   - [x] Support [MariaDB](https://mariadb.org/).
   - [x] Support [SQL Server](https://www.microsoft.com/en-us/sql-server/).
   - [x] Support [Oracle](https://www.oracle.com/).
   - [ ] Support [MongoDB](https://www.mongodb.com/).
   - [ ] Support [Redis](https://redis.io/).
   - [ ] Support [Minio](https://min.io/).
   - [ ] Support [HBase](https://hbase.apache.org/).
-  - [ ] Support [ElasticSearch](https://www.elastic.co/)
-  - [ ] Support [zincsearch](https://zinc.dev/)
-  - [ ] Support other storages
+  - [ ] Support [ElasticSearch](https://www.elastic.co/).
+  - [ ] Support [Duckdb](https://github.com/duckdb/duckdb).
+  - [ ] Support other storages.
 - **Vector Store**:
 The **Vector Store** module helps find the K most similar requests from the input request's extracted embedding. The results can help assess similarity. GPTCache provides a user-friendly interface that supports various vector stores, including Milvus, Zilliz Cloud, and FAISS. More options will be available in the future.
-  - [x] Support [Milvus](https://milvus.io/).
-  - [x] Support [Zilliz Cloud](https://cloud.zilliz.com/).
-  - [x] Support [FAISS](https://faiss.ai/).
-  - [ ] Support other vector databases
+  - [x] Support [Milvus](https://milvus.io/), an open-source vector database for production-ready AI/LLM applicaionts. 
+  - [x] Support [Zilliz Cloud](https://cloud.zilliz.com/), a fully-managed cloud vector database based on Milvus.
+  - [x] Support [FAISS](https://faiss.ai/), a library for efficient similarity search and clustering of dense vectors.
+  - [ ] Support other vector databases.
 - **Cache Manager**:
 The **Cache Manager** is responsible for controlling the operation of both the **Cache Storage** and **Vector Store**.
   - **Eviction Policy**:
   Currently, GPTCache makes decisions about evictions based solely on the number of lines. This approach can result in inaccurate resource evaluation and may cause out-of-memory (OOM) errors. We are actively investigating and developing a more sophisticated strategy.
-    - [x] LRU eviction policy
-    - [x] FIFO eviction policy
-    - [ ] More complicated eviction policies
+    - [x] Support LRU eviction policy.
+    - [x] Support FIFO eviction policy.
+    - [ ] Support more complicated eviction policies.
 - **Similarity Evaluator**: 
 This module collects data from both the **Cache Storage** and **Vector Store**, and uses various strategies to determine the similarity between the input request and the requests from the **Vector Store**. Based on this similarity, it determines whether a request matches the cache. GPTCache provides a standardized interface for integrating various strategies, along with a collection of implementations to use. The following similarity definitions are currently supported or will be supported in the future:
   - [x] The distance we obtain from the **Vector Store**.
   - [x] A model-based similarity determined using the GPTCache/albert-duplicate-onnx model from [ONNX](https://onnx.ai/).
   - [x] Exact matches between the input request and the requests obtained from the **Vector Store**.
   - [x] Distance represented by applying linalg.norm from numpy to the embeddings.
-  - [ ] BM25 and other similarity measurements
-  - [ ] Support other model serving framework such as PyTorch
+  - [ ] BM25 and other similarity measurements.
+  - [ ] Support other model serving framework such as PyTorch.
  
   
   **Note**:Not all combinations of different modules may be compatible with each other. For instance, if we disable the **Embedding Extractor**, the **Vector Store** may not function as intended. We are currently working on implementing a combination sanity check for **GPTCache**.
 
 ## 😇 Roadmap
 Coming soon! [Stay tuned!](https://twitter.com/zilliz_universe)
```

### Comparing `gptcache-0.1.5/README.md` & `gptcache-0.1.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # GPTCache : A Library for Creating Semantic Cache for LLM Queries
 Slash Your LLM API Costs by 10x 💰, Boost Speed by 100x ⚡ 
 
-[![Release](https://img.shields.io/pypi/v/gptcache?label=Release&color)](https://pypi.org/project/gptcache/)
-[![CI](https://github.com/zilliztech/gptcache/actions/workflows/CI_main.yaml/badge.svg)](https://github.com/zilliztech/gptcache/actions/workflows/CI_main.yaml)
-[![pip download](https://img.shields.io/pypi/dm/gptcache.svg?color=bright-green)](https://pypi.org/project/gptcache/)
+[![Release](https://img.shields.io/pypi/v/gptcache?label=Release&color&logo=Python)](https://pypi.org/project/gptcache/)
+[![Pylint](https://img.shields.io/github/actions/workflow/status/zilliztech/GPTCache/pylint.yaml?label=Pylint&logo=Github)](https://github.com/zilliztech/gptcache/actions/workflows/pylint.yaml)
+[![CI](https://img.shields.io/github/actions/workflow/status/zilliztech/GPTCache/unit_test_main.yaml?label=Test&logo=Github)](https://github.com/zilliztech/gptcache/actions/workflows/unit_test_main.yaml)
+[![pip download](https://img.shields.io/pypi/dm/gptcache.svg?color=bright-green&logo=Pypi)](https://pypi.org/project/gptcache/)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/license/mit/)
 [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/zilliz_universe.svg?style=social&label=Follow%20%40Zilliz)](https://twitter.com/zilliz_universe)
 [![Discord](https://dcbadge.vercel.app/api/server/Q8C6WEjSWV?compact=true&style=flat)](https://discord.gg/Q8C6WEjSWV)
 
 Documentation: https://gptcache.readthedocs.io/en/latest/.
 
 Discord: https://discord.gg/Q8C6WEjSWV.
@@ -19,45 +20,30 @@
 
 `pip install gptcache`
 
 ## 🚀 What is GPTCache?
 
 ChatGPT and various large language models (LLMs) boast incredible versatility, enabling the development of a wide range of applications. However, as your application grows in popularity and encounters higher traffic levels, the expenses related to LLM API calls can become substantial. Additionally, LLM services might exhibit slow response times, especially when dealing with a significant number of requests.
 
-To tackle this challenge, we have created GPTCache, a project dedicated to building a semantic cache for storing LLM responses. This library offers the following primary benefits:
-
-1. **Decreased expenses**: Most LLM services charge fees based on a combination of number of requests and [token count](https://openai.com/pricing). By caching query results, GPTCache reduces both the number of requests and the number of tokens sent to the LLM service. This minimizes the overall cost of using the service. 
-2. **Enhanced performance**: LLMs employ generative AI algorithms to generate responses in real-time, a process that can sometimes be time-consuming. However, when a similar query is cached, the response time significantly improves, as the result is fetched directly from the cache, eliminating the need to interact with the LLM service. In most situations, GPTCache can also provide superior query throughput compared to standard LLM services.
-3. **Improved scalability and availability**: LLM services frequently enforce [rate limits](https://platform.openai.com/docs/guides/rate-limits), which are constraints that APIs place on the number of times a user or client can access the server within a given timeframe. Hitting a rate limit means that additional requests will be blocked until a certain period has elapsed, leading to a service outage. With GPTCache, you can easily scale to accommodate an increasing volume of of queries, ensuring consistent performance as your application's user base expands.
-4. **Flexible development environment**: When developing LLM applications, an LLM APIs connection is required to prove concepts. GPTCache offers the same interface as LLM APIs and can store LLM-generated or mocked data. This helps to verify your application's features without connecting to the LLM APIs or even the network.
-
-## 🤔 How does it work?
-
-A good analogy for GptCache is to think of it as a more semantic version of Redis. In GPTCache, hits are not limited to exact matches, but rather also include prompts and context similar to previous queries. We believe that the traditional cache design still works for AIGC applications due to the following reasons:
-
-- Locality is present everywhere. Like traditional application systems, AIGC applications also face similar hot topics. For instance, ChatGPT itself may be a popular topic among programmers.
-- For purpose-built SaaS services, users tend to ask questions within a specific domain, with both temporal and spatial locality.
-- By utilizing vector similarity search, it is possible to find a similarity relationship between questions and answers at a relatively low cost.
-
-We provide [benchmarks](https://github.com/zilliztech/gpt-cache/blob/main/examples/benchmark/benchmark_sqlite_faiss_onnx.py) to illustrate the concept. In semantic caching, there are three key measurement dimensions: false positives, false negatives, and hit latency. With the plugin-style implementation, users can easily tradeoff these three measurements according to their needs.
+To tackle this challenge, we have created GPTCache, a project dedicated to building a semantic cache for storing LLM responses. 
 
 ## 😊 Quick Start
 
 **Note**:
 
 - You can quickly try GPTCache and put it into a production environment without heavy development. However, please note that the repository is still under heavy development.
 - By default, only a limited number of libraries are installed to support the basic cache functionalities. When you need to use additional features, the related libraries will be **automatically installed**.
 - Make sure that the Python version is **3.8.1 or higher**, check: `python --version`
 - If you encounter issues installing a library due to a low pip version, run: `python -m pip install --upgrade pip`.
 
 ### dev install
 
 ```bash
 # clone GPTCache repo
-git clone https://github.com/zilliztech/GPTCache.git
+git clone -b dev https://github.com/zilliztech/GPTCache.git
 cd GPTCache
 
 # install the repo
 pip install -r requirements.txt
 python setup.py install
 ```
 
@@ -157,21 +143,21 @@
 
 def response_text(openai_resp):
     return openai_resp['choices'][0]['message']['content']
 
 from gptcache import cache
 from gptcache.adapter import openai
 from gptcache.embedding import Onnx
-from gptcache.manager.factory import get_data_manager
+from gptcache.manager import CacheBase, VectorBase, get_data_manager
 from gptcache.similarity_evaluation.distance import SearchDistanceEvaluation
 
 print("Cache loading.....")
 
 onnx = Onnx()
-data_manager = get_data_manager("sqlite", "faiss", dimension=onnx.dimension)
+data_manager = get_data_manager(CacheBase("sqlite"), VectorBase("faiss", dimension=onnx.dimension))
 cache.init(
     embedding_func=onnx.to_embeddings,
     data_manager=data_manager,
     similarity_evaluation=SearchDistanceEvaluation(),
     )
 cache.set_openai_key()
 
@@ -212,14 +198,40 @@
 
 More Docs：
 
 - [Usage, how to use GPTCache better](docs/usage.md)
 - [Features, all features currently supported by the cache](docs/feature.md)
 - [Examples, learn better custom caching](examples/README.md)
 
+## 😎 What can this help with?
+GPTCache offers the following primary benefits:
+
+- **Decreased expenses**: Most LLM services charge fees based on a combination of number of requests and [token count](https://openai.com/pricing). By caching query results, GPTCache reduces both the number of requests and the number of tokens sent to the LLM service. This minimizes the overall cost of using the service. 
+- **Enhanced performance**: LLMs employ generative AI algorithms to generate responses in real-time, a process that can sometimes be time-consuming. However, when a similar query is cached, the response time significantly improves, as the result is fetched directly from the cache, eliminating the need to interact with the LLM service. In most situations, GPTCache can also provide superior query throughput compared to standard LLM services.
+- **Improved scalability and availability**: LLM services frequently enforce [rate limits](https://platform.openai.com/docs/guides/rate-limits), which are constraints that APIs place on the number of times a user or client can access the server within a given timeframe. Hitting a rate limit means that additional requests will be blocked until a certain period has elapsed, leading to a service outage. With GPTCache, you can easily scale to accommodate an increasing volume of of queries, ensuring consistent performance as your application's user base expands.
+- **Flexible development environment**: When developing LLM applications, an LLM APIs connection is required to prove concepts. GPTCache offers the same interface as LLM APIs and can store LLM-generated or mocked data. This helps to verify your application's features without connecting to the LLM APIs or even the network.
+
+## 🤔 How does it work?
+
+Online services often exhibit data locality, with users frequently accessing popular or trending content. Cache systems take advantage of this behavior by storing commonly accessed data, which in turn reduces data retrieval time, improves response times, and eases the burden on backend servers. Traditional cache systems typically utilize an exact match between a new query and a cached query to determine if the requested content is available in the cache before fetching the data.
+
+However, using an exact match approach for LLM caches is less effective due to the complexity and variability of LLM queries, resulting in a low cache hit rate. To address this issue, GPTCache adopt alternative strategies like semantic caching. Semantic caching identifies and stores similar or related queries, thereby increasing cache hit probability and enhancing overall caching efficiency. 
+
+GPTCache employs embedding algorithms to convert queries into embeddings and uses a vector store for similarity search on these embeddings. This process allows GPTCache to identify and retrieve similar or related queries from the cache storage, as illustrated in the [Modules section](https://github.com/zilliztech/GPTCache#-modules). 
+
+Featuring a modular design, GPTCache makes it easy for users to customize their own semantic cache. The system offers various implementations for each module, and users can even develop their own implementations to suit their specific needs.
+
+In a semantic cache, false positives can occur during cache hits and false negatives during cache misses. GPTCache provides three metrics to evaluate its performance:
+
+- Precision: the ratio of true positives to the total of true positives and false positives.
+- Recall: the ratio of true positives to the total of true positives and false negatives.
+- Latency: the time required for a query to be processed and the corresponding data to be fetched from the cache.
+
+A [sample benchmark](https://github.com/zilliztech/gpt-cache/blob/main/examples/benchmark/benchmark_sqlite_faiss_onnx.py) is included for users to start with assessing the performance of their semantic cache.
+
 ## 🤗 Modules
 
 ![GPTCache Struct](docs/GPTCacheStructure.png)
 
 - **LLM Adapter**: 
 The LLM Adapter is designed to integrate different LLM models by unifying their APIs and request protocols. GPTCache offers a standardized interface for this purpose, with current support for ChatGPT integration.
   - [x] Support OpenAI ChatGPT API.
@@ -230,51 +242,51 @@
   - [x] Disable embedding. This will turn GPTCache into a keyword-matching cache.
   - [x] Support OpenAI embedding API.
   - [x] Support [ONNX](https://onnx.ai/) with the GPTCache/paraphrase-albert-onnx model.
   - [x] Support [Hugging Face](https://huggingface.co/) embedding API.
   - [x] Support [Cohere](https://docs.cohere.ai/reference/embed) embedding API.
   - [x] Support [fastText](https://fasttext.cc) embedding API.
   - [x] Support [SentenceTransformers](https://www.sbert.net) embedding API.
-  - [ ] Support other embedding apis
+  - [ ] Support other embedding APIs.
 - **Cache Storage**:
 **Cache Storage** is where the response from LLMs, such as ChatGPT, is stored. Cached responses are retrieved to assist in evaluating similarity and are returned to the requester if there is a good semantic match. At present, GPTCache supports SQLite and offers a universally accessible interface for extension of this module.
   - [x] Support [SQLite](https://sqlite.org/docs.html).
   - [x] Support [PostgreSQL](https://www.postgresql.org/).
   - [x] Support [MySQL](https://www.mysql.com/).
   - [x] Support [MariaDB](https://mariadb.org/).
   - [x] Support [SQL Server](https://www.microsoft.com/en-us/sql-server/).
   - [x] Support [Oracle](https://www.oracle.com/).
   - [ ] Support [MongoDB](https://www.mongodb.com/).
   - [ ] Support [Redis](https://redis.io/).
   - [ ] Support [Minio](https://min.io/).
   - [ ] Support [HBase](https://hbase.apache.org/).
-  - [ ] Support [ElasticSearch](https://www.elastic.co/)
-  - [ ] Support [zincsearch](https://zinc.dev/)
-  - [ ] Support other storages
+  - [ ] Support [ElasticSearch](https://www.elastic.co/).
+  - [ ] Support [Duckdb](https://github.com/duckdb/duckdb).
+  - [ ] Support other storages.
 - **Vector Store**:
 The **Vector Store** module helps find the K most similar requests from the input request's extracted embedding. The results can help assess similarity. GPTCache provides a user-friendly interface that supports various vector stores, including Milvus, Zilliz Cloud, and FAISS. More options will be available in the future.
-  - [x] Support [Milvus](https://milvus.io/).
-  - [x] Support [Zilliz Cloud](https://cloud.zilliz.com/).
-  - [x] Support [FAISS](https://faiss.ai/).
-  - [ ] Support other vector databases
+  - [x] Support [Milvus](https://milvus.io/), an open-source vector database for production-ready AI/LLM applicaionts. 
+  - [x] Support [Zilliz Cloud](https://cloud.zilliz.com/), a fully-managed cloud vector database based on Milvus.
+  - [x] Support [FAISS](https://faiss.ai/), a library for efficient similarity search and clustering of dense vectors.
+  - [ ] Support other vector databases.
 - **Cache Manager**:
 The **Cache Manager** is responsible for controlling the operation of both the **Cache Storage** and **Vector Store**.
   - **Eviction Policy**:
   Currently, GPTCache makes decisions about evictions based solely on the number of lines. This approach can result in inaccurate resource evaluation and may cause out-of-memory (OOM) errors. We are actively investigating and developing a more sophisticated strategy.
-    - [x] LRU eviction policy
-    - [x] FIFO eviction policy
-    - [ ] More complicated eviction policies
+    - [x] Support LRU eviction policy.
+    - [x] Support FIFO eviction policy.
+    - [ ] Support more complicated eviction policies.
 - **Similarity Evaluator**: 
 This module collects data from both the **Cache Storage** and **Vector Store**, and uses various strategies to determine the similarity between the input request and the requests from the **Vector Store**. Based on this similarity, it determines whether a request matches the cache. GPTCache provides a standardized interface for integrating various strategies, along with a collection of implementations to use. The following similarity definitions are currently supported or will be supported in the future:
   - [x] The distance we obtain from the **Vector Store**.
   - [x] A model-based similarity determined using the GPTCache/albert-duplicate-onnx model from [ONNX](https://onnx.ai/).
   - [x] Exact matches between the input request and the requests obtained from the **Vector Store**.
   - [x] Distance represented by applying linalg.norm from numpy to the embeddings.
-  - [ ] BM25 and other similarity measurements
-  - [ ] Support other model serving framework such as PyTorch
+  - [ ] BM25 and other similarity measurements.
+  - [ ] Support other model serving framework such as PyTorch.
  
   
   **Note**:Not all combinations of different modules may be compatible with each other. For instance, if we disable the **Embedding Extractor**, the **Vector Store** may not function as intended. We are currently working on implementing a combination sanity check for **GPTCache**.
 
 ## 😇 Roadmap
 Coming soon! [Stay tuned!](https://twitter.com/zilliz_universe)
```

### Comparing `gptcache-0.1.5/gptcache/__init__.py` & `gptcache-0.1.6/gptcache/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import atexit
 import os
 import time
 import openai
 
-from .embedding.string import to_embeddings as string_embedding
-from .manager.data_manager import DataManager
-from .manager.factory import get_user_data_manager
-from .processor.post import first
-from .processor.pre import last_content
-from .similarity_evaluation.similarity_evaluation import SimilarityEvaluation
-from .similarity_evaluation.exact_match import ExactMatchEvaluation
-from .utils.error import CacheError
+from gptcache.embedding.string import to_embeddings as string_embedding
+from gptcache.manager.data_manager import DataManager
+from gptcache.manager.factory import get_data_manager
+from gptcache.processor.post import first
+from gptcache.processor.pre import last_content
+from gptcache.similarity_evaluation.similarity_evaluation import SimilarityEvaluation
+from gptcache.similarity_evaluation.exact_match import ExactMatchEvaluation
+from gptcache.utils.error import CacheError
 
 
-def cache_all(*args, **kwargs):
+def cache_all(*_, **__):
     return True
 
 
 def time_cal(func, func_name=None, report_func=None):
     def inner(*args, **kwargs):
         time_start = time.time()
         res = func(*args, **kwargs)
         delta_time = time.time() - time_start
         if cache.config.log_time_func:
-            cache.config.log_time_func(func.__name__ if func_name is None else func_name, delta_time)
+            cache.config.log_time_func(
+                func.__name__ if func_name is None else func_name, delta_time
+            )
         if report_func is not None:
             report_func(delta_time)
         return res
 
     return inner
 
 
@@ -42,27 +44,29 @@
     Example:
         .. code-block:: python
 
             from gptcache import Config
 
             configs = Config(similarity_threshold=0.6)
     """
-    def __init__(self,
-                 log_time_func=None,
-                 similarity_threshold=0.8,
-                 ):
+
+    def __init__(
+        self,
+        log_time_func=None,
+        similarity_threshold=0.8,
+    ):
         if similarity_threshold < 0 or similarity_threshold > 1:
-            raise CacheError('Invalid the similarity threshold param')
+            raise CacheError("Invalid the similarity threshold param")
         self.log_time_func = log_time_func
         self.similarity_threshold = similarity_threshold
 
 
 class Report:
-    """Get GPTCache report including time and counts for different operations.
-    """
+    """Get GPTCache report including time and counts for different operations."""
+
     def __init__(self):
         self.embedding_all_time = 0
         self.embedding_count = 0
         self.search_all_time = 0
         self.search_count = 0
         self.hint_cache_count = 0
 
@@ -83,18 +87,28 @@
         self.search_count += 1
 
     def average_embedding_time(self):
         """Average embedding time.
 
         :param delta_time: delta time.
         """
-        return round(self.embedding_all_time / self.embedding_count if self.embedding_count != 0 else 0, 4)
+        return round(
+            self.embedding_all_time / self.embedding_count
+            if self.embedding_count != 0
+            else 0,
+            4,
+        )
 
     def average_search_time(self):
-        return round(self.search_all_time / self.search_count if self.embedding_count != 0 else 0, 4)
+        return round(
+            self.search_all_time / self.search_count
+            if self.embedding_count != 0
+            else 0,
+            4,
+        )
 
     def hint_cache(self):
         self.hint_cache_count += 1
 
 
 class Cache:
     """Initialize GPTCache.
@@ -107,45 +121,46 @@
 
             from gptcache import cache
             from gptcache.adapter import openai
 
             cache.init()
             cache.set_openai_key()
     """
+
     similarity_evaluation: SimilarityEvaluation
 
     # it should be called when start the cache system
     def __init__(self):
         self.has_init = False
         self.cache_enable_func = None
         self.pre_embedding_func = None
         self.embedding_func = None
         self.data_manager = None
         self.post_process_messages_func = None
         self.config = Config()
         self.report = Report()
         self.next_cache = None
 
-    def init(self,
-             cache_enable_func=cache_all,
-             pre_embedding_func=last_content,
-             embedding_func=string_embedding,
-             data_manager: DataManager = get_user_data_manager('map'),
-             similarity_evaluation=ExactMatchEvaluation(),
-             post_process_messages_func=first,
-             config=Config(),
-             next_cache=None,
-             **kwargs
-             ):
+    def init(
+        self,
+        cache_enable_func=cache_all,
+        pre_embedding_func=last_content,
+        embedding_func=string_embedding,
+        data_manager: DataManager = get_data_manager(),
+        similarity_evaluation=ExactMatchEvaluation(),
+        post_process_messages_func=first,
+        config=Config(),
+        next_cache=None,
+    ):
         """Pass parameters to initialize GPTCache.
 
         :param cache_enable_func: a function to enable cache, defaults to ``cache_all``
         :param pre_embedding_func: a function to preprocess embedding, defaults to ``last_content``
         :param embedding_func: a function to extract embeddings from requests for similarity search, defaults to ``string_embedding``
-        :param data_manager: a ``DataManager`` module, defaults to ``get_user_data_manager('map')``
+        :param data_manager: a ``DataManager`` module, defaults to ``get_data_manager()``
         :param similarity_evaluation: a module to calculate embedding similarity, defaults to ``ExactMatchEvaluation()``
         :param post_process_messages_func: a function to post-process messages, defaults to ``first``
         :param config: a module to pass configurations, defaults to ``Config()``
         :param next_cache: customized method for next cache
         """
         self.has_init = True
         self.cache_enable_func = cache_enable_func
@@ -157,16 +172,16 @@
         self.config = config
         self.next_cache = next_cache
 
         @atexit.register
         def close():
             try:
                 self.data_manager.close()
-            except Exception as e:
+            except Exception as e:  # pylint: disable=W0703
                 print(e)
 
     @staticmethod
     def set_openai_key():
-        openai.api_key = os.getenv('OPENAI_API_KEY')
+        openai.api_key = os.getenv("OPENAI_API_KEY")
 
 
 cache = Cache()
```

### Comparing `gptcache-0.1.5/gptcache/adapter/langchain_llms.py` & `gptcache-0.1.6/gptcache/adapter/langchain_llms.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 from typing import Optional, List
-from .adapter import adapt
+from gptcache.adapter.adapter import adapt
 
 
 class LangChainLLMs:
+    """LangChain LLM Wrapper"""
+
     def __init__(self, llm):
         self._llm = llm
 
     def __call__(self, prompt: str, stop: Optional[List[str]] = None, **kwargs):
         # TODO handle the array result
-        return adapt(self._llm, cache_data_convert, update_cache_callback, prompt=prompt, stop=stop, **kwargs)
+        return adapt(
+            self._llm,
+            cache_data_convert,
+            update_cache_callback,
+            prompt=prompt,
+            stop=stop,
+            **kwargs
+        )
 
 
 def cache_data_convert(cache_data):
     return cache_data
 
 
 def update_cache_callback(llm_data, update_cache_func):
```

### Comparing `gptcache-0.1.5/gptcache/embedding/__init__.py` & `gptcache-0.1.6/gptcache/embedding/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,35 @@
-__all__ = ['OpenAI', 'Huggingface', 'SBERT', 'Cohere', 'Onnx', 'FastText']
+__all__ = ["OpenAI", "Huggingface", "SBERT", "Cohere", "Onnx", "FastText"]
 
 
 from gptcache.utils.lazy_import import LazyImport
 
-openai = LazyImport('openai', globals(), 'gptcache.embedding.openai')
-huggingface = LazyImport('huggingface', globals(), 'gptcache.embedding.huggingface')
-sbert = LazyImport('sbert', globals(), 'gptcache.embedding.sbert')
-onnx = LazyImport('onnx', globals(), 'gptcache.embedding.onnx')
-cohere = LazyImport('cohere', globals(), 'gptcache.embedding.cohere')
-fasttext = LazyImport('fasttext', globals(), 'gptcache.embedding.fasttext')
+openai = LazyImport("openai", globals(), "gptcache.embedding.openai")
+huggingface = LazyImport("huggingface", globals(), "gptcache.embedding.huggingface")
+sbert = LazyImport("sbert", globals(), "gptcache.embedding.sbert")
+onnx = LazyImport("onnx", globals(), "gptcache.embedding.onnx")
+cohere = LazyImport("cohere", globals(), "gptcache.embedding.cohere")
+fasttext = LazyImport("fasttext", globals(), "gptcache.embedding.fasttext")
 
 
-def Cohere(model='large', api_key=None):
+def Cohere(model="large", api_key=None):
     return cohere.Cohere(model, api_key)
 
-def OpenAI(model='text-embedding-ada-002', api_key=None):
+
+def OpenAI(model="text-embedding-ada-002", api_key=None):
     return openai.OpenAI(model, api_key)
 
-def Huggingface(model='sentence-transformers/all-mpnet-base-v2'):
+
+def Huggingface(model="sentence-transformers/all-mpnet-base-v2"):
     return huggingface.Huggingface(model)
 
-def SBERT(model='all-MiniLM-L6-v2'):
+
+def SBERT(model="all-MiniLM-L6-v2"):
     return sbert.SBERT(model)
 
-def Onnx(model='GPTCache/paraphrase-albert-onnx'):
+
+def Onnx(model="GPTCache/paraphrase-albert-onnx"):
     return onnx.Onnx(model)
 
-def FastText(model='large', dim=None):
+
+def FastText(model="large", dim=None):
     return fasttext.FastText(model, dim)
```

### Comparing `gptcache-0.1.5/gptcache/embedding/cohere.py` & `gptcache-0.1.6/gptcache/embedding/cohere.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,65 @@
+import numpy as np
+
 from gptcache.utils import import_cohere
-import_cohere()
+from gptcache.embedding.base import BaseEmbedding
 
-import numpy as np
-import cohere
+import_cohere()
 
-from .base import BaseEmbedding
+import cohere  # pylint: disable=C0413
 
 
 class Cohere(BaseEmbedding):
     """Generate text embedding for given text using Cohere.
 
     :param model: model name (size), defaults to 'large'.
     :type model: str
     :param api_key: Cohere API Key.
     :type api_key: str
 
     Example:
         .. code-block:: python
 
             from gptcache.embedding import Cohere
-            
-            test_sentence = 'Hello, world.' 
+
+            test_sentence = 'Hello, world.'
             encoder = Cohere(model='small', api_key='your_cohere_key')
             embed = encoder.to_embeddings(test_sentence)
     """
-    def __init__(self, model: str='large', api_key: str=None, **kwargs):
+
+    def __init__(self, model: str = "large", api_key: str = None):
         self.co = cohere.Client(api_key)
         self.model = model
 
         if model in self.dim_dict():
             self.__dimension = self.dim_dict()[model]
         else:
             self.__dimension = None
-    
-    def to_embeddings(self, data):
+
+    def to_embeddings(self, data, **_):
         """Generate embedding given text input
 
         :param data: text in string.
         :type data: str
 
         :return: a text embedding in shape of (dim,).
         """
         if not isinstance(data, list):
             data = [data]
         response = self.co.embed(texts=data, model=self.model)
         embeddings = response.embeddings
-        return np.array(embeddings).astype('float32').squeeze(0)
+        return np.array(embeddings).astype("float32").squeeze(0)
 
     @property
     def dimension(self):
         """Embedding dimension.
 
         :return: embedding dimension
         """
         if not self.__dimension:
-            foo_emb = self.to_embeddings('foo')
+            foo_emb = self.to_embeddings("foo")
             self.__dimension = len(foo_emb)
         return self.__dimension
-    
+
     @staticmethod
     def dim_dict():
-        return {
-            'large': 4096,
-            'small': 1024
-        }
+        return {"large": 4096, "small": 1024}
```

### Comparing `gptcache-0.1.5/gptcache/embedding/fasttext.py` & `gptcache-0.1.6/gptcache/embedding/fasttext.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,55 @@
-from gptcache.utils import import_fasttext
-import_fasttext()
-
-import fasttext.util
 import numpy as np
 import os
 
-from .base import BaseEmbedding
+from gptcache.utils import import_fasttext
+from gptcache.embedding.base import BaseEmbedding
+
+import_fasttext()
+
+import fasttext.util  # pylint: disable=C0413
 
 
 class FastText(BaseEmbedding):
     """Generate sentence embedding for given text using pretrained models of different languages from fastText.
 
     :param model: model name, defaults to 'en'.
     :type model: str
     :param dim: reduced dimension of embedding. If this parameter is not provided, the embedding dimension (300) will not change.
     :type dim: int
 
     Example:
         .. code-block:: python
-        
+
             from gptcache.embedding import FastText
-            
-            test_sentence = 'Hello, world.' 
+
+            test_sentence = 'Hello, world.'
             encoder = FastText(model='en', dim=100)
             embed = encoder.to_embeddings(test_sentence)
     """
-    def __init__(self, model: str='en', dim: int=None):
+
+    def __init__(self, model: str = "en", dim: int = None):
         self.model_path = os.path.abspath(fasttext.util.download_model(model))
         self.ft = fasttext.load_model(self.model_path)
 
         if dim:
             fasttext.util.reduce_model(self.ft, dim)
         self.__dimension = self.ft.get_dimension()
 
-    def to_embeddings(self, data, **kwargs):
+    def to_embeddings(self, data, **_):
         """Generate embedding given text input
 
         :param data: text in string.
         :type data: str
 
         :return: a text embedding in shape of (dim,).
         """
-        assert isinstance(data, str), 'Only allow string as input.'
+        assert isinstance(data, str), "Only allow string as input."
         emb = self.ft.get_sentence_vector(data)
-        return np.array(emb).astype('float32')
+        return np.array(emb).astype("float32")
 
     @property
     def dimension(self):
         """Embedding dimension.
 
         :return: embedding dimension
         """
```

### Comparing `gptcache-0.1.5/gptcache/embedding/huggingface.py` & `gptcache-0.1.6/gptcache/embedding/huggingface.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,77 @@
+import numpy as np
+
 from gptcache.utils import import_huggingface, import_torch
+from gptcache.embedding.base import BaseEmbedding
+
 import_huggingface()
 import_torch()
 
-import numpy as np
-import torch
-from transformers import AutoTokenizer, AutoModel
-
-from .base import BaseEmbedding
+import torch  # pylint: disable=C0413
+from transformers import AutoTokenizer, AutoModel  # pylint: disable=C0413
 
 
 class Huggingface(BaseEmbedding):
     """Generate sentence embedding for given text using pretrained models from Huggingface transformers.
 
     :param model: model name, defaults to 'sentence-transformers/all-MiniLM-L6-v2'.
     :type model: str
 
     Example:
         .. code-block:: python
-        
+
             from gptcache.embedding import Huggingface
-            
-            test_sentence = 'Hello, world.' 
+
+            test_sentence = 'Hello, world.'
             encoder = Huggingface(model='sentence-transformers/all-MiniLM-L6-v2')
             embed = encoder.to_embeddings(test_sentence)
     """
-    def __init__(self, model: str='sentence-transformers/all-MiniLM-L6-v2'):
+
+    def __init__(self, model: str = "sentence-transformers/all-MiniLM-L6-v2"):
         self.model = AutoModel.from_pretrained(model)
         self.model.eval()
 
         self.tokenizer = AutoTokenizer.from_pretrained(model)
         if not self.tokenizer.pad_token:
-            self.tokenizer.pad_token = '[PAD]'
+            self.tokenizer.pad_token = "[PAD]"
         try:
             self.__dimension = self.model.config.hidden_size
-        except Exception:
-            from transformers import AutoConfig
+        except Exception:  # pylint: disable=W0703
+            from transformers import AutoConfig  # pylint: disable=C0415
+
             config = AutoConfig.from_pretrained(model)
             self.__dimension = config.hidden_size
 
-    def to_embeddings(self, data, **kwargs):
+    def to_embeddings(self, data, **_):
         """Generate embedding given text input
 
         :param data: text in string.
         :type data: str
 
         :return: a text embedding in shape of (dim,).
         """
         if not isinstance(data, list):
             data = [data]
-        inputs = self.tokenizer(data, padding=True, truncation=True, return_tensors='pt')
+        inputs = self.tokenizer(
+            data, padding=True, truncation=True, return_tensors="pt"
+        )
         outs = self.model(**inputs).last_hidden_state
         emb = self.post_proc(outs, inputs).squeeze(0).detach().numpy()
-        return np.array(emb).astype('float32')
-    
+        return np.array(emb).astype("float32")
+
     def post_proc(self, token_embeddings, inputs):
-        attention_mask = inputs['attention_mask']
-        input_mask_expanded = attention_mask.unsqueeze(-1).expand(token_embeddings.size()).float()
+        attention_mask = inputs["attention_mask"]
+        input_mask_expanded = (
+            attention_mask.unsqueeze(-1).expand(token_embeddings.size()).float()
+        )
         sentence_embs = torch.sum(
-            token_embeddings * input_mask_expanded, 1) / torch.clamp(input_mask_expanded.sum(1), min=1e-9)
+            token_embeddings * input_mask_expanded, 1
+        ) / torch.clamp(input_mask_expanded.sum(1), min=1e-9)
         return sentence_embs
 
     @property
     def dimension(self):
         """Embedding dimension.
 
         :return: embedding dimension
         """
-        return self.__dimension
+        return self.__dimension
```

### Comparing `gptcache-0.1.5/gptcache/embedding/onnx.py` & `gptcache-0.1.6/gptcache/embedding/onnx.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,66 +1,80 @@
-from gptcache.utils import import_onnxruntime, import_huggingface_hub, import_huggingface
+import numpy as np
+
+from gptcache.embedding.base import BaseEmbedding
+from gptcache.utils import (
+    import_onnxruntime,
+    import_huggingface_hub,
+    import_huggingface,
+)
+
 import_huggingface()
 import_onnxruntime()
 import_huggingface_hub()
-import numpy as np
-from transformers import AutoTokenizer, AutoConfig
-from huggingface_hub import hf_hub_download
-import onnxruntime
 
-from .base import BaseEmbedding
+from transformers import AutoTokenizer, AutoConfig  # pylint: disable=C0413
+from huggingface_hub import hf_hub_download  # pylint: disable=C0413
+import onnxruntime  # pylint: disable=C0413
 
 
 class Onnx(BaseEmbedding):
     """Generate text embedding for given text using ONNX Model.
 
     Example:
         .. code-block:: python
-        
+
             from gptcache.embedding import Onnx
 
             test_sentence = 'Hello, world.'
             encoder = Onnx(model='GPTCache/paraphrase-albert-onnx')
             embed = encoder.to_embeddings(test_sentence)
     """
-    def __init__(self, api_key, model= 'GPTCache/paraphrase-albert-onnx', **kwargs):
-        tokenizer_name = 'sentence-transformers/paraphrase-albert-small-v2'
+
+    def __init__(self, model="GPTCache/paraphrase-albert-onnx"):
+        tokenizer_name = "sentence-transformers/paraphrase-albert-small-v2"
         self.tokenizer = AutoTokenizer.from_pretrained(tokenizer_name)
         self.model = model
-        onnx_model_path = hf_hub_download(repo_id=model, filename = 'model.onnx')
+        onnx_model_path = hf_hub_download(repo_id=model, filename="model.onnx")
         self.ort_session = onnxruntime.InferenceSession(onnx_model_path)
-        config = AutoConfig.from_pretrained('sentence-transformers/paraphrase-albert-small-v2')
+        config = AutoConfig.from_pretrained(
+            "sentence-transformers/paraphrase-albert-small-v2"
+        )
         self.__dimension = config.hidden_size
 
-    
-    def to_embeddings(self, data, **kwargs):
+    def to_embeddings(self, data, **_):
         """Generate embedding given text input.
 
         :param data: text in string.
         :type data: str
 
         :return: a text embedding in shape of (dim,).
         """
-        encoded_text = self.tokenizer.encode_plus(data, padding='max_length')
-        ort_inputs = {'input_ids': np.array(encoded_text['input_ids']).reshape(1,-1), 
-               'attention_mask': np.array(encoded_text['attention_mask']).reshape(1,-1),
-               'token_type_ids': np.array(encoded_text['token_type_ids']).reshape(1,-1)}
+        encoded_text = self.tokenizer.encode_plus(data, padding="max_length")
+        ort_inputs = {
+            "input_ids": np.array(encoded_text["input_ids"]).reshape(1, -1),
+            "attention_mask": np.array(encoded_text["attention_mask"]).reshape(1, -1),
+            "token_type_ids": np.array(encoded_text["token_type_ids"]).reshape(1, -1),
+        }
 
         ort_outputs = self.ort_session.run(None, ort_inputs)
         ort_feat = ort_outputs[0]
-        emb = self.post_proc(ort_feat, ort_inputs['attention_mask'])
+        emb = self.post_proc(ort_feat, ort_inputs["attention_mask"])
         return emb.flatten()
 
-    def post_proc(self, token_embeddings, attention_mask): 
-        token_embeddings = token_embeddings
-        input_mask_expanded = np.expand_dims(attention_mask, -1).repeat(token_embeddings.shape[-1], -1).astype(float)
-        sentence_embs = np.sum(token_embeddings * input_mask_expanded, 1) / np.maximum(input_mask_expanded.sum(1), 1e-9)
+    def post_proc(self, token_embeddings, attention_mask):
+        input_mask_expanded = (
+            np.expand_dims(attention_mask, -1)
+            .repeat(token_embeddings.shape[-1], -1)
+            .astype(float)
+        )
+        sentence_embs = np.sum(token_embeddings * input_mask_expanded, 1) / np.maximum(
+            input_mask_expanded.sum(1), 1e-9
+        )
         return sentence_embs
 
     @property
     def dimension(self):
         """Embedding dimension.
 
         :return: embedding dimension
         """
         return self.__dimension
-
```

### Comparing `gptcache-0.1.5/gptcache/embedding/openai.py` & `gptcache-0.1.6/gptcache/embedding/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,67 +1,63 @@
 import numpy as np
 import openai
 import os
 
-from .base import BaseEmbedding
+from gptcache.embedding.base import BaseEmbedding
 
 
 class OpenAI(BaseEmbedding):
     """Generate text embedding for given text using OpenAI.
 
     :param model: model name, defaults to 'text-embedding-ada-002'.
     :type model: str
     :param api_key: OpenAI API Key. When the parameter is not specified, it will load the key by default if it is available.
     :type api_key: str
 
     Example:
         .. code-block:: python
 
             from gptcache.embedding import OpenAI
-            
-            test_sentence = 'Hello, world.' 
+
+            test_sentence = 'Hello, world.'
             encoder = OpenAI(api_key='your_openai_key')
             embed = encoder.to_embeddings(test_sentence)
     """
-    def __init__(self, model: str='text-embedding-ada-002', api_key: str=None, **kwargs):
+
+    def __init__(self, model: str = "text-embedding-ada-002", api_key: str = None):
         if not api_key:
             if openai.api_key:
                 api_key = openai.api_key
             else:
-                api_key = os.getenv('OPENAI_API_KEY')
+                api_key = os.getenv("OPENAI_API_KEY")
         openai.api_key = api_key
         self.model = model
         if model in self.dim_dict():
             self.__dimension = self.dim_dict()[model]
         else:
             self.__dimension = None
-    
-    def to_embeddings(self, data):
+
+    def to_embeddings(self, data, **_):
         """Generate embedding given text input
 
         :param data: text in string.
         :type data: str
 
         :return: a text embedding in shape of (dim,).
         """
-        sentence_embeddings = openai.Embedding.create(
-            model=self.model,
-            input=data
-        )
-        return np.array(sentence_embeddings['data'][0]['embedding']).astype('float32')
+        sentence_embeddings = openai.Embedding.create(model=self.model, input=data)
+        return np.array(sentence_embeddings["data"][0]["embedding"]).astype("float32")
 
     @property
     def dimension(self):
         """Embedding dimension.
 
         :return: embedding dimension
         """
         if not self.__dimension:
-            foo_emb = self.to_embeddings('foo')
+            foo_emb = self.to_embeddings("foo")
             self.__dimension = len(foo_emb)
         return self.__dimension
-    
+
     @staticmethod
     def dim_dict():
-        return {
-            'text-embedding-ada-002': 1536
-        }
+        return {"text-embedding-ada-002": 1536}
```

### Comparing `gptcache-0.1.5/gptcache/embedding/sbert.py` & `gptcache-0.1.6/gptcache/embedding/sbert.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,55 @@
+import numpy as np
 from gptcache.utils import import_sbert
-import_sbert()
+from gptcache.embedding.base import BaseEmbedding
 
-import numpy as np
-from sentence_transformers import SentenceTransformer
+import_sbert()
 
-from .base import BaseEmbedding
+from sentence_transformers import SentenceTransformer  # pylint: disable=C0413
 
 
 class SBERT(BaseEmbedding):
     """Generate sentence embedding for given text using pretrained models of Sentence Transformers.
 
     :param model: model name, defaults to 'all-MiniLM-L6-v2'.
     :type model: str
 
     Example:
         .. code-block:: python
-        
+
             from gptcache.embedding import SBERT
-            
-            test_sentence = 'Hello, world.' 
+
+            test_sentence = 'Hello, world.'
             encoder = SBERT('paraphrase-albert-small-v2')
             embed = encoder.to_embeddings(test_sentence)
     """
-    def __init__(self, model: str='all-MiniLM-L6-v2'):
+
+    def __init__(self, model: str = "all-MiniLM-L6-v2"):
         self.model = SentenceTransformer(model)
         self.model.eval()
         self.__dimension = None
 
-    def to_embeddings(self, data, **kwargs):
+    def to_embeddings(self, data, **_):
         """Generate embedding given text input
 
         :param data: text in string.
         :type data: str
 
         :return: a text embedding in shape of (dim,).
         """
         if not isinstance(data, list):
             data = [data]
         emb = self.model.encode(data).squeeze(0)
 
         if not self.__dimension:
             self.__dimension = len(emb)
-        return np.array(emb).astype('float32')
-    
+        return np.array(emb).astype("float32")
+
     @property
     def dimension(self):
         """Embedding dimension.
 
         :return: embedding dimension
         """
         if not self.__dimension:
-            self.__dimension == self.to_embeddings('foo')
+            self.__dimension = self.to_embeddings("foo")
         return self.__dimension
```

### Comparing `gptcache-0.1.5/gptcache/manager/data_manager.py` & `gptcache-0.1.6/gptcache/manager/data_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,129 +1,124 @@
-import hashlib
 from abc import abstractmethod, ABCMeta
 import pickle
 import cachetools
 import numpy as np
 
 from gptcache.utils.error import CacheError
-from .scalar_data.base import CacheStorage
-from .vector_data.base import VectorBase, ClearStrategy
-from .eviction import EvictionManager
+from gptcache.manager.scalar_data.base import CacheStorage
+from gptcache.manager.vector_data.base import VectorBase, ClearStrategy
+from gptcache.manager.eviction import EvictionManager
 
 
 class DataManager(metaclass=ABCMeta):
+    """DataManager manage the cache data, including save and search"""
+
     @abstractmethod
     def save(self, question, answer, embedding_data, **kwargs):
         pass
 
     # should return the tuple, (question, answer)
     @abstractmethod
-    def get_scalar_data(self, vector_data, **kwargs):
+    def get_scalar_data(self, res_data, **kwargs):
         pass
 
     @abstractmethod
     def search(self, embedding_data, **kwargs):
         pass
 
     @abstractmethod
     def close(self):
         pass
 
 
 class MapDataManager(DataManager):
+    """MapDataManager, store all data in a map data structure."""
+
     def __init__(self, data_path, max_size, get_data_container=None):
         if get_data_container is None:
             self.data = cachetools.LRUCache(max_size)
         else:
             self.data = get_data_container(max_size)
         self.data_path = data_path
         self.init()
 
-    def init(self, **kwargs):
+    def init(self):
         try:
-            f = open(self.data_path, 'rb')
-            self.data = pickle.load(f)
-            f.close()
+            with open(self.data_path, "rb") as f:
+                self.data = pickle.load(f)
         except FileNotFoundError:
-            # print(f'File <${self.data_path}> is not found.')
             return
         except PermissionError:
-            raise CacheError(f'You don\'t have permission to access this file <${self.data_path}>.')
+            raise CacheError(  # pylint: disable=W0707
+                f"You don't have permission to access this file <${self.data_path}>."
+            )
 
     def save(self, question, answer, embedding_data, **kwargs):
         self.data[embedding_data] = (question, answer)
 
-    def get_scalar_data(self, vector_data, **kwargs):
-        return vector_data
+    def get_scalar_data(self, res_data, **kwargs):
+        return res_data
 
     def search(self, embedding_data, **kwargs):
         try:
             return [self.data[embedding_data]]
         except KeyError:
             return []
 
     def close(self):
         try:
-            f = open(self.data_path, 'wb')
-            pickle.dump(self.data, f)
-            f.close()
+            with open(self.data_path, "wb") as f:
+                pickle.dump(self.data, f)
         except PermissionError:
-            print(f'You don\'t have permission to access this file <${self.data_path}>.')
-
-
-def sha_data(data):
-    if isinstance(data, list):
-        data = np.array(data)
-    m = hashlib.sha1()
-    m.update(data.astype('float32').tobytes())
-    return m.hexdigest()
+            print(f"You don't have permission to access this file <${self.data_path}>.")
 
 
 def normalize(vec):
     magnitude = np.linalg.norm(vec)
     normalized_v = vec / magnitude
     return normalized_v
 
 
 class SSDataManager(DataManager):
     """Generate SSDataManage to manager the data.
 
-    :param max_size: the max size for the cache, defaults to 1000.
-    :type max_size: int.
-    :param clean_size: the size to clean up, defaults to `max_size * 0.2`.
-    :type clean_size: int.
     :param s: CacheStorage to manager the scalar data.
     :type s: CacheStorage.
     :param v: VectorBase to manager the vector data.
     :type v:  VectorBase.
+    :param max_size: the max size for the cache, defaults to 1000.
+    :type max_size: int.
+    :param clean_size: the size to clean up, defaults to `max_size * 0.2`.
+    :type clean_size: int.
     :param eviction: The eviction policy, it is support "LRU" and "FIFO" now, and defaults to "LRU".
     :type eviction:  str.
     """
+
     s: CacheStorage
     v: VectorBase
 
-    def __init__(self, max_size, clean_size, s, v, eviction='LRU'):
+    def __init__(self, s, v, max_size, clean_size, eviction="LRU"):
         self.max_size = max_size
         self.cur_size = 0
         self.clean_size = clean_size
         self.s = s
         self.v = v
-        self.eviction = EvictionManager(s, v, eviction)
+        self.eviction = EvictionManager(self.s, self.v, eviction)
         self.cur_size = self.s.count()
 
     def _clear(self):
         self.eviction.soft_evict(self.clean_size)
         if not self.eviction.check_evict():
             pass
         elif self.v.clear_strategy() == ClearStrategy.DELETE:
             self.eviction.delete()
         elif self.v.clear_strategy() == ClearStrategy.REBUILD:
             self.eviction.rebuild()
         else:
-            raise RuntimeError('Unknown clear strategy')
+            raise RuntimeError("Unknown clear strategy")
         self.cur_size = self.s.count()
 
     def save(self, question, answer, embedding_data, **kwargs):
         """Save the data and vectors to cache and vector storage.
 
         :param question: question data.
         :type question: str
@@ -132,33 +127,32 @@
         :param embedding_data: vector data.
         :type embedding_data: np.ndarray
 
         Example:
             .. code-block:: python
 
                 import numpy as np
-                from gptcache.manager.factory import get_data_manager
+                from gptcache.manager import get_data_manager, CacheBase, VectorBase
 
-                data_manager = get_data_manager("sqlite", "faiss", dimension=128)
+                data_manager = get_data_manager(CacheBase('sqlite'), VectorBase('faiss', dimension=128))
                 data_manager.save('hello', 'hi', np.random.random((128, )).astype('float32'))
         """
 
         if self.cur_size >= self.max_size:
             self._clear()
         embedding_data = normalize(embedding_data)
-        key = sha_data(embedding_data)
-        self.s.insert(key, question, answer, embedding_data.astype('float32'))
+        if self.v.clear_strategy() == ClearStrategy.DELETE:
+            key = self.s.insert(question, answer)
+        elif self.v.clear_strategy() == ClearStrategy.REBUILD:
+            key = self.s.insert(question, answer, embedding_data.astype("float32"))
         self.v.add(key, embedding_data)
         self.cur_size += 1
 
-    def get_scalar_data(self, search_data, **kwargs):
-        distance, vector_data = search_data
-        key = sha_data(vector_data)
-        self.s.update_access_time(key)
-        return self.s.get_data_by_id(key)
+    def get_scalar_data(self, res_data, **kwargs):
+        return self.s.get_data_by_id(res_data[1])
 
     def search(self, embedding_data, **kwargs):
         embedding_data = normalize(embedding_data)
         return self.v.search(embedding_data)
 
     def close(self):
         self.s.close()
```

### Comparing `gptcache-0.1.5/gptcache/manager/eviction.py` & `gptcache-0.1.6/gptcache/manager/eviction.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 import numpy as np
 
 
 class EvictionManager:
+    """
+    EvictionManager to manager the eviction policy.
+    """
+
     MAX_MARK_COUNT = 5000
     MAX_MARK_RATE = 0.1
     BATCH_SIZE = 100000
 
     def __init__(self, scalar_storage, vector_base, policy="LRU"):
         self._scalar_storage = scalar_storage
         self._vector_base = vector_base
         self._policy = policy
 
     def check_evict(self):
         mark_count = self._scalar_storage.count(state=-1)
         all_count = self._scalar_storage.count(is_all=True)
-        if mark_count > self.MAX_MARK_COUNT or mark_count / all_count > self.MAX_MARK_RATE:
+        if (
+            mark_count > self.MAX_MARK_COUNT
+            or mark_count / all_count > self.MAX_MARK_RATE
+        ):
             return True
         return False
 
     def delete(self):
         mark_ids = self._scalar_storage.get_ids_by_state(state=-1)
         mark_ids = [i[0] for i in mark_ids]
         self._scalar_storage.remove_by_state()
         self._vector_base.delete(mark_ids)
 
     def rebuild(self):
         self._scalar_storage.remove_by_state()
         count = self._scalar_storage.count()
         offset = 0
         while offset < count:
-            data = self._scalar_storage.get_embedding_data(offset, self.BATCH_SIZE)
-            np_data = [np.frombuffer(d[0], np.float32) for d in data]
-            self._vector_base.rebuild(np_data)
+            res = self._scalar_storage.get_embedding_data(offset, self.BATCH_SIZE)
+            ids = [d[0] for d in res]
+            np_data = [np.frombuffer(d[1], np.float32) for d in res]
+            self._vector_base.rebuild(np_data, ids)
             offset += self.BATCH_SIZE
 
     def soft_evict(self, count):
         if self._policy == "FIFO":
             marked_keys = self._scalar_storage.get_old_create(count)
         else:
             marked_keys = self._scalar_storage.get_old_access(count)
```

### Comparing `gptcache-0.1.5/gptcache/manager/scalar_data/base.py` & `gptcache-0.1.6/gptcache/manager/scalar_data/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 import numpy as np
 
 
 class CacheStorage(metaclass=ABCMeta):
     """
     BaseStorage for scalar data.
     """
+
     @abstractmethod
     def create(self):
         pass
 
     @abstractmethod
-    def insert(self, key, data, reply, embedding_data: np.ndarray = None):
+    def insert(self, data, reply, embedding_data: np.ndarray = None):
         pass
 
     @abstractmethod
     def get_data_by_id(self, key):
         pass
 
     @abstractmethod
@@ -44,13 +45,9 @@
         pass
 
     @abstractmethod
     def get_old_create(self, count):
         pass
 
     @abstractmethod
-    def count(self):
-        pass
-
-    @abstractmethod
     def close(self):
         pass
```

### Comparing `gptcache-0.1.5/gptcache/manager/scalar_data/sqlalchemy.py` & `gptcache-0.1.6/gptcache/manager/scalar_data/sqlalchemy.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,114 +1,167 @@
-from gptcache.utils import import_sqlalchemy
-import_sqlalchemy()
-
 import numpy as np
 from datetime import datetime
-from sqlalchemy import func, create_engine, Column, Sequence
-from sqlalchemy.types import String, DateTime, LargeBinary, Integer
-from sqlalchemy.orm import sessionmaker
-from sqlalchemy.ext.declarative import declarative_base
 
-from .base import CacheStorage
+from gptcache.utils import import_sqlalchemy
+from gptcache.manager.scalar_data.base import CacheStorage
+
+import_sqlalchemy()
+
+from sqlalchemy import func, create_engine, Column, Sequence  # pylint: disable=C0413
+from sqlalchemy.types import (  # pylint: disable=C0413
+    String,
+    DateTime,
+    LargeBinary,
+    Integer,
+)
+from sqlalchemy.orm import sessionmaker  # pylint: disable=C0413
+from sqlalchemy.ext.declarative import declarative_base  # pylint: disable=C0413
 
 Base = declarative_base()
 
 
 def get_model(table_name, db_type):
     class CacheTable(Base):
         """
         cache_table
         """
+
         __tablename__ = table_name
-        __table_args__ = {'extend_existing': True}
+        __table_args__ = {"extend_existing": True}
 
-        uid = Column(Integer, primary_key=True, autoincrement=True)
-        id = Column(String(500), nullable=False)
+        id = Column(Integer, primary_key=True, autoincrement=True)
         data = Column(String(1000), nullable=False)
         reply = Column(String(1000), nullable=False)
         create_on = Column(DateTime, default=datetime.now)
         last_access = Column(DateTime, default=datetime.now)
         embedding_data = Column(LargeBinary, nullable=True)
         state = Column(Integer, default=0)
+        type = Column(Integer, default=0)
 
     class CacheTableSequence(Base):
         """
         cache_table sequence
         """
+
         __tablename__ = table_name
-        __table_args__ = {'extend_existing': True}
+        __table_args__ = {"extend_existing": True}
 
-        uid = Column(Integer, Sequence('id_seq', start=1), primary_key=True, autoincrement=True)
-        id = Column(String(500), nullable=False)
+        id = Column(
+            Integer, Sequence("id_seq", start=1), primary_key=True, autoincrement=True
+        )
         data = Column(String(1000), nullable=False)
         reply = Column(String(1000), nullable=False)
         create_on = Column(DateTime, default=datetime.now)
         last_access = Column(DateTime, default=datetime.now)
         embedding_data = Column(LargeBinary, nullable=True)
         state = Column(Integer, default=0)
+        type = Column(Integer, default=0)
 
-    if db_type == 'oracle':
+    if db_type == "oracle":
         return CacheTableSequence
     else:
         return CacheTable
 
 
 class SQLDataBase(CacheStorage):
     """
     Using sqlalchemy to manage SQLite, PostgreSQL, MySQL, MariaDB, SQL Server and Oracle.
     """
-    def __init__(self, db_type: str = 'sqlite', url: str = 'sqlite:///./gptcache.db', table_name: str = 'gptcache'):
+
+    def __init__(
+            self,
+            db_type: str = "sqlite",
+            url: str = "sqlite:///./sqlite.db",
+            table_name: str = "gptcache",
+    ):
         self._url = url
         self._model = get_model(table_name, db_type)
         self._engine = create_engine(self._url)
-        Session = sessionmaker(bind=self._engine)
+        Session = sessionmaker(bind=self._engine)  # pylint: disable=invalid-name
         self._session = Session()
         self.create()
 
     def create(self):
         self._model.__table__.create(bind=self._engine, checkfirst=True)
 
-    def insert(self, key, data, reply, embedding_data: np.ndarray = None):
-        embedding_data = embedding_data.tobytes()
-        model_obj = self._model(id=key, data=data, reply=reply, embedding_data=embedding_data)
+    def insert(self, data, reply, embedding_data: np.ndarray = None):
+        if embedding_data is None:
+            model_obj = self._model(data=data, reply=reply)
+        else:
+            embedding_data = embedding_data.tobytes()
+            model_obj = self._model(data=data, reply=reply, embedding_data=embedding_data)
         self._session.add(model_obj)
         self._session.commit()
+        return model_obj.id
 
     def get_data_by_id(self, key):
-        res = self._session.query(self._model.data, self._model.reply).filter(self._model.id == key).filter(self._model.state == 0).first()
+        res = (
+            self._session.query(self._model.data, self._model.reply)
+            .filter(self._model.id == key)
+            .filter(self._model.state == 0)
+            .first()
+        )
         return res
 
     def get_ids_by_state(self, state):
-        res = self._session.query(self._model.id).filter(self._model.state == state).all()
+        res = (
+            self._session.query(self._model.id).filter(self._model.state == state).all()
+        )
         return res
 
     def get_embedding_data(self, offset, size):
-        res = self._session.query(self._model.embedding_data).order_by(self._model.uid.asc()).limit(size).offset(offset).all()
+        res = (
+            self._session.query(self._model.id, self._model.embedding_data)
+            .order_by(self._model.id.asc())
+            .limit(size)
+            .offset(offset)
+            .all()
+        )
         return res
 
     def update_access_time(self, key):
-        self._session.query(self._model).filter(self._model.id == key).update({'last_access': datetime.now()})
+        self._session.query(self._model).filter(self._model.id == key).update(
+            {"last_access": datetime.now()}
+        )
         self._session.commit()
 
     def get_old_access(self, count):
-        res = self._session.query(self._model.id).order_by(self._model.last_access.asc()).filter(self._model.state == 0).limit(count).all()
+        res = (
+            self._session.query(self._model.id)
+            .order_by(self._model.last_access.asc())
+            .filter(self._model.state == 0)
+            .limit(count)
+            .all()
+        )
         return res
 
     def get_old_create(self, count):
-        res = self._session.query(self._model.id).order_by(self._model.create_on.asc()).filter(self._model.state == 0).limit(count).all()
+        res = (
+            self._session.query(self._model.id)
+            .order_by(self._model.create_on.asc())
+            .filter(self._model.state == 0)
+            .limit(count)
+            .all()
+        )
         return res
 
     def update_state(self, keys):
-        self._session.query(self._model).filter(self._model.id.in_(keys)).update({'state': -1})
+        self._session.query(self._model).filter(self._model.id.in_(keys)).update(
+            {"state": -1}
+        )
         self._session.commit()
 
     def remove_by_state(self):
         self._session.query(self._model).filter(self._model.state == -1).delete()
         self._session.commit()
 
     def count(self, state: int = 0, is_all: bool = False):
         if is_all:
             return self._session.query(func.count(self._model.id)).scalar()
-        return self._session.query(func.count(self._model.id)).filter(self._model.state == state).scalar()
+        return (
+            self._session.query(func.count(self._model.id))
+            .filter(self._model.state == state)
+            .scalar()
+        )
 
     def close(self):
         self._session.close()
```

### Comparing `gptcache-0.1.5/gptcache/similarity_evaluation/__init__.py` & `gptcache-0.1.6/gptcache/similarity_evaluation/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,34 @@
-__all__ = ['OnnxModelEvaluation', 'NumpyNormEvaluation', 'SearchDistanceEvaluation', 'ExactMatchEvaluation']
+from gptcache.similarity_evaluation.similarity_evaluation import SimilarityEvaluation
+
+__all__ = [
+    "SimilarityEvaluation",
+    "OnnxModelEvaluation",
+    "NumpyNormEvaluation",
+    "SearchDistanceEvaluation",
+    "ExactMatchEvaluation",
+]
 
 from gptcache.utils.lazy_import import LazyImport
 
-onnx = LazyImport('onnx', globals(), 'gptcache.similarity_evaluation.onnx')
-np = LazyImport('np', globals(), 'gptcache.similarity_evaluation.np')
-distance = LazyImport('simple', globals(), 'gptcache.similarity_evaluation.distance')
-exact_match = LazyImport('exact_match', globals(), 'gptcache.similarity_evaluation.exact_match')
+onnx = LazyImport("onnx", globals(), "gptcache.similarity_evaluation.onnx")
+np = LazyImport("np", globals(), "gptcache.similarity_evaluation.np")
+distance = LazyImport("simple", globals(), "gptcache.similarity_evaluation.distance")
+exact_match = LazyImport(
+    "exact_match", globals(), "gptcache.similarity_evaluation.exact_match"
+)
+
 
-def OnnxModelEvaluation(model = 'GPTCache/albert-duplicate-onnx'):
+def OnnxModelEvaluation(model="GPTCache/albert-duplicate-onnx"):
     return onnx.OnnxModelEvaluation(model)
 
+
 def NumpyNormEvaluation(enable_normal: bool = False):
     return np.NumpyNormEvaluation(enable_normal)
 
-def SearchDistanceEvaluation(max_distance = 4.0, positive = False):
+
+def SearchDistanceEvaluation(max_distance=4.0, positive=False):
     return distance.SearchDistanceEvaluation(max_distance, positive)
 
+
 def ExactMatchEvaluation():
     return exact_match.ExactMatchEvaluation()
```

### Comparing `gptcache-0.1.5/gptcache/similarity_evaluation/distance.py` & `gptcache-0.1.6/gptcache/similarity_evaluation/distance.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,57 @@
-from .similarity_evaluation import SimilarityEvaluation
+from typing import Tuple, Dict, Any
+
+from gptcache.similarity_evaluation import SimilarityEvaluation
 
 
 class SearchDistanceEvaluation(SimilarityEvaluation):
     """Using search distance to evaluate sentences pair similarity.
 
-    :param max_distance: the bound of maximum distance. 
+    :param max_distance: the bound of maximum distance.
     :type max_distance: float
     :param positive: if the larger distance indicates more similar of two entities, It is True. Otherwise it is False.
     :type positive: bool
 
     Example:
         .. code-block:: python
-        
+
             from gptcache.similarity_evaluation import SearchDistanceEvaluation
-            
+
             evaluation = SearchDistanceEvaluation()
             score = evaluation.evaluation(
                 {},
                 {
                     "search_result": (1, None)
                 }
             )
     """
 
     def __init__(self, max_distance=4.0, positive=False):
         self.max_distance = max_distance
         self.positive = positive
 
-    def evaluation(self, src_dict, cache_dict, **kwargs):
+    def evaluation(
+        self, src_dict: Dict[str, Any], cache_dict: Dict[str, Any], **_
+    ) -> float:
         """Evaluate the similarity score of pair.
         :param src_dict: the query dictionary to evaluate with cache.
         :type src_dict: Dict
         :param cache_dict: the cache dictionary.
         :type cache_dict: Dict
 
         :return: evaluation score.
         """
-        distance, _ = cache_dict['search_result']
+        distance, _ = cache_dict["search_result"]
         if distance < 0:
             distance = 0
         elif distance > self.max_distance:
             distance = self.max_distance
         if self.positive:
             return distance
         return self.max_distance - distance
 
-    def range(self):
+    def range(self) -> Tuple[float, float]:
         """Range of similarity score.
-        
+
         :return: minimum and maximum of similarity score.
         """
         return 0.0, self.max_distance
```

### Comparing `gptcache-0.1.5/gptcache/similarity_evaluation/exact_match.py` & `gptcache-0.1.6/gptcache/similarity_evaluation/exact_match.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,47 @@
-from .similarity_evaluation import SimilarityEvaluation
+from typing import Tuple, Dict, Any
+
+from gptcache.similarity_evaluation.similarity_evaluation import SimilarityEvaluation
 
 
 class ExactMatchEvaluation(SimilarityEvaluation):
     """Using exact metric to evaluate sentences pair similarity.
 
     Example:
         .. code-block:: python
 
             from gptcache.similarity_evaluation import ExactMatchEvaluation
-            
+
             evaluation = ExactMatchEvaluation()
             score = evaluation.evaluation(
-                {   
-                    "question": "What is the color of sky?" 
+                {
+                    "question": "What is the color of sky?"
                 },
                 {
                     "question": "What is the color of sky?"
                 }
             )
     """
+
     def __init__(self):
         pass
 
-    def evaluation(self, src_dict, cache_dict, **kwargs):
+    def evaluation(
+        self, src_dict: Dict[str, Any], cache_dict: Dict[str, Any], **_
+    ) -> float:
         """Evaluate the similarity score of pair.
-        
+
         :param src_dict: the query dictionary to evaluate with cache_dict.
         :type src_dict: Dict
         :param cache_dict: the cache dictionary.
         :type cache_dict: Dict
 
         :return: evaluation score.
         """
-        return 1 if cache_dict['question'] == src_dict['question'] else 0
+        return 1 if cache_dict["question"] == src_dict["question"] else 0
 
-    def range(self):
+    def range(self) -> Tuple[float, float]:
         """Range of similarity score.
-        
+
         :return: minimum and maximum of similarity score.
         """
         return 0, 1
```

### Comparing `gptcache-0.1.5/gptcache/similarity_evaluation/np.py` & `gptcache-0.1.6/gptcache/similarity_evaluation/np.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,75 @@
+from typing import Dict, Tuple, Any
+
 import numpy as np
 
-from .similarity_evaluation import SimilarityEvaluation
+from gptcache.similarity_evaluation import SimilarityEvaluation
 
 
 class NumpyNormEvaluation(SimilarityEvaluation):
     """Using Numpy norm to evaluate sentences pair similarity.
 
     :param enable_normal: whether to normalize the embedding, defaults to False.
-    :type enable_normal: bool 
+    :type enable_normal: bool
 
     Example:
         .. code-block:: python
 
             from gptcache.similarity_evaluation import NumpyNormEvaluation
             import numpy as np
-            
+
             evaluation = NumpyNormEvaluation()
             score = evaluation.evaluation(
                 {
                     'embedding': np.array([-0.5, -0.5])
                 },
                 {
                     'search_result': (0, np.array([1, 1]))
                 }
             )
     """
 
-    def __init__(self, enable_normal: bool = False):
+    def __init__(self, enable_normal: bool = True):
         self.enable_normal = enable_normal
 
     @staticmethod
-    def normalize(vec):
+    def normalize(vec: np.ndarray):
         """Normalize the input vector.
-        
+
         :param vec: numpy vector needs to normalize.
-        :type vec: numpy.array 
+        :type vec: numpy.array
 
         :return: normalized vector.
         """
         magnitude = np.linalg.norm(vec)
         normalized_v = vec / magnitude
         return normalized_v
 
-    def evaluation(self, src_dict, cache_dict, **kwargs):
+    def evaluation(
+        self, src_dict: Dict[str, Any], cache_dict: Dict[str, Any], **_
+    ) -> float:
         """Evaluate the similarity score of pair.
-        
+
         :param src_dict: the query dictionary to evaluate with cache.
         :type src_dict: Dict
         :param cache_dict: the cache dictionary.
         :type cache_dict: Dict
 
         :return: evaluation score.
         """
-        src_embedding = self.normalize(src_dict['embedding']) if self.enable_normal else src_dict['embedding']
-        _, cache_embedding = cache_dict['search_result']
-        cache_embedding = self.normalize(cache_embedding) if self.enable_normal \
-            else cache_embedding
+        src_embedding = (
+            self.normalize(src_dict["embedding"])
+            if self.enable_normal
+            else src_dict["embedding"]
+        )
+        _, cache_embedding = cache_dict["search_result"]
+        cache_embedding = (
+            self.normalize(cache_embedding) if self.enable_normal else cache_embedding
+        )
         return np.linalg.norm(src_embedding - cache_embedding)
 
-    def range(self):
+    def range(self) -> Tuple[float, float]:
         """Range of similarity score.
-        
+
         :return: minimum and maximum of similarity score.
         """
         return 0.0, 2.0
```

### Comparing `gptcache-0.1.5/gptcache/similarity_evaluation/onnx.py` & `gptcache-0.1.6/gptcache/similarity_evaluation/onnx.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,102 +1,131 @@
-from gptcache.utils import import_onnxruntime, import_huggingface_hub, import_huggingface
-from .similarity_evaluation import SimilarityEvaluation
+from typing import Dict, List, Tuple, Any
+import numpy as np
+from gptcache.utils import (
+    import_onnxruntime,
+    import_huggingface_hub,
+    import_huggingface,
+)
+from gptcache.similarity_evaluation import SimilarityEvaluation
 
 import_onnxruntime()
 import_huggingface_hub()
 import_huggingface()
-import numpy as np
-from transformers import AutoTokenizer
-from huggingface_hub import hf_hub_download
-from typing import List
-import onnxruntime
 
-def pad_sequence(input_ids_list, padding_value=0):
+from transformers import AutoTokenizer  # pylint: disable=C0413
+from huggingface_hub import hf_hub_download  # pylint: disable=C0413
+import onnxruntime  # pylint: disable=C0413
+
+
+def pad_sequence(input_ids_list: List[np.ndarray], padding_value: int = 0):
     max_len = max(len(sequence) for sequence in input_ids_list)
     padded_sequences = np.full((len(input_ids_list), max_len), padding_value)
     for i, sequence in enumerate(input_ids_list):
-        padded_sequences[i, :len(sequence)] = sequence
+        padded_sequences[i, : len(sequence)] = sequence
     return padded_sequences
 
+
 class OnnxModelEvaluation(SimilarityEvaluation):
     """Using ONNX model to evaluate sentences pair similarity.
 
     :param model: model name of OnnxModelEvaluation. Default is 'GPTCache/albert-duplicate-onnx'.
-    :type model: str 
+    :type model: str
 
     Example:
         .. code-block:: python
 
             from gptcache.similarity_evaluation import OnnxModelEvaluation
-            
+
             evaluation = OnnxModelEvaluation()
             score = evaluation.evaluation(
                 {
                     'question': 'What is the color of sky?'
                 },
                 {
                     'question': 'hello'
                 }
             )
     """
-    def __init__(self, model = 'GPTCache/albert-duplicate-onnx'):
-        tokenizer_name = 'albert-base-v2'
+
+    def __init__(self, model: str = "GPTCache/albert-duplicate-onnx"):
+        tokenizer_name = "albert-base-v2"
         self.tokenizer = AutoTokenizer.from_pretrained(tokenizer_name)
         self.model = model
-        onnx_model_path = hf_hub_download(repo_id=model, filename = 'model.onnx')
+        onnx_model_path = hf_hub_download(repo_id=model, filename="model.onnx")
         self.ort_session = onnxruntime.InferenceSession(onnx_model_path)
 
     # WARNING: the model cannot evaluate text with more than 512 tokens
-    def evaluation(self, src_dict, cache_dict, **kwargs):
+    def evaluation(
+        self, src_dict: Dict[str, Any], cache_dict: Dict[str, Any], **_
+    ) -> float:
         """Evaluate the similarity score of pair.
 
         :param src_dict: the query dictionary to evaluate with cache.
         :type src_dict: Dict
         :param cache_dict: the cache dictionary.
         :type cache_dict: Dict
 
         :return: evaluation score.
         """
         try:
-            src_question = src_dict['question']
-            cache_question = cache_dict['question']
+            src_question = src_dict["question"]
+            cache_question = cache_dict["question"]
             if src_question == cache_question:
                 return 1
             return self.inference(src_question, [cache_question])
-        except Exception:
+        except Exception:  # pylint: disable=W0703
             return 0
 
-    def range(self):
+    def range(self) -> Tuple[float, float]:
         """Range of similarity score.
-        
+
         :return: minimum and maximum of similarity score.
         """
         return 0.0, 1.0
 
     def inference(self, reference: str, candidates: List[str]) -> np.ndarray:
         """Inference the ONNX model.
-        
+
         :param reference: reference sentence.
-        :type reference: str 
+        :type reference: str
         :param candidates: candidate sentences.
         :type candidates: List[str]
 
-        :return: probability score indcates how much is reference similar to candidates. 
+        :return: probability score indcates how much is reference similar to candidates.
         """
-        n_candidates= len(candidates)
-        inference_texts = [{'text_a': reference, 'text_b': candidate } for candidate in candidates]
-        batch_encoding_list = [self.tokenizer.encode_plus(text['text_a'], text['text_b'], padding='longest') for text in inference_texts]
-
-        input_ids_list = [np.array(encode.input_ids) for encode in batch_encoding_list] 
-        attention_mask_list = [np.array(encode.attention_mask) for encode in batch_encoding_list] 
-        token_type_ids_list = [np.array(encode.token_type_ids) for encode in batch_encoding_list]
- 
-        padded_input_ids = pad_sequence(input_ids_list, padding_value=self.tokenizer.pad_token_id)
-        padded_attention_mask = pad_sequence(attention_mask_list, padding_value=self.tokenizer.pad_token_id)
-        padded_token_type_ids = pad_sequence(token_type_ids_list, padding_value=self.tokenizer.pad_token_id)
- 
-        ort_inputs = {'input_ids': padded_input_ids.reshape(n_candidates,-1), 
-                      'attention_mask': padded_attention_mask.reshape(n_candidates,-1),
-                      'token_type_ids': padded_token_type_ids.reshape(n_candidates,-1)}
+        n_candidates = len(candidates)
+        inference_texts = [
+            {"text_a": reference, "text_b": candidate} for candidate in candidates
+        ]
+        batch_encoding_list = [
+            self.tokenizer.encode_plus(
+                text["text_a"], text["text_b"], padding="longest"
+            )
+            for text in inference_texts
+        ]
+
+        input_ids_list = [np.array(encode.input_ids) for encode in batch_encoding_list]
+        attention_mask_list = [
+            np.array(encode.attention_mask) for encode in batch_encoding_list
+        ]
+        token_type_ids_list = [
+            np.array(encode.token_type_ids) for encode in batch_encoding_list
+        ]
+
+        padded_input_ids = pad_sequence(
+            input_ids_list, padding_value=self.tokenizer.pad_token_id
+        )
+        padded_attention_mask = pad_sequence(
+            attention_mask_list, padding_value=self.tokenizer.pad_token_id
+        )
+        padded_token_type_ids = pad_sequence(
+            token_type_ids_list, padding_value=self.tokenizer.pad_token_id
+        )
+
+        ort_inputs = {
+            "input_ids": padded_input_ids.reshape(n_candidates, -1),
+            "attention_mask": padded_attention_mask.reshape(n_candidates, -1),
+            "token_type_ids": padded_token_type_ids.reshape(n_candidates, -1),
+        }
         ort_outputs = self.ort_session.run(None, ort_inputs)
         scores = ort_outputs[0][:, 1]
         return scores
```

### Comparing `gptcache-0.1.5/gptcache/utils/lazy_import.py` & `gptcache-0.1.6/gptcache/utils/lazy_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from types import ModuleType
 
 
 class LazyImport(ModuleType):
     """
     Lazily import a module.
     """
+
     def __init__(self, local_name, parent_module_globals, name):
         self._local_name = local_name
         self._parent_module_globals = parent_module_globals
         super().__init__(name)
 
     def _load(self):
         module = importlib.import_module(self.__name__)
```

### Comparing `gptcache-0.1.5/gptcache.egg-info/PKG-INFO` & `gptcache-0.1.6/gptcache.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: gptcache
-Version: 0.1.5
+Version: 0.1.6
 Summary: GPT Cache, a powerful caching library that can be used to speed up and lower the cost of chat applications that rely on the LLM service. GPT Cache works as a memcache for AIGC applications, similar to how Redis works for traditional applications.
 Home-page: https://github.com/zilliztech/GPTCache
 Author: SimFG
 Author-email: bang.fu@zilliz.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GPTCache : A Library for Creating Semantic Cache for LLM Queries
 Slash Your LLM API Costs by 10x 💰, Boost Speed by 100x ⚡ 
 
-[![Release](https://img.shields.io/pypi/v/gptcache?label=Release&color)](https://pypi.org/project/gptcache/)
-[![CI](https://github.com/zilliztech/gptcache/actions/workflows/CI_main.yaml/badge.svg)](https://github.com/zilliztech/gptcache/actions/workflows/CI_main.yaml)
-[![pip download](https://img.shields.io/pypi/dm/gptcache.svg?color=bright-green)](https://pypi.org/project/gptcache/)
+[![Release](https://img.shields.io/pypi/v/gptcache?label=Release&color&logo=Python)](https://pypi.org/project/gptcache/)
+[![Pylint](https://img.shields.io/github/actions/workflow/status/zilliztech/GPTCache/pylint.yaml?label=Pylint&logo=Github)](https://github.com/zilliztech/gptcache/actions/workflows/pylint.yaml)
+[![CI](https://img.shields.io/github/actions/workflow/status/zilliztech/GPTCache/unit_test_main.yaml?label=Test&logo=Github)](https://github.com/zilliztech/gptcache/actions/workflows/unit_test_main.yaml)
+[![pip download](https://img.shields.io/pypi/dm/gptcache.svg?color=bright-green&logo=Pypi)](https://pypi.org/project/gptcache/)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/license/mit/)
 [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/zilliz_universe.svg?style=social&label=Follow%20%40Zilliz)](https://twitter.com/zilliz_universe)
 [![Discord](https://dcbadge.vercel.app/api/server/Q8C6WEjSWV?compact=true&style=flat)](https://discord.gg/Q8C6WEjSWV)
 
 Documentation: https://gptcache.readthedocs.io/en/latest/.
 
 Discord: https://discord.gg/Q8C6WEjSWV.
@@ -31,45 +32,30 @@
 
 `pip install gptcache`
 
 ## 🚀 What is GPTCache?
 
 ChatGPT and various large language models (LLMs) boast incredible versatility, enabling the development of a wide range of applications. However, as your application grows in popularity and encounters higher traffic levels, the expenses related to LLM API calls can become substantial. Additionally, LLM services might exhibit slow response times, especially when dealing with a significant number of requests.
 
-To tackle this challenge, we have created GPTCache, a project dedicated to building a semantic cache for storing LLM responses. This library offers the following primary benefits:
-
-1. **Decreased expenses**: Most LLM services charge fees based on a combination of number of requests and [token count](https://openai.com/pricing). By caching query results, GPTCache reduces both the number of requests and the number of tokens sent to the LLM service. This minimizes the overall cost of using the service. 
-2. **Enhanced performance**: LLMs employ generative AI algorithms to generate responses in real-time, a process that can sometimes be time-consuming. However, when a similar query is cached, the response time significantly improves, as the result is fetched directly from the cache, eliminating the need to interact with the LLM service. In most situations, GPTCache can also provide superior query throughput compared to standard LLM services.
-3. **Improved scalability and availability**: LLM services frequently enforce [rate limits](https://platform.openai.com/docs/guides/rate-limits), which are constraints that APIs place on the number of times a user or client can access the server within a given timeframe. Hitting a rate limit means that additional requests will be blocked until a certain period has elapsed, leading to a service outage. With GPTCache, you can easily scale to accommodate an increasing volume of of queries, ensuring consistent performance as your application's user base expands.
-4. **Flexible development environment**: When developing LLM applications, an LLM APIs connection is required to prove concepts. GPTCache offers the same interface as LLM APIs and can store LLM-generated or mocked data. This helps to verify your application's features without connecting to the LLM APIs or even the network.
-
-## 🤔 How does it work?
-
-A good analogy for GptCache is to think of it as a more semantic version of Redis. In GPTCache, hits are not limited to exact matches, but rather also include prompts and context similar to previous queries. We believe that the traditional cache design still works for AIGC applications due to the following reasons:
-
-- Locality is present everywhere. Like traditional application systems, AIGC applications also face similar hot topics. For instance, ChatGPT itself may be a popular topic among programmers.
-- For purpose-built SaaS services, users tend to ask questions within a specific domain, with both temporal and spatial locality.
-- By utilizing vector similarity search, it is possible to find a similarity relationship between questions and answers at a relatively low cost.
-
-We provide [benchmarks](https://github.com/zilliztech/gpt-cache/blob/main/examples/benchmark/benchmark_sqlite_faiss_onnx.py) to illustrate the concept. In semantic caching, there are three key measurement dimensions: false positives, false negatives, and hit latency. With the plugin-style implementation, users can easily tradeoff these three measurements according to their needs.
+To tackle this challenge, we have created GPTCache, a project dedicated to building a semantic cache for storing LLM responses. 
 
 ## 😊 Quick Start
 
 **Note**:
 
 - You can quickly try GPTCache and put it into a production environment without heavy development. However, please note that the repository is still under heavy development.
 - By default, only a limited number of libraries are installed to support the basic cache functionalities. When you need to use additional features, the related libraries will be **automatically installed**.
 - Make sure that the Python version is **3.8.1 or higher**, check: `python --version`
 - If you encounter issues installing a library due to a low pip version, run: `python -m pip install --upgrade pip`.
 
 ### dev install
 
 ```bash
 # clone GPTCache repo
-git clone https://github.com/zilliztech/GPTCache.git
+git clone -b dev https://github.com/zilliztech/GPTCache.git
 cd GPTCache
 
 # install the repo
 pip install -r requirements.txt
 python setup.py install
 ```
 
@@ -169,21 +155,21 @@
 
 def response_text(openai_resp):
     return openai_resp['choices'][0]['message']['content']
 
 from gptcache import cache
 from gptcache.adapter import openai
 from gptcache.embedding import Onnx
-from gptcache.manager.factory import get_data_manager
+from gptcache.manager import CacheBase, VectorBase, get_data_manager
 from gptcache.similarity_evaluation.distance import SearchDistanceEvaluation
 
 print("Cache loading.....")
 
 onnx = Onnx()
-data_manager = get_data_manager("sqlite", "faiss", dimension=onnx.dimension)
+data_manager = get_data_manager(CacheBase("sqlite"), VectorBase("faiss", dimension=onnx.dimension))
 cache.init(
     embedding_func=onnx.to_embeddings,
     data_manager=data_manager,
     similarity_evaluation=SearchDistanceEvaluation(),
     )
 cache.set_openai_key()
 
@@ -224,14 +210,40 @@
 
 More Docs：
 
 - [Usage, how to use GPTCache better](docs/usage.md)
 - [Features, all features currently supported by the cache](docs/feature.md)
 - [Examples, learn better custom caching](examples/README.md)
 
+## 😎 What can this help with?
+GPTCache offers the following primary benefits:
+
+- **Decreased expenses**: Most LLM services charge fees based on a combination of number of requests and [token count](https://openai.com/pricing). By caching query results, GPTCache reduces both the number of requests and the number of tokens sent to the LLM service. This minimizes the overall cost of using the service. 
+- **Enhanced performance**: LLMs employ generative AI algorithms to generate responses in real-time, a process that can sometimes be time-consuming. However, when a similar query is cached, the response time significantly improves, as the result is fetched directly from the cache, eliminating the need to interact with the LLM service. In most situations, GPTCache can also provide superior query throughput compared to standard LLM services.
+- **Improved scalability and availability**: LLM services frequently enforce [rate limits](https://platform.openai.com/docs/guides/rate-limits), which are constraints that APIs place on the number of times a user or client can access the server within a given timeframe. Hitting a rate limit means that additional requests will be blocked until a certain period has elapsed, leading to a service outage. With GPTCache, you can easily scale to accommodate an increasing volume of of queries, ensuring consistent performance as your application's user base expands.
+- **Flexible development environment**: When developing LLM applications, an LLM APIs connection is required to prove concepts. GPTCache offers the same interface as LLM APIs and can store LLM-generated or mocked data. This helps to verify your application's features without connecting to the LLM APIs or even the network.
+
+## 🤔 How does it work?
+
+Online services often exhibit data locality, with users frequently accessing popular or trending content. Cache systems take advantage of this behavior by storing commonly accessed data, which in turn reduces data retrieval time, improves response times, and eases the burden on backend servers. Traditional cache systems typically utilize an exact match between a new query and a cached query to determine if the requested content is available in the cache before fetching the data.
+
+However, using an exact match approach for LLM caches is less effective due to the complexity and variability of LLM queries, resulting in a low cache hit rate. To address this issue, GPTCache adopt alternative strategies like semantic caching. Semantic caching identifies and stores similar or related queries, thereby increasing cache hit probability and enhancing overall caching efficiency. 
+
+GPTCache employs embedding algorithms to convert queries into embeddings and uses a vector store for similarity search on these embeddings. This process allows GPTCache to identify and retrieve similar or related queries from the cache storage, as illustrated in the [Modules section](https://github.com/zilliztech/GPTCache#-modules). 
+
+Featuring a modular design, GPTCache makes it easy for users to customize their own semantic cache. The system offers various implementations for each module, and users can even develop their own implementations to suit their specific needs.
+
+In a semantic cache, false positives can occur during cache hits and false negatives during cache misses. GPTCache provides three metrics to evaluate its performance:
+
+- Precision: the ratio of true positives to the total of true positives and false positives.
+- Recall: the ratio of true positives to the total of true positives and false negatives.
+- Latency: the time required for a query to be processed and the corresponding data to be fetched from the cache.
+
+A [sample benchmark](https://github.com/zilliztech/gpt-cache/blob/main/examples/benchmark/benchmark_sqlite_faiss_onnx.py) is included for users to start with assessing the performance of their semantic cache.
+
 ## 🤗 Modules
 
 ![GPTCache Struct](docs/GPTCacheStructure.png)
 
 - **LLM Adapter**: 
 The LLM Adapter is designed to integrate different LLM models by unifying their APIs and request protocols. GPTCache offers a standardized interface for this purpose, with current support for ChatGPT integration.
   - [x] Support OpenAI ChatGPT API.
@@ -242,51 +254,51 @@
   - [x] Disable embedding. This will turn GPTCache into a keyword-matching cache.
   - [x] Support OpenAI embedding API.
   - [x] Support [ONNX](https://onnx.ai/) with the GPTCache/paraphrase-albert-onnx model.
   - [x] Support [Hugging Face](https://huggingface.co/) embedding API.
   - [x] Support [Cohere](https://docs.cohere.ai/reference/embed) embedding API.
   - [x] Support [fastText](https://fasttext.cc) embedding API.
   - [x] Support [SentenceTransformers](https://www.sbert.net) embedding API.
-  - [ ] Support other embedding apis
+  - [ ] Support other embedding APIs.
 - **Cache Storage**:
 **Cache Storage** is where the response from LLMs, such as ChatGPT, is stored. Cached responses are retrieved to assist in evaluating similarity and are returned to the requester if there is a good semantic match. At present, GPTCache supports SQLite and offers a universally accessible interface for extension of this module.
   - [x] Support [SQLite](https://sqlite.org/docs.html).
   - [x] Support [PostgreSQL](https://www.postgresql.org/).
   - [x] Support [MySQL](https://www.mysql.com/).
   - [x] Support [MariaDB](https://mariadb.org/).
   - [x] Support [SQL Server](https://www.microsoft.com/en-us/sql-server/).
   - [x] Support [Oracle](https://www.oracle.com/).
   - [ ] Support [MongoDB](https://www.mongodb.com/).
   - [ ] Support [Redis](https://redis.io/).
   - [ ] Support [Minio](https://min.io/).
   - [ ] Support [HBase](https://hbase.apache.org/).
-  - [ ] Support [ElasticSearch](https://www.elastic.co/)
-  - [ ] Support [zincsearch](https://zinc.dev/)
-  - [ ] Support other storages
+  - [ ] Support [ElasticSearch](https://www.elastic.co/).
+  - [ ] Support [Duckdb](https://github.com/duckdb/duckdb).
+  - [ ] Support other storages.
 - **Vector Store**:
 The **Vector Store** module helps find the K most similar requests from the input request's extracted embedding. The results can help assess similarity. GPTCache provides a user-friendly interface that supports various vector stores, including Milvus, Zilliz Cloud, and FAISS. More options will be available in the future.
-  - [x] Support [Milvus](https://milvus.io/).
-  - [x] Support [Zilliz Cloud](https://cloud.zilliz.com/).
-  - [x] Support [FAISS](https://faiss.ai/).
-  - [ ] Support other vector databases
+  - [x] Support [Milvus](https://milvus.io/), an open-source vector database for production-ready AI/LLM applicaionts. 
+  - [x] Support [Zilliz Cloud](https://cloud.zilliz.com/), a fully-managed cloud vector database based on Milvus.
+  - [x] Support [FAISS](https://faiss.ai/), a library for efficient similarity search and clustering of dense vectors.
+  - [ ] Support other vector databases.
 - **Cache Manager**:
 The **Cache Manager** is responsible for controlling the operation of both the **Cache Storage** and **Vector Store**.
   - **Eviction Policy**:
   Currently, GPTCache makes decisions about evictions based solely on the number of lines. This approach can result in inaccurate resource evaluation and may cause out-of-memory (OOM) errors. We are actively investigating and developing a more sophisticated strategy.
-    - [x] LRU eviction policy
-    - [x] FIFO eviction policy
-    - [ ] More complicated eviction policies
+    - [x] Support LRU eviction policy.
+    - [x] Support FIFO eviction policy.
+    - [ ] Support more complicated eviction policies.
 - **Similarity Evaluator**: 
 This module collects data from both the **Cache Storage** and **Vector Store**, and uses various strategies to determine the similarity between the input request and the requests from the **Vector Store**. Based on this similarity, it determines whether a request matches the cache. GPTCache provides a standardized interface for integrating various strategies, along with a collection of implementations to use. The following similarity definitions are currently supported or will be supported in the future:
   - [x] The distance we obtain from the **Vector Store**.
   - [x] A model-based similarity determined using the GPTCache/albert-duplicate-onnx model from [ONNX](https://onnx.ai/).
   - [x] Exact matches between the input request and the requests obtained from the **Vector Store**.
   - [x] Distance represented by applying linalg.norm from numpy to the embeddings.
-  - [ ] BM25 and other similarity measurements
-  - [ ] Support other model serving framework such as PyTorch
+  - [ ] BM25 and other similarity measurements.
+  - [ ] Support other model serving framework such as PyTorch.
  
   
   **Note**:Not all combinations of different modules may be compatible with each other. For instance, if we disable the **Embedding Extractor**, the **Vector Store** may not function as intended. We are currently working on implementing a combination sanity check for **GPTCache**.
 
 ## 😇 Roadmap
 Coming soon! [Stay tuned!](https://twitter.com/zilliz_universe)
```

### Comparing `gptcache-0.1.5/gptcache.egg-info/SOURCES.txt` & `gptcache-0.1.6/gptcache.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,19 +22,21 @@
 gptcache/embedding/string.py
 gptcache/manager/__init__.py
 gptcache/manager/data_manager.py
 gptcache/manager/eviction.py
 gptcache/manager/factory.py
 gptcache/manager/scalar_data/__init__.py
 gptcache/manager/scalar_data/base.py
+gptcache/manager/scalar_data/manager.py
 gptcache/manager/scalar_data/sqlalchemy.py
 gptcache/manager/vector_data/__init__.py
 gptcache/manager/vector_data/base.py
 gptcache/manager/vector_data/chroma.py
 gptcache/manager/vector_data/faiss.py
+gptcache/manager/vector_data/manager.py
 gptcache/manager/vector_data/milvus.py
 gptcache/processor/__init__.py
 gptcache/processor/post.py
 gptcache/processor/pre.py
 gptcache/similarity_evaluation/__init__.py
 gptcache/similarity_evaluation/distance.py
 gptcache/similarity_evaluation/exact_match.py
```

### Comparing `gptcache-0.1.5/setup.py` & `gptcache-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             if require.strip() and not require.startswith('#')
         ]
 
 
 setuptools.setup(
     name="gptcache",
     packages=find_packages(),
-    version="0.1.5",
+    version="0.1.6",
     author="SimFG",
     author_email="bang.fu@zilliz.com",
     description="GPT Cache, a powerful caching library that can be used to speed up and lower the cost of chat "
                 "applications that rely on the LLM service. GPT Cache works as a memcache for AIGC applications, "
                 "similar to how Redis works for traditional applications.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

