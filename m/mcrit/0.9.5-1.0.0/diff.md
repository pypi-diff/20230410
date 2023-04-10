# Comparing `tmp/mcrit-0.9.5.tar.gz` & `tmp/mcrit-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcrit-0.9.5.tar", last modified: Tue Jul 12 05:42:46 2022, max compression
+gzip compressed data, was "mcrit-1.0.0.tar", last modified: Mon Apr 10 16:38:50 2023, max compression
```

## Comparing `mcrit-0.9.5.tar` & `mcrit-1.0.0.tar`

### file list

```diff
@@ -1,64 +1,84 @@
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-07-12 05:42:46.442952 mcrit-0.9.5/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    35149 2022-05-13 09:44:28.000000 mcrit-0.9.5/LICENSE
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     7378 2022-07-12 05:42:46.442952 mcrit-0.9.5/PKG-INFO
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     5657 2022-07-12 05:41:59.000000 mcrit-0.9.5/README.md
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-07-12 05:42:46.438953 mcrit-0.9.5/mcrit/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    13071 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/Worker.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/__init__.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3260 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/__main__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-07-12 05:42:46.438953 mcrit-0.9.5/mcrit/client/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    14399 2022-07-12 05:42:37.000000 mcrit-0.9.5/mcrit/client/McritClient.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/client/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-07-12 05:42:46.442952 mcrit-0.9.5/mcrit/config/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      855 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/config/ConfigInterface.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      961 2022-07-12 05:42:13.000000 mcrit-0.9.5/mcrit/config/McritConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1870 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/config/MinHashConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      821 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/config/QueueConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1974 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/config/ShinglerConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1774 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/config/StorageConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/config/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-07-12 05:42:46.442952 mcrit-0.9.5/mcrit/index/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    18658 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/index/MinHashIndex.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/index/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-07-12 05:42:46.442952 mcrit-0.9.5/mcrit/libs/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/libs/__init__.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    14859 2022-07-12 05:42:37.000000 mcrit-0.9.5/mcrit/libs/mongoqueue.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    14152 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/libs/pymmh3.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2028 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/libs/utility.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-07-12 05:42:46.442952 mcrit-0.9.5/mcrit/minhash/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3662 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/minhash/MinHash.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     9505 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/minhash/MinHasher.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3212 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/minhash/ShingleLoader.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/minhash/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-07-12 05:42:46.442952 mcrit-0.9.5/mcrit/server/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2251 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/server/FamilyResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1771 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/server/FunctionResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3320 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/server/JobResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2170 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/server/MatchResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2456 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/server/QueryResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6422 2022-06-02 15:12:49.000000 mcrit-0.9.5/mcrit/server/SampleResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3110 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/server/StatusResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/server/__init__.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     4172 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/server/application_routes.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1369 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/server/utils.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)       69 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/server/wsgi.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-07-12 05:42:46.442952 mcrit-0.9.5/mcrit/storage/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     5622 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/storage/FunctionEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3481 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/storage/MatchedFunctionEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6494 2022-05-13 10:41:04.000000 mcrit-0.9.5/mcrit/storage/MatchedSampleEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      567 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/storage/MatchingCache.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    10300 2022-07-12 05:37:25.000000 mcrit-0.9.5/mcrit/storage/MatchingResult.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    19282 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/storage/MemoryStorage.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    29880 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/storage/MongoDbStorage.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     4933 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/storage/SampleEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      728 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/storage/StorageFactory.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    19948 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/storage/StorageInterface.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-0.9.5/mcrit/storage/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2022-07-12 05:42:46.438953 mcrit-0.9.5/mcrit.egg-info/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     7378 2022-07-12 05:42:46.000000 mcrit-0.9.5/mcrit.egg-info/PKG-INFO
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1400 2022-07-12 05:42:46.000000 mcrit-0.9.5/mcrit.egg-info/SOURCES.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        1 2022-07-12 05:42:46.000000 mcrit-0.9.5/mcrit.egg-info/dependency_links.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      104 2022-07-12 05:42:46.000000 mcrit-0.9.5/mcrit.egg-info/requires.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        6 2022-07-12 05:42:46.000000 mcrit-0.9.5/mcrit.egg-info/top_level.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)       38 2022-07-12 05:42:46.442952 mcrit-0.9.5/setup.cfg
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1302 2022-07-12 05:41:06.000000 mcrit-0.9.5/setup.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-04-10 16:38:50.104970 mcrit-1.0.0/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    35149 2022-05-13 09:44:28.000000 mcrit-1.0.0/LICENSE
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    12656 2023-04-10 16:38:50.104970 mcrit-1.0.0/PKG-INFO
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    10327 2023-04-10 16:33:01.000000 mcrit-1.0.0/README.md
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-04-10 16:38:50.100970 mcrit-1.0.0/mcrit/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    21415 2022-12-14 11:14:13.000000 mcrit-1.0.0/mcrit/Worker.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/__init__.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1838 2023-03-21 09:06:40.000000 mcrit-1.0.0/mcrit/__main__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-04-10 16:38:50.100970 mcrit-1.0.0/mcrit/client/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    28146 2023-03-24 15:01:21.000000 mcrit-1.0.0/mcrit/client/McritClient.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    17638 2023-04-10 16:19:48.000000 mcrit-1.0.0/mcrit/client/McritConsole.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/client/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-04-10 16:38:50.100970 mcrit-1.0.0/mcrit/config/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      855 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/config/ConfigInterface.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      960 2023-04-10 15:55:00.000000 mcrit-1.0.0/mcrit/config/McritConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2148 2023-04-10 15:53:10.000000 mcrit-1.0.0/mcrit/config/MinHashConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      821 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/config/QueueConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1974 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/config/ShinglerConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1775 2022-07-29 10:29:16.000000 mcrit-1.0.0/mcrit/config/StorageConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/config/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-04-10 16:38:50.100970 mcrit-1.0.0/mcrit/index/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    29049 2023-04-10 15:53:10.000000 mcrit-1.0.0/mcrit/index/MinHashIndex.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3890 2022-08-08 11:41:38.000000 mcrit-1.0.0/mcrit/index/SearchCursor.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6210 2022-08-08 11:41:38.000000 mcrit-1.0.0/mcrit/index/SearchQueryParser.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6366 2022-08-08 11:41:38.000000 mcrit-1.0.0/mcrit/index/SearchQueryTree.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/index/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-04-10 16:38:50.100970 mcrit-1.0.0/mcrit/libs/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/libs/__init__.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    16784 2022-08-23 11:53:24.000000 mcrit-1.0.0/mcrit/libs/mongoqueue.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    14152 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/libs/pymmh3.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2028 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/libs/utility.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-04-10 16:38:50.100970 mcrit-1.0.0/mcrit/matchers/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6378 2022-08-31 07:13:17.000000 mcrit-1.0.0/mcrit/matchers/MatcherCross.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    28260 2023-04-10 15:53:10.000000 mcrit-1.0.0/mcrit/matchers/MatcherInterface.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3014 2022-11-25 14:50:57.000000 mcrit-1.0.0/mcrit/matchers/MatcherQuery.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3097 2023-04-10 15:53:10.000000 mcrit-1.0.0/mcrit/matchers/MatcherQueryFunction.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      751 2022-09-28 13:53:00.000000 mcrit-1.0.0/mcrit/matchers/MatcherSample.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2429 2022-12-14 11:14:13.000000 mcrit-1.0.0/mcrit/matchers/MatcherVs.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-08-29 06:59:30.000000 mcrit-1.0.0/mcrit/matchers/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-04-10 16:38:50.100970 mcrit-1.0.0/mcrit/minhash/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3662 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/minhash/MinHash.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    10547 2022-11-11 10:02:06.000000 mcrit-1.0.0/mcrit/minhash/MinHasher.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3212 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/minhash/ShingleLoader.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/minhash/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-04-10 16:38:50.104970 mcrit-1.0.0/mcrit/queue/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    10980 2022-08-31 07:13:17.000000 mcrit-1.0.0/mcrit/queue/LocalQueue.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1308 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/queue/QueueFactory.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    14987 2022-10-12 12:19:42.000000 mcrit-1.0.0/mcrit/queue/QueueRemoteCalls.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-08-29 06:36:44.000000 mcrit-1.0.0/mcrit/queue/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-04-10 16:38:50.104970 mcrit-1.0.0/mcrit/server/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1297 2023-03-21 14:19:34.000000 mcrit-1.0.0/mcrit/server/BlocksResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6004 2023-03-21 14:19:34.000000 mcrit-1.0.0/mcrit/server/FamilyResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3486 2023-03-21 14:19:34.000000 mcrit-1.0.0/mcrit/server/FunctionResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     4609 2023-03-21 14:19:34.000000 mcrit-1.0.0/mcrit/server/JobResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3551 2023-03-21 14:19:34.000000 mcrit-1.0.0/mcrit/server/MatchResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     7608 2023-03-22 15:50:20.000000 mcrit-1.0.0/mcrit/server/QueryResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    11793 2023-03-21 14:19:34.000000 mcrit-1.0.0/mcrit/server/SampleResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     5159 2023-03-21 14:19:34.000000 mcrit-1.0.0/mcrit/server/StatusResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/server/__init__.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     5887 2023-03-17 17:07:42.000000 mcrit-1.0.0/mcrit/server/application_routes.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1868 2023-03-21 14:19:34.000000 mcrit-1.0.0/mcrit/server/utils.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)       69 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/server/wsgi.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-04-10 16:38:50.104970 mcrit-1.0.0/mcrit/storage/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2077 2022-08-03 10:24:19.000000 mcrit-1.0.0/mcrit/storage/FamilyEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6415 2023-03-21 14:19:34.000000 mcrit-1.0.0/mcrit/storage/FunctionEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1661 2023-03-21 14:19:34.000000 mcrit-1.0.0/mcrit/storage/FunctionLabelEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2764 2023-02-27 12:31:29.000000 mcrit-1.0.0/mcrit/storage/MatchedFunctionEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6617 2023-02-14 15:17:18.000000 mcrit-1.0.0/mcrit/storage/MatchedSampleEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1389 2023-04-10 15:53:10.000000 mcrit-1.0.0/mcrit/storage/MatchingCache.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    21812 2023-03-14 13:04:24.000000 mcrit-1.0.0/mcrit/storage/MatchingResult.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    44811 2023-03-24 15:01:21.000000 mcrit-1.0.0/mcrit/storage/MemoryStorage.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    59588 2023-03-24 15:01:21.000000 mcrit-1.0.0/mcrit/storage/MongoDbStorage.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     4932 2023-03-17 17:07:42.000000 mcrit-1.0.0/mcrit/storage/SampleEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      735 2022-11-13 10:29:45.000000 mcrit-1.0.0/mcrit/storage/StorageFactory.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    25158 2023-03-21 14:19:34.000000 mcrit-1.0.0/mcrit/storage/StorageInterface.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/storage/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-04-10 16:38:50.100970 mcrit-1.0.0/mcrit.egg-info/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    12656 2023-04-10 16:38:49.000000 mcrit-1.0.0/mcrit.egg-info/PKG-INFO
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1950 2023-04-10 16:38:49.000000 mcrit-1.0.0/mcrit.egg-info/SOURCES.txt
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        1 2023-04-10 16:38:49.000000 mcrit-1.0.0/mcrit.egg-info/dependency_links.txt
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      135 2023-04-10 16:38:49.000000 mcrit-1.0.0/mcrit.egg-info/requires.txt
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        6 2023-04-10 16:38:49.000000 mcrit-1.0.0/mcrit.egg-info/top_level.txt
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)       38 2023-04-10 16:38:50.104970 mcrit-1.0.0/setup.cfg
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1355 2023-04-10 16:10:06.000000 mcrit-1.0.0/setup.py
```

### Comparing `mcrit-0.9.5/LICENSE` & `mcrit-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mcrit-0.9.5/mcrit/config/ConfigInterface.py` & `mcrit-1.0.0/mcrit/config/ConfigInterface.py`

 * *Files identical despite different names*

### Comparing `mcrit-0.9.5/mcrit/config/McritConfig.py` & `mcrit-1.0.0/mcrit/config/McritConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .ShinglerConfig import ShinglerConfig
 from .StorageConfig import StorageConfig
 
 
 class McritConfig(object):
 
     # NOTE to self: always change this in setup.py as well!
