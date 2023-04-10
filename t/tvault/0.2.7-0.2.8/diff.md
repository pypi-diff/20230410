# Comparing `tmp/tvault-0.2.7-py3-none-any.whl.zip` & `tmp/tvault-0.2.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9021 bytes, number of entries: 10
--rw-r--r--  2.0 unx     1284 b- defN 23-Apr-10 03:52 tvault/__init__.py
+Zip file size: 9077 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     1455 b- defN 23-Apr-10 04:16 tvault/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-03 04:19 tvault/model_diff.py
 -rw-r--r--  2.0 unx     4789 b- defN 23-Apr-03 06:15 tvault/model_log.py
 -rw-r--r--  2.0 unx     5737 b- defN 23-Apr-05 05:40 tvault/parse_utils.py
 -rw-r--r--  2.0 unx    12413 b- defN 23-Apr-10 04:10 tvault/torchvault.py
--rw-r--r--  2.0 unx     1067 b- defN 23-Apr-10 04:10 tvault-0.2.7.dist-info/LICENSE
--rw-r--r--  2.0 unx      380 b- defN 23-Apr-10 04:10 tvault-0.2.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 04:10 tvault-0.2.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-10 04:10 tvault-0.2.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      760 b- defN 23-Apr-10 04:10 tvault-0.2.7.dist-info/RECORD
-10 files, 26529 bytes uncompressed, 7735 bytes compressed:  70.8%
+-rw-r--r--  2.0 unx     1067 b- defN 23-Apr-10 04:16 tvault-0.2.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx      380 b- defN 23-Apr-10 04:16 tvault-0.2.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 04:16 tvault-0.2.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-10 04:16 tvault-0.2.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      760 b- defN 23-Apr-10 04:16 tvault-0.2.8.dist-info/RECORD
+10 files, 26700 bytes uncompressed, 7791 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: tvault/parse_utils.py
 Comment: 
 
 Filename: tvault/torchvault.py
 Comment: 
 
-Filename: tvault-0.2.7.dist-info/LICENSE
+Filename: tvault-0.2.8.dist-info/LICENSE
 Comment: 
 
-Filename: tvault-0.2.7.dist-info/METADATA
+Filename: tvault-0.2.8.dist-info/METADATA
 Comment: 
 
-Filename: tvault-0.2.7.dist-info/WHEEL
+Filename: tvault-0.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: tvault-0.2.7.dist-info/top_level.txt
+Filename: tvault-0.2.8.dist-info/top_level.txt
 Comment: 
 
-Filename: tvault-0.2.7.dist-info/RECORD
+Filename: tvault-0.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tvault/__init__.py

```diff
@@ -17,17 +17,18 @@
 
 
 def log_optimizer(optimizer, log_dir="./model_log", model_dir="./"):
     vault = TorchVault(log_dir, model_dir)
     vault.log_optimizer(optimizer)
 
 
-def diff(sha1, sha2, log_dir="./model_log"):
+def diff(sha1="", index1=-1, sha2="", index2=-1, out=False, ask_gpt=False, log_dir="./model_log"):
+    # def diff(self, sha1="", index1=-1, sha2="", index2=-1, out=False, ask_gpt=False)
     vault = TorchVault(log_dir)
-    vault.diff(sha1, sha2)
+    vault.diff(sha1, index1, sha2, index2, out, ask_gpt)
 
 
 def add_tag(tag="", sha="", log_dir="./model_log"):
     vault = TorchVault(log_dir)
     vault.add_tag(sha, tag)
```

## Comparing `tvault-0.2.7.dist-info/LICENSE` & `tvault-0.2.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tvault-0.2.7.dist-info/RECORD` & `tvault-0.2.8.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-tvault/__init__.py,sha256=zbyjOOh-Y_ITUBJU3o0DdjvEjGVeIHjXDQpZ5OphLLQ,1284
+tvault/__init__.py,sha256=XV3fMuqbI9ErJxH59gLGAV-YlC5uYV_wdzQFLflMGoE,1455
 tvault/model_diff.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tvault/model_log.py,sha256=ZD1LeL1wBRKQEZaAfZEcjYP7w76yeD0eMRAnI-fBOiA,4789
 tvault/parse_utils.py,sha256=1gNwxk5UScEHIF_TG1te3r_gsYtFUaZTkWziLczvZ8I,5737
 tvault/torchvault.py,sha256=E88y2zTJKA9yAHE32vkOnf9IGrghqBasRcBe78aFOVI,12413
-tvault-0.2.7.dist-info/LICENSE,sha256=WMAFuHtOPuSTgn-WJtxM1LLEDLfqaKQes7X7VhOaaOU,1067
-tvault-0.2.7.dist-info/METADATA,sha256=976MvT9NhCoGRRYSUEZp9TN_GVSjSfS4xsMk-3FWJI8,380
-tvault-0.2.7.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-tvault-0.2.7.dist-info/top_level.txt,sha256=Z1ZnwpooKsyvyYmlAXuGVOIRK1hO7QkkDVaneY85JDI,7
-tvault-0.2.7.dist-info/RECORD,,
+tvault-0.2.8.dist-info/LICENSE,sha256=WMAFuHtOPuSTgn-WJtxM1LLEDLfqaKQes7X7VhOaaOU,1067
+tvault-0.2.8.dist-info/METADATA,sha256=srgiLBc_c4juJwtw72Rc0al0N9d4Jp_l6rct8cnu1Rc,380
+tvault-0.2.8.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+tvault-0.2.8.dist-info/top_level.txt,sha256=Z1ZnwpooKsyvyYmlAXuGVOIRK1hO7QkkDVaneY85JDI,7
+tvault-0.2.8.dist-info/RECORD,,
```

