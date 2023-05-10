# Comparing `tmp/xpartition-0.2.0.tar.gz` & `tmp/xpartition-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xpartition-0.2.0.tar", last modified: Wed May  5 19:23:05 2021, max compression
+gzip compressed data, was "xpartition-0.2.1.tar", last modified: Wed May 10 21:19:42 2023, max compression
```

## Comparing `xpartition-0.2.0.tar` & `xpartition-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 spencer    (501) staff       (20)        0 2021-05-05 19:23:05.000000 xpartition-0.2.0/
--rw-r--r--   0 spencer    (501) staff       (20)      238 2021-04-27 19:21:27.000000 xpartition-0.2.0/.codecov.yaml
-drwxr-xr-x   0 spencer    (501) staff       (20)        0 2021-05-05 19:23:05.000000 xpartition-0.2.0/.github/
-drwxr-xr-x   0 spencer    (501) staff       (20)        0 2021-05-05 19:23:05.000000 xpartition-0.2.0/.github/workflows/
--rw-r--r--   0 spencer    (501) staff       (20)      266 2021-04-27 19:21:27.000000 xpartition-0.2.0/.github/workflows/pre-commit.yaml
--rw-r--r--   0 spencer    (501) staff       (20)     1109 2021-04-27 19:21:27.000000 xpartition-0.2.0/.github/workflows/tests.yaml
--rw-r--r--   0 spencer    (501) staff       (20)      178 2021-04-27 19:21:27.000000 xpartition-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 spencer    (501) staff       (20)     1070 2021-01-03 16:51:22.000000 xpartition-0.2.0/LICENSE
--rw-r--r--   0 spencer    (501) staff       (20)      990 2021-05-05 19:23:05.000000 xpartition-0.2.0/PKG-INFO
--rw-r--r--   0 spencer    (501) staff       (20)     5093 2021-05-05 12:42:54.000000 xpartition-0.2.0/README.md
-drwxr-xr-x   0 spencer    (501) staff       (20)        0 2021-05-05 19:23:05.000000 xpartition-0.2.0/ci/
--rw-r--r--   0 spencer    (501) staff       (20)      159 2021-04-27 19:21:27.000000 xpartition-0.2.0/ci/environment.yaml
--rw-r--r--   0 spencer    (501) staff       (20)     1790 2021-05-05 19:23:05.000000 xpartition-0.2.0/setup.cfg
--rw-r--r--   0 spencer    (501) staff       (20)      103 2021-01-03 16:51:44.000000 xpartition-0.2.0/setup.py
--rw-r--r--   0 spencer    (501) staff       (20)     8496 2021-05-05 16:08:25.000000 xpartition-0.2.0/test_xpartition.py
--rw-r--r--   0 spencer    (501) staff       (20)      459 2021-04-13 12:13:27.000000 xpartition-0.2.0/tox.ini
-drwxr-xr-x   0 spencer    (501) staff       (20)        0 2021-05-05 19:23:05.000000 xpartition-0.2.0/xpartition.egg-info/
--rw-r--r--   0 spencer    (501) staff       (20)      990 2021-05-05 19:23:05.000000 xpartition-0.2.0/xpartition.egg-info/PKG-INFO
--rw-r--r--   0 spencer    (501) staff       (20)      400 2021-05-05 19:23:05.000000 xpartition-0.2.0/xpartition.egg-info/SOURCES.txt
--rw-r--r--   0 spencer    (501) staff       (20)        1 2021-05-05 19:23:05.000000 xpartition-0.2.0/xpartition.egg-info/dependency_links.txt
--rw-r--r--   0 spencer    (501) staff       (20)        1 2021-05-05 19:23:05.000000 xpartition-0.2.0/xpartition.egg-info/not-zip-safe
--rw-r--r--   0 spencer    (501) staff       (20)       96 2021-05-05 19:23:05.000000 xpartition-0.2.0/xpartition.egg-info/requires.txt
--rw-r--r--   0 spencer    (501) staff       (20)       11 2021-05-05 19:23:05.000000 xpartition-0.2.0/xpartition.egg-info/top_level.txt
--rw-r--r--   0 spencer    (501) staff       (20)    15093 2021-05-05 19:20:16.000000 xpartition-0.2.0/xpartition.py
+drwxr-xr-x   0 spencer    (501) staff       (20)        0 2023-05-10 21:19:42.871131 xpartition-0.2.1/
+-rw-r--r--   0 spencer    (501) staff       (20)      238 2021-04-27 19:21:27.000000 xpartition-0.2.1/.codecov.yaml
+drwxr-xr-x   0 spencer    (501) staff       (20)        0 2023-05-10 21:19:42.861806 xpartition-0.2.1/.github/
+drwxr-xr-x   0 spencer    (501) staff       (20)        0 2023-05-10 21:19:42.867414 xpartition-0.2.1/.github/workflows/
+-rw-r--r--   0 spencer    (501) staff       (20)      260 2023-05-08 15:44:46.000000 xpartition-0.2.1/.github/workflows/pre-commit.yaml
+-rw-r--r--   0 spencer    (501) staff       (20)     1109 2021-04-27 19:21:27.000000 xpartition-0.2.1/.github/workflows/tests.yaml
+-rw-r--r--   0 spencer    (501) staff       (20)      182 2023-05-08 15:44:46.000000 xpartition-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 spencer    (501) staff       (20)     1070 2021-01-03 16:51:22.000000 xpartition-0.2.1/LICENSE
+-rw-r--r--   0 spencer    (501) staff       (20)      950 2023-05-10 21:19:42.871330 xpartition-0.2.1/PKG-INFO
+-rw-r--r--   0 spencer    (501) staff       (20)     5402 2023-05-08 15:44:46.000000 xpartition-0.2.1/README.md
+drwxr-xr-x   0 spencer    (501) staff       (20)        0 2023-05-10 21:19:42.867885 xpartition-0.2.1/ci/
+-rw-r--r--   0 spencer    (501) staff       (20)      159 2021-04-27 19:21:27.000000 xpartition-0.2.1/ci/environment.yaml
+-rw-r--r--   0 spencer    (501) staff       (20)     1790 2023-05-10 21:19:42.872034 xpartition-0.2.1/setup.cfg
+-rw-r--r--   0 spencer    (501) staff       (20)      103 2021-01-03 16:51:44.000000 xpartition-0.2.1/setup.py
+-rw-r--r--   0 spencer    (501) staff       (20)    13181 2023-05-10 20:45:51.000000 xpartition-0.2.1/test_xpartition.py
+-rw-r--r--   0 spencer    (501) staff       (20)      459 2021-04-13 12:13:27.000000 xpartition-0.2.1/tox.ini
+drwxr-xr-x   0 spencer    (501) staff       (20)        0 2023-05-10 21:19:42.870842 xpartition-0.2.1/xpartition.egg-info/
+-rw-r--r--   0 spencer    (501) staff       (20)      950 2023-05-10 21:19:42.000000 xpartition-0.2.1/xpartition.egg-info/PKG-INFO
+-rw-r--r--   0 spencer    (501) staff       (20)      400 2023-05-10 21:19:42.000000 xpartition-0.2.1/xpartition.egg-info/SOURCES.txt
+-rw-r--r--   0 spencer    (501) staff       (20)        1 2023-05-10 21:19:42.000000 xpartition-0.2.1/xpartition.egg-info/dependency_links.txt
+-rw-r--r--   0 spencer    (501) staff       (20)        1 2021-05-05 19:23:05.000000 xpartition-0.2.1/xpartition.egg-info/not-zip-safe
+-rw-r--r--   0 spencer    (501) staff       (20)       96 2023-05-10 21:19:42.000000 xpartition-0.2.1/xpartition.egg-info/requires.txt
+-rw-r--r--   0 spencer    (501) staff       (20)       11 2023-05-10 21:19:42.000000 xpartition-0.2.1/xpartition.egg-info/top_level.txt
+-rw-r--r--   0 spencer    (501) staff       (20)    20097 2023-05-10 21:12:55.000000 xpartition-0.2.1/xpartition.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `xpartition-0.2.0/.github/workflows/tests.yaml` & `xpartition-0.2.1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `xpartition-0.2.0/LICENSE` & `xpartition-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xpartition-0.2.0/PKG-INFO` & `xpartition-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: xpartition
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tool for writing large xarray datasets to zarr stores with independent processes
 Home-page: https://github.com/spencerkclark/xpartition
 Author: Spencer K. Clark
 Author-email: spencerkclark@gmail.com
 License: MIT License
