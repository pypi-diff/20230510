# Comparing `tmp/proteinflow-1.3.0.tar.gz` & `tmp/proteinflow-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinflow-1.3.0.tar", last modified: Tue May  9 16:52:22 2023, max compression
+gzip compressed data, was "proteinflow-1.3.1.tar", last modified: Wed May 10 11:04:36 2023, max compression
```

## Comparing `proteinflow-1.3.0.tar` & `proteinflow-1.3.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:52:22.335201 proteinflow-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-09 16:52:07.000000 proteinflow-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8779 2023-05-09 16:52:22.335201 proteinflow-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-05-09 16:52:07.000000 proteinflow-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:52:22.331201 proteinflow-1.3.0/proteinflow/
--rw-r--r--   0 runner    (1001) docker     (123)    93730 2023-05-09 16:52:07.000000 proteinflow-1.3.0/proteinflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:52:22.335201 proteinflow-1.3.0/proteinflow/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:52:07.000000 proteinflow-1.3.0/proteinflow/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-09 16:52:07.000000 proteinflow-1.3.0/proteinflow/scripts/proteinflow_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:52:22.335201 proteinflow-1.3.0/proteinflow/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:52:07.000000 proteinflow-1.3.0/proteinflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-09 16:52:07.000000 proteinflow-1.3.0/proteinflow/utils/async_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-09 16:52:07.000000 proteinflow-1.3.0/proteinflow/utils/biotite_sse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-05-09 16:52:07.000000 proteinflow-1.3.0/proteinflow/utils/build_pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    41037 2023-05-09 16:52:07.000000 proteinflow-1.3.0/proteinflow/utils/cluster_and_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-09 16:52:07.000000 proteinflow-1.3.0/proteinflow/utils/filter_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-09 16:52:07.000000 proteinflow-1.3.0/proteinflow/utils/mmcif_fix.py
--rw-r--r--   0 runner    (1001) docker     (123)    16990 2023-05-09 16:52:07.000000 proteinflow-1.3.0/proteinflow/utils/process_pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-05-09 16:52:07.000000 proteinflow-1.3.0/proteinflow/utils/split_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:52:22.335201 proteinflow-1.3.0/proteinflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8779 2023-05-09 16:52:22.000000 proteinflow-1.3.0/proteinflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-09 16:52:22.000000 proteinflow-1.3.0/proteinflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:52:22.000000 proteinflow-1.3.0/proteinflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-09 16:52:22.000000 proteinflow-1.3.0/proteinflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-09 16:52:22.000000 proteinflow-1.3.0/proteinflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-09 16:52:22.000000 proteinflow-1.3.0/proteinflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-09 16:52:07.000000 proteinflow-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 16:52:22.335201 proteinflow-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:52:22.335201 proteinflow-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-09 16:52:07.000000 proteinflow-1.3.0/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-09 16:52:07.000000 proteinflow-1.3.0/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-09 16:52:07.000000 proteinflow-1.3.0/tests/test_sabdab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:04:36.732840 proteinflow-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-10 11:04:23.000000 proteinflow-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-05-10 11:04:36.732840 proteinflow-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-05-10 11:04:23.000000 proteinflow-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:04:36.728840 proteinflow-1.3.1/proteinflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    97798 2023-05-10 11:04:23.000000 proteinflow-1.3.1/proteinflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:04:36.728840 proteinflow-1.3.1/proteinflow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 11:04:23.000000 proteinflow-1.3.1/proteinflow/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-10 11:04:23.000000 proteinflow-1.3.1/proteinflow/scripts/proteinflow_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:04:36.732840 proteinflow-1.3.1/proteinflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 11:04:23.000000 proteinflow-1.3.1/proteinflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-10 11:04:23.000000 proteinflow-1.3.1/proteinflow/utils/async_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-10 11:04:23.000000 proteinflow-1.3.1/proteinflow/utils/biotite_sse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-05-10 11:04:23.000000 proteinflow-1.3.1/proteinflow/utils/build_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41037 2023-05-10 11:04:23.000000 proteinflow-1.3.1/proteinflow/utils/cluster_and_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-10 11:04:23.000000 proteinflow-1.3.1/proteinflow/utils/filter_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-10 11:04:23.000000 proteinflow-1.3.1/proteinflow/utils/mmcif_fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16990 2023-05-10 11:04:23.000000 proteinflow-1.3.1/proteinflow/utils/process_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-05-10 11:04:23.000000 proteinflow-1.3.1/proteinflow/utils/split_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:04:36.728840 proteinflow-1.3.1/proteinflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-05-10 11:04:36.000000 proteinflow-1.3.1/proteinflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-10 11:04:36.000000 proteinflow-1.3.1/proteinflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 11:04:36.000000 proteinflow-1.3.1/proteinflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 11:04:36.000000 proteinflow-1.3.1/proteinflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-10 11:04:36.000000 proteinflow-1.3.1/proteinflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 11:04:36.000000 proteinflow-1.3.1/proteinflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-10 11:04:23.000000 proteinflow-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 11:04:36.732840 proteinflow-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:04:36.732840 proteinflow-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-10 11:04:23.000000 proteinflow-1.3.1/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-10 11:04:23.000000 proteinflow-1.3.1/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-10 11:04:23.000000 proteinflow-1.3.1/tests/test_sabdab.py
```

### Comparing `proteinflow-1.3.0/LICENSE` & `proteinflow-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.0/PKG-INFO` & `proteinflow-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 1.3.0
+Version: 1.3.1
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -25,15 +25,15 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI](https://img.shields.io/pypi/v/proteinflow)](https://pypi.org/project/proteinflow/)
 [![Conda](https://img.shields.io/conda/v/adaptyvbio/proteinflow)](https://anaconda.org/adaptyvbio/proteinflow)
 [![Docker Image Version (latest semver)](https://img.shields.io/docker/v/adaptyvbio/proteinflow?label=docker)](https://hub.docker.com/r/adaptyvbio/proteinflow/tags)
 ![Generic badge](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)
 
 
-ProteinFlow is an open-source Python library that streamlines the pre-processing of protein structure data for deep learning applications. ProteinFlow enables users to efficiently filter, cluster, and generate new datasets from resources like the Protein Data Bank (PDB).
+ProteinFlow is an open-source Python library that streamlines the pre-processing of protein structure data for deep learning applications. ProteinFlow enables users to efficiently filter, cluster, and generate new datasets from resources like the Protein Data Bank (PDB) and SAbDab (The Structural Antibody Database).
 
 Here are some of the key features we currently support:
 
 - ⛓️ Processing of both single-chain and multi-chain protein structures (Biounit PDB definition)
 - 🏷️ Various featurization options can be computed, including secondary structure features, torsion angles, etc.
 - 💾 A variety of data loading options and conversions to cater to different downstream training frameworks
 - 🧬 Access to up-to-date, pre-computed protein structure datasets
@@ -94,31 +94,39 @@
 ```bash
 proteinflow generate --tag new --resolution_thr 5 --pdb_snapshot 20190101 --not_filter_methods --min_seq_id 0.4 --max_length 1000 --min_length 5 --missing_ends_thr 0.1 --valid_split 0.1
 ```
 See the [docs](https://adaptyvbio.github.io/ProteinFlow/) (or `proteinflow generate --help`) for the full list of parameters and more information.
 
 A registry of all the files that are removed during the filtering as well as description with the reason for their removal is created automatically for each `generate` command. The log files are save (at `data/logs` by default) and a summary can be accessed running `proteinflow get_summary {log_path}`.
 
+You can also use the `--sabdab` option to load files from SAbDab and cluster them based on CDRs. Use together with `--zip_path` to process a custom SAbDab-like zip file.
+
 ### Splitting
 By default, both `proteinflow generate` and `proteinflow download` will also split your data into training, test and validation according to MMseqs2 clustering and homomer/heteromer/single chain proportions. However, you can skip this step with a `--skip_splitting` flag and then perform it separately with the `proteinflow split` command.
 
 The following command will perform the splitting with a 10% validation set, a 5% test set and a 50% threshold for sequence identity clusters.
 ```bash
 proteinflow split --tag new --valid_split 0.1 --test_split 0.5 --min_seq_id 0.5
 ```
 
+Use the `--exclude_chains` and `--exclude_threshold` parameters to move all biounits that contain chains similar to what you specify to a separate folder.
+
 ### Using the data
 The output files are pickled nested dictionaries where first-level keys are chain Ids and second-level keys are the following:
 - `'crd_bb'`: a `numpy` array of shape `(L, 4, 3)` with backbone atom coordinates (N, C, CA, O),
 - `'crd_sc'`: a `numpy` array of shape `(L, 10, 3)` with sidechain atom coordinates (check `proteinflow.sidechain_order()` for the order of atoms),
 - `'msk'`: a `numpy` array of shape `(L,)` where ones correspond to residues with known coordinates and
     zeros to missing values,
 - `'seq'`: a string of length `L` with residue types.
 
-Once your data is ready, you can open the files directly with `pickle` to access this data.
+In a SAbDab datasets, an additional key is added to the dictionary:
+- `'cdr'`: a `'numpy'` array of shape `(L,)` where CDR residues are marked with the corresponding type (`'H1'`, `'L1'`, ...) 
+    and non-CDR residues are marked with `'-'`.
+
+Once your data is ready, you can open the files with `pickle`.
 
 ```python
 import pickle
 import os
 
 train_folder = "./data/proteinflow_new/training"
 for filename in os.listdir(train_folder):
@@ -155,18 +163,18 @@
     ...
 ```
 See more details on available parameters and the data format in the [docs](https://adaptyvbio.github.io/ProteinFlow/) + [this repository](https://github.com/adaptyvbio/ProteinFlow-models) for a use case.
 
 ## ProteinFlow Stable Releases
 You can download them with `proteinflow download --tag {tag}` in the command line or browse in the [interface](https://proteinflow-datasets.s3.eu-west-1.amazonaws.com/index.html).
 
-|Tag    |Date    |Snapshot|Size|Min res|Min len|Max len|MMseqs thr|Split (train/val/test)|Missing thr (ends/middle)|Note|
-|-------|--------|--------|----|-------|-------|-------|----------|----------------------|-------------------------|----|
-|paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|first release, no mmCIF files|
-|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/5|0.3/0.1| v1.1.1|
+|Tag    |Date    |Snapshot|Size|Min res|Min len|Max len|MMseqs thr|Split (train/val/test)|Missing thr (ends/middle)|Source|Note|
+|-------|--------|--------|----|-------|-------|-------|----------|----------------------|-------------------------|---|----|
+|paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|first release, no mmCIF files|
+|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|v1.1.1|
 
 ## License
 The `proteinflow` package and data are released and distributed under the BSD 3-Clause License
 
 
 ## Contributions
 This is an open source project supported by [Adaptyv Bio](https://www.adaptyvbio.com/). Contributions, suggestions and bug-fixes are welcomed.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 1.3.0 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 1.3.1 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
@@ -15,76 +15,83 @@
 proteinflow)](https://anaconda.org/adaptyvbio/proteinflow) [![Docker Image
 Version (latest semver)](https://img.shields.io/docker/v/adaptyvbio/
 proteinflow?label=docker)](https://hub.docker.com/r/adaptyvbio/proteinflow/
 tags) ![Generic badge](https://img.shields.io/badge/Contributions-Welcome-
 brightgreen.svg) ProteinFlow is an open-source Python library that streamlines
 the pre-processing of protein structure data for deep learning applications.
 ProteinFlow enables users to efficiently filter, cluster, and generate new
-datasets from resources like the Protein Data Bank (PDB). Here are some of the
-key features we currently support: - âï¸ Processing of both single-chain and
-multi-chain protein structures (Biounit PDB definition) - ð·ï¸ Various
-featurization options can be computed, including secondary structure features,
-torsion angles, etc. - ð¾ A variety of data loading options and conversions
-to cater to different downstream training frameworks - ð§¬ Access to up-to-
-date, pre-computed protein structure datasets ![overview](https://
-raw.githubusercontent.com/adaptyvbio/ProteinFlow/main/media/pf-1.png) --- ##
-Installation conda: ```bash # This should take a few minutes, be patient conda
-install -c conda-forge -c bioconda -c adaptyvbio proteinflow ``` pip: ```bash
-pip install proteinflow ``` docker: ```bash docker pull adaptyvbio/proteinflow
-``` ### Troubleshooting - If you are using python 3.10 and encountering
-installation problems, try running `python -m pip install prody==2.4.0` before
-installing `proteinflow`. - If you are planning to generate new datasets and
-installed `proteinflow` with `pip`, you will need to additionally install
-[`mmseqs`](https://github.com/soedinglab/MMseqs2). - Generating new datasets
-also depends on the `rcsbsearch` package and the latest release [v0.2.3](https:
-//github.com/sbliven/rcsbsearch/releases/tag/v0.2.3) is currently not working
-correctly. The recommended fix is installing the version from [this pull
-request](https://github.com/sbliven/rcsbsearch/pull/6). ```bash python -m pip
-install "rcsbsearch @ git+https://github.com/sbliven/
-rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e" ``` - The docker image can
-be accessed in interactive mode with this command. ```bash docker run -it -v /
-path/to/data:/media adaptyvbio/proteinflow bash ``` ## Usage ### Downloading
-pre-computed datasets (stable) Already precomputed datasets with consensus set
-of parameters and can be accessed and downloaded using the `proteinflow`.
-package. Check the output of `proteinflow check_tags` for a list of available
-tags. ```bash proteinflow download --tag 20230102_stable ``` ### Running the
-pipeline You can also run `proteinflow` with your own parameters. Check the
-output of `proteinflow check_snapshots` for a list of available PDB snapshots
-(naming rule: `yyyymmdd`). For instance, let's generate a dataset with the
-following description: - resolution threshold: 5 angstrom, - PDB snapshot:
-20190101, - structure methods accepted: all (x-ray christolography, NRM, Cryo-
-EM), - sequence identity threshold for clustering: 40% sequence similarity, -
-maximum length per sequence: 1000 residues, - minimum length per sequence: 5
-residues, - maximum fraction of missing values at the ends: 10%, - size of
-validation subset: 10%. ```bash proteinflow generate --tag new --resolution_thr
-5 --pdb_snapshot 20190101 --not_filter_methods --min_seq_id 0.4 --max_length
-1000 --min_length 5 --missing_ends_thr 0.1 --valid_split 0.1 ``` See the [docs]
-(https://adaptyvbio.github.io/ProteinFlow/) (or `proteinflow generate --help`)
-for the full list of parameters and more information. A registry of all the
-files that are removed during the filtering as well as description with the
-reason for their removal is created automatically for each `generate` command.
-The log files are save (at `data/logs` by default) and a summary can be
-accessed running `proteinflow get_summary {log_path}`. ### Splitting By
-default, both `proteinflow generate` and `proteinflow download` will also split
-your data into training, test and validation according to MMseqs2 clustering
-and homomer/heteromer/single chain proportions. However, you can skip this step
-with a `--skip_splitting` flag and then perform it separately with the
-`proteinflow split` command. The following command will perform the splitting
-with a 10% validation set, a 5% test set and a 50% threshold for sequence
-identity clusters. ```bash proteinflow split --tag new --valid_split 0.1 --
-test_split 0.5 --min_seq_id 0.5 ``` ### Using the data The output files are
-pickled nested dictionaries where first-level keys are chain Ids and second-
-level keys are the following: - `'crd_bb'`: a `numpy` array of shape `(L, 4,
-3)` with backbone atom coordinates (N, C, CA, O), - `'crd_sc'`: a `numpy` array
-of shape `(L, 10, 3)` with sidechain atom coordinates (check
-`proteinflow.sidechain_order()` for the order of atoms), - `'msk'`: a `numpy`
-array of shape `(L,)` where ones correspond to residues with known coordinates
-and zeros to missing values, - `'seq'`: a string of length `L` with residue
-types. Once your data is ready, you can open the files directly with `pickle`
-to access this data. ```python import pickle import os train_folder = "./data/
+datasets from resources like the Protein Data Bank (PDB) and SAbDab (The
+Structural Antibody Database). Here are some of the key features we currently
+support: - âï¸ Processing of both single-chain and multi-chain protein
+structures (Biounit PDB definition) - ð·ï¸ Various featurization options can
+be computed, including secondary structure features, torsion angles, etc. -
+ð¾ A variety of data loading options and conversions to cater to different
+downstream training frameworks - ð§¬ Access to up-to-date, pre-computed
+protein structure datasets ![overview](https://raw.githubusercontent.com/
+adaptyvbio/ProteinFlow/main/media/pf-1.png) --- ## Installation conda: ```bash
+# This should take a few minutes, be patient conda install -c conda-forge -
+c bioconda -c adaptyvbio proteinflow ``` pip: ```bash pip install proteinflow
+``` docker: ```bash docker pull adaptyvbio/proteinflow ``` ### Troubleshooting
+- If you are using python 3.10 and encountering installation problems, try
+running `python -m pip install prody==2.4.0` before installing `proteinflow`. -
+If you are planning to generate new datasets and installed `proteinflow` with
+`pip`, you will need to additionally install [`mmseqs`](https://github.com/
+soedinglab/MMseqs2). - Generating new datasets also depends on the `rcsbsearch`
+package and the latest release [v0.2.3](https://github.com/sbliven/rcsbsearch/
+releases/tag/v0.2.3) is currently not working correctly. The recommended fix is
+installing the version from [this pull request](https://github.com/sbliven/
+rcsbsearch/pull/6). ```bash python -m pip install "rcsbsearch @ git+https://
+github.com/sbliven/rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e" ``` -
+The docker image can be accessed in interactive mode with this command. ```bash
+docker run -it -v /path/to/data:/media adaptyvbio/proteinflow bash ``` ## Usage
+### Downloading pre-computed datasets (stable) Already precomputed datasets
+with consensus set of parameters and can be accessed and downloaded using the
+`proteinflow`. package. Check the output of `proteinflow check_tags` for a list
+of available tags. ```bash proteinflow download --tag 20230102_stable ``` ###
+Running the pipeline You can also run `proteinflow` with your own parameters.
+Check the output of `proteinflow check_snapshots` for a list of available PDB
+snapshots (naming rule: `yyyymmdd`). For instance, let's generate a dataset
+with the following description: - resolution threshold: 5 angstrom, - PDB
+snapshot: 20190101, - structure methods accepted: all (x-ray christolography,
+NRM, Cryo-EM), - sequence identity threshold for clustering: 40% sequence
+similarity, - maximum length per sequence: 1000 residues, - minimum length per
+sequence: 5 residues, - maximum fraction of missing values at the ends: 10%, -
+size of validation subset: 10%. ```bash proteinflow generate --tag new --
+resolution_thr 5 --pdb_snapshot 20190101 --not_filter_methods --min_seq_id 0.4
+--max_length 1000 --min_length 5 --missing_ends_thr 0.1 --valid_split 0.1 ```
+See the [docs](https://adaptyvbio.github.io/ProteinFlow/) (or `proteinflow
+generate --help`) for the full list of parameters and more information. A
+registry of all the files that are removed during the filtering as well as
+description with the reason for their removal is created automatically for each
+`generate` command. The log files are save (at `data/logs` by default) and a
+summary can be accessed running `proteinflow get_summary {log_path}`. You can
+also use the `--sabdab` option to load files from SAbDab and cluster them based
+on CDRs. Use together with `--zip_path` to process a custom SAbDab-like zip
+file. ### Splitting By default, both `proteinflow generate` and `proteinflow
+download` will also split your data into training, test and validation
+according to MMseqs2 clustering and homomer/heteromer/single chain proportions.
+However, you can skip this step with a `--skip_splitting` flag and then perform
+it separately with the `proteinflow split` command. The following command will
+perform the splitting with a 10% validation set, a 5% test set and a 50%
+threshold for sequence identity clusters. ```bash proteinflow split --tag new -
+-valid_split 0.1 --test_split 0.5 --min_seq_id 0.5 ``` Use the `--
+exclude_chains` and `--exclude_threshold` parameters to move all biounits that
+contain chains similar to what you specify to a separate folder. ### Using the
+data The output files are pickled nested dictionaries where first-level keys
+are chain Ids and second-level keys are the following: - `'crd_bb'`: a `numpy`
+array of shape `(L, 4, 3)` with backbone atom coordinates (N, C, CA, O), -
+`'crd_sc'`: a `numpy` array of shape `(L, 10, 3)` with sidechain atom
+coordinates (check `proteinflow.sidechain_order()` for the order of atoms), -
+`'msk'`: a `numpy` array of shape `(L,)` where ones correspond to residues with
+known coordinates and zeros to missing values, - `'seq'`: a string of length
+`L` with residue types. In a SAbDab datasets, an additional key is added to the
+dictionary: - `'cdr'`: a `'numpy'` array of shape `(L,)` where CDR residues are
+marked with the corresponding type (`'H1'`, `'L1'`, ...) and non-CDR residues
+are marked with `'-'`. Once your data is ready, you can open the files with
+`pickle`. ```python import pickle import os train_folder = "./data/
 proteinflow_new/training" for filename in os.listdir(train_folder): with open
 (os.path.join(train_folder, filename), "rb") as f: data = pickle.load(f) crd_bb
 = data["crd_bb"] seq = data["seq"] ... ``` Alternatively, you can use our
 `ProteinDataset` or `ProteinLoader` classes for convenient processing. Among
 other things, they allow for feature extraction, single chain / homomer /
 heteromer filtering and randomized sampling from sequence identity clusters.
 For example, here is how we can create a data loader that: - samples a
@@ -101,15 +108,16 @@
 should be masked, 0 otherwise ... ``` See more details on available parameters
 and the data format in the [docs](https://adaptyvbio.github.io/ProteinFlow/) +
 [this repository](https://github.com/adaptyvbio/ProteinFlow-models) for a use
 case. ## ProteinFlow Stable Releases You can download them with `proteinflow
 download --tag {tag}` in the command line or browse in the [interface](https://
 proteinflow-datasets.s3.eu-west-1.amazonaws.com/index.html). |Tag |Date
 |Snapshot|Size|Min res|Min len|Max len|MMseqs thr|Split (train/val/
-test)|Missing thr (ends/middle)|Note| |-------|--------|--------|----|-------|-
-------|-------|----------|----------------------|-------------------------|----
-| |paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|first release,
-no mmCIF files| |20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/
-5|0.3/0.1| v1.1.1| ## License The `proteinflow` package and data are released
-and distributed under the BSD 3-Clause License ## Contributions This is an open
+test)|Missing thr (ends/middle)|Source|Note| |-------|--------|--------|----|--
+-----|-------|-------|----------|----------------------|-----------------------
+--|---|----| |paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/
+0.1|PDB|first release, no mmCIF files|
+|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/5|0.3/
+0.1|PDB|v1.1.1| ## License The `proteinflow` package and data are released and
+distributed under the BSD 3-Clause License ## Contributions This is an open
 source project supported by [Adaptyv Bio](https://www.adaptyvbio.com/).
 Contributions, suggestions and bug-fixes are welcomed.
```

### Comparing `proteinflow-1.3.0/README.md` & `proteinflow-1.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI](https://img.shields.io/pypi/v/proteinflow)](https://pypi.org/project/proteinflow/)
 [![Conda](https://img.shields.io/conda/v/adaptyvbio/proteinflow)](https://anaconda.org/adaptyvbio/proteinflow)
 [![Docker Image Version (latest semver)](https://img.shields.io/docker/v/adaptyvbio/proteinflow?label=docker)](https://hub.docker.com/r/adaptyvbio/proteinflow/tags)
 ![Generic badge](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)
 
 
-ProteinFlow is an open-source Python library that streamlines the pre-processing of protein structure data for deep learning applications. ProteinFlow enables users to efficiently filter, cluster, and generate new datasets from resources like the Protein Data Bank (PDB).
+ProteinFlow is an open-source Python library that streamlines the pre-processing of protein structure data for deep learning applications. ProteinFlow enables users to efficiently filter, cluster, and generate new datasets from resources like the Protein Data Bank (PDB) and SAbDab (The Structural Antibody Database).
 
 Here are some of the key features we currently support:
 
 - ⛓️ Processing of both single-chain and multi-chain protein structures (Biounit PDB definition)
 - 🏷️ Various featurization options can be computed, including secondary structure features, torsion angles, etc.
 - 💾 A variety of data loading options and conversions to cater to different downstream training frameworks
 - 🧬 Access to up-to-date, pre-computed protein structure datasets
@@ -83,31 +83,39 @@
 ```bash
 proteinflow generate --tag new --resolution_thr 5 --pdb_snapshot 20190101 --not_filter_methods --min_seq_id 0.4 --max_length 1000 --min_length 5 --missing_ends_thr 0.1 --valid_split 0.1
 ```
 See the [docs](https://adaptyvbio.github.io/ProteinFlow/) (or `proteinflow generate --help`) for the full list of parameters and more information.
 
 A registry of all the files that are removed during the filtering as well as description with the reason for their removal is created automatically for each `generate` command. The log files are save (at `data/logs` by default) and a summary can be accessed running `proteinflow get_summary {log_path}`.
 
+You can also use the `--sabdab` option to load files from SAbDab and cluster them based on CDRs. Use together with `--zip_path` to process a custom SAbDab-like zip file.
+
 ### Splitting
 By default, both `proteinflow generate` and `proteinflow download` will also split your data into training, test and validation according to MMseqs2 clustering and homomer/heteromer/single chain proportions. However, you can skip this step with a `--skip_splitting` flag and then perform it separately with the `proteinflow split` command.
 
 The following command will perform the splitting with a 10% validation set, a 5% test set and a 50% threshold for sequence identity clusters.
 ```bash
 proteinflow split --tag new --valid_split 0.1 --test_split 0.5 --min_seq_id 0.5
 ```
 
+Use the `--exclude_chains` and `--exclude_threshold` parameters to move all biounits that contain chains similar to what you specify to a separate folder.
+
 ### Using the data
 The output files are pickled nested dictionaries where first-level keys are chain Ids and second-level keys are the following:
 - `'crd_bb'`: a `numpy` array of shape `(L, 4, 3)` with backbone atom coordinates (N, C, CA, O),
 - `'crd_sc'`: a `numpy` array of shape `(L, 10, 3)` with sidechain atom coordinates (check `proteinflow.sidechain_order()` for the order of atoms),
 - `'msk'`: a `numpy` array of shape `(L,)` where ones correspond to residues with known coordinates and
     zeros to missing values,
 - `'seq'`: a string of length `L` with residue types.
 
-Once your data is ready, you can open the files directly with `pickle` to access this data.
+In a SAbDab datasets, an additional key is added to the dictionary:
+- `'cdr'`: a `'numpy'` array of shape `(L,)` where CDR residues are marked with the corresponding type (`'H1'`, `'L1'`, ...) 
+    and non-CDR residues are marked with `'-'`.
+
+Once your data is ready, you can open the files with `pickle`.
 
 ```python
 import pickle
 import os
 
 train_folder = "./data/proteinflow_new/training"
 for filename in os.listdir(train_folder):
@@ -144,18 +152,18 @@
     ...
 ```
 See more details on available parameters and the data format in the [docs](https://adaptyvbio.github.io/ProteinFlow/) + [this repository](https://github.com/adaptyvbio/ProteinFlow-models) for a use case.
 
 ## ProteinFlow Stable Releases
 You can download them with `proteinflow download --tag {tag}` in the command line or browse in the [interface](https://proteinflow-datasets.s3.eu-west-1.amazonaws.com/index.html).
 
-|Tag    |Date    |Snapshot|Size|Min res|Min len|Max len|MMseqs thr|Split (train/val/test)|Missing thr (ends/middle)|Note|
-|-------|--------|--------|----|-------|-------|-------|----------|----------------------|-------------------------|----|
-|paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|first release, no mmCIF files|
-|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/5|0.3/0.1| v1.1.1|
+|Tag    |Date    |Snapshot|Size|Min res|Min len|Max len|MMseqs thr|Split (train/val/test)|Missing thr (ends/middle)|Source|Note|
+|-------|--------|--------|----|-------|-------|-------|----------|----------------------|-------------------------|---|----|
+|paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|first release, no mmCIF files|
+|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|v1.1.1|
 
 ## License
 The `proteinflow` package and data are released and distributed under the BSD 3-Clause License
 
 
 ## Contributions
 This is an open source project supported by [Adaptyv Bio](https://www.adaptyvbio.com/). Contributions, suggestions and bug-fixes are welcomed.
```

#### html2text {}

```diff
@@ -8,76 +8,83 @@
 proteinflow)](https://anaconda.org/adaptyvbio/proteinflow) [![Docker Image
 Version (latest semver)](https://img.shields.io/docker/v/adaptyvbio/
 proteinflow?label=docker)](https://hub.docker.com/r/adaptyvbio/proteinflow/
 tags) ![Generic badge](https://img.shields.io/badge/Contributions-Welcome-
 brightgreen.svg) ProteinFlow is an open-source Python library that streamlines
 the pre-processing of protein structure data for deep learning applications.
 ProteinFlow enables users to efficiently filter, cluster, and generate new
-datasets from resources like the Protein Data Bank (PDB). Here are some of the
-key features we currently support: - âï¸ Processing of both single-chain and
-multi-chain protein structures (Biounit PDB definition) - ð·ï¸ Various
-featurization options can be computed, including secondary structure features,
-torsion angles, etc. - ð¾ A variety of data loading options and conversions
-to cater to different downstream training frameworks - ð§¬ Access to up-to-
-date, pre-computed protein structure datasets ![overview](https://
-raw.githubusercontent.com/adaptyvbio/ProteinFlow/main/media/pf-1.png) --- ##
-Installation conda: ```bash # This should take a few minutes, be patient conda
-install -c conda-forge -c bioconda -c adaptyvbio proteinflow ``` pip: ```bash
-pip install proteinflow ``` docker: ```bash docker pull adaptyvbio/proteinflow
-``` ### Troubleshooting - If you are using python 3.10 and encountering
-installation problems, try running `python -m pip install prody==2.4.0` before
-installing `proteinflow`. - If you are planning to generate new datasets and
-installed `proteinflow` with `pip`, you will need to additionally install
-[`mmseqs`](https://github.com/soedinglab/MMseqs2). - Generating new datasets
-also depends on the `rcsbsearch` package and the latest release [v0.2.3](https:
-//github.com/sbliven/rcsbsearch/releases/tag/v0.2.3) is currently not working
-correctly. The recommended fix is installing the version from [this pull
-request](https://github.com/sbliven/rcsbsearch/pull/6). ```bash python -m pip
-install "rcsbsearch @ git+https://github.com/sbliven/
-rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e" ``` - The docker image can
-be accessed in interactive mode with this command. ```bash docker run -it -v /
-path/to/data:/media adaptyvbio/proteinflow bash ``` ## Usage ### Downloading
-pre-computed datasets (stable) Already precomputed datasets with consensus set
-of parameters and can be accessed and downloaded using the `proteinflow`.
-package. Check the output of `proteinflow check_tags` for a list of available
-tags. ```bash proteinflow download --tag 20230102_stable ``` ### Running the
-pipeline You can also run `proteinflow` with your own parameters. Check the
-output of `proteinflow check_snapshots` for a list of available PDB snapshots
-(naming rule: `yyyymmdd`). For instance, let's generate a dataset with the
-following description: - resolution threshold: 5 angstrom, - PDB snapshot:
-20190101, - structure methods accepted: all (x-ray christolography, NRM, Cryo-
-EM), - sequence identity threshold for clustering: 40% sequence similarity, -
-maximum length per sequence: 1000 residues, - minimum length per sequence: 5
-residues, - maximum fraction of missing values at the ends: 10%, - size of
-validation subset: 10%. ```bash proteinflow generate --tag new --resolution_thr
-5 --pdb_snapshot 20190101 --not_filter_methods --min_seq_id 0.4 --max_length
-1000 --min_length 5 --missing_ends_thr 0.1 --valid_split 0.1 ``` See the [docs]
-(https://adaptyvbio.github.io/ProteinFlow/) (or `proteinflow generate --help`)
-for the full list of parameters and more information. A registry of all the
-files that are removed during the filtering as well as description with the
-reason for their removal is created automatically for each `generate` command.
-The log files are save (at `data/logs` by default) and a summary can be
-accessed running `proteinflow get_summary {log_path}`. ### Splitting By
-default, both `proteinflow generate` and `proteinflow download` will also split
-your data into training, test and validation according to MMseqs2 clustering
-and homomer/heteromer/single chain proportions. However, you can skip this step
-with a `--skip_splitting` flag and then perform it separately with the
-`proteinflow split` command. The following command will perform the splitting
-with a 10% validation set, a 5% test set and a 50% threshold for sequence
-identity clusters. ```bash proteinflow split --tag new --valid_split 0.1 --
-test_split 0.5 --min_seq_id 0.5 ``` ### Using the data The output files are
-pickled nested dictionaries where first-level keys are chain Ids and second-
-level keys are the following: - `'crd_bb'`: a `numpy` array of shape `(L, 4,
-3)` with backbone atom coordinates (N, C, CA, O), - `'crd_sc'`: a `numpy` array
-of shape `(L, 10, 3)` with sidechain atom coordinates (check
-`proteinflow.sidechain_order()` for the order of atoms), - `'msk'`: a `numpy`
-array of shape `(L,)` where ones correspond to residues with known coordinates
-and zeros to missing values, - `'seq'`: a string of length `L` with residue
-types. Once your data is ready, you can open the files directly with `pickle`
-to access this data. ```python import pickle import os train_folder = "./data/
+datasets from resources like the Protein Data Bank (PDB) and SAbDab (The
+Structural Antibody Database). Here are some of the key features we currently
+support: - âï¸ Processing of both single-chain and multi-chain protein
+structures (Biounit PDB definition) - ð·ï¸ Various featurization options can
+be computed, including secondary structure features, torsion angles, etc. -
+ð¾ A variety of data loading options and conversions to cater to different
+downstream training frameworks - ð§¬ Access to up-to-date, pre-computed
+protein structure datasets ![overview](https://raw.githubusercontent.com/
+adaptyvbio/ProteinFlow/main/media/pf-1.png) --- ## Installation conda: ```bash
+# This should take a few minutes, be patient conda install -c conda-forge -
+c bioconda -c adaptyvbio proteinflow ``` pip: ```bash pip install proteinflow
+``` docker: ```bash docker pull adaptyvbio/proteinflow ``` ### Troubleshooting
+- If you are using python 3.10 and encountering installation problems, try
+running `python -m pip install prody==2.4.0` before installing `proteinflow`. -
+If you are planning to generate new datasets and installed `proteinflow` with
+`pip`, you will need to additionally install [`mmseqs`](https://github.com/
+soedinglab/MMseqs2). - Generating new datasets also depends on the `rcsbsearch`
+package and the latest release [v0.2.3](https://github.com/sbliven/rcsbsearch/
+releases/tag/v0.2.3) is currently not working correctly. The recommended fix is
+installing the version from [this pull request](https://github.com/sbliven/
+rcsbsearch/pull/6). ```bash python -m pip install "rcsbsearch @ git+https://
+github.com/sbliven/rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e" ``` -
+The docker image can be accessed in interactive mode with this command. ```bash
+docker run -it -v /path/to/data:/media adaptyvbio/proteinflow bash ``` ## Usage
+### Downloading pre-computed datasets (stable) Already precomputed datasets
+with consensus set of parameters and can be accessed and downloaded using the
+`proteinflow`. package. Check the output of `proteinflow check_tags` for a list
+of available tags. ```bash proteinflow download --tag 20230102_stable ``` ###
+Running the pipeline You can also run `proteinflow` with your own parameters.
+Check the output of `proteinflow check_snapshots` for a list of available PDB
+snapshots (naming rule: `yyyymmdd`). For instance, let's generate a dataset
+with the following description: - resolution threshold: 5 angstrom, - PDB
+snapshot: 20190101, - structure methods accepted: all (x-ray christolography,
+NRM, Cryo-EM), - sequence identity threshold for clustering: 40% sequence
+similarity, - maximum length per sequence: 1000 residues, - minimum length per
+sequence: 5 residues, - maximum fraction of missing values at the ends: 10%, -
+size of validation subset: 10%. ```bash proteinflow generate --tag new --
+resolution_thr 5 --pdb_snapshot 20190101 --not_filter_methods --min_seq_id 0.4
+--max_length 1000 --min_length 5 --missing_ends_thr 0.1 --valid_split 0.1 ```
+See the [docs](https://adaptyvbio.github.io/ProteinFlow/) (or `proteinflow
+generate --help`) for the full list of parameters and more information. A
+registry of all the files that are removed during the filtering as well as
+description with the reason for their removal is created automatically for each
+`generate` command. The log files are save (at `data/logs` by default) and a
+summary can be accessed running `proteinflow get_summary {log_path}`. You can
+also use the `--sabdab` option to load files from SAbDab and cluster them based
+on CDRs. Use together with `--zip_path` to process a custom SAbDab-like zip
+file. ### Splitting By default, both `proteinflow generate` and `proteinflow
+download` will also split your data into training, test and validation
+according to MMseqs2 clustering and homomer/heteromer/single chain proportions.
+However, you can skip this step with a `--skip_splitting` flag and then perform
+it separately with the `proteinflow split` command. The following command will
+perform the splitting with a 10% validation set, a 5% test set and a 50%
+threshold for sequence identity clusters. ```bash proteinflow split --tag new -
+-valid_split 0.1 --test_split 0.5 --min_seq_id 0.5 ``` Use the `--
+exclude_chains` and `--exclude_threshold` parameters to move all biounits that
+contain chains similar to what you specify to a separate folder. ### Using the
+data The output files are pickled nested dictionaries where first-level keys
+are chain Ids and second-level keys are the following: - `'crd_bb'`: a `numpy`
+array of shape `(L, 4, 3)` with backbone atom coordinates (N, C, CA, O), -
+`'crd_sc'`: a `numpy` array of shape `(L, 10, 3)` with sidechain atom
+coordinates (check `proteinflow.sidechain_order()` for the order of atoms), -
+`'msk'`: a `numpy` array of shape `(L,)` where ones correspond to residues with
+known coordinates and zeros to missing values, - `'seq'`: a string of length
+`L` with residue types. In a SAbDab datasets, an additional key is added to the
+dictionary: - `'cdr'`: a `'numpy'` array of shape `(L,)` where CDR residues are
+marked with the corresponding type (`'H1'`, `'L1'`, ...) and non-CDR residues
+are marked with `'-'`. Once your data is ready, you can open the files with
+`pickle`. ```python import pickle import os train_folder = "./data/
 proteinflow_new/training" for filename in os.listdir(train_folder): with open
 (os.path.join(train_folder, filename), "rb") as f: data = pickle.load(f) crd_bb
 = data["crd_bb"] seq = data["seq"] ... ``` Alternatively, you can use our
 `ProteinDataset` or `ProteinLoader` classes for convenient processing. Among
 other things, they allow for feature extraction, single chain / homomer /
 heteromer filtering and randomized sampling from sequence identity clusters.
 For example, here is how we can create a data loader that: - samples a
@@ -94,15 +101,16 @@
 should be masked, 0 otherwise ... ``` See more details on available parameters
 and the data format in the [docs](https://adaptyvbio.github.io/ProteinFlow/) +
 [this repository](https://github.com/adaptyvbio/ProteinFlow-models) for a use
 case. ## ProteinFlow Stable Releases You can download them with `proteinflow
 download --tag {tag}` in the command line or browse in the [interface](https://
 proteinflow-datasets.s3.eu-west-1.amazonaws.com/index.html). |Tag |Date
 |Snapshot|Size|Min res|Min len|Max len|MMseqs thr|Split (train/val/
-test)|Missing thr (ends/middle)|Note| |-------|--------|--------|----|-------|-
-------|-------|----------|----------------------|-------------------------|----
-| |paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|first release,
-no mmCIF files| |20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/
-5|0.3/0.1| v1.1.1| ## License The `proteinflow` package and data are released
-and distributed under the BSD 3-Clause License ## Contributions This is an open
+test)|Missing thr (ends/middle)|Source|Note| |-------|--------|--------|----|--
+-----|-------|-------|----------|----------------------|-----------------------
+--|---|----| |paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/
+0.1|PDB|first release, no mmCIF files|
+|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/5|0.3/
+0.1|PDB|v1.1.1| ## License The `proteinflow` package and data are released and
+distributed under the BSD 3-Clause License ## Contributions This is an open
 source project supported by [Adaptyv Bio](https://www.adaptyvbio.com/).
 Contributions, suggestions and bug-fixes are welcomed.
```

### Comparing `proteinflow-1.3.0/proteinflow/__init__.py` & `proteinflow-1.3.1/proteinflow/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,98 +1,102 @@
 """
-Proteinflow is an open-source Python library that streamlines the pre-processing of protein structure data for deep learning applications. ProteinFlow enables users to efficiently filter, cluster, and generate new datasets from resources like the Protein Data Bank (PDB).
+ProteinFlow is an open-source Python library that streamlines the pre-processing of protein structure data for deep learning applications. ProteinFlow enables users to efficiently filter, cluster, and generate new datasets from resources like the Protein Data Bank (PDB) and SAbDab (The Structural Antibody Database).
 
 Here are some of the key features we currently support:
 
 - ⛓️ Processing of both single-chain and multi-chain protein structures (Biounit PDB definition)
 - 🏷️ Various featurization options can be computed, including secondary structure features, torsion angles, etc.
 - 💾 A variety of data loading options and conversions to cater to different downstream training frameworks
 - 🧬 Access to up-to-date, pre-computed protein structure datasets
 
 ![overview](https://raw.githubusercontent.com/adaptyvbio/ProteinFlow/main/media/pf-1.png)
 
 ---
 
 ## Installation
-Recommended: create a new `conda` environment and install `proteinflow` with `pip`. 
+conda:
 ```bash
-conda create --name proteinflow -y
-conda activate proteinflow
-python -m pip install proteinflow
+# This should take a few minutes, be patient
+conda install -c conda-forge -c bioconda -c adaptyvbio proteinflow
 ```
 
-If you are using `python 3.10` and encountering installation problems, try running `python -m pip install prody==2.4.0` before installing `proteinflow`.
-
-### Additional requirements
-In most cases, running the commands is enough. However, if you are planning to generate a new dataset, there is a couple additional requirements.
+pip:
+```bash
+pip install proteinflow
+```
 
-First, you will need to install `mmseqs`. The recommended way is to run the following command in your `conda` environment but there are alternative methods you can see [here](https://github.com/soedinglab/MMseqs2).
+docker:
 ```bash
-conda install -y -c conda-forge -c bioconda mmseqs2
+docker pull adaptyvbio/proteinflow
 ```
 
-In addition, `proteinflow` depends on the `rcsbsearch` package and the latest release [v0.2.3](https://github.com/sbliven/rcsbsearch/releases/tag/v0.2.3) is currently not working correctly. Follow the recommended fix:
+### Troubleshooting
+- If you are using python 3.10 and encountering installation problems, try running `python -m pip install prody==2.4.0` before installing `proteinflow`.
+- If you are planning to generate new datasets and installed `proteinflow` with `pip`, you will need to additionally install [`mmseqs`](https://github.com/soedinglab/MMseqs2).
+- Generating new datasets also depends on the `rcsbsearch` package and the latest release [v0.2.3](https://github.com/sbliven/rcsbsearch/releases/tag/v0.2.3) is currently not working correctly. The recommended fix is installing the version from [this pull request](https://github.com/sbliven/rcsbsearch/pull/6).
 ```bash
 python -m pip install "rcsbsearch @ git+https://github.com/sbliven/rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e"
 ```
-
-Finally, you can use our [docker image](https://hub.docker.com/r/adaptyvbio/proteinflow/tags) as an alternative.
+- The docker image can be accessed in interactive mode with this command.
 ```bash
 docker run -it -v /path/to/data:/media adaptyvbio/proteinflow bash
 ```
 
 ## Usage
-### Downloading pre-computed datasets
-We have already run the pipeline with a consensus set of parameters and saved the results at a server. You can download the resulting dataset with `proteinflow`. Check the output of `proteinflow check_tags` for a list of available tags.
+### Downloading pre-computed datasets (stable)
+Already precomputed datasets with consensus set of parameters and can be accessed and downloaded using the `proteinflow`. package. Check the output of `proteinflow check_tags` for a list of available tags.
 ```bash
-proteinflow download --tag paper 
+proteinflow download --tag 20230102_stable 
 ```
 
-See `proteinflow.download_data` (or run `proteinflow download --help`) for more information.
-
 ### Running the pipeline
-You can also run `proteinflow` with your own parameters. Check the output of `proteinflow check_snapshots` for a list of available snapshots (naming rule: `{year}{month}{day}`).
+You can also run `proteinflow` with your own parameters. Check the output of `proteinflow check_snapshots` for a list of available PDB snapshots (naming rule: `yyyymmdd`).
 
 For instance, let's generate a dataset with the following description:
-- resolution threshold 5 $\AA$,
-- PDB snapshot 20190101,
-- all structure methods accepted,
-- sequence identity threshold for clustering 40%,
-- maximum length per sequence 1000 residues,
-- minimum length per sequence 5 residues,
-- maximum fraction of missing values at the ends 10%,
-- validation subset 10%.
+- resolution threshold: 5 angstrom,
+- PDB snapshot: 20190101,
+- structure methods accepted: all (x-ray christolography, NRM, Cryo-EM),
+- sequence identity threshold for clustering: 40% sequence similarity,
+- maximum length per sequence: 1000 residues,
+- minimum length per sequence: 5 residues,
+- maximum fraction of missing values at the ends: 10%,
+- size of validation subset: 10%.
 
 ```bash
 proteinflow generate --tag new --resolution_thr 5 --pdb_snapshot 20190101 --not_filter_methods --min_seq_id 0.4 --max_length 1000 --min_length 5 --missing_ends_thr 0.1 --valid_split 0.1
 ```
-See `proteinflow.generate_data` (or run `proteinflow generate --help`) for the full list of parameters and more information.
+See the [docs](https://adaptyvbio.github.io/ProteinFlow/) (or `proteinflow generate --help`) for the full list of parameters and more information.
+
+A registry of all the files that are removed during the filtering as well as description with the reason for their removal is created automatically for each `generate` command. The log files are save (at `data/logs` by default) and a summary can be accessed running `proteinflow get_summary {log_path}`.
 
-The reasons for filtering files out are logged in text files (at `data/logs` by default). To get a summary, run `proteinflow get_summary {log_path}`.
+You can also use the `--sabdab` option to load files from SAbDab and cluster them based on CDRs. Use together with `--zip_path` to process a custom SAbDab-like zip file.
 
 ### Splitting
 By default, both `proteinflow generate` and `proteinflow download` will also split your data into training, test and validation according to MMseqs2 clustering and homomer/heteromer/single chain proportions. However, you can skip this step with a `--skip_splitting` flag and then perform it separately with the `proteinflow split` command.
 
 The following command will perform the splitting with a 10% validation set, a 5% test set and a 50% threshold for sequence identity clusters.
 ```bash
 proteinflow split --tag new --valid_split 0.1 --test_split 0.5 --min_seq_id 0.5
 ```
 
-See `proteinflow.split_data` (or run `proteinflow split --help`) for more information.
+Use the `--exclude_chains` and `--exclude_threshold` parameters to move all biounits that contain chains similar to what you specify to a separate folder.
 
 ### Using the data
 The output files are pickled nested dictionaries where first-level keys are chain Ids and second-level keys are the following:
-
 - `'crd_bb'`: a `numpy` array of shape `(L, 4, 3)` with backbone atom coordinates (N, C, CA, O),
 - `'crd_sc'`: a `numpy` array of shape `(L, 10, 3)` with sidechain atom coordinates (check `proteinflow.sidechain_order()` for the order of atoms),
 - `'msk'`: a `numpy` array of shape `(L,)` where ones correspond to residues with known coordinates and
     zeros to missing values,
 - `'seq'`: a string of length `L` with residue types.
 
-Once your data is ready, you can open the files directly with `pickle` to access this data.
+In a SAbDab datasets, an additional key is added to the dictionary:
+- `'cdr'`: a `'numpy'` array of shape `(L,)` where CDR residues are marked with the corresponding type (`'H1'`, `'L1'`, ...) 
+    and non-CDR residues are marked with `'-'`.
+
+Once your data is ready, you can open the files with `pickle`.
 
 ```python
 import pickle
 import os
 
 train_folder = "./data/proteinflow_new/training"
 for filename in os.listdir(train_folder):
@@ -106,37 +110,33 @@
 Alternatively, you can use our `ProteinDataset` or `ProteinLoader` classes 
 for convenient processing. Among other things, they allow for feature extraction, single chain / homomer / heteromer filtering and randomized sampling from sequence identity clusters.
 
 For example, here is how we can create a data loader that:
 - samples a different cluster representative at every epoch,
 - extracts dihedral angles, sidechain orientation and secondary structure features,
 - only loads pairs of interacting proteins (larger biounits are broken up into pairs),
-- generates a geometric mask for 10% of one of the chains (random generation at every pass),
 - has batch size 8.
 
 ```python
 from proteinflow import ProteinLoader
 train_loader = ProteinLoader.from_args(
     "./data/proteinflow_new/training", 
     clustering_dict_path="./data/proteinflow_new/splits_dict/train.pickle",
     node_features_type="dihedral+sidechain_orientation+secondary_structure",
     entry_type="pair",
-    mask_frac=0.1,
     batch_size=8,
 )
 for batch in train_loader:
     crd_bb = batch["X"] #(B, L, 4, 3)
     seq = batch["S"] #(B, L)
     sse = batch["secondary_structure"] #(B, L, 3)
     to_predict = batch["masked_res"] #(B, L), 1 where the residues should be masked, 0 otherwise
     ...
 ```
 
-See `proteinflow.ProteinLoader` for more information.
-
 """
 
 __pdoc__ = {"utils": False, "scripts": False}
 __docformat__ = "numpy"
 
 from proteinflow.utils.filter_database import _remove_database_redundancies
 from proteinflow.utils.process_pdb import (
@@ -187,14 +187,15 @@
 from editdistance import eval as edit_distance
 import requests
 import zipfile
 from bs4 import BeautifulSoup
 import urllib.request
 import string
 from einops import rearrange
+import tempfile
 
 MAIN_ATOMS = {
     "GLY": None,
     "ALA": 0,
     "VAL": 0,
     "LEU": 1,
     "ILE": 1,
@@ -450,29 +451,33 @@
     seq_identity_threshold=0.9,
     n=None,
     force=False,
     tag=None,
     pdb_snapshot=None,
     load_live=False,
     sabdab=False,
-    zip_path=None,
+    sabdab_data_path=None,
     require_antigen=False,
 ):
     """
     Download and parse PDB files that meet filtering criteria
 
     The output files are pickled nested dictionaries where first-level keys are chain Ids and second-level keys are
     the following:
 
     - `'crd_bb'`: a `numpy` array of shape `(L, 4, 3)` with backbone atom coordinates (N, C, CA, O),
     - `'crd_sc'`: a `numpy` array of shape `(L, 10, 3)` with sidechain atom coordinates (in a fixed order, check `sidechain_order()`),
     - `'msk'`: a `numpy` array of shape `(L,)` where ones correspond to residues with known coordinates and
         zeros to missing values,
     - `'seq'`: a string of length `L` with residue types.
 
+    When creating a SAbDab dataset, an additional key is added to the dictionary:
+    - `'cdr'`: a `'numpy'` array of shape `(L,)` where CDR residues are marked with the corresponding type (`'H1'`, `'L1'`, ...)
+        and non-CDR residues are marked with `'-'`.
+
     All errors including reasons for filtering a file out are logged in a log file.
 
     Parameters
     ----------
     tmp_folder : str, default "./data/tmp_pdb"
         The folder where temporary files will be saved
     output_folder : str, default "./data/pdb"
@@ -513,16 +518,16 @@
         A tag to add to the log file
     pdb_snapshot : str, optional
         the PDB snapshot to use, by default the latest is used (if `sabdab` is `True`, you can use any date in the format YYYYMMDD as a cutoff)
     load_live : bool, default False
         if `True`, load the files that are not in the latest PDB snapshot from the PDB FTP server (forced to `False` if `pdb_snapshot` is not `None`)
     sabdab : bool, default False
         if `True`, download the SAbDab database instead of PDB
-    zip_path : str, optional
-        path to a zip file containing SAbDab files (only used if `sabdab` is `True`)
+    sabdab_data_path : str, optional
+        path to a zip file or a directory containing SAbDab files (only used if `sabdab` is `True`)
     require_antigen : bool, default False
         if `True`, only keep files with antigen chains (only used if `sabdab` is `True`)
 
     Returns
     -------
     log : dict
         a dictionary where keys are recognized error names and values are lists of PDB ids that caused the errors
@@ -603,15 +608,15 @@
             filter_methods=filter_methods,
             pdb_snapshot=pdb_snapshot,
             log_folder=log_folder,
             n=n,
             tmp_folder=TMP_FOLDER,
             load_live=load_live,
             sabdab=sabdab,
-            zip_path=zip_path,
+            sabdab_data_path=sabdab_data_path,
             require_antigen=require_antigen,
         )
         for id in error_ids:
             with open(LOG_FILE, "a") as f:
                 f.write(f"<<< Could not download PDB/mmCIF file: {id} \n")
         # for x in [("data/tmp/5ivn.pdb", "A_nan_B")]:
         #     process_f(x, show_error=True, force=force, sabdab=True)
@@ -1029,15 +1034,15 @@
 
 
 def _load_sabdab(
     resolution_thr=3.5,
     filter_methods=True,
     pdb_snapshot=None,
     tmp_folder="data/tmp",
-    zip_path=None,
+    sabdab_data_path=None,
     require_antigen=True,
     n=None,
 ):
     """
     Download filtered SAbDab files and return a list of local file paths
     """
 
@@ -1046,15 +1051,15 @@
     if pdb_snapshot is not None:
         pdb_snapshot = datetime.strptime(pdb_snapshot, "%Y%m%d")
     if filter_methods:
         methods = ["X-RAY DIFFRACTION", "ELECTRON MICROSCOPY"]
     else:
         methods = ["All"]
     methods = [x.split() for x in methods]
-    if zip_path is None:
+    if sabdab_data_path is None:
         for method in methods:
             html = _make_sabdab_html(method, resolution_thr)
             page = requests.get(html)
             soup = BeautifulSoup(page.text, "html.parser")
             try:
                 zip_ref = soup.find_all(
                     lambda t: t.name == "a" and t.text.startswith("zip")
@@ -1074,29 +1079,40 @@
                 [
                     "wget",
                     zip_ref,
                     "-O",
                     os.path.join(tmp_folder, f"pdb_{'_'.join(method)}.zip"),
                 ]
             )
-        zip_paths = [
+        paths = [
             os.path.join(tmp_folder, f"pdb_{'_'.join(method)}.zip")
             for method in methods
         ]
     else:
-        zip_paths = [zip_path]
+        paths = [sabdab_data_path]
     ids = []
     pdb_ids = []
     print("Moving files...")
-    for path in zip_paths:
-        dir_path = path[:-4]
-        with zipfile.ZipFile(path, "r") as zip_ref:
-            zip_ref.extractall(dir_path)
-        if zip_path is None:
-            os.remove(path)
+    for path in paths:
+        if not os.path.isdir(path):
+            if not path.endswith(".zip"):
+                raise ValueError("SAbDab data path should be a zip file or a directory")
+            dir_path = path[:-4]
+            print(f"Unzipping {path}...")
+            with zipfile.ZipFile(path, "r") as zip_ref:
+                for member in tqdm(zip_ref.infolist()):
+                    try:
+                        zip_ref.extract(member, dir_path)
+                    except zipfile.error as e:
+                        pass
+            if sabdab_data_path is None:
+                os.remove(path)
+        else:
+            dir_path = path
+        print("Filtering...")
         summary_path = None
         for file in os.listdir(dir_path):
             if file.endswith(".tsv"):
                 summary_path = os.path.join(dir_path, file)
                 break
         if summary_path is None:
             raise ValueError("Summary file not found")
@@ -1106,27 +1122,31 @@
         summary = summary[summary["antigen_chain"] != summary["Lchain"]]
         summary = summary[summary["Lchain"] != summary["Hchain"]]
         if require_antigen:
             summary = summary[~summary["antigen_chain"].isna()]
         if pdb_snapshot is not None:
             date = pd.to_datetime(summary["date"], format="%m/%d/%Y")
             summary = summary[date <= pdb_snapshot]
-        if zip_path is not None:
-            summary = summary[summary["resolution"] <= resolution_thr]
+        if sabdab_data_path is not None:
+            summary.loc[summary["resolution"] == "NOT", "resolution"] = 0
+            if summary["resolution"].dtype != float:
+                summary["resolution"] = summary["resolution"].str.split(", ").str[0]
+            summary = summary[summary["resolution"].astype(float) <= resolution_thr]
             if filter_methods:
                 summary = summary[
                     summary["method"].isin([" ".join(m) for m in methods])
                 ]
         if n is not None:
             summary = summary.iloc[:n]
         ids_method = summary["pdb"].unique().tolist()
-        for id in ids_method:
+        for id in tqdm(ids_method):
             pdb_path = os.path.join(dir_path, "chothia", f"{id}.pdb")
             shutil.move(pdb_path, os.path.join(tmp_folder, f"{id}.pdb"))
-        shutil.rmtree(dir_path)
+        if sabdab_data_path is None or sabdab_data_path.endswith(".zip"):
+            shutil.rmtree(dir_path)
         ids_full = summary.apply(
             lambda x: (x["pdb"], f"{x['Hchain']}_{x['Lchain']}_{x['antigen_chain']}"),
             axis=1,
         ).tolist()
         ids += ids_full
         pdb_ids += ids_method
     print("Downloading fasta files...")
@@ -1151,28 +1171,28 @@
     pdb_snapshot=None,
     filter_methods=True,
     log_folder="data/tmp/logs",
     n=None,
     tmp_folder="data/tmp",
     load_live=False,
     sabdab=False,
-    zip_path=None,
+    sabdab_data_path=None,
     require_antigen=False,
 ):
     """
     Download filtered structure files and return a list of local file paths
     """
 
     if sabdab:
         out = _load_sabdab(
             resolution_thr=resolution_thr,
             filter_methods=filter_methods,
             pdb_snapshot=pdb_snapshot,
             tmp_folder=tmp_folder,
-            zip_path=zip_path,
+            sabdab_data_path=sabdab_data_path,
             require_antigen=require_antigen,
             n=n,
         )
     else:
         out = _load_pdb(
             resolution_thr=resolution_thr,
             filter_methods=filter_methods,
@@ -1195,17 +1215,17 @@
         the name of the dataset to load
     local_datasets_folder : str, default "./data"
         the path to the folder that will store proteinflow datasets, logs and temporary files
     skip_splitting : bool, default False
         if `True`, skip the split dictionary creation and the file moving steps
     """
 
-    data_path = _download_dataset(tag, local_datasets_folder)
+    sabdab_data_path = _download_dataset(tag, local_datasets_folder)
     if not skip_splitting:
-        _split_data(data_path)
+        _split_data(sabdab_data_path)
 
 
 def generate_data(
     tag,
     local_datasets_folder="./data",
     min_length=30,
     max_length=10000,
@@ -1221,31 +1241,43 @@
     split_tolerance=0.2,
     test_split=0.05,
     valid_split=0.05,
     pdb_snapshot=None,
     load_live=False,
     min_seq_id=0.3,
     sabdab=False,
-    zip_path=None,
+    sabdab_data_path=None,
     require_antigen=False,
+    exclude_chains=None,
+    exclude_threshold=0.7,
+    exclude_clusters=False,
+    exclude_based_on_cdr=None,
 ):
     """
     Download and parse PDB files that meet filtering criteria
 
     The output files are pickled nested dictionaries where first-level keys are chain Ids and second-level keys are
     the following:
 
     - `'crd_bb'`: a `numpy` array of shape `(L, 4, 3)` with backbone atom coordinates (N, C, CA, O),
     - `'crd_sc'`: a `numpy` array of shape `(L, 10, 3)` with sidechain atom coordinates (in a fixed order, check `sidechain_order()`),
     - `'msk'`: a `numpy` array of shape `(L,)` where ones correspond to residues with known coordinates and
         zeros to missing values,
     - `'seq'`: a string of length `L` with residue types.
 
+    When creating a SAbDab dataset, an additional key is added to the dictionary:
+    - `'cdr'`: a `'numpy'` array of shape `(L,)` where CDR residues are marked with the corresponding type (`'H1'`, `'L1'`, ...)
+        and non-CDR residues are marked with `'-'`.
+
+    PDB datasets are split into clusters according to sequence identity and SAbDab datasets are split according to CDR similarity.
+
     All errors including reasons for filtering a file out are logged in the log file.
 
+    For more information on the splitting procedure and options, check out the `proteinflow.split_data` documentation.
+
     Parameters
     ----------
     tag : str
         the name of the dataset to load
     local_datasets_folder : str, default "./data"
         the path to the folder that will store proteinflow datasets, logs and temporary files
     min_length : int, default 30
@@ -1280,19 +1312,26 @@
         the PDB snapshot to use, by default the latest is used
     load_live : bool, default False
         if `True`, load the files that are not in the latest PDB snapshot from the PDB FTP server (forced to `False` if `pdb_snapshot` is not `None`)
     min_seq_id : float in [0, 1], default 0.3
         minimum sequence identity for `mmseqs`
     sabdab : bool, default False
         if `True`, download the SAbDab database instead of PDB
-    zip_path : str, optional
-        path to a zip file containing SAbDab files (only used if `sabdab` is `True`)
+    sabdab_data_path : str, optional
+        path to a zip file or a directory containing SAbDab files (only used if `sabdab` is `True`)
     require_antigen : bool, default False
         if `True`, only use SAbDab files with an antigen
-
+    exclude_chains : list of str, optional
+        a list of chains (`{pdb_id}-{chain_id}`) to exclude from the splitting (e.g. `["1A2B-A", "1A2B-B"]`); chain id is the author chain id
+    exclude_threshold : float in [0, 1], default 0.7
+        the sequence similarity threshold for excluding chains
+    exclude_clusters : bool, default False
+        if `True`, exclude clusters that contain chains similar to chains in the `exclude_chains` list
+    exclude_based_on_cdr : {"H1", "H2", "H3", "L1", "L2", "L3"}, optional
+        if given and `exclude_clusters` is `True` + the dataset is SAbDab, exclude files based on only the given CDR clusters
 
     Returns
     -------
     log : dict
         a dictionary where keys are recognized error names and values are lists of PDB ids that caused the errors
 
     """
@@ -1324,29 +1363,31 @@
         seq_identity_threshold=seq_identity_threshold,
         n=n,
         force=force,
         tag=tag,
         pdb_snapshot=pdb_snapshot,
         load_live=load_live,
         sabdab=sabdab,
-        zip_path=zip_path,
+        sabdab_data_path=sabdab_data_path,
         require_antigen=require_antigen,
     )
     if not skip_splitting:
-        _get_split_dictionaries(
-            tmp_folder=tmp_folder,
-            output_folder=output_folder,
+        split_data(
+            tag=tag,
+            local_datasets_folder=local_datasets_folder,
             split_tolerance=split_tolerance,
             test_split=test_split,
             valid_split=valid_split,
-            out_split_dict_folder=out_split_dict_folder,
+            ignore_existing=True,
             min_seq_id=min_seq_id,
+            exclude_chains=exclude_chains,
+            exclude_threshold=exclude_threshold,
+            exclude_clusters=exclude_clusters,
+            exclude_based_on_cdr=exclude_based_on_cdr,
         )
-
-        _split_data(output_folder)
     shutil.rmtree(tmp_folder)
     return log_dict
 
 
 def _get_excluded_files(
     tag, local_datasets_folder, tmp_folder, exclude_chains, exclude_threshold
 ):
@@ -1436,17 +1477,21 @@
 
     1. cluster chains by sequence identity,
     2. generate a graph where nodes are the clusters and edges are protein-protein interactions between chains
     from those clusters,
     3. split connected components of the graph into training, test and validation subsets while keeping the proportion
     of single chains, homomers and heteromers close to that in the full dataset (within `split_tolerance`).
 
-    Biounits that contain chains similar to those in the `exclude_chains` list (with `exclude_threshold` sequence identity)
-    are excluded from the splitting and placed into a separate folder.
+    For SAbDab datasets, instead of sequence identity, we use CDR cluster identity to cluster chains. We also connect the clusters
+    in the graph if CDRs from those clusters are seen in the same PDB.
 
+    Biounits that contain chains similar to those in the `exclude_chains` list (with `exclude_threshold` sequence identity)
+    are excluded from the splitting and placed into a separate folder. If you want to exclude clusters containing those chains
+    as well, set `exclude_clusters` to `True`. For SAbDab datasets, you can additionally choose to only exclude based on specific
+    CDR clusters. To do so, set `exclude_based_on_cdr` to the CDR type.
 
     Parameters
     ----------
     tag : str
         the name of the dataset to load
     local_datasets_folder : str, default "./data"
         the path to the folder that will store proteinflow datasets, logs and temporary files
@@ -1539,17 +1584,19 @@
 
     - `'sidechain_orientation'`: a unit vector in the direction of the sidechain, `(total_L, 3)`,
     - `'dihedral'`: the dihedral angles, `(total_L, 2)`,
     - `'chemical'`: hydropathy, volume, charge, polarity, acceptor/donor features, `(total_L, 6)`,
     - `'secondary_structure'`: a one-hot encoding of secondary structure ([alpha-helix, beta-sheet, coil]), `(total_L, 3)`,
     - `'sidechain_coords'`: the coordinates of the sidechain atoms (see `proteinflow.sidechain_order()` for the order), `(total_L, 10, 3)`.
 
-    If the dataset contains a `'cdr'` key, the output files will also additionally contain a `'cdr'` key with a CDR tensor of length `total_L`.
-    In the array, the CDR residues are marked with the corresponding CDR type (H1=1, H2=2, H3=3, L1=4, L2=5, L3=6) and the rest of
-    the residues are marked with 0s.
+    If the dataset contains a `'cdr'` key (if it was generated from SAbDab files), the output files will also additionally contain a `'cdr'`
+    key with a CDR tensor of length `total_L`. In the array, the CDR residues are marked with the corresponding CDR type
+    (H1=1, H2=2, H3=3, L1=4, L2=5, L3=6) and the rest of the residues are marked with 0s.
+
+    Use the `set_cdr` method to only iterate over biounits that contain specific CDRs.
 
     In order to compute additional features, use the `feature_functions` parameter. It should be a dictionary with keys
     corresponding to the feature names and values corresponding to the functions that compute the features. The functions
     should take a chain dictionary and an integer representation of the sequence as input (the dictionary is in `proteinflow` format,
     see the docs for `generate_data` for details) and return a `numpy` array shaped as `(#residues, #features)`.
 
     """
@@ -1736,14 +1783,17 @@
                 for chain, file_list in self.files[id].items():
                     for file in file_list:
                         if file in seen:
                             continue
                         seen.add(file)
                         with open(file, "rb") as f:
                             self.loaded[file] = pickle.load(f)
+        sample_file = list(self.files.keys())[0]
+        sample_chain = list(self.files[sample_file].keys())[0]
+        self.sabdab = "__" in sample_chain
         self.cdr = 0
         self.set_cdr(None)
 
     def _interpolate(self, crd_i, mask_i):
         """
         Fill in missing values in the middle with linear interpolation and (if fill_ends is true) build an initialization for the ends
 
@@ -2056,14 +2106,25 @@
             for key, value_list in node_features.items():
                 out[key] = torch.from_numpy(np.concatenate(value_list))
             with open(output_file, "wb") as f:
                 pickle.dump(out, f)
         return output_names
 
     def set_cdr(self, cdr):
+        """
+        Set the CDR to be iterated over (only for SAbDab datasets).
+
+        Parameters
+        ----------
+        cdr : str
+            The CDR to be iterated over. Set to `None` to go back to iterating over all chains.
+        """
+
+        if not self.sabdab:
+            cdr = None
         if cdr == self.cdr:
             return
         self.cdr = cdr
         if cdr is None:
             self.indices = list(range(len(self.data)))
         else:
             self.indices = []
@@ -2127,28 +2188,29 @@
 
 
 class ProteinLoader(DataLoader):
     """
     A subclass of `torch.data.utils.DataLoader` tuned for the `proteinflow` dataset
 
     Creates and iterates over an instance of `ProteinDataset`, omitting the `'chain_dict'` keys.
-    See the `ProteinDataset` docs for more information.
+    See the `ProteinDataset` documentation for more information.
 
     If batch size is larger than one, all objects are padded with zeros at the ends to reach the length of the
     longest protein in the batch.
 
     If `mask_residues` is `True`, an additional `'masked_res'` key is added to the output. The value is a binary
     tensor shaped `(B, L)` where 1 denotes the part that needs to be predicted and 0 is everything else. The tensors are generated
     according to the following rules:
-    - if `mask_whole_chains` is `True`, the whole chain is masked
+    - if the dataset is generated from SAbDab files, the sampled CDR is masked,
+    - if `mask_whole_chains` is `True`, the whole chain is masked,
     - if `mask_frac` is given, the number of residues to mask is `mask_frac` times the length of the chain,
     - otherwise, the number of residues to mask is sampled uniformly from the range [`lower_limit`, `upper_limit`].
 
     If `force_binding_sites_frac` > 0 and `mask_whole_chains` is `False`, in the fraction of cases where a chain
-    from a polymer is sampled, the center of the masked region will be forced to be in a binding site.
+    from a polymer is sampled, the center of the masked region will be forced to be in a binding site (in PDB datasets).
     """
 
     def __init__(
         self,
         dataset,
         lower_limit=15,
         upper_limit=100,
```

### Comparing `proteinflow-1.3.0/proteinflow/scripts/proteinflow_cli.py` & `proteinflow-1.3.1/proteinflow/scripts/proteinflow_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,17 +140,17 @@
 )
 @click.option(
     "--sabdab",
     is_flag=True,
     help="Use this flag to generate a dataset from SAbDab files instead of PDB",
 )
 @click.option(
-    "--zip_path",
+    "--sabdab_data_path",
     type=str,
-    help="Path to a zip file containing SAbDab files (only used if `sabdab` is `True`)",
+    help="Path to a zip file or a directory containing SAbDab files (only used if `sabdab` is `True`)",
 )
 @click.option(
     "--require_antigen",
     is_flag=True,
     help="Use this flag to require that the SAbDab files contain an antigen",
 )
 @cli.command("generate", help="Generate a new ProteinFlow dataset")
```

### Comparing `proteinflow-1.3.0/proteinflow/utils/async_download.py` & `proteinflow-1.3.1/proteinflow/utils/async_download.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.0/proteinflow/utils/biotite_sse.py` & `proteinflow-1.3.1/proteinflow/utils/biotite_sse.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.0/proteinflow/utils/build_pdb.py` & `proteinflow-1.3.1/proteinflow/utils/build_pdb.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.0/proteinflow/utils/cluster_and_partition.py` & `proteinflow-1.3.1/proteinflow/utils/cluster_and_partition.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.0/proteinflow/utils/filter_database.py` & `proteinflow-1.3.1/proteinflow/utils/filter_database.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.0/proteinflow/utils/mmcif_fix.py` & `proteinflow-1.3.1/proteinflow/utils/mmcif_fix.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.0/proteinflow/utils/process_pdb.py` & `proteinflow-1.3.1/proteinflow/utils/process_pdb.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.0/proteinflow/utils/split_dataset.py` & `proteinflow-1.3.1/proteinflow/utils/split_dataset.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.0/proteinflow.egg-info/PKG-INFO` & `proteinflow-1.3.1/proteinflow.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 1.3.0
+Version: 1.3.1
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -25,15 +25,15 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI](https://img.shields.io/pypi/v/proteinflow)](https://pypi.org/project/proteinflow/)
 [![Conda](https://img.shields.io/conda/v/adaptyvbio/proteinflow)](https://anaconda.org/adaptyvbio/proteinflow)
 [![Docker Image Version (latest semver)](https://img.shields.io/docker/v/adaptyvbio/proteinflow?label=docker)](https://hub.docker.com/r/adaptyvbio/proteinflow/tags)
 ![Generic badge](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)
 
 
-ProteinFlow is an open-source Python library that streamlines the pre-processing of protein structure data for deep learning applications. ProteinFlow enables users to efficiently filter, cluster, and generate new datasets from resources like the Protein Data Bank (PDB).
+ProteinFlow is an open-source Python library that streamlines the pre-processing of protein structure data for deep learning applications. ProteinFlow enables users to efficiently filter, cluster, and generate new datasets from resources like the Protein Data Bank (PDB) and SAbDab (The Structural Antibody Database).
 
 Here are some of the key features we currently support:
 
 - ⛓️ Processing of both single-chain and multi-chain protein structures (Biounit PDB definition)
 - 🏷️ Various featurization options can be computed, including secondary structure features, torsion angles, etc.
 - 💾 A variety of data loading options and conversions to cater to different downstream training frameworks
 - 🧬 Access to up-to-date, pre-computed protein structure datasets
@@ -94,31 +94,39 @@
 ```bash
 proteinflow generate --tag new --resolution_thr 5 --pdb_snapshot 20190101 --not_filter_methods --min_seq_id 0.4 --max_length 1000 --min_length 5 --missing_ends_thr 0.1 --valid_split 0.1
 ```
 See the [docs](https://adaptyvbio.github.io/ProteinFlow/) (or `proteinflow generate --help`) for the full list of parameters and more information.
 
 A registry of all the files that are removed during the filtering as well as description with the reason for their removal is created automatically for each `generate` command. The log files are save (at `data/logs` by default) and a summary can be accessed running `proteinflow get_summary {log_path}`.
 
+You can also use the `--sabdab` option to load files from SAbDab and cluster them based on CDRs. Use together with `--zip_path` to process a custom SAbDab-like zip file.
+
 ### Splitting
 By default, both `proteinflow generate` and `proteinflow download` will also split your data into training, test and validation according to MMseqs2 clustering and homomer/heteromer/single chain proportions. However, you can skip this step with a `--skip_splitting` flag and then perform it separately with the `proteinflow split` command.
 
 The following command will perform the splitting with a 10% validation set, a 5% test set and a 50% threshold for sequence identity clusters.
 ```bash
 proteinflow split --tag new --valid_split 0.1 --test_split 0.5 --min_seq_id 0.5
 ```
 
+Use the `--exclude_chains` and `--exclude_threshold` parameters to move all biounits that contain chains similar to what you specify to a separate folder.
+
 ### Using the data
 The output files are pickled nested dictionaries where first-level keys are chain Ids and second-level keys are the following:
 - `'crd_bb'`: a `numpy` array of shape `(L, 4, 3)` with backbone atom coordinates (N, C, CA, O),
 - `'crd_sc'`: a `numpy` array of shape `(L, 10, 3)` with sidechain atom coordinates (check `proteinflow.sidechain_order()` for the order of atoms),
 - `'msk'`: a `numpy` array of shape `(L,)` where ones correspond to residues with known coordinates and
     zeros to missing values,
 - `'seq'`: a string of length `L` with residue types.
 
-Once your data is ready, you can open the files directly with `pickle` to access this data.
+In a SAbDab datasets, an additional key is added to the dictionary:
+- `'cdr'`: a `'numpy'` array of shape `(L,)` where CDR residues are marked with the corresponding type (`'H1'`, `'L1'`, ...) 
+    and non-CDR residues are marked with `'-'`.
+
+Once your data is ready, you can open the files with `pickle`.
 
 ```python
 import pickle
 import os
 
 train_folder = "./data/proteinflow_new/training"
 for filename in os.listdir(train_folder):
@@ -155,18 +163,18 @@
     ...
 ```
 See more details on available parameters and the data format in the [docs](https://adaptyvbio.github.io/ProteinFlow/) + [this repository](https://github.com/adaptyvbio/ProteinFlow-models) for a use case.
 
 ## ProteinFlow Stable Releases
 You can download them with `proteinflow download --tag {tag}` in the command line or browse in the [interface](https://proteinflow-datasets.s3.eu-west-1.amazonaws.com/index.html).
 
-|Tag    |Date    |Snapshot|Size|Min res|Min len|Max len|MMseqs thr|Split (train/val/test)|Missing thr (ends/middle)|Note|
-|-------|--------|--------|----|-------|-------|-------|----------|----------------------|-------------------------|----|
-|paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|first release, no mmCIF files|
-|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/5|0.3/0.1| v1.1.1|
+|Tag    |Date    |Snapshot|Size|Min res|Min len|Max len|MMseqs thr|Split (train/val/test)|Missing thr (ends/middle)|Source|Note|
+|-------|--------|--------|----|-------|-------|-------|----------|----------------------|-------------------------|---|----|
+|paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|first release, no mmCIF files|
+|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|v1.1.1|
 
 ## License
 The `proteinflow` package and data are released and distributed under the BSD 3-Clause License
 
 
 ## Contributions
 This is an open source project supported by [Adaptyv Bio](https://www.adaptyvbio.com/). Contributions, suggestions and bug-fixes are welcomed.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 1.3.0 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 1.3.1 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
@@ -15,76 +15,83 @@
 proteinflow)](https://anaconda.org/adaptyvbio/proteinflow) [![Docker Image
 Version (latest semver)](https://img.shields.io/docker/v/adaptyvbio/
 proteinflow?label=docker)](https://hub.docker.com/r/adaptyvbio/proteinflow/
 tags) ![Generic badge](https://img.shields.io/badge/Contributions-Welcome-
 brightgreen.svg) ProteinFlow is an open-source Python library that streamlines
 the pre-processing of protein structure data for deep learning applications.
 ProteinFlow enables users to efficiently filter, cluster, and generate new
-datasets from resources like the Protein Data Bank (PDB). Here are some of the
-key features we currently support: - âï¸ Processing of both single-chain and
-multi-chain protein structures (Biounit PDB definition) - ð·ï¸ Various
-featurization options can be computed, including secondary structure features,
-torsion angles, etc. - ð¾ A variety of data loading options and conversions
-to cater to different downstream training frameworks - ð§¬ Access to up-to-
-date, pre-computed protein structure datasets ![overview](https://
-raw.githubusercontent.com/adaptyvbio/ProteinFlow/main/media/pf-1.png) --- ##
-Installation conda: ```bash # This should take a few minutes, be patient conda
-install -c conda-forge -c bioconda -c adaptyvbio proteinflow ``` pip: ```bash
-pip install proteinflow ``` docker: ```bash docker pull adaptyvbio/proteinflow
-``` ### Troubleshooting - If you are using python 3.10 and encountering
-installation problems, try running `python -m pip install prody==2.4.0` before
-installing `proteinflow`. - If you are planning to generate new datasets and
-installed `proteinflow` with `pip`, you will need to additionally install
-[`mmseqs`](https://github.com/soedinglab/MMseqs2). - Generating new datasets
-also depends on the `rcsbsearch` package and the latest release [v0.2.3](https:
-//github.com/sbliven/rcsbsearch/releases/tag/v0.2.3) is currently not working
-correctly. The recommended fix is installing the version from [this pull
-request](https://github.com/sbliven/rcsbsearch/pull/6). ```bash python -m pip
-install "rcsbsearch @ git+https://github.com/sbliven/
-rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e" ``` - The docker image can
-be accessed in interactive mode with this command. ```bash docker run -it -v /
-path/to/data:/media adaptyvbio/proteinflow bash ``` ## Usage ### Downloading
-pre-computed datasets (stable) Already precomputed datasets with consensus set
-of parameters and can be accessed and downloaded using the `proteinflow`.
-package. Check the output of `proteinflow check_tags` for a list of available
-tags. ```bash proteinflow download --tag 20230102_stable ``` ### Running the
-pipeline You can also run `proteinflow` with your own parameters. Check the
-output of `proteinflow check_snapshots` for a list of available PDB snapshots
-(naming rule: `yyyymmdd`). For instance, let's generate a dataset with the
-following description: - resolution threshold: 5 angstrom, - PDB snapshot:
-20190101, - structure methods accepted: all (x-ray christolography, NRM, Cryo-
-EM), - sequence identity threshold for clustering: 40% sequence similarity, -
-maximum length per sequence: 1000 residues, - minimum length per sequence: 5
-residues, - maximum fraction of missing values at the ends: 10%, - size of
-validation subset: 10%. ```bash proteinflow generate --tag new --resolution_thr
-5 --pdb_snapshot 20190101 --not_filter_methods --min_seq_id 0.4 --max_length
-1000 --min_length 5 --missing_ends_thr 0.1 --valid_split 0.1 ``` See the [docs]
-(https://adaptyvbio.github.io/ProteinFlow/) (or `proteinflow generate --help`)
-for the full list of parameters and more information. A registry of all the
-files that are removed during the filtering as well as description with the
-reason for their removal is created automatically for each `generate` command.
-The log files are save (at `data/logs` by default) and a summary can be
-accessed running `proteinflow get_summary {log_path}`. ### Splitting By
-default, both `proteinflow generate` and `proteinflow download` will also split
-your data into training, test and validation according to MMseqs2 clustering
-and homomer/heteromer/single chain proportions. However, you can skip this step
-with a `--skip_splitting` flag and then perform it separately with the
-`proteinflow split` command. The following command will perform the splitting
-with a 10% validation set, a 5% test set and a 50% threshold for sequence
-identity clusters. ```bash proteinflow split --tag new --valid_split 0.1 --
-test_split 0.5 --min_seq_id 0.5 ``` ### Using the data The output files are
-pickled nested dictionaries where first-level keys are chain Ids and second-
-level keys are the following: - `'crd_bb'`: a `numpy` array of shape `(L, 4,
-3)` with backbone atom coordinates (N, C, CA, O), - `'crd_sc'`: a `numpy` array
-of shape `(L, 10, 3)` with sidechain atom coordinates (check
-`proteinflow.sidechain_order()` for the order of atoms), - `'msk'`: a `numpy`
-array of shape `(L,)` where ones correspond to residues with known coordinates
-and zeros to missing values, - `'seq'`: a string of length `L` with residue
-types. Once your data is ready, you can open the files directly with `pickle`
-to access this data. ```python import pickle import os train_folder = "./data/
+datasets from resources like the Protein Data Bank (PDB) and SAbDab (The
+Structural Antibody Database). Here are some of the key features we currently
+support: - âï¸ Processing of both single-chain and multi-chain protein
+structures (Biounit PDB definition) - ð·ï¸ Various featurization options can
+be computed, including secondary structure features, torsion angles, etc. -
+ð¾ A variety of data loading options and conversions to cater to different
+downstream training frameworks - ð§¬ Access to up-to-date, pre-computed
+protein structure datasets ![overview](https://raw.githubusercontent.com/
+adaptyvbio/ProteinFlow/main/media/pf-1.png) --- ## Installation conda: ```bash
+# This should take a few minutes, be patient conda install -c conda-forge -
+c bioconda -c adaptyvbio proteinflow ``` pip: ```bash pip install proteinflow
+``` docker: ```bash docker pull adaptyvbio/proteinflow ``` ### Troubleshooting
+- If you are using python 3.10 and encountering installation problems, try
+running `python -m pip install prody==2.4.0` before installing `proteinflow`. -
+If you are planning to generate new datasets and installed `proteinflow` with
+`pip`, you will need to additionally install [`mmseqs`](https://github.com/
+soedinglab/MMseqs2). - Generating new datasets also depends on the `rcsbsearch`
+package and the latest release [v0.2.3](https://github.com/sbliven/rcsbsearch/
+releases/tag/v0.2.3) is currently not working correctly. The recommended fix is
+installing the version from [this pull request](https://github.com/sbliven/
+rcsbsearch/pull/6). ```bash python -m pip install "rcsbsearch @ git+https://
+github.com/sbliven/rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e" ``` -
+The docker image can be accessed in interactive mode with this command. ```bash
+docker run -it -v /path/to/data:/media adaptyvbio/proteinflow bash ``` ## Usage
+### Downloading pre-computed datasets (stable) Already precomputed datasets
+with consensus set of parameters and can be accessed and downloaded using the
+`proteinflow`. package. Check the output of `proteinflow check_tags` for a list
+of available tags. ```bash proteinflow download --tag 20230102_stable ``` ###
+Running the pipeline You can also run `proteinflow` with your own parameters.
+Check the output of `proteinflow check_snapshots` for a list of available PDB
+snapshots (naming rule: `yyyymmdd`). For instance, let's generate a dataset
+with the following description: - resolution threshold: 5 angstrom, - PDB
+snapshot: 20190101, - structure methods accepted: all (x-ray christolography,
+NRM, Cryo-EM), - sequence identity threshold for clustering: 40% sequence
+similarity, - maximum length per sequence: 1000 residues, - minimum length per
+sequence: 5 residues, - maximum fraction of missing values at the ends: 10%, -
+size of validation subset: 10%. ```bash proteinflow generate --tag new --
+resolution_thr 5 --pdb_snapshot 20190101 --not_filter_methods --min_seq_id 0.4
+--max_length 1000 --min_length 5 --missing_ends_thr 0.1 --valid_split 0.1 ```
+See the [docs](https://adaptyvbio.github.io/ProteinFlow/) (or `proteinflow
+generate --help`) for the full list of parameters and more information. A
+registry of all the files that are removed during the filtering as well as
+description with the reason for their removal is created automatically for each
+`generate` command. The log files are save (at `data/logs` by default) and a
+summary can be accessed running `proteinflow get_summary {log_path}`. You can
+also use the `--sabdab` option to load files from SAbDab and cluster them based
+on CDRs. Use together with `--zip_path` to process a custom SAbDab-like zip
+file. ### Splitting By default, both `proteinflow generate` and `proteinflow
+download` will also split your data into training, test and validation
+according to MMseqs2 clustering and homomer/heteromer/single chain proportions.
+However, you can skip this step with a `--skip_splitting` flag and then perform
+it separately with the `proteinflow split` command. The following command will
+perform the splitting with a 10% validation set, a 5% test set and a 50%
+threshold for sequence identity clusters. ```bash proteinflow split --tag new -
+-valid_split 0.1 --test_split 0.5 --min_seq_id 0.5 ``` Use the `--
+exclude_chains` and `--exclude_threshold` parameters to move all biounits that
+contain chains similar to what you specify to a separate folder. ### Using the
+data The output files are pickled nested dictionaries where first-level keys
+are chain Ids and second-level keys are the following: - `'crd_bb'`: a `numpy`
+array of shape `(L, 4, 3)` with backbone atom coordinates (N, C, CA, O), -
+`'crd_sc'`: a `numpy` array of shape `(L, 10, 3)` with sidechain atom
+coordinates (check `proteinflow.sidechain_order()` for the order of atoms), -
+`'msk'`: a `numpy` array of shape `(L,)` where ones correspond to residues with
+known coordinates and zeros to missing values, - `'seq'`: a string of length
+`L` with residue types. In a SAbDab datasets, an additional key is added to the
+dictionary: - `'cdr'`: a `'numpy'` array of shape `(L,)` where CDR residues are
+marked with the corresponding type (`'H1'`, `'L1'`, ...) and non-CDR residues
+are marked with `'-'`. Once your data is ready, you can open the files with
+`pickle`. ```python import pickle import os train_folder = "./data/
 proteinflow_new/training" for filename in os.listdir(train_folder): with open
 (os.path.join(train_folder, filename), "rb") as f: data = pickle.load(f) crd_bb
 = data["crd_bb"] seq = data["seq"] ... ``` Alternatively, you can use our
 `ProteinDataset` or `ProteinLoader` classes for convenient processing. Among
 other things, they allow for feature extraction, single chain / homomer /
 heteromer filtering and randomized sampling from sequence identity clusters.
 For example, here is how we can create a data loader that: - samples a
@@ -101,15 +108,16 @@
 should be masked, 0 otherwise ... ``` See more details on available parameters
 and the data format in the [docs](https://adaptyvbio.github.io/ProteinFlow/) +
 [this repository](https://github.com/adaptyvbio/ProteinFlow-models) for a use
 case. ## ProteinFlow Stable Releases You can download them with `proteinflow
 download --tag {tag}` in the command line or browse in the [interface](https://
 proteinflow-datasets.s3.eu-west-1.amazonaws.com/index.html). |Tag |Date
 |Snapshot|Size|Min res|Min len|Max len|MMseqs thr|Split (train/val/
-test)|Missing thr (ends/middle)|Note| |-------|--------|--------|----|-------|-
-------|-------|----------|----------------------|-------------------------|----
-| |paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|first release,
-no mmCIF files| |20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/
-5|0.3/0.1| v1.1.1| ## License The `proteinflow` package and data are released
-and distributed under the BSD 3-Clause License ## Contributions This is an open
+test)|Missing thr (ends/middle)|Source|Note| |-------|--------|--------|----|--
+-----|-------|-------|----------|----------------------|-----------------------
+--|---|----| |paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/
+0.1|PDB|first release, no mmCIF files|
+|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/5|0.3/
+0.1|PDB|v1.1.1| ## License The `proteinflow` package and data are released and
+distributed under the BSD 3-Clause License ## Contributions This is an open
 source project supported by [Adaptyv Bio](https://www.adaptyvbio.com/).
 Contributions, suggestions and bug-fixes are welcomed.
```

### Comparing `proteinflow-1.3.0/proteinflow.egg-info/SOURCES.txt` & `proteinflow-1.3.1/proteinflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.0/pyproject.toml` & `proteinflow-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proteinflow"
-version = "1.3.0"
+version = "1.3.1"
 authors = [
     {name = "Liza Kozlova", email = "liza@adaptyvbio.com"},
     {name = "Arthur Valentin", email = "arthur@adaptyvbio.com"}
 ]
 description = "Versatile pipeline for processing protein structure data for deep learning applications."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `proteinflow-1.3.0/tests/test_download.py` & `proteinflow-1.3.1/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.0/tests/test_generate.py` & `proteinflow-1.3.1/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.0/tests/test_sabdab.py` & `proteinflow-1.3.1/tests/test_sabdab.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     if os.path.exists(folder):
         shutil.rmtree(folder)
     start = time()
     # generate_data(tag="test", n=50, sabdab=True, resolution_thr=1)
     generate_data(
         tag="test",
         sabdab=True,
-        zip_path="./sample_data/sabdab.zip",
+        sabdab_data_path="./sample_data/sabdab.zip",
         require_antigen=True,
         skip_splitting=True,
     )
     end = time()
     assert all(["nan_nan" not in file for file in os.listdir(folder)])
     train_loader = ProteinLoader.from_args(
         dataset_folder=folder,
```

