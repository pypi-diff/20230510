# Comparing `tmp/toffy-0.1.2.tar.gz` & `tmp/toffy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toffy-0.1.2.tar", max compression
+gzip compressed data, was "toffy-0.2.0.tar", max compression
```

## Comparing `toffy-0.1.2.tar` & `toffy-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11640 2023-03-21 20:19:13.919172 toffy-0.1.2/LICENSE
--rw-r--r--   0        0        0    17763 2023-03-21 20:19:13.919172 toffy-0.1.2/README.md
--rw-r--r--   0        0        0     2798 2023-03-21 20:23:35.098016 toffy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-21 20:19:13.943174 toffy-0.1.2/src/toffy/__init__.py
--rw-r--r--   0        0        0     2559 2023-03-21 20:19:13.943174 toffy-0.1.2/src/toffy/bin_extraction.py
--rw-r--r--   0        0        0     2302 2023-03-21 20:19:13.943174 toffy-0.1.2/src/toffy/detector_sweep.py
--rw-r--r--   0        0        0     2203 2023-03-21 20:19:13.943174 toffy-0.1.2/src/toffy/file_hash.py
--rw-r--r--   0        0        0    11116 2023-03-21 20:19:13.943174 toffy-0.1.2/src/toffy/fov_watcher.py
--rw-r--r--   0        0        0     7059 2023-03-21 20:19:13.943174 toffy-0.1.2/src/toffy/image_stitching.py
--rw-r--r--   0        0        0     6053 2023-03-21 20:19:13.943174 toffy-0.1.2/src/toffy/json_utils.py
--rw-r--r--   0        0        0    12822 2023-03-21 20:19:13.943174 toffy-0.1.2/src/toffy/mibitracker_utils.py
--rw-r--r--   0        0        0     6537 2023-03-21 20:19:13.943174 toffy-0.1.2/src/toffy/mph_comp.py
--rw-r--r--   0        0        0     4164 2023-03-21 20:19:13.943174 toffy-0.1.2/src/toffy/mph_inspect.py
--rw-r--r--   0        0        0    30529 2023-03-21 20:19:13.943174 toffy-0.1.2/src/toffy/normalize.py
--rw-r--r--   0        0        0     7411 2023-03-21 20:19:13.943174 toffy-0.1.2/src/toffy/panel_utils.py
--rw-r--r--   0        0        0    20234 2023-03-21 20:19:13.943174 toffy-0.1.2/src/toffy/qc_comp.py
--rw-r--r--   0        0        0     2948 2023-03-21 20:19:13.943174 toffy-0.1.2/src/toffy/qc_metrics_plots.py
--rw-r--r--   0        0        0     6246 2023-03-21 20:19:13.943174 toffy-0.1.2/src/toffy/reorg.py
--rw-r--r--   0        0        0    28519 2023-03-21 20:19:13.943174 toffy-0.1.2/src/toffy/rosetta.py
--rw-r--r--   0        0        0     1473 2023-03-21 20:19:13.943174 toffy-0.1.2/src/toffy/settings.py
--rw-r--r--   0        0        0    18199 2023-03-21 20:19:13.943174 toffy-0.1.2/src/toffy/streak_detection.py
--rw-r--r--   0        0        0    82064 2023-03-21 20:19:13.943174 toffy-0.1.2/src/toffy/tiling_utils.py
--rw-r--r--   0        0        0    13936 2023-03-21 20:19:13.943174 toffy-0.1.2/src/toffy/watcher_callbacks.py
--rw-r--r--   0        0        0    19059 1970-01-01 00:00:00.000000 toffy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11640 2023-05-10 17:47:35.860828 toffy-0.2.0/LICENSE
+-rw-r--r--   0        0        0    19122 2023-05-10 17:47:35.860828 toffy-0.2.0/README.md
+-rw-r--r--   0        0        0     2920 2023-05-10 17:48:08.572925 toffy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-10 17:47:35.888828 toffy-0.2.0/src/toffy/__init__.py
+-rw-r--r--   0        0        0     2559 2023-05-10 17:47:35.888828 toffy-0.2.0/src/toffy/bin_extraction.py
+-rw-r--r--   0        0        0     2302 2023-05-10 17:47:35.888828 toffy-0.2.0/src/toffy/detector_sweep.py
+-rw-r--r--   0        0        0     2203 2023-05-10 17:47:35.888828 toffy-0.2.0/src/toffy/file_hash.py
+-rw-r--r--   0        0        0    11622 2023-05-10 17:47:35.888828 toffy-0.2.0/src/toffy/fov_watcher.py
+-rw-r--r--   0        0        0     8109 2023-05-10 17:47:35.888828 toffy-0.2.0/src/toffy/image_stitching.py
+-rw-r--r--   0        0        0     6053 2023-05-10 17:47:35.888828 toffy-0.2.0/src/toffy/json_utils.py
+-rw-r--r--   0        0        0    12822 2023-05-10 17:47:35.888828 toffy-0.2.0/src/toffy/mibitracker_utils.py
+-rw-r--r--   0        0        0     6687 2023-05-10 17:47:35.888828 toffy-0.2.0/src/toffy/mph_comp.py
+-rw-r--r--   0        0        0     4164 2023-05-10 17:47:35.888828 toffy-0.2.0/src/toffy/mph_inspect.py
+-rw-r--r--   0        0        0    31476 2023-05-10 17:47:35.888828 toffy-0.2.0/src/toffy/normalize.py
+-rw-r--r--   0        0        0     7411 2023-05-10 17:47:35.888828 toffy-0.2.0/src/toffy/panel_utils.py
+-rw-r--r--   0        0        0    20234 2023-05-10 17:47:35.888828 toffy-0.2.0/src/toffy/qc_comp.py
+-rw-r--r--   0        0        0     2948 2023-05-10 17:47:35.888828 toffy-0.2.0/src/toffy/qc_metrics_plots.py
+-rw-r--r--   0        0        0     6246 2023-05-10 17:47:35.888828 toffy-0.2.0/src/toffy/reorg.py
+-rw-r--r--   0        0        0    28519 2023-05-10 17:47:35.888828 toffy-0.2.0/src/toffy/rosetta.py
+-rw-r--r--   0        0        0     1473 2023-05-10 17:47:35.888828 toffy-0.2.0/src/toffy/settings.py
+-rw-r--r--   0        0        0    18199 2023-05-10 17:47:35.888828 toffy-0.2.0/src/toffy/streak_detection.py
+-rw-r--r--   0        0        0    82064 2023-05-10 17:47:35.888828 toffy-0.2.0/src/toffy/tiling_utils.py
+-rw-r--r--   0        0        0    14450 2023-05-10 17:47:35.888828 toffy-0.2.0/src/toffy/watcher_callbacks.py
+-rw-r--r--   0        0        0    20487 1970-01-01 00:00:00.000000 toffy-0.2.0/PKG-INFO
```

### Comparing `toffy-0.1.2/LICENSE` & `toffy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toffy-0.1.2/README.md` & `toffy-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,80 @@
+Metadata-Version: 2.1
+Name: toffy
+Version: 0.2.0
+Summary: Scripts for interacting with and generating data from the commercial MIBIScope.
+Home-page: https://github.com/angelolab/toffy
+License: Modified Apache 2.0
+Author: Noah Frey Greenwald
+Author-email: nfgreen@stanford.edu
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: alpineer (==0.1.7)
+Requires-Dist: ipywidgets (>=8,<9)
+Requires-Dist: mibi-bin-tools (==0.2.9)
+Requires-Dist: natsort (>=8,<9)
+Requires-Dist: numpy (>=1.0.0,<2.0.0)
+Requires-Dist: pandas (>=1,<2)
+Requires-Dist: scikit-learn (>=1,<2)
+Requires-Dist: seaborn (>=0.12,<0.13)
+Requires-Dist: tqdm (>=4,<5)
+Requires-Dist: watchdog (>=3,<4)
+Project-URL: Documentation, https://toffy.readthedocs.io
+Project-URL: Repository, https://github.com/angelolab/toffy
+Description-Content-Type: text/markdown
+
 # toffy
