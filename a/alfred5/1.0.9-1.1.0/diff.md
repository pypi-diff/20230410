# Comparing `tmp/alfred5-1.0.9.tar.gz` & `tmp/alfred5-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfred5-1.0.9.tar", last modified: Sun Apr  9 03:30:45 2023, max compression
+gzip compressed data, was "alfred5-1.1.0.tar", last modified: Mon Apr 10 14:03:39 2023, max compression
```

## Comparing `alfred5-1.0.9.tar` & `alfred5-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:30:45.533282 alfred5-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-09 03:30:36.000000 alfred5-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-09 03:30:36.000000 alfred5-1.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-04-09 03:30:45.533282 alfred5-1.0.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:30:45.529282 alfred5-1.0.9/alfred5/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-09 03:30:36.000000 alfred5-1.0.9/alfred5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-04-09 03:30:36.000000 alfred5-1.0.9/alfred5/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-09 03:30:36.000000 alfred5-1.0.9/alfred5/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:30:45.533282 alfred5-1.0.9/alfred5/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    35477 2023-04-09 03:30:36.000000 alfred5-1.0.9/alfred5/icons/error.png
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-09 03:30:36.000000 alfred5-1.0.9/alfred5/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:30:45.533282 alfred5-1.0.9/alfred5.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-04-09 03:30:45.000000 alfred5-1.0.9/alfred5.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-09 03:30:45.000000 alfred5-1.0.9/alfred5.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 03:30:45.000000 alfred5-1.0.9/alfred5.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 03:30:45.000000 alfred5-1.0.9/alfred5.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-09 03:30:45.000000 alfred5-1.0.9/alfred5.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-09 03:30:45.000000 alfred5-1.0.9/alfred5.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:30:45.533282 alfred5-1.0.9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-09 03:30:36.000000 alfred5-1.0.9/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 03:30:45.533282 alfred5-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-09 03:30:36.000000 alfred5-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:30:45.533282 alfred5-1.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 03:30:36.000000 alfred5-1.0.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-09 03:30:36.000000 alfred5-1.0.9/tests/test_snippets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:03:39.031641 alfred5-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-10 14:03:28.000000 alfred5-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-10 14:03:28.000000 alfred5-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-04-10 14:03:39.031641 alfred5-1.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:03:39.027641 alfred5-1.1.0/alfred5/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-10 14:03:28.000000 alfred5-1.1.0/alfred5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-04-10 14:03:28.000000 alfred5-1.1.0/alfred5/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-10 14:03:28.000000 alfred5-1.1.0/alfred5/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:03:39.031641 alfred5-1.1.0/alfred5/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-04-10 14:03:28.000000 alfred5-1.1.0/alfred5/icons/download.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35477 2023-04-10 14:03:28.000000 alfred5-1.1.0/alfred5/icons/error.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-10 14:03:28.000000 alfred5-1.1.0/alfred5/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:03:39.031641 alfred5-1.1.0/alfred5.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-04-10 14:03:39.000000 alfred5-1.1.0/alfred5.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-10 14:03:39.000000 alfred5-1.1.0/alfred5.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 14:03:39.000000 alfred5-1.1.0/alfred5.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 14:03:38.000000 alfred5-1.1.0/alfred5.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-10 14:03:39.000000 alfred5-1.1.0/alfred5.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 14:03:39.000000 alfred5-1.1.0/alfred5.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:03:39.031641 alfred5-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-10 14:03:28.000000 alfred5-1.1.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 14:03:39.031641 alfred5-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-10 14:03:28.000000 alfred5-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:03:39.031641 alfred5-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 14:03:28.000000 alfred5-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-10 14:03:28.000000 alfred5-1.1.0/tests/test_snippets.py
```

### Comparing `alfred5-1.0.9/LICENSE` & `alfred5-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alfred5-1.0.9/PKG-INFO` & `alfred5-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfred5
-Version: 1.0.9
+Version: 1.1.0
 Summary: Simple python wrapper for alfred workflow / snippets
 Home-page: https://github.com/yedhrab/alfred5
 Author: Yunus Emre Ak
 Author-email: yemreak.com@gmail.com
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/yedhrab/alfred5/
 Project-URL: Documentation, https://github.com/yedhrab/alfred5/wiki
```

### Comparing `alfred5-1.0.9/alfred5/client.py` & `alfred5-1.1.0/alfred5/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from __future__ import annotations
 from logging import Logger, StreamHandler
 import json
+from .models import Result
 from traceback import format_exc
 import sys
 from asyncio import run
 from collections.abc import Callable, Coroutine
 from pathlib import Path
 from shutil import copy2, move
 from tempfile import TemporaryDirectory
 from zipfile import ZIP_DEFLATED, ZipFile
 from ruamel.yaml import load as yaml_load, dump as yaml_dump
 from plistlib import load as plist_load
