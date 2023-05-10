# Comparing `tmp/biglist-0.8.1.tar.gz` & `tmp/biglist-0.8.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biglist-0.8.1.tar", last modified: Mon Apr 24 18:37:43 2023, max compression
+gzip compressed data, was "biglist-0.8.2b1.tar", last modified: Wed May 10 04:35:28 2023, max compression
```

## Comparing `biglist-0.8.1.tar` & `biglist-0.8.2b1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1067 2023-01-09 08:46:44.766242 biglist-0.8.1/LICENSE
--rw-r--r--   0        0        0      931 2023-04-10 09:40:14.837561 biglist-0.8.1/README.rst
--rw-r--r--   0        0        0     1527 2023-04-24 18:36:06.413180 biglist-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     2215 2023-04-24 18:28:48.591995 biglist-0.8.1/src/biglist/__init__.py
--rw-r--r--   0        0        0    18004 2023-04-24 18:29:53.379253 biglist-0.8.1/src/biglist/_base.py
--rw-r--r--   0        0        0    44435 2023-04-24 18:32:33.472154 biglist-0.8.1/src/biglist/_biglist.py
--rw-r--r--   0        0        0    34773 2023-04-18 03:17:34.278504 biglist-0.8.1/src/biglist/_parquet.py
--rw-r--r--   0        0        0    12025 2023-04-14 07:17:29.111106 biglist-0.8.1/src/biglist/_util.py
--rw-r--r--   0        0        0        0 2023-01-09 08:46:44.766242 biglist-0.8.1/src/biglist/py.typed
--rw-r--r--   0        0        0     2179 1970-01-01 00:00:00.000000 biglist-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-01-09 08:46:44.766242 biglist-0.8.2b1/LICENSE
+-rw-r--r--   0        0        0      844 2023-05-10 04:18:49.342974 biglist-0.8.2b1/README.rst
+-rw-r--r--   0        0        0     1527 2023-04-26 03:52:56.948542 biglist-0.8.2b1/pyproject.toml
+-rw-r--r--   0        0        0     2193 2023-05-10 04:27:34.423850 biglist-0.8.2b1/src/biglist/__init__.py
+-rw-r--r--   0        0        0    17969 2023-04-26 03:52:56.948542 biglist-0.8.2b1/src/biglist/_base.py
+-rw-r--r--   0        0        0    44336 2023-05-10 04:10:02.906662 biglist-0.8.2b1/src/biglist/_biglist.py
+-rw-r--r--   0        0        0    34440 2023-05-10 04:22:39.780895 biglist-0.8.2b1/src/biglist/_parquet.py
+-rw-r--r--   0        0        0    11997 2023-04-26 03:52:56.948542 biglist-0.8.2b1/src/biglist/_util.py
+-rw-r--r--   0        0        0        0 2023-01-09 08:46:44.766242 biglist-0.8.2b1/src/biglist/py.typed
+-rw-r--r--   0        0        0     2094 1970-01-01 00:00:00.000000 biglist-0.8.2b1/PKG-INFO
```

### Comparing `biglist-0.8.1/LICENSE` & `biglist-0.8.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `biglist-0.8.1/README.rst` & `biglist-0.8.2b1/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -24,8 +24,7 @@
 
 Python version
 --------------
 
 Development and testing were conducted in Python 3.8 until version 0.7.8.
 Starting with 0.7.9, development and testing happen in Python 3.10.
 Code continues to NOT intentionally use features beyond Python 3.8.
-I intend to test agsint versions 3.8, 3.9, 3.10, 3.11 once I find time to set that up.
```

### Comparing `biglist-0.8.1/pyproject.toml` & `biglist-0.8.2b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [project]
 name = "biglist"
 authors = [
     {name = "Zepu Zhang", email = "zepu.zhang@gmail.com"},
 ]
 dependencies = [
-    "upathlib >= 0.7.9",
+    "upathlib >= 0.8.0",
     "deprecation",
     "mpservice >= 0.12.5",
     "pyarrow >= 10.0.0",
     "typing-extensions",
 ]
 requires-python = ">=3.8"
 readme = "README.rst"
