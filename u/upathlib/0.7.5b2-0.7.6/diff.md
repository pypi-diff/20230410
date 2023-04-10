# Comparing `tmp/upathlib-0.7.5b2.tar.gz` & `tmp/upathlib-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upathlib-0.7.5b2.tar", last modified: Thu Mar 30 19:12:41 2023, max compression
+gzip compressed data, was "upathlib-0.7.6.tar", last modified: Mon Apr 10 08:04:35 2023, max compression
```

## Comparing `upathlib-0.7.5b2.tar` & `upathlib-0.7.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2022-12-13 07:44:37.384893 upathlib-0.7.5b2/LICENSE
--rw-r--r--   0        0        0      993 2023-03-30 16:49:23.794031 upathlib-0.7.5b2/README.rst
--rw-r--r--   0        0        0     1713 2023-03-30 16:49:41.256026 upathlib-0.7.5b2/pyproject.toml
--rw-r--r--   0        0        0     2305 2023-03-30 16:54:28.426040 upathlib-0.7.5b2/src/upathlib/__init__.py
--rw-r--r--   0        0        0     4536 2023-03-05 06:02:46.639594 upathlib-0.7.5b2/src/upathlib/_blob.py
--rw-r--r--   0        0        0    11279 2023-03-30 16:49:23.804031 upathlib-0.7.5b2/src/upathlib/_local.py
--rw-r--r--   0        0        0     7852 2023-03-07 05:27:40.006650 upathlib-0.7.5b2/src/upathlib/_tests.py
--rw-r--r--   0        0        0    35033 2023-03-30 16:49:41.256026 upathlib-0.7.5b2/src/upathlib/_upath.py
--rw-r--r--   0        0        0    12789 2023-03-30 16:49:23.804031 upathlib-0.7.5b2/src/upathlib/azure.py
--rw-r--r--   0        0        0    25555 2023-03-30 16:56:27.764554 upathlib-0.7.5b2/src/upathlib/gcs.py
--rw-r--r--   0        0        0        0 2022-12-13 07:44:37.384893 upathlib-0.7.5b2/src/upathlib/py.typed
--rw-r--r--   0        0        0     3184 2023-03-30 16:49:23.804031 upathlib-0.7.5b2/src/upathlib/serializer.py
--rw-r--r--   0        0        0     2334 1970-01-01 00:00:00.000000 upathlib-0.7.5b2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-12-13 07:44:37.384893 upathlib-0.7.6/LICENSE
+-rw-r--r--   0        0        0      993 2023-03-30 16:49:23.794031 upathlib-0.7.6/README.rst
+-rw-r--r--   0        0        0     1696 2023-04-10 07:23:59.351683 upathlib-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0     2303 2023-04-10 07:17:33.658634 upathlib-0.7.6/src/upathlib/__init__.py
+-rw-r--r--   0        0        0     4438 2023-04-10 07:20:14.097239 upathlib-0.7.6/src/upathlib/_blob.py
+-rw-r--r--   0        0        0    11037 2023-04-10 07:21:09.179727 upathlib-0.7.6/src/upathlib/_local.py
+-rw-r--r--   0        0        0     7852 2023-03-07 05:27:40.006650 upathlib-0.7.6/src/upathlib/_tests.py
+-rw-r--r--   0        0        0    33718 2023-04-10 08:02:16.156083 upathlib-0.7.6/src/upathlib/_upath.py
+-rw-r--r--   0        0        0    12562 2023-04-10 07:22:06.641407 upathlib-0.7.6/src/upathlib/azure.py
+-rw-r--r--   0        0        0    25298 2023-04-10 07:23:12.279817 upathlib-0.7.6/src/upathlib/gcs.py
+-rw-r--r--   0        0        0        0 2022-12-13 07:44:37.384893 upathlib-0.7.6/src/upathlib/py.typed
+-rw-r--r--   0        0        0     3763 2023-04-10 07:52:52.476823 upathlib-0.7.6/src/upathlib/serializer.py
+-rw-r--r--   0        0        0     2381 1970-01-01 00:00:00.000000 upathlib-0.7.6/PKG-INFO
```

### Comparing `upathlib-0.7.5b2/LICENSE` & `upathlib-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.5b2/README.rst` & `upathlib-0.7.6/README.rst`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.5b2/pyproject.toml` & `upathlib-0.7.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -7,18 +7,15 @@
 name = "upathlib"
 authors = [
     {name = "Zepu Zhang", email = "zepu.zhang@gmail.com"},
 ]
 dependencies = [
     "filelock >= 3.9.1",
     "deprecation",
-    "orjson",
-    "overrides",
     "tqdm",
-    "zstandard >=0.18.0",
     "typing-extensions",
     "mpservice >= 0.11.9",
 ]
 requires-python = ">=3.8"
 readme = "README.rst"
 license = {file = "LICENSE"}
 classifiers = [
@@ -39,14 +36,16 @@
 ]
 gcs = [
     "google-auth",
     "google-api-python-client >=2.13.9,<3.0",
     "google-cloud-storage >=2.0,<3.0",
     "requests",
 ]
+zstandard = ["zstandard"]
+lz4 = ["lz4"]
 doc = [
     "sphinx",
     "numpydoc",
     "pydata-sphinx-theme",
 ]
 test = [
     "black",
```

