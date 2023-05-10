# Comparing `tmp/simcardems-2023.3.0.tar.gz` & `tmp/simcardems-2023.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simcardems-2023.3.0.tar", last modified: Fri Mar 31 14:03:39 2023, max compression
+gzip compressed data, was "simcardems-2023.4.0.tar", last modified: Wed May 10 08:10:53 2023, max compression
```

## Comparing `simcardems-2023.3.0.tar` & `simcardems-2023.4.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:03:39.391273 simcardems-2023.3.0/
--rw-r--r--   0 root         (0) root         (0)    26526 2023-03-31 13:46:36.000000 simcardems-2023.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3845 2023-03-31 14:03:39.391273 simcardems-2023.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3141 2023-03-31 13:46:36.000000 simcardems-2023.3.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1821 2023-03-31 14:03:39.391273 simcardems-2023.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      296 2023-03-31 13:46:36.000000 simcardems-2023.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:03:39.371273 simcardems-2023.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:03:39.379273 simcardems-2023.3.0/src/simcardems/
--rw-r--r--   0 root         (0) root         (0)     3453 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1654 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/benchmark.py
--rw-r--r--   0 root         (0) root         (0)     5423 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/boundary_conditions.py
--rw-r--r--   0 root         (0) root         (0)     9241 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/cli.py
--rw-r--r--   0 root         (0) root         (0)     1919 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/config.py
--rw-r--r--   0 root         (0) root         (0)    18669 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/datacollector.py
--rw-r--r--   0 root         (0) root         (0)     9907 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/ep_model.py
--rw-r--r--   0 root         (0) root         (0)    16740 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/geometry.py
--rw-r--r--   0 root         (0) root         (0)    11745 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/gui.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/lvgeometry.py
--rw-r--r--   0 root         (0) root         (0)    11482 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/mechanics_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:03:39.383273 simcardems-2023.3.0/src/simcardems/models/
--rw-r--r--   0 root         (0) root         (0)      660 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6841 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/models/em_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:03:39.383273 simcardems-2023.3.0/src/simcardems/models/explicit_ORdmm_Land/
--rw-r--r--   0 root         (0) root         (0)      819 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/models/explicit_ORdmm_Land/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60660 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/models/explicit_ORdmm_Land/cell_model.py
--rw-r--r--   0 root         (0) root         (0)    13512 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/models/explicit_ORdmm_Land/em_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:03:39.383273 simcardems-2023.3.0/src/simcardems/models/fully_coupled_ORdmm_Land/
--rw-r--r--   0 root         (0) root         (0)      567 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/models/fully_coupled_ORdmm_Land/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6993 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/models/fully_coupled_ORdmm_Land/active_model.py
--rw-r--r--   0 root         (0) root         (0)    60244 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/models/fully_coupled_ORdmm_Land/cell_model.py
--rw-r--r--   0 root         (0) root         (0)    11304 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/models/fully_coupled_ORdmm_Land/em_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:03:39.387273 simcardems-2023.3.0/src/simcardems/models/fully_coupled_Tor_Land/
--rw-r--r--   0 root         (0) root         (0)      559 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/models/fully_coupled_Tor_Land/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6989 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/models/fully_coupled_Tor_Land/active_model.py
--rw-r--r--   0 root         (0) root         (0)    70534 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/models/fully_coupled_Tor_Land/cell_model.py
--rw-r--r--   0 root         (0) root         (0)    11302 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/models/fully_coupled_Tor_Land/em_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:03:39.387273 simcardems-2023.3.0/src/simcardems/models/pureEP_ORdmm_Land/
--rw-r--r--   0 root         (0) root         (0)      419 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/models/pureEP_ORdmm_Land/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60536 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/models/pureEP_ORdmm_Land/cell_model.py
--rw-r--r--   0 root         (0) root         (0)     5012 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/models/pureEP_ORdmm_Land/em_model.py
--rw-r--r--   0 root         (0) root         (0)     5730 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/newton_solver.py
--rw-r--r--   0 root         (0) root         (0)    18276 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/postprocess.py
--rw-r--r--   0 root         (0) root         (0)     7156 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/runner.py
--rw-r--r--   0 root         (0) root         (0)     6485 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/save_load_functions.py
--rw-r--r--   0 root         (0) root         (0)     4515 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/slabgeometry.py
--rw-r--r--   0 root         (0) root         (0)     2642 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/time_stepper.py
--rw-r--r--   0 root         (0) root         (0)     5462 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/utils.py
--rw-r--r--   0 root         (0) root         (0)     4826 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/value_extractor.py
--rw-r--r--   0 root         (0) root         (0)       25 2023-03-31 13:46:36.000000 simcardems-2023.3.0/src/simcardems/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:03:39.383273 simcardems-2023.3.0/src/simcardems.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3845 2023-03-31 14:03:39.000000 simcardems-2023.3.0/src/simcardems.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2016 2023-03-31 14:03:39.000000 simcardems-2023.3.0/src/simcardems.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 14:03:39.000000 simcardems-2023.3.0/src/simcardems.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-03-31 14:03:39.000000 simcardems-2023.3.0/src/simcardems.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 13:47:00.000000 simcardems-2023.3.0/src/simcardems.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      328 2023-03-31 14:03:39.000000 simcardems-2023.3.0/src/simcardems.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-03-31 14:03:39.000000 simcardems-2023.3.0/src/simcardems.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:03:39.391273 simcardems-2023.3.0/tests/
--rw-r--r--   0 root         (0) root         (0)      523 2023-03-31 13:46:36.000000 simcardems-2023.3.0/tests/test_boundary_conditions.py
--rw-r--r--   0 root         (0) root         (0)     3454 2023-03-31 13:46:36.000000 simcardems-2023.3.0/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     2974 2023-03-31 13:46:36.000000 simcardems-2023.3.0/tests/test_datacollector.py
--rw-r--r--   0 root         (0) root         (0)     2559 2023-03-31 13:46:36.000000 simcardems-2023.3.0/tests/test_geometry.py
--rw-r--r--   0 root         (0) root         (0)     3507 2023-03-31 13:46:36.000000 simcardems-2023.3.0/tests/test_mechanics_model.py
--rw-r--r--   0 root         (0) root         (0)     1959 2023-03-31 13:46:36.000000 simcardems-2023.3.0/tests/test_models.py
--rw-r--r--   0 root         (0) root         (0)     1187 2023-03-31 13:46:36.000000 simcardems-2023.3.0/tests/test_postprocessing.py
--rw-r--r--   0 root         (0) root         (0)     1956 2023-03-31 13:46:36.000000 simcardems-2023.3.0/tests/test_runner.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-03-31 13:46:36.000000 simcardems-2023.3.0/tests/test_save_load_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:10:53.958935 simcardems-2023.4.0/
+-rw-r--r--   0 root         (0) root         (0)    26526 2023-05-10 07:53:22.000000 simcardems-2023.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3845 2023-05-10 08:10:53.958935 simcardems-2023.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3141 2023-05-10 07:53:22.000000 simcardems-2023.4.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-05-10 08:10:53.958935 simcardems-2023.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      296 2023-05-10 07:53:22.000000 simcardems-2023.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:10:53.938935 simcardems-2023.4.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:10:53.946935 simcardems-2023.4.0/src/simcardems/
+-rw-r--r--   0 root         (0) root         (0)     3453 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       77 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/benchmark.py
+-rw-r--r--   0 root         (0) root         (0)     5423 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/boundary_conditions.py
+-rw-r--r--   0 root         (0) root         (0)     9241 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/config.py
+-rw-r--r--   0 root         (0) root         (0)    18669 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/datacollector.py
+-rw-r--r--   0 root         (0) root         (0)     9907 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/ep_model.py
+-rw-r--r--   0 root         (0) root         (0)    17148 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/geometry.py
+-rw-r--r--   0 root         (0) root         (0)    11745 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/gui.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/lvgeometry.py
+-rw-r--r--   0 root         (0) root         (0)    11482 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/mechanics_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:10:53.950935 simcardems-2023.4.0/src/simcardems/models/
+-rw-r--r--   0 root         (0) root         (0)      660 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6841 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/em_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:10:53.950935 simcardems-2023.4.0/src/simcardems/models/explicit_ORdmm_Land/
+-rw-r--r--   0 root         (0) root         (0)      819 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/explicit_ORdmm_Land/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60660 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/explicit_ORdmm_Land/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)    14001 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/explicit_ORdmm_Land/em_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:10:53.954935 simcardems-2023.4.0/src/simcardems/models/fully_coupled_ORdmm_Land/
+-rw-r--r--   0 root         (0) root         (0)      567 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/fully_coupled_ORdmm_Land/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6993 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/fully_coupled_ORdmm_Land/active_model.py
+-rw-r--r--   0 root         (0) root         (0)    60244 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/fully_coupled_ORdmm_Land/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)    11882 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/fully_coupled_ORdmm_Land/em_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:10:53.954935 simcardems-2023.4.0/src/simcardems/models/fully_coupled_Tor_Land/
+-rw-r--r--   0 root         (0) root         (0)      559 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/fully_coupled_Tor_Land/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6989 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/fully_coupled_Tor_Land/active_model.py
+-rw-r--r--   0 root         (0) root         (0)    70534 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/fully_coupled_Tor_Land/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)    11880 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/fully_coupled_Tor_Land/em_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:10:53.954935 simcardems-2023.4.0/src/simcardems/models/pureEP_ORdmm_Land/
+-rw-r--r--   0 root         (0) root         (0)      419 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/pureEP_ORdmm_Land/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60536 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/pureEP_ORdmm_Land/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)     5012 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/pureEP_ORdmm_Land/em_model.py
+-rw-r--r--   0 root         (0) root         (0)     5730 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/newton_solver.py
+-rw-r--r--   0 root         (0) root         (0)    21621 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/postprocess.py
+-rw-r--r--   0 root         (0) root         (0)     7156 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/runner.py
+-rw-r--r--   0 root         (0) root         (0)     6485 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/save_load_functions.py
+-rw-r--r--   0 root         (0) root         (0)     4515 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/slabgeometry.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/time_stepper.py
+-rw-r--r--   0 root         (0) root         (0)     5462 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4826 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/value_extractor.py
+-rw-r--r--   0 root         (0) root         (0)       25 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:10:53.950935 simcardems-2023.4.0/src/simcardems.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3845 2023-05-10 08:10:53.000000 simcardems-2023.4.0/src/simcardems.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2016 2023-05-10 08:10:53.000000 simcardems-2023.4.0/src/simcardems.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 08:10:53.000000 simcardems-2023.4.0/src/simcardems.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-05-10 08:10:53.000000 simcardems-2023.4.0/src/simcardems.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 07:53:45.000000 simcardems-2023.4.0/src/simcardems.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      337 2023-05-10 08:10:53.000000 simcardems-2023.4.0/src/simcardems.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-10 08:10:53.000000 simcardems-2023.4.0/src/simcardems.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:10:53.958935 simcardems-2023.4.0/tests/
+-rw-r--r--   0 root         (0) root         (0)      523 2023-05-10 07:53:22.000000 simcardems-2023.4.0/tests/test_boundary_conditions.py
+-rw-r--r--   0 root         (0) root         (0)     3454 2023-05-10 07:53:22.000000 simcardems-2023.4.0/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     2974 2023-05-10 07:53:22.000000 simcardems-2023.4.0/tests/test_datacollector.py
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-05-10 07:53:22.000000 simcardems-2023.4.0/tests/test_geometry.py
+-rw-r--r--   0 root         (0) root         (0)     3507 2023-05-10 07:53:22.000000 simcardems-2023.4.0/tests/test_mechanics_model.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-05-10 07:53:22.000000 simcardems-2023.4.0/tests/test_models.py
+-rw-r--r--   0 root         (0) root         (0)     2793 2023-05-10 07:53:22.000000 simcardems-2023.4.0/tests/test_postprocessing.py
+-rw-r--r--   0 root         (0) root         (0)     1956 2023-05-10 07:53:22.000000 simcardems-2023.4.0/tests/test_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-05-10 07:53:22.000000 simcardems-2023.4.0/tests/test_save_load_functions.py
```

### Comparing `simcardems-2023.3.0/LICENSE` & `simcardems-2023.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/PKG-INFO` & `simcardems-2023.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simcardems
-Version: 2023.3.0
+Version: 2023.4.0
 Summary: Simula Cardiac electromechanics solver
 Home-page: https://github.com/ComputationalPhysiology/simcardems
 Author: Henrik Finsberg, Ilsbeth van Herck, Cécile Daversin-Catty
 Author-email: henriknf@simula.no
 License: LGPL-2.1
 Keywords: action potential,cardiac mechanics,electrophysiology,electromechanics
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
```

### Comparing `simcardems-2023.3.0/README.md` & `simcardems-2023.4.0/README.md`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/setup.cfg` & `simcardems-2023.4.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 	twine
 	wheel
 docs = 
 	jupyter-book
 	jupytext
 	pandas
 	plotly
+	requests
 	sphinxcontrib-bibtex
 gui = 
 	fenics-plotly
 	streamlit
 
 [flake8]
 exclude = docs
```

