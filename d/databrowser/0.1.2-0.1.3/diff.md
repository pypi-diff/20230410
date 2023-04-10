# Comparing `tmp/databrowser-0.1.2.tar.gz` & `tmp/databrowser-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databrowser-0.1.2.tar", max compression
+gzip compressed data, was "databrowser-0.1.3.tar", max compression
```

## Comparing `databrowser-0.1.2.tar` & `databrowser-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-03-19 11:53:06.886355 databrowser-0.1.2/LICENSE
--rw-r--r--   0        0        0     1139 2023-03-23 16:41:28.293645 databrowser-0.1.2/README.md
--rw-r--r--   0        0        0     1073 2023-03-24 14:42:35.850876 databrowser-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-23 15:37:24.509484 databrowser-0.1.2/src/databrowser/__init__.py
--rw-r--r--   0        0        0      353 2023-03-19 11:53:23.933491 databrowser-0.1.2/src/databrowser/data_browser.css
--rw-r--r--   0        0        0     4170 2023-03-24 14:18:14.120777 databrowser-0.1.2/src/databrowser/data_browser.py
--rw-r--r--   0        0        0      118 2023-03-24 12:44:37.403775 databrowser-0.1.2/src/databrowser/widgets/__init__.py
--rw-r--r--   0        0        0     6637 2023-03-24 14:15:30.066816 databrowser-0.1.2/src/databrowser/widgets/_directory_filter_tree.py
--rw-r--r--   0        0        0     2006 1970-01-01 00:00:00.000000 databrowser-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-03-19 11:53:06.886355 databrowser-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1139 2023-04-10 15:34:17.335155 databrowser-0.1.3/README.md
+-rw-r--r--   0        0        0     1199 2023-04-10 16:28:44.526146 databrowser-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 15:34:17.342376 databrowser-0.1.3/src/databrowser/__init__.py
+-rw-r--r--   0        0        0      353 2023-04-10 15:34:17.346013 databrowser-0.1.3/src/databrowser/data_browser.css
+-rw-r--r--   0        0        0     4256 2023-04-10 16:19:44.558279 databrowser-0.1.3/src/databrowser/data_browser.py
+-rw-r--r--   0        0        0      118 2023-04-10 15:34:17.350519 databrowser-0.1.3/src/databrowser/widgets/__init__.py
+-rw-r--r--   0        0        0     6522 2023-04-10 16:14:58.950117 databrowser-0.1.3/src/databrowser/widgets/_directory_filter_tree.py
+-rw-r--r--   0        0        0     2161 1970-01-01 00:00:00.000000 databrowser-0.1.3/PKG-INFO
```

### Comparing `databrowser-0.1.2/LICENSE` & `databrowser-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `databrowser-0.1.2/README.md` & `databrowser-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `databrowser-0.1.2/pyproject.toml` & `databrowser-0.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 [tool.poetry]
 name = "databrowser"
-version = "0.1.2"
+version = "0.1.3"
 description = "Quick tool to browse and view data files (json,csv,parquet,more) on local disk and s3"
 authors = ["Jacob Verhoeks <jacob.verhoeks@gmail.com>"]
 repository = "https://github.com/jverhoeks/databrowser"
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 s3fs = {extras = ["boto3"], version = "^2023.3.0"}
 s3path = "^0.4.1"
-pandas = "^1.3.5"
-textual = "^0.16.0"
+pandas = "^1.5.2"
+textual = ">=0.16,<0.20"
 pyarrow = ">=5.0.0"
+xlrd = "^2.0.1"
+beautifulsoup4 = "^4.12.2"
+lxml = "^4.9.2"
+html5lib = "^1.1"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.17.1"
 pytest = "^7.2.2"
 black = "^23.1.0"
 bandit = "^1.7.5"
 
@@ -28,19 +32,22 @@
 databrowser = "databrowser.data_browser:run"
 
 [tool.isort]
 profile = "black"
 
 [tool.black]
 includes = "src"