### Comparing `upathlib-0.7.5b2/src/upathlib/__init__.py` & `upathlib-0.7.6/src/upathlib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 One use case is the package `biglist <https://biglist.readthedocs.io/en/latest/>`__,
 where the class `Biglist <https://biglist.readthedocs.io/en/latest/#biglist.Biglist>`__ takes a Upath object to indicate its location of storage.
 It does not care whether the storage is local or in a cloud blob store---it
 simply uses the common API to operate the storage.
 """
 
-__version__ = "0.7.5b2"
+__version__ = "0.7.6"
 
 from pathlib import Path
 from typing import Union
 
 from ._blob import BlobUpath
 from ._local import LocalUpath
 from ._upath import FileInfo, LockAcquireError, LockReleaseError, Upath
```

### Comparing `upathlib-0.7.5b2/src/upathlib/_blob.py` & `upathlib-0.7.6/src/upathlib/_blob.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 import pathlib
 import sys
 from collections.abc import Iterator
 
-from overrides import EnforceOverrides, overrides
 from typing_extensions import Self
 
 from ._local import LocalPathType, LocalUpath
 from ._upath import Upath
 
 
 def _resolve_local_path(p: LocalPathType):
@@ -17,15 +16,15 @@
     if isinstance(p, pathlib.Path):
         p = LocalUpath(str(p.resolve().absolute()))
     else:
         assert isinstance(p, LocalUpath)
     return p
 
 
-class BlobUpath(Upath, EnforceOverrides):
+class BlobUpath(Upath):
     """
     BlobUpath is a base class for paths in a *cloud* storage, aka "blob store".
     This is in contrast to a *local* disk storage, which is implemnted by :class:`LocalUpath`.
     """
 
     @property
     def blob_name(self) -> str:
@@ -33,15 +32,14 @@
         Return the "name" of the blob. This is the "path" without a leading ``'/'``.
         In cloud blob stores, this is exactly the name of the blob. The name often
         contains ``'/'``, which has no special role in the name per se but is *interpreted*
         by users to be a directory separator.
         """
         return self._path.lstrip("/")
 
-    @overrides
     def is_dir(self) -> bool:
         """In a typical blob store, there is no such concept as a
         "directory". Here we emulate the concept in a local file
         system. If there is a blob named like
 
         ::
 
@@ -63,15 +61,14 @@
         """
         try:
             next(self.iterdir())
             return True
         except StopIteration:
             return False
 
-    @overrides
     def iterdir(self) -> Iterator[Self]:
         """
         Yield immediate children under the current dir.
 
         This is a naive, inefficient implementation.
         Expected to be refined by subclasses.
         """
```

### Comparing `upathlib-0.7.5b2/src/upathlib/_local.py` & `upathlib-0.7.6/src/upathlib/_local.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 # `filelock` is also called `py-filelock`.
 # Tried `fasteners` also. In one use case,
 # `filelock` worked whereas `fasteners.InterprocessLock` failed.
 #
 # Other options to look into include
 # `oslo.concurrency`, `pylocker`, `portalocker`.
 from deprecation import deprecated
-from overrides import overrides
 
 from ._upath import FileInfo, LockAcquireError, LockReleaseError, Upath
 
 # End user may want to do this:
 # logging.getLogger("filelock").setLevel(logging.WARNING)
 
 
@@ -70,53 +69,48 @@
     def __setstate__(self, data):
         _, z1 = data
         self._lock_count = 0
         self._lock = None
         super().__setstate__(z1)
 
     @property
-    @overrides
     def path(self) -> pathlib.Path:
         """
         Return the `pathlib.Path <https://docs.python.org/3/library/pathlib.html#pathlib.Path>`_ object
         of the path.
         """
         return pathlib.Path(self._path)
 
     @property
     @deprecated(
         deprecated_in="0.6.9", removed_in="0.8.0", details="Use `path` instead."
     )
     def localpath(self):
         return self.path
 
-    @overrides
     def as_uri(self) -> str:
         """
         Represent the path as a file URI.
         On Linux, this is like 'file:///home/username/path/to/file'.
         On Windows, this is like 'file:///C:/Users/username/path/to/file'.
         """
         return self.path.as_uri()
 
-    @overrides
     def is_dir(self) -> bool:
         """
         Return whether the current path is a dir.
         """
         return self.path.is_dir()
 
-    @overrides
     def is_file(self) -> bool:
         """
         Return whether the current path is a file.
         """
         return self.path.is_file()
 
-    @overrides
     def file_info(self) -> Optional[FileInfo]:
         """
         Return file info if the current path is a file;
         otherwise return ``None``.
         """
         if not self.is_file():
             return None
@@ -130,35 +124,32 @@
             details=st,
         )
         # If an existing file is written to again using `write_...`,
         # then its `ctime` and `mtime` are both updated.
         # My experiments showed that `ctime` and `mtime` are equal.
 
     @property
-    @overrides
     def root(self) -> LocalUpath:
         """
         Return a new path representing the root.
 
         On Windows, this is the root on the same drive, like ``LocalUpath('C:\')``.
         On Linux and Mac, this is ``LocalUpath('/')``.
         """
         return self.__class__(self.path.root)
 
-    @overrides
     def read_bytes(self) -> bytes:
         """
         Read the content of the current file as bytes.
         """
         try:
             return self.path.read_bytes()
         except (IsADirectoryError, FileNotFoundError) as e:
             raise FileNotFoundError(self) from e
 