-from .models import SNIPPET_INFO_TEMPLATE, Result, Snippet, yaml
+from .models import SNIPPET_INFO_TEMPLATE, Result, Snippet
 from typing import NoReturn
 from .errors import WorkflowError
+from ruamel.yaml import YAML
 
 
 class SnippetClient:
     snippets: list[Snippet]
 
     def __init__(self) -> None:
         self.snippets: list[Snippet] = []
@@ -55,14 +57,16 @@
 
 
 class WorkflowClient:
     query: str
     page_count: int
     bundleid: str
 
+    icondir: Path
+
     datadir: Path
     db_results: Path
 
     results: list[Result]
 
     logger: Logger
 
@@ -74,51 +78,102 @@
         self.page_count = sys.argv[1].count("+") + 1
         self.query = sys.argv[1].replace("+", "")
 
         self.log(
             f"sys.argv: {sys.argv} page_count: {self.page_count} query: {self.query}"
         )
 
+        self.icondir = Path(__file__).parent / "icons"
+
         self.log(f"bundleid reading from info.plist...")
         with Path("info.plist").open("rb") as f:
             self.bundleid = plist_load(f)["bundleid"]
             self.log(f"bundleid: {self.bundleid}")
         self.datadir = Path("db")
         self.datadir.mkdir(parents=True, exist_ok=True)
 
         self.log(f"datadir: {self.datadir.absolute()}")
         self.db_results = self.datadir / "results.yml"
         self.log(f"db_results: {self.db_results}")
 
+        self.yaml = YAML()
+
         self.results = []
 
     def log(self, msg: str):
         self.logger.debug(msg)
 
+    def install_requirements(self) -> None:
+        """Check if requirements are met"""
+        self.log(f"checking requirements...")
+        req_file = Path("requirements.txt")
+        if req_file.exists():
+            packages = req_file.read_text().splitlines()
+            self.log(f"found requirements.txt: {packages}")
+            try:
+                import pkg_resources
+
+                pkg_resources.require(packages)
+            except Exception:
+                import subprocess
+
+                command = ["python3", "-m", "pip", "install", "--target=.", *packages]
+                subprocess.Popen(
+                    command,
+                    start_new_session=True,
+                    stdout=subprocess.DEVNULL,
+                    stderr=subprocess.DEVNULL,
+                )
+                self.add_result(
+                    title="Requirements are installing (you can close alfred)",
+                    subtitle=f"Executed command: {' '.join(command)}",
+                    icon_path=self.icondir / "download.png",
+                    arg=" ".join(command),
+                )
+                self.response()
+        else:
+            self.log(f"no requirements.txt found")
+
     def cache_response(self) -> None:
         """Cache response to workflow db_results"""
         if not self.db_results.exists():
             self.db_results.parent.mkdir(parents=True, exist_ok=True)
             self.db_results.touch()
         with self.db_results.open("r") as f:
             data = yaml_load(f) or {}
-        data[self.query] = self.results
+        data[self.query] = [
+            {
+                "title": result.title,
+                "subtitle": result.subtitle,
+                "icon_path": result.icon.path if result.icon else None,
+            }
+            for result in self.results
+        ]
         with self.db_results.open("w") as f:
             yaml_dump(data, f)
             self.log(f"cached response to {self.db_results}")
 
     def load_cached_response(self) -> bool:
         """Load cached result from alfred"""
         self.log(f"checking if `{self.query}` exists in `{self.db_results}`")
         if self.db_results.exists():
             with self.db_results.open("r") as f:
-                data: dict[str, list[Result]] = yaml.load(f)
+                data: dict[str, list[dict[str, str]]] = self.yaml.load(f)
                 self.log(f"loaded data from {self.db_results} {len(data.keys())}")
                 if self.query in data:
