# Comparing `tmp/types-jieba-0.0.5.tar.gz` & `tmp/types-jieba-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-jieba-0.0.5.tar", last modified: Fri Apr  7 06:28:08 2023, max compression
+gzip compressed data, was "types-jieba-0.0.6.tar", last modified: Mon Apr 10 02:46:40 2023, max compression
```

## Comparing `types-jieba-0.0.5.tar` & `types-jieba-0.0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 06:28:08.557661 types-jieba-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 06:28:08.553661 types-jieba-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 06:28:08.557661 types-jieba-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-07 06:27:56.000000 types-jieba-0.0.5/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-07 06:27:56.000000 types-jieba-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-07 06:27:56.000000 types-jieba-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-07 06:28:08.557661 types-jieba-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-07 06:27:56.000000 types-jieba-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 06:28:08.557661 types-jieba-0.0.5/jieba-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-07 06:27:56.000000 types-jieba-0.0.5/jieba-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-07 06:27:56.000000 types-jieba-0.0.5/jieba-stubs/_compat.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 06:28:08.557661 types-jieba-0.0.5/jieba-stubs/analyse/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-07 06:27:56.000000 types-jieba-0.0.5/jieba-stubs/analyse/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-07 06:27:56.000000 types-jieba-0.0.5/jieba-stubs/analyse/textrank.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-07 06:27:56.000000 types-jieba-0.0.5/jieba-stubs/analyse/tfidf.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 06:28:08.557661 types-jieba-0.0.5/jieba-stubs/posseg/
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-07 06:27:56.000000 types-jieba-0.0.5/jieba-stubs/posseg/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-07 06:27:56.000000 types-jieba-0.0.5/jieba-stubs/posseg/char_state_tab.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-07 06:27:56.000000 types-jieba-0.0.5/jieba-stubs/posseg/prob_emit.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 06:27:56.000000 types-jieba-0.0.5/jieba-stubs/posseg/prob_start.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-07 06:27:56.000000 types-jieba-0.0.5/jieba-stubs/posseg/prob_trans.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-07 06:27:56.000000 types-jieba-0.0.5/jieba-stubs/posseg/viterbi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-07 06:27:56.000000 types-jieba-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 06:28:08.557661 types-jieba-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 06:28:08.557661 types-jieba-0.0.5/types_jieba.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-07 06:28:08.000000 types-jieba-0.0.5/types_jieba.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-07 06:28:08.000000 types-jieba-0.0.5/types_jieba.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 06:28:08.000000 types-jieba-0.0.5/types_jieba.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-07 06:28:08.000000 types-jieba-0.0.5/types_jieba.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:46:40.881873 types-jieba-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:46:40.877874 types-jieba-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:46:40.881873 types-jieba-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-10 02:46:27.000000 types-jieba-0.0.6/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-10 02:46:27.000000 types-jieba-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-10 02:46:27.000000 types-jieba-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-10 02:46:40.881873 types-jieba-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-10 02:46:27.000000 types-jieba-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:46:40.881873 types-jieba-0.0.6/jieba-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-10 02:46:27.000000 types-jieba-0.0.6/jieba-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-10 02:46:27.000000 types-jieba-0.0.6/jieba-stubs/_compat.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:46:40.881873 types-jieba-0.0.6/jieba-stubs/analyse/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-10 02:46:27.000000 types-jieba-0.0.6/jieba-stubs/analyse/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-10 02:46:27.000000 types-jieba-0.0.6/jieba-stubs/analyse/textrank.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-10 02:46:27.000000 types-jieba-0.0.6/jieba-stubs/analyse/tfidf.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:46:40.881873 types-jieba-0.0.6/jieba-stubs/posseg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-10 02:46:27.000000 types-jieba-0.0.6/jieba-stubs/posseg/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-10 02:46:27.000000 types-jieba-0.0.6/jieba-stubs/posseg/char_state_tab.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-10 02:46:27.000000 types-jieba-0.0.6/jieba-stubs/posseg/prob_emit.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 02:46:27.000000 types-jieba-0.0.6/jieba-stubs/posseg/prob_start.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-10 02:46:27.000000 types-jieba-0.0.6/jieba-stubs/posseg/prob_trans.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-10 02:46:27.000000 types-jieba-0.0.6/jieba-stubs/posseg/viterbi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-10 02:46:27.000000 types-jieba-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 02:46:40.881873 types-jieba-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:46:40.881873 types-jieba-0.0.6/types_jieba.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-10 02:46:40.000000 types-jieba-0.0.6/types_jieba.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-10 02:46:40.000000 types-jieba-0.0.6/types_jieba.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 02:46:40.000000 types-jieba-0.0.6/types_jieba.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-10 02:46:40.000000 types-jieba-0.0.6/types_jieba.egg-info/top_level.txt
```

### Comparing `types-jieba-0.0.5/.github/workflows/publish.yaml` & `types-jieba-0.0.6/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `types-jieba-0.0.5/.gitignore` & `types-jieba-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `types-jieba-0.0.5/LICENSE` & `types-jieba-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `types-jieba-0.0.5/PKG-INFO` & `types-jieba-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-jieba
-Version: 0.0.5
+Version: 0.0.6
 Summary: jieba 类型库
 Author-email: thep0y <thepoy@163.com>
 License: MIT License
         
         Copyright (c) 2022 thep0y
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: types-jieba Version: 0.0.5 Summary: jieba ç±»ååº
+Metadata-Version: 2.1 Name: types-jieba Version: 0.0.6 Summary: jieba ç±»ååº
 Author-email: thep0y
 163.com> License: MIT License Copyright (c) 2022 thep0y Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `types-jieba-0.0.5/jieba-stubs/__init__.pyi` & `types-jieba-0.0.6/jieba-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-jieba-0.0.5/jieba-stubs/analyse/__init__.pyi` & `types-jieba-0.0.6/jieba-stubs/analyse/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # @Author:      thepoy
 # @Email:       thepoy@163.com
 # @File Name:   __init__.pyi
 # @Created At:  2022-08-03 09:47:47
