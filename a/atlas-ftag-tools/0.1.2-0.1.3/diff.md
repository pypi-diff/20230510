# Comparing `tmp/atlas-ftag-tools-0.1.2.tar.gz` & `tmp/atlas-ftag-tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlas-ftag-tools-0.1.2.tar", last modified: Wed Apr 26 11:03:09 2023, max compression
+gzip compressed data, was "atlas-ftag-tools-0.1.3.tar", last modified: Wed May 10 10:04:11 2023, max compression
```

## Comparing `atlas-ftag-tools-0.1.2.tar` & `atlas-ftag-tools-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:03:09.649164 atlas-ftag-tools-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-26 11:03:09.649164 atlas-ftag-tools-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:03:09.645164 atlas-ftag-tools-0.1.2/atlas_ftag_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-26 11:03:09.000000 atlas-ftag-tools-0.1.2/atlas_ftag_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-26 11:03:09.000000 atlas-ftag-tools-0.1.2/atlas_ftag_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:03:09.000000 atlas-ftag-tools-0.1.2/atlas_ftag_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-26 11:03:09.000000 atlas-ftag-tools-0.1.2/atlas_ftag_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-26 11:03:09.000000 atlas-ftag-tools-0.1.2/atlas_ftag_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-26 11:03:09.000000 atlas-ftag-tools-0.1.2/atlas_ftag_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:03:09.645164 atlas-ftag-tools-0.1.2/ftag/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/cuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/flavour.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/flavours.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:03:09.645164 atlas-ftag-tools-0.1.2/ftag/hdf5/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/hdf5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/hdf5/h5reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/hdf5/h5utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/hdf5/h5writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/vds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:03:09.645164 atlas-ftag-tools-0.1.2/ftag/wps/
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/wps/discriminant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/wps/working_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 11:03:09.649164 atlas-ftag-tools-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:04:11.926552 atlas-ftag-tools-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-10 10:04:11.926552 atlas-ftag-tools-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:04:11.922552 atlas-ftag-tools-0.1.3/atlas_ftag_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-10 10:04:11.000000 atlas-ftag-tools-0.1.3/atlas_ftag_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-10 10:04:11.000000 atlas-ftag-tools-0.1.3/atlas_ftag_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 10:04:11.000000 atlas-ftag-tools-0.1.3/atlas_ftag_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-10 10:04:11.000000 atlas-ftag-tools-0.1.3/atlas_ftag_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-10 10:04:11.000000 atlas-ftag-tools-0.1.3/atlas_ftag_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-10 10:04:11.000000 atlas-ftag-tools-0.1.3/atlas_ftag_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:04:11.926552 atlas-ftag-tools-0.1.3/ftag/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/cuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/flavour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/flavours.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:04:11.926552 atlas-ftag-tools-0.1.3/ftag/hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/hdf5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/hdf5/h5reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/hdf5/h5utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/hdf5/h5writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/vds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:04:11.926552 atlas-ftag-tools-0.1.3/ftag/wps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/wps/discriminant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/ftag/wps/working_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-10 10:03:48.000000 atlas-ftag-tools-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 10:04:11.926552 atlas-ftag-tools-0.1.3/setup.cfg
```

### Comparing `atlas-ftag-tools-0.1.2/PKG-INFO` & `atlas-ftag-tools-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-ftag-tools
-Version: 0.1.2
+Version: 0.1.3
 Summary: ATLAS Flavour Tagging Tools
 Author: Sam Van Stroud, Philipp Gadow
 License: MIT
 Project-URL: Homepage, https://github.com/umami-hep/atlas-ftag-tools/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -15,37 +15,59 @@
 
 # ATLAS FTAG Python Tools
 
 This is a collection of Python tools for working with files produced with the FTAG [ntuple dumper](https://gitlab.cern.ch/atlas-flavor-tagging-tools/training-dataset-dumper/).
 The code is intended to be used a [library](https://iscinumpy.dev/post/app-vs-library/) for other projects.
 Please see the [example notebook](ftag/example.ipynb) for usage.
 
+# Quickstart 
+
 ## Installation
 
-To install the package you can install from pip using the [release on pypi](https://pypi.org/project/atlas-ftag-tools/) via
+If you want to use this package without modification, you can install from [pypi](https://pypi.org/project/atlas-ftag-tools/) using `pip`.
 
 ```bash
 pip install atlas-ftag-tools
 ```
 
-or you can clone the repository and install in editable mode with
+To additionally install the development dependencies (for formatting and linting) rn
 ```bash
-python -m pip install -e .
+pip install atlas-ftag-tools[dev]
 ```
 
-To install optional development dependencies (for formatting and linting) you can instead install with either from pip
+## Development
+
+If you plan on making changes to teh code, instead clone the repository and install the package from source in editable mode with
+
 ```bash
-pip install atlas-ftag-tools[dev]
+python -m pip install -e .
 ```
 
-or from source
+Include development dependencies with
+
 ```bash
 python -m pip install -e ".[dev]"
 ```
 
+You can set up pre-commit hooks with
+
+```bash
+pre-commit install
+```
+
+To run the tests you can use the `pytest` or `coverage` command, for example
+
+```bash
+coverage run --source ftag -m pytest --show-capture=stdout
+```
+
+Running `coverage report` will display the test coverage.
+
+
+# Usage
 
 ## Create virtual file
 
 This package contains a script to easily merge a set of H5 files.
 A virtual file is a fast and lightweight way to wrap a set of files.
 See the [h5py documentation](https://docs.h5py.org/en/stable/vds.html) for more information on virtual datasets.
 
@@ -53,14 +75,16 @@
 
 ```
 vds <pattern> <output path>
 ```
 
 The `<pattern>` argument should be a quotes enclosed [glob pattern](https://en.wikipedia.org/wiki/Glob_(programming)), for example `"dsid/path/*.h5"`
 
+See `vds --help` for more options and information.
+
 
 ## Calculate WPs
 
 This package contains a script to calculate tagger working points (WPs).
 The script is `working_points.py` and can be run after installing this package with
 
 ```
@@ -75,19 +99,10 @@
 If you want to use the `ttbar` WPs get the efficiencies and rejections for the `zprime` sample, you can add `--zprime "path/to/zprime/*.h5"` to the command.
 Note that a default selection of $p_T > 250 ~GeV$ to jets in the `zprime` sample.
 
 If instead of defining the working points for a series of signal efficiencies, you wish to calculate a WP corresponding to a specific background rejection, the `--rejection` option can be given along with the desired background.
 
 By default the working points are printed to the terminal, but you can save the results to a YAML file with the `--outfile` option.
 
-Use `--help` for more options and information.
-
+See `wps --help` for more options and information.
 
-## Tests
 
-To run the tests you can use the `pytest` or `coverage` command, for example
-
-```bash
-coverage run --source ftag -m pytest --show-capture=stdout
-```
-
-Running `coverage report` will display the test coverage.
```

### Comparing `atlas-ftag-tools-0.1.2/README.md` & `atlas-ftag-tools-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,37 +4,59 @@
 
 # ATLAS FTAG Python Tools
 
 This is a collection of Python tools for working with files produced with the FTAG [ntuple dumper](https://gitlab.cern.ch/atlas-flavor-tagging-tools/training-dataset-dumper/).
 The code is intended to be used a [library](https://iscinumpy.dev/post/app-vs-library/) for other projects.
 Please see the [example notebook](ftag/example.ipynb) for usage.
 
+# Quickstart 
+
 ## Installation
 
-To install the package you can install from pip using the [release on pypi](https://pypi.org/project/atlas-ftag-tools/) via
+If you want to use this package without modification, you can install from [pypi](https://pypi.org/project/atlas-ftag-tools/) using `pip`.
 
 ```bash
 pip install atlas-ftag-tools
 ```
 
-or you can clone the repository and install in editable mode with
+To additionally install the development dependencies (for formatting and linting) rn
 ```bash
-python -m pip install -e .
+pip install atlas-ftag-tools[dev]
 ```
 
-To install optional development dependencies (for formatting and linting) you can instead install with either from pip
+## Development
+
+If you plan on making changes to teh code, instead clone the repository and install the package from source in editable mode with
+
 ```bash
-pip install atlas-ftag-tools[dev]
+python -m pip install -e .
 ```
 
-or from source
+Include development dependencies with
+
 ```bash
 python -m pip install -e ".[dev]"
 ```
 
+You can set up pre-commit hooks with
+
+```bash
+pre-commit install
+```
+
+To run the tests you can use the `pytest` or `coverage` command, for example
+
+```bash
+coverage run --source ftag -m pytest --show-capture=stdout
+```
+
+Running `coverage report` will display the test coverage.
+
+
+# Usage
 
 ## Create virtual file
 
 This package contains a script to easily merge a set of H5 files.
 A virtual file is a fast and lightweight way to wrap a set of files.
 See the [h5py documentation](https://docs.h5py.org/en/stable/vds.html) for more information on virtual datasets.
 
@@ -42,14 +64,16 @@
 
 ```
 vds <pattern> <output path>
 ```
 
 The `<pattern>` argument should be a quotes enclosed [glob pattern](https://en.wikipedia.org/wiki/Glob_(programming)), for example `"dsid/path/*.h5"`
 
+See `vds --help` for more options and information.
+
 
 ## Calculate WPs
 
 This package contains a script to calculate tagger working points (WPs).
 The script is `working_points.py` and can be run after installing this package with
 
 ```
@@ -64,19 +88,10 @@
 If you want to use the `ttbar` WPs get the efficiencies and rejections for the `zprime` sample, you can add `--zprime "path/to/zprime/*.h5"` to the command.
 Note that a default selection of $p_T > 250 ~GeV$ to jets in the `zprime` sample.
 
 If instead of defining the working points for a series of signal efficiencies, you wish to calculate a WP corresponding to a specific background rejection, the `--rejection` option can be given along with the desired background.
 
 By default the working points are printed to the terminal, but you can save the results to a YAML file with the `--outfile` option.
 
-Use `--help` for more options and information.
-
+See `wps --help` for more options and information.
 
-## Tests
 
-To run the tests you can use the `pytest` or `coverage` command, for example
-
-```bash
-coverage run --source ftag -m pytest --show-capture=stdout
-```
-
-Running `coverage report` will display the test coverage.
```

### Comparing `atlas-ftag-tools-0.1.2/atlas_ftag_tools.egg-info/PKG-INFO` & `atlas-ftag-tools-0.1.3/atlas_ftag_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-ftag-tools
-Version: 0.1.2
+Version: 0.1.3
 Summary: ATLAS Flavour Tagging Tools
 Author: Sam Van Stroud, Philipp Gadow
 License: MIT
 Project-URL: Homepage, https://github.com/umami-hep/atlas-ftag-tools/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -15,37 +15,59 @@
 
 # ATLAS FTAG Python Tools
 
 This is a collection of Python tools for working with files produced with the FTAG [ntuple dumper](https://gitlab.cern.ch/atlas-flavor-tagging-tools/training-dataset-dumper/).
 The code is intended to be used a [library](https://iscinumpy.dev/post/app-vs-library/) for other projects.
 Please see the [example notebook](ftag/example.ipynb) for usage.
 
+# Quickstart 
+
 ## Installation
 
-To install the package you can install from pip using the [release on pypi](https://pypi.org/project/atlas-ftag-tools/) via
+If you want to use this package without modification, you can install from [pypi](https://pypi.org/project/atlas-ftag-tools/) using `pip`.
 
 ```bash
 pip install atlas-ftag-tools
 ```
 
-or you can clone the repository and install in editable mode with
+To additionally install the development dependencies (for formatting and linting) rn
 ```bash
-python -m pip install -e .
+pip install atlas-ftag-tools[dev]
 ```
 
-To install optional development dependencies (for formatting and linting) you can instead install with either from pip
+## Development
+
+If you plan on making changes to teh code, instead clone the repository and install the package from source in editable mode with
+
 ```bash
-pip install atlas-ftag-tools[dev]
+python -m pip install -e .
 ```
 
-or from source
+Include development dependencies with
+
 ```bash
 python -m pip install -e ".[dev]"
 ```
 
+You can set up pre-commit hooks with
+
+```bash
+pre-commit install
+```
+
+To run the tests you can use the `pytest` or `coverage` command, for example
+
+```bash
+coverage run --source ftag -m pytest --show-capture=stdout
+```
+
+Running `coverage report` will display the test coverage.
+
+
+# Usage
 
 ## Create virtual file
 
 This package contains a script to easily merge a set of H5 files.
 A virtual file is a fast and lightweight way to wrap a set of files.
 See the [h5py documentation](https://docs.h5py.org/en/stable/vds.html) for more information on virtual datasets.
 
@@ -53,14 +75,16 @@
 
 ```
 vds <pattern> <output path>
 ```
 
 The `<pattern>` argument should be a quotes enclosed [glob pattern](https://en.wikipedia.org/wiki/Glob_(programming)), for example `"dsid/path/*.h5"`
 
+See `vds --help` for more options and information.
+
 
 ## Calculate WPs
 
 This package contains a script to calculate tagger working points (WPs).
 The script is `working_points.py` and can be run after installing this package with
 
 ```
@@ -75,19 +99,10 @@
 If you want to use the `ttbar` WPs get the efficiencies and rejections for the `zprime` sample, you can add `--zprime "path/to/zprime/*.h5"` to the command.
 Note that a default selection of $p_T > 250 ~GeV$ to jets in the `zprime` sample.
 
 If instead of defining the working points for a series of signal efficiencies, you wish to calculate a WP corresponding to a specific background rejection, the `--rejection` option can be given along with the desired background.
 
 By default the working points are printed to the terminal, but you can save the results to a YAML file with the `--outfile` option.
 
-Use `--help` for more options and information.
-
+See `wps --help` for more options and information.
 
-## Tests
 
-To run the tests you can use the `pytest` or `coverage` command, for example
-
-```bash
-coverage run --source ftag -m pytest --show-capture=stdout
-```
-
-Running `coverage report` will display the test coverage.
```

### Comparing `atlas-ftag-tools-0.1.2/atlas_ftag_tools.egg-info/SOURCES.txt` & `atlas-ftag-tools-0.1.3/atlas_ftag_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.2/ftag/__init__.py` & `atlas-ftag-tools-0.1.3/ftag/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """atlas-ftag-tools - Common tools for ATLAS flavour tagging software."""
 
 
-__version__ = "v0.1.2"
+__version__ = "v0.1.3"
 
 
 import ftag.hdf5 as hdf5
 from ftag.cuts import Cuts
 from ftag.flavour import Flavour, Flavours
 from ftag.mock import get_mock_file
 from ftag.sample import Sample
```

### Comparing `atlas-ftag-tools-0.1.2/ftag/cuts.py` & `atlas-ftag-tools-0.1.3/ftag/cuts.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.2/ftag/flavour.py` & `atlas-ftag-tools-0.1.3/ftag/flavour.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.2/ftag/flavours.yaml` & `atlas-ftag-tools-0.1.3/ftag/flavours.yaml`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.2/ftag/hdf5/h5reader.py` & `atlas-ftag-tools-0.1.3/ftag/hdf5/h5reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,17 @@
     jets_name: str = "jets"
     precision: str | None = None
     shuffle: bool = True
     do_remove_inf: bool = False
 
     def __post_init__(self) -> None:
         self.sample = Sample(self.fname)
-        self.fname = self.sample.virtual_file()
+        if len(self.sample.virtual_file()) != 1:
+            raise ValueError("H5SingleReader should only read a single file")
+        self.fname = self.sample.virtual_file()[0]
 
     @cached_property
     def num_jets(self) -> int:
         with h5py.File(self.fname) as f:
             return len(f[self.jets_name])
 
     def get_attr(self, name, group=None):
```

### Comparing `atlas-ftag-tools-0.1.2/ftag/hdf5/h5utils.py` & `atlas-ftag-tools-0.1.3/ftag/hdf5/h5utils.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.2/ftag/hdf5/h5writer.py` & `atlas-ftag-tools-0.1.3/ftag/hdf5/h5writer.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.2/ftag/mock.py` & `atlas-ftag-tools-0.1.3/ftag/mock.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.2/ftag/sample.py` & `atlas-ftag-tools-0.1.3/ftag/sample.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,35 +6,39 @@
 
 from ftag.flavour import remove_suffix
 from ftag.vds import create_virtual_file
 
 
 @dataclass(frozen=True)
 class Sample:
-    pattern: Path | str
+    pattern: Path | str | tuple[Path | str, ...]
     ntuple_dir: Path | str | None = None
     name: str | None = None
 
     def __post_init__(self) -> None:
         if not self.pattern:
             raise ValueError("Sample pattern cannot be empty")
         if "*" in str(self.pattern) and not self.files:
             raise FileNotFoundError(f"No files matched pattern {self.pattern}")
         if missing := [file for file in self.files if not Path(file).is_file()]:
             raise FileNotFoundError(f"The following files do not exist: {missing}")
 
     @property
-    def path(self) -> Path:
+    def path(self) -> tuple[Path, ...]:
+        pattern_tuple = self.pattern if isinstance(self.pattern, (list, tuple)) else (self.pattern,)
         if self.ntuple_dir is not None:
-            return Path(self.ntuple_dir, self.pattern)
-        return Path(self.pattern)
+            return tuple(Path(self.ntuple_dir, p) for p in pattern_tuple)
+        return tuple(Path(p) for p in pattern_tuple)
 
     @property
     def files(self) -> list[str]:
-        return glob.glob(str(self.path)) if "*" in str(self.path) else [str(self.path)]
+        files = []
+        for p in self.path:
+            files += glob.glob(str(p)) if "*" in str(p) else [str(p)]
+        return files
 
     @property
     def num_files(self) -> int:
         return len(self.files)
 
     @property
     def dsid(self) -> list[str]:
@@ -57,18 +61,19 @@
         return list(set([tag for tags in self.tags for tag in tags.split("_") if "r" in tag]))
 
     @property
     def dumper_tag(self) -> list[str]:
         hashes = [remove_suffix(dsid.split(".")[7], "_output") for dsid in self.dsid]
         return list(set(hashes))
 
-    def virtual_file(self, **kwargs) -> Path | str:
-        if "*" in str(self.path):
-            return create_virtual_file(self.path, **kwargs)
-        return self.path
+    def virtual_file(self, **kwargs) -> list[Path | str]:
+        virtual_file_paths = []
+        for p in self.path:
+            virtual_file_paths.append(create_virtual_file(p, **kwargs) if "*" in str(p) else p)
+        return virtual_file_paths
 
     def __str__(self):
         return self.name
 
     def __lt__(self, other):
         return self.name < other.name
```

### Comparing `atlas-ftag-tools-0.1.2/ftag/vds.py` & `atlas-ftag-tools-0.1.3/ftag/vds.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.2/ftag/wps/discriminant.py` & `atlas-ftag-tools-0.1.3/ftag/wps/discriminant.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import numpy as np
 
 from ftag.flavour import Flavour, Flavours
 
 
 def btag_discriminant(pb, pc, pu, fc=0.1, epsilon=1e-10):
     return np.log((pb + epsilon) / ((1.0 - fc) * pu + fc * pc + epsilon))
```

### Comparing `atlas-ftag-tools-0.1.2/ftag/wps/working_points.py` & `atlas-ftag-tools-0.1.3/ftag/wps/working_points.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.2/pyproject.toml` & `atlas-ftag-tools-0.1.3/pyproject.toml`

 * *Files identical despite different names*