@@ -35,15 +35,15 @@
 lz4 = ["lz4"]
 doc = [
     "sphinx",
     "numpydoc",
     "pydata-sphinx-theme",
 ]
 gcs = [
-    "upathlib[gcs] >= 0.7.9",
+    "upathlib[gcs] >= 0.8.0",
     "google-auth",
 ]
 test = [
     "boltons",
     "mypy",
     "ruff",
     "pytest-asyncio",
```

### Comparing `biglist-0.8.1/src/biglist/__init__.py` & `biglist-0.8.2b1/src/biglist/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,16 @@
     ParquetFileReader,
     ParquetFileSeq,
     make_parquet_field,
     make_parquet_schema,
     make_parquet_type,
     read_parquet_file,
     write_arrays_to_parquet,
-    write_parquet_file,
     write_pylist_to_parquet,
 )
 from ._util import (
     Chain,
     Seq,
     Slicer,
 )
 
-__version__ = "0.8.1"
+__version__ = "0.8.2b1"
```

### Comparing `biglist-0.8.1/src/biglist/_base.py` & `biglist-0.8.2b1/src/biglist/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,15 @@
 import logging
 import os
 import queue
 import tempfile
 import uuid
 from abc import abstractmethod
 from collections.abc import Iterator
-from typing import (
-    Optional,
-    TypeVar,
-)
+from typing import TypeVar
 
 from mpservice.concurrent.futures import get_shared_thread_pool
 from upathlib import LocalUpath, PathType, Upath, resolve_path
 
 from ._util import Element, Seq
 
 logger = logging.getLogger(__name__)
@@ -195,17 +192,17 @@
             os.path.abspath(tempfile.gettempdir()), str(uuid.uuid4())
         )  # type: ignore
         return path  # type: ignore
 
     @classmethod
     def new(
         cls,
-        path: Optional[PathType] = None,
+        path: PathType | None = None,
         *,
-        keep_files: Optional[bool] = None,
+        keep_files: bool | None = None,
         init_info: dict = None,
         **kwargs,
     ) -> BiglistBase:
         """
         Create a new object of this class (of a subclass, to be precise) and then add data to it.
 
         Parameters
@@ -316,17 +313,17 @@
         path
             Directory that contains files written by an instance
             of this class.
         """
         self.path: Upath = resolve_path(path)
         """Root directory of the storage space for this object."""
 
-        self._read_buffer: Optional[Seq[Element]] = None
+        self._read_buffer: Seq[Element] | None = None
         self._read_buffer_file_idx = None
-        self._read_buffer_item_range: Optional[tuple[int, int]] = None
+        self._read_buffer_item_range: tuple[int, int] | None = None
         # `self._read_buffer` contains the content of the file
         # indicated by `self._read_buffer_file_idx`.
 
         self._thread_pool_ = None
 
         self.info: dict
         """Various meta info."""
```

### Comparing `biglist-0.8.1/src/biglist/_biglist.py` & `biglist-0.8.2b1/src/biglist/_biglist.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,15 @@
 import string
 import threading
 import warnings
 import weakref
 from collections.abc import Iterable, Iterator, Sequence
 from concurrent.futures import Future, ThreadPoolExecutor
 from datetime import datetime