### Comparing `simcardems-2023.3.0/src/simcardems/__init__.py` & `simcardems-2023.4.0/src/simcardems/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/boundary_conditions.py` & `simcardems-2023.4.0/src/simcardems/boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/cli.py` & `simcardems-2023.4.0/src/simcardems/cli.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/config.py` & `simcardems-2023.4.0/src/simcardems/config.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/datacollector.py` & `simcardems-2023.4.0/src/simcardems/datacollector.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/ep_model.py` & `simcardems-2023.4.0/src/simcardems/ep_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/geometry.py` & `simcardems-2023.4.0/src/simcardems/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,16 +318,26 @@
 
     def _interpolate_microstructure(self) -> pulse.Microstructure:
         element = self.f0.ufl_element()
         if element.family() == "Quadrature":
             return self._default_microstructure(mesh=self.ep_mesh, ffun=self.ffun_ep)
         else:
             V = dolfin.FunctionSpace(self.ep_mesh, element)
+            try:
+                f0 = dolfin.interpolate(self.f0, V)
+            except RuntimeError:
+                logger.info(
+                    "Extrapolate fibers in order to interpolate from mechanics to ep mesh",
+                )
+                self.f0.set_allow_extrapolation(True)
+                self.s0.set_allow_extrapolation(True)
+                self.n0.set_allow_extrapolation(True)
+
+                f0 = dolfin.interpolate(self.f0, V)
 