-# @Modified At: 2023-04-07 13:58:38
+# @Modified At: 2023-04-10 10:44:24
 # @Modified By: thepoy
 
 from .tfidf import TFIDF
 from .textrank import TextRank
 
 default_tfidf: TFIDF
 default_textrank: TextRank
```

### Comparing `types-jieba-0.0.5/jieba-stubs/analyse/tfidf.pyi` & `types-jieba-0.0.6/jieba-stubs/analyse/tfidf.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 DEFAULT_IDF: str
 
 class KeywordExtractor:
     STOP_WORDS: Set[str]
 
     def set_stop_words(self, stop_words_path: str) -> None: ...
     @abstractmethod
-    def extract_tags(self, *args: Any, **kwargs: Dict[str, Any]) -> None: ...
+    def extract_tags(self, *args: Any, **kwargs: Dict[str, Any]) -> Any: ...
 
 class IDFLoader(object):
     path: str
     idf_freq: Dict[str, float]
     median_idf: float
 
     def __init__(self, idf_path: str | None = ...) -> None: ...
```

### Comparing `types-jieba-0.0.5/jieba-stubs/posseg/__init__.pyi` & `types-jieba-0.0.6/jieba-stubs/posseg/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-jieba-0.0.5/pyproject.toml` & `types-jieba-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `types-jieba-0.0.5/types_jieba.egg-info/PKG-INFO` & `types-jieba-0.0.6/types_jieba.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-jieba
-Version: 0.0.5
+Version: 0.0.6
 Summary: jieba 类型库
 Author-email: thep0y <thepoy@163.com>
 License: MIT License
         
         Copyright (c) 2022 thep0y
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: types-jieba Version: 0.0.5 Summary: jieba ç±»ååº
+Metadata-Version: 2.1 Name: types-jieba Version: 0.0.6 Summary: jieba ç±»ååº
 Author-email: thep0y
 163.com> License: MIT License Copyright (c) 2022 thep0y Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `types-jieba-0.0.5/types_jieba.egg-info/SOURCES.txt` & `types-jieba-0.0.6/types_jieba.egg-info/SOURCES.txt`

 * *Files identical despite different names*

