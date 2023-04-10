# Comparing `tmp/chelydra-0.0.2.tar.gz` & `tmp/chelydra-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chelydra-0.0.2.tar", last modified: Mon Apr 10 12:18:50 2023, max compression
+gzip compressed data, was "chelydra-0.0.4.tar", last modified: Mon Apr 10 19:29:29 2023, max compression
```

## Comparing `chelydra-0.0.2.tar` & `chelydra-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 12:18:50.237059 chelydra-0.0.2/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)    35148 2023-04-10 12:14:00.000000 chelydra-0.0.2/LICENSE
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       37 2023-04-10 12:14:00.000000 chelydra-0.0.2/MANIFEST.in
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      785 2023-04-10 12:18:50.237059 chelydra-0.0.2/PKG-INFO
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       47 2023-04-10 12:14:00.000000 chelydra-0.0.2/README.md
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       84 2023-04-10 12:14:00.000000 chelydra-0.0.2/pyproject.toml
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       38 2023-04-10 12:18:50.237059 chelydra-0.0.2/setup.cfg
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1106 2023-04-10 12:15:38.000000 chelydra-0.0.2/setup.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 12:18:50.225059 chelydra-0.0.2/src/
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 12:18:50.233059 chelydra-0.0.2/src/chelydra/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 12:14:00.000000 chelydra-0.0.2/src/chelydra/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     6222 2023-04-10 12:14:00.000000 chelydra-0.0.2/src/chelydra/backup.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 12:18:50.237059 chelydra-0.0.2/src/chelydra/tools/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 12:14:00.000000 chelydra-0.0.2/src/chelydra/tools/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1563 2023-04-10 12:14:00.000000 chelydra-0.0.2/src/chelydra/tools/compression.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1268 2023-04-10 12:14:00.000000 chelydra-0.0.2/src/chelydra/tools/cryptography.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1711 2023-04-10 12:14:00.000000 chelydra-0.0.2/src/chelydra/tools/directory.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2419 2023-04-10 12:14:00.000000 chelydra-0.0.2/src/chelydra/version.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 12:18:50.237059 chelydra-0.0.2/src/chelydra.egg-info/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      785 2023-04-10 12:18:50.000000 chelydra-0.0.2/src/chelydra.egg-info/PKG-INFO
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      435 2023-04-10 12:18:50.000000 chelydra-0.0.2/src/chelydra.egg-info/SOURCES.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        1 2023-04-10 12:18:50.000000 chelydra-0.0.2/src/chelydra.egg-info/dependency_links.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        9 2023-04-10 12:18:50.000000 chelydra-0.0.2/src/chelydra.egg-info/top_level.txt
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 12:18:50.237059 chelydra-0.0.2/tests/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       38 2023-04-10 12:17:20.000000 chelydra-0.0.2/tests/test_success.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        5 2023-04-10 12:14:00.000000 chelydra-0.0.2/version.txt
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 19:29:29.050991 chelydra-0.0.4/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)    35148 2023-04-10 12:14:00.000000 chelydra-0.0.4/LICENSE
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       37 2023-04-10 12:14:00.000000 chelydra-0.0.4/MANIFEST.in
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      785 2023-04-10 19:29:29.050991 chelydra-0.0.4/PKG-INFO
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       47 2023-04-10 12:14:00.000000 chelydra-0.0.4/README.md
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       84 2023-04-10 12:14:00.000000 chelydra-0.0.4/pyproject.toml
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       38 2023-04-10 19:29:29.050991 chelydra-0.0.4/setup.cfg
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1106 2023-04-10 12:15:38.000000 chelydra-0.0.4/setup.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 19:29:29.046991 chelydra-0.0.4/src/
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 19:29:29.046991 chelydra-0.0.4/src/chelydra/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 12:14:00.000000 chelydra-0.0.4/src/chelydra/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     6816 2023-04-10 19:26:52.000000 chelydra-0.0.4/src/chelydra/backup.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 19:29:29.050991 chelydra-0.0.4/src/chelydra/tools/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 12:14:00.000000 chelydra-0.0.4/src/chelydra/tools/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1642 2023-04-10 19:05:38.000000 chelydra-0.0.4/src/chelydra/tools/compression.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1268 2023-04-10 12:14:00.000000 chelydra-0.0.4/src/chelydra/tools/cryptography.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2075 2023-04-10 19:05:38.000000 chelydra-0.0.4/src/chelydra/tools/directory.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2419 2023-04-10 12:14:00.000000 chelydra-0.0.4/src/chelydra/version.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 19:29:29.050991 chelydra-0.0.4/src/chelydra.egg-info/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      785 2023-04-10 19:29:29.000000 chelydra-0.0.4/src/chelydra.egg-info/PKG-INFO
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      435 2023-04-10 19:29:29.000000 chelydra-0.0.4/src/chelydra.egg-info/SOURCES.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        1 2023-04-10 19:29:29.000000 chelydra-0.0.4/src/chelydra.egg-info/dependency_links.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        9 2023-04-10 19:29:29.000000 chelydra-0.0.4/src/chelydra.egg-info/top_level.txt
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-10 19:29:29.050991 chelydra-0.0.4/tests/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       38 2023-04-10 12:17:20.000000 chelydra-0.0.4/tests/test_success.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        5 2023-04-10 19:28:51.000000 chelydra-0.0.4/version.txt
```

### Comparing `chelydra-0.0.2/LICENSE` & `chelydra-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chelydra-0.0.2/PKG-INFO` & `chelydra-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chelydra
-Version: 0.0.2
+Version: 0.0.4
 Summary: A zip based backup-restore tool
 Home-page: https://github.com/LostSavannah/chelydra
 Author: Erick Fernando Mora Ramirez
 Author-email: erickfernandomoraramirez@gmail.com
 Project-URL: Bug Tracker, https://dev.moradev.dev/chelydra/issues
 Project-URL: Documentation, https://dev.moradev.dev/chelydra/documentation
 Project-URL: Examples, https://dev.moradev.dev/chelydra/examples