-            f0 = dolfin.interpolate(self.f0, V)
             s0 = dolfin.interpolate(self.s0, V)
             n0 = dolfin.interpolate(self.n0, V)
             return pulse.Microstructure(f0=f0, s0=s0, n0=n0)
 
     @property
     def microstructure(self) -> pulse.Microstructure:
         return self._microstructure  # type: ignore
```

### Comparing `simcardems-2023.3.0/src/simcardems/gui.py` & `simcardems-2023.4.0/src/simcardems/gui.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/lvgeometry.py` & `simcardems-2023.4.0/src/simcardems/lvgeometry.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/mechanics_model.py` & `simcardems-2023.4.0/src/simcardems/mechanics_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/models/__init__.py` & `simcardems-2023.4.0/src/simcardems/models/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/models/em_model.py` & `simcardems-2023.4.0/src/simcardems/models/em_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/models/explicit_ORdmm_Land/__init__.py` & `simcardems-2023.4.0/src/simcardems/models/explicit_ORdmm_Land/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/models/explicit_ORdmm_Land/cell_model.py` & `simcardems-2023.4.0/src/simcardems/models/explicit_ORdmm_Land/cell_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/models/explicit_ORdmm_Land/em_model.py` & `simcardems-2023.4.0/src/simcardems/models/explicit_ORdmm_Land/em_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,14 +76,32 @@
         self._projector_V_ep = utils.Projector(self.V_ep)
         self._projector_V_mech = utils.Projector(self.V_mech)
 
         if lmbda is not None:
             self.lmbda_ep.vector()[:] = lmbda.vector()
             self.lmbda_ep_prev.vector()[:] = lmbda.vector()
 