-    VERSION = "0.10.0"
+    VERSION = "1.0.0"
     CONFIG_FILE_PATH = str(os.path.abspath(__file__))
     PROJECT_ROOT = str(os.path.abspath(os.sep.join([CONFIG_FILE_PATH, "..", ".."])))
 
     ### global logging-config setup
     # Only do basicConfig if no handlers have been configured
     LOG_PATH = "./"
     LOG_LEVEL = logging.INFO
```

### Comparing `mcrit-0.9.5/mcrit/config/MinHashConfig.py` & `mcrit-1.0.0/mcrit/config/MinHashConfig.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,16 +23,20 @@
     # The lower bound at which paired MinHashes are considered a match (range: 0-100)
     MINHASH_MATCHING_THRESHOLD: int = 50
     # random seed to be used when initiating XOR values for minhash seeds
     MINHASH_SEED: int = 0xDEADBEEF
     # When using as server, Gunicorn/Falcon may have issues with multiprocessing while indexing, which can be disabled this way.
     MINHASH_POOL_INDEXING: bool = True
     MINHASH_POOL_MATCHING: bool = True
+    # The minimum number of band matches a minhash must have before being considered a candidate for matching
+    BAND_MATCHES_REQUIRED = 2
     # minimum function size for considering PicHash matching
     PICHASH_SIZE: int = 10
+    # do not perform minhash matching for pichash matches, instead assume they are implied
+    PICHASH_IMPLIES_MINHASH_MATCH: bool = True
 
     def getConfigHash(self):
         config_str = ""
         config_str += f"_{self.MINHASH_STRATEGY}_{self.MINHASH_FN_MIN_INS}_{self.MINHASH_FN_MIN_BLOCKS}"
         config_str += f"_{self.MINHASH_SIGNATURE_LENGTH}_{self.MINHASH_SIGNATURE_BITS}_{self.MINHASH_SEED}"
         config_str += f"_{self.PICHASH_SIZE}"
         return hashlib.sha256(config_str.encode('utf-8')).hexdigest()