-Description: 
-        xpartition provides a way to split N-dimensional dask-backed arrays into
-        a user-specified number of blocks of dask chunks.  This can be useful for
-        assigning work to batch jobs on HPC systems or Dataflow workers in an
-        Apache Beam pipeline in the cloud.
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/plain
+License-File: LICENSE
+
+
+xpartition provides a way to split N-dimensional dask-backed arrays into
+a user-specified number of blocks of dask chunks.  This can be useful for
+assigning work to batch jobs on HPC systems or Dataflow workers in an
+Apache Beam pipeline in the cloud.
```

### Comparing `xpartition-0.2.0/README.md` & `xpartition-0.2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -32,28 +32,37 @@
 
 ```python
 import argparse
 import xpartition
 
 from external import construct_lazy_dataset
 
+parser = argparse.ArgumentParser(
+    prog="initialize_store",
+    description="initialize a zarr store for a dataset"
+)
 parser.add_argument("store", help="absolute path to directory to store zarr result")
+
+args = parser.parse_args()
 ds = construct_lazy_dataset()
 ds.partition.initialize_store(args.store)
 ```
 
 Next we'll write one called `write_partition.py`:
 
 ```python
 import argparse
 import xpartition
 
 from external import construct_lazy_dataset
 
-
+parser = argparse.ArgumentParser(
+    prog="write_partition",
+    description="write a partition of a dataset"
+)
 parser.add_argument("store", help="absolute path to directory to store zarr result")
 parser.add_argument("ranks", type=int, help="total number of available ranks")
 parser.add_argument("rank", type=int, help="rank of job")
 
 args = parser.parse_args()
 
 # xpartition uses these as the dimensions to partition the jobs over.
@@ -113,21 +122,21 @@
 ```
 
 ## Motivation
 
 It is not always advantageous to let all computations be controlled by a single
 dask client.  At the moment, the dask scheduler breaks down when having to
 manage a large number of memory-intensive tasks, often leading to slowdowns or