+        self.transfer_matrix = dolfin.PETScDMCollection.create_transfer_matrix(
+            self.V_mech,
+            self.V_ep,
+        ).mat()
+
+    def interpolate(
+        self,
+        f_mech: dolfin.Function,
+        f_ep: dolfin.Function,
+    ) -> dolfin.Function:
+        """Interpolates function from mechanics to ep mesh"""
+
+        x = dolfin.as_backend_type(f_mech.vector()).vec()
+        _, temp = self.transfer_matrix.getVecs()
+        self.transfer_matrix.mult(x, temp)
+        f_ep.vector().vec().aypx(0.0, temp)
+        f_ep.vector().apply("")
+
     def __eq__(self, __o: object) -> bool:
         if not isinstance(__o, type(self)):
             return NotImplemented
 
         if not super().__eq__(__o):
             return False
 
@@ -280,17 +298,15 @@
 
     def mechanics_to_coupling(self):
         logger.debug("Transfer variables from mechanics to coupling")
         self.u_mech_assigner.assign(
             self.u_mech,
             utils.sub_function(self.mech_state, self._u_subspace_index),
         )
-        self.lmbda_ep.interpolate(self.lmbda_mech_func)
-        # self.u_ep.interpolate(self.u_mech)
-        # self._project_lmbda()
+        self.interpolate(self.lmbda_mech_func, self.lmbda_ep)
 
         logger.debug("Done transferring variables from mechanics to coupling")
 
     def coupling_to_ep(self):
         logger.debug("Update EP")
         logger.debug("Done updating EP")