-    @overrides
     def write_bytes(
         self, data: bytes | BufferedReader, *, overwrite: bool = False
     ) -> None:
         """
         Write the bytes ``data`` to the current file.
         """
         if self.is_file():
@@ -172,39 +163,36 @@
         except TypeError:
             data = data.read()  # file-like object, like BytesIO, that is at beginning
         self.path.write_bytes(data)
 
         # If `self` is an existing directory, will raise `IsADirectoryError`.
         # If `self` is an existing file, will overwrite.
 
-    @overrides
     def _copy_file(self, target: Upath, *, overwrite: bool = False):
         if isinstance(target, LocalUpath):
             if not overwrite and target.is_file():
                 raise FileExistsError(target)
             os.makedirs(target.parent, exist_ok=True)
             # If `p` is a file and we try to `os.makedirs(p / 'subdir`)`,
             # on Linux it raises `NotADirectoryError`;
             # on Windows it raises `FileNotFoundError`.
             shutil.copyfile(self.path, target.path)
             # If target already exists, it will be overwritten.
         else:
             super()._copy_file(target, overwrite=overwrite)
 
-    @overrides
     def remove_dir(self, **kwargs) -> int:
         """
         Remove the current dir along with all its contents recursively.
         """
         n = super().remove_dir(**kwargs)
         if self.path.is_dir():
             shutil.rmtree(self.path)
         return n
 
-    @overrides
     def remove_file(self) -> None:
         """Remove the current file."""
         try:
             self.path.unlink()
         except PermissionError as e:  # this happens on Windows if `self` is a dir.
             if self.is_dir():
                 raise IsADirectoryError(self) from e
@@ -284,38 +272,35 @@
         target_ = self.parent / target
         if target_ == self:
             return self
 
         self._rename_file(target_._path, overwrite=overwrite)
         return target_
 
-    @overrides
     def iterdir(self) -> Iterator[LocalUpath]:
         """
         Yield the immediate children under the current dir.
         """
         try:
             for p in self.path.iterdir():
                 yield self / p.name
         except (NotADirectoryError, FileNotFoundError):
             pass
 
-    @overrides
     def riterdir(self) -> Iterator[LocalUpath]:
         """
         Yield all files under the current dir recursively.
         """
         for p in self.iterdir():
             if p.is_file():
                 yield p
             elif p.is_dir():
                 yield from p.riterdir()
 
     @contextlib.contextmanager
-    @overrides
     def lock(self, *, timeout=None):
         """
         This uses the package `filelock <https://github.com/tox-dev/py-filelock>`_ to implement
         a file lock for inter-process communication.
         """
         if timeout is None:
             timeout = 60
```

### Comparing `upathlib-0.7.5b2/src/upathlib/_tests.py` & `upathlib-0.7.6/src/upathlib/_tests.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.5b2/src/upathlib/_upath.py` & `upathlib-0.7.6/src/upathlib/_upath.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,30 +29,34 @@
 from io import BufferedReader, UnsupportedOperation
 from typing import (
     Any,
     Callable,
     Optional,
 )
 
-from deprecation import deprecated
 from mpservice.util import MAX_THREADS, get_shared_thread_pool
-from overrides import EnforceOverrides
 from tqdm.auto import tqdm
 from typing_extensions import Self
 
 from .serializer import (
     JsonSerializer,
-    OrjsonSerializer,
     PickleSerializer,
-    ZOrjsonSerializer,
     ZPickleSerializer,
-    ZstdOrjsonSerializer,
-    ZstdPickleSerializer,
 )
 
+try:
+    from .serializer import ZstdPickleSerializer
+except ImportError:
+    ZstdPickleSerializer = None
+try:
+    from .serializer import Lz4PickleSerializer
+except ImportError:
+    Lz4PickleSerializer = None
+
+
 # End user may want to do this:
 #  logging.getLogger('urllib3.connectionpool').setLevel(logging.ERROR)
 # to suppress the "urllib3 connection lost" warning.
 
 
 class LockAcquireError(TimeoutError):
     pass
@@ -69,15 +73,15 @@
     time_created: datetime.datetime  #: Creation time as an ``datetime`` object.
     time_modified: datetime.datetime  #: Last modification time as an ``datetime`` object.
     size: int  #: In bytes.
     details: Any  #: Platform-dependent.
 
 
 @functools.total_ordering
