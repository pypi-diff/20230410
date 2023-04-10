# Comparing `tmp/tvault-0.1.9-py3-none-any.whl.zip` & `tmp/tvault-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8708 bytes, number of entries: 10
--rw-r--r--  2.0 unx      923 b- defN 23-Apr-04 09:57 tvault/__init__.py
+Zip file size: 8968 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     1083 b- defN 23-Apr-10 01:10 tvault/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-03 04:19 tvault/model_diff.py
 -rw-r--r--  2.0 unx     4789 b- defN 23-Apr-03 06:15 tvault/model_log.py
--rw-r--r--  2.0 unx     5706 b- defN 23-Apr-05 05:02 tvault/parse_utils.py
--rw-r--r--  2.0 unx    11258 b- defN 23-Apr-05 05:34 tvault/torchvault.py
--rw-r--r--  2.0 unx     1067 b- defN 23-Apr-05 05:36 tvault-0.1.9.dist-info/LICENSE
--rw-r--r--  2.0 unx      353 b- defN 23-Apr-05 05:36 tvault-0.1.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-05 05:36 tvault-0.1.9.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-05 05:36 tvault-0.1.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      759 b- defN 23-Apr-05 05:36 tvault-0.1.9.dist-info/RECORD
-10 files, 24954 bytes uncompressed, 7422 bytes compressed:  70.3%
+-rw-r--r--  2.0 unx     5737 b- defN 23-Apr-05 05:40 tvault/parse_utils.py
+-rw-r--r--  2.0 unx    12480 b- defN 23-Apr-10 01:34 tvault/torchvault.py
+-rw-r--r--  2.0 unx     1067 b- defN 23-Apr-10 01:35 tvault-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      353 b- defN 23-Apr-10 01:35 tvault-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 01:35 tvault-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-10 01:35 tvault-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      760 b- defN 23-Apr-10 01:35 tvault-0.2.0.dist-info/RECORD
+10 files, 26368 bytes uncompressed, 7682 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: tvault/parse_utils.py
 Comment: 
 
 Filename: tvault/torchvault.py
 Comment: 
 
-Filename: tvault-0.1.9.dist-info/LICENSE
+Filename: tvault-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: tvault-0.1.9.dist-info/METADATA
+Filename: tvault-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: tvault-0.1.9.dist-info/WHEEL
+Filename: tvault-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: tvault-0.1.9.dist-info/top_level.txt
+Filename: tvault-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: tvault-0.1.9.dist-info/RECORD
+Filename: tvault-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tvault/__init__.py

```diff
@@ -1,13 +1,13 @@
 from .torchvault import TorchVault
 
 
 def log(model, log_dir="./model_log", model_dir="./"):
     vault = TorchVault(log_dir, model_dir)
-    vault.analyze_model(model)
+    vault.log_model(model)
 
 
 def log_scheduler(scheduler, log_dir="./model_log", model_dir="./"):
     vault = TorchVault(log_dir, model_dir)
     vault.log_scheduler(scheduler)
 
 
@@ -17,20 +17,27 @@
 
 
 def diff(sha1, sha2, log_dir="./model_log"):
     vault = TorchVault(log_dir)
     vault.diff(sha1, sha2)
 
 
-def ask_diff(sha1, sha2, log_dir="./model_log"):
-    vault = TorchVault(log_dir)
-    vault.ask_diff(sha1, sha2)
-
-
 def add_tag(tag="", sha="", log_dir="./model_log"):
     vault = TorchVault(log_dir)
     vault.add_tag(sha, tag)
 
 
 def add_result(result=0, sha="", log_dir="./model_log"):
     vault = TorchVault(log_dir)
     vault.add_result(sha, result)
+
+
+"""
+Logging everything all at once. Cannot specify commit hash
+"""
+
+
+def log_all(model, tag="", result=0, log_dir="./model_log", model_dir="./"):
+    vault = TorchVault(log_dir, model_dir)
+    vault.log_model(model)
+    vault.add_tag("", tag)
+    vault.add_result("", result)
```

## tvault/parse_utils.py

```diff
@@ -147,7 +147,9 @@
             func_diff_dict[p_func] = "function removed"
     for c_func, c_source in cur_model["external_func"].items():
         if c_func not in prev_model["external_func"].keys():
             func_diff_dict[c_func] = "function added"
     diff_dict["func"] = func_diff_dict
 
     ret_str = print_util(diff_dict)
+
+    return ret_str, diff_dict
```

## tvault/torchvault.py