```

### Comparing `simcardems-2023.3.0/src/simcardems/models/fully_coupled_ORdmm_Land/__init__.py` & `simcardems-2023.4.0/src/simcardems/models/fully_coupled_ORdmm_Land/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/models/fully_coupled_ORdmm_Land/active_model.py` & `simcardems-2023.4.0/src/simcardems/models/fully_coupled_ORdmm_Land/active_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/models/fully_coupled_ORdmm_Land/cell_model.py` & `simcardems-2023.4.0/src/simcardems/models/fully_coupled_ORdmm_Land/cell_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/models/fully_coupled_ORdmm_Land/em_model.py` & `simcardems-2023.4.0/src/simcardems/models/fully_coupled_ORdmm_Land/em_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,32 @@
         self.XW_mech = dolfin.Function(self.V_mech, name="XW_mech")
 
         self.V_ep = dolfin.FunctionSpace(self.ep_mesh, "CG", 1)
         self.lmbda_ep = dolfin.Function(self.V_ep, name="lambda_ep")
         self.Zetas_ep = dolfin.Function(self.V_ep, name="Zetas_ep")
         self.Zetaw_ep = dolfin.Function(self.V_ep, name="Zetaw_ep")
 
+        self.transfer_matrix = dolfin.PETScDMCollection.create_transfer_matrix(
+            self.V_mech,
+            self.V_ep,
+        ).mat()
+
+    def interpolate(
+        self,
+        f_mech: dolfin.Function,
+        f_ep: dolfin.Function,
+    ) -> dolfin.Function:
+        """Interpolates function from mechanics to ep mesh"""
+
+        x = dolfin.as_backend_type(f_mech.vector()).vec()
+        _, temp = self.transfer_matrix.getVecs()
+        self.transfer_matrix.mult(x, temp)
+        f_ep.vector().vec().aypx(0.0, temp)
+        f_ep.vector().apply("")
+
     @property
     def coupling_type(self):
         return "fully_coupled_ORdmm_Land"
 
     def __eq__(self, __o: object) -> bool:
         if not isinstance(__o, type(self)):
             return NotImplemented
@@ -192,17 +210,17 @@
         if hasattr(self, "_assigners"):
             self.XS_mech.interpolate(self.assigners.functions["ep"]["XS"])
             self.XW_mech.interpolate(self.assigners.functions["ep"]["XW"])
         logger.debug("Done interpolating mechanics")
 
     def mechanics_to_coupling(self):
         logger.debug("Interpolate EP")
