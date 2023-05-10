# Comparing `tmp/pyhalo-0.0.1.tar.gz` & `tmp/pyhalo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhalo-0.0.1.tar", last modified: Fri May  5 21:00:56 2023, max compression
+gzip compressed data, was "pyhalo-0.2.0.tar", last modified: Wed May 10 03:55:10 2023, max compression
```

## Comparing `pyhalo-0.0.1.tar` & `pyhalo-0.2.0.tar`

### file list

```diff
@@ -1,83 +1,85 @@
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-05 21:00:56.108088 pyhalo-0.0.1/
--rw-r--r--   0 danielgilman   (501) staff       (20)      156 2018-08-15 00:45:59.000000 pyhalo-0.0.1/AUTHORS.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     3515 2018-08-15 00:45:59.000000 pyhalo-0.0.1/CONTRIBUTING.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       89 2018-08-15 00:45:59.000000 pyhalo-0.0.1/HISTORY.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     1072 2018-08-15 00:45:59.000000 pyhalo-0.0.1/LICENSE
--rw-r--r--   0 danielgilman   (501) staff       (20)      262 2018-08-15 00:45:59.000000 pyhalo-0.0.1/MANIFEST.in
--rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-05-05 21:00:56.108224 pyhalo-0.0.1/PKG-INFO
--rw-r--r--   0 danielgilman   (501) staff       (20)     1838 2022-06-30 13:05:47.000000 pyhalo-0.0.1/README.rst
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-05 21:00:56.072435 pyhalo-0.0.1/docs/
--rw-r--r--   0 danielgilman   (501) staff       (20)      607 2018-08-15 00:45:59.000000 pyhalo-0.0.1/docs/Makefile
--rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.0.1/docs/authors.rst
--rwxr-xr-x   0 danielgilman   (501) staff       (20)     4799 2018-10-06 19:25:46.000000 pyhalo-0.0.1/docs/conf.py
--rw-r--r--   0 danielgilman   (501) staff       (20)       33 2018-08-15 00:45:59.000000 pyhalo-0.0.1/docs/contributing.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.0.1/docs/history.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)      303 2018-08-15 00:45:59.000000 pyhalo-0.0.1/docs/index.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     1110 2018-08-15 00:45:59.000000 pyhalo-0.0.1/docs/installation.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)      768 2018-08-15 00:45:59.000000 pyhalo-0.0.1/docs/make.bat
--rw-r--r--   0 danielgilman   (501) staff       (20)       27 2018-08-15 00:45:59.000000 pyhalo-0.0.1/docs/readme.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       67 2018-08-15 00:45:59.000000 pyhalo-0.0.1/docs/usage.rst
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-05 21:00:56.081087 pyhalo-0.0.1/pyHalo/
--rw-r--r--   0 danielgilman   (501) staff       (20)      149 2018-08-15 00:45:59.000000 pyhalo-0.0.1/pyHalo/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2570 2023-05-05 20:46:58.000000 pyhalo-0.0.1/pyHalo/concentration_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3846 2023-05-05 20:46:58.000000 pyhalo-0.0.1/pyHalo/defaults.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2447 2023-05-05 20:46:58.000000 pyhalo-0.0.1/pyHalo/mass_function_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    36931 2023-05-05 20:46:58.000000 pyhalo-0.0.1/pyHalo/preset_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5617 2023-05-05 20:46:58.000000 pyhalo-0.0.1/pyHalo/pyhalo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    26366 2023-05-05 20:46:58.000000 pyhalo-0.0.1/pyHalo/realization_extensions.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    36187 2023-05-05 20:46:58.000000 pyhalo-0.0.1/pyHalo/single_realization.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      845 2023-05-05 20:46:58.000000 pyhalo-0.0.1/pyHalo/truncation_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    14194 2023-05-05 20:46:58.000000 pyhalo-0.0.1/pyHalo/utilities.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-05 21:00:56.084547 pyhalo-0.0.1/pyHalo.egg-info/
--rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-05-05 21:00:56.000000 pyhalo-0.0.1/pyHalo.egg-info/PKG-INFO
--rw-r--r--   0 danielgilman   (501) staff       (20)     2468 2023-05-05 21:00:56.000000 pyhalo-0.0.1/pyHalo.egg-info/SOURCES.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)        1 2023-05-05 21:00:56.000000 pyhalo-0.0.1/pyHalo.egg-info/dependency_links.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)       43 2023-05-05 21:00:56.000000 pyhalo-0.0.1/pyHalo.egg-info/entry_points.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)        1 2018-08-23 21:07:23.000000 pyhalo-0.0.1/pyHalo.egg-info/not-zip-safe
--rw-r--r--   0 danielgilman   (501) staff       (20)       11 2023-05-05 21:00:56.000000 pyhalo-0.0.1/pyHalo.egg-info/requires.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)        7 2023-05-05 21:00:56.000000 pyhalo-0.0.1/pyHalo.egg-info/top_level.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)      526 2023-05-05 20:59:31.000000 pyhalo-0.0.1/pyproject.toml
--rw-r--r--   0 danielgilman   (501) staff       (20)      389 2023-05-05 21:00:56.108782 pyhalo-0.0.1/setup.cfg
--rw-r--r--   0 danielgilman   (501) staff       (20)     1594 2021-02-01 15:25:54.000000 pyhalo-0.0.1/setup.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-05 21:00:56.090041 pyhalo-0.0.1/tests/
--rw-r--r--   0 danielgilman   (501) staff       (20)       61 2018-10-06 19:25:46.000000 pyhalo-0.0.1/tests/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1688 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_concentration_models.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-05 21:00:56.093539 pyhalo-0.0.1/tests/test_cosmology/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-10-18 06:20:01.000000 pyhalo-0.0.1/tests/test_cosmology/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5023 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_cosmology/test_cone_geometry.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3841 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_cosmology/test_cosmo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3969 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_cosmology/test_cylinder_geometry.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-05 21:00:56.100754 pyhalo-0.0.1/tests/test_halos/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-12-04 22:13:12.000000 pyhalo-0.0.1/tests/test_halos/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4220 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_halos/test_concentrations.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1334 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_halos/test_gaussian.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4656 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_halos/test_general_nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3407 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_halos/test_lenscosmo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2667 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_halos/test_nfw_halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3343 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_halos/test_pjaffe.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1665 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_halos/test_point_mass.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2719 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_halos/test_tnfw_halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1301 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_halos/test_truncation.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5003 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_halos/test_uldm.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      874 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_mass_function_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3224 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_preset_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8793 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_pyhalo_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    16257 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_realization_extensions.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-05 21:00:56.103472 pyhalo-0.0.1/tests/test_rendering/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.0.1/tests/test_rendering/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2584 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_rendering/test_2halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3422 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_rendering/test_los.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-05 21:00:56.105603 pyhalo-0.0.1/tests/test_rendering/test_mass_functions/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_rendering/test_mass_functions/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4769 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_rendering/test_mass_functions/test_base_functions.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2173 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_rendering/test_mass_functions/test_delta_function.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    11175 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_rendering/test_mass_functions/test_sheth_tormen.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2936 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_rendering/test_population.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-05 21:00:56.107640 pyhalo-0.0.1/tests/test_rendering/test_spatial_distribution/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_rendering/test_spatial_distribution/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2096 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_rendering/test_spatial_distribution/test_correlated.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2191 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_rendering/test_spatial_distribution/test_nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2153 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_rendering/test_spatial_distribution/test_uniform.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3491 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_rendering/test_subhalos.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    23809 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_single_realization.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2551 2023-05-05 20:46:58.000000 pyhalo-0.0.1/tests/test_utilities.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-10 03:55:10.822519 pyhalo-0.2.0/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      156 2018-08-15 00:45:59.000000 pyhalo-0.2.0/AUTHORS.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3515 2018-08-15 00:45:59.000000 pyhalo-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       89 2018-08-15 00:45:59.000000 pyhalo-0.2.0/HISTORY.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1072 2018-08-15 00:45:59.000000 pyhalo-0.2.0/LICENSE
+-rw-r--r--   0 danielgilman   (501) staff       (20)      262 2018-08-15 00:45:59.000000 pyhalo-0.2.0/MANIFEST.in
+-rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-05-10 03:55:10.822922 pyhalo-0.2.0/PKG-INFO
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2052 2023-05-10 03:31:30.000000 pyhalo-0.2.0/README.rst
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-10 03:55:10.419995 pyhalo-0.2.0/docs/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      607 2018-08-15 00:45:59.000000 pyhalo-0.2.0/docs/Makefile
+-rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.0/docs/authors.rst
+-rwxr-xr-x   0 danielgilman   (501) staff       (20)     4799 2018-10-06 19:25:46.000000 pyhalo-0.2.0/docs/conf.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)       33 2018-08-15 00:45:59.000000 pyhalo-0.2.0/docs/contributing.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.0/docs/history.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)      303 2018-08-15 00:45:59.000000 pyhalo-0.2.0/docs/index.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1110 2018-08-15 00:45:59.000000 pyhalo-0.2.0/docs/installation.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)      768 2018-08-15 00:45:59.000000 pyhalo-0.2.0/docs/make.bat
+-rw-r--r--   0 danielgilman   (501) staff       (20)       27 2018-08-15 00:45:59.000000 pyhalo-0.2.0/docs/readme.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       67 2018-08-15 00:45:59.000000 pyhalo-0.2.0/docs/usage.rst
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-10 03:55:10.454563 pyhalo-0.2.0/pyHalo/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      149 2018-08-15 00:45:59.000000 pyhalo-0.2.0/pyHalo/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2570 2023-05-10 03:31:30.000000 pyhalo-0.2.0/pyHalo/concentration_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3846 2023-05-10 03:31:30.000000 pyhalo-0.2.0/pyHalo/defaults.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2447 2023-05-10 03:31:30.000000 pyhalo-0.2.0/pyHalo/mass_function_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    36931 2023-05-10 03:31:30.000000 pyhalo-0.2.0/pyHalo/preset_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5617 2023-05-10 03:31:30.000000 pyhalo-0.2.0/pyHalo/pyhalo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    26366 2023-05-10 03:31:30.000000 pyhalo-0.2.0/pyHalo/realization_extensions.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    36187 2023-05-10 03:31:30.000000 pyhalo-0.2.0/pyHalo/single_realization.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1176 2023-05-10 03:31:30.000000 pyhalo-0.2.0/pyHalo/truncation_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    13604 2023-05-10 03:31:30.000000 pyhalo-0.2.0/pyHalo/utilities.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-10 03:55:10.476848 pyhalo-0.2.0/pyHalo.egg-info/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-05-10 03:55:10.000000 pyhalo-0.2.0/pyHalo.egg-info/PKG-INFO
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2539 2023-05-10 03:55:10.000000 pyhalo-0.2.0/pyHalo.egg-info/SOURCES.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)        1 2023-05-10 03:55:10.000000 pyhalo-0.2.0/pyHalo.egg-info/dependency_links.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)       43 2023-05-10 03:55:10.000000 pyhalo-0.2.0/pyHalo.egg-info/entry_points.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)        1 2018-08-23 21:07:23.000000 pyhalo-0.2.0/pyHalo.egg-info/not-zip-safe
+-rw-r--r--   0 danielgilman   (501) staff       (20)       11 2023-05-10 03:55:10.000000 pyhalo-0.2.0/pyHalo.egg-info/requires.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)        7 2023-05-10 03:55:10.000000 pyhalo-0.2.0/pyHalo.egg-info/top_level.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)      526 2023-05-10 03:37:12.000000 pyhalo-0.2.0/pyproject.toml
+-rw-r--r--   0 danielgilman   (501) staff       (20)      389 2023-05-10 03:55:10.824897 pyhalo-0.2.0/setup.cfg
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1594 2023-05-10 03:31:45.000000 pyhalo-0.2.0/setup.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-10 03:55:10.665311 pyhalo-0.2.0/tests/
+-rw-r--r--   0 danielgilman   (501) staff       (20)       61 2018-10-06 19:25:46.000000 pyhalo-0.2.0/tests/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1688 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_concentration_models.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-10 03:55:10.671231 pyhalo-0.2.0/tests/test_cosmology/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-10-18 06:20:01.000000 pyhalo-0.2.0/tests/test_cosmology/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5023 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_cosmology/test_cone_geometry.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3841 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_cosmology/test_cosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3969 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_cosmology/test_cylinder_geometry.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-10 03:55:10.800078 pyhalo-0.2.0/tests/test_halos/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-12-04 22:13:12.000000 pyhalo-0.2.0/tests/test_halos/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2981 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_halos/test_adiabatic_tides.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4220 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_halos/test_concentrations.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1334 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_halos/test_gaussian.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4656 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_halos/test_general_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3407 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_halos/test_lenscosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2682 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_halos/test_nfw_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3343 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_halos/test_pjaffe.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1665 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_halos/test_point_mass.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2719 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_halos/test_tnfw_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2446 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_halos/test_truncation.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5002 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_halos/test_uldm.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1068 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_halos/test_util.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      874 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_mass_function_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3224 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_preset_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8793 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_pyhalo_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    16257 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_realization_extensions.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-10 03:55:10.811419 pyhalo-0.2.0/tests/test_rendering/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.0/tests/test_rendering/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2584 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_rendering/test_2halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3422 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_rendering/test_los.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-10 03:55:10.816602 pyhalo-0.2.0/tests/test_rendering/test_mass_functions/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_rendering/test_mass_functions/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5915 2023-05-10 03:38:38.000000 pyhalo-0.2.0/tests/test_rendering/test_mass_functions/test_base_functions.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2173 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_rendering/test_mass_functions/test_delta_function.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    11175 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_rendering/test_mass_functions/test_sheth_tormen.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2936 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_rendering/test_population.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-10 03:55:10.821311 pyhalo-0.2.0/tests/test_rendering/test_spatial_distribution/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_rendering/test_spatial_distribution/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2096 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_rendering/test_spatial_distribution/test_correlated.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2191 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_rendering/test_spatial_distribution/test_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2153 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_rendering/test_spatial_distribution/test_uniform.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3491 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_rendering/test_subhalos.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    23809 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_single_realization.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3373 2023-05-10 03:31:30.000000 pyhalo-0.2.0/tests/test_utilities.py
```

### Comparing `pyhalo-0.0.1/CONTRIBUTING.rst` & `pyhalo-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/LICENSE` & `pyhalo-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/PKG-INFO` & `pyhalo-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhalo
-Version: 0.0.1
+Version: 0.2.0
 Summary: A python package for generating populations of dark matter halos
 Home-page: https://github.com/dangilman/pyHalo
 Author: Daniel Gilman
 Author-email: Daniel Gilman <daniel.gilman@utoronto.ca>
 License: MIT license
 Project-URL: Homepage, https://github.com/dangilman/pyHalo
 Project-URL: Bug Tracker, https://github.com/dangilman/pyHalo/issues
