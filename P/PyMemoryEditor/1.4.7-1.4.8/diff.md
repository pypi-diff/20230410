# Comparing `tmp/PyMemoryEditor-1.4.7.tar.gz` & `tmp/PyMemoryEditor-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMemoryEditor-1.4.7.tar", last modified: Mon Apr 10 01:36:22 2023, max compression
+gzip compressed data, was "PyMemoryEditor-1.4.8.tar", last modified: Mon Apr 10 04:50:35 2023, max compression
```

## Comparing `PyMemoryEditor-1.4.7.tar` & `PyMemoryEditor-1.4.8.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 01:36:22.342990 PyMemoryEditor-1.4.7/
--rw-rw-rw-   0        0        0     1110 2023-04-03 04:22:57.000000 PyMemoryEditor-1.4.7/LICENSE
--rw-rw-rw-   0        0        0     3909 2023-04-10 01:36:22.342990 PyMemoryEditor-1.4.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 01:36:22.327367 PyMemoryEditor-1.4.7/PyMemoryEditor/
--rw-rw-rw-   0        0        0      430 2023-04-10 01:35:55.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/__init__.py
--rw-rw-rw-   0        0        0     5049 2023-04-09 23:42:46.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/open_process.py
-drwxrwxrwx   0        0        0        0 2023-04-10 01:36:22.342990 PyMemoryEditor-1.4.7/PyMemoryEditor/process/
--rw-rw-rw-   0        0        0     1676 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/process/__init__.py
--rw-rw-rw-   0        0        0      717 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/process/errors.py
--rw-rw-rw-   0        0        0      746 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/process/util.py
-drwxrwxrwx   0        0        0        0 2023-04-10 01:36:22.342990 PyMemoryEditor-1.4.7/PyMemoryEditor/win32/
-drwxrwxrwx   0        0        0        0 2023-04-10 01:36:22.342990 PyMemoryEditor-1.4.7/PyMemoryEditor/win32/enums/
--rw-rw-rw-   0        0        0      281 2023-04-09 23:43:15.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/win32/enums/__init__.py
--rw-rw-rw-   0        0        0     2449 2023-04-09 23:42:16.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/win32/enums/memory_allocation_states.py
--rw-rw-rw-   0        0        0     6600 2023-04-09 23:42:16.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/win32/enums/memory_protections.py
--rw-rw-rw-   0        0        0      537 2023-04-09 23:42:46.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/win32/enums/memory_types.py
--rw-rw-rw-   0        0        0     2681 2023-04-09 23:42:46.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/win32/enums/process_operations.py
--rw-rw-rw-   0        0        0      977 2023-04-09 23:41:45.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/win32/enums/standard_access_rights.py
--rw-rw-rw-   0        0        0     7619 2023-04-09 23:42:46.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/win32/functions.py
--rw-rw-rw-   0        0        0     1791 2023-04-09 16:56:11.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/win32/types.py
--rw-rw-rw-   0        0        0      928 2023-04-09 16:07:32.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/win32/util.py
-drwxrwxrwx   0        0        0        0 2023-04-10 01:36:22.342990 PyMemoryEditor-1.4.7/PyMemoryEditor.egg-info/
--rw-rw-rw-   0        0        0     3909 2023-04-10 01:36:22.000000 PyMemoryEditor-1.4.7/PyMemoryEditor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      753 2023-04-10 01:36:22.000000 PyMemoryEditor-1.4.7/PyMemoryEditor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 01:36:22.000000 PyMemoryEditor-1.4.7/PyMemoryEditor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-10 01:36:22.000000 PyMemoryEditor-1.4.7/PyMemoryEditor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-10 01:36:22.000000 PyMemoryEditor-1.4.7/PyMemoryEditor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2640 2023-04-09 22:47:34.000000 PyMemoryEditor-1.4.7/README.md
--rw-rw-rw-   0        0        0       42 2023-04-10 01:36:22.342990 PyMemoryEditor-1.4.7/setup.cfg
--rw-rw-rw-   0        0        0     1727 2023-04-10 01:35:30.000000 PyMemoryEditor-1.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 04:50:35.264084 PyMemoryEditor-1.4.8/
+-rw-rw-rw-   0        0        0     1110 2023-04-03 04:22:57.000000 PyMemoryEditor-1.4.8/LICENSE
+-rw-rw-rw-   0        0        0     4341 2023-04-10 04:50:35.263014 PyMemoryEditor-1.4.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 04:50:35.240442 PyMemoryEditor-1.4.8/PyMemoryEditor/
+-rw-rw-rw-   0        0        0      445 2023-04-10 04:29:19.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/__init__.py
+-rw-rw-rw-   0        0        0     5196 2023-04-10 03:54:13.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/open_process.py
+drwxrwxrwx   0        0        0        0 2023-04-10 04:50:35.247505 PyMemoryEditor-1.4.8/PyMemoryEditor/process/
+-rw-rw-rw-   0        0        0     1676 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/process/__init__.py
+-rw-rw-rw-   0        0        0      717 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/process/errors.py
+-rw-rw-rw-   0        0        0      746 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/process/util.py
+drwxrwxrwx   0        0        0        0 2023-04-10 04:50:35.247505 PyMemoryEditor-1.4.8/PyMemoryEditor/win32/
+drwxrwxrwx   0        0        0        0 2023-04-10 04:50:35.247505 PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/
+-rw-rw-rw-   0        0        0      320 2023-04-10 03:44:13.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/__init__.py
+-rw-rw-rw-   0        0        0     2449 2023-04-09 23:42:16.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/memory_allocation_states.py
+-rw-rw-rw-   0        0        0     6600 2023-04-09 23:42:16.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/memory_protections.py
+-rw-rw-rw-   0        0        0      537 2023-04-10 03:44:01.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/memory_types.py
+-rw-rw-rw-   0        0        0     2681 2023-04-09 23:42:46.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/process_operations.py
+-rw-rw-rw-   0        0        0      221 2023-04-10 03:51:01.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/scan_types.py
+-rw-rw-rw-   0        0        0      977 2023-04-09 23:41:45.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/standard_access_rights.py
+-rw-rw-rw-   0        0        0     7901 2023-04-10 04:29:04.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/win32/functions.py
+-rw-rw-rw-   0        0        0     1791 2023-04-09 16:56:11.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/win32/types.py
+-rw-rw-rw-   0        0        0      928 2023-04-09 16:07:32.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/win32/util.py
+drwxrwxrwx   0        0        0        0 2023-04-10 04:50:35.247505 PyMemoryEditor-1.4.8/PyMemoryEditor.egg-info/
+-rw-rw-rw-   0        0        0     4341 2023-04-10 04:50:35.000000 PyMemoryEditor-1.4.8/PyMemoryEditor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      794 2023-04-10 04:50:35.000000 PyMemoryEditor-1.4.8/PyMemoryEditor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 04:50:35.000000 PyMemoryEditor-1.4.8/PyMemoryEditor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-10 04:50:35.000000 PyMemoryEditor-1.4.8/PyMemoryEditor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-10 04:50:35.000000 PyMemoryEditor-1.4.8/PyMemoryEditor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3072 2023-04-10 04:50:08.000000 PyMemoryEditor-1.4.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-10 04:50:35.264084 PyMemoryEditor-1.4.8/setup.cfg
+-rw-rw-rw-   0        0        0     1727 2023-04-10 01:35:30.000000 PyMemoryEditor-1.4.8/setup.py
```

### Comparing `PyMemoryEditor-1.4.7/LICENSE` & `PyMemoryEditor-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.7/PKG-INFO` & `PyMemoryEditor-1.4.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMemoryEditor
-Version: 1.4.7
+Version: 1.4.8
 Summary: A Python library to edit and track memory of Windows processes (32 bits and 64 bits).
 Home-page: https://github.com/JeanExtreme002/PyMemoryEditor
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: memory virtual writer reader read write override address pointer edit editor process win32 api cheat scan scanner debug trainer
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -64,21 +64,34 @@
     # Getting value from the process memory.
     value = process.read_process_memory(address, int, 4)
 
     # Writing to the process memory.
     process.write_process_memory(address, int, 4, value + 7)
 ```
 
-## Getting memory addresses by a target value:
+# Getting memory addresses by a target value:
 You can look up a value in memory and get the address of all matches, like this:
 ```
 for address process.search_by_value(int, 4, target_value):
     print("Found address:", address)
 ```
 
+## Choosing the comparison method used for scanning:
+There are three options to scan the memory:
+- EXACT_VALUE
+- BIGGER_THAN
+- SMALLER_THAN
+
+The default option is `EXACT_VALUE`, but you can change it at `scan_type` parameter:
+```
+for address process.search_by_value(int, 4, target_value, scan_type = ScanTypesEnum.BIGGER_THAN):
+    print("Found address:", address)
+```
+
+## Extra information from search_by_value method:
 This method also has the `progress_information` parameter that returns a dictionary containing search progress information.
 ```
 for address, info process.search_by_value(int, 4, target_value, progress_information = True):
     template = "Address: 0x{:<10X} | Progress: {:.1f}%"
     progress = info["progress"] * 100
     
     print(template.format(address, progress))