```diff
@@ -1,15 +1,16 @@
 import os
 import sys
 import ast
 import git
 import json
 import openai
-import difflib
+import pickle
 import astunparse
+from prettytable import PrettyTable
 from collections import defaultdict
 
 from .parse_utils import match_external_funcs, extract_info_from_model, extract_diff
 
 OPENAI_API_KEY = "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"
 openai.api_key = OPENAI_API_KEY
 
@@ -36,109 +37,116 @@
     """
 
     def read_model_log(self, sha=""):
         if sha == "":
             sha = self.sha
 
         if os.path.exists(f"{self.log_dir}/model_{sha}"):
-            with open(f"{self.log_dir}/model_{sha}", "r") as f:
-                model_log = defaultdict(lambda: dict(), json.load(f))
+            with open(f"{self.log_dir}/model_{sha}", "rb") as f:
+                model_log = defaultdict(lambda: dict(), pickle.load(f))
         else:
             model_log = defaultdict(lambda: dict())
         return model_log
 
     """
     write model log to git hash
     """
 
     def write_model_log(self, sha="", model_log=defaultdict(lambda: dict())):
         if sha == "":
             sha = self.sha
-        model_json = json.dumps(dict(model_log), sort_keys=True, indent=4)
-        with open(f"{self.log_dir}/model_{sha}", "w") as f:
-            f.write(model_json)
+        with open(f"{self.log_dir}/model_{sha}", "wb") as f:
+            pickle.dump(dict(model_log), f)
 
     """
     log torch scheduler 
     """
 
     def log_scheduler(self, scheduler):
         model_log = self.read_model_log()
-        model_log["scheduler"] = scheduler.__str__()
+        model_idx = len(model_log.keys()) - 1
+        print(f"model idx - add scheduler: {model_idx}")
+        model_log[model_idx]["scheduler"] = scheduler.__str__()
         self.write_model_log("", model_log)
 
     """
     log torch optimizer
     """
 
     def log_optimizer(self, optimizer):
         model_log = self.read_model_log()
-        model_log["optimizer"] = optimizer.__str__()
+        model_idx = len(model_log.keys()) - 1
+        print(f"model idx - add optimizer: {model_idx}")
+        model_log[model_idx]["optimizer"] = optimizer.__str__()
         self.write_model_log("", model_log)
 
     """
     add tag to model log, commit sha may be from previous results.
     if idx is set to -1, all models in the commit hash are tagged.
     if idx is set to None, tag of most recent model is changed.
     """
 
     def add_tag(self, sha="", tag="", idx=None):
         # if commit hash is not given, use current commit hash
         model_log = self.read_model_log(sha)
+        print(f"add tag: got model_log {model_log}")
         if len(model_log.keys()) == 0:
             print(f"tvault error: model log with commit hash {sha} does not exist.")
             raise TorchVaultError
 
         if idx == -1:
             target_idxs = list(range(len(model_log.keys())))
         elif idx == None:
             target_idxs = [len(model_log.keys()) - 1]
+            print(f"add tags: {target_idxs}")
         else:
             target_idxs = [idx]
 
         for model_idx in target_idxs:
             if "tag" in model_log[model_idx].keys():
                 print(
                     f"tvault: changing tag from {model_log[model_idx]['tag']} to {tag} for model {sha}"
                 )
             else:
                 print(f"tvault: setting tag {tag} for model {sha}")
             model_log[model_idx]["tag"] = tag
-
+        print(f"write log: {model_log}")
         self.write_model_log(sha, model_log)
 
     """
     add result to model log, commit sha may be from previous results.
     if idx is set to -1, all models in the commit hash are tagged.
     if idx is set to None, tag of most recent model is changed.
     """
 
     def add_result(self, sha="", result=0, idx=None):
         # if commit hash is not given, use current commit hash
         model_log = self.read_model_log(sha)
+        print(f"add result: got model_log {model_log}")
         if len(model_log.keys()) == 0:
             print(f"tvault error: model log with commit hash {sha} does not exist.")
             raise TorchVaultError
 
         if idx == -1:
             target_idxs = list(range(len(model_log.keys())))
         elif idx == None:
             target_idxs = [len(model_log.keys()) - 1]
+            print(f"add results: {target_idxs}")
         else:
             target_idxs = [idx]
 
         for model_idx in target_idxs:
             if "result" in model_log[model_idx].keys():
                 print(
                     f"tvault: changing result from {model_log[model_idx]['result']} to {result} for model {sha}"
                 )
             else:
                 print(f"tvault: setting result {result} for model {sha}")
             model_log[model_idx]["result"] = result
-
+        print(f"write log: {model_log}")
         self.write_model_log(sha, model_log)
 
     """
     Basic logging for pytorch model.
     1. Retrives target modules from pytorch model representation.
     2. Get class definition of target modules.
     3. Get external function definition of those used in target model.
@@ -173,17 +181,19 @@
                 if self.use_astunparse:
                     filter_target_funcs[k] = astunparse.unparse(v)
                 else:
                     filter_target_funcs[k] = ast.unparse(v)
 
         model_log = self.read_model_log()
         model_idx = len(model_log.keys())
+        print(f"model idx: {model_idx}")
         model_log[model_idx]["model"] = model.__str__()
         model_log[model_idx]["src"] = dict(filter_target_class)
         model_log[model_idx]["external_func"] = dict(filter_target_funcs)
+        print(f"write model in model log {model_log}")
         self.write_model_log("", model_log)
 
     """
     Basic diff calculator between two pytorch models.
     sha1: commit hash of previous model, must be set. (for now)
     index1: model index of model in commit hash sha1. If not set, use latest.
     sha2: commit hash of current model, must be set. (for now)
@@ -200,16 +210,16 @@
         if len(cur_model.keys()) == 0:
             print(f"tvault error: sha2 argument must be provided.")
         if index1 == -1:
             index1 = len(prev_model.keys()) - 1
         if index2 == -1:
             index2 = len(cur_model.keys()) - 1
 
-        prev_model = prev_model[index1]
-        cur_model = cur_model[index2]
+        prev_model = prev_model[str(index1)]
+        cur_model = cur_model[str(index2)]
 
         ret_str, diff_dict = extract_diff(prev_model, cur_model)
 
         if out:
             with open(f"{self.log_dir}/diff_{sha1}_{sha2}", "w") as f:
                 f.write(ret_str)
         print(ret_str)
@@ -276,25 +286,41 @@
                         f"tvault: model {hash} exists! - contains {len(model_log.keys())} experiments"
                     )
                 else:
                     print(f"tvault: model {hash} does not exist.")
             elif condition == "tag":
                 target_models = []
                 for model in os.listdir(self.log_dir):
-                    with open(f"{self.log_dir}/{model}", "r") as f:
-                        model_log = json.load(f)
+                    with open(f"{self.log_dir}/{model}", "rb") as f:
+                        model_log = pickle.load(f)
                     for model_idx, v in model_log.items():
                         if "tag" in v.keys() and v["tag"] == tag:
                             target_models.append([model, model_idx])
                 print(f"tvault: models {target_models} match tag {tag}.")
             elif condition == "result":
                 target_models = []
                 for model in os.listdir(self.log_dir):
-                    with open(f"{self.log_dir}/{model}", "r") as f:
-                        model_log = json.load(f)
+                    with open(f"{self.log_dir}/{model}", "rb") as f:
+                        model_log = pickle.load(f)
                     for model_idx, v in model_log.items():
                         if "result" in v.keys() and min <= v["result"] <= max:
                             target_models.append([model, model_idx])
                 print(f"tvault: models {target_models} have result between {min} ~ {max}.")
             else:
                 print(f"tvault error:condition other than [hash, tag, result] is not supported.")
                 raise TorchVaultError
+
+    def show_result(self, sha=""):
+        model_log = self.read_model_log(sha)
+        print(f"add result: got model_log {model_log}")
+        if len(model_log.keys()) == 0:
+            print(f"tvault error: model log with commit hash {sha} is empty.")
+            raise TorchVaultError
+
+        target_idxs = list(range(len(model_log.keys())))
+        table = ["MODEL-IDX", "RESULT"]
+        tab = PrettyTable(table)
+        for i in range(target_idxs):
+            target_model = model_log[i]
+            if "result" in target_model.keys():
+                tab.add_rows([i, target_model["result"]])
+        print(tab)
```

