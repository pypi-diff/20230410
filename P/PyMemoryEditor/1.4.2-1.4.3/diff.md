# Comparing `tmp/PyMemoryEditor-1.4.2.tar.gz` & `tmp/PyMemoryEditor-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMemoryEditor-1.4.2.tar", last modified: Sun Apr  9 19:49:45 2023, max compression
+gzip compressed data, was "PyMemoryEditor-1.4.3.tar", last modified: Sun Apr  9 22:45:01 2023, max compression
```

## Comparing `PyMemoryEditor-1.4.2.tar` & `PyMemoryEditor-1.4.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 19:49:45.559958 PyMemoryEditor-1.4.2/
--rw-rw-rw-   0        0        0     1110 2023-04-03 04:22:57.000000 PyMemoryEditor-1.4.2/LICENSE
--rw-rw-rw-   0        0        0     2976 2023-04-09 19:49:45.559958 PyMemoryEditor-1.4.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-09 19:49:45.507680 PyMemoryEditor-1.4.2/PyMemoryEditor/
--rw-rw-rw-   0        0        0      426 2023-04-09 19:49:26.000000 PyMemoryEditor-1.4.2/PyMemoryEditor/__init__.py
--rw-rw-rw-   0        0        0     4750 2023-04-09 19:48:02.000000 PyMemoryEditor-1.4.2/PyMemoryEditor/open_process.py
-drwxrwxrwx   0        0        0        0 2023-04-09 19:49:45.544357 PyMemoryEditor-1.4.2/PyMemoryEditor/process/
--rw-rw-rw-   0        0        0     1676 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.2/PyMemoryEditor/process/__init__.py
--rw-rw-rw-   0        0        0      717 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.2/PyMemoryEditor/process/errors.py
--rw-rw-rw-   0        0        0      746 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.2/PyMemoryEditor/process/util.py
-drwxrwxrwx   0        0        0        0 2023-04-09 19:49:45.559958 PyMemoryEditor-1.4.2/PyMemoryEditor/win32/
--rw-rw-rw-   0        0        0    13242 2023-04-09 18:49:26.000000 PyMemoryEditor-1.4.2/PyMemoryEditor/win32/constants.py
--rw-rw-rw-   0        0        0     2671 2023-04-09 18:35:56.000000 PyMemoryEditor-1.4.2/PyMemoryEditor/win32/enum.py
--rw-rw-rw-   0        0        0     6575 2023-04-09 19:43:23.000000 PyMemoryEditor-1.4.2/PyMemoryEditor/win32/functions.py
--rw-rw-rw-   0        0        0     1791 2023-04-09 16:56:11.000000 PyMemoryEditor-1.4.2/PyMemoryEditor/win32/types.py
--rw-rw-rw-   0        0        0      928 2023-04-09 16:07:32.000000 PyMemoryEditor-1.4.2/PyMemoryEditor/win32/util.py
-drwxrwxrwx   0        0        0        0 2023-04-09 19:49:45.544357 PyMemoryEditor-1.4.2/PyMemoryEditor.egg-info/
--rw-rw-rw-   0        0        0     2976 2023-04-09 19:49:45.000000 PyMemoryEditor-1.4.2/PyMemoryEditor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-04-09 19:49:45.000000 PyMemoryEditor-1.4.2/PyMemoryEditor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 19:49:45.000000 PyMemoryEditor-1.4.2/PyMemoryEditor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-09 19:49:45.000000 PyMemoryEditor-1.4.2/PyMemoryEditor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-09 19:49:45.000000 PyMemoryEditor-1.4.2/PyMemoryEditor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2025 2023-04-03 04:59:56.000000 PyMemoryEditor-1.4.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-09 19:49:45.559958 PyMemoryEditor-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1341 2023-04-03 13:26:23.000000 PyMemoryEditor-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 22:45:01.453164 PyMemoryEditor-1.4.3/
+-rw-rw-rw-   0        0        0     1110 2023-04-03 04:22:57.000000 PyMemoryEditor-1.4.3/LICENSE
+-rw-rw-rw-   0        0        0     3593 2023-04-09 22:45:01.453164 PyMemoryEditor-1.4.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-09 22:45:01.373360 PyMemoryEditor-1.4.3/PyMemoryEditor/
+-rw-rw-rw-   0        0        0      426 2023-04-09 22:14:19.000000 PyMemoryEditor-1.4.3/PyMemoryEditor/__init__.py
+-rw-rw-rw-   0        0        0     4994 2023-04-09 22:20:30.000000 PyMemoryEditor-1.4.3/PyMemoryEditor/open_process.py
+drwxrwxrwx   0        0        0        0 2023-04-09 22:45:01.420968 PyMemoryEditor-1.4.3/PyMemoryEditor/process/
+-rw-rw-rw-   0        0        0     1676 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.3/PyMemoryEditor/process/__init__.py
+-rw-rw-rw-   0        0        0      717 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.3/PyMemoryEditor/process/errors.py
+-rw-rw-rw-   0        0        0      746 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.3/PyMemoryEditor/process/util.py
+drwxrwxrwx   0        0        0        0 2023-04-09 22:45:01.453164 PyMemoryEditor-1.4.3/PyMemoryEditor/win32/
+-rw-rw-rw-   0        0        0    13242 2023-04-09 18:49:26.000000 PyMemoryEditor-1.4.3/PyMemoryEditor/win32/constants.py
+-rw-rw-rw-   0        0        0     2671 2023-04-09 18:35:56.000000 PyMemoryEditor-1.4.3/PyMemoryEditor/win32/enum.py
+-rw-rw-rw-   0        0        0     7512 2023-04-09 22:20:21.000000 PyMemoryEditor-1.4.3/PyMemoryEditor/win32/functions.py
+-rw-rw-rw-   0        0        0     1791 2023-04-09 16:56:11.000000 PyMemoryEditor-1.4.3/PyMemoryEditor/win32/types.py
+-rw-rw-rw-   0        0        0      928 2023-04-09 16:07:32.000000 PyMemoryEditor-1.4.3/PyMemoryEditor/win32/util.py
+drwxrwxrwx   0        0        0        0 2023-04-09 22:45:01.389193 PyMemoryEditor-1.4.3/PyMemoryEditor.egg-info/
+-rw-rw-rw-   0        0        0     3593 2023-04-09 22:45:01.000000 PyMemoryEditor-1.4.3/PyMemoryEditor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-04-09 22:45:01.000000 PyMemoryEditor-1.4.3/PyMemoryEditor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 22:45:01.000000 PyMemoryEditor-1.4.3/PyMemoryEditor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-09 22:45:01.000000 PyMemoryEditor-1.4.3/PyMemoryEditor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-09 22:45:01.000000 PyMemoryEditor-1.4.3/PyMemoryEditor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2642 2023-04-09 22:44:40.000000 PyMemoryEditor-1.4.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-09 22:45:01.453164 PyMemoryEditor-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1341 2023-04-03 13:26:23.000000 PyMemoryEditor-1.4.3/setup.py
```

### Comparing `PyMemoryEditor-1.4.2/LICENSE` & `PyMemoryEditor-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.2/PKG-INFO` & `PyMemoryEditor-1.4.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: PyMemoryEditor
-Version: 1.4.2
-Summary: Process memory reader and writer.
-Home-page: https://github.com/JeanExtreme002/PyMemoryEditor
-Author: Jean Loui Bernard Silva de Jesus
-License: MIT
-Keywords: memory writer write reader read override address pointer peditor process win32 api cheat
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Win32 (MS Windows)
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyMemoryEditor
 
 A Python library developed with [ctypes](https://docs.python.org/3/library/ctypes.html) to manipulate Windows processes (32 bits and 64 bits), <br>
 reading and writing values in the process memory.
 
 [![Python Package](https://github.com/JeanExtreme002/PyMemoryEditor/actions/workflows/python-package.yml/badge.svg)](https://github.com/JeanExtreme002/PyMemoryEditor/actions/workflows/python-package.yml)
 [![Pypi](https://img.shields.io/pypi/v/PyMemoryEditor)](https://pypi.org/project/PyMemoryEditor/)
@@ -33,35 +11,49 @@
 
 # Installing PyMemoryEditor:
 ```
 pip3 install PyMemoryEditor
 ```
 
 # Basic Usage:
-
 Import `PyMemoryEditor` and open a process using the `OpenProcess` class, passing a window title, process name <br>
 or PID as an argument. You can use the context manager to do this.
-
 ```
 from PyMemoryEditor import OpenProcess
 
 with OpenProcess(process_name = "example.exe") as process:
     # Do something...
 ```
 
 After that, use the methods `read_process_memory` and `write_process_memory` to manipulate the process <br>
 memory, passing in the function call the memory address, data type and its size. See the example below:
-
 ```
 from PyMemoryEditor import OpenProcess
 
 title = "Window title of an example program"
 address = 0x0005000C
 
 with OpenProcess(window_title = title) as process:
 
     # Getting value from the process memory.
     value = process.read_process_memory(address, int, 4)
 
     # Writing to the process memory.
     process.write_process_memory(address, int, 4, value + 7)
 ```
+
+## Getting memory addresses by a target value:
+
+You can look up a value in memory and get the address of all matches, like this:
+```
+for address process.search_by_value(int, 4, target_value):
+    print("Found address:", address)
+```
+
+This method also has the `progress_information` parameter that returns a dictionary containing search progress information.
+```
+for address, info process.search_by_value(int, 4, target_value, progress_information = True):
+    template = "Address: 0x{:<10X} | Progress: {:.1f}%"
+    progress = info["progress"] * 100
+    
+    print(template.format(address, progress))
+```
```

### Comparing `PyMemoryEditor-1.4.2/PyMemoryEditor/open_process.py` & `PyMemoryEditor-1.4.3/PyMemoryEditor/open_process.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     CloseProcessHandle,
     GetProcessHandle,
     ReadProcessMemory,
     SearchAllMemory,
     WriteProcessMemory
 )
 
-from typing import List, Optional, Type, TypeVar, Union
+from typing import Generator, Optional, Tuple, Type, TypeVar, Union
 
 
 T = TypeVar("T")
 
 
 class OpenProcess(object):
     """
@@ -69,32 +69,35 @@
         """
         return CloseProcessHandle(self.__process_handle)
 
     def search_by_value(
         self,
         pytype: Type[T],
         bufflength: int,
-        value: Union[bool, int, float, str, bytes]
-    ) -> List[int]:
+        value: Union[bool, int, float, str, bytes],
+        *,
+        progress_information: Optional[bool] = False,
+    ) -> Generator[Union[int, Tuple[int, dict]], None, None]:
         """
         Search the whole memory space, accessible to the process,
         for the provided value, returning the found addresses.
 
         :param pytype: type of value to be queried (bool, int, float, str or bytes).
         :param bufflength: value size in bytes (1, 2, 4, 8).
         :param value: value to be queried (bool, int, float, str or bytes).
+        :param progress_information: if True, a dictionary with the progress information will be return.
         """
         valid_permissions = [
             ProcessOperations.PROCESS_ALL_ACCESS.value,
             ProcessOperations.PROCESS_VM_READ.value
         ]
         if self.__permission.value not in valid_permissions:
             raise PermissionError("The handle does not have permission to read the process memory.")
 
-        return list(SearchAllMemory(self.__process_handle, pytype, bufflength, value))
+        return SearchAllMemory(self.__process_handle, pytype, bufflength, value, progress_information)
 
     def read_process_memory(
         self,
         address: int,
         pytype: Type[T],
         bufflength: int
     ) -> T:
```

### Comparing `PyMemoryEditor-1.4.2/PyMemoryEditor/process/__init__.py` & `PyMemoryEditor-1.4.3/PyMemoryEditor/process/__init__.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.2/PyMemoryEditor/process/errors.py` & `PyMemoryEditor-1.4.3/PyMemoryEditor/process/errors.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.2/PyMemoryEditor/process/util.py` & `PyMemoryEditor-1.4.3/PyMemoryEditor/process/util.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.2/PyMemoryEditor/win32/constants.py` & `PyMemoryEditor-1.4.3/PyMemoryEditor/win32/constants.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.2/PyMemoryEditor/win32/enum.py` & `PyMemoryEditor-1.4.3/PyMemoryEditor/win32/enum.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.2/PyMemoryEditor/win32/functions.py` & `PyMemoryEditor-1.4.3/PyMemoryEditor/win32/functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # https://learn.microsoft.com/en-us/windows/win32/api/processthreadsapi/
 # https://learn.microsoft.com/en-us/windows/win32/api/psapi/
 # ...
 
 from .constants import MEM_COMMIT, MEM_PRIVATE, PAGE_READABLE
 from .types import MEMORY_BASIC_INFORMATION, SYSTEM_INFO, WNDENUMPROC
 from .util import get_c_type_of
-from typing import Generator, Type, TypeVar, Union
+from typing import Generator, Optional, Tuple, Type, TypeVar, Union
 
 import ctypes
 import ctypes.wintypes
 
 # Load the libraries.
 kernel32 = ctypes.windll.LoadLibrary("kernel32.dll")
 user32 = ctypes.windll.LoadLibrary("user32.dll")
@@ -127,51 +127,76 @@
     return str(data.value) if pytype is str else data.value
 
 
 def SearchAllMemory(
     process_handle: int,
     pytype: Type[T],
     bufflength: int,
-    value: Union[bool, int, float, str, bytes]
-) -> Generator[int, None, None]:
+    value: Union[bool, int, float, str, bytes],
+    progress_information: Optional[bool] = False,
+) -> Generator[Union[int, Tuple[int, dict]], None, None]:
     """
     Search the whole memory space, accessible to the process,
     for the provided value, returning the found addresses.
     """
     if pytype not in [bool, int, float, str, bytes]:
         raise ValueError("The type must be bool, int, float, str or bytes.")
 
+    # Get the target value as bytes.
     target_value = get_c_type_of(pytype, bufflength)
     target_value.value = value
 
-    # Check each memory region used by the process.
+    target_value = bytes(target_value)
+
+    regions = list()
+    memory_total = 0
+
+    # Get the memory regions, computing the space size.
     for region in GetMemoryRegions(process_handle):
 
         # Only committed, non-shared and readable memory pages.
         if region["struct"].State != MEM_COMMIT: continue
         if region["struct"].Type != MEM_PRIVATE: continue
         if region["struct"].Protect & PAGE_READABLE == 0: continue
 
+        memory_total += region["size"]
+        regions.append(region)
+
+    checked_memory_size = 0
+
+    # Check each memory region used by the process.
+    for region in regions:
         address, size = region["address"], region["size"]
         region_data = (ctypes.c_byte * size)()
 
         # Get data from the region.
         kernel32.ReadProcessMemory(process_handle, ctypes.c_void_p(address), ctypes.byref(region_data), size, None)
+        region_data = bytes(region_data)
 
         # Walk by the returned bytes, searching for the target value.
-        haystack = bytes(region_data)
-        needle = bytes(target_value)
+        current_index = 0
+        result_index = 0
+
+        while current_index < size and result_index != -1:
+            result_index = region_data.find(target_value, current_index)
 
-        start = 0
-        index = haystack.find(needle, start)
+            # Result equals (-1) means that there is no more match in the region data.
+            if result_index == -1: break
+            current_index = result_index + 1
+
+            found_address = address + result_index
+
+            extra_information = {
+                "memory_total": memory_total,
+                "progress": (checked_memory_size + current_index) / memory_total
+            }
+            yield (found_address, extra_information) if progress_information else found_address
 
-        while start < len(haystack) and index != -1:
-            yield address + index
-            start = index + 1
-            index = haystack.find(needle, start)
+        # Compute the region size to the checked memory size.
+        checked_memory_size += size
 
 
 def WriteProcessMemory(
     process_handle: int,
     address: int,
     pytype: Type[T],
     bufflength: int,
```

### Comparing `PyMemoryEditor-1.4.2/PyMemoryEditor/win32/types.py` & `PyMemoryEditor-1.4.3/PyMemoryEditor/win32/types.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.2/PyMemoryEditor/win32/util.py` & `PyMemoryEditor-1.4.3/PyMemoryEditor/win32/util.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.2/PyMemoryEditor.egg-info/PKG-INFO` & `PyMemoryEditor-1.4.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMemoryEditor
-Version: 1.4.2
+Version: 1.4.3
 Summary: Process memory reader and writer.
 Home-page: https://github.com/JeanExtreme002/PyMemoryEditor
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: memory writer write reader read override address pointer peditor process win32 api cheat
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -33,35 +33,49 @@
 
 # Installing PyMemoryEditor:
 ```
 pip3 install PyMemoryEditor
 ```
 
 # Basic Usage:
-
 Import `PyMemoryEditor` and open a process using the `OpenProcess` class, passing a window title, process name <br>
 or PID as an argument. You can use the context manager to do this.
-
 ```
 from PyMemoryEditor import OpenProcess
 
 with OpenProcess(process_name = "example.exe") as process:
     # Do something...
 ```
 
 After that, use the methods `read_process_memory` and `write_process_memory` to manipulate the process <br>
 memory, passing in the function call the memory address, data type and its size. See the example below:
-
 ```
 from PyMemoryEditor import OpenProcess
 
 title = "Window title of an example program"
 address = 0x0005000C
 
 with OpenProcess(window_title = title) as process:
 
     # Getting value from the process memory.
     value = process.read_process_memory(address, int, 4)
 
     # Writing to the process memory.
     process.write_process_memory(address, int, 4, value + 7)
 ```
+
+## Getting memory addresses by a target value:
+
+You can look up a value in memory and get the address of all matches, like this:
+```
+for address process.search_by_value(int, 4, target_value):
+    print("Found address:", address)
+```
+
+This method also has the `progress_information` parameter that returns a dictionary containing search progress information.
+```
+for address, info process.search_by_value(int, 4, target_value, progress_information = True):
+    template = "Address: 0x{:<10X} | Progress: {:.1f}%"
+    progress = info["progress"] * 100
+    
+    print(template.format(address, progress))
+```
```

### Comparing `PyMemoryEditor-1.4.2/PyMemoryEditor.egg-info/SOURCES.txt` & `PyMemoryEditor-1.4.3/PyMemoryEditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.2/setup.py` & `PyMemoryEditor-1.4.3/setup.py`

 * *Files identical despite different names*