-                    self.results = data[self.query]
+                    self.results = [
+                        Result(
+                            title=result["title"],
+                            subtitle=result["subtitle"],
+                            icon=Result.Icon(result["icon_path"])
+                            if result["icon_path"]
+                            else None,
+                        )
+                        for result in data[self.query]
+                    ]
                     self.log(f"found: {self.query} in {self.db_results}")
                     return True
         self.log(f"not found `{self.query}` in `{self.db_results}`")
         return False
 
     @classmethod
     def run(
@@ -134,48 +189,78 @@
 
         if __name__ == "__main__":
             AlfredWorkflowClient.run(main)
         ```
         """
         client = cls()
         try:
+            client.install_requirements()
             run(func(client))
             client.response()
         except Exception as e:
             if isinstance(e, WorkflowError):
-                client.error_response(title=e.title, subtitle=e.subtitle)
+                client.error_response(
+                    title=e.title,
+                    subtitle=e.subtitle,
+                    arg=e.arg,
+                )
             else:
                 client.error_response(
-                    title=str(e), subtitle=format_exc().strip().split("\n")[-1]
+                    title=str(e),
+                    subtitle=format_exc().strip().split("\n")[-1],
+                    arg=format_exc().strip(),
                 )
 
     def add_result(
         self,
         title: str,
         subtitle: str = "",
         icon_path: str | Path | None = None,
         arg: str = "",
         http_downloader: Callable[[str], str] | None = None,
     ) -> None:
-        """Create and add alfred result."""
+        """Create and add alfred result
+
+        - title: result title
+        - subtitle: result subtitle
+        - icon_path: result icon path
+        - arg: argument to pass to alfred
+        - http_downloader: function to download http icon
+        """
         icon = None
         if icon_path:
             if http_downloader and "http" in str(icon_path):
                 self.log(f"downloading icon from {icon_path}")
                 icon_path = http_downloader(str(icon_path))
             icon = Result.Icon(str(icon_path))
         self.results.append(Result(title=title, subtitle=subtitle, icon=icon, arg=arg))
 
     def error_response(
-        self, title: str, subtitle: str, icon_path: str | Path | None = None
+        self,
+        title: str,
+        subtitle: str,
+        icon_path: str | Path | None = None,
+        arg: str = "",
     ) -> NoReturn:
+        """Create and add alfred error result
+
+        - title: error title
+        - subtitle: error subtitle
+        - icon_path: error icon path
+        - arg: argument to pass to alfred
+        - terminate: terminate workflow
+        """
         self.add_result(
             title=title,
             subtitle=subtitle,
-            icon_path=icon_path or Path(__file__).parent / "icons" / "error.png",
+            icon_path=icon_path or self.icondir / "error.png",
+            arg=arg,
         )
         self.response()
 
     def response(self) -> NoReturn:
-        """Print alfred results and exit."""
+        """Print alfred results and exit
+
+        - terminate: terminate workflow
+        """
         print(json.dumps({"items": [result.to_dict() for result in self.results]}))
         exit(0)
```

### Comparing `alfred5-1.0.9/alfred5/icons/error.png` & `alfred5-1.1.0/alfred5/icons/error.png`

 * *Files identical despite different names*

### Comparing `alfred5-1.0.9/alfred5/models.py` & `alfred5-1.1.0/alfred5/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 from __future__ import annotations
 
 from dataclasses import asdict, dataclass, field
 from json import dump
 from pathlib import Path
 from uuid import uuid4
-from ruamel.yaml import YAML, yaml_object
 
 SNIPPET_INFO_TEMPLATE = """<?xml version="1.0" encoding="UTF-8"?>
 <!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
 <plist version="1.0">
 <dict>
 	<key>snippetkeywordprefix</key>
 	<string>{}</string>
 	<key>snippetkeywordsuffix</key>
 	<string>{}</string>
 </dict>
 </plist>"""
 
-yaml = YAML()
 
-
-@yaml_object(yaml)
 @dataclass
 class Snippet:
     """Alfred snippet
 
     ```json
     // name [uid].json
     // Example Markdown [543B95E5-469E-4D8D-B4B7-D16336E08A28].json
@@ -51,15 +47,14 @@
         """Save snippet to file"""
         snippet_path = snippets_dir / f"{self.name} [{self.uid}].json"
         with snippet_path.open("w") as f:
             dump({"alfredsnippet": asdict(self)}, f, indent=4)
         return snippet_path
 
 
-@yaml_object(yaml)
 @dataclass
 class Result:
     """Alfred result
 
     https://www.alfredapp.com/help/workflows/inputs/script-filter/json/
 
     ```json
```

### Comparing `alfred5-1.0.9/alfred5.egg-info/PKG-INFO` & `alfred5-1.1.0/alfred5.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfred5
-Version: 1.0.9
+Version: 1.1.0
 Summary: Simple python wrapper for alfred workflow / snippets
 Home-page: https://github.com/yedhrab/alfred5
 Author: Yunus Emre Ak
 Author-email: yemreak.com@gmail.com
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/yedhrab/alfred5/
 Project-URL: Documentation, https://github.com/yedhrab/alfred5/wiki
```

### Comparing `alfred5-1.0.9/docs/README.md` & `alfred5-1.1.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `alfred5-1.0.9/setup.py` & `alfred5-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from glob import glob
 from os.path import basename, splitext
 from setuptools import find_packages, setup
 from pathlib import Path
 
-VERSION = "1.0.9"
+VERSION = "1.1.0"
 README_PATH = "docs/README.md"
 USERNAME = "yedhrab"
 REPOSITORY = "alfred5"
 
 setup(
     name=REPOSITORY,
     version=VERSION,
```