```

### Comparing `mcrit-0.9.5/mcrit/config/QueueConfig.py` & `mcrit-1.0.0/mcrit/config/QueueConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-0.9.5/mcrit/config/ShinglerConfig.py` & `mcrit-1.0.0/mcrit/config/ShinglerConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-0.9.5/mcrit/config/StorageConfig.py` & `mcrit-1.0.0/mcrit/config/StorageConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     # Use this as endpoint for our server
     STORAGE_SERVER: str = "127.0.0.1"
     # By default, MongoDbStorage's DB's name and MongoQueue's DB's name are both "mcrit"
     # Changing one DB name here or at runtime DOES NOT change the other name!
     STORAGE_MONGODB_DBNAME: str = "mcrit"
     STORAGE_PORT: ... = None
     # Once MinHashes have been calculated, discard disassembly from function entries
-    STORAGE_DROP_DISASSEMBLY: bool = True
+    STORAGE_DROP_DISASSEMBLY: bool = False
     # random seed to be used when deriving sequences used as bands
     STORAGE_BAND_SEED: int = 0xDEADBEEF
     # Banding supports:
     #  * MemoryStorage: arbitrary banding configuration, multiple lengths
     #  * MongoDbStorage: arbitrary banding configuration, multiple lengths
     # configuration for bands, dict with size:number as structure - we allow mixed sizes to increase scatter effect and randomness
     _default_storage_bands = {4: 20}
```

### Comparing `mcrit-0.9.5/mcrit/libs/mongoqueue.py` & `mcrit-1.0.0/mcrit/libs/mongoqueue.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,30 +12,33 @@
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 
 import json
 import traceback
 from datetime import datetime, timedelta
+from typing import List
 
 import gridfs
 import pymongo
 from pymongo import ReturnDocument
 from bson.objectid import ObjectId
 
 DEFAULT_INSERT = {
     "locked_by": None,
     "locked_at": None,
     "last_error": None,
     "finished_at": None,
     "created_at": None,
     "started_at": None,
     "terminated": False,
+    "required_by": [],
     "number": None,
     "result": None,
+    "notify_done": False,
 }
 
 # added to track incremental job numbers via MCRIT storage (apart from OIDs)
 def _useCounter(database, name: str) -> int:
     result = database.counters.find_one_and_update(
         filter={"name": name}, 
         update={"$inc": {"value": 1}}, 
@@ -94,35 +97,68 @@
             update={"$set": {"locked_by": None, "locked_at": None}, "$inc": {"attempts_left": -1}},
         )
 
     def drop_max_attempts(self):
         """ """
         self.collection.find_one_and_update({"attempts_left": {"$lte": 0}}, remove=True)
 
-    def put(self, payload, priority=0):
+    def put(self, payload, priority=0, await_jobs:List[str]=[]):
         """Place a job into the queue"""
         job = dict(self._default_insert)
         job["number"] = _useCounter(self.collection.database, "job")
         job["created_at"] = datetime.now()
         job["priority"] = priority
         job["payload"] = payload
+        await_jobs_set = set(await_jobs)
+        job["unfinished_dependencies"] = list(await_jobs_set)
+        job["all_dependencies"] = list(await_jobs_set)
         insert_result = self.collection.insert_one(job)
         if insert_result.acknowledged:
-            return insert_result.inserted_id
+            job_id = insert_result.inserted_id
+            for child_job_id in await_jobs_set:
+                self._notify_on_done(child_job_id, job_id)
+            return job_id
         return None
 
+    def _notify_on_done(self, notifying_job_id:str, notified_job_id:str):
+        self.collection.find_one_and_update(
+            filter={"_id": ObjectId(notifying_job_id)},
+            update={"$push": {'required_by': notified_job_id}}
+        )
+        notifying_job = self.collection.find_one({"_id": ObjectId(notifying_job_id)})
+        if notifying_job["notify_done"]:
+            self.collection.find_one_and_update(
+                filter={"_id": ObjectId(notified_job_id)},
+                update={"$pull": {'unfinished_dependencies': notifying_job_id}},
+            )
+        #     # atomically
+        #     # should handle already deleted deps gracefully
+        #     remove job.id from job_to_notify.unfinished_deps
+    
+    def _notify_dependent_jobs(self, job_id:str):
+        job = self.collection.find_one_and_update(
+            filter={"_id": ObjectId(job_id)},
+            update={"$set": {'notify_done': True}},
+        )
+        for job_id_to_notify in job["required_by"]:
+            self.collection.find_one_and_update(
+                filter={"_id": ObjectId(job_id_to_notify)},
+                update={"$pull": {'unfinished_dependencies': job_id}},
+            )
+
     def next(self):
         current_time = datetime.now()
         return self._wrap_one(
             self.collection.find_one_and_update(
                 filter={
                     "locked_by": None,
                     "locked_at": None,
                     "attempts_left": {"$gt": 0},
                     "finished_at": None,
+                    "unfinished_dependencies": [],
                 },
                 update={"$set": {"locked_by": self.consumer_id, "locked_at": current_time, "started_at": current_time}},
                 sort=[("priority", pymongo.DESCENDING), ("created_at", pymongo.ASCENDING)],
                 new=1,
                 # limit=1
             )
         )
@@ -369,40 +405,47 @@
             method_str += "(" + ", ".join([str(v) for v in combined_values]) + ")"
         return method_str
 
     @property
     def progress(self):
         return self._data["progress"]
 
+
+    # This is a GridFS id, not the actual result
     @property
     def result(self):
         return self._data["result"]
 
     @result.setter
     def result(self, res):
         self._data["result"] = res
 
     ## job control
 
     def complete(self, result=None):
         """job has been completed."""
         if result:
             self._data["result"] = result