-class Upath(abc.ABC, EnforceOverrides):
+class Upath(abc.ABC):
     def __init__(
         self,
         *pathsegments: str,
     ):
         """
         Create a ``Upath`` instance. Because ``Upath`` is an abstract class,
         this is always called on a subclass to instantiate a path on the specific
@@ -633,83 +637,49 @@
 
     def read_pickle_z(self, **kwargs) -> Any:
         """
         ``**kwargs`` are passed to :meth:`serializer.ZPickleSerializer.deserialize`.
         """
         return ZPickleSerializer.deserialize(self.read_bytes(), **kwargs)
 
-    def write_pickle_zstd(self, data: Any, *, overwrite=False, **kwargs) -> None:
-        """
-        ``overwrite`` is passed to :meth:`write_bytes`.
-
-        ``**kwargs`` are passed to :meth:`serializer.ZstdPickleSerializer.serialize`.
-        """
-        self.write_bytes(
-            ZstdPickleSerializer.serialize(data, **kwargs), overwrite=overwrite
-        )
-
-    def read_pickle_zstd(self, **kwargs) -> Any:
-        """
-        ``**kwargs`` are passed to :meth:`serializer.ZstdPickleSerializer.deserialize`.
-        """
-        return ZstdPickleSerializer.deserialize(self.read_bytes(), **kwargs)
-
-    @deprecated(deprecated_in="0.7.3", removed_in="0.7.6")
-    def write_orjson(self, data: Any, *, overwrite=False, **kwargs) -> None:
-        """
-        ``overwrite`` is passed to :meth:`write_bytes`.
-
-        ``**kwargs`` are passed to :meth:`serializer.OrjsonSerializer.serialize`.
-        """
-        self.write_bytes(
-            OrjsonSerializer.serialize(data, **kwargs), overwrite=overwrite
-        )
-
-    @deprecated(deprecated_in="0.7.3", removed_in="0.7.6")
-    def read_orjson(self, **kwargs) -> Any:
-        """
-        ``**kwargs`` are passed to :meth:`serializer.OrjsonSerializer.deserialize`.
-        """
-        return OrjsonSerializer.deserialize(self.read_bytes(), **kwargs)
-
-    @deprecated(deprecated_in="0.7.3", removed_in="07.6")
-    def write_orjson_z(self, data: Any, *, overwrite=False, **kwargs) -> None:
-        """
-        ``overwrite`` is passed to :meth:`write_bytes`.
-
-        ``**kwargs`` are passed to :meth:`serializer.ZOrjsonSerializer.serialize`.
-        """
-        self.write_bytes(
-            ZOrjsonSerializer.serialize(data, **kwargs), overwrite=overwrite
-        )
-
-    @deprecated(deprecated_in="0.7.3", removed_in="0.7.6")
-    def read_orjson_z(self, **kwargs) -> Any:
-        """
-        ``**kwargs`` are passed to :meth:`serializer.ZOrjsonSerializer.deserialize`.
-        """
-        return ZOrjsonSerializer.deserialize(self.read_bytes(), **kwargs)
+    if ZstdPickleSerializer is not None:
 
-    @deprecated(deprecated_in="0.7.3", removed_in="0.7.6")
-    def write_orjson_zstd(self, data: Any, *, overwrite=False, **kwargs) -> None:
-        """
-        ``overwrite`` is passed to :meth:`write_bytes`.
+        def write_pickle_zstd(self, data: Any, *, overwrite=False, **kwargs) -> None:
+            """
+            ``overwrite`` is passed to :meth:`write_bytes`.
+
+            ``**kwargs`` are passed to :meth:`serializer.ZstdPickleSerializer.serialize`.
+            """
+            self.write_bytes(
+                ZstdPickleSerializer.serialize(data, **kwargs), overwrite=overwrite
+            )
 