-        self.lmbda_ep.interpolate(self.lmbda_mech)
-        self.Zetas_ep.interpolate(self.Zetas_mech)
-        self.Zetaw_ep.interpolate(self.Zetaw_mech)
+        self.interpolate(self.lmbda_mech, self.lmbda_ep)
+        self.interpolate(self.Zetas_mech, self.Zetas_ep)
+        self.interpolate(self.Zetaw_mech, self.Zetaw_ep)
         logger.debug("Done interpolating EP")
 
     def coupling_to_ep(self):
         logger.debug("Update EP")
         logger.debug("Done updating EP")
 
     def solve_mechanics(self) -> None:
```

### Comparing `simcardems-2023.3.0/src/simcardems/models/fully_coupled_Tor_Land/__init__.py` & `simcardems-2023.4.0/src/simcardems/models/fully_coupled_Tor_Land/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/models/fully_coupled_Tor_Land/active_model.py` & `simcardems-2023.4.0/src/simcardems/models/fully_coupled_Tor_Land/active_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/models/fully_coupled_Tor_Land/cell_model.py` & `simcardems-2023.4.0/src/simcardems/models/fully_coupled_Tor_Land/cell_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -659,15 +659,15 @@
         aK1 = 4.094 / (1.0 + ufl.exp(0.1217 * (v - EK - 49.934)))
         bK1 = (
             15.72 * ufl.exp(0.0674 * (v - EK - 3.257))
             + ufl.exp(0.0618 * (v - EK - 594.31))
         ) / (1.0 + ufl.exp(-0.1629 * (v - EK + 14.207)))
         K1ss = aK1 / (aK1 + bK1)
         GK1 = 0.6992 * scale_IK1 * scale_drug_IK1 * scale_popu_GK1 * HF_scaling_GK1
-        IK1 = ufl.sqrt(ko) * (-EK + v) * GK1 * GK1 * K1ss
+        IK1 = ufl.sqrt(ko / 5.0) * (-EK + v) * GK1 * K1ss
 
         # Expressions for the INaCa_i component
         hca = ufl.exp(F * qca * v / (R * T))
         hna = ufl.exp(F * qna * v / (R * T))
         h1_i = 1 + (1 + hna) * nai / kna3
         h2_i = hna * nai / (kna3 * h1_i)
         h3_i = 1.0 / h1_i
```

### Comparing `simcardems-2023.3.0/src/simcardems/models/fully_coupled_Tor_Land/em_model.py` & `simcardems-2023.4.0/src/simcardems/models/fully_coupled_Tor_Land/em_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,32 @@
         self.XW_mech = dolfin.Function(self.V_mech, name="XW_mech")
 
         self.V_ep = dolfin.FunctionSpace(self.ep_mesh, "CG", 1)
         self.lmbda_ep = dolfin.Function(self.V_ep, name="lambda_ep")
         self.Zetas_ep = dolfin.Function(self.V_ep, name="Zetas_ep")
         self.Zetaw_ep = dolfin.Function(self.V_ep, name="Zetaw_ep")
 
+        self.transfer_matrix = dolfin.PETScDMCollection.create_transfer_matrix(
+            self.V_mech,
+            self.V_ep,
+        ).mat()
+
+    def interpolate(
+        self,
+        f_mech: dolfin.Function,
+        f_ep: dolfin.Function,
+    ) -> dolfin.Function:
+        """Interpolates function from mechanics to ep mesh"""
+
+        x = dolfin.as_backend_type(f_mech.vector()).vec()
+        _, temp = self.transfer_matrix.getVecs()
+        self.transfer_matrix.mult(x, temp)
+        f_ep.vector().vec().aypx(0.0, temp)
+        f_ep.vector().apply("")
+
     @property
     def coupling_type(self):
         return "fully_coupled_Tor_Land"
 
     def __eq__(self, __o: object) -> bool:
         if not isinstance(__o, type(self)):
             return NotImplemented
