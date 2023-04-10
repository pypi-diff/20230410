# Comparing `tmp/tvault-0.2.1-py3-none-any.whl.zip` & `tmp/tvault-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9009 bytes, number of entries: 10
--rw-r--r--  2.0 unx     1256 b- defN 23-Apr-10 03:48 tvault/__init__.py
+Zip file size: 9021 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     1284 b- defN 23-Apr-10 03:52 tvault/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-03 04:19 tvault/model_diff.py
 -rw-r--r--  2.0 unx     4789 b- defN 23-Apr-03 06:15 tvault/model_log.py
 -rw-r--r--  2.0 unx     5737 b- defN 23-Apr-05 05:40 tvault/parse_utils.py
 -rw-r--r--  2.0 unx    12480 b- defN 23-Apr-10 01:34 tvault/torchvault.py
--rw-r--r--  2.0 unx     1067 b- defN 23-Apr-10 03:48 tvault-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      380 b- defN 23-Apr-10 03:48 tvault-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 03:48 tvault-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-10 03:48 tvault-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      760 b- defN 23-Apr-10 03:48 tvault-0.2.1.dist-info/RECORD
-10 files, 26568 bytes uncompressed, 7723 bytes compressed:  70.9%
+-rw-r--r--  2.0 unx     1067 b- defN 23-Apr-10 03:52 tvault-0.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      380 b- defN 23-Apr-10 03:52 tvault-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 03:52 tvault-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-10 03:52 tvault-0.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      760 b- defN 23-Apr-10 03:52 tvault-0.2.2.dist-info/RECORD
+10 files, 26596 bytes uncompressed, 7735 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: tvault/parse_utils.py
 Comment: 
 
 Filename: tvault/torchvault.py
 Comment: 
 
-Filename: tvault-0.2.1.dist-info/LICENSE
+Filename: tvault-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: tvault-0.2.1.dist-info/METADATA
+Filename: tvault-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: tvault-0.2.1.dist-info/WHEEL
+Filename: tvault-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: tvault-0.2.1.dist-info/top_level.txt
+Filename: tvault-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: tvault-0.2.1.dist-info/RECORD
+Filename: tvault-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tvault/__init__.py

```diff
@@ -47,7 +47,8 @@
 Other utils
 """
 
 
 def find(log_dir="./model_log", model_dir="./", condition="hash", hash="", tag="", min=0, max=100):
     vault = TorchVault(log_dir, model_dir)
     vault.find(condition, hash, tag, min, max)
+    vault.show_result(hash)
```

## Comparing `tvault-0.2.1.dist-info/LICENSE` & `tvault-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tvault-0.2.1.dist-info/RECORD` & `tvault-0.2.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-tvault/__init__.py,sha256=qT5qpPNsTq74jgp631r_eJeRCH_cVNQgH7xt3jcgnuU,1256
+tvault/__init__.py,sha256=zbyjOOh-Y_ITUBJU3o0DdjvEjGVeIHjXDQpZ5OphLLQ,1284
 tvault/model_diff.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tvault/model_log.py,sha256=ZD1LeL1wBRKQEZaAfZEcjYP7w76yeD0eMRAnI-fBOiA,4789
 tvault/parse_utils.py,sha256=1gNwxk5UScEHIF_TG1te3r_gsYtFUaZTkWziLczvZ8I,5737
 tvault/torchvault.py,sha256=y4IjNeiSMkmiOdQPOp3Ur8-b34g0MtFZ5i_yulTiJuI,12480
-tvault-0.2.1.dist-info/LICENSE,sha256=WMAFuHtOPuSTgn-WJtxM1LLEDLfqaKQes7X7VhOaaOU,1067
-tvault-0.2.1.dist-info/METADATA,sha256=NIu_3CQavpnf4PdGW1CX6EYTNvtevlBW-vLPaKO6eOs,380
-tvault-0.2.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-tvault-0.2.1.dist-info/top_level.txt,sha256=Z1ZnwpooKsyvyYmlAXuGVOIRK1hO7QkkDVaneY85JDI,7
-tvault-0.2.1.dist-info/RECORD,,
+tvault-0.2.2.dist-info/LICENSE,sha256=WMAFuHtOPuSTgn-WJtxM1LLEDLfqaKQes7X7VhOaaOU,1067
+tvault-0.2.2.dist-info/METADATA,sha256=KIhnMxzr14vNvqHZ5sG70yaXNXoFWlxFVrdSG3hzCc0,380
+tvault-0.2.2.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+tvault-0.2.2.dist-info/top_level.txt,sha256=Z1ZnwpooKsyvyYmlAXuGVOIRK1hO7QkkDVaneY85JDI,7
+tvault-0.2.2.dist-info/RECORD,,
```

