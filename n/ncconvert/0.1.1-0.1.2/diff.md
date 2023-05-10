# Comparing `tmp/ncconvert-0.1.1.tar.gz` & `tmp/ncconvert-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncconvert-0.1.1.tar", last modified: Thu May  4 18:57:12 2023, max compression
+gzip compressed data, was "ncconvert-0.1.2.tar", last modified: Tue May  9 23:57:43 2023, max compression
```

## Comparing `ncconvert-0.1.1.tar` & `ncconvert-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:57:12.199913 ncconvert-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-04 18:57:00.000000 ncconvert-0.1.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:57:12.195913 ncconvert-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:57:12.199913 ncconvert-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-04 18:57:00.000000 ncconvert-0.1.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-04 18:57:00.000000 ncconvert-0.1.1/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-04 18:57:00.000000 ncconvert-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-04 18:57:00.000000 ncconvert-0.1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-04 18:57:12.199913 ncconvert-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-04 18:57:00.000000 ncconvert-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-04 18:57:00.000000 ncconvert-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 18:57:12.199913 ncconvert-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-04 18:57:00.000000 ncconvert-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:57:12.199913 ncconvert-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:57:12.199913 ncconvert-0.1.1/src/ncconvert/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-04 18:57:00.000000 ncconvert-0.1.1/src/ncconvert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-04 18:57:00.000000 ncconvert-0.1.1/src/ncconvert/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 18:57:12.000000 ncconvert-0.1.1/src/ncconvert/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-04 18:57:00.000000 ncconvert-0.1.1/src/ncconvert/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-04 18:57:00.000000 ncconvert-0.1.1/src/ncconvert/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-04 18:57:00.000000 ncconvert-0.1.1/src/ncconvert/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:57:00.000000 ncconvert-0.1.1/src/ncconvert/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-04 18:57:00.000000 ncconvert-0.1.1/src/ncconvert/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:57:12.199913 ncconvert-0.1.1/src/ncconvert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-04 18:57:12.000000 ncconvert-0.1.1/src/ncconvert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-04 18:57:12.000000 ncconvert-0.1.1/src/ncconvert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 18:57:12.000000 ncconvert-0.1.1/src/ncconvert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-04 18:57:12.000000 ncconvert-0.1.1/src/ncconvert.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-04 18:57:12.000000 ncconvert-0.1.1/src/ncconvert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 18:57:12.000000 ncconvert-0.1.1/src/ncconvert.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:57:12.199913 ncconvert-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-04 18:57:00.000000 ncconvert-0.1.1/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-04 18:57:00.000000 ncconvert-0.1.1/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-04 18:57:00.000000 ncconvert-0.1.1/test/test_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-05-04 18:57:00.000000 ncconvert-0.1.1/test/test_parquet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:57:43.839316 ncconvert-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-09 23:57:31.000000 ncconvert-0.1.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:57:43.831315 ncconvert-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:57:43.835315 ncconvert-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-09 23:57:31.000000 ncconvert-0.1.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-09 23:57:31.000000 ncconvert-0.1.2/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-09 23:57:31.000000 ncconvert-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-09 23:57:31.000000 ncconvert-0.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-09 23:57:31.000000 ncconvert-0.1.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-09 23:57:43.839316 ncconvert-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-09 23:57:31.000000 ncconvert-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-09 23:57:31.000000 ncconvert-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 23:57:43.839316 ncconvert-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-09 23:57:31.000000 ncconvert-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:57:43.831315 ncconvert-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:57:43.835315 ncconvert-0.1.2/src/ncconvert/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-09 23:57:31.000000 ncconvert-0.1.2/src/ncconvert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-09 23:57:31.000000 ncconvert-0.1.2/src/ncconvert/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-09 23:57:43.000000 ncconvert-0.1.2/src/ncconvert/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-09 23:57:31.000000 ncconvert-0.1.2/src/ncconvert/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-09 23:57:31.000000 ncconvert-0.1.2/src/ncconvert/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-09 23:57:31.000000 ncconvert-0.1.2/src/ncconvert/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 23:57:31.000000 ncconvert-0.1.2/src/ncconvert/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-09 23:57:31.000000 ncconvert-0.1.2/src/ncconvert/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:57:43.839316 ncconvert-0.1.2/src/ncconvert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-09 23:57:43.000000 ncconvert-0.1.2/src/ncconvert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-09 23:57:43.000000 ncconvert-0.1.2/src/ncconvert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 23:57:43.000000 ncconvert-0.1.2/src/ncconvert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-09 23:57:43.000000 ncconvert-0.1.2/src/ncconvert.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-09 23:57:43.000000 ncconvert-0.1.2/src/ncconvert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 23:57:43.000000 ncconvert-0.1.2/src/ncconvert.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:57:43.839316 ncconvert-0.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-09 23:57:31.000000 ncconvert-0.1.2/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-09 23:57:31.000000 ncconvert-0.1.2/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-09 23:57:31.000000 ncconvert-0.1.2/test/test_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-05-09 23:57:31.000000 ncconvert-0.1.2/test/test_parquet.py
```

### Comparing `ncconvert-0.1.1/.github/workflows/pypi.yml` & `ncconvert-0.1.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `ncconvert-0.1.1/.github/workflows/pytest.yml` & `ncconvert-0.1.2/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `ncconvert-0.1.1/README.md` & `ncconvert-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ncconvert-0.1.1/pyproject.toml` & `ncconvert-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 authors = [
   { name="tsdat", email="tsdat@pnnl.gov" },
 ]
 description = "Convert netCDF to other formats."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["netCDF", "cdf", "nc"]
