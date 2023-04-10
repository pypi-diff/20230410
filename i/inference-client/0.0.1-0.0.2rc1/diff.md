# Comparing `tmp/inference_client-0.0.1.tar.gz` & `tmp/inference_client-0.0.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inference_client-0.0.1.tar", last modified: Wed Mar  1 10:48:23 2023, max compression
+gzip compressed data, was "inference_client-0.0.2rc1.tar", max compression
```

## Comparing `inference_client-0.0.1.tar` & `inference_client-0.0.2rc1.tar`

### file list

```diff
@@ -1,15 +1,9 @@
-drwxr-xr-x   0 ziniuyu    (501) staff       (20)        0 2023-03-01 10:48:23.268130 inference_client-0.0.1/
--rw-r--r--   0 ziniuyu    (501) staff       (20)    10825 2023-03-01 10:34:26.000000 inference_client-0.0.1/LICENSE
--rw-r--r--   0 ziniuyu    (501) staff       (20)      565 2023-03-01 10:48:23.267983 inference_client-0.0.1/PKG-INFO
--rw-r--r--   0 ziniuyu    (501) staff       (20)       45 2023-03-01 10:28:09.000000 inference_client-0.0.1/README.md
--rw-r--r--   0 ziniuyu    (501) staff       (20)      591 2023-03-01 10:48:18.000000 inference_client-0.0.1/pyproject.toml
--rw-r--r--   0 ziniuyu    (501) staff       (20)       38 2023-03-01 10:48:23.268171 inference_client-0.0.1/setup.cfg
-drwxr-xr-x   0 ziniuyu    (501) staff       (20)        0 2023-03-01 10:48:23.266011 inference_client-0.0.1/src/
-drwxr-xr-x   0 ziniuyu    (501) staff       (20)        0 2023-03-01 10:48:23.267049 inference_client-0.0.1/src/inference_client/
--rw-r--r--   0 ziniuyu    (501) staff       (20)        0 2023-03-01 10:26:50.000000 inference_client-0.0.1/src/inference_client/__init__.py
--rw-r--r--   0 ziniuyu    (501) staff       (20)       42 2023-03-01 10:27:05.000000 inference_client-0.0.1/src/inference_client/example.py
-drwxr-xr-x   0 ziniuyu    (501) staff       (20)        0 2023-03-01 10:48:23.267774 inference_client-0.0.1/src/inference_client.egg-info/
--rw-r--r--   0 ziniuyu    (501) staff       (20)      565 2023-03-01 10:48:23.000000 inference_client-0.0.1/src/inference_client.egg-info/PKG-INFO
--rw-r--r--   0 ziniuyu    (501) staff       (20)      273 2023-03-01 10:48:23.000000 inference_client-0.0.1/src/inference_client.egg-info/SOURCES.txt
--rw-r--r--   0 ziniuyu    (501) staff       (20)        1 2023-03-01 10:48:23.000000 inference_client-0.0.1/src/inference_client.egg-info/dependency_links.txt
--rw-r--r--   0 ziniuyu    (501) staff       (20)       17 2023-03-01 10:48:23.000000 inference_client-0.0.1/src/inference_client.egg-info/top_level.txt
+-rw-r--r--   0        0        0    11357 2023-04-10 13:14:50.023323 inference_client-0.0.2rc1/LICENSE
+-rw-r--r--   0        0        0    12002 2023-04-10 13:14:50.023323 inference_client-0.0.2rc1/README.md
+-rw-r--r--   0        0        0       27 2023-04-10 13:14:50.027323 inference_client-0.0.2rc1/inference_client/__init__.py
+-rw-r--r--   0        0        0      443 2023-04-10 13:14:50.027323 inference_client-0.0.2rc1/inference_client/__version__.py
+-rw-r--r--   0        0        0     9590 2023-04-10 13:14:50.027323 inference_client-0.0.2rc1/inference_client/base.py
+-rw-r--r--   0        0        0      990 2023-04-10 13:14:50.027323 inference_client-0.0.2rc1/inference_client/client.py
+-rw-r--r--   0        0        0     5142 2023-04-10 13:14:50.027323 inference_client-0.0.2rc1/inference_client/helper.py
+-rw-r--r--   0        0        0     1316 2023-04-10 13:14:50.027323 inference_client-0.0.2rc1/pyproject.toml
+-rw-r--r--   0        0        0    24300 1970-01-01 00:00:00.000000 inference_client-0.0.2rc1/PKG-INFO
```

### Comparing `inference_client-0.0.1/LICENSE` & `inference_client-0.0.2rc1/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-Copyright 2020-2021 Jina AI Limited.  All rights reserved.
-
-
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
@@ -174,20 +171,31 @@
       of any other Contributor, and only if You agree to indemnify,
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
 
-   Copyright 2020-2021 Jina AI Limited
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
-   limitations under the License.
+   limitations under the License.
```