-        ``**kwargs`` are passed to :meth:`serializer.ZstdOrjsonSerializer.serialize`.
-        """
-        self.write_bytes(
-            ZstdOrjsonSerializer.serialize(data, **kwargs), overwrite=overwrite
-        )
+        def read_pickle_zstd(self, **kwargs) -> Any:
+            """
+            ``**kwargs`` are passed to :meth:`serializer.ZstdPickleSerializer.deserialize`.
+            """
+            return ZstdPickleSerializer.deserialize(self.read_bytes(), **kwargs)
+
+    if Lz4PickleSerializer is not None:
+
+        def write_pickle_lz4(self, data: Any, *, overwrite=False, **kwargs) -> None:
+            """
+            ``overwrite`` is passed to :meth:`write_bytes`.
+
+            ``**kwargs`` are passed to :meth:`serializer.Lz4PickleSerializer.serialize`.
+            """
+            self.write_bytes(
+                Lz4PickleSerializer.serialize(data, **kwargs), overwrite=overwrite
+            )
 
-    @deprecated(deprecated_in="0.7.3", removed_in="0.7.6")
-    def read_orjson_zstd(self, **kwargs) -> Any:
-        """
-        ``**kwargs`` are passed to :meth:`serializer.ZstdOrjsonSerializer.deserialize`.
-        """
-        return ZstdOrjsonSerializer.deserialize(self.read_bytes(), **kwargs)
+        def read_pickle_lz4(self, **kwargs) -> Any:
+            """
+            ``**kwargs`` are passed to :meth:`serializer.Lz4PickleSerializer.deserialize`.
+            """
+            return Lz4PickleSerializer.deserialize(self.read_bytes(), **kwargs)
 
     def _copy_dir(
         self, source, dest, method: str, *, overwrite: bool, quiet: bool, reversed=False
     ):
         def foo():
             source_path = source.path
             ovwt = overwrite
```

### Comparing `upathlib-0.7.5b2/src/upathlib/azure.py` & `upathlib-0.7.6/src/upathlib/azure.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 # )
 from azure.core.exceptions import (
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
 )
 from azure.storage.blob import BlobClient, BlobLeaseClient, ContainerClient
-from overrides import overrides
 from typing_extensions import Self
 
 from ._blob import BlobUpath, LocalPathType, _resolve_local_path
 from ._upath import FileInfo, LockAcquireError, LockReleaseError, Upath
 
 # End user may want to do this:
 # logging.getLogger("azure.storage").setLevel(logging.WARNING)
@@ -95,29 +94,26 @@
         return "{}('{}', container_name='{}')".format(
             self.__class__.__name__, self._path, self._container_name
         )
 
     def __str__(self) -> str:
         return f"{self._container_name}://{self._path.lstrip('/')}"
 
-    @overrides
     def as_uri(self) -> str:
         # TODO: what's the conventional lead word for Azure?
         return f"azure://{self._container_name}/{self._path.lstrip('/')}"
 
     @property
     def container_name(self):
         return self._container_name
 
-    @overrides
     def is_file(self) -> bool:
         with self._provide_blob_client():
             return self._blob_client.exists()
 
-    @overrides
     def file_info(self):
         try:
             with self._provide_blob_client():
                 info = self._blob_client.get_blob_properties()
                 return FileInfo(
                     ctime=info.creation_time.timestamp(),
                     mtime=info.last_modified.timestamp(),
@@ -130,15 +126,14 @@
                 # `write_...(..., overwrite=True)`,
                 # then its `ctime` will not change; only `mtime`
                 # will be updated.
         except ResourceNotFoundError:
             return None
 
     @property
-    @overrides
     def root(self) -> AzureBlobUpath:
         """
         Return a new path representing the root of the same container.
         """
         return self.__class__(
             container_name=self._container_name,
         )
@@ -149,22 +144,20 @@
             with source._provide_blob_client():
                 copy = self._blob_client.start_copy_from_url(
                     source._blob_client.url,
                     requires_sync=True,
                 )
                 assert copy["copy_status"] == "success"
 
-    @overrides
     def _copy_file(self, target: Upath, *, overwrite=False):
         if isinstance(target, AzureBlobUpath):
             target._copy_file_from(self, overwrite=overwrite)
         else:
             super()._copy_file(target, overwrite=overwrite)
 
-    @overrides
     def download_file(self, target: LocalPathType, *, overwrite=False) -> None:
         target = _resolve_local_path(target)
         if target.is_file():
             if not overwrite:
                 raise FileExistsError(str(target))
             target.remove_file()
         elif target.is_dir():
@@ -174,28 +167,26 @@
             # TODO: check behavior of `download_blob` about
             # overwrite.
             os.makedirs(str(target.parent), exist_ok=True)
             with open(str(target), "wb") as f:
                 data = self._blob_client.download_blob()
                 data.readinto(f)
 
-    @overrides
     def upload_file(self, source: LocalPathType, *, overwrite: bool = False):
         source = _resolve_local_path(source)
         if self.is_file():
             if not overwrite:
                 # TODO: check the behavior of `upload_blob` related to
                 # behavior about overwrite.
                 raise FileExistsError(self)
             self.remove_file()
         with self._provide_blob_client():
             with open(str(source), "rb") as data:
                 self._blob_client.upload_blob(data)
 
-    @overrides
     def iterdir(self) -> Iterator[Self]:
         with self._provide_container_client():
             prefix = self.blob_name + "/"
             k = len(prefix)
             for p in self._container_client.walk_blobs(name_starts_with=prefix):
                 yield self / p.name[k:]
 
@@ -235,15 +226,14 @@
 
             t1 = time.perf_counter()
             if t1 - t0 >= timeout:
                 raise LockAcquireError(self, t1 - t0)
             time.sleep(random.uniform(0.05, 1.0))
 
     @contextmanager
-    @overrides
     def lock(self, *, timeout=None):
         """
         References:
         https://docs.microsoft.com/en-us/azure/storage/blobs/concurrency-manage?tabs=dotnet
         """
         with self._provide_blob_client():
             if self._lease is None:
@@ -322,42 +312,38 @@
                 with cc:
                     yield
             finally:
                 self._container_client = None
         else:
             yield
 
-    @overrides
     def read_bytes(self) -> bytes:
         with self._provide_blob_client():
             try:
                 return self._blob_client.download_blob().readall()
             except ResourceNotFoundError as e:
                 raise FileNotFoundError(self) from e
 
-    @overrides
     def remove_file(self):
         with self._provide_blob_client():
             try:
 
                 self._blob_client.delete_blob(
                     delete_snapshots="include", lease=self._lease
                 )
             except ResourceNotFoundError:
                 raise FileNotFoundError(self)
 
-    @overrides
     def riterdir(self) -> Iterator[Self]:
         with self._provide_container_client():
             prefix = self.blob_name + "/"
             k = len(prefix)
             for p in self._container_client.list_blobs(name_starts_with=prefix):
                 yield self / p.name[k:]
 
-    @overrides
     def write_bytes(self, data: bytes | BufferedReader, *, overwrite=False) -> None:
         if self._path == "/":
             raise UnsupportedOperation("can not write to root as a blob", self)
 
         with self._provide_blob_client():
             try:
                 self._blob_client.upload_blob(
```

### Comparing `upathlib-0.7.5b2/src/upathlib/gcs.py` & `upathlib-0.7.6/src/upathlib/gcs.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from google import resumable_media
 from google.api_core import exceptions
 from google.api_core.retry import if_exception_type
 from google.auth import exceptions as auth_exceptions
 from google.cloud import storage
 from google.cloud.storage.retry import DEFAULT_RETRY
 from mpservice.util import MAX_THREADS, get_shared_thread_pool
-from overrides import overrides
 from typing_extensions import Self
 
 from ._blob import BlobUpath, LocalPathType, _resolve_local_path
 from ._upath import FileInfo, LockAcquireError, LockReleaseError, Upath
 
 logger = logging.getLogger(__name__)
 
@@ -230,30 +229,27 @@
     def _blob(self) -> storage.Blob:
         """
         This constructs a Blob object irrespective of whether the blob
         exists in GCS.
         """
         return self._bucket().blob(self.blob_name)
 
-    @overrides
     def as_uri(self) -> str:
         """
         Represent the path as a file URI, like 'gs://bucket-name/path/to/blob'.
         """
         return f"gs://{self.bucket_name}/{self._path.lstrip('/')}"
 
-    @overrides
     def is_file(self) -> bool:
         """
         The result of this call is not cached, in case the object is modified anytime
         by other clients.
         """
         return self._blob().exists(self._client())
 
-    @overrides
     def is_dir(self) -> bool:
         """
         If there is a dummy blob with name ``f"{self.name}/"``,
         this will return ``True``.
         This is the case after creating a "folder" on the GCP dashboard.
         In programatic use, it's recommended to avoid such situations so that
         ``is_dir()`` returns ``True`` if and only if there are blobs