-        return self._queue.collection.find_one_and_update(
+        job = self._queue.collection.find_one_and_update(
             filter={"_id": self.job_id, "locked_by": self._queue.consumer_id},
             update={"$set": {"finished_at": datetime.now(), "result": self._data["result"], "progress": 1}},
             return_document=ReturnDocument.AFTER
         )
+        self._queue._notify_dependent_jobs(str(job["_id"]))
+        return job 
 
     def error(self, message=None):
         """note an error processing a job, and return it to the queue."""
-        self._queue.collection.find_one_and_update(
+        job = self._queue.collection.find_one_and_update(
             filter={"_id": self.job_id, "locked_by": self._queue.consumer_id},
             update={"$set": {"locked_by": None, "locked_at": None, "last_error": message}, "$inc": {"attempts_left": -1}},
+            return_document=ReturnDocument.AFTER
         )
+        if job["attempts_left"] <= 0:
+            self._queue._notify_dependent_jobs(self, str(job["_id"]))
 
     def progressor(self, count=0):
         """note progress on a long running task."""
         return self._queue.collection.find_one_and_update(
             filter={"_id": self.job_id, "locked_by": self._queue.consumer_id},
             update={"$set": {"progress": count, "locked_at": datetime.now()}},
             return_document=ReturnDocument.AFTER
```

### Comparing `mcrit-0.9.5/mcrit/libs/pymmh3.py` & `mcrit-1.0.0/mcrit/libs/pymmh3.py`

 * *Files identical despite different names*

### Comparing `mcrit-0.9.5/mcrit/libs/utility.py` & `mcrit-1.0.0/mcrit/libs/utility.py`

 * *Files identical despite different names*

### Comparing `mcrit-0.9.5/mcrit/minhash/MinHash.py` & `mcrit-1.0.0/mcrit/minhash/MinHash.py`

 * *Files identical despite different names*

### Comparing `mcrit-0.9.5/mcrit/minhash/MinHasher.py` & `mcrit-1.0.0/mcrit/minhash/MinHasher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 
 import logging
 import random
-from collections import Counter
-from typing import List, Tuple
+from collections import Counter, defaultdict
+from typing import List, Tuple, Dict
 
 from mcrit.libs.utility import generate_segmented_sequence
 from mcrit.minhash.MinHash import MinHash
 from mcrit.minhash.ShingleLoader import ShingleLoader
 
 logging.basicConfig(level=logging.INFO)
 LOGGER = logging.getLogger(__name__)
@@ -81,14 +81,34 @@
         for function_tuple in function_tuples:
             function_id, smda_function = function_tuple
             minhash = self._calculateMinHash(smda_function)
             minhash.function_id = function_id
             minhashes.append(minhash)
         return minhashes
 
+    def calculateAggregatedScoresFromPackedTuples(
+        self,
+        packed_tuples: List[Tuple[int, int, bytes, int, int, bytes]],
+        ignore_threshold=False,
+        minhash_threshold=None,
+    ) -> Dict[Tuple[int, int, int], Tuple[int, float]]:
+        results: Dict[Tuple[int, int, int], Tuple[int, float]] = {}
+        if minhash_threshold is None:
+            minhash_threshold = self._minhash_config.MINHASH_MATCHING_THRESHOLD
+        for minhash_tuple in packed_tuples:
+            sample_id_a, function_id_a, minhash_a, sample_id_b, function_id_b, minhash_b = minhash_tuple
+            score = MinHash.calculateMinHashScore(
+                minhash_a, minhash_b, minhash_bits=self._minhash_config.MINHASH_SIGNATURE_BITS
+            )
+            if ignore_threshold or score > minhash_threshold:
+                key = (sample_id_a, function_id_a, sample_id_b)
+                if key not in results or score > results[key][1]:
+                    results[key] = (function_id_b, score)
+        return results
+
     def calculateScoresFromPackedTuples(
         self,
         packed_tuples: List[Tuple[int, int, bytes, int, int, bytes]],
         ignore_threshold=False,
         minhash_threshold=None,
     ) -> List[Tuple[int, int, int, int, float]]:
         results = []
@@ -184,8 +204,8 @@
             xored_outputs = [shingle ^ hash_seed for shingle in shingler_outputs[shingler_name]]
             minhash_value = min(xored_outputs)
             if self._minhash_config.MINHASH_SIGNATURE_BITS < 32:
                 minhash_value = minhash_value % (2 ** self._minhash_config.MINHASH_SIGNATURE_BITS)
             minhash_signature.append(minhash_value)
         minhash_result.setMinHash(minhash_signature)
         minhash_result.shingler_composition = dict(shingler_composition)
-        return minhash_result
+        return minhash_result
```

### Comparing `mcrit-0.9.5/mcrit/minhash/ShingleLoader.py` & `mcrit-1.0.0/mcrit/minhash/ShingleLoader.py`

 * *Files identical despite different names*

### Comparing `mcrit-0.9.5/mcrit/server/application_routes.py` & `mcrit-1.0.0/mcrit/server/application_routes.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import falcon
 
 from mcrit.index.MinHashIndex import MinHashIndex
 from mcrit.server.FamilyResource import FamilyResource
 from .FunctionResource import FunctionResource
 from .JobResource import JobResource
 from .MatchResource import MatchResource
+from .BlocksResource import BlocksResource
 from .QueryResource import QueryResource
 from .SampleResource import SampleResource
 from .StatusResource import StatusResource
 
 # Only do basicConfig if no handlers have been configured
 if len(logging._handlerList) == 0:
     logging.basicConfig(level=logging.INFO, format="%(asctime)-15s %(message)s")
@@ -38,62 +39,82 @@
 def get_app():
     index = create_index()
     status_resource = StatusResource(index)
     family_resource = FamilyResource(index)
     sample_resource = SampleResource(index)
     function_resource = FunctionResource(index)
     match_resource = MatchResource(index)
+    block_resource = BlocksResource(index)
     query_resource = QueryResource(index)
     job_resource = JobResource(index)
 
     _app = falcon.App()
     _app.req_options.strip_url_path_trailing_slash = True
     _app.add_route("/", status_resource)
     _app.add_route("/status", status_resource, suffix="status")
+    _app.add_route("/version", status_resource, suffix="version")
     _app.add_route("/config", status_resource, suffix="config")
     _app.add_route("/export", status_resource, suffix="export")
     _app.add_route("/export/{comma_separated_sample_ids}", status_resource, suffix="export_selection")
     # NOTE: adds to storage, does not replace storage
     _app.add_route("/import", status_resource, suffix="import")  # post
     # drops storage and sets up new empty instance
     _app.add_route("/respawn", status_resource, suffix="respawn")  # post
+    # schedule a job that calculates all missing minhashes for all samples/functions, in case the respective jobs failed before
+    _app.add_route("/complete_minhashes", status_resource, suffix="complete_minhashes")  # get
+
     # search suitable fields based on query
-    _app.add_route("/search/{search_term}", status_resource, suffix="search")
+    _app.add_route("/search/families", status_resource, suffix="search_families")
+    _app.add_route("/search/samples", status_resource, suffix="search_samples")
+    _app.add_route("/search/functions", status_resource, suffix="search_functions")
 
     _app.add_route("/families", family_resource, suffix="collection")
+    # supports GET, PUT (for modification of family_name, is_library), DELETE (for all samples)
     _app.add_route("/families/{family_id:int}", family_resource)
 
-    # supports GET and POST(to insert one sample)
+    # supports GET and POST (to insert one sample)
     _app.add_route("/samples", sample_resource, suffix="collection")
     # post only
     _app.add_route("/samples/binary", sample_resource, suffix="submit_binary")
-    # supports GET and DELETE(for one sample)
+    # supports GET, PUT (for modification of family_name, version, component, is_library), DELETE (for one sample)
     _app.add_route("/samples/{sample_id:int}", sample_resource)
+    #
+    _app.add_route("/samples/sha256/{sample_sha256}", sample_resource, suffix="by_sha256")
     _app.add_route("/samples/{sample_id:int}/functions", sample_resource, suffix="functions")
     _app.add_route(
         "/samples/{sample_id:int}/functions/{function_id:int}",
         sample_resource,
         suffix="function",
     )
 
     _app.add_route("/functions", function_resource, suffix="collection")
     _app.add_route("/functions/{function_id:int}", function_resource)
 
     _app.add_route("/matches/sample/{sample_id:int}", match_resource, suffix="sample")
-    _app.add_route("/matches/sample/{sample_id:int}/{sample_id_2:int}", match_resource, suffix="sample_vs")
-    _app.add_route("/matches/function/{function_id:int}/{function_id_2:int}", match_resource, suffix="function_vs")
+    _app.add_route("/matches/sample/cross/{sample_ids}", match_resource, suffix="sample_cross")
+    _app.add_route("/matches/sample/{sample_id:int}/{sample_id_b:int}", match_resource, suffix="sample_vs")
+    _app.add_route("/matches/function/{function_id:int}/{function_id_b:int}", match_resource, suffix="function_vs")
     _app.add_route("/matches/function/{function_id:int}", match_resource, suffix="function")
 
+    _app.add_route("/uniqueblocks/samples/{comma_separated_sample_ids}", block_resource, suffix="unique_blocks_for_samples")
+    _app.add_route("/uniqueblocks/family/{family_id:int}", block_resource, suffix="unique_blocks_for_family")
+
     _app.add_route("/query", query_resource, suffix="query_smda")
     _app.add_route("/query/binary", query_resource, suffix="query_binary")
     _app.add_route(
         "/query/binary/mapped/{base_address}",
         query_resource,
         suffix="query_binary_mapped",
     )
+    _app.add_route("/query/function", query_resource, suffix="query_smda_function")
+    _app.add_route("/query/pichash/{pichash}", query_resource, suffix="query_pichash")
+    _app.add_route("/query/pichash/{pichash}/summary", query_resource, suffix="query_pichash_summary")
+    _app.add_route("/query/picblockhash/{picblockhash}", query_resource, suffix="query_picblockhash")
+    _app.add_route("/query/picblockhash/{picblockhash}/summary", query_resource, suffix="query_picblockhash_summary")
 
     _app.add_route("/jobs", job_resource, suffix="collection")
     _app.add_route("/jobs/{job_id}", job_resource)
     _app.add_route("/jobs/{job_id}/result", job_resource, suffix="job_result")
     _app.add_route("/results/{result_id}", job_resource, suffix="results")
+    _app.add_route("/results/{result_id}/job", job_resource, suffix="result_job")
 
     return _app
```

### Comparing `mcrit-0.9.5/mcrit/server/utils.py` & `mcrit-1.0.0/mcrit/server/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 from timeit import default_timer as timer
 from bson import json_util
 import logging
 
 LOGGER = logging.getLogger(__name__)
 
 
+def db_log_msg(index, req, message, level=None):
+    username = req.get_header("username", default="anonymous")
+    if level is None:
+        LOGGER.info(f"{username} - {message}")
+    index._storage.dbLogEvent(message, username=username)
+    return
+
+
 def getMatchingParams(req_params):
     parameters = {}
     for key, value in req_params.items():
         try:
             if key == "pichash_size":
                 pichash_size = int(value)
                 pichash_size = max(0, pichash_size)
@@ -17,16 +25,20 @@
             if key == "minhash_score":
                 minhash_score = int(value)
                 minhash_score = max(0, min(100, minhash_score))
                 parameters["minhash_threshold"] = minhash_score
             if key == "force_recalculation":
                 if value.lower() == "true":
                     parameters["force_recalculation"] = True
+            if key == "band_matches_required":
+                band_matches_required = int(value)
+                band_matches_required = max(0, band_matches_required)
+                parameters["band_matches_required"] = band_matches_required
         except:
-            LOGGER.warn(f"Failed to handle request parameter: {key}: {value}")
+            LOGGER.warning(f"Failed to handle request parameter: {key}: {value}")
     return parameters
 
 
 def jsonify(content, debug_print=False):
     if debug_print:
         print(content)
         print(json_util.dumps(content).encode("utf-8"))
```

### Comparing `mcrit-0.9.5/mcrit/storage/FunctionEntry.py` & `mcrit-1.0.0/mcrit/storage/FunctionEntry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from typing import TYPE_CHECKING, Dict, Optional
 
+from smda.common.BinaryInfo import BinaryInfo
+from smda.common.SmdaFunction import SmdaFunction
+
 from mcrit.minhash.MinHash import MinHash
+from mcrit.storage.FunctionLabelEntry import FunctionLabelEntry
 
 if TYPE_CHECKING:  # pragma: no cover
     from mcrit.storage.SampleEntry import SampleEntry
     from smda.common.SmdaFunction import SmdaFunction
 
 # Dataclass, post init
 # constructor -> .fromSmdaFunction
@@ -20,17 +24,18 @@
     sample_id: int
     minhash: bytes  # TODO rename -> minhash_bytes? minhash_hex?
     minhash_shingle_composition: Dict = None  # FIXME MongoDbStorage fails without this, ... why?
     # inherited from sample
     architecture: str
     # smda information
     function_name: str
+    function_labels: list
     matches: Dict
     pichash: int
-    picblockhashes: Dict
+    picblockhashes: list
     num_blocks: int
     num_instructions: int
     binweight: float
     offset: int
     xcfg: Dict
 
     def __init__(
@@ -49,35 +54,42 @@
             self.num_blocks = smda_function.num_blocks
             self.num_instructions = smda_function.num_instructions
             self.binweight = smda_function.binweight
             self.offset = smda_function.offset
             self.xcfg = smda_function.toDict()
             self.function_name = smda_function.function_name
             self.pichash = smda_function.pic_hash
-            self.picblockhashes = {}
+            self.picblockhashes = []
+        self.function_labels = []
         self.matches = {}
         empty_minhash = MinHash()
         self.minhash = minhash.getMinHash() if minhash else empty_minhash.getMinHash()
         self.shingler_composition = minhash.getComposition() if minhash else empty_minhash.getComposition()
 
     def getMinHash(self, minhash_bits=32):
         return MinHash(function_id=self.function_id, minhash_bytes=self.minhash, minhash_bits=minhash_bits)
 
+    def toSmdaFunction(self):
+        binary_info = BinaryInfo(b"")
+        binary_info.architecture = self.architecture
+        return SmdaFunction.fromDict(self.xcfg, binary_info=binary_info)
+
     def toDict(self):
         empty_minhash = MinHash()
         minhash = self.minhash if self.minhash else empty_minhash.getMinHash()
         shingler_composition = (
             self.minhash_shingle_composition if self.minhash_shingle_composition else empty_minhash.getComposition()
         )
         function_entry = {
             "architecture": self.architecture,
             "binweight": self.binweight,
             "family_id": self.family_id,
             "function_id": self.function_id,
             "function_name": self.function_name,
+            "function_labels": [l.toDict() for l in self.function_labels],
             "matches": self.matches,
             "minhash": minhash.hex(),
             "minhash_shingle_composition": shingler_composition,
             "num_blocks": self.num_blocks,
             "num_instructions": self.num_instructions,
             "offset": self.offset,
             "pichash": self.pichash,
@@ -91,24 +103,27 @@
     def fromDict(cls, entry_dict):
         function_entry = cls(None, None, entry_dict["function_id"])  # type: ignore
         function_entry.family_id = entry_dict["family_id"]
         # function_entry.function_id = entry_dict["function_id"]
         function_entry.sample_id = entry_dict["sample_id"]
         function_entry.architecture = entry_dict["architecture"]
         function_entry.function_name = entry_dict["function_name"]
+        function_entry.function_labels = [FunctionLabelEntry.fromDict(l) for l in entry_dict["function_labels"]] if "function_labels" in entry_dict else []
+        for label in function_entry.function_labels:
+            label.setFunctionId(entry_dict["function_id"])
         function_entry.matches = entry_dict["matches"]
         function_entry.pichash = entry_dict["pichash"]
         function_entry.picblockhashes = entry_dict["picblockhashes"]
         function_entry.minhash = bytes.fromhex(entry_dict["minhash"])
         function_entry.minhash_shingle_composition = entry_dict["minhash_shingle_composition"]
         function_entry.num_blocks = entry_dict["num_blocks"]
         function_entry.num_instructions = entry_dict["num_instructions"]
         function_entry.binweight = entry_dict["binweight"]
         function_entry.offset = entry_dict["offset"]
-        function_entry.xcfg = entry_dict["xcfg"]
+        function_entry.xcfg = entry_dict["xcfg"] if "xcfg" in entry_dict else None
         return function_entry
 
     @classmethod
     def fromAlchemyFunction(cls, function):
         function_entry = cls(None, None)  # type:ignore
         function_entry.binweight = function.binweight
         function_entry.function_id = function.id
```

### Comparing `mcrit-0.9.5/mcrit/storage/MatchedFunctionEntry.py` & `mcrit-1.0.0/mcrit/storage/MatchedFunctionEntry.py`

 * *Files 19% similar despite different names*

```diff
@@ -54,25 +54,15 @@
             "offset": self.offset,
             "matches": self.getMatchTuple()
         }
         return matching_entry
 
     @classmethod
     def fromDict(cls, entry_dict):
-        matching_entry = cls(None)
-        matching_entry.function_id = entry_dict["fid"]
-        matching_entry.num_bytes = entry_dict["num_bytes"]
-        matching_entry.offset = entry_dict["offset"]
-        matching_entry.matched_family_id = entry_dict["matches"][0]
-        matching_entry.matched_sample_id = entry_dict["matches"][1]
-        matching_entry.matched_function_id = entry_dict["matches"][2]
-        matching_entry.matched_score = entry_dict["matches"][3]
-        matching_entry.match_is_minhash = True if entry_dict["matches"][4] & MatcherInterface.IS_MINHASH_FLAG else False
-        matching_entry.match_is_pichash = True if entry_dict["matches"][4] & MatcherInterface.IS_PICHASH_FLAG else False
-        matching_entry.match_is_library = True if entry_dict["matches"][4] & MatcherInterface.IS_LIBRARY_FLAG else False
+        matching_entry = cls(entry_dict["fid"], entry_dict["num_bytes"], entry_dict["offset"], entry_dict["matches"])
         return matching_entry
 
     def __str__(self):
         flag_str = "m" if self.match_is_minhash else "."
         flag_str += "p" if self.match_is_pichash else "."
         flag_str += "l" if self.match_is_library else "."
         return "Function: fid({}) num_bytes({}) - Matched: family_id({}) sample_id({}) function_id({}) score({}) flags({})".format(
```

### Comparing `mcrit-0.9.5/mcrit/storage/MatchedSampleEntry.py` & `mcrit-1.0.0/mcrit/storage/MatchedSampleEntry.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     version: str
     bitness: int
     sha256: str
     filename: str
     sample_id: int
     num_bytes: int
     num_functions: int
+    is_library: bool
     # related to matching
     matched_functions_minhash: int
     matched_functions_pichash: int
     matched_functions_combined: int
     matched_functions_library: int
     # scores
     matched_bytes_unweighted: float
@@ -101,14 +102,15 @@
         matching_entry.version = entry_dict["version"]
         matching_entry.bitness = entry_dict["bitness"]
         matching_entry.sha256 = entry_dict["sha256"]
         matching_entry.filename = entry_dict["filename"]
         matching_entry.sample_id = entry_dict["sample_id"]
         matching_entry.num_bytes = entry_dict["num_bytes"]
         matching_entry.num_functions = entry_dict["num_functions"]
+        matching_entry.is_library = entry_dict["is_library"] if "is_library" in entry_dict else False
 
         matching_entry.matched_functions_minhash = entry_dict["matched"]["functions"]["minhashes"]
         matching_entry.matched_functions_pichash = entry_dict["matched"]["functions"]["pichashes"]
         matching_entry.matched_functions_combined = entry_dict["matched"]["functions"]["combined"]
         matching_entry.matched_functions_library = entry_dict["matched"]["functions"]["library"]
 
         matching_entry.matched_bytes_unweighted = entry_dict["matched"]["bytes"]["unweighted"]
```

### Comparing `mcrit-0.9.5/mcrit/storage/SampleEntry.py` & `mcrit-1.0.0/mcrit/storage/SampleEntry.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
         return self.sha256
 
     def getShortFilename(self, size_visible=20):
         if len(self.filename) > 2 * size_visible:
             return self.filename[:size_visible] + "..." + self.filename[-size_visible:]
         return self.filename
 
-
     def toDict(self):
         sample_entry = {
             "architecture": self.architecture,
             "base_addr": self.base_addr,
             "binary_size": self.binary_size,
             "binweight": self.binweight,
             "bitness": self.bitness,
```

### Comparing `mcrit-0.9.5/mcrit/storage/StorageFactory.py` & `mcrit-1.0.0/mcrit/storage/StorageFactory.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 class StorageFactory:
 
     STORAGE_METHOD_MEMORY = "memory"
     STORAGE_METHOD_ALCHEMY = "alchemy"
     STORAGE_METHOD_MONGODB = "mongodb"
 
     @staticmethod
-    def getStorage(storage_config):
-        if storage_config.STORAGE_METHOD == StorageFactory.STORAGE_METHOD_MONGODB:
-            return MongoDbStorage(storage_config)
+    def getStorage(mcrit_config):
+        if mcrit_config.STORAGE_CONFIG.STORAGE_METHOD == StorageFactory.STORAGE_METHOD_MONGODB:
+            return MongoDbStorage(mcrit_config)
         # Alchemy not supported right now
         # if storage_config.STORAGE_METHOD == StorageFactory.STORAGE_METHOD_ALCHEMY:
         #     return AlchemyStorage(storage_config)
-        return MemoryStorage(storage_config)
+        return MemoryStorage(mcrit_config)
```

### Comparing `mcrit-0.9.5/mcrit/storage/StorageInterface.py` & `mcrit-1.0.0/mcrit/storage/StorageInterface.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import random
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Set, Tuple, Union
 
 from mcrit.minhash.MinHash import MinHash
 
 if TYPE_CHECKING: # pragma: no cover
     from mcrit.config.StorageConfig import StorageConfig
+    from mcrit.config.McritConfig import McritConfig
+    from mcrit.config.MinHashConfig import MinHashConfig
     from mcrit.storage.FunctionEntry import FunctionEntry
     from mcrit.storage.MatchingCache import MatchingCache
     from mcrit.storage.MemoryStorage import MemoryStorage
     from mcrit.storage.SampleEntry import SampleEntry
     from smda.common.SmdaFunction import SmdaFunction
     from smda.common.SmdaReport import SmdaReport
 
@@ -21,45 +23,60 @@
 BandHash = int
 PicHash = int
 Sha256 = str
 
 
 class StorageInterface:
     _config: "StorageConfig"
+    _band_projection: None
 
-    def __init__(self, config: "StorageConfig") -> None:
+    def __init__(self, config: "McritConfig") -> None:
         """Set the StorageConfig, sets up an empty Storage or loads existing data, ensures indexing,
         and ensures the existence of an Family with name \"\" and family_id 0.
 
         Args:
             config: the configuration of this Storage
 
         Raises:
             AssertionError: If family_id 0 already exists, but does not refer to Family \"\".
         """
         self._config = config
+        self._storage_config = config.STORAGE_CONFIG
+        self._minhash_config = config.MINHASH_CONFIG
+        self._band_projection = None
+
+    def dbLogEvent(self, event_msg: str, username: Optional[str] = None, details: Optional[dict] = None) -> None:
+        """ Log an event to the database
+
+        Args:
+            event_msg: a string describing the event
+            username: (optional) a username tied to this event
+            details: a dict with arbitrary additional information
+        """
 
     # -> Set[function_id]
-    def getCandidatesForMinHash(self, minhash: "MinHash") -> Set[int]:
+    def getCandidatesForMinHash(self, minhash: "MinHash", band_matches_required=1) -> Set[int]:
         """Given a MinHash, return all candidates from all matching bands.
 
         Args:
             minhash: a MinHash
+            band_matches_required: the number of bands a minhash needs to match before being considered a candidate
 
         Returns:
             candidates: a set of function_ids
         """
         raise NotImplementedError
 
     # -> Dict[function_id, Set[function_id]]
-    def getCandidatesForMinHashes(self, function_id_to_minhash: Dict[int, "MinHash"]) -> Dict[int, Set[int]]:
+    def getCandidatesForMinHashes(self, function_id_to_minhash: Dict[int, "MinHash"], band_matches_required=1) -> Dict[int, Set[int]]:
         """Given MinHashes by function_id, return all candidates from all matching bands.
 
         Args:
             function_id_to_minhash: a dict mapping a function_id to a MinHash.
+            band_matches_required: the number of bands a minhash needs to match before being considered a candidate
 
         Returns:
             candidates: a dict mapping a function_id to a set of candidate function_ids.
         """
         raise NotImplementedError
 
     def deleteXcfgData(self) -> None:
@@ -96,27 +113,41 @@
             sha256: The SHA256 value to look up.
 
         Returns:
             A SampleEntry with the specified SHA256 or None, if no such SampleEntry exists.
         """
         raise NotImplementedError
 
-    def addSmdaReport(self, smda_report: "SmdaReport") -> Optional["SampleEntry"]:
+    def addSmdaReport(self, smda_report: "SmdaReport", isQuery=False) -> Optional["SampleEntry"]:
         """Add a SMDA report to storage to create its sample representation and return corresponding SampleEntry object.
         This also adds the sample's functions. If the sample's family is not in storage yet, it will be added.
         If a sample with the same SHA256 already exists in storage, smda_report is not added and None is returned.
 
         Args:
             smda_report: the SmdaReport to add to the storage
+            isQuery: True if this SmdaReport is associated with a matching query and its data shall not be persisted in the main DB
 
         Returns:
             A SampleEntry corresponding to smda_report or None, if SmdaReport was already added.
         """
         raise NotImplementedError
 
+    def updateFunctionLabels(self, smda_report: "SmdaReport", username: str) -> Optional["SampleEntry"]:
+        """Use a given SMDA report to update all non-dummy function labels for the SampleEntry matching its SHA256
+        If no matching SampleEntry exists, no update happens.
+
+        Args:
+            smda_report: the SmdaReport to be used for updating function labels
+            username: a username that allows tracking who submitted the labels
+
+        Returns:
+            True if SampleEntry was found and potentially labels were added, False otherwise.
+        """
+        raise NotImplementedError
+
     def importSampleEntry(self, sample_entry: "SampleEntry") -> Optional["SampleEntry"]:
         """Import a sample_entry to storage based on a previously exported SampleEntry.
         We assume that the family_id was already remapped by the MinHashIndex, meaning that only the sample_id needs to be adjusted
         If a sample with the same SHA256 already exists in storage, sample_entry is not added and None is returned.
 
         Args:
             sample_entry: the SampleEntry to add to the storage
@@ -124,25 +155,61 @@
         Returns:
             An adjusted SampleEntry if successful or None, if SampleEntry was already added.
         """
         raise NotImplementedError
 
     def importFunctionEntry(self, function_entry: "FunctionEntry") -> Optional["FunctionEntry"]:
         """Import a function_entry to storage based on a previously exported FunctionEntry.
-        We assume that the family_id and sample_id was already remapped by the MinHashIndex, meaning that only the function_id needs to be adjusted
-        When importing similarity hashes (pichash, minhash, ...) make sure they are added to their respective lookup indices. 
+        We assume that the family_id and sample_id were already remapped by the MinHashIndex, meaning that only the function_id needs to be adjusted.
 
         Args:
             function_entry: the FunctionEntry to add to the storage
 
         Returns:
             An adjusted FunctionEntry if successful or None, if we failed somewhere in the procedure
         """
         raise NotImplementedError
 
+
+    def importFunctionEntries(self, function_entries: List["FunctionEntry"]) -> Optional[List["FunctionEntry"]]:
+        """Import multiple function_entries to storage based on previously exported FunctionEntry objects.
+        We assume that the family_id and sample_id were already remapped by the MinHashIndex, meaning that only the function_ids need to be adjusted.
+
+        Args:
+            function_entries: List of FunctionEntry objects to add to the storage
+
+        Returns:
+            A list of adjusted FunctionEntry objects if successful or None, if we failed somewhere in the procedure
+        """
+        raise NotImplementedError
+
+    def modifyFamily(self, family_id: int, update_information: dict) -> bool:
+        """Update a family from the storage
+
+        Args:
+            family_id: the id of the sample to modify
+            update_information: a dictionary with update information for fields (family_name, is_library)
+
+        Returns:
+            True if family_id was contained in the storage and updated successfully, False otherwise
+        """
+        raise NotImplementedError
+
+    def modifySample(self, sample_id: int, update_information: dict) -> bool:
+        """Update a sample from the storage
+
+        Args:
+            sample_id: the id of the sample to modify
+            update_information: a dictionary with update information for fields (family_name, version, component, is_library)
+
+        Returns:
+            True if sample_id was contained in the storage and updated successfully, False otherwise
+        """
+        raise NotImplementedError
+
     def deleteSample(self, sample_id: int) -> bool:
         """Remove a sample from the storage, also removes all functions of the sample.
         All minhashes will be removed from the bands.
 
         Args:
             sample_id: the id of the sample to delete
 
@@ -215,46 +282,42 @@
 
         Returns:
             If sample_id exists in storage and belongs to a library: a dict with keys
                 "family" and "version" containing the respective data from the sample_id's SampeEnty, otherwise None.
         """
         raise NotImplementedError
 
-    # (check if sample_id exists?)
-    def _addFunction(
-        self, sample_entry: "SampleEntry", smda_function: "SmdaFunction", minhash: Optional["MinHash"] = None
-    ) -> "FunctionEntry":
-        """Add a function (and optionally its MinHash) to storage, using the respective SampleEntry for reference.
+    def getFunctionsBySampleId(self, sample_id: int) -> Optional[List["FunctionEntry"]]:
+        """For a given sample_id, get all corresponding FunctionEntries.
 
         Args:
-            sample_entry: The SampleEntry of smda_function
-            smda_function: The SmdaFunction to be added.
-            minhash: (Optional, defaults to None) The MinHash of the Function
+            sample_id: a sample_id
 
         Returns:
-            A FunctionEntry
+            A list of FunctionEntries or None, if sample_id does not exist
         """
         raise NotImplementedError
 
-    def getFunctionsBySampleId(self, sample_id: int) -> Optional[List["FunctionEntry"]]:
-        """For a given sample_id, get all corresponding FunctionEntries.
+    def getFunctionIdsBySampleId(self, sample_id: int) -> Optional[List["int"]]:
+        """For a given sample_id, get all corresponding function_ids.
 
         Args:
             sample_id: a sample_id
 
         Returns:
-            A list of FunctionEntries or None, if sample_id does not exist
+            A list of int or None, if sample_id does not exist
         """
         raise NotImplementedError
 
-    def getFunctionById(self, function_id: int) -> Optional["FunctionEntry"]:
+    def getFunctionById(self, function_id: int, with_xcfg=False) -> Optional["FunctionEntry"]:
         """Given a function_id, return the respective FunctionEntry or None, if function_id is not contained otherwise.
 
         Args:
             function_id: a function id
+            with_xcfg: include xcfg info (default: False)
 
         Returns:
             the respective FunctionEntry or None, if function_id is not contained otherwise
 
         """
         raise NotImplementedError
 
@@ -384,14 +447,26 @@
             family_name: The name of the family to add
 
         Returns:
             family_id of the added (or already existing) family name
         """
         raise NotImplementedError
 
+    def deleteFamily(self, family_id: int, keep_samples: Optional[str] = False) -> bool:
+        """Delete family if known and return boolean success state
+
+        Args:
+            family_id: The family_id of the family to delete
+            keep_samples: instead of deleting all samples and functions, reassign their family to "Unnamed (0)"
+
+        Returns:
+            True if successful
+        """
+        raise NotImplementedError
+
     def getFamilyIds(self) -> List[int]:
         """Returns a List of all family ids
 
         Returns:
             a List of all family ids
         """
         raise NotImplementedError
@@ -467,40 +542,66 @@
             sample_id: the sample id for PicHash matching
 
         Returns:
             a dict mapping the sample's function's pichashes to a set of (sample_id, function_id) having the same pichash or None.
         """
         raise NotImplementedError
 
-    def getMatchesForPicHash(self, pichash: int) -> Set[Tuple[int, int]]:
-        """Get the set of all (sample_id, function_id) tuples for a given PicHash. If no function has the given pichash, the empty set is returned
+    def getMatchesForPicHash(self, pichash: int) -> Set[Tuple[int, int, int]]:
+        """Get the set of all (family_id, sample_id, function_id) tuples for a given PicHash. If no function has the given pichash, the empty set is returned
 
         Args:
             pichash: the pichash to look up
 
         Returns:
-            a set of (sample_id, function_id) tuples with the given pichash
+            a set of (family_id, sample_id, function_id) tuples with the given pichash
+        """
+        raise NotImplementedError
+
+
+    def getMatchesForPicBlockHash(self, picblockhash: int) -> Set[Tuple[int, int, int, int]]:
+        """Get the set of all (family_id, sample_id, function_id, offset) tuples for a given PicBlockHash. If no function has the given picblockhash, the empty set is returned
+
+        Args:
+            picblockhash: the picblockhash to look up
+
+        Returns:
+            a set of (family_id, sample_id, function_id, offset) tuples with the given picblockhash
         """
         raise NotImplementedError
 
     def getStats(self) -> Dict[str, Union[int, Dict[int, int]]]:
         raise NotImplementedError
 
-    def getUnhashedFunctions(self, function_ids: Optional[List[int]] = None) -> List["FunctionEntry"]:
+    def getUnhashedFunctions(self, function_ids: Optional[List[int]] = None, only_function_ids=False) -> List["FunctionEntry"]:
         """Given a list of function_ids, return all FunctionEntry objects corresponding to these IDs if they do not have a minhash yet.
         Otherwise, return all FunctionEntry objects that do not have a minhash.
 
         Args:
             function_ids: (optional) a list of function_ids
+            only_function_ids: (optional) instead if FunctionEntry objects, only return function_ids
 
         Returns:
             a list of FunctionEntry objects without minhash
         """
         raise NotImplementedError
 
+
+    def getUniqueBlocks(self, sample_ids: Optional[List[int]] = None, progress_reporter=None) -> Dict:
+        """Given a list of sample_ids, return all basic blocks that are only found in any of these samples (and no other samples in the storage)
+
+        Args:
+            sample_ids: (optional) a list of sample_ids
+            progress_reporter: (optional) might be passed by worker to inquiry progress of this DB only operation
+
+        Returns:
+            a dictionary with the isolated blocks
+        """
+        raise NotImplementedError
+
     def findFamilyByString(self, needle: str, max_num_results: int = 100) -> Dict[int, str]:
         """Given a needle, return all families that contain the term we are searching.
 
         Args:
             needle: a search string
             max_num_results: (optional) maximum number of results to return, default 100
 
@@ -529,30 +630,42 @@
             max_num_results: (optional) maximum number of results to return, default 100
 
         Returns:
             a dict of function_id->FunctionEntry containing the needle
         """
         raise NotImplementedError
 
+    def createBandhashProjection(self, minhash):
+        """Calculate a projection for index permutation based on a given minhash
+        Args:
+            minhash: the MinHash used as reference
+        Returns:
+            a dict containing signature indices used for bandhashing by band id
+        """
+        band_projection = {}
+        random.seed(self._storage_config.STORAGE_BAND_SEED)
+        band_index = 0
+        for band_size, num_bands in self._storage_config.STORAGE_BANDS.items():
+            for _ in range(num_bands):
+                index_sequence = [index for index in range(len(minhash.getMinHashInt()))]
+                random.shuffle(index_sequence)
+                band_projection[band_index] = index_sequence[:band_size]
+                band_index += 1
+        return band_projection
+
     # -> Dict[BandIndex, BandHash]
     def getBandHashesForMinHash(self, minhash: "MinHash") -> Dict[int, int]:
         """Calculate band hashes for a given minhash, based on config parameters (STORAGE_BAND_SEED, STORAGE_BANDS)
-
         Args:
             minhash: the MinHash for which the BandHashes will be calculated
-
         Returns:
             a dict containing BandHashes by BandId
         """
+        if self._band_projection is None:
+            self._band_projection = self.createBandhashProjection(minhash)
         band_hashes = {}
-        random.seed(self._config.STORAGE_BAND_SEED)
-        band_index = 0
         minhash_data = minhash.getMinHashInt()
-        for band_size, num_bands in self._config.STORAGE_BANDS.items():
-            for _ in range(num_bands):
-                index_sequence = [index for index in range(len(minhash.getMinHashInt()))]
-                random.shuffle(index_sequence)
-                band_data = [minhash_data[i] for i in index_sequence[:band_size]]
-                hashed_band_data = MinHash.hashData(band_data, 0)
-                band_hashes[band_index] = hashed_band_data
-                band_index += 1
+        for band_index, permutation in self._band_projection.items():
+            band_data = [minhash_data[i] for i in permutation]
+            hashed_band_data = MinHash.hashData(band_data, 0)
+            band_hashes[band_index] = hashed_band_data
         return band_hashes
```

### Comparing `mcrit-0.9.5/setup.py` & `mcrit-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,33 +2,36 @@
 
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     README = f.read()
 
 requirements = [
+    "dataclasses",
     "falcon>=2.0.0",
-    "waitress",
+    "fastcluster",
     "mmh3>=2.5.1",
     "numpy",
-    "tqdm",
-    "smda>=1.3.0",
-    "dataclasses",
-    "pymongo",
     "picblocks>=1.1.2",
-    "requests"
+    "pymongo",
+    "pyparsing>=3",
+    "requests",
+    "scipy",
+    "smda>=1.3.0",
+    "tqdm",
+    "waitress",
 ]
 
 setup(
     name='mcrit',
-    version="0.9.5",
+    version="1.0.0",
     description='MCRIT is a framework created for simplified application of the MinHash algorithm to code similarity.',
     long_description_content_type="text/markdown",
     long_description=README,
-    author='Daniel Plohmann, Steffen Enders, Paul Hordiienko, Manuel Blatt',
+    author='Daniel Plohmann, Manuel Blatt, Steffen Enders, Paul Hordiienko',
     author_email='daniel.plohmann@fkie.fraunhofer.de',
     url='https://github.com/danielplohmann/mcrit',
     license="NU General Public License v3 (GPLv3)",
     packages=find_packages(exclude=("tests", "data", "docs", "examples", "plugins")),
     install_requires=requirements,
     data_files=[
         ("", ["LICENSE"]),
```