-line-length = 200
+line-length = 120
 
 [tool.pylint]
 #rcfile = "pylintrc"
 
+[tool.pylint.format]
+max-line-length = 120
+
 [tool.bandit]
 target = ["src"]
 skips = ["B101"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `databrowser-0.1.2/src/databrowser/data_browser.py` & `databrowser-0.1.3/src/databrowser/data_browser.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import pandas as pd
 from rich.text import Text
 from textual import events
 from textual.app import App, ComposeResult
 from textual.containers import Container, Vertical
 from textual.reactive import var
 from textual.widgets import DataTable, Footer, Header, Static
+
 from .widgets import DirectoryFilterTree
 
 
 class Notification(Static):
     """Helper class for notications"""
 
     def on_mount(self) -> None:
@@ -43,32 +44,33 @@
         ("q", "quit", "Quit"),
     ]
 
     LOADERS = {
         ".csv": pd.read_csv,
         ".parquet": pd.read_parquet,
         ".json": pd.read_json,
+        ".xlsx": pd.read_excel,
+        ".xml": pd.read_xml,
+        ".html": pd.read_html,
     }
 
     show_tree = var(True)
     show_dtype = var(False)
     dataframe = None
 
-    def _load_table(self, df_in=None):
+    def _load_table(self, suffix=None, file_path=None):
         """internal function to load the table"""
         table = self.query_one("#data", DataTable)
         table.clear(columns=True)
 
-        if df_in:
-            self.dataframe = df_in
+        if file_path:
+            self.dataframe = self.LOADERS[suffix](file_path)
 
         if self.show_dtype:
-            show_df = pd.DataFrame(
-                self.dataframe.dtypes.apply(lambda x: x.name).reset_index()
-            )
+            show_df = pd.DataFrame(self.dataframe.dtypes.apply(lambda x: x.name).reset_index())
             show_df.columns = ["field", "dtype"]
         else:
             show_df = self.dataframe
 
         table.add_columns(*show_df.columns.to_list())
         table.zebra_stripes = True
         for i in range(min(100, len(show_df))):
@@ -93,29 +95,27 @@
         yield Footer()
 
     def on_mount(self, event: events.Mount) -> None:
         """event: mount"""
         del event
         self.query_one(DirectoryFilterTree).focus()
 
-    def on_directory_filter_tree_file_selected(
-        self, event: DirectoryFilterTree.FileSelected
-    ) -> None:
+    def on_directory_filter_tree_file_selected(self, event: DirectoryFilterTree.FileSelected) -> None:
         """Called when the user click a file in the directory tree."""
         event.stop()
 
         suffix = pathlib.Path(event.path).suffix.lower()
 
         try:
             if suffix in self.LOADERS:
-                self._load_table(self.LOADERS[suffix](event.path))
+                self._load_table(suffix, event.path)
             else:
                 self.sub_title = f"Unsupported file type:  {suffix}"
         except Exception as exc:  # pylint: disable=W0703
-            self.sub_title = f"ERROR {exc} {suffix}"
+            self.sub_title = f"ERROR {exc} {event.path}"
         else:
             self.sub_title = event.path
 
     def action_toggle_files(self) -> None:
         """Called in response to key binding."""
         self.show_tree = not self.show_tree
```

### Comparing `databrowser-0.1.2/src/databrowser/widgets/_directory_filter_tree.py` & `databrowser-0.1.3/src/databrowser/widgets/_directory_filter_tree.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """ Updated widget to support filter and other Filesystems """
 from __future__ import annotations
 
 from dataclasses import dataclass
 from pathlib import Path
 from typing import ClassVar
 
-from s3path import S3Path
 from rich.style import Style
 from rich.text import Text, TextType
-
+from s3path import S3Path
 from textual.message import Message
 from textual.widgets._tree import TOGGLE_STYLE, Tree, TreeNode
 
 
 @dataclass
 class DirEntry:
     """Attaches directory information ot a node."""
@@ -89,21 +88,22 @@
         file_filter: list[str],
         *,
         name: str | None = None,
         id: str | None = None,  # pylint: disable=W0622
         classes: str | None = None,
         disabled: bool = False,
     ) -> None:
