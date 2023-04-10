# Comparing `tmp/upathlib-0.7.6.tar.gz` & `tmp/upathlib-0.7.7b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upathlib-0.7.6.tar", last modified: Mon Apr 10 08:04:35 2023, max compression
+gzip compressed data, was "upathlib-0.7.7b1.tar", last modified: Mon Apr 10 09:15:46 2023, max compression
```

## Comparing `upathlib-0.7.6.tar` & `upathlib-0.7.7b1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2022-12-13 07:44:37.384893 upathlib-0.7.6/LICENSE
--rw-r--r--   0        0        0      993 2023-03-30 16:49:23.794031 upathlib-0.7.6/README.rst
--rw-r--r--   0        0        0     1696 2023-04-10 07:23:59.351683 upathlib-0.7.6/pyproject.toml
--rw-r--r--   0        0        0     2303 2023-04-10 07:17:33.658634 upathlib-0.7.6/src/upathlib/__init__.py
--rw-r--r--   0        0        0     4438 2023-04-10 07:20:14.097239 upathlib-0.7.6/src/upathlib/_blob.py
--rw-r--r--   0        0        0    11037 2023-04-10 07:21:09.179727 upathlib-0.7.6/src/upathlib/_local.py
--rw-r--r--   0        0        0     7852 2023-03-07 05:27:40.006650 upathlib-0.7.6/src/upathlib/_tests.py
--rw-r--r--   0        0        0    33718 2023-04-10 08:02:16.156083 upathlib-0.7.6/src/upathlib/_upath.py
--rw-r--r--   0        0        0    12562 2023-04-10 07:22:06.641407 upathlib-0.7.6/src/upathlib/azure.py
--rw-r--r--   0        0        0    25298 2023-04-10 07:23:12.279817 upathlib-0.7.6/src/upathlib/gcs.py
--rw-r--r--   0        0        0        0 2022-12-13 07:44:37.384893 upathlib-0.7.6/src/upathlib/py.typed
--rw-r--r--   0        0        0     3763 2023-04-10 07:52:52.476823 upathlib-0.7.6/src/upathlib/serializer.py
--rw-r--r--   0        0        0     2381 1970-01-01 00:00:00.000000 upathlib-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-12-13 07:44:37.384893 upathlib-0.7.7b1/LICENSE
+-rw-r--r--   0        0        0      993 2023-03-30 16:49:23.794031 upathlib-0.7.7b1/README.rst
+-rw-r--r--   0        0        0     1696 2023-04-10 08:06:32.336660 upathlib-0.7.7b1/pyproject.toml
+-rw-r--r--   0        0        0     2305 2023-04-10 09:02:39.215528 upathlib-0.7.7b1/src/upathlib/__init__.py
+-rw-r--r--   0        0        0     4438 2023-04-10 08:06:32.336660 upathlib-0.7.7b1/src/upathlib/_blob.py
+-rw-r--r--   0        0        0    11176 2023-04-10 09:03:09.436670 upathlib-0.7.7b1/src/upathlib/_local.py
+-rw-r--r--   0        0        0     7852 2023-03-07 05:27:40.006650 upathlib-0.7.7b1/src/upathlib/_tests.py
+-rw-r--r--   0        0        0    34266 2023-04-10 09:03:09.506671 upathlib-0.7.7b1/src/upathlib/_upath.py
+-rw-r--r--   0        0        0    12562 2023-04-10 08:06:32.346660 upathlib-0.7.7b1/src/upathlib/azure.py
+-rw-r--r--   0        0        0    25298 2023-04-10 08:06:32.346660 upathlib-0.7.7b1/src/upathlib/gcs.py
+-rw-r--r--   0        0        0        0 2022-12-13 07:44:37.384893 upathlib-0.7.7b1/src/upathlib/py.typed
+-rw-r--r--   0        0        0     3763 2023-04-10 08:06:32.346660 upathlib-0.7.7b1/src/upathlib/serializer.py
+-rw-r--r--   0        0        0     2383 1970-01-01 00:00:00.000000 upathlib-0.7.7b1/PKG-INFO
```

### Comparing `upathlib-0.7.6/LICENSE` & `upathlib-0.7.7b1/LICENSE`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.6/README.rst` & `upathlib-0.7.7b1/README.rst`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.6/pyproject.toml` & `upathlib-0.7.7b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.6/src/upathlib/__init__.py` & `upathlib-0.7.7b1/src/upathlib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 One use case is the package `biglist <https://biglist.readthedocs.io/en/latest/>`__,
 where the class `Biglist <https://biglist.readthedocs.io/en/latest/#biglist.Biglist>`__ takes a Upath object to indicate its location of storage.
 It does not care whether the storage is local or in a cloud blob store---it
 simply uses the common API to operate the storage.
 """
 
-__version__ = "0.7.6"
+__version__ = "0.7.7b1"
 
 from pathlib import Path
 from typing import Union
 
 from ._blob import BlobUpath
 from ._local import LocalUpath
 from ._upath import FileInfo, LockAcquireError, LockReleaseError, Upath
```

### Comparing `upathlib-0.7.6/src/upathlib/_blob.py` & `upathlib-0.7.7b1/src/upathlib/_blob.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.6/src/upathlib/_local.py` & `upathlib-0.7.7b1/src/upathlib/_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,14 +202,15 @@
 
     def rename_dir(
         self,
         target: str | LocalUpath,
         *,
         overwrite: bool = False,
         quiet: bool = False,
+        concurrent: bool = True,
     ) -> LocalUpath:
         """Rename the current dir (i.e. ``self``) to ``target``.
 
         ``overwrite`` is applied file-wise. If there are
         files under ``target`` that do not have counterparts under ``self``,
         they are left untouched.
 
