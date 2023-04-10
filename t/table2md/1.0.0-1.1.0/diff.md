# Comparing `tmp/table2md-1.0.0.tar.gz` & `tmp/table2md-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "table2md-1.0.0.tar", last modified: Sun Nov 21 17:23:59 2021, max compression
+gzip compressed data, was "table2md-1.1.0.tar", last modified: Mon Apr 10 12:36:29 2023, max compression
```

## Comparing `table2md-1.0.0.tar` & `table2md-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 mikolaj   (1000) users      (985)        0 2021-11-21 17:23:59.966780 table2md-1.0.0/
--rw-r--r--   0 mikolaj   (1000) users      (985)     1076 2021-11-21 15:08:16.000000 table2md-1.0.0/LICENSE
--rw-r--r--   0 mikolaj   (1000) users      (985)     6670 2021-11-21 17:23:59.966780 table2md-1.0.0/PKG-INFO
--rw-r--r--   0 mikolaj   (1000) users      (985)     6107 2021-11-21 17:15:56.000000 table2md-1.0.0/README.md
--rw-r--r--   0 mikolaj   (1000) users      (985)       90 2021-11-21 15:32:57.000000 table2md-1.0.0/pyproject.toml
--rw-r--r--   0 mikolaj   (1000) users      (985)      767 2021-11-21 17:23:59.966780 table2md-1.0.0/setup.cfg
-drwxr-xr-x   0 mikolaj   (1000) users      (985)        0 2021-11-21 17:23:59.966780 table2md-1.0.0/table2md/
--rw-r--r--   0 mikolaj   (1000) users      (985)     7135 2021-11-21 17:22:03.000000 table2md-1.0.0/table2md/__init__.py
-drwxr-xr-x   0 mikolaj   (1000) users      (985)        0 2021-11-21 17:23:59.966780 table2md-1.0.0/table2md.egg-info/
--rw-r--r--   0 mikolaj   (1000) users      (985)     6670 2021-11-21 17:23:59.000000 table2md-1.0.0/table2md.egg-info/PKG-INFO
--rw-r--r--   0 mikolaj   (1000) users      (985)      222 2021-11-21 17:23:59.000000 table2md-1.0.0/table2md.egg-info/SOURCES.txt
--rw-r--r--   0 mikolaj   (1000) users      (985)        1 2021-11-21 17:23:59.000000 table2md-1.0.0/table2md.egg-info/dependency_links.txt
--rw-r--r--   0 mikolaj   (1000) users      (985)       45 2021-11-21 17:23:59.000000 table2md-1.0.0/table2md.egg-info/requires.txt
--rw-r--r--   0 mikolaj   (1000) users      (985)        9 2021-11-21 17:23:59.000000 table2md-1.0.0/table2md.egg-info/top_level.txt
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-04-10 12:36:29.157340 table2md-1.1.0/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1076 2021-11-21 15:08:16.000000 table2md-1.1.0/LICENSE
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     6846 2023-04-10 12:36:29.157340 table2md-1.1.0/PKG-INFO
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     6303 2023-04-10 12:27:09.000000 table2md-1.1.0/README.md
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       90 2021-11-21 15:32:57.000000 table2md-1.1.0/pyproject.toml
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      767 2023-04-10 12:36:29.157340 table2md-1.1.0/setup.cfg
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-04-10 12:36:29.157340 table2md-1.1.0/table2md/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     7690 2023-04-10 12:31:37.000000 table2md-1.1.0/table2md/__init__.py
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-04-10 12:36:29.157340 table2md-1.1.0/table2md.egg-info/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     6846 2023-04-10 12:36:29.000000 table2md-1.1.0/table2md.egg-info/PKG-INFO
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      245 2023-04-10 12:36:29.000000 table2md-1.1.0/table2md.egg-info/SOURCES.txt
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        1 2023-04-10 12:36:29.000000 table2md-1.1.0/table2md.egg-info/dependency_links.txt
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       45 2023-04-10 12:36:29.000000 table2md-1.1.0/table2md.egg-info/requires.txt
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        9 2023-04-10 12:36:29.000000 table2md-1.1.0/table2md.egg-info/top_level.txt
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-04-10 12:36:29.157340 table2md-1.1.0/tests/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     5094 2021-11-21 15:48:38.000000 table2md-1.1.0/tests/test_table2md.py
```

### Comparing `table2md-1.0.0/LICENSE` & `table2md-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `table2md-1.0.0/PKG-INFO` & `table2md-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: table2md
-Version: 1.0.0
+Version: 1.1.0
 Summary: Print tabular data in markdown format
 Home-page: https://github.com/MKuranowski/table2md
 Author: Mikołaj Kuranowski
 Author-email: mkuranowski+pypackages@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/MKuranowski/table2md/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -130,14 +129,20 @@
 - **markdown_table.print(end: str = "", file: SupportsWrite[str] = sys.stdout, flush: bool = False) -> None**:  
     Validates the table, and then prints it.
     'end', 'file' and 'flush' arguments are passed
     through to the builtin print function.  
     Pleas note that the serialized table already has a newline at the end,
     so `end="\n"` is not necessary.
 
+- **markdown_table.display() -> None**:  
+    Validates the table, then tries to pretty-print
+    using IPython.display.display_markdown.
+
+    If that is not available, the same as table.print()
+
 - **MarkdownTable.from_2d_iterable(iters: Iterable[Iterable[Any]]) -> MarkdownTable**:  
     Initializes the table from a 2D iterable.
     Every cell is saved by calling `str(cell)`.
     If provided with a 2D list, those lists are copied
     (this is different to the behavior from the constructor).
 
 - **MarkdownTable.from_dicts(dicts: Iterable[Mapping[str, Any]]) -> MarkdownTable:**:  
@@ -189,9 +194,7 @@
     Anything with a `_fields` property, which is an iterable of strings
     representing field names; that is itself iterable.
 
 - **_Serializable**:
     Anything with a `_fields` property, which is an iterable of strings
     representing field names; and with a `serialize() -> Iterable[str]` method
     which returns all the held field values as strings.
-
-
```

