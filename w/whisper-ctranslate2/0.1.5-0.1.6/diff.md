# Comparing `tmp/whisper-ctranslate2-0.1.5.tar.gz` & `tmp/whisper-ctranslate2-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-ctranslate2-0.1.5.tar", last modified: Sun Apr  9 16:41:00 2023, max compression
+gzip compressed data, was "whisper-ctranslate2-0.1.6.tar", last modified: Mon Apr 10 13:55:18 2023, max compression
```

## Comparing `whisper-ctranslate2-0.1.5.tar` & `whisper-ctranslate2-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-09 16:41:00.583496 whisper-ctranslate2-0.1.5/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-03-17 10:20:50.000000 whisper-ctranslate2-0.1.5/LICENSE
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3982 2023-04-09 16:41:00.583496 whisper-ctranslate2-0.1.5/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3331 2023-04-09 16:29:17.000000 whisper-ctranslate2-0.1.5/README.md
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-04-09 16:41:00.583496 whisper-ctranslate2-0.1.5/setup.cfg
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1321 2023-04-09 14:32:30.000000 whisper-ctranslate2-0.1.5/setup.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-09 16:41:00.583496 whisper-ctranslate2-0.1.5/src/
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-09 16:41:00.583496 whisper-ctranslate2-0.1.5/src/whisper_ctranslate2/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2846 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.1.5/src/whisper_ctranslate2/languages.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4648 2023-04-04 20:15:50.000000 whisper-ctranslate2-0.1.5/src/whisper_ctranslate2/models.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5136 2023-04-09 16:29:09.000000 whisper-ctranslate2-0.1.5/src/whisper_ctranslate2/transcribe.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    11296 2023-04-09 16:29:09.000000 whisper-ctranslate2-0.1.5/src/whisper_ctranslate2/whisper_ctranslate2.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5527 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.1.5/src/whisper_ctranslate2/writers.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-09 16:41:00.583496 whisper-ctranslate2-0.1.5/whisper_ctranslate2.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3982 2023-04-09 16:41:00.000000 whisper-ctranslate2-0.1.5/whisper_ctranslate2.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      487 2023-04-09 16:41:00.000000 whisper-ctranslate2-0.1.5/whisper_ctranslate2.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-04-09 16:41:00.000000 whisper-ctranslate2-0.1.5/whisper_ctranslate2.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-04-09 16:41:00.000000 whisper-ctranslate2-0.1.5/whisper_ctranslate2.egg-info/entry_points.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       80 2023-04-09 16:41:00.000000 whisper-ctranslate2-0.1.5/whisper_ctranslate2.egg-info/requires.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2023-04-09 16:41:00.000000 whisper-ctranslate2-0.1.5/whisper_ctranslate2.egg-info/top_level.txt
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-10 13:55:18.262423 whisper-ctranslate2-0.1.6/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-03-17 10:20:50.000000 whisper-ctranslate2-0.1.6/LICENSE
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3982 2023-04-10 13:55:18.262423 whisper-ctranslate2-0.1.6/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3331 2023-04-09 16:29:17.000000 whisper-ctranslate2-0.1.6/README.md
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-04-10 13:55:18.262423 whisper-ctranslate2-0.1.6/setup.cfg
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1499 2023-04-10 13:39:26.000000 whisper-ctranslate2-0.1.6/setup.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-10 13:55:18.262423 whisper-ctranslate2-0.1.6/src/
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-10 13:55:18.262423 whisper-ctranslate2-0.1.6/src/whisper_ctranslate2/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2846 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.1.6/src/whisper_ctranslate2/languages.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4674 2023-04-10 13:24:17.000000 whisper-ctranslate2-0.1.6/src/whisper_ctranslate2/models.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5136 2023-04-10 13:24:17.000000 whisper-ctranslate2-0.1.6/src/whisper_ctranslate2/transcribe.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2023-04-10 13:39:26.000000 whisper-ctranslate2-0.1.6/src/whisper_ctranslate2/version.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    11529 2023-04-10 13:39:26.000000 whisper-ctranslate2-0.1.6/src/whisper_ctranslate2/whisper_ctranslate2.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5527 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.1.6/src/whisper_ctranslate2/writers.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-10 13:55:18.262423 whisper-ctranslate2-0.1.6/whisper_ctranslate2.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3982 2023-04-10 13:55:18.000000 whisper-ctranslate2-0.1.6/whisper_ctranslate2.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      522 2023-04-10 13:55:18.000000 whisper-ctranslate2-0.1.6/whisper_ctranslate2.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-04-10 13:55:18.000000 whisper-ctranslate2-0.1.6/whisper_ctranslate2.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-04-10 13:55:18.000000 whisper-ctranslate2-0.1.6/whisper_ctranslate2.egg-info/entry_points.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       80 2023-04-10 13:55:18.000000 whisper-ctranslate2-0.1.6/whisper_ctranslate2.egg-info/requires.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2023-04-10 13:55:18.000000 whisper-ctranslate2-0.1.6/whisper_ctranslate2.egg-info/top_level.txt
```

### Comparing `whisper-ctranslate2-0.1.5/LICENSE` & `whisper-ctranslate2-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.5/PKG-INFO` & `whisper-ctranslate2-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.1.5
+Version: 0.1.6
 Summary: Whisper command line client that uses CTranslate2
 Home-page: https://github.com/jordimas/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `whisper-ctranslate2-0.1.5/README.md` & `whisper-ctranslate2-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.5/setup.py` & `whisper-ctranslate2-0.1.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,17 +3,23 @@
 import pkg_resources
 import os
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
+
+def read_version(fname="src/whisper_ctranslate2/version.py"):
+    exec(compile(open(fname, encoding="utf-8").read(), fname, "exec"))
+    return locals()["__version__"]
+
+
 setup(
     name="whisper-ctranslate2",
-    version="0.1.5",
+    version=read_version(),
     description="Whisper command line client that uses CTranslate2",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/jordimas/whisper-ctranslate2",
     author="Jordi Mas",
     author_email="jmas@softcatala.org",
     license="MIT",
```

### Comparing `whisper-ctranslate2-0.1.5/src/whisper_ctranslate2/languages.py` & `whisper-ctranslate2-0.1.6/src/whisper_ctranslate2/languages.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.5/src/whisper_ctranslate2/models.py` & `whisper-ctranslate2-0.1.6/src/whisper_ctranslate2/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,27 +57,28 @@
 
         raise RuntimeError(
             "Model has been downloaded but the SHA256 checksum does not not match. Please retry downloading the model."
         )
 
     def _are_localfile_checksums_correct(self, model: str, url: str) -> bool:
         model_path = self.get_model_path(model)
-        model_bytes = bytes()
         expected_sha256 = url.split("/")[-2].rsplit(".", 1)[0]
 
+        _hash = hashlib.sha256()
         for _file in self._FILES:
             _file = os.path.join(model_path, _file)
 
             if not os.path.exists(_file):
                 return False
 
             with open(_file, "rb") as f:
-                model_bytes += f.read()
+                while chunk := f.read(8192):
+                    _hash.update(chunk)
 
-        got = hashlib.sha256(model_bytes).hexdigest()
+        got = _hash.hexdigest()
         return got == expected_sha256
 
     def _download(self, model: str, url: str):
         model_path = self.get_model_path(model)
         os.makedirs(model_path, exist_ok=True)
 
         download_target = os.path.join(model_path, os.path.basename(url))
```

### Comparing `whisper-ctranslate2-0.1.5/src/whisper_ctranslate2/transcribe.py` & `whisper-ctranslate2-0.1.6/src/whisper_ctranslate2/transcribe.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.5/src/whisper_ctranslate2/whisper_ctranslate2.py` & `whisper-ctranslate2-0.1.6/src/whisper_ctranslate2/whisper_ctranslate2.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .transcribe import Transcribe, TranscriptionOptions
 from .models import Models
 from .languages import LANGUAGES, TO_LANGUAGE_CODE, from_language_to_iso_code
 import numpy as np
 import warnings
 from typing import Union, List
 from .writers import get_writer
+from .version import __version__
 
 
 def optional_int(string):
     return None if string == "None" else int(string)
 
 
 def str2bool(string):
@@ -233,14 +234,21 @@
     parser.add_argument(
         "--print_colors",
         type=str2bool,
         default=False,
         help="Print the transcribed text using an experimental color coding strategy to highlight words with high or low confidence",
     )
 
+    parser.add_argument(
+        "--version",
+        action="version",
+        version="%(prog)s {version}".format(version=__version__),
+        help="Show program's version number and exit",
+    )
+
     return parser.parse_args().__dict__
 
 
 def main():
     args = read_command_line()
     output_dir: str = args.pop("output_dir")
     output_format: str = args.pop("output_format")
```

### Comparing `whisper-ctranslate2-0.1.5/src/whisper_ctranslate2/writers.py` & `whisper-ctranslate2-0.1.6/src/whisper_ctranslate2/writers.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.5/whisper_ctranslate2.egg-info/PKG-INFO` & `whisper-ctranslate2-0.1.6/whisper_ctranslate2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.1.5
+Version: 0.1.6
 Summary: Whisper command line client that uses CTranslate2
 Home-page: https://github.com/jordimas/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