-license = {text = "BSD 3-Clause License"}
+license = {file = "LICENSE.md"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
   "xarray[io]",
   "pandas[hdf5, parquet, feather, spss, excel]",
 ]
@@ -28,15 +28,15 @@
   "build",
   "black",
   "ruff",
   "isort",
 ]
 
 cli = [
-  "typer",
+  "typer>=0.9.0",
   "tqdm",
   "rich",
 ]
 
 [project.scripts]
 ncconvert = "ncconvert.cli:app"
```

### Comparing `ncconvert-0.1.1/src/ncconvert/cli.py` & `ncconvert-0.1.2/src/ncconvert/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from __future__ import annotations
-
 import logging
 import re
 import sys
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Protocol, Tuple, Union
 
 import xarray as xr
+from typing_extensions import Annotated
 
 try:
     import tqdm
     import typer
 except ImportError:
     logging.exception("")
     print(
@@ -21,25 +20,28 @@
         "Aborting..."
     )
     sys.exit(1)
 
 from .csv import to_csv, to_csv_collection
 from .parquet import to_parquet, to_parquet_collection
 
-ConvertMethod = Callable[
-    [
-        xr.Dataset,
-        Union[str, Path],
-        Optional[Dict[str, Any]],
-    ],
-    Tuple[Union[Tuple[Path, ...], Path], Path],
-]
+
+class Converter(Protocol):
+    def __call__(
+        self,
+        dataset: xr.Dataset,
+        filepath: Union[Path, str],
+        metadata: bool = False,
+        **kwargs: Optional[Any],
+    ) -> Tuple[Union[Tuple[Path, ...], Path], Optional[Path]]:
+        ...
+
 
 # Register to_* methods as options. For now this is a manual process
