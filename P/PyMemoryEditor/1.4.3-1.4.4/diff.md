# Comparing `tmp/PyMemoryEditor-1.4.3.tar.gz` & `tmp/PyMemoryEditor-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMemoryEditor-1.4.3.tar", last modified: Sun Apr  9 22:45:01 2023, max compression
+gzip compressed data, was "PyMemoryEditor-1.4.4.tar", last modified: Mon Apr 10 00:03:51 2023, max compression
```

## Comparing `PyMemoryEditor-1.4.3.tar` & `PyMemoryEditor-1.4.4.tar`

### file list

```diff
@@ -1,25 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 22:45:01.453164 PyMemoryEditor-1.4.3/
--rw-rw-rw-   0        0        0     1110 2023-04-03 04:22:57.000000 PyMemoryEditor-1.4.3/LICENSE
--rw-rw-rw-   0        0        0     3593 2023-04-09 22:45:01.453164 PyMemoryEditor-1.4.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-09 22:45:01.373360 PyMemoryEditor-1.4.3/PyMemoryEditor/
--rw-rw-rw-   0        0        0      426 2023-04-09 22:14:19.000000 PyMemoryEditor-1.4.3/PyMemoryEditor/__init__.py
--rw-rw-rw-   0        0        0     4994 2023-04-09 22:20:30.000000 PyMemoryEditor-1.4.3/PyMemoryEditor/open_process.py
-drwxrwxrwx   0        0        0        0 2023-04-09 22:45:01.420968 PyMemoryEditor-1.4.3/PyMemoryEditor/process/
--rw-rw-rw-   0        0        0     1676 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.3/PyMemoryEditor/process/__init__.py
--rw-rw-rw-   0        0        0      717 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.3/PyMemoryEditor/process/errors.py
--rw-rw-rw-   0        0        0      746 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.3/PyMemoryEditor/process/util.py
-drwxrwxrwx   0        0        0        0 2023-04-09 22:45:01.453164 PyMemoryEditor-1.4.3/PyMemoryEditor/win32/
--rw-rw-rw-   0        0        0    13242 2023-04-09 18:49:26.000000 PyMemoryEditor-1.4.3/PyMemoryEditor/win32/constants.py
--rw-rw-rw-   0        0        0     2671 2023-04-09 18:35:56.000000 PyMemoryEditor-1.4.3/PyMemoryEditor/win32/enum.py
--rw-rw-rw-   0        0        0     7512 2023-04-09 22:20:21.000000 PyMemoryEditor-1.4.3/PyMemoryEditor/win32/functions.py
--rw-rw-rw-   0        0        0     1791 2023-04-09 16:56:11.000000 PyMemoryEditor-1.4.3/PyMemoryEditor/win32/types.py
--rw-rw-rw-   0        0        0      928 2023-04-09 16:07:32.000000 PyMemoryEditor-1.4.3/PyMemoryEditor/win32/util.py
-drwxrwxrwx   0        0        0        0 2023-04-09 22:45:01.389193 PyMemoryEditor-1.4.3/PyMemoryEditor.egg-info/
--rw-rw-rw-   0        0        0     3593 2023-04-09 22:45:01.000000 PyMemoryEditor-1.4.3/PyMemoryEditor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-04-09 22:45:01.000000 PyMemoryEditor-1.4.3/PyMemoryEditor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 22:45:01.000000 PyMemoryEditor-1.4.3/PyMemoryEditor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-09 22:45:01.000000 PyMemoryEditor-1.4.3/PyMemoryEditor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-09 22:45:01.000000 PyMemoryEditor-1.4.3/PyMemoryEditor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2642 2023-04-09 22:44:40.000000 PyMemoryEditor-1.4.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-09 22:45:01.453164 PyMemoryEditor-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1341 2023-04-03 13:26:23.000000 PyMemoryEditor-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:03:51.235187 PyMemoryEditor-1.4.4/
+-rw-rw-rw-   0        0        0     1110 2023-04-03 04:22:57.000000 PyMemoryEditor-1.4.4/LICENSE
+-rw-rw-rw-   0        0        0     3591 2023-04-10 00:03:51.235187 PyMemoryEditor-1.4.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 00:03:51.217617 PyMemoryEditor-1.4.4/PyMemoryEditor/
+-rw-rw-rw-   0        0        0      430 2023-04-09 23:45:50.000000 PyMemoryEditor-1.4.4/PyMemoryEditor/__init__.py
+-rw-rw-rw-   0        0        0     5049 2023-04-09 23:42:46.000000 PyMemoryEditor-1.4.4/PyMemoryEditor/open_process.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:03:51.232686 PyMemoryEditor-1.4.4/PyMemoryEditor/process/
+-rw-rw-rw-   0        0        0     1676 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.4/PyMemoryEditor/process/__init__.py
+-rw-rw-rw-   0        0        0      717 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.4/PyMemoryEditor/process/errors.py
+-rw-rw-rw-   0        0        0      746 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.4/PyMemoryEditor/process/util.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:03:51.233683 PyMemoryEditor-1.4.4/PyMemoryEditor/win32/
+-rw-rw-rw-   0        0        0     7619 2023-04-09 23:42:46.000000 PyMemoryEditor-1.4.4/PyMemoryEditor/win32/functions.py
+-rw-rw-rw-   0        0        0     1791 2023-04-09 16:56:11.000000 PyMemoryEditor-1.4.4/PyMemoryEditor/win32/types.py
+-rw-rw-rw-   0        0        0      928 2023-04-09 16:07:32.000000 PyMemoryEditor-1.4.4/PyMemoryEditor/win32/util.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:03:51.230684 PyMemoryEditor-1.4.4/PyMemoryEditor.egg-info/
+-rw-rw-rw-   0        0        0     3591 2023-04-10 00:03:51.000000 PyMemoryEditor-1.4.4/PyMemoryEditor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2023-04-10 00:03:51.000000 PyMemoryEditor-1.4.4/PyMemoryEditor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 00:03:51.000000 PyMemoryEditor-1.4.4/PyMemoryEditor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-10 00:03:51.000000 PyMemoryEditor-1.4.4/PyMemoryEditor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-10 00:03:51.000000 PyMemoryEditor-1.4.4/PyMemoryEditor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2640 2023-04-09 22:47:34.000000 PyMemoryEditor-1.4.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-10 00:03:51.235705 PyMemoryEditor-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1341 2023-04-03 13:26:23.000000 PyMemoryEditor-1.4.4/setup.py
```

### Comparing `PyMemoryEditor-1.4.3/LICENSE` & `PyMemoryEditor-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.3/PKG-INFO` & `PyMemoryEditor-1.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMemoryEditor
-Version: 1.4.3
+Version: 1.4.4
 Summary: Process memory reader and writer.
 Home-page: https://github.com/JeanExtreme002/PyMemoryEditor
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: memory writer write reader read override address pointer peditor process win32 api cheat
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -60,15 +60,14 @@
     value = process.read_process_memory(address, int, 4)
 
     # Writing to the process memory.
     process.write_process_memory(address, int, 4, value + 7)
 ```
 
 ## Getting memory addresses by a target value:
-
 You can look up a value in memory and get the address of all matches, like this:
 ```
 for address process.search_by_value(int, 4, target_value):
     print("Found address:", address)
 ```
 
 This method also has the `progress_information` parameter that returns a dictionary containing search progress information.
```