-
         # identity file system
         if path[0:5] == "s3://":
             self.file_system = "s3"
             self.path = path[4:]  # replace s3:// with / for S3Path
+            self.path_object = S3Path
         else:
             self.path = path
+            self.path_object = Path
             self.file_system = "local"
 
         self.file_filter = file_filter
 
         super().__init__(
             path,
             data=DirEntry(self.path, True, self.file_system),
@@ -132,49 +132,40 @@
 
     def render_label(self, node: TreeNode[DirEntry], base_style: Style, style: Style):
         node_label = node._label.copy()  # pylint: disable=W0212
         node_label.stylize(style)
 
         if node._allow_expand:  # pylint: disable=W0212
             prefix = ("📂 " if node.is_expanded else "📁 ", base_style + TOGGLE_STYLE)
-            node_label.stylize_before(
-                self.get_component_rich_style("directory-tree--folder", partial=True)
-            )
+            node_label.stylize_before(self.get_component_rich_style("directory-tree--folder", partial=True))
         else:
             prefix = (
                 "📄 ",
                 base_style,
             )
             node_label.stylize_before(
                 self.get_component_rich_style("directory-tree--file", partial=True),
             )
             node_label.highlight_regex(
                 r"\..+$",
-                self.get_component_rich_style(
-                    "directory-tree--extension", partial=True
-                ),
+                self.get_component_rich_style("directory-tree--extension", partial=True),
             )
 
         if node_label.plain.startswith("."):
-            node_label.stylize_before(
-                self.get_component_rich_style("directory-tree--hidden")
-            )
+            node_label.stylize_before(self.get_component_rich_style("directory-tree--hidden"))
 
         text = Text.assemble(prefix, node_label)
         return text
 
     def load_directory(self, node: TreeNode[DirEntry]) -> None:
         """Load the selected directory into nodes and show"""
         assert node.data is not None
         node.data.loaded = True
 
-        if self.file_system == "s3":
-            dir_path = S3Path(node.data.path)
-        else:
-            dir_path = Path(node.data.path)
+        dir_path = self.path_object(node.data.path)
 
         directory = sorted(
             list(dir_path.iterdir()),
             key=lambda path: (not path.is_dir(), path.name.lower()),
         )
         for path in directory:
             if path.is_dir() or path.suffix.lower() in self.file_filter:
```

### Comparing `databrowser-0.1.2/PKG-INFO` & `databrowser-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: databrowser
-Version: 0.1.2
+Version: 0.1.3
 Summary: Quick tool to browse and view data files (json,csv,parquet,more) on local disk and s3
 Home-page: https://github.com/jverhoeks/databrowser
 License: MIT
 Author: Jacob Verhoeks
 Author-email: jacob.verhoeks@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pandas (>=1.3.5,<2.0.0)
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: html5lib (>=1.1,<2.0)
+Requires-Dist: lxml (>=4.9.2,<5.0.0)
+Requires-Dist: pandas (>=1.5.2,<2.0.0)
 Requires-Dist: pyarrow (>=5.0.0)
 Requires-Dist: s3fs[boto3] (>=2023.3.0,<2024.0.0)
 Requires-Dist: s3path (>=0.4.1,<0.5.0)
-Requires-Dist: textual (>=0.16.0,<0.17.0)
+Requires-Dist: textual (>=0.16,<0.20)
+Requires-Dist: xlrd (>=2.0.1,<3.0.0)
 Project-URL: Repository, https://github.com/jverhoeks/databrowser
 Description-Content-Type: text/markdown
 
 # databrowser
 
 A easy file browser to view data files.
```

