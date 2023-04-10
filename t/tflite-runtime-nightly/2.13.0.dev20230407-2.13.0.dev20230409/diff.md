# Comparing `tmp/tflite_runtime_nightly-2.13.0.dev20230407-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/tflite_runtime_nightly-2.13.0.dev20230409-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 2546442 bytes, number of entries: 9
--rw-rw-r--  2.0 unx       80 b- defN 23-Apr-08 04:51 tflite_runtime/__init__.py
--rwxrwxr-x  2.0 unx  7379728 b- defN 23-Apr-08 04:53 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
--rw-rw-r--  2.0 unx    38775 b- defN 23-Apr-08 04:51 tflite_runtime/interpreter.py
--rw-rw-r--  2.0 unx     1542 b- defN 23-Apr-08 04:51 tflite_runtime/metrics_interface.py
--rw-rw-r--  2.0 unx     2048 b- defN 23-Apr-08 04:51 tflite_runtime/metrics_portable.py
--rw-rw-r--  2.0 unx     1440 b- defN 23-Apr-08 04:53 tflite_runtime_nightly-2.13.0.dev20230407.dist-info/METADATA
--rw-rw-r--  2.0 unx      111 b- defN 23-Apr-08 04:53 tflite_runtime_nightly-2.13.0.dev20230407.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Apr-08 04:53 tflite_runtime_nightly-2.13.0.dev20230407.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      878 b- defN 23-Apr-08 04:53 tflite_runtime_nightly-2.13.0.dev20230407.dist-info/RECORD
-9 files, 7424617 bytes uncompressed, 2544896 bytes compressed:  65.7%
+Zip file size: 2546441 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx       80 b- defN 23-Apr-10 04:56 tflite_runtime/__init__.py
+-rwxrwxr-x  2.0 unx  7379728 b- defN 23-Apr-10 04:58 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
+-rw-rw-r--  2.0 unx    38775 b- defN 23-Apr-10 04:56 tflite_runtime/interpreter.py
+-rw-rw-r--  2.0 unx     1542 b- defN 23-Apr-10 04:56 tflite_runtime/metrics_interface.py
+-rw-rw-r--  2.0 unx     2048 b- defN 23-Apr-10 04:56 tflite_runtime/metrics_portable.py
+-rw-rw-r--  2.0 unx     1440 b- defN 23-Apr-10 04:58 tflite_runtime_nightly-2.13.0.dev20230409.dist-info/METADATA
+-rw-rw-r--  2.0 unx      111 b- defN 23-Apr-10 04:58 tflite_runtime_nightly-2.13.0.dev20230409.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Apr-10 04:58 tflite_runtime_nightly-2.13.0.dev20230409.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      878 b- defN 23-Apr-10 04:58 tflite_runtime_nightly-2.13.0.dev20230409.dist-info/RECORD
+9 files, 7424617 bytes uncompressed, 2544895 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: tflite_runtime/metrics_interface.py
 Comment: 
 
 Filename: tflite_runtime/metrics_portable.py
 Comment: 
 
-Filename: tflite_runtime_nightly-2.13.0.dev20230407.dist-info/METADATA
+Filename: tflite_runtime_nightly-2.13.0.dev20230409.dist-info/METADATA
 Comment: 
 
-Filename: tflite_runtime_nightly-2.13.0.dev20230407.dist-info/WHEEL
+Filename: tflite_runtime_nightly-2.13.0.dev20230409.dist-info/WHEEL
 Comment: 
 
-Filename: tflite_runtime_nightly-2.13.0.dev20230407.dist-info/top_level.txt
+Filename: tflite_runtime_nightly-2.13.0.dev20230409.dist-info/top_level.txt
 Comment: 
 
-Filename: tflite_runtime_nightly-2.13.0.dev20230407.dist-info/RECORD
+Filename: tflite_runtime_nightly-2.13.0.dev20230409.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tflite_runtime/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__ = '2.13.0dev20230407'
-__git_version__ = '0.6.0-146116-gd6898f052da'
+__version__ = '2.13.0dev20230409'
+__git_version__ = '0.6.0-146138-g9df4da28b3f'
```

## Comparing `tflite_runtime_nightly-2.13.0.dev20230407.dist-info/METADATA` & `tflite_runtime_nightly-2.13.0.dev20230409.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tflite-runtime-nightly
-Version: 2.13.0.dev20230407
+Version: 2.13.0.dev20230409
 Summary: TensorFlow Lite is for mobile and embedded devices.
 Home-page: https://www.tensorflow.org/lite/
 Author: Google, LLC
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Keywords: tflite tensorflow tensor machine learning
 Classifier: Development Status :: 5 - Production/Stable
```