```

### Comparing `chelydra-0.0.2/setup.py` & `chelydra-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `chelydra-0.0.2/src/chelydra/backup.py` & `chelydra-0.0.4/src/chelydra/backup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 ##    GNU General Public License for more details.
 ##
 ##    You should have received a copy of the GNU General Public License
 ##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ##
 ##    mailto:erickfernandomoraramirez@gmail.com
 
-from genericpath import isfile
+import tempfile
 import os
 import json
 import time
 from typing import Dict, List
-from .tools.directory import get_files
+from .tools.directory import delete_file, empty_directory, get_files
 from .tools.cryptography import get_file_hash, get_list_hash
 from .tools.compression import extract_to_folder, update, update_bytes
 from .version import VERSION_MODE_FULL, VERSION_MODE_PART, Version, VersionId
 
 MANIFEST_NAME:str = 'manifest.json'
 
 def get_status_from_path(path:str) -> Dict[str, str]:
@@ -135,23 +135,38 @@
         content = json.dumps(version.get_dict()).encode('latin1')
         filename = f'{version.id.code}.json'
         update_bytes(full_filename, filename, content)
     current_manifest = get_manifest(backup)
     current_manifest['versions'].append(version.get_dict())
     save_manifest(backup, current_manifest)
 
-def restore_into(backup:str, target:str, till_epoch:float = None):
+def restore_into(backup:str, target:str, till_epoch:float = None, empty_target:bool = False):
     if not os.path.exists(target):
         os.makedirs(target)
     elif os.path.isfile(target):
         raise Exception(f"Can't restore into file: {target}")
     files:Dict[str, Version] = {}
+    deletions:List[str] = []
     for version in get_restore_order(backup, till_epoch):
         for file in version.changes:
             files[file] = version
+            if file in deletions:
+                deletions.remove(file)
         for deletion in version.deletions:
             del files[deletion]
+            if deletion not in deletions:
+                deletions.append(deletion)
+    if empty_target:
+        empty_directory(target)
     for entry in files:
         compressed_file_name = files[entry].get_filename('.zip')
         fullname = os.sep.join([backup, compressed_file_name])
         extract_to_folder(fullname, entry, target)
-    
+    for deletion in deletions:
+        delete_file(target, deletion)
+
+def syncronize(folders:List[str], source:str, backup:str):
+    if create_version(source, backup):
+        for target in folders:
+            if target == source:
+                continue
+            restore_into(backup, target, empty_target=True)
```

### Comparing `chelydra-0.0.2/src/chelydra/tools/compression.py` & `chelydra-0.0.4/src/chelydra/tools/compression.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 ##    GNU General Public License for more details.
 ##
 ##    You should have received a copy of the GNU General Public License
 ##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ##
 ##    mailto:erickfernandomoraramirez@gmail.com
 
+from dataclasses import replace
 from zipfile import ZipFile
 
 def update(compressed_file_name:str, entry_name:str, absolute_filename:str):
     with open(absolute_filename, 'rb') as fi:
         update_bytes(compressed_file_name, entry_name, fi.read())
 
 def update_bytes(compressed_file_name:str, entry_name:str, data:bytes):
@@ -29,8 +30,9 @@
 
 def get_entries(compressed_file_name:str):
     zipfile = ZipFile(compressed_file_name, 'r')
     for zipinfo in zipfile.filelist:
         yield zipinfo.filename
 
 def extract_to_folder(compressed_file_name:str, entry_name:str, folder_name:str):
+    entry_name = entry_name.replace('\\', '/')
     ZipFile(compressed_file_name, 'r').extract(entry_name, folder_name)
```

### Comparing `chelydra-0.0.2/src/chelydra/tools/cryptography.py` & `chelydra-0.0.4/src/chelydra/tools/cryptography.py`

 * *Files identical despite different names*

### Comparing `chelydra-0.0.2/src/chelydra/tools/directory.py` & `chelydra-0.0.4/src/chelydra/tools/directory.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,8 +38,19 @@
 
 def get_files(path, ignore:List[str] = None):
     for directory in get_directories(path, ignore):
         if os.path.isfile(directory):
             yield directory
 
 def delete_file(path:str, filename:str):
-    os.remove(os.sep.join([path, filename]))
+    full:str = os.sep.join([path, filename])
+    if os.path.exists(full) and os.path.isfile(full):
+        os.remove(full)
+
+def empty_directory(path:str):
+    for f in os.listdir(path):
+        fullpath = os.sep.join([path, f])
+        if os.path.isdir(fullpath):
+            empty_directory(fullpath)
+            os.removedirs(fullpath)
+        elif os.path.isfile(fullpath):
+            os.remove(fullpath)
```

### Comparing `chelydra-0.0.2/src/chelydra/version.py` & `chelydra-0.0.4/src/chelydra/version.py`

 * *Files identical despite different names*

### Comparing `chelydra-0.0.2/src/chelydra.egg-info/PKG-INFO` & `chelydra-0.0.4/src/chelydra.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chelydra
-Version: 0.0.2
+Version: 0.0.4
 Summary: A zip based backup-restore tool
 Home-page: https://github.com/LostSavannah/chelydra
 Author: Erick Fernando Mora Ramirez
 Author-email: erickfernandomoraramirez@gmail.com
 Project-URL: Bug Tracker, https://dev.moradev.dev/chelydra/issues
 Project-URL: Documentation, https://dev.moradev.dev/chelydra/documentation
 Project-URL: Examples, https://dev.moradev.dev/chelydra/examples
```

