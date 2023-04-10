# Comparing `tmp/biglist-0.7.8.tar.gz` & `tmp/biglist-0.7.9b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biglist-0.7.8.tar", last modified: Sun Mar 19 08:08:36 2023, max compression
+gzip compressed data, was "biglist-0.7.9b1.tar", last modified: Mon Apr 10 09:32:11 2023, max compression
```

## Comparing `biglist-0.7.8.tar` & `biglist-0.7.9b1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1067 2023-01-09 08:46:44.766242 biglist-0.7.8/LICENSE
--rw-r--r--   0        0        0      601 2023-01-09 08:46:44.766242 biglist-0.7.8/README.rst
--rw-r--r--   0        0        0     1443 2023-03-19 08:06:14.031668 biglist-0.7.8/pyproject.toml
--rw-r--r--   0        0        0     2215 2023-03-19 08:00:06.612370 biglist-0.7.8/src/biglist/__init__.py
--rw-r--r--   0        0        0    21313 2023-03-10 06:42:20.339391 biglist-0.7.8/src/biglist/_base.py
--rw-r--r--   0        0        0    49309 2023-03-19 08:03:00.661812 biglist-0.7.8/src/biglist/_biglist.py
--rw-r--r--   0        0        0    26119 2023-03-10 06:42:20.339391 biglist-0.7.8/src/biglist/_parquet.py
--rw-r--r--   0        0        0    19737 2023-03-11 19:27:43.873638 biglist-0.7.8/src/biglist/_util.py
--rw-r--r--   0        0        0        0 2023-01-09 08:46:44.766242 biglist-0.7.8/src/biglist/py.typed
--rw-r--r--   0        0        0     1792 1970-01-01 00:00:00.000000 biglist-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-01-09 08:46:44.766242 biglist-0.7.9b1/LICENSE
+-rw-r--r--   0        0        0      931 2023-03-22 00:51:16.691348 biglist-0.7.9b1/README.rst
+-rw-r--r--   0        0        0     1684 2023-04-10 09:18:54.169355 biglist-0.7.9b1/pyproject.toml
+-rw-r--r--   0        0        0     2217 2023-04-10 09:19:33.793840 biglist-0.7.9b1/src/biglist/__init__.py
+-rw-r--r--   0        0        0    18415 2023-04-10 09:27:34.589743 biglist-0.7.9b1/src/biglist/_base.py
+-rw-r--r--   0        0        0    45513 2023-04-10 09:27:34.429899 biglist-0.7.9b1/src/biglist/_biglist.py
+-rw-r--r--   0        0        0    33751 2023-03-30 06:44:24.186176 biglist-0.7.9b1/src/biglist/_parquet.py
+-rw-r--r--   0        0        0    12025 2023-03-30 06:41:51.563305 biglist-0.7.9b1/src/biglist/_util.py
+-rw-r--r--   0        0        0        0 2023-01-09 08:46:44.766242 biglist-0.7.9b1/src/biglist/py.typed
+-rw-r--r--   0        0        0     2273 1970-01-01 00:00:00.000000 biglist-0.7.9b1/PKG-INFO
```

### Comparing `biglist-0.7.8/LICENSE` & `biglist-0.7.9b1/LICENSE`

 * *Files identical despite different names*

### Comparing `biglist-0.7.8/pyproject.toml` & `biglist-0.7.9b1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -5,21 +5,20 @@
 
 [project]
 name = "biglist"
 authors = [
     {name = "Zepu Zhang", email = "zepu.zhang@gmail.com"},
 ]
 dependencies = [
-    "upathlib >= 0.7.3",
+    "upathlib >= 0.7.7b1",
     "deprecation",
     "mpservice >= 0.11.9",
     "orjson",
     "pyarrow >= 10.0.0",
     "typing-extensions",
-    "zstandard",
 ]
 requires-python = ">=3.8"
 readme = "README.rst"
 license = {file = "LICENSE"}
 classifiers = [
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
@@ -29,14 +28,16 @@
 
 
 [project.urls]
 Source = "https://github.com/zpz/biglist"
 
 
 [project.optional-dependencies]
+zstandard = ["upathlib[zstandard] >= 0.7.7b1"]
+lz4 = ["upathlib[lz4] >= 0.7.7b1"]
 doc = [
     "sphinx",
     "numpydoc",
     "pydata-sphinx-theme",
 ]
 gcs = [
     "upathlib[gcs] >= 0.7.3b1",
@@ -47,33 +48,37 @@
     "boltons",
     "mypy",
     "ruff",
     "pytest-asyncio",
 ]
 
 # `parquet` option became empty in 0.7.5 because `arrow` became mandatory.
+# To be removed later.
 
 
+# See https://beta.ruff.rs/docs/rules/
 [tool.ruff]
-target-version = "py38"
-select = ["E", "F", "I001"]  # isort
-ignore = ["E501"]  # line length
+target-version = "py310"
+select = ["E", "F", "S", "I001"]  # isort
+ignore = ["E501", "S101", "S102", "S103", "S104", "S108", "S301", "S311", "S608"]
 
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["E402", "F401"]
 
 
 [tool.pytest.ini_options]
 minversion = "6.0"
-addopts = "-sv --log-cli-level info -p no:cacheprovider --tb=short"
+testpaths = ["tests"]
+addopts = "-sv --log-cli-level info -p no:cacheprovider --tb=short --durations 3"
 
 
 [tool.coverage.report]
 fail_under = 85
 show_missing = true
 skip_empty = true
 
 
 [tool.coverage.run]
+source = ["biglist"]
 data_file = "/tmp/.coverage"
```

### Comparing `biglist-0.7.8/src/biglist/__init__.py` & `biglist-0.7.9b1/src/biglist/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,22 +34,22 @@
 from ._base import BiglistBase, FileReader, FileSeq
 from ._biglist import Biglist, BiglistFileReader, BiglistFileSeq, Multiplexer
 from ._parquet import (
     ParquetBatchData,
     ParquetBiglist,
     ParquetFileReader,
     ParquetFileSeq,
-    read_parquet_file,
-)
-from ._util import (
-    Chain,
-    Seq,
-    Slicer,
     make_parquet_field,
     make_parquet_schema,
     make_parquet_type,
+    read_parquet_file,
     write_arrays_to_parquet,
     write_parquet_file,
     write_pylist_to_parquet,
 )
+from ._util import (
+    Chain,
+    Seq,
+    Slicer,
+)
 
-__version__ = "0.7.8"
+__version__ = "0.7.9b1"
```

### Comparing `biglist-0.7.8/src/biglist/_base.py` & `biglist-0.7.9b1/src/biglist/_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,27 +4,25 @@
 import logging
 import os
 import queue
 import tempfile
 import uuid
 from abc import abstractmethod
 from collections.abc import Iterator
-from datetime import datetime
 from typing import (
     Any,
     Callable,
     Optional,
     TypeVar,
 )
 
-from deprecation import deprecated
 from mpservice.util import get_shared_thread_pool
 from upathlib import LocalUpath, PathType, Upath, resolve_path
 
-from ._util import Element, Seq, lock_to_use
+from ._util import Element, Seq
 
 logger = logging.getLogger(__name__)
 
 
 def _get_global_thread_pool():
     return get_shared_thread_pool("biglist")
 
@@ -175,82 +173,14 @@
         saves info about the data files, and any other info the implementation chooses
         to save.
 
         Note that this location does not need to be related to the location of the data files.
         """
         raise NotImplementedError
 
-    @deprecated(deprecated_in="0.7.7", removed_in="0.7.9")
-    def _concurrent_iter_info_file(self, task_id: str) -> Upath:
-        """
-        ``task_id``: returned by :meth:`new_concurrent_iter`.
-        """
-        return self.path / ".concurrent_file_iter" / task_id / "info.json"
-
-    @deprecated(deprecated_in="0.7.7", removed_in="0.7.9")
-    def new_concurrent_iter(self) -> str:
-        """
-        Initiate a concurrent iteration of the data files by multiple workers.
-
-        One worker, such as a "coordinator", calls this method and obtains a task-ID.
-        After that, one or more workers independently call :meth:`concurrent_iter`,
-        providing the task-ID, which they have received from the coordinator.
-        Each data file will be obtained by exactly one worker.
-
-        During this iteration, the data files should stay unchanged.
-        """
-        task_id = datetime.utcnow().isoformat()
-        self._concurrent_iter_info_file(task_id).write_json(
-            {"n_files_claimed": 0}, overwrite=False
-        )
-        return task_id
-
-    @deprecated(deprecated_in="0.7.7", removed_in="0.7.9")
-    def concurrent_iter(self, task_id: str) -> Iterator[FileReaderType]:
-        """
-        Parameters
-        ----------
-        task_id
-            The string returned by :meth:`new_concurrent_iter`.
-            All workers that call this method using the same ``task_id``
-            will consume the data files collectively.
-
-        .. seealso:: :meth:`__getitem__`, :meth:`new_concurrent_iter`
-        """
-        nfiles = self.__len__()
-        while True:
-            with lock_to_use(self._concurrent_iter_info_file(task_id)) as ff:
-                iter_info = ff.read_json()
-                n_files_claimed = iter_info["n_files_claimed"]
-                if n_files_claimed >= nfiles:
-                    # No more date files to process.
-                    break
-
-                iter_info["n_files_claimed"] = n_files_claimed + 1
-                ff.write_json(iter_info, overwrite=True)
-
-            logger.debug('yielding file #"%d"', n_files_claimed)
-            yield self.__getitem__(n_files_claimed)
-
-    @deprecated(deprecated_in="0.7.7", removed_in="0.7.9")
-    def concurrent_iter_stat(self, task_id: str) -> dict:
-        """Return status info for an ongoing "concurrent file iter"
-        identified by the task ID.
-
-        .. seealso: :meth:`new_concurrent_iter`.
-        """
-        info = self._concurrent_iter_info_file(task_id).read_json()
-        return {**info, "n_files": self.__len__()}
-
-    @deprecated(deprecated_in="0.7.7", removed_in="0.7.9")
-    def concurrent_iter_done(self, task_id: str) -> bool:
-        """Return whether the "concurrent file iter" identified by ``task_id`` is finished."""
-        zz = self.concurrent_iter_stat(task_id)
-        return zz["n_files_claimed"] >= zz["n_files"]
-
 
 class BiglistBase(Seq[Element]):
     """
     This base class contains code mainly concerning *reading*.
     The subclass :class:`~biglist.Biglist` adds functionalities for writing.
     Another subclass :class:`~biglist.ParquetBiglist` is read-only.
     Here, "reading" and "read-only" is talking about the *data files*.
@@ -436,17 +366,17 @@
         return self.num_data_items
 
     def _get_thread_pool(self):
         if self._thread_pool_ is None:
             self._thread_pool_ = _get_global_thread_pool()
         return self._thread_pool_
 
-    def destroy(self) -> None:
+    def destroy(self, *, concurrent=True) -> None:
         self.keep_files = False
-        self.path.rmrf()
+        self.path.rmrf(concurrent=concurrent)
 
     def __del__(self):
         if getattr(self, "keep_files", True) is False:
             self.destroy()
 
     def __getitem__(self, idx: int) -> Element:
         """
```

### Comparing `biglist-0.7.8/src/biglist/_biglist.py` & `biglist-0.7.9b1/src/biglist/_biglist.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,42 +10,40 @@
 import logging
 import multiprocessing
 import os
 import string
 import threading
 import warnings
 import weakref
-import zlib
 from collections.abc import Iterable, Iterator, Sequence
 from concurrent.futures import Future, ThreadPoolExecutor
 from datetime import datetime
 from typing import (
     Any,
     Callable,
     Optional,
 )
 from uuid import uuid4
 
 import orjson
 import pyarrow
-import zstandard
-from deprecation import deprecated
 from typing_extensions import Self
 from upathlib import serializer
 
 from ._base import (
     BiglistBase,
     Element,
     FileReader,
     FileSeq,
     PathType,
     Upath,
     resolve_path,
 )
-from ._util import lock_to_use, make_parquet_schema
+from ._parquet import make_parquet_schema
+from ._util import lock_to_use
 
 logger = logging.getLogger(__name__)
 
 
 _biglist_objs = weakref.WeakSet()
 
 
@@ -401,15 +399,15 @@
                     if new_info:
                         self.info["data_files_info"] = new_info
                         with lock_to_use(self._info_file) as ff:
                             ff.write_json(self.info, overwrite=True)
 
     def __del__(self) -> None:
         if getattr(self, "keep_files", True) is False:
-            self.destroy()
+            self.destroy(concurrent=False)
         else:
             if not self._flushed:
                 warnings.warn(
                     f"did you forget to flush {self.__class__.__name__} at '{self.path}'?"
                 )
             self.flush()
 
@@ -654,135 +652,14 @@
             [
                 (str(self.data_path / row[0]), *row[1:])
                 for row in self.info["data_files_info"]
             ],
             fun,
         )
 
-    @deprecated(
-        deprecated_in="0.7.7",
-        removed_in="0.7.9",
-        details="Use ``Multiplexer`` instead.",
-    )
-    def _multiplex_info_file(self, task_id: str) -> Upath:
-        """
-        `task_id`: returned by :meth:`new_multiplexer`.
-        """
-        return self.path / ".multiplexer" / task_id / "info.json"
-
-    @deprecated(
-        deprecated_in="0.7.7",
-        removed_in="0.7.9",
-        details="Use ``Multiplexer`` instead.",
-    )
-    def new_multiplexer(self) -> str:
-        """
-        One worker, such as a "coordinator", calls this method once.
-        After that, one or more workers independently call :meth:`multiplex_iter`
-        to iterate over the :class:`Biglist`. :meth:`multiplex_iter` takes the task-ID returned by
-        this method. The content of the :class:`Biglist` is
-        split between the workers in that each data element will be obtained
-        by exactly one worker.
-
-        During this iteration, the :class:`Biglist` object should stay unchanged---no
-        calls to :meth:`append` and :meth:`extend`.
-
-        Difference between :meth:`~_base.BiglistBase.concurrent_iter_files` and :meth:`multiplex_iter`: the former
-        distributes files to workers, whereas the latter distributes individual
-        data elements to workers.
-
-        The intended use case of multiplexer: each data element represents considerable amounts
-        of work--it is a "hyper-parameter" or the like; :meth:`multiplex_iter` facilitates
-        splitting the work represented by different values of this "hyper-parameter"
-        between multiple workers.
-        """
-        assert not self._append_buffer
-        if not self._flushed:
-            warnings.warn(
-                f"did you forget to flush {self.__class__.__name__} at '{self.path}'?"
-            )
-        task_id = datetime.utcnow().isoformat()
-        self._multiplex_info_file(task_id).write_json(
-            {
-                "total": len(self),
-                "next": 0,
-                "time": datetime.utcnow().isoformat(),
-            },
-            overwrite=False,
-        )
-        return task_id
-
-    @deprecated(
-        deprecated_in="0.7.7",
-        removed_in="0.7.9",
-        details="Use ``Multiplexer`` instead.",
-    )
-    def multiplex_iter(
-        self, task_id: str, worker_id: Optional[str] = None
-    ) -> Iterator[Element]:
-        """
-        Parameters
-        ----------
-        task_id
-            The string returned by :meth:`new_multiplexer`.
-        worker_id
-            A string representing a particular worker. If missing,
-            a default is constructed based on thread name and process name of the worker.
-        """
-        if not worker_id:
-            worker_id = "{} {}".format(
-                multiprocessing.current_process().name,
-                threading.current_thread().name,
-            )
-        finfo = self._multiplex_info_file(task_id)
-        while True:
-            with lock_to_use(finfo) as ff:
-                # In concurrent use cases, I've observed
-                # `upathlib.LockAcquireError` raised here.
-                # User may want to do retry here.
-                ss = ff.read_json()
-                # In concurrent use cases, I've observed
-                # `FileNotFoundError` here. User may want
-                # to do retry here.
-
-                n = ss["next"]
-                if n == ss["total"]:
-                    return
-                ff.write_json(
-                    {
-                        "next": n + 1,
-                        "worker_id": worker_id,
-                        "time": datetime.utcnow().isoformat(),
-                        "total": ss["total"],
-                    },
-                    overwrite=True,
-                )
-            yield self[n]
-
-    @deprecated(
-        deprecated_in="0.7.7",
-        removed_in="0.7.9",
-        details="Use ``Multiplexer`` instead.",
-    )
-    def multiplex_stat(self, task_id: str) -> dict:
-        """
-        Return status info of an ongoing "multiplex iter".
-        """
-        return self._multiplex_info_file(task_id).read_json()
-
-    @deprecated(
-        deprecated_in="0.7.7",
-        removed_in="0.7.9",
-        details="Use ``Multiplexer`` instead.",
-    )
-    def multiplex_done(self, task_id: str) -> bool:
-        """Return whether the "multiplex iter" identified by ``task_id`` is finished."""
-        ss = self.multiplex_stat(task_id)
-        return ss["next"] == ss["total"]
-
 
 class Dumper:
     """
     This class performs file-saving in a thread pool.
 
     Parameters
     ----------
@@ -936,31 +813,19 @@
         return serializer._loads(orjson.loads, y)  # pylint: disable=no-member
 
 
 class ZOrjsonSerializer(OrjsonSerializer):
     @classmethod
     def serialize(cls, x, *, level=serializer.ZLIB_LEVEL, **kwargs):
         y = super().serialize(x, **kwargs)
-        return zlib.compress(y, level=level)
+        return serializer.z_compress(y, level=level)
 
     @classmethod
     def deserialize(cls, y):
-        y = zlib.decompress(y)
-        return super().deserialize(y)
-
-
-class ZstdOrjsonSerializer(OrjsonSerializer):
-    @classmethod
-    def serialize(cls, x, *, level=serializer.ZSTD_LEVEL, **kwargs):
-        y = super().serialize(x, **kwargs)
-        return zstandard.compress(y, level=level)
-
-    @classmethod
-    def deserialize(cls, y):
-        y = zstandard.decompress(y)
+        y = serializer.z_decompress(y)
         return super().deserialize(y)
 
 
 class ParquetSerializer(serializer.ByteSerializer):
     @classmethod
     def serialize(
         cls,
@@ -1025,21 +890,53 @@
         table = pyarrow.parquet.ParquetFile(y, **kwargs).read()
         return table.to_pylist()
 
 
 Biglist.register_storage_format("json", JsonByteSerializer)
 Biglist.register_storage_format("pickle", serializer.PickleSerializer)
 Biglist.register_storage_format("pickle-z", serializer.ZPickleSerializer)
-Biglist.register_storage_format("pickle-zstd", serializer.ZstdPickleSerializer)
 Biglist.register_storage_format("orjson", OrjsonSerializer)
 Biglist.register_storage_format("orjson-z", ZOrjsonSerializer)
-Biglist.register_storage_format("orjson-zstd", ZstdOrjsonSerializer)
 Biglist.register_storage_format("parquet", ParquetSerializer)
 
 
+if hasattr(serializer, 'zstd_compress'):
+
+    class ZstdOrjsonSerializer(OrjsonSerializer):
+        @classmethod
+        def serialize(cls, x, *, level=serializer.ZSTD_LEVEL, **kwargs):
+            y = super().serialize(x, **kwargs)
+            return serializer.zstd_compress(y, level=level)
+
+        @classmethod
+        def deserialize(cls, y):
+            y = serializer.zstd_decompress(y)
+            return super().deserialize(y)
+
+    Biglist.register_storage_format("pickle-zstd", serializer.ZstdPickleSerializer)
+    Biglist.register_storage_format("orjson-zstd", ZstdOrjsonSerializer)
+
+
+if hasattr(serializer, 'lz4_compress'):
+
+    class Lz4OrjsonSerializer(OrjsonSerializer):
+        @classmethod
+        def serialize(cls, x, *, level=serializer.LZ4_LEVEL, **kwargs):
+            y = super().serialize(x, **kwargs)
+            return serializer.lz4_compress(y, level=level)
+
+        @classmethod
+        def deserialize(cls, y):
+            y = serializer.lz4_decompress(y)
+            return super().deserialize(y)
+
+    Biglist.register_storage_format("pickle-lz4", serializer.Lz4PickleSerializer)
+    Biglist.register_storage_format("orjson-lz4", Lz4OrjsonSerializer)
+
+
 class Multiplexer:
     """
     Multiplexer is used to distribute data elements to multiple "workers" so that
     each element is obtained by exactly one worker.
 
     Typically, the data element is small in size but requires significant time to process
     by the worker. The data elements are "hyper parameters".
```

### Comparing `biglist-0.7.8/src/biglist/_parquet.py` & `biglist-0.7.9b1/src/biglist/_parquet.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from __future__ import annotations
 
 import itertools
 import logging
-from collections.abc import Iterator, Sequence
+from collections.abc import Iterable, Iterator, Sequence
 from pathlib import Path
 from typing import Any, Callable, Optional
 
 import pyarrow
+from deprecation import deprecated
 from pyarrow.fs import FileSystem, GcsFileSystem
 from pyarrow.parquet import FileMetaData, ParquetFile
+from upathlib import LocalUpath, PathType, Upath, resolve_path
 
 from ._base import (
     BiglistBase,
     FileReader,
     FileSeq,
-    PathType,
     Seq,
-    Upath,
     _get_global_thread_pool,
-    resolve_path,
 )
 from ._util import locate_idx_in_chunked_seq, lock_to_use
 
 # If data is in Google Cloud Storage, `pyarrow.fs.GcsFileSystem` accepts "access_token"
 # and "credential_token_expiration". These can be obtained via
 # a "google.oauth2.service_account.Credentials" object, e.g.
 #
@@ -721,7 +720,227 @@
     """
     Parameters
     ----------
     path
         Path of the file.
     """
     return ParquetFileReader(path, ParquetBiglist.load_data_file)
+
+
+def make_parquet_type(type_spec: str | Sequence):
+    """
+    ``type_spec`` is a spec of arguments to one of pyarrow's data type
+    `factory functions <https://arrow.apache.org/docs/python/api/datatypes.html#factory-functions>`_.
+
+    For simple types, this may be just the type name (or function name), e.g. ``'bool_'``, ``'string'``, ``'float64'``.
+
+    For type functions expecting arguments, this is a list or tuple with the type name followed by other arguments,
+    for example,
+
+    ::
+
+        ('time32', 's')
+        ('decimal128', 5, -3)
+
+    For compound types (types constructed by other types), this is a "recursive" structure, such as
+
+    ::
+
+        ('list_', 'int64')
+        ('list_', ('time32', 's'), 5)
+
+    where the second element is the spec for the member type, or
+
+    ::
+
+        ('map_', 'string', ('list_', 'int64'), True)
+
+    where the second and third elements are specs for the key type and value type, respectively,
+    and the fourth element is the optional argument ``keys_sorted`` to
+    `pyarrow.map_() <https://arrow.apache.org/docs/python/generated/pyarrow.map_.html#pyarrow.map_>`_.
+    Below is an example of a struct type::
+
+        ('struct', [('name', 'string', False), ('age', 'uint8', True), ('income', ('struct', (('currency', 'string'), ('amount', 'uint64'))), False)])
+
+    Here, the second element is the list of fields in the struct.
+    Each field is expressed by a spec that is taken by :meth:`make_parquet_field`.
+    """
+    if isinstance(type_spec, str):
+        type_name = type_spec
+        args = ()
+    else:
+        type_name = type_spec[0]
+        args = type_spec[1:]
+
+    # print('\ntype_spec', type_spec)
+    # print('type_name', type_name)
+    # print('type_args', args)
+
+    if type_name in ("string", "float64", "bool_", "int8", "int64", "uint8", "uint64"):
+        assert not args
+        return getattr(pyarrow, type_name)()
+
+    if type_name == "list_":
+        if len(args) > 2:
+            raise ValueError(f"'pyarrow.list_' expects 1 or 2 args, got `{args}`")
+        return pyarrow.list_(make_parquet_type(args[0]), *args[1:])
+
+    if type_name in ("map_", "dictionary"):
+        if len(args) > 3:
+            raise ValueError(f"'pyarrow.{type_name}' expects 2 or 3 args, got `{args}`")
+        return getattr(pyarrow, type_name)(
+            make_parquet_type(args[0]),
+            make_parquet_type(args[1]),
+            *args[2:],
+        )
+
+    if type_name == "struct":
+        assert len(args) == 1
+        return pyarrow.struct((make_parquet_field(v) for v in args[0]))
+
+    if type_name == "large_list":
+        assert len(args) == 1
+        return pyarrow.large_list(make_parquet_type(args[0]))
+
+    if type_name in (
+        "int16",
+        "int32",
+        "uint16",
+        "uint32",
+        "float32",
+        "date32",
+        "date64",
+        "month_day_nano_interval",
+        "utf8",
+        "large_binary",
+        "large_string",
+        "large_utf8" "null",
+    ):
+        assert not args
+        return getattr(pyarrow, type_name)()
+
+    if type_name in ("time32", "time64", "duration"):
+        assert len(args) == 1
+    elif type_name in ("timestamp", "decimal128"):
+        assert len(args) in (1, 2)
+    elif type_name in ("binary",):
+        assert len(args) <= 1
+    else:
+        raise ValueError(f"unknown pyarrow type '{type_name}'")
+    return getattr(pyarrow, type_name)(*args)
+
+
+def make_parquet_field(field_spec: Sequence):
+    """
+    ``filed_spec`` is a list or tuple with 2, 3, or 4 elements.
+    The first element is the name of the field.
+    The second element is the spec of the type, to be passed to function :func:`make_parquet_type`.
+    Additional elements are the optional ``nullable`` and ``metadata`` to the function
+    `pyarrow.field() <https://arrow.apache.org/docs/python/generated/pyarrow.field.html#pyarrow.field>`_.
+    """
+    # print('\nfield_spec:', field_spec)
+    field_name = field_spec[0]
+    type_spec = field_spec[1]
+    assert len(field_spec) <= 4  # two optional elements are `nullable` and `metadata`.
+    return pyarrow.field(field_name, make_parquet_type(type_spec), *field_spec[3:])
+
+
+def make_parquet_schema(fields_spec: Iterable[Sequence]):
+    """
+    This function constructs a pyarrow schema that is expressed by simple Python types
+    that can be json-serialized.
+
+    ``fields_spec`` is a list or tuple, each of its elements accepted by :func:`make_parquet_field`.
+
+    This function is motivated by the need of :class:`~biglist._biglist.ParquetSerializer`.
+    When :class:`biglist.Biglist` uses a "storage-format" that takes options (such as 'parquet'),
+    these options can be passed into :func:`biglist.Biglist.new` (via ``serialize_kwargs`` and ``deserialize_kwargs``) and saved in "info.json".
+    However, this requires the options to be json-serializable.
+    Therefore, the argument ``schema`` to :meth:`ParquetSerializer.serialize() <biglist._biglist.ParquetSerializer.serialize>`
+    can not be used by this mechanism.
+    As an alternative, user can use the argument ``schema_spec``;
+    this argument can be saved in "info.json", and it is handled by this function.
+    """
+    return pyarrow.schema((make_parquet_field(v) for v in fields_spec))
+
+
+def write_parquet_table(
+    table: pyarrow.Table,
+    path: PathType,
+    **kwargs,
+) -> None:
+    """
+    If the file already exists, it will be overwritten.
+
+    Parameters
+    ----------
+    path
+        Path of the file to create and write to.
+    table
+        pyarrow Table object.
+    **kwargs
+        Passed on to `pyarrow.parquet.write_table() <https://arrow.apache.org/docs/python/generated/pyarrow.parquet.write_table.html>`_.
+    """
+    path = resolve_path(path)
+    if isinstance(path, LocalUpath):
+        path.parent.path.mkdir(exist_ok=True, parents=True)
+    ff, pp = FileSystem.from_uri(str(path))
+    if isinstance(ff, GcsFileSystem):
+        from ._parquet import ParquetBiglist
+
+        ff = ParquetBiglist.get_gcsfs()
+    pyarrow.parquet.write_table(table, ff.open_output_stream(pp), **kwargs)
+
+
+def write_arrays_to_parquet(
+    data: Sequence[pyarrow.Array | pyarrow.ChunkedArray | Iterable],
+    path: PathType,
+    *,
+    names: Optional[Sequence[str]],
+    **kwargs,
+) -> None:
+    """
+    Parameters
+    ----------
+    path
+        Path of the file to create and write to.
+    data
+        A list of data arrays.
+    names
+        List of names for the arrays in ``data``.
+    **kwargs
+        Passed on to `pyarrow.parquet.write_table() <https://arrow.apache.org/docs/python/generated/pyarrow.parquet.write_table.html>`_.
+    """
+    assert len(names) == len(data)
+    arrays = [
+        a if isinstance(a, (pyarrow.Array, pyarrow.ChunkedArray)) else pyarrow.array(a)
+        for a in data
+    ]
+    table = pyarrow.Table.from_arrays(arrays, names=names)
+    return write_parquet_table(table, path, **kwargs)
+
+
+def write_pylist_to_parquet(
+    data: Sequence,
+    path: PathType,
+    *,
+    schema=None,
+    schema_spec=None,
+    metadata=None,
+    **kwargs,
+):
+    if schema is not None:
+        assert schema_spec is None
+    elif schema_spec is not None:
+        assert schema is None
+        schema = make_parquet_schema(schema_spec)
+    table = pyarrow.Table.from_pylist(data, schema=schema, metadata=metadata)
+    return write_parquet_table(table, path, **kwargs)
+
+
+@deprecated(
+    deprecated_in="0.7.7",
+    removed_in="0.8.0",
+    details="Use ``write_arrays_to_parquet`` instead.",
+)
+def write_parquet_file(path, data, names, **kwargs):
+    return write_arrays_to_parquet(data, path, names=names, **kwargs)
```