@@ -192,17 +210,17 @@
         if hasattr(self, "_assigners"):
             self.XS_mech.interpolate(self.assigners.functions["ep"]["XS"])
             self.XW_mech.interpolate(self.assigners.functions["ep"]["XW"])
         logger.debug("Done interpolating mechanics")
 
     def mechanics_to_coupling(self):
         logger.debug("Interpolate EP")
-        self.lmbda_ep.interpolate(self.lmbda_mech)
-        self.Zetas_ep.interpolate(self.Zetas_mech)
-        self.Zetaw_ep.interpolate(self.Zetaw_mech)
+        self.interpolate(self.lmbda_mech, self.lmbda_ep)
+        self.interpolate(self.Zetas_mech, self.Zetas_ep)
+        self.interpolate(self.Zetaw_mech, self.Zetaw_ep)
         logger.debug("Done interpolating EP")
 
     def coupling_to_ep(self):
         logger.debug("Update EP")
         logger.debug("Done updating EP")
 
     def solve_mechanics(self) -> None:
```

### Comparing `simcardems-2023.3.0/src/simcardems/models/pureEP_ORdmm_Land/cell_model.py` & `simcardems-2023.4.0/src/simcardems/models/pureEP_ORdmm_Land/cell_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/models/pureEP_ORdmm_Land/em_model.py` & `simcardems-2023.4.0/src/simcardems/models/pureEP_ORdmm_Land/em_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/newton_solver.py` & `simcardems-2023.4.0/src/simcardems/newton_solver.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/postprocess.py` & `simcardems-2023.4.0/src/simcardems/postprocess.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from collections import defaultdict
 from pathlib import Path
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
@@ -10,14 +11,15 @@
 import ap_features as apf
 import dolfin
 import matplotlib.pyplot as plt
 import numpy as np
 import tqdm
 
 from . import utils
+from .datacollector import DataCollector
 from .datacollector import DataGroups
 from .datacollector import DataLoader
 
 logger = utils.getLogger(__name__)
 
 
 def plot_peaks(fname, data, threshold):
@@ -282,15 +284,15 @@
     times = np.array(results["m1"]["time"], dtype=float)
     if reset_time:
         times = times - times[0]
     fig, ax = plt.subplots(2, 2, figsize=(10, 8), sharex=True)
     for PoMm in range(1, num_models + 1):
         ax[0, 0].plot(
             times,
-            np.array(results[f"m{PoMm}"]["mechanics"]["lmbda"], dtype=float),
+            np.array(results[f"m{PoMm}"]["mechanics"]["lambda"], dtype=float),
         )
         ax[0, 1].plot(
             times,
             np.array(results[f"m{PoMm}"]["mechanics"]["Ta"], dtype=float),
         )
         ax[1, 0].plot(times, np.array(results[f"m{PoMm}"]["ep"]["V"], dtype=float))
         ax[1, 1].plot(
@@ -549,7 +551,103 @@
             v.vector()[:] >= threshold,
             activation_map.vector()[:] < t0,
         )
 
         activation_map.vector()[np.where(dofs)[0]] = float(t)
 
     return activation_map