@@ -225,15 +226,22 @@
             target = target._path
         target_ = self.parent / target
         if target_ == self:
             return self
 
         if not quiet:
             print(f"Renaming {self!r} to {target_!r}", file=sys.stderr)
-        self._copy_dir(self, target_, "rename_file", overwrite=overwrite, quiet=quiet)
+        self._copy_dir(
+            self,
+            target_,
+            "rename_file",
+            overwrite=overwrite,
+            quiet=quiet,
+            concurrent=concurrent,
+        )
 
         def _remove_empty_dir(path):
             k = 0
             for p in path.iterdir():
                 if p.is_dir():
                     k += _remove_empty_dir(p)
                 else:
```

### Comparing `upathlib-0.7.6/src/upathlib/_tests.py` & `upathlib-0.7.7b1/src/upathlib/_tests.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.6/src/upathlib/_upath.py` & `upathlib-0.7.7b1/src/upathlib/_upath.py`

 * *Files 2% similar despite different names*

```diff
@@ -674,15 +674,23 @@
         def read_pickle_lz4(self, **kwargs) -> Any:
             """
             ``**kwargs`` are passed to :meth:`serializer.Lz4PickleSerializer.deserialize`.
             """
             return Lz4PickleSerializer.deserialize(self.read_bytes(), **kwargs)
 
     def _copy_dir(
-        self, source, dest, method: str, *, overwrite: bool, quiet: bool, reversed=False
+        self,
+        source,
+        dest,
+        method: str,
+        *,
+        overwrite: bool,
+        quiet: bool,
+        reversed=False,
+        concurrent: bool = True,
     ):
         def foo():
             source_path = source.path
             ovwt = overwrite
             for p in source.riterdir():
                 extra = str(p.path.relative_to(source_path))
                 if reversed:
@@ -697,24 +705,30 @@
                         getattr(p, method),
                         (dest / extra,),
                         {"overwrite": ovwt},
                         extra,
                     )
 
         n = 0
