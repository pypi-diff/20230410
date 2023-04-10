# Comparing `tmp/ddir-2.0.1-py3-none-any.whl.zip` & `tmp/ddir-2.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 13595 bytes, number of entries: 13
--rw-r--r--  2.0 unx     4924 b- defN 23-Apr-08 14:53 ddir/__init__.py
--rw-r--r--  2.0 unx     4483 b- defN 23-Apr-08 14:53 ddir/__main__.py
--rw-r--r--  2.0 unx      156 b- defN 23-Apr-08 14:53 ddir/__version__.py
--rw-r--r--  2.0 unx    11304 b- defN 23-Apr-08 14:53 ddir/diff.py
--rw-r--r--  2.0 unx      665 b- defN 23-Apr-08 14:53 ddir/initialize.py
--rw-r--r--  2.0 unx     2570 b- defN 23-Apr-08 14:53 ddir/legacy.py
--rw-r--r--  2.0 unx     5792 b- defN 23-Apr-08 14:53 ddir/target.py
--rw-r--r--  2.0 unx      191 b- defN 23-Apr-08 14:53 ddir-2.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3535 b- defN 23-Apr-08 14:53 ddir-2.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-08 14:53 ddir-2.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 23-Apr-08 14:53 ddir-2.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Apr-08 14:53 ddir-2.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      968 b- defN 23-Apr-08 14:53 ddir-2.0.1.dist-info/RECORD
-13 files, 34729 bytes uncompressed, 12005 bytes compressed:  65.4%
+Zip file size: 13844 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     4924 b- defN 23-Apr-10 16:17 ddir/__init__.py
+-rw-r--r--  2.0 unx     4445 b- defN 23-Apr-10 16:17 ddir/__main__.py
+-rw-r--r--  2.0 unx      156 b- defN 23-Apr-10 16:18 ddir/__version__.py
+-rw-r--r--  2.0 unx    11824 b- defN 23-Apr-10 16:17 ddir/diff.py
+-rw-r--r--  2.0 unx      668 b- defN 23-Apr-10 16:17 ddir/initialize.py
+-rw-r--r--  2.0 unx     2600 b- defN 23-Apr-10 16:17 ddir/legacy.py
+-rw-r--r--  2.0 unx     5828 b- defN 23-Apr-10 16:17 ddir/target.py
+-rw-r--r--  2.0 unx      191 b- defN 23-Apr-10 16:18 ddir-2.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3535 b- defN 23-Apr-10 16:18 ddir-2.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 16:18 ddir-2.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 23-Apr-10 16:18 ddir-2.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Apr-10 16:18 ddir-2.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      968 b- defN 23-Apr-10 16:18 ddir-2.0.2.dist-info/RECORD
+13 files, 35280 bytes uncompressed, 12254 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: ddir/legacy.py
 Comment: 
 
 Filename: ddir/target.py
 Comment: 
 
-Filename: ddir-2.0.1.dist-info/LICENSE
+Filename: ddir-2.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: ddir-2.0.1.dist-info/METADATA
+Filename: ddir-2.0.2.dist-info/METADATA
 Comment: 
 
-Filename: ddir-2.0.1.dist-info/WHEEL
+Filename: ddir-2.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: ddir-2.0.1.dist-info/entry_points.txt
+Filename: ddir-2.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: ddir-2.0.1.dist-info/top_level.txt
+Filename: ddir-2.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: ddir-2.0.1.dist-info/RECORD
+Filename: ddir-2.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ddir/__main__.py

```diff
@@ -61,45 +61,44 @@
     - 0: skip
     - 1: apply (type dependent, see below)
     - 2: choose manually
 """)
 
 
 def _handle_init() -> None:
-    initialize.initialize(_CURRENT_DIRECTORY)
+    initialize.initialize(_DDIR)
 
 
 def _handle_version() -> None:
     print(f'ddir {__version__.VERSION}')
 
 
 @_is_ddir_controlled
 def _handle_diff_create(name: str) -> None:
     with open(sep.join([_DDIR, 'ddir.json']), 'r', encoding=ENCODING) as file:
         config = GlobalConfiguration.from_dict(loads(file.read()))
 
         _target = target.load(_TARGET_D, name)
-        print(_target)
         with diff.DiffFileCreator(sep.join([_TARGET_D, _target.hash.value])) as file:
             diff.create(file, _CURRENT_DIRECTORY, _target.path, _target.fast_mode, config.ignore)
 
 
 @_is_ddir_controlled
 def _handle_diff_resolve(name: str, modes: tuple) -> None:
     _target = target.load(_TARGET_D, name)
-    diff_file = diff.ask_for_diff(_target)
+    diff_file = diff.ask_for(_target)
 
     with diff.DiffFileReader(diff_file.path) as parser:
         diff.resolve(parser, tuple(int(c) for c in modes))
 
 
 @_is_ddir_controlled
 def _handle_diff_list(name: str) -> None:
     _target = target.load(_TARGET_D, name)
-    diffs = diff.ask_for_diff(_target.this)
+    diffs = diff.load_diffs_meta(_target.this)
 
     print(f'Diffs for target {_target.name}:')
     for index, _diff in enumerate(diffs):
         print(f'  {index + 1}: {_diff.creation}')
 
 
 @_is_ddir_controlled
```

