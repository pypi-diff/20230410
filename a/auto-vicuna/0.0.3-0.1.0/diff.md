# Comparing `tmp/auto_vicuna-0.0.3.tar.gz` & `tmp/auto_vicuna-0.1.0.tar.gz`

## Comparing `auto_vicuna-0.0.3.tar` & `auto_vicuna-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 auto_vicuna-0.0.3/.coveragerc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 auto_vicuna-0.0.3/.editorconfig
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 auto_vicuna-0.0.3/.flake8
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 auto_vicuna-0.0.3/.isort.cfg
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 auto_vicuna-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 auto_vicuna-0.0.3/.sourcery.yaml
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 auto_vicuna-0.0.3/clean_all.sh
--rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 auto_vicuna-0.0.3/pylintrc
--rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 auto_vicuna-0.0.3/qa.bat
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 auto_vicuna-0.0.3/qa.sh
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 auto_vicuna-0.0.3/requirements.txt
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 auto_vicuna-0.0.3/run_pylint.py
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 auto_vicuna-0.0.3/style.bat
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 auto_vicuna-0.0.3/style.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auto_vicuna-0.0.3/src/auto_vicuna/__init__.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 auto_vicuna-0.0.3/src/auto_vicuna/__main__.py
--rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 auto_vicuna-0.0.3/src/auto_vicuna/model.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 auto_vicuna-0.0.3/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 auto_vicuna-0.0.3/LICENSE
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 auto_vicuna-0.0.3/README.md
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 auto_vicuna-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 auto_vicuna-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 auto_vicuna-0.1.0/.coveragerc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 auto_vicuna-0.1.0/.editorconfig
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 auto_vicuna-0.1.0/.flake8
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 auto_vicuna-0.1.0/.isort.cfg
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 auto_vicuna-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 auto_vicuna-0.1.0/.sourcery.yaml
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 auto_vicuna-0.1.0/clean_all.sh
+-rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 auto_vicuna-0.1.0/pylintrc
+-rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 auto_vicuna-0.1.0/qa.bat
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 auto_vicuna-0.1.0/qa.sh
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 auto_vicuna-0.1.0/requirements.txt
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 auto_vicuna-0.1.0/run_pylint.py
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 auto_vicuna-0.1.0/style.bat
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 auto_vicuna-0.1.0/style.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auto_vicuna-0.1.0/src/auto_vicuna/__init__.py
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 auto_vicuna-0.1.0/src/auto_vicuna/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auto_vicuna-0.1.0/src/auto_vicuna/config.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 auto_vicuna-0.1.0/src/auto_vicuna/loop.py
+-rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 auto_vicuna-0.1.0/src/auto_vicuna/model.py
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 auto_vicuna-0.1.0/src/auto_vicuna/plugins.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 auto_vicuna-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 auto_vicuna-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 auto_vicuna-0.1.0/README.md
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 auto_vicuna-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 auto_vicuna-0.1.0/PKG-INFO
```

### Comparing `auto_vicuna-0.0.3/.coveragerc` & `auto_vicuna-0.1.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `auto_vicuna-0.0.3/.pre-commit-config.yaml` & `auto_vicuna-0.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `auto_vicuna-0.0.3/.sourcery.yaml` & `auto_vicuna-0.1.0/.sourcery.yaml`

 * *Files identical despite different names*

### Comparing `auto_vicuna-0.0.3/pylintrc` & `auto_vicuna-0.1.0/pylintrc`

 * *Files identical despite different names*

### Comparing `auto_vicuna-0.0.3/src/auto_vicuna/__main__.py` & `auto_vicuna-0.1.0/src/auto_vicuna/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from pathlib import Path
 
 import click
 import torch
 from dotenv import load_dotenv
 
 from auto_vicuna.model import load_model
+from auto_vicuna.loop import main_loop
+from auto_vicuna.plugins import load_plugins
 
 DEVICE = "cuda" if torch.cuda.is_available() else "cpu"
 load_dotenv()
 
 
 @click.command()
 @click.option(
@@ -21,30 +23,35 @@
     type=click.Path(exists=True),
     default=lambda: os.environ.get("VICUNA_WEIGHTS", ""),
 )
 @click.option("--num_gpus", type=int, default=1)
 @click.option("--device", type=str, default=DEVICE)
 @click.option("--debug", is_flag=True)
 @click.option("--load_8bit", is_flag=True)