## Comparing `tvault-0.1.9.dist-info/LICENSE` & `tvault-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tvault-0.1.9.dist-info/RECORD` & `tvault-0.2.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-tvault/__init__.py,sha256=SWHTddZeWPUwoWshUwqUx0UImLOAsA9mAdBtQu_G6SE,923
+tvault/__init__.py,sha256=qQofqVKUmfjL0KVEncNYBG55TlBk2ML03DA7c179D0E,1083
 tvault/model_diff.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tvault/model_log.py,sha256=ZD1LeL1wBRKQEZaAfZEcjYP7w76yeD0eMRAnI-fBOiA,4789
-tvault/parse_utils.py,sha256=EzV7xL66t4zQnNJ2C232VcR_ZgIrTiBvBNZ_C1nypnI,5706
-tvault/torchvault.py,sha256=vu1TlfS8W3fBolOtk2DkJ-nIN0YstgyxD4k1rMHU0kc,11258
-tvault-0.1.9.dist-info/LICENSE,sha256=WMAFuHtOPuSTgn-WJtxM1LLEDLfqaKQes7X7VhOaaOU,1067
-tvault-0.1.9.dist-info/METADATA,sha256=Y4YrDkc6rruKtEkpQs_w_d-4UNuNdcDUqucpwIirv-Q,353
-tvault-0.1.9.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-tvault-0.1.9.dist-info/top_level.txt,sha256=Z1ZnwpooKsyvyYmlAXuGVOIRK1hO7QkkDVaneY85JDI,7
-tvault-0.1.9.dist-info/RECORD,,
+tvault/parse_utils.py,sha256=1gNwxk5UScEHIF_TG1te3r_gsYtFUaZTkWziLczvZ8I,5737
+tvault/torchvault.py,sha256=y4IjNeiSMkmiOdQPOp3Ur8-b34g0MtFZ5i_yulTiJuI,12480
+tvault-0.2.0.dist-info/LICENSE,sha256=WMAFuHtOPuSTgn-WJtxM1LLEDLfqaKQes7X7VhOaaOU,1067
+tvault-0.2.0.dist-info/METADATA,sha256=U32xJie5P-Pkbet1dVtIAH7sgejW4PBve3BquGrgW3M,353
+tvault-0.2.0.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+tvault-0.2.0.dist-info/top_level.txt,sha256=Z1ZnwpooKsyvyYmlAXuGVOIRK1hO7QkkDVaneY85JDI,7
+tvault-0.2.0.dist-info/RECORD,,
```