## ddir/__version__.py

```diff
@@ -1,7 +1,7 @@
 """
 This module holds the version of ddir.
 
 It contains a placeholder for the version number, which is replaced by the build script.
 """
 
-VERSION = '2.0.1'
+VERSION = '2.0.2'
```

## ddir/diff.py

```diff
@@ -7,19 +7,20 @@
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 from datetime import date
 from enum import Enum
 from hashlib import md5
+from math import ceil
 from os import sep, listdir, mkdir, stat
 from os.path import exists, isfile, isdir
 from random import randint as rand
 from re import match
-from shutil import copy as cp
+from shutil import copy2 as cp
 from time import localtime, strftime
 from typing import List
 
 from ddir import ENCODING, ProgramError
 from ddir.target import Target
 
 
@@ -76,15 +77,15 @@
 
     def description(self) -> str:
         """Returns the description of that `DiffType`."""
         return self.value[2]
 
     # pylint: disable=E0307
     def __str__(self) -> str:
-        match self.value.index():
+        match self.value[0]:
             case 0: return 'positive'
             case 1: return 'negative'
             case 2: return 'newer'
             case 3: return 'older'
             case _: return 'unknown'
 
 
@@ -195,15 +196,15 @@
             creation = stat(diff).st_mtime  # re.sub('-\d*.diff', '', element)
             meta = Meta(diff, strftime('%Y-%m-%d %H:%M:%S', localtime(creation)))
             diffs.append(meta)
 
     return sorted(diffs, key=lambda diff: diff.creation)
 
 
-def ask_for_diff(target: Target) -> Meta:
+def ask_for(target: Target) -> Meta:
     """Loads all diffs of a target and asks for user input to choose a diff."""
 
     diffs = load_diffs_meta(target.this)
 
     print(f'Diffs for target {target.name}:')
     for index, diff in enumerate(diffs):
         print(f'  {index + 1}: {diff.creation}')
@@ -254,21 +255,28 @@
 
 
 def _create_for_file(diff: DiffFileCreator, source: str, target: str, fast: bool) -> None:
     if not exists(target):
         print(f'file not in target: {source} {target}')
         diff.add_diff(Diff(DiffType.POSITIVE, 'f', source, target))
     else:
-        source_last_changed = stat(source).st_mtime
-        target_last_changed = stat(target).st_mtime
-
-        if source_last_changed > target_last_changed:
+        # It may occur that the source modification time has a higher/lower
+        # precision than the target modification time. As rounding to e.g. 2
+        # decimal places may lead to a difference of .01, we round to the
+        # ceiling to avoid false positives.
+        source_last_changed = ceil(stat(source).st_mtime)
+        target_last_changed = ceil(stat(target).st_mtime)
+
+        # Here, we check if the files are different by more than one second.
+        # This is because on some file systems, the modification time may be
+        # different by one second, even if the file has not been changed.
+        if source_last_changed - target_last_changed > 1:
             print(f'files differ: {source} is newer than {target}')
             diff.add_diff(Diff(DiffType.NEWER, 'f', source, target))
-        elif target_last_changed > source_last_changed:
+        elif target_last_changed - source_last_changed > 1:
             print(f'files differ: {target} is newer than {source}')
             diff.add_diff(Diff(DiffType.OLDER, 'f', source, target))
         elif not fast:
             with open(source, 'rb', encoding=ENCODING) as source_file, \
                     open(target, 'rb', encoding=ENCODING) as target_file:
                 source_md5 = md5(source_file.read()).hexdigest()
                 target_md5 = md5(target_file.read()).hexdigest()
@@ -311,45 +319,45 @@
     print(f'    type: {str(diff.type)}')
     print(f'    flag: {diff.flag}')
     print(f'    source: {diff.source}')
     print(f'    target: {diff.target}')
     print()
     print(f'Applying will {diff.type.description()}')
 
-    selection = input('Do you want to apply this diff? (y/N)')
+    selection = input('Do you want to apply this diff? (y/N) ')
     if selection == 'y':
         return 'y'
 
     return 'n'
 
 
-def _get_mode_from_selection(mode: int, _diff: Diff) -> int:
-    if mode == 2 and _get_mode_selection(_diff) == 'y':
+def _get_mode_from_selection(mode: int, diff: Diff) -> int:
+    if mode == 2 and _get_mode_selection(diff) == 'y':
         return 1
 
     return mode
 
 
-def _copy_file_or_directory(source: str, _target: str) -> None:
+def _copy_file_or_directory(source: str, target: str) -> None:
     if isfile(source):
-        cp(source, _target)
-        print(f'Copied/overridden file {source} to {_target}')
+        cp(source, target)
+        print(f'Copied/overridden file {source} to {target}')
     elif isdir(source):
-        mkdir(_target)
+        mkdir(target)
 
         for file in listdir(source):
             abs_target = sep.join([source, file])
-            abs_source = sep.join([_target, file])
+            abs_source = sep.join([target, file])
 
             cp(abs_target, abs_source)
-            print(f'Copied/overridden file {abs_target} to {_target}')
+            print(f'Copied/overridden file {abs_target} to {target}')
     else:
         print(f'{source} does not exist anymore, thus is skipped')
 
 
-def _copy_with_mode_check(mode: int, _diff: Diff, source: str, _target: str) -> None:
-    mode = _get_mode_from_selection(mode, _diff)
+def _copy_with_mode_check(mode: int, diff: Diff, source: str, target: str) -> None:
+    mode = _get_mode_from_selection(mode, diff)
 
     if mode == 0:
-        print(f'Skip copy/override {source} to/with {_target}')
+        print(f'Skip copy/override {source} to/with {target}')
     elif mode == 1:
-        _copy_file_or_directory(source, _target)
+        _copy_file_or_directory(source, target)
```

