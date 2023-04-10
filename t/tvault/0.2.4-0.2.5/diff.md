# Comparing `tmp/tvault-0.2.4-py3-none-any.whl.zip` & `tmp/tvault-0.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9044 bytes, number of entries: 10
+Zip file size: 9042 bytes, number of entries: 10
 -rw-r--r--  2.0 unx     1284 b- defN 23-Apr-10 03:52 tvault/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-03 04:19 tvault/model_diff.py
 -rw-r--r--  2.0 unx     4789 b- defN 23-Apr-03 06:15 tvault/model_log.py
 -rw-r--r--  2.0 unx     5737 b- defN 23-Apr-05 05:40 tvault/parse_utils.py
--rw-r--r--  2.0 unx    12467 b- defN 23-Apr-10 03:57 tvault/torchvault.py
--rw-r--r--  2.0 unx     1067 b- defN 23-Apr-10 03:57 tvault-0.2.4.dist-info/LICENSE
--rw-r--r--  2.0 unx      380 b- defN 23-Apr-10 03:57 tvault-0.2.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 03:57 tvault-0.2.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-10 03:57 tvault-0.2.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      760 b- defN 23-Apr-10 03:57 tvault-0.2.4.dist-info/RECORD
-10 files, 26583 bytes uncompressed, 7758 bytes compressed:  70.8%
+-rw-r--r--  2.0 unx    12460 b- defN 23-Apr-10 04:04 tvault/torchvault.py
+-rw-r--r--  2.0 unx     1067 b- defN 23-Apr-10 04:04 tvault-0.2.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx      380 b- defN 23-Apr-10 04:04 tvault-0.2.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 04:04 tvault-0.2.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-10 04:04 tvault-0.2.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      760 b- defN 23-Apr-10 04:04 tvault-0.2.5.dist-info/RECORD
+10 files, 26576 bytes uncompressed, 7756 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: tvault/parse_utils.py
 Comment: 
 
 Filename: tvault/torchvault.py
 Comment: 
 
-Filename: tvault-0.2.4.dist-info/LICENSE
+Filename: tvault-0.2.5.dist-info/LICENSE
 Comment: 
 
-Filename: tvault-0.2.4.dist-info/METADATA
+Filename: tvault-0.2.5.dist-info/METADATA
 Comment: 
 
-Filename: tvault-0.2.4.dist-info/WHEEL
+Filename: tvault-0.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: tvault-0.2.4.dist-info/top_level.txt
+Filename: tvault-0.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: tvault-0.2.4.dist-info/RECORD
+Filename: tvault-0.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tvault/torchvault.py

```diff
@@ -317,12 +317,12 @@
 
         import ipdb
 
         ipdb.set_trace()
         target_idxs = [*range(len(model_log.keys()))]
         table = ["MODEL-IDX", "RESULT"]
         tab = PrettyTable(table)
-        for i in range(target_idxs):
+        for i in target_idxs:
             target_model = model_log[i]
             if "result" in target_model.keys():
                 tab.add_rows([i, target_model["result"]])
         print(tab)
```

## Comparing `tvault-0.2.4.dist-info/LICENSE` & `tvault-0.2.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tvault-0.2.4.dist-info/RECORD` & `tvault-0.2.5.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 tvault/__init__.py,sha256=zbyjOOh-Y_ITUBJU3o0DdjvEjGVeIHjXDQpZ5OphLLQ,1284
 tvault/model_diff.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tvault/model_log.py,sha256=ZD1LeL1wBRKQEZaAfZEcjYP7w76yeD0eMRAnI-fBOiA,4789
 tvault/parse_utils.py,sha256=1gNwxk5UScEHIF_TG1te3r_gsYtFUaZTkWziLczvZ8I,5737
-tvault/torchvault.py,sha256=Ek4Bm1fPoAQOVBKveOf9s0GTX-OyGStXJaAqngVf4Iw,12467
-tvault-0.2.4.dist-info/LICENSE,sha256=WMAFuHtOPuSTgn-WJtxM1LLEDLfqaKQes7X7VhOaaOU,1067
-tvault-0.2.4.dist-info/METADATA,sha256=VLozwYpNCbMhfZCdKnfl2pVn7SbQiCdxM_sKdly67fs,380
-tvault-0.2.4.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-tvault-0.2.4.dist-info/top_level.txt,sha256=Z1ZnwpooKsyvyYmlAXuGVOIRK1hO7QkkDVaneY85JDI,7
-tvault-0.2.4.dist-info/RECORD,,
+tvault/torchvault.py,sha256=iaGusBjI_1o8p698EG1Q-EtROn0P02VPa4MIAZrVKNA,12460
+tvault-0.2.5.dist-info/LICENSE,sha256=WMAFuHtOPuSTgn-WJtxM1LLEDLfqaKQes7X7VhOaaOU,1067
+tvault-0.2.5.dist-info/METADATA,sha256=gejBISf5GgYX0PORhTT3nMNf1dUTDGwRiVaAX5J1GIs,380
+tvault-0.2.5.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+tvault-0.2.5.dist-info/top_level.txt,sha256=Z1ZnwpooKsyvyYmlAXuGVOIRK1hO7QkkDVaneY85JDI,7
+tvault-0.2.5.dist-info/RECORD,,
```

