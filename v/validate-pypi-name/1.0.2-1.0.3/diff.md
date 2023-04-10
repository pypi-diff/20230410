# Comparing `tmp/validate_pypi_name-1.0.2-py3-none-any.whl.zip` & `tmp/validate_pypi_name-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4315 bytes, number of entries: 8
+Zip file size: 4314 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 00:41 validate_pypi_name/__init__.py
 -rw-r--r--  2.0 unx     3942 b- defN 23-Apr-10 00:38 validate_pypi_name/validator.py
--rw-r--r--  2.0 unx     1075 b- defN 23-Apr-10 00:42 validate_pypi_name-1.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      739 b- defN 23-Apr-10 00:42 validate_pypi_name-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 00:42 validate_pypi_name-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       60 b- defN 23-Apr-10 00:42 validate_pypi_name-1.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       19 b- defN 23-Apr-10 00:42 validate_pypi_name-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      718 b- defN 23-Apr-10 00:42 validate_pypi_name-1.0.2.dist-info/RECORD
-8 files, 6645 bytes uncompressed, 3033 bytes compressed:  54.4%
+-rw-r--r--  2.0 unx     1075 b- defN 23-Apr-10 00:44 validate_pypi_name-1.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      739 b- defN 23-Apr-10 00:44 validate_pypi_name-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 00:44 validate_pypi_name-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       60 b- defN 23-Apr-10 00:44 validate_pypi_name-1.0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       19 b- defN 23-Apr-10 00:44 validate_pypi_name-1.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      718 b- defN 23-Apr-10 00:44 validate_pypi_name-1.0.3.dist-info/RECORD
+8 files, 6645 bytes uncompressed, 3032 bytes compressed:  54.4%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: validate_pypi_name/__init__.py
 Comment: 
 
 Filename: validate_pypi_name/validator.py
 Comment: 
 
-Filename: validate_pypi_name-1.0.2.dist-info/LICENSE
+Filename: validate_pypi_name-1.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: validate_pypi_name-1.0.2.dist-info/METADATA
+Filename: validate_pypi_name-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: validate_pypi_name-1.0.2.dist-info/WHEEL
+Filename: validate_pypi_name-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: validate_pypi_name-1.0.2.dist-info/entry_points.txt
+Filename: validate_pypi_name-1.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: validate_pypi_name-1.0.2.dist-info/top_level.txt
+Filename: validate_pypi_name-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: validate_pypi_name-1.0.2.dist-info/RECORD
+Filename: validate_pypi_name-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `validate_pypi_name-1.0.2.dist-info/LICENSE` & `validate_pypi_name-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `validate_pypi_name-1.0.2.dist-info/METADATA` & `validate_pypi_name-1.0.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validate-pypi-name
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simple CLI to determine validity of pypi pakage name.
 Home-page: https://github.com/pablojosecodes/pypi_name_validator
 Author: Pablo Hansen
 Author-email: pablosfsanchz@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `validate_pypi_name-1.0.2.dist-info/RECORD` & `validate_pypi_name-1.0.3.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 validate_pypi_name/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 validate_pypi_name/validator.py,sha256=SN-mSI40Zy_6XxBwZiXJYBXcEWZRan8PXVYNuFvVbok,3942
-validate_pypi_name-1.0.2.dist-info/LICENSE,sha256=D6PwCClZO8hbQ-nZxTH6HQEW9RuPmzIQC6lx-RWXs6k,1075
-validate_pypi_name-1.0.2.dist-info/METADATA,sha256=y2V8Y9Zf79CdL7DKhJQQJHcL7gx4LUEbxByUXD97VqI,739
-validate_pypi_name-1.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-validate_pypi_name-1.0.2.dist-info/entry_points.txt,sha256=82JN6dh_UL3S2o1vZbMoVNfdp4dEVL_nBzeMTXlXPpo,60
-validate_pypi_name-1.0.2.dist-info/top_level.txt,sha256=xhHh-CD0yA5lJ0vt2c9aJXVqvgnWkm9iqfVh69wFy4g,19
-validate_pypi_name-1.0.2.dist-info/RECORD,,
+validate_pypi_name-1.0.3.dist-info/LICENSE,sha256=D6PwCClZO8hbQ-nZxTH6HQEW9RuPmzIQC6lx-RWXs6k,1075
+validate_pypi_name-1.0.3.dist-info/METADATA,sha256=H0Hwl_U-EtptCYGzIYLBjWu8MnDZbqyM_i24koUjktI,739
+validate_pypi_name-1.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+validate_pypi_name-1.0.3.dist-info/entry_points.txt,sha256=82JN6dh_UL3S2o1vZbMoVNfdp4dEVL_nBzeMTXlXPpo,60
+validate_pypi_name-1.0.3.dist-info/top_level.txt,sha256=xhHh-CD0yA5lJ0vt2c9aJXVqvgnWkm9iqfVh69wFy4g,19
+validate_pypi_name-1.0.3.dist-info/RECORD,,
```