```

### Comparing `PyMemoryEditor-1.4.7/PyMemoryEditor/open_process.py` & `PyMemoryEditor-1.4.8/PyMemoryEditor/open_process.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 from .process import Process
-from PyMemoryEditor.win32.enums import ProcessOperationsEnum
+from PyMemoryEditor.win32.enums import ProcessOperationsEnum, ScanTypesEnum
 
 from .win32.functions import (
     CloseProcessHandle,
     GetProcessHandle,
     ReadProcessMemory,
     SearchAllMemory,
     WriteProcessMemory
@@ -70,34 +70,36 @@
         return CloseProcessHandle(self.__process_handle)
 
     def search_by_value(
         self,
         pytype: Type[T],
         bufflength: int,
         value: Union[bool, int, float, str, bytes],
+        scan_type: ScanTypesEnum = ScanTypesEnum.EXACT_VALUE,
         *,
         progress_information: Optional[bool] = False,
     ) -> Generator[Union[int, Tuple[int, dict]], None, None]:
         """
         Search the whole memory space, accessible to the process,
         for the provided value, returning the found addresses.
 
         :param pytype: type of value to be queried (bool, int, float, str or bytes).
         :param bufflength: value size in bytes (1, 2, 4, 8).
         :param value: value to be queried (bool, int, float, str or bytes).
+        :param scan_type: the way to compare the values.
         :param progress_information: if True, a dictionary with the progress information will be return.
         """
         valid_permissions = [
             ProcessOperationsEnum.PROCESS_ALL_ACCESS.value,
             ProcessOperationsEnum.PROCESS_VM_READ.value
         ]
         if self.__permission.value not in valid_permissions:
             raise PermissionError("The handle does not have permission to read the process memory.")
 
-        return SearchAllMemory(self.__process_handle, pytype, bufflength, value, progress_information)
+        return SearchAllMemory(self.__process_handle, pytype, bufflength, value, scan_type, progress_information)
 
     def read_process_memory(
         self,
         address: int,
         pytype: Type[T],
         bufflength: int
     ) -> T:
```

### Comparing `PyMemoryEditor-1.4.7/PyMemoryEditor/process/__init__.py` & `PyMemoryEditor-1.4.8/PyMemoryEditor/process/__init__.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.7/PyMemoryEditor/process/errors.py` & `PyMemoryEditor-1.4.8/PyMemoryEditor/process/errors.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.7/PyMemoryEditor/process/util.py` & `PyMemoryEditor-1.4.8/PyMemoryEditor/process/util.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.7/PyMemoryEditor/win32/enums/memory_allocation_states.py` & `PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/memory_allocation_states.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.7/PyMemoryEditor/win32/enums/memory_protections.py` & `PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/memory_protections.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.7/PyMemoryEditor/win32/enums/memory_types.py` & `PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/memory_types.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.7/PyMemoryEditor/win32/enums/process_operations.py` & `PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/process_operations.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.7/PyMemoryEditor/win32/enums/standard_access_rights.py` & `PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/standard_access_rights.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.7/PyMemoryEditor/win32/functions.py` & `PyMemoryEditor-1.4.8/PyMemoryEditor/win32/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read more about operations with processes by win32 api here:
 # https://learn.microsoft.com/en-us/windows/win32/api/memoryapi/
 # https://learn.microsoft.com/en-us/windows/win32/api/processthreadsapi/
 # https://learn.microsoft.com/en-us/windows/win32/api/psapi/
 # ...
 
-from .enums import MemoryAllocationStatesEnum, MemoryProtectionsEnum, MemoryTypesEnum
+from .enums import MemoryAllocationStatesEnum, MemoryProtectionsEnum, MemoryTypesEnum, ScanTypesEnum
 from .types import MEMORY_BASIC_INFORMATION, SYSTEM_INFO, WNDENUMPROC
 from .util import get_c_type_of
 from typing import Generator, Optional, Tuple, Type, TypeVar, Union
 
 import ctypes
 import ctypes.wintypes
 
@@ -128,28 +128,30 @@
 
 
 def SearchAllMemory(
     process_handle: int,
     pytype: Type[T],
     bufflength: int,
     value: Union[bool, int, float, str, bytes],
+    scan_type: ScanTypesEnum = ScanTypesEnum.EXACT_VALUE,
     progress_information: Optional[bool] = False,
 ) -> Generator[Union[int, Tuple[int, dict]], None, None]:
     """
     Search the whole memory space, accessible to the process,
     for the provided value, returning the found addresses.
     """
     if pytype not in [bool, int, float, str, bytes]:
         raise ValueError("The type must be bool, int, float, str or bytes.")
 
     # Get the target value as bytes.
     target_value = get_c_type_of(pytype, bufflength)
     target_value.value = value
 
-    target_value = bytes(target_value)
+    target_value_bytes = ctypes.cast(ctypes.byref(target_value), ctypes.POINTER(ctypes.c_byte * bufflength))
+    target_value_bytes = bytes(target_value_bytes.contents)
 
     regions = list()
     memory_total = 0
 
     # Get the memory regions, computing the space size.
     for region in GetMemoryRegions(process_handle):
 
@@ -166,32 +168,30 @@
     # Check each memory region used by the process.
     for region in regions:
         address, size = region["address"], region["size"]
         region_data = (ctypes.c_byte * size)()
 
         # Get data from the region.
         kernel32.ReadProcessMemory(process_handle, ctypes.c_void_p(address), ctypes.byref(region_data), size, None)
-        region_data = bytes(region_data)
 
         # Walk by the returned bytes, searching for the target value.
-        current_index = 0
-        result_index = 0
+        for index in range(size - bufflength):
+            data = region_data[index: index + bufflength]
+            data = bytes((ctypes.c_byte * bufflength)(*data))
+
+            # Compare the values.
+            if scan_type is ScanTypesEnum.EXACT_VALUE and data != target_value_bytes: continue
+            elif scan_type is ScanTypesEnum.BIGGER_THAN and data <= target_value_bytes: continue
+            elif scan_type is ScanTypesEnum.SMALLER_THAN and data >= target_value_bytes: continue
 
-        while current_index < size and result_index != -1:
-            result_index = region_data.find(target_value, current_index)
-
-            # Result equals (-1) means that there is no more match in the region data.
-            if result_index == -1: break
-            current_index = result_index + 1
-
-            found_address = address + result_index
+            found_address = address + index
 
             extra_information = {
                 "memory_total": memory_total,
-                "progress": (checked_memory_size + current_index) / memory_total
+                "progress": (checked_memory_size + index) / memory_total,
             }
             yield (found_address, extra_information) if progress_information else found_address
 
         # Compute the region size to the checked memory size.
         checked_memory_size += size
```

### Comparing `PyMemoryEditor-1.4.7/PyMemoryEditor/win32/types.py` & `PyMemoryEditor-1.4.8/PyMemoryEditor/win32/types.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.7/PyMemoryEditor/win32/util.py` & `PyMemoryEditor-1.4.8/PyMemoryEditor/win32/util.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.7/PyMemoryEditor.egg-info/PKG-INFO` & `PyMemoryEditor-1.4.8/PyMemoryEditor.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMemoryEditor
-Version: 1.4.7
+Version: 1.4.8
 Summary: A Python library to edit and track memory of Windows processes (32 bits and 64 bits).
 Home-page: https://github.com/JeanExtreme002/PyMemoryEditor
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: memory virtual writer reader read write override address pointer edit editor process win32 api cheat scan scanner debug trainer
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -64,21 +64,34 @@
     # Getting value from the process memory.
     value = process.read_process_memory(address, int, 4)
 
     # Writing to the process memory.
     process.write_process_memory(address, int, 4, value + 7)
 ```
 
-## Getting memory addresses by a target value:
+# Getting memory addresses by a target value:
 You can look up a value in memory and get the address of all matches, like this:
 ```
 for address process.search_by_value(int, 4, target_value):
     print("Found address:", address)
 ```
 
+## Choosing the comparison method used for scanning:
+There are three options to scan the memory:
+- EXACT_VALUE
+- BIGGER_THAN
+- SMALLER_THAN
+
+The default option is `EXACT_VALUE`, but you can change it at `scan_type` parameter:
+```
+for address process.search_by_value(int, 4, target_value, scan_type = ScanTypesEnum.BIGGER_THAN):
+    print("Found address:", address)
+```
+
+## Extra information from search_by_value method:
 This method also has the `progress_information` parameter that returns a dictionary containing search progress information.
 ```
 for address, info process.search_by_value(int, 4, target_value, progress_information = True):
     template = "Address: 0x{:<10X} | Progress: {:.1f}%"
     progress = info["progress"] * 100
     
     print(template.format(address, progress))
```

### Comparing `PyMemoryEditor-1.4.7/PyMemoryEditor.egg-info/SOURCES.txt` & `PyMemoryEditor-1.4.8/PyMemoryEditor.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,8 +15,9 @@
 PyMemoryEditor/win32/types.py
 PyMemoryEditor/win32/util.py
 PyMemoryEditor/win32/enums/__init__.py
 PyMemoryEditor/win32/enums/memory_allocation_states.py
 PyMemoryEditor/win32/enums/memory_protections.py
 PyMemoryEditor/win32/enums/memory_types.py
 PyMemoryEditor/win32/enums/process_operations.py
+PyMemoryEditor/win32/enums/scan_types.py
 PyMemoryEditor/win32/enums/standard_access_rights.py
```

### Comparing `PyMemoryEditor-1.4.7/README.md` & `PyMemoryEditor-1.4.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -37,21 +37,34 @@
     # Getting value from the process memory.
     value = process.read_process_memory(address, int, 4)
 
     # Writing to the process memory.
     process.write_process_memory(address, int, 4, value + 7)
 ```
 
-## Getting memory addresses by a target value:
+# Getting memory addresses by a target value:
 You can look up a value in memory and get the address of all matches, like this:
 ```
 for address process.search_by_value(int, 4, target_value):
     print("Found address:", address)
 ```
 
+## Choosing the comparison method used for scanning:
+There are three options to scan the memory:
+- EXACT_VALUE
+- BIGGER_THAN
+- SMALLER_THAN
+
+The default option is `EXACT_VALUE`, but you can change it at `scan_type` parameter:
+```
+for address process.search_by_value(int, 4, target_value, scan_type = ScanTypesEnum.BIGGER_THAN):
+    print("Found address:", address)
+```
+
+## Extra information from search_by_value method:
 This method also has the `progress_information` parameter that returns a dictionary containing search progress information.
 ```
 for address, info process.search_by_value(int, 4, target_value, progress_information = True):
     template = "Address: 0x{:<10X} | Progress: {:.1f}%"
     progress = info["progress"] * 100
     
     print(template.format(address, progress))
```

### Comparing `PyMemoryEditor-1.4.7/setup.py` & `PyMemoryEditor-1.4.8/setup.py`

 * *Files identical despite different names*