### Comparing `table2md-1.0.0/README.md` & `table2md-1.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -113,14 +113,20 @@
 - **markdown_table.print(end: str = "", file: SupportsWrite[str] = sys.stdout, flush: bool = False) -> None**:  
     Validates the table, and then prints it.
     'end', 'file' and 'flush' arguments are passed
     through to the builtin print function.  
     Pleas note that the serialized table already has a newline at the end,
     so `end="\n"` is not necessary.
 
+- **markdown_table.display() -> None**:  
+    Validates the table, then tries to pretty-print
+    using IPython.display.display_markdown.
+
+    If that is not available, the same as table.print()
+
 - **MarkdownTable.from_2d_iterable(iters: Iterable[Iterable[Any]]) -> MarkdownTable**:  
     Initializes the table from a 2D iterable.
     Every cell is saved by calling `str(cell)`.
     If provided with a 2D list, those lists are copied
     (this is different to the behavior from the constructor).
 
 - **MarkdownTable.from_dicts(dicts: Iterable[Mapping[str, Any]]) -> MarkdownTable:**:
```

### Comparing `table2md-1.0.0/setup.cfg` & `table2md-1.1.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = table2md
-version = 1.0.0
+version = 1.1.0
 author = Mikołaj Kuranowski
 author_email = mkuranowski+pypackages@gmail.com
 license = MIT
 license_file = LICENSE
 description = Print tabular data in markdown format
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `table2md-1.0.0/table2md/__init__.py` & `table2md-1.1.0/table2md/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,37 @@
-# © Copyright 2021 Mikołaj Kuranowski
+# © Copyright 2021, 2023 Mikołaj Kuranowski
 # SPDX-License-Identifier: MIT
 
 import sys
 from typing import TYPE_CHECKING, Any, Iterable, Iterator, List, Mapping
 
 if sys.version_info < (3, 8):
     from typing_extensions import Protocol
 else:
     from typing import Protocol
 
 if TYPE_CHECKING:
     from _typeshed import SupportsWrite
 
 
+try:
+    from IPython.display import display_markdown  # type: ignore
+    has_display_markdown = True
+except ImportError:
+    has_display_markdown = False
+
+
 __title__ = "table2md"
 __description__ = "Print tabular data in markdown format"
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 __url__ = "https://github.com/MKuranowski/table2md"
 __author__ = "Mikołaj Kuranowski"
 __email__ = "mkuranowski+pypackages@gmail.com"
 
-__copyright__ = "© Copyright 2021 Mikołaj Kuranowski"
+__copyright__ = "© Copyright 2021, 2023 Mikołaj Kuranowski"
 __license__ = "MIT"
 
 
 class _NamedTupleLike(Protocol):
     """_NamedTupleLike describes the interface accepted by
     MarkdownTable.from_namedtuples.
 
@@ -132,15 +139,27 @@
         'end', 'file' and 'flush' arguments are passed
         through to the builtin print function.
 
         Pleas note that the serialized table already has a newline at the end,
         so `end="\n"` is not necessary.
         """
         self.validate()
-        print(str(self), end=end, file=file, flush=flush)
+        print(str(self), end=end, file=file, flush=flush)  # type: ignore
+
+    def display(self) -> None:
+        """Validates the table, then tries to pretty-print
+        using IPython.display.display_markdown.
+
+        If that is not available, the same as table.print()
+        """
+        self.validate()
+        if has_display_markdown:
+            display_markdown(str(self), raw=True)
+        else:
+            print(str(self), end="")
 
     @classmethod
     def from_2d_iterable(cls, iters: Iterable[Iterable[Any]]) -> "MarkdownTable":
         """Initializes the table from a 2D iterable.
         Every cell is saved by calling `str(cell)`.
         If provided with a 2D list, those lists are copied
         (this is different to the behavior from the constructor).
```