### Comparing `PyMemoryEditor-1.4.3/PyMemoryEditor/open_process.py` & `PyMemoryEditor-1.4.4/PyMemoryEditor/open_process.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 from .process import Process
-from .win32.enum import ProcessOperations
+from PyMemoryEditor.win32.enums import ProcessOperationsEnum
 
 from .win32.functions import (
     CloseProcessHandle,
     GetProcessHandle,
     ReadProcessMemory,
     SearchAllMemory,
     WriteProcessMemory
@@ -29,15 +29,15 @@
 
     def __init__(
         self,
         *,
         window_title: Optional[str] = None,
         process_name: Optional[str] = None,
         pid: Optional[int] = None,
-        permission: ProcessOperations = ProcessOperations.PROCESS_ALL_ACCESS
+        permission: ProcessOperationsEnum = ProcessOperationsEnum.PROCESS_ALL_ACCESS
     ):
         """
         :param window_title: window title of the target program.
         :param process_name: name of the target process.
         :param pid: process ID.
         :param permission: access mode to the process.
         """
@@ -83,16 +83,16 @@
 
         :param pytype: type of value to be queried (bool, int, float, str or bytes).
         :param bufflength: value size in bytes (1, 2, 4, 8).
         :param value: value to be queried (bool, int, float, str or bytes).
         :param progress_information: if True, a dictionary with the progress information will be return.
         """
         valid_permissions = [
-            ProcessOperations.PROCESS_ALL_ACCESS.value,
-            ProcessOperations.PROCESS_VM_READ.value
+            ProcessOperationsEnum.PROCESS_ALL_ACCESS.value,
+            ProcessOperationsEnum.PROCESS_VM_READ.value
         ]
         if self.__permission.value not in valid_permissions:
             raise PermissionError("The handle does not have permission to read the process memory.")
 
         return SearchAllMemory(self.__process_handle, pytype, bufflength, value, progress_information)
 
     def read_process_memory(
@@ -105,16 +105,16 @@
         Return a value from a memory address.
 
         :param address: target memory address (ex: 0x006A9EC0).
         :param pytype: type of the value to be received (bool, int, float, str or bytes).
         :param bufflength: value size in bytes (1, 2, 4, 8).
         """
         valid_permissions = [
-            ProcessOperations.PROCESS_ALL_ACCESS.value,
-            ProcessOperations.PROCESS_VM_READ.value
+            ProcessOperationsEnum.PROCESS_ALL_ACCESS.value,
+            ProcessOperationsEnum.PROCESS_VM_READ.value
         ]
         if self.__permission.value not in valid_permissions:
             raise PermissionError("The handle does not have permission to read the process memory.")
 
         return ReadProcessMemory(self.__process_handle, address, pytype, bufflength)
 
     def write_process_memory(
@@ -129,14 +129,14 @@
 
         :param address: target memory address (ex: 0x006A9EC0).
         :param pytype: type of value to be written into memory (bool, int, float, str or bytes).
         :param bufflength: value size in bytes (1, 2, 4, 8).
         :param value: value to be written (bool, int, float, str or bytes).
         """
         valid_permissions = [
-            ProcessOperations.PROCESS_ALL_ACCESS.value,
-            ProcessOperations.PROCESS_VM_OPERATION.value | ProcessOperations.PROCESS_VM_WRITE.value
+            ProcessOperationsEnum.PROCESS_ALL_ACCESS.value,
+            ProcessOperationsEnum.PROCESS_VM_OPERATION.value | ProcessOperationsEnum.PROCESS_VM_WRITE.value
         ]
         if self.__permission.value not in valid_permissions:
             raise PermissionError("The handle does not have permission to write to the process memory.")
 
         return WriteProcessMemory(self.__process_handle, address, pytype, bufflength, value)
```

### Comparing `PyMemoryEditor-1.4.3/PyMemoryEditor/process/__init__.py` & `PyMemoryEditor-1.4.4/PyMemoryEditor/process/__init__.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.3/PyMemoryEditor/process/errors.py` & `PyMemoryEditor-1.4.4/PyMemoryEditor/process/errors.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.3/PyMemoryEditor/process/util.py` & `PyMemoryEditor-1.4.4/PyMemoryEditor/process/util.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.3/PyMemoryEditor/win32/functions.py` & `PyMemoryEditor-1.4.4/PyMemoryEditor/win32/functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read more about operations with processes by win32 api here:
 # https://learn.microsoft.com/en-us/windows/win32/api/memoryapi/
 # https://learn.microsoft.com/en-us/windows/win32/api/processthreadsapi/
 # https://learn.microsoft.com/en-us/windows/win32/api/psapi/
 # ...
 
-from .constants import MEM_COMMIT, MEM_PRIVATE, PAGE_READABLE
+from .enums import MemoryAllocationStatesEnum, MemoryProtectionsEnum, MemoryTypesEnum
 from .types import MEMORY_BASIC_INFORMATION, SYSTEM_INFO, WNDENUMPROC
 from .util import get_c_type_of
 from typing import Generator, Optional, Tuple, Type, TypeVar, Union
 
 import ctypes
 import ctypes.wintypes
 
@@ -150,17 +150,17 @@
     regions = list()
     memory_total = 0
 
     # Get the memory regions, computing the space size.
     for region in GetMemoryRegions(process_handle):
 
         # Only committed, non-shared and readable memory pages.
-        if region["struct"].State != MEM_COMMIT: continue
-        if region["struct"].Type != MEM_PRIVATE: continue
-        if region["struct"].Protect & PAGE_READABLE == 0: continue
+        if region["struct"].State != MemoryAllocationStatesEnum.MEM_COMMIT.value: continue
+        if region["struct"].Type != MemoryTypesEnum.MEM_PRIVATE.value: continue
+        if region["struct"].Protect & MemoryProtectionsEnum.PAGE_READABLE.value == 0: continue
 
         memory_total += region["size"]
         regions.append(region)
 
     checked_memory_size = 0
 
     # Check each memory region used by the process.
```

### Comparing `PyMemoryEditor-1.4.3/PyMemoryEditor/win32/types.py` & `PyMemoryEditor-1.4.4/PyMemoryEditor/win32/types.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.3/PyMemoryEditor/win32/util.py` & `PyMemoryEditor-1.4.4/PyMemoryEditor/win32/util.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.3/PyMemoryEditor.egg-info/PKG-INFO` & `PyMemoryEditor-1.4.4/PyMemoryEditor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMemoryEditor
-Version: 1.4.3
+Version: 1.4.4
 Summary: Process memory reader and writer.
 Home-page: https://github.com/JeanExtreme002/PyMemoryEditor
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: memory writer write reader read override address pointer peditor process win32 api cheat
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -60,15 +60,14 @@
     value = process.read_process_memory(address, int, 4)
 
     # Writing to the process memory.
     process.write_process_memory(address, int, 4, value + 7)
 ```
 
 ## Getting memory addresses by a target value:
-
 You can look up a value in memory and get the address of all matches, like this:
 ```
 for address process.search_by_value(int, 4, target_value):
     print("Found address:", address)
 ```
 
 This method also has the `progress_information` parameter that returns a dictionary containing search progress information.
```

### Comparing `PyMemoryEditor-1.4.3/README.md` & `PyMemoryEditor-1.4.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     value = process.read_process_memory(address, int, 4)
 
     # Writing to the process memory.
     process.write_process_memory(address, int, 4, value + 7)
 ```
 
 ## Getting memory addresses by a target value:
-
 You can look up a value in memory and get the address of all matches, like this:
 ```
 for address process.search_by_value(int, 4, target_value):
     print("Found address:", address)
 ```
 
 This method also has the `progress_information` parameter that returns a dictionary containing search progress information.
```

### Comparing `PyMemoryEditor-1.4.3/setup.py` & `PyMemoryEditor-1.4.4/setup.py`

 * *Files identical despite different names*