@@ -265,15 +261,14 @@
             prefix=prefix,
             max_results=1,
             page_size=1,
             fields="items(name),nextPageToken",
         )
         return len(list(blobs)) > 0
 
-    @overrides
     def file_info(self) -> Optional[FileInfo]:
         """
         Return file info if the current path is a file;
         otherwise return ``None``.
         """
         b = self._blob()
         try:
@@ -289,15 +284,14 @@
             details=b._properties,
         )
         # If an existing file is written to again using `write_...`,
         # then its `ctime` and `mtime` are both updated.
         # My experiments showed that `ctime` and `mtime` are equal.
 
     @property
-    @overrides
     def root(self) -> GcsBlobUpath:
         """
         Return a new path representing the root of the same bucket.
         """
         obj = self.__class__(
             bucket_name=self.bucket_name,
         )
@@ -326,15 +320,14 @@
             raise FileExistsError(self)
 
     def _write_bytes(self, data, **kwargs):
         b = BytesIO(data)
         b.seek(0)
         self._write_from_buffer(b, content_type="text/plain", size=len(data), **kwargs)
 
-    @overrides
     def write_bytes(self, data: bytes | BufferedReader, *, overwrite=False):
         """
         Write bytes ``data`` to the current blob.
 
         In the usual case, ``data`` is bytes.
         The case where ``data`` is a ``BufferedReader`` object, such as an open file,
         is not well tested.
@@ -413,15 +406,14 @@
                 self._blob().download_to_file(file_obj, client=self._client())
                 return
             except exceptions.NotFound:
                 raise FileNotFoundError(self)
         else:
             self._multipart_download(file_size, file_obj)
 
-    @overrides
     def read_bytes(self) -> bytes:
         """
         Return the content of the current blob as bytes.
         """
         buffer = BytesIO()
         self._read_into_buffer(buffer)
         return buffer.getvalue()
@@ -434,15 +426,14 @@
         f = DEFAULT_RETRY.with_predicate(if_exception_type(*RETRY_WRITE_ON_EXCEPTIONS))(
             func
         )
         # Apply this inside the function so that user could add elements
         # to ``RETRY_WRITE_ON_EXCEPTIONS``.
         return f(*args, **kwargs)
 
-    @overrides
     def _copy_file(self, target: Upath, *, overwrite=False) -> None:
         if isinstance(target, GcsBlobUpath):
             # https://cloud.google.com/storage/docs/copying-renaming-moving-objects
             try:
                 self._bucket().copy_blob(
                     self._blob(),
                     target._bucket(),
@@ -453,15 +444,14 @@
             except exceptions.NotFound:
                 raise FileNotFoundError(self)
             except exceptions.PreconditionFailed:
                 raise FileExistsError(target)
         else:
             super()._copy_file(target, overwrite=overwrite)
 
-    @overrides
     def download_file(self, target: LocalPathType, *, overwrite=False) -> None:
         """
         Download the content of the current blob to ``target``.
         """
         target = _resolve_local_path(target)
         if target.is_file():
             if not overwrite:
@@ -480,15 +470,14 @@
             if updated is not None:
                 mtime = updated.timestamp()
                 os.utime(target, (mtime, mtime))
         except resumable_media.DataCorruption:
             target.remove_file()
             raise
 
-    @overrides
     def upload_file(self, source: LocalPathType, *, overwrite=False) -> None:
         """
         Upload the content of ``source`` to the current blob.
         """
         source = _resolve_local_path(source)
         filename = str(source)
         content_type = self._blob()._get_content_type(None, filename=filename)
@@ -506,15 +495,14 @@
                     size=total_bytes,
                     content_type=content_type,
                     overwrite=overwrite,
                 )
 
         self._blob_rate_limit(_upload)
 
-    @overrides
     def iterdir(self) -> Iterator[Self]:
         """
         Yield immediate children under the current dir.
         """
         # From Google doc:
         #
         # Lists all the blobs in the bucket that begin with the prefix.
@@ -562,38 +550,35 @@
             obj = self / p.name[k:]  # files
             yield obj
         for p in blobs.prefixes:
             yield self / p[k:].rstrip("/")  # "subdirectories"
             # If this is an "empty subfolder", it is counted but it can be
             # misleading. User should avoid creating such empty folders.
 
-    @overrides
     def remove_dir(self, **kwargs) -> int:
         """
         Remove the current dir and all the content under it recursively.
         Return the number of blobs removed.
         """
         z = super().remove_dir(**kwargs)
         prefix = self.blob_name + "/"
         for p in self._client().list_blobs(self._bucket(), prefix=prefix):
             assert p.name.endswith("/")
             p.delete()
         return z
 
-    @overrides
     def remove_file(self) -> None:
         """
         Remove the current blob.
         """
         try:
             self._blob_rate_limit(self._blob().delete, client=self._client())
         except exceptions.NotFound:
             raise FileNotFoundError(self)
 
-    @overrides
     def riterdir(self) -> Iterator[Self]:
         """
         Yield all blobs recursively under the current dir.
         """
         prefix = self.blob_name + "/"
         k = len(prefix)
         for p in self._client().list_blobs(self._bucket(), prefix=prefix):
@@ -656,15 +641,14 @@
                 ) from e
         except Exception as e:
             raise LockAcquireError(
                 f"waited on '{self}' for {time.perf_counter() - t0:.2f} seconds"
             ) from e
 
     @contextlib.contextmanager
-    @overrides
     def lock(self, *, timeout: int | float = None):
         """
         This implementation does not prevent the file from being deleted
         by other workers that does not use the 'if-generation-match' condition.
         It relies on the assumption that this blob
         is used *cooperatively* solely in this locking logic.
