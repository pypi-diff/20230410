# Comparing `tmp/tokenizador-1.45.tar.gz` & `tmp/tokenizador-1.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenizador-1.45.tar", last modified: Mon Mar 27 20:25:31 2023, max compression
+gzip compressed data, was "tokenizador-1.50.tar", last modified: Mon Apr 10 19:01:53 2023, max compression
```

## Comparing `tokenizador-1.45.tar` & `tokenizador-1.50.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1082 2023-03-27 15:24:58.174577 tokenizador-1.45/LICENSE
--rw-r--r--   0        0        0      501 2023-03-27 20:18:45.306764 tokenizador-1.45/pyproject.toml
--rw-r--r--   0        0        0     1904 2023-03-27 15:24:58.181244 tokenizador-1.45/readme.md
--rw-r--r--   0        0        0       62 2023-03-27 20:25:26.310853 tokenizador-1.45/tokenizador/__init__.py
--rw-r--r--   0        0        0      336 2023-03-27 20:24:48.970780 tokenizador-1.45/tokenizador/abbr_helpers.py
--rw-r--r--   0        0        0      112 2023-03-27 15:38:31.275102 tokenizador-1.45/tokenizador/data/en
--rw-r--r--   0        0        0      143 2023-03-27 15:39:30.585234 tokenizador-1.45/tokenizador/data/pt
--rwxr-xr-x   0        0        0     6053 2023-03-27 20:25:16.257500 tokenizador-1.45/tokenizador/main.py
--rw-r--r--   0        0        0       73 2023-03-27 16:14:02.475990 tokenizador-1.45/tokenizador/tokenizador.py
--rw-r--r--   0        0        0     2250 1970-01-01 00:00:00.000000 tokenizador-1.45/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-03-27 15:24:58.174577 tokenizador-1.50/LICENSE
+-rw-r--r--   0        0        0      501 2023-03-27 20:18:45.306764 tokenizador-1.50/pyproject.toml
+-rw-r--r--   0        0        0     1904 2023-03-27 15:24:58.181244 tokenizador-1.50/readme.md
+-rw-r--r--   0        0        0       62 2023-04-10 19:01:48.201699 tokenizador-1.50/tokenizador/__init__.py
+-rw-r--r--   0        0        0      336 2023-03-27 20:24:48.970780 tokenizador-1.50/tokenizador/abbr_helpers.py
+-rw-r--r--   0        0        0      112 2023-03-27 15:38:31.275102 tokenizador-1.50/tokenizador/data/en
+-rw-r--r--   0        0        0      143 2023-03-27 15:39:30.585234 tokenizador-1.50/tokenizador/data/pt
+-rwxr-xr-x   0        0        0     6053 2023-03-29 13:53:44.633449 tokenizador-1.50/tokenizador/main.py
+-rw-r--r--   0        0        0       73 2023-03-27 16:14:02.475990 tokenizador-1.50/tokenizador/tokenizador.py
+-rw-r--r--   0        0        0     2250 1970-01-01 00:00:00.000000 tokenizador-1.50/PKG-INFO
```

### Comparing `tokenizador-1.45/LICENSE` & `tokenizador-1.50/LICENSE`

 * *Files identical despite different names*

### Comparing `tokenizador-1.45/readme.md` & `tokenizador-1.50/readme.md`

 * *Files identical despite different names*

### Comparing `tokenizador-1.45/tokenizador/main.py` & `tokenizador-1.50/tokenizador/main.py`

 * *Files identical despite different names*

### Comparing `tokenizador-1.45/PKG-INFO` & `tokenizador-1.50/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenizador
-Version: 1.45
+Version: 1.50
 Summary: Text tokenizer done for SPLN 2022/2023
 Author-email: jpdiasfernandes <jpdiasfernandes13@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Source, https://github.com/jpdiasfernandes/spln-2223/tree/master/TPC5/project
```