### Comparing `table2md-1.0.0/table2md.egg-info/PKG-INFO` & `table2md-1.1.0/table2md.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: table2md
-Version: 1.0.0
+Version: 1.1.0
 Summary: Print tabular data in markdown format
 Home-page: https://github.com/MKuranowski/table2md
 Author: Mikołaj Kuranowski
 Author-email: mkuranowski+pypackages@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/MKuranowski/table2md/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -130,14 +129,20 @@
 - **markdown_table.print(end: str = "", file: SupportsWrite[str] = sys.stdout, flush: bool = False) -> None**:  
     Validates the table, and then prints it.
     'end', 'file' and 'flush' arguments are passed
     through to the builtin print function.  
     Pleas note that the serialized table already has a newline at the end,
     so `end="\n"` is not necessary.
 
+- **markdown_table.display() -> None**:  
+    Validates the table, then tries to pretty-print
+    using IPython.display.display_markdown.
+
+    If that is not available, the same as table.print()
+
 - **MarkdownTable.from_2d_iterable(iters: Iterable[Iterable[Any]]) -> MarkdownTable**:  
     Initializes the table from a 2D iterable.
     Every cell is saved by calling `str(cell)`.
     If provided with a 2D list, those lists are copied
     (this is different to the behavior from the constructor).
 
 - **MarkdownTable.from_dicts(dicts: Iterable[Mapping[str, Any]]) -> MarkdownTable:**:  
@@ -189,9 +194,7 @@
     Anything with a `_fields` property, which is an iterable of strings
     representing field names; that is itself iterable.
 
 - **_Serializable**:
     Anything with a `_fields` property, which is an iterable of strings
     representing field names; and with a `serialize() -> Iterable[str]` method
     which returns all the held field values as strings.
-
-
```