```

### Comparing `pyhalo-0.0.1/README.rst` & `pyhalo-0.2.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -4,27 +4,31 @@
 
 .. image:: https://travis-ci.com/dangilman/pyHalo.svg?branch=master
         :target: https://travis-ci.com/dangilman/pyHalo
 
 .. image:: https://coveralls.io/repos/github/dangilman/pyHalo/badge.svg?branch=master
         :target: https://coveralls.io/github/dangilman/pyHalo?branch=master
         
+.. image:: https://badge.fury.io/py/pyhalo.svg
+        :target: https://badge.fury.io/py/pyhalo.svg
+        
 .. image:: https://github.com/dangilman/pyHalo/blob/master/readme_fig.jpg
         :target: https://github.com/dangilman/pyHalo/blob/master/readme_fig
 
 pyHalo renders full mass distributions for substructure lensing simulations with the open source gravitational lensing software package lenstronomy (https://github.com/sibirrer/lenstronomy). The example notebooks illustrate the core functionality of this package. 
 
 If you would like to use this package and have questions, please get in touch with me at daniel.gilman@utoronto.ca - I am happy to help! 
 
 Installation
 ------------
-Clone the repository, navigate into the main pyHalo directory and run python3 setup.py develop --user. (in the process of making this pip-installable) 
+Download from pypi: pip install pyhalo
 
-In order to use this package you'll need to install colossus http://www.benediktdiemer.com/code/colossus/ 
+For earlier releases: clone the repository, select the version you want to download from the commit history (first code release is 8302393), clone it, run python3 setup.py develop --user. 
 
+In order to use this package when not installing via pip, you'll need to install colossus http://www.benediktdiemer.com/code/colossus/ 
 
 Features
 --------
 
 - Quickly render full populations of dark matter subhalos and line of sight halos for gravitational lensing simulations. Implemented models currently include cold and warm dark matter, custom mass-concentration relations, self-interacting dark matter, and more.
 - Translte halo properties (mass, concentration, redshift, etc) into angular units for lensing computations with lenstronomy
```

### Comparing `pyhalo-0.0.1/docs/Makefile` & `pyhalo-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/docs/conf.py` & `pyhalo-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/docs/installation.rst` & `pyhalo-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/docs/make.bat` & `pyhalo-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/pyHalo/concentration_models.py` & `pyhalo-0.2.0/pyHalo/concentration_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/pyHalo/defaults.py` & `pyhalo-0.2.0/pyHalo/defaults.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/pyHalo/mass_function_models.py` & `pyhalo-0.2.0/pyHalo/mass_function_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/pyHalo/preset_models.py` & `pyhalo-0.2.0/pyHalo/preset_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/pyHalo/pyhalo.py` & `pyhalo-0.2.0/pyHalo/pyhalo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/pyHalo/realization_extensions.py` & `pyhalo-0.2.0/pyHalo/realization_extensions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/pyHalo/single_realization.py` & `pyhalo-0.2.0/pyHalo/single_realization.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/pyHalo/truncation_models.py` & `pyhalo-0.2.0/pyHalo/truncation_models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,28 @@
-from pyHalo.Halos.tidal_truncation import TruncationRN, TruncationRoche
+from pyHalo.Halos.tidal_truncation import TruncationRN, TruncationRoche, AdiabaticTidesTruncation, TruncationSplashBack
+
 
 def truncation_models(model_name):
     """
     Loads and returns methods to set the tidal truncation radius (or equivalent parameter) of halos
     """
     kwargs_model = {}
     if model_name == 'TRUNCATION_R50':
-        kwargs_model['N'] = 50
+        kwargs_model['LOS_truncation_factor'] = 50
         # truncates NFW halos at r50 (for field halos, this is comparable to the splashback radius)
         return TruncationRN, kwargs_model
     elif model_name == 'TRUNCATION_RN':
         return TruncationRN, kwargs_model
     elif model_name == 'TRUNCATION_ROCHE':
         return TruncationRoche, kwargs_model
     elif model_name == 'TRUNCATION_ROCHE_GILMAN2020':
         kwargs_model['RocheNorm'] = 1.4
         kwargs_model['m_power'] = 1./3
         kwargs_model['RocheNu'] = 2./3
         return TruncationRoche, kwargs_model
+    elif model_name == 'ADIABATIC_TIDES':
+        return AdiabaticTidesTruncation, kwargs_model
+    elif model_name == 'SPLASHBACK':
+        return TruncationSplashBack, kwargs_model
+    else:
+        raise Exception('model '+str(model_name)+' not recognized')
+
```

### Comparing `pyhalo-0.0.1/pyHalo/utilities.py` & `pyhalo-0.2.0/pyHalo/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,45 @@
 import numpy as np
 from pyHalo.defaults import lenscone_default
 from scipy.interpolate import interp1d
 from pyHalo.Cosmology.cosmology import Cosmology
 from scipy.integrate import quad
 from pyHalo.Halos.lens_cosmo import LensCosmo
-from scipy.special import jv
 from scipy.integrate import simps
 from pyHalo.concentration_models import preset_concentration_models
 
+class ITSampling(object):
+
+    def __init__(self, samples):
+        """
+        This class performs inverse transform sampling of a distribution given samples from the distribution
+        :param samples: samples from the distribution
+        """
+        ran = (np.min(samples), np.max(samples))
+        h, x = np.histogram(samples, range=ran, bins=150)
+        x = x[0:-1] + (x[1] - x[0])/2
+        cdf = np.cumsum(h)
+        cdf = cdf / float(np.max(cdf))
+        self._cdf_inverse = interp1d(cdf, x)
+        self._umin = cdf[0]
+        self._umax = cdf[-1]
+
+    def __call__(self, n_samples):
+        """
+        Generates samples from the distribution
+        :param n_samples: number of samples to draw
+        :return: the samples
+        """
+        u = np.random.uniform(self._umin, self._umax, int(n_samples))
+        samples_out = self._cdf_inverse(u)
+        if n_samples == 1:
+            return float(samples_out)
+        else:
+            return np.squeeze(samples_out)
+
 def inverse_transform_sampling(x, function, args, n_samples):
     """
 
     :param x: the domain of the function across which you want to obtain samples
     :param function: the function or probability density you want to sample from
     :param args: arguments passed to function after x
     :param n_samples: number of samples to draw
@@ -166,66 +194,14 @@
         if terminate_at_source:
             d_src = comoving_distance_calc(zsource)
             x_list[-1] = source_x * d_src
             y_list[-1] = source_y * d_src
 
         return np.array(x_list), np.array(y_list), np.array(distances)
 
-def sample_density(probability_density, Nsamples, pixel_scale, x_0, y_0, Rmax, smoothing_scale=4):
-    """
-
-    :param probability_density:
-    :param Nsamples:
-    :param pixel_scale:
-    :param x_0:
-    :param y_0:
-    :param Rmax:
-    :param smoothing_scale:
-    :return:
-    """
-
-    probnorm = probability_density / probability_density.sum()
-
-    s = probnorm.shape[0]
-    p = probnorm.ravel()
-
-    values = np.arange(s ** 2)
-
-    x_out, y_out = np.array([]), np.array([])
-
-    ndraw = Nsamples
-
-    while ndraw > 0:
-        ndraw = Nsamples - len(x_out)
-
-        inds = np.random.choice(values, p=p, size=ndraw, replace=True)
-
-        pairs = np.indices(dimensions=(s, s)).T
-
-        locations = pairs.reshape(-1, 2)[inds]
-        x_sample_pixel, y_sample_pixel = locations[:, 0], locations[:, 1]
-
-        # transform to arcsec
-        x_sample_arcsec = (x_sample_pixel - s / 2) * pixel_scale
-        y_sample_arcsec = (y_sample_pixel - s / 2) * pixel_scale
-
-        # smooth on sub-pixel scale
-        pixel_smoothing_kernel = pixel_scale / smoothing_scale
-        # apply smoothing to remove artificial tiling
-        x_sample_arcsec += np.random.normal(0, pixel_smoothing_kernel, ndraw)
-        y_sample_arcsec += np.random.normal(0, pixel_smoothing_kernel, ndraw)
-
-        # keep circular symmetry
-        r = np.sqrt(x_sample_arcsec ** 2 + y_sample_arcsec ** 2)
-        keep = np.where(r <= Rmax)
-        x_out = np.append(x_out, x_sample_arcsec[keep])
-        y_out = np.append(y_out, y_sample_arcsec[keep])
-
-    return x_out, y_out
-
 def de_broglie_wavelength(log10_m_uldm,v):
     '''
     Returns de Broglie wavelength of the ultra-light axion in kpc.
 
     :param log10_m_uldm: log(axion mass) in eV
     :param v: velocity in km/s
     '''
```

### Comparing `pyhalo-0.0.1/pyHalo.egg-info/PKG-INFO` & `pyhalo-0.2.0/pyHalo.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhalo
-Version: 0.0.1
+Version: 0.2.0
 Summary: A python package for generating populations of dark matter halos
 Home-page: https://github.com/dangilman/pyHalo
 Author: Daniel Gilman
 Author-email: Daniel Gilman <daniel.gilman@utoronto.ca>
 License: MIT license
 Project-URL: Homepage, https://github.com/dangilman/pyHalo
 Project-URL: Bug Tracker, https://github.com/dangilman/pyHalo/issues
```

### Comparing `pyhalo-0.0.1/pyHalo.egg-info/SOURCES.txt` & `pyhalo-0.2.0/pyHalo.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -54,24 +54,26 @@
 tests/test_single_realization.py
 tests/test_utilities.py
 tests/test_cosmology/__init__.py
 tests/test_cosmology/test_cone_geometry.py
 tests/test_cosmology/test_cosmo.py
 tests/test_cosmology/test_cylinder_geometry.py
 tests/test_halos/__init__.py
+tests/test_halos/test_adiabatic_tides.py
 tests/test_halos/test_concentrations.py
 tests/test_halos/test_gaussian.py
 tests/test_halos/test_general_nfw.py
 tests/test_halos/test_lenscosmo.py
 tests/test_halos/test_nfw_halo.py
 tests/test_halos/test_pjaffe.py
 tests/test_halos/test_point_mass.py
 tests/test_halos/test_tnfw_halo.py
 tests/test_halos/test_truncation.py
 tests/test_halos/test_uldm.py
+tests/test_halos/test_util.py
 tests/test_rendering/__init__.py
 tests/test_rendering/test_2halo.py
 tests/test_rendering/test_los.py
 tests/test_rendering/test_population.py
 tests/test_rendering/test_subhalos.py
 tests/test_rendering/test_mass_functions/__init__.py
 tests/test_rendering/test_mass_functions/test_base_functions.py
```

### Comparing `pyhalo-0.0.1/pyproject.toml` & `pyhalo-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyhalo"
-version = "0.0.1"
+version = "0.2.0"
 authors = [
   { name="Daniel Gilman", email="daniel.gilman@utoronto.ca" },
 ]
 description = "A python package for generating populations of dark matter halos"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `pyhalo-0.0.1/setup.py` & `pyhalo-0.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,16 +40,16 @@
         ],
     },
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='pyHalo',
-    name='pyHalo',
+    name='pyhalo',
     packages=find_packages(include=['pyHalo']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/dangilman/pyHalo',
-    version='0.1.0',
+    version='0.2.0',
     zip_safe=False,
 )
```

### Comparing `pyhalo-0.0.1/tests/test_concentration_models.py` & `pyhalo-0.2.0/tests/test_concentration_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/tests/test_cosmology/test_cone_geometry.py` & `pyhalo-0.2.0/tests/test_cosmology/test_cone_geometry.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/tests/test_cosmology/test_cosmo.py` & `pyhalo-0.2.0/tests/test_cosmology/test_cosmo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/tests/test_cosmology/test_cylinder_geometry.py` & `pyhalo-0.2.0/tests/test_cosmology/test_cylinder_geometry.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/tests/test_halos/test_concentrations.py` & `pyhalo-0.2.0/tests/test_halos/test_concentrations.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/tests/test_halos/test_gaussian.py` & `pyhalo-0.2.0/tests/test_halos/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/tests/test_halos/test_general_nfw.py` & `pyhalo-0.2.0/tests/test_halos/test_general_nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/tests/test_halos/test_lenscosmo.py` & `pyhalo-0.2.0/tests/test_halos/test_lenscosmo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/tests/test_halos/test_nfw_halo.py` & `pyhalo-0.2.0/tests/test_halos/test_nfw_halo.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
         astropy = FlatLambdaCDM(70.0, 0.3)
         cosmo = Cosmology(astropy_instance=astropy)
         self.zhalo = 0.5
         self.zsource = 2.0
         self.lens_cosmo = LensCosmo(self.zhalo, self.zsource, cosmo)
         self.truncation_class = None
-        self.concentration_class = ConcentrationDiemerJoyce(self.lens_cosmo)
+        self.concentration_class = ConcentrationDiemerJoyce(self.lens_cosmo, scatter=False)
         self.lclenstronomy = LensCosmoLenstronomy(self.zhalo, self.zsource, astropy)
 
     def test_lenstronomy_params(self):
 
         m = 10 ** 8
         x = 0.5
         y = 1.0
```

### Comparing `pyhalo-0.0.1/tests/test_halos/test_pjaffe.py` & `pyhalo-0.2.0/tests/test_halos/test_pjaffe.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/tests/test_halos/test_point_mass.py` & `pyhalo-0.2.0/tests/test_halos/test_point_mass.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/tests/test_halos/test_tnfw_halo.py` & `pyhalo-0.2.0/tests/test_halos/test_tnfw_halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/tests/test_halos/test_uldm.py` & `pyhalo-0.2.0/tests/test_halos/test_uldm.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         _,theta_c,kappa_0 = self.subhalo.profile_args
         rho0 = Uldm().density_lens(0,uldm_kwargs['kappa_0'],
                                     uldm_kwargs['theta_c'])
         rhos = CNFW().density_lens(0,cnfw_kwargs['Rs'],
                                  cnfw_kwargs['alpha_Rs'],
                                  cnfw_kwargs['r_core'])
         rho_goal = Uldm().density_lens(0,kappa_0,theta_c)
-        npt.assert_array_less(np.array([1-(rho0+rhos)/rho_goal]),np.array([0.03])) # less than 3% error
+        npt.assert_array_less(np.array([1-(rho0+rhos)/rho_goal]),np.array([0.1])) # less than 3% error
 
     def test_profile_normalization_fieldhalo(self):
         """
         Test that the mass enclosed within r200 of the composite profile is correct
         and check that the ULDM core density is correct.
         """
```

### Comparing `pyhalo-0.0.1/tests/test_mass_function_models.py` & `pyhalo-0.2.0/tests/test_mass_function_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/tests/test_preset_models.py` & `pyhalo-0.2.0/tests/test_preset_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/tests/test_pyhalo_base.py` & `pyhalo-0.2.0/tests/test_pyhalo_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/tests/test_realization_extensions.py` & `pyhalo-0.2.0/tests/test_realization_extensions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/tests/test_rendering/test_2halo.py` & `pyhalo-0.2.0/tests/test_rendering/test_2halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/tests/test_rendering/test_los.py` & `pyhalo-0.2.0/tests/test_rendering/test_los.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/tests/test_rendering/test_mass_functions/test_base_functions.py` & `pyhalo-0.2.0/tests/test_rendering/test_mass_functions/test_base_functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pytest
 import numpy as np
 import numpy.testing as npt
-from pyHalo.Cosmology.cosmology import Cosmology
 from pyHalo.Rendering.MassFunctions.mass_function_base import CDMPowerLaw, WDMPowerLaw, MixedWDMPowerLaw
 
 
 class TestCDMPowerLaw(object):
 
     def setup_method(self):
 
@@ -105,9 +104,38 @@
 
     def test_pure_cdm(self):
 
         first_moment_cdm = self.mass_function_mixed_pure_cdm.first_moment
         first_moment_mixed_pure_cdm = self.mass_function_pure_cdm.first_moment
         npt.assert_almost_equal(first_moment_cdm/first_moment_mixed_pure_cdm, 1.0, 8)
 
+# class TestTabulated(object):
+#
+#     def setup_method(self):
+#
+#         self.log_mlow = 6.0
+#         self.log_mhigh = 8.0
+#         self.power_law_index = -1.9
+#         self.draw_poisson = False
+#         self.normalization = 1e10
+#         self.mass_function_powerlaw = CDMPowerLaw(self.log_mlow, self.log_mhigh, self.power_law_index,
+#                                          self.draw_poisson, self.normalization)
+#
+#         m = np.logspace(6, 8, 1000)
+#         dndm = self.normalization * m ** self.power_law_index
+#         self.mass_function_tabulated = Tabulated(self.log_mlow, self.log_mhigh, self.draw_poisson,
+#                                                  m, dndm)
+#
+#     def test_zeroth_moment(self):
+#
+#         npt.assert_almost_equal(self.mass_function_powerlaw.n_mean/self.mass_function_tabulated.n_mean, 1.0, 3)
+#
+#     def test_first_moment(self):
+#
+#         npt.assert_almost_equal(self.mass_function_powerlaw.first_moment/self.mass_function_tabulated.first_moment, 1.0, 3)
+#         rendered = np.sum(self.mass_function_tabulated.draw())
+#         expected = np.sum(self.mass_function_powerlaw.draw())
+#         npt.assert_almost_equal(rendered/expected,1.0)
+
+
 if __name__ == '__main__':
    pytest.main()
```

### Comparing `pyhalo-0.0.1/tests/test_rendering/test_mass_functions/test_delta_function.py` & `pyhalo-0.2.0/tests/test_rendering/test_mass_functions/test_delta_function.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/tests/test_rendering/test_mass_functions/test_sheth_tormen.py` & `pyhalo-0.2.0/tests/test_rendering/test_mass_functions/test_sheth_tormen.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/tests/test_rendering/test_population.py` & `pyhalo-0.2.0/tests/test_rendering/test_population.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/tests/test_rendering/test_spatial_distribution/test_correlated.py` & `pyhalo-0.2.0/tests/test_rendering/test_spatial_distribution/test_correlated.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/tests/test_rendering/test_spatial_distribution/test_nfw.py` & `pyhalo-0.2.0/tests/test_rendering/test_spatial_distribution/test_nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/tests/test_rendering/test_spatial_distribution/test_uniform.py` & `pyhalo-0.2.0/tests/test_rendering/test_spatial_distribution/test_uniform.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/tests/test_rendering/test_subhalos.py` & `pyhalo-0.2.0/tests/test_rendering/test_subhalos.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/tests/test_single_realization.py` & `pyhalo-0.2.0/tests/test_single_realization.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.0.1/tests/test_utilities.py` & `pyhalo-0.2.0/tests/test_utilities.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from lenstronomy.LensModel.lens_model import LensModel
 import numpy.testing as npt
 import numpy as np
-from pyHalo.utilities import interpolate_ray_paths, de_broglie_wavelength, delta_sigma
+from pyHalo.utilities import interpolate_ray_paths, de_broglie_wavelength, delta_sigma, ITSampling, inverse_transform_sampling
 from pyHalo.Cosmology.cosmology import Cosmology
-
+import pytest
 
 class TestUtilities(object):
 
     def test_interp_ray_paths(self):
 
         cosmo = Cosmology()
         x = [1.4, -1.]
@@ -47,7 +47,32 @@
         m=1e13 #M_solar
         rein=6. #kpc
 
         lambda_dB = de_broglie_wavelength(log10_m_uldm,v)
         npt.assert_almost_equal(lambda_dB,0.6)
         delta_kappa = delta_sigma(m,z_lens,rein,lambda_dB)
         npt.assert_almost_equal(delta_kappa/80837585.696, 1, 2)
+
+    def test_inverse_transform_sampling(self):
+
+        mu = 2.0
+        sigma = 1.5
+        func = lambda x: np.exp(-0.5 * (x - mu) ** 2 / sigma**2)
+        x = np.linspace(mu - 5*sigma, mu + 5*sigma, 1000)
+        x_samples = inverse_transform_sampling(x, func, (), 100000)
+        npt.assert_almost_equal(np.mean(x_samples)/mu, 1.0, 2)
+        npt.assert_almost_equal(np.std(x_samples)/sigma, 1.0, 2)
+
+    def test_ITSampling(self):
+
+        mu = 2.14
+        sigma = 0.35
+        x = np.random.normal(mu, sigma, 250000)
+        sampler = ITSampling(x)
+        x_samples = sampler(100000)
+        npt.assert_almost_equal(np.mean(x_samples)/mu, 1.0, 2)
+        npt.assert_almost_equal(np.std(x_samples)/sigma, 1.0, 2)
+
+
+if __name__ == '__main__':
+
+    pytest.main()
```