## ddir/initialize.py

```diff
@@ -3,20 +3,20 @@
 from json import dumps
 from os import makedirs as mkdir, sep
 from os.path import exists
 
 from ddir import API_VERSION, ENCODING, GlobalConfiguration, ProgramError
 
 
-def initialize(directory: str) -> None:
+def initialize(ddir: str) -> None:
     """Initializes an empty ddir source."""
-    if exists(directory):
-        raise ProgramError.is_ddir(directory)
+    if exists(ddir):
+        raise ProgramError.is_ddir(ddir)
 
-    ddir = sep.join([directory, '.ddir'])
     mkdir(ddir)
 
-    raw_config = dumps(GlobalConfiguration(API_VERSION, ['.ddir', '.DS_Store']).to_json())
+    raw_config = dumps(GlobalConfiguration(API_VERSION, ['.ddir', '.DS_Store']).to_json(),
+                        indent = 2, separators=(',', ': '))
     with open(sep.join([ddir, 'ddir.json']), 'w', encoding=ENCODING) as file:
         file.write(raw_config)
 
     print('Initialized empty ddir source.')
```

## ddir/legacy.py

```diff
@@ -3,15 +3,15 @@
 
 Its purpose is to migrate old source configurations to the latest version.
 """
 
 from json import dumps
 from os import sep, listdir, remove as rm
 from os.path import exists, isfile
-from shutil import copy as cp
+from shutil import copy2 as cp
 
 from ddir import API_VERSION, ENCODING, GlobalConfiguration, target
 
 def migrate(path: str, ddir: str, target_d: str) -> None:
     """Determines the current API version and upgrades to the latest one."""
 
     if exists(ddir) and not exists(target_d):
@@ -53,13 +53,14 @@
                 print('Fast mode not defined, so inferring no fast mode')
 
             _target = target.create(target_d, 'default', destination, fast_mode)
             for element in listdir(ddir):
                 diff = sep.join([ddir, element])
                 if isfile(diff) and element.endswith('.diff'):
                     cp(diff, _target.this)
+                    rm(diff)
                     print(f'Copied diff {element} to {_target.this}')
 
             rm(destination_file)
             print(f'Created target {_target.name}')
     else:
         print('There was no destination set, so no target is created')
```

## ddir/target.py

```diff
@@ -160,15 +160,15 @@
     )
 
     if exists(target.this):
         raise ProgramError.target_already_exists(target.name)
 
     mkdir(target.this)
     with open(sep.join([target.this, 'target.json']), 'w', encoding=ENCODING) as file:
-        file.write(dumps(target.to_json()))
+        file.write(dumps(target.to_json(), indent = 2, separators=(',', ': ')))
 
     return target
 
 
 def create_interactive(target_d: str) -> Target:
     """Creates a new target in an interactive mode."""
```

## Comparing `ddir-2.0.1.dist-info/METADATA` & `ddir-2.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddir
-Version: 2.0.1
+Version: 2.0.2
 Summary: Diff a directory and sync changes.
 License: Public Domain
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ddir
```