-from typing import (
-    Any,
-    Callable,
-    Optional,
-)
+from typing import Any, Callable
 from uuid import uuid4
 
 import pyarrow
 from typing_extensions import Self
 from upathlib import serializer
 
 from ._base import (
@@ -161,20 +157,20 @@
         ]
         data = path.read_bytes()
         return deserializer.deserialize(data, **kwargs)
 
     @classmethod
     def new(
         cls,
-        path: Optional[PathType] = None,
+        path: PathType | None = None,
         *,
-        batch_size: Optional[int] = None,
-        storage_format: Optional[str] = None,
-        serialize_kwargs: Optional[dict] = None,
-        deserialize_kwargs: Optional[dict] = None,
+        batch_size: int | None = None,
+        storage_format: str | None = None,
+        serialize_kwargs: dict | None = None,
+        deserialize_kwargs: dict | None = None,
         init_info: dict = None,
         **kwargs,
     ) -> Self:
         """
         Parameters
         ----------
         path
@@ -292,14 +288,21 @@
         """
         Please see the base class for additional documentation.
         """
         super().__init__(*args, **kwargs)
         self.keep_files: bool = True
         """Indicates whether the persisted files should be kept or deleted when the object is garbage-collected."""
 
+        self._flushed = True
+        # Set this early in case ``__del__`` is triggered before ``__init__`` finishes.
+        # If True, some changes have been made but `.flush` has not been called.
+        # Note it's about `.flush()`, not `._flush()`.
+        # This flag exists to remind user that they need to call `.flush()` at the end
+        # of their writing session.
+
         self._append_buffer: list = []
         self._append_files_buffer: list = []
         self._file_dumper = None
         self._n_write_threads = 3
         self._serialize_kwargs = self.info.get("serialize_kwargs", {})
         self._deserialize_kwargs = self.info.get("deserialize_kwargs", {})
         if self.storage_format == "parquet" and "schema_spec" in self._serialize_kwargs:
@@ -308,15 +311,14 @@
             assert "schema" not in self._serialize_kwargs
             kk = copy.deepcopy(self._serialize_kwargs)
             kk["schema"] = make_parquet_schema(kk["schema_spec"])
             del kk["schema_spec"]
             self._serialize_kwargs = kk
 
         _biglist_objs.add(self)
-        self._flushed = True
 
         # For back compat.
         if self.info.get("storage_version", 0) < 3:
             # This is not called by ``new``, instead is opening an existing dataset.
             # Usually these legacy datasets are in a "read-only" mode, i.e., you should
             # not append more data to them. If you do, the back-compat code below
             # may not be totally reliable if the dataset is being used by multiple workers
@@ -400,18 +402,15 @@
                         with lock_to_use(self._info_file) as ff:
                             ff.write_json(self.info, overwrite=True)
 
     def __del__(self) -> None:
         if getattr(self, "keep_files", True) is False:
             self.destroy(concurrent=False)
         else:
-            if not getattr(self, '_flushed', True):
-                warnings.warn(
-                    f"did you forget to flush {self.__class__.__name__} at '{self.path}'?"
-                )
+            self._warn_flush()
             self.flush()
 
     @property
     def batch_size(self) -> int:
         """The max number of data items in one data file."""
         return self.info["batch_size"]
 
@@ -425,30 +424,33 @@
         return self.info["storage_format"].replace("_", "-")
 
     @property
     def storage_version(self) -> int:
         """The internal format used in persistence. This is a read-only attribute for information only."""
         return self.info.get("storage_version", 0)
 
+    def _warn_flush(self):
+        if not self._flushed:
+            warnings.warn(
+                f"did you forget to flush {self.__class__.__name__} at '{self.path}'?"
+            )
+
     def __len__(self) -> int:
         """
         Number of data items in this biglist.
 
         If data is being appended to this biglist, then this method only includes the items
         that have been "flushed" to storage. Data items in the internal memory buffer
         are not counted. The buffer is empty upon calling :meth:`_flush` (internally and automatically)
         or :meth:`flush` (explicitly by user).
 
         .. versionchanged:: 0.7.4
             In previous versions, this count includes items that are not yet flushed.
         """
-        if not self._flushed:
-            warnings.warn(
-                f"did you forget to flush {self.__class__.__name__} at '{self.path}'?"
-            )
+        self._warn_flush()
         return super().__len__()
 
     def __getitem__(self, idx: int) -> Element:
         """
         Access a data item by its index; negative index works as expected.
 
         Items not yet "flushed" are not accessible by this method.
@@ -465,18 +467,15 @@
         Iterate over all the elements.
 
         Items that are not yet "flushed" are invisible to this iteration.
 
         .. versionchanged:: 0.7.4
             In previous versions, this iteration includes those items that are not yet flushed.
         """
-        if not self._flushed:
-            warnings.warn(
-                f"did you forget to flush {self.__class__.__name__} at '{self.path}'?"
-            )
+        self._warn_flush()
         return super().__iter__()
 
     def append(self, x: Element) -> None:
         """
         Append a single element to the :class:`Biglist`.
 
         In implementation, this appends to an in-memory buffer.
@@ -492,15 +491,15 @@
 
         .. note:: Use the "spawn" method to start processes.
             In ``multiprocessing``, look for the method `get_context <https://docs.python.org/3/library/multiprocessing.html#multiprocessing.get_context>`_.
             In ``concurrent.futures.ProcessPoolExecutor``, look for the parameter `mp_context <https://docs.python.org/3/library/concurrent.futures.html#concurrent.futures.ProcessPoolExecutor>`_.
             Also check out `mpservice.multiprocesing.MP_SPAWN_CTX <https://mpservice.readthedocs.io/en/latest/util.html#mpservice.multiprocessing.MP_SPAWN_CTX>`_.
         """
         self._append_buffer.append(x)
-        self._flushed = False  # This is about `flush`, not `_flush`.
+        self._flushed = False
         if len(self._append_buffer) >= self.batch_size:
             self._flush()
 
     def extend(self, x: Iterable[Element]) -> None:
         """This simply calls :meth:`append` repeatedly."""
         for v in x:
             self.append(v)
@@ -597,15 +596,15 @@
 
         After a call to ``flush()``, there's no problem to add more elements again by
         :meth:`append` or :meth:`extend`. Data files created by ``flush()`` with less than
         :data:`batch_size` elements will stay as is among larger files.
         This is a legitimate case in parallel or distributed writing, or writing in
         multiple sessions.
         """
