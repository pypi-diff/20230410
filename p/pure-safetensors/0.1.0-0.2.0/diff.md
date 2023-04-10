# Comparing `tmp/pure_safetensors-0.1.0.tar.gz` & `tmp/pure_safetensors-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure_safetensors-0.1.0.tar", last modified: Sat Apr  8 04:14:28 2023, max compression
+gzip compressed data, was "pure_safetensors-0.2.0.tar", last modified: Mon Apr 10 08:59:53 2023, max compression
```

## Comparing `pure_safetensors-0.1.0.tar` & `pure_safetensors-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-08 04:14:28.880732 pure_safetensors-0.1.0/
--rw-r--r--   0 user      (1000) user      (1000)     2820 2023-04-08 04:14:28.880732 pure_safetensors-0.1.0/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     2077 2023-04-08 04:10:54.000000 pure_safetensors-0.1.0/README.md
--rw-r--r--   0 user      (1000) user      (1000)       50 2023-04-08 04:10:54.000000 pure_safetensors-0.1.0/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)      110 2023-04-08 04:14:28.880732 pure_safetensors-0.1.0/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      756 2023-04-08 04:10:54.000000 pure_safetensors-0.1.0/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-08 04:14:28.870733 pure_safetensors-0.1.0/src/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-08 04:14:28.870733 pure_safetensors-0.1.0/src/pure_safetensors/
--rw-r--r--   0 user      (1000) user      (1000)       35 2023-04-08 04:10:54.000000 pure_safetensors-0.1.0/src/pure_safetensors/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      163 2023-04-08 04:10:54.000000 pure_safetensors-0.1.0/src/pure_safetensors/exc.py
--rw-r--r--   0 user      (1000) user      (1000)     2373 2023-04-08 04:10:54.000000 pure_safetensors-0.1.0/src/pure_safetensors/numpy.py
--rw-r--r--   0 user      (1000) user      (1000)    22993 2023-04-08 04:10:54.000000 pure_safetensors-0.1.0/src/pure_safetensors/safetensors.py
--rw-r--r--   0 user      (1000) user      (1000)      891 2023-04-08 04:10:54.000000 pure_safetensors-0.1.0/src/pure_safetensors/util.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-08 04:14:28.880732 pure_safetensors-0.1.0/src/pure_safetensors.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     2820 2023-04-08 04:14:28.000000 pure_safetensors-0.1.0/src/pure_safetensors.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      418 2023-04-08 04:14:28.000000 pure_safetensors-0.1.0/src/pure_safetensors.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-08 04:14:28.000000 pure_safetensors-0.1.0/src/pure_safetensors.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       36 2023-04-08 04:14:28.000000 pure_safetensors-0.1.0/src/pure_safetensors.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       17 2023-04-08 04:14:28.000000 pure_safetensors-0.1.0/src/pure_safetensors.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-10 08:59:53.166548 pure_safetensors-0.2.0/
+-rw-r--r--   0 user      (1000) user      (1000)     3660 2023-04-10 08:59:53.166548 pure_safetensors-0.2.0/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     2741 2023-04-10 08:57:54.000000 pure_safetensors-0.2.0/README.md
+-rw-r--r--   0 user      (1000) user      (1000)       50 2023-04-10 08:57:54.000000 pure_safetensors-0.2.0/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)      110 2023-04-10 08:59:53.166548 pure_safetensors-0.2.0/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      756 2023-04-10 08:57:54.000000 pure_safetensors-0.2.0/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-10 08:59:53.166548 pure_safetensors-0.2.0/src/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-10 08:59:53.166548 pure_safetensors-0.2.0/src/pure_safetensors/
+-rw-r--r--   0 user      (1000) user      (1000)       35 2023-04-10 08:57:54.000000 pure_safetensors-0.2.0/src/pure_safetensors/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      163 2023-04-10 08:57:54.000000 pure_safetensors-0.2.0/src/pure_safetensors/exc.py
+-rw-r--r--   0 user      (1000) user      (1000)     6921 2023-04-10 08:57:54.000000 pure_safetensors-0.2.0/src/pure_safetensors/mmap.py
+-rw-r--r--   0 user      (1000) user      (1000)     1570 2023-04-10 08:57:54.000000 pure_safetensors-0.2.0/src/pure_safetensors/numpy.py
+-rw-r--r--   0 user      (1000) user      (1000)    24148 2023-04-10 08:57:54.000000 pure_safetensors-0.2.0/src/pure_safetensors/safetensors.py
+-rw-r--r--   0 user      (1000) user      (1000)     1158 2023-04-10 08:57:54.000000 pure_safetensors-0.2.0/src/pure_safetensors/util.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-10 08:59:53.166548 pure_safetensors-0.2.0/src/pure_safetensors.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3660 2023-04-10 08:59:52.000000 pure_safetensors-0.2.0/src/pure_safetensors.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      447 2023-04-10 08:59:52.000000 pure_safetensors-0.2.0/src/pure_safetensors.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-10 08:59:52.000000 pure_safetensors-0.2.0/src/pure_safetensors.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       36 2023-04-10 08:59:52.000000 pure_safetensors-0.2.0/src/pure_safetensors.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       17 2023-04-10 08:59:52.000000 pure_safetensors-0.2.0/src/pure_safetensors.egg-info/top_level.txt
```

### Comparing `pure_safetensors-0.1.0/PKG-INFO` & `pure_safetensors-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,62 @@
-Metadata-Version: 2.1
-Name: pure_safetensors
-Version: 0.1.0
-Summary: Pure-Python safetensors
-Home-page: UNKNOWN
-Author: Eduard Christian Dumitrescu
-Author-email: eduard.c.dumitrescu@gmail.com
-License: MIT
-Description: # pure_safetensors
-        
-        [Safetensors](https://github.com/huggingface/safetensors) library but in pure clean Python. Run it on PyPy or IronPython or wherever.
-        
-        # Dependencies
-        
-        We try to keep dependencies light:
-        
-        - [attrs](https://pypi.org/project/attrs/) dataclass library (2881 LoC)
-        - [marshmallow](https://pypi.org/project/marshmallow/) serialization and validation library (2647 LoC)
-        - [sortedcollections](https://pypi.org/project/sortedcollections/) tiny sorted collections library (339 LoC) built on top of [sortedcontainers](https://pypi.org/project/sortedcontainers/) (1493 LoC)
-        - (optional) [sparsefile](https://pypi.org/project/sparsefile/) sparse file library (191 LoC)
-        
-        Optionally, this library integrates with NumPy (if available). PyTorch integration is planned.
-        
-        To run the tests, you'll need `pytest`, `numpy`, and optionally `hypothesis`.
-        
-        # Examples
-        
-        TODO
-        
-        # Bugs
-        
-        The space allocator is a greedy algorithm based on first-fit-decreasing bin packing. So if you add/remove tensors to an existing file, it may leave too much empty space behind.
-        
-        # Alternatives
-        
-        - [safetensors](https://github.com/huggingface/safetensors/)
-        - [Narsil/pure_torch.py](https://gist.github.com/Narsil/3edeec2669a5e94e4707aa0f901d2282)
-        - [Narsil/safetensors.cpp](https://gist.github.com/Narsil/5d6bf307995158ad2c4994f323967284)
-        
-        |                                                | pure_safetensors | safetensors | pure_torch.py | safetensors.cpp |
-        |------------------------------------------------|------------------|-------------|---------------|-----------------|
-        | Written in pure Python?                        | ✅ | ❌ | ✅ | — |
-        | Supports NumPy directly (no PyTorch)?          | ✅ | ✅ | ❌ | — |
-        | Can write safetensors files?                   | ✅ | ✅ | ❌ | ❌ |
-        | Can add/delete tensors in-place (no copying)?  | ✅ | ❌ | ❌ | ❌ |
-        | Has unit tests?                                | ✅ | ✅ | ❌ | ❌ |
-        | Stable API?                                    | 🤷 | ✅ | ❔ | ❔ |
-        | Automatically make files sparse to save space? | ✅ | ❌ | ❌ | ❌ |
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
+# pure_safetensors
+
+[Safetensors](https://github.com/huggingface/safetensors) library but in pure clean Python. Run it on PyPy or IronPython or wherever.
+
+# Dependencies
+
+We try to keep dependencies light:
+
+- [attrs](https://pypi.org/project/attrs/) dataclass library (2881 LoC)
+- [marshmallow](https://pypi.org/project/marshmallow/) serialization and validation library (2647 LoC)
+- [sortedcollections](https://pypi.org/project/sortedcollections/) tiny sorted collections library (339 LoC) built on top of [sortedcontainers](https://pypi.org/project/sortedcontainers/) (1493 LoC)
+- (optional) [sparsefile](https://pypi.org/project/sparsefile/) sparse file library (191 LoC)
+
+Optionally, this library integrates with NumPy (if available). PyTorch integration is planned, someday.
+
+To run the tests, you'll need `pytest`, `numpy`, and optionally `hypothesis`.
+
+# Examples
+
+```python
+from pure_safetensors import SafeTensors
+
+with SafeTensors("/path/to/example.safetensors", "r+") as sf, sf.as_numpy() as arrays:
+    arrays["hello"][3, :] += 420.69
+    arrays["world"] = arrays["hello"][0:2] * 10
+
+    # assign multiple arrays! much faster!
+    arrays.update(
+        {
+            "q": my_array_1,
+            "k": my_array_2,
+            "v": my_array_3,
+        }
+    )
+
+    # delete arrays! such wonders!
+    del arrays["v"]
+```
+
+# Bugs
+
+The space allocator is a greedy algorithm based on first-fit-decreasing bin packing. So if you add/remove tensors to an existing file, it may leave too much empty space behind.
+
+PyTorch support isn't implemented yet.
+
+# Alternatives
+
+- [safetensors](https://github.com/huggingface/safetensors/)
+- [Narsil/pure_torch.py](https://gist.github.com/Narsil/3edeec2669a5e94e4707aa0f901d2282)
+- [Narsil/safetensors.cpp](https://gist.github.com/Narsil/5d6bf307995158ad2c4994f323967284)
+
+|                                                 | pure_safetensors | safetensors | pure_torch.py | safetensors.cpp |
+|-------------------------------------------------|------------------|-------------|---------------|-----------------|
+| Written in pure Python?                         | ✅ | ❌ | ✅ | — |
+| Supports NumPy (without PyTorch)?               | ✅ | ✅ | ❌ | — |
+| Can work without numpy or pytorch?              | ✅ | ✅ | ❌ | — |
+| Can write safetensors files?                    | ✅ | ✅ | ❌ | ❌ |
+| Can modify file in-place to add/remove tensors? | ✅ | ❌ | ❌ | ❌ |
+| Has test suite?                                 | ✅ | ✅ | ❌ | ❌ |
+| Stable API?                                     | 🤷 | ✅ | ❔ | ❔ |
+| Automatically makes files sparse to save space? | ✅ | ❌ | ❌ | ❌ |
+| Works on platforms without mmap?                | ✅ | ❌ | ❌ | ❌ |
```

### Comparing `pure_safetensors-0.1.0/setup.py` & `pure_safetensors-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text("utf-8")
 
 setup(
     name="pure_safetensors",
     description="Pure-Python safetensors",
-    version="0.1.0",
+    version="0.2.0",
     author="Eduard Christian Dumitrescu",
     author_email="eduard.c.dumitrescu@gmail.com",
     install_requires=["attrs", "marshmallow", "sortedcollections"],
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     license="MIT",
     classifiers=[
```

### Comparing `pure_safetensors-0.1.0/src/pure_safetensors/safetensors.py` & `pure_safetensors-0.2.0/src/pure_safetensors/safetensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 import json
 import operator
 import os
 import struct
-from typing import Dict, Iterable, List, Optional, Tuple
+from typing import Dict, IO, Iterable, List, Optional, Tuple
 
 import attr
 import marshmallow
 from marshmallow import fields
 import sortedcollections
 import warnings
 
@@ -29,54 +29,69 @@
     Resizing the file may result in a crash:
     https://stackoverflow.com/questions/19545949/detect-that-mmap-ed-file-has-been-truncated
 
     Parameters
     ----------
     file: str, file-like, or Path
         File to operate on.
-    mode: {"r", "r+", "w+", "c"}
+    mode: {"r", "r+", "x+", "w+", "c"}
         r: Open existing file for reading only.
         r+: Open existing file for reading and writing.
         w+: Create or overwrite existing file for reading and writing.
         c: Copy-on-write: assignments affect data in memory, but changes are
            not saved to disk. The file on disk is read-only.
     sparse: bool or None, optional
         If True, make the file sparse. If False, then don't. If None, then
         try to make it sparse but don't raise an exception if it's not possible
         to do so.
     """
 
-    _valid_modes = frozenset(("r", "r+", "w+", "c"))
+    _valid_modes = frozenset(("r", "r+", "x+", "w+", "c"))
 
-    file: object = attr.ib()
+    file: IO = attr.ib()
     mode: str = attr.ib()
     sparse: bool = attr.ib(default=None)
-    settings: "FileMapSettings" = attr.ib(
-        factory=lambda: FileMapSettings(), kw_only=True
-    )
+    settings: "Settings" = attr.ib(factory=lambda: Settings(), kw_only=True)
 
     map: "FileMap"
 
     tensors: "Dict[str, SafeTensorInfo]"
-    _close_file = False
+    _close_on_exit: bool = False
+
+    def _open_file(self):
+        self.file = open(self.file, self.mode.replace("c", "r") + "b")
+
+    def __attrs_post_init__(self):
+        if not hasattr(self.file, "read"):
+            # the user passed in a Path or str, so we need to make sure to close it
+            self._open_file()
+            self._close_on_exit = True
+
+        # replace "x+" with "w+" since they are equivalent after the file is created
+        if self.mode == "x+":
+            self.mode = "w+"
+
+        # load file or write empty header if creating new file
+        self._initialize_structure()
 
     @mode.validator
     def check(self, attribute, value):
         if value not in self._valid_modes:
             raise ValueError(f"{value!r} not in {self._valid_modes!r}")
 
     @property
     def readonly(self):
         return "+" not in self.mode
 
-    def __attrs_post_init__(self):
-        if not hasattr(self.file, "fileno"):
-            raise AssertionError
+    def __enter__(self):
+        return self
 
-        self._initialize_structure()
+    def __exit__(self, exc_type, exc_value, traceback):
+        if self._close_on_exit:
+            self.file.close()
 
     def _initialize_structure(self):
         if self.mode != "w+":
             try:
                 self._read_header()
             except SafeTensorEmptyFileError:
                 # if the file is totally empty and mode == "r+" (read+write), then
@@ -138,29 +153,27 @@
 
     def as_numpy(self, **kw):
         """
         Examples
         --------
 
         ::
-            st = SafeTensors(...)
-            st_numpy = st.as_numpy()
-
-            my_tensor = st_numpy["my_tensor_name"]
-            st_numpy.update({"new_tensor": my_array, "another_tensor": my_array_2})
-            del st_numpy["my_tensor_name"]
+            with SafeTensors(...) as st, st.as_numpy() as st_numpy:
+                do_stuff(st_numpy["my_tensor_name"] * 3 + 1)
+                st_numpy.update({"new_tensor": my_array, "another_tensor": my_array_2})
+                del st_numpy["my_tensor_name"]
         """
         from .numpy import NumpyAdapter
 
         return NumpyAdapter(self, **kw)
 
-    def as_pytorch(self, **kw):
-        raise NotImplementedError(
-            "pytorch support not implemented, why don't you do it and submit a patch?"
-        )
+    def as_buffer(self, **kw):
+        from .mmap import BufferAdapter
+
+        return BufferAdapter(self, **kw)
 
     def create_or_replace_or_delete_tensors(
         self, tensors: "Dict[str, Optional[SafeTensorInfo]]"
     ) -> None:
         """
         Allocate tensors. This may resize the JSON header, and sometimes even
         move existing tensors to make way for a larger header. As such, it is NOT
@@ -179,28 +192,26 @@
             delete={name for name, tensor in tensors.items() if tensor is None},
         )
 
         self.file.seek(file_map.minimum_file_size)
         self.file.write(b"\0")
         self.file.flush()
         self._write_header(file_map)
+        self.truncate()
         self.sparsify()
 
     def truncate(self):
         """
         Truncate file to its smallest possible size.
         """
-        try:
-            last_tensor = self.tensors.values()[-1]
-        except IndexError:
-            eof = self.header_size
-        else:
-            eof = last_tensor.end
-
-        self.file.truncate(eof)
+        n = self.map.minimum_file_size
+        self.file.seek(n)
+        self.file.write(b"\0")
+        self.file.flush()
+        self.file.truncate(n)
 
     def sparsify(self):
         """
         Make file sparse, depending on the value of :attr:`sparse`.
         """
         if self.sparse is False:
             return
@@ -226,33 +237,34 @@
             else:
                 sparsefile.ensure_sparse(self.file, start, length)
 
 
 @attr.s
 class DType:
     name: str = attr.ib()
+    kind: str = attr.ib()
     size_in_bytes: int = attr.ib()
     numpy_name: str = attr.ib()
     recommended_alignment_in_bytes: int = attr.ib(default=None)
 
     def __attrs_post_init__(self):
         if self.recommended_alignment_in_bytes is None:
             self.recommended_alignment_in_bytes = max(8, self.size_in_bytes)
 
     def __str__(self):
         return self.name
 
 
 _dtypes_list = [
-    DType("BOOL", 1, "bool"),
-    DType("BF16", 2, "bfloat16"),
+    DType("BOOL", "b", 1, "bool"),
+    DType("BF16", "bf", 2, "bfloat16"),
 ]
-_dtypes_list += (DType(f"U{n}", n // 8, f"uint{n}") for n in (8, 16, 32, 64))
-_dtypes_list += (DType(f"I{n}", n // 8, f"int{n}") for n in (8, 16, 32, 64))
-_dtypes_list += (DType(f"F{n}", n // 8, f"float{n}") for n in (16, 32, 64))
+_dtypes_list += (DType(f"U{n * 8}", "u", n, f"uint{n * 8}") for n in (1, 2, 4, 8))
+_dtypes_list += (DType(f"I{n * 8}", "i", n, f"int{n * 8}") for n in (1, 2, 4, 8))
+_dtypes_list += (DType(f"F{n * 8}", "f", n, f"float{n * 8}") for n in (2, 4, 8))
 dtypes = {dt.name: dt for dt in _dtypes_list}
 del _dtypes_list
 
 
 class NonnegativeInteger(fields.Integer):
     def _deserialize(self, value, attr, data, **kwargs):
         if not isinstance(value, int) or value < 0:
@@ -321,15 +333,15 @@
 class SafeTensorsSchema(marshmallow.Schema):
     class Meta:
         unknown = marshmallow.RAISE
 
     tensors = fields.Dict(
         fields.String(), fields.Nested(SafeTensorSchema), required=True
     )
-    metadata = fields.Raw(required=False)
+    metadata = fields.Dict(fields.String(), fields.String(), required=False)
 
     @marshmallow.pre_load
     def pre_load_metadata_split(self, data, **kwargs):
         if type(data) is not dict:
             raise marshmallow.ValidationError("root object must be dictionary")
 
         split = {"tensors": data.copy()}
@@ -353,20 +365,21 @@
             merged["__metadata__"] = data["metadata"]
         except KeyError:
             pass  # metadata is optional
 
         return merged
 
 
-@attr.s
-class FileMapSettings:
+@attr.s(eq=False)
+class Settings:
     header_size_alignment: int = attr.ib(default=4096)
     header_size_padding: int = attr.ib(default=1024)
     new_tensor_alignment: int = attr.ib(default=64)
     maximum_header_size: int = attr.ib(default=100_000_000)
+    maximum_file_size: int = attr.ib(2 ** 40)
 
 
 @attr.s
 class MoveRequest:
     src: int = attr.ib()
     dst: int = attr.ib()
     len: int = attr.ib()
@@ -374,16 +387,16 @@
 
 def sorted_tensors_dict(values=()):
     return sortedcollections.ValueSortedDict(lambda value: value.start, values)
 
 
 @attr.s
 class FileMap:
-    settings: FileMapSettings = attr.ib()
-    metadata: object = attr.ib(default=None)
+    settings: Settings = attr.ib()
+    metadata: Optional[Dict[str, str]] = attr.ib(default=None)
     tensors: "Dict[str, SafeTensorInfo]" = attr.ib(factory=sorted_tensors_dict)
     pending_moves: List[MoveRequest] = attr.ib(factory=list)
 
     _header = None
 
     @attr.s
     class _Header:
@@ -457,15 +470,15 @@
         self._load_header(value)
 
     @header.deleter
     def header(self):
         self._header = None
 
     @classmethod
-    def from_file(cls, f, settings: FileMapSettings, **kw):
+    def from_file(cls, f, settings: Settings, **kw):
         f.seek(0)
         length_data = f.read(8)
         if not length_data:
             raise SafeTensorEmptyFileError
         json_size = cls._parse_size(length_data)
 
         # check size constraint
@@ -541,53 +554,67 @@
                 # The larger-JSON header would overlap with the first tensor,
                 # so revert back to the smallest-JSON header.
                 final_header = smallest_json_header
         else:
             # The smallest possible header size would still exceed the available
             # space. Since tensors must be moved, make enough room so that
             # this movement doesn't need to happen again too soon.
-            header_size = align(
-                self.settings.header_size_alignment,
-                largest_json_header.unpadded_length + self.settings.header_size_padding,
+            header_size = self.compute_reserved_header_space(
+                largest_json_header.unpadded_length
             )
             final_header = self._get_header_for_header_size(header_size)
 
         return bytes(final_header)
 
+    def compute_reserved_header_space(self, header_size: int) -> int:
+        return align(
+            self.settings.header_size_alignment,
+            header_size + self.settings.header_size_padding,
+        )
+
     @property
     def header_size(self):
         return len(self.header)
 
     def validate(self):
         prev_end = self.header_size
         for name, tensor in self.tensors.items():
             start = tensor.start
             end = tensor.end
 
-            if start == end:
-                continue  # ignore empty tensors
-
-            if start < prev_end:
+            req_size = tensor.required_size
+            if req_size != end - start:
                 raise SafeTensorError(
-                    f"tensor {name!r} overlaps with previous structure"
+                    f"tensor {name!r} {tensor!r} size is wrong, expected {req_size}"
                 )
-            if end <= start:
-                raise SafeTensorError(f"tensor {name!r} does not obey `start < end`")
+
+            if start != end:
+                # only check tensors of nonzero size
+
+                if start < prev_end:
+                    raise SafeTensorError(
+                        f"tensor {name!r} overlaps with previous structure"
+                    )
 
             prev_end = end
 
+        if prev_end > self.settings.maximum_file_size:
+            raise SafeTensorError(
+                f"last tensor position {prev_end} exceeds maximum file size"
+            )
+
     @property
     def minimum_file_size(self):
         tensors = self.tensors
         p = tensors.values()[-1].end if tensors else 0
         return max(p, self.header_size)
 
     def get_empty_ranges(self):
         ranges = []
-        prev_end = self.header_size
+        prev_end = self.compute_reserved_header_space(self.header_size)
 
         for name, tensor in self.tensors.items():
             start = tensor.start
             end = tensor.end
 
             if start == end:
                 continue  # ignore empty tensors
```

### Comparing `pure_safetensors-0.1.0/src/pure_safetensors/util.py` & `pure_safetensors-0.2.0/src/pure_safetensors/util.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,23 @@
+import os
+from typing import IO
+
+
 def align(alignment: int, position: int) -> int:
     assert alignment & (alignment - 1) == 0
     mask = alignment - 1
     return (position + mask) & ~mask
 
 
+def align_down(alignment: int, position: int) -> int:
+    assert alignment & (alignment - 1) == 0
+    mask = alignment - 1
+    return position & ~mask
+
+
 def samefile_copy(f, src: int, dst: int, length: int, block_size: int = 1 << 18):
     if src < dst:
         src += length
         dst += length
         while length:
             to_read = min(length, block_size)
             src -= to_read
@@ -24,7 +34,10 @@
             length -= to_read
             f.seek(src)
             data = f.read(to_read).ljust(to_read, b"\0")
             f.seek(dst)
             f.write(data)
             src += to_read
             dst += to_read
+
+def get_file_size(file: IO) -> int:
+    return os.fstat(file.fileno()).st_size
```

