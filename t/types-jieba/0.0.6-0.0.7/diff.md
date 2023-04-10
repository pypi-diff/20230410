# Comparing `tmp/types-jieba-0.0.6.tar.gz` & `tmp/types-jieba-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-jieba-0.0.6.tar", last modified: Mon Apr 10 02:46:40 2023, max compression
+gzip compressed data, was "types-jieba-0.0.7.tar", last modified: Mon Apr 10 10:31:56 2023, max compression
```

## Comparing `types-jieba-0.0.6.tar` & `types-jieba-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:46:40.881873 types-jieba-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:46:40.877874 types-jieba-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:46:40.881873 types-jieba-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-10 02:46:27.000000 types-jieba-0.0.6/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-10 02:46:27.000000 types-jieba-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-10 02:46:27.000000 types-jieba-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-10 02:46:40.881873 types-jieba-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-10 02:46:27.000000 types-jieba-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:46:40.881873 types-jieba-0.0.6/jieba-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-10 02:46:27.000000 types-jieba-0.0.6/jieba-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-10 02:46:27.000000 types-jieba-0.0.6/jieba-stubs/_compat.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:46:40.881873 types-jieba-0.0.6/jieba-stubs/analyse/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-10 02:46:27.000000 types-jieba-0.0.6/jieba-stubs/analyse/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-10 02:46:27.000000 types-jieba-0.0.6/jieba-stubs/analyse/textrank.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-10 02:46:27.000000 types-jieba-0.0.6/jieba-stubs/analyse/tfidf.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:46:40.881873 types-jieba-0.0.6/jieba-stubs/posseg/
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-10 02:46:27.000000 types-jieba-0.0.6/jieba-stubs/posseg/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-10 02:46:27.000000 types-jieba-0.0.6/jieba-stubs/posseg/char_state_tab.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-10 02:46:27.000000 types-jieba-0.0.6/jieba-stubs/posseg/prob_emit.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 02:46:27.000000 types-jieba-0.0.6/jieba-stubs/posseg/prob_start.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-10 02:46:27.000000 types-jieba-0.0.6/jieba-stubs/posseg/prob_trans.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-10 02:46:27.000000 types-jieba-0.0.6/jieba-stubs/posseg/viterbi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-10 02:46:27.000000 types-jieba-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 02:46:40.881873 types-jieba-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:46:40.881873 types-jieba-0.0.6/types_jieba.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-10 02:46:40.000000 types-jieba-0.0.6/types_jieba.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-10 02:46:40.000000 types-jieba-0.0.6/types_jieba.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 02:46:40.000000 types-jieba-0.0.6/types_jieba.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-10 02:46:40.000000 types-jieba-0.0.6/types_jieba.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:31:56.833979 types-jieba-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:31:56.825979 types-jieba-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:31:56.829979 types-jieba-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-10 10:31:44.000000 types-jieba-0.0.7/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-10 10:31:44.000000 types-jieba-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-10 10:31:44.000000 types-jieba-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-10 10:31:56.833979 types-jieba-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-10 10:31:44.000000 types-jieba-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:31:56.829979 types-jieba-0.0.7/jieba-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-10 10:31:44.000000 types-jieba-0.0.7/jieba-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-10 10:31:44.000000 types-jieba-0.0.7/jieba-stubs/_compat.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:31:56.829979 types-jieba-0.0.7/jieba-stubs/analyse/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-10 10:31:44.000000 types-jieba-0.0.7/jieba-stubs/analyse/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-10 10:31:44.000000 types-jieba-0.0.7/jieba-stubs/analyse/textrank.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-10 10:31:44.000000 types-jieba-0.0.7/jieba-stubs/analyse/tfidf.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:31:56.829979 types-jieba-0.0.7/jieba-stubs/posseg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-10 10:31:44.000000 types-jieba-0.0.7/jieba-stubs/posseg/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-10 10:31:44.000000 types-jieba-0.0.7/jieba-stubs/posseg/char_state_tab.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-10 10:31:44.000000 types-jieba-0.0.7/jieba-stubs/posseg/prob_emit.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 10:31:44.000000 types-jieba-0.0.7/jieba-stubs/posseg/prob_start.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-10 10:31:44.000000 types-jieba-0.0.7/jieba-stubs/posseg/prob_trans.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-10 10:31:44.000000 types-jieba-0.0.7/jieba-stubs/posseg/viterbi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-10 10:31:44.000000 types-jieba-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 10:31:56.833979 types-jieba-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:31:56.829979 types-jieba-0.0.7/types_jieba.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-10 10:31:56.000000 types-jieba-0.0.7/types_jieba.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-10 10:31:56.000000 types-jieba-0.0.7/types_jieba.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 10:31:56.000000 types-jieba-0.0.7/types_jieba.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-10 10:31:56.000000 types-jieba-0.0.7/types_jieba.egg-info/top_level.txt
```

### Comparing `types-jieba-0.0.6/.github/workflows/publish.yaml` & `types-jieba-0.0.7/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `types-jieba-0.0.6/.gitignore` & `types-jieba-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `types-jieba-0.0.6/LICENSE` & `types-jieba-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `types-jieba-0.0.6/PKG-INFO` & `types-jieba-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-jieba
-Version: 0.0.6
+Version: 0.0.7
 Summary: jieba 类型库
 Author-email: thep0y <thepoy@163.com>
 License: MIT License
         
         Copyright (c) 2022 thep0y
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: types-jieba Version: 0.0.6 Summary: jieba ç±»ååº
+Metadata-Version: 2.1 Name: types-jieba Version: 0.0.7 Summary: jieba ç±»ååº
 Author-email: thep0y
 163.com> License: MIT License Copyright (c) 2022 thep0y Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `types-jieba-0.0.6/jieba-stubs/__init__.pyi` & `types-jieba-0.0.7/jieba-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-jieba-0.0.6/jieba-stubs/analyse/__init__.pyi` & `types-jieba-0.0.7/jieba-stubs/analyse/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-jieba-0.0.6/jieba-stubs/analyse/textrank.pyi` & `types-jieba-0.0.7/jieba-stubs/analyse/textrank.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # @Author:      thepoy
 # @Email:       thepoy@163.com
 # @File Name:   textrank.pyi
 # @Created At:  2022-08-03 09:47:47