-        for _ in self._run_in_executor(foo(), quiet):
-            n += 1
+        if concurrent:
+            for _ in self._run_in_executor(foo(), quiet):
+                n += 1
+        else:
+            for f, args, kwargs, _ in foo():
+                f(*args, **kwargs)
+                n += 1
         return n
 
     def copy_dir(
         self,
         target: str | Upath,
         *,
         overwrite: bool = False,
         quiet: bool = False,
+        concurrent: bool = True,
     ) -> int:
         """Copy the content of the current directory (i.e. ``self``) recursively to ``target``.
 
         If ``target`` is an string, then it is in the same store the the current path,
         and it is either absolute, or relative to ``self.parent``.
         In this case,
         the directory created by this operation will be the path ``self.parent / target``.
@@ -745,15 +759,20 @@
                 return 0
         else:
             target_ = target
 
         if not quiet:
             print(f"Copying from {self!r} into {target_!r}", file=sys.stderr)
         return self._copy_dir(
-            self, target_, "copy_file", overwrite=overwrite, quiet=quiet
+            self,
+            target_,
+            "copy_file",
+            overwrite=overwrite,
+            quiet=quiet,
+            concurrent=concurrent,
         )
 
     def _copy_file(self, target: Upath, *, overwrite: bool = False) -> None:
         target.write_bytes(self.read_bytes(), overwrite=overwrite)
 
     def copy_file(self, target: str | Upath, *, overwrite: bool = False) -> None:
         """Copy the current file (i.e. ``self``) to ``target``.
@@ -791,15 +810,15 @@
             if target_ == self:
                 return
         else:
             target_ = target
 
         self._copy_file(target_, overwrite=overwrite)
 
-    def remove_dir(self, *, quiet: bool = True) -> int:
+    def remove_dir(self, *, quiet: bool = True, concurrent: bool = True) -> int:
         """Remove the current directory (i.e. ``self``) and all its contents recursively.
 
         Essentially, this removes each file that is yielded by :meth:`riterdir`.
         Subclasses should take care to remove "empty directories", if applicable,
         that are left behind.
 
         ``quiet`` controls whether to print progress info.
@@ -811,16 +830,21 @@
         """
 
         def foo():
             for p in self.riterdir():
                 yield p.remove_file, [], {}, str(p.path.relative_to(self.path))
 
         n = 0
-        for _ in self._run_in_executor(foo(), quiet):
-            n += 1
+        if concurrent:
+            for _ in self._run_in_executor(foo(), quiet):
+                n += 1
+        else:
+            for f, *_ in foo():
+                f()
+                n += 1
         return n
 
     @abc.abstractmethod
     def remove_file(self) -> None:
         """Remove the current file (i.e. ``self``).
 
         If ``self`` is not an existing file, ``FileNotFoundError`` is raised.
@@ -870,15 +894,15 @@
         Similar to :meth:`iterdir`, if ``self`` is not a dir or does not exist,
         then nothing is yielded, and no exception is raised either.
 
         There is no guarantee on the order of the returned elements.
         """
         raise NotImplementedError
 
-    def rmrf(self, *, quiet: bool = True) -> int:
+    def rmrf(self, *, quiet: bool = True, concurrent: bool = True) -> int:
         """Remove the current file or dir (i.e. ``self``) recursively.
 
         Analogous to the Linux command ``rm -rf``, hence the name of this method.
 
         Return the number of files removed.
 
         For example, if these blobs are present::
@@ -894,15 +918,15 @@
         try:
             self.remove_file()
         except (FileNotFoundError, IsADirectoryError):
             n = 0
         else:
             n = 1
         try:
-            m = self.remove_dir(quiet=quiet)
+            m = self.remove_dir(quiet=quiet, concurrent=concurrent)
         except FileNotFoundError:
             m = 0
         return n + m
 
     @contextlib.contextmanager
     @abc.abstractmethod
     def lock(self, *, timeout: int = None):
```

### Comparing `upathlib-0.7.6/src/upathlib/azure.py` & `upathlib-0.7.7b1/src/upathlib/azure.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.6/src/upathlib/gcs.py` & `upathlib-0.7.7b1/src/upathlib/gcs.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.6/src/upathlib/serializer.py` & `upathlib-0.7.7b1/src/upathlib/serializer.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.6/PKG-INFO` & `upathlib-0.7.7b1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upathlib
-Version: 0.7.6
+Version: 0.7.7b1
 Summary: The package *upathlib*
 Author-email: Zepu Zhang <zepu.zhang@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