```

### Comparing `upathlib-0.7.5b2/src/upathlib/serializer.py` & `upathlib-0.7.6/src/upathlib/serializer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 import abc
 import gc
 import json
 import pickle
 import zlib
 from typing import TypeVar
 
-import orjson
-import zstandard
+# zstandard has good compression ratio and also quite fast.
+# It is very "balanced".
+# lz4 has lower compression ratio than zstandard but is much faster.
+#
+# See:
+#   https://stackoverflow.com/questions/67537111/how-do-i-decide-between-lz4-and-snappy-compression
+#   https://gist.github.com/oldcai/7230548
 
 T = TypeVar("T")
 
 
 MEGABYTE = 1048576  # 1024 * 1024
 ZLIB_LEVEL = 3  # official default is 6
 ZSTD_LEVEL = 3  # official default is 3
+LZ4_LEVEL = (
+    0  # official default is 0; high-compression value is 3, much slower at compressing
+)
+PICKLE_PROTOCOL = pickle.HIGHEST_PROTOCOL
 
 
 def _loads(func, data, **kwargs):
     if len(data) < MEGABYTE:
         return func(data, **kwargs)
     isgc = gc.isenabled()
     if isgc:
@@ -25,107 +34,117 @@
     try:
         return func(data, **kwargs)
     finally:
         if isgc:
             gc.enable()
 
 
-class ByteSerializer(abc.ABC):
-    @classmethod
-    @abc.abstractmethod
-    def serialize(cls, x: T, **kwargs) -> bytes:
-        raise NotImplementedError
-
-    @classmethod
-    @abc.abstractmethod
-    def deserialize(cls, y: bytes, **kwargs) -> T:
-        raise NotImplementedError
-
-
 class TextSerializer(abc.ABC):
     @classmethod
     @abc.abstractmethod
     def serialize(cls, x: T, **kwargs) -> str:
         raise NotImplementedError
 
     @classmethod
     @abc.abstractmethod
     def deserialize(cls, y: str, **kwargs) -> T:
         raise NotImplementedError
 
 
-class PickleSerializer(ByteSerializer):
+class JsonSerializer(TextSerializer):
     @classmethod
-    def serialize(cls, x, *, protocol=None):
-        return pickle.dumps(x, protocol=protocol)
+    def serialize(cls, x, **kwargs):
+        return json.dumps(x, **kwargs)
 
     @classmethod
-    def deserialize(cls, y):
-        return _loads(pickle.loads, y)
+    def deserialize(cls, y, **kwargs):
+        return _loads(json.loads, y, **kwargs)
 
 
-class ZPickleSerializer(PickleSerializer):
+class ByteSerializer(abc.ABC):
     @classmethod
-    def serialize(cls, x, *, level=ZLIB_LEVEL, protocol=None):
-        y = super().serialize(x, protocol=protocol)
-        return zlib.compress(y, level=level)
+    @abc.abstractmethod
+    def serialize(cls, x: T, **kwargs) -> bytes:
+        raise NotImplementedError
 
     @classmethod
-    def deserialize(cls, y):
-        y = zlib.decompress(y)
-        return super().deserialize(y)
+    @abc.abstractmethod
+    def deserialize(cls, y: bytes, **kwargs) -> T:
+        raise NotImplementedError
 
 
-class ZstdPickleSerializer(PickleSerializer):
+class PickleSerializer(ByteSerializer):
     @classmethod
-    def serialize(cls, x, *, level=ZSTD_LEVEL, protocol=None):
-        y = super().serialize(x, protocol=protocol)
-        return zstandard.compress(y, level=level)
+    def serialize(cls, x, *, protocol=None):
+        return pickle.dumps(x, protocol=protocol or PICKLE_PROTOCOL)
 
     @classmethod
     def deserialize(cls, y):