-AVAILABLE_METHODS: dict[str, ConvertMethod] = {
+AVAILABLE_METHODS: Dict[str, Converter] = {
     to_csv.__name__: to_csv,
     to_csv_collection.__name__: to_csv_collection,
     to_parquet.__name__: to_parquet,
     to_parquet_collection.__name__: to_parquet_collection,
 }
 _available_methods = list(AVAILABLE_METHODS)
 
@@ -63,44 +65,62 @@
 
 
 app = typer.Typer(no_args_is_help=True)
 
 
 @app.command(no_args_is_help=True)
 def ncconvert(
-    method: str = typer.Argument(
-        ...,
-        help=f"How to convert the netCDF file(s). Options are: {_available_methods}",
-    ),
-    files: List[Path] = typer.Argument(
-        ...,
-        resolve_path=True,
-        dir_okay=False,
-        callback=_expand_paths,
-        help="The path to the netCDF files to convert.",
-    ),
-    output_dir: Path = typer.Option(
-        Path("./data"),
-        dir_okay=True,
-        file_okay=False,
-        help="The output dir where the converted file(s) should be saved.",
-    ),
-    verbose: bool = typer.Option(False, help="Run in verbose mode."),
+    method: Annotated[
+        str,
+        typer.Argument(
+            help=f"How to convert the netCDF file(s). Options are: {_available_methods}",
+        ),
+    ],
+    files: Annotated[
+        List[Path],
+        typer.Argument(
+            ...,
+            resolve_path=True,
+            dir_okay=False,
+            callback=_expand_paths,
+            help="The path to the netCDF files to convert.",
+        ),
+    ],
+    output_dir: Annotated[
+        Path,
+        typer.Option(
+            dir_okay=True,
+            file_okay=False,
+            help="The output dir where the converted file(s) should be saved.",
+        ),
+    ] = Path("./data"),
+    metadata: Annotated[
+        bool,
+        typer.Option(help="Write dataset metadata to a .json file"),
+    ] = True,
+    verbose: Annotated[
+        bool,
+        typer.Option(help="Run in verbose mode."),
+    ] = False,
 ):
     """Convert netCDF files to another format."""
-    
     convert_function = AVAILABLE_METHODS[method]
 
     file_iterator = tqdm.tqdm(files) if verbose else files
 
     for file in file_iterator:
         ds = xr.open_dataset(file)
         output_filepath = output_dir / file.name
-        output_data_files, metadata_file = convert_function(ds, output_filepath, None)
-        if verbose:
+        output_data_files, metadata_file = convert_function(
+            dataset=ds,
+            filepath=output_filepath,
+            metadata=metadata,
+        )
+        if verbose and output_data_files:
             typer.echo(f"Wrote data to {output_data_files}")
+        if verbose and metadata:
             typer.echo(f"Wrote metadata to {metadata_file}")
 
     if verbose:
         typer.echo("Done!")
 
     return
```

### Comparing `ncconvert-0.1.1/src/ncconvert/csv.py` & `ncconvert-0.1.2/src/ncconvert/csv.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,59 @@
 from __future__ import annotations
 
 from pathlib import Path
-from typing import Any, Dict
+from typing import Any
 
 import xarray as xr
 
 from .utils import _dump_metadata, _to_dataframe, _to_dataframe_collection
 
 
 def to_csv(
     dataset: xr.Dataset,
     filepath: str | Path,
-    to_csv_kwargs: Dict[str, Any] | None = None,
-) -> tuple[Path, Path]:
+    metadata: bool = True,
+    **kwargs: Any,
+) -> tuple[Path, Path | None]:
     """Writes an xarray dataset to a csv file using basic settings.
 
     The output file will be indexed by the cartesian product of the dataset's indexes
     (coordinate variables).
 
     Args:
         dataset (xr.Dataset): The dataset to write.
         filepath (str | Path): Where to write the file. This should be the path to a
             file, not the path to a folder. This should include the file extension.
+        metadata (bool): If True, metadata from the xr.Dataset will be written to a
+            .json file next to the output file. Defaults to True.
         to_csv_kwargs (Dict[str, Any] | None, optional): Extra arguments to provide to
             pandas.DataFrame.to_csv() as keyword arguments. Defaults to None.
 
     Returns:
-        tuple[Path, Path]: The path to the written csv file and associated metadata
-            file.
+        tuple[Path, Path | None]: The path to the written csv file and associated
+            metadata file.
     """
-    if to_csv_kwargs is None:
-        to_csv_kwargs = {}
+    to_csv_kwargs = kwargs.get("to_csv_kwargs", {})
 
     Path(filepath).parent.mkdir(parents=True, exist_ok=True)
 
     filepath, df = _to_dataframe(dataset, filepath, ".csv")
     df.to_csv(filepath, **to_csv_kwargs)  # type: ignore
 
