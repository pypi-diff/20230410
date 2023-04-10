# Comparing `tmp/tvmer-0.1.5.dev2.tar.gz` & `tmp/tvmer-0.1.5.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvmer-0.1.5.dev2.tar", last modified: Sun Apr  2 09:18:21 2023, max compression
+gzip compressed data, was "tvmer-0.1.5.dev3.tar", last modified: Mon Apr 10 09:25:19 2023, max compression
```

## Comparing `tvmer-0.1.5.dev2.tar` & `tvmer-0.1.5.dev3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      193 2023-04-02 09:18:09.118254 tvmer-0.1.5.dev2/README.md
--rw-r--r--   0        0        0      464 2023-04-02 09:18:09.122254 tvmer-0.1.5.dev2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-02 09:18:09.122254 tvmer-0.1.5.dev2/tvmer/__init__.py
--rw-r--r--   0        0        0     4169 2023-04-02 09:18:09.122254 tvmer-0.1.5.dev2/tvmer/__main__.py
--rw-r--r--   0        0        0     5021 2023-04-02 09:18:09.122254 tvmer-0.1.5.dev2/tvmer/utils.py
--rw-r--r--   0        0        0      386 1970-01-01 00:00:00.000000 tvmer-0.1.5.dev2/PKG-INFO
+-rw-r--r--   0        0        0      193 2023-04-10 09:25:10.660720 tvmer-0.1.5.dev3/README.md
+-rw-r--r--   0        0        0      464 2023-04-10 09:25:10.660720 tvmer-0.1.5.dev3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 09:25:10.660720 tvmer-0.1.5.dev3/tvmer/__init__.py
+-rw-r--r--   0        0        0     4954 2023-04-10 09:25:10.660720 tvmer-0.1.5.dev3/tvmer/__main__.py
+-rw-r--r--   0        0        0     5035 2023-04-10 09:25:10.660720 tvmer-0.1.5.dev3/tvmer/utils.py
+-rw-r--r--   0        0        0      386 1970-01-01 00:00:00.000000 tvmer-0.1.5.dev3/PKG-INFO
```

### Comparing `tvmer-0.1.5.dev2/tvmer/__main__.py` & `tvmer-0.1.5.dev3/tvmer/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from __future__ import annotations
 
 import os
-
 import tvm
 from tvm.contrib.graph_executor import GraphModule
 import numpy as np
 import typer
 import rich
 from rich.progress import Progress, ProgressBar
 from pathlib import Path
 from tvm import auto_scheduler
 from tvm import autotvm
+from typing import List
 
 from tvmer.utils import load_onnx, gen_library, load_module, TunerStr
 import tvmer.utils as utils
 
 app = typer.Typer(rich_markup_mode="rich")
 
 
 @app.command()
-def run(lib_path: Path, dev: str, repeat: int = 10):
+def run(lib_path: Path, data_path: Path, dev: str = "cpu"):
     """
     run a compiled module
     """
     dev = tvm.device(dev)
     module = load_module(lib_path, dev)
     ftimer = module.module.time_evaluator("run", dev, number=10, repeat=repeat)
     prof_res = np.array(ftimer().results) * 1000
@@ -33,28 +33,45 @@
     # print(module.inp())
     # print(module.get_input_info())
     # module.set_input("479", np.zeros([1, 64, 8400]))
     # module.set_input("p1", np.zeros([1, 2, 8400]))
 
 
 @app.command()
+def test(lib_paths: List[Path], dev: str = "cpu", repeat: int = 10):
+    """
+    test a compiled module or some compiled modules
+    """
+    dev = tvm.device(dev)
+    for lib_path in lib_paths:
+        module = load_module(lib_path, dev)
+        ftimer = module.module.time_evaluator("run", dev, number=10, repeat=repeat)
+        prof_res = np.array(ftimer().results) * 1000
+        rich.print(
+            f"mean: {np.mean(prof_res):.2f} ms, std: {np.std(prof_res):.2f} ms"
+        )
+
+
+@app.command()
 def compile(
         model_path: Path,
         target: str = "llvm",
         target_host: str = None,
-        export_path: Path = ".tvmer/lib/default.so",
+        export_path: Path = None,
         dtype="float32"
 ):
     """
     compile a model
     """
-    target = tvm.target.Target(target, host=target_host)
+    if export_path is None:
+        export_path = f".tvmer/lib/{target}_{target_host}_{os.path.basename(model_path)}.so"
 
+    target = tvm.target.Target(target, host=target_host)
     mod, params = load_onnx(path=model_path, batch_size=1, dtype=dtype)
-    graph_json, lib, params = gen_library(mod, params, target, export_path)
+    lib = gen_library(mod, params, target, export_path).get_lib()
 
     if not os.path.exists(".tvmer/source"):
         os.makedirs(".tvmer/source")
     for i, imported_module in enumerate(lib.imported_modules):
         with open(f".tvmer/source/imported_module{i}.dev", mode="w") as f:
             f.write(imported_module.get_source())
     with open(".tvmer/source/module.host", mode="w") as f:
@@ -62,22 +79,25 @@
 
 
 @app.command()
 def tune(
         model_path: Path,
         target: str = "llvm",
         target_host: str = None,
-        export_path: Path = ".tvmer/lib/tuned_default.so",
+        export_path: Path = None,
         dtype="float32",
         num_measure_trials: int = 200,
         tuner: TunerStr = None,
 ):
     """
     auto-tune a model
     """
+    if export_path is None:
+        prefix = f"tuned_{tuner}" if tuner else "tuned"
+        export_path = f".tvmer/lib/{prefix}_{target}_{target_host}_{os.path.basename(model_path)}.so"
     target = tvm.target.Target(target, host=target_host)
 
     print("Extract tasks...")
     mod, params = load_onnx(path=model_path, batch_size=1, dtype=dtype)
     if tuner is None:
         utils.tune(mod, params, target, num_measure_trials)
         gen_library(mod, params, target, export_path)
```

### Comparing `tvmer-0.1.5.dev2/tvmer/utils.py` & `tvmer-0.1.5.dev3/tvmer/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 if TYPE_CHECKING:
     Path = Union[Path, str]
 
 
 class TunerStr(str, Enum):
     xgb = "xgb"
+    ga = "ga"
     random = "random"
     gridsearch = "gridsearch"
 
 
 def str2tuner(tuner_str: TunerStr, task):
     if tuner_str == TunerStr.xgb:
         tuner = autotvm.tuner.XGBTuner(task, loss_type="rank")
```

