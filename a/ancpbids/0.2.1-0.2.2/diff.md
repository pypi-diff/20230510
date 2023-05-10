# Comparing `tmp/ancpbids-0.2.1.tar.gz` & `tmp/ancpbids-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ancpbids-0.2.1.tar", last modified: Wed Nov 16 18:24:17 2022, max compression
+gzip compressed data, was "ancpbids-0.2.2.tar", last modified: Wed May 10 14:56:13 2023, max compression
```

## Comparing `ancpbids-0.2.1.tar` & `ancpbids-0.2.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:24:17.721021 ancpbids-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-11-16 18:24:08.000000 ancpbids-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-11-16 18:24:08.000000 ancpbids-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2283 2022-11-16 18:24:17.721021 ancpbids-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-11-16 18:24:08.000000 ancpbids-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:24:17.721021 ancpbids-0.2.1/ancpbids/
--rw-r--r--   0 runner    (1001) docker     (121)     5416 2022-11-16 18:24:08.000000 ancpbids-0.2.1/ancpbids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-11-16 18:24:17.721021 ancpbids-0.2.1/ancpbids/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:24:17.721021 ancpbids-0.2.1/ancpbids/data/
--rw-r--r--   0 runner    (1001) docker     (121)     3712 2022-11-16 18:24:08.000000 ancpbids-0.2.1/ancpbids/data/bids_graph_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    72453 2022-11-16 18:24:08.000000 ancpbids-0.2.1/ancpbids/model_v1_8_0.py
--rw-r--r--   0 runner    (1001) docker     (121)     5844 2022-11-16 18:24:08.000000 ancpbids-0.2.1/ancpbids/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:24:17.721021 ancpbids-0.2.1/ancpbids/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:24:08.000000 ancpbids-0.2.1/ancpbids/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8453 2022-11-16 18:24:08.000000 ancpbids-0.2.1/ancpbids/plugins/plugin_dsloader.py
--rw-r--r--   0 runner    (1001) docker     (121)     4180 2022-11-16 18:24:08.000000 ancpbids-0.2.1/ancpbids/plugins/plugin_dssaver.py
--rw-r--r--   0 runner    (1001) docker     (121)     3582 2022-11-16 18:24:08.000000 ancpbids-0.2.1/ancpbids/plugins/plugin_dsvalidator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2337 2022-11-16 18:24:08.000000 ancpbids-0.2.1/ancpbids/plugins/plugin_files_handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1359 2022-11-16 18:24:08.000000 ancpbids-0.2.1/ancpbids/plugins/plugin_metadata_inheritance_principle.py
--rw-r--r--   0 runner    (1001) docker     (121)    11991 2022-11-16 18:24:08.000000 ancpbids-0.2.1/ancpbids/plugins/plugin_schema_patches.py
--rw-r--r--   0 runner    (1001) docker     (121)    10182 2022-11-16 18:24:08.000000 ancpbids-0.2.1/ancpbids/pybids_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)    11674 2022-11-16 18:24:08.000000 ancpbids-0.2.1/ancpbids/query.py
--rw-r--r--   0 runner    (1001) docker     (121)     7284 2022-11-16 18:24:08.000000 ancpbids-0.2.1/ancpbids/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:24:17.721021 ancpbids-0.2.1/ancpbids.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2283 2022-11-16 18:24:17.000000 ancpbids-0.2.1/ancpbids.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-11-16 18:24:17.000000 ancpbids-0.2.1/ancpbids.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 18:24:17.000000 ancpbids-0.2.1/ancpbids.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-16 18:24:17.000000 ancpbids-0.2.1/ancpbids.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-11-16 18:24:08.000000 ancpbids-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:24:08.000000 ancpbids-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1143 2022-11-16 18:24:17.721021 ancpbids-0.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      821 2022-11-16 18:24:08.000000 ancpbids-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:24:17.721021 ancpbids-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:24:08.000000 ancpbids-0.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:24:17.721021 ancpbids-0.2.1/tests/auto/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:24:08.000000 ancpbids-0.2.1/tests/auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6522 2022-11-16 18:24:08.000000 ancpbids-0.2.1/tests/auto/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (121)     2352 2022-11-16 18:24:08.000000 ancpbids-0.2.1/tests/auto/test_derivative.py
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-11-16 18:24:08.000000 ancpbids-0.2.1/tests/auto/test_fetch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     5242 2022-11-16 18:24:08.000000 ancpbids-0.2.1/tests/auto/test_query.py
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-11-16 18:24:08.000000 ancpbids-0.2.1/tests/auto/test_regressions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1758 2022-11-16 18:24:08.000000 ancpbids-0.2.1/tests/auto/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     2145 2022-11-16 18:24:08.000000 ancpbids-0.2.1/tests/auto/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4417 2022-11-16 18:24:08.000000 ancpbids-0.2.1/tests/auto/test_writing.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-11-16 18:24:08.000000 ancpbids-0.2.1/tests/base_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:24:17.721021 ancpbids-0.2.1/tests/manual/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:24:08.000000 ancpbids-0.2.1/tests/manual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      993 2022-11-16 18:24:08.000000 ancpbids-0.2.1/tests/manual/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-11-16 18:24:08.000000 ancpbids-0.2.1/tests/manual/test_performance_regressions.py
--rw-r--r--   0 runner    (1001) docker     (121)    78254 2022-11-16 18:24:08.000000 ancpbids-0.2.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:13.618826 ancpbids-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-10 14:56:02.000000 ancpbids-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-10 14:56:02.000000 ancpbids-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-10 14:56:13.618826 ancpbids-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-10 14:56:02.000000 ancpbids-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:13.618826 ancpbids-0.2.2/ancpbids/
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-10 14:56:13.618826 ancpbids-0.2.2/ancpbids/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32110 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47198 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/model_v1_8_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:13.614825 ancpbids-0.2.2/ancpbids/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10839 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/plugins/plugin_dsloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/plugins/plugin_dssaver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/plugins/plugin_dsvalidator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/plugins/plugin_files_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/plugins/plugin_metadata_inheritance_principle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12168 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/plugins/plugin_schema_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/pybids_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:13.610825 ancpbids-0.2.2/ancpbids.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-10 14:56:13.000000 ancpbids-0.2.2/ancpbids.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-10 14:56:13.000000 ancpbids-0.2.2/ancpbids.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:56:13.000000 ancpbids-0.2.2/ancpbids.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 14:56:13.000000 ancpbids-0.2.2/ancpbids.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-10 14:56:02.000000 ancpbids-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:02.000000 ancpbids-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-10 14:56:13.618826 ancpbids-0.2.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      821 2023-05-10 14:56:02.000000 ancpbids-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:13.614825 ancpbids-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:13.618826 ancpbids-0.2.2/tests/auto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/auto/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/auto/test_derivative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/auto/test_fetch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/auto/test_ignored_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/auto/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/auto/test_regressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/auto/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/auto/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/auto/test_writing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/base_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:13.618826 ancpbids-0.2.2/tests/manual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/manual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/manual/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/manual/test_performance_regressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78254 2023-05-10 14:56:02.000000 ancpbids-0.2.2/versioneer.py
```

### Comparing `ancpbids-0.2.1/LICENSE` & `ancpbids-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.1/PKG-INFO` & `ancpbids-0.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: ancpbids
-Version: 0.2.1
+Version: 0.2.2
 Summary: Read/write/validate/query BIDS datasets
 Home-page: https://github.com/ANCPLabOldenburg/ancp-bids
 Author: Erdal Karaca
 Author-email: erdal.karaca.de@gmail.com
 Maintainer: ANCP Lab, University of Oldenburg
 Maintainer-email: currentancp@listserv.uni-oldenburg.de
 License: MIT
 Platform: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Documentation Status](https://readthedocs.org/projects/ancpbids/badge/?version=latest)](http://ancpbids.readthedocs.io/en/latest/?badge=latest)
 [![Latest Version](https://img.shields.io/pypi/v/ancpbids.svg)](https://pypi.python.org/pypi/ancpbids/)
@@ -32,11 +32,13 @@
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 # About
 ancpBIDS is a lightweight Python library to read/query/validate/write BIDS datasets.
 It can be used in workflows or analysis pipelines to handle IO specific aspects without bothering much about low level file system operations.
 Its implementation is based on the BIDS schema and allows it to evolve with the BIDS specification in a generic way.
 Using a plugin mechanism, contributors can extend its functionality in a controlled and clean manner.
 
-
+!!! ANNOUNCEMENT !!! As of version 0.22.0 the BIDSLayout has moved over to [PyBIDS](https://github.com/bids-standard/pybids) where it will be developed and maintained in future.
+ancpBIDS itself does not support this interface anymore but will act as a core package to PyBIDS and downstream projects needing a lightweight IO library to handle BIDS datasets.
+This documentation has not yet been updated to reflect this change.
 
 Read more on [readthedocs.io](https://ancpbids.readthedocs.io)
```

### Comparing `ancpbids-0.2.1/ancpbids/__init__.py` & `ancpbids-0.2.2/ancpbids/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,78 @@
 import logging
 import os
 import sys
+from dataclasses import dataclass
+from typing import Union, List, Optional
 
 from . import plugins
 from . import utils
 from .plugin import get_plugins, load_plugins_by_package, DatasetPlugin, WritingPlugin, ValidationPlugin, SchemaPlugin, \
     FileHandlerPlugin
 from .query import BoolExpr, Select, EqExpr, AnyExpr, AllExpr, ReExpr, CustomOpExpr, \
     EntityExpr
+from . import model_v1_8_0
+from . import model_v1_8_0 as model_latest
 
 LOGGER = logging.getLogger("ancpbids")
 
+
 # ENTITIES_PATTERN = regex.compile(r'(([^\W_]+)-([^\W_]+)_)+([^\W_]+)((\.[^\W_]+)+)')
 
+@dataclass
+class DatasetOptions(dict):
+    """All options that can be set to influence handling of reading/writing a dataset from/to file system."""
+    infer_artifact_datatype: bool = False
+    """If True, will determine the datatype an Artifact is contained in, either directly or within a sub-directory.
+        For example, given the path "sub-02/func/sub-02_task-mixedgamblestask_run-01_bold.nii.gz", the datatype will be "func".
+        
+        By default, this option is set to False as it may have a negative performance impact.
+    """
+
+    ignore: Union[bool, List[str]] = False
+    """If a .bidsignore file is available at the root, all resources (files/folders) matching the filters
+        in that file will not be added to the in-memory graph. Alternatively, a list of fnmatch patterns can be provided.
+        
+        By default, this option is set to False as it may have a negative performance impact."""
 
-def load_dataset(base_dir: str):
+
+def load_dataset(base_dir: str, options: Optional[DatasetOptions] = None):
     """Loads a dataset given its directory path on the file system.
 
     .. code-block::
 
         from ancpbids import load_dataset, validate_dataset
         dataset_path = 'path/to/your/dataset'
-        dataset = load_dataset(dataset_path)
+        dataset = load_dataset(dataset_path, DatasetOptions(ignore=False, infer_artifact_datatype=True))
 
     Parameters
     ----------
     base_dir:
         the dataset path to load from
+    options:
+        the options to use, see :py:class:`DatasetOptions` class for available options
 
     Returns
     -------
     str
-        an object instance of type :py:class:`ancpbids.model.Dataset` which represents the dataset as an in-memory graph
+        a Dataset object depending on the used schema which represents the dataset as an in-memory graph
     """
     if not os.path.isdir(base_dir):
         raise ValueError("Invalid Directory")
     schema = load_schema(base_dir)
     ds = schema.Dataset()
+    ds._versioned_schema = schema
+    ds.options = options
+    if ds.options is None:
+        ds.options = DatasetOptions()
     ds.name = os.path.basename(base_dir)
     ds.base_dir_ = base_dir
     dataset_plugins = get_plugins(DatasetPlugin)
     for dsplugin in dataset_plugins:
-        dsplugin.execute(ds)
+        dsplugin.execute(ds, schema)
     return ds
 
 
 def load_schema(base_dir):
     """Loads a BIDS schema object which represents the static/formal definition of the BIDS specification.
 
     As per BIDS spec, a BIDS compliant dataset must have a BIDSVersion field in the dataset_description.json
@@ -148,27 +175,22 @@
     save_dataset(ds, target_dir=ds.get_absolute_path(), context_folder=derivative)
 
 
 # load system plugins using lowest rank value
 load_plugins_by_package(plugins, ranking=0, system=True)
 
 # execute all SchemaPlugins, these plugins may monkey-patch the schema
-from ancpbids import model_v1_8_0
-from ancpbids import model_v1_8_0 as model_latest
-
 for pl in get_plugins(SchemaPlugin):
-    for model in [model_latest]:
-        pl.execute(model)
+    for schema in [model_v1_8_0]:
+        pl.execute(schema)
 
 # load file handler plugins
 for pl in get_plugins(FileHandlerPlugin):
     pl.execute(utils.FILE_READERS, utils.FILE_WRITERS)
 
-from .pybids_compat import BIDSLayout
-
 select = Select
 any_of = AnyExpr
 all_of = AllExpr
 eq = EqExpr
 re = ReExpr
 op = CustomOpExpr
 entity = EntityExpr
```

### Comparing `ancpbids-0.2.1/ancpbids/plugin.py` & `ancpbids-0.2.2/ancpbids/plugin.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.1/ancpbids/plugins/plugin_dsloader.py` & `ancpbids-0.2.2/ancpbids/plugins/plugin_dsloader.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,107 @@
+import fnmatch
 import inspect
 import os
 import re
 
+from .plugin_files_handlers import read_plain_text
 from .. import utils
 from ..plugin import DatasetPlugin
-
+from ..model_base import *
 
 class DatasetPopulationPlugin(DatasetPlugin):
-    def execute(self, dataset):
-        base_dir = dataset.base_dir_
-        self.schema = dataset.get_schema()
+
+    def execute(self, dataset, schema):
+        base_dir = str(dataset.base_dir_)
+        self.schema = schema
+        self.options = dataset.options
+        self._load_bidsignore(base_dir)
+
         # load file system structure
-        self._load_folder(dataset, base_dir)
+        self._load_folder(dataset, base_dir, base_dir)
         # transform files to artifacts, i.e. files containing entities in their name
         self._convert_files_to_artifacts(dataset)
+
+        # handle special files
+        self._handle_metadata_files(dataset)
+        self._handle_tsv_files(dataset)
+
         # expand structure based on schema-files
         self._expand_members(dataset)
         # convert Folders within derivatives to DerivativeFolder
         self._convert_derivatives_folders(dataset.derivatives)
 
+        # do optional stuff
+        self._determine_artifact_datatype(dataset)
+
+    def _determine_artifact_datatype(self, dataset):
+        if not self.options.infer_artifact_datatype:
+            return
+        datatype_folders = dataset.select(DatatypeFolder).objects()
+        for folder in datatype_folders:
+            artifacts = folder.select(Artifact).objects()
+            for artifact in artifacts:
+                artifact.datatype = folder.name
+
+    def _load_bidsignore(self, base_dir):
+        self.bidsignore = lambda relative_path: False
+        if self.options.ignore:
+            patterns = []
+            if isinstance(self.options.ignore, bool):
+                bidsignore_file = os.path.join(base_dir, ".bidsignore")
+                if os.path.exists(bidsignore_file):
+                    patterns = read_plain_text(bidsignore_file)
+            elif isinstance(self.options.ignore, list):
+                patterns = self.options.ignore
+
+            if patterns:
+                patterns = list(map(lambda pattern: pattern.strip(), patterns))
+                # TODO cleanup invalid filter such as empty lines or comments
+                self.bidsignore = lambda relative_path: next(
+                    filter(lambda pattern: fnmatch.fnmatch(relative_path, pattern), patterns), False)
+
+    def _handle_metadata_files(self, folder):
+        if not isinstance(folder, Folder):
+            return
+        for file in filter(lambda f: f.name.endswith(".json"), folder.files):
+            if isinstance(file, Artifact):
+                mdfile = MetadataArtifact()
+            else:
+                mdfile = MetadataFile()
+            mdfile.parent_object_ = folder
+            mdfile.update(file)
+            mdfile.contents = mdfile.load_contents()
+            folder.files.remove(file)
+            folder.files.append(mdfile)
+
+        for child in folder.folders:
+            self._handle_metadata_files(child)
+
+    def _handle_tsv_files(self, folder):
+        if not isinstance(folder, Folder):
+            return
+        for file in filter(lambda f: f.name.endswith(".tsv"), folder.files):
+            if isinstance(file, Artifact):
+                newfile = TSVArtifact()
+            else:
+                newfile = TSVFile()
+            newfile.parent_object_ = folder
+            newfile.update(file)
+            newfile.contents = newfile.load_contents()
+            folder.files.remove(file)
+            folder.files.append(newfile)
+
+        for child in folder.folders:
+            self._handle_tsv_files(child)
+
     def _convert_derivatives_folders(self, parent):
         if not parent:
             return
         for i, folder in enumerate(list(parent.folders)):
-            dfolder = self.schema.DerivativeFolder()
+            dfolder = DerivativeFolder()
             dfolder.parent_object_ = parent
             dfolder.update(folder)
             parent.folders[i] = dfolder
             self._convert_derivatives_folders(dfolder)
             self._expand_members(dfolder)
 
     def _convert_files_to_artifacts(self, parent):
@@ -40,134 +114,128 @@
         for folder in parent.folders:
             self._convert_files_to_artifacts(folder)
 
     def _convert_to_artifact(self, file):
         parts = utils.parse_bids_name(file.name)
         if not parts:
             return None
-        artifact = self.schema.Artifact()
+        artifact = Artifact()
         artifact.name = file.name
         for key, value in parts['entities'].items():
-            entity = self.schema.EntityRef()
+            entity = EntityRef()
             entity.key = key
             value = self.schema.process_entity_value(key, value)
             entity.value = value
             artifact.entities.append(entity)
         artifact.suffix = parts['suffix']
         artifact.extension = parts['extension']
         return artifact
 
     def _handle_direct_folders(self, parent, member, pattern, new_type):
-        if not isinstance(parent, self.schema.Folder):
+        if not isinstance(parent, Folder):
             return
-        folders = list(filter(lambda f: re.match(pattern, f.name), parent.get_folders_sorted()))
+        parent_folders = parent.get_folders_sorted()
+        folders = list(filter(lambda f: re.match(pattern, f.name), parent_folders))
         for folder in folders:
             obj = new_type()
             obj.name = folder.name
             obj.files = folder.files
+            for ofile in obj.files:
+                ofile.parent_object_ = obj
             obj.folders = folder.folders
+            for ofolder in obj.folders:
+                ofolder.parent_object_ = obj
             parent.remove_folder(folder.name)
             obj.parent_object_ = parent
             if member['max'] > 1:
                 getattr(parent, member['name']).append(obj)
             else:
                 setattr(parent, member['name'], obj)
             self._expand_members(obj)
 
     def _expand_member(self, parent, member):
         typ = member['type']
-        if not issubclass(typ, self.schema.Model):
+        if not issubclass(typ, Model):
             return
         mapper_name = '_type_handler_%s' % typ.__name__
         if mapper_name not in _TYPE_MAPPERS:
             mapper_name = '_type_handler_default'
         mapper = _TYPE_MAPPERS[mapper_name]
         mapper(self, parent, member)
 
     def _expand_members(self, folder):
-        members = folder.get_schema().get_members(type(folder))
+        members = self.schema.get_members(type(folder))
         for member in members:
             self._expand_member(folder, member)
 
-    def _load_folder(self, parent, dir_path):
+    def _load_folder(self, parent, dir_path, ds_path):
         for root, directories, files in os.walk(dir_path):
+            rel_base = root[len(ds_path):]
             for directory in sorted(directories):
-                folder = self.schema.Folder()
+                directory_ds_rel_path = '/'.join([rel_base, directory])[1:]
+                if self.bidsignore(directory_ds_rel_path):
+                    continue
+                folder = Folder()
                 folder.parent_object_ = parent
                 folder.name = directory
                 parent.folders.append(folder)
-                self._load_folder(folder, '/'.join([root, directory]))
+                self._load_folder(folder, '/'.join([root, directory]), ds_path)
             for file in sorted(files):
-                model_file = self.schema.File()
+                file_ds_rel_path = '/'.join([rel_base, file])[1:]
+                if self.bidsignore(file_ds_rel_path):
+                    continue
+                model_file = File()
                 model_file.parent_object_ = parent
                 model_file.name = file
                 parent.files.append(model_file)
+            # do not traverse into sub-dirs as they have been already processed recursively
             break
 
     def _type_handler_default(self, parent, member):
         typ = member['type']
-        if issubclass(typ, self.schema.JsonFile):
+        if issubclass(typ, JsonFile):
             self._type_handler_JsonFile(parent, member, True)
-        elif issubclass(typ, self.schema.Folder):
+        elif issubclass(typ, Folder):
             pattern = '.*'
             meta = member['meta']
             if 'name_pattern' in meta:
                 pattern = meta['name_pattern']
             self._handle_direct_folders(parent, member, pattern=pattern, new_type=typ)
 
     def _type_handler_File(self, parent, member):
-        if not isinstance(parent, self.schema.Folder):
+        if not isinstance(parent, Folder):
             return
-        file = parent.get_file(member['name'])
+        file_name = member['name']
+        meta = member['meta']
+        if 'name_pattern' in meta:
+            file_name = meta['name_pattern']
+        file = parent.get_file(file_name)
         if file:
             setattr(parent, member['name'], file)
             parent.remove_file(file.name)
 
-    def _type_handler_MetadataFile(self, parent, member):
-        if not isinstance(parent, self.schema.Folder):
-            return
-        if member['max'] > 1:
-            files = parent.get_files(member['meta']['name_pattern'])
-            files = list(filter(lambda f: isinstance(f, self.schema.Artifact), files))
-            for file in files:
-                mdfile = self.schema.MetadataFile()
-                mdfile.parent_object_ = parent
-                mdfile.update(file)
-                mdfile.contents = mdfile.load_contents()
-                getattr(parent, member['name']).append(mdfile)
-                parent.remove_file(file.name, from_meta=False)
-        else:
-            file = parent.get_file(member['name'])
-            if isinstance(file, self.schema.Artifact):
-                mdfile = self.schema.MetadataFile()
-                mdfile.parent_object_ = parent
-                mdfile.update(file)
-                mdfile.contents = mdfile.load_contents()
-                setattr(parent, member['name'], mdfile)
-                parent.remove_file(file.name, from_meta=False)
-
     def _type_handler_Artifact(self, parent, member):
-        if not isinstance(parent, self.schema.Folder):
+        if not isinstance(parent, Folder):
             return
         attr = getattr(parent, member['name'])
         multi = isinstance(attr, list)
         name = member['name']
         files = parent.files if multi else list(filter(lambda f: f.name == name, parent.files))
         for file in files:
-            if not isinstance(file, self.schema.Artifact):
+            if not isinstance(file, Artifact):
                 continue
             file.parent_object_ = parent
             parent.remove_file(file.name)
             if multi:
                 attr.append(file)
             else:
                 setattr(parent, member['name'], file)
 
     def _type_handler_Folder(self, parent, member):
-        if not isinstance(parent, self.schema.Folder):
+        if not isinstance(parent, Folder):
             return
         name = member['name']
         folder = parent.get_folder(name)
         if folder:
             setattr(parent, name, folder)
             parent.remove_folder(name)
```

### Comparing `ancpbids-0.2.1/ancpbids/plugins/plugin_dssaver.py` & `ancpbids-0.2.2/ancpbids/plugins/plugin_dssaver.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             for child_file in folder.files:
                 self._type_handler_File(src_dir, target_dir, child_file)
 
     def _get_ordered_entity_keys(self, artifact):
         schema = artifact.get_schema()
         entity_refs = artifact.entities
 
-        schema_entities = list(map(lambda e: e.literal_, list(schema.EntityEnum)))
+        schema_entities = list(map(lambda e: e.value['name'], list(schema.EntityEnum)))
         expected_key_order = {k: i for i, k in enumerate(schema_entities)}
         expected_order_key = {i: k for i, k in enumerate(schema_entities)}
 
         artifact_keys = list(map(lambda e: e.key, entity_refs))
         actual_keys_order = list(map(lambda k: expected_key_order[k], artifact_keys))
         expected = tuple(map(lambda k: expected_order_key[k], sorted(actual_keys_order)))
         return expected
@@ -79,15 +79,15 @@
                     artifact.add_entity('ses', name[4:])
                 if name.startswith("sub-"):
                     artifact.add_entity('sub', name[4:])
 
         # sort according order defined in schema
         ordered_keys = self._get_ordered_entity_keys(artifact)
         for ok in ordered_keys:
-            seg = '-'.join([ok, artifact.get_entity(ok)])
+            seg = '-'.join([ok, str(artifact.get_entity(ok))])
             segments.append(seg)
         segments.append(artifact.suffix)
         new_file_name = '_'.join(segments) + artifact.extension
         artifact.name = new_file_name
         self._type_handler_File(src_dir, target_dir, artifact, new_file_name)
```

### Comparing `ancpbids-0.2.1/ancpbids/plugins/plugin_dsvalidator.py` & `ancpbids-0.2.2/ancpbids/plugins/plugin_dsvalidator.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,30 +23,30 @@
                     report.warn(f"Missing recommended field {name} at {top_path}.",
                                 obj)
 
 
 class DatatypesValidationPlugin(ValidationPlugin):
     def execute(self, dataset, report: ValidationPlugin.ValidationReport):
         invalid = []
-        valid_datatypes = [v.literal_ for v in dataset.get_schema().DatatypeEnum.__members__.values()]
+        valid_datatypes = [v.name for v in dataset.get_schema().DatatypeEnum.__members__.values()]
         for subject in dataset.subjects:
             invalid.extend([f for f in subject.datatypes if f.name not in valid_datatypes])
             for session in subject.sessions:
                 invalid.extend([f for f in session.datatypes if f.name not in valid_datatypes])
 
         for folder in invalid:
             report.error("Unsupported datatype folder '%s'" % folder.get_relative_path(),
                          folder)
 
 
 class EntitiesValidationPlugin(ValidationPlugin):
     def execute(self, dataset, report: ValidationPlugin.ValidationReport):
         schema = dataset.get_schema()
         artifacts = dataset.select(schema.Artifact).get_artifacts()
-        entities = list(map(lambda e: e.literal_, list(schema.EntityEnum)))
+        entities = list(map(lambda e: e.value['name'], list(schema.EntityEnum)))
         expected_key_order = {k: i for i, k in enumerate(entities)}
         expected_order_key = {i: k for i, k in enumerate(entities)}
         for artifact in artifacts:
             entity_refs = artifact.entities
             found_invalid_key = False
             for ref in entity_refs:
                 if ref.key not in entities:
```

### Comparing `ancpbids-0.2.1/ancpbids/plugins/plugin_files_handlers.py` & `ancpbids-0.2.2/ancpbids/plugins/plugin_files_handlers.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.1/ancpbids/plugins/plugin_schema_patches.py` & `ancpbids-0.2.2/ancpbids/plugins/plugin_schema_patches.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 import sys
 from difflib import SequenceMatcher
 
 from ancpbids.plugin import SchemaPlugin
 from ancpbids.query import Select, query, query_entities
 from ancpbids.utils import resolve_segments, convert_to_relative
+from ancpbids.model_base import *
 
 
 def has_entity(artifact, entity_):
     for e in artifact.entities:
         if e.key == entity_:
             return True
     return False
@@ -20,25 +21,29 @@
 def get_entity(artifact, entity_):
     for e in artifact.entities:
         if e.key == entity_:
             return e.value
     return None
 
 
-def add_entity(artifact, key, value):
-    schema = artifact.get_schema()
+def add_entity(schema, artifact, key, value):
     if isinstance(key, schema.EntityEnum):
         key = key.entity_
-    eref = schema.EntityRef(key, value)
-    artifact.entities.append(eref)
 
+    found = list(filter(lambda er: er.key == key, artifact.entities))
+    if found:
+        found[0].value = value
+    else:
+        eref = EntityRef(key, value)
+        artifact.entities.append(eref)
 
-def add_entities(artifact, **kwargs):
+
+def add_entities(schema, artifact, **kwargs):
     for k, v in kwargs.items():
-        add_entity(artifact, k, v)
+        add_entity(schema, artifact, k, v)
 
 
 def load_file_contents(folder, file_name, return_type: str = None):
     from ancpbids import utils
     file_path = get_absolute_path(folder, file_name)
     contents = utils.load_contents(file_path, return_type)
     return contents
@@ -64,113 +69,109 @@
 
 
 def _file_get_relative_path(file):
     return _get_path(file.parent_object_, file.name, False)
 
 
 def _get_path(folder, file_name=None, absolute=True):
-    schema = folder.get_schema()
     segments = []
     if file_name:
         segments.append(file_name)
     current_folder = folder
     while current_folder is not None:
-        if isinstance(current_folder, schema.Dataset):
+        if isinstance(current_folder, Dataset):
             if absolute:
                 segments.insert(0, current_folder.base_dir_)
             # assume we reached the highest level, maybe not good for nested datasets
             break
         else:
             segments.insert(0, current_folder.name)
         current_folder = current_folder.parent_object_
     _path = os.path.join(*segments) if segments else ''
-    return os.path.normpath(_path)
+    _path = os.path.normpath(_path)
+    if absolute:
+        _path = os.path.abspath(_path)
+    return _path
 
 
-def remove_file(folder, file_name, from_meta=True):
+def remove_file(folder, file_name):
     folder.files = list(filter(lambda file: file.name != file_name, folder.files))
-    if from_meta:
-        folder.metadatafiles = list(filter(lambda file: file.name != file_name, folder.metadatafiles))
 
 
 def create_artifact(folder, raw=None):
-    schema = folder.get_schema()
-    artifact = schema.Artifact()
-    if isinstance(raw, schema.Artifact):
+    artifact = Artifact()
+    if isinstance(raw, Artifact):
         artifact.entities.extend(raw.entities)
     artifact.parent_object_ = folder
     folder.files.append(artifact)
     return artifact
 
 
 def create_folder(folder, type_=None, **kwargs):
     if not type_:
-        type_ = folder.get_schema().Folder
+        type_ = Folder
     sub_folder = type_(**kwargs)
     sub_folder.parent_object_ = folder
     folder.folders.append(sub_folder)
     return sub_folder
 
 
 def create_derivative(ds, path=None, **kwargs):
-    schema = ds.get_schema()
     derivatives_folder = ds.derivatives
     if not ds.derivatives:
-        derivatives_folder = schema.DerivativeFolder()
+        derivatives_folder = DerivativeFolder()
         derivatives_folder.parent_object_ = ds
         derivatives_folder.name = "derivatives"
         ds.derivatives = derivatives_folder
     path = convert_to_relative(ds, path)
     target_folder, _ = resolve_segments(derivatives_folder, path, create_if_missing=True)
-    derivative = schema.DerivativeFolder(**kwargs)
+    derivative = DerivativeFolder(**kwargs)
     derivative.parent_object_ = target_folder
     target_folder.folders.append(derivative)
 
-    derivative.dataset_description = schema.DerivativeDatasetDescriptionFile()
+    derivative.dataset_description = DerivativeDatasetDescriptionFile()
     derivative.dataset_description.parent_object_ = derivative
-    derivative.dataset_description.GeneratedBy = schema.GeneratedBy()
+    derivative.dataset_description.GeneratedBy = GeneratedBy()
 
     if ds.dataset_description:
         derivative.dataset_description.update(ds.dataset_description)
 
     return derivative
 
 
 def create_dataset(schema, **kwargs):
-    ds = schema.Dataset()
+    ds = Dataset()
+    ds._versioned_schema = schema
     ds.update(**kwargs)
-    ds.dataset_description = schema.DatasetDescriptionFile(name="dataset_description.json")
+    ds.dataset_description = DatasetDescriptionFile(name="dataset_description.json")
     ds.dataset_description.BIDSVersion = schema.VERSION
     ds.dataset_description.parent_object_ = ds
     return ds
 
 
 def get_file(folder, file_name):
     folder, file_name = resolve_segments(folder, file_name, True)
     if not folder:
         return None
-    schema = folder.get_schema()
-    direct_files = folder.to_generator(depth_first=True, depth=1, filter_=lambda n: isinstance(n, schema.File))
+    direct_files = folder.to_generator(depth_first=True, depth=1, filter_=lambda n: isinstance(n, File))
     file = next(filter(lambda f: f.name == file_name, direct_files), None)
     return file
 
 
 def get_files(folder, name_pattern):
-    schema = folder.get_schema()
-    direct_files = folder.to_generator(depth_first=True, depth=1, filter_=lambda n: isinstance(n, schema.File))
+    direct_files = folder.to_generator(depth_first=True, depth=1, filter_=lambda n: isinstance(n, File))
     return list(filter(lambda file: fnmatch.fnmatch(file.name, name_pattern), direct_files))
 
 
 def remove_folder(folder, folder_name):
     folder.folders = list(filter(lambda f: f.name != folder_name, folder.folders))
 
 
 def get_folder(folder, folder_name):
-    schema = folder.get_schema()
-    direct_folders = folder.to_generator(depth_first=True, depth=1, filter_=lambda n: isinstance(n, schema.Folder))
+    direct_folders = folder.to_generator(depth_first=True, depth=1, filter_=lambda n: isinstance(n, Folder))
     return next(filter(lambda f: f.name == folder_name, direct_folders), None)
 
 
 def get_files_sorted(folder):
     return sorted(folder.files, key=lambda f: f.name)
 
 
@@ -183,21 +184,20 @@
         return
 
     if not depth_first:
         if filter_ and not filter_(source):
             return
         yield source
 
-    schema = source.get_schema()
     for key, value in source.items():
-        if isinstance(value, schema.Model):
+        if isinstance(value, Model):
             yield from to_generator(value, depth_first, filter_, depth - 1)
         elif isinstance(value, list):
             for item in value:
-                if isinstance(item, schema.Model):
+                if isinstance(item, Model):
                     yield from to_generator(item, depth_first, filter_, depth - 1)
 
     if depth_first:
         if filter_ and not filter_(source):
             return
         yield source
 
@@ -274,26 +274,26 @@
         return value
 
 
 def process_entity_value(schema, key, value):
     if not value:
         return value
     if isinstance(key, schema.EntityEnum):
-        key = key.literal_
-    for sc_entity in filter(lambda e: e.literal_ == key, schema.EntityEnum.__members__.values()):
-        if sc_entity.format_ == 'index':
+        key = key.value['name']
+    for sc_entity in filter(lambda e: e.value['name'] == key, schema.EntityEnum.__members__.values()):
+        if sc_entity.value['format'] == 'index':
             if isinstance(value, list):
                 return list(map(lambda v: _trim_int(v) if v is not None else v, value))
             else:
                 return _trim_int(value)
     return value
 
 
 def fuzzy_match_entity_key(schema, user_key):
-    return fuzzy_match_entity(schema, user_key).literal_
+    return fuzzy_match_entity(schema, user_key).value['name']
 
 
 def fuzzy_match_entity(schema, user_key):
     ratios = list(
         map(lambda item: (
             item,
             1.0 if item.name.startswith(user_key) else SequenceMatcher(None, user_key,
@@ -313,27 +313,37 @@
     return Select(context, target_type)
 
 
 def get_entities(artifact):
     return {e['key']: e['value'] for e in artifact.entities}
 
 
+def get_schema(model):
+    current = model
+    while current is not None:
+        if isinstance(current, Dataset):
+            return current._versioned_schema
+        current = current.parent_object_
+    return None
+
+
 class PatchingSchemaPlugin(SchemaPlugin):
     def execute(self, schema):
+        schema.Model.get_schema = get_schema
         schema.Model.__hash__ = lambda self: hash(tuple(self))
         schema.Folder.select = select
         schema.Folder.query = query
         schema.Folder.query_entities = query_entities
         schema.File.get_parent = get_parent
         schema.Folder.get_parent = get_parent
         schema.Artifact.has_entity = has_entity
         schema.Artifact.get_entity = get_entity
         schema.Artifact.get_entities = get_entities
-        schema.Artifact.add_entity = add_entity
-        schema.Artifact.add_entities = add_entities
+        schema.Artifact.add_entity = lambda artifact, key, value: add_entity(schema, artifact, key, value)
+        schema.Artifact.add_entities = lambda artifact, **kwargs: add_entities(schema, artifact, **kwargs)
         schema.Folder.load_file_contents = load_file_contents
         schema.File.load_contents = load_contents
         schema.File.get_absolute_path = get_absolute_path_by_file
         schema.Folder.get_relative_path = _folder_get_relative_path
         schema.Folder.get_absolute_path = get_absolute_path
         schema.File.get_relative_path = _file_get_relative_path
         schema.Folder.remove_file = remove_file
```

### Comparing `ancpbids-0.2.1/ancpbids/pybids_compat.py` & `ancpbids-0.2.2/ancpbids/pybids_compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os.path
 import warnings
-from collections import OrderedDict
 from functools import partial
 from typing import List, Union, Dict
 
 import ancpbids
-from ancpbids import CustomOpExpr, EntityExpr, AllExpr, ValidationPlugin
-from . import load_dataset, LOGGER
-from .query import query, query_entities, FnMatchExpr, AnyExpr
-from .utils import deepupdate, resolve_segments, convert_to_relative
-
+from ancpbids import ValidationPlugin
+from . import load_dataset
+from .query import query, query_entities
+from .utils import resolve_segments, convert_to_relative
 
 warnings.warn('Development of the BIDSLayout interface will continue in the pybids project.')
 
 class BIDSLayout:
-    """A convenience class to provide access to an in-memory representation of a BIDS dataset.
+    """WARNING: Development of this class will continue in the pybids project.
+
+    A convenience class to provide access to an in-memory representation of a BIDS dataset.
 
     .. code-block::
 
         dataset_path = 'path/to/your/dataset'
         layout = BIDSLayout(dataset_path)
 
     Parameters
@@ -73,15 +73,15 @@
         path = os.path.normpath(path)
         # make relative to dataset root, i.e., remove base path
         if path.startswith(self.dataset.base_dir_):
             path = path[len(self.dataset.base_dir_):].strip(os.sep)
         file = self.dataset.get_file(path)
         md = file.get_metadata()
         if md and include_entities:
-            schema_entities = {e.entity_: e.literal_ for e in list(self.schema.EntityEnum)}
+            schema_entities = {e.literal_: e.name for e in list(self.schema.EntityEnum)}
             md.update({schema_entities[e.key]: e.value for e in file.entities})
         return md
 
     def get(self, return_type: str = 'object', target: str = None, scope: str = None,
             extension: Union[str, List[str]] = None, suffix: Union[str, List[str]] = None,
             **entities) -> Union[List[str], List[object]]:
         """Depending on the return_type value returns either paths to files that matched the filtering criteria
```

### Comparing `ancpbids-0.2.1/ancpbids/query.py` & `ancpbids-0.2.2/ancpbids/query.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import os
 import re
 import sys
 from collections import OrderedDict
 from fnmatch import fnmatch
 from typing import Union, List
 
 from ancpbids.utils import resolve_segments
+from ancpbids.model_base import *
 
 
 class Expr:
     def convert_value(self, value):
         if hasattr(self, 'value_converter'):
             value = self.value_converter(value)
         return value
@@ -107,15 +109,15 @@
         self.op = op(schema.EntityRef.value, pattern)
         self.op.value_converter = lambda v: schema.process_entity_value(key, v)
 
     def eval(self, context) -> bool:
         if not isinstance(context, self.schema.Artifact):
             # for non-Artifacts, for example File, just return false
             return False
-        ents = list(filter(lambda e: e.key == self.key.literal_, context.entities))
+        ents = list(filter(lambda e: e.key == self.key.value['name'], context.entities))
         if not ents:
             # the entity must not exist
             if self.pattern is None:
                 return True
             return False
         if self.pattern is None:
             # the entity must not exist, but we found one
@@ -140,19 +142,19 @@
         return self
 
     def _exec(self, callback, depth=sys.maxsize):
         for m in self.context.to_generator(filter_=lambda o: self._subtree.eval(o), depth=depth):
             if isinstance(m, self.filter_type) and self._where.eval(m):
                 yield callback(m)
 
-    def get_file_paths(self):
-        return self._exec(self.schema.File.get_relative_path)
+    def get_file_paths(self, depth=sys.maxsize):
+        return self._exec(self.schema.File.get_relative_path, depth=depth)
 
-    def get_file_paths_absolute(self):
-        return self._exec(self.schema.File.get_absolute_path)
+    def get_file_paths_absolute(self, depth=sys.maxsize):
+        return self._exec(self.schema.File.get_absolute_path, depth=depth)
 
     def get_artifacts(self):
         # TODO filter by Artifact instances
         return self.objects()
 
     def objects(self, as_list=False, depth=sys.maxsize):
         result = self._exec(callback=lambda m: m, depth=depth)
@@ -185,15 +187,15 @@
         a wrapping expression to make sure that the provided object is an instance of Artifact
     """
     return AllExpr(CustomOpExpr(lambda m: isinstance(m, schema.Artifact)), expr)
 
 
 def query(folder, return_type: str = 'object', target: str = None, scope: str = None,
           extension: Union[str, List[str]] = None, suffix: Union[str, List[str]] = None,
-          regex_search=False,
+          regex_search=False, sorter=None,
           **entities) -> Union[List[str], List[object]]:
     """Depending on the return_type value returns either paths to files that matched the filtering criteria
     or :class:`Artifact <ancpbids.model_v1_7_0.Artifact>` objects for further processing by the caller.
 
     Note that all provided filter criteria are AND combined, i.e. subj='02',task='lang' will match files containing
     '02' as a subject AND 'lang' as a task. If you provide a list of values for a criteria, they will be OR combined.
 
@@ -240,79 +242,87 @@
     if return_type == 'id':
         if not target:
             raise ValueError("return_type=id requires the target parameter to be set")
 
     schema = folder.get_schema()
     context = folder
     ops = []
-    target_type = schema.File
+    target_type = File
     if scope not in ['all', 'raw', 'self']:
         context, _ = resolve_segments(folder, scope, False)
 
     if not context:
         return None
 
     select = context.select(target_type)
 
     if scope == 'raw':
         # the raw scope does not search in derivatives folder but everything else
-        select.subtree(CustomOpExpr(lambda m: not isinstance(m, schema.DerivativeFolder)))
+        select.subtree(CustomOpExpr(lambda m: not isinstance(m, DerivativeFolder)))
 
     result_extractor = None
     if target:
         if target in 'suffixes':
             suffix = '*'
-            result_extractor = lambda artifacts: [a.suffix for a in artifacts]
+            result_extractor = lambda artifacts: [a.suffix for a in artifacts if a.suffix]
         elif target in 'extensions':
             extension = '*'
-            result_extractor = lambda artifacts: [a.extension for a in artifacts]
+            result_extractor = lambda artifacts: [a.extension for a in artifacts if a.extension]
         else:
             target = schema.fuzzy_match_entity_key(target)
             entities = {**entities, target: '*'}
             result_extractor = lambda artifacts: [entity.value for a in artifacts for entity in
-                                                  filter(lambda e: e.key == target, a.entities)]
+                                                  filter(lambda e: e.key == target, a.entities) if a.entities]
 
     search_operator = FnMatchExpr
     if regex_search:
         search_operator = ReExpr
 
     for k, v in entities.items():
         entity_key = schema.fuzzy_match_entity(k)
         v = schema.process_entity_value(entity_key, v)
         ops.append(
             _require_artifact(schema,
                               _to_any_expr(v, lambda val: EntityExpr(schema, entity_key, val, op=search_operator))))
 
     if extension:
         converter = lambda v: "." + v if v != "*" and not v.startswith(".") else v
-        any_expr = _to_any_expr(extension, lambda ext: search_operator(schema.Artifact.extension, ext), converter)
+        any_expr = _to_any_expr(extension, lambda ext: search_operator(Artifact.extension, ext), converter)
         require_expr = _require_artifact(schema, any_expr)
         ops.append(require_expr)
 
     if suffix:
         ops.append(
             _require_artifact(schema,
-                              _to_any_expr(suffix, lambda suf: search_operator(schema.Artifact.suffix, suf))))
+                              _to_any_expr(suffix, lambda suf: search_operator(Artifact.suffix, suf))))
 
     select.where(AllExpr(*ops))
 
+    search_depth = sys.maxsize
+    if scope == "self":
+        search_depth = 1
+
     if return_type:
         if return_type.startswith("file"):
             return list(select.get_file_paths_absolute())
         elif return_type == 'dir':
-            result = filter(lambda o: isinstance(o, schema.File), select.objects())
+            result = filter(lambda o: isinstance(o, File), select.objects(depth=search_depth))
             return set(map(lambda a: a.get_parent().get_relative_path(), result))
 
-    artifacts = select.objects()
+    artifacts = select.objects(depth=search_depth)
+    if sorter is None:
+        sorter = lambda artifact: artifact.name
+    if callable(sorter):
+        artifacts = sorted(artifacts, key=sorter)
     if result_extractor:
         return sorted(set(result_extractor(artifacts)))
     return list(artifacts)
 
 
-def query_entities(folder, scope: str = None, sort: bool = False, long_form=False) -> dict:
+def query_entities(folder, scope: str = None, sort: bool = False, long_form=True) -> dict:
     """Returns a unique set of entities found within the dataset as a dict.
     Each key of the resulting dict contains a list of values (with at least one element).
 
     Example dict:
     .. code-block::
 
         {
@@ -331,20 +341,20 @@
 
     Returns
     -------
     dict
         a unique set of entities found within the dataset as a dict
     """
     schema = folder.get_schema()
-    known_entities = {e.name: e.literal_ for e in list(schema.EntityEnum)}
     artifacts = filter(lambda m: isinstance(m, schema.Artifact), query(folder, scope=scope))
     result = {}
     for e in [e for a in artifacts for e in a.entities]:
         key = e.key
         if key not in result:
             result[key] = set()
         result[key].add(e.value)
     if long_form:
+        known_entities = {e.value['name']: e.name for e in list(schema.EntityEnum)}
         result = {known_entities[k] if k in known_entities else k: v for k, v in result.items()}
     if sort:
         result = {k: sorted(v) for k, v in sorted(result.items())}
     return result
```

### Comparing `ancpbids-0.2.1/ancpbids/utils.py` & `ancpbids-0.2.2/ancpbids/utils.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.1/ancpbids.egg-info/PKG-INFO` & `ancpbids-0.2.2/ancpbids.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: ancpbids
-Version: 0.2.1
+Version: 0.2.2
 Summary: Read/write/validate/query BIDS datasets
 Home-page: https://github.com/ANCPLabOldenburg/ancp-bids
 Author: Erdal Karaca
 Author-email: erdal.karaca.de@gmail.com
 Maintainer: ANCP Lab, University of Oldenburg
 Maintainer-email: currentancp@listserv.uni-oldenburg.de
 License: MIT
 Platform: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Documentation Status](https://readthedocs.org/projects/ancpbids/badge/?version=latest)](http://ancpbids.readthedocs.io/en/latest/?badge=latest)
 [![Latest Version](https://img.shields.io/pypi/v/ancpbids.svg)](https://pypi.python.org/pypi/ancpbids/)
@@ -32,11 +32,13 @@
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 # About
 ancpBIDS is a lightweight Python library to read/query/validate/write BIDS datasets.
 It can be used in workflows or analysis pipelines to handle IO specific aspects without bothering much about low level file system operations.
 Its implementation is based on the BIDS schema and allows it to evolve with the BIDS specification in a generic way.
 Using a plugin mechanism, contributors can extend its functionality in a controlled and clean manner.
 
-
+!!! ANNOUNCEMENT !!! As of version 0.22.0 the BIDSLayout has moved over to [PyBIDS](https://github.com/bids-standard/pybids) where it will be developed and maintained in future.
+ancpBIDS itself does not support this interface anymore but will act as a core package to PyBIDS and downstream projects needing a lightweight IO library to handle BIDS datasets.
+This documentation has not yet been updated to reflect this change.
 
 Read more on [readthedocs.io](https://ancpbids.readthedocs.io)
```

### Comparing `ancpbids-0.2.1/ancpbids.egg-info/SOURCES.txt` & `ancpbids-0.2.2/ancpbids.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -4,37 +4,38 @@
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 versioneer.py
 ancpbids/__init__.py
 ancpbids/_version.py
+ancpbids/model_base.py
 ancpbids/model_v1_8_0.py
 ancpbids/plugin.py
 ancpbids/pybids_compat.py
 ancpbids/query.py
 ancpbids/utils.py
 ancpbids.egg-info/PKG-INFO
 ancpbids.egg-info/SOURCES.txt
 ancpbids.egg-info/dependency_links.txt
 ancpbids.egg-info/top_level.txt
-ancpbids/data/bids_graph_schema.yaml
 ancpbids/plugins/__init__.py
 ancpbids/plugins/plugin_dsloader.py
 ancpbids/plugins/plugin_dssaver.py
 ancpbids/plugins/plugin_dsvalidator.py
 ancpbids/plugins/plugin_files_handlers.py
 ancpbids/plugins/plugin_metadata_inheritance_principle.py
 ancpbids/plugins/plugin_schema_patches.py
 tests/__init__.py
 tests/base_test_case.py
 tests/auto/__init__.py
 tests/auto/test_basic.py
 tests/auto/test_derivative.py
 tests/auto/test_fetch_dataset.py
+tests/auto/test_ignored_resources.py
 tests/auto/test_query.py
 tests/auto/test_regressions.py
 tests/auto/test_schema.py
 tests/auto/test_validation.py
 tests/auto/test_writing.py
 tests/manual/__init__.py
 tests/manual/test_benchmark.py
```

### Comparing `ancpbids-0.2.1/setup.py` & `ancpbids-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.1/tests/auto/test_basic.py` & `ancpbids-0.2.2/tests/auto/test_basic.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import os.path
+
 import numpy
 
-from ancpbids import load_dataset
+from ancpbids import load_dataset, DatasetOptions
 from ancpbids.utils import parse_bids_name
 from ..base_test_case import *
 
 
 class BasicTestCase(BaseTestCase):
     def test_naming_scheme(self):
         valid_names = ["sub-11_task-mixedgamblestask_run-02_events.tsv", "sub-11_dwi.nii.gz", "x-01_y-02_z-03_xyz.abc",
@@ -57,22 +59,29 @@
         self.assertEqual(3, len(datatypes))
 
         anat_datatype = datatypes[0]
         self.assertEqual("anat", anat_datatype.name)
         func_datatype = datatypes[-1]
         self.assertEqual("func", func_datatype.name)
 
-        artifacts = func_datatype.artifacts
-        self.assertEqual(6, len(artifacts))
+        artifacts = func_datatype.query(suffix="bold", scope="self")
+        self.assertEqual(3, len(artifacts))
         self.assertEqual("sub-01_task-mixedgamblestask_run-01_bold.nii.gz", artifacts[0].name)
-        self.assertEqual("sub-01_task-mixedgamblestask_run-03_events.tsv", artifacts[-1].name)
+        self.assertEqual("sub-01_task-mixedgamblestask_run-02_bold.nii.gz", artifacts[1].name)
+        self.assertEqual("sub-01_task-mixedgamblestask_run-03_bold.nii.gz", artifacts[2].name)
 
-        metadatafiles = func_datatype.metadatafiles
-        self.assertEqual(1, len(metadatafiles))
-        self.assertEqual("sub-01_task-mixedgamblestask_run-01_events.json", metadatafiles[0].name)
+        eventmetafiles = func_datatype.query(suffix="events", extension=".json", scope="self")
+        self.assertEqual(1, len(eventmetafiles))
+        self.assertEqual("sub-01_task-mixedgamblestask_run-01_events.json", eventmetafiles[0].name)
+
+        tsvfiles = func_datatype.query(extension=".tsv", scope="self")
+        self.assertEqual(3, len(tsvfiles))
+        self.assertEqual("sub-01_task-mixedgamblestask_run-01_events.tsv", tsvfiles[0].name)
+        self.assertEqual("sub-01_task-mixedgamblestask_run-02_events.tsv", tsvfiles[1].name)
+        self.assertEqual("sub-01_task-mixedgamblestask_run-03_events.tsv", tsvfiles[2].name)
 
     def test_json_file_contents(self):
         ds005 = load_dataset(DS005_DIR)
         dataset_description = ds005.load_file_contents("dataset_description.json")
         self.assertTrue(isinstance(dataset_description, dict), "Expected a dictionary")
         self.assertEqual("1.0.0rc2", dataset_description['BIDSVersion'])
         self.assertEqual("Mixed-gambles task", dataset_description['Name'])
@@ -89,15 +98,15 @@
         self.assertListEqual(['participant_id', 'sex', 'age'], list(participants.columns))
         self.assertEqual(16, len(participants))
 
     def test_parse_entities_in_filenames(self):
         ds005 = load_dataset(DS005_DIR)
         # get first artifact in func datatype of first subject/session:
         # sub-16_task-mixedgamblesatask_run-01_bold.nii.gz
-        artifact = ds005.subjects[0].datatypes[-1].artifacts[0]
+        artifact = ds005.subjects[0].datatypes[-1].query(scope="self")[0]
         self.assertTrue(isinstance(artifact, ds005.get_schema().Artifact))
 
         self.assertEqual("bold", artifact.suffix)
         self.assertEqual(".nii.gz", artifact.extension)
 
         entities = artifact.entities
         self.assertTrue(isinstance(entities, list))
@@ -138,10 +147,39 @@
         ds005 = load_dataset(DS005_DIR)
         self.assertEqual("{'name': 'ds005'}", str(ds005))
         self.assertEqual("{'name': 'derivatives'}", str(ds005.derivatives))
         self.assertEqual("{'name': 'README'}", str(ds005.README))
         expected = "{'name': 'dataset_description.json', 'Name': 'Mixed-gambles task', 'BIDSVersion': '1.0.0rc2', 'License': 'This dataset is made available u[...]'}"
         self.assertEqual(expected, str(ds005.dataset_description))
 
+    def test_participants_tsv(self):
+        ds005 = load_dataset(DS005_DIR)
+        schema = ds005.get_schema()
+        self.assertTrue(isinstance(ds005.participants_tsv, schema.TSVFile))
+        contents = ds005.participants_tsv.contents
+        self.assertTrue(contents is not None)
+        self.assertEqual(16, len(contents))
+        self.assertEqual(['participant_id', 'sex', 'age'], list(contents[0].keys()))
+        self.assertEqual(['sub-01', '0', '28'], list(contents[0].values()))
+
+        # or short form:
+        self.assertEqual({'participant_id': 'sub-01', 'sex': '0', 'age': '28'}, contents[0])
+
+    def test_absolute_path(self):
+        ds_path_norm = os.path.normpath(DS005_DIR)
+        ds005 = load_dataset(ds_path_norm)
+        ds_path = ds005.get_absolute_path()
+        self.assertEqual(ds_path, ds_path_norm)
+
+    def test_datatype_of_artifact(self):
+        ds005 = load_dataset(DS005_DIR)
+        anat_files = ds005.query(scope="raw", sub="01", suffix="T1w")
+        assert len(anat_files) == 1
+        assert anat_files[0].datatype is None
+
+        ds005 = load_dataset(DS005_DIR, DatasetOptions(infer_artifact_datatype=True))
+        anat_files = ds005.query(scope="raw", sub="01", suffix="T1w")
+        assert len(anat_files) == 1
+        assert anat_files[0].datatype == "anat"
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ancpbids-0.2.1/tests/auto/test_derivative.py` & `ancpbids-0.2.2/tests/auto/test_derivative.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.1/tests/auto/test_fetch_dataset.py` & `ancpbids-0.2.2/tests/auto/test_fetch_dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import os.path
 import unittest
 import tempfile
 
-from ancpbids import utils, BIDSLayout
+from ancpbids import utils, load_dataset
 from ..base_test_case import BaseTestCase
 
 
 class FetchDatasetTestCase(BaseTestCase):
     def test_fetch_dataset(self):
         with tempfile.TemporaryDirectory() as temp_dir:
             ds_path = utils.fetch_dataset('ds003483', output_dir=temp_dir)
             self.assertEqual(os.path.join(temp_dir, 'ds003483'), ds_path)
-            layout = BIDSLayout(ds_path)
+            dataset = load_dataset(ds_path)
 
             # some basic checks to make sure the dataset is downloaded and unzipped as expected
-            self.assertEqual('ds003483', layout.dataset.name)
-            self.assertEqual(21, len(layout.get_subjects()))
-            self.assertEqual(['channels', 'coordsystem', 'events', 'meg', 'scans'], layout.get_suffixes())
+            self.assertEqual('ds003483', dataset.name)
+
+            entities = dataset.query_entities()
+            self.assertEqual(21, len(entities["subject"]))
+            suffixes = dataset.query(target="suffixes")
+            self.assertEqual(['channels', 'coordsystem', 'events', 'meg', 'scans'], suffixes)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ancpbids-0.2.1/tests/auto/test_query.py` & `ancpbids-0.2.2/tests/auto/test_query.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,102 +2,106 @@
 
 import ancpbids
 from ancpbids import select, re, any_of, all_of, eq, op, entity
 from ..base_test_case import *
 
 
 class QueryTestCase(BaseTestCase):
-    def test_bidslayout_entities_formatting(self):
-        layout = ancpbids.BIDSLayout(ENTITIES_DIR)
-        files = layout.get(sub='02', run='3', return_type='filename')
+    def test_entities_formatting(self):
+        layout = ancpbids.load_dataset(ENTITIES_DIR)
+        files = layout.query(sub='02', run='3', return_type='filename')
         self.assertEqual(1, len(files))
         self.assertTrue(files[0].endswith("sub-02_task-abc_run-00003_events.tsv"))
 
-        files = layout.get(sub='02', run=['000000003'], return_type='filename')
+        files = layout.query(sub='02', run=['000000003'], return_type='filename')
         self.assertEqual(1, len(files))
         self.assertTrue(files[0].endswith("sub-02_task-abc_run-00003_events.tsv"))
 
         # should also handle invalid formats, i.e. run not as an index but a label
-        files = layout.get(sub='02', run='xyz', return_type='filename')
+        files = layout.query(sub='02', run='xyz', return_type='filename')
         self.assertEqual(1, len(files))
         self.assertTrue(files[0].endswith("sub-02_task-abc_run-xyz_events.tsv"))
 
     def test_bidslayout_entities_any(self):
-        layout = ancpbids.BIDSLayout(ENTITIES_DIR)
-        files = layout.get(sub='*', suffix='test', task='abc', return_type='filename')
+        layout = ancpbids.load_dataset(ENTITIES_DIR)
+        files = layout.query(sub='*', suffix='test', task='abc', return_type='filename')
         self.assertEqual(2, len(files))
         self.assertTrue(files[0].endswith("sub-bar_task-abc_test.txt"))
         self.assertTrue(files[1].endswith("sub-foo_task-abc_test.txt"))
 
     def test_bidslayout_subjects_filtered(self):
-        layout = ancpbids.BIDSLayout(ENTITIES_DIR)
-        subjects = layout.get_subjects(task='abc')
+        layout = ancpbids.load_dataset(ENTITIES_DIR)
+        subjects = layout.query(target="sub", task='abc')
         self.assertEqual(3, len(subjects))
         self.assertListEqual(['02', 'bar', 'foo'], subjects)
 
     def test_bidslayout(self):
-        layout = ancpbids.BIDSLayout(DS005_DIR)
+        layout = ancpbids.load_dataset(DS005_DIR)
+        ents = layout.query_entities()
 
-        subjects = layout.get_subjects()
-        subjects_expected = ['%02d' % i for i in range(1, 17)]
-        self.assertListEqual(subjects_expected, subjects)
+        subjects = ents["subject"]
+        subjects_expected = {'%02d' % i for i in range(1, 17)}
+        self.assertSetEqual(subjects_expected, subjects)
 
-        sessions = layout.get_sessions()
-        self.assertEqual(0, len(sessions))
+        self.assertNotIn("session", ents)
 
-        tasks = layout.get_tasks()
-        self.assertListEqual(['mixedgamblestask'], tasks)
+        tasks = ents["task"]
+        self.assertSetEqual({'mixedgamblestask'}, tasks)
 
     def test_bidslayout_get(self):
-        layout = ancpbids.BIDSLayout(SYNTHETIC_DIR)
-        mask_niftis = layout.get(scope='derivatives',
-                                 return_type='filename',
-                                 suffix='mask',
-                                 extension='.nii',
-                                 sub='03',
-                                 ses='02',
-                                 task='nback',
-                                 run=["01", "02"])
+        layout = ancpbids.load_dataset(SYNTHETIC_DIR)
+        mask_niftis = layout.query(scope='derivatives',
+                                   return_type='filename',
+                                   suffix='mask',
+                                   extension='.nii',
+                                   sub='03',
+                                   ses='02',
+                                   task='nback',
+                                   run=["01", "02"])
         self.assertEqual(4, len(mask_niftis))
         expected_paths = [
             'derivatives/fmriprep/sub-03/ses-02/func/sub-03_ses-02_task-nback_run-01_space-MNI152NLin2009cAsym_desc-brain_mask.nii',
             'derivatives/fmriprep/sub-03/ses-02/func/sub-03_ses-02_task-nback_run-01_space-T1w_desc-brain_mask.nii',
             'derivatives/fmriprep/sub-03/ses-02/func/sub-03_ses-02_task-nback_run-02_space-MNI152NLin2009cAsym_desc-brain_mask.nii',
             'derivatives/fmriprep/sub-03/ses-02/func/sub-03_ses-02_task-nback_run-02_space-T1w_desc-brain_mask.nii',
         ]
         expected_paths = list(map(lambda p: os.path.normpath(os.path.join(SYNTHETIC_DIR, p)), expected_paths))
         for file in expected_paths:
             self.assertTrue(list(filter(lambda p: file == p, mask_niftis)))
 
     def test_bidslayout_get_entities(self):
-        layout = ancpbids.BIDSLayout(DS005_DIR)
-        sorted_entities = layout.get_entities(scope='raw', sort=True)
+        layout = ancpbids.load_dataset(DS005_DIR)
+        sorted_entities = layout.query_entities(scope='raw', sort=True)
         # note: 'ds' and 'type' entities are contained in folder 'models' at dataset level, so considered raw data
-        self.assertListEqual(['ds', 'run', 'sub', 'task', 'type'], list(sorted_entities.keys()))
+        self.assertListEqual(['ds', 'run', 'subject', 'task', 'type'], list(sorted_entities.keys()))
         self.assertListEqual([1, 2, 3], sorted_entities['run'])
-        self.assertEqual(['%02d' % i for i in range(1, 17)], sorted_entities['sub'])
+        self.assertEqual(['%02d' % i for i in range(1, 17)], sorted_entities['subject'])
         self.assertListEqual(['mixedgamblestask'], sorted_entities['task'])
 
     def test_bidslayout_get_suffixes(self):
-        layout = ancpbids.BIDSLayout(DS005_DIR)
-        suffixes = layout.get_suffixes()
+        layout = ancpbids.load_dataset(DS005_DIR)
+        suffixes = layout.query(target="suffixe")
         self.assertListEqual(['T1w', 'bold', 'dwi', 'events', 'model'], suffixes)
 
     def test_bidslayout_get_extensions(self):
-        layout = ancpbids.BIDSLayout(DS005_DIR)
-        extensions = layout.get_extensions()
+        layout = ancpbids.load_dataset(DS005_DIR)
+        extensions = layout.query(target="extension")
         self.assertListEqual(['.json', '.nii.gz', '.tsv'], extensions)
 
     def test_bidslayout_get_metadata(self):
-        layout = ancpbids.BIDSLayout(DS005_DIR)
-        metadata = layout.get_metadata("sub-01/func/sub-01_task-mixedgamblestask_run-01_bold.nii.gz")
+        layout = ancpbids.load_dataset(DS005_DIR)
+        metadata = layout.get_file("sub-01/func/sub-01_task-mixedgamblestask_run-01_bold.nii.gz").get_metadata(
+            include_entities=True)
         self.assertTrue(isinstance(metadata, dict))
         self.assertEqual(2.0, metadata['RepetitionTime'])
         self.assertEqual('mixed-gambles task', metadata['TaskName'])
         self.assertListEqual([0.0, 0.0571, 0.1143, 0.1714, 0.2286, 0.2857], metadata['SliceTiming'])
+        self.assertEqual('01', metadata['subject'])
+        self.assertEqual('mixedgamblestask', metadata['task'])
+        self.assertEqual(1, metadata['run'])
 
     def test_query_language(self):
         ds = ancpbids.load_dataset(DS005_DIR)
         schema = ds.get_schema()
         file_paths = ds.select(schema.Artifact) \
             .where(all_of(eq(schema.Artifact.suffix, 'bold'),
                           entity(schema, schema.EntityEnum.subject, '02'))) \
```

### Comparing `ancpbids-0.2.1/tests/auto/test_regressions.py` & `ancpbids-0.2.2/tests/auto/test_regressions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import ancpbids
 from ..base_test_case import *
 
 
 class RegressionsTestCase(BaseTestCase):
     def test_get_all_files_from_pipeline(self):
-        layout = ancpbids.BIDSLayout(DS005_DIR)
-        all_derivative_files = layout.get(scope='derivatives/affine/matrix', return_type='file')
+        dataset = ancpbids.load_dataset(DS005_DIR)
+        all_derivative_files = dataset.query(scope='derivatives/affine/matrix', return_type='file')
         # that derivatives folder has no valid BIDS files (of type model.Artifact)
         # but ordinary files (if type model.File)
         self.assertEqual(16, len(all_derivative_files))
 
     def test_report_errors(self):
-        layout = ancpbids.BIDSLayout(DS005_DIR)
-        report = layout.validate()
+        dataset = ancpbids.load_dataset(DS005_DIR)
+        report = ancpbids.validate_dataset(dataset)
         self.assertTrue(report.has_errors())
 
     def test_get_entitites_no_scope(self):
-        layout = ancpbids.BIDSLayout(DS005_DIR)
-        entities = layout.get_entities(scope=None)
-        self.assertEqual(['ds', 'type', 'task', 'sub', 'run', 'desc'], list(entities.keys()))
+        dataset = ancpbids.load_dataset(DS005_DIR)
+        entities = dataset.query_entities(scope=None)
+        self.assertEqual(['ds', 'type', 'subject', 'task', 'run', 'description'], list(entities.keys()))
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ancpbids-0.2.1/tests/auto/test_schema.py` & `ancpbids-0.2.2/tests/auto/test_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from ancpbids import model_latest, model_v1_8_0, load_dataset, load_schema
+from ancpbids import model_v1_8_0, model_v1_8_0 as model_latest, load_dataset, load_schema
 from ..base_test_case import BaseTestCase, DS005_DIR, DS005_SMALL_DIR
 
 
 class SchemaTestCase(BaseTestCase):
     def test_entitmatching(self):
         self.assertEqual('sub', model_latest.fuzzy_match_entity_key('sub'))
         self.assertEqual('sub', model_latest.fuzzy_match_entity_key('subject'))
```

### Comparing `ancpbids-0.2.1/tests/auto/test_validation.py` & `ancpbids-0.2.2/tests/auto/test_validation.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.1/tests/auto/test_writing.py` & `ancpbids-0.2.2/tests/auto/test_writing.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,80 +6,89 @@
 import pandas as pd
 import shutil
 import tempfile
 
 from numpy.testing import tempdir
 
 import ancpbids
-from ancpbids import model, re
+from ancpbids import model_latest, re
 from ..base_test_case import BaseTestCase, DS005_DIR
 
 
 class WritingTestCase(BaseTestCase):
 
     def write_test_derivative(self):
-        layout = ancpbids.BIDSLayout(DS005_DIR)
-        dataset = layout.get_dataset()
+        dataset = ancpbids.load_dataset(DS005_DIR)
         pipeline_name = "mypipeline-%d" % time.time()
         derivative = dataset.create_derivative(name=pipeline_name)
         derivative.dataset_description.GeneratedBy.Name = "My Test Pipeline"
-        task_label = layout.get_tasks()[0]
+        ents = dataset.query_entities()
+        task_label = list(ents['task'])[0]
 
-        for sub_label in layout.get_subjects():
+        for sub_label in ents["subject"]:
             subject = derivative.create_folder(name='sub-' + sub_label)
             # create an additional folder level to increase complexity of generation
             session = subject.create_folder(name='ses-01')
 
             # do some complex task
             # ... doing complex task ...
             # ... done
             txt_artifact = session.create_artifact()
-            txt_artifact.add_entity("desc", "mypipeline")
+            txt_artifact.add_entities(desc="mypipeline", run=1, sub=sub_label)
             txt_artifact.suffix = 'textual'
             txt_artifact.extension = ".txt"
             txt_artifact.content = "Subject %s participated in task %s" % (sub_label, task_label)
 
             # create some random data
             df = pd.DataFrame(np.random.randint(0, 100, size=(100, 4)), columns=list('ABCD'))
             ev_artifact = session.create_artifact()
-            ev_artifact.add_entity("desc", "mypipeline")
+            ev_artifact.add_entities(desc="mypipeline", run=1, sub=sub_label)
             ev_artifact.suffix = 'events'
             ev_artifact.extension = ".tsv"
             # at this point, the file path is not known and will be provided
             # to lambda when the derivative is written to disk
             ev_artifact.content = lambda file_path, df=df: df.to_csv(file_path, index=None)
 
-        layout.write_derivative(derivative)
+        ancpbids.write_derivative(dataset, derivative)
         return DS005_DIR, pipeline_name
 
     def test_write_derivative(self):
         # create a temporary dataset with a test derivative and return its root path and the created derivative
         ds_path, pipeline_name = self.write_test_derivative()
         # pretend loading a new dataset
-        layout = ancpbids.BIDSLayout(ds_path)
+        dataset = ancpbids.load_dataset(ds_path)
         # get the underlying graph/dataset for further inspection
-        dataset = layout.get_dataset()
         derivative_folder = filter(lambda f: f.name == pipeline_name, dataset.derivatives.folders)
         self.assertIsNotNone(derivative_folder)
         derivative_folder = next(derivative_folder)
         schema = dataset.get_schema()
         subjects = derivative_folder.select(schema.Folder) \
             .where(re(schema.Folder.name, r"sub-[\d]+")) \
             .objects(True)
         self.assertEqual(16, len(subjects))
 
         for i, subject in enumerate(subjects):
-            exptected_sub_name = "sub-%02d" % (i + 1)
-            self.assertEqual(exptected_sub_name, subject.name)
-            for artifact in subject.files:
-                # check if 'sub' entity has been automatically added as it is inferrable from its parent directory
-                self.assertEqual(exptected_sub_name, "sub-%s" % artifact.get_entity('sub'))
+            sub_label = "%02d" % (i + 1)
+            expected_sub_name = "sub-%s" % sub_label
+            self.assertEqual(expected_sub_name, subject.name)
+
+            expected_ses_name = "ses-01"
+            self.assertEqual(expected_ses_name, subject.folders[0].name)
+
+            ses_folder = subject.folders[0]
+            for artifact in ses_folder.files:
+                ents = artifact.get_entities()
+                self.assertEqual(
+                    "{'sub': '%s', 'ses': '01', 'run': 1, 'desc': 'mypipeline'}" % (sub_label),
+                    str(ents))
+                self.assertTrue(artifact.name.startswith('sub-%s_ses-01_run-1_desc-mypipeline_' % sub_label))
 
         self.assertTrue(isinstance(derivative_folder.dataset_description, schema.DerivativeDatasetDescriptionFile))
         self.assertEqual(derivative_folder.dataset_description.GeneratedBy.Name, "My Test Pipeline")
+        shutil.rmtree(derivative_folder.get_absolute_path())
 
     def test_create_new_dataset(self):
         from ancpbids import model_latest as schema
         dataset = schema.create_dataset(name='my-test-ds')
         dataset.dataset_description.Name = 'a programmatically created dataset'
         dataset.dataset_description.BIDSVersion = schema.VERSION
```

### Comparing `ancpbids-0.2.1/tests/manual/test_benchmark.py` & `ancpbids-0.2.2/tests/manual/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.1/versioneer.py` & `ancpbids-0.2.2/versioneer.py`

 * *Files identical despite different names*