-# @Modified At: 2023-04-07 14:00:55
+# @Modified At: 2023-04-10 18:29:55
 # @Modified By: thepoy
 
 from collections import defaultdict
 from jieba import Tokenizer
 from jieba.posseg import pair
 from .tfidf import KeywordExtractor
 from typing import List, Set, Tuple
@@ -39,8 +39,8 @@
     def extract_tags(
         self,
         sentence: str,
         topK: int = ...,
         withWeight: bool = ...,
         allowPOS: Tuple[str, ...] = ...,
         withFlag: bool = ...,
-    ) -> List[Tuple[str, float] | str]: ...
+    ) -> List[Tuple[str, float] | Tuple[pair, float] | str]: ...
```

### Comparing `types-jieba-0.0.6/jieba-stubs/analyse/tfidf.pyi` & `types-jieba-0.0.7/jieba-stubs/analyse/tfidf.pyi`

 * *Files identical despite different names*

### Comparing `types-jieba-0.0.6/jieba-stubs/posseg/__init__.pyi` & `types-jieba-0.0.7/jieba-stubs/posseg/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-jieba-0.0.6/pyproject.toml` & `types-jieba-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `types-jieba-0.0.6/types_jieba.egg-info/PKG-INFO` & `types-jieba-0.0.7/types_jieba.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-jieba
-Version: 0.0.6
+Version: 0.0.7
 Summary: jieba 类型库
 Author-email: thep0y <thepoy@163.com>
 License: MIT License
         
         Copyright (c) 2022 thep0y
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: types-jieba Version: 0.0.6 Summary: jieba ç±»ååº
+Metadata-Version: 2.1 Name: types-jieba Version: 0.0.7 Summary: jieba ç±»ååº
 Author-email: thep0y
 163.com> License: MIT License Copyright (c) 2022 thep0y Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `types-jieba-0.0.6/types_jieba.egg-info/SOURCES.txt` & `types-jieba-0.0.7/types_jieba.egg-info/SOURCES.txt`

 * *Files identical despite different names*