-out of memory errors (see [this
-issue](https://github.com/dask/distributed/issues/2602) for more discussion).
-Breaking the problem down in the way that `xpartition` does, allows you to gain
-the benefits of dask's laziness on each independent process, while working in a
-distributed environment.  *In an ideal world we wouldn't need a package like
-this -- we would let dask and dask distributed handle everything -- but in
-practice that does not work perfectly yet.*
+out of memory errors ([this issue](https://github.com/dask/distributed/issues/6360) 
+is perhaps a good summary of the state of things currently in dask). Breaking the 
+problem down in the way that `xpartition` does, allows you to gain the benefits of
+dask's laziness on each independent process, while working in a distributed 
+environment.  *In an ideal world we wouldn't need a package like this -- we would 
+let dask and dask distributed handle everything -- but in practice that does not 
+work perfectly yet.*
 
 ## Installation
 
 `xpartition` can either be installed from PyPI:
 
 ```
 $ pip install xpartition
```

### Comparing `xpartition-0.2.0/setup.cfg` & `xpartition-0.2.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.0
+current_version = 0.2.1
 commit = True
 tag = True
 
 [metadata]
 name = xpartition
 version = attr: xpartition.__version__
 author = Spencer K. Clark
```

### Comparing `xpartition-0.2.0/test_xpartition.py` & `xpartition-0.2.1/test_xpartition.py`

 * *Files 25% similar despite different names*

```diff
@@ -96,18 +96,23 @@
     name = "foo"
     return _construct_dataarray(shape, chunks, name)
 
 
 def _construct_dataarray(shape, chunks, name):
     dims = list(string.ascii_lowercase[: len(shape)])
     data = np.random.random(shape)
-    da = xr.DataArray(data, dims=dims, name=name)
+    coords = [range(length) for length in shape]
+    da = xr.DataArray(data, dims=dims, name=name, coords=coords)
     if chunks is not None:
         chunks = {dim: chunk for dim, chunk in zip(dims, chunks)}
         da = da.chunk(chunks)
+
+        # Add coverage for chunked coordinates
+        chunked_coord_name = f"{da.name}_chunked_coord"
+        da = da.assign_coords({chunked_coord_name: da.chunk(chunks)})
     return da
 
 
 ALIGNED_SHAPE_AND_CHUNK_PAIRS = [
     ((5,), (1,)),
     ((5,), (2,)),
     ((5,), (5,)),
@@ -134,26 +139,75 @@
     for i, (shape, chunks) in enumerate(ALIGNED_SHAPE_AND_CHUNK_PAIRS):
         da = _construct_dataarray(shape, chunks, f"chunked_{i}")
         chunked_dataarrays.append(da)
 
     return xr.merge(unchunked_dataarrays + chunked_dataarrays)
 
 
+def get_files(directory):
+    names = os.listdir(directory)
+    files = []
+    for name in names:
+        path = os.path.join(directory, name)
+        if os.path.isfile(path):
+            files.append(path)
+    return files
+
+
+def get_unchunked_variable_names(ds):
+    names = []
+    for name, variable in ds.variables.items():
+        if not isinstance(variable.data, dask.array.Array):
+            names.append(name)
+    return names
+
+
+def checkpoint_modification_times(store, variables):
+    times = {}
+    for variable in variables:
+        directory = os.path.join(store, variable)
+        files = get_files(directory)
+        for file in files:
+            times[file] = os.path.getmtime(file)
+    return times
+
+
 @pytest.mark.filterwarnings("ignore:Specified Dask chunks")
 @pytest.mark.parametrize("ranks", [1, 2, 3, 5, 10, 11])
-def test_dataset_mappable_write(tmpdir, ds, ranks):
+@pytest.mark.parametrize("collect_variable_writes", [False, True])
+def test_dataset_mappable_write(tmpdir, ds, ranks, collect_variable_writes):
+    unchunked_variables = get_unchunked_variable_names(ds)
+
     store = os.path.join(tmpdir, "test.zarr")
     ds.partition.initialize_store(store)
 
+    # Checkpoint modification times of all files associated with unchunked
+    # variables.  These should remain unchanged after initialization.
+    expected_times = checkpoint_modification_times(store, unchunked_variables)
+
     with multiprocessing.get_context("spawn").Pool(ranks) as pool:
-        pool.map(ds.partition.mappable_write(store, ranks, ds.dims), range(ranks))
+        pool.map(
+            ds.partition.mappable_write(
+                store, ranks, ds.dims, collect_variable_writes=collect_variable_writes
+            ),
+            range(ranks),
+        )
 
     result = xr.open_zarr(store)
+
+    # Check that dataset roundtrips identically.
     xr.testing.assert_identical(result, ds)
 
+    # Checkpoint modification times of all files associated with unchunked
+    # variables after writing the chunked variables.  The modification times of
+    # the unchunked variables should be the same as before writing the chunked
+    # variables.
+    resulting_times = checkpoint_modification_times(store, unchunked_variables)
+    assert expected_times == resulting_times
+
 
 @pytest.mark.parametrize("has_coord", [True, False])
 @pytest.mark.parametrize(
     "original_chunks", [{"x": 2}, {"x": 2, "y": 5}], ids=lambda x: f"{x}"
 )
 def test_PartitionMapper_integration(tmpdir, has_coord, original_chunks):
     def func(ds):
@@ -253,7 +307,92 @@
 
 
 def test_partition_indexers_invalid_rank_error():
     data = dask.array.zeros((6, 4), chunks=((6, 4)))
     da = xr.DataArray(data, dims=["x", "y"])
     with pytest.raises(ValueError, match="greater than maximum rank"):
         da.partition.indexers(1, 1, ["x"])
+
+
+@pytest.mark.parametrize(
+    ("unfrozen_indexers", "frozen_indexers"),
+    [
+        (
+            {"a": slice(None, None, 3), "b": slice(1, 10, 2)},
+            (("a", (None, None, 3)), ("b", (1, 10, 2))),
+        ),
+        (None, None),
+    ],
+    ids=lambda x: f"{x}",
+)
+def test_freeze_unfreeze_indexers(unfrozen_indexers, frozen_indexers):
+    assert xpartition.freeze_indexers(unfrozen_indexers) == frozen_indexers
+    assert xpartition.unfreeze_indexers(frozen_indexers) == unfrozen_indexers
+
+
+@pytest.mark.parametrize(
+    ("a", "b"),
+    [
+        (
+            {"a": slice(None, None, 3), "b": slice(1, 10, 2)},
+            {"b": slice(1, 10, 2), "a": slice(None, None, 3)},
+        ),
+        (None, None),
+    ],
+    ids=lambda x: f"{x}",
+)
+def test_hashability_of_frozen_indexers(a, b):
+    assert a == b
+    frozen_indexers_a = xpartition.freeze_indexers(a)
+    frozen_indexers_b = xpartition.freeze_indexers(b)
+
+    # Despite having different key orders, the hashes of the frozen indexers
+    # should be equal.
+    assert hash(frozen_indexers_a) == hash(frozen_indexers_b)
+
+
+class CountingScheduler:
+    """Inspired by xarray
+
+    https://github.com/pydata/xarray/blob/33fbb648ac042f821a11870ffa544e5bcb6e178f/xarray/tests/__init__.py#L97-L113
+    """
+
+    def __init__(self):
+        self.total_computes = 0
+
+    def __call__(self, dsk, keys, **kwargs):
+        self.total_computes += 1
+        return dask.get(dsk, keys, **kwargs)
+
+
+@pytest.mark.parametrize(
+    ("collect_variable_writes", "expected_computes"), [(False, 9), (True, 3)]
+)
+def test_dataset_mappable_write_minimizes_compute_calls(
+    tmpdir, collect_variable_writes, expected_computes
+):
+    # This tests to ensure that calls to compute are minimized when writing
+    # partitioned Datasets.  Previously, a compute was called separately for
+    # each variable in the Dataset.  For fields that have common intermediates --
+    # e.g. loading a particular variable from somewhere -- this is inefficient,
+    # because it means these intermediates must be computed multiple times.  If
+    # the option to collect_variable_writes is turned, however, we expect more
+    # computes to be called (one for each partition and data variable in the
+    # Dataset).
+    store = os.path.join(tmpdir, "test.zarr")
+
+    foo = _construct_dataarray((2, 9), (2, 3), "foo")
+    bar = (2 * foo).rename("bar")
+    ds = xr.merge([foo, bar])
+
+    ds.partition.initialize_store(store)
+    scheduler = CountingScheduler()
+
+    with dask.config.set(scheduler=scheduler):
+        ranks = 3
+        for rank in range(ranks):
+            ds.partition.write(store, ranks, ds.dims, rank, collect_variable_writes)
+
+        assert scheduler.total_computes == expected_computes
+
+    result = xr.open_zarr(store)
+    xr.testing.assert_identical(result, ds)
```

### Comparing `xpartition-0.2.0/xpartition.egg-info/PKG-INFO` & `xpartition-0.2.1/xpartition.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: xpartition
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tool for writing large xarray datasets to zarr stores with independent processes
 Home-page: https://github.com/spencerkclark/xpartition
 Author: Spencer K. Clark
 Author-email: spencerkclark@gmail.com
 License: MIT License
-Description: 
-        xpartition provides a way to split N-dimensional dask-backed arrays into
-        a user-specified number of blocks of dask chunks.  This can be useful for
-        assigning work to batch jobs on HPC systems or Dataflow workers in an
-        Apache Beam pipeline in the cloud.
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/plain
+License-File: LICENSE
+
+
+xpartition provides a way to split N-dimensional dask-backed arrays into
+a user-specified number of blocks of dask chunks.  This can be useful for
+assigning work to batch jobs on HPC systems or Dataflow workers in an
+Apache Beam pipeline in the cloud.
```

### Comparing `xpartition-0.2.0/xpartition.py` & `xpartition-0.2.1/xpartition.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,27 @@
+import collections
 import functools
 import math
 
 import dask.array
 import numpy as np
 import xarray as xr
 import dataclasses
 import logging
 
-from typing import Callable, Dict, Hashable, Sequence, Tuple, Mapping
+from typing import Callable, Dict, Hashable, Mapping, Sequence, Tuple, Union
 
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 
-Region = Sequence[Mapping[Hashable, slice]]
+Region = Union[None, Mapping[Hashable, slice]]
 Partition = Sequence[Region]
+HashableSlice = Tuple[Union[None, int], Union[None, int], Union[None, int]]
+HashableIndexers = Union[None, Tuple[Tuple[Hashable, HashableSlice], ...]]
 
 
 def _is_integer(value):
     """Check if a value is a Python or NumPy integer instance."""
     return isinstance(value, (int, np.integer))
 
 
@@ -177,27 +180,68 @@
         # TODO: should we squeeze out dimensions where scalars were passed?
         return self._obj.isel(slices)
 
 
 def _write_partition_dataarray(
     da: xr.DataArray, store: str, ranks: int, dims: Sequence[Hashable], rank: int
 ):
-    ds = da.to_dataset()
+    ds = da.drop_vars(da.coords).to_dataset()
     partition = da.partition.indexers(ranks, rank, dims)
     if partition is not None:
         ds.isel(partition).to_zarr(store, region=partition)
 
 
-def _write_partition_dataset(
+def freeze_indexers(indexers: Region) -> HashableIndexers:
+    """Return an immutable (hashable) version of the indexers."""
+    if indexers is None:
+        return indexers
+    else:
+        immutable = ((k, (s.start, s.stop, s.step)) for k, s in indexers.items())
+        return tuple(sorted(immutable, key=lambda x: x[0]))
+
+
+def unfreeze_indexers(frozen_indexers: HashableIndexers) -> Region:
+    """Convert an immutable version of the indexers back to its usual type."""
+    if frozen_indexers is None:
+        return frozen_indexers
+    else:
+        return {k: slice(*s) for k, s in frozen_indexers}
+
+
+def _collect_by_partition(
+    ds: xr.Dataset, ranks: int, dims: Sequence[Hashable], rank: int
+) -> Sequence[Tuple[Region, xr.Dataset]]:
+    """Return a list of pairs of partitions and Datasets containing
+    DataArrays that can be written out to those partitions.
+    """
+    dataarrays = collections.defaultdict(list)
+    for da in {**ds.coords, **ds.data_vars}.values():
+        if isinstance(da.data, dask.array.Array):
+            partition_dims = [dim for dim in dims if dim in da.dims]
+            indexers = da.partition.indexers(ranks, rank, partition_dims)
+            dataarrays[freeze_indexers(indexers)].append(da.drop_vars(da.coords))
+    return [(unfreeze_indexers(k), xr.merge(v)) for k, v in dataarrays.items()]
+
+
+def _write_partition_dataset_via_individual_variables(
     ds: xr.Dataset, store: str, ranks: int, dims: Sequence[Hashable], rank: int
 ):
-    for da in ds.data_vars.values():
+    for da in {**ds.coords, **ds.data_vars}.values():
         if isinstance(da.data, dask.array.Array):
             partition_dims = [dim for dim in dims if dim in da.dims]
-            da.partition.write(store, ranks, partition_dims, rank)
+            _write_partition_dataarray(da, store, ranks, partition_dims, rank)
+
+
+def _write_partition_dataset_via_collected_variables(
+    ds: xr.Dataset, store: str, ranks: int, dims: Sequence[Hashable], rank: int
+):
+    collected_by_partition = _collect_by_partition(ds, ranks, dims, rank)
+    for partition, d in collected_by_partition:
+        if partition is not None:
+            d.isel(partition).to_zarr(store, region=partition)
 
 
 class Map(Sequence):
     """Lazy sequence"""
 
     def __init__(self, func, seq):
         self.seq = seq
@@ -305,22 +349,35 @@
         except ValueError:
             return None
         else:
             meta_indexers = dict(zip(meta_array.dims, meta_indices))
             dask_indexers = meta_array.blocks.indexers(**meta_indexers)
             return self._obj.blocks.indexers(**dask_indexers)
 
-    def write(self, store: str, ranks: int, dims: Sequence[Hashable], rank: int):
-        _write_partition_dataarray(self._obj, store, ranks, dims, rank)
+    def write(
+        self,
+        store: str,
+        ranks: int,
+        dims: Sequence[Hashable],
+        rank: int,
+        collect_variable_writes: bool = False,
+    ):
+        self.to_dataset().partition.write(
+            store, ranks, dims, rank, collect_variable_writes
+        )
 
     def mappable_write(
-        self, store: str, ranks: int, dims: Sequence[Hashable]
+        self,
+        store: str,
+        ranks: int,
+        dims: Sequence[Hashable],
+        collect_variable_writes: bool = False,
     ) -> Callable[[int], None]:
-        return functools.partial(
-            _write_partition_dataarray, self._obj, store, ranks, dims
+        return self._obj.to_dataset().partition.mappable_write(
+            store, ranks, dims, collect_variable_writes
         )
 
     @property
     def _chunks(self):
         return {dim: self._obj.chunks[k] for k, dim in enumerate(self._obj.dims)}
 
     def map(
@@ -334,23 +391,90 @@
 class PartitionDatasetAccessor:
     def __init__(self, xarray_obj):
         self._obj = xarray_obj
 
     def initialize_store(self, store: str):
         self._obj.to_zarr(store, compute=False)
 
-    def write(self, store: str, ranks: int, dims: Sequence[Hashable], rank: int):
-        _write_partition_dataset(self._obj, store, ranks, dims, rank)
+    def write(
+        self,
+        store: str,
+        ranks: int,
+        dims: Sequence[Hashable],
+        rank: int,
+        collect_variable_writes: bool = False,
+    ):
+        """Write a Dataset partition to disk on a given rank.
+
+        Parameters
+        ----------
+        store : str
+            Path to zarr store.
+        ranks : int
+            Total number of ranks available to partition across.
+        dims : Sequence[Hashable]
+            Dimensions to partition among; if a dimension is left out
+            no partitions will be made along that dimension.
+        rank : int
+            Rank of process to write partition from.
+        collect_variable_writes : bool
+            Whether to collect data variables with like partition indexers
+            together when writing data out to disk (default False).  It can
+            be beneficial to set this to True if data variables in the Dataset
+            have like chunk structure, and also share intermediate data.  An
+            example of this would be two fields that derive from the same
+            input data.  By default this input data would need be computed or
+            loaded twice; with this option set to True, it the input data would
+            only need to be computed or loaded once.  A caveat, however, is that
+            it can increase memory usage.
+        """
+        if collect_variable_writes:
+            f = _write_partition_dataset_via_collected_variables
+        else:
+            f = _write_partition_dataset_via_individual_variables
+        f(self._obj, store, ranks, dims, rank)
 
     def mappable_write(
-        self, store: str, ranks: int, dims: Sequence[Hashable]
+        self,
+        store: str,
+        ranks: int,
+        dims: Sequence[Hashable],
+        collect_variable_writes: bool = False,
     ) -> Callable[[int], None]:
-        return functools.partial(
-            _write_partition_dataset, self._obj, store, ranks, dims
-        )
+        """Return a function that can write data for a partition on a rank.
+
+        Parameters
+        ----------
+        store : str
+            Path to zarr store.
+        ranks : int
+            Total number of ranks available to partition across.
+        dims : Sequence[Hashable]
+            Dimensions to partition among; if a dimension is left out
+            no partitions will be made along that dimension.
+        collect_variable_writes : bool
+            Whether to collect data variables with like partition indexers
+            together when writing data out to disk (default False).  It can
+            be beneficial to set this to True if data variables in the Dataset
+            have like chunk structure, and also share intermediate data.  An
+            example of this would be two fields that derive from the same
+            input data.  By default this input data would need be computed or
+            loaded twice; with this option set to True, it the input data would
+            only need to be computed or loaded once.  A caveat, however, is that
+            it can increase memory usage.
+
+        Returns
+        -------
+        function
+        """
+        if collect_variable_writes:
+            f = _write_partition_dataset_via_collected_variables
+        else:
+            f = _write_partition_dataset_via_individual_variables
+        return functools.partial(f, self._obj, store, ranks, dims)
 
 
 def _merge_chunks(arr, override_chunks):
     chunks_to_update = {}
     for dim, sizes in override_chunks.items():
         if dim in arr.dims:
             axis = arr.get_axis_num(dim)
@@ -395,15 +519,14 @@
 
 class _ValidWorkPlan:
     """A mapping between input and output partitionings that will
     avoid race conditions in parallel jobs
     """
 
     def __init__(self, partitioner, ranks: int, dims: Sequence[Hashable]):
-
         self._partitioner = partitioner
         self._ranks = ranks
         self.dims = dims
 
     @property
     def output_chunks(self):
         return {dim: self._partitioner._chunks[dim] for dim in self.dims}
```