-        if self._flushed:
+        if getattr(self, '_flushed', True):
             return
 
         self._flush(wait=True)
 
         # Other workers in other threads, processes, or machines may have appended data
         # to the list. This block merges the appends by the current worker with
         # appends by other workers. The last call to ``flush`` across all workers
@@ -638,18 +637,15 @@
         # with lock_to_use(self._info_file):
         # self.info = self._info_file.read_json()
         self.info = self._info_file.read_json()
 
     @property
     def files(self):
         # This method should be cheap to call.
-        if not self._flushed:
-            warnings.warn(
-                f"did you forget to flush {self.__class__.__name__} at '{self.path}'?"
-            )
+        self._warn_flush()
         if self._deserialize_kwargs:
             fun = functools.partial(self.load_data_file, **self._deserialize_kwargs)
         else:
             fun = self.load_data_file
         return BiglistFileSeq(
             self.path,
             [
@@ -671,15 +667,15 @@
         this many submitted and unfinished file-dumping tasks
         at any time.
     """
 
     def __init__(self, executor: ThreadPoolExecutor, n_threads: int):
         self._executor: executor = executor
         self._n_threads = n_threads
-        self._sem: Optional[threading.Semaphore] = None  # type: ignore
+        self._sem: threading.Semaphore | None = None  # type: ignore
         self._tasks: set[Future] = set()
 
     def _callback(self, t):
         self._sem.release()
         self._tasks.remove(t)
         if t.exception():
             raise t.exception()
@@ -738,15 +734,15 @@
             This must be pickle-able.
             Usually this is :meth:`Biglist.load_data_file`.
             If you customize this, please see the doc of :meth:`FileReader.__init__`.
         """
         super().__init__()
         self.path: Upath = resolve_path(path)
         self.loader = loader
-        self._data: Optional[list] = None
+        self._data: list | None = None
 
     def __getstate__(self):
         return self.path, self.loader
 
     def __setstate__(self, data):
         self.path, self.loader = data
         self._data = None
@@ -915,15 +911,15 @@
         collectively, i.e., each element is obtained by exactly one worker.
     """
 
     @classmethod
     def new(
         cls,
         data: Iterable[Any],
-        path: Optional[PathType],
+        path: PathType | None,
         *,
         batch_size: int = 10_000,
         storage_format: str = 'pickle',
     ):
         """
         Parameters
         ----------
@@ -951,16 +947,16 @@
         bl.flush()
         assert len(bl) > 0
         return cls(path)
 
     def __init__(
         self,
         path: PathType,
-        task_id: Optional[str] = None,
-        worker_id: Optional[str] = None,
+        task_id: str | None = None,
+        worker_id: str | None = None,
         timeout: int | float = 120,
     ):
         """
         Create a Multiplexer object and use it to distribute the data elements that have been
         stored by :meth:`new`.
 
         Parameters
```

### Comparing `biglist-0.8.1/src/biglist/_parquet.py` & `biglist-0.8.2b1/src/biglist/_parquet.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,16 @@
 
 import io
 import itertools
 import logging
 from collections.abc import Iterable, Iterator, Sequence
 from multiprocessing.util import Finalize
 from pathlib import Path
-from typing import Optional
 
 import pyarrow
-from deprecation import deprecated
 from pyarrow.fs import FileSystem, GcsFileSystem
 from pyarrow.parquet import FileMetaData, ParquetFile
 from upathlib import LocalUpath, PathType, Upath, resolve_path
 
 try:
     from upathlib.gcs import get_google_auth
 except ImportError:
@@ -86,14 +84,17 @@
             If ``True`` (the default), only *meta* info is loaded to construct
             a ``ParquetFile`` object.
             If ``False``, ``path.read_bytes()`` is called to read in the entire file into memory,
             and the bytes are then used to construct a ``ParquetFile`` object.
             The second route is provided to work around an issue encountered when
             ``path`` is in Google Cloud Storage.
         '''
+        # References for the issue:
+        # https://stackoverflow.com/q/76012391/6178706
+        # https://github.com/apache/arrow/issues/35318
         if lazy:
             ff, pp = FileSystem.from_uri(str(path))
             if isinstance(ff, GcsFileSystem):
                 ff = cls.get_gcsfs()
             file = ParquetFile(pp, filesystem=ff)
         else:
             data = io.BytesIO(path.read_bytes())
@@ -116,20 +117,20 @@
         # This attribute is not controlled by a parameter conveniently because
         # this may be removed later once the issue it is working around is resolved.
         # To use this, just set its value directly on the ``ParquetFileReader`` object
         # before the object has been used (hence its ``file`` may have been called).
         self._reset()
 
     def _reset(self):
-        self._file: Optional[ParquetFile] = None
-        self._data: Optional[ParquetBatchData] = None
+        self._file: ParquetFile | None = None
+        self._data: ParquetBatchData | None = None
 
         self._row_groups_num_rows = None
         self._row_groups_num_rows_cumsum = None
-        self._row_groups: Optional[list[ParquetBatchData]] = None
+        self._row_groups: None | list[ParquetBatchData] = None
 
         self._column_names = None
         self._columns = {}
         self._getitem_last_row_group = None
 
         self._scalar_as_py = None
         self.scalar_as_py = True
@@ -564,15 +565,15 @@
     by :meth:`new`.
     """
 
     @classmethod
     def new(
         cls,
         data_path: PathType | Sequence[PathType],
-        path: Optional[PathType] = None,
+        path: PathType | None = None,
         *,
         suffix: str = ".parquet",
         **kwargs,
     ) -> ParquetBiglist:
         """
         This classmethod gathers info of the specified data files and
         saves the info to facilitate reading the data files.
@@ -798,18 +799,14 @@
     if isinstance(type_spec, str):
         type_name = type_spec
         args = ()
     else:
         type_name = type_spec[0]
         args = type_spec[1:]
 
-    # print('\ntype_spec', type_spec)
-    # print('type_name', type_name)
-    # print('type_args', args)
-
     if type_name in ("string", "float64", "bool_", "int8", "int64", "uint8", "uint64"):
         assert not args
         return getattr(pyarrow, type_name)()
 
     if type_name == "list_":
         if len(args) > 2:
             raise ValueError(f"'pyarrow.list_' expects 1 or 2 args, got `{args}`")
@@ -864,15 +861,14 @@
     """
     ``filed_spec`` is a list or tuple with 2, 3, or 4 elements.
     The first element is the name of the field.
     The second element is the spec of the type, to be passed to function :func:`make_parquet_type`.
     Additional elements are the optional ``nullable`` and ``metadata`` to the function
     `pyarrow.field() <https://arrow.apache.org/docs/python/generated/pyarrow.field.html#pyarrow.field>`_.
     """
-    # print('\nfield_spec:', field_spec)
     field_name = field_spec[0]
     type_spec = field_spec[1]
     assert len(field_spec) <= 4  # two optional elements are `nullable` and `metadata`.
     return pyarrow.field(field_name, make_parquet_type(type_spec), *field_spec[3:])
 
 
 def make_parquet_schema(fields_spec: Iterable[Sequence]):
@@ -920,15 +916,15 @@
     pyarrow.parquet.write_table(table, ff.open_output_stream(pp), **kwargs)
 
 
 def write_arrays_to_parquet(
     data: Sequence[pyarrow.Array | pyarrow.ChunkedArray | Iterable],
     path: PathType,
     *,
-    names: Optional[Sequence[str]],
+    names: Sequence[str],
     **kwargs,
 ) -> None:
     """
     Parameters
     ----------
     path
         Path of the file to create and write to.
@@ -960,16 +956,7 @@
     if schema is not None:
         assert schema_spec is None
     elif schema_spec is not None:
         assert schema is None
         schema = make_parquet_schema(schema_spec)
     table = pyarrow.Table.from_pylist(data, schema=schema, metadata=metadata)
     return write_parquet_table(table, path, **kwargs)
-
-
-@deprecated(
-    deprecated_in="0.7.7",
-    removed_in="0.8.0",
-    details="Use ``write_arrays_to_parquet`` instead.",
-)
-def write_parquet_file(path, data, names, **kwargs):
-    return write_arrays_to_parquet(data, path, names=names, **kwargs)
```

### Comparing `biglist-0.8.1/src/biglist/_util.py` & `biglist-0.8.2b1/src/biglist/_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from __future__ import annotations
 
 import bisect
 import itertools
 from collections.abc import Iterator, Sequence
 from contextlib import contextmanager
-from typing import Generic, Optional, Protocol, TypeVar, runtime_checkable
+from typing import Generic, Protocol, TypeVar, runtime_checkable
 
 from upathlib import Upath
 
 
 @contextmanager
 def lock_to_use(file: Upath, timeout=120):
     f = file.with_suffix(file.suffix + ".lock")
     with f.lock(timeout=timeout):
         yield file
 
 
 def locate_idx_in_chunked_seq(
     idx: int,
     len_cumsum: Sequence[int],
-    last_chunk: Optional[tuple[int, int, int]] = None,
+    last_chunk: None | tuple[int, int, int] = None,
 ):
     """
     Suppose a sequence is composed of a number of member sequences.
     This function finds which member sequence contains the requested item.
 
     Parameters
     ----------
@@ -159,15 +159,15 @@
 
         def func(x: Slicer[list[int]]):
             ...
 
     ``Slicer`` implements the :class:`Seq` protocol.
     """
 
-    def __init__(self, list_: SeqType, range_: Optional[range | Seq[int]] = None):
+    def __init__(self, list_: SeqType, range_: None | range | Seq[int] = None):
         """
         This provides a "slice" of, or "window" into, ``list_``.
 
         The selection of elements is represented by the optional ``range_``,
         which is eithe a `range <https://docs.python.org/3/library/stdtypes.html#range>`_
         such as ``range(3, 8)``,
         or a list of indices such as ``[1, 3, 5, 6]``.
@@ -239,15 +239,15 @@
 
     @property
     def raw(self) -> SeqType:
         """Return the underlying data :class:`Seq`."""
         return self._list
 
     @property
-    def range(self) -> Optional[range | Seq[int]]:
+    def range(self) -> None | range | Seq[int]:
         """Return the parameter ``range_`` that was provided to :meth:`__init__`, representing the selection of items in the underlying Seq."""
         return self._range
 
     def collect(self) -> list:
         """
         Return a list containing the elements in the current window.
         This is equivalent to ``list(self)``.
@@ -288,17 +288,17 @@
 
     This class is in contrast with the standard `itertools.chain <https://docs.python.org/3/library/itertools.html#itertools.chain>`_,
     which takes iterables.
     """
 
     def __init__(self, list_: SeqType, *lists: SeqType):
         self._lists = (list_, *lists)
-        self._lists_len: Optional[list[int]] = None
-        self._lists_len_cumsum: Optional[list[int]] = None
-        self._len: Optional[int] = None
+        self._lists_len: None | list[int] = None
+        self._lists_len_cumsum: None | list[int] = None
+        self._len: None | int = None
 
         # Records info about the last call to `__getitem__`
         # to hopefully speed up the next call, under the assumption
         # that user tends to access consecutive or neighboring
         # elements.
         self._get_item_last_list = None
```

### Comparing `biglist-0.8.1/PKG-INFO` & `biglist-0.8.2b1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: biglist
-Version: 0.8.1
+Version: 0.8.2b1
 Summary: The package `biglist <https://github.com/zpz/biglist>`_ provides persisted, out-of-memory Python data structures
 Author-email: Zepu Zhang <zepu.zhang@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: upathlib >= 0.7.9
+Requires-Dist: upathlib >= 0.8.0
 Requires-Dist: deprecation
 Requires-Dist: mpservice >= 0.12.5
 Requires-Dist: pyarrow >= 10.0.0
 Requires-Dist: typing-extensions
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: numpydoc ; extra == "doc"
 Requires-Dist: pydata-sphinx-theme ; extra == "doc"
-Requires-Dist: upathlib[gcs] >= 0.7.9 ; extra == "gcs"
+Requires-Dist: upathlib[gcs] >= 0.8.0 ; extra == "gcs"
 Requires-Dist: google-auth ; extra == "gcs"
 Requires-Dist: lz4 ; extra == "lz4"
 Requires-Dist: boltons ; extra == "test"
 Requires-Dist: mypy ; extra == "test"
 Requires-Dist: ruff ; extra == "test"
 Requires-Dist: pytest-asyncio ; extra == "test"
 Requires-Dist: zstandard ; extra == "zstandard"
@@ -57,9 +57,8 @@
 
 Python version
 --------------
 
 Development and testing were conducted in Python 3.8 until version 0.7.8.
 Starting with 0.7.9, development and testing happen in Python 3.10.
 Code continues to NOT intentionally use features beyond Python 3.8.
-I intend to test agsint versions 3.8, 3.9, 3.10, 3.11 once I find time to set that up.
```

