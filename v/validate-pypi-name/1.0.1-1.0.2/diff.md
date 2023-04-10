# Comparing `tmp/validate_pypi_name-1.0.1-py3-none-any.whl.zip` & `tmp/validate_pypi_name-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4245 bytes, number of entries: 8
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-08 19:14 zzkkz/__init__.py
--rw-r--r--  2.0 unx     3942 b- defN 23-Apr-10 00:38 zzkkz/validator.py
--rw-r--r--  2.0 unx     1075 b- defN 23-Apr-10 00:40 validate_pypi_name-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      739 b- defN 23-Apr-10 00:40 validate_pypi_name-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 00:40 validate_pypi_name-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       60 b- defN 23-Apr-10 00:40 validate_pypi_name-1.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Apr-10 00:40 validate_pypi_name-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      691 b- defN 23-Apr-10 00:40 validate_pypi_name-1.0.1.dist-info/RECORD
-8 files, 6605 bytes uncompressed, 3015 bytes compressed:  54.4%
+Zip file size: 4315 bytes, number of entries: 8
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 00:41 validate_pypi_name/__init__.py
+-rw-r--r--  2.0 unx     3942 b- defN 23-Apr-10 00:38 validate_pypi_name/validator.py
+-rw-r--r--  2.0 unx     1075 b- defN 23-Apr-10 00:42 validate_pypi_name-1.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      739 b- defN 23-Apr-10 00:42 validate_pypi_name-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 00:42 validate_pypi_name-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       60 b- defN 23-Apr-10 00:42 validate_pypi_name-1.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       19 b- defN 23-Apr-10 00:42 validate_pypi_name-1.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      718 b- defN 23-Apr-10 00:42 validate_pypi_name-1.0.2.dist-info/RECORD
+8 files, 6645 bytes uncompressed, 3033 bytes compressed:  54.4%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: zzkkz/__init__.py
+Filename: validate_pypi_name/__init__.py
 Comment: 
 
-Filename: zzkkz/validator.py
+Filename: validate_pypi_name/validator.py
 Comment: 
 
-Filename: validate_pypi_name-1.0.1.dist-info/LICENSE
+Filename: validate_pypi_name-1.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: validate_pypi_name-1.0.1.dist-info/METADATA
+Filename: validate_pypi_name-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: validate_pypi_name-1.0.1.dist-info/WHEEL
+Filename: validate_pypi_name-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: validate_pypi_name-1.0.1.dist-info/entry_points.txt
+Filename: validate_pypi_name-1.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: validate_pypi_name-1.0.1.dist-info/top_level.txt
+Filename: validate_pypi_name-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: validate_pypi_name-1.0.1.dist-info/RECORD
+Filename: validate_pypi_name-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `zzkkz/validator.py` & `validate_pypi_name/validator.py`

 * *Files identical despite different names*

## Comparing `validate_pypi_name-1.0.1.dist-info/LICENSE` & `validate_pypi_name-1.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `validate_pypi_name-1.0.1.dist-info/METADATA` & `validate_pypi_name-1.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validate-pypi-name
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simple CLI to determine validity of pypi pakage name.
 Home-page: https://github.com/pablojosecodes/pypi_name_validator
 Author: Pablo Hansen
 Author-email: pablosfsanchz@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