-        y = zstandard.decompress(y)
-        return super().deserialize(y)
+        return _loads(pickle.loads, y)
 
 
-class JsonSerializer(TextSerializer):
-    @classmethod
-    def serialize(cls, x, **kwargs):
-        return json.dumps(x, **kwargs)
+def z_compress(x: bytes, level=ZLIB_LEVEL) -> bytes:
+    return zlib.compress(x, level=level)
 
-    @classmethod
-    def deserialize(cls, y, **kwargs):
-        return _loads(json.loads, y, **kwargs)
 
+def z_decompress(x: bytes) -> bytes:
+    return zlib.decompress(x)
 
-class OrjsonSerializer(ByteSerializer):
-    @classmethod
-    def serialize(cls, x, **kwargs):
-        return orjson.dumps(x, **kwargs)  # pylint: disable=no-member
 
+class ZPickleSerializer(PickleSerializer):
     @classmethod
-    def deserialize(cls, y):
-        return _loads(orjson.loads, y)  # pylint: disable=no-member
-
-
-class ZOrjsonSerializer(OrjsonSerializer):
-    @classmethod
-    def serialize(cls, x, *, level=ZLIB_LEVEL, **kwargs):
-        y = super().serialize(x, **kwargs)
-        return zlib.compress(y, level=level)
+    def serialize(cls, x, *, level=ZLIB_LEVEL, protocol=None):
+        y = super().serialize(x, protocol=protocol)
+        return z_compress(y, level=level)
 
     @classmethod
     def deserialize(cls, y):
-        y = zlib.decompress(y)
+        y = z_decompress(y)
         return super().deserialize(y)
 
 
-class ZstdOrjsonSerializer(OrjsonSerializer):
-    @classmethod
-    def serialize(cls, x, *, level=ZSTD_LEVEL, **kwargs):
-        y = super().serialize(x, **kwargs)
-        return zstandard.compress(y, level=level)
-
-    @classmethod
-    def deserialize(cls, y):
-        y = zstandard.decompress(y)
-        return super().deserialize(y)
+try:
+    import zstandard
+except ImportError:
+    pass
+else:
+
+    def zstd_compress(x: bytes, level=ZSTD_LEVEL) -> bytes:
+        return zstandard.compress(x, level=level)
+
+    def zstd_decompress(x: bytes) -> bytes:
+        return zstandard.decompress(x)
+
+    class ZstdPickleSerializer(PickleSerializer):
+        @classmethod
+        def serialize(cls, x, *, level=ZSTD_LEVEL, protocol=None):
+            y = super().serialize(x, protocol=protocol)
+            return zstd_compress(y, level=level)
+
+        @classmethod
+        def deserialize(cls, y):
+            y = zstd_decompress(y)
+            return super().deserialize(y)
+
+
+try:
+    import lz4.frame
+except ImportError:
+    pass
+else:
+
+    def lz4_compress(x: bytes, level=LZ4_LEVEL) -> bytes:
+        return lz4.frame.compress(x, compression_level=level)
+
+    def lz4_decompress(x: bytes) -> bytes:
+        return lz4.frame.decompress(x)
+
+    class Lz4PickleSerializer(PickleSerializer):
+        @classmethod
+        def serialize(cls, x, *, level=LZ4_LEVEL, protocol=None):
+            y = super().serialize(x, protocol=protocol)
+            return lz4_compress(y, level=level)
+
+        @classmethod
+        def deserialize(cls, y):
+            y = lz4_decompress(y)
+            return super().deserialize(y)
```

### Comparing `upathlib-0.7.5b2/PKG-INFO` & `upathlib-0.7.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 Metadata-Version: 2.1
 Name: upathlib
-Version: 0.7.5b2
+Version: 0.7.6
 Summary: The package *upathlib*
 Author-email: Zepu Zhang <zepu.zhang@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: filelock >= 3.9.1
 Requires-Dist: deprecation
-Requires-Dist: orjson
-Requires-Dist: overrides
 Requires-Dist: tqdm
-Requires-Dist: zstandard >=0.18.0
 Requires-Dist: typing-extensions
 Requires-Dist: mpservice >= 0.11.9
 Requires-Dist: azure-storage-blob >=12.9.0,<13.0 ; extra == "abs"
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: numpydoc ; extra == "doc"
 Requires-Dist: pydata-sphinx-theme ; extra == "doc"
 Requires-Dist: google-auth ; extra == "gcs"
 Requires-Dist: google-api-python-client >=2.13.9,<3.0 ; extra == "gcs"
 Requires-Dist: google-cloud-storage >=2.0,<3.0 ; extra == "gcs"
 Requires-Dist: requests ; extra == "gcs"
+Requires-Dist: lz4 ; extra == "lz4"
 Requires-Dist: black ; extra == "test"
 Requires-Dist: mypy ; extra == "test"
 Requires-Dist: numpy ; extra == "test"
 Requires-Dist: pytest-mock ; extra == "test"
 Requires-Dist: ruff ; extra == "test"
+Requires-Dist: zstandard ; extra == "zstandard"
 Project-URL: Source, https://github.com/zpz/upathlib
 Provides-Extra: abs
 Provides-Extra: doc
 Provides-Extra: gcs
+Provides-Extra: lz4
 Provides-Extra: test
+Provides-Extra: zstandard
 
 upathlib
 ========
 
 The package ``upathlib``
 defines a unified API for cloud blob store (aka "object store") as well as local file systems.
```