+@click.option(
+    "--plugins_path", type=click.Path(exists=True),
+    default=lambda: os.environ.get("PLUGINS_PATH", Path(os.getcwd()) / "plugins")
+)
 def main(
     vicuna_weights: Path,
     num_gpus: int = 1,
     device: str = DEVICE,
     debug: bool = False,
     load_8bit: bool = False,
+    plugins_path: Path = Path(os.getcwd()) / "plugins",
 ) -> None:
     """Auto-Vicuna: A Python package for automatically generating Vicuna randomness."""
-    click.echo(f"Auto-Vicuna\n===========\nVersion: 0.0.1\nWeights: {vicuna_weights}")
+    click.echo(f"Auto-Vicuna\n===========\nVersion: 0.1.0\nWeights: {vicuna_weights}")
     click.echo(f"Device: {device}\nTorch version: {torch.__version__}")
     if "cpu" in torch.__version__:
         click.echo("\nError: CPU not supported. Install a GPU version of PyTorch.")
         click.echo("See https://pytorch.org/get-started/locally/ for more info.\n")
         sys.exit(1)
     try:
-        model = load_model(
+        model, tokenizer = load_model(
             vicuna_weights,
             device=device,
             num_gpus=num_gpus,
             debug=debug,
             load_8bit=load_8bit,
         )
     except ValueError as e:  # noqa: F841
@@ -59,13 +66,25 @@
             )
             sys.exit(1)
         click.echo(
             "Error: CPU not supported. Select a GPU device instead, e.g."
             " --device=cuda"
         )
         sys.exit(1)
+    plugins_found = load_plugins(plugins_path)
+    loaded_plugins = [plugin() for plugin in plugins_found]
+    if loaded_plugins:
+        click.echo(f"\nPlugins found: {len(loaded_plugins)}\n"
+                   "--------------------")
+    for plugin in loaded_plugins:
+        click.echo(f"{plugin._name}: {plugin._version} - {plugin._description}")
+
     if debug:
         click.echo(f"Model: {model}")
 
+    main_loop(model, tokenizer, "bair_v1", temperature=0.7,
+              max_new_tokens=512, plugins=loaded_plugins, debug=debug,
+              model_path=vicuna_weights)
+
 
 if __name__ == "__main__":
     main(sys.argv[1:])
```

### Comparing `auto_vicuna-0.0.3/src/auto_vicuna/model.py` & `auto_vicuna-0.1.0/src/auto_vicuna/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 import torch
 from fastchat.serve.compression import compress_module
 from fastchat.serve.monkey_patch_non_inplace import (
     replace_llama_attn_with_non_inplace_operations,
 )
 
 try:
-    # noqa: F401
     from transformers import (  # noqa: F401 pylint: disable=unused-import
         AutoModel,
         AutoModelForCausalLM,
         AutoTokenizer,
-        LlamaTokenizer,
+        LlamaTokenizer as Tokenizer
     )
 except ImportError:
     from transformers import (  # noqa: F401 pylint: disable=unused-import
         AutoModel,
         AutoModelForCausalLM,
         AutoTokenizer,
-        LLaMATokenizer,
+        LLaMATokenizer as Tokenizer
     )
 
 
 def load_model(model_name, device, num_gpus, load_8bit=False, debug=False):
     if device == "cpu":
         kwargs = {}
     elif device == "cuda":
```

### Comparing `auto_vicuna-0.0.3/.gitignore` & `auto_vicuna-0.1.0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 *.so
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
 dist/
+plugins/
 downloads/
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
```

### Comparing `auto_vicuna-0.0.3/LICENSE` & `auto_vicuna-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_vicuna-0.0.3/README.md` & `auto_vicuna-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `auto_vicuna-0.0.3/pyproject.toml` & `auto_vicuna-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "auto_vicuna"
-version = "0.0.3"
+version = "0.1.0"
 authors = [
   { name="Bill Schumacher", email="34168009+BillSchumacher@users.noreply.github.com" },
 ]
 description = "An experiment with Vicuna."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `auto_vicuna-0.0.3/PKG-INFO` & `auto_vicuna-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_vicuna
-Version: 0.0.3
+Version: 0.1.0
 Summary: An experiment with Vicuna.
 Project-URL: Homepage, https://github.com/BillSchumacher/Auto-Vicuna
 Project-URL: Bug Tracker, https://github.com/BillSchumacher/Auto-Vicuna/issues
 Author-email: Bill Schumacher <34168009+BillSchumacher@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

