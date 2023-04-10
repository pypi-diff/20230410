# Comparing `tmp/tvault-0.2.5-py3-none-any.whl.zip` & `tmp/tvault-0.2.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9042 bytes, number of entries: 10
+Zip file size: 9021 bytes, number of entries: 10
 -rw-r--r--  2.0 unx     1284 b- defN 23-Apr-10 03:52 tvault/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-03 04:19 tvault/model_diff.py
 -rw-r--r--  2.0 unx     4789 b- defN 23-Apr-03 06:15 tvault/model_log.py
 -rw-r--r--  2.0 unx     5737 b- defN 23-Apr-05 05:40 tvault/parse_utils.py
--rw-r--r--  2.0 unx    12460 b- defN 23-Apr-10 04:04 tvault/torchvault.py
--rw-r--r--  2.0 unx     1067 b- defN 23-Apr-10 04:04 tvault-0.2.5.dist-info/LICENSE
--rw-r--r--  2.0 unx      380 b- defN 23-Apr-10 04:04 tvault-0.2.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 04:04 tvault-0.2.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-10 04:04 tvault-0.2.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      760 b- defN 23-Apr-10 04:04 tvault-0.2.5.dist-info/RECORD
-10 files, 26576 bytes uncompressed, 7756 bytes compressed:  70.8%
+-rw-r--r--  2.0 unx    12413 b- defN 23-Apr-10 04:10 tvault/torchvault.py
+-rw-r--r--  2.0 unx     1067 b- defN 23-Apr-10 04:10 tvault-0.2.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx      380 b- defN 23-Apr-10 04:10 tvault-0.2.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 04:10 tvault-0.2.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-10 04:10 tvault-0.2.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      760 b- defN 23-Apr-10 04:10 tvault-0.2.7.dist-info/RECORD
+10 files, 26529 bytes uncompressed, 7735 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: tvault/parse_utils.py
 Comment: 
 
 Filename: tvault/torchvault.py
 Comment: 
 
-Filename: tvault-0.2.5.dist-info/LICENSE
+Filename: tvault-0.2.7.dist-info/LICENSE
 Comment: 
 
-Filename: tvault-0.2.5.dist-info/METADATA
+Filename: tvault-0.2.7.dist-info/METADATA
 Comment: 
 
-Filename: tvault-0.2.5.dist-info/WHEEL
+Filename: tvault-0.2.7.dist-info/WHEEL
 Comment: 
 
-Filename: tvault-0.2.5.dist-info/top_level.txt
+Filename: tvault-0.2.7.dist-info/top_level.txt
 Comment: 
 
-Filename: tvault-0.2.5.dist-info/RECORD
+Filename: tvault-0.2.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tvault/torchvault.py

```diff
@@ -311,18 +311,15 @@
 
     def show_result(self, sha=""):
         model_log = self.read_model_log(sha)
         if len(model_log.keys()) == 0:
             print(f"tvault error: model log with commit hash {sha} is empty.")
             raise TorchVaultError
 
-        import ipdb
-
-        ipdb.set_trace()
         target_idxs = [*range(len(model_log.keys()))]
         table = ["MODEL-IDX", "RESULT"]
         tab = PrettyTable(table)
         for i in target_idxs:
             target_model = model_log[i]
             if "result" in target_model.keys():
-                tab.add_rows([i, target_model["result"]])
+                tab.add_row([i, target_model["result"]])
         print(tab)
```

## Comparing `tvault-0.2.5.dist-info/LICENSE` & `tvault-0.2.7.dist-info/LICENSE`

 * *Files identical despite different names*