+
+
+def extract_sub_results(
+    results_file: utils.PathLike,
+    output_file: utils.PathLike,
+    t_start: float = 0.0,
+    t_end: float | None = None,
+    names: Optional[Dict[str, List[str]]] = None,
+) -> DataCollector:
+    """Extract sub results from another results file.
+    This can be useful if you have stored a lot of data in one file
+    and you want to create a smaller file containing only a subset
+    of the data (e.g only the last beat)
+
+    Parameters
+    ----------
+    results_file : utils.PathLike
+        The input result file
+    output_file : utils.PathLike
+        Path to file where you want to store the sub results
+    t_start : float, optional
+        Time point indicating when the sub results should start, by default 0.0
+    t_end : float | None, optional
+        Time point indicating when the sub results should end, by default None
+        in which case it will choose the last time point
+    names : Optional[Dict[str, List[str]]], optional
+        A dictionary of names for each group indicating which
+        functions to extract for the sub results. If not provided (default)
+        then all functions will be extracted.
+
+    Returns
+    -------
+    datacollector.DataCollector
+        A data collector containing the sub results
+
+    Raises
+    ------
+    FileNotFoundError
+        If the input file does not exist
+    KeyError
+        If some of the names provided does not exists
+        in the input file
+    """
+    results_file = Path(results_file)
+    if not results_file.is_file():
+        raise FileNotFoundError(f"File {results_file} does not exist")
+
+    loader = DataLoader(results_file)
+    assert loader.time_stamps is not None
+    if names is None:
+        # Extract everything
+        names = loader.names
+
+    t_start_idx = next(
+        (i for i, t in enumerate(map(float, loader.time_stamps)) if t > t_start - 1e-12)
+    )
+    if t_end is None:
+        t_end_idx = len(loader.time_stamps) - 1
+    else:
+        try:
+            t_end_idx = next(
+                i
+                for i, t in enumerate(map(float, loader.time_stamps))
+                if t > t_end + 1e-12
+            )
+        except StopIteration:
+            t_end_idx = len(loader.time_stamps) - 1
+
+    out = Path(output_file)
+    collector = DataCollector(
+        outdir=out.parent,
+        outfilename=out.name,
+        geo=loader.geo,
+    )
+
+    functions: Dict[str, Dict[str, dolfin.Function]] = defaultdict(dict)
+    for group_name, group in names.items():
+        for func_name in group:
+            try:
+                functions[group_name][func_name] = loader._functions[group_name][
+                    func_name
+                ]
+            except KeyError as e:
+                raise KeyError(
+                    f"Invalid group {group_name} and function {func_name}",
+                ) from e
+            collector.register(group_name, func_name, functions[group_name][func_name])
+
+    for ti in loader.time_stamps[t_start_idx:t_end_idx]:
+        for group_name, group in names.items():
+            for func_name in group:
+                functions[group_name][func_name].assign(
+                    loader.get(DataGroups[group_name], func_name, ti),
+                )
+        collector.store(float(ti))
+    return collector
```

### Comparing `simcardems-2023.3.0/src/simcardems/runner.py` & `simcardems-2023.4.0/src/simcardems/runner.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/save_load_functions.py` & `simcardems-2023.4.0/src/simcardems/save_load_functions.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/slabgeometry.py` & `simcardems-2023.4.0/src/simcardems/slabgeometry.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/time_stepper.py` & `simcardems-2023.4.0/src/simcardems/time_stepper.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/utils.py` & `simcardems-2023.4.0/src/simcardems/utils.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems/value_extractor.py` & `simcardems-2023.4.0/src/simcardems/value_extractor.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/src/simcardems.egg-info/PKG-INFO` & `simcardems-2023.4.0/src/simcardems.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simcardems
-Version: 2023.3.0
+Version: 2023.4.0
 Summary: Simula Cardiac electromechanics solver
 Home-page: https://github.com/ComputationalPhysiology/simcardems
 Author: Henrik Finsberg, Ilsbeth van Herck, Cécile Daversin-Catty
 Author-email: henriknf@simula.no
 License: LGPL-2.1
 Keywords: action potential,cardiac mechanics,electrophysiology,electromechanics
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
```

### Comparing `simcardems-2023.3.0/src/simcardems.egg-info/SOURCES.txt` & `simcardems-2023.4.0/src/simcardems.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/tests/test_boundary_conditions.py` & `simcardems-2023.4.0/tests/test_boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/tests/test_cli.py` & `simcardems-2023.4.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/tests/test_datacollector.py` & `simcardems-2023.4.0/tests/test_datacollector.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/tests/test_geometry.py` & `simcardems-2023.4.0/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/tests/test_mechanics_model.py` & `simcardems-2023.4.0/tests/test_mechanics_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/tests/test_models.py` & `simcardems-2023.4.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/tests/test_runner.py` & `simcardems-2023.4.0/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.3.0/tests/test_save_load_functions.py` & `simcardems-2023.4.0/tests/test_save_load_functions.py`

 * *Files identical despite different names*

