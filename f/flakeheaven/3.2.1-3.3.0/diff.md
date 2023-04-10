# Comparing `tmp/flakeheaven-3.2.1.tar.gz` & `tmp/flakeheaven-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flakeheaven-3.2.1.tar", max compression
+gzip compressed data, was "flakeheaven-3.3.0.tar", max compression
```

## Comparing `flakeheaven-3.2.1.tar` & `flakeheaven-3.3.0.tar`

### file list

```diff
@@ -1,51 +1,50 @@
--rw-r--r--   0        0        0     1080 2022-11-04 12:06:37.219746 flakeheaven-3.2.1/LICENSE
--rw-r--r--   0        0        0     5837 2022-11-04 12:06:37.219746 flakeheaven-3.2.1/README.md
--rw-r--r--   0        0        0      207 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/__init__.py
--rw-r--r--   0        0        0       50 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/__main__.py
--rw-r--r--   0        0        0     1569 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/_cli.py
--rw-r--r--   0        0        0     5132 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/_constants.py
--rw-r--r--   0        0        0      592 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/_logic/__init__.py
--rw-r--r--   0        0        0      334 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/_logic/_baseline.py
--rw-r--r--   0        0        0     1862 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/_logic/_colors.py
--rw-r--r--   0        0        0     2401 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/_logic/_config.py
--rw-r--r--   0        0        0     2821 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/_logic/_discover.py
--rw-r--r--   0        0        0    13019 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/_logic/_extractors.py
--rw-r--r--   0        0        0     4757 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/_logic/_plugin.py
--rw-r--r--   0        0        0     3417 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/_logic/_snapshot.py
--rw-r--r--   0        0        0       86 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/_patched/__init__.py
--rw-r--r--   0        0        0    10087 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/_patched/_app.py
--rw-r--r--   0        0        0    12181 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/_patched/_checkers.py
--rw-r--r--   0        0        0     1908 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/_patched/_plugins.py
--rw-r--r--   0        0        0      508 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/_patched/_processor.py
--rw-r--r--   0        0        0     2967 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/_patched/_style_guide.py
--rw-r--r--   0        0        0      754 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/_patched/_violation.py
--rw-r--r--   0        0        0      134 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/_types.py
--rw-r--r--   0        0        0      259 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/_version.py
--rw-r--r--   0        0        0      822 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/commands/__init__.py
--rw-r--r--   0        0        0      702 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/commands/_baseline.py
--rw-r--r--   0        0        0     1848 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/commands/_code.py
--rw-r--r--   0        0        0     1194 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/commands/_codes.py
--rw-r--r--   0        0        0     3898 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/commands/_config.py
--rw-r--r--   0        0        0      436 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/commands/_lint.py
--rw-r--r--   0        0        0      809 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/commands/_missed.py
--rw-r--r--   0        0        0     2081 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/commands/_plugins.py
--rw-r--r--   0        0        0      537 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/commands/_version.py
--rw-r--r--   0        0        0      419 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/formatters/__init__.py
--rw-r--r--   0        0        0      423 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/formatters/_baseline.py
--rw-r--r--   0        0        0     1948 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/formatters/_colored.py
--rw-r--r--   0        0        0     1357 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/formatters/_gitlab.py
--rw-r--r--   0        0        0     3710 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/formatters/_grouped.py
--rw-r--r--   0        0        0      564 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/formatters/_json.py
--rw-r--r--   0        0        0     1258 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/formatters/_stat.py
--rw-r--r--   0        0        0      672 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/parsers/__init__.py
--rw-r--r--   0        0        0      289 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/parsers/_base.py
--rw-r--r--   0        0        0      655 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/parsers/_jupyter.py
--rw-r--r--   0        0        0     2755 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/parsers/_markdown.py
--rw-r--r--   0        0        0      444 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/parsers/_python.py
--rw-r--r--   0        0        0     2733 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/parsers/_rst.py
--rw-r--r--   0        0        0     1891 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/parsers/_yaml.py
--rw-r--r--   0        0        0      238 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/plugins/__init__.py
--rw-r--r--   0        0        0     1416 2022-11-04 12:06:37.227746 flakeheaven-3.2.1/flakeheaven/plugins/_pylint.py
--rw-r--r--   0        0        0     4391 2022-11-04 12:06:37.231746 flakeheaven-3.2.1/pyproject.toml
--rw-r--r--   0        0        0     7814 1970-01-01 00:00:00.000000 flakeheaven-3.2.1/setup.py
--rw-r--r--   0        0        0     7639 1970-01-01 00:00:00.000000 flakeheaven-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-04-10 21:35:49.037616 flakeheaven-3.3.0/LICENSE
+-rw-r--r--   0        0        0     5840 2023-04-10 21:35:49.037616 flakeheaven-3.3.0/README.md
+-rw-r--r--   0        0        0      207 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/__init__.py
+-rw-r--r--   0        0        0       50 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/__main__.py
+-rw-r--r--   0        0        0     1569 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/_cli.py
+-rw-r--r--   0        0        0     5132 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/_constants.py
+-rw-r--r--   0        0        0      592 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/_logic/__init__.py
+-rw-r--r--   0        0        0      334 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/_logic/_baseline.py
+-rw-r--r--   0        0        0     1862 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/_logic/_colors.py
+-rw-r--r--   0        0        0     2401 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/_logic/_config.py
+-rw-r--r--   0        0        0     2821 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/_logic/_discover.py
+-rw-r--r--   0        0        0    13019 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/_logic/_extractors.py
+-rw-r--r--   0        0        0     4757 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/_logic/_plugin.py
+-rw-r--r--   0        0        0     3483 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/_logic/_snapshot.py
+-rw-r--r--   0        0        0       86 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/_patched/__init__.py
+-rw-r--r--   0        0        0    10087 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/_patched/_app.py
+-rw-r--r--   0        0        0    12181 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/_patched/_checkers.py
+-rw-r--r--   0        0        0     1908 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/_patched/_plugins.py
+-rw-r--r--   0        0        0      508 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/_patched/_processor.py
+-rw-r--r--   0        0        0     2967 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/_patched/_style_guide.py
+-rw-r--r--   0        0        0      754 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/_patched/_violation.py
+-rw-r--r--   0        0        0      134 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/_types.py
+-rw-r--r--   0        0        0      259 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/_version.py
+-rw-r--r--   0        0        0      822 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/commands/__init__.py
+-rw-r--r--   0        0        0      702 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/commands/_baseline.py
+-rw-r--r--   0        0        0     1848 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/commands/_code.py
+-rw-r--r--   0        0        0     1194 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/commands/_codes.py
+-rw-r--r--   0        0        0     3898 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/commands/_config.py
+-rw-r--r--   0        0        0      436 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/commands/_lint.py
+-rw-r--r--   0        0        0      809 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/commands/_missed.py
+-rw-r--r--   0        0        0     2081 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/commands/_plugins.py
+-rw-r--r--   0        0        0      537 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/commands/_version.py
+-rw-r--r--   0        0        0      419 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/formatters/__init__.py
+-rw-r--r--   0        0        0      423 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/formatters/_baseline.py
+-rw-r--r--   0        0        0     1948 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/formatters/_colored.py
+-rw-r--r--   0        0        0     1357 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/formatters/_gitlab.py
+-rw-r--r--   0        0        0     3710 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/formatters/_grouped.py
+-rw-r--r--   0        0        0      564 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/formatters/_json.py
+-rw-r--r--   0        0        0     1258 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/formatters/_stat.py
+-rw-r--r--   0        0        0      672 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/parsers/__init__.py
+-rw-r--r--   0        0        0      289 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/parsers/_base.py
+-rw-r--r--   0        0        0      655 2023-04-10 21:35:49.045616 flakeheaven-3.3.0/flakeheaven/parsers/_jupyter.py
+-rw-r--r--   0        0        0     2755 2023-04-10 21:35:49.049616 flakeheaven-3.3.0/flakeheaven/parsers/_markdown.py
+-rw-r--r--   0        0        0      444 2023-04-10 21:35:49.049616 flakeheaven-3.3.0/flakeheaven/parsers/_python.py
+-rw-r--r--   0        0        0     2733 2023-04-10 21:35:49.049616 flakeheaven-3.3.0/flakeheaven/parsers/_rst.py
+-rw-r--r--   0        0        0     1891 2023-04-10 21:35:49.049616 flakeheaven-3.3.0/flakeheaven/parsers/_yaml.py
+-rw-r--r--   0        0        0      238 2023-04-10 21:35:49.049616 flakeheaven-3.3.0/flakeheaven/plugins/__init__.py
+-rw-r--r--   0        0        0     1416 2023-04-10 21:35:49.049616 flakeheaven-3.3.0/flakeheaven/plugins/_pylint.py
+-rw-r--r--   0        0        0     4391 2023-04-10 21:35:49.049616 flakeheaven-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7647 1970-01-01 00:00:00.000000 flakeheaven-3.3.0/PKG-INFO
```

### Comparing `flakeheaven-3.2.1/LICENSE` & `flakeheaven-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/README.md` & `flakeheaven-3.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     + [Show all messages and codes for a plugin](https://flakeheaven.readthedocs.io/en/latest/commands/codes.html).
     + Allow codes intersection for different plugins.
 
 ![output example](./assets/grouped.png)
 
 ## Compatibility
 
-FlakeHeaven supports all flake8 plugins, formatters, and configs. However, FlakeHeaven has it's own beautiful way to configure enabled plugins and codes. So, options like `--ignore` and `--select` unsupported. You can have flake8 and FlakeHeaven in one project if you want but enabled plugins should be explicitly specified.
+FlakeHeaven supports all flake8 plugins, formatters, and configs. However, FlakeHeaven has its own beautiful way to configure enabled plugins and codes. So, options like `--ignore` and `--select` are unsupported. You can have flake8 and FlakeHeaven in one project if you want but enabled plugins should be explicitly specified.
 
 ## Installation
 
 ```bash
 python3 -m pip install --user flakeheaven
 ```
 
@@ -108,18 +108,18 @@
 This command accepts all the same arguments as Flake8.
 
 Read [the documentation](https://flakeheaven.readthedocs.io/en/latest/) for more information.
 
 ## Contributing
 
 1. Add tests when possible (eg for features / fixes / refactor, etc. )
-2. add your contribution to the code / docs
-3. Ensure your code passes all (both oririnal and your own) tests.
-4. commit using [proper header](https://www.conventionalcommits.org/en/v1.0.0/)
-5. create a PR
+2. Add your contribution to the code / docs
+3. Ensure your code passes all (both original and your own) tests.
+4. Commit using [proper header](https://www.conventionalcommits.org/en/v1.0.0/)
+5. Create a PR
 
 Contributions are welcome! A few ideas where you can contribute:
 
 + Improve documentation.
 + Add more tests.
 + Improve performance.
 + Found a bug? Fix it!
```

### Comparing `flakeheaven-3.2.1/flakeheaven/_cli.py` & `flakeheaven-3.3.0/flakeheaven/_cli.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/_constants.py` & `flakeheaven-3.3.0/flakeheaven/_constants.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/_logic/__init__.py` & `flakeheaven-3.3.0/flakeheaven/_logic/__init__.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/_logic/_colors.py` & `flakeheaven-3.3.0/flakeheaven/_logic/_colors.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/_logic/_config.py` & `flakeheaven-3.3.0/flakeheaven/_logic/_config.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/_logic/_discover.py` & `flakeheaven-3.3.0/flakeheaven/_logic/_discover.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/_logic/_extractors.py` & `flakeheaven-3.3.0/flakeheaven/_logic/_extractors.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/_logic/_plugin.py` & `flakeheaven-3.3.0/flakeheaven/_logic/_plugin.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/_logic/_snapshot.py` & `flakeheaven-3.3.0/flakeheaven/_logic/_snapshot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 # built-in
+import contextlib
 import json
 import os
+from datetime import timedelta
 from hashlib import md5
 from pathlib import Path
 from time import time
 from typing import Optional
 
 # external
 from flake8.checker import FileChecker
 from flake8.options.manager import OptionManager
 
 
 CACHE_PATH = Path(
-    os.environ.get('FLAKEHEAVEN_CACHE', Path.home() / '.cache/flakeheaven'),
+    os.environ.get('FLAKEHEAVEN_CACHE', Path().resolve() / '.flakeheaven_cache'),
 )
 
-THRESHOLD = int(os.getenv('FLAKEHEAVEN_CACHE_TIMEOUT', 3600 * 24))  # default is 1 day
+THRESHOLD = int(os.getenv('FLAKEHEAVEN_CACHE_TIMEOUT', timedelta(days=1).total_seconds()))
 
 
 def prepare_cache(path=CACHE_PATH):
     if not path.exists():
         path.mkdir(parents=True, exist_ok=True)
         return
+
+    _time = time()
     for fpath in path.iterdir():
-        try:
-            if time() - fpath.stat().st_atime <= THRESHOLD:
+        with contextlib.suppress(FileNotFoundError):
+            if _time - fpath.stat().st_atime <= THRESHOLD:
                 continue
             fpath.unlink()
-        except FileNotFoundError:
-            pass
 
 
 class Snapshot:
     _exists: Optional[bool] = None
     _digest: Optional[str] = None
     _results = None
```

### Comparing `flakeheaven-3.2.1/flakeheaven/_patched/_app.py` & `flakeheaven-3.3.0/flakeheaven/_patched/_app.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/_patched/_checkers.py` & `flakeheaven-3.3.0/flakeheaven/_patched/_checkers.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/_patched/_plugins.py` & `flakeheaven-3.3.0/flakeheaven/_patched/_plugins.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/_patched/_style_guide.py` & `flakeheaven-3.3.0/flakeheaven/_patched/_style_guide.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/_patched/_violation.py` & `flakeheaven-3.3.0/flakeheaven/_patched/_violation.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/commands/__init__.py` & `flakeheaven-3.3.0/flakeheaven/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/commands/_baseline.py` & `flakeheaven-3.3.0/flakeheaven/commands/_baseline.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/commands/_code.py` & `flakeheaven-3.3.0/flakeheaven/commands/_code.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/commands/_codes.py` & `flakeheaven-3.3.0/flakeheaven/commands/_codes.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/commands/_config.py` & `flakeheaven-3.3.0/flakeheaven/commands/_config.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/commands/_missed.py` & `flakeheaven-3.3.0/flakeheaven/commands/_missed.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/commands/_plugins.py` & `flakeheaven-3.3.0/flakeheaven/commands/_plugins.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/commands/_version.py` & `flakeheaven-3.3.0/flakeheaven/commands/_version.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/formatters/_colored.py` & `flakeheaven-3.3.0/flakeheaven/formatters/_colored.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/formatters/_gitlab.py` & `flakeheaven-3.3.0/flakeheaven/formatters/_gitlab.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/formatters/_grouped.py` & `flakeheaven-3.3.0/flakeheaven/formatters/_grouped.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/formatters/_json.py` & `flakeheaven-3.3.0/flakeheaven/formatters/_json.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/formatters/_stat.py` & `flakeheaven-3.3.0/flakeheaven/formatters/_stat.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/parsers/__init__.py` & `flakeheaven-3.3.0/flakeheaven/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/parsers/_jupyter.py` & `flakeheaven-3.3.0/flakeheaven/parsers/_jupyter.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/parsers/_markdown.py` & `flakeheaven-3.3.0/flakeheaven/parsers/_markdown.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/parsers/_rst.py` & `flakeheaven-3.3.0/flakeheaven/parsers/_rst.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/parsers/_yaml.py` & `flakeheaven-3.3.0/flakeheaven/parsers/_yaml.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/flakeheaven/plugins/_pylint.py` & `flakeheaven-3.3.0/flakeheaven/plugins/_pylint.py`

 * *Files identical despite different names*

### Comparing `flakeheaven-3.2.1/pyproject.toml` & `flakeheaven-3.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flakeheaven"
-version = "3.2.1"
+version = "3.3.0"
 description = "FlakeHeaven is a [Flake8](https://gitlab.com/pycqa/flake8) wrapper to make it cool."
 authors = ["Gram <master_fess@mail.ru>"]
 repository = "https://github.com/flakeheaven/flakeheaven"
 homepage = "https://github.com/flakeheaven/flakeheaven"
 documentation = "https://flakeheaven.readthedocs.io/"
 readme = "README.md"
 license = "MIT"
@@ -147,12 +147,12 @@
 import_heading_stdlib = "built-in"
 import_heading_thirdparty = "external"
 import_heading_firstparty = "project"
 import_heading_localfolder = "app"
 
 
 [tool.commitizen]
-version = "3.2.1"
+version = "3.3.0"
 annotated_tag = true
 update_changelog_on_bump = true
 bump_message = "bump: $current_version → $new_version"  # keep in sync with .github/workflows/bumpversion.yml!!!
 changelog_start_rev = "0.11.0"
```

### Comparing `flakeheaven-3.2.1/setup.py` & `flakeheaven-3.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,185 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: flakeheaven
+Version: 3.3.0
+Summary: FlakeHeaven is a [Flake8](https://gitlab.com/pycqa/flake8) wrapper to make it cool.
+Home-page: https://github.com/flakeheaven/flakeheaven
+License: MIT
+Author: Gram
+Author-email: master_fess@mail.ru
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Framework :: Flake8
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Quality Assurance
+Provides-Extra: docs
+Requires-Dist: alabaster ; extra == "docs"
+Requires-Dist: colorama
+Requires-Dist: entrypoints
+Requires-Dist: flake8 (>=4.0.1,<5.0.0)
+Requires-Dist: importlib-metadata (>=1.0) ; python_version < "3.8"
+Requires-Dist: myst-parser (>=0.18.0,<0.19.0) ; extra == "docs"
+Requires-Dist: pygments
+Requires-Dist: pygments-github-lexers ; extra == "docs"
+Requires-Dist: sphinx ; extra == "docs"
+Requires-Dist: toml
+Requires-Dist: urllib3
+Project-URL: Documentation, https://flakeheaven.readthedocs.io/
+Project-URL: Repository, https://github.com/flakeheaven/flakeheaven
+Description-Content-Type: text/markdown
+
+# FlakeHeaven
+
+[![License: MIT](https://img.shields.io/pypi/l/flakeheaven)](https://opensource.org/licenses/MIT)
+[![python versions](https://img.shields.io/pypi/pyversions/flakeheaven)](https://pypi.org/project/flakeheaven/)
+
+[![version](https://img.shields.io/pypi/v/flakeheaven)](https://pypi.org/project/flakeheaven/)
+[![conda](https://anaconda.org/conda-forge/flakeheaven/badges/version.svg)](https://anaconda.org/conda-forge/flakeheaven)
+[![Downloads](https://img.shields.io/pypi/dm/flakeheaven)](https://pypi.org/project/flakeheaven/)
+
+[![CI](https://github.com/flakeheaven/flakeheaven/actions/workflows/ci.yaml/badge.svg)](https://github.com/flakeheaven/flakeheaven/actions/workflows/ci.yaml)
+[![Docs](https://readthedocs.org/projects/flakeheaven/badge/?version=latest)](https://flakeheaven.readthedocs.io/en/latest/)
+
+
+flakeheaven is a python linter built around flake8 to enable inheritable and complex toml configuration.
+
+This project is a fork of [FlakeHell](https://github.com/life4/flakehell). FlakeHell and other forks of it such as
+flakehell/flakehell are [no longer maintained](https://github.com/flakehell/flakehell/issues/25) and do not work with Flake8 4.0.x.
+
+FlakeHeaven works with Flake8 4.0.1 or greater. This fork will be [maintained by the community](https://github.com/flakeheaven/flakeheaven/discussions/1) that developed the existing forks.
+
++ [Lint md, rst, ipynb, and more](https://flakeheaven.readthedocs.io/en/latest/parsers.html).
++ [Shareable and remote configs](https://flakeheaven.readthedocs.io/en/latest/config.html#base).
++ [Legacy-friendly](https://flakeheaven.readthedocs.io/en/latest/commands/baseline.html): ability to get report only about new errors.
++ Caching for much better performance.
++ [Use only specified plugins](https://flakeheaven.readthedocs.io/en/latest/config.html#plugins), not everything installed.
++ [Make output beautiful](https://flakeheaven.readthedocs.io/en/latest//formatters.html).
++ [pyproject.toml](https://www.python.org/dev/peps/pep-0518/) support.
++ [Check that all required plugins are installed](https://flakeheaven.readthedocs.io/en/latest/commands/missed.html).
++ [Syntax highlighting in messages and code snippets](https://flakeheaven.readthedocs.io/en/latest/formatters.html#colored-with-source-code).
++ [PyLint](https://github.com/PyCQA/pylint) integration.
++ [Powerful GitLab support](https://flakeheaven.readthedocs.io/en/latest/formatters.html#gitlab).
++ Codes management:
+    + Manage codes per plugin.
+    + Enable and disable plugins and codes by wildcard.
+    + [Show codes for installed plugins](https://flakeheaven.readthedocs.io/en/latest/commands/plugins.html).
+    + [Show all messages and codes for a plugin](https://flakeheaven.readthedocs.io/en/latest/commands/codes.html).
+    + Allow codes intersection for different plugins.
+
+![output example](./assets/grouped.png)
+
+## Compatibility
+
+FlakeHeaven supports all flake8 plugins, formatters, and configs. However, FlakeHeaven has its own beautiful way to configure enabled plugins and codes. So, options like `--ignore` and `--select` are unsupported. You can have flake8 and FlakeHeaven in one project if you want but enabled plugins should be explicitly specified.
+
+## Installation
+
+```bash
+python3 -m pip install --user flakeheaven
+```
+
+## Usage
+
+First of all, let's create `pyproject.toml` config:
+
+```toml
+[tool.flakeheaven]
+# optionally inherit from remote config (or local if you want)
+base = "https://raw.githubusercontent.com/flakeheaven/flakeheaven/main/pyproject.toml"
+# specify any flake8 options. For example, exclude "example.py":
+exclude = ["example.py"]
+# make output nice
+format = "grouped"
+# 80 chars aren't enough in 21 century
+max_line_length = 90
+# show line of source code in output
+show_source = true
+
+# list of plugins and rules for them
+[tool.flakeheaven.plugins]
+# include everything in pyflakes except F401
+pyflakes = ["+*", "-F401"]
+# enable only codes from S100 to S199
+flake8-bandit = ["-*", "+S1??"]
+# enable everything that starts from `flake8-`
+"flake8-*" = ["+*"]
+# explicitly disable plugin
+flake8-docstrings = ["-*"]
+```
+
+Show plugins that aren't installed yet:
+
+```bash
+flakeheaven missed
+```
+
+Show installed plugins, used plugins, specified rules, codes prefixes:
+
+```bash
+flakeheaven plugins
+```
+
+![plugins command output](./assets/plugins.png)
+
+Show codes and messages for a specific plugin:
+
+```bash
+flakeheaven codes pyflakes
+```
+
+![codes command output](./assets/codes.png)
+
+Run flake8 against the code:
+
+```bash
+flakeheaven lint
+```
+
+This command accepts all the same arguments as Flake8.
+
+Read [the documentation](https://flakeheaven.readthedocs.io/en/latest/) for more information.
+
+## Contributing
+
+1. Add tests when possible (eg for features / fixes / refactor, etc. )
+2. Add your contribution to the code / docs
+3. Ensure your code passes all (both original and your own) tests.
+4. Commit using [proper header](https://www.conventionalcommits.org/en/v1.0.0/)
+5. Create a PR
+
+Contributions are welcome! A few ideas where you can contribute:
+
++ Improve documentation.
++ Add more tests.
++ Improve performance.
++ Found a bug? Fix it!
++ Made an article about FlakeHeaven? Great! Let's add it into the `README.md`.
++ Don't have time to code? No worries! Just tell your friends and subscribers about the project. More users -> more contributors -> more cool features.
+
+A convenient way to run tests is using [Poetry](https://python-poetry.org/docs/master/#installing-with-the-official-installer):
+
+```bash
+curl -sSL https://install.python-poetry.org | python3 -
+poetry install
+poetry run pytest tests
+```
 
-packages = \
-['flakeheaven',
- 'flakeheaven._logic',
- 'flakeheaven._patched',
- 'flakeheaven.commands',
- 'flakeheaven.formatters',
- 'flakeheaven.parsers',
- 'flakeheaven.plugins']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['colorama',
- 'entrypoints',
- 'flake8>=4.0.1,<5.0.0',
- 'pygments',
- 'toml',
- 'urllib3']
-
-extras_require = \
-{':python_version < "3.8"': ['importlib-metadata>=1.0'],
- 'docs': ['alabaster',
-          'pygments-github-lexers',
-          'sphinx',
-          'myst-parser>=0.18.0,<0.19.0']}
-
-entry_points = \
-{'console_scripts': ['flake8heavened = flakeheaven:flake8_entrypoint',
-                     'flakeheaven = flakeheaven:entrypoint'],
- 'flake8.extension': ['pylint = flakeheaven.plugins:PyLintChecker'],
- 'flake8.report': ['baseline = flakeheaven.formatters:BaseLineFormatter',
-                   'colored = flakeheaven.formatters:ColoredFormatter',
-                   'gitlab = flakeheaven.formatters:GitlabFormatter',
-                   'grouped = flakeheaven.formatters:GroupedFormatter',
-                   'json = flakeheaven.formatters:JSONFormatter',
-                   'stat = flakeheaven.formatters:StatFormatter']}
-
-setup_kwargs = {
-    'name': 'flakeheaven',
-    'version': '3.2.1',
-    'description': 'FlakeHeaven is a [Flake8](https://gitlab.com/pycqa/flake8) wrapper to make it cool.',
-    'long_description': '# FlakeHeaven\n\n[![License: MIT](https://img.shields.io/pypi/l/flakeheaven)](https://opensource.org/licenses/MIT)\n[![python versions](https://img.shields.io/pypi/pyversions/flakeheaven)](https://pypi.org/project/flakeheaven/)\n\n[![version](https://img.shields.io/pypi/v/flakeheaven)](https://pypi.org/project/flakeheaven/)\n[![conda](https://anaconda.org/conda-forge/flakeheaven/badges/version.svg)](https://anaconda.org/conda-forge/flakeheaven)\n[![Downloads](https://img.shields.io/pypi/dm/flakeheaven)](https://pypi.org/project/flakeheaven/)\n\n[![CI](https://github.com/flakeheaven/flakeheaven/actions/workflows/ci.yaml/badge.svg)](https://github.com/flakeheaven/flakeheaven/actions/workflows/ci.yaml)\n[![Docs](https://readthedocs.org/projects/flakeheaven/badge/?version=latest)](https://flakeheaven.readthedocs.io/en/latest/)\n\n\nflakeheaven is a python linter built around flake8 to enable inheritable and complex toml configuration.\n\nThis project is a fork of [FlakeHell](https://github.com/life4/flakehell). FlakeHell and other forks of it such as\nflakehell/flakehell are [no longer maintained](https://github.com/flakehell/flakehell/issues/25) and do not work with Flake8 4.0.x.\n\nFlakeHeaven works with Flake8 4.0.1 or greater. This fork will be [maintained by the community](https://github.com/flakeheaven/flakeheaven/discussions/1) that developed the existing forks.\n\n+ [Lint md, rst, ipynb, and more](https://flakeheaven.readthedocs.io/en/latest/parsers.html).\n+ [Shareable and remote configs](https://flakeheaven.readthedocs.io/en/latest/config.html#base).\n+ [Legacy-friendly](https://flakeheaven.readthedocs.io/en/latest/commands/baseline.html): ability to get report only about new errors.\n+ Caching for much better performance.\n+ [Use only specified plugins](https://flakeheaven.readthedocs.io/en/latest/config.html#plugins), not everything installed.\n+ [Make output beautiful](https://flakeheaven.readthedocs.io/en/latest//formatters.html).\n+ [pyproject.toml](https://www.python.org/dev/peps/pep-0518/) support.\n+ [Check that all required plugins are installed](https://flakeheaven.readthedocs.io/en/latest/commands/missed.html).\n+ [Syntax highlighting in messages and code snippets](https://flakeheaven.readthedocs.io/en/latest/formatters.html#colored-with-source-code).\n+ [PyLint](https://github.com/PyCQA/pylint) integration.\n+ [Powerful GitLab support](https://flakeheaven.readthedocs.io/en/latest/formatters.html#gitlab).\n+ Codes management:\n    + Manage codes per plugin.\n    + Enable and disable plugins and codes by wildcard.\n    + [Show codes for installed plugins](https://flakeheaven.readthedocs.io/en/latest/commands/plugins.html).\n    + [Show all messages and codes for a plugin](https://flakeheaven.readthedocs.io/en/latest/commands/codes.html).\n    + Allow codes intersection for different plugins.\n\n![output example](./assets/grouped.png)\n\n## Compatibility\n\nFlakeHeaven supports all flake8 plugins, formatters, and configs. However, FlakeHeaven has it\'s own beautiful way to configure enabled plugins and codes. So, options like `--ignore` and `--select` unsupported. You can have flake8 and FlakeHeaven in one project if you want but enabled plugins should be explicitly specified.\n\n## Installation\n\n```bash\npython3 -m pip install --user flakeheaven\n```\n\n## Usage\n\nFirst of all, let\'s create `pyproject.toml` config:\n\n```toml\n[tool.flakeheaven]\n# optionally inherit from remote config (or local if you want)\nbase = "https://raw.githubusercontent.com/flakeheaven/flakeheaven/main/pyproject.toml"\n# specify any flake8 options. For example, exclude "example.py":\nexclude = ["example.py"]\n# make output nice\nformat = "grouped"\n# 80 chars aren\'t enough in 21 century\nmax_line_length = 90\n# show line of source code in output\nshow_source = true\n\n# list of plugins and rules for them\n[tool.flakeheaven.plugins]\n# include everything in pyflakes except F401\npyflakes = ["+*", "-F401"]\n# enable only codes from S100 to S199\nflake8-bandit = ["-*", "+S1??"]\n# enable everything that starts from `flake8-`\n"flake8-*" = ["+*"]\n# explicitly disable plugin\nflake8-docstrings = ["-*"]\n```\n\nShow plugins that aren\'t installed yet:\n\n```bash\nflakeheaven missed\n```\n\nShow installed plugins, used plugins, specified rules, codes prefixes:\n\n```bash\nflakeheaven plugins\n```\n\n![plugins command output](./assets/plugins.png)\n\nShow codes and messages for a specific plugin:\n\n```bash\nflakeheaven codes pyflakes\n```\n\n![codes command output](./assets/codes.png)\n\nRun flake8 against the code:\n\n```bash\nflakeheaven lint\n```\n\nThis command accepts all the same arguments as Flake8.\n\nRead [the documentation](https://flakeheaven.readthedocs.io/en/latest/) for more information.\n\n## Contributing\n\n1. Add tests when possible (eg for features / fixes / refactor, etc. )\n2. add your contribution to the code / docs\n3. Ensure your code passes all (both oririnal and your own) tests.\n4. commit using [proper header](https://www.conventionalcommits.org/en/v1.0.0/)\n5. create a PR\n\nContributions are welcome! A few ideas where you can contribute:\n\n+ Improve documentation.\n+ Add more tests.\n+ Improve performance.\n+ Found a bug? Fix it!\n+ Made an article about FlakeHeaven? Great! Let\'s add it into the `README.md`.\n+ Don\'t have time to code? No worries! Just tell your friends and subscribers about the project. More users -> more contributors -> more cool features.\n\nA convenient way to run tests is using [Poetry](https://python-poetry.org/docs/master/#installing-with-the-official-installer):\n\n```bash\ncurl -sSL https://install.python-poetry.org | python3 -\npoetry install\npoetry run pytest tests\n```\n\nThank you :heart:\n\n![](./assets/flaky.png)\n\nThe FlakeHeaven mascot (Flaky) is created by [@illustrator.way](https://www.instagram.com/illustrator.way/) and licensed under the [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) license.\n',
-    'author': 'Gram',
-    'author_email': 'master_fess@mail.ru',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/flakeheaven/flakeheaven',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+Thank you :heart:
 
+![](./assets/flaky.png)
+
+The FlakeHeaven mascot (Flaky) is created by [@illustrator.way](https://www.instagram.com/illustrator.way/) and licensed under the [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) license.
 
-setup(**setup_kwargs)
```

