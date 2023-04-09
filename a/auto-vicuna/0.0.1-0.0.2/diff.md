# Comparing `tmp/auto_vicuna-0.0.1.tar.gz` & `tmp/auto_vicuna-0.0.2.tar.gz`

## Comparing `auto_vicuna-0.0.1.tar` & `auto_vicuna-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 auto_vicuna-0.0.1/.coveragerc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 auto_vicuna-0.0.1/.editorconfig
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 auto_vicuna-0.0.1/.flake8
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 auto_vicuna-0.0.1/.isort.cfg
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 auto_vicuna-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 auto_vicuna-0.0.1/.sourcery.yaml
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 auto_vicuna-0.0.1/clean_all.sh
--rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 auto_vicuna-0.0.1/pylintrc
--rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 auto_vicuna-0.0.1/qa.bat
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 auto_vicuna-0.0.1/qa.sh
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 auto_vicuna-0.0.1/requirements.txt
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 auto_vicuna-0.0.1/run_pylint.py
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 auto_vicuna-0.0.1/style.bat
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 auto_vicuna-0.0.1/style.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auto_vicuna-0.0.1/src/auto_vicuna/__init__.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 auto_vicuna-0.0.1/src/auto_vicuna/__main__.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 auto_vicuna-0.0.1/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 auto_vicuna-0.0.1/LICENSE
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 auto_vicuna-0.0.1/README.md
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 auto_vicuna-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 auto_vicuna-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 auto_vicuna-0.0.2/.coveragerc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 auto_vicuna-0.0.2/.editorconfig
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 auto_vicuna-0.0.2/.flake8
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 auto_vicuna-0.0.2/.isort.cfg
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 auto_vicuna-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 auto_vicuna-0.0.2/.sourcery.yaml
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 auto_vicuna-0.0.2/clean_all.sh
+-rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 auto_vicuna-0.0.2/pylintrc
+-rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 auto_vicuna-0.0.2/qa.bat
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 auto_vicuna-0.0.2/qa.sh
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 auto_vicuna-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 auto_vicuna-0.0.2/run_pylint.py
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 auto_vicuna-0.0.2/style.bat
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 auto_vicuna-0.0.2/style.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auto_vicuna-0.0.2/src/auto_vicuna/__init__.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 auto_vicuna-0.0.2/src/auto_vicuna/__main__.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 auto_vicuna-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 auto_vicuna-0.0.2/LICENSE
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 auto_vicuna-0.0.2/README.md
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 auto_vicuna-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 auto_vicuna-0.0.2/PKG-INFO
```

### Comparing `auto_vicuna-0.0.1/.coveragerc` & `auto_vicuna-0.0.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `auto_vicuna-0.0.1/.pre-commit-config.yaml` & `auto_vicuna-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `auto_vicuna-0.0.1/.sourcery.yaml` & `auto_vicuna-0.0.2/.sourcery.yaml`

 * *Files identical despite different names*

### Comparing `auto_vicuna-0.0.1/pylintrc` & `auto_vicuna-0.0.2/pylintrc`

 * *Files identical despite different names*

### Comparing `auto_vicuna-0.0.1/.gitignore` & `auto_vicuna-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `auto_vicuna-0.0.1/LICENSE` & `auto_vicuna-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_vicuna-0.0.1/pyproject.toml` & `auto_vicuna-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "auto_vicuna"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Bill Schumacher", email="34168009+BillSchumacher@users.noreply.github.com" },
 ]
 description = "An experiment with Vicuna."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "click", "tqdm", "python-dotenv", "fschat", "torch", "redis", "orjson"
+  "click", "tqdm", "python-dotenv", "fschat", "torch", "redis", "orjson",
+  "fschat", "transformers"
 ]
+
 [project.urls]
 "Homepage" = "https://github.com/BillSchumacher/Auto-Vicuna"
 "Bug Tracker" = "https://github.com/BillSchumacher/Auto-Vicuna/issues"
 
 [project.scripts]
 auto_vicuna = "auto_vicuna.__main__:main"
 
+[tool.hatch.metadata]
+allow-direct-references = true
+
 [tool.hatch.build.targets.wheel.force-include]
 "bin/auto_vicuna.py" = "auto_vicuna/__main__.py"
 
 [tool.black]
 line-length = 88
 target-version = ['py310']
 include = '\.pyi?$'
```

### Comparing `auto_vicuna-0.0.1/PKG-INFO` & `auto_vicuna-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_vicuna
-Version: 0.0.1
+Version: 0.0.2
 Summary: An experiment with Vicuna.
 Project-URL: Homepage, https://github.com/BillSchumacher/Auto-Vicuna
 Project-URL: Bug Tracker, https://github.com/BillSchumacher/Auto-Vicuna/issues
 Author-email: Bill Schumacher <34168009+BillSchumacher@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,10 +13,11 @@
 Requires-Dist: click
 Requires-Dist: fschat
 Requires-Dist: orjson
 Requires-Dist: python-dotenv
 Requires-Dist: redis
 Requires-Dist: torch
 Requires-Dist: tqdm
+Requires-Dist: transformers
 Description-Content-Type: text/markdown
 
 # Auto-Vicuna
```