-    metadata_path = _dump_metadata(dataset, filepath)
+    metadata_path = _dump_metadata(dataset, filepath) if metadata else None
 
     return Path(filepath), metadata_path
 
 
 def to_csv_collection(
     dataset: xr.Dataset,
     filepath: str | Path,
-    to_csv_kwargs: Dict[str, Any] | None = None,
-) -> tuple[tuple[Path, ...], Path]:
+    metadata: bool = True,
+    **kwargs: Any,
+) -> tuple[tuple[Path, ...], Path | None]:
     """Writes an xarray dataset to a collection of csv files.
 
     Output files are split such that each file contains the cartesian product of each
     unique pairing of coordinate dimensions.
 
     E.g., for a dataset with dimensions time and height with some variables dimensioned
     by time, some by height, and some by both, this will create three output files: one
@@ -59,35 +62,30 @@
     dimensioned by both (indexed by the cartesian product of time and height).
 
     Args:
         dataset (xr.Dataset): The dataset to write.
         filepath (str | Path): The base path for where to write the files. This should
             be the path to a file, not the path to a folder. This does not need to
             include a file extension; one will be added if not provided.
+        metadata (bool): If True, metadata from the xr.Dataset will be written to a
+            .json file next to the output file(s). Defaults to True.
         to_csv_kwargs (Dict[str, Any] | None, optional): Extra arguments to provide to
             pandas.DataFrame.to_csv() as keyword arguments. Defaults to None.
 
     Returns:
-        tuple[tuple[Path, ...], Path]: The paths to the written csv files and associated
-            metadata file.
+        tuple[tuple[Path, ...], Path | None]: The paths to the written csv files and
+            associated metadata file.
     """
-    if to_csv_kwargs is None:
-        to_csv_kwargs = {}
+    to_csv_kwargs = kwargs.get("to_csv_kwargs", {})
 
     Path(filepath).parent.mkdir(parents=True, exist_ok=True)
 
     data_groups = _to_dataframe_collection(dataset, filepath, ".csv")
 
     filepaths = []
     for fpath, df in data_groups:
         df.to_csv(fpath, **to_csv_kwargs)
         filepaths.append(fpath)
 
-    metadata_path = _dump_metadata(dataset, filepath)
+    metadata_path = _dump_metadata(dataset, filepath) if metadata else None
 
     return tuple(filepaths), metadata_path
-
-
-def to_timestream_csv():
-    ...
-
-    # tuple(filepaths), metadata_path
```

### Comparing `ncconvert-0.1.1/src/ncconvert/parquet.py` & `ncconvert-0.1.2/src/ncconvert/parquet.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,59 @@
 from __future__ import annotations
 
 from pathlib import Path
-from typing import Any, Dict
+from typing import Any
 
 import xarray as xr
 
 from .utils import _dump_metadata, _to_dataframe, _to_dataframe_collection
 
 
 def to_parquet(
     dataset: xr.Dataset,
     filepath: str | Path,
-    to_parquet_kwargs: Dict[str, Any] | None = None,
-) -> tuple[Path, Path]:
+    metadata: bool = True,
+    **kwargs: Any,
+) -> tuple[Path, Path | None]:
     """Writes an xarray dataset to a parquet file using basic settings.
 
     The output file will be indexed by the cartesian product of the dataset's indexes
     (coordinate variables).
 
     Args:
         dataset (xr.Dataset): The dataset to write.
         filepath (str | Path): Where to write the file. This should be the path to a
             file, not the path to a folder. This should include the file extension.
         to_parquet_kwargs (Dict[str, Any] | None, optional): Extra arguments to provide
             to pandas.DataFrame.to_parquet() as keyword arguments. Defaults to None.
+        metadata (bool): If True, metadata from the xr.Dataset will be written to a
+            .json file next to the output file. Defaults to True.
 
     Returns:
-        tuple[Path, Path]: The path to the written parquet file and associated metadata
-            file.
+        tuple[Path, Path | None]: The path to the written parquet file and associated
+            metadata file.
     """
-    if to_parquet_kwargs is None:
-        to_parquet_kwargs = {}
+    to_parquet_kwargs = kwargs.get("to_parquet_kwargs", {})
 
     Path(filepath).parent.mkdir(parents=True, exist_ok=True)
 
     filepath, df = _to_dataframe(dataset, filepath, ".parquet")
     df.to_parquet(filepath, **to_parquet_kwargs)  # type: ignore
 