+
+<div align="center">
+
+| | |
+| ---        |    ---  |
+| CI / CD | [![CI](https://github.com/angelolab/toffy/actions/workflows/ci.yml/badge.svg)](https://github.com/angelolab/toffy/actions/workflows/ci.yml) [![Coverage Status](https://coveralls.io/repos/github/angelolab/toffy/badge.svg?branch=main)](https://coveralls.io/github/angelolab/mibi-bin-tools?branch=main) |
+| Package | [![PyPI - Version](https://img.shields.io/pypi/v/toffy.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/toffy/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/toffy.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold)](https://pypi.org/project/toffy/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/toffy.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/toffy/) |
+|Meta | [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![PyPI - License](https://img.shields.io/pypi/l/toffy?color=9400d3)](LICENSE) |
+</div>
+
+
 The toffy repo is designed to simplify the process of generating and processing data on the MIBIScope platform.
 
-This repo is currently in beta testing. None of the code has been published yet, and we will be making breaking changes frequently. If you find bugs, please [open an issue](https://github.com/angelolab/toffy/issues/new/choose). If you have questions or want to collaborate, please reach out to Noah (nfgreen@stanford.edu)
+This repo is currently in beta testing. None of the code has been published yet, and we will be making breaking changes frequently. If you find bugs, please [open an issue](https://github.com/angelolab/toffy/issues/new/choose).
 
 ## Table of Contents
 - [Overview](#overview)
   - [1. Using toffy for the first time](#1-using-toffy-for-the-first-time)
   - [2. Setting up a MIBI run](#2-setting-up-a-mibi-run)
   - [3. Evaluating a MIBI run](#3-evaluating-a-mibi-run)
-  - [4. Processing data after a MIBI run](#4-processing-mibi-data)
-  - [5. Formatting data for downstream analysis](#5-formatting-mibi-runs-for-analysis)
+  - [4. Processing After a MIBI run](#4-processing-after-a-mibi-run)
+  - [5. Formatting MIBI Data for Downstream Analysis](#5-formatting-mibi-data-for-downstream-analysis)
+- [Pipeline Flowchart](#pipeline-flowchart)
 - [Installation](#installation)
   - [Requirements for specific operating systems](#requirements-for-specific-operating-systems)
     - [Windows](#windows)
     - [macOS](#macos)
   - [Setting up the virtual environment](#setting-up-the-virtual-environment)
   - [Using the repo](#using-the-repo)
   - [Updating the repo](#updating-the-repo)
 - [Directory structure](#directory-structure)
 - [Panel format](#panel-format)
 - [Median Pulse Height](#median-pulse-height)
+- [Development Notes](#development-notes)
+  - [Requirements](#requirements)
+  - [Setup](#setup)
 - [Questions?](#questions)
+- [How to cite](#how-to-cite)
 
 ## Overview
 The repo has four main parts, with associated code and jupyter notebooks for each.
 We have also recorded workshop talks which complement the repository. [MIBI Workshop (Pre-Recorded Lectures) Playlist](https://www.youtube.com/playlist?list=PLjNbkEm4vA27f8-EB7q9u_lDPI7oxohhn).
 
 ### 1. Using toffy for the first time
 The first time you use toffy on one of the commercial instruments, you'll need to perform some basic tasks to ensure everything is working properly. The [set up](./templates/1_set_up_toffy.ipynb) jupyter notebook will guide you through this process and the resulting directory structure is explained below ([directory structure](#directory-structure)).
@@ -46,20 +96,20 @@
 - 3b - 3e: post-run monitoring. For each step in the monitoring notebook, we have a dedicated notebook that can perform the same tasks once a run is complete.
 For more information, see the [image processing and extraction walkthrough](https://www.youtube.com/watch?v=QSzjW-cuZtg&list=PLjNbkEm4vA27f8-EB7q9u_lDPI7oxohhn&index=3).
   - 3b: [image extraction notebook](./templates/3b_extract_images_from_bin.ipynb) will extract images from bin files that have not already been processed
   - 3c: [qc metrics notebook](./templates/3c_generate_qc_metrics.ipynb) computes and visualizes the QC metrics for the images
   - 3d: [median pulse heights notebook](./templates/3d_compute_median_pulse_height.ipynb) generates plots showing median pulse heights for each FOV, along with estimated run time
   - 3e: [stitch images notebook](./templates/3e_stitch_images.ipynb) creates a single stitched image for each channel in your panel across all of the FOVs in your run
 
-### 4. Processing MIBI data
+### 4. Processing After a MIBI run
 Once your run has finished, you can begin to process the data to make it ready for analysis. To remove background signal contamination, as well as compensate for channel crosstalk, you can use the [compensation](./templates/4a_compensate_image_data.ipynb) notebook. This will guide you through the Rosetta algorithm, which uses a flow-cytometry style compensation approach to remove spurious signal.
 
 Following compensation, you will want to normalize your images to ensure consistent intensity across the run. You can use the [normalization](./templates/4b_normalize_image_data.ipynb) notebook to perform this step.
 
-### 5. Formatting MIBI runs for analysis
+### 5. Formatting MIBI Data for Downstream Analysis
 After the image processing and cleanup from *toffy* is complete, the final step is to format your data to faciliate easy downstream analysis. The [reorganization](./templates/5_rename_and_reorganize.ipynb) notebook will walk you through the process of renaming FOVs, combining partial runs, and consolidating your images.
 For more information, see the [reorganizing your data walkthrough](https://www.youtube.com/watch?v=nKYGWQ7GXC4&list=PLjNbkEm4vA27f8-EB7q9u_lDPI7oxohhn&index=5).
 
 ## Pipeline Flowchart
 
 ![flow-chart](templates/img/toffy_processing.png)
 
@@ -230,30 +280,34 @@
       * If you are using `pipx`, run the following installation commands
         ```sh
         brew install pipx
         pipx ensurepath
         ```
 * [pre-commit](https://pre-commit.com)
     ```sh
-    brew isntall pre-commit
+    brew install pre-commit
     ```
 
-## Setup
+### Setup
 
 1. Clone the repo: `git clone https://github.com/angelolab/toffy.git`
 2. `cd` into `toffy`.
 3. Install the pre-commit hooks with `pre-commit install --install-hooks`
 4. Set up Poetry for `toffy`
-   1. Run `poetry install` to install `alpineer` into your virtual environment (this will create a local virtual environment).
+   1. Run `poetry install` to install `toffy` into your virtual environment (this will create a local virtual environment).
       1. Poetry utilizes [Python's Virtual Environments](https://docs.python.org/3/tutorial/venv.html))
    2. Run `poetry install --with test`: Installs all the [dependencies needed for tests](pyproject.toml) (labeled under `tool.poetry.group.test.dependencies`)
    3. Run `poetry install --with dev`: Installs all the [dependencies needed for development](pyproject.coml) (labeled under `tool.poetry.group.dev.dependencies`)
    4. You may combine these as well with `poetry install --with dev,test`. Installing the base dependencies and the two optional groups.
 5. In order to test to see if Poetry is working properly, run `poetry show --tree`. This will output the dependency tree for the base dependencies (labeled under `tool.poetry.dependencies`).
 6. All tests can be run with `poetry run pytest`
 7. For every commit, *pre-commit* will format your changes to be complient with `pycodestyle`.
 
 ## Questions?
 
 If you have a general question or are having trouble with part of the repo, head to the [discussions](https://github.com/angelolab/toffy/discussions) tab to get help. If you've found a bug with the codebase, first make sure there's not already an [open issue](https://github.com/angelolab/toffy/issues), and if not, you can then [open an issue](https://github.com/angelolab/toffy/issues/new/choose) describing the bug.
 
 Before opening, please double check and see that someone else hasn't opened an issue for your question already.
+
+## How to cite
+Please directly cite the `toffy` repo (https://github.com/angelolab/toffy) if it was a part of your analysis.
+
```

### Comparing `toffy-0.1.2/pyproject.toml` & `toffy-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Toffy"
-version = "0.1.2"
+version = "0.2.0"
 description = "Scripts for interacting with and generating data from the commercial MIBIScope."
 authors = [
     "Noah Frey Greenwald <nfgreen@stanford.edu>",
     "Adam Kagel <ackagel@stanford.edu>",
     "Alex Kong <alkong@stanford.edu>",
     "Cami Laura Sowers <csowers@stanford.edu>",
     "Sricharan Reddy Varra <srivarra@stanford.edu>",
@@ -14,15 +14,17 @@
 repository = "https://github.com/angelolab/toffy"
 documentation = "https://toffy.readthedocs.io"
 readme = "README.md"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 packages = [{ include = 'toffy', from = 'src' }]
 
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
@@ -30,24 +32,25 @@
 enable = false
 vcs = "git"
 bump = true
 style = "pep440"
 metadata = false
 
 [tool.poetry.dependencies]
-python = "^3.8"
-alpineer = "^0.1.5"
-mibi-bin-tools = "^0.2.8"
+python = "^3.9"
+alpineer = "0.1.7"
+mibi-bin-tools = "0.2.9"
 ipywidgets = "^8"
 numpy = "1.*"
 natsort = "^8"
 seaborn = "^0.12"
 scikit-learn = "^1"
 watchdog = "^3"
 tqdm = "^4"
+pandas = "^1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 coveralls = { version = "^3.3.1", extras = ["toml"] }
 pytest = "^7.2.2"
@@ -66,26 +69,26 @@
 isort = "^5.10.1"
 jupyterlab = "^3.6.1"
 jupyter-contrib-nbextensions = "^0.7.0"
 
 ## TYPE CHECKING ##
 
 [tool.mypy]
-python_version = "3.8"
+python_version = "3.9"
 mypy_path = "$MYPY_CONFIG_FILE_DIR/src:$MYPY_CONFIG_FILE_DIR/tests"
 warn_return_any = true
 warn_unused_configs = true
 warn_unused_ignores = false
 ignore_missing_imports = true
 
 ## LINTING, FORMATTING ##
 
 [tool.black]
 line-length = 100
-target-version = ['py38']
+target-version = ["py39", "py310", "py311"]
 include = '\.pyi?$'
 preview = true
 
 [tool.isort]
 py_version = 38
 line_length = 100
 profile = "black"
```

### Comparing `toffy-0.1.2/src/toffy/bin_extraction.py` & `toffy-0.2.0/src/toffy/bin_extraction.py`

 * *Files identical despite different names*

### Comparing `toffy-0.1.2/src/toffy/detector_sweep.py` & `toffy-0.2.0/src/toffy/detector_sweep.py`

 * *Files identical despite different names*

### Comparing `toffy-0.1.2/src/toffy/file_hash.py` & `toffy-0.2.0/src/toffy/file_hash.py`

 * *Files identical despite different names*

### Comparing `toffy-0.1.2/src/toffy/fov_watcher.py` & `toffy-0.2.0/src/toffy/fov_watcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,14 +199,15 @@
 
         # create run structure
         self.run_structure = RunStructure(run_folder, timeout=timeout)
 
         self.fov_func = fov_callback
         self.run_func = run_callback
         self.inter_func = intermediate_callback
+        self.inter_return_vals = None
 
         for root, dirs, files in os.walk(run_folder):
             for name in files:
                 self.on_created(FileCreatedEvent(os.path.join(root, name)))
 
     def on_created(self, event: FileCreatedEvent):
         """Handles file creation events
@@ -247,15 +248,25 @@
                 f"Running {self.fov_func.__name__} on {point_name}\n"
             )
 
             self.fov_func(self.run_folder, point_name)
             self.run_structure.processed(point_name)
 
             if self.inter_func:
-                self.inter_func(self.run_folder)
+                # clear plots contained in intermediate return values if set
+                if self.inter_return_vals:
+                    qc_plots = self.inter_return_vals.get("plot_qc_metrics", None)
+                    mph_plot = self.inter_return_vals.get("plot_mph_metrics", None)
+
+                    if qc_plots or mph_plot:
+                        plt.cla()
+                        plt.clf()
+                        plt.close("all")
+
+                self.inter_return_vals = self.inter_func(self.run_folder)
 
             logf.close()
             self.check_complete()
 
     def check_complete(self):
         """Checks run structure fov_progress status
```

### Comparing `toffy-0.1.2/src/toffy/image_stitching.py` & `toffy-0.2.0/src/toffy/image_stitching.py`

 * *Files 7% similar despite different names*

```diff
@@ -82,16 +82,16 @@
     for fov in run_data["fovs"]:
         run_order = fov.get("runOrder")
         default_name = f"fov-{run_order}-scan-1"
 
         if default_name in fov_list:
             # get tiled name
             tiled_name = fov.get("name")
-            # filter out moly fovs
-            if tiled_name != "MoQC":
+            # filter out non-tiled and moly fovs
+            if re.search(re.compile(r"(R\+?\d+)(C\+?\d+)"), tiled_name) and tiled_name != "MoQC":
                 fov_names[tiled_name] = default_name
 
     return fov_names
 
 
 def stitch_images(tiff_out_dir, run_dir=None, channels=None, img_sub_folder=None, tiled=False):
     """Creates a new directory containing stitched channel images for the run
@@ -103,17 +103,18 @@
         tiled (bool): whether to stitch images back into original tiled shape"""
 
     io_utils.validate_paths(tiff_out_dir)
     if run_dir:
         io_utils.validate_paths(run_dir)
 
     # check for previous stitching
-    stitched_dir = os.path.join(tiff_out_dir, "stitched_images")
+    run_name = os.path.basename(tiff_out_dir)
+    stitched_dir = os.path.join(tiff_out_dir, f"{run_name}_stitched")
     if tiled:
-        stitched_dir = os.path.join(tiff_out_dir, "stitched_images_tiled")
+        stitched_dir = os.path.join(tiff_out_dir, f"{run_name}_tiled")
         if run_dir is None:
             raise ValueError(
                 "You must provide the run directory to stitch images into their "
                 "original tiled shape."
             )
     if os.path.exists(stitched_dir):
         raise ValueError(f"The stitch_images subdirectory already exists in {tiff_out_dir}")
@@ -142,46 +143,64 @@
                     substrs=".tiff",
                 )
             ),
         )
 
     # get load and stitching args
     if tiled:
-        folders_dict = get_tiled_names(folders, run_dir)
         # returns a dict with keys RnCm and values og folder names
+        folders_dict = get_tiled_names(folders, run_dir)
         try:
-            expected_fovs, num_rows, num_cols = load_utils.get_tiled_fov_names(
+            expected_tiles = load_utils.get_tiled_fov_names(
                 list(folders_dict.keys()), return_dims=True
             )
         except AttributeError:
             raise ValueError(f"FOV names found in the run file were not in tiled (RnCm) format.")
     else:
         num_cols = math.isqrt(len(folders))
         max_img_size = get_max_img_size(tiff_out_dir, img_sub_folder, run_dir)
 
     # make stitched subdir
     os.makedirs(stitched_dir)
 
     # save the stitched images to the stitched_image subdir
     for chan in channels:
-        # tiled image loading
         if tiled:
-            image_data = load_utils.load_tiled_img_data(
-                tiff_out_dir,
-                folders_dict,
-                expected_fovs,
-                chan,
-                single_dir=False,
-                img_sub_folder=img_sub_folder,
-            )
+            for tile in expected_tiles:
+                prefix, expected_fovs, num_rows, num_cols = tile
+                if prefix == "":
+                    prefix = "unnamed_tile"
+                # subset the folders_dict for fovs found in the current tile
+                tile_dict = {
+                    fov: folders_dict[fov] for fov in expected_fovs if fov in folders_dict.keys()
+                }
+
+                # save to individual tile subdirs
+                tile_stitched_dir = os.path.join(stitched_dir, prefix)
+                if not os.path.exists(tile_stitched_dir):
+                    os.makedirs(tile_stitched_dir)
+
+                image_data = load_utils.load_tiled_img_data(
+                    tiff_out_dir,
+                    tile_dict,
+                    expected_fovs,
+                    chan,
+                    single_dir=False,
+                    img_sub_folder=img_sub_folder,
+                )
+                fname = os.path.join(tile_stitched_dir, chan + "_stitched.tiff")
+                stitched = data_utils.stitch_images(image_data, num_cols)
+                current_img = stitched.loc["stitched_image", :, :, chan].values
+                image_utils.save_image(fname, current_img)
+
         else:
             image_data = load_utils.load_imgs_from_tree(
                 tiff_out_dir,
                 img_sub_folder=img_sub_folder,
                 fovs=folders,
                 channels=[chan],
                 max_image_size=max_img_size,
             )
-        stitched = data_utils.stitch_images(image_data, num_cols)
-        current_img = stitched.loc["stitched_image", :, :, chan].values
-        fname = os.path.join(stitched_dir, chan + "_stitched.tiff")
-        image_utils.save_image(fname, current_img)
+            fname = os.path.join(stitched_dir, chan + "_stitched.tiff")
+            stitched = data_utils.stitch_images(image_data, num_cols)
+            current_img = stitched.loc["stitched_image", :, :, chan].values
+            image_utils.save_image(fname, current_img)
```

### Comparing `toffy-0.1.2/src/toffy/json_utils.py` & `toffy-0.2.0/src/toffy/json_utils.py`

 * *Files identical despite different names*

### Comparing `toffy-0.1.2/src/toffy/mibitracker_utils.py` & `toffy-0.2.0/src/toffy/mibitracker_utils.py`

 * *Files identical despite different names*

### Comparing `toffy-0.1.2/src/toffy/mph_comp.py` & `toffy-0.2.0/src/toffy/mph_comp.py`

 * *Files 11% similar despite different names*

```diff
@@ -136,37 +136,38 @@
     combined_df.to_csv(os.path.join(csv_dir, "mph_pulse_combined.csv"), index=False)
 
     # return data
     if return_data:
         return combined_df
 
 
-def visualize_mph(mph_df, out_dir, regression: bool = False):
+def visualize_mph(mph_df, out_dir, regression: bool = False, return_plot: bool = False):
     """Create a scatterplot visualizing median pulse heights by FOV cumulative count
     Args:
         mph_df (pd.DataFrame): data detailing total counts and pulse heights
         out_dir (str): path of directory to save plot to
         regression (bool): whether to plot regression line, default is False
+        return_plot (bool): if True, this will return the plot. Defaults to False.
     """
 
     # path validation checks
     if out_dir is not None:
         io_utils.validate_paths(out_dir)
 
     # visualize the median pulse heights
-    plt.title("FOV total counts vs median pulse height")
     fig = plt.figure()
     ax1 = fig.add_subplot(111)
     x = mph_df["cum_total_count"] / 1000000
     y = mph_df["MPH"]
     ax1.set_xlabel("FOV cumulative count (in millions)")
     ax1.set_ylabel("median pulse height")
     ax1.scatter(x, y)
     ax2 = ax1.twiny()
     ax2.set_xlabel("estimated time (hours)")
+    plt.title("FOV total counts vs median pulse height")
 
     # create time axis
     new_ticks = generate_time_ticks(mph_df)
     tick_locations = new_ticks[0]
     tick_labels = new_ticks[1]
     ax2.set_xlim(ax1.get_xlim())
     ax2.set_xticks(tick_locations)
@@ -182,7 +183,10 @@
         ax1.plot(x2, m * x2 + b)
 
     # save figure
     file_path = os.path.join(out_dir, "fov_vs_mph.png")
     if os.path.exists(file_path):
         os.remove(file_path)
     plt.savefig(file_path)
+
+    if return_plot:
+        return fig
```

### Comparing `toffy-0.1.2/src/toffy/mph_inspect.py` & `toffy-0.2.0/src/toffy/mph_inspect.py`

 * *Files identical despite different names*

### Comparing `toffy-0.1.2/src/toffy/normalize.py` & `toffy-0.2.0/src/toffy/normalize.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,18 +99,27 @@
     def poly_4(x, a, b, c, d, e):
         return a * x + b * x**2 + c * x**3 + d * x**4 + e
 
     def poly_5(x, a, b, c, d, e, f):
         return a * x + b * x**2 + c * x**3 + d * x**4 + e * x**5 + f
 
     def log(x, a, b):
-        return a * np.log(x) + b
+        # edge case appears when x is a single int/float that returns non NaN/inf for np.log
+        # in this case, return the base np.log calculation
+        try:
+            return (a * np.ma.log(x) + b).filled(0)
+        except AttributeError:
+            return a * np.log(x) + b
 
     def exp(x, a, b, c, d):
-        x_log = np.log(x)
+        try:
+            x_log = (np.ma.log(x)).filled(0)
+        except AttributeError:
+            x_log = a * np.log(x) + b
+
         return a * x_log + b * x_log**2 + c * x_log**3 + d
 
     objectives = {
         "poly_2": poly_2,
         "poly_3": poly_3,
         "poly_4": poly_4,
         "poly_5": poly_5,
@@ -626,25 +635,31 @@
     pulse_height_df["pulse_height_fit"] = 0
 
     # create x axis values
     num_fovs = len(np.unique(pulse_height_df["fov"]))
     fov_order = np.linspace(0, num_fovs - 1, num_fovs)
 
     for mass in masses:
-        # load channel-specific prediction function
+        # if channel-specific prediction function does not exist, set to 0
         mass_path = os.path.join(obj_func_dir, str(mass) + "_norm_func.json")
+        mass_idx = pulse_height_df["mass"] == mass
+
+        if not os.path.exists(mass_path):
+            pulse_height_df.loc[mass_idx, "pulse_height_fit"] = 0.0
+            continue
+
+        # load channel-specific prediction function
         mass_json = read_json_file(mass_path)
 
         # compute predicted MPH
         name, weights = mass_json["name"], mass_json["weights"]
         pred_func = create_prediction_function(name=name, weights=weights)
         pred_vals = pred_func(fov_order)
 
         # update df
-        mass_idx = pulse_height_df["mass"] == mass
         pulse_height_df.loc[mass_idx, "pulse_height_fit"] = pred_vals
 
     return pulse_height_df
 
 
 def create_fitted_pulse_heights_file(pulse_height_dir, panel_info, norm_dir, mass_obj_func):
     """Create a single file containing the pulse heights after fitting a curve per mass
@@ -673,14 +688,20 @@
         pulse_height_df["fov"], ordered=True, categories=ordering
     )
     pulse_height_df = pulse_height_df.sort_values("fov")
 
     # loop over each mass, and fit a curve for MPH over the course of the run
     for mass in masses:
         mph_vals = pulse_height_df.loc[pulse_height_df["mass"] == mass, "pulse_height"].values
+
+        # only create a _norm_func file if the mph_vals are non-zero
+        if np.all(mph_vals == 0):
+            warnings.warn("Skipping normalization for mass %s with all zero pulse heights" % mass)
+            continue
+
         fit_mass_mph_curve(mph_vals=mph_vals, mass=mass, save_dir=fit_dir, obj_func=mass_obj_func)
 
     # update pulse_height_df to include fitted mph values
     pulse_height_df = create_fitted_mass_mph_vals(
         pulse_height_df=pulse_height_df, obj_func_dir=fit_dir
     )
 
@@ -703,17 +724,19 @@
         bad_channels = np.array(channels)[extreme_mask]
         warnings.warn(
             "The following channel(s) had an extreme normalization "
             "value for fov {}. Manual inspection for accuracy is "
             "recommended: {}".format(fov, bad_channels)
         )
 
-    # correct images and save
+    # correct images and save, ensure that no division by zero happens
     norm_vals = norm_vals.astype(img_data.dtype)
-    normalized_images = img_data / norm_vals.reshape((1, 1, 1, len(norm_vals)))
+    norm_div = norm_vals.reshape((1, 1, 1, len(norm_vals)))
+    norm_vals_masked = np.ma.masked_values(x=norm_vals, value=0)
+    normalized_images = np.ma.divide(img_data.values, norm_div).filled(0)
 
     for idx, chan in enumerate(channels):
         fname = os.path.join(output_fov_dir, chan + ".tiff")
         image_utils.save_image(fname, normalized_images[0, :, :, idx])
 
     # save logs
     log_df = pd.DataFrame({"channels": channels, "norm_vals": norm_vals})
@@ -774,16 +797,16 @@
     pulse_fovs = np.unique(pulse_height_df["fov"])
     misc_utils.verify_same_elements(image_data_fovs=img_fovs, pulse_height_csv_files=pulse_fovs)
 
     # loop over each fov
     for fov in img_fovs:
         # compute per-mass normalization constant
         pulse_height_fov = pulse_height_df.loc[pulse_height_df["fov"] == fov, :]
-        norm_vals = norm_func(pulse_height_fov["pulse_height_fit"].values)
         channels = pulse_height_fov["Target"].values
+        norm_vals = norm_func(pulse_height_fov["pulse_height_fit"].values)
 
         # get images
         images = load_utils.load_imgs_from_tree(
             img_dir, fovs=[fov], channels=channels, img_sub_folder=img_sub_folder
         )
 
         # normalize and save
```

### Comparing `toffy-0.1.2/src/toffy/panel_utils.py` & `toffy-0.2.0/src/toffy/panel_utils.py`

 * *Files identical despite different names*

### Comparing `toffy-0.1.2/src/toffy/qc_comp.py` & `toffy-0.2.0/src/toffy/qc_comp.py`

 * *Files identical despite different names*

### Comparing `toffy-0.1.2/src/toffy/qc_metrics_plots.py` & `toffy-0.2.0/src/toffy/qc_metrics_plots.py`

 * *Files identical despite different names*

### Comparing `toffy-0.1.2/src/toffy/reorg.py` & `toffy-0.2.0/src/toffy/reorg.py`

 * *Files identical despite different names*

### Comparing `toffy-0.1.2/src/toffy/rosetta.py` & `toffy-0.2.0/src/toffy/rosetta.py`

 * *Files identical despite different names*

### Comparing `toffy-0.1.2/src/toffy/settings.py` & `toffy-0.2.0/src/toffy/settings.py`

 * *Files identical despite different names*

### Comparing `toffy-0.1.2/src/toffy/streak_detection.py` & `toffy-0.2.0/src/toffy/streak_detection.py`

 * *Files identical despite different names*

### Comparing `toffy-0.1.2/src/toffy/tiling_utils.py` & `toffy-0.2.0/src/toffy/tiling_utils.py`

 * *Files identical despite different names*

### Comparing `toffy-0.1.2/src/toffy/watcher_callbacks.py` & `toffy-0.2.0/src/toffy/watcher_callbacks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import inspect
 import os
 import platform
 from dataclasses import dataclass, field
 from typing import Iterable
 
-if platform.system() == "Darwin":
-    import matplotlib
+# prevent memory leaking from creating plots that are never shown
+import matplotlib
 
-    matplotlib.use("Agg")
+matplotlib.use("Agg")
 
 import matplotlib.pyplot as plt
 import pandas as pd
 import xarray as xr
 from alpineer import misc_utils
 from mibi_bin_tools.bin_files import _write_out, extract_bin_files
 from mibi_bin_tools.type_utils import any_true
@@ -45,46 +45,59 @@
                 Additional arguments for `toffy.qc_comp.visualize_qc_metrics`.
                 Accepted kwargs are
 
              - axes_size
              - wrap
              - dpi
              - save_dir
+        Returns:
+            dict:
+                Maps each metric name to their respective plot
         """
         # filter kwargs
         valid_kwargs = ["axes_size", "wrap", "dpi", "save_dir"]
         viz_kwargs = {k: v for k, v in kwargs.items() if k in valid_kwargs}
+        qc_plots = {}
 
         combine_qc_metrics(qc_out_dir)
         for metric_name in QC_COLUMNS:
-            visualize_qc_metrics(metric_name, qc_out_dir, **viz_kwargs)
+            qc_plots[metric_name] = visualize_qc_metrics(
+                metric_name, qc_out_dir, **viz_kwargs, return_plot=True
+            )
+
+        return qc_plots
 
     def plot_mph_metrics(self, mph_out_dir, plot_dir, **kwargs):
         """Plots mph metrics generated by the `generate_mph` callback
 
         Args:
             mph_out_dir (str): directory containing mph metric csv
             plot_dir (str): director to store the plot to
             **kwargs (Dict[str, Any]):
                 Additional arguments for `toffy.mph_comp.visualize_mph`.
                 Accepted kwargs are
 
              - regression
+        Returns:
+            matplotlib.figure.Figure:
+                The figure containing the MPH plot
         """
         if not os.path.exists(plot_dir):
             os.makedirs(plot_dir)
 
         # filter kwargs
         valid_kwargs = [
             "regression",
         ]
         viz_kwargs = {k: v for k, v in kwargs.items() if k in valid_kwargs}
 
         mph_df = combine_mph_metrics(mph_out_dir, return_data=True)
-        visualize_mph(mph_df, plot_dir, **viz_kwargs)
+        mph_fig = visualize_mph(mph_df, plot_dir, **viz_kwargs, return_plot=True)
+
+        return mph_fig
 
     def image_stitching(self, tiff_out_dir, **kwargs):
         """Stitches individual FOV channel images together into one tiff
 
         Args:
             tiff_out_dir (str): directory containing extracted images
             **kwargs (Dict[str, Any]):
@@ -378,16 +391,19 @@
 
     intermediate_callback = None
     intermediate_callback = None
     if intermediate_callbacks:
 
         def intermediate_callback(run_folder: str):
             callback_obj = RunCallbacks(run_folder)
+            inter_return_vals = {}
 
             for run_cb in intermediate_callbacks:
                 if cb := getattr(callback_obj, run_cb, None):
-                    cb(**kwargs)
+                    inter_return_vals[cb.__func__.__name__] = cb(**kwargs)
                 else:
                     # unreachable...
                     raise ValueError(f"Could not locate attribute {run_cb} in RunCallbacks object")
 
+            return inter_return_vals
+
     return fov_callback, run_callback, intermediate_callback
```

### Comparing `toffy-0.1.2/PKG-INFO` & `toffy-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,46 @@
-Metadata-Version: 2.1
-Name: toffy
-Version: 0.1.2
-Summary: Scripts for interacting with and generating data from the commercial MIBIScope.
-Home-page: https://github.com/angelolab/toffy
-License: Modified Apache 2.0
-Author: Noah Frey Greenwald
-Author-email: nfgreen@stanford.edu
-Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: alpineer (>=0.1.5,<0.2.0)
-Requires-Dist: ipywidgets (>=8,<9)
-Requires-Dist: mibi-bin-tools (>=0.2.8,<0.3.0)
-Requires-Dist: natsort (>=8,<9)
-Requires-Dist: numpy (>=1.0.0,<2.0.0)
-Requires-Dist: scikit-learn (>=1,<2)
-Requires-Dist: seaborn (>=0.12,<0.13)
-Requires-Dist: tqdm (>=4,<5)
-Requires-Dist: watchdog (>=3,<4)
-Project-URL: Documentation, https://toffy.readthedocs.io
-Project-URL: Repository, https://github.com/angelolab/toffy
-Description-Content-Type: text/markdown
-
 # toffy
+
+<div align="center">
+
+| | |
+| ---        |    ---  |
+| CI / CD | [![CI](https://github.com/angelolab/toffy/actions/workflows/ci.yml/badge.svg)](https://github.com/angelolab/toffy/actions/workflows/ci.yml) [![Coverage Status](https://coveralls.io/repos/github/angelolab/toffy/badge.svg?branch=main)](https://coveralls.io/github/angelolab/mibi-bin-tools?branch=main) |
+| Package | [![PyPI - Version](https://img.shields.io/pypi/v/toffy.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/toffy/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/toffy.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold)](https://pypi.org/project/toffy/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/toffy.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/toffy/) |
+|Meta | [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![PyPI - License](https://img.shields.io/pypi/l/toffy?color=9400d3)](LICENSE) |
+</div>
+
+
 The toffy repo is designed to simplify the process of generating and processing data on the MIBIScope platform.
 
-This repo is currently in beta testing. None of the code has been published yet, and we will be making breaking changes frequently. If you find bugs, please [open an issue](https://github.com/angelolab/toffy/issues/new/choose). If you have questions or want to collaborate, please reach out to Noah (nfgreen@stanford.edu)
+This repo is currently in beta testing. None of the code has been published yet, and we will be making breaking changes frequently. If you find bugs, please [open an issue](https://github.com/angelolab/toffy/issues/new/choose).
 
 ## Table of Contents
 - [Overview](#overview)
   - [1. Using toffy for the first time](#1-using-toffy-for-the-first-time)
   - [2. Setting up a MIBI run](#2-setting-up-a-mibi-run)
   - [3. Evaluating a MIBI run](#3-evaluating-a-mibi-run)
-  - [4. Processing data after a MIBI run](#4-processing-mibi-data)
-  - [5. Formatting data for downstream analysis](#5-formatting-mibi-runs-for-analysis)
+  - [4. Processing After a MIBI run](#4-processing-after-a-mibi-run)
+  - [5. Formatting MIBI Data for Downstream Analysis](#5-formatting-mibi-data-for-downstream-analysis)
+- [Pipeline Flowchart](#pipeline-flowchart)
 - [Installation](#installation)
   - [Requirements for specific operating systems](#requirements-for-specific-operating-systems)
     - [Windows](#windows)
     - [macOS](#macos)
   - [Setting up the virtual environment](#setting-up-the-virtual-environment)
   - [Using the repo](#using-the-repo)
   - [Updating the repo](#updating-the-repo)
 - [Directory structure](#directory-structure)
 - [Panel format](#panel-format)
 - [Median Pulse Height](#median-pulse-height)
+- [Development Notes](#development-notes)
+  - [Requirements](#requirements)
+  - [Setup](#setup)
 - [Questions?](#questions)
+- [How to cite](#how-to-cite)
 
 ## Overview
 The repo has four main parts, with associated code and jupyter notebooks for each.
 We have also recorded workshop talks which complement the repository. [MIBI Workshop (Pre-Recorded Lectures) Playlist](https://www.youtube.com/playlist?list=PLjNbkEm4vA27f8-EB7q9u_lDPI7oxohhn).
 
 ### 1. Using toffy for the first time
 The first time you use toffy on one of the commercial instruments, you'll need to perform some basic tasks to ensure everything is working properly. The [set up](./templates/1_set_up_toffy.ipynb) jupyter notebook will guide you through this process and the resulting directory structure is explained below ([directory structure](#directory-structure)).
@@ -78,20 +62,20 @@
 - 3b - 3e: post-run monitoring. For each step in the monitoring notebook, we have a dedicated notebook that can perform the same tasks once a run is complete.
 For more information, see the [image processing and extraction walkthrough](https://www.youtube.com/watch?v=QSzjW-cuZtg&list=PLjNbkEm4vA27f8-EB7q9u_lDPI7oxohhn&index=3).
   - 3b: [image extraction notebook](./templates/3b_extract_images_from_bin.ipynb) will extract images from bin files that have not already been processed
   - 3c: [qc metrics notebook](./templates/3c_generate_qc_metrics.ipynb) computes and visualizes the QC metrics for the images
   - 3d: [median pulse heights notebook](./templates/3d_compute_median_pulse_height.ipynb) generates plots showing median pulse heights for each FOV, along with estimated run time
   - 3e: [stitch images notebook](./templates/3e_stitch_images.ipynb) creates a single stitched image for each channel in your panel across all of the FOVs in your run
 
-### 4. Processing MIBI data
+### 4. Processing After a MIBI run
 Once your run has finished, you can begin to process the data to make it ready for analysis. To remove background signal contamination, as well as compensate for channel crosstalk, you can use the [compensation](./templates/4a_compensate_image_data.ipynb) notebook. This will guide you through the Rosetta algorithm, which uses a flow-cytometry style compensation approach to remove spurious signal.
 
 Following compensation, you will want to normalize your images to ensure consistent intensity across the run. You can use the [normalization](./templates/4b_normalize_image_data.ipynb) notebook to perform this step.
 
-### 5. Formatting MIBI runs for analysis
+### 5. Formatting MIBI Data for Downstream Analysis
 After the image processing and cleanup from *toffy* is complete, the final step is to format your data to faciliate easy downstream analysis. The [reorganization](./templates/5_rename_and_reorganize.ipynb) notebook will walk you through the process of renaming FOVs, combining partial runs, and consolidating your images.
 For more information, see the [reorganizing your data walkthrough](https://www.youtube.com/watch?v=nKYGWQ7GXC4&list=PLjNbkEm4vA27f8-EB7q9u_lDPI7oxohhn&index=5).
 
 ## Pipeline Flowchart
 
 ![flow-chart](templates/img/toffy_processing.png)
 
@@ -262,31 +246,33 @@
       * If you are using `pipx`, run the following installation commands
         ```sh
         brew install pipx
         pipx ensurepath
         ```
 * [pre-commit](https://pre-commit.com)
     ```sh
-    brew isntall pre-commit
+    brew install pre-commit
     ```
 
-## Setup
+### Setup
 
 1. Clone the repo: `git clone https://github.com/angelolab/toffy.git`
 2. `cd` into `toffy`.
 3. Install the pre-commit hooks with `pre-commit install --install-hooks`
 4. Set up Poetry for `toffy`
-   1. Run `poetry install` to install `alpineer` into your virtual environment (this will create a local virtual environment).
+   1. Run `poetry install` to install `toffy` into your virtual environment (this will create a local virtual environment).
       1. Poetry utilizes [Python's Virtual Environments](https://docs.python.org/3/tutorial/venv.html))
    2. Run `poetry install --with test`: Installs all the [dependencies needed for tests](pyproject.toml) (labeled under `tool.poetry.group.test.dependencies`)
    3. Run `poetry install --with dev`: Installs all the [dependencies needed for development](pyproject.coml) (labeled under `tool.poetry.group.dev.dependencies`)
    4. You may combine these as well with `poetry install --with dev,test`. Installing the base dependencies and the two optional groups.
 5. In order to test to see if Poetry is working properly, run `poetry show --tree`. This will output the dependency tree for the base dependencies (labeled under `tool.poetry.dependencies`).
 6. All tests can be run with `poetry run pytest`
 7. For every commit, *pre-commit* will format your changes to be complient with `pycodestyle`.
 
 ## Questions?
 
 If you have a general question or are having trouble with part of the repo, head to the [discussions](https://github.com/angelolab/toffy/discussions) tab to get help. If you've found a bug with the codebase, first make sure there's not already an [open issue](https://github.com/angelolab/toffy/issues), and if not, you can then [open an issue](https://github.com/angelolab/toffy/issues/new/choose) describing the bug.
 
 Before opening, please double check and see that someone else hasn't opened an issue for your question already.
 
+## How to cite
+Please directly cite the `toffy` repo (https://github.com/angelolab/toffy) if it was a part of your analysis.
```