-    metadata_path = _dump_metadata(dataset, filepath)
+    metadata_path = _dump_metadata(dataset, filepath) if metadata else None
 
     return Path(filepath), metadata_path
 
 
 def to_parquet_collection(
     dataset: xr.Dataset,
     filepath: str | Path,
-    to_parquet_kwargs: Dict[str, Any] | None = None,
-) -> tuple[tuple[Path, ...], Path]:
+    metadata: bool = True,
+    **kwargs: Any,
+) -> tuple[tuple[Path, ...], Path | None]:
     """Writes an xarray dataset to a collection of parquet files.
 
     Output files are split such that each file contains the cartesian product of each
     unique pairing of coordinate dimensions.
 
     E.g., for a dataset with dimensions time and height with some variables dimensioned
     by time, some by height, and some by both, this will create three output files: one
@@ -61,27 +64,28 @@
     Args:
         dataset (xr.Dataset): The dataset to write.
         filepath (str | Path): The base path for where to write the files. This should
             be the path to a file, not the path to a folder. This does not need to
             include a file extension; one will be added if not provided.
         to_parquet_kwargs (Dict[str, Any] | None, optional): Extra arguments to provide
             to pandas.DataFrame.to_parquet() as keyword arguments. Defaults to None.
+        metadata (bool): If True, metadata from the xr.Dataset will be written to a
+            .json file next to the output file(s). Defaults to True.
 
     Returns:
-        tuple[tuple[Path, ...], Path]: The paths to the written parquet files and
+        tuple[tuple[Path, ...], Path | None]: The paths to the written parquet files and
             associated metadata file.
     """
-    if to_parquet_kwargs is None:
-        to_parquet_kwargs = {}
+    to_parquet_kwargs = kwargs.get("to_parquet_kwargs", {})
 
     Path(filepath).parent.mkdir(parents=True, exist_ok=True)
 
     data_groups = _to_dataframe_collection(dataset, filepath, ".parquet")
 
     filepaths = []
     for fpath, df in data_groups:
         df.to_parquet(fpath, **to_parquet_kwargs)
         filepaths.append(fpath)
 
-    metadata_path = _dump_metadata(dataset, filepath)
+    metadata_path = _dump_metadata(dataset, filepath) if metadata else None
 
     return tuple(filepaths), metadata_path
```

### Comparing `ncconvert-0.1.1/src/ncconvert/utils.py` & `ncconvert-0.1.2/src/ncconvert/utils.py`

 * *Files identical despite different names*

### Comparing `ncconvert-0.1.1/src/ncconvert.egg-info/SOURCES.txt` & `ncconvert-0.1.2/src/ncconvert.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .coveragerc
 .gitignore
+LICENSE.md
 Makefile
 README.md
 pyproject.toml
 setup.py
 .github/workflows/pypi.yml
 .github/workflows/pytest.yml
 src/ncconvert/__init__.py
```

### Comparing `ncconvert-0.1.1/test/conftest.py` & `ncconvert-0.1.2/test/conftest.py`

 * *Files identical despite different names*

### Comparing `ncconvert-0.1.1/test/test_cli.py` & `ncconvert-0.1.2/test/test_cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,36 @@
+import sys
 from pathlib import Path
 
+import pytest
 import xarray as xr
 from typer.testing import CliRunner
 
 
+# NOTE: This test must run before any other tests that import ncconvert.cli, otherwise
+# the ncconvert.cli import will already be cached and we cannot mock missing deps
+def test_cli_import_error(
+    monkeypatch: pytest.MonkeyPatch, capsys: pytest.CaptureFixture[str]
+):
+    # Simulate the absence of required modules
+    monkeypatch.setitem(sys.modules, "tqdm", None)  # type: ignore
+    monkeypatch.setitem(sys.modules, "typer", None)  # type: ignore
+
+    # Importing the module with missing dependencies should exit with code 1
+    with pytest.raises(SystemExit) as e:
+        import ncconvert.cli  # noqa: F401
+    assert e.value.code == 1
+
+    # Check the output contains the expected error message
+    captured = capsys.readouterr()
+    assert "The ncconvert CLI requires extra dependencies" in captured.out
+    assert "Please run 'pip install ncconvert[cli]' to install these" in captured.out
+    assert "Aborting..." in captured.out
+
+
 def test_convert_cli(dataset: xr.Dataset):
     from ncconvert.cli import app
 
     # Hack needed to prevent xarray from raising a ValueError caused by it trying to
     # overwrite the 'units' attribute opn the time variable.
     dataset = dataset.copy()
     dataset["time"].encoding.update({"units": dataset["time"].attrs.pop("units")})
```

### Comparing `ncconvert-0.1.1/test/test_csv.py` & `ncconvert-0.1.2/test/test_csv.py`

 * *Files identical despite different names*

### Comparing `ncconvert-0.1.1/test/test_parquet.py` & `ncconvert-0.1.2/test/test_parquet.py`

 * *Files identical despite different names*

