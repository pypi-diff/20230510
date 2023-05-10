# Comparing `tmp/pyTMD-2.0.3.tar.gz` & `tmp/pyTMD-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTMD-2.0.3.tar", last modified: Sat Apr  8 20:10:31 2023, max compression
+gzip compressed data, was "pyTMD-2.0.4.tar", last modified: Wed May 10 18:23:56 2023, max compression
```

## Comparing `pyTMD-2.0.3.tar` & `pyTMD-2.0.4.tar`

### file list

```diff
@@ -1,71 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 20:10:31.279295 pyTMD-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (122)      442 2023-04-08 20:10:16.000000 pyTMD-2.0.3/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)      908 2023-04-08 20:10:16.000000 pyTMD-2.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      620 2023-04-08 20:10:16.000000 pyTMD-2.0.3/CONTRIBUTORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-04-08 20:10:16.000000 pyTMD-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-08 20:10:16.000000 pyTMD-2.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7831 2023-04-08 20:10:31.279295 pyTMD-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6929 2023-04-08 20:10:16.000000 pyTMD-2.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-04-08 20:10:16.000000 pyTMD-2.0.3/postBuild
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 20:10:31.263295 pyTMD-2.0.3/pyTMD/
--rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14671 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/astro.py
--rw-r--r--   0 runner    (1001) docker     (122)     3376 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/calc_astrol_longitudes.py
--rw-r--r--   0 runner    (1001) docker     (122)     8723 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/check_tide_points.py
--rw-r--r--   0 runner    (1001) docker     (122)    53397 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/compute_tide_corrections.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    12861 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    16115 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/convert_crs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2974 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/convert_ll_xy.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 20:10:31.275295 pyTMD-2.0.3/pyTMD/data/
--rwxr-xr-x   0 runner    (1001) docker     (122)    12369 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/data/deltat.data
--rwxr-xr-x   0 runner    (1001) docker     (122)  3529324 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/data/finals.all
--rwxr-xr-x   0 runner    (1001) docker     (122)    30345 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/data/historic_deltat.data
--rwxr-xr-x   0 runner    (1001) docker     (122)   130160 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/data/iers_deltat.data
--rwxr-xr-x   0 runner    (1001) docker     (122)    10666 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/data/leap-seconds.list
--rwxr-xr-x   0 runner    (1001) docker     (122)    78848 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/data/mean-pole.tab
--rwxr-xr-x   0 runner    (1001) docker     (122)   153560 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/data/merged_deltat.data
--rwxr-xr-x   0 runner    (1001) docker     (122)  6325011 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/data/opoleloadcoefcmcor.txt.gz
--rwxr-xr-x   0 runner    (1001) docker     (122)    40928 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/data/ser7.dat
--rw-r--r--   0 runner    (1001) docker     (122)    15314 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/eop.py
--rw-r--r--   0 runner    (1001) docker     (122)    15243 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/interpolate.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 20:10:31.275295 pyTMD-2.0.3/pyTMD/io/
--rw-r--r--   0 runner    (1001) docker     (122)    42922 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/io/ATLAS.py
--rw-r--r--   0 runner    (1001) docker     (122)    31482 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/io/FES.py
--rw-r--r--   0 runner    (1001) docker     (122)    28297 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/io/GOT.py
--rw-r--r--   0 runner    (1001) docker     (122)    70382 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/io/OTIS.py
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4469 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/io/constituents.py
--rw-r--r--   0 runner    (1001) docker     (122)    71442 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/io/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     5761 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/io/ocean_pole_tide.py
--rw-r--r--   0 runner    (1001) docker     (122)     4731 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/load_constituent.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    21033 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/load_nodal_corrections.py
--rw-r--r--   0 runner    (1001) docker     (122)    39924 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)    53934 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/spatial.py
--rw-r--r--   0 runner    (1001) docker     (122)     2945 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/tidal_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (122)    47262 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/time.py
--rw-r--r--   0 runner    (1001) docker     (122)    11766 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/tools.py
--rw-r--r--   0 runner    (1001) docker     (122)    37472 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 20:10:31.263295 pyTMD-2.0.3/pyTMD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7831 2023-04-08 20:10:31.000000 pyTMD-2.0.3/pyTMD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1447 2023-04-08 20:10:31.000000 pyTMD-2.0.3/pyTMD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-08 20:10:31.000000 pyTMD-2.0.3/pyTMD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-04-08 20:10:31.000000 pyTMD-2.0.3/pyTMD.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-08 20:10:31.000000 pyTMD-2.0.3/pyTMD.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-08 20:10:16.000000 pyTMD-2.0.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-04-08 20:10:16.000000 pyTMD-2.0.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 20:10:31.279295 pyTMD-2.0.3/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)     5421 2023-04-08 20:10:16.000000 pyTMD-2.0.3/scripts/arcticdata_tides.py
--rw-r--r--   0 runner    (1001) docker     (122)    13042 2023-04-08 20:10:16.000000 pyTMD-2.0.3/scripts/aviso_fes_tides.py
--rw-r--r--   0 runner    (1001) docker     (122)    16845 2023-04-08 20:10:16.000000 pyTMD-2.0.3/scripts/compute_LPET_elevations.py
--rw-r--r--   0 runner    (1001) docker     (122)    20936 2023-04-08 20:10:16.000000 pyTMD-2.0.3/scripts/compute_LPT_displacements.py
--rw-r--r--   0 runner    (1001) docker     (122)    23346 2023-04-08 20:10:16.000000 pyTMD-2.0.3/scripts/compute_OPT_displacements.py
--rw-r--r--   0 runner    (1001) docker     (122)    20421 2023-04-08 20:10:16.000000 pyTMD-2.0.3/scripts/compute_SET_displacements.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    25487 2023-04-08 20:10:16.000000 pyTMD-2.0.3/scripts/compute_tidal_currents.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    25673 2023-04-08 20:10:16.000000 pyTMD-2.0.3/scripts/compute_tidal_elevations.py
--rw-r--r--   0 runner    (1001) docker     (122)    11669 2023-04-08 20:10:16.000000 pyTMD-2.0.3/scripts/reduce_OTIS_files.py
--rw-r--r--   0 runner    (1001) docker     (122)     5128 2023-04-08 20:10:16.000000 pyTMD-2.0.3/scripts/usap_cats_tides.py
--rw-r--r--   0 runner    (1001) docker     (122)     7865 2023-04-08 20:10:16.000000 pyTMD-2.0.3/scripts/verify_box_tpxo.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-08 20:10:31.279295 pyTMD-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3960 2023-04-08 20:10:16.000000 pyTMD-2.0.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-08 20:10:16.000000 pyTMD-2.0.3/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 18:23:56.429118 pyTMD-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-05-10 18:23:42.000000 pyTMD-2.0.4/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-05-10 18:23:42.000000 pyTMD-2.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     5545 2023-05-10 18:23:42.000000 pyTMD-2.0.4/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      620 2023-05-10 18:23:42.000000 pyTMD-2.0.4/CONTRIBUTORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-05-10 18:23:42.000000 pyTMD-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-10 18:23:42.000000 pyTMD-2.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6792 2023-05-10 18:23:56.429118 pyTMD-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5890 2023-05-10 18:23:42.000000 pyTMD-2.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-05-10 18:23:42.000000 pyTMD-2.0.4/postBuild
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 18:23:56.413118 pyTMD-2.0.4/pyTMD/
+-rw-r--r--   0 runner    (1001) docker     (122)     1422 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    20738 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43001 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/astro.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3376 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/calc_astrol_longitudes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9072 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/check_tide_points.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43968 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/compute_tide_corrections.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    12861 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16129 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/convert_crs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2974 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/convert_ll_xy.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 18:23:56.425118 pyTMD-2.0.4/pyTMD/data/
+-rwxr-xr-x   0 runner    (1001) docker     (122)    12369 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/data/deltat.data
+-rwxr-xr-x   0 runner    (1001) docker     (122)  3534588 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/data/finals.all
+-rwxr-xr-x   0 runner    (1001) docker     (122)    30345 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/data/historic_deltat.data
+-rwxr-xr-x   0 runner    (1001) docker     (122)   130160 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/data/iers_deltat.data
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10666 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/data/leap-seconds.list
+-rwxr-xr-x   0 runner    (1001) docker     (122)    78880 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/data/mean-pole.tab
+-rwxr-xr-x   0 runner    (1001) docker     (122)   154120 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/data/merged_deltat.data
+-rwxr-xr-x   0 runner    (1001) docker     (122)  6325011 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/data/opoleloadcoefcmcor.txt.gz
+-rwxr-xr-x   0 runner    (1001) docker     (122)    41126 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/data/ser7.dat
+-rw-r--r--   0 runner    (1001) docker     (122)     5849 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/data/tab5.2e.txt
+-rw-r--r--   0 runner    (1001) docker     (122)   145678 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/data/tab5.3a.txt
+-rw-r--r--   0 runner    (1001) docker     (122)   113660 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/data/tab5.3b.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    17529 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/eop.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15243 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/interpolate.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 18:23:56.429118 pyTMD-2.0.4/pyTMD/io/
+-rw-r--r--   0 runner    (1001) docker     (122)    43622 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/io/ATLAS.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31908 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/io/FES.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28562 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/io/GOT.py
+-rw-r--r--   0 runner    (1001) docker     (122)    71516 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/io/OTIS.py
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4469 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/io/constituents.py
+-rw-r--r--   0 runner    (1001) docker     (122)    66799 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/io/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6162 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/io/ocean_pole_tide.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/load_constituent.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4904 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/load_nodal_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42856 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)    61796 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2966 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/tidal_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (122)    59301 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11840 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39544 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 18:23:56.413118 pyTMD-2.0.4/pyTMD.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6792 2023-05-10 18:23:56.000000 pyTMD-2.0.4/pyTMD.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1555 2023-05-10 18:23:56.000000 pyTMD-2.0.4/pyTMD.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 18:23:56.000000 pyTMD-2.0.4/pyTMD.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-10 18:23:56.000000 pyTMD-2.0.4/pyTMD.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-10 18:23:56.000000 pyTMD-2.0.4/pyTMD.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-10 18:23:42.000000 pyTMD-2.0.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-05-10 18:23:42.000000 pyTMD-2.0.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 18:23:56.429118 pyTMD-2.0.4/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)     5497 2023-05-10 18:23:42.000000 pyTMD-2.0.4/scripts/arcticdata_tides.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13412 2023-05-10 18:23:42.000000 pyTMD-2.0.4/scripts/aviso_fes_tides.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14751 2023-05-10 18:23:42.000000 pyTMD-2.0.4/scripts/compute_LPET_elevations.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18641 2023-05-10 18:23:42.000000 pyTMD-2.0.4/scripts/compute_LPT_displacements.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20962 2023-05-10 18:23:42.000000 pyTMD-2.0.4/scripts/compute_OPT_displacements.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19178 2023-05-10 18:23:42.000000 pyTMD-2.0.4/scripts/compute_SET_displacements.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    23166 2023-05-10 18:23:42.000000 pyTMD-2.0.4/scripts/compute_tidal_currents.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    23367 2023-05-10 18:23:42.000000 pyTMD-2.0.4/scripts/compute_tidal_elevations.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11545 2023-05-10 18:23:42.000000 pyTMD-2.0.4/scripts/reduce_OTIS_files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5125 2023-05-10 18:23:42.000000 pyTMD-2.0.4/scripts/usap_cats_tides.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7921 2023-05-10 18:23:42.000000 pyTMD-2.0.4/scripts/verify_box_tpxo.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-10 18:23:56.429118 pyTMD-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3960 2023-05-10 18:23:42.000000 pyTMD-2.0.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-10 18:23:42.000000 pyTMD-2.0.4/version.txt
```

### Comparing `pyTMD-2.0.3/.gitignore` & `pyTMD-2.0.4/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 .DS_Store?
 ._*
 .Spotlight-V100
 .Trashes
 ehthumbs.db
 Thumbs.db
 # LaTeX and Vim #
-######################
+#################
 *.aux
 *.bbl
 *.blg
 *.dvi
 *.fdb_latexmk
 *.glg
 *.glo
@@ -80,11 +80,15 @@
 *.vrb
 *.maf
 *.mtc
 *.mtc0
 *.sw*
 *.hidden
 None*.png
+# JPL ephemerides #
+# #################
+*.bpc
+*.bsp
 # Jupyter Checkpoints #
 #######################
 .ipynb_checkpoints
 Untitled.ipynb
```

### Comparing `pyTMD-2.0.3/CONTRIBUTORS.rst` & `pyTMD-2.0.4/CONTRIBUTORS.rst`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.3/LICENSE` & `pyTMD-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.3/PKG-INFO` & `pyTMD-2.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTMD
-Version: 2.0.3
+Version: 2.0.4
 Summary: Tide Model Driver to read OTIS, GOT and FES formatted tidal solutions and make tidal predictions
 Home-page: https://github.com/tsutterley/pyTMD
 Author: Tyler Sutterley
 Author-email: tsutterl@uw.edu
 License: MIT
 Keywords: Ocean Tides,Load Tides,Pole Tides,Tidal Prediction,OTIS,GOT,FES
 Classifier: Development Status :: 3 - Alpha
@@ -26,16 +26,14 @@
 
 |Language|
 |License|
 |PyPI Version|
 |Anaconda-Server|
 |Documentation Status|
 |codecov|
-|Binder|
-|Pangeo|
 |zenodo|
 
 .. |Language| image:: https://img.shields.io/pypi/pyversions/pyTMD?color=green
    :target: https://www.python.org/
 
 .. |License| image:: https://img.shields.io/github/license/tsutterley/pyTMD
    :target: https://github.com/tsutterley/pyTMD/blob/main/LICENSE
@@ -48,23 +46,16 @@
 
 .. |Documentation Status| image:: https://readthedocs.org/projects/pytmd/badge/?version=latest
    :target: https://pytmd.readthedocs.io/en/latest/?badge=latest
 
 .. |codecov| image:: https://codecov.io/gh/tsutterley/pyTMD/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/tsutterley/pyTMD
 
-.. |Binder| image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/tsutterley/pyTMD/main
-
-.. |Pangeo| image:: https://img.shields.io/static/v1.svg?logo=Jupyter&label=PangeoBinderAWS&message=us-west-2&color=orange
-   :target: https://aws-uswest2-binder.pangeo.io/v2/gh/tsutterley/pyTMD/main?urlpath=lab
-
-.. |zenodo| image:: https://zenodo.org/badge/107997403.svg
-   :target: https://zenodo.org/badge/latestdoi/107997403
-
+.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5555395.svg
+   :target: https://doi.org/10.5281/zenodo.5555395
 
 Python-based tidal prediction software for estimating ocean, load, solid Earth and pole tides
 
 Ocean and load tidal predictions using OTIS, GOT and FES formatted tidal solutions
 
 - `OSU Tidal Prediction Software (OTPS) <https://www.tpxo.net/otps>`_
 - `ESR Tide Model Driver (TMD) Matlab Toolbox <https://www.esr.org/research/polar-tide-models/tmd-software/>`_
@@ -83,39 +74,32 @@
 - `IERS Daily Earth Orientation Parameters (EOP) from USNO <http://www.usno.navy.mil/USNO/earth-orientation/eo-products/weekly>`_
 - `IERS Daily Earth Orientation Parameters (EOP) from NASA CDDIS <ftp://cddis.nasa.gov/products/iers/finals.all>`_
 - `IERS Ocean Pole Load Tide Coefficients Map <http://maia.usno.navy.mil/conventions/2010/2010_update/chapter7/additional_info/opoleloadcoefcmcor.txt.gz>`_
 
 Dependencies
 ############
 
-- `cartopy: Python package designed for geospatial data processing <https://scitools.org.uk/cartopy/docs/latest/>`_
 - `dateutil: powerful extensions to datetime <https://dateutil.readthedocs.io/en/stable/>`_
-- `gdal: Pythonic interface to the Geospatial Data Abstraction Library (GDAL) <https://pypi.python.org/pypi/GDAL>`_
-- `h5py: Python interface for Hierarchal Data Format 5 (HDF5) <https://www.h5py.org/>`_
-- `ipyleaflet: Jupyter / Leaflet bridge enabling interactive maps <https://github.com/jupyter-widgets/ipyleaflet>`_
-- `ipywidgets: interactive HTML widgets for Jupyter notebooks and IPython <https://ipywidgets.readthedocs.io/en/latest/>`_
 - `lxml: processing XML and HTML in Python <https://pypi.python.org/pypi/lxml>`_
-- `matplotlib: Python 2D plotting library <https://matplotlib.org/>`_
 - `netCDF4: Python interface to the netCDF C library <https://unidata.github.io/netcdf4-python/>`_
 - `numpy: Scientific Computing Tools For Python <https://www.numpy.org>`_
 - `pyproj: Python interface to PROJ library <https://pypi.org/project/pyproj/>`_
-- `PyYAML: YAML parser and emitter for Python <https://github.com/yaml/pyyaml>`_
 - `scipy: Scientific Tools for Python <https://www.scipy.org/>`_
 - `setuptools_scm: manager for python package versions using scm metadata <https://pypi.org/project/setuptools-scm/1.9.0/>`_
 
 References
 ##########
 
     T. C. Sutterley, T. Markus, T. A. Neumann, M. R. van den Broeke, J. M. van Wessem, and S. R. M. Ligtenberg,
     "Antarctic ice shelf thickness change from multimission lidar mapping", *The Cryosphere*,
-    13, 1801-1817, (2019). `doi:tc-13-1801-2019 <https://doi.org/10.5194/tc-13-1801-2019>`_
+    13, 1801-1817, (2019). `doi: 10.5194/tc-13-1801-2019 <https://doi.org/10.5194/tc-13-1801-2019>`_
 
     L. Padman, M. R. Siegfried, H. A. Fricker,
     "Ocean Tide Influences on the Antarctic and Greenland Ice Sheets", *Reviews of Geophysics*,
-    56, 142-184, (2018). `doi:10.1002/2016RG000546 <https://doi.org/10.1002/2016RG000546>`_
+    56, 142-184, (2018). `doi: 10.1002/2016RG000546 <https://doi.org/10.1002/2016RG000546>`_
 
 Download
 ########
 
 | The program homepage is:
 | https://github.com/tsutterley/pyTMD
 | A zip archive of the latest version is available directly at:
```

### Comparing `pyTMD-2.0.3/README.rst` & `pyTMD-2.0.4/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 
 |Language|
 |License|
 |PyPI Version|
 |Anaconda-Server|
 |Documentation Status|
 |codecov|
-|Binder|
-|Pangeo|
 |zenodo|
 
 .. |Language| image:: https://img.shields.io/pypi/pyversions/pyTMD?color=green
    :target: https://www.python.org/
 
 .. |License| image:: https://img.shields.io/github/license/tsutterley/pyTMD
    :target: https://github.com/tsutterley/pyTMD/blob/main/LICENSE
@@ -26,23 +24,16 @@
 
 .. |Documentation Status| image:: https://readthedocs.org/projects/pytmd/badge/?version=latest
    :target: https://pytmd.readthedocs.io/en/latest/?badge=latest
 
 .. |codecov| image:: https://codecov.io/gh/tsutterley/pyTMD/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/tsutterley/pyTMD
 
-.. |Binder| image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/tsutterley/pyTMD/main
-
-.. |Pangeo| image:: https://img.shields.io/static/v1.svg?logo=Jupyter&label=PangeoBinderAWS&message=us-west-2&color=orange
-   :target: https://aws-uswest2-binder.pangeo.io/v2/gh/tsutterley/pyTMD/main?urlpath=lab
-
-.. |zenodo| image:: https://zenodo.org/badge/107997403.svg
-   :target: https://zenodo.org/badge/latestdoi/107997403
-
+.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5555395.svg
+   :target: https://doi.org/10.5281/zenodo.5555395
 
 Python-based tidal prediction software for estimating ocean, load, solid Earth and pole tides
 
 Ocean and load tidal predictions using OTIS, GOT and FES formatted tidal solutions
 
 - `OSU Tidal Prediction Software (OTPS) <https://www.tpxo.net/otps>`_
 - `ESR Tide Model Driver (TMD) Matlab Toolbox <https://www.esr.org/research/polar-tide-models/tmd-software/>`_
@@ -61,39 +52,32 @@
 - `IERS Daily Earth Orientation Parameters (EOP) from USNO <http://www.usno.navy.mil/USNO/earth-orientation/eo-products/weekly>`_
 - `IERS Daily Earth Orientation Parameters (EOP) from NASA CDDIS <ftp://cddis.nasa.gov/products/iers/finals.all>`_
 - `IERS Ocean Pole Load Tide Coefficients Map <http://maia.usno.navy.mil/conventions/2010/2010_update/chapter7/additional_info/opoleloadcoefcmcor.txt.gz>`_
 
 Dependencies
 ############
 
-- `cartopy: Python package designed for geospatial data processing <https://scitools.org.uk/cartopy/docs/latest/>`_
 - `dateutil: powerful extensions to datetime <https://dateutil.readthedocs.io/en/stable/>`_
-- `gdal: Pythonic interface to the Geospatial Data Abstraction Library (GDAL) <https://pypi.python.org/pypi/GDAL>`_
-- `h5py: Python interface for Hierarchal Data Format 5 (HDF5) <https://www.h5py.org/>`_
-- `ipyleaflet: Jupyter / Leaflet bridge enabling interactive maps <https://github.com/jupyter-widgets/ipyleaflet>`_
-- `ipywidgets: interactive HTML widgets for Jupyter notebooks and IPython <https://ipywidgets.readthedocs.io/en/latest/>`_
 - `lxml: processing XML and HTML in Python <https://pypi.python.org/pypi/lxml>`_
-- `matplotlib: Python 2D plotting library <https://matplotlib.org/>`_
 - `netCDF4: Python interface to the netCDF C library <https://unidata.github.io/netcdf4-python/>`_
 - `numpy: Scientific Computing Tools For Python <https://www.numpy.org>`_
 - `pyproj: Python interface to PROJ library <https://pypi.org/project/pyproj/>`_
-- `PyYAML: YAML parser and emitter for Python <https://github.com/yaml/pyyaml>`_
 - `scipy: Scientific Tools for Python <https://www.scipy.org/>`_
 - `setuptools_scm: manager for python package versions using scm metadata <https://pypi.org/project/setuptools-scm/1.9.0/>`_
 
 References
 ##########
 
     T. C. Sutterley, T. Markus, T. A. Neumann, M. R. van den Broeke, J. M. van Wessem, and S. R. M. Ligtenberg,
     "Antarctic ice shelf thickness change from multimission lidar mapping", *The Cryosphere*,
-    13, 1801-1817, (2019). `doi:tc-13-1801-2019 <https://doi.org/10.5194/tc-13-1801-2019>`_
+    13, 1801-1817, (2019). `doi: 10.5194/tc-13-1801-2019 <https://doi.org/10.5194/tc-13-1801-2019>`_
 
     L. Padman, M. R. Siegfried, H. A. Fricker,
     "Ocean Tide Influences on the Antarctic and Greenland Ice Sheets", *Reviews of Geophysics*,
-    56, 142-184, (2018). `doi:10.1002/2016RG000546 <https://doi.org/10.1002/2016RG000546>`_
+    56, 142-184, (2018). `doi: 10.1002/2016RG000546 <https://doi.org/10.1002/2016RG000546>`_
 
 Download
 ########
 
 | The program homepage is:
 | https://github.com/tsutterley/pyTMD
 | A zip archive of the latest version is available directly at:
```

### Comparing `pyTMD-2.0.3/pyTMD/__init__.py` & `pyTMD-2.0.4/pyTMD/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import pyTMD.predict
 import pyTMD.spatial
 import pyTMD.time
 import pyTMD.tools
 import pyTMD.utilities
 import pyTMD.version
 from pyTMD import io
+from pyTMD.arguments import arguments
 from pyTMD.check_tide_points import check_tide_points
 from pyTMD.compute_tide_corrections import (
     compute_corrections,
     compute_tide_corrections,
     compute_LPET_corrections,
     compute_LPT_corrections,
     compute_OPT_corrections,
@@ -32,15 +33,16 @@
 )
 from pyTMD.constants import (
     constants,
     _ellipsoids
 )
 from pyTMD.convert_crs import convert_crs
 from pyTMD.load_constituent import load_constituent
-from pyTMD.load_nodal_corrections import load_nodal_corrections
 from pyTMD.tidal_ellipse import tidal_ellipse
 
 # Deprecated functions
+from pyTMD.calc_astrol_longitudes import calc_astrol_longitudes
 from pyTMD.convert_ll_xy import convert_ll_xy
+from pyTMD.load_nodal_corrections import load_nodal_corrections
 
 # get semantic version from setuptools-scm
 __version__ = pyTMD.version.version
```

### Comparing `pyTMD-2.0.3/pyTMD/calc_astrol_longitudes.py` & `pyTMD-2.0.4/pyTMD/calc_astrol_longitudes.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.3/pyTMD/check_tide_points.py` & `pyTMD-2.0.4/pyTMD/check_tide_points.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 check_tide_points.py
-Written by Tyler Sutterley (03/2023)
+Written by Tyler Sutterley (04/2023)
 Check if points are within a tide model domain
 
 OTIS format tidal solutions provided by Ohio State University and ESR
     http://volkov.oce.orst.edu/tides/region.html
     https://www.esr.org/research/polar-tide-models/list-of-polar-tide-models/
     ftp://ftp.esr.org/pub/datasets/tmd/
 Global Tide Model (GOT) solutions provided by Richard Ray at GSFC
@@ -48,14 +48,15 @@
     io/OTIS.py: extract tidal harmonic constants from OTIS tide models
     io/ATLAS.py: extract tidal harmonic constants from ATLAS netcdf models
     io/GOT.py: extract tidal harmonic constants from GSFC GOT models
     io/FES.py: extract tidal harmonic constants from FES tide models
     interpolate.py: interpolation routines for spatial data
 
 UPDATE HISTORY:
+    Updated 04/2023: using pathlib to define and expand paths
     Updated 03/2023: add basic variable typing to function inputs
     Updated 12/2022: refactored tide read programs under io
         refactored bilinear interpolation routine
     Updated 11/2022: place some imports within try/except statements
         use f-strings for formatting verbose or ascii output
     Updated 05/2022: added ESR netCDF4 formats to list of model types
         updated keyword arguments to read tide model programs
@@ -63,15 +64,15 @@
     Updated 09/2021: refactor to use model class for files and attributes
     Updated 07/2021: added check that tide model directory is accessible
     Updated 06/2021: add try/except for input projection strings
     Written 05/2021
 """
 from __future__ import print_function, annotations
 
-import os
+import pathlib
 import warnings
 import numpy as np
 import scipy.interpolate
 
 import pyTMD.io
 import pyTMD.io.model
 import pyTMD.convert_crs
@@ -84,19 +85,19 @@
     warnings.filterwarnings("module")
     warnings.warn("pyproj not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: compute tides at points and times using tide model algorithms
 def check_tide_points(x: np.ndarray, y: np.ndarray,
-        DIRECTORY: str | None = None,
+        DIRECTORY: str | pathlib.Path | None = None,
         MODEL: str | None = None,
         ATLAS_FORMAT: str = 'netcdf',
         GZIP: bool = False,
-        DEFINITION_FILE: str | None = None,
+        DEFINITION_FILE: str | pathlib.Path | None = None,
         EPSG: str | int = 3031,
         METHOD: str = 'spline'
     ):
     """
     Check if points are within a tide model domain
 
     Parameters
@@ -130,22 +131,23 @@
     Returns
     -------
     valid: bool
         array describing if input coordinate is within model domain
     """
 
     # check that tide directory is accessible
-    try:
-        os.access(DIRECTORY, os.F_OK)
-    except:
-        raise FileNotFoundError("Invalid tide directory")
+    if DIRECTORY is not None:
+        DIRECTORY = pathlib.Path(DIRECTORY).expanduser()
+        if not DIRECTORY.exists():
+            raise FileNotFoundError("Invalid tide directory")
 
     # get parameters for tide model
     if DEFINITION_FILE is not None:
-        model = pyTMD.io.model(DIRECTORY).from_file(DEFINITION_FILE)
+        model = pyTMD.io.model(DIRECTORY).from_file(
+            pathlib.Path(DEFINITION_FILE).expanduser())
     else:
         model = pyTMD.io.model(DIRECTORY, format=ATLAS_FORMAT,
             compressed=GZIP).elevation(MODEL)
 
     # input shape of data
     idim = np.shape(x)
     # converting x,y from input coordinate reference system
@@ -162,45 +164,48 @@
         np.atleast_1d(x).flatten(), np.atleast_1d(y).flatten()
     )
 
     # read tidal constants and interpolate to grid points
     if model.format in ('OTIS','ATLAS','ESR'):
         # if reading a single OTIS solution
         xi, yi, hz, mz, iob, dt = pyTMD.io.OTIS.read_otis_grid(
-            model.grid_file)
+            pathlib.Path(model.grid_file).expanduser())
         # invert model mask
         mz = np.logical_not(mz)
         # adjust dimensions of input coordinates to be iterable
         # run wrapper function to convert coordinate systems of input lat/lon
         X, Y = pyTMD.convert_crs(lon, lat, model.projection, 'F')
     elif (model.format == 'netcdf'):
         # if reading a netCDF OTIS atlas solution
-        xi, yi, hz = pyTMD.io.ATLAS.read_netcdf_grid(model.grid_file,
+        xi, yi, hz = pyTMD.io.ATLAS.read_netcdf_grid(
+            pathlib.Path(model.grid_file).expanduser(),
             compressed=model.compressed, type=model.type)
         # copy bathymetry mask
         mz = np.copy(hz.mask)
         # copy latitude and longitude and adjust longitudes
         X,Y = np.copy([lon,lat]).astype(np.float64)
         lt0, = np.nonzero(X < 0)
         X[lt0] += 360.0
     elif (model.format == 'GOT'):
         # if reading a NASA GOT solution
         hc, xi, yi, c = pyTMD.io.GOT.read_ascii_file(
-            model.model_file[0], compressed=model.compressed)
+            pathlib.Path(model.model_file[0]).expanduser(),
+            compressed=model.compressed)
         # copy tidal constituent mask
         mz = np.copy(hc.mask)
         # copy latitude and longitude and adjust longitudes
         X, Y = np.copy([lon,lat]).astype(np.float64)
         lt0, = np.nonzero(X < 0)
         X[lt0] += 360.0
     elif (model.format == 'FES'):
         # if reading a FES netCDF solution
         hc, xi, yi = pyTMD.io.FES.read_netcdf_file(
-            model.model_file[0], compressed=model.compressed,
-            type=model.type, version=model.version)
+            pathlib.Path(model.model_file[0]).expanduser(),
+            compressed=model.compressed, type=model.type,
+            version=model.version)
         # copy tidal constituent mask
         mz = np.copy(hc.mask)
         # copy latitude and longitude and adjust longitudes
         X, Y = np.copy([lon,lat]).astype(np.float64)
         lt0, = np.nonzero(X < 0)
         X[lt0] += 360.0
```

### Comparing `pyTMD-2.0.3/pyTMD/compute_tide_corrections.py` & `pyTMD-2.0.4/pyTMD/time.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,1228 +1,1686 @@
 #!/usr/bin/env python
 u"""
-compute_tide_corrections.py
-Written by Tyler Sutterley (04/2023)
-Calculates tidal elevations for correcting elevation or imagery data
-
-Ocean and Load Tides
-Uses OTIS format tidal solutions provided by Ohio State University and ESR
-    http://volkov.oce.orst.edu/tides/region.html
-    https://www.esr.org/research/polar-tide-models/list-of-polar-tide-models/
-    ftp://ftp.esr.org/pub/datasets/tmd/
-Global Tide Model (GOT) solutions provided by Richard Ray at GSFC
-or Finite Element Solution (FES) models provided by AVISO
-
-Long-Period Equilibrium Tides (LPET)
-Calculates long-period equilibrium tidal elevations for correcting
-elevation or imagery data from the summation of fifteen spectral lines
-    https://doi.org/10.1111/j.1365-246X.1973.tb03420.x
-
-Load Pole Tides (LPT)
-Calculates radial load pole tide displacements following IERS Convention
-(2010) guidelines for correcting elevation or imagery data
-    https://iers-conventions.obspm.fr/chapter7.php
-
-Ocean Pole Tides (OPT)
-Calculates radial ocean pole load tide displacements following IERS Convention
-(2010) guidelines for correcting elevation or imagery data
-    https://iers-conventions.obspm.fr/chapter7.php
-
-Ocean Pole Tides (SET)
-Calculates radial Solid Earth tide displacements following IERS Convention
-(2010) guidelines for correcting elevation or imagery data
-    https://iers-conventions.obspm.fr/chapter7.php
+time.py
+Written by Tyler Sutterley (05/2023)
+Utilities for calculating time operations
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
-        https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
-    scipy: Scientific Tools for Python
-        https://docs.scipy.org/doc/
-    netCDF4: Python interface to the netCDF C library
-         https://unidata.github.io/netcdf4-python/netCDF4/index.html
-    pyproj: Python interface to PROJ library
-        https://pypi.org/project/pyproj/
+    dateutil: powerful extensions to datetime
+        https://dateutil.readthedocs.io/en/stable/
+    lxml: processing XML and HTML in Python
+        https://pypi.python.org/pypi/lxml
 
 PROGRAM DEPENDENCIES:
-    time.py: utilities for calculating time operations
-    spatial: utilities for reading, writing and operating on spatial data
     utilities.py: download and management utilities for syncing files
-    astro.py: computes the basic astronomical mean longitudes
-    convert_crs.py: convert points to and from Coordinates Reference Systems
-    load_constituent.py: loads parameters for a given tidal constituent
-    load_nodal_corrections.py: load the nodal corrections for tidal constituents
-    predict.py: predict tide values using harmonic constants
-    io/model.py: retrieves tide model parameters for named tide models
-    io/OTIS.py: extract tidal harmonic constants from OTIS tide models
-    io/ATLAS.py: extract tidal harmonic constants from netcdf models
-    io/GOT.py: extract tidal harmonic constants from GSFC GOT models
-    io/FES.py: extract tidal harmonic constants from FES tide models
-    interpolate.py: interpolation routines for spatial data
 
 UPDATE HISTORY:
-    Updated 04/2023: added function for radial solid earth tides
+    Updated 05/2023: add timescale class for converting between time scales
+        added timescale to_datetime function to create datetime arrays
+        allow epoch arguments to be numpy datetime64 variables or strings
+    Updated 04/2023: using pathlib to define and expand paths
     Updated 03/2023: add basic variable typing to function inputs
-        added function for long-period equilibrium tides
-        added function for radial load pole tides
-        added function for radial ocean pole tides
-    Updated 12/2022: refactored tide read and prediction programs
-    Updated 11/2022: place some imports within try/except statements
+    Updated 12/2022: added interpolation for delta time (TT - UT1)
+        output variables for some standard epochs used within tide programs
+    Updated 11/2022: use IERS https server as default for Bulletin-A files
+        added download function for latest Bulletin-A file from IERS
+        added function to append from existing merged delta time file
         use f-strings for formatting verbose or ascii output
-    Updated 05/2022: added ESR netCDF4 formats to list of model types
-        updated keyword arguments to read tide model programs
-        added option to apply flexure to heights for applicable models
+    Updated 10/2022: added encoding for reading leap seconds ascii files
+    Updated 08/2022: output variables to unit conversion to seconds
+        and the number of days per month for both leap and standard years
+    Updated 05/2022: changed keyword arguments to camel case
     Updated 04/2022: updated docstrings to numpy documentation format
-    Updated 12/2021: added function to calculate a tidal time series
-        verify coordinate dimensions for each input data type
-        added option for converting from LORAN times to UTC
-    Updated 09/2021: refactor to use model class for files and attributes
-    Updated 07/2021: can use numpy datetime arrays as input time variable
-        added function for determining the input spatial variable type
-        added check that tide model directory is accessible
-    Updated 06/2021: added new Gr1km-v2 1km Greenland model from ESR
-        add try/except for input projection strings
-    Updated 05/2021: added option for extrapolation cutoff in kilometers
-    Updated 03/2021: added TPXO9-atlas-v4 in binary OTIS format
-        simplified netcdf inputs to be similar to binary OTIS read program
-    Updated 02/2021: replaced numpy bool to prevent deprecation warning
-    Updated 12/2020: added valid data extrapolation with nearest_extrap
-    Updated 11/2020: added model constituents from TPXO9-atlas-v3
-    Updated 08/2020: using builtin time operations.
-        calculate difference in leap seconds from start of epoch
-        using conversion protocols following pyproj-2 updates
-    Updated 07/2020: added function docstrings, FES2014 and TPXO9-atlas-v2
-        use merged delta time files combining biannual, monthly and daily files
-    Updated 03/2020: added TYPE, TIME, FILL_VALUE and METHOD options
-    Written 03/2020
+    Updated 04/2021: updated NIST ftp server url for leap-seconds.list
+    Updated 03/2021: replaced numpy bool/int to prevent deprecation warnings
+    Updated 02/2021: NASA CDDIS anonymous ftp access discontinued
+    Updated 01/2021: added ftp connection checks
+        add date parser for cases when only a calendar date with no units
+    Updated 12/2020: merged with convert_julian and convert_calendar_decimal
+        added calendar_days routine to get number of days per month
+    Updated 09/2020: added wrapper function for merging Bulletin-A files
+        can parse date strings in form "time-units since yyyy-mm-dd hh:mm:ss"
+    Updated 08/2020: added NASA Earthdata routines for downloading from CDDIS
+    Written 07/2020
 """
-from __future__ import print_function, annotations
+from __future__ import annotations
 
-import os
+import re
+import copy
+import logging
+import pathlib
 import warnings
+import datetime
+import traceback
 import numpy as np
+import dateutil.parser
 import scipy.interpolate
-import pyTMD.constants
-import pyTMD.eop
-import pyTMD.io
-import pyTMD.time
-import pyTMD.io.model
-import pyTMD.predict
-import pyTMD.spatial
 import pyTMD.utilities
 
-# attempt imports
-try:
-    import pyproj
-except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("pyproj not available", ImportWarning)
-# ignore warnings
-warnings.filterwarnings("ignore")
-
-# PURPOSE: wrapper function for computing corrections
-def compute_corrections(x, y, delta_time, CORRECTION='ocean', **kwargs):
-    """
-    Wrapper function to compute tide corrections at points and times
+# conversion factors between time units and seconds
+_to_sec = {'microseconds': 1e-6, 'microsecond': 1e-6,
+           'microsec': 1e-6, 'microsecs': 1e-6,
+           'milliseconds': 1e-3, 'millisecond': 1e-3,
+           'millisec': 1e-3, 'millisecs': 1e-3,
+           'msec': 1e-3, 'msecs': 1e-3, 'ms': 1e-3,
+           'seconds': 1.0, 'second': 1.0, 'sec': 1.0,
+           'secs': 1.0, 's': 1.0,
+           'minutes': 60.0, 'minute': 60.0,
+           'min': 60.0, 'mins': 60.0,
+           'hours': 3600.0, 'hour': 3600.0,
+           'hr': 3600.0, 'hrs': 3600.0, 'h': 3600.0,
+           'day': 86400.0, 'days': 86400.0, 'd': 86400.0}
+
+# standard epochs
+_mjd_epoch = (1858, 11, 17, 0, 0, 0)
+_ntp_epoch = (1900, 1, 1, 0, 0, 0)
+_unix_epoch = (1970, 1, 1, 0, 0, 0)
+_gps_epoch = (1980, 1, 6, 0, 0, 0)
+_tide_epoch = (1992, 1, 1, 0, 0, 0)
+_j2000_epoch = (2000, 1, 1, 12, 0, 0)
+_atlas_sdp_epoch = (2018, 1, 1, 0, 0, 0)
+
+# PURPOSE: parse a date string into epoch and units scale
+def parse_date_string(date_string: str):
+    """
+    parse a date string of the form
+
+    - time-units since ``yyyy-mm-dd hh:mm:ss``
+    - ``yyyy-mm-dd hh:mm:ss`` for exact calendar dates
 
     Parameters
     ----------
-    x: np.ndarray
-        x-coordinates in projection EPSG
-    y: np.ndarray
-        y-coordinates in projection EPSG
-    delta_time: np.ndarray
-        seconds since EPOCH or datetime array
-    CORRECTION: str, default 'ocean'
-        Correction type to compute
-
-            - ``'ocean'``: ocean tide
-            - ``'load'``: load tide
-            - ``'LPET'``: long-period equilibrium tide
-            - ``'LPT'``: solid earth load pole tide
-            - ``'OPT'``: ocean pole tide
-            - ``'SET'``: solid earth tide
-    **kwargs: dict
-        keyword arguments for correction functions
+    date_string: str
+        time-units since yyyy-mm-dd hh:mm:ss
 
     Returns
     -------
-    correction: np.ndarray
-        tidal correction at coordinates and time in meters
+    epoch: list
+        epoch of ``delta_time``
+    conversion_factor: float
+        multiplication factor to convert to seconds
+    """
+    # try parsing the original date string as a date
+    try:
+        epoch = dateutil.parser.parse(date_string)
+    except ValueError:
+        pass
+    else:
+        # return the epoch (as list)
+        return (datetime_to_list(epoch),0.0)
+    # split the date string into units and epoch
+    units,epoch = split_date_string(date_string)
+    if units not in _to_sec.keys():
+        raise ValueError(f'Invalid units: {units}')
+    # return the epoch (as list) and the time unit conversion factors
+    return (datetime_to_list(epoch), _to_sec[units])
+
+# PURPOSE: split a date string into units and epoch
+def split_date_string(date_string: str):
+    """
+    Split a date string into units and epoch
+
+    Parameters
+    ----------
+    date_string: str
+        time-units since yyyy-mm-dd hh:mm:ss
     """
-    if CORRECTION.lower() in ('ocean', 'load'):
-        return compute_tide_corrections(x, y, delta_time, **kwargs)
-    elif (CORRECTION.upper() == 'LPET'):
-        return compute_LPET_corrections(x, y, delta_time, **kwargs)
-    elif (CORRECTION.upper() == 'LPT'):
-        return compute_LPT_corrections(x, y, delta_time, **kwargs)
-    elif (CORRECTION.upper() == 'OPT'):
-        return compute_OPT_corrections(x, y, delta_time, **kwargs)
-    elif (CORRECTION.upper() == 'SET'):
-        return compute_SET_corrections(x, y, delta_time, **kwargs)
+    try:
+        units,_,epoch = date_string.split(None, 2)
+    except ValueError:
+        raise ValueError(f'Invalid format: {date_string}')
     else:
-        raise ValueError(f'Unrecognized correction type: {CORRECTION}')
+        return (units.lower(), dateutil.parser.parse(epoch))
+
+# PURPOSE: convert a datetime object into a list
+def datetime_to_list(date):
+    """
+    convert a datetime object into a list
+
+    Parameters
+    ----------
+    date: datetime object
+        Input datetime object to convert
 
-# PURPOSE: compute tides at points and times using tide model algorithms
-def compute_tide_corrections(
-        x: np.ndarray, y: np.ndarray, delta_time: np.ndarray,
-        DIRECTORY: str | None = None,
-        MODEL: str | None = None,
-        ATLAS_FORMAT: str = 'netcdf',
-        GZIP: bool = False,
-        DEFINITION_FILE: str | None = None,
-        EPSG: str | int = 3031,
-        EPOCH: list | tuple = (2000, 1, 1, 0, 0, 0),
-        TYPE: str or None = 'drift',
-        TIME: str = 'UTC',
-        METHOD: str = 'spline',
-        EXTRAPOLATE: bool = False,
-        CUTOFF: int | float=10.0,
-        APPLY_FLEXURE: bool = False,
-        FILL_VALUE: float = np.nan,
-        **kwargs
+    Returns
+    -------
+    date: list
+        [year,month,day,hour,minute,second]
+    """
+    return [date.year, date.month, date.day,
+            date.hour, date.minute, date.second]
+
+# days per month in a leap and a standard year
+# only difference is February (29 vs. 28)
+_dpm_leap = [31, 29, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
+_dpm_stnd = [31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
+
+# PURPOSE: gets the number of days per month for a given year
+def calendar_days(year: int | float | np.ndarray) -> np.ndarray:
+    """
+    Calculates the number of days per month for a given year
+
+    Parameters
+    ----------
+    year: int, float or np.ndarray
+        calendar year
+
+    Returns
+    -------
+    dpm: list
+        number of days for each month
+    """
+    # Rules in the Gregorian calendar for a year to be a leap year:
+    # divisible by 4, but not by 100 unless divisible by 400
+    # True length of the year is about 365.2422 days
+    # Adding a leap day every four years ==> average 365.25
+    # Subtracting a leap year every 100 years ==> average 365.24
+    # Adding a leap year back every 400 years ==> average 365.2425
+    # Subtracting a leap year every 4000 years ==> average 365.24225
+    m4 = (year % 4)
+    m100 = (year % 100)
+    m400 = (year % 400)
+    m4000 = (year % 4000)
+    # find indices for standard years and leap years using criteria
+    if ((m4 == 0) & (m100 != 0) | (m400 == 0) & (m4000 != 0)):
+        return np.array(_dpm_leap, dtype=np.float64)
+    elif ((m4 != 0) | (m100 == 0) & (m400 != 0) | (m4000 == 0)):
+        return np.array(_dpm_stnd, dtype=np.float64)
+
+# PURPOSE: convert a numpy datetime array to delta times since an epoch
+def convert_datetime(
+        date: float | np.ndarray,
+        epoch: str | tuple | list | np.datetime64 = _unix_epoch
     ):
     """
-    Compute tides at points and times using tidal harmonics
+    Convert a numpy datetime array to seconds since ``epoch``
+
+    Parameters
+    ----------
+    date: np.ndarray
+        numpy datetime array
+    epoch: str, tuple, list, np.ndarray, default (1970,1,1,0,0,0)
+        epoch for output ``delta_time``
+
+    Returns
+    -------
+    delta_time: float
+        seconds since epoch
+    """
+    # convert epoch to datetime variables
+    if isinstance(epoch, (tuple, list)):
+        epoch = np.datetime64(datetime.datetime(*epoch))
+    elif isinstance(epoch, str):
+        epoch = np.datetime64(dateutil.parser.parse(epoch))
+    # convert to delta time
+    return (date - epoch) / np.timedelta64(1, 's')
+
+# PURPOSE: convert times from seconds since epoch1 to time since epoch2
+def convert_delta_time(
+        delta_time: np.ndarray,
+        epoch1: str | tuple | list | np.datetime64 | None = None,
+        epoch2: str | tuple | list | np.datetime64 | None = None,
+        scale: float = 1.0
+    ):
+    """
+    Convert delta time from seconds since ``epoch1`` to time since ``epoch2``
 
     Parameters
     ----------
-    x: np.ndarray
-        x-coordinates in projection EPSG
-    y: np.ndarray
-        y-coordinates in projection EPSG
     delta_time: np.ndarray
-        seconds since EPOCH or datetime array
-    DIRECTORY: str or NoneType, default None
-        working data directory for tide models
-    MODEL: str or NoneType, default None
-        Tide model to use in correction
-    ATLAS_FORMAT: str, default 'netcdf'
-        ATLAS tide model format
-
-            - ``'OTIS'``
-            - ``'netcdf'``
-    GZIP: bool, default False
-        Tide model files are gzip compressed
-    DEFINITION_FILE: str or NoneType, default None
-        Tide model definition file for use
-    EPSG: int, default: 3031 (Polar Stereographic South, WGS84)
-        Input coordinate system
-    EPOCH: tuple, default (2000,1,1,0,0,0)
-        Time period for calculating delta times
-    TYPE: str or NoneType, default 'drift'
-        Input data type
-
-            - ``None``: determined from input variable dimensions
-            - ``'drift'``: drift buoys or satellite/airborne altimetry
-            - ``'grid'``: spatial grids or images
-            - ``'time series'``: time series at a single point
-    TIME: str, default 'UTC'
-        Time type if need to compute leap seconds to convert to UTC
-
-            - ``'GPS'``: leap seconds needed
-            - ``'LORAN'``: leap seconds needed (LORAN = GPS + 9 seconds)
-            - ``'TAI'``: leap seconds needed (TAI = GPS + 19 seconds)
-            - ``'UTC'``: no leap seconds needed
-            - ``'datetime'``: numpy datatime array in UTC
-    METHOD: str
-        Interpolation method
-
-            - ```bilinear```: quick bilinear interpolation
-            - ```spline```: scipy bivariate spline interpolation
-            - ```linear```, ```nearest```: scipy regular grid interpolations
-
-    EXTRAPOLATE: bool, default False
-        Extrapolate with nearest-neighbors
-    CUTOFF: int or float, default 10.0
-        Extrapolation cutoff in kilometers
-
-        Set to ``np.inf`` to extrapolate for all points
-    APPLY_FLEXURE: bool, default False
-        Apply ice flexure scaling factor to height constituents
-
-        Only valid for models containing flexure fields
-    FILL_VALUE: float, default np.nan
-        Output invalid value
+        seconds since epoch1
+    epoch1: tuple or NoneType, default None
+        epoch for input ``delta_time``
+    epoch2: tuple or NoneType, default None
+        epoch for output ``delta_time``
+    scale: float, default 1.0
+        scaling factor for converting time to output units
+    """
+    # convert epochs to datetime variables
+    if isinstance(epoch1, (tuple, list)):
+        epoch1 = np.datetime64(datetime.datetime(*epoch1))
+    elif isinstance(epoch1, str):
+        epoch1 = np.datetime64(dateutil.parser.parse(epoch1))
+    if isinstance(epoch2, (tuple, list)):
+        epoch2 = np.datetime64(datetime.datetime(*epoch2))
+    elif isinstance(epoch2, str):
+        epoch2 = np.datetime64(dateutil.parser.parse(epoch2))
+    # calculate the total difference in time in seconds
+    delta_time_epochs = (epoch2 - epoch1) / np.timedelta64(1, 's')
+    # subtract difference in time and rescale to output units
+    return scale*(delta_time - delta_time_epochs)
+
+# PURPOSE: calculate the delta time from calendar date
+# http://scienceworld.wolfram.com/astronomy/JulianDate.html
+def convert_calendar_dates(
+        year: np.ndarray,
+        month: np.ndarray,
+        day: np.ndarray,
+        hour: np.ndarray | float = 0.0,
+        minute: np.ndarray | float = 0.0,
+        second: np.ndarray | float = 0.0,
+        epoch: tuple | list | np.datetime64 = _tide_epoch,
+        scale: float = 1.0
+    ) -> np.ndarray:
+    """
+    Calculate the time in time units since ``epoch`` from calendar dates
+
+    Parameters
+    ----------
+    year: np.ndarray
+        calendar year
+    month: np.ndarray
+        month of the year
+    day: np.ndarray
+        day of the month
+    hour: np.ndarray or float, default 0.0
+        hour of the day
+    minute: np.ndarray or float, default 0.0
+        minute of the hour
+    second: np.ndarray or float, default 0.0
+        second of the minute
+    epoch: tuple or list, default pyTMD.time._tide_epoch
+        epoch for output ``delta_time``
+    scale: float, default 1.0
+        scaling factor for converting time to output units
 
     Returns
     -------
-    tide: np.ndarray
-        tidal elevation at coordinates and time in meters
+    delta_time: np.ndarray
+        time since epoch
+    """
+    # calculate date in Modified Julian Days (MJD) from calendar date
+    # MJD: days since November 17, 1858 (1858-11-17T00:00:00)
+    MJD = 367.0*year - np.floor(7.0*(year + np.floor((month+9.0)/12.0))/4.0) - \
+        np.floor(3.0*(np.floor((year + (month - 9.0)/7.0)/100.0) + 1.0)/4.0) + \
+        np.floor(275.0*month/9.0) + day + hour/24.0 + minute/1440.0 + \
+        second/86400.0 + 1721028.5 - 2400000.5
+    # convert epochs to datetime variables
+    epoch1 = np.datetime64(datetime.datetime(*_mjd_epoch))
+    if isinstance(epoch, (tuple, list)):
+        epoch = np.datetime64(datetime.datetime(*epoch))
+    elif isinstance(epoch, str):
+        epoch = np.datetime64(dateutil.parser.parse(epoch))
+    # calculate the total difference in time in days
+    delta_time_epochs = (epoch - epoch1) / np.timedelta64(1, 'D')
+    # return the date in units (default days) since epoch
+    return scale*np.array(MJD - delta_time_epochs, dtype=np.float64)
+
+# PURPOSE: Converts from calendar dates into decimal years
+def convert_calendar_decimal(
+        year: np.ndarray,
+        month: np.ndarray,
+        day: np.ndarray,
+        hour: np.ndarray | float | None = None,
+        minute: np.ndarray | float | None = None,
+        second: np.ndarray | float | None = None,
+        DofY: np.ndarray | float | None = None,
+    ) -> np.ndarray:
     """
+    Converts from calendar date into decimal years taking into
+    account leap years
 
-    # check that tide directory is accessible
-    try:
-        os.access(DIRECTORY, os.F_OK)
-    except:
-        raise FileNotFoundError("Invalid tide directory")
-
-    # validate input arguments
-    assert TIME in ('GPS', 'LORAN', 'TAI', 'UTC', 'datetime')
-    assert METHOD in ('bilinear', 'spline', 'linear', 'nearest')
-
-    # get parameters for tide model
-    if DEFINITION_FILE is not None:
-        model = pyTMD.io.model(DIRECTORY).from_file(DEFINITION_FILE)
+    Parameters
+    ----------
+    year: np.ndarray
+        calendar year
+    month: np.ndarray
+        calendar month
+    day: np.ndarray, float or NoneType, default None
+        day of the month
+    hour: np.ndarray, float or NoneType, default None
+        hour of the day
+    minute: np.ndarray, float or NoneType, default None
+        minute of the hour
+    second: np.ndarray, float or NoneType, default None
+        second of the minute
+    DofY: np.ndarray, float or NoneType, default None
+        day of the year
+
+    Returns
+    -------
+    t_date: np.ndarray
+        date in decimal-year format
+
+    References
+    ----------
+    .. [1] N. Dershowitz, and E. M. Reingold.
+        *Calendrical Calculations*,
+        Cambridge: Cambridge University Press, (2008).
+    """
+
+    # number of dates
+    n_dates = len(np.atleast_1d(year))
+
+    # create arrays for calendar date variables
+    cal_date = {}
+    cal_date['year'] = np.zeros((n_dates))
+    cal_date['month'] = np.zeros((n_dates))
+    cal_date['day'] = np.zeros((n_dates))
+    cal_date['hour'] = np.zeros((n_dates))
+    cal_date['minute'] = np.zeros((n_dates))
+    cal_date['second'] = np.zeros((n_dates))
+    # day of the year
+    cal_date['DofY'] = np.zeros((n_dates))
+
+    # remove singleton dimensions and use year and month
+    cal_date['year'][:] = np.squeeze(year)
+    cal_date['month'][:] = np.squeeze(month)
+
+    # create output date variable
+    t_date = np.zeros((n_dates))
+
+    # days per month in a leap and a standard year
+    # only difference is February (29 vs. 28)
+    dpm_leap = np.array(_dpm_leap, dtype=np.float64)
+    dpm_stnd = np.array(_dpm_stnd, dtype=np.float64)
+
+    # Rules in the Gregorian calendar for a year to be a leap year:
+    # divisible by 4, but not by 100 unless divisible by 400
+    # True length of the year is about 365.2422 days
+    # Adding a leap day every four years ==> average 365.25
+    # Subtracting a leap year every 100 years ==> average 365.24
+    # Adding a leap year back every 400 years ==> average 365.2425
+    # Subtracting a leap year every 4000 years ==> average 365.24225
+    m4 = (cal_date['year'] % 4)
+    m100 = (cal_date['year'] % 100)
+    m400 = (cal_date['year'] % 400)
+    m4000 = (cal_date['year'] % 4000)
+    # find indices for standard years and leap years using criteria
+    leap, = np.nonzero((m4 == 0) & (m100 != 0) | (m400 == 0) & (m4000 != 0))
+    stnd, = np.nonzero((m4 != 0) | (m100 == 0) & (m400 != 0) | (m4000 == 0))
+
+    # calculate the day of the year
+    if DofY is not None:
+        # if entered directly as an input
+        # remove 1 so day 1 (Jan 1st) = 0.0 in decimal format
+        cal_date['DofY'][:] = np.squeeze(DofY)-1
     else:
-        model = pyTMD.io.model(DIRECTORY, format=ATLAS_FORMAT,
-            compressed=GZIP).elevation(MODEL)
+        # use calendar month and day of the month to calculate day of the year
+        # month minus 1: January = 0, February = 1, etc (indice of month)
+        # in decimal form: January = 0.0
+        month_m1 = np.array(cal_date['month'],dtype=int) - 1
+
+        # day of month
+        if day is not None:
+            # remove 1 so 1st day of month = 0.0 in decimal format
+            cal_date['day'][:] = np.squeeze(day)-1.0
+        else:
+            # if not entering days as an input
+            # will use the mid-month value
+            cal_date['day'][leap] = dpm_leap[month_m1[leap]]/2.0
+            cal_date['day'][stnd] = dpm_stnd[month_m1[stnd]]/2.0
+
+        # create matrix with the lower half = 1
+        # this matrix will be used in a matrix multiplication
+        # to calculate the total number of days for prior months
+        # the -1 will make the diagonal == 0
+        # i.e. first row == all zeros and the
+        # last row == ones for all but the last element
+        mon_mat=np.tri(12,12,-1)
+        # using a dot product to calculate total number of days
+        # for the months before the input date
+        # basically is sum(i*dpm)
+        # where i is 1 for all months < the month of interest
+        # and i is 0 for all months >= the month of interest
+        # month of interest is zero as the exact days will be
+        # used to calculate the date
+
+        # calculate the day of the year for leap and standard
+        # use total days of all months before date
+        # and add number of days before date in month
+        cal_date['DofY'][stnd] = cal_date['day'][stnd] + \
+            np.dot(mon_mat[month_m1[stnd],:],dpm_stnd)
+        cal_date['DofY'][leap] = cal_date['day'][leap] + \
+            np.dot(mon_mat[month_m1[leap],:],dpm_leap)
+
+    # hour of day (else is zero)
+    if hour is not None:
+        cal_date['hour'][:] = np.squeeze(hour)
+
+    # minute of hour (else is zero)
+    if minute is not None:
+        cal_date['minute'][:] = np.squeeze(minute)
+
+    # second in minute (else is zero)
+    if second is not None:
+        cal_date['second'][:] = np.squeeze(second)
+
+    # calculate decimal date
+    # convert hours, minutes and seconds into days
+    # convert calculated fractional days into decimal fractions of the year
+    # Leap years
+    t_date[leap] = cal_date['year'][leap] + \
+        (cal_date['DofY'][leap] + cal_date['hour'][leap]/24. + \
+        cal_date['minute'][leap]/1440. + \
+        cal_date['second'][leap]/86400.)/np.sum(dpm_leap)
+    # Standard years
+    t_date[stnd] = cal_date['year'][stnd] + \
+        (cal_date['DofY'][stnd] + cal_date['hour'][stnd]/24. + \
+        cal_date['minute'][stnd]/1440. + \
+        cal_date['second'][stnd]/86400.)/np.sum(dpm_stnd)
 
-    # determine input data type based on variable dimensions
-    if not TYPE:
-        TYPE = pyTMD.spatial.data_type(x, y, delta_time)
-    # reform coordinate dimensions for input grids
-    # or verify coordinate dimension shapes
-    if (TYPE.lower() == 'grid') and (np.size(x) != np.size(y)):
-        x,y = np.meshgrid(np.copy(x),np.copy(y))
-    elif (TYPE.lower() == 'grid'):
-        x = np.atleast_2d(x)
-        y = np.atleast_2d(y)
-    elif TYPE.lower() in ('time series', 'drift'):
-        x = np.atleast_1d(x)
-        y = np.atleast_1d(y)
+    return t_date
 
-    # converting x,y from EPSG to latitude/longitude
-    try:
-        # EPSG projection code string or int
-        crs1 = pyproj.CRS.from_epsg(int(EPSG))
-    except (ValueError,pyproj.exceptions.CRSError):
-        # Projection SRS string
-        crs1 = pyproj.CRS.from_string(EPSG)
-    # output coordinate reference system
-    crs2 = pyproj.CRS.from_epsg(4326)
-    transformer = pyproj.Transformer.from_crs(crs1, crs2, always_xy=True)
-    lon,lat = transformer.transform(x.flatten(), y.flatten())
-
-    # assert delta time is an array
-    delta_time = np.atleast_1d(delta_time)
-    # calculate leap seconds if specified
-    if (TIME.upper() == 'GPS'):
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(0, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    elif (TIME.upper() == 'LORAN'):
-        # LORAN time is ahead of GPS time by 9 seconds
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(-9.0, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time-9.0, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    elif (TIME.upper() == 'TAI'):
-        # TAI time is ahead of GPS time by 19 seconds
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(-19.0, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time-19.0, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
+# PURPOSE: Converts from Julian day to calendar date and time
+def convert_julian(JD: np.ndarray, **kwargs):
+    """
+    Converts from Julian day to calendar date and time
+
+    Parameters
+    ----------
+    JD: np.ndarray
+        Julian Day (days since 01-01-4713 BCE at 12:00:00)
+    astype: str or NoneType, default None
+        convert output to variable type
+    format: str, default 'dict'
+        format of output variables
+
+            - ``'dict'``: dictionary with variable keys
+            - ``'tuple'``: tuple in most-to-least-significant order
+            - ``'zip'``: aggregated variable sets
+
+    Returns
+    -------
+    year: np.ndarray
+        calendar year
+    month: np.ndarray
+        calendar month
+    day: np.ndarray
+        day of the month
+    hour: np.ndarray
+        hour of the day
+    minute: np.ndarray
+        minute of the hour
+    second: np.ndarray
+        second of the minute
+
+    References
+    ----------
+    .. [1] W. H. Press, *Numerical Recipes in C*,
+        Brian P. Flannery, Saul A. Teukolsky, and William T. Vetterling.
+        Cambridge University Press, (1988).
+    .. [2] D. A. Hatcher, "Simple Formulae for Julian Day Numbers and
+        Calendar Dates", *Quarterly Journal of the Royal Astronomical
+        Society*, 25(1), 1984.
+    """
+    # set default keyword arguments
+    kwargs.setdefault('astype', None)
+    kwargs.setdefault('format', 'dict')
+    # raise warnings for deprecated keyword arguments
+    deprecated_keywords = dict(ASTYPE='astype', FORMAT='format')
+    for old,new in deprecated_keywords.items():
+        if old in kwargs.keys():
+            warnings.warn(f"""Deprecated keyword argument {old}.
+                Changed to '{new}'""", DeprecationWarning)
+            # set renamed argument to not break workflows
+            kwargs[new] = copy.copy(kwargs[old])
+
+    # convert to array if only a single value was imported
+    if (np.ndim(JD) == 0):
+        JD = np.atleast_1d(JD)
+        single_value = True
     else:
-        leap_seconds = 0.0
+        single_value = False
+
+    # verify julian day
+    JDO = np.floor(JD + 0.5)
+    C = np.zeros_like(JD)
+    # calculate C for dates before and after the switch to Gregorian
+    IGREG = 2299161.0
+    ind1, = np.nonzero(JDO < IGREG)
+    C[ind1] = JDO[ind1] + 1524.0
+    ind2, = np.nonzero(JDO >= IGREG)
+    B = np.floor((JDO[ind2] - 1867216.25)/36524.25)
+    C[ind2] = JDO[ind2] + B - np.floor(B/4.0) + 1525.0
+    # calculate coefficients for date conversion
+    D = np.floor((C - 122.1)/365.25)
+    E = np.floor((365.0 * D) + np.floor(D/4.0))
+    F = np.floor((C - E)/30.6001)
+    # calculate day, month, year and hour
+    day = np.floor(C - E + 0.5) - np.floor(30.6001*F)
+    month = F - 1.0 - 12.0*np.floor(F/14.0)
+    year = D - 4715.0 - np.floor((7.0 + month)/10.0)
+    hour = np.floor(24.0*(JD + 0.5 - JDO))
+    # calculate minute and second
+    G = (JD + 0.5 - JDO) - hour/24.0
+    minute = np.floor(G*1440.0)
+    second = (G - minute/1440.0) * 86400.0
+
+    # convert all variables to output type (from float)
+    if kwargs['astype'] is not None:
+        year = year.astype(kwargs['astype'])
+        month = month.astype(kwargs['astype'])
+        day = day.astype(kwargs['astype'])
+        hour = hour.astype(kwargs['astype'])
+        minute = minute.astype(kwargs['astype'])
+        second = second.astype(kwargs['astype'])
+
+    # if only a single value was imported initially: remove singleton dims
+    if single_value:
+        year = year.item(0)
+        month = month.item(0)
+        day = day.item(0)
+        hour = hour.item(0)
+        minute = minute.item(0)
+        second = second.item(0)
+
+    # return date variables in output format
+    if (kwargs['format'] == 'dict'):
+        return dict(year=year, month=month, day=day,
+            hour=hour, minute=minute, second=second)
+    elif (kwargs['format'] == 'tuple'):
+        return (year, month, day, hour, minute, second)
+    elif (kwargs['format'] == 'zip'):
+        return zip(year, month, day, hour, minute, second)
 
-    # convert delta times or datetimes objects
-    if (TIME.lower() == 'datetime'):
+# delta time (TT - UT1) file
+_delta_file = pyTMD.utilities.get_data_path(['data','merged_deltat.data'])
+
+class timescale:
+    """
+    Class for converting between time scales
+
+    Attributes
+    ----------
+    leaps: np.ndarray
+        Number of leap seconds
+    MJD: np.ndarray
+        Modified Julian Days
+    century: float
+        Days in a Julian century
+    day: float
+        Seconds in a day
+    turn: float
+        Fraction of a full turn
+    turndeg: float
+        Degrees in a full turn
+    tau: float
+        Radians in a full turn
+    deg2rad: float
+        Degrees to radians
+    deg2asec: float
+        Degrees to arcseconds
+    """
+    def __init__(self, MJD=None):
+        # leap seconds
+        self.leaps = None
+        # modified Julian Days
+        self.MJD = MJD
+        # Julian century
+        self.century = 36525.0
+        # seconds per day
+        self.day = 86400.0
+        # 360 degrees
+        self.turn = 1.0
+        self.turndeg = 360.0
+        self.tau = 2.0*np.pi
+        # degrees to radians
+        self.deg2rad = np.pi/180.0
+        # degrees to arcseconds
+        self.deg2asec = 3600.0
+        # iterator
+        self.__index__ = 0
+
+    def from_deltatime(self,
+            delta_time: np.ndarray,
+            epoch: str | tuple | list | np.ndarray,
+            standard: str = 'UTC'
+        ):
+        """
+        Converts a delta time array and into a ``timescale`` object
+
+        Parameters
+        ----------
+        delta_time: np.ndarray
+            seconds since ``epoch``
+        epoch: str, uuple, list or np.ndarray
+            epoch for input ``delta_time``
+        standard: str, default 'UTC'
+            time standard for input ``delta_time``
+        """
+        # assert delta time is an array
+        delta_time = np.atleast_1d(delta_time)
+        # calculate leap seconds if specified
+        if (standard.upper() == 'GPS'):
+            GPS_Epoch_Time = convert_delta_time(0, epoch1=epoch,
+                epoch2= _gps_epoch, scale=1.0)
+            GPS_Time = convert_delta_time(delta_time, epoch1=epoch,
+                epoch2=_gps_epoch, scale=1.0)
+            # calculate difference in leap seconds from start of epoch
+            self.leaps = count_leap_seconds(GPS_Time) - \
+                count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
+        elif (standard.upper() == 'LORAN'):
+            # LORAN time is ahead of GPS time by 9 seconds
+            GPS_Epoch_Time = convert_delta_time(-9.0, epoch1=epoch,
+                epoch2=_gps_epoch, scale=1.0)
+            GPS_Time = convert_delta_time(delta_time - 9.0, epoch1=epoch,
+                epoch2=_gps_epoch, scale=1.0)
+            # calculate difference in leap seconds from start of epoch
+            self.leaps = count_leap_seconds(GPS_Time) - \
+                count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
+        elif (standard.upper() == 'TAI'):
+            # TAI time is ahead of GPS time by 19 seconds
+            GPS_Epoch_Time = convert_delta_time(-19.0, epoch1=epoch,
+                epoch2=_gps_epoch, scale=1.0)
+            GPS_Time = convert_delta_time(delta_time-19.0, epoch1=epoch,
+                epoch2=_gps_epoch, scale=1.0)
+            # calculate difference in leap seconds from start of epoch
+            self.leaps = count_leap_seconds(GPS_Time) - \
+                count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
+        else:
+            self.leaps = 0.0
+        # convert time to days relative to Modified Julian days in UTC
+        self.MJD = convert_delta_time(delta_time - self.leaps,
+            epoch1=epoch, epoch2=_mjd_epoch, scale=(1.0/self.day))
+        return self
+
+    def from_datetime(self, dtime: np.ndarray):
+        """
+        Reads a ``datetime`` array and converts into a ``timescale`` object
+
+        Parameters
+        ----------
+        dtime: np.ndarray
+            ``numpy.datetime64`` array
+        """
         # convert delta time array from datetime object
         # to days relative to 1992-01-01T00:00:00
-        t = pyTMD.time.convert_datetime(delta_time,
-            epoch=pyTMD.time._tide_epoch)/86400.0
-    else:
-        # convert time to days relative to Jan 1, 1992 (48622mjd)
-        t = pyTMD.time.convert_delta_time(delta_time - leap_seconds,
-            epoch1=EPOCH, epoch2=pyTMD.time._tide_epoch, scale=(1.0/86400.0))
-    # delta time (TT - UT1) file
-    delta_file = pyTMD.utilities.get_data_path(['data','merged_deltat.data'])
-
-    # read tidal constants and interpolate to grid points
-    if model.format in ('OTIS','ATLAS','ESR'):
-        amp,ph,D,c = pyTMD.io.OTIS.extract_constants(lon, lat, model.grid_file,
-            model.model_file, model.projection, type=model.type,
-            method=METHOD, extrapolate=EXTRAPOLATE, cutoff=CUTOFF,
-            grid=model.format, apply_flexure=APPLY_FLEXURE)
-        # use delta time at 2000.0 to match TMD outputs
-        deltat = np.zeros_like(t)
-    elif (model.format == 'netcdf'):
-        amp,ph,D,c = pyTMD.io.ATLAS.extract_constants(lon, lat, model.grid_file,
-            model.model_file, type=model.type, method=METHOD,
-            extrapolate=EXTRAPOLATE, cutoff=CUTOFF, scale=model.scale,
-            compressed=model.compressed)
-        # use delta time at 2000.0 to match TMD outputs
-        deltat = np.zeros_like(t)
-    elif (model.format == 'GOT'):
-        amp,ph,c = pyTMD.io.GOT.extract_constants(lon, lat, model.model_file,
-            method=METHOD, extrapolate=EXTRAPOLATE, cutoff=CUTOFF,
-            scale=model.scale, compressed=model.compressed)
-        # interpolate delta times from calendar dates to tide time
-        deltat = pyTMD.time.interpolate_delta_time(delta_file, t)
-    elif (model.format == 'FES'):
-        amp,ph = pyTMD.io.FES.extract_constants(lon, lat, model.model_file,
-            type=model.type, version=model.version, method=METHOD,
-            extrapolate=EXTRAPOLATE, cutoff=CUTOFF, scale=model.scale,
-            compressed=model.compressed)
-        # available model constituents
-        c = model.constituents
-        # interpolate delta times from calendar dates to tide time
-        deltat = pyTMD.time.interpolate_delta_time(delta_file, t)
-
-    # calculate complex phase in radians for Euler's
-    cph = -1j*ph*np.pi/180.0
-    # calculate constituent oscillation
-    hc = amp*np.exp(cph)
-
-    # predict tidal elevations at time and infer minor corrections
-    if (TYPE.lower() == 'grid'):
-        ny,nx = np.shape(x); nt = len(t)
-        tide = np.ma.zeros((ny,nx,nt),fill_value=FILL_VALUE)
-        tide.mask = np.zeros((ny,nx,nt),dtype=bool)
-        for i in range(nt):
-            TIDE = pyTMD.predict.map(t[i], hc, c,
-                deltat=deltat[i], corrections=model.format)
-            MINOR = pyTMD.predict.infer_minor(t[i], hc, c,
-                deltat=deltat[i], corrections=model.format)
-            # add major and minor components and reform grid
-            tide[:,:,i] = np.reshape((TIDE+MINOR), (ny,nx))
-            tide.mask[:,:,i] = np.reshape((TIDE.mask | MINOR.mask), (ny,nx))
-    elif (TYPE.lower() == 'drift'):
-        npts = len(t)
-        tide = np.ma.zeros((npts), fill_value=FILL_VALUE)
-        tide.mask = np.any(hc.mask,axis=1)
-        tide.data[:] = pyTMD.predict.drift(t, hc, c,
-            deltat=deltat, corrections=model.format)
-        minor = pyTMD.predict.infer_minor(t, hc, c,
-            deltat=deltat, corrections=model.format)
-        tide.data[:] += minor.data[:]
-    elif (TYPE.lower() == 'time series'):
-        npts = len(t)
-        tide = np.ma.zeros((npts), fill_value=FILL_VALUE)
-        tide.mask = np.any(hc.mask,axis=1)
-        tide.data[:] = pyTMD.predict.time_series(t, hc, c,
-            deltat=deltat, corrections=model.format)
-        minor = pyTMD.predict.infer_minor(t, hc, c,
-            deltat=deltat, corrections=model.format)
-        tide.data[:] += minor.data[:]
-    # replace invalid values with fill value
-    tide.data[tide.mask] = tide.fill_value
-
-    # return the ocean or load tide correction
-    return tide
-
-# PURPOSE: compute long-period equilibrium tidal elevations
-def compute_LPET_corrections(
-        x: np.ndarray, y: np.ndarray, delta_time: np.ndarray,
-        EPSG: str | int = 3031,
-        EPOCH: list | tuple = (2000, 1, 1, 0, 0, 0),
-        TYPE: str or None = 'drift',
-        TIME: str = 'UTC',
-        **kwargs
+        self.MJD = convert_datetime(dtime, epoch=_mjd_epoch)/self.day
+        return self
+
+    def to_deltatime(self,
+            epoch: str | tuple | list | np.ndarray,
+            scale: float = 1.0
+        ):
+        """
+        Convert a ``timescale`` object to a delta time array
+
+        Parameters
+        ----------
+        epoch: str, tuple, list, or np.ndarray
+            epoch for output ``delta_time``
+        scale: float, default 1.0
+            scaling factor for converting time to output units
+
+        Returns
+        -------
+        delta_time: np.ndarray
+            time since epoch
+        """
+        # convert epochs to numpy datetime variables
+        epoch1 = np.datetime64(datetime.datetime(*_mjd_epoch))
+        if isinstance(epoch, (tuple, list)):
+            epoch = np.datetime64(datetime.datetime(*epoch))
+        elif isinstance(epoch, str):
+            epoch = np.datetime64(dateutil.parser.parse(epoch))
+        # calculate the difference in epochs in days
+        delta_time_epochs = (epoch - epoch1) / np.timedelta64(1, 'D')
+        # return the date in time (default days) since epoch
+        return scale*np.array(self.MJD - delta_time_epochs, dtype=np.float64)
+
+    def to_datetime(self):
+        """
+        Convert a ``timescale`` object to a ``datetime`` array
+
+        Returns
+        -------
+        dtime: np.ndarray
+            ``numpy.datetime64`` array
+        """
+        # convert Modified Julian Day epoch to datetime variable
+        epoch = np.datetime64(datetime.datetime(*_mjd_epoch))
+        # use nanoseconds to keep as much precision as possible
+        delta_time = np.atleast_1d(self.MJD*self.day*1e9).astype(np.int64)
+        # return the datetime array
+        return np.array([epoch + np.timedelta64(s, 'ns') for s in delta_time])
+
+    # PURPOSE: calculate the sum of a polynomial function of time
+    def polynomial_sum(self, coefficients: list | np.ndarray, t: np.ndarray):
+        """
+        Calculates the sum of a polynomial function of time
+
+        Parameters
+        ----------
+        coefficients: list or np.ndarray
+            leading coefficient of polynomials of increasing order
+        t: np.ndarray
+            delta time in units for a given astronomical longitudes calculation
+        """
+        # convert time to array if importing a single value
+        t = np.atleast_1d(t)
+        return np.sum([c * (t ** i) for i, c in enumerate(coefficients)], axis=0)
+
+    @pyTMD.utilities.reify
+    def era(self):
+        """Earth Rotation Angle (ERA) in degrees
+        """
+        # earth rotation angle using Universal Time
+        J = self.MJD - 51544.5
+        fraction = np.mod(J, self.turn)
+        theta = np.mod(0.7790572732640 + 0.00273781191135448*J, self.turn)
+        return self.turndeg*np.mod(theta + fraction, self.turn)
+
+    @pyTMD.utilities.reify
+    def gha(self):
+        """Greenwich Hour Angle (GHA) in degrees
+        """
+        return np.mod(self.gmst*self.turndeg +
+                      self.turndeg*self.T*self.century +
+                      self.turndeg/2.0, self.turndeg)
+
+    @pyTMD.utilities.reify
+    def gmst(self):
+        """Greenwich Mean Sidereal Time (GMST) in fractions of day
+        """
+        GMST = np.array([24110.54841, 8640184.812866, 9.3104e-2, -6.2e-6])
+        # convert from seconds to fractions of day
+        return np.mod(self.polynomial_sum(GMST, self.T)/self.day, self.turn)
+
+    @pyTMD.utilities.reify
+    def J2000(self):
+        """Seconds since 2000-01-01T12:00:00
+        """
+        return (self.tt - 2451545.0)*self.day
+
+    @pyTMD.utilities.reify
+    def st(self):
+        """Greenwich Mean Sidereal Time (GMST) in fractions of a day
+        from the Equinox Method
+        """
+        # sidereal time polynomial coefficients in arcseconds
+        sidereal_time = np.array([0.014506, 4612.156534, 1.3915817, -4.4e-7,
+            -2.9956e-05, -3.68e-08])
+        ST = self.polynomial_sum(sidereal_time, self.T)
+        # get earth rotation angle and convert to arcseconds
+        return np.mod(ST + self.era*self.deg2asec, self.turnasec)/self.turnasec
+
+    @pyTMD.utilities.reify
+    def tide(self):
+        """Days since 1992-01-01T00:00:00
+        """
+        return self.MJD - 48622.0
+
+    @pyTMD.utilities.reify
+    def tt(self):
+        """Dynamic Time (TT) as Julian Days
+        """
+        return self.MJD + self.tt_ut1 + 2400000.5
+
+    @pyTMD.utilities.reify
+    def tt_ut1(self):
+        """
+        Difference between universal time (UT) and dynamical time (TT)
+        """
+        # return the delta time for the input date converted to days
+        return interpolate_delta_time(_delta_file, self.tide)
+
+    @pyTMD.utilities.reify
+    def T(self):
+        """Centuries since 2000-01-01T12:00:00
+        """
+        return (self.tt - 2451545.0)/self.century
+
+    @pyTMD.utilities.reify
+    def ut1(self):
+        """Universal Time (UT) as Julian Days
+        """
+        return self.MJD + 2400000.5
+
+    @property
+    def turnasec(self):
+        """Arcseconds in a full turn
+        """
+        return self.turndeg*self.deg2asec
+
+    @property
+    def asec2rad(self):
+        """Arcseconds to radians
+        """
+        return self.deg2rad/self.deg2asec
+
+    @property
+    def masec2rad(self):
+        """Microarcseconds to radians
+        """
+        return self.asec2rad/1.0e6
+
+    @property
+    def dtype(self):
+        """Main data type of ``timescale`` object"""
+        return self.MJD.dtype
+
+    @property
+    def shape(self):
+        """Dimensions of ``timescale`` object
+        """
+        return np.shape(self.MJD)
+
+    @property
+    def ndim(self):
+        """Number of dimensions in ``timescale`` object
+        """
+        return np.ndim(self.MJD)
+
+    def __len__(self):
+        """Number of time values
+        """
+        return len(np.atleast_1d(self.MJD))
+
+    def __iter__(self):
+        """Iterate over time values
+        """
+        self.__index__ = 0
+        return self
+
+    def __next__(self):
+        """Get the next time step
+        """
+        temp = timescale()
+        try:
+            temp.MJD = np.atleast_1d(self.MJD)[self.__index__].copy()
+        except IndexError as exc:
+            raise StopIteration from exc
+        # add to index
+        self.__index__ += 1
+        return temp
+
+# PURPOSE: calculate the difference between universal time and dynamical time
+# by interpolating a delta time file to a given date
+def interpolate_delta_time(
+        delta_file: str | pathlib.Path | None,
+        idays: np.ndarray,
     ):
     """
-    Compute long-period equilibrium tidal elevations at points and times
+    Calculates the difference between universal time (UT) and
+    dynamical time (TT)
 
     Parameters
     ----------
-    x: np.ndarray
-        x-coordinates in projection EPSG
-    y: np.ndarray
-        y-coordinates in projection EPSG
-    delta_time: np.ndarray
-        seconds since EPOCH or datetime array
-    EPSG: int, default: 3031 (Polar Stereographic South, WGS84)
-        Input coordinate system
-    EPOCH: tuple, default (2000,1,1,0,0,0)
-        Time period for calculating delta times
-    TYPE: str or NoneType, default 'drift'
-        Input data type
-
-            - ``None``: determined from input variable dimensions
-            - ``'drift'``: drift buoys or satellite/airborne altimetry
-            - ``'grid'``: spatial grids or images
-            - ``'time series'``: time series at a single point
-    TIME: str, default 'UTC'
-        Time type if need to compute leap seconds to convert to UTC
-
-            - ``'GPS'``: leap seconds needed
-            - ``'LORAN'``: leap seconds needed (LORAN = GPS + 9 seconds)
-            - ``'TAI'``: leap seconds needed (TAI = GPS + 19 seconds)
-            - ``'UTC'``: no leap seconds needed
-            - ``'datetime'``: numpy datatime array in UTC
-    FILL_VALUE: float, default np.nan
-        Output invalid value
+    delta_file: str or Pathlib.Path
+        file containing the delta times
+    idays: float
+        input times to interpolate (days since 1992-01-01T00:00:00)
 
     Returns
     -------
-    tide_lpe: np.ndarray
-        long-period equilibrium tide at coordinates and time in meters
+    deltat: float
+        delta time at the input time
+
+    References
+    ----------
+    .. [1] J. Meeus, *Astronomical Algorithms*, 2nd edition, 477 pp., (1998).
+    """
+    # read delta time file
+    delta_file = pathlib.Path(delta_file).expanduser().absolute()
+    dinput = np.loadtxt(delta_file)
+    # calculate Julian days and then convert to days since 1992-01-01T00:00:00
+    days = pyTMD.time.convert_calendar_dates(
+        dinput[:,0], dinput[:,1], dinput[:,2],
+        epoch=_tide_epoch)
+    # use scipy interpolating splines to interpolate delta times
+    spl = scipy.interpolate.UnivariateSpline(days, dinput[:,3], k=1, s=0, ext=0)
+    # return the delta time for the input date converted to days
+    return spl(idays)/86400.0
+
+# PURPOSE: Count number of leap seconds that have passed for each GPS time
+def count_leap_seconds(
+        GPS_Time: np.ndarray | float,
+        truncate: bool = True
+    ):
     """
+    Counts the number of leap seconds between a given GPS time and UTC
 
-    # validate input arguments
-    assert TIME in ('GPS', 'LORAN', 'TAI', 'UTC', 'datetime')
-    # determine input data type based on variable dimensions
-    if not TYPE:
-        TYPE = pyTMD.spatial.data_type(x, y, delta_time)
-    # reform coordinate dimensions for input grids
-    # or verify coordinate dimension shapes
-    if (TYPE.lower() == 'grid') and (np.size(x) != np.size(y)):
-        x,y = np.meshgrid(np.copy(x),np.copy(y))
-    elif (TYPE.lower() == 'grid'):
-        x = np.atleast_2d(x)
-        y = np.atleast_2d(y)
-    elif TYPE.lower() in ('time series', 'drift'):
-        x = np.atleast_1d(x)
-        y = np.atleast_1d(y)
+    Parameters
+    ----------
+    GPS_Time: np.ndarray or float
+        seconds since January 6, 1980 at 00:00:00
+    truncate: bool, default True
+        Reduce list of leap seconds to positive GPS times
 
-    # converting x,y from EPSG to latitude/longitude
-    try:
-        # EPSG projection code string or int
-        crs1 = pyproj.CRS.from_epsg(int(EPSG))
-    except (ValueError,pyproj.exceptions.CRSError):
-        # Projection SRS string
-        crs1 = pyproj.CRS.from_string(EPSG)
-    # output coordinate reference system
-    crs2 = pyproj.CRS.from_epsg(4326)
-    transformer = pyproj.Transformer.from_crs(crs1, crs2, always_xy=True)
-    lon, lat = transformer.transform(x.flatten(), y.flatten())
-
-    # assert delta time is an array
-    delta_time = np.atleast_1d(delta_time)
-    # calculate leap seconds if specified
-    if (TIME.upper() == 'GPS'):
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(0, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    elif (TIME.upper() == 'LORAN'):
-        # LORAN time is ahead of GPS time by 9 seconds
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(-9.0, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time-9.0, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    elif (TIME.upper() == 'TAI'):
-        # TAI time is ahead of GPS time by 19 seconds
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(-19.0, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time-19.0, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    else:
-        leap_seconds = 0.0
+    Returns
+    -------
+    n_leaps: float
+        number of elapsed leap seconds
+    """
+    # get the valid leap seconds
+    leaps = get_leap_seconds(truncate=truncate)
+    # number of leap seconds prior to GPS_Time
+    n_leaps = np.zeros_like(GPS_Time,dtype=np.float64)
+    for i,leap in enumerate(leaps):
+        count = np.count_nonzero(GPS_Time >= leap)
+        if (count > 0):
+            indices = np.nonzero(GPS_Time >= leap)
+            n_leaps[indices] += 1.0
+    # return the number of leap seconds for converting to UTC
+    return n_leaps
 
-    if (TIME.lower() == 'datetime'):
-        # convert delta time array from datetime object
-        # to days relative to 1992-01-01T00:00:00
-        tide_time = pyTMD.time.convert_datetime(delta_time,
-            epoch=pyTMD.time._tide_epoch)/86400.0
-    else:
-        # convert time from units to days since 1992-01-01T00:00:00 (UTC)
-        tide_time = pyTMD.time.convert_delta_time(delta_time-leap_seconds,
-            epoch1=EPOCH, epoch2=pyTMD.time._tide_epoch, scale=1.0/86400.0)
-
-    # interpolate delta times from calendar dates to tide time
-    delta_file = pyTMD.utilities.get_data_path(['data','merged_deltat.data'])
-    deltat = pyTMD.time.interpolate_delta_time(delta_file, tide_time)
-    # number of time points
-    nt = len(tide_time)
-
-    # predict long-period equilibrium tides at time
-    if (TYPE == 'grid'):
-        ny,nx = np.shape(x)
-        tide_lpe = np.zeros((ny,nx,nt))
-        for i in range(nt):
-            lpet = pyTMD.predict.equilibrium_tide(tide_time[i] + deltat[i], lat)
-            tide_lpe[:,:,i] = np.reshape(lpet,(ny,nx))
-    elif (TYPE == 'drift'):
-        tide_lpe = pyTMD.predict.equilibrium_tide(tide_time + deltat, lat)
-    elif (TYPE == 'time series'):
-        nstation = len(x)
-        tide_lpe = np.zeros((nstation,nt))
-        for s in range(nstation):
-            lpet = pyTMD.predict.equilibrium_tide(tide_time + deltat, lat[s])
-            tide_lpe[s,:] = np.copy(lpet)
-
-    # return the long-period equilibrium tide corrections
-    return tide_lpe
-
-# PURPOSE: compute radial load pole tide displacements
-# following IERS Convention (2010) guidelines
-def compute_LPT_corrections(
-        x: np.ndarray, y: np.ndarray, delta_time: np.ndarray,
-        h: float | np.ndarray = 0.0,
-        EPSG: str | int = 3031,
-        EPOCH: list | tuple = (2000, 1, 1, 0, 0, 0),
-        TYPE: str or None = 'drift',
-        TIME: str = 'UTC',
-        ELLIPSOID: str = 'WGS84',
-        CONVENTION: str = '2018',
-        FILL_VALUE: float = np.nan,
-        **kwargs
-    ):
+# PURPOSE: Define GPS leap seconds
+def get_leap_seconds(truncate: bool = True):
     """
-    Compute radial load pole tide displacements at points and times
-    following IERS Convention (2010) guidelines
+    Gets a list of GPS times for when leap seconds occurred
 
     Parameters
     ----------
-    x: np.ndarray
-        x-coordinates in projection EPSG
-    y: np.ndarray
-        y-coordinates in projection EPSG
-    delta_time: np.ndarray
-        seconds since EPOCH or datetime array
-    h: float or np.ndarray, default 0.0
-        height coordinates in meters
-    EPSG: int, default: 3031 (Polar Stereographic South, WGS84)
-        Input coordinate system
-    EPOCH: tuple, default (2000,1,1,0,0,0)
-        Time period for calculating delta times
-    TYPE: str or NoneType, default 'drift'
-        Input data type
-
-            - ``None``: determined from input variable dimensions
-            - ``'drift'``: drift buoys or satellite/airborne altimetry
-            - ``'grid'``: spatial grids or images
-            - ``'time series'``: time series at a single point
-    TIME: str, default 'UTC'
-        Time type if need to compute leap seconds to convert to UTC
-
-            - ``'GPS'``: leap seconds needed
-            - ``'LORAN'``: leap seconds needed (LORAN = GPS + 9 seconds)
-            - ``'TAI'``: leap seconds needed (TAI = GPS + 19 seconds)
-            - ``'UTC'``: no leap seconds needed
-            - ``'datetime'``: numpy datatime array in UTC
-    ELLIPSOID: str, default 'WGS84'
-        Ellipsoid for calculating Earth parameters
-    CONVENTION: str, default '2018'
-        IERS Mean or Secular Pole Convention
-
-            - ``'2003'``
-            - ``'2010'``
-            - ``'2015'``
-            - ``'2018'``
-    FILL_VALUE: float, default np.nan
-        Output invalid value
+    truncate: bool, default True
+        Reduce list of leap seconds to positive GPS times
 
     Returns
     -------
-    Srad: np.ndarray
-        solid earth pole tide at coordinates and time in meters
+    GPS time: float
+        GPS seconds when leap seconds occurred
+    """
+    leap_secs = pyTMD.utilities.get_data_path(['data','leap-seconds.list'])
+    # find line with file expiration as delta time
+    with leap_secs.open(mode='r', encoding='utf8') as fid:
+        secs, = [re.findall(r'\d+',i).pop() for i in fid.read().splitlines()
+            if re.match(r'^(?=#@)',i)]
+    # check that leap seconds file is still valid
+    expiry = datetime.datetime(*_ntp_epoch) + datetime.timedelta(seconds=int(secs))
+    today = datetime.datetime.now()
+    update_leap_seconds() if (expiry < today) else None
+    # get leap seconds
+    leap_UTC,TAI_UTC = np.loadtxt(leap_secs).T
+    # TAI time is ahead of GPS by 19 seconds
+    TAI_GPS = 19.0
+    # convert leap second epochs from NTP to GPS
+    # convert from time of 2nd leap second to time of 1st leap second
+    leap_GPS = convert_delta_time(leap_UTC + TAI_UTC - TAI_GPS - 1,
+        epoch1=_ntp_epoch, epoch2=_gps_epoch)
+    # return the GPS times of leap second occurance
+    if truncate:
+        return leap_GPS[leap_GPS >= 0].astype(np.float64)
+    else:
+        return leap_GPS.astype(np.float64)
+
+# PURPOSE: connects to servers and downloads leap second files
+def update_leap_seconds(
+        timeout: int | None = 20,
+        verbose: bool = False,
+        mode: oct = 0o775
+    ):
     """
+    Connects to servers to download leap-seconds.list files from NIST servers
+
+    - https://www.nist.gov/pml/time-and-frequency-division/leap-seconds-faqs
 
-    # validate input arguments
-    assert TIME in ('GPS', 'LORAN', 'TAI', 'UTC', 'datetime')
-    assert ELLIPSOID in pyTMD._ellipsoids
-    assert CONVENTION in pyTMD.eop._conventions
-    # determine input data type based on variable dimensions
-    if not TYPE:
-        TYPE = pyTMD.spatial.data_type(x, y, delta_time)
-    # reform coordinate dimensions for input grids
-    # or verify coordinate dimension shapes
-    if (TYPE.lower() == 'grid') and (np.size(x) != np.size(y)):
-        x,y = np.meshgrid(np.copy(x),np.copy(y))
-    elif (TYPE.lower() == 'grid'):
-        x = np.atleast_2d(x)
-        y = np.atleast_2d(y)
-    elif TYPE.lower() in ('time series', 'drift'):
-        x = np.atleast_1d(x)
-        y = np.atleast_1d(y)
+    Servers and Mirrors
 
-    # converting x,y from EPSG to latitude/longitude
+    - ftp://ftp.nist.gov/pub/time/leap-seconds.list
+    - https://www.ietf.org/timezones/data/leap-seconds.list
+
+    Parameters
+    ----------
+    timeout: int or None, default 20
+        timeout in seconds for blocking operations
+    verbose: bool, default False
+        print file information about output file
+    mode: oct, default 0o775
+        permissions mode of output file
+    """
+    # local version of file
+    FILE = 'leap-seconds.list'
+    LOCAL = pyTMD.utilities.get_data_path(['data',FILE])
+    HASH = pyTMD.utilities.get_hash(LOCAL)
+
+    # try downloading from NIST ftp servers
+    HOST = ['ftp.nist.gov','pub','time',FILE]
     try:
-        # EPSG projection code string or int
-        crs1 = pyproj.CRS.from_epsg(int(EPSG))
-    except (ValueError,pyproj.exceptions.CRSError):
-        # Projection SRS string
-        crs1 = pyproj.CRS.from_string(EPSG)
-    # output coordinate reference system
-    crs2 = pyproj.CRS.from_epsg(4326)
-    transformer = pyproj.Transformer.from_crs(crs1, crs2, always_xy=True)
-    lon,lat = transformer.transform(x.flatten(), y.flatten())
-
-    # assert delta time is an array
-    delta_time = np.atleast_1d(delta_time)
-    # calculate leap seconds if specified
-    if (TIME.upper() == 'GPS'):
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(0, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    elif (TIME.upper() == 'LORAN'):
-        # LORAN time is ahead of GPS time by 9 seconds
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(-9.0, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time-9.0, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    elif (TIME.upper() == 'TAI'):
-        # TAI time is ahead of GPS time by 19 seconds
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(-19.0, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time-19.0, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
+        pyTMD.utilities.check_ftp_connection(HOST[0])
+        pyTMD.utilities.from_ftp(HOST, timeout=timeout, local=LOCAL,
+            hash=HASH, verbose=verbose, mode=mode)
+    except Exception as exc:
+        logging.debug(traceback.format_exc())
+        pass
     else:
-        leap_seconds = 0.0
+        return
 
-    if (TIME.lower() == 'datetime'):
-        # convert delta time array from datetime object
-        # to Modified Julian days (days since 1858-11-17T00:00:00)
-        MJD = pyTMD.time.convert_datetime(delta_time,
-            epoch=pyTMD.time._mjd_epoch)/86400.0
+    # try downloading from Internet Engineering Task Force (IETF) mirror
+    REMOTE = ['https://www.ietf.org','timezones','data',FILE]
+    try:
+        pyTMD.utilities.from_http(REMOTE, timeout=timeout, local=LOCAL,
+            hash=HASH, verbose=verbose, mode=mode)
+    except Exception as exc:
+        logging.debug(traceback.format_exc())
+        pass
     else:
-        # convert dates to Modified Julian days (days since 1858-11-17T00:00:00)
-        MJD = pyTMD.time.convert_delta_time(delta_time-leap_seconds,
-            epoch1=EPOCH, epoch2=pyTMD.time._mjd_epoch, scale=1.0/86400.0)
-    # add offset to convert to Julian days and then convert to calendar dates
-    Y,M,D,h,m,s = pyTMD.time.convert_julian(2400000.5 + MJD, format='tuple')
-    # calculate time in year-decimal format
-    time_decimal = pyTMD.time.convert_calendar_decimal(Y, M, day=D,
-        hour=h, minute=m, second=s)
-    # number of time points
-    nt = len(time_decimal)
-
-    # degrees and arcseconds to radians
-    dtr = np.pi/180.0
-    atr = np.pi/648000.0
-    # earth and physical parameters for ellipsoid
-    units = pyTMD.constants(ELLIPSOID)
-    # tidal love number appropriate for the load tide
-    hb2 = 0.6207
-
-    # flatten heights
-    h = np.array(h).flatten() if np.ndim(h) else h
-    # convert from geodetic latitude to geocentric latitude
-    # calculate X, Y and Z from geodetic latitude and longitude
-    X,Y,Z = pyTMD.spatial.to_cartesian(lon.flatten(), lat.flatten(), h=h,
-        a_axis=units.a_axis, flat=units.flat)
-    rr = np.sqrt(X**2.0 + Y**2.0 + Z**2.0)
-    # calculate geocentric latitude and convert to degrees
-    latitude_geocentric = np.arctan(Z / np.sqrt(X**2.0 + Y**2.0))/dtr
-    # geocentric colatitude and longitude in radians
-    theta = dtr*(90.0 - latitude_geocentric)
-    phi = dtr*lon.flatten()
-
-    # compute normal gravity at spatial location and elevation of points.
-    # Normal gravity at height h. p. 82, Eqn.(2-215)
-    gamma_h = units.gamma_h(theta, h)
-    dfactor = -hb2*atr*(units.omega**2*rr**2)/(2.0*gamma_h)
-
-    # pole tide files (mean and daily)
-    mean_pole_file = pyTMD.utilities.get_data_path(['data','mean-pole.tab'])
-    pole_tide_file = pyTMD.utilities.get_data_path(['data','finals.all'])
-    # calculate angular coordinates of mean/secular pole at time
-    mpx, mpy, fl = pyTMD.eop.iers_mean_pole(mean_pole_file, time_decimal,
-        CONVENTION)
-    # read IERS daily polar motion values
-    EOP = pyTMD.eop.iers_daily_EOP(pole_tide_file)
-    # interpolate daily polar motion values to MJD using cubic splines
-    xSPL = scipy.interpolate.UnivariateSpline(EOP['MJD'],EOP['x'],k=3,s=0)
-    ySPL = scipy.interpolate.UnivariateSpline(EOP['MJD'],EOP['y'],k=3,s=0)
-    px = xSPL(MJD)
-    py = ySPL(MJD)
-    # calculate differentials from mean/secular pole positions
-    mx = px - mpx
-    my = -(py - mpy)
-
-    # calculate radial displacement at time
-    if (TYPE == 'grid'):
-        ny,nx = np.shape(x)
-        Srad = np.ma.zeros((ny,nx,nt),fill_value=FILL_VALUE)
-        Srad.mask = np.zeros((ny,nx,nt),dtype=bool)
-        for i in range(nt):
-            SRAD = dfactor*np.sin(2.0*theta)*(mx[i]*np.cos(phi)+my[i]*np.sin(phi))
-            # reform grid
-            Srad.data[:,:,i] = np.reshape(SRAD, (ny,nx))
-            Srad.mask[:,:,i] = np.isnan(Srad.data[:,:,i])
-    elif (TYPE == 'drift'):
-        Srad = np.ma.zeros((nt),fill_value=FILL_VALUE)
-        Srad.data[:] = dfactor*np.sin(2.0*theta)*(mx*np.cos(phi)+my*np.sin(phi))
-        Srad.mask = np.isnan(Srad.data)
-    elif (TYPE == 'time series'):
-        nstation = len(x)
-        Srad = np.ma.zeros((nstation,nt),fill_value=FILL_VALUE)
-        Srad.mask = np.zeros((nstation,nt),dtype=bool)
-        for s in range(nstation):
-            SRAD = dfactor[s]*np.sin(2.0*theta[s])*(mx*np.cos(phi[s])+my*np.sin(phi[s]))
-            Srad.data[s,:] = np.copy(SRAD)
-            Srad.mask[s,:] = np.isnan(Srad.data[s,:])
-    # replace invalid data with fill values
-    Srad.data[Srad.mask] = Srad.fill_value
-
-    # return the solid earth pole tide corrections
-    return Srad
-
-# PURPOSE: compute radial load pole tide displacements
-# following IERS Convention (2010) guidelines
-def compute_OPT_corrections(
-        x: np.ndarray, y: np.ndarray, delta_time: np.ndarray,
-        h: float | np.ndarray = 0.0,
-        EPSG: str | int = 3031,
-        EPOCH: list | tuple = (2000, 1, 1, 0, 0, 0),
-        TYPE: str or None = 'drift',
-        TIME: str = 'UTC',
-        ELLIPSOID: str = 'WGS84',
-        CONVENTION: str = '2018',
-        METHOD: str = 'spline',
-        FILL_VALUE: float = np.nan,
-        **kwargs
+        return
+
+# PURPOSE: Download delta time files and merge into a single
+def merge_delta_time(
+        username: str | None = None,
+        password: str | None = None,
+        verbose: bool = False,
+        mode: oct = 0o775
     ):
     """
-    Compute radial ocean pole tide displacements at points and times
-    following IERS Convention (2010) guidelines
+    Connects to servers to download historic_deltat.data and deltat.data files
+
+    Reads IERS Bulletin-A produced iers_deltat.data files
+
+    Creates a merged file combining the historic, monthly and daily files
+
+    Long-term Delta T
+
+    - https://www.usno.navy.mil/USNO/earth-orientation/eo-products/long-term
 
     Parameters
     ----------
-    x: np.ndarray
-        x-coordinates in projection EPSG
-    y: np.ndarray
-        y-coordinates in projection EPSG
-    delta_time: np.ndarray
-        seconds since EPOCH or datetime array
-    h: float or np.ndarray, default 0.0
-        height coordinates in meters
-    EPSG: int, default: 3031 (Polar Stereographic South, WGS84)
-        Input coordinate system
-    EPOCH: tuple, default (2000,1,1,0,0,0)
-        Time period for calculating delta times
-    TYPE: str or NoneType, default 'drift'
-        Input data type
-
-            - ``None``: determined from input variable dimensions
-            - ``'drift'``: drift buoys or satellite/airborne altimetry
-            - ``'grid'``: spatial grids or images
-            - ``'time series'``: time series at a single point
-    TIME: str, default 'UTC'
-        Time type if need to compute leap seconds to convert to UTC
-
-            - ``'GPS'``: leap seconds needed
-            - ``'LORAN'``: leap seconds needed (LORAN = GPS + 9 seconds)
-            - ``'TAI'``: leap seconds needed (TAI = GPS + 19 seconds)
-            - ``'UTC'``: no leap seconds needed
-            - ``'datetime'``: numpy datatime array in UTC
-    ELLIPSOID: str, default 'WGS84'
-        Ellipsoid for calculating Earth parameters
-    CONVENTION: str, default '2018'
-        IERS Mean or Secular Pole Convention
-
-            - ``'2003'``
-            - ``'2010'``
-            - ``'2015'``
-            - ``'2018'``
-    METHOD: str
-        Interpolation method
-
-            - ```bilinear```: quick bilinear interpolation
-            - ```spline```: scipy bivariate spline interpolation
-            - ```linear```, ```nearest```: scipy regular grid interpolations
-    FILL_VALUE: float, default np.nan
-        Output invalid value
+    username: str or NoneType, default None
+        NASA Earthdata username
+    password: str or NoneType, default None
+        NASA Earthdata password
+    verbose: bool, default False
+        print file information about output file
+    mode: oct, default 0o775
+        permissions mode of output file
+
+    Notes
+    -----
+    Delta times are the difference between universal time and dynamical time
+    """
+    # retrieve history delta time files
+    pull_deltat_file('historic_deltat.data',
+        username=username, password=password,
+        verbose=verbose, mode=mode
+    )
+    # read historic delta time file
+    historic_file=pyTMD.utilities.get_data_path(['data','historic_deltat.data'])
+    historic = np.loadtxt(historic_file, skiprows=2)
+    HY = np.floor(historic[:,0])
+    HM = 12.0*np.mod(historic[:,0],1.0) + 1.0
+    HD = np.ones_like(historic[:,0])
+    # retrieve monthly delta time files
+    pull_deltat_file('deltat.data',
+        username=username, password=password,
+        verbose=verbose, mode=mode
+    )
+    # read modern monthly delta time file
+    monthly_file = pyTMD.utilities.get_data_path(['data','deltat.data'])
+    monthly = np.loadtxt(monthly_file)
+    monthly_time = convert_calendar_decimal(monthly[:,0],monthly[:,1],
+        day=monthly[:,2])
+    # retrieve daily delta time files
+    merge_bulletin_a_files(
+        username=username, password=password,
+        verbose=verbose, mode=mode
+    )
+    # read modern daily delta time file from IERS Bulletin A files
+    daily_file = pyTMD.utilities.get_data_path(['data','iers_deltat.data'])
+    daily = np.loadtxt(daily_file)
+    daily_time = convert_calendar_decimal(daily[:,0], daily[:,1],
+        day=daily[:,2])
+    # write to new merged file
+    merged_file = pyTMD.utilities.get_data_path(['data','merged_deltat.data'])
+    fid = merged_file.open(mode='w', encoding='utf8')
+    logging.info(str(merged_file))
+    file_format = ' {0:4.0f} {1:2.0f} {2:2.0f} {3:7.4f}'
+    # use historical values for times prior to monthly
+    ind1, = np.nonzero(historic[:,0] < monthly_time[0])
+    for i in ind1:
+        args = (HY[i],HM[i],HD[i],historic[i,1])
+        print(file_format.format(*args),file=fid)
+    # use monthly values for times prior to daily
+    ind2, = np.nonzero(monthly_time < np.min(daily_time))
+    for i in ind2:
+        args = (monthly[i,0],monthly[i,1],monthly[i,2],monthly[i,3])
+        print(file_format.format(*args),file=fid)
+    # use daily values for all times available
+    for i in np.argsort(daily_time):
+        args = (daily[i,0],daily[i,1],daily[i,2],daily[i,3])
+        print(file_format.format(*args),file=fid)
+    # close the merged file and change the permissions mode
+    fid.close()
+    merged_file.chmod(mode)
 
-    Returns
-    -------
-    Urad: np.ndarray
-        ocean pole tide at coordinates and time in meters
+# PURPOSE: Append Bulletin-A file to merged delta time file
+def append_delta_time(verbose: bool = False, mode: oct = 0o775):
     """
+    Appends merged delta time file with values from latest Bulletin-A file
 
-    # validate input arguments
-    assert TIME in ('GPS', 'LORAN', 'TAI', 'UTC', 'datetime')
-    assert ELLIPSOID in pyTMD._ellipsoids
-    assert CONVENTION in pyTMD.eop._conventions
-    assert METHOD in ('bilinear', 'spline', 'linear', 'nearest')
-    # determine input data type based on variable dimensions
-    if not TYPE:
-        TYPE = pyTMD.spatial.data_type(x, y, delta_time)
-    # reform coordinate dimensions for input grids
-    # or verify coordinate dimension shapes
-    if (TYPE.lower() == 'grid') and (np.size(x) != np.size(y)):
-        x,y = np.meshgrid(np.copy(x),np.copy(y))
-    elif (TYPE.lower() == 'grid'):
-        x = np.atleast_2d(x)
-        y = np.atleast_2d(y)
-    elif TYPE.lower() in ('time series', 'drift'):
-        x = np.atleast_1d(x)
-        y = np.atleast_1d(y)
+    Parameters
+    ----------
+    verbose: bool, default False
+        print file information about output file
+    mode: oct, default 0o775
+        permissions mode of output file
+
+    Notes
+    -----
+    Delta times are the difference between universal time and dynamical time
+    """
+
+    # append to merged file
+    merged_file = pyTMD.utilities.get_data_path(['data','merged_deltat.data'])
+    fid = merged_file.open(mode='a', encoding='utf8')
+    logging.info(str(merged_file))
+    file_format = ' {0:4.0f} {1:2.0f} {2:2.0f} {3:7.4f}'
+    # read latest Bulletin-A file from IERS
+    bulletin_file = pyTMD.utilities.get_data_path(['data','ser7.dat'])
+    logging.info(str(bulletin_file))
+    with bulletin_file.open(mode='rb') as fileID:
+        YY,MM,DD,DELTAT = read_iers_bulletin_a(fileID)
+    # append latest delta time values to merged file
+    for Y,M,D,T in zip(YY,MM,DD,DELTAT):
+        print(file_format.format(Y,M,D,T), file=fid)
+    # close the merged file and change the permissions mode
+    fid.close()
+    merged_file.chmod(mode)
+
+# PURPOSE: connect to IERS or CDDIS server and merge Bulletin-A files
+def merge_bulletin_a_files(
+        username: str | None = None,
+        password: str | None = None,
+        verbose: bool = False,
+        mode: oct = 0o775
+    ):
+    """
+    Attempt to connects to the IERS server and the CDDIS Earthdata server
+    to download and merge Bulletin-A files
+
+    Reads the IERS Bulletin-A files and calculates the daily delta times
+
+    Servers and Mirrors
 
-    # converting x,y from EPSG to latitude/longitude
+    - https://datacenter.iers.org/availableVersions.php?id=6
+    - ftp://ftp.iers.org/products/eop/rapid/bulletina/
+    - https://cddis.nasa.gov/archive/products/iers/iers_bulletins/bulletin_a/
+
+    Parameters
+    ----------
+    username: str or NoneType, default None
+        NASA Earthdata username
+    password: str or NoneType, default None
+        NASA Earthdata password
+    verbose: bool, default False
+        print file information about output file
+    mode: oct, default 0o775
+        permissions mode of output file
+
+    Notes
+    -----
+    Delta times are the difference between universal time and dynamical time
+    """
+    # if complete: replace previous version of file
+    LOCAL = pyTMD.utilities.get_data_path(['data','iers_deltat.data'])
+    COPY = pyTMD.utilities.get_data_path(['data','iers_deltat.temp'])
+    # try connecting to IERS http servers and merge Bulletin-A files
     try:
-        # EPSG projection code string or int
-        crs1 = pyproj.CRS.from_epsg(int(EPSG))
-    except (ValueError,pyproj.exceptions.CRSError):
-        # Projection SRS string
-        crs1 = pyproj.CRS.from_string(EPSG)
-    # output coordinate reference system
-    crs2 = pyproj.CRS.from_epsg(4326)
-    transformer = pyproj.Transformer.from_crs(crs1, crs2, always_xy=True)
-    lon,lat = transformer.transform(x.flatten(), y.flatten())
-
-    # assert delta time is an array
-    delta_time = np.atleast_1d(delta_time)
-    # calculate leap seconds if specified
-    if (TIME.upper() == 'GPS'):
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(0, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    elif (TIME.upper() == 'LORAN'):
-        # LORAN time is ahead of GPS time by 9 seconds
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(-9.0, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time-9.0, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    elif (TIME.upper() == 'TAI'):
-        # TAI time is ahead of GPS time by 19 seconds
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(-19.0, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time-19.0, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
+        iers_delta_time(COPY, verbose=verbose, mode=mode)
+    except Exception as exc:
+        logging.debug(traceback.format_exc())
+        COPY.unlink() if COPY.exists() else None
+        pass
     else:
-        leap_seconds = 0.0
+        pyTMD.utilities.copy(COPY, LOCAL, move=True)
+        return
 
-    if (TIME.lower() == 'datetime'):
-        # convert delta time array from datetime object
-        # to Modified Julian days (days since 1858-11-17T00:00:00)
-        MJD = pyTMD.time.convert_datetime(delta_time,
-            epoch=pyTMD.time._mjd_epoch)/86400.0
+    # try connecting to IERS ftp servers and merge Bulletin-A files
+    try:
+        iers_ftp_delta_time(COPY, verbose=verbose, mode=mode)
+    except Exception as exc:
+        logging.debug(traceback.format_exc())
+        COPY.unlink() if COPY.exists() else None
+        pass
     else:
-        # convert dates to Modified Julian days (days since 1858-11-17T00:00:00)
-        MJD = pyTMD.time.convert_delta_time(delta_time-leap_seconds,
-            epoch1=EPOCH, epoch2=pyTMD.time._mjd_epoch, scale=1.0/86400.0)
-    # add offset to convert to Julian days and then convert to calendar dates
-    Y,M,D,h,m,s = pyTMD.time.convert_julian(2400000.5 + MJD, format='tuple')
-    # calculate time in year-decimal format
-    time_decimal = pyTMD.time.convert_calendar_decimal(Y, M, day=D,
-        hour=h, minute=m, second=s)
-    # number of time points
-    nt = len(time_decimal)
-
-    # degrees and arcseconds to radians
-    dtr = np.pi/180.0
-    atr = np.pi/648000.0
-    # earth and physical parameters for ellipsoid
-    units = pyTMD.constants(ELLIPSOID)
-    # mean equatorial gravitational acceleration [m/s^2]
-    ge = 9.7803278
-    # density of sea water [kg/m^3]
-    rho_w = 1025.0
-    # tidal love number differential (1 + kl - hl) for pole tide frequencies
-    gamma = 0.6870 + 0.0036j
-
-    # flatten heights
-    h = np.array(h).flatten() if np.ndim(h) else h
-    # convert from geodetic latitude to geocentric latitude
-    # calculate X, Y and Z from geodetic latitude and longitude
-    X,Y,Z = pyTMD.spatial.to_cartesian(lon.flatten(), lat.flatten(), h=h,
-        a_axis=units.a_axis, flat=units.flat)
-    rr = np.sqrt(X**2.0 + Y**2.0 + Z**2.0)
-    # calculate geocentric latitude and convert to degrees
-    latitude_geocentric = np.arctan(Z / np.sqrt(X**2.0 + Y**2.0))/dtr
-
-    # pole tide displacement scale factor
-    Hp = np.sqrt(8.0*np.pi/15.0)*(units.omega**2*units.a_axis**4)/units.GM
-    K = 4.0*np.pi*units.G*rho_w*Hp*units.a_axis/(3.0*ge)
-    K1 = 4.0*np.pi*units.G*rho_w*Hp*units.a_axis**3/(3.0*units.GM)
-
-    # pole tide files (mean and daily)
-    mean_pole_file = pyTMD.utilities.get_data_path(['data','mean-pole.tab'])
-    pole_tide_file = pyTMD.utilities.get_data_path(['data','finals.all'])
-    # calculate angular coordinates of mean/secular pole at time
-    mpx, mpy, fl = pyTMD.eop.iers_mean_pole(mean_pole_file, time_decimal,
-        CONVENTION)
-    # read IERS daily polar motion values
-    EOP = pyTMD.eop.iers_daily_EOP(pole_tide_file)
-    # interpolate daily polar motion values to MJD using cubic splines
-    xSPL = scipy.interpolate.UnivariateSpline(EOP['MJD'],EOP['x'],k=3,s=0)
-    ySPL = scipy.interpolate.UnivariateSpline(EOP['MJD'],EOP['y'],k=3,s=0)
-    px = xSPL(MJD)
-    py = ySPL(MJD)
-    # calculate differentials from mean/secular pole positions
-    mx = px - mpx
-    my = -(py - mpy)
-
-    # read ocean pole tide map from Desai (2002)
-    ocean_pole_tide_file = pyTMD.utilities.get_data_path(['data',
-        'opoleloadcoefcmcor.txt.gz'])
-    iur,iun,iue,ilon,ilat = pyTMD.io.ocean_pole_tide(ocean_pole_tide_file)
-    # interpolate ocean pole tide map from Desai (2002)
-    if (METHOD == 'spline'):
-        # use scipy bivariate splines to interpolate to output points
-        f1 = scipy.interpolate.RectBivariateSpline(ilon, ilat[::-1],
-            iur[:,::-1].real, kx=1, ky=1)
-        f2 = scipy.interpolate.RectBivariateSpline(ilon, ilat[::-1],
-            iur[:,::-1].imag, kx=1, ky=1)
-        UR = np.zeros((len(latitude_geocentric)), dtype=np.longcomplex)
-        UR.real = f1.ev(lon.flatten(), latitude_geocentric)
-        UR.imag = f2.ev(lon.flatten(), latitude_geocentric)
+        pyTMD.utilities.copy(COPY, LOCAL, move=True)
+        return
+
+    # try connecting to CDDIS https servers and merge Bulletin-A files
+    try:
+        cddis_delta_time(COPY, username=username, password=password,
+            verbose=verbose, mode=mode)
+    except Exception as exc:
+        logging.debug(traceback.format_exc())
+        COPY.unlink() if COPY.exists() else None
+        pass
     else:
-        # use scipy regular grid to interpolate values for a given method
-        r1 = scipy.interpolate.RegularGridInterpolator((ilon,ilat[::-1]),
-            iur[:,::-1], method=METHOD)
-        UR = r1.__call__(np.c_[lon.flatten(), latitude_geocentric])
-
-    # calculate radial displacement at time
-    if (TYPE == 'grid'):
-        ny,nx = np.shape(x)
-        Urad = np.ma.zeros((ny,nx,nt),fill_value=FILL_VALUE)
-        Urad.mask = np.zeros((ny,nx,nt),dtype=bool)
-        for i in range(nt):
-            URAD = K*atr*np.real((mx[i]*gamma.real + my[i]*gamma.imag)*UR.real +
-                (my[i]*gamma.real - mx[i]*gamma.imag)*UR.imag)
-            # reform grid
-            Urad.data[:,:,i] = np.reshape(URAD, (ny,nx))
-            Urad.mask[:,:,i] = np.isnan(Urad.data[:,:,i])
-    elif (TYPE == 'drift'):
-        Urad = np.ma.zeros((nt),fill_value=FILL_VALUE)
-        Urad.data[:] = K*atr*np.real((mx*gamma.real + my*gamma.imag)*UR.real +
-            (my*gamma.real - mx*gamma.imag)*UR.imag)
-        Urad.mask = np.isnan(Urad.data)
-    elif (TYPE == 'time series'):
-        nstation = len(x)
-        Urad = np.ma.zeros((nstation,nt),fill_value=FILL_VALUE)
-        Urad.mask = np.zeros((nstation,nt),dtype=bool)
-        for s in range(nstation):
-            URAD = K*atr*np.real((mx*gamma.real + my*gamma.imag)*UR.real[s] +
-                (my*gamma.real - mx*gamma.imag)*UR.imag[s])
-            Urad.data[s,:] = np.copy(URAD)
-            Urad.mask[s,:] = np.isnan(Urad.data[s,:])
-    # replace invalid data with fill values
-    Urad.data[Urad.mask] = Urad.fill_value
-
-    # return the ocean pole tide corrections
-    return Urad
-
-# PURPOSE: compute solid earth tidal elevations
-def compute_SET_corrections(
-        x: np.ndarray, y: np.ndarray, delta_time: np.ndarray,
-        h: float | np.ndarray = 0.0,
-        EPSG: str | int = 3031,
-        EPOCH: list | tuple = (2000, 1, 1, 0, 0, 0),
-        TYPE: str or None = 'drift',
-        TIME: str = 'UTC',
-        ELLIPSOID: str = 'WGS84',
-        TIDE_SYSTEM='tide_free',
-        **kwargs
+        pyTMD.utilities.copy(COPY, LOCAL, move=True)
+        return
+
+# PURPOSE: connects to IERS ftp servers and finds Bulletin-A files
+def iers_ftp_delta_time(
+        daily_file: str | pathlib.Path,
+        timeout: int | None = 120,
+        verbose: bool = False,
+        mode: oct = 0o775
     ):
     """
-    Compute solid earth tidal elevations at points and times
-    following IERS Convention (2010) guidelines
+    Connects to the IERS ftp server to download Bulletin-A files
+
+    - https://datacenter.iers.org/productMetadata.php?id=6
+
+    Reads the IERS Bulletin-A files and calculates the daily delta times
+
+    Servers and Mirrors
+
+    - ftp://ftp.iers.org/products/eop/rapid/bulletina/
 
     Parameters
     ----------
-    x: np.ndarray
-        x-coordinates in projection EPSG
-    y: np.ndarray
-        y-coordinates in projection EPSG
-    delta_time: np.ndarray
-        seconds since EPOCH or datetime array
-    h: float or np.ndarray, default 0.0
-        height coordinates in meters
-    EPSG: int, default: 3031 (Polar Stereographic South, WGS84)
-        Input coordinate system
-    EPOCH: tuple, default (2000,1,1,0,0,0)
-        Time period for calculating delta times
-    TYPE: str or NoneType, default 'drift'
-        Input data type
-
-            - ``None``: determined from input variable dimensions
-            - ``'drift'``: drift buoys or satellite/airborne altimetry
-            - ``'grid'``: spatial grids or images
-            - ``'time series'``: time series at a single point
-    TIME: str, default 'UTC'
-        Time type if need to compute leap seconds to convert to UTC
-
-            - ``'GPS'``: leap seconds needed
-            - ``'LORAN'``: leap seconds needed (LORAN = GPS + 9 seconds)
-            - ``'TAI'``: leap seconds needed (TAI = GPS + 19 seconds)
-            - ``'UTC'``: no leap seconds needed
-            - ``'datetime'``: numpy datatime array in UTC
-    ELLIPSOID: str, default 'WGS84'
-        Ellipsoid for calculating Earth parameters
-    TIDE_SYSTEM: str, default 'tide_free'
-        Permanent tide system for the output solid Earth tide
+    daily_file: str or pathlib.Path
+        output daily delta time file from merged Bulletin-A files
+    timeout: int, default 120
+        timeout in seconds for blocking operations
+    verbose: bool, default False
+        print file information about output file
+    mode: oct, default 0o775
+        permissions mode of output file
+
+    Notes
+    -----
+    Delta times are the difference between universal time and dynamical time
+    """
+    # connect to ftp host for IERS bulletins
+    HOST = ['ftp.iers.org','products','eop','rapid','bulletina']
+    pyTMD.utilities.check_ftp_connection(HOST[0])
+    # regular expression pattern for finding files
+    rx = re.compile(r'bulletina-(.*?)-(\d+).txt$',re.VERBOSE)
+    # open output daily delta time file
+    daily_file = pathlib.Path(daily_file).expanduser().absolute()
+    fid = daily_file.open(mode='w', encoding='utf8')
+    # output file format
+    file_format = ' {0:4.0f} {1:2.0f} {2:2.0f} {3:7.4f}'
+    # find subdirectories
+    subdirectory,_ = pyTMD.utilities.ftp_list(HOST,timeout=timeout,
+        basename=True,sort=True)
+    # for each subdirectory
+    for SUB in subdirectory:
+        # find Bulletin-A files in ftp subdirectory
+        HOST.append(SUB)
+        logging.info(SUB)
+        bulletin_files,_ = pyTMD.utilities.ftp_list(HOST,
+            timeout=timeout,basename=True,sort=True,pattern=rx)
+        # for each Bulletin-A file
+        for f in sorted(bulletin_files):
+            logging.info(f)
+            # copy remote file contents to BytesIO object
+            HOST.append(f)
+            remote_buffer = pyTMD.utilities.from_ftp(HOST,timeout=timeout)
+            # read Bulletin-A file from BytesIO object
+            YY,MM,DD,DELTAT = read_iers_bulletin_a(remote_buffer)
+            # print delta time for week to output file
+            for Y,M,D,T in zip(YY,MM,DD,DELTAT):
+                print(file_format.format(Y,M,D,T),file=fid)
+            # close the bytesIO object
+            remote_buffer.close()
+            # remove the file from the list
+            HOST.remove(f)
+        # remove the subdirectory from the list
+        HOST.remove(SUB)
+    # close the output file
+    fid.close()
+    # change the permissions mode
+    daily_file.chmod(mode)
+
+# PURPOSE: connects to IERS http servers and finds Bulletin-A files
+def iers_delta_time(
+        daily_file: str | pathlib.Path,
+        timeout: int | None = 120,
+        verbose: bool = False,
+        mode: oct = 0o775
+    ):
+    """
+    Connects to the IERS server to download Bulletin-A files
 
-            - ``'tide_free'``: no permanent direct and indirect tidal potentials
-            - ``'mean_tide'``: permanent tidal potentials (direct and indirect)
+    - https://datacenter.iers.org/productMetadata.php?id=6
+
+    Reads the IERS Bulletin-A files and calculates the daily delta times
+
+    Servers and Mirrors
+
+    - https://datacenter.iers.org/availableVersions.php?id=6
+
+    Parameters
+    ----------
+    daily_file: str or pathlib.Path
+        output daily delta time file from merged Bulletin-A files
+    timeout: int, default 120
+        timeout in seconds for blocking operations
+    verbose: bool, default False
+        print file information about output file
+    mode: oct, default 0o775
+        permissions mode of output file
+
+    Notes
+    -----
+    Delta times are the difference between universal time and dynamical time
+    """
+    # open output daily delta time file
+    daily_file = pathlib.Path(daily_file).expanduser().absolute()
+    fid = daily_file.open(mode='w', encoding='utf8')
+    # output file format
+    file_format = ' {0:4.0f} {1:2.0f} {2:2.0f} {3:7.4f}'
+    # connect to http host for IERS Bulletin-A files
+    HOST = 'https://datacenter.iers.org/availableVersions.php?id=6'
+    bulletin_files,_ = pyTMD.utilities.iers_list(HOST, timeout=timeout)
+    # for each Bulletin-A file
+    for f in bulletin_files:
+        logging.info(f)
+        remote_buffer = pyTMD.utilities.from_http(f, timeout=timeout)
+        # read Bulletin-A file from BytesIO object
+        YY,MM,DD,DELTAT = read_iers_bulletin_a(remote_buffer)
+        # print delta time for week to output file
+        for Y,M,D,T in zip(YY,MM,DD,DELTAT):
+            print(file_format.format(Y,M,D,T), file=fid)
+        # close the bytesIO object
+        remote_buffer.close()
+    # close the output file
+    fid.close()
+    # change the permissions mode
+    daily_file.chmod(mode)
+
+# PURPOSE: connects to CDDIS Earthdata https server and finds Bulletin-A files
+def cddis_delta_time(
+        daily_file: str | pathlib.Path,
+        username: str | None = None,
+        password: str | None = None,
+        verbose: bool = False,
+        mode: oct = 0o775
+    ):
+    """
+    Connects to the CDDIS Earthdata server to download Bulletin-A files
+
+    Reads the IERS Bulletin-A files and calculates the daily delta times
+
+    Servers and Mirrors
+
+    - https://cddis.nasa.gov/archive/products/iers/iers_bulletins/bulletin_a/
+
+    Parameters
+    ----------
+    daily_file: str
+        output daily delta time file from merged Bulletin-A files
+    username: str or NoneType, default None
+        NASA Earthdata username
+    password: str or NoneType, default None
+        NASA Earthdata password
+    verbose: bool, default False
+        print file information about output file
+    mode: oct, default 0o775
+        permissions mode of output file
+
+    Notes
+    -----
+    Delta times are the difference between universal time and dynamical time
+    """
+    # connect to CDDIS Earthdata host for IERS bulletins
+    HOST = ['https://cddis.nasa.gov','archive','products','iers',
+        'iers_bulletins','bulletin_a']
+    # build NASA Earthdata opener for CDDIS and check credentials
+    pyTMD.utilities.build_opener(username, password)
+    pyTMD.utilities.check_credentials()
+    # regular expression pattern for finding directories
+    R1 = re.compile(r'volume_(.*?)$',re.VERBOSE)
+    # regular expression pattern for finding files
+    R2 = re.compile(r'iers_bulletina\.(.*?)_(\d+)$',re.VERBOSE)
+    # open output daily delta time file
+    daily_file = pathlib.Path(daily_file).expanduser().absolute()
+    fid = daily_file.open(mode='w', encoding='utf8')
+    file_format = ' {0:4.0f} {1:2.0f} {2:2.0f} {3:7.4f}'
+    # for each subdirectory
+    subdirectory, mtimes = pyTMD.utilities.cddis_list(
+        HOST, build=False, pattern=R1)
+    # extract roman numerals from subdirectories
+    roman = [R1.findall(s).pop() for s in subdirectory]
+    # sort the list of Roman numerals
+    subdirectory = [subdirectory[i] for i,j in sorted(enumerate(roman),
+        key=lambda i: pyTMD.utilities.roman_to_int(i[1]))]
+    # output file format
+    for SUB in subdirectory:
+        # find Bulletin-A files in https subdirectory
+        HOST.append(SUB)
+        bulletin_files, mtimes = pyTMD.utilities.cddis_list(
+            HOST, build=False, sort=True, pattern=R2)
+        # for each Bulletin-A file
+        for f in sorted(bulletin_files):
+            logging.info(f)
+            # copy remote file contents to BytesIO object
+            HOST.append(f)
+            remote_buffer = pyTMD.utilities.from_cddis(HOST,
+                build=False,timeout=20)
+            # read Bulletin-A file from BytesIO object
+            YY,MM,DD,DELTAT = read_iers_bulletin_a(remote_buffer)
+            # print delta time for week to output file
+            for Y,M,D,T in zip(YY,MM,DD,DELTAT):
+                print(file_format.format(Y,M,D,T),file=fid)
+            # close the bytesIO object
+            remote_buffer.close()
+            # remove the file from the list
+            HOST.remove(f)
+        # remove the subdirectory from the list
+        HOST.remove(SUB)
+    # close the output file
+    fid.close()
+    # change the permissions mode
+    daily_file.chmod(mode)
+
+# PURPOSE: reads IERS Bulletin-A and calculates the delta times
+def read_iers_bulletin_a(fileID):
+    """
+    Read a weekly IERS Bulletin-A file and calculate the
+    delta times (TT - UT1)
+
+    Parameters
+    ----------
+    fileID: obj
+        open file object for Bulletin-A file
 
     Returns
     -------
-    tide_se: np.ndarray
-        solid earth tide at coordinates and time in meters
+    Y: float,
+        calendar year
+    M: float
+        calendar month
+    D: float
+        day of the month
+    DELTAT: float
+        difference between universal time and dynamical time
+
+    Notes
+    -----
+    Delta times are the difference between universal time and dynamical time
+    """
+    # read contents from input file object
+    file_contents = fileID.read().decode('utf8').splitlines()
+
+    # parse header text to find time offsets
+    # TT-TAI
+    TT_TAI = 0
+    # TAI-UTC
+    TAI_UTC = 0
+    # counts the number of lines in the header
+    count = 0
+    HEADER = False
+    # Reading over header text
+    while not HEADER:
+        # file line at count
+        l = file_contents[count]
+        # check if line contains time offsets
+        if re.search(r'TT\s\=\sTAI',l):
+            TT_TAI = np.float64(re.findall(r'(\d+\.\d+)',l).pop())
+        if re.search(r'TAI-UTC',l):
+            TAI_UTC = np.float64(re.findall(r'=\s(\d+\.\d+)',l).pop())
+        # find line to set HEADER flag to True
+        HEADER = bool(re.search(r'COMBINED\sEARTH\sORIENTATION\sPARAMETERS:',l))
+        # add 1 to counter
+        count += 1
+
+    # convert variables to numpy arrays
+    MJD = np.zeros((7))
+    UT1_UTC = np.zeros((7))
+    valid = 0
+    # for each day in the week
+    for i in range(7):
+        try:
+            # split numerical instances from data line
+            line_contents = file_contents[count+i+4].split()
+            # years are not always complete in the bulletin file
+            # Modified Julian Day (days since 1858-11-17T00:00:00)
+            MJD[i] = np.float64(line_contents[3])
+            # difference between UT1 and UTC times
+            UT1_UTC[i] = np.float64(line_contents[8])
+        except (IndexError,ValueError):
+            pass
+        else:
+            valid += 1
+
+    # calculate components for delta time
+    # TAI time is ahead of GPS by 19 seconds
+    TAI_GPS = 19.0
+    # calculate calendar dates from Modified Julian days
+    Y,M,D,h,m,s = convert_julian(MJD[:valid]+2400000.5, format='tuple')
+    # calculate GPS Time (seconds since 1980-01-06T00:00:00)
+    # by converting the Modified Julian days (days since 1858-11-17T00:00:00)
+    GPS_Time = convert_delta_time(MJD[:valid]*8.64e4, epoch1=_mjd_epoch,
+        epoch2=_gps_epoch, scale=1.0) + TAI_UTC - TAI_GPS
+    # number of leap seconds between GPS and UTC
+    # this finds the daily correction for weeks with leap seconds
+    GPS_UTC = count_leap_seconds(GPS_Time)
+    # calculate delta time (TT - UT1) -->
+    # (TT-TAI) + (TAI-GPS) + (GPS-UTC) - (UT1-UTC)
+    DELTAT = TT_TAI + TAI_GPS + GPS_UTC - UT1_UTC[:valid]
+
+    # return dates and delta times
+    return (Y,M,D,DELTAT)
+
+# PURPOSE: connects to servers and downloads latest Bulletin-A file
+def update_bulletin_a(
+        timeout: int | None = 20,
+        verbose: bool = False,
+        mode: oct = 0o775
+    ):
     """
+    Connects to IERS Rapid Service/Prediction Center (RS/PC) and
+    downloads latest Bulletin-A file
+
+    - https://maia.usno.navy.mil/ser7/readme.bulla
+
+    Servers and Mirrors
 
-    # validate input arguments
-    assert TIME in ('GPS', 'LORAN', 'TAI', 'UTC', 'datetime')
-    assert TIDE_SYSTEM in ('mean_tide', 'tide_free')
-    # determine input data type based on variable dimensions
-    if not TYPE:
-        TYPE = pyTMD.spatial.data_type(x, y, delta_time)
-    # reform coordinate dimensions for input grids
-    # or verify coordinate dimension shapes
-    if (TYPE.lower() == 'grid') and (np.size(x) != np.size(y)):
-        x,y = np.meshgrid(np.copy(x),np.copy(y))
-    elif (TYPE.lower() == 'grid'):
-        x = np.atleast_2d(x)
-        y = np.atleast_2d(y)
-    elif TYPE.lower() in ('time series', 'drift'):
-        x = np.atleast_1d(x)
-        y = np.atleast_1d(y)
+    - https://maia.usno.navy.mil/ser7/ser7.dat
+
+    Parameters
+    ----------
+    timeout: int or NoneType, default 20
+        timeout in seconds for blocking operations
+    verbose: bool, default False
+        print file information about output file
+    mode: oct, default 0o775
+        permissions mode of output file
+    """
+    # local version of file
+    LOCAL = pyTMD.utilities.get_data_path(['data','ser7.dat'])
+    HASH = pyTMD.utilities.get_hash(LOCAL)
 
-    # converting x,y from EPSG to latitude/longitude
+    # try downloading from IERS Rapid Service/Prediction Center (RS/PC)
+    REMOTE = ['https://maia.usno.navy.mil','ser7','ser7.dat']
     try:
-        # EPSG projection code string or int
-        crs1 = pyproj.CRS.from_epsg(int(EPSG))
-    except (ValueError,pyproj.exceptions.CRSError):
-        # Projection SRS string
-        crs1 = pyproj.CRS.from_string(EPSG)
-    # output coordinate reference system
-    crs2 = pyproj.CRS.from_epsg(4326)
-    transformer = pyproj.Transformer.from_crs(crs1, crs2, always_xy=True)
-    lon, lat = transformer.transform(x.flatten(), y.flatten())
-
-    # assert delta time is an array
-    delta_time = np.atleast_1d(delta_time)
-    # calculate leap seconds if specified
-    if (TIME.upper() == 'GPS'):
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(0, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    elif (TIME.upper() == 'LORAN'):
-        # LORAN time is ahead of GPS time by 9 seconds
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(-9.0, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time-9.0, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    elif (TIME.upper() == 'TAI'):
-        # TAI time is ahead of GPS time by 19 seconds
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(-19.0, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time-19.0, epoch1=EPOCH,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
+        pyTMD.utilities.from_http(REMOTE, timeout=timeout, local=LOCAL,
+            hash=HASH, verbose=verbose, mode=mode)
+    except Exception as exc:
+        logging.debug(traceback.format_exc())
+        pass
     else:
-        leap_seconds = 0.0
+        return
 
-    if (TIME.lower() == 'datetime'):
-        # convert delta time array from datetime object
-        # to days relative to 1992-01-01T00:00:00
-        tide_time = pyTMD.time.convert_datetime(delta_time,
-            epoch=pyTMD.time._tide_epoch)/86400.0
+# PURPOSE: connects to servers and downloads delta time files
+def pull_deltat_file(
+        FILE: str,
+        username: str | None = None,
+        password: str | None = None,
+        timeout: int | None = 20,
+        verbose: bool = False,
+        mode: oct = 0o775
+    ):
+    """
+    Connects to servers and downloads delta time files
+
+    Servers and Mirrors
+
+    - http://maia.usno.navy.mil/ser7/
+    - https://cddis.nasa.gov/archive/products/iers/
+    - ftp://cddis.nasa.gov/products/iers/
+    - ftp://cddis.gsfc.nasa.gov/pub/products/iers/
+
+    Parameters
+    ----------
+    FILE: str
+        delta time file to download from remote servers
+
+            - deltat.data: monthly deltat file
+            - historic_deltat.data: historic deltat file
+    username: str or NoneType, default None
+        NASA Earthdata username
+    password: str or NoneType, default None
+        NASA Earthdata password
+    timeout: int or NoneType, default 20
+        timeout in seconds for blocking operations
+    verbose: bool, default False
+        print file information about output file
+    mode: oct, default 0o775
+        permissions mode of output file
+
+    Notes
+    -----
+    Delta times are the difference between universal time and dynamical time
+    """
+    # local version of file
+    LOCAL = pyTMD.utilities.get_data_path(['data',FILE])
+    HASH = pyTMD.utilities.get_hash(LOCAL)
+
+    # try downloading from US Naval Oceanography Portal
+    HOST = ['http://maia.usno.navy.mil','ser7',FILE]
+    try:
+        pyTMD.utilities.from_http(HOST,
+            timeout=timeout,
+            local=LOCAL,
+            hash=HASH,
+            verbose=verbose,
+            mode=mode)
+    except Exception as exc:
+        logging.debug(traceback.format_exc())
+        pass
+    else:
+        return
+
+    # try downloading from NASA Crustal Dynamics Data Information System
+    # NOTE: anonymous ftp access was discontinued on 2020-10-31
+    # requires using the following https Earthdata server
+    server = []
+    # server.append(['cddis.nasa.gov','pub','products','iers',FILE])
+    # server.append(['cddis.gsfc.nasa.gov','products','iers',FILE])
+    for HOST in server:
+        try:
+            pyTMD.utilities.check_ftp_connection(HOST[0])
+            pyTMD.utilities.from_ftp(HOST,
+                timeout=timeout,
+                local=LOCAL,
+                hash=HASH,
+                verbose=verbose,
+                mode=mode)
+        except Exception as exc:
+            logging.debug(traceback.format_exc())
+            pass
+        else:
+            return
+
+    # try downloading from NASA Crustal Dynamics Data Information System
+    # using NASA Earthdata credentials stored in netrc file
+    HOST = ['https://cddis.nasa.gov','archive','products','iers',FILE]
+    try:
+        pyTMD.utilities.from_cddis(HOST,
+            username=username,
+            password=password,
+            timeout=timeout,
+            local=LOCAL,
+            hash=HASH,
+            verbose=verbose,
+            mode=mode)
+    except Exception as exc:
+        logging.debug(traceback.format_exc())
+        pass
     else:
-        # convert time from units to days since 1992-01-01T00:00:00 (UTC)
-        tide_time = pyTMD.time.convert_delta_time(delta_time-leap_seconds,
-            epoch1=EPOCH, epoch2=pyTMD.time._tide_epoch, scale=1.0/86400.0)
-
-    # interpolate delta times from calendar dates to tide time
-    delta_file = pyTMD.utilities.get_data_path(['data','merged_deltat.data'])
-    deltat = pyTMD.time.interpolate_delta_time(delta_file, tide_time)
-    # number of time points
-    nt = len(tide_time)
-
-    # earth and physical parameters for ellipsoid
-    units = pyTMD.constants(ELLIPSOID)
-
-    # convert input coordinates to cartesian
-    X, Y, Z = pyTMD.spatial.to_cartesian(lon, lat, h=h,
-        a_axis=units.a_axis, flat=units.flat)
-    # convert time to Modified Julian Days (MJD) for ephemerides
-    MJD = tide_time + deltat + 48622.0
-    # get low-resolution solar and lunar ephemerides
-    SX, SY, SZ = pyTMD.astro.solar_ecef(MJD)
-    LX, LY, LZ = pyTMD.astro.lunar_ecef(MJD)
-
-    # calculate radial displacement at time
-    if (TYPE == 'grid'):
-        ny,nx = np.shape(x)
-        tide_se = np.zeros((ny,nx,nt))
-        # convert coordinates to column arrays
-        XYZ = np.c_[X, Y, Z]
-        for i in range(nt):
-            # reshape time to match spatial
-            t = tide_time[i] + deltat[i] + np.ones((ny*nx))
-            # convert coordinates to column arrays
-            SXYZ = np.repeat(np.c_[SX[i], SY[i], SZ[i]], ny*nx, axis=0)
-            LXYZ = np.repeat(np.c_[LX[i], LY[i], LZ[i]], ny*nx, axis=0)
-            # predict solid earth tides (cartesian)
-            dxi = pyTMD.predict.solid_earth_tide(t,
-                XYZ, SXYZ, LXYZ, a_axis=units.a_axis,
-                tide_system=TIDE_SYSTEM)
-            # calculate radial component of solid earth tides
-            dln,dlt,drad = pyTMD.spatial.to_geodetic(
-                X + dxi[:,0], Y + dxi[:,1], Z + dxi[:,2],
-                a_axis=units.a_axis, flat=units.flat)
-            # remove effects of original topography
-            # (if added when computing cartesian coordinates)
-            tide_se[:,:,i] = np.reshape(drad - h, (ny,nx))
-    elif (TYPE == 'drift'):
-        # convert coordinates to column arrays
-        XYZ = np.c_[X, Y, Z]
-        SXYZ = np.c_[SX, SY, SZ]
-        LXYZ = np.c_[LX, LY, LZ]
-        # predict solid earth tides (cartesian)
-        dxi = pyTMD.predict.solid_earth_tide(tide_time + deltat,
-            XYZ, SXYZ, LXYZ, a_axis=units.a_axis,
-            tide_system=TIDE_SYSTEM)
-        # calculate radial component of solid earth tides
-        dln,dlt,drad = pyTMD.spatial.to_geodetic(
-            X + dxi[:,0], Y + dxi[:,1], Z + dxi[:,2],
-            a_axis=units.a_axis, flat=units.flat)
-        # remove effects of original topography
-        # (if added when computing cartesian coordinates)
-        tide_se = drad - h
-    elif (TYPE == 'time series'):
-        nstation = len(x)
-        tide_se = np.zeros((nstation,nt))
-        # convert coordinates to column arrays
-        SXYZ = np.c_[SX, SY, SZ]
-        LXYZ = np.c_[LX, LY, LZ]
-        for s in range(nstation):
-            # convert coordinates to column arrays
-            XYZ = np.repeat(np.c_[X[s], Y[s], Z[s]], nt, axis=0)
-            # predict solid earth tides (cartesian)
-            dxi = pyTMD.predict.solid_earth_tide(tide_time + deltat,
-                XYZ, SXYZ, LXYZ, a_axis=units.a_axis,
-                tide_system=TIDE_SYSTEM)
-            # calculate radial component of solid earth tides
-            dln,dlt,drad = pyTMD.spatial.to_geodetic(
-                X + dxi[:,0], Y + dxi[:,1], Z + dxi[:,2],
-                a_axis=units.a_axis, flat=units.flat)
-            # remove effects of original topography
-            # (if added when computing cartesian coordinates)
-            tide_se[s,:] = drad - h
+        return
 
-    # return the solid earth tide corrections
-    return tide_se
```

### Comparing `pyTMD-2.0.3/pyTMD/constants.py` & `pyTMD-2.0.4/pyTMD/constants.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.3/pyTMD/convert_crs.py` & `pyTMD-2.0.4/pyTMD/convert_crs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python
 u"""
 convert_crs.py
 Written by Tyler Sutterley (03/2023)
 Converts points to and from Coordinates Reference Systems (CRS)
 
 CALLING SEQUENCE:
-    x,y = convert_crs(lon,lat,PROJ,'F')
-    lon,lat = convert_crs(x,y,PROJ,'B')
+    x, y = convert_crs(lon, lat, PROJ, 'F')
+    lon, lat = convert_crs(x, y, PROJ, 'B')
 
 INPUTS:
     i1: longitude ('F') or projection easting x ('B')
     i2: latitude ('F') or projection northing y ('B')
     PROJ: spatial reference system code for coordinate transformations
     BF: backwards ('B') or forward ('F') translations
 
@@ -128,22 +128,22 @@
     ----------
     PROJECTION: int or str
         Coordinate Reference System code
     """
     # EPSG projection code
     try:
         crs = pyproj.CRS.from_epsg(int(PROJECTION))
-    except (ValueError,pyproj.exceptions.CRSError):
+    except (ValueError, pyproj.exceptions.CRSError):
         pass
     else:
         return crs
     # coordinate reference system string
     try:
         crs = pyproj.CRS.from_string(PROJECTION)
-    except (ValueError,pyproj.exceptions.CRSError):
+    except (ValueError, pyproj.exceptions.CRSError):
         pass
     else:
         return crs
     # no projection can be made
     raise pyproj.exceptions.CRSError
 
 # wrapper function for models in EPSG 3031 (Antarctic Polar Stereographic)
@@ -364,27 +364,27 @@
     # projections for converting to and from input EPSG
     crs1 = crs_from_input(EPSG)
     crs2 = pyproj.CRS.from_epsg(4326)
     transformer = pyproj.Transformer.from_crs(crs1, crs2, always_xy=True)
     # convert lat/lon to (idealized) Polar-Stereographic x/y
     if (BF.upper() == 'F'):
         direction = pyproj.enums.TransformDirection.FORWARD
-        lon,lat = transformer.transform(i1, i2, direction=direction)
+        lon, lat = transformer.transform(i1, i2, direction=direction)
         o1 = (90.0-lat)*111.7*np.cos(lon/180.0*np.pi)
         o2 = (90.0-lat)*111.7*np.sin(lon/180.0*np.pi)
     # convert (idealized) Polar-Stereographic x/y to lat/lon
     elif (BF.upper() == 'B'):
         direction = pyproj.enums.TransformDirection.INVERSE
-        lon = np.arctan2(i2,i1)*180.0/np.pi
+        lon = np.arctan2(i2, i1)*180.0/np.pi
         lat = 90.0 - np.sqrt(i1**2+i2**2)/111.7
         ii, = np.nonzero(lon < 0)
         lon[ii] += 360.0
-        o1,o2 = transformer.transform(lon, lat, direction=direction)
+        o1, o2 = transformer.transform(lon, lat, direction=direction)
     # return the output variables
-    return (o1,o2)
+    return (o1, o2)
 
 # wrapper function to pass lat/lon values or convert if EPSG
 def _EPSG4326(
         i1: np.ndarray,
         i2: np.ndarray,
         BF: str,
         EPSG: int | str = 4326
```

### Comparing `pyTMD-2.0.3/pyTMD/convert_ll_xy.py` & `pyTMD-2.0.4/pyTMD/convert_ll_xy.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.3/pyTMD/data/deltat.data` & `pyTMD-2.0.4/pyTMD/data/deltat.data`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.3/pyTMD/data/finals.all` & `pyTMD-2.0.4/pyTMD/data/finals.all`

 * *Files 0% similar despite different names*

```diff
@@ -17963,796 +17963,796 @@
 22 3 8 59646.00 I  0.030999 0.000016  0.386703 0.000011  I-0.1036821 0.0000034 -0.1627 0.0024  I  -108.843    0.446    -7.322    0.060  0.031018  0.386712 -0.1036844  -108.826    -7.354  
 22 3 9 59647.00 I  0.032216 0.000019  0.388513 0.000016  I-0.1034078 0.0000028 -0.3902 0.0022  I  -108.861    0.640    -7.427    0.047  0.032281  0.388541 -0.1034089  -108.866    -7.460  
 22 310 59648.00 I  0.033082 0.000019  0.390308 0.000016  I-0.1029230 0.0000027 -0.5539 0.0020  I  -108.353    0.785    -7.426    0.029  0.033104  0.390312 -0.1029383  -108.612    -7.475  
 22 311 59649.00 I  0.033672 0.000020  0.392121 0.000016  I-0.1023276 0.0000028 -0.6347 0.0022  I  -108.004    0.785    -7.446    0.029  0.033708  0.392105 -0.1023346  -108.109    -7.473  
 22 312 59650.00 I  0.034135 0.000018  0.393692 0.000015  I-0.1016713 0.0000035 -0.6624 0.0026  I  -107.521    0.785    -7.560    0.029  0.034130  0.393729 -0.1016864  -107.569    -7.581  
 22 313 59651.00 I  0.034427 0.000025  0.395170 0.000020  I-0.1010163 0.0000044 -0.6498 0.0028  I  -107.088    0.707    -7.795    0.042  0.034502  0.395152 -0.1010372  -107.117    -7.813  
 22 314 59652.00 I  0.034370 0.000025  0.396639 0.000019  I-0.1003898 0.0000043 -0.5831 0.0038  I  -106.859    0.707    -8.049    0.042  0.034354  0.396685 -0.1004104  -106.877    -8.063  
-22 315 59653.00 I  0.034234 0.000023  0.398079 0.000015  I-0.0998758 0.0000061 -0.4393 0.0032  I  -106.851    0.600    -8.190    0.052  0.034250  0.398014 -0.0998830  -106.865    -8.198  
-22 316 59654.00 I  0.033955 0.000033  0.399537 0.000017  I-0.0995328 0.0000048 -0.2306 0.0039  I  -106.943    0.617    -8.165    0.103  0.033972  0.399563 -0.0995467  -106.918    -8.181  
-22 317 59655.00 I  0.033459 0.000033  0.401249 0.000017  I-0.0994310 0.0000047  0.0273 0.0035  I  -106.996    0.617    -8.034    0.103  0.033426  0.401244 -0.0994339  -106.930    -8.064  
-22 318 59656.00 I  0.033076 0.000031  0.402918 0.000017  I-0.0995526 0.0000051  0.1808 0.0034  I  -106.975    0.617    -7.902    0.103  0.033046  0.402931 -0.0995428  -106.876    -7.950  
-22 319 59657.00 I  0.032925 0.000027  0.404429 0.000011  I-0.0997804 0.0000048  0.2976 0.0035  I  -106.979    0.659    -7.847    0.165  0.032894  0.404430 -0.0998242  -106.884    -7.889  
-22 320 59658.00 I  0.033031 0.000027  0.405970 0.000011  I-0.1001533 0.0000047  0.4307 0.0032  I  -107.136    0.659    -7.886    0.165  0.033017  0.405997 -0.1001905  -107.059    -7.919  
-22 321 59659.00 I  0.033373 0.000033  0.407434 0.000014  I-0.1005689 0.0000043  0.3449 0.0036  I  -107.465    0.572    -7.977    0.111  0.033291  0.407432 -0.1005194  -107.409    -8.005  
-22 322 59660.00 I  0.034272 0.000023  0.408886 0.000011  I-0.1007884 0.0000054  0.0948 0.0031  I  -107.842    0.534    -8.059    0.071  0.034163  0.408866 -0.1007374  -107.806    -8.084  
-22 323 59661.00 I  0.035752 0.000024  0.410767 0.000016  I-0.1007727 0.0000045 -0.1128 0.0035  I  -108.082    0.499    -8.100    0.073  0.035739  0.410677 -0.1007668  -108.069    -8.122  
-22 324 59662.00 I  0.037151 0.000025  0.412868 0.000016  I-0.1005690 0.0000044 -0.3019 0.0031  I  -108.059    0.499    -8.123    0.073  0.037184  0.412921 -0.1005632  -108.121    -8.146  
-22 325 59663.00 I  0.038266 0.000024  0.415015 0.000016  I-0.1001862 0.0000042 -0.4391 0.0031  I  -107.763    0.499    -8.166    0.073  0.038276  0.415002 -0.1001852  -107.917    -8.187  
-22 326 59664.00 I  0.039265 0.000024  0.416908 0.000016  I-0.0997291 0.0000044 -0.4614 0.0032  I  -107.292    0.499    -8.238    0.073  0.039275  0.416959 -0.0997325  -107.413    -8.263  
-22 327 59665.00 I  0.040351 0.000019  0.418580 0.000015  I-0.0993023 0.0000047 -0.3669 0.0032  I  -106.803    0.533    -8.319    0.081  0.040293  0.418593 -0.0993188  -106.847    -8.345  
-22 328 59666.00 I  0.041640 0.000019  0.420162 0.000016  I-0.0990358 0.0000047 -0.1510 0.0038  I  -106.442    0.533    -8.383    0.081  0.041691  0.420175 -0.0990554  -106.412    -8.410  
-22 329 59667.00 I  0.042745 0.000018  0.421729 0.000012  I-0.0989806 0.0000059  0.0057 0.0033  I  -106.291    0.625    -8.422    0.085  0.042792  0.421696 -0.0989777  -106.189    -8.449  
-22 330 59668.00 I  0.043409 0.000021  0.423077 0.000019  I-0.0990310 0.0000047  0.1139 0.0039  I  -106.328    0.619    -8.428    0.096  0.043491  0.423055 -0.0990426  -106.244    -8.453  
-22 331 59669.00 I  0.043548 0.000022  0.424808 0.000019  I-0.0992196 0.0000050  0.2557 0.0035  I  -106.443    0.619    -8.390    0.096  0.043570  0.424794 -0.0992346  -106.398    -8.414  
-22 4 1 59670.00 I  0.043351 0.000023  0.426970 0.000020  I-0.0995107 0.0000051  0.3023 0.0038  I  -106.516    0.619    -8.316    0.096  0.043301  0.426919 -0.0995031  -106.506    -8.343  
-22 4 2 59671.00 I  0.043555 0.000018  0.428883 0.000018  I-0.0997950 0.0000058  0.2613 0.0041  I  -106.521    0.617    -8.257    0.101  0.043471  0.428898 -0.0997958  -106.536    -8.278  
-22 4 3 59672.00 I  0.044381 0.000021  0.431006 0.000020  I-0.1000069 0.0000064  0.1413 0.0043  I  -106.546    0.606    -8.280    0.077  0.044401  0.430964 -0.1000185  -106.583    -8.291  
-22 4 4 59673.00 I  0.045130 0.000020  0.433541 0.000020  I-0.1000660 0.0000063 -0.0133 0.0052  I  -106.670    0.606    -8.393    0.077  0.045179  0.433548 -0.1000877  -106.727    -8.395  
-22 4 5 59674.00 I  0.045606 0.000016  0.436188 0.000014  I-0.0999593 0.0000081 -0.2308 0.0049  I  -106.846    0.592    -8.523    0.031  0.045558  0.436184 -0.0999601  -106.928    -8.515  
-22 4 6 59675.00 I  0.046388 0.000019  0.438251 0.000020  I-0.0996011 0.0000075 -0.4581 0.0055  I  -106.936    0.628    -8.593    0.040  0.046324  0.438296 -0.0996161  -107.011    -8.588  
-22 4 7 59676.00 I  0.047706 0.000019  0.440056 0.000020  I-0.0990861 0.0000074 -0.5565 0.0053  I  -106.835    0.628    -8.610    0.040  0.047660  0.440084 -0.0991087  -106.904    -8.610  
-22 4 8 59677.00 I  0.049433 0.000018  0.441873 0.000020  I-0.0985111 0.0000074 -0.5858 0.0053  I  -106.535    0.628    -8.669    0.040  0.049412  0.441800 -0.0985116  -106.602    -8.670  
-22 4 9 59678.00 I  0.051231 0.000015  0.443553 0.000017  I-0.0979307 0.0000077 -0.5666 0.0050  I  -106.076    0.659    -8.845    0.046  0.051279  0.443588 -0.0979207  -106.131    -8.844  
-22 410 59679.00 I  0.052565 0.000016  0.445332 0.000019  I-0.0973866 0.0000066 -0.5212 0.0051  I  -105.537    0.793    -9.111    0.054  0.052631  0.445310 -0.0973816  -105.574    -9.106  
-22 411 59680.00 I  0.053446 0.000015  0.447041 0.000018  I-0.0969113 0.0000066 -0.4066 0.0041  I  -105.077    0.793    -9.359    0.054  0.053447  0.447037 -0.0969159  -105.095    -9.347  
-22 412 59681.00 I  0.054290 0.000013  0.449061 0.000018  I-0.0965831 0.0000048 -0.2628 0.0041  I  -104.899    0.832    -9.512    0.125  0.054284  0.449011 -0.0965845  -104.884    -9.491  
-22 413 59682.00 I  0.055326 0.000012  0.451022 0.000017  I-0.0964189 0.0000047 -0.0194 0.0035  I  -105.058    0.832    -9.557    0.125  0.055292  0.451073 -0.0964523  -105.062    -9.565  
-22 414 59683.00 I  0.056532 0.000013  0.452940 0.000017  I-0.0965550 0.0000050  0.2563 0.0034  I  -105.350    0.832    -9.494    0.125  0.056547  0.452892 -0.0965557  -105.379    -9.547  
-22 415 59684.00 I  0.057880 0.000015  0.454442 0.000018  I-0.0968981 0.0000049  0.4320 0.0032  I  -105.519    0.832    -9.312    0.125  0.057823  0.454485 -0.0968994  -105.550    -9.362  
-22 416 59685.00 I  0.059423 0.000018  0.456177 0.000016  I-0.0974024 0.0000040  0.5580 0.0033  I  -105.579    0.796    -9.059    0.167  0.059424  0.456172 -0.0974129  -105.603    -9.095  
-22 417 59686.00 I  0.061284 0.000019  0.457789 0.000016  I-0.0979718 0.0000043  0.5573 0.0043  I  -105.786    0.796    -8.879    0.167  0.061164  0.457851 -0.0979865  -105.807    -8.908  
-22 418 59687.00 I  0.063722 0.000021  0.459299 0.000016  I-0.0984747 0.0000077  0.4299 0.0045  I  -106.253    0.724    -8.900    0.008  0.063734  0.459266 -0.0985020  -106.274    -8.922  
-22 419 59688.00 I  0.066170 0.000022  0.460804 0.000016  I-0.0988063 0.0000080  0.2268 0.0046  I  -106.739    0.724    -9.095    0.008  0.066192  0.460869 -0.0988272  -106.773    -9.104  
-22 420 59689.00 I  0.068332 0.000025  0.462063 0.000024  I-0.0988957 0.0000051 -0.0742 0.0048  I  -106.903    0.795    -9.308    0.093  0.068329  0.461999 -0.0988949  -106.960    -9.291  
-22 421 59690.00 I  0.070493 0.000024  0.463008 0.000024  I-0.0986776 0.0000052 -0.3163 0.0038  I  -106.654    0.795    -9.426    0.093  0.070468  0.463064 -0.0987060  -106.695    -9.434  
-22 422 59691.00 I  0.072756 0.000021  0.464181 0.000024  I-0.0983201 0.0000055 -0.3874 0.0038  I  -106.197    0.795    -9.466    0.093  0.072707  0.464098 -0.0983386  -106.211    -9.508  
-22 423 59692.00 I  0.075223 0.000020  0.465050 0.000024  I-0.0979197 0.0000055 -0.4077 0.0041  I  -105.774    0.795    -9.494    0.093  0.075204  0.465058 -0.0979051  -105.797    -9.527  
-22 424 59693.00 I  0.077856 0.000017  0.466301 0.000036  I-0.0975340 0.0000060 -0.3402 0.0040  I  -105.461    0.842    -9.540    0.119  0.077859  0.466247 -0.0975194  -105.498    -9.555  
-22 425 59694.00 I  0.080486 0.000016  0.467889 0.000036  I-0.0972694 0.0000059 -0.1825 0.0059  I  -105.224    0.842    -9.588    0.119  0.080557  0.467896 -0.0972632  -105.265    -9.590  
-22 426 59695.00 I  0.082816 0.000010  0.469963 0.000031  I-0.0971736 0.0000101 -0.0109 0.0041  I  -105.067    0.779    -9.602    0.091  0.082859  0.469891 -0.0971847  -105.109    -9.593  
-22 427 59696.00 I  0.084841 0.000017  0.471409 0.000033  I-0.0972287 0.0000057  0.1039 0.0058  I  -105.061    0.809    -9.544    0.149  0.084908  0.471486 -0.0972203  -105.096    -9.548  
-22 428 59697.00 I  0.086493 0.000018  0.472748 0.000033  I-0.0973564 0.0000055  0.1437 0.0042  I  -105.231    0.809    -9.381    0.149  0.086518  0.472819 -0.0973522  -105.258    -9.407  
-22 429 59698.00 I  0.087930 0.000018  0.473584 0.000033  I-0.0974930 0.0000062  0.1143 0.0038  I  -105.466    0.809    -9.148    0.149  0.087895  0.473595 -0.0974914  -105.480    -9.203  
-22 430 59699.00 I  0.089676 0.000018  0.474053 0.000015  I-0.0975660 0.0000052  0.0279 0.0040  I  -105.611    0.840    -8.964    0.195  0.089653  0.474104 -0.0975559  -105.614    -9.011  
-22 5 1 59700.00 I  0.091699 0.000019  0.474622 0.000016  I-0.0975397 0.0000052 -0.0857 0.0037  I  -105.636    0.840    -8.955    0.195  0.091728  0.474632 -0.0975257  -105.627    -8.987  
-22 5 2 59701.00 I  0.093635 0.000023  0.475325 0.000020  I-0.0973966 0.0000054 -0.1934 0.0042  I  -105.635    0.789    -9.133    0.114  0.093634  0.475311 -0.0974187  -105.619    -9.154  
-22 5 3 59702.00 I  0.095564 0.000018  0.476094 0.000017  I-0.0971754 0.0000067 -0.2337 0.0043  I  -105.680    0.775    -9.361    0.031  0.095563  0.476140 -0.0972185  -105.662    -9.372  
-22 5 4 59703.00 I  0.097692 0.000024  0.476997 0.000026  I-0.0969100 0.0000066 -0.3318 0.0047  I  -105.740    0.803    -9.494    0.034  0.097691  0.476906 -0.0969126  -105.734    -9.493  
-22 5 5 59704.00 I  0.099821 0.000024  0.477829 0.000027  I-0.0965002 0.0000065 -0.4648 0.0047  I  -105.760    0.803    -9.532    0.034  0.099882  0.477903 -0.0964992  -105.770    -9.526  
-22 5 6 59705.00 I  0.101673 0.000024  0.478907 0.000026  I-0.0960205 0.0000066 -0.4776 0.0046  I  -105.730    0.803    -9.600    0.034  0.101687  0.478833 -0.0960256  -105.754    -9.581  
-22 5 7 59706.00 I  0.103385 0.000025  0.479460 0.000025  I-0.0955613 0.0000066 -0.4416 0.0046  I  -105.611    0.803    -9.787    0.034  0.103404  0.479538 -0.0955546  -105.646    -9.779  
-22 5 8 59707.00 I  0.105107 0.000024  0.480078 0.000027  I-0.0951513 0.0000064 -0.3637 0.0046  I  -105.317    0.823   -10.025    0.110  0.105117  0.480078 -0.0951550  -105.347   -10.030  
-22 5 9 59708.00 I  0.106696 0.000025  0.480494 0.000027  I-0.0948670 0.0000065 -0.1866 0.0045  I  -104.887    0.823   -10.186    0.110  0.106699  0.480537 -0.0949242  -104.904   -10.197  
-22 510 59709.00 I  0.108517 0.000019  0.481036 0.000018  I-0.0948000 0.0000062  0.0561 0.0040  I  -104.601    0.786   -10.242    0.154  0.108427  0.480933 -0.0948334  -104.607   -10.261  
-22 511 59710.00 I  0.110914 0.000019  0.481745 0.000028  I-0.0949934 0.0000046  0.3415 0.0039  I  -104.724    0.784   -10.269    0.175  0.110941  0.481776 -0.0950144  -104.732   -10.281  
-22 512 59711.00 I  0.113495 0.000018  0.482656 0.000028  I-0.0954568 0.0000047  0.5482 0.0035  I  -105.149    0.784   -10.278    0.175  0.113474  0.482707 -0.0954543  -105.174   -10.290  
-22 513 59712.00 I  0.116067 0.000018  0.483460 0.000028  I-0.0960590 0.0000052  0.6624 0.0038  I  -105.514    0.784   -10.142    0.175  0.116107  0.483379 -0.0960629  -105.566   -10.162  
-22 514 59713.00 I  0.118510 0.000014  0.483903 0.000023  I-0.0967479 0.0000060  0.6753 0.0039  I  -105.714    0.783    -9.781    0.191  0.118527  0.483975 -0.0967431  -105.773    -9.799  
-22 515 59714.00 I  0.120715 0.000021  0.484487 0.000032  I-0.0973706 0.0000059  0.5710 0.0043  I  -106.022    0.853    -9.383    0.166  0.120799  0.484444 -0.0973670  -106.086    -9.399  
-22 516 59715.00 I  0.122299 0.000022  0.485261 0.000032  I-0.0978725 0.0000061  0.4144 0.0054  I  -106.587    0.853    -9.262    0.166  0.122385  0.485333 -0.0978659  -106.653    -9.281  
-22 517 59716.00 I  0.123264 0.000022  0.485918 0.000024  I-0.0981789 0.0000091  0.1963 0.0055  I  -107.086    0.963    -9.493    0.130  0.123240  0.485912 -0.0981728  -107.146    -9.513  
-22 518 59717.00 I  0.124656 0.000028  0.485620 0.000037  I-0.0982664 0.0000091 -0.0180 0.0065  I  -107.099    0.997    -9.832    0.133  0.124614  0.485666 -0.0982338  -107.148    -9.846  
-22 519 59718.00 I  0.126492 0.000027  0.485532 0.000037  I-0.0981548 0.0000092 -0.1965 0.0065  I  -106.634    0.997   -10.029    0.133  0.126492  0.485563 -0.0980742  -106.655   -10.034  
-22 520 59719.00 I  0.128441 0.000027  0.485687 0.000037  I-0.0979230 0.0000093 -0.2261 0.0070  I  -106.083    0.997   -10.073    0.133  0.128370  0.485536 -0.0979421  -106.062   -10.068  
-22 521 59720.00 I  0.130661 0.000022  0.485982 0.000031  I-0.0977430 0.0000105 -0.1346 0.0062  I  -105.784    1.070   -10.077    0.139  0.130677  0.486020 -0.0977739  -105.765   -10.071  
-22 522 59721.00 I  0.132973 0.000024  0.486767 0.000038  I-0.0976719 0.0000081  0.0111 0.0066  I  -105.760    0.848   -10.064    0.091  0.132949  0.486774 -0.0977075  -105.758   -10.059  
-22 523 59722.00 I  0.135353 0.000025  0.487341 0.000038  I-0.0977663 0.0000079  0.1602 0.0055  I  -105.829    0.848    -9.980    0.091  0.135359  0.487350 -0.0977582  -105.848    -9.982  
-22 524 59723.00 I  0.137675 0.000018  0.488221 0.000025  I-0.0979707 0.0000075  0.2447 0.0054  I  -105.844    0.782    -9.818    0.064  0.137703  0.488205 -0.0979698  -105.891    -9.829  
-22 525 59724.00 I  0.139651 0.000020  0.488506 0.000034  I-0.0982390 0.0000075  0.2792 0.0053  I  -105.827    0.831    -9.611    0.068  0.139642  0.488593 -0.0982642  -105.852    -9.614  
-22 526 59725.00 I  0.141660 0.000019  0.488483 0.000034  I-0.0984964 0.0000075  0.2155 0.0053  I  -105.917    0.831    -9.372    0.068  0.141637  0.488529 -0.0985094  -105.918    -9.361  
-22 527 59726.00 I  0.143578 0.000020  0.488526 0.000034  I-0.0986417 0.0000074  0.0667 0.0056  I  -106.168    0.831    -9.113    0.068  0.143638  0.488445 -0.0986407  -106.153    -9.084  
-22 528 59727.00 I  0.145155 0.000016  0.488332 0.000026  I-0.0986054 0.0000084 -0.1553 0.0056  I  -106.455    0.876    -8.932    0.072  0.145102  0.488400 -0.0986068  -106.467    -8.914  
-22 529 59728.00 I  0.146685 0.000015  0.488251 0.000025  I-0.0983125 0.0000083 -0.4331 0.0055  I  -106.618    0.876    -8.975    0.072  0.146706  0.488268 -0.0983314  -106.669    -8.976  
-22 530 59729.00 I  0.148142 0.000026  0.487978 0.000036  I-0.0977393 0.0000070 -0.7107 0.0053  I  -106.623    0.864    -9.282    0.057  0.148067  0.488086 -0.0977877  -106.716    -9.292  
-22 531 59730.00 I  0.149844 0.000025  0.487054 0.000027  I-0.0969106 0.0000065 -0.9298 0.0045  I  -106.562    0.840    -9.686    0.031  0.149795  0.487092 -0.0969563  -106.700    -9.703  
-22 6 1 59731.00 I  0.152000 0.000030  0.486286 0.000038  I-0.0959030 0.0000056 -1.0789 0.0045  I  -106.542    1.030    -9.952    0.050  0.151943  0.486170 -0.0959109  -106.731    -9.971  
-22 6 2 59732.00 I  0.154336 0.000030  0.485357 0.000037  I-0.0947797 0.0000062 -1.1474 0.0044  I  -106.621    1.030   -10.003    0.050  0.154357  0.485426 -0.0947757  -106.670   -10.005  
-22 6 3 59733.00 I  0.156607 0.000030  0.484864 0.000037  I-0.0936407 0.0000067 -1.1184 0.0048  I  -106.804    1.030    -9.972    0.050  0.156589  0.484781 -0.0936356  -106.660    -9.955  
-22 6 4 59734.00 I  0.158875 0.000030  0.484102 0.000037  I-0.0925699 0.0000074 -1.0083 0.0064  I  -106.996    1.030   -10.005    0.050  0.158889  0.484149 -0.0925602  -106.851    -9.984  
-22 6 5 59735.00 I  0.161159 0.000020  0.483633 0.000027  I-0.0916234 0.0000110 -0.9002 0.0056  I  -107.007    1.266   -10.075    0.066  0.161161  0.483622 -0.0916220  -106.921   -10.058  
-22 6 6 59736.00 I  0.163475 0.000027  0.483155 0.000031  I-0.0907778 0.0000085 -0.7673 0.0075  I  -106.756    0.996   -10.057    0.087  0.163382  0.483150 -0.0908246  -106.715   -10.044  
-22 6 7 59737.00 I  0.166256 0.000021  0.482820 0.000018  I-0.0901222 0.0000102 -0.5342 0.0062  I  -106.478    0.872    -9.931    0.096  0.166198  0.482812 -0.0901686  -106.474    -9.925  
-22 6 8 59738.00 I  0.169366 0.000026  0.482909 0.000037  I-0.0896769 0.0000090 -0.3985 0.0068  I  -106.547    0.889    -9.829    0.091  0.169346  0.482843 -0.0896819  -106.581    -9.834  
-22 6 9 59739.00 I  0.172337 0.000026  0.482810 0.000037  I-0.0893174 0.0000089 -0.2862 0.0062  I  -107.042    0.889    -9.826    0.091  0.172338  0.482895 -0.0893344  -107.056    -9.817  
-22 610 59740.00 I  0.175169 0.000026  0.482967 0.000037  I-0.0890922 0.0000084 -0.2109 0.0060  I  -107.668    0.889    -9.774    0.091  0.175150  0.482907 -0.0890843  -107.652    -9.745  
-22 611 59741.00 I  0.177826 0.000026  0.482590 0.000037  I-0.0888448 0.0000081 -0.2879 0.0056  I  -108.215    0.889    -9.495    0.091  0.177834  0.482720 -0.0888551  -108.201    -9.465  
-22 612 59742.00 I  0.180320 0.000023  0.482009 0.000040  I-0.0884905 0.0000073 -0.4424 0.0054  I  -108.808    0.779    -9.107    0.101  0.180290  0.482016 -0.0885165  -108.809    -9.083  
-22 613 59743.00 I  0.182803 0.000023  0.481188 0.000040  I-0.0879264 0.0000071 -0.6975 0.0051  I  -109.514    0.779    -8.964    0.101  0.182826  0.481258 -0.0879480  -109.531    -8.942  
-22 614 59744.00 I  0.185076 0.000015  0.480464 0.000023  I-0.0870865 0.0000072 -0.9795 0.0049  I  -109.993    0.724    -9.208    0.111  0.185100  0.480403 -0.0870940  -110.036    -9.188  
-22 615 59745.00 I  0.187070 0.000034  0.479241 0.000037  I-0.0859877 0.0000068 -1.2005 0.0050  I  -109.870    0.734    -9.587    0.125  0.187052  0.479331 -0.0859830  -109.873    -9.588  
-22 616 59746.00 I  0.189198 0.000034  0.478011 0.000037  I-0.0847345 0.0000068 -1.2746 0.0048  I  -109.272    0.734    -9.808    0.125  0.189149  0.478024 -0.0847332  -109.222    -9.837  
-22 617 59747.00 I  0.191613 0.000034  0.476766 0.000037  I-0.0834981 0.0000068 -1.1698 0.0058  I  -108.690    0.734    -9.874    0.125  0.191602  0.476728 -0.0834949  -108.594    -9.934  
-22 618 59748.00 I  0.194037 0.000032  0.475516 0.000030  I-0.0824293 0.0000093 -0.9619 0.0063  I  -108.460    0.898    -9.926    0.199  0.194019  0.475550 -0.0824189  -108.365    -9.983  
-22 619 59749.00 I  0.196592 0.000032  0.474529 0.000030  I-0.0815690 0.0000106 -0.7700 0.0059  I  -108.584    0.898    -9.932    0.199  0.196541  0.474534 -0.0815575  -108.509    -9.976  
-22 620 59750.00 I  0.199463 0.000034  0.473569 0.000035  I-0.0808708 0.0000072 -0.6337 0.0063  I  -108.896    0.835    -9.762    0.155  0.199454  0.473574 -0.0808812  -108.836    -9.796  
-22 621 59751.00 I  0.202395 0.000013  0.472801 0.000020  I-0.0802855 0.0000069 -0.5458 0.0047  I  -109.207    0.832    -9.441    0.148  0.202403  0.472799 -0.0803109  -109.153    -9.467  
-22 622 59752.00 I  0.205095 0.000018  0.472319 0.000024  I-0.0797453 0.0000060 -0.5596 0.0046  I  -109.400    0.719    -9.156    0.139  0.205128  0.472282 -0.0797589  -109.347    -9.174  
-22 623 59753.00 I  0.207617 0.000019  0.471572 0.000025  I-0.0791174 0.0000062 -0.7200 0.0043  I  -109.533    0.719    -9.018    0.139  0.207619  0.471645 -0.0791011  -109.587    -9.025  
-22 624 59754.00 I  0.210140 0.000019  0.470821 0.000025  I-0.0782998 0.0000063 -0.8969 0.0045  I  -109.766    0.719    -8.977    0.139  0.210148  0.470821 -0.0782976  -109.961    -8.971  
-22 625 59755.00 I  0.212734 0.000020  0.469671 0.000025  I-0.0773292 0.0000064 -1.0569 0.0046  I  -110.124    0.719    -8.981    0.139  0.212693  0.469719 -0.0773260  -110.305    -8.982  
-22 626 59756.00 I  0.215402 0.000024  0.468458 0.000027  I-0.0761675 0.0000067 -1.2726 0.0047  I  -110.449    0.715    -9.097    0.145  0.215376  0.468485 -0.0761726  -110.571    -9.112  
-22 627 59757.00 I  0.218221 0.000024  0.467007 0.000026  I-0.0748089 0.0000069 -1.4138 0.0054  I  -110.584    0.715    -9.400    0.145  0.218164  0.467038 -0.0748406  -110.659    -9.428  
-22 628 59758.00 I  0.221334 0.000020  0.465664 0.000023  I-0.0733568 0.0000085 -1.5042 0.0056  I  -110.546    0.907    -9.791    0.161  0.221330  0.465623 -0.0733645  -110.576    -9.834  
-22 629 59759.00 I  0.224405 0.000022  0.464119 0.000035  I-0.0718014 0.0000088 -1.5917 0.0063  I  -110.489    0.982   -10.034    0.135  0.224443  0.464165 -0.0718011  -110.473   -10.052  
-22 630 59760.00 I  0.227228 0.000021  0.462589 0.000035  I-0.0702026 0.0000093 -1.5914 0.0064  I  -110.549    0.982    -9.993    0.135  0.227220  0.462671 -0.0702118  -110.474    -9.975  
-22 7 1 59761.00 I  0.230016 0.000021  0.460917 0.000035  I-0.0686538 0.0000094 -1.4853 0.0081  I  -110.749    0.982    -9.779    0.135  0.230002  0.460818 -0.0686663  -110.599    -9.722  
-22 7 2 59762.00 I  0.232933 0.000011  0.459176 0.000029  I-0.0672366 0.0000132 -1.3654 0.0073  I  -111.003    1.080    -9.606    0.072  0.232881  0.459225 -0.0672447  -110.959    -9.582  
-22 7 3 59763.00 I  0.236097 0.000015  0.457836 0.000038  I-0.0659447 0.0000112 -1.1804 0.0086  I  -111.152    0.913    -9.542    0.143  0.236109  0.457809 -0.0659625  -111.150    -9.536  
-22 7 4 59764.00 I  0.239192 0.000014  0.456518 0.000038  I-0.0649095 0.0000110 -0.8941 0.0074  I  -111.086    0.913    -9.489    0.143  0.239234  0.456579 -0.0649159  -111.121    -9.498  
-22 7 5 59765.00 I  0.241892 0.000014  0.455215 0.000034  I-0.0641385 0.0000096 -0.6617 0.0071  I  -110.905    0.851    -9.366    0.185  0.241892  0.455171 -0.0641393  -110.976    -9.390  
-22 7 6 59766.00 I  0.244459 0.000014  0.453233 0.000034  I-0.0635508 0.0000090 -0.5352 0.0066  I  -110.908    0.851    -9.242    0.185  0.244450  0.453302 -0.0635337  -110.950    -9.262  
-22 7 7 59767.00 I  0.247123 0.000014  0.451687 0.000034  I-0.0630483 0.0000090 -0.4680 0.0063  I  -111.302    0.851    -9.212    0.185  0.247124  0.451582 -0.0630501  -111.305    -9.226  
-22 7 8 59768.00 I  0.249745 0.000014  0.450070 0.000035  I-0.0625850 0.0000089 -0.4900 0.0065  I  -111.986    0.851    -9.221    0.185  0.249756  0.450120 -0.0625785  -111.978    -9.228  
-22 7 9 59769.00 I  0.252293 0.000011  0.448667 0.000026  I-0.0620259 0.0000094 -0.6391 0.0054  I  -112.729    0.943    -9.129    0.218  0.252297  0.448682 -0.0620271  -112.723    -9.129  
-22 710 59770.00 I  0.254694 0.000017  0.447033 0.000028  I-0.0612786 0.0000060 -0.8727 0.0057  I  -113.425    0.796    -8.964    0.149  0.254733  0.447060 -0.0612967  -113.423    -8.960  
-22 711 59771.00 I  0.256802 0.000016  0.445382 0.000019  I-0.0602832 0.0000066 -1.0982 0.0045  I  -113.995    0.755    -8.945    0.115  0.256857  0.445395 -0.0603249  -114.007    -8.936  
-22 712 59772.00 I  0.258322 0.000016  0.443981 0.000019  I-0.0591150 0.0000066 -1.2252 0.0049  I  -114.213    0.755    -9.158    0.115  0.258411  0.443974 -0.0591324  -114.246    -9.142  
-22 713 59773.00 I  0.259222 0.000017  0.442010 0.000025  I-0.0578239 0.0000072 -1.3788 0.0049  I  -113.935    0.783    -9.395    0.154  0.259174  0.442066 -0.0577813  -113.960    -9.403  
-22 714 59774.00 I  0.260256 0.000017  0.439903 0.000024  I-0.0564317 0.0000073 -1.3096 0.0052  I  -113.405    0.783    -9.444    0.154  0.260201  0.439888 -0.0564587  -113.418    -9.484  
-22 715 59775.00 I  0.261703 0.000017  0.438186 0.000024  I-0.0552591 0.0000074 -1.0771 0.0066  I  -113.034    0.783    -9.394    0.154  0.261642  0.438122 -0.0552630  -113.037    -9.466  
-22 716 59776.00 I  0.263452 0.000013  0.436323 0.000021  I-0.0542689 0.0000110 -0.8702 0.0056  I  -112.981    0.857    -9.438    0.216  0.263441  0.436373 -0.0542876  -112.983    -9.496  
-22 717 59777.00 I  0.265296 0.000017  0.434386 0.000022  I-0.0535129 0.0000084 -0.6806 0.0069  I  -113.167    0.907    -9.519    0.145  0.265267  0.434398 -0.0535228  -113.161    -9.544  
-22 718 59778.00 I  0.267260 0.000018  0.432324 0.000021  I-0.0528768 0.0000083 -0.5837 0.0057  I  -113.524    0.907    -9.408    0.145  0.267234  0.432352 -0.0528927  -113.506    -9.398  
-22 719 59779.00 I  0.269240 0.000018  0.430321 0.000012  I-0.0523099 0.0000076 -0.5937 0.0056  I  -113.990    0.933    -9.085    0.075  0.269260  0.430298 -0.0523068  -113.947    -9.037  
-22 720 59780.00 I  0.270985 0.000026  0.428180 0.000027  I-0.0516585 0.0000074 -0.6963 0.0054  I  -114.395    0.857    -8.814    0.130  0.270974  0.428173 -0.0516628  -114.393    -8.784  
-22 721 59781.00 I  0.272566 0.000027  0.426236 0.000027  I-0.0509072 0.0000076 -0.8291 0.0053  I  -114.621    0.857    -8.807    0.130  0.272574  0.426255 -0.0508922  -114.674    -8.805  
-22 722 59782.00 I  0.274101 0.000027  0.424534 0.000028  I-0.0499780 0.0000075 -1.0288 0.0060  I  -114.773    0.857    -8.993    0.130  0.274053  0.424453 -0.0499591  -114.884    -9.018  
-22 723 59783.00 I  0.275662 0.000024  0.422636 0.000027  I-0.0488588 0.0000093 -1.2010 0.0056  I  -115.013    0.708    -9.183    0.183  0.275681  0.422673 -0.0488673  -115.096    -9.210  
-22 724 59784.00 I  0.277054 0.000025  0.420927 0.000034  I-0.0475836 0.0000082 -1.3506 0.0062  I  -115.302    0.799    -9.322    0.190  0.277006  0.420915 -0.0476028  -115.333    -9.343  
-22 725 59785.00 I  0.278485 0.000025  0.419304 0.000035  I-0.0461801 0.0000082 -1.4329 0.0062  I  -115.469    0.799    -9.504    0.190  0.278471  0.419285 -0.0462003  -115.452    -9.519  
-22 726 59786.00 I  0.279854 0.000015  0.417978 0.000024  I-0.0447424 0.0000093 -1.4416 0.0060  I  -115.459    0.892    -9.758    0.202  0.279867  0.417962 -0.0447491  -115.399    -9.768  
-22 727 59787.00 I  0.281073 0.000025  0.416094 0.000039  I-0.0432971 0.0000088 -1.4499 0.0068  I  -115.382    0.892    -9.944    0.202  0.281044  0.416126 -0.0432579  -115.379    -9.934  
-22 728 59788.00 I  0.282268 0.000025  0.414126 0.000039  I-0.0418445 0.0000100 -1.4525 0.0073  I  -115.353    0.892    -9.901    0.202  0.282267  0.414205 -0.0417953  -115.431    -9.867  
-22 729 59789.00 I  0.283369 0.000024  0.411945 0.000038  I-0.0404251 0.0000117 -1.3560 0.0098  I  -115.381    0.892    -9.653    0.202  0.283345  0.411841 -0.0404282  -115.538    -9.595  
-22 730 59790.00 I  0.284623 0.000023  0.409371 0.000033  I-0.0391786 0.0000168 -1.1211 0.0097  I  -115.415    0.322    -9.394    0.160  0.284587  0.409400 -0.0392089  -115.593    -9.353  
-22 731 59791.00 I  0.285988 0.000034  0.407309 0.000040  I-0.0381710 0.0000156 -0.9219 0.0115  I  -115.418    0.796    -9.280    0.318  0.286000  0.407286 -0.0381849  -115.593    -9.273  
-22 8 1 59792.00 I  0.287131 0.000034  0.405160 0.000040  I-0.0373395 0.0000156 -0.7086 0.0098  I  -115.369    0.796    -9.289    0.318  0.287161  0.405194 -0.0373892  -115.536    -9.320  
-22 8 2 59793.00 I  0.287882 0.000028  0.403351 0.000030  I-0.0367458 0.0000120 -0.5192 0.0097  I  -115.284    0.762    -9.303    0.284  0.287882  0.403262 -0.0367846  -115.439    -9.376  
-22 8 3 59794.00 I  0.288544 0.000029  0.400939 0.000030  I-0.0362599 0.0000117 -0.4532 0.0081  I  -115.273    0.762    -9.263    0.284  0.288468  0.401019 -0.0362792  -115.414    -9.314  
-22 8 4 59795.00 I  0.289525 0.000029  0.398767 0.000029  I-0.0358141 0.0000110 -0.4630 0.0079  I  -115.510    0.762    -9.205    0.284  0.289489  0.398709 -0.0358145  -115.635    -9.222  
-22 8 5 59796.00 I  0.290539 0.000029  0.396534 0.000029  I-0.0353154 0.0000107 -0.5284 0.0066  I  -116.063    0.762    -9.176    0.284  0.290582  0.396579 -0.0353263  -116.154    -9.192  
-22 8 6 59797.00 I  0.291094 0.000015  0.394203 0.000017  I-0.0347291 0.0000074 -0.6785 0.0060  I  -116.788    0.736    -9.177    0.244  0.291080  0.394221 -0.0347316  -116.838    -9.204  
-22 8 7 59798.00 I  0.291546 0.000022  0.391643 0.000020  I-0.0339358 0.0000056 -0.8965 0.0051  I  -117.423    0.716    -9.224    0.251  0.291487  0.391652 -0.0339451  -117.435    -9.261  
-22 8 8 59799.00 I  0.292337 0.000021  0.389012 0.000014  I-0.0329625 0.0000070 -1.0355 0.0045  I  -117.732    0.707    -9.356    0.256  0.292293  0.389056 -0.0329721  -117.715    -9.399  
-22 8 9 59800.00 I  0.293207 0.000021  0.386258 0.000013  I-0.0318899 0.0000071 -1.0994 0.0046  I  -117.614    0.707    -9.521    0.256  0.293211  0.386232 -0.0318918  -117.585    -9.565  
-22 810 59801.00 I  0.293834 0.000023  0.383239 0.000025  I-0.0308023 0.0000059 -1.0476 0.0048  I  -117.209    0.739    -9.544    0.271  0.293803  0.383250 -0.0308088  -117.149    -9.591  
-22 811 59802.00 I  0.294451 0.000023  0.380323 0.000026  I-0.0298462 0.0000064 -0.8412 0.0045  I  -116.855    0.739    -9.347    0.271  0.294459  0.380298 -0.0298577  -116.770    -9.397  
-22 812 59803.00 I  0.295059 0.000023  0.377876 0.000026  I-0.0291298 0.0000067 -0.6051 0.0052  I  -116.787    0.739    -9.113    0.271  0.295055  0.377755 -0.0291384  -116.681    -9.171  
-22 813 59804.00 I  0.295579 0.000015  0.375683 0.000025  I-0.0286213 0.0000083 -0.4130 0.0051  I  -116.918    0.775    -9.085    0.284  0.295537  0.375740 -0.0286307  -116.834    -9.134  
-22 814 59805.00 I  0.296372 0.000014  0.373576 0.000025  I-0.0282774 0.0000076 -0.2999 0.0054  I  -117.059    0.775    -9.225    0.284  0.296313  0.373591 -0.0282983  -117.006    -9.266  
-22 815 59806.00 I  0.297512 0.000016  0.371305 0.000029  I-0.0279768 0.0000068 -0.3208 0.0068  I  -117.234    0.763    -9.267    0.243  0.297500  0.371314 -0.0279699  -117.203    -9.307  
-22 816 59807.00 I  0.298550 0.000014  0.369031 0.000020  I-0.0276026 0.0000112 -0.4412 0.0068  I  -117.579    0.739    -9.095    0.156  0.298583  0.369059 -0.0276395  -117.555    -9.139  
-22 817 59808.00 I  0.299278 0.000021  0.366802 0.000029  I-0.0270777 0.0000118 -0.6117 0.0082  I  -118.035    0.739    -8.900    0.156  0.299254  0.366732 -0.0270866  -118.003    -8.949  
-22 818 59809.00 I  0.299909 0.000021  0.364360 0.000029  I-0.0263509 0.0000119 -0.8670 0.0084  I  -118.387    0.739    -8.906    0.156  0.299866  0.364425 -0.0263517  -118.274    -8.865  
-22 819 59810.00 I  0.300904 0.000021  0.362096 0.000029  I-0.0253533 0.0000120 -1.0936 0.0086  I  -118.557    0.739    -9.087    0.156  0.300823  0.362010 -0.0253455  -118.335    -8.928  
-22 820 59811.00 I  0.302126 0.000021  0.359723 0.000029  I-0.0241783 0.0000125 -1.2766 0.0088  I  -118.646    0.739    -9.236    0.156  0.302176  0.359779 -0.0241871  -118.439    -9.105  
-22 821 59812.00 I  0.303009 0.000022  0.357442 0.000037  I-0.0228204 0.0000128 -1.3987 0.0089  I  -118.711    0.583    -9.251    0.088  0.302992  0.357455 -0.0228266  -118.572    -9.196  
-22 822 59813.00 I  0.303768 0.000022  0.354897 0.000037  I-0.0214092 0.0000127 -1.4359 0.0084  I  -118.688    0.583    -9.228    0.088  0.303769  0.354926 -0.0213929  -118.632    -9.243  
-22 823 59814.00 I  0.304481 0.000015  0.352582 0.000031  I-0.0199839 0.0000110 -1.3673 0.0071  I  -118.541    0.583    -9.300    0.088  0.304513  0.352500 -0.0199836  -118.587    -9.375  
-22 824 59815.00 I  0.304887 0.000016  0.349859 0.000037  I-0.0186814 0.0000065 -1.2785 0.0064  I  -118.346    0.652    -9.436    0.123  0.304896  0.349874 -0.0186613  -118.307    -9.531  
-22 825 59816.00 I  0.305185 0.000015  0.347444 0.000037  I-0.0174153 0.0000066 -1.2246 0.0044  I  -118.187    0.652    -9.478    0.123  0.305201  0.347486 -0.0174037  -118.023    -9.577  
-22 826 59817.00 I  0.305353 0.000014  0.345001 0.000037  I-0.0162761 0.0000059 -1.0389 0.0044  I  -118.052    0.652    -9.337    0.123  0.305398  0.344912 -0.0162851  -117.767    -9.438  
-22 827 59818.00 I  0.305270 0.000010  0.342297 0.000024  I-0.0153423 0.0000057 -0.8389 0.0043  I  -117.902    0.898    -9.106    0.171  0.305290  0.342335 -0.0153482  -117.637    -9.193  
-22 828 59819.00 I  0.304966 0.000019  0.339930 0.000030  I-0.0146069 0.0000063 -0.6130 0.0044  I  -117.764    0.774    -8.964    0.186  0.304974  0.339946 -0.0146136  -117.565    -9.035  
-22 829 59820.00 I  0.304625 0.000019  0.337374 0.000029  I-0.0141121 0.0000066 -0.3995 0.0049  I  -117.692    0.774    -8.995    0.186  0.304586  0.337401 -0.0140968  -117.551    -9.055  
-22 830 59821.00 I  0.304494 0.000019  0.335049 0.000020  I-0.0137905 0.0000075 -0.2380 0.0043  I  -117.681    0.736    -9.122    0.195  0.304464  0.334971 -0.0137838  -117.601    -9.176  
-22 831 59822.00 I  0.304616 0.000021  0.332698 0.000024  I-0.0136131 0.0000054 -0.1454 0.0047  I  -117.698    0.747    -9.208    0.165  0.304595  0.332751 -0.0136099  -117.612    -9.248  
-22 9 1 59823.00 I  0.304752 0.000021  0.330389 0.000024  I-0.0134602 0.0000056 -0.1711 0.0042  I  -117.799    0.747    -9.188    0.165  0.304814  0.330440 -0.0134836  -117.693    -9.211  
-22 9 2 59824.00 I  0.304504 0.000021  0.327695 0.000024  I-0.0132440 0.0000064 -0.2773 0.0043  I  -118.087    0.747    -9.109    0.165  0.304501  0.327651 -0.0132494  -118.154    -9.102  
-22 9 3 59825.00 I  0.304209 0.000012  0.325025 0.000015  I-0.0128866 0.0000064 -0.4403 0.0043  I  -118.530    0.757    -9.073    0.134  0.304186  0.324993 -0.0128821  -118.590    -9.080  
-22 9 4 59826.00 I  0.304086 0.000014  0.322772 0.000023  I-0.0123623 0.0000058 -0.6065 0.0043  I  -118.885    0.735    -9.140    0.190  0.304085  0.322764 -0.0123741  -118.929    -9.170  
-22 9 5 59827.00 I  0.303787 0.000014  0.320435 0.000023  I-0.0117020 0.0000058 -0.6873 0.0060  I  -118.883    0.735    -9.276    0.190  0.303820  0.320481 -0.0117203  -118.916    -9.328  
-22 9 6 59828.00 I  0.303227 0.000012  0.318033 0.000019  I-0.0110167 0.0000104 -0.6810 0.0050  I  -118.484    0.709    -9.345    0.245  0.303248  0.318029 -0.0110190  -118.525    -9.426  
-22 9 7 59829.00 I  0.302620 0.000014  0.314894 0.000027  I-0.0103855 0.0000082 -0.5380 0.0064  I  -117.956    0.865    -9.204    0.195  0.302652  0.314951 -0.0103738  -117.930    -9.248  
-22 9 8 59830.00 I  0.301725 0.000015  0.311753 0.000027  I-0.0099746 0.0000075 -0.2931 0.0059  I  -117.660    0.865    -8.859    0.195  0.301793  0.311758 -0.0099952  -117.557    -8.853  
-22 9 9 59831.00 I  0.300342 0.000016  0.308744 0.000029  I-0.0098010 0.0000085 -0.0431 0.0061  I  -117.717    0.865    -8.517    0.195  0.300297  0.308670 -0.0098037  -117.537    -8.461  
-22 910 59832.00 I  0.299160 0.000014  0.305635 0.000023  I-0.0098892 0.0000096  0.2094 0.0057  I  -117.914    1.166    -8.404    0.074  0.299086  0.305665 -0.0098938  -117.785    -8.354  
-22 911 59833.00 I  0.298571 0.000024  0.302860 0.000034  I-0.0101811 0.0000077  0.3460 0.0062  I  -117.993    0.970    -8.521    0.141  0.298524  0.302843 -0.0101991  -117.949    -8.495  
-22 912 59834.00 I  0.298129 0.000024  0.300249 0.000034  I-0.0105451 0.0000079  0.3744 0.0061  I  -117.974    0.970    -8.669    0.141  0.298153  0.300265 -0.0105663  -118.003    -8.665  
-22 913 59835.00 I  0.297553 0.000024  0.298016 0.000031  I-0.0108732 0.0000094  0.2329 0.0056  I  -118.082    0.886    -8.702    0.168  0.297509  0.297897 -0.0108687  -118.179    -8.722  
-22 914 59836.00 I  0.296978 0.000025  0.295772 0.000049  I-0.0109857 0.0000078  0.0159 0.0061  I  -118.400    0.902    -8.680    0.136  0.296992  0.295809 -0.0110048  -118.515    -8.694  
-22 915 59837.00 I  0.296334 0.000024  0.293794 0.000048  I-0.0108932 0.0000079 -0.2364 0.0055  I  -118.754    0.902    -8.730    0.136  0.296326  0.293853 -0.0109071  -118.881    -8.735  
-22 916 59838.00 I  0.295607 0.000024  0.291776 0.000048  I-0.0105233 0.0000078 -0.4575 0.0059  I  -118.926    0.902    -8.848    0.136  0.295633  0.291666 -0.0105453  -119.064    -8.840  
-22 917 59839.00 I  0.294744 0.000015  0.289567 0.000041  I-0.0099856 0.0000088 -0.6564 0.0056  I  -118.849    0.928    -8.900    0.088  0.294765  0.289613 -0.0099966  -118.954    -8.905  
-22 918 59840.00 I  0.293577 0.000019  0.287802 0.000054  I-0.0092294 0.0000081 -0.7986 0.0059  I  -118.591    0.988    -8.822    0.130  0.293594  0.287789 -0.0092502  -118.640    -8.844  
-22 919 59841.00 I  0.292284 0.000019  0.285822 0.000053  I-0.0084297 0.0000079 -0.8171 0.0059  I  -118.237    0.988    -8.710    0.130  0.292235  0.285928 -0.0084134  -118.223    -8.750  
-22 920 59842.00 I  0.291352 0.000018  0.283591 0.000037  I-0.0075714 0.0000086 -0.9071 0.0051  I  -117.863    1.078    -8.710    0.170  0.291284  0.283515 -0.0075559  -117.778    -8.771  
-22 921 59843.00 I  0.290658 0.000019  0.281017 0.000039  I-0.0066715 0.0000064 -0.8290 0.0052  I  -117.562    0.957    -8.833    0.126  0.290675  0.281089 -0.0066950  -117.531    -8.864  
-22 922 59844.00 I  0.289762 0.000019  0.278371 0.000038  I-0.0059625 0.0000060 -0.6035 0.0046  I  -117.391    0.957    -8.934    0.126  0.289785  0.278400 -0.0059969  -117.441    -8.921  
-22 923 59845.00 I  0.288623 0.000018  0.275583 0.000039  I-0.0054439 0.0000065 -0.4398 0.0046  I  -117.331    0.957    -8.873    0.126  0.288673  0.275532 -0.0054471  -117.457    -8.810  
-22 924 59846.00 I  0.287261 0.000014  0.272920 0.000015  I-0.0050916 0.0000071 -0.2501 0.0048  I  -117.326    0.805    -8.661    0.027  0.287244  0.272949 -0.0051006  -117.468    -8.622  
-22 925 59847.00 I  0.285950 0.000025  0.270442 0.000035  I-0.0049405 0.0000070 -0.0699 0.0050  I  -117.349    0.769    -8.451    0.192  0.285878  0.270404 -0.0049635  -117.484    -8.457  
-22 926 59848.00 I  0.285166 0.000025  0.268138 0.000034  I-0.0049423 0.0000071  0.0818 0.0057  I  -117.406    0.769    -8.388    0.192  0.285103  0.268121 -0.0049793  -117.537    -8.441  
-22 927 59849.00 I  0.284709 0.000024  0.266516 0.000032  I-0.0050966 0.0000089  0.2109 0.0053  I  -117.484    0.744    -8.488    0.260  0.284746  0.266357 -0.0051012  -117.616    -8.597  
-22 928 59850.00 I  0.283877 0.000025  0.264882 0.000033  I-0.0053042 0.0000079  0.1602 0.0058  I  -117.554    0.670    -8.634    0.185  0.283878  0.264953 -0.0053014  -117.693    -8.702  
-22 929 59851.00 I  0.283007 0.000025  0.263313 0.000033  I-0.0053854 0.0000074  0.0148 0.0053  I  -117.617    0.670    -8.699    0.185  0.282943  0.263319 -0.0054180  -117.779    -8.707  
-22 930 59852.00 I  0.282322 0.000024  0.261526 0.000033  I-0.0053250 0.0000071 -0.1570 0.0051  I  -117.701    0.670    -8.656    0.185  0.282338  0.261528 -0.0053388  -117.905    -8.603  
-2210 1 59853.00 I  0.281361 0.000013  0.259737 0.000015  I-0.0050433 0.0000069 -0.4129 0.0049  I  -117.771    0.566    -8.579    0.031  0.281388  0.259744 -0.0049041  -117.934    -8.536  
-2210 2 59854.00 I  0.280043 0.000011  0.257886 0.000015  I-0.0045474 0.0000067 -0.5240 0.0043  I  -117.700    0.566    -8.555    0.031  0.280092  0.257931 -0.0043864  -117.763    -8.633  
-2210 3 59855.00 I  0.278450 0.000017  0.255735 0.000018  I-0.0040462 0.0000051 -0.4823 0.0044  I  -117.362    0.918    -8.587    0.135  0.278478  0.255746 -0.0040146  -117.380    -8.681  
-2210 4 59856.00 I  0.276548 0.000016  0.253507 0.000016  I-0.0035886 0.0000057 -0.4232 0.0034  I  -116.792    1.082    -8.594    0.177  0.276607  0.253527 -0.0035590  -116.777    -8.672  
-2210 5 59857.00 I  0.274392 0.000017  0.251464 0.000021  I-0.0032267 0.0000044 -0.2836 0.0038  I  -116.216    1.068    -8.481    0.157  0.274352  0.251450 -0.0032281  -116.158    -8.550  
-2210 6 59858.00 I  0.272446 0.000021  0.249202 0.000022  I-0.0030613 0.0000049 -0.0244 0.0035  I  -115.894    1.068    -8.245    0.157  0.272409  0.249284 -0.0030816  -115.892    -8.306  
-2210 7 59859.00 I  0.270890 0.000023  0.246768 0.000020  I-0.0031814 0.0000055  0.2454 0.0037  I  -115.901    1.068    -7.990    0.157  0.270869  0.246728 -0.0031810  -115.963    -8.047  
-2210 8 59860.00 I  0.269392 0.000023  0.244256 0.000020  I-0.0035334 0.0000056  0.4593 0.0043  I  -116.075    1.068    -7.832    0.157  0.269464  0.244272 -0.0035337  -116.181    -7.889  
-2210 9 59861.00 I  0.267405 0.000018  0.242156 0.000017  I-0.0040709 0.0000067  0.5859 0.0039  I  -116.191    1.055    -7.793    0.132  0.267436  0.242181 -0.0040628  -116.323    -7.852  
-221010 59862.00 I  0.265325 0.000021  0.239989 0.000018  I-0.0046592 0.0000055  0.5744 0.0048  I  -116.181    0.930    -7.811    0.107  0.265240  0.239987 -0.0046541  -116.330    -7.871  
-221011 59863.00 I  0.263669 0.000020  0.237862 0.000011  I-0.0051762 0.0000069  0.4322 0.0041  I  -116.177    0.772    -7.838    0.071  0.263701  0.237885 -0.0051692  -116.344    -7.899  
-221012 59864.00 I  0.262028 0.000021  0.235769 0.000012  I-0.0054969 0.0000060  0.2098 0.0046  I  -116.323    0.827    -7.890    0.053  0.262046  0.235701 -0.0055011  -116.517    -7.950  
-221013 59865.00 I  0.259882 0.000019  0.233754 0.000012  I-0.0055875 0.0000062 -0.0376 0.0044  I  -116.581    0.827    -7.985    0.053  0.260021  0.233734 -0.0055722  -116.707    -8.023  
-221014 59866.00 I  0.256982 0.000019  0.232122 0.000011  I-0.0054408 0.0000064 -0.2277 0.0045  I  -116.749    0.827    -8.072    0.053  0.256936  0.232102 -0.0054362  -116.793    -8.078  
-221015 59867.00 I  0.254058 0.000019  0.230349 0.000011  I-0.0051764 0.0000064 -0.2850 0.0044  I  -116.645    0.827    -8.072    0.053  0.254063  0.230356 -0.0051876  -116.700    -8.075  
-221016 59868.00 I  0.251193 0.000020  0.228850 0.000025  I-0.0048938 0.0000059 -0.2732 0.0043  I  -116.260    0.986    -7.981    0.107  0.251206  0.228893 -0.0049099  -116.365    -7.987  
-221017 59869.00 I  0.248067 0.000023  0.227215 0.000026  I-0.0046590 0.0000058 -0.1745 0.0043  I  -115.731    0.986    -7.905    0.107  0.248052  0.227286 -0.0046783  -115.804    -7.935  
-221018 59870.00 I  0.245186 0.000019  0.225195 0.000026  I-0.0045591 0.0000062 -0.0330 0.0041  I  -115.203    1.037    -7.949    0.141  0.245102  0.225158 -0.0045660  -115.200    -8.015  
-221019 59871.00 I  0.243016 0.000022  0.222914 0.000030  I-0.0045886 0.0000058  0.0954 0.0042  I  -114.763    1.061    -8.091    0.163  0.243041  0.222898 -0.0045814  -114.747    -8.164  
-221020 59872.00 I  0.240707 0.000023  0.221149 0.000030  I-0.0047679 0.0000057  0.2777 0.0040  I  -114.469    1.061    -8.189    0.163  0.240817  0.221191 -0.0047645  -114.446    -8.265  
-221021 59873.00 I  0.237715 0.000023  0.219364 0.000030  I-0.0051485 0.0000055  0.4735 0.0053  I  -114.391    1.061    -8.113    0.163  0.237688  0.219313 -0.0051434  -114.344    -8.197  
-221022 59874.00 I  0.234654 0.000021  0.217508 0.000019  I-0.0057167 0.0000089  0.6746 0.0045  I  -114.551    1.092    -7.857    0.192  0.234606  0.217522 -0.0057243  -114.532    -7.927  
-221023 59875.00 I  0.232018 0.000021  0.216040 0.000022  I-0.0065038 0.0000072  0.8940 0.0058  I  -114.849    0.936    -7.538    0.157  0.231878  0.216031 -0.0064986  -114.866    -7.589  
-221024 59876.00 I  0.230034 0.000022  0.214631 0.000022  I-0.0074597 0.0000073  0.9785 0.0054  I  -115.109    0.936    -7.306    0.157  0.230043  0.214645 -0.0074339  -115.163    -7.341  
-221025 59877.00 I  0.228132 0.000021  0.213272 0.000022  I-0.0084074 0.0000080  0.9027 0.0054  I  -115.225    0.811    -7.248    0.109  0.228137  0.213232 -0.0084121  -115.318    -7.265  
-221026 59878.00 I  0.226079 0.000021  0.211730 0.000022  I-0.0092409 0.0000079  0.7541 0.0056  I  -115.215    0.811    -7.354    0.109  0.226115  0.211747 -0.0092591  -115.297    -7.349  
-221027 59879.00 I  0.223694 0.000021  0.210442 0.000022  I-0.0098807 0.0000079  0.5008 0.0052  I  -115.158    0.811    -7.525    0.109  0.223756  0.210409 -0.0098856  -115.222    -7.492  
-221028 59880.00 I  0.220829 0.000019  0.208825 0.000022  I-0.0102288 0.0000068  0.2063 0.0061  I  -115.084    0.811    -7.641    0.109  0.220823  0.208832 -0.0102779  -115.143    -7.612  
-221029 59881.00 I  0.217712 0.000017  0.207412 0.000017  I-0.0103283 0.0000094  0.0167 0.0049  I  -114.960    0.852    -7.642    0.076  0.217709  0.207418 -0.0103958  -115.022    -7.628  
-221030 59882.00 I  0.214510 0.000027  0.206266 0.000021  I-0.0102926 0.0000070 -0.0818 0.0057  I  -114.743    0.859    -7.574    0.183  0.214473  0.206229 -0.0103095  -114.810    -7.575  
-221031 59883.00 I  0.211393 0.000025  0.205209 0.000014  I-0.0101979 0.0000063 -0.0806 0.0047  I  -114.422    0.863    -7.519    0.229  0.211345  0.205237 -0.0101927  -114.492    -7.538  
-2211 1 59884.00 I  0.208602 0.000025  0.204260 0.000017  I-0.0101862 0.0000063  0.0850 0.0040  I  -114.034    0.863    -7.499    0.229  0.208514  0.204211 -0.0101774  -114.100    -7.544  
-2211 2 59885.00 I  0.206231 0.000026  0.203464 0.000020  I-0.0104066 0.0000049  0.3665 0.0041  I  -113.657    0.879    -7.466    0.199  0.206235  0.203545 -0.0104065  -113.700    -7.501  
-2211 3 59886.00 I  0.203876 0.000027  0.202375 0.000020  I-0.0109408 0.0000052  0.7126 0.0035  I  -113.389    0.879    -7.375    0.199  0.203841  0.202359 -0.0109528  -113.392    -7.399  
-2211 4 59887.00 I  0.201539 0.000026  0.201384 0.000020  I-0.0118032 0.0000051  0.9730 0.0044  I  -113.302    0.879    -7.229    0.199  0.201477  0.201353 -0.0118134  -113.257    -7.249  
-2211 5 59888.00 I  0.199497 0.000015  0.200681 0.000016  I-0.0128130 0.0000070  1.0122 0.0034  I  -113.393    0.897    -7.050    0.158  0.199403  0.200700 -0.0128173  -113.353    -7.066  
-2211 6 59889.00 I  0.197923 0.000018  0.199805 0.000021  I-0.0138019 0.0000044  0.9743 0.0043  I  -113.557    0.733    -6.858    0.097  0.197880  0.199789 -0.0138349  -113.543    -6.869  
-2211 7 59890.00 I  0.196417 0.000019  0.198990 0.000019  I-0.0147289 0.0000051  0.8384 0.0036  I  -113.646    0.733    -6.684    0.097  0.196436  0.198985 -0.0147274  -113.659    -6.688  
-2211 8 59891.00 I  0.194595 0.000031  0.198441 0.000023  I-0.0154439 0.0000056  0.5982 0.0036  I  -113.613    0.653    -6.592    0.031  0.194574  0.198424 -0.0154466  -113.660    -6.582  
-2211 9 59892.00 I  0.192635 0.000031  0.197558 0.000023  I-0.0159449 0.0000052  0.4169 0.0038  I  -113.554    0.653    -6.639    0.031  0.192696  0.197558 -0.0159684  -113.571    -6.657  
-221110 59893.00 I  0.190363 0.000030  0.196704 0.000023  I-0.0162460 0.0000050  0.1406 0.0034  I  -113.581    0.653    -6.799    0.031  0.190367  0.196722 -0.0162302  -113.564    -6.849  
-221111 59894.00 I  0.187843 0.000030  0.195900 0.000023  I-0.0162279 0.0000043 -0.1304 0.0058  I  -113.653    0.653    -6.956    0.031  0.187822  0.195880 -0.0162520  -113.631    -7.013  
-221112 59895.00 I  0.185419 0.000028  0.195029 0.000018  I-0.0160393 0.0000105 -0.2391 0.0037  I  -113.603    0.322    -7.003    0.160  0.185361  0.195076 -0.0160839  -113.596    -7.056  
-221113 59896.00 I  0.183320 0.000030  0.193966 0.000021  I-0.0157699 0.0000061 -0.2871 0.0059  I  -113.340    0.725    -6.956    0.094  0.183217  0.193981 -0.0158151  -113.352    -6.999  
-221114 59897.00 I  0.181907 0.000014  0.192821 0.000013  I-0.0155034 0.0000055 -0.2201 0.0042  I  -112.932    0.725    -6.928    0.094  0.181786  0.192794 -0.0155444  -112.967    -6.958  
-221115 59898.00 I  0.181149 0.000015  0.192273 0.000014  I-0.0153471 0.0000058 -0.1008 0.0036  I  -112.493    0.725    -6.992    0.094  0.181089  0.192167 -0.0153549  -112.549    -7.008  
-221116 59899.00 I  0.180590 0.000016  0.192094 0.000020  I-0.0153097 0.0000046  0.0422 0.0038  I  -112.067    0.764    -7.082    0.132  0.180613  0.192084 -0.0153236  -112.120    -7.099  
-221117 59900.00 I  0.179830 0.000016  0.192242 0.000021  I-0.0154617 0.0000048  0.2757 0.0034  I  -111.700    0.764    -7.070    0.132  0.179894  0.192217 -0.0154871  -111.735    -7.093  
-221118 59901.00 I  0.178493 0.000016  0.192679 0.000022  I-0.0158540 0.0000049  0.4877 0.0039  I  -111.552    0.764    -6.902    0.132  0.178587  0.192658 -0.0158559  -111.559    -6.936  
-221119 59902.00 I  0.176649 0.000012  0.192913 0.000019  I-0.0164109 0.0000061  0.6210 0.0032  I  -111.773    0.805    -6.643    0.164  0.176631  0.192939 -0.0164100  -111.782    -6.671  
-221120 59903.00 I  0.174676 0.000015  0.192891 0.000022  I-0.0171026 0.0000040  0.7740 0.0036  I  -112.264    0.733    -6.381    0.154  0.174678  0.192941 -0.0171134  -112.283    -6.399  
-221121 59904.00 I  0.172507 0.000014  0.192675 0.000022  I-0.0179203 0.0000038  0.8110 0.0030  I  -112.721    0.733    -6.150    0.154  0.172482  0.192686 -0.0178985  -112.747    -6.164  
-221122 59905.00 I  0.170163 0.000014  0.192562 0.000016  I-0.0186682 0.0000044  0.6787 0.0027  I  -112.943    0.689    -5.986    0.147  0.170135  0.192562 -0.0186627  -112.985    -5.999  
-221123 59906.00 I  0.167913 0.000021  0.192096 0.000033  I-0.0192694 0.0000038  0.5214 0.0029  I  -112.979    0.712    -5.977    0.143  0.167864  0.192125 -0.0192839  -113.015    -5.992  
-221124 59907.00 I  0.165799 0.000021  0.191630 0.000033  I-0.0196788 0.0000039  0.2676 0.0029  I  -112.924    0.712    -6.159    0.143  0.165815  0.191634 -0.0196773  -112.960    -6.178  
-221125 59908.00 I  0.163383 0.000021  0.191487 0.000033  I-0.0198052 0.0000043  0.0155 0.0036  I  -112.760    0.712    -6.396    0.143  0.163449  0.191394 -0.0198119  -112.800    -6.422  
-221126 59909.00 I  0.160411 0.000020  0.191081 0.000031  I-0.0197330 0.0000061 -0.1670 0.0038  I  -112.469    0.748    -6.480    0.139  0.160439  0.191188 -0.0197408  -112.502    -6.504  
-221127 59910.00 I  0.156937 0.000020  0.190795 0.000031  I-0.0195087 0.0000062 -0.2369 0.0039  I  -112.157    0.748    -6.372    0.139  0.156985  0.190819 -0.0195486  -112.173    -6.392  
-221128 59911.00 I  0.153233 0.000021  0.190266 0.000034  I-0.0193093 0.0000047 -0.1563 0.0043  I  -111.944    0.805    -6.232    0.109  0.153168  0.190278 -0.0193141  -111.939    -6.246  
-221129 59912.00 I  0.149941 0.000015  0.189773 0.000016  I-0.0192201 0.0000059 -0.0036 0.0030  I  -111.820    0.870    -6.194    0.069  0.149881  0.189736 -0.0192085  -111.789    -6.198  
-221130 59913.00 I  0.147023 0.000020  0.189891 0.000021  I-0.0193122 0.0000036  0.1794 0.0033  I  -111.712    0.787    -6.215    0.109  0.146998  0.189837 -0.0193120  -111.648    -6.204  
-2212 1 59914.00 I  0.144056 0.000023  0.190049 0.000021  I-0.0195852 0.0000030  0.3812 0.0024  I  -111.605    0.787    -6.182    0.109  0.144039  0.190129 -0.0196037  -111.563    -6.191  
-2212 2 59915.00 I  0.141123 0.000024  0.190001 0.000020  I-0.0200266 0.0000032  0.4391 0.0021  I  -111.546    0.787    -6.068    0.109  0.141086  0.190030 -0.0200182  -111.557    -6.103  
-2212 3 59916.00 I  0.138502 0.000023  0.189600 0.000020  I-0.0204300 0.0000030  0.3969 0.0024  I  -111.575    0.787    -5.915    0.109  0.138520  0.189588 -0.0204483  -111.593    -5.954  
-2212 4 59917.00 I  0.135671 0.000024  0.189559 0.000018  I-0.0208093 0.0000035  0.3216 0.0024  I  -111.680    0.842    -5.751    0.139  0.135739  0.189603 -0.0208072  -111.696    -5.787  
-2212 5 59918.00 I  0.132717 0.000025  0.189087 0.000018  I-0.0210329 0.0000038  0.1256 0.0033  I  -111.752    0.842    -5.590    0.139  0.132595  0.189132 -0.0210271  -111.763    -5.625  
-2212 6 59919.00 I  0.130242 0.000022  0.188827 0.000013  I-0.0210514 0.0000057 -0.0977 0.0034  I  -111.682    0.994    -5.492    0.147  0.130234  0.188807 -0.0210546  -111.664    -5.528  
-2212 7 59920.00 I  0.127861 0.000023  0.188832 0.000018  I-0.0208448 0.0000056 -0.2990 0.0040  I  -111.505    0.846    -5.545    0.123  0.127804  0.188914 -0.0208636  -111.530    -5.568  
-2212 8 59921.00 I  0.125543 0.000022  0.188699 0.000018  I-0.0204734 0.0000057 -0.4404 0.0041  I  -111.365    0.846    -5.762    0.123  0.125550  0.188683 -0.0204842  -111.431    -5.765  
-2212 9 59922.00 I  0.123012 0.000021  0.188942 0.000018  I-0.0199675 0.0000060 -0.5715 0.0047  I  -111.344    0.846    -6.019    0.123  0.123051  0.188943 -0.0199575  -111.450    -5.997  
-221210 59923.00 I  0.120043 0.000019  0.189225 0.000015  I-0.0193441 0.0000075 -0.6617 0.0041  I  -111.356    0.679    -6.161    0.090  0.120023  0.189212 -0.0193465  -111.433    -6.148  
-221211 59924.00 I  0.117117 0.000024  0.189452 0.000023  I-0.0186822 0.0000056 -0.6376 0.0047  I  -111.266    0.747    -6.164    0.166  0.117059  0.189519 -0.0187186  -111.306    -6.171  
-221212 59925.00 I  0.114541 0.000023  0.189301 0.000023  I-0.0181000 0.0000057 -0.5202 0.0036  I  -111.037    0.747    -6.140    0.166  0.114474  0.189311 -0.0181257  -111.063    -6.164  
-221213 59926.00 I  0.112253 0.000019  0.189470 0.000023  I-0.0176358 0.0000045 -0.4209 0.0035  I  -110.703    0.861    -6.170    0.200  0.112235  0.189380 -0.0176371  -110.733    -6.213  
-221214 59927.00 I  0.110085 0.000019  0.189731 0.000022  I-0.0172744 0.0000042 -0.2729 0.0030  I  -110.284    0.861    -6.189    0.200  0.110057  0.189733 -0.0172887  -110.324    -6.215  
-221215 59928.00 I  0.107803 0.000020  0.190663 0.000022  I-0.0170970 0.0000039 -0.1039 0.0028  I  -109.840    0.861    -6.078    0.200  0.107848  0.190644 -0.0170929  -109.882    -6.084  
-221216 59929.00 I  0.105273 0.000020  0.191570 0.000022  I-0.0170756 0.0000038  0.0920 0.0032  I  -109.579    0.861    -5.849    0.200  0.105276  0.191662 -0.0170407  -109.642    -5.845  
-221217 59930.00 I  0.102628 0.000012  0.192140 0.000014  I-0.0172698 0.0000050  0.2544 0.0024  I  -109.724    0.909    -5.650    0.185  0.102588  0.192217 -0.0171383  -109.796    -5.644  
-221218 59931.00 I  0.100234 0.000028  0.192470 0.000032  I-0.0175335 0.0000029  0.2642 0.0029  I  -110.230    0.870    -5.565    0.145  0.100160  0.192490 -0.0173664  -110.291    -5.561  
-221219 59932.00 I  0.098290 0.000027  0.192738 0.000030  I-0.0177794 0.0000029  0.2176 0.0020  I  -110.790    0.836    -5.495    0.096  0.098210  0.192803 -0.0177187  -110.824    -5.496  
-221220 59933.00 I  0.096776 0.000032  0.193200 0.000033  I-0.0179621 0.0000027  0.1511 0.0021  I  -111.222    0.724    -5.338    0.100  0.096711  0.193084 -0.0179634  -111.212    -5.340  
-221221 59934.00 I  0.095784 0.000032  0.193309 0.000033  I-0.0180808 0.0000029  0.0821 0.0020  I  -111.621    0.724    -5.212    0.100  0.095777  0.193348 -0.0181234  -111.654    -5.239  
-221222 59935.00 I  0.094824 0.000032  0.194070 0.000034  I-0.0180953 0.0000029 -0.0800 0.0021  I  -112.006    0.724    -5.343    0.100  0.094877  0.193950 -0.0181060  -112.105    -5.394  
-221223 59936.00 I  0.093412 0.000033  0.194919 0.000034  I-0.0179113 0.0000031 -0.2707 0.0025  I  -112.108    0.724    -5.694    0.100  0.093472  0.194922 -0.0178955  -112.150    -5.759  
-221224 59937.00 I  0.091301 0.000022  0.196106 0.000018  I-0.0176045 0.0000040 -0.3096 0.0026  I  -111.756    0.564    -5.935    0.105  0.091397  0.196126 -0.0175841  -111.706    -6.007  
-221225 59938.00 I  0.088379 0.000022  0.197001 0.000018  I-0.0173382 0.0000041 -0.2103 0.0047  I  -111.221    0.564    -5.867    0.105  0.088402  0.197099 -0.0173115  -111.094    -5.943  
-221226 59939.00 I  0.085231 0.000044  0.197373 0.000036  I-0.0172380 0.0000086  0.0515 0.0046  I  -110.902    0.636    -5.663    0.134  0.085204  0.197391 -0.0172323  -110.709    -5.742  
-221227 59940.00 I  0.081994 0.000044  0.197755 0.000036  I-0.0174611 0.0000082  0.3732 0.0056  I  -110.867    0.636    -5.577    0.134  0.082060  0.197809 -0.0174541  -110.623    -5.660  
-221228 59941.00 I  0.078270 0.000046  0.198455 0.000037  I-0.0179249 0.0000071  0.5163 0.0054  I  -110.929    0.677    -5.586    0.138  0.078253  0.198379 -0.0179243  -110.647    -5.673  
-221229 59942.00 I  0.074738 0.000045  0.198550 0.000037  I-0.0184560 0.0000071  0.5464 0.0050  I  -110.989    0.677    -5.498    0.138  0.074744  0.198584 -0.0184719  -110.694    -5.570  
-221230 59943.00 I  0.071208 0.000045  0.199194 0.000037  I-0.0190009 0.0000071  0.5262 0.0051  I  -111.090    0.677    -5.286    0.138  0.071281  0.199199 -0.0190102  -110.793    -5.341  
-221231 59944.00 I  0.067041 0.000045  0.200093 0.000037  I-0.0194827 0.0000073  0.4288 0.0053  I  -111.251    0.677    -5.104    0.138  0.067074  0.200103 -0.0194855  -110.973    -5.182  
-23 1 1 59945.00 I  0.062785 0.000019  0.200912 0.000015  I-0.0198218 0.0000080  0.2211 0.0049  I  -111.416    0.730    -5.047    0.142  0.062699  0.200944 -0.0197967  -111.162    -5.163  
-23 1 2 59946.00 I  0.059055 0.000026  0.201762 0.000023  I-0.0199203 0.0000065 -0.0006 0.0058  I  -111.505    0.621    -5.057    0.096  0.059003  0.201796 -0.0199243  -111.443    -5.114  
-23 1 3 59947.00 I  0.055737 0.000027  0.202450 0.000033  I-0.0198267 0.0000083 -0.2042 0.0054  I  -111.438    0.659    -5.073    0.126  0.055638  0.202514 -0.0198250  -111.467    -5.128  
-23 1 4 59948.00 I  0.052972 0.000026  0.203064 0.000034  I-0.0195071 0.0000087 -0.4223 0.0063  I  -111.185    0.659    -5.151    0.126  0.052933  0.202990 -0.0195007  -111.313    -5.194  
-23 1 5 59949.00 I  0.050800 0.000027  0.203922 0.000034  I-0.0190229 0.0000095 -0.5179 0.0064  I  -110.842    0.659    -5.367    0.126  0.050795  0.203830 -0.0190232  -110.822    -5.531  
-23 1 6 59950.00 I  0.048797 0.000027  0.205049 0.000034  I-0.0184927 0.0000095 -0.5492 0.0066  I  -110.575    0.659    -5.652    0.126  0.048795  0.205101 -0.0184663  -110.510    -5.834  
-23 1 7 59951.00 I  0.046881 0.000026  0.206245 0.000034  I-0.0179427 0.0000093 -0.5259 0.0066  I  -110.448    0.659    -5.834    0.126  0.046853  0.206221 -0.0179143  -110.392    -5.984  
-23 1 8 59952.00 I  0.045143 0.000025  0.207582 0.000033  I-0.0174730 0.0000091 -0.4062 0.0062  I  -110.370    0.873    -5.828    0.183  0.045146  0.207590 -0.0174487  -110.316    -5.948  
-23 1 9 59953.00 I  0.043365 0.000018  0.209037 0.000021  I-0.0171385 0.0000082 -0.2617 0.0060  I  -110.219    0.866    -5.728    0.162  0.043370  0.209111 -0.0171274  -110.159    -5.821  
-23 110 59954.00 I  0.041291 0.000017  0.210318 0.000019  I-0.0169603 0.0000077 -0.0849 0.0055  I  -109.953    0.866    -5.662    0.162  0.041325  0.210288 -0.0169671  -109.874    -5.733  
-23 111 59955.00 I  0.038966 0.000025  0.211076 0.000021  I-0.0169675 0.0000073  0.0884 0.0050  I  -109.602    0.831    -5.626    0.138  0.038979  0.211134 -0.0169747  -109.583    -5.665  
-23 112 59956.00 I  0.036562 0.000024  0.211937 0.000020  I-0.0170926 0.0000064  0.1281 0.0050  I  -109.241    0.831    -5.526    0.138  0.036547  0.211915 -0.0170559  -109.296    -5.533  
-23 113 59957.00 I  0.034177 0.000024  0.213072 0.000020  I-0.0172135 0.0000069  0.1371 0.0064  I  -109.019    0.831    -5.366    0.138  0.034173  0.213022 -0.0172046  -109.147    -5.343  
-23 114 59958.00 I  0.031794 0.000019  0.214404 0.000013  I-0.0173724 0.0000112  0.1630 0.0058  I  -109.098    0.749    -5.298    0.079  0.031810  0.214393 -0.0173877  -109.253    -5.273  
-23 115 59959.00 I  0.029348 0.000027  0.216085 0.000025  I-0.0175381 0.0000094  0.1848 0.0074  I  -109.453    0.765    -5.412    0.122  0.029351  0.216047 -0.0175710  -109.621    -5.396  
-23 116 59960.00 I  0.026874 0.000027  0.217932 0.000026  I-0.0177154 0.0000098  0.1268 0.0073  I  -109.862    0.765    -5.571    0.122  0.026882  0.217923 -0.0177110  -110.037    -5.563  
-23 117 59961.00 I  0.024325 0.000021  0.220321 0.000024  I-0.0177447 0.0000113 -0.0721 0.0066  I  -110.227    0.772    -5.561    0.141  0.024343  0.220214 -0.0177400  -110.403    -5.564  
-23 118 59962.00 I  0.021690 0.000044  0.222404 0.000023  I-0.0175737 0.0000089 -0.2636 0.0071  I  -110.731    0.782    -5.436    0.127  0.021681  0.222504 -0.0175873  -110.857    -5.445  
-23 119 59963.00 I  0.019115 0.000044  0.224223 0.000023  I-0.0172335 0.0000087 -0.4072 0.0062  I  -111.419    0.782    -5.500    0.127  0.019078  0.224261 -0.0172362  -111.474    -5.516  
-23 120 59964.00 I  0.016659 0.000045  0.225643 0.000023  I-0.0167603 0.0000085 -0.5477 0.0068  I  -111.874    0.782    -5.863    0.127  0.016715  0.225678 -0.0167521  -111.849    -5.887  
-23 121 59965.00 I  0.013979 0.000041  0.226843 0.000009  I-0.0161645 0.0000104 -0.6089 0.0051  I  -111.665    0.801    -6.213    0.103  0.014033  0.226892 -0.0161896  -111.635    -6.235  
-23 122 59966.00 I  0.010876 0.000043  0.227751 0.000011  I-0.0156072 0.0000057 -0.4759 0.0058  I  -110.964    0.577    -6.218    0.090  0.010879  0.227740 -0.0156593  -110.964    -6.230  
-23 123 59967.00 I  0.007811 0.000043  0.228849 0.000013  I-0.0152578 0.0000053 -0.2077 0.0040  I  -110.347    0.577    -5.974    0.090  0.007728  0.228830 -0.0153087  -110.393    -5.970  
-23 124 59968.00 I  0.005404 0.000022  0.230244 0.000015  I-0.0152021 0.0000056  0.0913 0.0035  I  -110.105    0.434    -5.812    0.081  0.005300  0.230244 -0.0152158  -110.223    -5.787  
-23 125 59969.00 I  0.003919 0.000026  0.231443 0.000024  I-0.0154039 0.0000046  0.2806 0.0036  I  -110.109    0.579    -5.809    0.163  0.003852  0.231401 -0.0153642  -110.193    -5.799  
-23 126 59970.00 I  0.002890 0.000027  0.233310 0.000026  I-0.0156939 0.0000046  0.2616 0.0032  I  -110.224    0.579    -5.762    0.163  0.002927  0.233231 -0.0156349  -110.268    -5.775  
-23 127 59971.00 I  0.001577 0.000026  0.235926 0.000027  I-0.0158984 0.0000044  0.1565 0.0038  I  -110.442    0.579    -5.597    0.163  0.001593  0.235918 -0.0158886  -110.468    -5.635  
-23 128 59972.00 I  0.000380 0.000022  0.238091 0.000027  I-0.0159846 0.0000060 -0.0156 0.0036  I  -110.698    0.725    -5.506    0.211  0.000279  0.238107 -0.0159862  -110.687    -5.537  
-23 129 59973.00 I -0.000271 0.000025  0.240389 0.000028  I-0.0158766 0.0000057 -0.1596 0.0039  I  -110.853    0.856    -5.641    0.196 -0.000230  0.240378 -0.0158927  -110.794    -5.657  
-23 130 59974.00 I -0.000861 0.000024  0.242664 0.000028  I-0.0156634 0.0000050 -0.3098 0.0055  I  -110.868    0.856    -5.898    0.196 -0.000925  0.242670 -0.0156444  -110.750    -5.905  
-23 131 59975.00 I -0.001399 0.000020  0.244993 0.000021  I-0.0152294 0.0000094 -0.5429 0.0049  I  -110.779    1.181    -6.079    0.157 -0.001326  0.244961 -0.0152262  -110.583    -6.080  
-23 2 1 59976.00 I -0.002309 0.000021  0.247832 0.000039  I-0.0146104 0.0000084 -0.6778 0.0063  I  -110.583    1.099    -6.154    0.172 -0.002296  0.247864 -0.0146010  -110.444    -6.163  
-23 2 2 59977.00 I -0.003561 0.000021  0.250285 0.000039  I-0.0138920 0.0000084 -0.7582 0.0059  I  -110.280    1.099    -6.242    0.172                                                     
-23 2 3 59978.00 I -0.004906 0.000021  0.252583 0.000039  I-0.0131166 0.0000084 -0.7708 0.0062  I  -109.983    1.099    -6.393    0.172                                                     
-23 2 4 59979.00 I -0.006471 0.000019  0.254237 0.000039  I-0.0123988 0.0000091 -0.6382 0.0049  I  -109.828    1.013    -6.494    0.185                                                     
-23 2 5 59980.00 I -0.008210 0.000022  0.255949 0.000039  I-0.0118614 0.0000052 -0.4421 0.0052  I  -109.805    0.774    -6.423    0.152                                                     
-23 2 6 59981.00 I -0.009960 0.000022  0.257720 0.000039  I-0.0114986 0.0000052 -0.2940 0.0034  I  -109.768    0.774    -6.219    0.152                                                     
-23 2 7 59982.00 I -0.011917 0.000021  0.259705 0.000017  I-0.0112742 0.0000043 -0.1436 0.0033  I  -109.608    0.657    -6.037    0.129                                                     
-23 2 8 59983.00 I -0.014093 0.000034  0.261632 0.000036  I-0.0112016 0.0000042 -0.0227 0.0030  I  -109.356    0.750    -5.959    0.103                                                     
-23 2 9 59984.00 I -0.015724 0.000034  0.263431 0.000035  I-0.0112376 0.0000041  0.1246 0.0030  I  -109.134    0.750    -5.939    0.103                                                     
-23 210 59985.00 I -0.016729 0.000034  0.265667 0.000036  I-0.0114593 0.0000043  0.2974 0.0042  I  -109.041    0.750    -5.922    0.103                                                     
-23 211 59986.00 I -0.017892 0.000030  0.267965 0.000034  I-0.0117914 0.0000074  0.3472 0.0033  I  -109.120    0.917    -5.960    0.043                                                     
-23 212 59987.00 I -0.019635 0.000032  0.270446 0.000035  I-0.0121214 0.0000051  0.3000 0.0044  I  -109.324    0.870    -6.124    0.125                                                     
-23 213 59988.00 I -0.021942 0.000033  0.273074 0.000037  I-0.0123682 0.0000049  0.1832 0.0036  I  -109.526    0.870    -6.349    0.125                                                     
-23 214 59989.00 I -0.024488 0.000019  0.275745 0.000020  I-0.0124643 0.0000050 -0.0043 0.0037  I  -109.671    0.834    -6.476    0.162                                                     
-23 215 59990.00 I -0.026965 0.000029  0.278156 0.000022  I-0.0123530 0.0000055 -0.2118 0.0036  I  -109.897    0.787    -6.485    0.157                                                     
-23 216 59991.00 I -0.029371 0.000029  0.280696 0.000022  I-0.0120637 0.0000053 -0.3504 0.0038  I  -110.308    0.787    -6.575    0.157                                                     
-23 217 59992.00 I -0.031758 0.000029  0.282901 0.000024  I-0.0116875 0.0000052 -0.3829 0.0049  I  -110.665    0.787    -6.879    0.157                                                     
-23 218 59993.00 I -0.033991 0.000024  0.284840 0.000023  I-0.0113639 0.0000083 -0.2172 0.0040  I  -110.582    0.461    -7.209    0.132                                                     
-23 219 59994.00 I -0.035823 0.000035  0.286852 0.000026  I-0.0113035 0.0000061  0.0997 0.0052  I  -110.035    0.806    -7.269    0.232                                                     
-23 220 59995.00 I -0.037241 0.000034  0.288944 0.000025  I-0.0115703 0.0000061  0.4378 0.0042  I  -109.414    0.806    -7.063    0.232                                                     
-23 221 59996.00 I -0.038252 0.000026  0.291554 0.000023  I-0.0121576 0.0000058  0.7116 0.0040  I  -109.046    0.826    -6.870    0.244                                                     
-23 222 59997.00 I -0.038779 0.000031  0.294587 0.000023  I-0.0129265 0.0000053  0.7844 0.0041  I  -108.959    0.820    -6.834    0.218                                                     
-23 223 59998.00 I -0.038963 0.000032  0.298258 0.000021  I-0.0137037 0.0000057  0.7892 0.0042  I  -109.085    0.820    -6.826    0.218                                                     
-23 224 59999.00 I -0.039169 0.000033  0.301880 0.000020  I-0.0144905 0.0000064  0.7510 0.0054  I  -109.393    0.820    -6.749    0.218                                                     
-23 225 60000.00 I -0.039675 0.000022  0.305084 0.000010  I-0.0151479 0.0000091  0.5395 0.0050  I  -109.758    0.761    -6.738    0.065                                                     
-23 226 60001.00 I -0.040937 0.000025  0.308181 0.000012  I-0.0155312 0.0000076  0.2133 0.0059  I  -109.980    0.864    -6.938    0.047                                                     
-23 227 60002.00 I -0.042707 0.000025  0.310711 0.000012  I-0.0156026 0.0000074 -0.0284 0.0059  I  -109.998    0.864    -7.258    0.047                                                     
-23 228 60003.00 I -0.044027 0.000019  0.313341 0.000010  I-0.0155053 0.0000090 -0.1773 0.0053  I  -109.887    0.924    -7.471    0.027                                                     
-23 3 1 60004.00 I -0.045093 0.000020  0.316292 0.000018  I-0.0152896 0.0000076 -0.2013 0.0056  I  -109.672    0.924    -7.496    0.027                                                     
-23 3 2 60005.00 I -0.046060 0.000020  0.318731 0.000019  I-0.0151046 0.0000068 -0.2196 0.0051  I  -109.305    0.924    -7.463    0.027                                                     
-23 3 3 60006.00 I -0.046664 0.000018  0.321152 0.000019  I-0.0148508 0.0000069 -0.2368 0.0061  I  -108.857    0.924    -7.504    0.027                                                     
-23 3 4 60007.00 I -0.046921 0.000015  0.323781 0.000020  I-0.0146829 0.0000102 -0.0982 0.0051  I  -108.521    0.322    -7.577    0.160                                                     
-23 3 5 60008.00 I -0.046595 0.000038  0.326597 0.000022  I-0.0146855 0.0000076  0.1337 0.0062  I  -108.407    0.943    -7.539    0.052                                                     
-23 3 6 60009.00 I -0.045654 0.000038  0.329761 0.000022  I-0.0149448 0.0000072  0.3491 0.0054  I  -108.414    0.943    -7.349    0.052                                                     
-23 3 7 60010.00 I -0.044610 0.000036  0.333355 0.000016  I-0.0153706 0.0000078  0.5251 0.0050  I  -108.385    0.943    -7.132    0.052                                                     
-23 3 8 60011.00 I -0.043512 0.000039  0.336613 0.000015  I-0.0159988 0.0000070  0.7125 0.0052  I  -108.301    0.916    -7.037    0.051                                                     
-23 3 9 60012.00 I -0.042352 0.000039  0.339813 0.000014  I-0.0167717 0.0000068  0.8282 0.0045  I  -108.258    0.916    -7.092    0.051                                                     
-23 310 60013.00 I -0.041307 0.000042  0.343088 0.000014  I-0.0176165 0.0000056  0.8277 0.0043  I  -108.313    0.916    -7.216    0.051                                                     
-23 311 60014.00 I -0.040753 0.000021  0.346408 0.000010  I-0.0184001 0.0000053  0.7461 0.0041  I  -108.424    0.853    -7.342    0.049                                                     
-23 312 60015.00 I -0.040508 0.000024  0.349531 0.000013  I-0.0190888 0.0000060  0.6049 0.0040  I  -108.525    0.914    -7.467    0.059                                                     
-23 313 60016.00 I -0.040071 0.000027  0.352565 0.000014  I-0.0195856 0.0000060  0.3909 0.0046  I  -108.580    0.914    -7.604    0.059                                                     
-23 314 60017.00 I -0.039712 0.000022  0.356013 0.000016  I-0.0198997 0.0000069  0.2642 0.0048  I  -108.558    0.975    -7.736    0.067                                                     
-23 315 60018.00 I -0.039666 0.000025  0.359413 0.000019  I-0.0200943 0.0000074  0.0785 0.0052  I  -108.455    0.975    -7.850    0.067                                                     
-23 316 60019.00 I -0.039787 0.000024  0.362290 0.000019  I-0.0200729 0.0000079 -0.0585 0.0055  I  -108.301    0.975    -7.989    0.067                                                     
-23 317 60020.00 I -0.039643 0.000022  0.364626 0.000020  I-0.0200420 0.0000081 -0.0014 0.0062  P  -108.177    0.278    -8.167    0.145                                                     
-23 318 60021.00 I -0.039037 0.000019  0.366856 0.000012  I-0.0201168 0.0000095  0.1959 0.0062  P  -108.066    0.288    -8.292    0.148                                                     
-23 319 60022.00 I -0.038084 0.000091  0.369004 0.000091  I-0.0204769 0.0000094  0.5226 0.0074  P  -107.967    0.297    -8.241    0.151                                                     
-23 320 60023.00 I -0.036882 0.000091  0.371270 0.000091  I-0.0211387 0.0000113  0.7792 0.0070  P  -107.927    0.304    -8.041    0.154                                                     
-23 321 60024.00 I -0.035468 0.000092  0.373949 0.000091  I-0.0219984 0.0000105  0.9249 0.0080  P  -107.965    0.309    -7.867    0.155                                                     
-23 322 60025.00 I -0.033934 0.000091  0.377079 0.000091  I-0.0229498 0.0000113  0.9545 0.0080  P  -108.051    0.313    -7.833    0.157                                                     
-23 323 60026.00 I -0.032488 0.000091  0.380234 0.000090  I-0.0238725 0.0000122  0.8795 0.0088  P  -108.199    0.316    -7.877    0.158                                                     
-23 324 60027.00 I -0.031160 0.000091  0.383304 0.000091  I-0.0246722 0.0000136  0.6948 0.0088  P  -108.455    0.318    -7.917    0.158                                                     
-23 325 60028.00 I -0.029845 0.000091  0.386413 0.000091  I-0.0252185 0.0000127  0.3792 0.0093  P  -108.763    0.319    -7.996    0.159                                                     
-23 326 60029.00 I -0.028351 0.000091  0.389518 0.000091  I-0.0254306 0.0000127  0.0635 0.0086  P  -108.967    0.320    -8.191    0.159                                                     
-23 327 60030.00 I -0.026565 0.000090  0.392645 0.000091  I-0.0253814 0.0000117 -0.1445 0.0087  P  -108.982    0.321    -8.441    0.160                                                     
-23 328 60031.00 I -0.024691 0.000091  0.395441 0.000091  I-0.0251694 0.0000118 -0.2690 0.0081  P  -108.844    0.321    -8.593    0.160                                                     
-23 329 60032.00 I -0.023033 0.000090  0.397906 0.000091  I-0.0248763 0.0000111 -0.2947 0.0078  P  -108.579    0.321    -8.590    0.160                                                     
-23 330 60033.00 I -0.021728 0.000090  0.400145 0.000090  I-0.0245876 0.0000102                 P  -108.155    0.321    -8.550    0.160                                                     
-23 331 60034.00 P -0.020328 0.000632  0.402343 0.000402  P-0.0243815 0.0001080                 P  -107.624    0.322    -8.602    0.160                                                     
-23 4 1 60035.00 P -0.019069 0.000938  0.404490 0.000663  P-0.0243045 0.0002041                 P  -107.189    0.322    -8.726    0.160                                                     
-23 4 2 60036.00 P -0.017744 0.001182  0.406627 0.000887  P-0.0243797 0.0003028                 P  -107.039    0.322    -8.770    0.160                                                     
-23 4 3 60037.00 P -0.016366 0.001392  0.408824 0.001092  P-0.0246181 0.0004021                 P  -107.156    0.322    -8.635    0.160                                                     
-23 4 4 60038.00 P -0.014956 0.001581  0.411084 0.001282  P-0.0250215 0.0005017                 P  -107.364    0.322    -8.393    0.160                                                     
-23 4 5 60039.00 P -0.013504 0.001754  0.413424 0.001462  P-0.0255725 0.0006014                 P  -107.530    0.322    -8.216    0.160                                                     
-23 4 6 60040.00 P -0.012020 0.001915  0.415790 0.001633  P-0.0262092 0.0007012                 P  -107.654    0.322    -8.211    0.160                                                     
-23 4 7 60041.00 P -0.010486 0.002067  0.418145 0.001798  P-0.0268385 0.0007500                 P  -107.784    0.322    -8.346    0.160                                                     
-23 4 8 60042.00 P -0.008915 0.002210  0.420466 0.001957  P-0.0273638 0.0005500                 P  -107.923    0.322    -8.516    0.160                                                     
-23 4 9 60043.00 P -0.007308 0.002347  0.422744 0.002112  P-0.0277033 0.0007548                 P  -108.046    0.322    -8.653    0.160                                                     
-23 410 60044.00 P -0.005666 0.002478  0.424993 0.002262  P-0.0278329 0.0009344                 P  -108.128    0.322    -8.763    0.160                                                     
-23 411 60045.00 P -0.003996 0.002604  0.427203 0.002408  P-0.0277760 0.0010994                 P  -108.115    0.322    -8.885    0.160                                                     
-23 412 60046.00 P -0.002298 0.002726  0.429377 0.002551  P-0.0275815 0.0012543                 P  -107.916    0.322    -9.039    0.160                                                     
-23 413 60047.00 P -0.000575 0.002843  0.431513 0.002690  P-0.0273482 0.0014016                 P  -107.493    0.322    -9.199    0.160                                                     
-23 414 60048.00 P  0.001177 0.002957  0.433618 0.002827  P-0.0272123 0.0015429                 P  -106.961    0.322    -9.308    0.160                                                     
-23 415 60049.00 P  0.002959 0.003068  0.435695 0.002962  P-0.0272968 0.0016792                 P  -106.542    0.322    -9.311    0.160                                                     
-23 416 60050.00 P  0.004774 0.003176  0.437746 0.003094  P-0.0276587 0.0018113                 P  -106.405    0.322    -9.196    0.160                                                     
-23 417 60051.00 P  0.006625 0.003281  0.439775 0.003224  P-0.0283032 0.0019399                 P  -106.544    0.322    -9.016    0.160                                                     
-23 418 60052.00 P  0.008508 0.003384  0.441781 0.003352  P-0.0291458 0.0020652                 P  -106.800    0.322    -8.859    0.160                                                     
-23 419 60053.00 P  0.010423 0.003484  0.443762 0.003478  P-0.0300608 0.0021877                 P  -107.013    0.322    -8.779    0.160                                                     
-23 420 60054.00 P  0.012368 0.003582  0.445717 0.003602  P-0.0309027 0.0023077                 P  -107.144    0.322    -8.770    0.160                                                     
-23 421 60055.00 P  0.014345 0.003679  0.447642 0.003725  P-0.0315476 0.0024255                 P  -107.254    0.322    -8.813    0.160                                                     
-23 422 60056.00 P  0.016351 0.003773  0.449537 0.003846  P-0.0319355 0.0025411                 P  -107.392    0.322    -8.920    0.160                                                     
-23 423 60057.00 P  0.018388 0.003866  0.451401 0.003966  P-0.0320641 0.0026548                 P  -107.526    0.322    -9.089    0.160                                                     
-23 424 60058.00 P  0.020453 0.003957  0.453232 0.004084  P-0.0319798 0.0027668                 P  -107.588    0.322    -9.256    0.160                                                     
-23 425 60059.00 P  0.022548 0.004046  0.455029 0.004201  P-0.0317505 0.0028772                 P  -107.537    0.322    -9.341    0.160                                                     
-23 426 60060.00 P  0.024671 0.004134  0.456794 0.004317  P-0.0314645 0.0029860                 P  -107.353    0.322    -9.351    0.160                                                     
-23 427 60061.00 P  0.026821 0.004221  0.458526 0.004431  P-0.0311954 0.0030934                 P  -107.018    0.322    -9.389    0.160                                                     
-23 428 60062.00 P  0.028998 0.004306  0.460224 0.004545  P-0.0310158 0.0031995                 P  -106.567    0.322    -9.530    0.160                                                     
-23 429 60063.00 P  0.031202 0.004390  0.461889 0.004657  P-0.0309729 0.0033043                 P  -106.140    0.322    -9.719    0.160                                                     
-23 430 60064.00 P  0.033432 0.004473  0.463520 0.004768  P-0.0310918 0.0034080                 P  -105.934    0.322    -9.801    0.160                                                     
-23 5 1 60065.00 P  0.035687 0.004555  0.465117 0.004879  P-0.0313780 0.0035105                 P  -106.058    0.322    -9.680    0.160                                                     
-23 5 2 60066.00 P  0.037968 0.004635  0.466679 0.004988  P-0.0318057 0.0036120                 P  -106.436    0.322    -9.411    0.160                                                     
-23 5 3 60067.00 P  0.040272 0.004715  0.468207 0.005096  P-0.0323266 0.0037124                 P  -106.864    0.322    -9.145    0.160                                                     
-23 5 4 60068.00 P  0.042601 0.004793  0.469699 0.005204  P-0.0328644 0.0038119                 P  -107.185    0.322    -9.008    0.160                                                     
-23 5 5 60069.00 P  0.044952 0.004871  0.471155 0.005310  P-0.0333214 0.0039105                 P  -107.389    0.322    -9.030    0.160                                                     
-23 5 6 60070.00 P  0.047325 0.004948  0.472576 0.005416  P-0.0335999 0.0040082                 P  -107.568    0.322    -9.169    0.160                                                     
-23 5 7 60071.00 P  0.049720 0.005023  0.473960 0.005521  P-0.0336392 0.0041051                 P  -107.771    0.322    -9.367    0.160                                                     
-23 5 8 60072.00 P  0.052137 0.005098  0.475307 0.005626  P-0.0334394 0.0042012                 P  -107.920    0.322    -9.572    0.160                                                     
-23 5 9 60073.00 P  0.054573 0.005172  0.476617 0.005729  P-0.0330542 0.0042965                 P  -107.884    0.322    -9.740    0.160                                                     
-23 510 60074.00 P  0.057030 0.005246  0.477889 0.005832  P-0.0325904 0.0043911                 P  -107.610    0.322    -9.846    0.160                                                     
-23 511 60075.00 P  0.059506 0.005318  0.479124 0.005934  P-0.0321779 0.0044849                 P  -107.176    0.322    -9.889    0.160                                                     
-23 512 60076.00 P  0.062000 0.005390  0.480321 0.006035  P-0.0319248 0.0045781                 P  -106.735    0.322    -9.875    0.160                                                     
-23 513 60077.00 P  0.064511 0.005461  0.481479 0.006136  P-0.0318955 0.0046706                 P  -106.431    0.322    -9.806    0.160                                                     
-23 514 60078.00 P  0.067040 0.005532  0.482600 0.006236  P-0.0320960 0.0047625                 P  -106.341    0.322    -9.687    0.160                                                     
-23 515 60079.00 P  0.069585 0.005601  0.483681 0.006336  P-0.0324647 0.0048537                 P  -106.468    0.322    -9.531    0.160                                                     
-23 516 60080.00 P  0.072146 0.005670  0.484724 0.006434  P-0.0328981 0.0049444                 P  -106.743    0.322    -9.351    0.160                                                     
-23 517 60081.00 P  0.074722 0.005739  0.485727 0.006533  P-0.0332704 0.0050344                 P  -107.050    0.322    -9.174    0.160                                                     
-23 518 60082.00 P  0.077313 0.005807  0.486692 0.006630  P-0.0334638 0.0051240                 P  -107.269    0.322    -9.054    0.160                                                     
-23 519 60083.00 P  0.079916 0.005874  0.487616 0.006728  P-0.0334017 0.0052129                 P  -107.352    0.322    -9.061    0.160                                                     
-23 520 60084.00 P  0.082533 0.005941  0.488502 0.006824  P-0.0330674 0.0053014                 P  -107.355    0.322    -9.222    0.160                                                     
-23 521 60085.00 P  0.085162 0.006007  0.489347 0.006920  P-0.0324981 0.0053893                 P  -107.379    0.322    -9.471    0.160                                                     
-23 522 60086.00 P  0.087803 0.006072  0.490152 0.007016  P-0.0317587 0.0054768                 P  -107.461    0.322    -9.677    0.160                                                     
-23 523 60087.00 P  0.090454 0.006137  0.490917 0.007111  P-0.0309290 0.0055637                 P  -107.552    0.322    -9.754    0.160                                                     
-23 524 60088.00 P  0.093115 0.006202  0.491641 0.007205  P-0.0300902 0.0056502                 P  -107.581    0.322    -9.748    0.160                                                     
-23 525 60089.00 P  0.095786 0.006266  0.492325 0.007299  P-0.0293170 0.0057362                 P  -107.508    0.322    -9.780    0.160                                                     
-23 526 60090.00 P  0.098466 0.006329  0.492968 0.007393  P-0.0286675 0.0058218                 P  -107.312    0.322    -9.904    0.160                                                     
-23 527 60091.00 P  0.101153 0.006393  0.493571 0.007486  P-0.0281770 0.0059070                 P  -107.017    0.322   -10.030    0.160                                                     
-23 528 60092.00 P  0.103848 0.006455  0.494133 0.007579  P-0.0278594 0.0059917                 P  -106.763    0.322   -10.018    0.160                                                     
-23 529 60093.00 P  0.106549 0.006517  0.494654 0.007671  P-0.0276978 0.0060760                 P  -106.784    0.322    -9.825    0.160                                                     
-23 530 60094.00 P  0.109255 0.006579  0.495134 0.007763  P-0.0276510 0.0061599                 P  -107.211    0.322    -9.546    0.160                                                     
-23 531 60095.00 P  0.111967 0.006640  0.495573 0.007854  P-0.0276541 0.0062434                 P  -107.889    0.322    -9.304    0.160                                                     
-23 6 1 60096.00 P  0.114684 0.006701  0.495970 0.007946  P-0.0276163 0.0063266                 P  -108.498    0.322    -9.148    0.160                                                     
-23 6 2 60097.00 P  0.117404 0.006761  0.496327 0.008036  P-0.0274449 0.0064093                 P  -108.877    0.322    -9.082    0.160                                                     
-23 6 3 60098.00 P  0.120126 0.006821  0.496643 0.008126  P-0.0270623 0.0064917                 P  -109.134    0.322    -9.140    0.160                                                     
-23 6 4 60099.00 P  0.122851 0.006881  0.496917 0.008216  P-0.0264360 0.0065737                 P  -109.381    0.322    -9.359    0.160                                                     
-23 6 5 60100.00 P  0.125578 0.006940  0.497150 0.008306  P-0.0256000 0.0066554                 P  -109.512    0.322    -9.662    0.160                                                     
-23 6 6 60101.00 P  0.128305 0.006999  0.497341 0.008395  P-0.0246517 0.0067368                 P  -109.359    0.322    -9.875    0.160                                                     
-23 6 7 60102.00 P  0.131032 0.007058  0.497492 0.008483  P-0.0237260 0.0068177                 P  -108.978    0.322    -9.887    0.160                                                     
-23 6 8 60103.00 P  0.133759 0.007116  0.497601 0.008572  P-0.0229500 0.0068984                 P  -108.642    0.322    -9.755    0.160                                                     
-23 6 9 60104.00 P  0.136484 0.007174  0.497669 0.008660  P-0.0224032 0.0069788                 P  -108.551    0.322    -9.608    0.160                                                     
-23 610 60105.00 P  0.139206 0.007231  0.497696 0.008747  P-0.0220943 0.0070588                 P  -108.661    0.322    -9.507    0.160                                                     
-23 611 60106.00 P  0.141926 0.007288  0.497682 0.008835  P-0.0219634 0.0071385                 P  -108.809    0.322    -9.424    0.160                                                     
-23 612 60107.00 P  0.144643 0.007345  0.497627 0.008922  P-0.0219064 0.0072179                 P  -108.920    0.322    -9.315    0.160                                                     
-23 613 60108.00 P  0.147355 0.007401  0.497531 0.009008  P-0.0218041 0.0072970                 P  -109.070    0.322    -9.157    0.160                                                     
-23 614 60109.00 P  0.150062 0.007457  0.497394 0.009095  P-0.0215485 0.0073758                 P  -109.341    0.322    -8.969    0.160                                                     
-23 615 60110.00 P  0.152764 0.007513  0.497216 0.009181  P-0.0210649 0.0074544                                                                                                             
-23 616 60111.00 P  0.155459 0.007569  0.496998 0.009266  P-0.0203238 0.0075326                                                                                                             
-23 617 60112.00 P  0.158146 0.007624  0.496739 0.009352  P-0.0193416 0.0076106                                                                                                             
-23 618 60113.00 P  0.160827 0.007679  0.496440 0.009437  P-0.0181698 0.0076883                                                                                                             
-23 619 60114.00 P  0.163498 0.007733  0.496100 0.009522  P-0.0168833 0.0077657                                                                                                             
-23 620 60115.00 P  0.166160 0.007787  0.495721 0.009606  P-0.0155653 0.0078428                                                                                                             
-23 621 60116.00 P  0.168813 0.007841  0.495301 0.009690  P-0.0142968 0.0079197                                                                                                             
-23 622 60117.00 P  0.171455 0.007895  0.494841 0.009774  P-0.0131412 0.0079964                                                                                                             
-23 623 60118.00 P  0.174085 0.007949  0.494342 0.009858  P-0.0121406 0.0080728                                                                                                             
-23 624 60119.00 P  0.176704 0.008002  0.493804 0.009941  P-0.0113101 0.0081489                                                                                                             
-23 625 60120.00 P  0.179310 0.008055  0.493226 0.010024  P-0.0106351 0.0082248                                                                                                             
-23 626 60121.00 P  0.181902 0.008107  0.492609 0.010107  P-0.0100819 0.0083005                                                                                                             
-23 627 60122.00 P  0.184481 0.008160  0.491954 0.010190  P-0.0095985 0.0083759                                                                                                             
-23 628 60123.00 P  0.187045 0.008212  0.491259 0.010272  P-0.0091171 0.0084511                                                                                                             
-23 629 60124.00 P  0.189594 0.008264  0.490527 0.010354  P-0.0085582 0.0085261                                                                                                             
-23 630 60125.00 P  0.192126 0.008315  0.489756 0.010436  P-0.0078433 0.0086008                                                                                                             
-23 7 1 60126.00 P  0.194642 0.008367  0.488948 0.010517  P-0.0069197 0.0086754                                                                                                             
-23 7 2 60127.00 P  0.197141 0.008418  0.488102 0.010599  P-0.0057898 0.0087497                                                                                                             
-23 7 3 60128.00 P  0.199622 0.008469  0.487219 0.010680  P-0.0045226 0.0088237                                                                                                             
-23 7 4 60129.00 P  0.202085 0.008519  0.486298 0.010760  P-0.0032438 0.0088976                                                                                                             
-23 7 5 60130.00 P  0.204528 0.008570  0.485342 0.010841  P-0.0020990 0.0089713                                                                                                             
-23 7 6 60131.00 P  0.206951 0.008620  0.484348 0.010921  P-0.0011992 0.0090448                                                                                                             
-23 7 7 60132.00 P  0.209354 0.008670  0.483319 0.011002  P-0.0005764 0.0091180                                                                                                             
-23 7 8 60133.00 P  0.211736 0.008720  0.482254 0.011081  P-0.0001758 0.0091911                                                                                                             
-23 7 9 60134.00 P  0.214097 0.008770  0.481153 0.011161  P 0.0001189 0.0092639                                                                                                             
-23 710 60135.00 P  0.216437 0.008819  0.480018 0.011241  P 0.0004462 0.0093366                                                                                                             
-23 711 60136.00 P  0.218755 0.008868  0.478848 0.011320  P 0.0009277 0.0094091                                                                                                             
-23 712 60137.00 P  0.221049 0.008917  0.477644 0.011399  P 0.0016409 0.0094814                                                                                                             
-23 713 60138.00 P  0.223319 0.008966  0.476406 0.011478  P 0.0026146 0.0095535                                                                                                             
-23 714 60139.00 P  0.225564 0.009015  0.475135 0.011556  P 0.0038325 0.0096254                                                                                                             
-23 715 60140.00 P  0.227785 0.009063  0.473830 0.011635  P 0.0052436 0.0096971                                                                                                             
-23 716 60141.00 P  0.229980 0.009111  0.472492 0.011713  P 0.0067771 0.0097686                                                                                                             
-23 717 60142.00 P  0.232149 0.009159  0.471122 0.011791  P 0.0083633 0.0098400                                                                                                             
-23 718 60143.00 P  0.234291 0.009207  0.469720 0.011869  P 0.0099095 0.0099112                                                                                                             
-23 719 60144.00 P  0.236405 0.009254  0.468286 0.011946  P 0.0113483 0.0099822                                                                                                             
-23 720 60145.00 P  0.238492 0.009302  0.466821 0.012024  P 0.0126329 0.0100531                                                                                                             
-23 721 60146.00 P  0.240551 0.009349  0.465326 0.012101  P 0.0137415 0.0101238                                                                                                             
-23 722 60147.00 P  0.242581 0.009396  0.463800 0.012178  P 0.0146808 0.0101943                                                                                                             
-23 723 60148.00 P  0.244581 0.009443  0.462245 0.012255  P 0.0154818 0.0102646                                                                                                             
-23 724 60149.00 P  0.246552 0.009490  0.460660 0.012331  P 0.0161953 0.0103348                                                                                                             
-23 725 60150.00 P  0.248493 0.009536  0.459046 0.012408  P 0.0168844 0.0104048                                                                                                             
-23 726 60151.00 P  0.250402 0.009583  0.457404 0.012484  P 0.0176193 0.0104747                                                                                                             
-23 727 60152.00 P  0.252281 0.009629  0.455734 0.012560  P 0.0184697 0.0105444                                                                                                             
-23 728 60153.00 P  0.254128 0.009675  0.454036 0.012636  P 0.0194906 0.0106139                                                                                                             
-23 729 60154.00 P  0.255942 0.009721  0.452312 0.012712  P 0.0207004 0.0106833                                                                                                             
-23 730 60155.00 P  0.257725 0.009767  0.450561 0.012787  P 0.0220586 0.0107526                                                                                                             
-23 731 60156.00 P  0.259474 0.009812  0.448784 0.012863  P 0.0234605 0.0108216                                                                                                             
-23 8 1 60157.00 P  0.261190 0.009858  0.446982 0.012938  P 0.0247588 0.0108906                                                                                                             
-23 8 2 60158.00 P  0.262872 0.009903  0.445154 0.013013  P 0.0258128 0.0109594                                                                                                             
-23 8 3 60159.00 P  0.264520 0.009948  0.443303 0.013088  P 0.0265439 0.0110280                                                                                                             
-23 8 4 60160.00 P  0.266133 0.009993  0.441427 0.013162  P 0.0269703 0.0110965                                                                                                             
-23 8 5 60161.00 P  0.267712 0.010038  0.439529 0.013237  P 0.0272012 0.0111649                                                                                                             
-23 8 6 60162.00 P  0.269255 0.010082  0.437607 0.013311  P 0.0273963 0.0112331                                                                                                             
-23 8 7 60163.00 P  0.270762 0.010127  0.435663 0.013386  P 0.0277104 0.0113012                                                                                                             
-23 8 8 60164.00 P  0.272233 0.010171  0.433698 0.013460  P 0.0282509 0.0113691                                                                                                             
-23 8 9 60165.00 P  0.273668 0.010215  0.431712 0.013533  P 0.0290596 0.0114369                                                                                                             
-23 810 60166.00 P  0.275067 0.010259  0.429705 0.013607  P 0.0301205 0.0115046                                                                                                             
-23 811 60167.00 P  0.276428 0.010303  0.427678 0.013681  P 0.0313782 0.0115721                                                                                                             
-23 812 60168.00 P  0.277752 0.010347  0.425631 0.013754  P 0.0327573 0.0116395                                                                                                             
-23 813 60169.00 P  0.279038 0.010390  0.423566 0.013828  P 0.0341774 0.0117067                                                                                                             
-23 814 60170.00 P  0.280286 0.010434  0.421483 0.013901  P 0.0355602 0.0117739                                                                                                             
-23 815 60171.00 P  0.281497 0.010477  0.419381 0.013974  P 0.0368375 0.0118409                                                                                                             
-23 816 60172.00 P  0.282668 0.010520  0.417263 0.014046  P 0.0379578 0.0119077                                                                                                             
-23 817 60173.00 P  0.283801 0.010564  0.415129 0.014119  P 0.0388935 0.0119745                                                                                                             
-23 818 60174.00 P  0.284896 0.010607  0.412978 0.014192  P 0.0396445 0.0120411                                                                                                             
-23 819 60175.00 P  0.285950 0.010649  0.410812 0.014264  P 0.0402391 0.0121076                                                                                                             
-23 820 60176.00 P  0.286966 0.010692  0.408632 0.014336  P 0.0407274 0.0121740                                                                                                             
-23 821 60177.00 P  0.287942 0.010735  0.406437 0.014408  P 0.0411743 0.0122402                                                                                                             
-23 822 60178.00 P  0.288878 0.010777  0.404229 0.014480  P 0.0416499 0.0123063                                                                                                             
-23 823 60179.00 P  0.289774 0.010819  0.402008 0.014552  P 0.0422202 0.0123723                                                                                                             
-23 824 60180.00 P  0.290630 0.010861  0.399775 0.014624  P 0.0429366 0.0124382                                                                                                             
-23 825 60181.00 P  0.291446 0.010904  0.397531 0.014696  P 0.0438227 0.0125040                                                                                                             
-23 826 60182.00 P  0.292221 0.010945  0.395275 0.014767  P 0.0448575 0.0125696                                                                                                             
-23 827 60183.00 P  0.292955 0.010987  0.393009 0.014838  P 0.0459643 0.0126352                                                                                                             
-23 828 60184.00 P  0.293649 0.011029  0.390733 0.014909  P 0.0470154 0.0127006                                                                                                             
-23 829 60185.00 P  0.294302 0.011071  0.388448 0.014980  P 0.0478631 0.0127659                                                                                                             
-23 830 60186.00 P  0.294914 0.011112  0.386155 0.015051  P 0.0483904 0.0128311                                                                                                             
-23 831 60187.00 P  0.295485 0.011153  0.383854 0.015122  P 0.0485617 0.0128962                                                                                                             
-23 9 1 60188.00 P  0.296014 0.011195  0.381545 0.015193  P 0.0484432 0.0129612                                                                                                             
-23 9 2 60189.00 P  0.296503 0.011236  0.379230 0.015263  P 0.0481845 0.0130260                                                                                                             
-23 9 3 60190.00 P  0.296950 0.011277  0.376909 0.015334  P 0.0479657 0.0130908                                                                                                             
-23 9 4 60191.00 P  0.297355 0.011318  0.374583 0.015404  P 0.0479391 0.0131554                                                                                                             
-23 9 5 60192.00 P  0.297719 0.011358  0.372252 0.015474  P 0.0481878 0.0132199                                                                                                             
-23 9 6 60193.00 P  0.298042 0.011399  0.369917 0.015544  P 0.0487189 0.0132844                                                                                                             
-23 9 7 60194.00 P  0.298324 0.011440  0.367578 0.015614  P 0.0494804 0.0133487                                                                                                             
-23 9 8 60195.00 P  0.298563 0.011480  0.365237 0.015684  P 0.0503895 0.0134129                                                                                                             
-23 9 9 60196.00 P  0.298762 0.011520  0.362893 0.015753  P 0.0513555 0.0134770                                                                                                             
-23 910 60197.00 P  0.298919 0.011561  0.360548 0.015823  P 0.0522941 0.0135410                                                                                                             
-23 911 60198.00 P  0.299034 0.011601  0.358203 0.015892  P 0.0531333 0.0136050                                                                                                             
-23 912 60199.00 P  0.299108 0.011641  0.355856 0.015962  P 0.0538175 0.0136688                                                                                                             
-23 913 60200.00 P  0.299141 0.011681  0.353511 0.016031  P 0.0543130 0.0137325                                                                                                             
-23 914 60201.00 P  0.299133 0.011720  0.351166 0.016100  P 0.0546131 0.0137961                                                                                                             
-23 915 60202.00 P  0.299083 0.011760  0.348823 0.016169  P 0.0547391 0.0138596                                                                                                             
-23 916 60203.00 P  0.298992 0.011800  0.346482 0.016238  P 0.0547387 0.0139230                                                                                                             
-23 917 60204.00 P  0.298860 0.011839  0.344144 0.016306  P 0.0546784 0.0139863                                                                                                             
-23 918 60205.00 P  0.298688 0.011879  0.341810 0.016375  P 0.0546338 0.0140495                                                                                                             
-23 919 60206.00 P  0.298474 0.011918  0.339479 0.016443  P 0.0546769 0.0141127                                                                                                             
-23 920 60207.00 P  0.298220 0.011957  0.337154 0.016512  P 0.0548633 0.0141757                                                                                                             
-23 921 60208.00 P  0.297925 0.011996  0.334834 0.016580  P 0.0552192 0.0142386                                                                                                             
-23 922 60209.00 P  0.297590 0.012035  0.332520 0.016648  P 0.0557310 0.0143014                                                                                                             
-23 923 60210.00 P  0.297214 0.012074  0.330212 0.016716  P 0.0563370 0.0143642                                                                                                             
-23 924 60211.00 P  0.296799 0.012113  0.327912 0.016784  P 0.0569295 0.0144268                                                                                                             
-23 925 60212.00 P  0.296344 0.012152  0.325620 0.016852  P 0.0573734 0.0144894                                                                                                             
-23 926 60213.00 P  0.295849 0.012191  0.323336 0.016920  P 0.0575398 0.0145519                                                                                                             
-23 927 60214.00 P  0.295314 0.012229  0.321061 0.016987  P 0.0573522 0.0146142                                                                                                             
-23 928 60215.00 P  0.294741 0.012268  0.318795 0.017055  P 0.0568209 0.0146765                                                                                                             
-23 929 60216.00 P  0.294128 0.012306  0.316540 0.017122  P 0.0560498 0.0147387                                                                                                             
-23 930 60217.00 P  0.293476 0.012344  0.314296 0.017190  P 0.0552066 0.0148008                                                                                                             
-2310 1 60218.00 P  0.292786 0.012382  0.312063 0.017257  P 0.0544678 0.0148629                                                                                                             
-2310 2 60219.00 P  0.292058 0.012421  0.309843 0.017324  P 0.0539626 0.0149248                                                                                                             
-2310 3 60220.00 P  0.291291 0.012459  0.307635 0.017391  P 0.0537418 0.0149867                                                                                                             
-2310 4 60221.00 P  0.290487 0.012496  0.305440 0.017458  P 0.0537793 0.0150484                                                                                                             
-2310 5 60222.00 P  0.289645 0.012534  0.303258 0.017525  P 0.0539979 0.0151101                                                                                                             
-2310 6 60223.00 P  0.288766 0.012572  0.301091 0.017591  P 0.0543017 0.0151717                                                                                                             
-2310 7 60224.00 P  0.287851 0.012610  0.298939 0.017658  P 0.0545995 0.0152332                                                                                                             
-2310 8 60225.00 P  0.286898 0.012647  0.296803 0.017724  P 0.0548174 0.0152946                                                                                                             
-2310 9 60226.00 P  0.285910 0.012685  0.294682 0.017791  P 0.0549031 0.0153560                                                                                                             
-231010 60227.00 P  0.284885 0.012722  0.292578 0.017857  P 0.0548288 0.0154172                                                                                                             
-231011 60228.00 P  0.283825 0.012760  0.290491 0.017923  P 0.0545923 0.0154784                                                                                                             
-231012 60229.00 P  0.282730 0.012797  0.288422 0.017990  P 0.0542184 0.0155395                                                                                                             
-231013 60230.00 P  0.281600 0.012834  0.286371 0.018056  P 0.0537557 0.0156005                                                                                                             
-231014 60231.00 P  0.280435 0.012871  0.284338 0.018122  P 0.0532722 0.0156614                                                                                                             
-231015 60232.00 P  0.279237 0.012908  0.282325 0.018187  P 0.0528471 0.0157223                                                                                                             
-231016 60233.00 P  0.278004 0.012945  0.280331 0.018253  P 0.0525590 0.0157831                                                                                                             
-231017 60234.00 P  0.276739 0.012982  0.278358 0.018319  P 0.0524701 0.0158438                                                                                                             
-231018 60235.00 P  0.275440 0.013019  0.276405 0.018384  P 0.0526096 0.0159044                                                                                                             
-231019 60236.00 P  0.274109 0.013055  0.274473 0.018450  P 0.0529618 0.0159649                                                                                                             
-231020 60237.00 P  0.272746 0.013092  0.272564 0.018515  P 0.0534630 0.0160254                                                                                                             
-231021 60238.00 P  0.271352 0.013129  0.270676 0.018581  P 0.0540085 0.0160858                                                                                                             
-231022 60239.00 P  0.269926 0.013165  0.268811 0.018646  P 0.0544691 0.0161461                                                                                                             
-231023 60240.00 P  0.268469 0.013201  0.266969 0.018711  P 0.0547161 0.0162063                                                                                                             
-231024 60241.00 P  0.266983 0.013238  0.265151 0.018776  P 0.0546528 0.0162665                                                                                                             
-231025 60242.00 P  0.265466 0.013274  0.263357 0.018841  P 0.0542464 0.0163265                                                                                                             
-231026 60243.00 P  0.263920 0.013310  0.261587 0.018906  P 0.0535463 0.0163866                                                                                                             
-231027 60244.00 P  0.262345 0.013346  0.259842 0.018971  P 0.0526787 0.0164465                                                                                                             
-231028 60245.00 P  0.260742 0.013382  0.258123 0.019035  P 0.0518105 0.0165063                                                                                                             
-231029 60246.00 P  0.259111 0.013418  0.256429 0.019100  P 0.0510984 0.0165661                                                                                                             
-231030 60247.00 P  0.257453 0.013454  0.254762 0.019164  P 0.0506420 0.0166258                                                                                                             
-231031 60248.00 P  0.255767 0.013490  0.253121 0.019229  P 0.0504628 0.0166855                                                                                                             
-2311 1 60249.00 P  0.254056 0.013526  0.251507 0.019293  P 0.0505165 0.0167451                                                                                                             
-2311 2 60250.00 P  0.252318 0.013561  0.249921 0.019357  P 0.0507203 0.0168046                                                                                                             
-2311 3 60251.00 P  0.250555 0.013597  0.248362 0.019422  P 0.0509764 0.0168640                                                                                                             
-2311 4 60252.00 P  0.248768 0.013632  0.246832 0.019486  P 0.0511873 0.0169233                                                                                                             
-2311 5 60253.00 P  0.246956 0.013668  0.245330 0.019550  P 0.0512771 0.0169826                                                                                                             
-2311 6 60254.00 P  0.245120 0.013703  0.243857 0.019614  P 0.0512116 0.0170419                                                                                                             
-2311 7 60255.00 P  0.243262 0.013738  0.242413 0.019678  P 0.0509708 0.0171010                                                                                                             
-2311 8 60256.00 P  0.241381 0.013774  0.240999 0.019741  P 0.0505782 0.0171601                                                                                                             
-2311 9 60257.00 P  0.239477 0.013809  0.239615 0.019805  P 0.0500653 0.0172191                                                                                                             
-231110 60258.00 P  0.237553 0.013844  0.238261 0.019869  P 0.0494916 0.0172780                                                                                                             
-231111 60259.00 P  0.235607 0.013879  0.236937 0.019932  P 0.0489388 0.0173369                                                                                                             
-231112 60260.00 P  0.233641 0.013914  0.235645 0.019996  P 0.0485036 0.0173957                                                                                                             
-231113 60261.00 P  0.231656 0.013949  0.234384 0.020059  P 0.0482618 0.0174545                                                                                                             
-231114 60262.00 P  0.229651 0.013984  0.233154 0.020122  P 0.0482924 0.0175131                                                                                                             
-231115 60263.00 P  0.227628 0.014019  0.231955 0.020186  P 0.0485563 0.0175718                                                                                                             
-231116 60264.00 P  0.225587 0.014053  0.230789 0.020249  P 0.0490282 0.0176303                                                                                                             
-231117 60265.00 P  0.223529 0.014088  0.229655 0.020312  P 0.0495574 0.0176888                                                                                                             
-231118 60266.00 P  0.221453 0.014122  0.228554 0.020375  P 0.0500460 0.0177472                                                                                                             
-231119 60267.00 P  0.219362 0.014157  0.227486 0.020438  P 0.0503385 0.0178055                                                                                                             
-231120 60268.00 P  0.217255 0.014191  0.226450 0.020501  P 0.0503187 0.0178638                                                                                                             
-231121 60269.00 P  0.215134 0.014226  0.225448 0.020563  P 0.0501147 0.0179220                                                                                                             
-231122 60270.00 P  0.212998 0.014260  0.224479 0.020626  P 0.0497002 0.0179802                                                                                                             
-231123 60271.00 P  0.210848 0.014294  0.223544 0.020689  P 0.0492021 0.0180383                                                                                                             
-231124 60272.00 P  0.208686 0.014329  0.222642 0.020751  P 0.0486819 0.0180963                                                                                                             
-231125 60273.00 P  0.206511 0.014363  0.221775 0.020814  P 0.0483208 0.0181543                                                                                                             
-231126 60274.00 P  0.204324 0.014397  0.220942 0.020876  P 0.0481401 0.0182122                                                                                                             
-231127 60275.00 P  0.202126 0.014431  0.220143 0.020938  P 0.0482268 0.0182700                                                                                                             
-231128 60276.00 P  0.199918 0.014465  0.219379 0.021001  P 0.0485402 0.0183278                                                                                                             
-231129 60277.00 P  0.197699 0.014499  0.218649 0.021063  P 0.0489747 0.0183855                                                                                                             
-231130 60278.00 P  0.195472 0.014533  0.217955 0.021125  P 0.0494227 0.0184432                                                                                                             
-2312 1 60279.00 P  0.193236 0.014566  0.217295 0.021187  P 0.0498048 0.0185008                                                                                                             
-2312 2 60280.00 P  0.190992 0.014600  0.216670 0.021249  P 0.0500445 0.0185583                                                                                                             
-2312 3 60281.00 P  0.188741 0.014634  0.216080 0.021311  P 0.0501621 0.0186158                                                                                                             
-2312 4 60282.00 P  0.186483 0.014667  0.215526 0.021373  P 0.0501348 0.0186732                                                                                                             
-2312 5 60283.00 P  0.184219 0.014701  0.215007 0.021434  P 0.0499551 0.0187306                                                                                                             
-2312 6 60284.00 P  0.181950 0.014734  0.214524 0.021496  P 0.0496786 0.0187879                                                                                                             
-2312 7 60285.00 P  0.179676 0.014768  0.214076 0.021558  P 0.0493266 0.0188451                                                                                                             
-2312 8 60286.00 P  0.177398 0.014801  0.213663 0.021619  P 0.0489229 0.0189023                                                                                                             
-2312 9 60287.00 P  0.175116 0.014834  0.213287 0.021681  P 0.0485963 0.0189594                                                                                                             
-231210 60288.00 P  0.172832 0.014868  0.212945 0.021742  P 0.0483677 0.0190165                                                                                                             
-231211 60289.00 P  0.170546 0.014901  0.212640 0.021804  P 0.0483031 0.0190735                                                                                                             
-231212 60290.00 P  0.168258 0.014934  0.212370 0.021865  P 0.0484269 0.0191305                                                                                                             
-231213 60291.00 P  0.165969 0.014967  0.212136 0.021926  P 0.0487995 0.0191874                                                                                                             
-231214 60292.00 P  0.163680 0.015000  0.211938 0.021987  P 0.0492605 0.0192442                                                                                                             
-231215 60293.00 P  0.161392 0.015033  0.211775 0.022048  P 0.0497595 0.0193010                                                                                                             
-231216 60294.00 P  0.159105 0.015066  0.211648 0.022109  P 0.0501340 0.0193577                                                                                                             
-231217 60295.00 P  0.156819 0.015099  0.211556 0.022170  P 0.0501999 0.0194144                                                                                                             
-231218 60296.00 P  0.154536 0.015132  0.211501 0.022231  P 0.0499481 0.0194710                                                                                                             
-231219 60297.00 P  0.152256 0.015165  0.211480 0.022292  P 0.0494864 0.0195276                                                                                                             
-231220 60298.00 P  0.149980 0.015197  0.211495 0.022353  P 0.0489513 0.0195841                                                                                                             
-231221 60299.00 P  0.147708 0.015230  0.211546 0.022414  P 0.0484313 0.0196405                                                                                                             
-231222 60300.00 P  0.145441 0.015263  0.211632 0.022474  P 0.0480623 0.0196969                                                                                                             
-231223 60301.00 P  0.143179 0.015295  0.211753 0.022535  P 0.0479217 0.0197532                                                                                                             
-231224 60302.00 P  0.140924 0.015328  0.211909 0.022595  P 0.0480566 0.0198095                                                                                                             
-231225 60303.00 P  0.138675 0.015360  0.212101 0.022656  P 0.0484915 0.0198658                                                                                                             
-231226 60304.00 P  0.136434 0.015393  0.212327 0.022716  P 0.0491044 0.0199219                                                                                                             
-231227 60305.00 P  0.134201 0.015425  0.212588 0.022776  P 0.0498551 0.0199781                                                                                                             
-231228 60306.00 P  0.131977 0.015457  0.212883 0.022837  P 0.0505910 0.0200341                                                                                                             
-231229 60307.00 P  0.129762 0.015489  0.213213 0.022897  P 0.0512715 0.0200902                                                                                                             
-231230 60308.00 P  0.127557 0.015522  0.213578 0.022957  P 0.0517838 0.0201461                                                                                                             
-231231 60309.00 P  0.125363 0.015554  0.213976 0.023017  P 0.0522116 0.0202021                                                                                                             
-24 1 1 60310.00 P  0.123179 0.015586  0.214409 0.023077  P 0.0523631 0.0202579                                                                                                             
-24 1 2 60311.00 P  0.121007 0.015618  0.214875 0.023137  P 0.0523738 0.0203137                                                                                                             
-24 1 3 60312.00 P  0.118848 0.015650  0.215375 0.023197  P 0.0523231 0.0203695                                                                                                             
-24 1 4 60313.00 P  0.116702 0.015682  0.215909 0.023257  P 0.0522029 0.0204252                                                                                                             
-24 1 5 60314.00 P  0.114569 0.015714  0.216475 0.023317  P 0.0520780 0.0204809                                                                                                             
-24 1 6 60315.00 P  0.112450 0.015746  0.217075 0.023376  P 0.0520078 0.0205365                                                                                                             
-24 1 7 60316.00 P  0.110346 0.015777  0.217707 0.023436  P 0.0520849 0.0205920                                                                                                             
-24 1 8 60317.00 P  0.108257 0.015809  0.218372 0.023496  P 0.0523144 0.0206475                                                                                                             
-24 1 9 60318.00 P  0.106183 0.015841  0.219069 0.023555  P 0.0527459 0.0207030                                                                                                             
-24 110 60319.00 P  0.104127 0.015873  0.219798 0.023615  P 0.0533876 0.0207584                                                                                                             
-24 111 60320.00 P  0.102087 0.015904  0.220558 0.023674  P 0.0541302 0.0208138                                                                                                             
-24 112 60321.00 P  0.100064 0.015936  0.221350 0.023733  P 0.0547331 0.0208691                                                                                                             
-24 113 60322.00 P  0.098060 0.015967  0.222174 0.023793  P 0.0551267 0.0209243                                                                                                             
-24 114 60323.00 P  0.096074 0.015999  0.223028 0.023852  P 0.0552283 0.0209795                                                                                                             
-24 115 60324.00 P  0.094107 0.016030  0.223913 0.023911  P 0.0550364 0.0210347                                                                                                             
-24 116 60325.00 P  0.092160 0.016061  0.224828 0.023970  P 0.0546602 0.0210898                                                                                                             
-24 117 60326.00 P  0.090233 0.016093  0.225773 0.024029  P 0.0543109 0.0211449                                                                                                             
-24 118 60327.00 P  0.088326 0.016124  0.226747 0.024088  P 0.0540668 0.0211999                                                                                                             
-24 119 60328.00 P  0.086441 0.016155  0.227751 0.024147  P 0.0540528 0.0212548                                                                                                             
-24 120 60329.00 P  0.084577 0.016187  0.228784 0.024206  P 0.0543434 0.0213098                                                                                                             
-24 121 60330.00 P  0.082735 0.016218  0.229846 0.024265  P 0.0548542 0.0213646                                                                                                             
-24 122 60331.00 P  0.080917 0.016249  0.230935 0.024324  P 0.0555676 0.0214195                                                                                                             
-24 123 60332.00 P  0.079121 0.016280  0.232053 0.024383  P 0.0564479 0.0214742                                                                                                             
-24 124 60333.00 P  0.077348 0.016311  0.233198 0.024441  P 0.0573771 0.0215290                                                                                                             
-24 125 60334.00 P  0.075600 0.016342  0.234371 0.024500  P 0.0582431 0.0215837                                                                                                             
-24 126 60335.00 P  0.073876 0.016373  0.235570 0.024558  P 0.0589979 0.0216383                                                                                                             
-24 127 60336.00 P  0.072178 0.016404  0.236795 0.024617  P 0.0596027 0.0216929                                                                                                             
-24 128 60337.00 P  0.070504 0.016434  0.238047 0.024675  P 0.0600032 0.0217474                                                                                                             
-24 129 60338.00 P  0.068857 0.016465  0.239324 0.024734  P 0.0601838 0.0218019                                                                                                             
-24 130 60339.00 P  0.067235 0.016496  0.240626 0.024792  P 0.0601972 0.0218564                                                                                                             
-24 131 60340.00 P  0.065641 0.016527  0.241953 0.024851  P 0.0601323 0.0219108                                                                                                             
-24 2 1 60341.00 P  0.064073 0.016557  0.243304 0.024909  P 0.0600850 0.0219652                                                                                                             
-24 2 2 60342.00 P  0.062533 0.016588  0.244680 0.024967  P 0.0601229 0.0220195                                                                                                             
-24 2 3 60343.00 P  0.061021 0.016619  0.246078 0.025025  P 0.0602644 0.0220738                                                                                                             
-24 2 4 60344.00 P  0.059537 0.016649  0.247500 0.025083  P 0.0606006 0.0221280                                                                                                             
-24 2 5 60345.00 P  0.058081 0.016680  0.248945 0.025141  P 0.0610290 0.0221822                                                                                                             
-24 2 6 60346.00 P  0.056655 0.016710  0.250411 0.025199  P 0.0616178 0.0222363                                                                                                             
-24 2 7 60347.00 P  0.055258 0.016740  0.251899 0.025257  P 0.0622696 0.0222904                                                                                                             
-24 2 8 60348.00 P  0.053891 0.016771  0.253408 0.025315  P 0.0627957 0.0223444                                                                                                             
-24 2 9 60349.00 P  0.052554 0.016801  0.254939 0.025373  P 0.0631241 0.0223985                                                                                                             
-24 210 60350.00 P  0.051247 0.016831  0.256489 0.025431  P 0.0631540 0.0224524                                                                                                             
-24 211 60351.00 P  0.049971 0.016862  0.258059 0.025488  P 0.0628483 0.0225063                                                                                                             
-24 212 60352.00 P  0.048725 0.016892  0.259649 0.025546  P 0.0622533 0.0225602                                                                                                             
-24 213 60353.00 P  0.047512 0.016922  0.261257 0.025604  P 0.0615197 0.0226140                                                                                                             
-24 214 60354.00 P  0.046329 0.016952  0.262883 0.025661  P 0.0607901 0.0226678                                                                                                             
-24 215 60355.00 P  0.045179 0.016982  0.264528 0.025719  P 0.0602016 0.0227216                                                                                                             
-24 216 60356.00 P  0.044061 0.017012  0.266190 0.025776  P 0.0598424 0.0227753                                                                                                             
-24 217 60357.00 P  0.042975 0.017042  0.267868 0.025834  P 0.0597476 0.0228290                                                                                                             
-24 218 60358.00 P  0.041922 0.017072  0.269563 0.025891  P 0.0598644 0.0228826                                                                                                             
-24 219 60359.00 P  0.040902 0.017102  0.271274 0.025949  P 0.0601242 0.0229362                                                                                                             
-24 220 60360.00 P  0.039915 0.017132  0.273000 0.026006  P 0.0604207 0.0229897                                                                                                             
-24 221 60361.00 P  0.038962 0.017162  0.274740 0.026063  P 0.0606420 0.0230432                                                                                                             
-24 222 60362.00 P  0.038042 0.017192  0.276495 0.026120  P 0.0607394 0.0230966                                                                                                             
-24 223 60363.00 P  0.037156 0.017221  0.278264 0.026177  P 0.0606299 0.0231500                                                                                                             
-24 224 60364.00 P  0.036304 0.017251  0.280046 0.026234  P 0.0603173 0.0232034                                                                                                             
-24 225 60365.00 P  0.035486 0.017281  0.281840 0.026292  P 0.0597616 0.0232567                                                                                                             
-24 226 60366.00 P  0.034702 0.017311  0.283647 0.026349  P 0.0590465 0.0233100                                                                                                             
-24 227 60367.00 P  0.033953 0.017340  0.285465 0.026405  P 0.0582919 0.0233633                                                                                                             
-24 228 60368.00 P  0.033239 0.017370  0.287294 0.026462  P 0.0575959 0.0234165                                                                                                             
-24 229 60369.00 P  0.032560 0.017399  0.289134 0.026519  P 0.0570284 0.0234697                                                                                                             
-24 3 1 60370.00 P  0.031916 0.017429  0.290983 0.026576  P 0.0565793 0.0235228                                                                                                             
-24 3 2 60371.00 P  0.031306 0.017458  0.292842 0.026633  P 0.0563132 0.0235759                                                                                                             
-24 3 3 60372.00 P  0.030733 0.017488  0.294710 0.026689  P 0.0562005 0.0236289                                                                                                             
-24 3 4 60373.00 P  0.030194 0.017517  0.296586 0.026746  P 0.0563053 0.0236819                                                                                                             
-24 3 5 60374.00 P  0.029691 0.017546  0.298470 0.026803  P 0.0565527 0.0237349                                                                                                             
-24 3 6 60375.00 P  0.029223 0.017576  0.300361 0.026859  P 0.0568205 0.0237878                                                                                                             
-24 3 7 60376.00 P  0.028791 0.017605  0.302259 0.026916  P 0.0569281 0.0238407                                                                                                             
-24 3 8 60377.00 P  0.028395 0.017634  0.304163 0.026972  P 0.0567295 0.0238935                                                                                                             
-24 3 9 60378.00 P  0.028034 0.017663  0.306072 0.027029  P 0.0561918 0.0239463                                                                                                             
-24 310 60379.00 P  0.027709 0.017693  0.307986 0.027085  P 0.0553172 0.0239991                                                                                                             
-24 311 60380.00 P  0.027420 0.017722  0.309905 0.027141  P 0.0542178 0.0240518                                                                                                             
-24 312 60381.00 P  0.027167 0.017751  0.311828 0.027198  P 0.0532283 0.0241045                                                                                                             
-24 313 60382.00 P  0.026950 0.017780  0.313753 0.027254  P 0.0525270 0.0241572                                                                                                             
-24 314 60383.00 P  0.026768 0.017809  0.315682 0.027310  P 0.0522001 0.0242098                                                                                                             
-24 315 60384.00 P  0.026622 0.017838  0.317613 0.027366  P 0.0522693 0.0242624                                                                                                             
-24 316 60385.00 P  0.026512 0.017867  0.319545 0.027423  P 0.0526628 0.0243149                                                                                                             
-24 317 60386.00 P  0.026438 0.017896  0.321478 0.027479  P 0.0532734 0.0243674                                                                                                             
-24 318 60387.00 P  0.026400 0.017925  0.323412 0.027535  P 0.0539657 0.0244199                                                                                                             
-24 319 60388.00 P  0.026397 0.017953  0.325346 0.027591  P 0.0546456 0.0244723                                                                                                             
-24 320 60389.00 P  0.026430 0.017982  0.327279 0.027647  P 0.0552173 0.0245247                                                                                                             
-24 321 60390.00 P  0.026498 0.018011  0.329211 0.027702  P 0.0555947 0.0245770                                                                                                             
-24 322 60391.00 P  0.026602 0.018040  0.331142 0.027758  P 0.0557116 0.0246293                                                                                                             
-24 323 60392.00 P  0.026742 0.018068  0.333070 0.027814  P 0.0556182 0.0246816                                                                                                             
-24 324 60393.00 P  0.026916 0.018097  0.334995 0.027870  P 0.0553662 0.0247338                                                                                                             
-24 325 60394.00 P  0.027126 0.018126  0.336917 0.027926  P 0.0549364 0.0247860                                                                                                             
-24 326 60395.00 P  0.027371 0.018154  0.338835 0.027981  P 0.0545022 0.0248382                                                                                                             
-24 327 60396.00 P  0.027651 0.018183  0.340748 0.028037  P 0.0541737 0.0248903                                                                                                             
-24 328 60397.00 P  0.027966 0.018211  0.342657 0.028092  P 0.0540236 0.0249424                                                                                                             
-24 329 60398.00 P  0.028315 0.018240  0.344560 0.028148  P 0.0541015 0.0249945                                                                                                             
-24 330 60399.00 P  0.028699 0.018268  0.346457 0.028203  P 0.0544037 0.0250465                                                                                                             
-24 331 60400.00 P  0.029117 0.018297  0.348347 0.028259  P 0.0548837 0.0250985                                                                                                             
-24 4 1 60401.00 P  0.029569 0.018325  0.350230 0.028314  P 0.0555562 0.0251504                                                                                                             
-24 4 2 60402.00 P  0.030056 0.018354  0.352106 0.028370  P 0.0562120 0.0252023                                                                                                             
-24 4 3 60403.00 P  0.030576 0.018382  0.353973 0.028425  P 0.0567599 0.0252542                                                                                                             
-24 4 4 60404.00 P  0.031129 0.018410  0.355831 0.028480  P 0.0570555 0.0253060                                                                                                             
-24 4 5 60405.00 P  0.031716 0.018439  0.357681 0.028536  P 0.0570363 0.0253578                                                                                                             
-24 4 6 60406.00 P  0.032336 0.018467  0.359520 0.028591  P 0.0567030 0.0254096                                                                                                             
-24 4 7 60407.00                                                                                                                                                                            
-24 4 8 60408.00                                                                                                                                                                            
-24 4 9 60409.00                                                                                                                                                                            
-24 410 60410.00                                                                                                                                                                            
-24 411 60411.00                                                                                                                                                                            
-24 412 60412.00                                                                                                                                                                            
-24 413 60413.00                                                                                                                                                                            
-24 414 60414.00                                                                                                                                                                            
-24 415 60415.00                                                                                                                                                                            
-24 416 60416.00                                                                                                                                                                            
-24 417 60417.00                                                                                                                                                                            
-24 418 60418.00                                                                                                                                                                            
-24 419 60419.00                                                                                                                                                                            
-24 420 60420.00                                                                                                                                                                            
-24 421 60421.00                                                                                                                                                                            
-24 422 60422.00                                                                                                                                                                            
-24 423 60423.00                                                                                                                                                                            
-24 424 60424.00                                                                                                                                                                            
-24 425 60425.00                                                                                                                                                                            
-24 426 60426.00                                                                                                                                                                            
-24 427 60427.00                                                                                                                                                                            
-24 428 60428.00                                                                                                                                                                            
-24 429 60429.00                                                                                                                                                                            
-24 430 60430.00                                                                                                                                                                            
-24 5 1 60431.00                                                                                                                                                                            
-24 5 2 60432.00                                                                                                                                                                            
-24 5 3 60433.00                                                                                                                                                                            
-24 5 4 60434.00                                                                                                                                                                            
+22 315 59653.00 I  0.034234 0.000023  0.398079 0.000015  I-0.0998758 0.0000061 -0.4393 0.0032  I  -106.880    0.600    -8.182    0.052  0.034250  0.398014 -0.0998830  -106.865    -8.198  
+22 316 59654.00 I  0.033955 0.000033  0.399537 0.000017  I-0.0995328 0.0000048 -0.2306 0.0039  I  -106.947    0.617    -8.164    0.103  0.033972  0.399563 -0.0995467  -106.918    -8.181  
+22 317 59655.00 I  0.033459 0.000033  0.401249 0.000017  I-0.0994310 0.0000047  0.0273 0.0035  I  -106.984    0.617    -8.037    0.103  0.033426  0.401244 -0.0994339  -106.930    -8.064  
+22 318 59656.00 I  0.033076 0.000031  0.402918 0.000017  I-0.0995526 0.0000051  0.1808 0.0034  I  -106.956    0.617    -7.907    0.103  0.033046  0.402931 -0.0995428  -106.876    -7.950  
+22 319 59657.00 I  0.032925 0.000027  0.404429 0.000011  I-0.0997804 0.0000048  0.2976 0.0035  I  -106.959    0.659    -7.852    0.165  0.032894  0.404430 -0.0998242  -106.884    -7.889  
+22 320 59658.00 I  0.033031 0.000027  0.405970 0.000011  I-0.1001533 0.0000047  0.4307 0.0032  I  -107.117    0.659    -7.890    0.165  0.033017  0.405997 -0.1001905  -107.059    -7.919  
+22 321 59659.00 I  0.033373 0.000033  0.407434 0.000014  I-0.1005689 0.0000043  0.3449 0.0036  I  -107.450    0.572    -7.980    0.111  0.033291  0.407432 -0.1005194  -107.409    -8.005  
+22 322 59660.00 I  0.034272 0.000023  0.408886 0.000011  I-0.1007884 0.0000054  0.0948 0.0031  I  -107.861    0.530    -8.021    0.068  0.034163  0.408866 -0.1007374  -107.806    -8.084  
+22 323 59661.00 I  0.035752 0.000024  0.410767 0.000016  I-0.1007727 0.0000045 -0.1128 0.0035  I  -108.093    0.497    -8.079    0.071  0.035739  0.410677 -0.1007668  -108.069    -8.122  
+22 324 59662.00 I  0.037151 0.000025  0.412868 0.000016  I-0.1005690 0.0000044 -0.3019 0.0031  I  -108.064    0.497    -8.114    0.071  0.037184  0.412921 -0.1005632  -108.121    -8.146  
+22 325 59663.00 I  0.038266 0.000024  0.415015 0.000016  I-0.1001862 0.0000042 -0.4391 0.0031  I  -107.764    0.497    -8.165    0.071  0.038276  0.415002 -0.1001852  -107.917    -8.187  
+22 326 59664.00 I  0.039265 0.000024  0.416908 0.000016  I-0.0997291 0.0000044 -0.4614 0.0032  I  -107.290    0.497    -8.243    0.071  0.039275  0.416959 -0.0997325  -107.413    -8.263  
+22 327 59665.00 I  0.040351 0.000019  0.418580 0.000015  I-0.0993023 0.0000047 -0.3669 0.0032  I  -106.799    0.538    -8.326    0.085  0.040293  0.418593 -0.0993188  -106.847    -8.345  
+22 328 59666.00 I  0.041640 0.000019  0.420162 0.000016  I-0.0990358 0.0000047 -0.1510 0.0038  I  -106.438    0.538    -8.391    0.085  0.041691  0.420175 -0.0990554  -106.412    -8.410  
+22 329 59667.00 I  0.042745 0.000018  0.421729 0.000012  I-0.0989806 0.0000059  0.0057 0.0033  I  -106.254    0.660    -8.423    0.077  0.042792  0.421696 -0.0989777  -106.189    -8.449  
+22 330 59668.00 I  0.043409 0.000021  0.423077 0.000019  I-0.0990310 0.0000047  0.1139 0.0039  I  -106.308    0.629    -8.427    0.080  0.043491  0.423055 -0.0990426  -106.244    -8.453  
+22 331 59669.00 I  0.043548 0.000022  0.424808 0.000019  I-0.0992196 0.0000050  0.2557 0.0035  I  -106.436    0.629    -8.386    0.080  0.043570  0.424794 -0.0992346  -106.398    -8.414  
+22 4 1 59670.00 I  0.043351 0.000023  0.426970 0.000020  I-0.0995107 0.0000051  0.3023 0.0038  I  -106.519    0.629    -8.310    0.080  0.043301  0.426919 -0.0995031  -106.506    -8.343  
+22 4 2 59671.00 I  0.043555 0.000018  0.428883 0.000018  I-0.0997950 0.0000058  0.2613 0.0041  I  -106.531    0.585    -8.249    0.083  0.043471  0.428898 -0.0997958  -106.536    -8.278  
+22 4 3 59672.00 I  0.044381 0.000021  0.431006 0.000020  I-0.1000069 0.0000064  0.1413 0.0043  I  -106.561    0.574    -8.269    0.062  0.044401  0.430964 -0.1000185  -106.583    -8.291  
+22 4 4 59673.00 I  0.045130 0.000020  0.433541 0.000020  I-0.1000660 0.0000063 -0.0133 0.0052  I  -106.688    0.574    -8.380    0.062  0.045179  0.433548 -0.1000877  -106.727    -8.395  
+22 4 5 59674.00 I  0.045606 0.000016  0.436188 0.000014  I-0.0999593 0.0000081 -0.2308 0.0049  I  -106.866    0.565    -8.510    0.032  0.045558  0.436184 -0.0999601  -106.928    -8.515  
+22 4 6 59675.00 I  0.046388 0.000019  0.438250 0.000020  I-0.0996011 0.0000075 -0.4581 0.0055  I  -107.021    0.620    -8.581    0.039  0.046324  0.438296 -0.0996161  -107.011    -8.588  
+22 4 7 59676.00 I  0.047706 0.000019  0.440056 0.000020  I-0.0990861 0.0000074 -0.5566 0.0053  I  -106.894    0.620    -8.605    0.039  0.047660  0.440084 -0.0991087  -106.904    -8.610  
+22 4 8 59677.00 I  0.049433 0.000018  0.441874 0.000019  I-0.0985111 0.0000074 -0.5857 0.0053  I  -106.565    0.620    -8.665    0.039  0.049412  0.441800 -0.0985116  -106.602    -8.670  
+22 4 9 59678.00 I  0.051231 0.000015  0.443552 0.000017  I-0.0979307 0.0000077 -0.5669 0.0050  I  -106.083    0.620    -8.840    0.039  0.051279  0.443588 -0.0979207  -106.131    -8.844  
+22 410 59679.00 I  0.052565 0.000016  0.445332 0.000019  I-0.0973866 0.0000066 -0.5204 0.0051  I  -105.529    0.786    -9.102    0.045  0.052631  0.445310 -0.0973816  -105.574    -9.106  
+22 411 59680.00 I  0.053446 0.000015  0.447041 0.000018  I-0.0969113 0.0000066 -0.4098 0.0041  I  -105.062    0.786    -9.348    0.045  0.053447  0.447037 -0.0969159  -105.095    -9.347  
+22 412 59681.00 I  0.054290 0.000013  0.449062 0.000017  I-0.0965831 0.0000048 -0.2510 0.0038  I  -104.883    0.835    -9.501    0.112  0.054284  0.449011 -0.0965845  -104.884    -9.491  
+22 413 59682.00 I  0.055326 0.000011  0.451035 0.000017  I-0.0964339 0.0000039 -0.0184 0.0033  I  -105.048    0.835    -9.551    0.112  0.055292  0.451073 -0.0964523  -105.062    -9.565  
+22 414 59683.00 I  0.056533 0.000011  0.452915 0.000017  I-0.0965583 0.0000044  0.2502 0.0029  I  -105.349    0.835    -9.494    0.112  0.056547  0.452892 -0.0965557  -105.379    -9.547  
+22 415 59684.00 I  0.057880 0.000015  0.454454 0.000018  I-0.0969079 0.0000043  0.4396 0.0030  I  -105.523    0.835    -9.313    0.112  0.057823  0.454485 -0.0968994  -105.550    -9.362  
+22 416 59685.00 I  0.059422 0.000018  0.456174 0.000016  I-0.0974121 0.0000042  0.5529 0.0031  I  -105.584    0.778    -9.059    0.154  0.059424  0.456172 -0.0974129  -105.603    -9.095  
+22 417 59686.00 I  0.061286 0.000020  0.457791 0.000016  I-0.0979771 0.0000044  0.5563 0.0043  I  -105.790    0.778    -8.874    0.154  0.061164  0.457851 -0.0979865  -105.807    -8.908  
+22 418 59687.00 I  0.063721 0.000022  0.459297 0.000016  I-0.0984833 0.0000074  0.4355 0.0043  I  -106.252    0.806    -8.891    0.015  0.063734  0.459266 -0.0985020  -106.274    -8.922  
+22 419 59688.00 I  0.066169 0.000023  0.460809 0.000016  I-0.0988174 0.0000075  0.2225 0.0042  I  -106.734    0.806    -9.084    0.015  0.066192  0.460869 -0.0988272  -106.773    -9.104  
+22 420 59689.00 I  0.068331 0.000027  0.462008 0.000026  I-0.0989000 0.0000041 -0.0756 0.0043  I  -106.892    0.792    -9.298    0.084  0.068329  0.461999 -0.0988949  -106.960    -9.291  
+22 421 59690.00 I  0.070493 0.000026  0.463048 0.000026  I-0.0986843 0.0000043 -0.3196 0.0032  I  -106.639    0.792    -9.423    0.084  0.070468  0.463064 -0.0987060  -106.695    -9.434  
+22 422 59691.00 I  0.072758 0.000023  0.464119 0.000027  I-0.0983194 0.0000049 -0.3878 0.0033  I  -106.183    0.792    -9.469    0.084  0.072707  0.464098 -0.0983386  -106.211    -9.508  
+22 423 59692.00 I  0.075224 0.000022  0.465083 0.000026  I-0.0979269 0.0000049 -0.4013 0.0037  I  -105.770    0.792    -9.496    0.084  0.075204  0.465058 -0.0979051  -105.797    -9.527  
+22 424 59693.00 I  0.077856 0.000017  0.466283 0.000040  I-0.0975412 0.0000056 -0.3417 0.0037  I  -105.474    0.768    -9.537    0.101  0.077859  0.466247 -0.0975194  -105.498    -9.555  
+22 425 59694.00 I  0.080485 0.000015  0.467920 0.000040  I-0.0972766 0.0000056 -0.1828 0.0055  I  -105.254    0.768    -9.578    0.101  0.080557  0.467896 -0.0972632  -105.265    -9.590  
+22 426 59695.00 I  0.082817 0.000012  0.469862 0.000035  I-0.0971782 0.0000095 -0.0162 0.0040  I  -105.108    0.734    -9.591    0.070  0.082859  0.469891 -0.0971847  -105.109    -9.593  
+22 427 59696.00 I  0.084841 0.000019  0.471453 0.000035  I-0.0972281 0.0000058  0.1021 0.0055  I  -105.101    0.742    -9.539    0.138  0.084908  0.471486 -0.0972203  -105.096    -9.548  
+22 428 59697.00 I  0.086493 0.000020  0.472743 0.000035  I-0.0973574 0.0000055  0.1456 0.0043  I  -105.262    0.742    -9.389    0.138  0.086518  0.472819 -0.0973522  -105.258    -9.407  
+22 429 59698.00 I  0.087931 0.000020  0.473543 0.000036  I-0.0974953 0.0000063  0.1172 0.0041  I  -105.486    0.742    -9.168    0.138  0.087895  0.473595 -0.0974914  -105.480    -9.203  
+22 430 59699.00 I  0.089677 0.000019  0.474074 0.000012  I-0.0975714 0.0000060  0.0277 0.0043  I  -105.626    0.749    -8.989    0.183  0.089653  0.474104 -0.0975559  -105.614    -9.011  
+22 5 1 59700.00 I  0.091698 0.000020  0.474621 0.000014  I-0.0975428 0.0000060 -0.0854 0.0043  I  -105.649    0.749    -8.979    0.183  0.091728  0.474632 -0.0975257  -105.627    -8.987  
+22 5 2 59701.00 I  0.093634 0.000024  0.475316 0.000020  I-0.0974058 0.0000062 -0.1830 0.0046  I  -105.648    0.749    -9.150    0.116  0.093634  0.475311 -0.0974187  -105.619    -9.154  
+22 5 3 59702.00 I  0.095564 0.000018  0.476114 0.000019  I-0.0971898 0.0000071 -0.2415 0.0044  I  -105.690    0.749    -9.369    0.030  0.095563  0.476140 -0.0972185  -105.662    -9.372  
+22 5 4 59703.00 I  0.097693 0.000023  0.476934 0.000028  I-0.0969119 0.0000062 -0.3327 0.0047  I  -105.741    0.784    -9.492    0.037  0.097691  0.476906 -0.0969126  -105.734    -9.493  
+22 5 5 59704.00 I  0.099820 0.000023  0.477875 0.000028  I-0.0965118 0.0000061 -0.4617 0.0044  I  -105.742    0.784    -9.521    0.037  0.099882  0.477903 -0.0964992  -105.770    -9.526  
+22 5 6 59705.00 I  0.101675 0.000024  0.478832 0.000028  I-0.0960246 0.0000062 -0.4825 0.0043  I  -105.695    0.784    -9.584    0.037  0.101687  0.478833 -0.0960256  -105.754    -9.581  
+22 5 7 59706.00 I  0.103386 0.000024  0.479498 0.000027  I-0.0955678 0.0000062 -0.4402 0.0040  I  -105.575    0.784    -9.772    0.037  0.103404  0.479538 -0.0955546  -105.646    -9.779  
+22 5 8 59707.00 I  0.105106 0.000024  0.480063 0.000027  I-0.0951540 0.0000051 -0.3685 0.0040  I  -105.296    0.796   -10.015    0.102  0.105117  0.480078 -0.0951550  -105.347   -10.030  
+22 5 9 59708.00 I  0.106695 0.000024  0.480513 0.000027  I-0.0948667 0.0000052 -0.1890 0.0036  I  -104.887    0.796   -10.184    0.102  0.106699  0.480537 -0.0949242  -104.904   -10.197  
+22 510 59709.00 I  0.108521 0.000019  0.480973 0.000018  I-0.0947987 0.0000052  0.0588 0.0032  I  -104.622    0.772   -10.246    0.139  0.108427  0.480933 -0.0948334  -104.607   -10.261  
+22 511 59710.00 I  0.110913 0.000019  0.481771 0.000026  I-0.0949980 0.0000037  0.3479 0.0033  I  -104.756    0.770   -10.275    0.158  0.110941  0.481776 -0.0950144  -104.732   -10.281  
+22 512 59711.00 I  0.113494 0.000018  0.482667 0.000026  I-0.0954640 0.0000041  0.5455 0.0031  I  -105.181    0.770   -10.283    0.158  0.113474  0.482707 -0.0954543  -105.174   -10.290  
+22 513 59712.00 I  0.116069 0.000018  0.483383 0.000026  I-0.0960615 0.0000049  0.6605 0.0037  I  -105.539    0.770   -10.145    0.158  0.116107  0.483379 -0.0960629  -105.566   -10.162  
+22 514 59713.00 I  0.118510 0.000014  0.483942 0.000021  I-0.0967521 0.0000061  0.6769 0.0039  I  -105.727    0.768    -9.783    0.175  0.118527  0.483975 -0.0967431  -105.773    -9.799  
+22 515 59714.00 I  0.120714 0.000021  0.484477 0.000032  I-0.0973746 0.0000061  0.5711 0.0044  I  -106.021    0.850    -9.387    0.156  0.120799  0.484444 -0.0973670  -106.086    -9.399  
+22 516 59715.00 I  0.122297 0.000022  0.485288 0.000031  I-0.0978783 0.0000063  0.4174 0.0059  I  -106.570    0.850    -9.269    0.156  0.122385  0.485333 -0.0978659  -106.653    -9.281  
+22 517 59716.00 I  0.123269 0.000022  0.485822 0.000025  I-0.0981863 0.0000101  0.1945 0.0062  I  -107.055    0.996    -9.502    0.128  0.123240  0.485912 -0.0981728  -107.146    -9.513  
+22 518 59717.00 I  0.124657 0.000028  0.485658 0.000040  I-0.0982695 0.0000106 -0.0219 0.0073  I  -107.059    1.005    -9.843    0.134  0.124614  0.485666 -0.0982338  -107.148    -9.846  
+22 519 59718.00 I  0.126491 0.000027  0.485546 0.000040  I-0.0981575 0.0000105 -0.1934 0.0076  I  -106.589    1.005   -10.040    0.134  0.126492  0.485563 -0.0980742  -106.655   -10.034  
+22 520 59719.00 I  0.128445 0.000027  0.485605 0.000040  I-0.0979287 0.0000108 -0.2268 0.0081  I  -106.037    1.005   -10.085    0.134  0.128370  0.485536 -0.0979421  -106.062   -10.068  
+22 521 59720.00 I  0.130661 0.000022  0.486032 0.000033  I-0.0977459 0.0000124 -0.1342 0.0070  I  -105.739    1.028   -10.087    0.145  0.130677  0.486020 -0.0977739  -105.765   -10.071  
+22 522 59721.00 I  0.132973 0.000026  0.486744 0.000041  I-0.0976768 0.0000089  0.0077 0.0076  I  -105.717    0.874   -10.070    0.090  0.132949  0.486774 -0.0977075  -105.758   -10.059  
+22 523 59722.00 I  0.135353 0.000026  0.487369 0.000041  I-0.0977624 0.0000088  0.1528 0.0060  I  -105.790    0.874    -9.983    0.090  0.135359  0.487350 -0.0977582  -105.848    -9.982  
+22 524 59723.00 I  0.137677 0.000021  0.488142 0.000028  I-0.0979667 0.0000080  0.2507 0.0055  I  -105.807    0.828    -9.817    0.055  0.137703  0.488205 -0.0979698  -105.891    -9.829  
+22 525 59724.00 I  0.139652 0.000023  0.488534 0.000037  I-0.0982384 0.0000066  0.2722 0.0052  I  -105.793    0.868    -9.608    0.057  0.139642  0.488593 -0.0982642  -105.852    -9.614  
+22 526 59725.00 I  0.141660 0.000022  0.488494 0.000037  I-0.0984847 0.0000065  0.2144 0.0046  I  -105.887    0.868    -9.368    0.057  0.141637  0.488529 -0.0985094  -105.918    -9.361  
+22 527 59726.00 I  0.143579 0.000023  0.488465 0.000037  I-0.0986411 0.0000065  0.0783 0.0046  I  -106.147    0.868    -9.108    0.057  0.143638  0.488445 -0.0986407  -106.153    -9.084  
+22 528 59727.00 I  0.145156 0.000017  0.488364 0.000028  I-0.0986082 0.0000066 -0.1570 0.0047  I  -106.453    0.896    -8.926    0.059  0.145102  0.488400 -0.0986068  -106.467    -8.914  
+22 529 59728.00 I  0.146684 0.000016  0.488245 0.000029  I-0.0983140 0.0000067 -0.4317 0.0045  I  -106.639    0.896    -8.969    0.059  0.146706  0.488268 -0.0983314  -106.669    -8.976  
+22 530 59729.00 I  0.148142 0.000026  0.487967 0.000040  I-0.0977444 0.0000060 -0.7076 0.0048  I  -106.662    0.852    -9.276    0.044  0.148067  0.488086 -0.0977877  -106.716    -9.292  
+22 531 59730.00 I  0.149845 0.000024  0.487088 0.000030  I-0.0969122 0.0000070 -0.9435 0.0042  I  -106.607    0.791    -9.682    0.022  0.149795  0.487092 -0.0969563  -106.700    -9.703  
+22 6 1 59731.00 I  0.152003 0.000030  0.486176 0.000040  I-0.0958957 0.0000059 -1.0646 0.0047  I  -106.571    0.998    -9.951    0.041  0.151943  0.486170 -0.0959109  -106.731    -9.971  
+22 6 2 59732.00 I  0.154335 0.000030  0.485423 0.000040  I-0.0947970 0.0000063 -1.1435 0.0045  I  -106.608    0.998   -10.006    0.041  0.154357  0.485426 -0.0947757  -106.670   -10.005  
+22 6 3 59733.00 I  0.156609 0.000030  0.484774 0.000040  I-0.0936398 0.0000068 -1.1289 0.0046  I  -106.744    0.998    -9.980    0.041  0.156589  0.484781 -0.0936356  -106.660    -9.955  
+22 6 4 59734.00 I  0.158876 0.000030  0.484145 0.000039  I-0.0925762 0.0000067 -1.0032 0.0051  I  -106.914    0.998   -10.017    0.041  0.158889  0.484149 -0.0925602  -106.851    -9.984  
+22 6 5 59735.00 I  0.161158 0.000021  0.483621 0.000028  I-0.0916252 0.0000077 -0.9022 0.0047  I  -106.931    1.250   -10.089    0.057  0.161161  0.483622 -0.0916220  -106.921   -10.058  
+22 6 6 59736.00 I  0.163476 0.000027  0.483151 0.000034  I-0.0907867 0.0000066 -0.7564 0.0053  I  -106.703    1.009   -10.071    0.084  0.163382  0.483150 -0.0908246  -106.715   -10.044  
+22 6 7 59737.00 I  0.166257 0.000021  0.482841 0.000020  I-0.0901364 0.0000073 -0.5384 0.0047  I  -106.450    0.875    -9.941    0.099  0.166198  0.482812 -0.0901686  -106.474    -9.925  
+22 6 8 59738.00 I  0.169366 0.000026  0.482835 0.000040  I-0.0896847 0.0000066 -0.3958 0.0049  I  -106.534    0.903    -9.833    0.086  0.169346  0.482843 -0.0896819  -106.581    -9.834  
+22 6 9 59739.00 I  0.172337 0.000026  0.482859 0.000041  I-0.0893328 0.0000066 -0.2891 0.0047  I  -107.025    0.903    -9.819    0.086  0.172338  0.482895 -0.0893344  -107.056    -9.817  
+22 610 59740.00 I  0.175171 0.000026  0.482888 0.000041  I-0.0890942 0.0000067 -0.2194 0.0047  I  -107.637    0.903    -9.756    0.086  0.175150  0.482907 -0.0890843  -107.652    -9.745  
+22 611 59741.00 I  0.177826 0.000026  0.482630 0.000041  I-0.0888492 0.0000068 -0.2842 0.0044  I  -108.182    0.903    -9.473    0.086  0.177834  0.482720 -0.0888551  -108.201    -9.465  
+22 612 59742.00 I  0.180320 0.000022  0.481995 0.000044  I-0.0884940 0.0000057 -0.4445 0.0044  I  -108.787    0.773    -9.087    0.090  0.180290  0.482016 -0.0885165  -108.809    -9.083  
+22 613 59743.00 I  0.182802 0.000022  0.481217 0.000044  I-0.0879285 0.0000056 -0.6999 0.0041  I  -109.509    0.773    -8.952    0.090  0.182826  0.481258 -0.0879480  -109.531    -8.942  
+22 614 59744.00 I  0.185077 0.000015  0.480375 0.000026  I-0.0870865 0.0000059 -0.9783 0.0039  I  -110.000    0.690    -9.206    0.105  0.185100  0.480403 -0.0870940  -110.036    -9.188  
+22 615 59745.00 I  0.187071 0.000035  0.479276 0.000036  I-0.0859923 0.0000055 -1.1956 0.0040  I  -109.879    0.704    -9.597    0.140  0.187052  0.479331 -0.0859830  -109.873    -9.588  
+22 616 59746.00 I  0.189198 0.000035  0.478011 0.000036  I-0.0847403 0.0000055 -1.2779 0.0039  I  -109.274    0.704    -9.829    0.140  0.189149  0.478024 -0.0847332  -109.222    -9.837  
+22 617 59747.00 I  0.191615 0.000035  0.476727 0.000036  I-0.0834987 0.0000056 -1.1735 0.0049  I  -108.681    0.704    -9.902    0.140  0.191602  0.476728 -0.0834949  -108.594    -9.934  
+22 618 59748.00 I  0.194038 0.000033  0.475538 0.000027  I-0.0824299 0.0000082 -0.9592 0.0054  I  -108.440    0.837    -9.955    0.222  0.194019  0.475550 -0.0824189  -108.365    -9.983  
+22 619 59749.00 I  0.196593 0.000033  0.474522 0.000027  I-0.0815733 0.0000092 -0.7661 0.0051  I  -108.556    0.837    -9.957    0.222  0.196541  0.474534 -0.0815575  -108.509    -9.976  
+22 620 59750.00 I  0.199463 0.000034  0.473569 0.000034  I-0.0808818 0.0000062 -0.6209 0.0055  I  -108.865    0.811    -9.779    0.159  0.199454  0.473574 -0.0808812  -108.836    -9.796  
+22 621 59751.00 I  0.202394 0.000012  0.472814 0.000023  I-0.0803065 0.0000059 -0.5507 0.0039  I  -109.177    0.808    -9.449    0.137  0.202403  0.472799 -0.0803109  -109.153    -9.467  
+22 622 59752.00 I  0.205097 0.000015  0.472255 0.000027  I-0.0797506 0.0000047 -0.5700 0.0038  I  -109.379    0.719    -9.158    0.135  0.205128  0.472282 -0.0797589  -109.347    -9.174  
+22 623 59753.00 I  0.207617 0.000016  0.471607 0.000028  I-0.0791237 0.0000049 -0.7178 0.0034  I  -109.530    0.719    -9.017    0.135  0.207619  0.471645 -0.0791011  -109.587    -9.025  
+22 624 59754.00 I  0.210143 0.000016  0.470771 0.000028  I-0.0783040 0.0000050 -0.8985 0.0035  I  -109.778    0.719    -8.977    0.135  0.210148  0.470821 -0.0782976  -109.961    -8.971  
+22 625 59755.00 I  0.212734 0.000017  0.469692 0.000028  I-0.0773340 0.0000050 -1.0572 0.0034  I  -110.138    0.719    -8.983    0.135  0.212693  0.469719 -0.0773260  -110.305    -8.982  
+22 626 59756.00 I  0.215401 0.000023  0.468441 0.000029  I-0.0761715 0.0000047 -1.2701 0.0035  I  -110.452    0.782    -9.102    0.139  0.215376  0.468485 -0.0761726  -110.571    -9.112  
+22 627 59757.00 I  0.218222 0.000023  0.467029 0.000028  I-0.0748172 0.0000048 -1.4127 0.0038  I  -110.568    0.782    -9.405    0.139  0.218164  0.467038 -0.0748406  -110.659    -9.428  
+22 628 59758.00 I  0.221337 0.000021  0.465597 0.000025  I-0.0733620 0.0000059 -1.5075 0.0040  I  -110.511    0.910    -9.794    0.144  0.221330  0.465623 -0.0733645  -110.576    -9.834  
+22 629 59759.00 I  0.224404 0.000022  0.464144 0.000038  I-0.0718066 0.0000065 -1.5892 0.0046  I  -110.442    0.947   -10.029    0.126  0.224443  0.464165 -0.0718011  -110.473   -10.052  
+22 630 59760.00 I  0.227228 0.000022  0.462598 0.000037  I-0.0702105 0.0000070 -1.5903 0.0048  I  -110.497    0.947    -9.979    0.126  0.227220  0.462671 -0.0702118  -110.474    -9.975  
+22 7 1 59761.00 I  0.230018 0.000022  0.460847 0.000037  I-0.0686605 0.0000072 -1.4879 0.0066  I  -110.702    0.947    -9.759    0.126  0.230002  0.460818 -0.0686663  -110.599    -9.722  
+22 7 2 59762.00 I  0.232934 0.000011  0.459215 0.000031  I-0.0672410 0.0000112 -1.3668 0.0058  I  -110.971    1.012    -9.587    0.082  0.232881  0.459225 -0.0672447  -110.959    -9.582  
+22 7 3 59763.00 I  0.236097 0.000015  0.457823 0.000041  I-0.0659491 0.0000092 -1.1793 0.0072  I  -111.139    0.873    -9.531    0.141  0.236109  0.457809 -0.0659625  -111.150    -9.536  
+22 7 4 59764.00 I  0.239191 0.000015  0.456540 0.000041  I-0.0649146 0.0000090 -0.8952 0.0058  I  -111.087    0.873    -9.488    0.141  0.239234  0.456579 -0.0649159  -111.121    -9.498  
+22 7 5 59765.00 I  0.241894 0.000013  0.455121 0.000035  I-0.0641420 0.0000072 -0.6610 0.0055  I  -110.909    0.820    -9.377    0.171  0.241892  0.455171 -0.0641393  -110.976    -9.390  
+22 7 6 59766.00 I  0.244459 0.000013  0.453293 0.000035  I-0.0635560 0.0000062 -0.5365 0.0048  I  -110.895    0.820    -9.261    0.171  0.244450  0.453302 -0.0635337  -110.950    -9.262  
+22 7 7 59767.00 I  0.247125 0.000013  0.451608 0.000035  I-0.0630519 0.0000063 -0.4634 0.0045  I  -111.265    0.820    -9.236    0.171  0.247124  0.451582 -0.0630501  -111.305    -9.226  
+22 7 8 59768.00 I  0.249746 0.000013  0.450109 0.000035  I-0.0625976 0.0000065 -0.4853 0.0047  I  -111.936    0.820    -9.244    0.171  0.249756  0.450120 -0.0625785  -111.978    -9.228  
+22 7 9 59769.00 I  0.252293 0.000009  0.448653 0.000024  I-0.0620343 0.0000071 -0.6483 0.0038  I  -112.679    0.877    -9.148    0.179  0.252297  0.448682 -0.0620271  -112.723    -9.129  
+22 710 59770.00 I  0.254694 0.000016  0.447028 0.000025  I-0.0612804 0.0000041 -0.8732 0.0043  I  -113.384    0.803    -8.977    0.143  0.254733  0.447060 -0.0612967  -113.423    -8.960  
+22 711 59771.00 I  0.256801 0.000016  0.445401 0.000017  I-0.0602888 0.0000047 -1.0954 0.0031  I  -113.968    0.771    -8.953    0.116  0.256857  0.445395 -0.0603249  -114.007    -8.936  
+22 712 59772.00 I  0.258321 0.000017  0.443917 0.000017  I-0.0591188 0.0000047 -1.2300 0.0030  I  -114.198    0.771    -9.165    0.116  0.258411  0.443974 -0.0591324  -114.246    -9.142  
+22 713 59773.00 I  0.259223 0.000017  0.442026 0.000020  I-0.0578269 0.0000037 -1.3704 0.0030  I  -113.927    0.783    -9.408    0.153  0.259174  0.442066 -0.0577813  -113.960    -9.403  
+22 714 59774.00 I  0.260256 0.000017  0.439915 0.000020  I-0.0564445 0.0000038 -1.3115 0.0027  I  -113.400    0.783    -9.466    0.153  0.260201  0.439888 -0.0564587  -113.418    -9.484  
+22 715 59775.00 I  0.261705 0.000018  0.438129 0.000019  I-0.0552622 0.0000040 -1.0778 0.0036  I  -113.026    0.783    -9.421    0.153  0.261642  0.438122 -0.0552630  -113.037    -9.466  
+22 716 59776.00 I  0.263451 0.000013  0.436348 0.000018  I-0.0542801 0.0000061 -0.8706 0.0029  I  -112.967    0.808    -9.463    0.195  0.263441  0.436373 -0.0542876  -112.983    -9.496  
+22 717 59777.00 I  0.265296 0.000017  0.434376 0.000019  I-0.0535137 0.0000041 -0.6852 0.0037  I  -113.148    0.864    -9.534    0.136  0.265267  0.434398 -0.0535228  -113.161    -9.544  
+22 718 59778.00 I  0.267260 0.000017  0.432334 0.000019  I-0.0528832 0.0000041 -0.5794 0.0031  I  -113.505    0.864    -9.412    0.136  0.267234  0.432352 -0.0528927  -113.506    -9.398  
+22 719 59779.00 I  0.269239 0.000018  0.430284 0.000014  I-0.0523133 0.0000046 -0.5984 0.0029  I  -113.979    0.894    -9.081    0.066  0.269260  0.430298 -0.0523068  -113.947    -9.037  
+22 720 59780.00 I  0.270985 0.000025  0.428191 0.000029  I-0.0516619 0.0000042 -0.6910 0.0032  I  -114.405    0.821    -8.811    0.126  0.270974  0.428173 -0.0516628  -114.393    -8.784  
+22 721 59781.00 I  0.272566 0.000025  0.426252 0.000029  I-0.0509175 0.0000044 -0.8252 0.0031  I  -114.656    0.821    -8.809    0.126  0.272574  0.426255 -0.0508922  -114.674    -8.805  
+22 722 59782.00 I  0.274104 0.000025  0.424462 0.000030  I-0.0499868 0.0000046 -1.0336 0.0040  I  -114.827    0.821    -9.001    0.126  0.274053  0.424453 -0.0499591  -114.884    -9.018  
+22 723 59783.00 I  0.275661 0.000023  0.422673 0.000029  I-0.0488637 0.0000068 -1.2019 0.0038  I  -115.068    0.680    -9.190    0.176  0.275681  0.422673 -0.0488673  -115.096    -9.210  
+22 724 59784.00 I  0.277055 0.000023  0.420910 0.000035  I-0.0475899 0.0000061 -1.3494 0.0045  I  -115.345    0.776    -9.322    0.182  0.277006  0.420915 -0.0476028  -115.333    -9.343  
+22 725 59785.00 I  0.278485 0.000023  0.419325 0.000035  I-0.0461853 0.0000059 -1.4356 0.0051  I  -115.498    0.776    -9.491    0.182  0.278471  0.419285 -0.0462003  -115.452    -9.519  
+22 726 59786.00 I  0.279855 0.000014  0.417904 0.000025  I-0.0447445 0.0000082 -1.4443 0.0052  I  -115.482    0.870    -9.730    0.190  0.279867  0.417962 -0.0447491  -115.399    -9.768  
+22 727 59787.00 I  0.281074 0.000023  0.416119 0.000039  I-0.0432977 0.0000086 -1.4500 0.0062  I  -115.416    0.830    -9.900    0.179  0.281044  0.416126 -0.0432579  -115.379    -9.934  
+22 728 59788.00 I  0.282267 0.000023  0.414141 0.000038  I-0.0418469 0.0000093 -1.4487 0.0070  I  -115.408    0.830    -9.844    0.179  0.282267  0.414205 -0.0417953  -115.431    -9.867  
+22 729 59789.00 I  0.283372 0.000022  0.411848 0.000038  I-0.0404312 0.0000111 -1.3549 0.0101  I  -115.451    0.830    -9.589    0.179  0.283345  0.411841 -0.0404282  -115.538    -9.595  
+22 730 59790.00 I  0.284624 0.000021  0.409427 0.000032  I-0.0391829 0.0000179 -1.1239 0.0077  I  -115.481    0.671    -9.334    0.152  0.284587  0.409400 -0.0392089  -115.593    -9.353  
+22 731 59791.00 I  0.285988 0.000025  0.407284 0.000041  I-0.0381740 0.0000107 -0.9213 0.0104  I  -115.463    0.777    -9.232    0.276  0.286000  0.407286 -0.0381849  -115.593    -9.273  
+22 8 1 59792.00 I  0.287130 0.000025  0.405197 0.000041  I-0.0373444 0.0000107 -0.7063 0.0069  I  -115.386    0.777    -9.258    0.276  0.287161  0.405194 -0.0373892  -115.536    -9.320  
+22 8 2 59793.00 I  0.287887 0.000019  0.403236 0.000032  I-0.0367524 0.0000088 -0.5181 0.0068  I  -115.276    0.760    -9.288    0.277  0.287882  0.403262 -0.0367846  -115.439    -9.376  
+22 8 3 59794.00 I  0.288545 0.000019  0.400998 0.000032  I-0.0362662 0.0000084 -0.4557 0.0057  I  -115.252    0.760    -9.258    0.277  0.288468  0.401019 -0.0362792  -115.414    -9.314  
+22 8 4 59795.00 I  0.289527 0.000020  0.398720 0.000032  I-0.0358181 0.0000073 -0.4618 0.0055  I  -115.487    0.760    -9.205    0.277  0.289489  0.398709 -0.0358145  -115.635    -9.222  
+22 8 5 59796.00 I  0.290537 0.000019  0.396553 0.000032  I-0.0353231 0.0000071 -0.5264 0.0052  I  -116.042    0.760    -9.178    0.277  0.290582  0.396579 -0.0353263  -116.154    -9.192  
+22 8 6 59797.00 I  0.291094 0.000015  0.394197 0.000017  I-0.0347348 0.0000073 -0.6826 0.0044  I  -116.770    0.717    -9.178    0.251  0.291080  0.394221 -0.0347316  -116.838    -9.204  
+22 8 7 59798.00 I  0.291548 0.000021  0.391643 0.000021  I-0.0339401 0.0000052 -0.8924 0.0047  I  -117.409    0.700    -9.224    0.255  0.291487  0.391652 -0.0339451  -117.435    -9.261  
+22 8 8 59799.00 I  0.292337 0.000020  0.389021 0.000014  I-0.0329722 0.0000058 -1.0357 0.0039  I  -117.722    0.685    -9.355    0.258  0.292293  0.389056 -0.0329721  -117.715    -9.399  
+22 8 9 59800.00 I  0.293210 0.000019  0.386220 0.000014  I-0.0318940 0.0000058 -1.1032 0.0037  I  -117.607    0.685    -9.520    0.258  0.293211  0.386232 -0.0318918  -117.585    -9.565  
+22 810 59801.00 I  0.293835 0.000021  0.383251 0.000026  I-0.0308084 0.0000045 -1.0430 0.0039  I  -117.203    0.743    -9.546    0.269  0.293803  0.383250 -0.0308088  -117.149    -9.591  
+22 811 59802.00 I  0.294451 0.000021  0.380334 0.000027  I-0.0298561 0.0000051 -0.8386 0.0036  I  -116.848    0.743    -9.352    0.269  0.294459  0.380298 -0.0298577  -116.770    -9.397  
+22 812 59803.00 I  0.295060 0.000021  0.377818 0.000027  I-0.0291393 0.0000057 -0.6098 0.0043  I  -116.775    0.743    -9.121    0.269  0.295055  0.377755 -0.0291384  -116.681    -9.171  
+22 813 59804.00 I  0.295579 0.000015  0.375709 0.000025  I-0.0286242 0.0000068 -0.4179 0.0043  I  -116.898    0.780    -9.090    0.278  0.295537  0.375740 -0.0286307  -116.834    -9.134  
+22 814 59805.00 I  0.296373 0.000014  0.373568 0.000025  I-0.0282806 0.0000064 -0.2948 0.0046  I  -117.029    0.780    -9.224    0.278  0.296313  0.373591 -0.0282983  -117.006    -9.266  
+22 815 59806.00 I  0.297512 0.000015  0.371304 0.000029  I-0.0279874 0.0000063 -0.3135 0.0064  I  -117.196    0.779    -9.256    0.230  0.297500  0.371314 -0.0279699  -117.203    -9.307  
+22 816 59807.00 I  0.298550 0.000014  0.369042 0.000019  I-0.0276157 0.0000110 -0.4461 0.0065  I  -117.539    0.779    -9.069    0.125  0.298583  0.369059 -0.0276395  -117.555    -9.139  
+22 817 59808.00 I  0.299277 0.000019  0.366742 0.000030  I-0.0270842 0.0000114 -0.6119 0.0080  I  -118.001    0.760    -8.854    0.125  0.299254  0.366732 -0.0270866  -118.003    -8.949  
+22 818 59809.00 I  0.299910 0.000020  0.364400 0.000031  I-0.0263618 0.0000115 -0.8682 0.0081  I  -118.372    0.760    -8.836    0.125  0.299866  0.364425 -0.0263517  -118.274    -8.865  
+22 819 59810.00 I  0.300903 0.000020  0.362025 0.000030  I-0.0253584 0.0000115 -1.0929 0.0083  I  -118.566    0.760    -8.999    0.125  0.300823  0.362010 -0.0253455  -118.335    -8.928  
+22 820 59811.00 I  0.302125 0.000020  0.359758 0.000030  I-0.0241888 0.0000120 -1.2792 0.0073  I  -118.672    0.760    -9.151    0.125  0.302176  0.359779 -0.0241871  -118.439    -9.105  
+22 821 59812.00 I  0.303009 0.000024  0.357421 0.000041  I-0.0228220 0.0000091 -1.3997 0.0074  I  -118.743    0.614    -9.185    0.108  0.302992  0.357455 -0.0228266  -118.572    -9.196  
+22 822 59813.00 I  0.303768 0.000023  0.354930 0.000041  I-0.0214199 0.0000088 -1.4289 0.0058  I  -118.711    0.614    -9.191    0.108  0.303769  0.354926 -0.0213929  -118.632    -9.243  
+22 823 59814.00 I  0.304486 0.000019  0.352484 0.000034  I-0.0199959 0.0000073 -1.3632 0.0052  I  -118.541    0.616    -9.290    0.104  0.304513  0.352500 -0.0199836  -118.587    -9.375  
+22 824 59815.00 I  0.304888 0.000018  0.349901 0.000039  I-0.0187048 0.0000057 -1.2636 0.0047  I  -118.308    0.714    -9.445    0.131  0.304896  0.349874 -0.0186613  -118.307    -9.531  
+22 825 59816.00 I  0.305185 0.000018  0.347450 0.000039  I-0.0174463 0.0000059 -1.2314 0.0040  I  -118.107    0.714    -9.495    0.131  0.305201  0.347486 -0.0174037  -118.023    -9.577  
+22 826 59817.00 I  0.305355 0.000017  0.344924 0.000039  I-0.0162886 0.0000056 -1.0596 0.0044  I  -117.944    0.714    -9.357    0.131  0.305398  0.344912 -0.0162851  -117.767    -9.438  
+22 827 59818.00 I  0.305270 0.000010  0.342339 0.000023  I-0.0153432 0.0000065 -0.8395 0.0038  I  -117.795    0.895    -9.125    0.159  0.305290  0.342335 -0.0153482  -117.637    -9.193  
+22 828 59819.00 I  0.304966 0.000020  0.339915 0.000030  I-0.0146130 0.0000051 -0.6090 0.0041  I  -117.681    0.774    -8.981    0.178  0.304974  0.339946 -0.0146136  -117.565    -9.035  
+22 829 59820.00 I  0.304625 0.000020  0.337394 0.000030  I-0.0141175 0.0000049 -0.4014 0.0037  I  -117.644    0.774    -9.007    0.178  0.304586  0.337401 -0.0140968  -117.551    -9.055  
+22 830 59821.00 I  0.304498 0.000020  0.334986 0.000023  I-0.0137965 0.0000053 -0.2348 0.0032  I  -117.661    0.717    -9.129    0.191  0.304464  0.334971 -0.0137838  -117.601    -9.176  
+22 831 59822.00 I  0.304617 0.000022  0.332728 0.000027  I-0.0136230 0.0000040 -0.1431 0.0034  I  -117.689    0.747    -9.210    0.165  0.304595  0.332751 -0.0136099  -117.612    -9.248  
+22 9 1 59823.00 I  0.304750 0.000022  0.330386 0.000027  I-0.0134686 0.0000041 -0.1767 0.0032  I  -117.787    0.747    -9.184    0.165  0.304814  0.330440 -0.0134836  -117.693    -9.211  
+22 9 2 59824.00 I  0.304506 0.000022  0.327664 0.000027  I-0.0132462 0.0000050 -0.2806 0.0035  I  -118.070    0.747    -9.104    0.165  0.304501  0.327651 -0.0132494  -118.154    -9.102  
+22 9 3 59825.00 I  0.304210 0.000012  0.325045 0.000017  I-0.0128899 0.0000057 -0.4371 0.0043  I  -118.518    0.778    -9.070    0.133  0.304186  0.324993 -0.0128821  -118.590    -9.080  
+22 9 4 59826.00 I  0.304085 0.000015  0.322759 0.000024  I-0.0123677 0.0000070 -0.6065 0.0046  I  -118.883    0.750    -9.143    0.193  0.304085  0.322764 -0.0123741  -118.929    -9.170  
+22 9 5 59827.00 I  0.303787 0.000015  0.320457 0.000023  I-0.0117012 0.0000071 -0.7029 0.0075  I  -118.887    0.750    -9.283    0.193  0.303820  0.320481 -0.0117203  -118.916    -9.328  
+22 9 6 59828.00 I  0.303228 0.000014  0.317957 0.000019  I-0.0110127 0.0000133 -0.6468 0.0063  I  -118.480    0.719    -9.351    0.246  0.303248  0.318029 -0.0110190  -118.525    -9.426  
+22 9 7 59829.00 I  0.302620 0.000015  0.314925 0.000027  I-0.0104235 0.0000103 -0.5430 0.0082  I  -117.922    0.887    -9.202    0.188  0.302652  0.314951 -0.0103738  -117.930    -9.248  
+22 9 8 59830.00 I  0.301723 0.000016  0.311761 0.000028  I-0.0099635 0.0000097 -0.3287 0.0072  I  -117.587    0.887    -8.845    0.188  0.301793  0.311758 -0.0099952  -117.557    -8.853  
+22 9 9 59831.00 I  0.300346 0.000017  0.308693 0.000029  I-0.0097973 0.0000102 -0.0208 0.0068  I  -117.613    0.887    -8.495    0.188  0.300297  0.308670 -0.0098037  -117.537    -8.461  
+22 910 59832.00 I  0.299161 0.000014  0.305663 0.000024  I-0.0098957 0.0000095  0.2087 0.0058  I  -117.807    1.155    -8.381    0.070  0.299086  0.305665 -0.0098938  -117.785    -8.354  
+22 911 59833.00 I  0.298571 0.000024  0.302851 0.000036  I-0.0101846 0.0000057  0.3481 0.0055  I  -117.909    1.007    -8.506    0.141  0.298524  0.302843 -0.0101991  -117.949    -8.495  
+22 912 59834.00 I  0.298128 0.000024  0.300270 0.000036  I-0.0105534 0.0000057  0.3720 0.0042  I  -117.924    1.007    -8.664    0.141  0.298153  0.300265 -0.0105663  -118.003    -8.665  
+22 913 59835.00 I  0.297554 0.000024  0.297926 0.000032  I-0.0108733 0.0000062  0.2298 0.0037  I  -118.064    0.934    -8.704    0.175  0.297509  0.297897 -0.0108687  -118.179    -8.722  
+22 914 59836.00 I  0.296978 0.000025  0.295807 0.000051  I-0.0109921 0.0000048  0.0247 0.0040  I  -118.400    0.930    -8.681    0.134  0.296992  0.295809 -0.0110048  -118.515    -8.694  
+22 915 59837.00 I  0.296334 0.000024  0.293809 0.000051  I-0.0109032 0.0000049 -0.2389 0.0034  I  -118.757    0.930    -8.727    0.134  0.296326  0.293853 -0.0109071  -118.881    -8.735  
+22 916 59838.00 I  0.295609 0.000024  0.291699 0.000051  I-0.0105284 0.0000048 -0.4602 0.0039  I  -118.920    0.930    -8.842    0.134  0.295633  0.291666 -0.0105453  -119.064    -8.840  
+22 917 59839.00 I  0.294744 0.000015  0.289611 0.000043  I-0.0099908 0.0000061 -0.6573 0.0035  I  -118.830    0.926    -8.900    0.072  0.294765  0.289613 -0.0099966  -118.954    -8.905  
+22 918 59840.00 I  0.293576 0.000020  0.287789 0.000057  I-0.0092324 0.0000052 -0.7984 0.0040  I  -118.558    0.998    -8.834    0.118  0.293594  0.287789 -0.0092502  -118.640    -8.844  
+22 919 59841.00 I  0.292285 0.000020  0.285843 0.000056  I-0.0084335 0.0000052 -0.8210 0.0040  I  -118.192    0.998    -8.732    0.118  0.292235  0.285928 -0.0084134  -118.223    -8.750  
+22 920 59842.00 I  0.291356 0.000020  0.283523 0.000039  I-0.0075709 0.0000060 -0.9020 0.0035  I  -117.817    1.067    -8.735    0.149  0.291284  0.283515 -0.0075559  -117.778    -8.771  
+22 921 59843.00 I  0.290657 0.000020  0.281046 0.000041  I-0.0066828 0.0000046 -0.8229 0.0037  I  -117.525    0.969    -8.846    0.115  0.290675  0.281089 -0.0066950  -117.531    -8.864  
+22 922 59844.00 I  0.289762 0.000020  0.278371 0.000041  I-0.0059691 0.0000044 -0.6116 0.0034  I  -117.370    0.969    -8.930    0.115  0.289785  0.278400 -0.0059969  -117.441    -8.921  
+22 923 59845.00 I  0.288625 0.000019  0.275550 0.000041  I-0.0054454 0.0000049 -0.4428 0.0038  I  -117.323    0.969    -8.857    0.115  0.288673  0.275532 -0.0054471  -117.457    -8.810  
+22 924 59846.00 I  0.287260 0.000013  0.272936 0.000016  I-0.0050921 0.0000063 -0.2480 0.0036  I  -117.318    0.763    -8.651    0.022  0.287244  0.272949 -0.0051006  -117.468    -8.622  
+22 925 59847.00 I  0.285951 0.000027  0.270430 0.000037  I-0.0049465 0.0000054 -0.0618 0.0041  I  -117.333    0.723    -8.458    0.183  0.285878  0.270404 -0.0049635  -117.484    -8.457  
+22 926 59848.00 I  0.285167 0.000027  0.268165 0.000037  I-0.0049533 0.0000054  0.0787 0.0043  I  -117.383    0.723    -8.414    0.183  0.285103  0.268121 -0.0049793  -117.537    -8.441  
+22 927 59849.00 I  0.284710 0.000027  0.266423 0.000035  I-0.0050996 0.0000066  0.2061 0.0039  I  -117.466    0.699    -8.523    0.247  0.284746  0.266357 -0.0051012  -117.616    -8.597  
+22 928 59850.00 I  0.283878 0.000028  0.264922 0.000035  I-0.0053099 0.0000055  0.1666 0.0041  I  -117.562    0.627    -8.655    0.177  0.283878  0.264953 -0.0053014  -117.693    -8.702  
+22 929 59851.00 I  0.283008 0.000027  0.263304 0.000035  I-0.0053962 0.0000048  0.0171 0.0036  I  -117.663    0.627    -8.692    0.177  0.282943  0.263319 -0.0054180  -117.779    -8.707  
+22 930 59852.00 I  0.282323 0.000027  0.261509 0.000035  I-0.0053342 0.0000048 -0.1623 0.0035  I  -117.778    0.627    -8.623    0.177  0.282338  0.261528 -0.0053388  -117.905    -8.603  
+2210 1 59853.00 I  0.281362 0.000013  0.259745 0.000014  I-0.0050464 0.0000050 -0.4173 0.0034  I  -117.857    0.514    -8.534    0.036  0.281388  0.259744 -0.0049041  -117.934    -8.536  
+2210 2 59854.00 I  0.280043 0.000011  0.257884 0.000014  I-0.0045487 0.0000049 -0.5250 0.0033  I  -117.774    0.514    -8.512    0.036  0.280092  0.257931 -0.0043864  -117.763    -8.633  
+2210 3 59855.00 I  0.278450 0.000018  0.255736 0.000015  I-0.0040472 0.0000043 -0.4801 0.0038  I  -117.410    0.880    -8.557    0.121  0.278478  0.255746 -0.0040146  -117.380    -8.681  
+2210 4 59856.00 I  0.276547 0.000017  0.253520 0.000015  I-0.0035918 0.0000058 -0.4251 0.0030  I  -116.810    1.094    -8.578    0.164  0.276607  0.253527 -0.0035590  -116.777    -8.672  
+2210 5 59857.00 I  0.274395 0.000017  0.251432 0.000021  I-0.0032284 0.0000042 -0.2760 0.0037  I  -116.208    1.048    -8.478    0.140  0.274352  0.251450 -0.0032281  -116.158    -8.550  
+2210 6 59858.00 I  0.272446 0.000021  0.249225 0.000021  I-0.0030735 0.0000047 -0.0259 0.0033  I  -115.870    1.048    -8.246    0.140  0.272409  0.249284 -0.0030816  -115.892    -8.306  
+2210 7 59859.00 I  0.270893 0.000024  0.246721 0.000019  I-0.0031817 0.0000051  0.2393 0.0035  I  -115.873    1.048    -7.990    0.140  0.270869  0.246728 -0.0031810  -115.963    -8.047  
+2210 8 59860.00 I  0.269391 0.000024  0.244284 0.000019  I-0.0035383 0.0000052  0.4630 0.0039  I  -116.056    1.048    -7.831    0.140  0.269464  0.244272 -0.0035337  -116.181    -7.889  
+2210 9 59861.00 I  0.267405 0.000019  0.242149 0.000017  I-0.0040726 0.0000058  0.5813 0.0033  I  -116.188    1.007    -7.792    0.112  0.267436  0.242181 -0.0040628  -116.323    -7.852  
+221010 59862.00 I  0.265327 0.000021  0.239992 0.000019  I-0.0046613 0.0000042  0.5807 0.0038  I  -116.197    0.874    -7.810    0.088  0.265240  0.239987 -0.0046541  -116.330    -7.871  
+221011 59863.00 I  0.263669 0.000021  0.237871 0.000012  I-0.0051858 0.0000050  0.4356 0.0032  I  -116.209    0.740    -7.835    0.055  0.263701  0.237885 -0.0051692  -116.344    -7.899  
+221012 59864.00 I  0.262030 0.000020  0.235728 0.000012  I-0.0055026 0.0000047  0.2007 0.0035  I  -116.363    0.783    -7.883    0.043  0.262046  0.235701 -0.0055011  -116.517    -7.950  
+221013 59865.00 I  0.259880 0.000018  0.233780 0.000012  I-0.0055839 0.0000049 -0.0440 0.0035  I  -116.617    0.783    -7.970    0.043  0.260021  0.233734 -0.0055722  -116.707    -8.023  
+221014 59866.00 I  0.256987 0.000018  0.232088 0.000011  I-0.0054369 0.0000051 -0.2219 0.0036  I  -116.775    0.783    -8.049    0.043  0.256936  0.232102 -0.0054362  -116.793    -8.078  
+221015 59867.00 I  0.254059 0.000018  0.230367 0.000011  I-0.0051795 0.0000053 -0.2815 0.0042  I  -116.667    0.783    -8.045    0.043  0.254063  0.230356 -0.0051876  -116.700    -8.075  
+221016 59868.00 I  0.251191 0.000018  0.228842 0.000026  I-0.0048947 0.0000066 -0.2786 0.0042  I  -116.282    0.899    -7.956    0.072  0.251206  0.228893 -0.0049099  -116.365    -7.987  
+221017 59869.00 I  0.248067 0.000022  0.227228 0.000027  I-0.0046568 0.0000064 -0.1721 0.0050  I  -115.752    0.899    -7.885    0.072  0.248052  0.227286 -0.0046783  -115.804    -7.935  
+221018 59870.00 I  0.245191 0.000020  0.225137 0.000028  I-0.0045624 0.0000075 -0.0299 0.0046  I  -115.218    0.932    -7.935    0.095  0.245102  0.225158 -0.0045660  -115.200    -8.015  
+221019 59871.00 I  0.243016 0.000019  0.222944 0.000034  I-0.0045918 0.0000067  0.0969 0.0050  I  -114.761    0.988    -8.085    0.131  0.243041  0.222898 -0.0045814  -114.747    -8.164  
+221020 59872.00 I  0.240704 0.000020  0.221151 0.000034  I-0.0047742 0.0000067  0.2779 0.0047  I  -114.447    0.988    -8.190    0.131  0.240817  0.221191 -0.0047645  -114.446    -8.265  
+221021 59873.00 I  0.237720 0.000020  0.219311 0.000034  I-0.0051502 0.0000065  0.4669 0.0053  I  -114.357    0.988    -8.118    0.131  0.237688  0.219313 -0.0051434  -114.344    -8.197  
+221022 59874.00 I  0.234655 0.000019  0.217534 0.000023  I-0.0057149 0.0000083  0.6766 0.0048  I  -114.523    1.044    -7.862    0.163  0.234606  0.217522 -0.0057243  -114.532    -7.927  
+221023 59875.00 I  0.232019 0.000015  0.216033 0.000026  I-0.0065072 0.0000070  0.8978 0.0055  I  -114.840    0.896    -7.540    0.137  0.231878  0.216031 -0.0064986  -114.866    -7.589  
+221024 59876.00 I  0.230033 0.000016  0.214646 0.000026  I-0.0074610 0.0000071  0.9706 0.0050  I  -115.124    0.896    -7.301    0.137  0.230043  0.214645 -0.0074339  -115.163    -7.341  
+221025 59877.00 I  0.228137 0.000016  0.213211 0.000023  I-0.0084031 0.0000072  0.9075 0.0050  I  -115.259    0.739    -7.232    0.089  0.228137  0.213232 -0.0084121  -115.318    -7.265  
+221026 59878.00 I  0.226079 0.000016  0.211770 0.000023  I-0.0092495 0.0000071  0.7650 0.0051  I  -115.255    0.739    -7.324    0.089  0.226115  0.211747 -0.0092591  -115.297    -7.349  
+221027 59879.00 I  0.223699 0.000015  0.210386 0.000022  I-0.0098860 0.0000071  0.4812 0.0048  I  -115.194    0.739    -7.484    0.089  0.223756  0.210409 -0.0098856  -115.222    -7.492  
+221028 59880.00 I  0.220829 0.000013  0.208851 0.000022  I-0.0102130 0.0000065  0.2008 0.0054  I  -115.114    0.739    -7.599    0.089  0.220823  0.208832 -0.0102779  -115.143    -7.612  
+221029 59881.00 I  0.217712 0.000013  0.207409 0.000017  I-0.0103254 0.0000081  0.0338 0.0043  I  -114.987    0.748    -7.609    0.051  0.217709  0.207418 -0.0103958  -115.022    -7.628  
+221030 59882.00 I  0.214510 0.000016  0.206265 0.000024  I-0.0102972 0.0000057 -0.0836 0.0047  I  -114.766    0.780    -7.555    0.167  0.214473  0.206229 -0.0103095  -114.810    -7.575  
+221031 59883.00 I  0.211392 0.000016  0.205212 0.000019  I-0.0101973 0.0000049 -0.0839 0.0038  I  -114.440    0.806    -7.516    0.226  0.211345  0.205237 -0.0101927  -114.492    -7.538  
+2211 1 59884.00 I  0.208608 0.000017  0.204242 0.000021  I-0.0101869 0.0000049  0.0882 0.0033  I  -114.044    0.806    -7.509    0.226  0.208514  0.204211 -0.0101774  -114.100    -7.544  
+2211 2 59885.00 I  0.206230 0.000018  0.203468 0.000026  I-0.0104110 0.0000045  0.3720 0.0034  I  -113.657    0.829    -7.483    0.192  0.206235  0.203545 -0.0104065  -113.700    -7.501  
+2211 3 59886.00 I  0.203875 0.000019  0.202379 0.000026  I-0.0109490 0.0000047  0.7099 0.0031  I  -113.378    0.829    -7.392    0.192  0.203841  0.202359 -0.0109528  -113.392    -7.399  
+2211 4 59887.00 I  0.201541 0.000018  0.201374 0.000026  I-0.0118059 0.0000044  0.9730 0.0041  I  -113.284    0.829    -7.243    0.192  0.201477  0.201353 -0.0118134  -113.257    -7.249  
+2211 5 59888.00 I  0.199498 0.000015  0.200681 0.000019  I-0.0128218 0.0000066  1.0165 0.0032  I  -113.375    0.852    -7.059    0.145  0.199403  0.200700 -0.0128173  -113.353    -7.066  
+2211 6 59889.00 I  0.197923 0.000015  0.199801 0.000025  I-0.0138082 0.0000047  0.9680 0.0043  I  -113.545    0.736    -6.862    0.097  0.197880  0.199789 -0.0138349  -113.543    -6.869  
+2211 7 59890.00 I  0.196415 0.000015  0.199008 0.000023  I-0.0147313 0.0000054  0.8401 0.0035  I  -113.642    0.736    -6.683    0.097  0.196436  0.198985 -0.0147274  -113.659    -6.688  
+2211 8 59891.00 I  0.194600 0.000028  0.198378 0.000025  I-0.0154511 0.0000053  0.6003 0.0036  I  -113.614    0.662    -6.585    0.027  0.194574  0.198424 -0.0154466  -113.660    -6.582  
+2211 9 59892.00 I  0.192635 0.000027  0.197577 0.000025  I-0.0159487 0.0000048  0.4110 0.0035  I  -113.553    0.662    -6.626    0.027  0.192696  0.197558 -0.0159684  -113.571    -6.657  
+221110 59893.00 I  0.190360 0.000027  0.196720 0.000025  I-0.0162472 0.0000047  0.1441 0.0032  I  -113.575    0.662    -6.784    0.027  0.190367  0.196722 -0.0162302  -113.564    -6.849  
+221111 59894.00 I  0.187844 0.000027  0.195891 0.000025  I-0.0162361 0.0000041 -0.1252 0.0041  I  -113.643    0.662    -6.941    0.027  0.187822  0.195880 -0.0162520  -113.631    -7.013  
+221112 59895.00 I  0.185418 0.000027  0.195030 0.000018  I-0.0160488 0.0000067 -0.2386 0.0029  I  -113.593    0.739    -6.991    0.002  0.185361  0.195076 -0.0160839  -113.596    -7.056  
+221113 59896.00 I  0.183321 0.000028  0.193962 0.000022  I-0.0157853 0.0000040 -0.2729 0.0038  I  -113.330    0.716    -6.948    0.082  0.183217  0.193981 -0.0158151  -113.352    -6.999  
+221114 59897.00 I  0.181908 0.000014  0.192835 0.000015  I-0.0155290 0.0000034 -0.2294 0.0027  I  -112.924    0.714    -6.924    0.090  0.181786  0.192794 -0.0155444  -112.967    -6.958  
+221115 59898.00 I  0.181149 0.000015  0.192237 0.000015  I-0.0153533 0.0000035 -0.1057 0.0026  I  -112.489    0.714    -6.991    0.090  0.181089  0.192167 -0.0153549  -112.549    -7.008  
+221116 59899.00 I  0.180591 0.000016  0.192106 0.000022  I-0.0153330 0.0000039  0.0641 0.0027  I  -112.067    0.740    -7.083    0.128  0.180613  0.192084 -0.0153236  -112.120    -7.099  
+221117 59900.00 I  0.179829 0.000015  0.192248 0.000023  I-0.0154898 0.0000042  0.2586 0.0029  I  -111.705    0.740    -7.071    0.128  0.179894  0.192217 -0.0154871  -111.735    -7.093  
+221118 59901.00 I  0.178495 0.000016  0.192646 0.000023  I-0.0158574 0.0000044  0.4745 0.0041  I  -111.561    0.740    -6.902    0.128  0.178587  0.192658 -0.0158559  -111.559    -6.936  
+221119 59902.00 I  0.176650 0.000012  0.192925 0.000020  I-0.0164186 0.0000071  0.6297 0.0031  I  -111.786    0.775    -6.640    0.159  0.176631  0.192939 -0.0164100  -111.782    -6.671  
+221120 59903.00 I  0.174676 0.000012  0.192883 0.000023  I-0.0171102 0.0000043  0.7650 0.0041  I  -112.281    0.703    -6.374    0.142  0.174678  0.192941 -0.0171134  -112.283    -6.399  
+221121 59904.00 I  0.172507 0.000012  0.192690 0.000023  I-0.0179166 0.0000042  0.8042 0.0030  I  -112.743    0.703    -6.140    0.142  0.172482  0.192686 -0.0178985  -112.747    -6.164  
+221122 59905.00 I  0.170166 0.000011  0.192510 0.000017  I-0.0186673 0.0000041  0.6894 0.0038  I  -112.971    0.650    -5.974    0.128  0.170135  0.192562 -0.0186627  -112.985    -5.999  
+221123 59906.00 I  0.167914 0.000014  0.192110 0.000035  I-0.0192786 0.0000063  0.5243 0.0038  I  -113.014    0.651    -5.963    0.121  0.167864  0.192125 -0.0192839  -113.015    -5.992  
+221124 59907.00 I  0.165798 0.000014  0.191649 0.000035  I-0.0196865 0.0000064  0.2709 0.0046  I  -112.965    0.651    -6.144    0.121  0.165815  0.191634 -0.0196773  -112.960    -6.178  
+221125 59908.00 I  0.163386 0.000014  0.191406 0.000035  I-0.0198183 0.0000067  0.0111 0.0061  I  -112.800    0.651    -6.380    0.121  0.163449  0.191394 -0.0198119  -112.800    -6.422  
+221126 59909.00 I  0.160411 0.000016  0.191123 0.000034  I-0.0197335 0.0000103 -0.1744 0.0060  I  -112.499    0.651    -6.463    0.113  0.160439  0.191188 -0.0197408  -112.502    -6.504  
+221127 59910.00 I  0.156936 0.000016  0.190783 0.000034  I-0.0195087 0.0000100 -0.2422 0.0064  I  -112.171    0.651    -6.352    0.113  0.156985  0.190819 -0.0195486  -112.173    -6.392  
+221128 59911.00 I  0.153234 0.000016  0.190262 0.000036  I-0.0193018 0.0000077 -0.1519 0.0059  I  -111.942    0.736    -6.211    0.087  0.153168  0.190278 -0.0193141  -111.939    -6.246  
+221129 59912.00 I  0.149942 0.000013  0.189790 0.000016  I-0.0192279 0.0000064  0.0073 0.0047  I  -111.811    0.832    -6.173    0.051  0.149881  0.189736 -0.0192085  -111.789    -6.198  
+221130 59913.00 I  0.147025 0.000017  0.189832 0.000022  I-0.0193202 0.0000054  0.1777 0.0041  I  -111.708    0.751    -6.197    0.094  0.146998  0.189837 -0.0193120  -111.648    -6.204  
+2212 1 59914.00 I  0.144055 0.000021  0.190078 0.000022  I-0.0195939 0.0000051  0.3798 0.0037  I  -111.623    0.751    -6.170    0.094  0.144039  0.190129 -0.0196037  -111.563    -6.191  
+2212 2 59915.00 I  0.141127 0.000021  0.189960 0.000023  I-0.0200307 0.0000051  0.4346 0.0036  I  -111.587    0.751    -6.064    0.094  0.141086  0.190030 -0.0200182  -111.557    -6.103  
+2212 3 59916.00 I  0.138501 0.000021  0.189628 0.000024  I-0.0204323 0.0000051  0.3970 0.0035  I  -111.616    0.751    -5.917    0.094  0.138520  0.189588 -0.0204483  -111.593    -5.954  
+2212 4 59917.00 I  0.135670 0.000022  0.189544 0.000025  I-0.0208113 0.0000048  0.3191 0.0036  I  -111.697    0.814    -5.757    0.131  0.135739  0.189603 -0.0208072  -111.696    -5.787  
+2212 5 59918.00 I  0.132719 0.000023  0.189098 0.000025  I-0.0210310 0.0000050  0.1227 0.0036  I  -111.740    0.814    -5.596    0.131  0.132595  0.189132 -0.0210271  -111.763    -5.625  
+2212 6 59919.00 I  0.130243 0.000023  0.188804 0.000021  I-0.0210519 0.0000053 -0.0881 0.0037  I  -111.650    0.986    -5.494    0.142  0.130234  0.188807 -0.0210546  -111.664    -5.528  
+2212 7 59920.00 I  0.127862 0.000020  0.188834 0.000024  I-0.0208563 0.0000055 -0.2946 0.0039  I  -111.476    0.838    -5.541    0.113  0.127804  0.188914 -0.0208636  -111.530    -5.568  
+2212 8 59921.00 I  0.125542 0.000018  0.188710 0.000023  I-0.0204801 0.0000057 -0.4490 0.0041  I  -111.358    0.838    -5.750    0.113  0.125550  0.188683 -0.0204842  -111.431    -5.765  
+2212 9 59922.00 I  0.123013 0.000018  0.188908 0.000021  I-0.0199683 0.0000061 -0.5733 0.0049  I  -111.367    0.838    -6.002    0.113  0.123051  0.188943 -0.0199575  -111.450    -5.997  
+221210 59923.00 I  0.120044 0.000016  0.189244 0.000016  I-0.0193466 0.0000079 -0.6583 0.0046  I  -111.403    0.680    -6.145    0.074  0.120023  0.189212 -0.0193465  -111.433    -6.148  
+221211 59924.00 I  0.117118 0.000016  0.189440 0.000024  I-0.0186865 0.0000069 -0.6389 0.0052  I  -111.328    0.690    -6.154    0.158  0.117059  0.189519 -0.0187186  -111.306    -6.171  
+221212 59925.00 I  0.114540 0.000014  0.189327 0.000024  I-0.0181000 0.0000069 -0.5260 0.0043  I  -111.104    0.690    -6.137    0.158  0.114474  0.189311 -0.0181257  -111.063    -6.164  
+221213 59926.00 I  0.112258 0.000014  0.189386 0.000024  I-0.0176349 0.0000052 -0.4120 0.0042  I  -110.761    0.814    -6.172    0.193  0.112235  0.189380 -0.0176371  -110.733    -6.213  
+221214 59927.00 I  0.110085 0.000014  0.189773 0.000024  I-0.0172862 0.0000048 -0.2676 0.0034  I  -110.321    0.814    -6.191    0.193  0.110057  0.189733 -0.0172887  -110.324    -6.215  
+221215 59928.00 I  0.107805 0.000014  0.190633 0.000023  I-0.0171043 0.0000043 -0.1095 0.0032  I  -109.852    0.814    -6.076    0.193  0.107848  0.190644 -0.0170929  -109.882    -6.084  
+221216 59929.00 I  0.105273 0.000014  0.191581 0.000023  I-0.0170815 0.0000041  0.0914 0.0030  I  -109.576    0.814    -5.844    0.193  0.105276  0.191662 -0.0170407  -109.642    -5.845  
+221217 59930.00 I  0.102628 0.000011  0.192140 0.000016  I-0.0172736 0.0000041  0.2518 0.0030  I  -109.720    0.903    -5.642    0.178  0.102588  0.192217 -0.0171383  -109.796    -5.644  
+221218 59931.00 I  0.100234 0.000024  0.192465 0.000038  I-0.0175355 0.0000044  0.2635 0.0038  I  -110.233    0.796    -5.555    0.137  0.100160  0.192490 -0.0173664  -110.291    -5.561  
+221219 59932.00 I  0.098289 0.000024  0.192767 0.000037  I-0.0177821 0.0000065  0.2198 0.0031  I  -110.805    0.687    -5.485    0.080  0.098210  0.192803 -0.0177187  -110.824    -5.496  
+221220 59933.00 I  0.096780 0.000026  0.193098 0.000038  I-0.0179687 0.0000045  0.1569 0.0040  I  -111.251    0.630    -5.327    0.078  0.096711  0.193084 -0.0179634  -111.212    -5.340  
+221221 59934.00 I  0.095783 0.000025  0.193369 0.000038  I-0.0180915 0.0000046  0.0808 0.0033  I  -111.661    0.630    -5.201    0.078  0.095777  0.193348 -0.0181234  -111.654    -5.239  
+221222 59935.00 I  0.094827 0.000026  0.194012 0.000039  I-0.0181006 0.0000047 -0.0842 0.0033  I  -112.054    0.630    -5.333    0.078  0.094877  0.193950 -0.0181060  -112.105    -5.394  
+221223 59936.00 I  0.093412 0.000028  0.194949 0.000039  I-0.0179155 0.0000048 -0.2718 0.0033  I  -112.157    0.630    -5.687    0.078  0.093472  0.194922 -0.0178955  -112.150    -5.759  
+221224 59937.00 I  0.091299 0.000019  0.196101 0.000017  I-0.0176065 0.0000047 -0.3109 0.0034  I  -111.801    0.565    -5.935    0.075  0.091397  0.196126 -0.0175841  -111.706    -6.007  
+221225 59938.00 I  0.088380 0.000019  0.197002 0.000016  I-0.0173420 0.0000048 -0.2050 0.0041  I  -111.256    0.565    -5.874    0.075  0.088402  0.197099 -0.0173115  -111.094    -5.943  
+221226 59939.00 I  0.085232 0.000042  0.197368 0.000041  I-0.0172482 0.0000066  0.0561 0.0039  I  -110.922    0.578    -5.678    0.166  0.085204  0.197391 -0.0172323  -110.709    -5.742  
+221227 59940.00 I  0.081991 0.000042  0.197787 0.000041  I-0.0174689 0.0000062  0.3613 0.0044  I  -110.868    0.578    -5.600    0.166  0.082060  0.197809 -0.0174541  -110.623    -5.660  
+221228 59941.00 I  0.078272 0.000044  0.198344 0.000042  I-0.0179183 0.0000057  0.5088 0.0042  I  -110.909    0.656    -5.613    0.153  0.078253  0.198379 -0.0179243  -110.647    -5.673  
+221229 59942.00 I  0.074738 0.000043  0.198601 0.000042  I-0.0184524 0.0000057  0.5538 0.0040  I  -110.946    0.656    -5.528    0.153  0.074744  0.198584 -0.0184719  -110.694    -5.570  
+221230 59943.00 I  0.071203 0.000043  0.199206 0.000041  I-0.0190020 0.0000055  0.5269 0.0040  I  -111.032    0.656    -5.314    0.153  0.071281  0.199199 -0.0190102  -110.793    -5.341  
+221231 59944.00 I  0.067041 0.000043  0.200080 0.000041  I-0.0194825 0.0000057  0.4288 0.0045  I  -111.201    0.656    -5.125    0.153  0.067074  0.200103 -0.0194855  -110.973    -5.182  
+23 1 1 59945.00 I  0.062786 0.000019  0.200919 0.000015  I-0.0198241 0.0000071  0.2244 0.0042  I  -111.392    0.715    -5.058    0.140  0.062699  0.200944 -0.0197967  -111.162    -5.163  
+23 1 2 59946.00 I  0.059055 0.000022  0.201756 0.000023  I-0.0199237 0.0000061 -0.0026 0.0055  I  -111.512    0.573    -5.059    0.097  0.059003  0.201796 -0.0199243  -111.443    -5.114  
+23 1 3 59947.00 I  0.055737 0.000019  0.202460 0.000034  I-0.0198258 0.0000083 -0.2090 0.0053  I  -111.469    0.606    -5.072    0.132  0.055638  0.202514 -0.0198250  -111.467    -5.128  
+23 1 4 59948.00 I  0.052977 0.000019  0.203016 0.000035  I-0.0195029 0.0000087 -0.4239 0.0063  I  -111.218    0.606    -5.156    0.132  0.052933  0.202990 -0.0195007  -111.313    -5.194  
+23 1 5 59949.00 I  0.050803 0.000019  0.203873 0.000036  I-0.0190209 0.0000095 -0.5102 0.0064  I  -110.849    0.606    -5.390    0.132  0.050795  0.203830 -0.0190232  -110.822    -5.531  
+23 1 6 59950.00 I  0.048797 0.000020  0.205075 0.000036  I-0.0185006 0.0000095 -0.5423 0.0066  I  -110.557    0.606    -5.689    0.132  0.048795  0.205101 -0.0184663  -110.510    -5.834  
+23 1 7 59951.00 I  0.046882 0.000019  0.206241 0.000036  I-0.0179517 0.0000093 -0.5281 0.0068  I  -110.422    0.606    -5.873    0.132  0.046853  0.206221 -0.0179143  -110.392    -5.984  
+23 1 8 59952.00 I  0.045143 0.000016  0.207584 0.000032  I-0.0174789 0.0000098 -0.4104 0.0063  I  -110.350    0.816    -5.861    0.177  0.045146  0.207590 -0.0174487  -110.316    -5.948  
+23 1 9 59953.00 I  0.043364 0.000011  0.209053 0.000016  I-0.0171414 0.0000085 -0.2611 0.0063  I  -110.218    0.807    -5.750    0.146  0.043370  0.209111 -0.0171274  -110.159    -5.821  
+23 110 59954.00 I  0.041296 0.000010  0.210242 0.000014  I-0.0169623 0.0000078 -0.0951 0.0055  I  -109.978    0.807    -5.672    0.146  0.041325  0.210288 -0.0169671  -109.874    -5.733  
+23 111 59955.00 I  0.038966 0.000015  0.211106 0.000015  I-0.0169544 0.0000071  0.0806 0.0050  I  -109.660    0.754    -5.624    0.124  0.038979  0.211134 -0.0169747  -109.583    -5.665  
+23 112 59956.00 I  0.036561 0.000014  0.211940 0.000014  I-0.0170840 0.0000062  0.1377 0.0049  I  -109.330    0.754    -5.514    0.124  0.036547  0.211915 -0.0170559  -109.296    -5.533  
+23 113 59957.00 I  0.034182 0.000014  0.213038 0.000014  I-0.0172129 0.0000067  0.1439 0.0059  I  -109.128    0.754    -5.350    0.124  0.034173  0.213022 -0.0172046  -109.147    -5.343  
+23 114 59958.00 I  0.031794 0.000013  0.214424 0.000012  I-0.0173780 0.0000100  0.1685 0.0057  I  -109.206    0.669    -5.284    0.088  0.031810  0.214393 -0.0173877  -109.253    -5.273  
+23 115 59959.00 I  0.029348 0.000016  0.216072 0.000021  I-0.0175473 0.0000092  0.1852 0.0069  I  -109.544    0.637    -5.405    0.113  0.029351  0.216047 -0.0175710  -109.621    -5.396  
+23 116 59960.00 I  0.026873 0.000016  0.217964 0.000021  I-0.0177223 0.0000096  0.1237 0.0073  I  -109.926    0.637    -5.573    0.113  0.026882  0.217923 -0.0177110  -110.037    -5.563  
+23 117 59961.00 I  0.024332 0.000012  0.220219 0.000019  I-0.0177507 0.0000114 -0.0699 0.0070  I  -110.263    0.618    -5.571    0.129  0.024343  0.220214 -0.0177400  -110.403    -5.564  
+23 118 59962.00 I  0.021691 0.000039  0.222446 0.000019  I-0.0175815 0.0000102 -0.2667 0.0075  I  -110.744    0.676    -5.452    0.136  0.021681  0.222504 -0.0175873  -110.857    -5.445  
+23 119 59963.00 I  0.019115 0.000040  0.224215 0.000019  I-0.0172334 0.0000099 -0.4154 0.0071  I  -111.419    0.676    -5.518    0.136  0.019078  0.224261 -0.0172362  -111.474    -5.516  
+23 120 59964.00 I  0.016663 0.000040  0.225636 0.000019  I-0.0167586 0.0000100 -0.5405 0.0081  I  -111.873    0.676    -5.878    0.136  0.016715  0.225678 -0.0167521  -111.849    -5.887  
+23 121 59965.00 I  0.013978 0.000039  0.226843 0.000011  I-0.0161722 0.0000128 -0.6062 0.0061  I  -111.678    0.845    -6.222    0.148  0.014033  0.226892 -0.0161896  -111.635    -6.235  
+23 122 59966.00 I  0.010876 0.000040  0.227751 0.000014  I-0.0156162 0.0000070 -0.4621 0.0072  I  -110.999    0.550    -6.218    0.105  0.010879  0.227740 -0.0156593  -110.964    -6.230  
+23 123 59967.00 I  0.007811 0.000040  0.228860 0.000016  I-0.0152836 0.0000066 -0.2113 0.0047  I  -110.403    0.550    -5.965    0.105  0.007728  0.228830 -0.0153087  -110.393    -5.970  
+23 124 59968.00 I  0.005409 0.000019  0.230211 0.000017  I-0.0152066 0.0000063  0.0787 0.0045  I  -110.171    0.354    -5.799    0.066  0.005300  0.230244 -0.0152158  -110.223    -5.787  
+23 125 59969.00 I  0.003919 0.000023  0.231456 0.000027  I-0.0154123 0.0000062  0.2828 0.0045  I  -110.167    0.569    -5.797    0.149  0.003852  0.231401 -0.0153642  -110.193    -5.799  
+23 126 59970.00 I  0.002888 0.000024  0.233326 0.000029  I-0.0156952 0.0000063  0.2558 0.0043  I  -110.257    0.569    -5.756    0.149  0.002927  0.233231 -0.0156349  -110.268    -5.775  
+23 127 59971.00 I  0.001580 0.000024  0.235870 0.000030  I-0.0159019 0.0000061  0.1627 0.0050  I  -110.440    0.569    -5.596    0.149  0.001593  0.235918 -0.0158886  -110.468    -5.635  
+23 128 59972.00 I  0.000382 0.000022  0.238117 0.000030  I-0.0159939 0.0000077 -0.0105 0.0046  I  -110.658    0.709    -5.505    0.193  0.000279  0.238107 -0.0159862  -110.687    -5.537  
+23 129 59973.00 I -0.000272 0.000026  0.240384 0.000033  I-0.0158863 0.0000070 -0.1675 0.0051  I  -110.780    0.831    -5.637    0.183 -0.000230  0.240378 -0.0158927  -110.794    -5.657  
+23 130 59974.00 I -0.000860 0.000025  0.242657 0.000033  I-0.0156617 0.0000067 -0.3160 0.0051  I  -110.770    0.831    -5.889    0.183 -0.000925  0.242670 -0.0156444  -110.750    -5.905  
+23 131 59975.00 I -0.001399 0.000022  0.245014 0.000026  I-0.0152307 0.0000075 -0.5352 0.0046  I  -110.670    1.146    -6.069    0.163 -0.001326  0.244961 -0.0152262  -110.583    -6.080  
+23 2 1 59976.00 I -0.002309 0.000021  0.247812 0.000044  I-0.0146170 0.0000062 -0.6772 0.0048  I  -110.483    1.038    -6.146    0.176 -0.002296  0.247864 -0.0146010  -110.444    -6.163  
+23 2 2 59977.00 I -0.003561 0.000021  0.250310 0.000044  I-0.0138942 0.0000061 -0.7653 0.0045  I  -110.206    1.038    -6.240    0.176 -0.003547  0.250346 -0.0138591  -110.219    -6.262  
+23 2 3 59978.00 I -0.004904 0.000021  0.252506 0.000043  I-0.0131142 0.0000064 -0.7699 0.0046  I  -109.945    1.038    -6.398    0.176 -0.004856  0.252572 -0.0130960  -109.978    -6.426  
+23 2 4 59979.00 I -0.006471 0.000017  0.254279 0.000041  I-0.0124022 0.0000070 -0.6312 0.0042  I  -109.831    0.944    -6.503    0.187 -0.006428  0.254285 -0.0124190  -109.861    -6.529  
+23 2 5 59980.00 I -0.008209 0.000019  0.255937 0.000041  I-0.0118695 0.0000053 -0.4395 0.0044  I  -109.848    0.729    -6.432    0.154 -0.008204  0.255923 -0.0118777  -109.870    -6.457  
+23 2 6 59981.00 I -0.009960 0.000020  0.257733 0.000041  I-0.0115082 0.0000053 -0.2930 0.0037  I  -109.838    0.729    -6.225    0.154 -0.009964  0.257731 -0.0114958  -109.866    -6.252  
+23 2 7 59982.00 I -0.011916 0.000020  0.259667 0.000017  I-0.0112781 0.0000051 -0.1629 0.0032  I  -109.683    0.541    -6.037    0.116 -0.011876  0.259655 -0.0112745  -109.747    -6.070  
+23 2 8 59983.00 I -0.014092 0.000033  0.261639 0.000038  I-0.0111853 0.0000035 -0.0240 0.0031  I  -109.407    0.739    -5.952    0.086 -0.014175  0.261674 -0.0111959  -109.435    -5.978  
+23 2 9 59984.00 I -0.015723 0.000033  0.263453 0.000038  I-0.0112377 0.0000034  0.1379 0.0026  I  -109.143    0.739    -5.923    0.086 -0.015815  0.263434 -0.0112446  -109.132    -5.933  
+23 210 59985.00 I -0.016726 0.000032  0.265588 0.000038  I-0.0114608 0.0000039  0.2990 0.0031  I  -109.015    0.739    -5.903    0.086 -0.016692  0.265519 -0.0114722  -108.968    -5.888  
+23 211 59986.00 I -0.017893 0.000029  0.268005 0.000037  I-0.0117978 0.0000052  0.3465 0.0029  I  -109.086    0.911    -5.945    0.044 -0.017796  0.268043 -0.0117909  -109.040    -5.942  
+23 212 59987.00 I -0.019635 0.000029  0.270435 0.000037  I-0.0121300 0.0000044  0.3227 0.0034  I  -109.308    0.766    -6.117    0.124 -0.019580  0.270405 -0.0121316  -109.260    -6.133  
+23 213 59988.00 I -0.021943 0.000029  0.273088 0.000038  I-0.0124043 0.0000044  0.1822 0.0035  I  -109.543    0.766    -6.351    0.124 -0.021949  0.273140 -0.0123642  -109.473    -6.379  
+23 214 59989.00 I -0.024483 0.000015  0.275695 0.000018  I-0.0124673 0.0000055 -0.0397 0.0036  I  -109.724    0.669    -6.481    0.163 -0.024489  0.275701 -0.0124632  -109.625    -6.523  
+23 215 59990.00 I -0.026965 0.000028  0.278180 0.000020  I-0.0123414 0.0000058 -0.2120 0.0039  I  -109.979    0.644    -6.487    0.150 -0.026961  0.278194 -0.0123539  -109.980    -6.504  
+23 216 59991.00 I -0.029371 0.000027  0.280690 0.000021  I-0.0120581 0.0000054 -0.3400 0.0040  I  -110.406    0.644    -6.568    0.150 -0.029393  0.280732 -0.0120613  -110.553    -6.554  
+23 217 59992.00 I -0.031759 0.000027  0.282893 0.000023  I-0.0116893 0.0000054 -0.3844 0.0049  I  -110.766    0.644    -6.863    0.150 -0.031780  0.282935 -0.0116902  -111.072    -6.818  
+23 218 59993.00 I -0.033991 0.000025  0.284847 0.000023  I-0.0113602 0.0000081 -0.2161 0.0045  I  -110.672    0.401    -7.189    0.084 -0.034066  0.284869 -0.0113623  -110.935    -7.143  
+23 219 59994.00 I -0.035823 0.000032  0.286845 0.000028  I-0.0113092 0.0000071  0.1087 0.0054  I  -110.105    0.723    -7.250    0.201 -0.035884  0.286825 -0.0113117  -110.257    -7.216  
+23 220 59995.00 I -0.037241 0.000031  0.288962 0.000027  I-0.0115755 0.0000071  0.4273 0.0049  I  -109.463    0.723    -7.046    0.201 -0.037338  0.288920 -0.0115669  -109.509    -7.029  
+23 221 59996.00 I -0.038246 0.000021  0.291495 0.000025  I-0.0121539 0.0000068  0.7162 0.0045  I  -109.083    0.769    -6.853    0.230 -0.038274  0.291422 -0.0121587  -109.019    -6.868  
+23 222 59997.00 I -0.038779 0.000023  0.294616 0.000025  I-0.0129434 0.0000056  0.8116 0.0046  I  -108.997    0.742    -6.809    0.179 -0.038866  0.294588 -0.0129291  -108.925    -6.815  
+23 223 59998.00 I -0.038964 0.000025  0.298256 0.000023  I-0.0137351 0.0000063  0.7809 0.0048  I  -109.136    0.742    -6.788    0.179 -0.038960  0.298263 -0.0137066  -109.077    -6.785  
+23 224 59999.00 I -0.039164 0.000025  0.301855 0.000023  I-0.0144986 0.0000077  0.7305 0.0057  I  -109.461    0.742    -6.697    0.179 -0.039119  0.301926 -0.0145020  -109.413    -6.693  
+23 225 60000.00 I -0.039676 0.000017  0.305101 0.000012  I-0.0151485 0.0000095  0.5375 0.0058  I  -109.838    0.661    -6.674    0.065 -0.039564  0.305114 -0.0151424  -109.790    -6.690  
+23 226 60001.00 I -0.040939 0.000021  0.308169 0.000017  I-0.0155416 0.0000088  0.2486 0.0065  I  -110.068    0.721    -6.866    0.058 -0.040856  0.308232 -0.0155421  -110.020    -6.905  
+23 227 60002.00 I -0.042704 0.000021  0.310720 0.000018  I-0.0156487 0.0000089 -0.0314 0.0076  I  -110.088    0.721    -7.178    0.058 -0.042777  0.310760 -0.0156050  -110.045    -7.236  
+23 228 60003.00 I -0.044028 0.000020  0.313321 0.000018  I-0.0155140 0.0000125 -0.2059 0.0064  I  -109.978    0.881    -7.382    0.021 -0.044051  0.313293 -0.0155019  -109.938    -7.454  
+23 3 1 60004.00 I -0.045094 0.000019  0.316290 0.000019  I-0.0152981 0.0000093 -0.1968 0.0073  I  -109.760    0.860    -7.398    0.122 -0.045086  0.316379 -0.0152786  -109.729    -7.431  
+23 3 2 60005.00 I -0.046059 0.000018  0.318742 0.000019  I-0.0151048 0.0000077 -0.2343 0.0059  I  -109.391    0.860    -7.357    0.122                                                     
+23 3 3 60006.00 I -0.046662 0.000016  0.321114 0.000019  I-0.0148428 0.0000074 -0.2317 0.0053  I  -108.939    0.860    -7.396    0.122                                                     
+23 3 4 60007.00 I -0.046920 0.000012  0.323798 0.000016  I-0.0146892 0.0000072 -0.0856 0.0049  I  -108.601    0.815    -7.476    0.217                                                     
+23 3 5 60008.00 I -0.046594 0.000036  0.326590 0.000019  I-0.0146899 0.0000065  0.1155 0.0047  I  -108.485    0.909    -7.452    0.104                                                     
+23 3 6 60009.00 I -0.045655 0.000037  0.329778 0.000018  I-0.0149303 0.0000060  0.3471 0.0047  I  -108.494    0.909    -7.280    0.104                                                     
+23 3 7 60010.00 I -0.044607 0.000036  0.333305 0.000017  I-0.0153729 0.0000068  0.5452 0.0040  I  -108.473    0.929    -7.082    0.044                                                     
+23 3 8 60011.00 I -0.043512 0.000037  0.336633 0.000016  I-0.0160144 0.0000054  0.7245 0.0042  I  -108.402    0.795    -7.004    0.038                                                     
+23 3 9 60012.00 I -0.042352 0.000037  0.339812 0.000016  I-0.0167934 0.0000050  0.8182 0.0036  I  -108.377    0.795    -7.072    0.038                                                     
+23 310 60013.00 I -0.041303 0.000037  0.343079 0.000015  I-0.0176197 0.0000048  0.8185 0.0031  I  -108.451    0.795    -7.207    0.038                                                     
+23 311 60014.00 I -0.040750 0.000013  0.346411 0.000009  I-0.0184076 0.0000038  0.7504 0.0035  I  -108.577    0.697    -7.341    0.034                                                     
+23 312 60015.00 I -0.040529 0.000013  0.349519 0.000010  I-0.0190955 0.0000050  0.6074 0.0032  I  -108.692    0.740    -7.472    0.052                                                     
+23 313 60016.00 I -0.040089 0.000013  0.352556 0.000010  I-0.0195973 0.0000052  0.3892 0.0041  I  -108.759    0.740    -7.613    0.052                                                     
+23 314 60017.00 I -0.039702 0.000014  0.355962 0.000012  I-0.0199053 0.0000064  0.2651 0.0040  I  -108.752    0.812    -7.748    0.072                                                     
+23 315 60018.00 I -0.039676 0.000014  0.359426 0.000012  I-0.0201092 0.0000062  0.0860 0.0045  I  -108.662    0.812    -7.869    0.072                                                     
+23 316 60019.00 I -0.039798 0.000013  0.362273 0.000012  I-0.0200828 0.0000063 -0.0765 0.0043  I  -108.523    0.812    -8.015    0.072                                                     
+23 317 60020.00 I -0.039667 0.000012  0.364618 0.000012  I-0.0200346 0.0000061 -0.0039 0.0045  I  -108.359    0.812    -8.204    0.072                                                     
+23 318 60021.00 I -0.039055 0.000011  0.366839 0.000011  I-0.0201205 0.0000064  0.2053 0.0036  I  -108.157    0.322    -8.346    0.160                                                     
+23 319 60022.00 I -0.038098 0.000013  0.368982 0.000012  I-0.0204823 0.0000038  0.5260 0.0037  I  -107.940    0.618    -8.312    0.078                                                     
+23 320 60023.00 I -0.036912 0.000009  0.371252 0.000008  I-0.0211481 0.0000037  0.7737 0.0027  I  -107.779    0.618    -8.122    0.078                                                     
+23 321 60024.00 I -0.035479 0.000009  0.373933 0.000008  I-0.0219994 0.0000037  0.9307 0.0029  I  -107.712    0.618    -7.952    0.078                                                     
+23 322 60025.00 I -0.033921 0.000012  0.377070 0.000012  I-0.0229696 0.0000045  0.9681 0.0030  I  -107.716    0.707    -7.911    0.051                                                     
+23 323 60026.00 I -0.032493 0.000012  0.380217 0.000013  I-0.0238906 0.0000046  0.8705 0.0033  I  -107.807    0.707    -7.942    0.051                                                     
+23 324 60027.00 I -0.031182 0.000011  0.383297 0.000013  I-0.0246833 0.0000048  0.6911 0.0036  I  -108.032    0.707    -7.964    0.051                                                     
+23 325 60028.00 I -0.029863 0.000009  0.386398 0.000013  I-0.0252281 0.0000056  0.3777 0.0033  I  -108.331    0.760    -8.024    0.019                                                     
+23 326 60029.00 I -0.028393 0.000014  0.389489 0.000018  I-0.0254387 0.0000045  0.0642 0.0036  I  -108.543    0.803    -8.200    0.111                                                     
+23 327 60030.00 I -0.026607 0.000014  0.392602 0.000018  I-0.0253946 0.0000045 -0.1350 0.0035  I  -108.576    0.803    -8.441    0.111                                                     
+23 328 60031.00 I -0.024709 0.000013  0.395453 0.000016  I-0.0251881 0.0000054 -0.2759 0.0033  I  -108.466    0.855    -8.595    0.160                                                     
+23 329 60032.00 I -0.023045 0.000016  0.397855 0.000020  I-0.0248770 0.0000049 -0.3142 0.0038  I  -108.236    0.748    -8.615    0.111                                                     
+23 330 60033.00 I -0.021724 0.000019  0.400028 0.000021  I-0.0245949 0.0000053 -0.2468 0.0041  I  -107.846    0.748    -8.609    0.111                                                     
+23 331 60034.00 I -0.020386 0.000020  0.402185 0.000021  I-0.0243988 0.0000066 -0.1332 0.0051  I  -107.337    0.748    -8.700    0.111                                                     
+23 4 1 60035.00 I -0.018859 0.000018  0.404604 0.000018  I-0.0243379 0.0000086  0.0086 0.0052  I  -106.905    0.681    -8.858    0.021                                                     
+23 4 2 60036.00 I -0.017328 0.000019  0.407371 0.000020  I-0.0244346 0.0000080  0.2062 0.0057  I  -106.739    0.752    -8.927    0.064                                                     
+23 4 3 60037.00 I -0.015623 0.000019  0.409983 0.000020  I-0.0247491 0.0000074  0.4001 0.0057  I  -106.831    0.752    -8.808    0.064                                                     
+23 4 4 60038.00 I -0.013828 0.000019  0.412632 0.000017  I-0.0252205 0.0000080  0.5511 0.0053  I  -107.017    0.827    -8.572    0.091                                                     
+23 4 5 60039.00 I -0.012262 0.000015  0.415452 0.000016  I-0.0258395 0.0000075  0.6668 0.0045  I  -107.171    0.827    -8.392    0.091                                                     
+23 4 6 60040.00 I -0.010695 0.000014  0.418299 0.000015  I-0.0265260 0.0000042  0.6982 0.0042  I  -107.290    0.827    -8.375    0.091                                                     
+23 4 7 60041.00 I -0.009135 0.000016  0.421177 0.000016  I-0.0272234 0.0000037  0.6921 0.0027  I  -107.415    0.827    -8.494    0.091                                                     
+23 4 8 60042.00 I -0.007828 0.000017  0.423799 0.000013  I-0.0278895 0.0000035  0.6238 0.0034  I  -107.547    0.623    -8.646    0.041                                                     
+23 4 9 60043.00 I -0.006576 0.000020  0.426300 0.000014  I-0.0284459 0.0000056  0.4801 0.0051  I  -107.663    0.623    -8.762    0.041                                                     
+23 410 60044.00 I -0.005292 0.000021  0.428820 0.000031  I-0.0288332 0.0000096  0.2869 0.0052  I  -107.737    0.807    -8.850    0.052                                                     
+23 411 60045.00 I -0.004038 0.000023  0.431406 0.000037  I-0.0290175 0.0000088  0.0872 0.0067  I  -107.717    0.807    -8.951    0.052                                                     
+23 412 60046.00 I -0.002990 0.000027  0.434157 0.000046  I-0.0290319 0.0000094 -0.0397 0.0061  I  -107.512    0.807    -9.085    0.052                                                     
+23 413 60047.00 I -0.002338 0.000032  0.436744 0.000045  I-0.0289827 0.0000085 -0.0327 0.0062  P  -107.117    0.278    -9.229    0.145                                                     
+23 414 60048.00 I -0.001819 0.000034  0.439283 0.000045  I-0.0290127 0.0000081  0.1129 0.0059  P  -106.640    0.288    -9.330    0.148                                                     
+23 415 60049.00 I -0.001066 0.000090  0.441657 0.000092  I-0.0292411 0.0000083  0.3561 0.0060  P  -106.290    0.297    -9.328    0.151                                                     
+23 416 60050.00 I  0.000200 0.000091  0.443585 0.000091  I-0.0297580 0.0000089  0.6984 0.0062  P  -106.224    0.304    -9.210    0.154                                                     
+23 417 60051.00 I  0.001657 0.000090  0.445290 0.000092  I-0.0306114 0.0000093  0.9611 0.0061  P  -106.421    0.309    -9.026    0.155                                                     
+23 418 60052.00 I  0.002987 0.000090  0.446940 0.000092  I-0.0316040 0.0000082  0.9952 0.0062  P  -106.720    0.313    -8.867    0.157                                                     
+23 419 60053.00 I  0.004305 0.000091  0.448616 0.000091  I-0.0325574 0.0000083  0.8959 0.0061  P  -106.960    0.316    -8.786    0.158                                                     
+23 420 60054.00 I  0.005764 0.000091  0.450465 0.000091  I-0.0333667 0.0000089  0.7091 0.0070  P  -107.104    0.318    -8.775    0.158                                                     
+23 421 60055.00 I  0.007427 0.000091  0.452647 0.000091  I-0.0339484 0.0000113  0.4405 0.0076  P  -107.221    0.319    -8.817    0.159                                                     
+23 422 60056.00 I  0.009113 0.000091  0.455146 0.000091  I-0.0342550 0.0000123  0.1938 0.0080  P  -107.362    0.320    -8.923    0.159                                                     
+23 423 60057.00 I  0.010750 0.000091  0.457872 0.000090  I-0.0343540 0.0000114  0.0011 0.0080  P  -107.498    0.321    -9.092    0.160                                                     
+23 424 60058.00 I  0.012658 0.000090  0.460576 0.000091  I-0.0342664 0.0000101 -0.1641 0.0077  P  -107.563    0.321    -9.258    0.160                                                     
+23 425 60059.00 I  0.014958 0.000091  0.462922 0.000093  I-0.0340566 0.0000105 -0.2370 0.0073  P  -107.516    0.321    -9.342    0.160                                                     
+23 426 60060.00 I  0.017303 0.000091  0.465025 0.000091  I-0.0338232 0.0000106 -0.2177 0.0066  P  -107.336    0.321    -9.352    0.160                                                     
+23 427 60061.00 I  0.019415 0.000090  0.467238 0.000090  I-0.0336324 0.0000079                 P  -107.006    0.322    -9.390    0.160                                                     
+23 428 60062.00 P  0.021500 0.000609  0.469218 0.000465  P-0.0335307 0.0001080                 P  -106.558    0.322    -9.531    0.160                                                     
+23 429 60063.00 P  0.023535 0.000904  0.471236 0.000766  P-0.0335677 0.0002041                 P  -106.134    0.322    -9.719    0.160                                                     
+23 430 60064.00 P  0.025626 0.001139  0.473071 0.001025  P-0.0337684 0.0003028                 P  -105.930    0.322    -9.802    0.160                                                     
+23 5 1 60065.00 P  0.027749 0.001342  0.474787 0.001261  P-0.0341255 0.0004021                 P  -106.055    0.322    -9.681    0.160                                                     
+23 5 2 60066.00 P  0.029939 0.001524  0.476435 0.001481  P-0.0346244 0.0005017                 P  -106.433    0.322    -9.411    0.160                                                     
+23 5 3 60067.00 P  0.032223 0.001691  0.478048 0.001689  P-0.0352347 0.0006014                 P  -106.862    0.322    -9.145    0.160                                                     
+23 5 4 60068.00 P  0.034596 0.001846  0.479640 0.001887  P-0.0358935 0.0007012                 P  -107.183    0.322    -9.009    0.160                                                     
+23 5 5 60069.00 P  0.037027 0.001992  0.481213 0.002078  P-0.0364921 0.0007500                 P  -107.387    0.322    -9.031    0.160                                                     
+23 5 6 60070.00 P  0.039491 0.002130  0.482773 0.002262  P-0.0369163 0.0005500                 P  -107.567    0.322    -9.170    0.160                                                     
+23 5 7 60071.00 P  0.041976 0.002262  0.484298 0.002440  P-0.0370816 0.0007548                 P  -107.770    0.322    -9.368    0.160                                                     
+23 5 8 60072.00 P  0.044471 0.002388  0.485767 0.002613  P-0.0370035 0.0009344                 P  -107.919    0.322    -9.572    0.160                                                     
+23 5 9 60073.00 P  0.046977 0.002510  0.487192 0.002782  P-0.0367542 0.0010994                 P  -107.884    0.322    -9.740    0.160                                                     
+23 510 60074.00 P  0.049509 0.002627  0.488582 0.002947  P-0.0364366 0.0012543                 P  -107.610    0.322    -9.846    0.160                                                     
+23 511 60075.00 P  0.052068 0.002740  0.489930 0.003109  P-0.0361623 0.0014016                 P  -107.176    0.322    -9.889    0.160                                                     
+23 512 60076.00 P  0.054642 0.002850  0.491231 0.003267  P-0.0360305 0.0015429                 P  -106.735    0.322    -9.875    0.160                                                     
+23 513 60077.00 P  0.057230 0.002957  0.492483 0.003422  P-0.0361034 0.0016792                 P  -106.431    0.322    -9.806    0.160                                                     
+23 514 60078.00 P  0.059836 0.003061  0.493689 0.003575  P-0.0364047 0.0018113                 P  -106.341    0.322    -9.687    0.160                                                     
+23 515 60079.00 P  0.062464 0.003162  0.494848 0.003725  P-0.0368909 0.0019399                 P  -106.468    0.322    -9.531    0.160                                                     
+23 516 60080.00 P  0.065116 0.003261  0.495960 0.003873  P-0.0374412 0.0020652                 P  -106.743    0.322    -9.351    0.160                                                     
+23 517 60081.00 P  0.067793 0.003358  0.497026 0.004019  P-0.0379318 0.0021877                 P  -107.050    0.322    -9.174    0.160                                                     
+23 518 60082.00 P  0.070491 0.003453  0.498050 0.004163  P-0.0382537 0.0023077                 P  -107.269    0.322    -9.054    0.160                                                     
+23 519 60083.00 P  0.073209 0.003545  0.499036 0.004304  P-0.0383224 0.0024255                 P  -107.352    0.322    -9.061    0.160                                                     
+23 520 60084.00 P  0.075944 0.003636  0.499982 0.004444  P-0.0380999 0.0025411                 P  -107.355    0.322    -9.222    0.160                                                     
+23 521 60085.00 P  0.078692 0.003726  0.500888 0.004583  P-0.0376153 0.0026548                 P  -107.379    0.322    -9.471    0.160                                                     
+23 522 60086.00 P  0.081452 0.003813  0.501753 0.004719  P-0.0369379 0.0027668                 P  -107.461    0.322    -9.677    0.160                                                     
+23 523 60087.00 P  0.084224 0.003900  0.502576 0.004855  P-0.0361511 0.0028772                 P  -107.552    0.322    -9.754    0.160                                                     
+23 524 60088.00 P  0.087007 0.003984  0.503355 0.004988  P-0.0353369 0.0029860                 P  -107.581    0.322    -9.748    0.160                                                     
+23 525 60089.00 P  0.089800 0.004068  0.504090 0.005121  P-0.0345677 0.0030934                 P  -107.508    0.322    -9.780    0.160                                                     
+23 526 60090.00 P  0.092604 0.004150  0.504783 0.005252  P-0.0339047 0.0031995                 P  -107.312    0.322    -9.904    0.160                                                     
+23 527 60091.00 P  0.095417 0.004231  0.505432 0.005381  P-0.0333877 0.0033043                 P  -107.017    0.322   -10.030    0.160                                                     
+23 528 60092.00 P  0.098239 0.004311  0.506037 0.005510  P-0.0330278 0.0034080                 P  -106.763    0.322   -10.018    0.160                                                     
+23 529 60093.00 P  0.101069 0.004390  0.506598 0.005637  P-0.0328174 0.0035105                 P  -106.784    0.322    -9.825    0.160                                                     
+23 530 60094.00 P  0.103906 0.004467  0.507115 0.005764  P-0.0327199 0.0036120                 P  -107.211    0.322    -9.546    0.160                                                     
+23 531 60095.00 P  0.106750 0.004544  0.507589 0.005889  P-0.0326785 0.0037124                 P  -107.889    0.322    -9.304    0.160                                                     
+23 6 1 60096.00 P  0.109601 0.004620  0.508019 0.006013  P-0.0326131 0.0038119                 P  -108.498    0.322    -9.148    0.160                                                     
+23 6 2 60097.00 P  0.112457 0.004694  0.508407 0.006136  P-0.0324290 0.0039105                 P  -108.877    0.322    -9.082    0.160                                                     
+23 6 3 60098.00 P  0.115317 0.004768  0.508750 0.006259  P-0.0320484 0.0040082                 P  -109.134    0.322    -9.140    0.160                                                     
+23 6 4 60099.00 P  0.118180 0.004841  0.509051 0.006380  P-0.0314371 0.0041051                 P  -109.381    0.322    -9.359    0.160                                                     
+23 6 5 60100.00 P  0.121046 0.004913  0.509308 0.006500  P-0.0306248 0.0042012                 P  -109.512    0.322    -9.662    0.160                                                     
+23 6 6 60101.00 P  0.123913 0.004985  0.509522 0.006620  P-0.0297054 0.0042965                 P  -109.359    0.322    -9.875    0.160                                                     
+23 6 7 60102.00 P  0.126782 0.005056  0.509692 0.006739  P-0.0288150 0.0043911                 P  -108.978    0.322    -9.887    0.160                                                     
+23 6 8 60103.00 P  0.129650 0.005125  0.509818 0.006857  P-0.0280774 0.0044849                 P  -108.642    0.322    -9.755    0.160                                                     
+23 6 9 60104.00 P  0.132518 0.005195  0.509901 0.006974  P-0.0275749 0.0045781                 P  -108.551    0.322    -9.608    0.160                                                     
+23 610 60105.00 P  0.135384 0.005263  0.509940 0.007090  P-0.0273112 0.0046706                 P  -108.661    0.322    -9.507    0.160                                                     
+23 611 60106.00 P  0.138249 0.005331  0.509935 0.007206  P-0.0272236 0.0047625                 P  -108.809    0.322    -9.424    0.160                                                     
+23 612 60107.00 P  0.141110 0.005398  0.509887 0.007321  P-0.0272054 0.0048537                 P  -108.920    0.322    -9.315    0.160                                                     
+23 613 60108.00 P  0.143968 0.005465  0.509796 0.007435  P-0.0271323 0.0049444                 P  -109.070    0.322    -9.157    0.160                                                     
+23 614 60109.00 P  0.146822 0.005531  0.509661 0.007549  P-0.0268981 0.0050344                 P  -109.341    0.322    -8.969    0.160                                                     
+23 615 60110.00 P  0.149671 0.005596  0.509483 0.007662  P-0.0264294 0.0051240                 P  -109.673    0.322    -8.825    0.160                                                     
+23 616 60111.00 P  0.152514 0.005661  0.509262 0.007774  P-0.0256968 0.0052129                 P  -109.909    0.322    -8.838    0.160                                                     
+23 617 60112.00 P  0.155350 0.005725  0.508999 0.007885  P-0.0247123 0.0053014                 P  -109.979    0.322    -9.073    0.160                                                     
+23 618 60113.00 P  0.158179 0.005789  0.508692 0.007996  P-0.0235275 0.0053893                 P  -109.974    0.322    -9.446    0.160                                                     
+23 619 60114.00 P  0.161001 0.005852  0.508342 0.008107  P-0.0222220 0.0054768                 P  -110.025    0.322    -9.752    0.160                                                     
+23 620 60115.00 P  0.163813 0.005915  0.507950 0.008217  P-0.0208764 0.0055637                 P  -110.165    0.322    -9.831    0.160                                                     
+23 621 60116.00 P  0.166616 0.005977  0.507516 0.008326  P-0.0195681 0.0056502                 P  -110.343    0.322    -9.712    0.160                                                     
+23 622 60117.00 P  0.169408 0.006039  0.507039 0.008435  P-0.0183613 0.0057362                 P  -110.499    0.322    -9.571    0.160                                                     
+23 623 60118.00 P  0.172189 0.006100  0.506520 0.008543  P-0.0172940 0.0058218                 P  -110.557    0.322    -9.521    0.160                                                     
+23 624 60119.00 P  0.174959 0.006161  0.505960 0.008650  P-0.0163799 0.0059070                 P  -110.442    0.322    -9.496    0.160                                                     
+23 625 60120.00 P  0.177717 0.006221  0.505357 0.008758  P-0.0156112 0.0059917                 P  -110.208    0.322    -9.370    0.160                                                     
+23 626 60121.00 P  0.180461 0.006281  0.504713 0.008864  P-0.0149551 0.0060760                 P  -110.142    0.322    -9.142    0.160                                                     
+23 627 60122.00 P  0.183191 0.006340  0.504028 0.008970  P-0.0143643 0.0061599                 P  -110.555    0.322    -8.958    0.160                                                     
+23 628 60123.00 P  0.185907 0.006399  0.503302 0.009076  P-0.0137728 0.0062434                 P  -111.413    0.322    -8.925    0.160                                                     
+23 629 60124.00 P  0.188608 0.006458  0.502535 0.009181  P-0.0130994 0.0063266                 P  -112.302    0.322    -8.979    0.160                                                     
+23 630 60125.00 P  0.191292 0.006516  0.501727 0.009286  P-0.0122650 0.0064093                 P  -112.871    0.322    -9.003    0.160                                                     
+23 7 1 60126.00 P  0.193960 0.006574  0.500880 0.009390  P-0.0112211 0.0064917                 P  -113.141    0.322    -9.026    0.160                                                     
+23 7 2 60127.00 P  0.196611 0.006632  0.499992 0.009494  P-0.0099751 0.0065737                 P  -113.269    0.322    -9.183    0.160                                                     
+23 7 3 60128.00 P  0.199244 0.006689  0.499064 0.009597  P-0.0085984 0.0066554                 P  -113.215    0.322    -9.455    0.160                                                     
+23 7 4 60129.00 P  0.201858 0.006745  0.498098 0.009700  P-0.0072181 0.0067368                 P  -112.895    0.322    -9.621    0.160                                                     
+23 7 5 60130.00 P  0.204452 0.006802  0.497092 0.009803  P-0.0059789 0.0068177                 P  -112.498    0.322    -9.531    0.160                                                     
+23 7 6 60131.00 P  0.207027 0.006858  0.496047 0.009905  P-0.0049909 0.0068984                 P  -112.373    0.322    -9.315    0.160                                                     
+23 7 7 60132.00 P  0.209581 0.006914  0.494964 0.010006  P-0.0042882 0.0069788                 P  -112.639    0.322    -9.189    0.160                                                     
+23 7 8 60133.00 P  0.212114 0.006969  0.493842 0.010108  P-0.0038173 0.0070588                 P  -113.093    0.322    -9.180    0.160                                                     
+23 7 9 60134.00 P  0.214624 0.007024  0.492683 0.010209  P-0.0034636 0.0071385                 P  -113.469    0.322    -9.160    0.160                                                     
+23 710 60135.00 P  0.217112 0.007079  0.491486 0.010309  P-0.0030867 0.0072179                 P  -113.667    0.322    -9.067    0.160                                                     
+23 711 60136.00 P  0.219577 0.007133  0.490253 0.010409  P-0.0025646 0.0072970                 P  -113.773    0.322    -8.960    0.160                                                     
+23 712 60137.00 P  0.222018 0.007187  0.488982 0.010509  P-0.0018183 0.0073758                                                                                                             
+23 713 60138.00 P  0.224435 0.007241  0.487676 0.010608  P-0.0008148 0.0074544                                                                                                             
+23 714 60139.00 P  0.226826 0.007294  0.486333 0.010707  P 0.0004295 0.0075326                                                                                                             
+23 715 60140.00 P  0.229192 0.007347  0.484955 0.010806  P 0.0018653 0.0076106                                                                                                             
+23 716 60141.00 P  0.231532 0.007400  0.483542 0.010904  P 0.0034216 0.0076883                                                                                                             
+23 717 60142.00 P  0.233844 0.007453  0.482094 0.011002  P 0.0050178 0.0077657                                                                                                             
+23 718 60143.00 P  0.236130 0.007505  0.480612 0.011100  P 0.0065759 0.0078428                                                                                                             
+23 719 60144.00 P  0.238387 0.007557  0.479096 0.011197  P 0.0080291 0.0079197                                                                                                             
+23 720 60145.00 P  0.240616 0.007609  0.477547 0.011294  P 0.0093314 0.0079964                                                                                                             
+23 721 60146.00 P  0.242815 0.007660  0.475964 0.011391  P 0.0104615 0.0080728                                                                                                             
+23 722 60147.00 P  0.244985 0.007712  0.474350 0.011487  P 0.0114255 0.0081489                                                                                                             
+23 723 60148.00 P  0.247125 0.007763  0.472703 0.011583  P 0.0122537 0.0082248                                                                                                             
+23 724 60149.00 P  0.249234 0.007813  0.471025 0.011679  P 0.0129944 0.0083005                                                                                                             
+23 725 60150.00 P  0.251311 0.007864  0.469316 0.011774  P 0.0137082 0.0083759                                                                                                             
+23 726 60151.00 P  0.253357 0.007914  0.467576 0.011869  P 0.0144644 0.0084511                                                                                                             
+23 727 60152.00 P  0.255371 0.007964  0.465806 0.011964  P 0.0153333 0.0085261                                                                                                             
+23 728 60153.00 P  0.257352 0.008014  0.464007 0.012059  P 0.0163704 0.0086008                                                                                                             
+23 729 60154.00 P  0.259299 0.008063  0.462179 0.012153  P 0.0175943 0.0086754                                                                                                             
+23 730 60155.00 P  0.261213 0.008113  0.460322 0.012247  P 0.0189649 0.0087497                                                                                                             
+23 731 60156.00 P  0.263093 0.008162  0.458437 0.012341  P 0.0203776 0.0088237                                                                                                             
+23 8 1 60157.00 P  0.264938 0.008211  0.456525 0.012434  P 0.0216850 0.0088976                                                                                                             
+23 8 2 60158.00 P  0.266748 0.008259  0.454586 0.012527  P 0.0227443 0.0089713                                                                                                             
+23 8 3 60159.00 P  0.268522 0.008308  0.452621 0.012620  P 0.0234766 0.0090448                                                                                                             
+23 8 4 60160.00 P  0.270261 0.008356  0.450629 0.012712  P 0.0238991 0.0091180                                                                                                             
+23 8 5 60161.00 P  0.271963 0.008404  0.448613 0.012805  P 0.0241204 0.0091911                                                                                                             
+23 8 6 60162.00 P  0.273628 0.008452  0.446572 0.012897  P 0.0243034 0.0092639                                                                                                             
+23 8 7 60163.00 P  0.275258 0.008499  0.444505 0.012989  P 0.0246031 0.0093366                                                                                                             
+23 8 8 60164.00 P  0.276849 0.008547  0.442414 0.013080  P 0.0251257 0.0094091                                                                                                             
+23 8 9 60165.00 P  0.278403 0.008594  0.440300 0.013172  P 0.0259117 0.0094814                                                                                                             
+23 810 60166.00 P  0.279919 0.008641  0.438164 0.013263  P 0.0269440 0.0095535                                                                                                             
+23 811 60167.00 P  0.281396 0.008688  0.436007 0.013353  P 0.0281671 0.0096254                                                                                                             
+23 812 60168.00 P  0.282834 0.008734  0.433828 0.013444  P 0.0295067 0.0096971                                                                                                             
+23 813 60169.00 P  0.284232 0.008781  0.431628 0.013534  P 0.0308811 0.0097686                                                                                                             
+23 814 60170.00 P  0.285591 0.008827  0.429409 0.013624  P 0.0322409 0.0098400                                                                                                             
+23 815 60171.00 P  0.286910 0.008873  0.427171 0.013714  P 0.0334934 0.0099112                                                                                                             
+23 816 60172.00 P  0.288189 0.008919  0.424914 0.013804  P 0.0345874 0.0099822                                                                                                             
+23 817 60173.00 P  0.289428 0.008965  0.422639 0.013893  P 0.0354956 0.0100531                                                                                                             
+23 818 60174.00 P  0.290625 0.009010  0.420346 0.013983  P 0.0362182 0.0101238                                                                                                             
+23 819 60175.00 P  0.291782 0.009056  0.418037 0.014072  P 0.0367833 0.0101943                                                                                                             
+23 820 60176.00 P  0.292897 0.009101  0.415712 0.014160  P 0.0372418 0.0102646                                                                                                             
+23 821 60177.00 P  0.293971 0.009146  0.413371 0.014249  P 0.0376592 0.0103348                                                                                                             
+23 822 60178.00 P  0.295003 0.009191  0.411015 0.014337  P 0.0381063 0.0104048                                                                                                             
+23 823 60179.00 P  0.295993 0.009235  0.408645 0.014425  P 0.0386494 0.0104747                                                                                                             
+23 824 60180.00 P  0.296941 0.009280  0.406262 0.014513  P 0.0393405 0.0105444                                                                                                             
+23 825 60181.00 P  0.297846 0.009324  0.403865 0.014601  P 0.0402031 0.0106139                                                                                                             
+23 826 60182.00 P  0.298709 0.009368  0.401457 0.014689  P 0.0412161 0.0106833                                                                                                             
+23 827 60183.00 P  0.299530 0.009413  0.399037 0.014776  P 0.0423017 0.0107526                                                                                                             
+23 828 60184.00 P  0.300307 0.009456  0.396606 0.014863  P 0.0433319 0.0108216                                                                                                             
+23 829 60185.00 P  0.301041 0.009500  0.394165 0.014950  P 0.0441596 0.0108906                                                                                                             
+23 830 60186.00 P  0.301732 0.009544  0.391714 0.015037  P 0.0446683 0.0109594                                                                                                             
+23 831 60187.00 P  0.302380 0.009587  0.389254 0.015123  P 0.0448220 0.0110280                                                                                                             
+23 9 1 60188.00 P  0.302985 0.009631  0.386786 0.015209  P 0.0446878 0.0110965                                                                                                             
+23 9 2 60189.00 P  0.303546 0.009674  0.384310 0.015296  P 0.0444152 0.0111649                                                                                                             
+23 9 3 60190.00 P  0.304063 0.009717  0.381828 0.015381  P 0.0441848 0.0112331                                                                                                             
+23 9 4 60191.00 P  0.304537 0.009760  0.379339 0.015467  P 0.0441487 0.0113012                                                                                                             
+23 9 5 60192.00 P  0.304967 0.009802  0.376845 0.015553  P 0.0443903 0.0113691                                                                                                             
+23 9 6 60193.00 P  0.305353 0.009845  0.374345 0.015638  P 0.0449160 0.0114369                                                                                                             
+23 9 7 60194.00 P  0.305695 0.009887  0.371842 0.015723  P 0.0456738 0.0115046                                                                                                             
+23 9 8 60195.00 P  0.305994 0.009930  0.369335 0.015808  P 0.0465813 0.0115721                                                                                                             
+23 9 9 60196.00 P  0.306249 0.009972  0.366825 0.015893  P 0.0475482 0.0116395                                                                                                             
+23 910 60197.00 P  0.306459 0.010014  0.364313 0.015978  P 0.0484896 0.0117067                                                                                                             
+23 911 60198.00 P  0.306626 0.010056  0.361799 0.016062  P 0.0493323 0.0117739                                                                                                             
+23 912 60199.00 P  0.306750 0.010097  0.359285 0.016147  P 0.0500210 0.0118409                                                                                                             
+23 913 60200.00 P  0.306829 0.010139  0.356770 0.016231  P 0.0505217 0.0119077                                                                                                             
+23 914 60201.00 P  0.306865 0.010181  0.354256 0.016315  P 0.0508275 0.0119745                                                                                                             
+23 915 60202.00 P  0.306856 0.010222  0.351743 0.016399  P 0.0509594 0.0120411                                                                                                             
+23 916 60203.00 P  0.306805 0.010263  0.349232 0.016482  P 0.0509650 0.0121076                                                                                                             
+23 917 60204.00 P  0.306709 0.010304  0.346723 0.016566  P 0.0509108 0.0121740                                                                                                             
+23 918 60205.00 P  0.306571 0.010345  0.344218 0.016649  P 0.0508729 0.0122402                                                                                                             
+23 919 60206.00 P  0.306389 0.010386  0.341716 0.016732  P 0.0509240 0.0123063                                                                                                             
+23 920 60207.00 P  0.306163 0.010427  0.339218 0.016815  P 0.0511197 0.0123723                                                                                                             
+23 921 60208.00 P  0.305895 0.010468  0.336726 0.016898  P 0.0514866 0.0124382                                                                                                             
+23 922 60209.00 P  0.305584 0.010508  0.334240 0.016981  P 0.0520114 0.0125040                                                                                                             
+23 923 60210.00 P  0.305229 0.010549  0.331760 0.017063  P 0.0526331 0.0125696                                                                                                             
+23 924 60211.00 P  0.304832 0.010589  0.329287 0.017146  P 0.0532454 0.0126352                                                                                                             
+23 925 60212.00 P  0.304393 0.010629  0.326822 0.017228  P 0.0537145 0.0127006                                                                                                             
+23 926 60213.00 P  0.303911 0.010669  0.324366 0.017310  P 0.0539128 0.0127659                                                                                                             
+23 927 60214.00 P  0.303387 0.010709  0.321918 0.017392  P 0.0537648 0.0128311                                                                                                             
+23 928 60215.00 P  0.302822 0.010749  0.319480 0.017474  P 0.0532825 0.0128962                                                                                                             
+23 929 60216.00 P  0.302214 0.010789  0.317053 0.017555  P 0.0525721 0.0129612                                                                                                             
+23 930 60217.00 P  0.301565 0.010828  0.314636 0.017637  P 0.0518038 0.0130260                                                                                                             
+2310 1 60218.00 P  0.300875 0.010868  0.312231 0.017718  P 0.0511561 0.0130908                                                                                                             
+2310 2 60219.00 P  0.300144 0.010907  0.309839 0.017799  P 0.0507601 0.0131554                                                                                                             
+2310 3 60220.00 P  0.299372 0.010947  0.307459 0.017880  P 0.0506685 0.0132199                                                                                                             
+2310 4 60221.00 P  0.298560 0.010986  0.305092 0.017961  P 0.0508567 0.0132844                                                                                                             
+2310 5 60222.00 P  0.297708 0.011025  0.302740 0.018042  P 0.0512483 0.0133487                                                                                                             
+2310 6 60223.00 P  0.296815 0.011064  0.300402 0.018123  P 0.0517448 0.0134129                                                                                                             
+2310 7 60224.00 P  0.295884 0.011103  0.298080 0.018203  P 0.0522506 0.0134770                                                                                                             
+2310 8 60225.00 P  0.294912 0.011141  0.295773 0.018284  P 0.0526857 0.0135410                                                                                                             
+2310 9 60226.00 P  0.293902 0.011180  0.293483 0.018364  P 0.0529885 0.0136050                                                                                                             
+231010 60227.00 P  0.292854 0.011219  0.291210 0.018444  P 0.0531202 0.0136688                                                                                                             
+231011 60228.00 P  0.291767 0.011257  0.288955 0.018524  P 0.0530662 0.0137325                                                                                                             
+231012 60229.00 P  0.290642 0.011296  0.286718 0.018604  P 0.0528392 0.0137961                                                                                                             
+231013 60230.00 P  0.289480 0.011334  0.284500 0.018683  P 0.0524778 0.0138596                                                                                                             
+231014 60231.00 P  0.288281 0.011372  0.282301 0.018763  P 0.0520438 0.0139230                                                                                                             
+231015 60232.00 P  0.287044 0.011410  0.280122 0.018842  P 0.0516138 0.0139863                                                                                                             
+231016 60233.00 P  0.285772 0.011448  0.277963 0.018921  P 0.0512674 0.0140495                                                                                                             
+231017 60234.00 P  0.284463 0.011486  0.275826 0.019001  P 0.0510719 0.0141127                                                                                                             
+231018 60235.00 P  0.283119 0.011524  0.273710 0.019080  P 0.0510659 0.0141757                                                                                                             
+231019 60236.00 P  0.281740 0.011561  0.271616 0.019158  P 0.0512442 0.0142386                                                                                                             
+231020 60237.00 P  0.280326 0.011599  0.269545 0.019237  P 0.0515541 0.0143014                                                                                                             
+231021 60238.00 P  0.278878 0.011637  0.267497 0.019316  P 0.0518997 0.0143642                                                                                                             
+231022 60239.00 P  0.277396 0.011674  0.265472 0.019394  P 0.0521588 0.0144268                                                                                                             
+231023 60240.00 P  0.275881 0.011711  0.263472 0.019473  P 0.0522097 0.0144894                                                                                                             
+231024 60241.00 P  0.274332 0.011749  0.261497 0.019551  P 0.0519642 0.0145519                                                                                                             
+231025 60242.00 P  0.272752 0.011786  0.259546 0.019629  P 0.0513989 0.0146142                                                                                                             
+231026 60243.00 P  0.271139 0.011823  0.257621 0.019707  P 0.0505721 0.0146765                                                                                                             
+231027 60244.00 P  0.269495 0.011860  0.255723 0.019785  P 0.0496129 0.0147387                                                                                                             
+231028 60245.00 P  0.267820 0.011897  0.253851 0.019863  P 0.0486859 0.0148008                                                                                                             
+231029 60246.00 P  0.266115 0.011934  0.252006 0.019941  P 0.0479408 0.0148629                                                                                                             
+231030 60247.00 P  0.264379 0.011970  0.250188 0.020018  P 0.0474690 0.0149248                                                                                                             
+231031 60248.00 P  0.262615 0.012007  0.248399 0.020096  P 0.0472851 0.0149867                                                                                                             
+2311 1 60249.00 P  0.260821 0.012043  0.246637 0.020173  P 0.0473358 0.0150484                                                                                                             
+2311 2 60250.00 P  0.258999 0.012080  0.244905 0.020250  P 0.0475285 0.0151101                                                                                                             
+2311 3 60251.00 P  0.257149 0.012116  0.243202 0.020327  P 0.0477618 0.0151717                                                                                                             
+2311 4 60252.00 P  0.255272 0.012153  0.241528 0.020404  P 0.0479466 0.0152332                                                                                                             
+2311 5 60253.00 P  0.253368 0.012189  0.239885 0.020481  P 0.0480149 0.0152946                                                                                                             
+2311 6 60254.00 P  0.251439 0.012225  0.238272 0.020558  P 0.0479218 0.0153560                                                                                                             
+2311 7 60255.00 P  0.249483 0.012261  0.236690 0.020634  P 0.0476451 0.0154172                                                                                                             
+2311 8 60256.00 P  0.247503 0.012297  0.235139 0.020711  P 0.0471862 0.0154784                                                                                                             
+2311 9 60257.00 P  0.245498 0.012333  0.233619 0.020787  P 0.0465716 0.0155395                                                                                                             
+231110 60258.00 P  0.243470 0.012369  0.232132 0.020864  P 0.0458531 0.0156005                                                                                                             
+231111 60259.00 P  0.241418 0.012405  0.230677 0.020940  P 0.0451043 0.0156614                                                                                                             
+231112 60260.00 P  0.239343 0.012440  0.229254 0.021016  P 0.0444110 0.0157223                                                                                                             
+231113 60261.00 P  0.237247 0.012476  0.227864 0.021092  P 0.0438562 0.0157831                                                                                                             
+231114 60262.00 P  0.235129 0.012511  0.226508 0.021168  P 0.0435000 0.0158438                                                                                                             
+231115 60263.00 P  0.232990 0.012547  0.225185 0.021243  P 0.0433589 0.0159044                                                                                                             
+231116 60264.00 P  0.230832 0.012582  0.223896 0.021319  P 0.0433945 0.0159649                                                                                                             
+231117 60265.00 P  0.228653 0.012617  0.222641 0.021395  P 0.0435162 0.0160254                                                                                                             
+231118 60266.00 P  0.226456 0.012653  0.221421 0.021470  P 0.0436006 0.0160858                                                                                                             
+231119 60267.00 P  0.224241 0.012688  0.220235 0.021546  P 0.0435246 0.0161461                                                                                                             
+231120 60268.00 P  0.222008 0.012723  0.219085 0.021621  P 0.0432010 0.0162063                                                                                                             
+231121 60269.00 P  0.219757 0.012758  0.217969 0.021696  P 0.0426059 0.0162665                                                                                                             
+231122 60270.00 P  0.217491 0.012793  0.216889 0.021771  P 0.0417890 0.0163265                                                                                                             
+231123 60271.00 P  0.215209 0.012828  0.215845 0.021846  P 0.0408640 0.0163866                                                                                                             
+231124 60272.00 P  0.212911 0.012862  0.214837 0.021921  P 0.0399825 0.0164465                                                                                                             
+231125 60273.00 P  0.210600 0.012897  0.213865 0.021996  P 0.0392942 0.0165063                                                                                                             
+231126 60274.00 P  0.208274 0.012932  0.212929 0.022070  P 0.0389021 0.0165661                                                                                                             
+231127 60275.00 P  0.205936 0.012966  0.212030 0.022145  P 0.0388359 0.0166258                                                                                                             
+231128 60276.00 P  0.203585 0.013001  0.211167 0.022219  P 0.0390596 0.0166855                                                                                                             
+231129 60277.00 P  0.201223 0.013035  0.210341 0.022294  P 0.0395015 0.0167451                                                                                                             
+231130 60278.00 P  0.198849 0.013070  0.209553 0.022368  P 0.0400779 0.0168046                                                                                                             
+2312 1 60279.00 P  0.196465 0.013104  0.208801 0.022442  P 0.0406978 0.0168640                                                                                                             
+2312 2 60280.00 P  0.194071 0.013138  0.208087 0.022516  P 0.0412682 0.0169233                                                                                                             
+2312 3 60281.00 P  0.191668 0.013172  0.207410 0.022590  P 0.0417085 0.0169826                                                                                                             
+2312 4 60282.00 P  0.189257 0.013206  0.206771 0.022664  P 0.0419631 0.0170419                                                                                                             
+2312 5 60283.00 P  0.186838 0.013240  0.206170 0.022738  P 0.0420175 0.0171010                                                                                                             
+2312 6 60284.00 P  0.184412 0.013274  0.205606 0.022811  P 0.0419412 0.0171601                                                                                                             
+2312 7 60285.00 P  0.181980 0.013308  0.205081 0.022885  P 0.0418369 0.0172191                                                                                                             
+2312 8 60286.00 P  0.179542 0.013342  0.204593 0.022959  P 0.0416830 0.0172780                                                                                                             
+2312 9 60287.00 P  0.177099 0.013376  0.204143 0.023032  P 0.0415537 0.0173369                                                                                                             
+231210 60288.00 P  0.174652 0.013410  0.203731 0.023105  P 0.0415743 0.0173957                                                                                                             
+231211 60289.00 P  0.172201 0.013443  0.203358 0.023179  P 0.0417571 0.0174545                                                                                                             
+231212 60290.00 P  0.169747 0.013477  0.203022 0.023252  P 0.0422176 0.0175131                                                                                                             
+231213 60291.00 P  0.167291 0.013510  0.202725 0.023325  P 0.0429097 0.0175718                                                                                                             
+231214 60292.00 P  0.164834 0.013544  0.202466 0.023398  P 0.0436917 0.0176303                                                                                                             
+231215 60293.00 P  0.162375 0.013577  0.202245 0.023471  P 0.0444560 0.0176888                                                                                                             
+231216 60294.00 P  0.159917 0.013611  0.202063 0.023543  P 0.0450289 0.0177472                                                                                                             
+231217 60295.00 P  0.157459 0.013644  0.201918 0.023616  P 0.0453556 0.0178055                                                                                                             
+231218 60296.00 P  0.155002 0.013677  0.201812 0.023689  P 0.0454324 0.0178638                                                                                                             
+231219 60297.00 P  0.152546 0.013710  0.201743 0.023761  P 0.0451616 0.0179220                                                                                                             
+231220 60298.00 P  0.150094 0.013743  0.201713 0.023834  P 0.0446772 0.0179802                                                                                                             
+231221 60299.00 P  0.147644 0.013776  0.201721 0.023906  P 0.0442080 0.0180383                                                                                                             
+231222 60300.00 P  0.145199 0.013809  0.201766 0.023978  P 0.0437720 0.0180963                                                                                                             
+231223 60301.00 P  0.142758 0.013842  0.201850 0.024051  P 0.0435796 0.0181543                                                                                                             
+231224 60302.00 P  0.140322 0.013875  0.201971 0.024123  P 0.0435857 0.0182122                                                                                                             
+231225 60303.00 P  0.137892 0.013908  0.202130 0.024195  P 0.0438538 0.0182700                                                                                                             
+231226 60304.00 P  0.135468 0.013940  0.202326 0.024267  P 0.0442804 0.0183278                                                                                                             
+231227 60305.00 P  0.133052 0.013973  0.202560 0.024338  P 0.0448303 0.0183855                                                                                                             
+231228 60306.00 P  0.130643 0.014006  0.202831 0.024410  P 0.0454067 0.0184432                                                                                                             
+231229 60307.00 P  0.128243 0.014038  0.203139 0.024482  P 0.0459122 0.0185008                                                                                                             
+231230 60308.00 P  0.125853 0.014071  0.203484 0.024554  P 0.0462828 0.0185583                                                                                                             
+231231 60309.00 P  0.123472 0.014103  0.203866 0.024625  P 0.0465129 0.0186158                                                                                                             
+24 1 1 60310.00 P  0.121101 0.014136  0.204285 0.024697  P 0.0465067 0.0186732                                                                                                             
+24 1 2 60311.00 P  0.118741 0.014168  0.204740 0.024768  P 0.0463767 0.0187306                                                                                                             
+24 1 3 60312.00 P  0.116394 0.014200  0.205232 0.024839  P 0.0461709 0.0187879                                                                                                             
+24 1 4 60313.00 P  0.114058 0.014232  0.205759 0.024910  P 0.0459194 0.0188451                                                                                                             
+24 1 5 60314.00 P  0.111736 0.014265  0.206322 0.024982  P 0.0457071 0.0189023                                                                                                             
+24 1 6 60315.00 P  0.109427 0.014297  0.206921 0.025053  P 0.0456175 0.0189594                                                                                                             
+24 1 7 60316.00 P  0.107132 0.014329  0.207556 0.025124  P 0.0457165 0.0190165                                                                                                             
+24 1 8 60317.00 P  0.104852 0.014361  0.208225 0.025195  P 0.0460445 0.0190735                                                                                                             
+24 1 9 60318.00 P  0.102588 0.014393  0.208929 0.025265  P 0.0466387 0.0191305                                                                                                             
+24 110 60319.00 P  0.100340 0.014425  0.209669 0.025336  P 0.0473939 0.0191874                                                                                                             
+24 111 60320.00 P  0.098108 0.014456  0.210442 0.025407  P 0.0482096 0.0192442                                                                                                             
+24 112 60321.00 P  0.095893 0.014488  0.211250 0.025477  P 0.0489080 0.0193010                                                                                                             
+24 113 60322.00 P  0.093697 0.014520  0.212091 0.025548  P 0.0493736 0.0193577                                                                                                             
+24 114 60323.00 P  0.091518 0.014552  0.212966 0.025618  P 0.0494698 0.0194144                                                                                                             
+24 115 60324.00 P  0.089359 0.014583  0.213874 0.025689  P 0.0492097 0.0194710                                                                                                             
+24 116 60325.00 P  0.087219 0.014615  0.214815 0.025759  P 0.0488662 0.0195276                                                                                                             
+24 117 60326.00 P  0.085099 0.014646  0.215789 0.025829  P 0.0485051 0.0195841                                                                                                             
+24 118 60327.00 P  0.083000 0.014678  0.216795 0.025899  P 0.0483270 0.0196405                                                                                                             
+24 119 60328.00 P  0.080923 0.014709  0.217833 0.025969  P 0.0483326 0.0196969                                                                                                             
+24 120 60329.00 P  0.078866 0.014741  0.218902 0.026039  P 0.0486390 0.0197532                                                                                                             
+24 121 60330.00 P  0.076833 0.014772  0.220003 0.026109  P 0.0491327 0.0198095                                                                                                             
+24 122 60331.00 P  0.074822 0.014803  0.221135 0.026179  P 0.0498234 0.0198658                                                                                                             
+24 123 60332.00 P  0.072834 0.014835  0.222297 0.026249  P 0.0505894 0.0199219                                                                                                             
+24 124 60333.00 P  0.070870 0.014866  0.223489 0.026319  P 0.0513096 0.0199781                                                                                                             
+24 125 60334.00 P  0.068931 0.014897  0.224711 0.026388  P 0.0518992 0.0200341                                                                                                             
+24 126 60335.00 P  0.067016 0.014928  0.225962 0.026458  P 0.0523067 0.0200902                                                                                                             
+24 127 60336.00 P  0.065127 0.014959  0.227242 0.026527  P 0.0524787 0.0201461                                                                                                             
+24 128 60337.00 P  0.063264 0.014990  0.228551 0.026597  P 0.0524781 0.0202021                                                                                                             
+24 129 60338.00 P  0.061426 0.015021  0.229888 0.026666  P 0.0523301 0.0202579                                                                                                             
+24 130 60339.00 P  0.059616 0.015052  0.231253 0.026735  P 0.0520729 0.0203137                                                                                                             
+24 131 60340.00 P  0.057833 0.015083  0.232644 0.026805  P 0.0517763 0.0203695                                                                                                             
+24 2 1 60341.00 P  0.056078 0.015113  0.234063 0.026874  P 0.0514996 0.0204252                                                                                                             
+24 2 2 60342.00 P  0.054350 0.015144  0.235508 0.026943  P 0.0512642 0.0204809                                                                                                             
+24 2 3 60343.00 P  0.052652 0.015175  0.236979 0.027012  P 0.0511788 0.0205365                                                                                                             
+24 2 4 60344.00 P  0.050982 0.015205  0.238475 0.027081  P 0.0512445 0.0205920                                                                                                             
+24 2 5 60345.00 P  0.049341 0.015236  0.239997 0.027150  P 0.0514714 0.0206475                                                                                                             
+24 2 6 60346.00 P  0.047731 0.015267  0.241543 0.027218  P 0.0518228 0.0207030                                                                                                             
+24 2 7 60347.00 P  0.046151 0.015297  0.243113 0.027287  P 0.0522952 0.0207584                                                                                                             
+24 2 8 60348.00 P  0.044601 0.015328  0.244706 0.027356  P 0.0526760 0.0208138                                                                                                             
+24 2 9 60349.00 P  0.043082 0.015358  0.246323 0.027424  P 0.0528869 0.0208691                                                                                                             
+24 210 60350.00 P  0.041595 0.015388  0.247962 0.027493  P 0.0527814 0.0209243                                                                                                             
+24 211 60351.00 P  0.040139 0.015419  0.249624 0.027561  P 0.0522585 0.0209795                                                                                                             
+24 212 60352.00 P  0.038715 0.015449  0.251307 0.027630  P 0.0514242 0.0210347                                                                                                             
+24 213 60353.00 P  0.037324 0.015479  0.253011 0.027698  P 0.0505031 0.0210898                                                                                                             
+24 214 60354.00 P  0.035965 0.015509  0.254736 0.027766  P 0.0497110 0.0211449                                                                                                             
+24 215 60355.00 P  0.034640 0.015540  0.256480 0.027834  P 0.0491538 0.0211999                                                                                                             
+24 216 60356.00 P  0.033348 0.015570  0.258245 0.027903  P 0.0489245 0.0212548                                                                                                             
+24 217 60357.00 P  0.032090 0.015600  0.260028 0.027971  P 0.0489961 0.0213098                                                                                                             
+24 218 60358.00 P  0.030865 0.015630  0.261830 0.028039  P 0.0493041 0.0213646                                                                                                             
+24 219 60359.00 P  0.029675 0.015660  0.263649 0.028107  P 0.0498066 0.0214195                                                                                                             
+24 220 60360.00 P  0.028519 0.015690  0.265486 0.028175  P 0.0503365 0.0214742                                                                                                             
+24 221 60361.00 P  0.027399 0.015720  0.267340 0.028242  P 0.0508384 0.0215290                                                                                                             
+24 222 60362.00 P  0.026313 0.015749  0.269210 0.028310  P 0.0512073 0.0215837                                                                                                             
+24 223 60363.00 P  0.025262 0.015779  0.271096 0.028378  P 0.0514034 0.0216383                                                                                                             
+24 224 60364.00 P  0.024247 0.015809  0.272997 0.028445  P 0.0513907 0.0216929                                                                                                             
+24 225 60365.00 P  0.023268 0.015839  0.274913 0.028513  P 0.0512575 0.0217474                                                                                                             
+24 226 60366.00 P  0.022325 0.015868  0.276843 0.028580  P 0.0508828 0.0218019                                                                                                             
+24 227 60367.00 P  0.021418 0.015898  0.278786 0.028648  P 0.0504285 0.0218564                                                                                                             
+24 228 60368.00 P  0.020547 0.015928  0.280743 0.028715  P 0.0499940 0.0219108                                                                                                             
+24 229 60369.00 P  0.019713 0.015957  0.282711 0.028783  P 0.0496001 0.0219652                                                                                                             
+24 3 1 60370.00 P  0.018915 0.015987  0.284692 0.028850  P 0.0492945 0.0220195                                                                                                             
+24 3 2 60371.00 P  0.018155 0.016016  0.286683 0.028917  P 0.0491032 0.0220738                                                                                                             
+24 3 3 60372.00 P  0.017431 0.016046  0.288685 0.028984  P 0.0491006 0.0221280                                                                                                             
+24 3 4 60373.00 P  0.016745 0.016075  0.290698 0.029051  P 0.0492206 0.0221822                                                                                                             
+24 3 5 60374.00 P  0.016095 0.016104  0.292720 0.029118  P 0.0494549 0.0222363                                                                                                             
+24 3 6 60375.00 P  0.015483 0.016134  0.294750 0.029185  P 0.0497490 0.0222904                                                                                                             
+24 3 7 60376.00 P  0.014909 0.016163  0.296789 0.029252  P 0.0499638 0.0223444                                                                                                             
+24 3 8 60377.00 P  0.014372 0.016192  0.298836 0.029319  P 0.0498662 0.0223985                                                                                                             
+24 3 9 60378.00 P  0.013873 0.016221  0.300890 0.029386  P 0.0494344 0.0224524                                                                                                             
+24 310 60379.00 P  0.013412 0.016250  0.302950 0.029452  P 0.0486708 0.0225063                                                                                                             
+24 311 60380.00 P  0.012989 0.016280  0.305016 0.029519  P 0.0476832 0.0225602                                                                                                             
+24 312 60381.00 P  0.012603 0.016309  0.307088 0.029586  P 0.0466673 0.0226140                                                                                                             
+24 313 60382.00 P  0.012255 0.016338  0.309164 0.029652  P 0.0458657 0.0226678                                                                                                             
+24 314 60383.00 P  0.011945 0.016367  0.311245 0.029719  P 0.0453529 0.0227216                                                                                                             
+24 315 60384.00 P  0.011674 0.016396  0.313329 0.029785  P 0.0451817 0.0227753                                                                                                             
+24 316 60385.00 P  0.011440 0.016425  0.315416 0.029851  P 0.0453401 0.0228290                                                                                                             
+24 317 60386.00 P  0.011244 0.016453  0.317505 0.029918  P 0.0456535 0.0228826                                                                                                             
+24 318 60387.00 P  0.011086 0.016482  0.319597 0.029984  P 0.0460693 0.0229362                                                                                                             
+24 319 60388.00 P  0.010966 0.016511  0.321689 0.030050  P 0.0464914 0.0229897                                                                                                             
+24 320 60389.00 P  0.010884 0.016540  0.323782 0.030116  P 0.0468438 0.0230432                                                                                                             
+24 321 60390.00 P  0.010840 0.016569  0.325876 0.030182  P 0.0470460 0.0230966                                                                                                             
+24 322 60391.00 P  0.010833 0.016597  0.327968 0.030248  P 0.0470908 0.0231500                                                                                                             
+24 323 60392.00 P  0.010864 0.016626  0.330060 0.030314  P 0.0469821 0.0232034                                                                                                             
+24 324 60393.00 P  0.010933 0.016654  0.332150 0.030380  P 0.0466940 0.0232567                                                                                                             
+24 325 60394.00 P  0.011040 0.016683  0.334237 0.030446  P 0.0462492 0.0233100                                                                                                             
+24 326 60395.00 P  0.011184 0.016712  0.336322 0.030512  P 0.0457381 0.0233633                                                                                                             
+24 327 60396.00 P  0.011365 0.016740  0.338403 0.030578  P 0.0452591 0.0234165                                                                                                             
+24 328 60397.00 P  0.011584 0.016769  0.340480 0.030643  P 0.0449109 0.0234697                                                                                                             
+24 329 60398.00 P  0.011839 0.016797  0.342552 0.030709  P 0.0447445 0.0235228                                                                                                             
+24 330 60399.00 P  0.012132 0.016825  0.344619 0.030775  P 0.0447647 0.0235759                                                                                                             
+24 331 60400.00 P  0.012461 0.016854  0.346681 0.030840  P 0.0449747 0.0236289                                                                                                             
+24 4 1 60401.00 P  0.012828 0.016882  0.348736 0.030906  P 0.0452442 0.0236819                                                                                                             
+24 4 2 60402.00 P  0.013230 0.016910  0.350784 0.030971  P 0.0455560 0.0237349                                                                                                             
+24 4 3 60403.00 P  0.013669 0.016939  0.352825 0.031036  P 0.0457845 0.0237878                                                                                                             
+24 4 4 60404.00 P  0.014144 0.016967  0.354857 0.031102  P 0.0457536 0.0238407                                                                                                             
+24 4 5 60405.00 P  0.014655 0.016995  0.356881 0.031167  P 0.0454107 0.0238935                                                                                                             
+24 4 6 60406.00 P  0.015202 0.017023  0.358896 0.031232  P 0.0447695 0.0239463                                                                                                             
+24 4 7 60407.00 P  0.015784 0.017051  0.360902 0.031297  P 0.0438145 0.0239991                                                                                                             
+24 4 8 60408.00 P  0.016401 0.017079  0.362897 0.031362  P 0.0427448 0.0240518                                                                                                             
+24 4 9 60409.00 P  0.017054 0.017107  0.364881 0.031428  P 0.0417120 0.0241045                                                                                                             
+24 410 60410.00 P  0.017741 0.017135  0.366854 0.031493  P 0.0408498 0.0241572                                                                                                             
+24 411 60411.00 P  0.018463 0.017163  0.368815 0.031557  P 0.0402576 0.0242098                                                                                                             
+24 412 60412.00 P  0.019219 0.017191  0.370763 0.031622  P 0.0399386 0.0242624                                                                                                             
+24 413 60413.00 P  0.020009 0.017219  0.372699 0.031687  P 0.0398489 0.0243149                                                                                                             
+24 414 60414.00 P  0.020832 0.017247  0.374621 0.031752  P 0.0399089 0.0243674                                                                                                             
+24 415 60415.00 P  0.021690 0.017275  0.376529 0.031817  P 0.0399873 0.0244199                                                                                                             
+24 416 60416.00 P  0.022580 0.017303  0.378423 0.031881  P 0.0400005 0.0244723                                                                                                             
+24 417 60417.00 P  0.023503 0.017330  0.380302 0.031946  P 0.0398683 0.0245247                                                                                                             
+24 418 60418.00 P  0.024458 0.017358  0.382165 0.032011  P 0.0395609 0.0245770                                                                                                             
+24 419 60419.00 P  0.025445 0.017386  0.384013 0.032075  P 0.0390531 0.0246293                                                                                                             
+24 420 60420.00 P  0.026465 0.017413  0.385844 0.032140  P 0.0383783 0.0246816                                                                                                             
+24 421 60421.00 P  0.027515 0.017441  0.387658 0.032204  P 0.0375410 0.0247338                                                                                                             
+24 422 60422.00 P  0.028597 0.017469  0.389454 0.032268  P 0.0366522 0.0247860                                                                                                             
+24 423 60423.00 P  0.029710 0.017496  0.391233 0.032333  P 0.0358383 0.0248382                                                                                                             
+24 424 60424.00 P  0.030852 0.017524  0.392993 0.032397  P 0.0352065 0.0248903                                                                                                             
+24 425 60425.00 P  0.032025 0.017551  0.394734 0.032461  P 0.0348191 0.0249424                                                                                                             
+24 426 60426.00 P  0.033228 0.017579  0.396456 0.032525  P 0.0346363 0.0249945                                                                                                             
+24 427 60427.00 P  0.034459 0.017606  0.398159 0.032590  P 0.0346869 0.0250465                                                                                                             
+24 428 60428.00 P  0.035719 0.017634  0.399841 0.032654  P 0.0348689 0.0250985                                                                                                             
+24 429 60429.00 P  0.037008 0.017661  0.401502 0.032718  P 0.0351870 0.0251504                                                                                                             
+24 430 60430.00 P  0.038325 0.017688  0.403143 0.032782  P 0.0355292 0.0252023                                                                                                             
+24 5 1 60431.00 P  0.039669 0.017716  0.404762 0.032846  P 0.0357579 0.0252542                                                                                                             
+24 5 2 60432.00 P  0.041040 0.017743  0.406359 0.032910  P 0.0357293 0.0253060                                                                                                             
+24 5 3 60433.00 P  0.042437 0.017770  0.407934 0.032973  P 0.0353708 0.0253578                                                                                                             
+24 5 4 60434.00 P  0.043861 0.017797  0.409486 0.033037  P 0.0347628 0.0254096                                                                                                             
 24 5 5 60435.00                                                                                                                                                                            
 24 5 6 60436.00                                                                                                                                                                            
 24 5 7 60437.00                                                                                                                                                                            
 24 5 8 60438.00                                                                                                                                                                            
 24 5 9 60439.00                                                                                                                                                                            
 24 510 60440.00                                                                                                                                                                            
 24 511 60441.00                                                                                                                                                                            
@@ -18767,7 +18767,35 @@
 24 520 60450.00                                                                                                                                                                            
 24 521 60451.00                                                                                                                                                                            
 24 522 60452.00                                                                                                                                                                            
 24 523 60453.00                                                                                                                                                                            
 24 524 60454.00                                                                                                                                                                            
 24 525 60455.00                                                                                                                                                                            
 24 526 60456.00                                                                                                                                                                            
+24 527 60457.00                                                                                                                                                                            
+24 528 60458.00                                                                                                                                                                            
+24 529 60459.00                                                                                                                                                                            
+24 530 60460.00                                                                                                                                                                            
+24 531 60461.00                                                                                                                                                                            
+24 6 1 60462.00                                                                                                                                                                            
+24 6 2 60463.00                                                                                                                                                                            
+24 6 3 60464.00                                                                                                                                                                            
+24 6 4 60465.00                                                                                                                                                                            
+24 6 5 60466.00                                                                                                                                                                            
+24 6 6 60467.00                                                                                                                                                                            
+24 6 7 60468.00                                                                                                                                                                            
+24 6 8 60469.00                                                                                                                                                                            
+24 6 9 60470.00                                                                                                                                                                            
+24 610 60471.00                                                                                                                                                                            
+24 611 60472.00                                                                                                                                                                            
+24 612 60473.00                                                                                                                                                                            
+24 613 60474.00                                                                                                                                                                            
+24 614 60475.00                                                                                                                                                                            
+24 615 60476.00                                                                                                                                                                            
+24 616 60477.00                                                                                                                                                                            
+24 617 60478.00                                                                                                                                                                            
+24 618 60479.00                                                                                                                                                                            
+24 619 60480.00                                                                                                                                                                            
+24 620 60481.00                                                                                                                                                                            
+24 621 60482.00                                                                                                                                                                            
+24 622 60483.00                                                                                                                                                                            
+24 623 60484.00
```

### Comparing `pyTMD-2.0.3/pyTMD/data/historic_deltat.data` & `pyTMD-2.0.4/pyTMD/data/historic_deltat.data`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.3/pyTMD/data/iers_deltat.data` & `pyTMD-2.0.4/pyTMD/data/iers_deltat.data`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.3/pyTMD/data/leap-seconds.list` & `pyTMD-2.0.4/pyTMD/data/leap-seconds.list`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.3/pyTMD/data/mean-pole.tab` & `pyTMD-2.0.4/pyTMD/data/mean-pole.tab`

 * *Files 1% similar despite different names*

```diff
@@ -2122,15 +2122,15 @@
 2006.05   0.0610127   0.3452846
 2006.10   0.0612252   0.3453088
 2006.15   0.0614390   0.3453320
 2006.20   0.0616541   0.3453541
 2006.25   0.0618705   0.3453751
 2006.30   0.0620881   0.3453950
 2006.35   0.0623070   0.3454139
-2006.40   0.0625271   0.3454317
+2006.40   0.0625270   0.3454317
 2006.45   0.0627484   0.3454485
 2006.50   0.0629709   0.3454644
 2006.55   0.0631946   0.3454792
 2006.60   0.0634194   0.3454930
 2006.65   0.0636455   0.3455059
 2006.70   0.0638727   0.3455179
 2006.75   0.0641010   0.3455290
@@ -2140,325 +2140,326 @@
 2006.95   0.0650252   0.3455644
 2007.00   0.0652589   0.3455712
 2007.05   0.0654936   0.3455772
 2007.10   0.0657294   0.3455825
 2007.15   0.0659661   0.3455870
 2007.20   0.0662038   0.3455908
 2007.25   0.0664424   0.3455939
-2007.30   0.0666820   0.3455964
+2007.30   0.0666819   0.3455964
 2007.35   0.0669224   0.3455982
 2007.40   0.0671637   0.3455995
 2007.45   0.0674059   0.3456001
 2007.50   0.0676489   0.3456002
 2007.55   0.0678928   0.3455998
 2007.60   0.0681374   0.3455989
-2007.65   0.0683828   0.3455976
+2007.65   0.0683827   0.3455976
 2007.70   0.0686289   0.3455958
 2007.75   0.0688757   0.3455937
 2007.80   0.0691232   0.3455911
 2007.85   0.0693714   0.3455883
-2007.90   0.0696203   0.3455851
+2007.90   0.0696202   0.3455851
 2007.95   0.0698697   0.3455817
 2008.00   0.0701197   0.3455780
-2008.05   0.0703704   0.3455742
+2008.05   0.0703703   0.3455742
 2008.10   0.0706215   0.3455701
-2008.15   0.0708732   0.3455659
+2008.15   0.0708731   0.3455659
 2008.20   0.0711253   0.3455616
 2008.25   0.0713779   0.3455573
-2008.30   0.0716310   0.3455529
+2008.30   0.0716309   0.3455529
 2008.35   0.0718844   0.3455485
-2008.40   0.0721383   0.3455441
-2008.45   0.0723925   0.3455398
+2008.40   0.0721382   0.3455441
+2008.45   0.0723924   0.3455398
 2008.50   0.0726470   0.3455356
-2008.55   0.0729019   0.3455315
+2008.55   0.0729018   0.3455315
 2008.60   0.0731570   0.3455276
 2008.65   0.0734124   0.3455239
-2008.70   0.0736681   0.3455204
-2008.75   0.0739239   0.3455172
+2008.70   0.0736680   0.3455204
+2008.75   0.0739238   0.3455172
 2008.80   0.0741799   0.3455143
-2008.85   0.0744361   0.3455116
+2008.85   0.0744360   0.3455117
 2008.90   0.0746924   0.3455094
-2008.95   0.0749489   0.3455076
-2009.00   0.0752054   0.3455061
-2009.05   0.0754620   0.3455052
-2009.10   0.0757186   0.3455047
-2009.15   0.0759752   0.3455047
-2009.20   0.0762318   0.3455053
-2009.25   0.0764884   0.3455065
-2009.30   0.0767450   0.3455083
-2009.35   0.0770015   0.3455107
-2009.40   0.0772578   0.3455138
-2009.45   0.0775141   0.3455176
-2009.50   0.0777702   0.3455221
-2009.55   0.0780262   0.3455274
-2009.60   0.0782820   0.3455334
-2009.65   0.0785376   0.3455403
-2009.70   0.0787930   0.3455480
-2009.75   0.0790481   0.3455565
-2009.80   0.0793030   0.3455659
-2009.85   0.0795576   0.3455762
-2009.90   0.0798120   0.3455875
-2009.95   0.0800660   0.3455997
-2010.00   0.0803197   0.3456129
-2010.05   0.0805731   0.3456270
-2010.10   0.0808261   0.3456422
-2010.15   0.0810788   0.3456584
-2010.20   0.0813311   0.3456756
-2010.25   0.0815830   0.3456939
-2010.30   0.0818345   0.3457133
-2010.35   0.0820855   0.3457337
-2010.40   0.0823362   0.3457553
-2010.45   0.0825864   0.3457780
-2010.50   0.0828361   0.3458018
-2010.55   0.0830854   0.3458268
-2010.60   0.0833343   0.3458530
-2010.65   0.0835826   0.3458803
-2010.70   0.0838305   0.3459088
-2010.75   0.0840779   0.3459384
-2010.80   0.0843247   0.3459693
-2010.85   0.0845711   0.3460013
-2010.90   0.0848169   0.3460346
-2010.95   0.0850622   0.3460691
-2011.00   0.0853070   0.3461047
-2011.05   0.0855513   0.3461416
-2011.10   0.0857950   0.3461797
-2011.15   0.0860382   0.3462190
-2011.20   0.0862809   0.3462595
-2011.25   0.0865230   0.3463012
-2011.30   0.0867645   0.3463442
-2011.35   0.0870055   0.3463883
-2011.40   0.0872460   0.3464336
-2011.45   0.0874859   0.3464801
-2011.50   0.0877253   0.3465278
-2011.55   0.0879641   0.3465766
-2011.60   0.0882024   0.3466267
-2011.65   0.0884401   0.3466778
-2011.70   0.0886773   0.3467302
-2011.75   0.0889139   0.3467836
-2011.80   0.0891500   0.3468382
-2011.85   0.0893855   0.3468938
-2011.90   0.0896206   0.3469506
-2011.95   0.0898550   0.3470084
-2012.00   0.0900890   0.3470673
-2012.05   0.0903224   0.3471272
-2012.10   0.0905554   0.3471882
-2012.15   0.0907878   0.3472501
-2012.20   0.0910196   0.3473130
-2012.25   0.0912510   0.3473769
-2012.30   0.0914819   0.3474417
-2012.35   0.0917123   0.3475075
-2012.40   0.0919422   0.3475741
-2012.45   0.0921717   0.3476416
-2012.50   0.0924006   0.3477099
-2012.55   0.0926291   0.3477790
-2012.60   0.0928572   0.3478490
-2012.65   0.0930847   0.3479196
-2012.70   0.0933119   0.3479911
-2012.75   0.0935386   0.3480632
-2012.80   0.0937648   0.3481360
-2012.85   0.0939907   0.3482095
-2012.90   0.0942161   0.3482835
-2012.95   0.0944411   0.3483582
-2013.00   0.0946657   0.3484334
-2013.05   0.0948900   0.3485091
-2013.10   0.0951138   0.3485854
-2013.15   0.0953372   0.3486621
-2013.20   0.0955603   0.3487392
-2013.25   0.0957830   0.3488167
-2013.30   0.0960054   0.3488946
-2013.35   0.0962274   0.3489728
-2013.40   0.0964491   0.3490513
-2013.45   0.0966704   0.3491301
-2013.50   0.0968915   0.3492090
-2013.55   0.0971121   0.3492882
-2013.60   0.0973325   0.3493675
-2013.65   0.0975526   0.3494470
-2013.70   0.0977724   0.3495265
-2013.75   0.0979919   0.3496061
-2013.80   0.0982111   0.3496857
-2013.85   0.0984300   0.3497653
-2013.90   0.0986486   0.3498448
-2013.95   0.0988670   0.3499243
-2014.00   0.0990851   0.3500036
-2014.05   0.0993029   0.3500827
-2014.10   0.0995205   0.3501617
-2014.15   0.0997379   0.3502404
-2014.20   0.0999550   0.3503189
-2014.25   0.1001718   0.3503970
-2014.30   0.1003885   0.3504748
-2014.35   0.1006049   0.3505523
-2014.40   0.1008210   0.3506294
-2014.45   0.1010370   0.3507060
-2014.50   0.1012527   0.3507821
-2014.55   0.1014682   0.3508578
-2014.60   0.1016835   0.3509329
-2014.65   0.1018985   0.3510075
-2014.70   0.1021134   0.3510814
-2014.75   0.1023280   0.3511548
-2014.80   0.1025424   0.3512274
-2014.85   0.1027566   0.3512994
-2014.90   0.1029706   0.3513707
-2014.95   0.1031844   0.3514412
-2015.00   0.1033980   0.3515109
-2015.05   0.1036114   0.3515798
-2015.10   0.1038245   0.3516479
-2015.15   0.1040375   0.3517152
-2015.20   0.1042502   0.3517815
-2015.25   0.1044627   0.3518469
-2015.30   0.1046750   0.3519114
-2015.35   0.1048870   0.3519749
-2015.40   0.1050989   0.3520374
-2015.45   0.1053105   0.3520989
-2015.50   0.1055219   0.3521594
-2015.55   0.1057330   0.3522188
-2015.60   0.1059439   0.3522772
-2015.65   0.1061546   0.3523344
-2015.70   0.1063650   0.3523905
-2015.75   0.1065752   0.3524454
-2015.80   0.1067851   0.3524992
-2015.85   0.1069947   0.3525518
-2015.90   0.1072041   0.3526033
-2015.95   0.1074132   0.3526534
-2016.00   0.1076220   0.3527024
-2016.05   0.1078305   0.3527501
-2016.10   0.1080387   0.3527966
-2016.15   0.1082466   0.3528417
-2016.20   0.1084542   0.3528856
-2016.25   0.1086615   0.3529282
-2016.30   0.1088685   0.3529694
-2016.35   0.1090751   0.3530093
-2016.40   0.1092814   0.3530479
-2016.45   0.1094874   0.3530851
-2016.50   0.1096930   0.3531210
-2016.55   0.1098982   0.3531555
-2016.60   0.1101031   0.3531886
-2016.65   0.1103075   0.3532203
-2016.70   0.1105116   0.3532506
-2016.75   0.1107153   0.3532795
-2016.80   0.1109185   0.3533070
-2016.85   0.1111214   0.3533331
-2016.90   0.1113238   0.3533578
-2016.95   0.1115258   0.3533811
-2017.00   0.1117273   0.3534029
-2017.05   0.1119283   0.3534233
-2017.10   0.1121289   0.3534423
-2017.15   0.1123291   0.3534599
-2017.20   0.1125287   0.3534760
-2017.25   0.1127278   0.3534907
-2017.30   0.1129264   0.3535039
-2017.35   0.1131245   0.3535157
-2017.40   0.1133221   0.3535261
-2017.45   0.1135191   0.3535350
-2017.50   0.1137156   0.3535425
-2017.55   0.1139115   0.3535486
-2017.60   0.1141068   0.3535533
-2017.65   0.1143016   0.3535565
-2017.70   0.1144958   0.3535583
-2017.75   0.1146894   0.3535587
-2017.80   0.1148823   0.3535577
-2017.85   0.1150747   0.3535553
-2017.90   0.1152664   0.3535515
-2017.95   0.1154575   0.3535463
-2018.00   0.1156479   0.3535397
-2018.05   0.1158376   0.3535317
-2018.10   0.1160267   0.3535223
-2018.15   0.1162152   0.3535116
-2018.20   0.1164029   0.3534995
-2018.25   0.1165899   0.3534861
-2018.30   0.1167763   0.3534713
-2018.35   0.1169619   0.3534551
-2018.40   0.1171468   0.3534376
-2018.45   0.1173309   0.3534188
-2018.50   0.1175143   0.3533987
-2018.55   0.1176970   0.3533773
-2018.60   0.1178789   0.3533546
-2018.65   0.1180600   0.3533306
-2018.70   0.1182404   0.3533053
-2018.75   0.1184200   0.3532787
-2018.80   0.1185988   0.3532509
-2018.85   0.1187768   0.3532218
-2018.90   0.1189540   0.3531915
-2018.95   0.1191303   0.3531600
-2019.00   0.1193059   0.3531272
-2019.05   0.1194806   0.3530932
-2019.10   0.1196545   0.3530580
-2019.15   0.1198276   0.3530217
-2019.20   0.1199998   0.3529841
-2019.25   0.1201711   0.3529454
-2019.30   0.1203416   0.3529055
-2019.35   0.1205113   0.3528645
-2019.40   0.1206801   0.3528223
-2019.45   0.1208479   0.3527790
-2019.50   0.1210150   0.3527346
-2019.55   0.1211811   0.3526890
-2019.60   0.1213463   0.3526424
-2019.65   0.1215107   0.3525947
-2019.70   0.1216741   0.3525459
-2019.75   0.1218366   0.3524961
-2019.80   0.1219983   0.3524452
-2019.85   0.1221590   0.3523932
-2019.90   0.1223188   0.3523403
-2019.95   0.1224777   0.3522863
-2020.00   0.1226356   0.3522313
-2020.05   0.1227927   0.3521753
-2020.10   0.1229488   0.3521183
-2020.15   0.1231039   0.3520603
-2020.20   0.1232582   0.3520013
-2020.25   0.1234115   0.3519414
-2020.30   0.1235638   0.3518805
-2020.35   0.1237153   0.3518187
-2020.40   0.1238657   0.3517560
-2020.45   0.1240153   0.3516923
-2020.50   0.1241638   0.3516278
-2020.55   0.1243115   0.3515623
-2020.60   0.1244581   0.3514960
-2020.65   0.1246039   0.3514287
-2020.70   0.1247486   0.3513606
-2020.75   0.1248925   0.3512916
-2020.80   0.1250353   0.3512218
-2020.85   0.1251772   0.3511512
-2020.90   0.1253182   0.3510797
-2020.95   0.1254582   0.3510073
-2021.00   0.1255972   0.3509342
-2021.05   0.1257353   0.3508602
-2021.10   0.1258724   0.3507855
-2021.15   0.1260086   0.3507099
-2021.20   0.1261438   0.3506336
-2021.25   0.1262781   0.3505565
-2021.30   0.1264114   0.3504787
-2021.35   0.1265437   0.3504000
-2021.40   0.1266751   0.3503207
-2021.45   0.1268055   0.3502406
-2021.50   0.1269350   0.3501597
-2021.55   0.1270636   0.3500782
-2021.60   0.1271912   0.3499959
-2021.65   0.1273178   0.3499129
-2021.70   0.1274435   0.3498293
-2021.75   0.1275683   0.3497449
-2021.80   0.1276921   0.3496598
-2021.85   0.1278150   0.3495741
-2021.90   0.1279369   0.3494877
-2021.95   0.1280579   0.3494006
-2022.00   0.1281779   0.3493129
-2022.05   0.1282971   0.3492245
-2022.10   0.1284152   0.3491355
-2022.15   0.1285325   0.3490459
-2022.20   0.1286489   0.3489556
-2022.25   0.1287643   0.3488647
-2022.30   0.1288788   0.3487732
-2022.35   0.1289923   0.3486811
-2022.40   0.1291050   0.3485884
-2022.45   0.1292167   0.3484951
-2022.50   0.1293276   0.3484012
-2022.55   0.1294375   0.3483067
-2022.60   0.1295465   0.3482117
-2022.65   0.1296546   0.3481160
-2022.70   0.1297618   0.3480199
-2022.75   0.1298682   0.3479231
-2022.80   0.1299736   0.3478258
-2022.85   0.1300781   0.3477280
-2022.90   0.1301818   0.3476297
-2022.95   0.1302845   0.3475308
-2023.00   0.1303864   0.3474313
-2023.05   0.1304874   0.3473314
-2023.10   0.1305875   0.3472309
-2023.15   0.1306868   0.3471300
+2008.95   0.0749488   0.3455076
+2009.00   0.0752053   0.3455061
+2009.05   0.0754619   0.3455052
+2009.10   0.0757185   0.3455047
+2009.15   0.0759751   0.3455047
+2009.20   0.0762317   0.3455053
+2009.25   0.0764883   0.3455065
+2009.30   0.0767449   0.3455083
+2009.35   0.0770013   0.3455107
+2009.40   0.0772577   0.3455138
+2009.45   0.0775139   0.3455176
+2009.50   0.0777701   0.3455221
+2009.55   0.0780260   0.3455274
+2009.60   0.0782818   0.3455334
+2009.65   0.0785374   0.3455403
+2009.70   0.0787927   0.3455480
+2009.75   0.0790479   0.3455565
+2009.80   0.0793027   0.3455659
+2009.85   0.0795574   0.3455763
+2009.90   0.0798117   0.3455875
+2009.95   0.0800657   0.3455997
+2010.00   0.0803194   0.3456129
+2010.05   0.0805727   0.3456270
+2010.10   0.0808258   0.3456422
+2010.15   0.0810784   0.3456584
+2010.20   0.0813307   0.3456756
+2010.25   0.0815825   0.3456939
+2010.30   0.0818340   0.3457133
+2010.35   0.0820851   0.3457337
+2010.40   0.0823357   0.3457553
+2010.45   0.0825859   0.3457780
+2010.50   0.0828356   0.3458019
+2010.55   0.0830848   0.3458268
+2010.60   0.0833336   0.3458530
+2010.65   0.0835819   0.3458803
+2010.70   0.0838298   0.3459088
+2010.75   0.0840771   0.3459385
+2010.80   0.0843239   0.3459693
+2010.85   0.0845702   0.3460014
+2010.90   0.0848160   0.3460346
+2010.95   0.0850613   0.3460691
+2011.00   0.0853060   0.3461048
+2011.05   0.0855502   0.3461416
+2011.10   0.0857939   0.3461797
+2011.15   0.0860370   0.3462190
+2011.20   0.0862796   0.3462595
+2011.25   0.0865217   0.3463013
+2011.30   0.0867631   0.3463442
+2011.35   0.0870041   0.3463883
+2011.40   0.0872445   0.3464336
+2011.45   0.0874843   0.3464801
+2011.50   0.0877236   0.3465278
+2011.55   0.0879623   0.3465767
+2011.60   0.0882005   0.3466267
+2011.65   0.0884381   0.3466779
+2011.70   0.0886751   0.3467302
+2011.75   0.0889117   0.3467837
+2011.80   0.0891476   0.3468382
+2011.85   0.0893831   0.3468939
+2011.90   0.0896180   0.3469506
+2011.95   0.0898523   0.3470085
+2012.00   0.0900861   0.3470674
+2012.05   0.0903194   0.3471273
+2012.10   0.0905522   0.3471882
+2012.15   0.0907844   0.3472502
+2012.20   0.0910161   0.3473131
+2012.25   0.0912473   0.3473770
+2012.30   0.0914780   0.3474418
+2012.35   0.0917082   0.3475075
+2012.40   0.0919380   0.3475741
+2012.45   0.0921672   0.3476416
+2012.50   0.0923959   0.3477099
+2012.55   0.0926242   0.3477791
+2012.60   0.0928520   0.3478490
+2012.65   0.0930793   0.3479197
+2012.70   0.0933062   0.3479911
+2012.75   0.0935326   0.3480632
+2012.80   0.0937586   0.3481360
+2012.85   0.0939841   0.3482095
+2012.90   0.0942092   0.3482836
+2012.95   0.0944339   0.3483582
+2013.00   0.0946582   0.3484334
+2013.05   0.0948820   0.3485092
+2013.10   0.0951055   0.3485854
+2013.15   0.0953285   0.3486621
+2013.20   0.0955512   0.3487392
+2013.25   0.0957735   0.3488167
+2013.30   0.0959955   0.3488946
+2013.35   0.0962170   0.3489728
+2013.40   0.0964382   0.3490513
+2013.45   0.0966591   0.3491300
+2013.50   0.0968796   0.3492090
+2013.55   0.0970997   0.3492882
+2013.60   0.0973196   0.3493675
+2013.65   0.0975391   0.3494469
+2013.70   0.0977582   0.3495264
+2013.75   0.0979771   0.3496060
+2013.80   0.0981956   0.3496856
+2013.85   0.0984139   0.3497652
+2013.90   0.0986318   0.3498447
+2013.95   0.0988495   0.3499241
+2014.00   0.0990669   0.3500034
+2014.05   0.0992839   0.3500825
+2014.10   0.0995007   0.3501614
+2014.15   0.0997172   0.3502402
+2014.20   0.0999335   0.3503186
+2014.25   0.1001494   0.3503967
+2014.30   0.1003651   0.3504745
+2014.35   0.1005806   0.3505520
+2014.40   0.1007957   0.3506290
+2014.45   0.1010106   0.3507056
+2014.50   0.1012253   0.3507817
+2014.55   0.1014397   0.3508573
+2014.60   0.1016538   0.3509324
+2014.65   0.1018677   0.3510069
+2014.70   0.1020813   0.3510808
+2014.75   0.1022947   0.3511541
+2014.80   0.1025078   0.3512267
+2014.85   0.1027207   0.3512987
+2014.90   0.1029333   0.3513699
+2014.95   0.1031456   0.3514404
+2015.00   0.1033577   0.3515100
+2015.05   0.1035696   0.3515789
+2015.10   0.1037811   0.3516469
+2015.15   0.1039924   0.3517141
+2015.20   0.1042035   0.3517804
+2015.25   0.1044143   0.3518457
+2015.30   0.1046247   0.3519102
+2015.35   0.1048350   0.3519736
+2015.40   0.1050449   0.3520360
+2015.45   0.1052545   0.3520975
+2015.50   0.1054639   0.3521579
+2015.55   0.1056730   0.3522172
+2015.60   0.1058817   0.3522755
+2015.65   0.1060902   0.3523326
+2015.70   0.1062983   0.3523886
+2015.75   0.1065061   0.3524435
+2015.80   0.1067136   0.3524972
+2015.85   0.1069208   0.3525497
+2015.90   0.1071276   0.3526010
+2015.95   0.1073341   0.3526511
+2016.00   0.1075402   0.3526999
+2016.05   0.1077459   0.3527475
+2016.10   0.1079513   0.3527939
+2016.15   0.1081563   0.3528389
+2016.20   0.1083609   0.3528827
+2016.25   0.1085652   0.3529251
+2016.30   0.1087690   0.3529662
+2016.35   0.1089724   0.3530060
+2016.40   0.1091753   0.3530444
+2016.45   0.1093779   0.3530815
+2016.50   0.1095799   0.3531172
+2016.55   0.1097816   0.3531516
+2016.60   0.1099827   0.3531845
+2016.65   0.1101834   0.3532161
+2016.70   0.1103836   0.3532463
+2016.75   0.1105833   0.3532750
+2016.80   0.1107825   0.3533024
+2016.85   0.1109812   0.3533283
+2016.90   0.1111794   0.3533529
+2016.95   0.1113770   0.3533760
+2017.00   0.1115740   0.3533976
+2017.05   0.1117705   0.3534179
+2017.10   0.1119664   0.3534367
+2017.15   0.1121618   0.3534540
+2017.20   0.1123565   0.3534700
+2017.25   0.1125506   0.3534844
+2017.30   0.1127442   0.3534975
+2017.35   0.1129370   0.3535091
+2017.40   0.1131293   0.3535193
+2017.45   0.1133208   0.3535281
+2017.50   0.1135117   0.3535354
+2017.55   0.1137020   0.3535413
+2017.60   0.1138915   0.3535457
+2017.65   0.1140804   0.3535488
+2017.70   0.1142685   0.3535504
+2017.75   0.1144559   0.3535506
+2017.80   0.1146426   0.3535493
+2017.85   0.1148285   0.3535467
+2017.90   0.1150137   0.3535427
+2017.95   0.1151981   0.3535373
+2018.00   0.1153817   0.3535305
+2018.05   0.1155645   0.3535223
+2018.10   0.1157465   0.3535127
+2018.15   0.1159278   0.3535018
+2018.20   0.1161082   0.3534894
+2018.25   0.1162877   0.3534758
+2018.30   0.1164665   0.3534608
+2018.35   0.1166443   0.3534444
+2018.40   0.1168213   0.3534267
+2018.45   0.1169975   0.3534077
+2018.50   0.1171727   0.3533874
+2018.55   0.1173471   0.3533658
+2018.60   0.1175206   0.3533428
+2018.65   0.1176931   0.3533186
+2018.70   0.1178648   0.3532931
+2018.75   0.1180355   0.3532664
+2018.80   0.1182053   0.3532384
+2018.85   0.1183741   0.3532091
+2018.90   0.1185420   0.3531786
+2018.95   0.1187089   0.3531468
+2019.00   0.1188749   0.3531139
+2019.05   0.1190399   0.3530797
+2019.10   0.1192039   0.3530444
+2019.15   0.1193669   0.3530078
+2019.20   0.1195289   0.3529701
+2019.25   0.1196899   0.3529312
+2019.30   0.1198499   0.3528912
+2019.35   0.1200089   0.3528500
+2019.40   0.1201668   0.3528077
+2019.45   0.1203238   0.3527643
+2019.50   0.1204797   0.3527197
+2019.55   0.1206345   0.3526741
+2019.60   0.1207884   0.3526274
+2019.65   0.1209411   0.3525795
+2019.70   0.1210928   0.3525307
+2019.75   0.1212435   0.3524807
+2019.80   0.1213931   0.3524298
+2019.85   0.1215416   0.3523777
+2019.90   0.1216891   0.3523247
+2019.95   0.1218354   0.3522707
+2020.00   0.1219807   0.3522156
+2020.05   0.1221250   0.3521596
+2020.10   0.1222681   0.3521025
+2020.15   0.1224101   0.3520446
+2020.20   0.1225511   0.3519856
+2020.25   0.1226909   0.3519257
+2020.30   0.1228297   0.3518649
+2020.35   0.1229674   0.3518031
+2020.40   0.1231039   0.3517404
+2020.45   0.1232394   0.3516769
+2020.50   0.1233738   0.3516124
+2020.55   0.1235070   0.3515470
+2020.60   0.1236392   0.3514808
+2020.65   0.1237702   0.3514136
+2020.70   0.1239002   0.3513457
+2020.75   0.1240290   0.3512769
+2020.80   0.1241567   0.3512072
+2020.85   0.1242833   0.3511367
+2020.90   0.1244088   0.3510654
+2020.95   0.1245332   0.3509933
+2021.00   0.1246565   0.3509204
+2021.05   0.1247787   0.3508468
+2021.10   0.1248998   0.3507723
+2021.15   0.1250197   0.3506970
+2021.20   0.1251386   0.3506210
+2021.25   0.1252563   0.3505443
+2021.30   0.1253730   0.3504668
+2021.35   0.1254885   0.3503885
+2021.40   0.1256029   0.3503096
+2021.45   0.1257163   0.3502299
+2021.50   0.1258285   0.3501495
+2021.55   0.1259397   0.3500684
+2021.60   0.1260497   0.3499866
+2021.65   0.1261587   0.3499042
+2021.70   0.1262666   0.3498210
+2021.75   0.1263733   0.3497372
+2021.80   0.1264790   0.3496527
+2021.85   0.1265836   0.3495676
+2021.90   0.1266872   0.3494818
+2021.95   0.1267896   0.3493954
+2022.00   0.1268910   0.3493084
+2022.05   0.1269913   0.3492207
+2022.10   0.1270905   0.3491325
+2022.15   0.1271887   0.3490436
+2022.20   0.1272858   0.3489541
+2022.25   0.1273818   0.3488640
+2022.30   0.1274768   0.3487734
+2022.35   0.1275708   0.3486821
+2022.40   0.1276636   0.3485903
+2022.45   0.1277555   0.3484979
+2022.50   0.1278463   0.3484050
+2022.55   0.1279360   0.3483115
+2022.60   0.1280247   0.3482175
+2022.65   0.1281124   0.3481229
+2022.70   0.1281991   0.3480278
+2022.75   0.1282847   0.3479322
+2022.80   0.1283693   0.3478360
+2022.85   0.1284529   0.3477394
+2022.90   0.1285355   0.3476422
+2022.95   0.1286171   0.3475446
+2023.00   0.1286976   0.3474464
+2023.05   0.1287772   0.3473478
+2023.10   0.1288558   0.3472487
+2023.15   0.1289334   0.3471491
+2023.20   0.1290100   0.3470490
```

### Comparing `pyTMD-2.0.3/pyTMD/data/merged_deltat.data` & `pyTMD-2.0.4/pyTMD/data/merged_deltat.data`

 * *Files 1% similar despite different names*

```diff
@@ -7672,7 +7672,35 @@
  2023  3 31 69.2084
  2023  4  1 69.2083
  2023  4  2 69.2084
  2023  4  3 69.2087
  2023  4  4 69.2092
  2023  4  5 69.2098
  2023  4  6 69.2105
+ 2023  4  7 69.2112
+ 2023  4  8 69.2119
+ 2023  4  9 69.2124
+ 2023  4 10 69.2128
+ 2023  4 11 69.2130
+ 2023  4 12 69.2130
+ 2023  4 13 69.2130
+ 2023  4 14 69.2130
+ 2023  4 15 69.2132
+ 2023  4 16 69.2138
+ 2023  4 17 69.2146
+ 2023  4 18 69.2156
+ 2023  4 19 69.2165
+ 2023  4 20 69.2173
+ 2023  4 21 69.2179
+ 2023  4 22 69.2183
+ 2023  4 23 69.2184
+ 2023  4 24 69.2183
+ 2023  4 25 69.2181
+ 2023  4 26 69.2178
+ 2023  4 27 69.2176
+ 2023  4 28 69.2175
+ 2023  4 29 69.2175
+ 2023  4 30 69.2178
+ 2023  5  1 69.2182
+ 2023  5  2 69.2188
+ 2023  5  3 69.2195
+ 2023  5  4 69.2201
```

### Comparing `pyTMD-2.0.3/pyTMD/data/opoleloadcoefcmcor.txt.gz` & `pyTMD-2.0.4/pyTMD/data/opoleloadcoefcmcor.txt.gz`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.3/pyTMD/data/ser7.dat` & `pyTMD-2.0.4/pyTMD/data/ser7.dat`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
                                                                                
       **********************************************************************   
       *                                                                    *   
       *                   I E R S   B U L L E T I N - A                    *   
       *                                                                    *   
       *           Rapid Service/Prediction of Earth Orientation            *   
       **********************************************************************   
-      6 April 2023                                        Vol. XXXVI No. 014   
+      4 May 2023                                          Vol. XXXVI No. 018   
       ______________________________________________________________________   
       GENERAL INFORMATION:                                                     
          MJD = Julian Date - 2 400 000.5 days                                  
          UT2-UT1 = 0.022 sin(2*pi*T) - 0.012 cos(2*pi*T)                       
                                      - 0.006 sin(4*pi*T) + 0.007 cos(4*pi*T)   
             where pi = 3.14159265... and T is the date in Besselian years.     
          TT = TAI + 32.184 seconds                                             
@@ -49,518 +49,521 @@
      ________________________________________________________________________  
                                                                                
       COMBINED EARTH ORIENTATION PARAMETERS:                                   
                                                                                
                               IERS Rapid Service                               
               MJD      x    error     y    error   UT1-UTC   error             
                        "      "       "      "        s        s               
-   23  3 31  60034 -.02035 .00009 0.40219 .00009 -0.024413 0.000012          
-   23  4  1  60035 -.01885 .00009 0.40461 .00009 -0.024328 0.000012          
-   23  4  2  60036 -.01730 .00009 0.40738 .00009 -0.024399 0.000012          
-   23  4  3  60037 -.01561 .00009 0.41000 .00009 -0.024715 0.000008          
-   23  4  4  60038 -.01384 .00009 0.41265 .00009 -0.025218 0.000007          
-   23  4  5  60039 -.01224 .00009 0.41546 .00009 -0.025822 0.000007          
-   23  4  6  60040 -.01072 .00009 0.41839 .00009 -0.026508 0.000007          
+   23  4 28  60062 0.02151 .00009 0.46907 .00009 -0.033484 0.000012          
+   23  4 29  60063 0.02382 .00009 0.47067 .00009 -0.033535 0.000012          
+   23  4 30  60064 0.02597 .00009 0.47211 .00009 -0.033779 0.000015          
+   23  5  1  60065 0.02758 .00009 0.47345 .00009 -0.034219 0.000012          
+   23  5  2  60066 0.02886 .00009 0.47464 .00009 -0.034805 0.000013          
+   23  5  3  60067 0.03027 .00009 0.47567 .00009 -0.035459 0.000012          
+   23  5  4  60068 0.03192 .00009 0.47664 .00009 -0.036125 0.000012          
                                                                                
                               IERS Final Values                                
                                MJD        x        y      UT1-UTC              
                                           "        "         s                 
-           23  2  2           59977   -0.0035   0.2503  -0.01386       
-           23  2  3           59978   -0.0049   0.2526  -0.01310       
-           23  2  4           59979   -0.0064   0.2543  -0.01242       
-           23  2  5           59980   -0.0082   0.2559  -0.01188       
-           23  2  6           59981   -0.0100   0.2577  -0.01150       
-           23  2  7           59982   -0.0119   0.2597  -0.01127       
-           23  2  8           59983   -0.0142   0.2617  -0.01120       
-           23  2  9           59984   -0.0158   0.2634  -0.01124       
-           23  2 10           59985   -0.0167   0.2655  -0.01147       
-           23  2 11           59986   -0.0178   0.2680  -0.01179       
-           23  2 12           59987   -0.0196   0.2704  -0.01213       
-           23  2 13           59988   -0.0219   0.2731  -0.01236       
-           23  2 14           59989   -0.0245   0.2757  -0.01246       
-           23  2 15           59990   -0.0270   0.2782  -0.01235       
-           23  2 16           59991   -0.0294   0.2807  -0.01206       
-           23  2 17           59992   -0.0318   0.2829  -0.01169       
-           23  2 18           59993   -0.0341   0.2849  -0.01136       
-           23  2 19           59994   -0.0359   0.2868  -0.01131       
-           23  2 20           59995   -0.0373   0.2889  -0.01157       
-           23  2 21           59996   -0.0383   0.2914  -0.01216       
-           23  2 22           59997   -0.0389   0.2946  -0.01293       
-           23  2 23           59998   -0.0390   0.2983  -0.01371       
-           23  2 24           59999   -0.0391   0.3019  -0.01450       
-           23  2 25           60000   -0.0396   0.3051  -0.01514       
-           23  2 26           60001   -0.0409   0.3082  -0.01554       
-           23  2 27           60002   -0.0428   0.3108  -0.01561       
-           23  2 28           60003   -0.0441   0.3133  -0.01550       
-           23  3  1           60004   -0.0451   0.3164  -0.01528       
+           23  3  2           60005   -0.0461   0.3188  -0.01506       
+           23  3  3           60006   -0.0467   0.3211  -0.01482       
+           23  3  4           60007   -0.0469   0.3238  -0.01468       
+           23  3  5           60008   -0.0465   0.3266  -0.01468       
+           23  3  6           60009   -0.0457   0.3298  -0.01491       
+           23  3  7           60010   -0.0446   0.3333  -0.01537       
+           23  3  8           60011   -0.0435   0.3366  -0.01601       
+           23  3  9           60012   -0.0424   0.3398  -0.01678       
+           23  3 10           60013   -0.0413   0.3431  -0.01760       
+           23  3 11           60014   -0.0408   0.3464  -0.01840       
+           23  3 12           60015   -0.0405   0.3495  -0.01909       
+           23  3 13           60016   -0.0401   0.3526  -0.01960       
+           23  3 14           60017   -0.0397   0.3560  -0.01991       
+           23  3 15           60018   -0.0397   0.3594  -0.02006       
+           23  3 16           60019   -0.0398   0.3622  -0.02007       
+           23  3 17           60020   -0.0397   0.3646  -0.02004       
+           23  3 18           60021   -0.0390   0.3669  -0.02013       
+           23  3 19           60022   -0.0381   0.3690  -0.02049       
+           23  3 20           60023   -0.0369   0.3713  -0.02114       
+           23  3 21           60024   -0.0355   0.3740  -0.02200       
+           23  3 22           60025   -0.0339   0.3771  -0.02296       
+           23  3 23           60026   -0.0325   0.3802  -0.02389       
+           23  3 24           60027   -0.0312   0.3833  -0.02469       
+           23  3 25           60028   -0.0299   0.3864  -0.02522       
+           23  3 26           60029   -0.0284   0.3895  -0.02543       
+           23  3 27           60030   -0.0266   0.3926  -0.02539       
+           23  3 28           60031   -0.0247   0.3954  -0.02518       
+           23  3 29           60032   -0.0230   0.3979  -0.02488       
+           23  3 30           60033   -0.0217   0.4000  -0.02458       
+           23  3 31           60034   -0.0204   0.4022  -0.02439       
+           23  4  1           60035   -0.0188   0.4046  -0.02434       
                                                                                
       _______________________________________________________________________  
                                                                                
       PREDICTIONS:                                                             
       The following formulas will not reproduce the predictions given below,   
       but may be used to extend the predictions beyond the end of this table.  
                                                                                
-      x =  0.1589 - 0.1152 cos A + 0.0163 sin A - 0.0532 cos C + 0.0623 sin C  
-      y =  0.3443 + 0.0143 cos A + 0.1096 sin A + 0.0623 cos C + 0.0532 sin C  
-         UT1-UTC = -0.0075 + 0.00020 (MJD - 60048) - (UT2-UT1)                 
+      x =  0.1424 - 0.0845 cos A + 0.0826 sin A - 0.0244 cos C + 0.0613 sin C  
+      y =  0.3369 + 0.0754 cos A + 0.0822 sin A + 0.0613 cos C + 0.0244 sin C  
+         UT1-UTC = -0.0082 + 0.00018 (MJD - 60076) - (UT2-UT1)                 
                                                                                
-      where A = 2*pi*(MJD-60040)/365.25 and C = 2*pi*(MJD-60040)/435.          
+      where A = 2*pi*(MJD-60068)/365.25 and C = 2*pi*(MJD-60068)/435.          
                                                                                
-         TAI-UTC(MJD 60041) = 37.0                                             
+         TAI-UTC(MJD 60069) = 37.0                                             
       The accuracy may be estimated from the expressions:                      
-      S x,y = 0.00068 (MJD-60040)**0.80   S t = 0.00025 (MJD-60040)**0.75      
+      S x,y = 0.00068 (MJD-60068)**0.80   S t = 0.00025 (MJD-60068)**0.75      
       Estimated accuracies are:  Predictions     10 d   20 d   30 d   40 d     
                                  Polar coord's  0.004  0.007  0.010  0.013     
                                  UT1-UTC        0.0014 0.0024 0.0032 0.0040    
                                                                                
                     MJD      x(arcsec)   y(arcsec)   UT1-UTC(sec)              
-       2023  4  7  60041      -0.0092      0.4211     -0.02720         
-       2023  4  8  60042      -0.0077      0.4237     -0.02785         
-       2023  4  9  60043      -0.0061      0.4261     -0.02836         
-       2023  4 10  60044      -0.0044      0.4285     -0.02868         
-       2023  4 11  60045      -0.0027      0.4307     -0.02882         
-       2023  4 12  60046      -0.0010      0.4329     -0.02880         
-       2023  4 13  60047       0.0008      0.4351     -0.02875         
-       2023  4 14  60048       0.0026      0.4372     -0.02879         
-       2023  4 15  60049       0.0045      0.4393     -0.02904         
-       2023  4 16  60050       0.0064      0.4413     -0.02959         
-       2023  4 17  60051       0.0083      0.4434     -0.03041         
-       2023  4 18  60052       0.0102      0.4454     -0.03137         
-       2023  4 19  60053       0.0122      0.4474     -0.03233         
-       2023  4 20  60054       0.0142      0.4494     -0.03318         
-       2023  4 21  60055       0.0162      0.4513     -0.03378         
-       2023  4 22  60056       0.0183      0.4532     -0.03410         
-       2023  4 23  60057       0.0203      0.4550     -0.03413         
-       2023  4 24  60058       0.0224      0.4568     -0.03392         
-       2023  4 25  60059       0.0246      0.4586     -0.03355         
-       2023  4 26  60060       0.0267      0.4603     -0.03311         
-       2023  4 27  60061       0.0289      0.4620     -0.03270         
-       2023  4 28  60062       0.0311      0.4637     -0.03238         
-       2023  4 29  60063       0.0334      0.4653     -0.03222         
-       2023  4 30  60064       0.0357      0.4669     -0.03226         
-       2023  5  1  60065       0.0379      0.4684     -0.03249         
-       2023  5  2  60066       0.0403      0.4700     -0.03289         
-       2023  5  3  60067       0.0426      0.4714     -0.03341         
-       2023  5  4  60068       0.0450      0.4729     -0.03395         
-       2023  5  5  60069       0.0473      0.4743     -0.03443         
-       2023  5  6  60070       0.0498      0.4757     -0.03474         
-       2023  5  7  60071       0.0522      0.4770     -0.03483         
-       2023  5  8  60072       0.0546      0.4783     -0.03468         
-       2023  5  9  60073       0.0571      0.4796     -0.03435         
-       2023  5 10  60074       0.0596      0.4808     -0.03395         
-       2023  5 11  60075       0.0621      0.4820     -0.03360         
-       2023  5 12  60076       0.0646      0.4831     -0.03341         
-       2023  5 13  60077       0.0672      0.4842     -0.03346         
-       2023  5 14  60078       0.0697      0.4853     -0.03375         
-       2023  5 15  60079       0.0723      0.4863     -0.03421         
-       2023  5 16  60080       0.0749      0.4873     -0.03473         
-       2023  5 17  60081       0.0775      0.4883     -0.03518         
-       2023  5 18  60082       0.0801      0.4892     -0.03544         
-       2023  5 19  60083       0.0827      0.4900     -0.03544         
-       2023  5 20  60084       0.0854      0.4909     -0.03516         
-       2023  5 21  60085       0.0880      0.4917     -0.03462         
-       2023  5 22  60086       0.0907      0.4924     -0.03389         
-       2023  5 23  60087       0.0933      0.4931     -0.03304         
-       2023  5 24  60088       0.0960      0.4938     -0.03217         
-       2023  5 25  60089       0.0987      0.4944     -0.03136         
-       2023  5 26  60090       0.1014      0.4950     -0.03065         
-       2023  5 27  60091       0.1041      0.4956     -0.03010         
-       2023  5 28  60092       0.1068      0.4961     -0.02971         
-       2023  5 29  60093       0.1096      0.4965     -0.02947         
-       2023  5 30  60094       0.1123      0.4970     -0.02935         
-       2023  5 31  60095       0.1150      0.4973     -0.02928         
-       2023  6  1  60096       0.1177      0.4977     -0.02918         
-       2023  6  2  60097       0.1205      0.4980     -0.02896         
-       2023  6  3  60098       0.1232      0.4982     -0.02855         
-       2023  6  4  60099       0.1260      0.4984     -0.02789         
-       2023  6  5  60100       0.1287      0.4986     -0.02704         
-       2023  6  6  60101       0.1314      0.4988     -0.02608         
-       2023  6  7  60102       0.1342      0.4988     -0.02515         
-       2023  6  8  60103       0.1369      0.4989     -0.02438         
-       2023  6  9  60104       0.1397      0.4989     -0.02385         
-       2023  6 10  60105       0.1424      0.4989     -0.02357         
-       2023  6 11  60106       0.1451      0.4988     -0.02347         
-       2023  6 12  60107       0.1478      0.4987     -0.02343         
-       2023  6 13  60108       0.1506      0.4985     -0.02335         
-       2023  6 14  60109       0.1533      0.4983     -0.02310         
-       2023  6 15  60110       0.1560      0.4981     -0.02261         
-       2023  6 16  60111       0.1587      0.4978     -0.02186         
-       2023  6 17  60112       0.1614      0.4975     -0.02087         
-       2023  6 18  60113       0.1641      0.4971     -0.01968         
-       2023  6 19  60114       0.1667      0.4967     -0.01837         
-       2023  6 20  60115       0.1694      0.4963     -0.01702         
-       2023  6 21  60116       0.1721      0.4958     -0.01571         
-       2023  6 22  60117       0.1747      0.4953     -0.01451         
-       2023  6 23  60118       0.1773      0.4947     -0.01346         
-       2023  6 24  60119       0.1799      0.4942     -0.01258         
-       2023  6 25  60120       0.1826      0.4935     -0.01185         
-       2023  6 26  60121       0.1851      0.4928     -0.01125         
-       2023  6 27  60122       0.1877      0.4921     -0.01073         
-       2023  6 28  60123       0.1903      0.4914     -0.01020         
-       2023  6 29  60124       0.1928      0.4906     -0.00960         
-       2023  6 30  60125       0.1954      0.4897     -0.00884         
-       2023  7  1  60126       0.1979      0.4889     -0.00786         
-       2023  7  2  60127       0.2004      0.4880     -0.00669         
-       2023  7  3  60128       0.2028      0.4870     -0.00538         
-       2023  7  4  60129       0.2053      0.4861     -0.00406         
-       2023  7  5  60130       0.2077      0.4850     -0.00289         
-       2023  7  6  60131       0.2101      0.4840     -0.00196         
-       2023  7  7  60132       0.2125      0.4829     -0.00132         
-       2023  7  8  60133       0.2149      0.4818     -0.00091         
-       2023  7  9  60134       0.2173      0.4806     -0.00061         
-       2023  7 10  60135       0.2196      0.4794     -0.00029         
-       2023  7 11  60136       0.2219      0.4782      0.00018         
-       2023  7 12  60137       0.2242      0.4769      0.00087         
-       2023  7 13  60138       0.2264      0.4756      0.00181         
-       2023  7 14  60139       0.2286      0.4743      0.00299         
-       2023  7 15  60140       0.2309      0.4730      0.00435         
-       2023  7 16  60141       0.2330      0.4716      0.00584         
-       2023  7 17  60142       0.2352      0.4701      0.00737         
-       2023  7 18  60143       0.2373      0.4687      0.00887         
-       2023  7 19  60144       0.2394      0.4672      0.01026         
-       2023  7 20  60145       0.2415      0.4657      0.01150         
-       2023  7 21  60146       0.2435      0.4641      0.01257         
-       2023  7 22  60147       0.2455      0.4625      0.01348         
-       2023  7 23  60148       0.2475      0.4609      0.01426         
-       2023  7 24  60149       0.2494      0.4593      0.01496         
-       2023  7 25  60150       0.2514      0.4576      0.01565         
-       2023  7 26  60151       0.2532      0.4559      0.01639         
-       2023  7 27  60152       0.2551      0.4542      0.01724         
-       2023  7 28  60153       0.2569      0.4524      0.01827         
-       2023  7 29  60154       0.2587      0.4507      0.01949         
-       2023  7 30  60155       0.2605      0.4489      0.02086         
-       2023  7 31  60156       0.2622      0.4470      0.02227         
-       2023  8  1  60157       0.2639      0.4452      0.02358         
-       2023  8  2  60158       0.2655      0.4433      0.02465         
-       2023  8  3  60159       0.2671      0.4414      0.02540         
-       2023  8  4  60160       0.2687      0.4395      0.02584         
-       2023  8  5  60161       0.2703      0.4375      0.02608         
-       2023  8  6  60162       0.2718      0.4356      0.02629         
-       2023  8  7  60163       0.2733      0.4336      0.02662         
-       2023  8  8  60164       0.2747      0.4315      0.02717         
-       2023  8  9  60165       0.2761      0.4295      0.02798         
-       2023  8 10  60166       0.2775      0.4275      0.02905         
-       2023  8 11  60167       0.2788      0.4254      0.03030         
-       2023  8 12  60168       0.2801      0.4233      0.03168         
-       2023  8 13  60169       0.2813      0.4212      0.03310         
-       2023  8 14  60170       0.2825      0.4191      0.03447         
-       2023  8 15  60171       0.2837      0.4169      0.03574         
-       2023  8 16  60172       0.2849      0.4147      0.03684         
-       2023  8 17  60173       0.2859      0.4126      0.03776         
-       2023  8 18  60174       0.2870      0.4104      0.03849         
-       2023  8 19  60175       0.2880      0.4082      0.03907         
-       2023  8 20  60176       0.2890      0.4059      0.03953         
-       2023  8 21  60177       0.2899      0.4037      0.03996         
-       2023  8 22  60178       0.2908      0.4015      0.04041         
-       2023  8 23  60179       0.2917      0.3992      0.04097         
-       2023  8 24  60180       0.2925      0.3969      0.04166         
-       2023  8 25  60181       0.2933      0.3946      0.04254         
-       2023  8 26  60182       0.2940      0.3923      0.04356         
-       2023  8 27  60183       0.2947      0.3900      0.04465         
-       2023  8 28  60184       0.2954      0.3877      0.04570         
-       2023  8 29  60185       0.2960      0.3854      0.04654         
-       2023  8 30  60186       0.2965      0.3831      0.04706         
-       2023  8 31  60187       0.2971      0.3807      0.04723         
-       2023  9  1  60188       0.2975      0.3784      0.04711         
-       2023  9  2  60189       0.2980      0.3761      0.04686         
-       2023  9  3  60190       0.2984      0.3737      0.04664         
-       2023  9  4  60191       0.2987      0.3713      0.04662         
-       2023  9  5  60192       0.2991      0.3690      0.04688         
-       2023  9  6  60193       0.2993      0.3666      0.04742         
-       2023  9  7  60194       0.2996      0.3643      0.04818         
-       2023  9  8  60195       0.2998      0.3619      0.04910         
-       2023  9  9  60196       0.2999      0.3595      0.05007         
-       2023  9 10  60197       0.3000      0.3571      0.05102         
-       2023  9 11  60198       0.3001      0.3548      0.05187         
-       2023  9 12  60199       0.3001      0.3524      0.05256         
-       2023  9 13  60200       0.3001      0.3500      0.05307         
-       2023  9 14  60201       0.3000      0.3477      0.05337         
-       2023  9 15  60202       0.2999      0.3453      0.05351         
-       2023  9 16  60203       0.2998      0.3429      0.05352         
-       2023  9 17  60204       0.2996      0.3406      0.05347         
-       2023  9 18  60205       0.2994      0.3382      0.05343         
-       2023  9 19  60206       0.2991      0.3359      0.05349         
-       2023  9 20  60207       0.2988      0.3335      0.05369         
-       2023  9 21  60208       0.2985      0.3312      0.05406         
-       2023  9 22  60209       0.2981      0.3288      0.05459         
-       2023  9 23  60210       0.2977      0.3265      0.05522         
-       2023  9 24  60211       0.2972      0.3242      0.05583         
-       2023  9 25  60212       0.2967      0.3219      0.05631         
-       2023  9 26  60213       0.2961      0.3196      0.05651         
-       2023  9 27  60214       0.2956      0.3173      0.05637         
-       2023  9 28  60215       0.2949      0.3150      0.05589         
-       2023  9 29  60216       0.2943      0.3128      0.05517         
-       2023  9 30  60217       0.2936      0.3105      0.05440         
-       2023 10  1  60218       0.2928      0.3083      0.05375         
-       2023 10  2  60219       0.2920      0.3060      0.05334         
-       2023 10  3  60220       0.2912      0.3038      0.05322         
-       2023 10  4  60221       0.2904      0.3016      0.05338         
-       2023 10  5  60222       0.2895      0.2994      0.05372         
-       2023 10  6  60223       0.2885      0.2972      0.05416         
-       2023 10  7  60224       0.2876      0.2951      0.05460         
-       2023 10  8  60225       0.2866      0.2929      0.05494         
-       2023 10  9  60226       0.2855      0.2908      0.05513         
-       2023 10 10  60227       0.2844      0.2887      0.05512         
-       2023 10 11  60228       0.2833      0.2866      0.05491         
-       2023 10 12  60229       0.2822      0.2845      0.05450         
-       2023 10 13  60230       0.2810      0.2825      0.05393         
-       2023 10 14  60231       0.2798      0.2805      0.05327         
-       2023 10 15  60232       0.2785      0.2784      0.05259         
-       2023 10 16  60233       0.2772      0.2765      0.05199         
-       2023 10 17  60234       0.2759      0.2745      0.05154         
-       2023 10 18  60235       0.2745      0.2725      0.05128         
-       2023 10 19  60236       0.2732      0.2706      0.05123         
-       2023 10 20  60237       0.2717      0.2687      0.05133         
-       2023 10 21  60238       0.2703      0.2668      0.05151         
-       2023 10 22  60239       0.2688      0.2650      0.05164         
-       2023 10 23  60240       0.2673      0.2631      0.05161         
-       2023 10 24  60241       0.2658      0.2613      0.05134         
-       2023 10 25  60242       0.2642      0.2595      0.05080         
-       2023 10 26  60243       0.2626      0.2578      0.05006         
-       2023 10 27  60244       0.2610      0.2560      0.04923         
-       2023 10 28  60245       0.2593      0.2543      0.04847         
-       2023 10 29  60246       0.2576      0.2526      0.04793         
-       2023 10 30  60247       0.2559      0.2510      0.04769         
-       2023 10 31  60248       0.2542      0.2494      0.04777         
-       2023 11  1  60249       0.2524      0.2478      0.04811         
-       2023 11  2  60250       0.2506      0.2462      0.04862         
-       2023 11  3  60251       0.2488      0.2446      0.04920         
-       2023 11  4  60252       0.2469      0.2431      0.04975         
-       2023 11  5  60253       0.2451      0.2416      0.05018         
-       2023 11  6  60254       0.2432      0.2402      0.05042         
-       2023 11  7  60255       0.2413      0.2388      0.05046         
-       2023 11  8  60256       0.2393      0.2374      0.05029         
-       2023 11  9  60257       0.2374      0.2360      0.04994         
-       2023 11 10  60258       0.2354      0.2347      0.04948         
-       2023 11 11  60259       0.2334      0.2334      0.04896         
-       2023 11 12  60260       0.2314      0.2321      0.04849         
-       2023 11 13  60261       0.2294      0.2309      0.04813         
-       2023 11 14  60262       0.2273      0.2296      0.04794         
-       2023 11 15  60263       0.2252      0.2285      0.04794         
-       2023 11 16  60264       0.2231      0.2273      0.04812         
-       2023 11 17  60265       0.2210      0.2262      0.04837         
-       2023 11 18  60266       0.2189      0.2251      0.04857         
-       2023 11 19  60267       0.2168      0.2241      0.04858         
-       2023 11 20  60268       0.2146      0.2231      0.04835         
-       2023 11 21  60269       0.2124      0.2221      0.04782         
-       2023 11 22  60270       0.2102      0.2212      0.04708         
-       2023 11 23  60271       0.2080      0.2203      0.04621         
-       2023 11 24  60272       0.2058      0.2194      0.04536         
-       2023 11 25  60273       0.2036      0.2186      0.04468         
-       2023 11 26  60274       0.2014      0.2178      0.04431         
-       2023 11 27  60275       0.1991      0.2170      0.04427         
-       2023 11 28  60276       0.1969      0.2163      0.04459         
-       2023 11 29  60277       0.1946      0.2156      0.04512         
-       2023 11 30  60278       0.1923      0.2149      0.04580         
-       2023 12  1  60279       0.1901      0.2143      0.04645         
-       2023 12  2  60280       0.1878      0.2137      0.04703         
-       2023 12  3  60281       0.1855      0.2131      0.04744         
-       2023 12  4  60282       0.1832      0.2126      0.04764         
-       2023 12  5  60283       0.1809      0.2121      0.04776         
-       2023 12  6  60284       0.1785      0.2117      0.04778         
-       2023 12  7  60285       0.1762      0.2113      0.04776         
-       2023 12  8  60286       0.1739      0.2109      0.04769         
-       2023 12  9  60287       0.1716      0.2106      0.04768         
-       2023 12 10  60288       0.1693      0.2103      0.04772         
-       2023 12 11  60289       0.1669      0.2100      0.04790         
-       2023 12 12  60290       0.1646      0.2098      0.04825         
-       2023 12 13  60291       0.1623      0.2096      0.04872         
-       2023 12 14  60292       0.1599      0.2094      0.04921         
-       2023 12 15  60293       0.1576      0.2093      0.04962         
-       2023 12 16  60294       0.1553      0.2092      0.04983         
-       2023 12 17  60295       0.1530      0.2092      0.04982         
-       2023 12 18  60296       0.1506      0.2092      0.04954         
-       2023 12 19  60297       0.1483      0.2092      0.04902         
-       2023 12 20  60298       0.1460      0.2092      0.04840         
-       2023 12 21  60299       0.1437      0.2093      0.04779         
-       2023 12 22  60300       0.1414      0.2095      0.04727         
-       2023 12 23  60301       0.1391      0.2096      0.04702         
-       2023 12 24  60302       0.1368      0.2098      0.04702         
-       2023 12 25  60303       0.1345      0.2101      0.04726         
-       2023 12 26  60304       0.1322      0.2104      0.04770         
-       2023 12 27  60305       0.1300      0.2107      0.04832         
-       2023 12 28  60306       0.1277      0.2110      0.04893         
-       2023 12 29  60307       0.1255      0.2114      0.04953         
-       2023 12 30  60308       0.1232      0.2118      0.05002         
-       2023 12 31  60309       0.1210      0.2122      0.05028         
-       2024  1  1  60310       0.1188      0.2127      0.05033         
-       2024  1  2  60311       0.1166      0.2132      0.05027         
-       2024  1  3  60312       0.1144      0.2138      0.05018         
-       2024  1  4  60313       0.1122      0.2144      0.05006         
-       2024  1  5  60314       0.1101      0.2150      0.04999         
-       2024  1  6  60315       0.1079      0.2156      0.05001         
-       2024  1  7  60316       0.1058      0.2163      0.05017         
-       2024  1  8  60317       0.1037      0.2170      0.05056         
-       2024  1  9  60318       0.1016      0.2178      0.05111         
-       2024  1 10  60319       0.0995      0.2186      0.05180         
-       2024  1 11  60320       0.0974      0.2194      0.05249         
-       2024  1 12  60321       0.0954      0.2202      0.05307         
-       2024  1 13  60322       0.0934      0.2211      0.05336         
-       2024  1 14  60323       0.0913      0.2220      0.05342         
-       2024  1 15  60324       0.0894      0.2230      0.05308         
-       2024  1 16  60325       0.0874      0.2239      0.05256         
-       2024  1 17  60326       0.0854      0.2249      0.05204         
-       2024  1 18  60327       0.0835      0.2259      0.05161         
-       2024  1 19  60328       0.0816      0.2270      0.05138         
-       2024  1 20  60329       0.0797      0.2281      0.05139         
-       2024  1 21  60330       0.0779      0.2292      0.05167         
-       2024  1 22  60331       0.0760      0.2303      0.05213         
-       2024  1 23  60332       0.0742      0.2315      0.05274         
-       2024  1 24  60333       0.0724      0.2327      0.05345         
-       2024  1 25  60334       0.0707      0.2339      0.05419         
-       2024  1 26  60335       0.0689      0.2352      0.05478         
-       2024  1 27  60336       0.0672      0.2365      0.05524         
-       2024  1 28  60337       0.0655      0.2378      0.05554         
-       2024  1 29  60338       0.0639      0.2391      0.05567         
-       2024  1 30  60339       0.0622      0.2405      0.05567         
-       2024  1 31  60340       0.0606      0.2419      0.05568         
-       2024  2  1  60341       0.0590      0.2433      0.05568         
-       2024  2  2  60342       0.0575      0.2447      0.05575         
-       2024  2  3  60343       0.0560      0.2461      0.05598         
-       2024  2  4  60344       0.0545      0.2476      0.05632         
-       2024  2  5  60345       0.0530      0.2491      0.05682         
-       2024  2  6  60346       0.0516      0.2506      0.05751         
-       2024  2  7  60347       0.0502      0.2522      0.05828         
-       2024  2  8  60348       0.0488      0.2537      0.05896         
-       2024  2  9  60349       0.0475      0.2553      0.05944         
-       2024  2 10  60350       0.0462      0.2569      0.05961         
-       2024  2 11  60351       0.0449      0.2586      0.05941         
-       2024  2 12  60352       0.0436      0.2602      0.05887         
-       2024  2 13  60353       0.0424      0.2619      0.05817         
-       2024  2 14  60354       0.0412      0.2635      0.05752         
-       2024  2 15  60355       0.0401      0.2652      0.05710         
-       2024  2 16  60356       0.0390      0.2670      0.05699         
-       2024  2 17  60357       0.0379      0.2687      0.05717         
-       2024  2 18  60358       0.0368      0.2704      0.05762         
-       2024  2 19  60359       0.0358      0.2722      0.05814         
-       2024  2 20  60360       0.0348      0.2740      0.05873         
-       2024  2 21  60361       0.0339      0.2758      0.05928         
-       2024  2 22  60362       0.0329      0.2776      0.05966         
-       2024  2 23  60363       0.0321      0.2794      0.05990         
-       2024  2 24  60364       0.0312      0.2812      0.05999         
-       2024  2 25  60365       0.0304      0.2831      0.05991         
-       2024  2 26  60366       0.0296      0.2849      0.05968         
-       2024  2 27  60367       0.0289      0.2868      0.05935         
-       2024  2 28  60368       0.0282      0.2887      0.05893         
-       2024  2 29  60369       0.0275      0.2906      0.05850         
-       2024  3  1  60370       0.0269      0.2925      0.05812         
-       2024  3  2  60371       0.0263      0.2944      0.05786         
-       2024  3  3  60372       0.0257      0.2963      0.05775         
-       2024  3  4  60373       0.0252      0.2982      0.05779         
-       2024  3  5  60374       0.0247      0.3002      0.05790         
-       2024  3  6  60375       0.0242      0.3021      0.05796         
-       2024  3  7  60376       0.0238      0.3041      0.05786         
-       2024  3  8  60377       0.0234      0.3060      0.05742         
-       2024  3  9  60378       0.0231      0.3080      0.05660         
-       2024  3 10  60379       0.0228      0.3099      0.05537         
-       2024  3 11  60380       0.0225      0.3119      0.05389         
-       2024  3 12  60381       0.0223      0.3139      0.05242         
-       2024  3 13  60382       0.0221      0.3158      0.05119         
-       2024  3 14  60383       0.0219      0.3178      0.05032         
-       2024  3 15  60384       0.0218      0.3198      0.04980         
-       2024  3 16  60385       0.0217      0.3218      0.04959         
-       2024  3 17  60386       0.0216      0.3237      0.04957         
-       2024  3 18  60387       0.0216      0.3257      0.04970         
-       2024  3 19  60388       0.0216      0.3277      0.04987         
-       2024  3 20  60389       0.0217      0.3297      0.04999         
-       2024  3 21  60390       0.0218      0.3316      0.04996         
-       2024  3 22  60391       0.0219      0.3336      0.04974         
-       2024  3 23  60392       0.0221      0.3356      0.04938         
-       2024  3 24  60393       0.0222      0.3376      0.04887         
-       2024  3 25  60394       0.0225      0.3395      0.04827         
-       2024  3 26  60395       0.0228      0.3415      0.04778         
-       2024  3 27  60396       0.0231      0.3434      0.04747         
-       2024  3 28  60397       0.0234      0.3454      0.04735         
-       2024  3 29  60398       0.0238      0.3473      0.04746         
-       2024  3 30  60399       0.0242      0.3493      0.04779         
-       2024  3 31  60400       0.0246      0.3512      0.04831         
-       2024  4  1  60401       0.0251      0.3531      0.04894         
-       2024  4  2  60402       0.0256      0.3550      0.04961         
-       2024  4  3  60403       0.0262      0.3569      0.05017         
-       2024  4  4  60404       0.0267      0.3588      0.05046         
-       2024  4  5  60405       0.0274      0.3607      0.05035         
+       2023  5  5  60069       0.0338      0.4777     -0.03679         
+       2023  5  6  60070       0.0359      0.4789     -0.03735         
+       2023  5  7  60071       0.0381      0.4802     -0.03771         
+       2023  5  8  60072       0.0405      0.4816     -0.03790         
+       2023  5  9  60073       0.0428      0.4831     -0.03799         
+       2023  5 10  60074       0.0453      0.4845     -0.03806         
+       2023  5 11  60075       0.0477      0.4859     -0.03822         
+       2023  5 12  60076       0.0502      0.4872     -0.03857         
+       2023  5 13  60077       0.0526      0.4884     -0.03915         
+       2023  5 14  60078       0.0551      0.4896     -0.03993         
+       2023  5 15  60079       0.0576      0.4908     -0.04082         
+       2023  5 16  60080       0.0601      0.4919     -0.04170         
+       2023  5 17  60081       0.0626      0.4930     -0.04244         
+       2023  5 18  60082       0.0652      0.4940     -0.04297         
+       2023  5 19  60083       0.0678      0.4949     -0.04322         
+       2023  5 20  60084       0.0704      0.4959     -0.04316         
+       2023  5 21  60085       0.0731      0.4968     -0.04283         
+       2023  5 22  60086       0.0757      0.4977     -0.04229         
+       2023  5 23  60087       0.0784      0.4986     -0.04161         
+       2023  5 24  60088       0.0811      0.4994     -0.04090         
+       2023  5 25  60089       0.0839      0.5002     -0.04023         
+       2023  5 26  60090       0.0866      0.5009     -0.03968         
+       2023  5 27  60091       0.0893      0.5016     -0.03928         
+       2023  5 28  60092       0.0920      0.5023     -0.03904         
+       2023  5 29  60093       0.0948      0.5029     -0.03895         
+       2023  5 30  60094       0.0975      0.5035     -0.03897         
+       2023  5 31  60095       0.1003      0.5040     -0.03902         
+       2023  6  1  60096       0.1031      0.5045     -0.03902         
+       2023  6  2  60097       0.1059      0.5050     -0.03887         
+       2023  6  3  60098       0.1086      0.5054     -0.03851         
+       2023  6  4  60099       0.1114      0.5058     -0.03790         
+       2023  6  5  60100       0.1142      0.5061     -0.03706         
+       2023  6  6  60101       0.1170      0.5064     -0.03610         
+       2023  6  7  60102       0.1198      0.5066     -0.03516         
+       2023  6  8  60103       0.1226      0.5068     -0.03437         
+       2023  6  9  60104       0.1254      0.5070     -0.03381         
+       2023  6 10  60105       0.1282      0.5071     -0.03349         
+       2023  6 11  60106       0.1310      0.5072     -0.03337         
+       2023  6 12  60107       0.1338      0.5072     -0.03333         
+       2023  6 13  60108       0.1366      0.5072     -0.03325         
+       2023  6 14  60109       0.1394      0.5071     -0.03302         
+       2023  6 15  60110       0.1422      0.5070     -0.03256         
+       2023  6 16  60111       0.1450      0.5069     -0.03185         
+       2023  6 17  60112       0.1478      0.5067     -0.03089         
+       2023  6 18  60113       0.1506      0.5065     -0.02974         
+       2023  6 19  60114       0.1533      0.5062     -0.02848         
+       2023  6 20  60115       0.1561      0.5059     -0.02718         
+       2023  6 21  60116       0.1588      0.5056     -0.02592         
+       2023  6 22  60117       0.1616      0.5052     -0.02476         
+       2023  6 23  60118       0.1643      0.5048     -0.02375         
+       2023  6 24  60119       0.1670      0.5043     -0.02290         
+       2023  6 25  60120       0.1697      0.5038     -0.02220         
+       2023  6 26  60121       0.1724      0.5032     -0.02162         
+       2023  6 27  60122       0.1751      0.5026     -0.02110         
+       2023  6 28  60123       0.1778      0.5020     -0.02057         
+       2023  6 29  60124       0.1805      0.5013     -0.01996         
+       2023  6 30  60125       0.1831      0.5006     -0.01918         
+       2023  7  1  60126       0.1857      0.4999     -0.01818         
+       2023  7  2  60127       0.1884      0.4991     -0.01697         
+       2023  7  3  60128       0.1910      0.4983     -0.01561         
+       2023  7  4  60129       0.1935      0.4974     -0.01423         
+       2023  7  5  60130       0.1961      0.4965     -0.01297         
+       2023  7  6  60131       0.1987      0.4955     -0.01196         
+       2023  7  7  60132       0.2012      0.4945     -0.01122         
+       2023  7  8  60133       0.2037      0.4935     -0.01071         
+       2023  7  9  60134       0.2062      0.4925     -0.01031         
+       2023  7 10  60135       0.2086      0.4914     -0.00988         
+       2023  7 11  60136       0.2111      0.4902     -0.00930         
+       2023  7 12  60137       0.2135      0.4891     -0.00850         
+       2023  7 13  60138       0.2159      0.4879     -0.00745         
+       2023  7 14  60139       0.2183      0.4866     -0.00618         
+       2023  7 15  60140       0.2206      0.4853     -0.00472         
+       2023  7 16  60141       0.2230      0.4840     -0.00314         
+       2023  7 17  60142       0.2253      0.4827     -0.00153         
+       2023  7 18  60143       0.2275      0.4813      0.00003         
+       2023  7 19  60144       0.2298      0.4799      0.00148         
+       2023  7 20  60145       0.2320      0.4784      0.00278         
+       2023  7 21  60146       0.2342      0.4770      0.00389         
+       2023  7 22  60147       0.2364      0.4754      0.00483         
+       2023  7 23  60148       0.2385      0.4739      0.00563         
+       2023  7 24  60149       0.2406      0.4723      0.00635         
+       2023  7 25  60150       0.2427      0.4707      0.00705         
+       2023  7 26  60151       0.2447      0.4691      0.00780         
+       2023  7 27  60152       0.2468      0.4674      0.00867         
+       2023  7 28  60153       0.2487      0.4657      0.00971         
+       2023  7 29  60154       0.2507      0.4640      0.01094         
+       2023  7 30  60155       0.2526      0.4622      0.01233         
+       2023  7 31  60156       0.2545      0.4605      0.01376         
+       2023  8  1  60157       0.2564      0.4587      0.01509         
+       2023  8  2  60158       0.2582      0.4568      0.01618         
+       2023  8  3  60159       0.2600      0.4550      0.01695         
+       2023  8  4  60160       0.2617      0.4531      0.01741         
+       2023  8  5  60161       0.2635      0.4512      0.01768         
+       2023  8  6  60162       0.2651      0.4492      0.01790         
+       2023  8  7  60163       0.2668      0.4472      0.01824         
+       2023  8  8  60164       0.2684      0.4453      0.01879         
+       2023  8  9  60165       0.2700      0.4433      0.01962         
+       2023  8 10  60166       0.2715      0.4412      0.02069         
+       2023  8 11  60167       0.2730      0.4392      0.02195         
+       2023  8 12  60168       0.2745      0.4371      0.02333         
+       2023  8 13  60169       0.2759      0.4350      0.02474         
+       2023  8 14  60170       0.2773      0.4329      0.02611         
+       2023  8 15  60171       0.2787      0.4307      0.02737         
+       2023  8 16  60172       0.2800      0.4286      0.02847         
+       2023  8 17  60173       0.2813      0.4264      0.02937         
+       2023  8 18  60174       0.2825      0.4242      0.03009         
+       2023  8 19  60175       0.2837      0.4220      0.03065         
+       2023  8 20  60176       0.2849      0.4198      0.03109         
+       2023  8 21  60177       0.2860      0.4175      0.03150         
+       2023  8 22  60178       0.2871      0.4153      0.03193         
+       2023  8 23  60179       0.2881      0.4130      0.03246         
+       2023  8 24  60180       0.2891      0.4107      0.03314         
+       2023  8 25  60181       0.2901      0.4084      0.03399         
+       2023  8 26  60182       0.2910      0.4061      0.03499         
+       2023  8 27  60183       0.2918      0.4038      0.03607         
+       2023  8 28  60184       0.2927      0.4014      0.03708         
+       2023  8 29  60185       0.2935      0.3991      0.03790         
+       2023  8 30  60186       0.2942      0.3967      0.03839         
+       2023  8 31  60187       0.2949      0.3944      0.03853         
+       2023  9  1  60188       0.2956      0.3920      0.03839         
+       2023  9  2  60189       0.2962      0.3896      0.03810         
+       2023  9  3  60190       0.2968      0.3872      0.03786         
+       2023  9  4  60191       0.2973      0.3848      0.03781         
+       2023  9  5  60192       0.2978      0.3824      0.03804         
+       2023  9  6  60193       0.2983      0.3800      0.03855         
+       2023  9  7  60194       0.2987      0.3776      0.03929         
+       2023  9  8  60195       0.2991      0.3752      0.04018         
+       2023  9  9  60196       0.2994      0.3727      0.04114         
+       2023  9 10  60197       0.2997      0.3703      0.04206         
+       2023  9 11  60198       0.2999      0.3679      0.04289         
+       2023  9 12  60199       0.3001      0.3654      0.04356         
+       2023  9 13  60200       0.3003      0.3630      0.04405         
+       2023  9 14  60201       0.3004      0.3606      0.04434         
+       2023  9 15  60202       0.3005      0.3581      0.04446         
+       2023  9 16  60203       0.3005      0.3557      0.04446         
+       2023  9 17  60204       0.3005      0.3533      0.04439         
+       2023  9 18  60205       0.3004      0.3508      0.04435         
+       2023  9 19  60206       0.3003      0.3484      0.04440         
+       2023  9 20  60207       0.3002      0.3460      0.04459         
+       2023  9 21  60208       0.3000      0.3436      0.04496         
+       2023  9 22  60209       0.2998      0.3411      0.04549         
+       2023  9 23  60210       0.2995      0.3387      0.04612         
+       2023  9 24  60211       0.2992      0.3363      0.04675         
+       2023  9 25  60212       0.2989      0.3339      0.04723         
+       2023  9 26  60213       0.2985      0.3315      0.04744         
+       2023  9 27  60214       0.2980      0.3291      0.04731         
+       2023  9 28  60215       0.2976      0.3268      0.04684         
+       2023  9 29  60216       0.2971      0.3244      0.04614         
+       2023  9 30  60217       0.2965      0.3220      0.04539         
+       2023 10  1  60218       0.2959      0.3197      0.04475         
+       2023 10  2  60219       0.2953      0.3174      0.04437         
+       2023 10  3  60220       0.2946      0.3150      0.04429         
+       2023 10  4  60221       0.2939      0.3127      0.04448         
+       2023 10  5  60222       0.2931      0.3104      0.04487         
+       2023 10  6  60223       0.2923      0.3081      0.04537         
+       2023 10  7  60224       0.2915      0.3059      0.04587         
+       2023 10  8  60225       0.2906      0.3036      0.04630         
+       2023 10  9  60226       0.2897      0.3014      0.04660         
+       2023 10 10  60227       0.2888      0.2992      0.04672         
+       2023 10 11  60228       0.2878      0.2969      0.04665         
+       2023 10 12  60229       0.2868      0.2947      0.04640         
+       2023 10 13  60230       0.2857      0.2926      0.04602         
+       2023 10 14  60231       0.2846      0.2904      0.04557         
+       2023 10 15  60232       0.2835      0.2883      0.04512         
+       2023 10 16  60233       0.2824      0.2862      0.04475         
+       2023 10 17  60234       0.2812      0.2841      0.04454         
+       2023 10 18  60235       0.2799      0.2820      0.04451         
+       2023 10 19  60236       0.2786      0.2799      0.04468         
+       2023 10 20  60237       0.2773      0.2779      0.04498         
+       2023 10 21  60238       0.2760      0.2759      0.04532         
+       2023 10 22  60239       0.2746      0.2739      0.04557         
+       2023 10 23  60240       0.2732      0.2719      0.04562         
+       2023 10 24  60241       0.2718      0.2699      0.04538         
+       2023 10 25  60242       0.2703      0.2680      0.04483         
+       2023 10 26  60243       0.2688      0.2661      0.04402         
+       2023 10 27  60244       0.2673      0.2642      0.04309         
+       2023 10 28  60245       0.2657      0.2624      0.04220         
+       2023 10 29  60246       0.2641      0.2605      0.04150         
+       2023 10 30  60247       0.2625      0.2587      0.04109         
+       2023 10 31  60248       0.2609      0.2570      0.04098         
+       2023 11  1  60249       0.2592      0.2552      0.04112         
+       2023 11  2  60250       0.2575      0.2535      0.04142         
+       2023 11  3  60251       0.2558      0.2518      0.04177         
+       2023 11  4  60252       0.2540      0.2501      0.04208         
+       2023 11  5  60253       0.2522      0.2485      0.04229         
+       2023 11  6  60254       0.2504      0.2469      0.04233         
+       2023 11  7  60255       0.2486      0.2453      0.04219         
+       2023 11  8  60256       0.2467      0.2438      0.04188         
+       2023 11  9  60257       0.2448      0.2423      0.04141         
+       2023 11 10  60258       0.2429      0.2408      0.04085         
+       2023 11 11  60259       0.2409      0.2393      0.04026         
+       2023 11 12  60260       0.2390      0.2379      0.03972         
+       2023 11 13  60261       0.2370      0.2365      0.03932         
+       2023 11 14  60262       0.2350      0.2351      0.03912         
+       2023 11 15  60263       0.2330      0.2338      0.03911         
+       2023 11 16  60264       0.2309      0.2325      0.03927         
+       2023 11 17  60265       0.2289      0.2312      0.03949         
+       2023 11 18  60266       0.2268      0.2300      0.03965         
+       2023 11 19  60267       0.2247      0.2288      0.03962         
+       2023 11 20  60268       0.2226      0.2276      0.03934         
+       2023 11 21  60269       0.2204      0.2265      0.03876         
+       2023 11 22  60270       0.2183      0.2254      0.03793         
+       2023 11 23  60271       0.2161      0.2243      0.03697         
+       2023 11 24  60272       0.2139      0.2233      0.03600         
+       2023 11 25  60273       0.2117      0.2223      0.03517         
+       2023 11 26  60274       0.2095      0.2213      0.03459         
+       2023 11 27  60275       0.2073      0.2204      0.03431         
+       2023 11 28  60276       0.2050      0.2195      0.03429         
+       2023 11 29  60277       0.2028      0.2187      0.03445         
+       2023 11 30  60278       0.2005      0.2178      0.03469         
+       2023 12  1  60279       0.1983      0.2171      0.03493         
+       2023 12  2  60280       0.1960      0.2163      0.03508         
+       2023 12  3  60281       0.1937      0.2156      0.03510         
+       2023 12  4  60282       0.1914      0.2149      0.03496         
+       2023 12  5  60283       0.1891      0.2143      0.03468         
+       2023 12  6  60284       0.1867      0.2137      0.03431         
+       2023 12  7  60285       0.1844      0.2131      0.03391         
+       2023 12  8  60286       0.1821      0.2126      0.03355         
+       2023 12  9  60287       0.1797      0.2121      0.03329         
+       2023 12 10  60288       0.1774      0.2116      0.03316         
+       2023 12 11  60289       0.1751      0.2112      0.03320         
+       2023 12 12  60290       0.1727      0.2108      0.03344         
+       2023 12 13  60291       0.1704      0.2105      0.03391         
+       2023 12 14  60292       0.1680      0.2101      0.03453         
+       2023 12 15  60293       0.1656      0.2099      0.03521         
+       2023 12 16  60294       0.1633      0.2096      0.03576         
+       2023 12 17  60295       0.1609      0.2094      0.03608         
+       2023 12 18  60296       0.1586      0.2093      0.03608         
+       2023 12 19  60297       0.1562      0.2091      0.03578         
+       2023 12 20  60298       0.1538      0.2090      0.03536         
+       2023 12 21  60299       0.1515      0.2090      0.03500         
+       2023 12 22  60300       0.1491      0.2090      0.03474         
+       2023 12 23  60301       0.1468      0.2090      0.03468         
+       2023 12 24  60302       0.1444      0.2090      0.03493         
+       2023 12 25  60303       0.1421      0.2091      0.03542         
+       2023 12 26  60304       0.1398      0.2093      0.03620         
+       2023 12 27  60305       0.1374      0.2094      0.03713         
+       2023 12 28  60306       0.1351      0.2096      0.03807         
+       2023 12 29  60307       0.1328      0.2099      0.03893         
+       2023 12 30  60308       0.1305      0.2101      0.03962         
+       2023 12 31  60309       0.1282      0.2104      0.04014         
+       2024  1  1  60310       0.1259      0.2108      0.04052         
+       2024  1  2  60311       0.1236      0.2112      0.04065         
+       2024  1  3  60312       0.1214      0.2116      0.04061         
+       2024  1  4  60313       0.1191      0.2120      0.04054         
+       2024  1  5  60314       0.1169      0.2125      0.04040         
+       2024  1  6  60315       0.1146      0.2130      0.04037         
+       2024  1  7  60316       0.1124      0.2136      0.04041         
+       2024  1  8  60317       0.1102      0.2142      0.04063         
+       2024  1  9  60318       0.1080      0.2148      0.04098         
+       2024  1 10  60319       0.1058      0.2154      0.04148         
+       2024  1 11  60320       0.1037      0.2161      0.04201         
+       2024  1 12  60321       0.1015      0.2168      0.04241         
+       2024  1 13  60322       0.0994      0.2176      0.04256         
+       2024  1 14  60323       0.0973      0.2184      0.04243         
+       2024  1 15  60324       0.0952      0.2192      0.04193         
+       2024  1 16  60325       0.0931      0.2200      0.04126         
+       2024  1 17  60326       0.0911      0.2209      0.04059         
+       2024  1 18  60327       0.0890      0.2218      0.04003         
+       2024  1 19  60328       0.0870      0.2228      0.03971         
+       2024  1 20  60329       0.0850      0.2238      0.03970         
+       2024  1 21  60330       0.0830      0.2248      0.04001         
+       2024  1 22  60331       0.0811      0.2258      0.04057         
+       2024  1 23  60332       0.0791      0.2269      0.04133         
+       2024  1 24  60333       0.0772      0.2280      0.04216         
+       2024  1 25  60334       0.0753      0.2291      0.04297         
+       2024  1 26  60335       0.0735      0.2302      0.04366         
+       2024  1 27  60336       0.0716      0.2314      0.04419         
+       2024  1 28  60337       0.0698      0.2326      0.04448         
+       2024  1 29  60338       0.0680      0.2339      0.04454         
+       2024  1 30  60339       0.0662      0.2351      0.04458         
+       2024  1 31  60340       0.0645      0.2364      0.04458         
+       2024  2  1  60341       0.0628      0.2377      0.04465         
+       2024  2  2  60342       0.0611      0.2391      0.04474         
+       2024  2  3  60343       0.0594      0.2404      0.04498         
+       2024  2  4  60344       0.0578      0.2418      0.04530         
+       2024  2  5  60345       0.0562      0.2432      0.04578         
+       2024  2  6  60346       0.0546      0.2447      0.04636         
+       2024  2  7  60347       0.0530      0.2461      0.04691         
+       2024  2  8  60348       0.0515      0.2476      0.04732         
+       2024  2  9  60349       0.0500      0.2491      0.04746         
+       2024  2 10  60350       0.0486      0.2507      0.04719         
+       2024  2 11  60351       0.0471      0.2522      0.04658         
+       2024  2 12  60352       0.0457      0.2538      0.04572         
+       2024  2 13  60353       0.0444      0.2554      0.04475         
+       2024  2 14  60354       0.0430      0.2570      0.04386         
+       2024  2 15  60355       0.0417      0.2586      0.04322         
+       2024  2 16  60356       0.0404      0.2603      0.04284         
+       2024  2 17  60357       0.0392      0.2620      0.04279         
+       2024  2 18  60358       0.0380      0.2637      0.04297         
+       2024  2 19  60359       0.0368      0.2654      0.04329         
+       2024  2 20  60360       0.0356      0.2671      0.04363         
+       2024  2 21  60361       0.0345      0.2689      0.04401         
+       2024  2 22  60362       0.0334      0.2706      0.04425         
+       2024  2 23  60363       0.0324      0.2724      0.04437         
+       2024  2 24  60364       0.0314      0.2742      0.04432         
+       2024  2 25  60365       0.0304      0.2760      0.04403         
+       2024  2 26  60366       0.0294      0.2778      0.04356         
+       2024  2 27  60367       0.0285      0.2796      0.04303         
+       2024  2 28  60368       0.0277      0.2815      0.04256         
+       2024  2 29  60369       0.0268      0.2833      0.04216         
+       2024  3  1  60370       0.0260      0.2852      0.04191         
+       2024  3  2  60371       0.0252      0.2871      0.04181         
+       2024  3  3  60372       0.0245      0.2890      0.04189         
+       2024  3  4  60373       0.0238      0.2909      0.04217         
+       2024  3  5  60374       0.0231      0.2928      0.04252         
+       2024  3  6  60375       0.0225      0.2947      0.04286         
+       2024  3  7  60376       0.0219      0.2967      0.04303         
+       2024  3  8  60377       0.0213      0.2986      0.04290         
+       2024  3  9  60378       0.0208      0.3005      0.04238         
+       2024  3 10  60379       0.0203      0.3025      0.04157         
+       2024  3 11  60380       0.0199      0.3044      0.04043         
+       2024  3 12  60381       0.0195      0.3064      0.03926         
+       2024  3 13  60382       0.0191      0.3084      0.03829         
+       2024  3 14  60383       0.0188      0.3104      0.03760         
+       2024  3 15  60384       0.0185      0.3123      0.03722         
+       2024  3 16  60385       0.0182      0.3143      0.03709         
+       2024  3 17  60386       0.0180      0.3163      0.03717         
+       2024  3 18  60387       0.0178      0.3183      0.03732         
+       2024  3 19  60388       0.0176      0.3203      0.03748         
+       2024  3 20  60389       0.0175      0.3223      0.03762         
+       2024  3 21  60390       0.0174      0.3242      0.03770         
+       2024  3 22  60391       0.0173      0.3262      0.03758         
+       2024  3 23  60392       0.0173      0.3282      0.03732         
+       2024  3 24  60393       0.0174      0.3302      0.03693         
+       2024  3 25  60394       0.0174      0.3322      0.03644         
+       2024  3 26  60395       0.0175      0.3342      0.03592         
+       2024  3 27  60396       0.0176      0.3362      0.03551         
+       2024  3 28  60397       0.0178      0.3381      0.03521         
+       2024  3 29  60398       0.0180      0.3401      0.03508         
+       2024  3 30  60399       0.0182      0.3421      0.03517         
+       2024  3 31  60400       0.0185      0.3440      0.03539         
+       2024  4  1  60401       0.0188      0.3460      0.03575         
+       2024  4  2  60402       0.0192      0.3480      0.03616         
+       2024  4  3  60403       0.0195      0.3499      0.03650         
+       2024  4  4  60404       0.0200      0.3518      0.03662         
+       2024  4  5  60405       0.0204      0.3538      0.03643         
+       2024  4  6  60406       0.0209      0.3557      0.03592         
+       2024  4  7  60407       0.0214      0.3576      0.03509         
+       2024  4  8  60408       0.0219      0.3595      0.03406         
+       2024  4  9  60409       0.0225      0.3614      0.03306         
+       2024  4 10  60410       0.0231      0.3633      0.03228         
+       2024  4 11  60411       0.0238      0.3652      0.03186         
+       2024  4 12  60412       0.0245      0.3670      0.03180         
+       2024  4 13  60413       0.0252      0.3689      0.03200         
+       2024  4 14  60414       0.0259      0.3707      0.03238         
+       2024  4 15  60415       0.0267      0.3725      0.03272         
+       2024  4 16  60416       0.0275      0.3743      0.03302         
+       2024  4 17  60417       0.0284      0.3761      0.03320         
+       2024  4 18  60418       0.0292      0.3779      0.03319         
+       2024  4 19  60419       0.0302      0.3797      0.03302         
+       2024  4 20  60420       0.0311      0.3814      0.03277         
+       2024  4 21  60421       0.0321      0.3832      0.03239         
+       2024  4 22  60422       0.0331      0.3849      0.03199         
+       2024  4 23  60423       0.0341      0.3866      0.03159         
+       2024  4 24  60424       0.0351      0.3883      0.03124         
+       2024  4 25  60425       0.0362      0.3900      0.03100         
+       2024  4 26  60426       0.0373      0.3916      0.03088         
+       2024  4 27  60427       0.0385      0.3932      0.03092         
+       2024  4 28  60428       0.0396      0.3949      0.03111         
+       2024  4 29  60429       0.0408      0.3964      0.03137         
+       2024  4 30  60430       0.0421      0.3980      0.03158         
+       2024  5  1  60431       0.0433      0.3996      0.03161         
+       2024  5  2  60432       0.0446      0.4011      0.03136         
+       2024  5  3  60433       0.0459      0.4026      0.03077         
       These predictions are based on all announced leap seconds.               
                                                                                
       CELESTIAL POLE OFFSET SERIES:                                            
                            NEOS Celestial Pole Offset Series                   
                        MJD      dpsi    error     deps    error                
                                         (msec. of arc)                         
-                      60020  -108.26    0.97   -8.18    0.07   
-                      60021  -108.08    0.32   -8.33    0.16   
-                      60022  -107.89    0.61   -8.30    0.09   
-                      60023  -107.76    0.61   -8.12    0.09   
-                      60024  -107.74    0.61   -7.97    0.09   
+                      60047  -107.11    0.81   -9.29    0.04   
+                      60048  -106.56    0.81   -9.40    0.04   
                                                                                
                      IERS Celestial Pole Offset Final Series                   
                            MJD          dpsi      deps                         
                                         (msec. of arc)                         
-                          59977      -110.2      -6.3                      
-                          59978      -110.0      -6.4                      
-                          59979      -109.9      -6.5                      
-                          59980      -109.9      -6.5                      
-                          59981      -109.9      -6.3                      
-                          59982      -109.7      -6.1                      
-                          59983      -109.4      -6.0                      
-                          59984      -109.1      -5.9                      
-                          59985      -109.0      -5.9                      
-                          59986      -109.0      -5.9                      
-                          59987      -109.3      -6.1                      
-                          59988      -109.5      -6.4                      
-                          59989      -109.6      -6.5                      
-                          59990      -110.0      -6.5                      
-                          59991      -110.6      -6.6                      
-                          59992      -111.1      -6.8                      
-                          59993      -110.9      -7.1                      
-                          59994      -110.3      -7.2                      
-                          59995      -109.5      -7.0                      
-                          59996      -109.0      -6.9                      
-                          59997      -108.9      -6.8                      
-                          59998      -109.1      -6.8                      
-                          59999      -109.4      -6.7                      
-                          60000      -109.8      -6.7                      
-                          60001      -110.0      -6.9                      
-                          60002      -110.0      -7.2                      
-                          60003      -109.9      -7.5                      
-                          60004      -109.7      -7.4                      
+                          60005      -109.4      -7.3                      
+                          60006      -109.0      -7.3                      
+                          60007      -108.6      -7.4                      
+                          60008      -108.5      -7.4                      
+                          60009      -108.5      -7.3                      
+                          60010      -108.4      -7.2                      
+                          60011      -108.4      -7.1                      
+                          60012      -108.4      -7.1                      
+                          60013      -108.6      -7.3                      
+                          60014      -108.7      -7.4                      
+                          60015      -108.8      -7.5                      
+                          60016      -108.9      -7.7                      
+                          60017      -108.8      -7.8                      
+                          60018      -108.6      -7.9                      
+                          60019      -108.4      -8.1                      
+                          60020      -108.2      -8.3                      
+                          60021      -108.1      -8.4                      
+                          60022      -107.9      -8.4                      
+                          60023      -107.8      -8.2                      
+                          60024      -107.8      -8.0                      
+                          60025      -107.8      -8.0                      
+                          60026      -107.9      -8.0                      
+                          60027      -108.1      -8.0                      
+                          60028      -108.3      -8.1                      
+                          60029      -108.5      -8.2                      
+                          60030      -108.5      -8.4                      
+                          60031      -108.4      -8.6                      
+                          60032      -108.2      -8.6                      
+                          60033      -107.8      -8.6                      
+                          60034      -107.4      -8.8                      
+                          60035      -106.9      -8.9                      
                                                             
                      IAU2000A Celestial Pole Offset Series  
                       MJD      dX     error     dY     error
                                     (msec. of arc)          
-                      60020    0.320  0.388   -0.076   0.067          
-                      60021    0.306  0.128   -0.079   0.160          
-                      60022    0.292  0.243   -0.083   0.090          
-                      60023    0.276  0.243   -0.086   0.090          
-                      60024    0.260  0.243   -0.090   0.090          
+                      60047    0.311  0.323   -0.003   0.040          
+                      60048    0.318  0.323   -0.002   0.040          
                                                                                
                                                                                
                  IAU2000A Celestial Pole Offset Final Series 
                              MJD     dX         dY           
                              (msec. of arc)          
-                           59977     0.41      -0.16
-                           59978     0.37      -0.17
-                           59979     0.34      -0.16
-                           59980     0.31      -0.15
-                           59981     0.28      -0.13
-                           59982     0.25      -0.12
-                           59983     0.27      -0.09
-                           59984     0.30      -0.06
-                           59985     0.33      -0.02
-                           59986     0.34      -0.04
-                           59987     0.34      -0.08
-                           59988     0.33      -0.11
-                           59989     0.33      -0.15
-                           59990     0.27      -0.14
-                           59991     0.20      -0.12
-                           59992     0.13      -0.10
-                           59993     0.15      -0.12
-                           59994     0.21      -0.15
-                           59995     0.26      -0.18
-                           59996     0.31      -0.21
-                           59997     0.32      -0.17
-                           59998     0.32      -0.12
-                           59999     0.31      -0.07
-                           60000     0.32      -0.05
-                           60001     0.32      -0.04
-                           60002     0.33      -0.02
-                           60003     0.33      -0.00
-                           60004     0.33       0.06
+                           60005     0.31       0.12
+                           60006     0.31       0.19
+                           60007     0.32       0.17
+                           60008     0.34       0.11
+                           60009     0.35       0.04
+                           60010     0.35      -0.04
+                           60011     0.33      -0.06
+                           60012     0.29      -0.05
+                           60013     0.26      -0.04
+                           60014     0.25      -0.05
+                           60015     0.25      -0.06
+                           60016     0.26      -0.08
+                           60017     0.27      -0.09
+                           60018     0.30      -0.10
+                           60019     0.32      -0.11
+                           60020     0.32      -0.11
+                           60021     0.30      -0.11
+                           60022     0.28      -0.11
+                           60023     0.25      -0.11
+                           60024     0.23      -0.10
+                           60025     0.24      -0.07
+                           60026     0.26      -0.04
+                           60027     0.28      -0.01
+                           60028     0.30       0.04
+                           60029     0.32       0.10
+                           60030     0.33       0.14
+                           60031     0.34       0.16
+                           60032     0.32       0.12
+                           60033     0.29       0.06
+                           60034     0.27      -0.01
+                           60035     0.27      -0.06
```

### Comparing `pyTMD-2.0.3/pyTMD/eop.py` & `pyTMD-2.0.4/pyTMD/eop.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,47 @@
 #!/usr/bin/env python
 u"""
 eop.py
-Written by Tyler Sutterley (03/2023)
+Written by Tyler Sutterley (04/2023)
 Utilities for maintaining and calculating Earth Orientation Parameters (EOP)
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
     lxml: processing XML and HTML in Python
         https://pypi.python.org/pypi/lxml
 
 PROGRAM DEPENDENCIES:
     utilities.py: download and management utilities for syncing files
 
 UPDATE HISTORY:
+    Updated 04/2023: using pathlib to define and expand paths
+        add wrapper function for interpolating daily EOP values
+        have mean pole and finals file as attributes of EOP module
     Updated 03/2023: add secular pole model from IERS 2018 conventions
     Updated 11/2022: added encoding for writing ascii files
         use f-strings for formatting verbose or ascii output
     Updated 04/2022: updated docstrings to numpy documentation format
     Updated 03/2021: replaced numpy bool/int to prevent deprecation warnings
     Written 11/2020
 """
 from __future__ import annotations
 
-import os
 import logging
+import pathlib
+import traceback
 import numpy as np
+import scipy.interpolate
 import pyTMD.utilities
 
+# IERS mean pole file for 2015 conventional mean pole
+_mean_pole_file = pyTMD.utilities.get_data_path(['data','mean-pole.tab'])
+# daily polar motion file from IERS
+_finals_file = pyTMD.utilities.get_data_path(['data','finals.all'])
+
 # PURPOSE: connects to servers and downloads mean pole files
 def update_mean_pole(verbose: bool = False, mode: oct = 0o775):
     """
     Connects to servers to download mean-pole.tab files from HPIERS servers
 
     - ftp://hpiers.obspm.fr/iers/eop/eopc01/mean-pole.readme
 
@@ -43,41 +53,42 @@
     Parameters
     ----------
     verbose: bool, default False
         print file information about output file
     mode: oct, default 0o775
         permissions mode of output file
     """
-    # local version of file
-    FILE = 'mean-pole.tab'
-    LOCAL = pyTMD.utilities.get_data_path(['data',FILE])
-    HASH = pyTMD.utilities.get_hash(LOCAL)
+    # check hash of local version of file
+    LOCAL = _mean_pole_file
+    HASH = pyTMD.utilities.get_hash(_mean_pole_file)
 
     # try downloading from Paris Observatory IERS Centers ftp servers
-    HOST = ['hpiers.obspm.fr','iers','eop','eopc01',FILE]
+    HOST = ['hpiers.obspm.fr', 'iers', 'eop', 'eopc01', 'mean-pole.tab']
     try:
         pyTMD.utilities.from_ftp(HOST, timeout=20, local=LOCAL,
             hash=HASH, verbose=verbose, mode=mode)
     except Exception as exc:
+        logging.debug(traceback.format_exc(exc))
         pass
     else:
         return
 
     # try downloading from Paris Observatory IERS Centers https servers
-    HOST = ['http://hpiers.obspm.fr','eoppc','eop','eopc01',FILE]
+    HOST = ['http://hpiers.obspm.fr', 'eoppc', 'eop', 'eopc01', 'mean-pole.tab']
     try:
         pyTMD.utilities.from_http(HOST, timeout=20, local=LOCAL,
             hash=HASH, verbose=verbose, mode=mode)
     except Exception as exc:
+        logging.debug(traceback.format_exc(exc))
         pass
     else:
         return
 
     # raise exception
-    raise RuntimeError(f'Unable to download {FILE}')
+    raise RuntimeError(f'Unable to download {LOCAL}')
 
 # PURPOSE: read table of IERS pole coordinates and calculate Gaussian average
 def calculate_mean_pole(verbose: bool = False, mode: oct = 0o775):
     """
     Calculates the mean pole coordinates x and y are obtained by a
     Gaussian-weighted average of the IERS pole coordinates
 
@@ -105,35 +116,35 @@
 
     # read contents from input file object
     file_contents = remote_buffer.read().decode('utf8').splitlines()
     header = file_contents[0][1:].split()
     nlines = len(file_contents) - 1
     data = {h:np.zeros((nlines)) for h in header}
     # extract data for all lines
-    for i,line in enumerate(file_contents[1:]):
+    for i, line in enumerate(file_contents[1:]):
         line_contents = line.split()
-        for h,l in zip(header,line_contents):
+        for h, l in zip(header, line_contents):
             data[h][i] = np.float64(l)
     # output mean pole coordinates
     xm = np.zeros((nlines))
     ym = np.zeros((nlines))
     # output file with mean pole coordinates
-    LOCAL = pyTMD.utilities.get_data_path(['data','mean-pole.tab'])
-    fid = open(LOCAL, mode='w', encoding='utf8')
-    logging.info(LOCAL)
-    for i,T in enumerate(data['an']):
+    LOCAL = _mean_pole_file
+    fid = LOCAL.open(mode='w', encoding='utf8')
+    logging.info(str(LOCAL))
+    for i, T in enumerate(data['an']):
         # mean pole is Gaussian Weight of all dates with a = 3.40 years.
-        Wi = np.exp(-0.5*((data['an']-T)/3.4)**2)
+        Wi = np.exp(-0.5*((data['an'] - T)/3.4)**2)
         xm[i] = np.sum(Wi*data['x(")'])/np.sum(Wi)
         ym[i] = np.sum(Wi*data['y(")'])/np.sum(Wi)
-        print('{0:6.2f} {1:11.7f} {2:11.7f}'.format(T,xm[i],ym[i]),file=fid)
+        print(f'{T:6.2f} {xm[i]:11.7f} {ym[i]:11.7f}', file=fid)
     # close the output file
     fid.close()
     # change the permissions mode of the output mean pole file
-    os.chmod(LOCAL, mode)
+    LOCAL.chmod(mode)
 
 # PURPOSE: connects to servers and downloads IERS pole coordinates files
 def pull_pole_coordinates(FILE: str, verbose: bool = False):
     """
     Connects to servers and downloads IERS pole coordinate files
 
     Servers and Mirrors
@@ -151,33 +162,33 @@
             - eopc01.1900-now.dat
             - eopc01.iau2000.1900-now.dat
             - eopc01.iau2000.1846-now.dat
     verbose: bool, default False
         print file information about output file
     """
     # try downloading from IERS ftp server
-    HOST = ['ftp.iers.org','products','eop','long-term','c01',FILE]
+    HOST = ['ftp.iers.org', 'products', 'eop', 'long-term', 'c01', FILE]
     try:
         buffer = pyTMD.utilities.from_ftp(HOST, verbose=verbose, timeout=20)
     except Exception as exc:
         pass
     else:
         return buffer
 
     # try downloading from Paris Observatory IERS Centers ftp servers
-    HOST = ['hpiers.obspm.fr','iers','eop','eopc01',FILE]
+    HOST = ['hpiers.obspm.fr', 'iers', 'eop', 'eopc01', FILE]
     try:
         buffer = pyTMD.utilities.from_ftp(HOST, verbose=verbose, timeout=20)
     except Exception as exc:
         pass
     else:
         return buffer
 
     # try downloading from Paris Observatory IERS Centers https servers
-    HOST = ['http://hpiers.obspm.fr','eoppc','eop','eopc01',FILE]
+    HOST = ['http://hpiers.obspm.fr', 'eoppc', 'eop', 'eopc01', FILE]
     try:
         buffer = pyTMD.utilities.from_http(HOST, verbose=verbose, timeout=20)
     except Exception as exc:
         pass
     else:
         return buffer
 
@@ -212,19 +223,19 @@
         timeout in seconds for blocking operations
     verbose: bool, default False
         print file information about output file
     mode: oct, default 0o775
         permissions mode of output file
     """
     # local version of file
-    LOCAL = pyTMD.utilities.get_data_path(['data','finals.all'])
+    LOCAL = _finals_file
     HASH = pyTMD.utilities.get_hash(LOCAL)
 
     # try downloading from US Naval Oceanography Portal
-    HOST = ['http://maia.usno.navy.mil','ser7','finals.all']
+    HOST = ['http://maia.usno.navy.mil', 'ser7', 'finals.all']
     try:
         pyTMD.utilities.from_http(HOST,
             timeout=timeout,
             local=LOCAL,
             hash=HASH,
             verbose=verbose,
             mode=mode
@@ -234,16 +245,16 @@
     else:
         return
 
     # try downloading from NASA Crustal Dynamics Data Information System
     # note: anonymous ftp access will be discontinued on 2020-10-31
     # will require using the following https Earthdata server after that date
     server = []
-    server.append(['cddis.nasa.gov','pub','products','iers','finals.all'])
-    server.append(['cddis.gsfc.nasa.gov','products','iers','finals.all'])
+    server.append(['cddis.nasa.gov', 'pub', 'products', 'iers', 'finals.all'])
+    server.append(['cddis.gsfc.nasa.gov', 'products', 'iers', 'finals.all'])
     for HOST in server:
         try:
             pyTMD.utilities.from_ftp(HOST,
                 timeout=timeout,
                 local=LOCAL,
                 hash=HASH,
                 verbose=verbose,
@@ -251,15 +262,15 @@
         except Exception as exc:
             pass
         else:
             return
 
     # try downloading from NASA Crustal Dynamics Data Information System
     # using NASA Earthdata credentials stored in netrc file
-    HOST = ['https://cddis.nasa.gov','archive','products','iers','finals.all']
+    HOST = ['https://cddis.nasa.gov', 'archive', 'products', 'iers', 'finals.all']
     try:
         pyTMD.utilities.from_cddis(HOST,
             username=username,
             password=password,
             timeout=timeout,
             local=LOCAL,
             hash=HASH,
@@ -268,40 +279,39 @@
         )
     except Exception as exc:
         pass
     else:
         return
 
 # IERS mean or secular pole conventions
-_conventions = ('2003','2010','2015','2018')
+_conventions = ('2003', '2010', '2015', '2018')
 # read table of mean pole values, calculate angular coordinates at epoch
 def iers_mean_pole(
-        input_file: str,
         input_epoch: np.ndarray,
-        convention: str,
+        convention: str = '2018',
         **kwargs
     ):
     """
     Calculates the angular coordinates of the IERS Conventional Mean Pole (CMP)
     or IERS Secular Pole (2018 convention)
 
     Parameters
     ----------
-    input_file: str
-        Full path to mean-pole.tab file provided by IERS
     input_epoch: np.ndarray
         Dates for the angular coordinates of the Conventional Mean Pole
         in decimal years
-    convention: str
+    convention: str, default '2018'
         IERS Mean or Secular Pole Convention
 
             - ``'2003'``
             - ``'2010'``
             - ``'2015'``
             - ``'2018'``
+    input_file: str or pathlib.Path
+        Full path to mean-pole.tab file provided by IERS
     fill_value: float, default np.nan
         Value for invalid flags
 
     Returns
     -------
     x: np.ndarray
         Angular coordinate x of conventional mean pole or secular pole
@@ -310,43 +320,50 @@
     flag: np.ndarray
         epoch is valid for version and version number is valid
 
     References
     ----------
     .. [1] G. Petit and B. Luzum (eds.), *IERS Conventions (2010)*,
         International Earth Rotation and Reference Systems Service (IERS),
-        `IERS Technical Note No. 36 <https://iers-conventions.obspm.fr/content/tn36.pdf>`_
+        `IERS Technical Note No. 36
+        <https://iers-conventions.obspm.fr/content/tn36.pdf>`_
     """
     # set default keyword arguments
+    kwargs.setdefault('file', _mean_pole_file)
     kwargs.setdefault('fill_value', np.nan)
     # verify IERS model version
     assert convention in _conventions, "Incorrect IERS model convention"
-    # read mean pole file
-    table = np.loadtxt(os.path.expanduser(input_file))
-    # reduce to 1971 to end date
-    ii, = np.nonzero(table[:,0] >= 1971)
-    table = np.copy(table[ii,:])
-    # reduce to yearly values
-    jj, = np.nonzero((table[:,0] % 1) == 0.0)
-    table = np.copy(table[jj,:])
-    end_time = table[-1,0] + 0.2
-    # final shape of the table
-    nrows, *_ = np.shape(table)
+    # read the conventional mean pole file
+    if (convention == '2015'):
+        # read mean pole file
+        input_file = pathlib.Path(kwargs['file']).expanduser().absolute()
+        table = np.loadtxt(input_file)
+        # reduce to 1971 to end date
+        ii, = np.nonzero(table[:, 0] >= 1971)
+        table = np.copy(table[ii,:])
+        # reduce to yearly values
+        jj, = np.nonzero((table[:, 0] % 1) == 0.0)
+        table = np.copy(table[jj,:])
+        end_time = table[-1, 0] + 0.2
+        # final shape of the table
+        nrows, *_ = np.shape(table)
+    else:
+        end_time = np.inf
     # allocate for output arrays
     x = np.full_like(input_epoch, kwargs['fill_value'])
     y = np.full_like(input_epoch, kwargs['fill_value'])
     flag = np.zeros_like(input_epoch, dtype=bool)
     for t, epoch in enumerate(input_epoch):
         # Conventional mean pole model in IERS Conventions 2003
-        if (convention == '2003') and (epoch >= 1975) and (epoch < end_time):
+        if (convention == '2003') and (epoch >= 1975):
             x[t] = 0.054 + 0.00083*(epoch - 2000.0)
             y[t] = 0.357 + 0.00395*(epoch - 2000.0)
             flag[t] = True
         # Conventional mean pole model in IERS Conventions 2010
-        elif (convention == '2010') and (epoch >= 1975) and (epoch < end_time):
+        elif (convention == '2010') and (epoch >= 1975):
             dx = epoch - 2000.0
             if (dx < 10.0):
                 x[t] = 0.055974 + 1.8243e-3*dx + 1.8413e-4*dx**2 + 7.024e-6*dx**3
                 y[t] = 0.346346 + 1.7896e-3*dx - 1.0729e-4*dx**2 - 0.908e-6*dx**3
             else:
                 x[t] = 0.023513 + 0.0076141*dx
                 y[t] = 0.358891 - 0.0006287*dx
@@ -355,68 +372,69 @@
         # must be below maximum valid date within file (e.g. 2015.2 for 2015)
         elif (convention == '2015') and (epoch >= 1975) and (epoch < end_time):
             # find epoch within mean pole table
             i = 1
             j = nrows+1
             while (j > (i+1)):
                 k = (i+j)//2
-                if (epoch < table[k,0]):
+                if (epoch < table[k, 0]):
                     j = k
                 else:
                     i = k
             # calculate differential from point in table
-            dx = epoch - table[i,0]
+            dx = epoch - table[i, 0]
             if (i == (nrows-1)):
-                x[t] = table[i,1] + dx*(table[nrows-1,1]-table[nrows-2,1])
-                y[t] = table[i,2] + dx*(table[nrows-1,1]-table[nrows-2,2])
+                x[t] = table[i, 1] + dx*(table[nrows-1, 1]-table[nrows-2, 1])
+                y[t] = table[i, 2] + dx*(table[nrows-1, 1]-table[nrows-2, 2])
             else:
-                x[t] = table[i,1] + dx*(table[i+1,1]-table[i,1])
-                y[t] = table[i,2] + dx*(table[i+1,2]-table[i,2])
+                x[t] = table[i, 1] + dx*(table[i+1, 1]-table[i, 1])
+                y[t] = table[i, 2] + dx*(table[i+1, 2]-table[i, 2])
             flag[t] = True
         # Secular pole model in IERS Conventions 2018
         elif (convention == '2018'):
             # calculate secular pole
             x[t] = 0.055 + 0.001677*(epoch - 2000.0)
             y[t] = 0.3205 + 0.00346*(epoch - 2000.0)
             flag[t] = True
     # return mean/secular pole values
     return (x, y, flag)
 
 # PURPOSE: read daily earth orientation parameters (EOP) file from IERS
-def iers_daily_EOP(input_file: str):
+def iers_daily_EOP(input_file: str | pathlib.Path = _finals_file):
     """
     Read daily earth orientation parameters (EOP) file from IERS
 
     Parameters
     ----------
-    input_file: str
+    input_file: str or Pathlib.Path
         full path to IERS EOP "finals" file
 
     Returns
     -------
     MJD: np.ndarray
-        modified Julian date of EOP measurements
+        Modified Julian Date of EOP measurements
     x: np.ndarray
         Angular coordinate x [arcsec]
     y: np.ndarray
         Angular coordinate y [arcsec]
 
     References
     ----------
     .. [1] G. Petit and B. Luzum (eds.), *IERS Conventions (2010)*,
         International Earth Rotation and Reference Systems Service (IERS),
-        `IERS Technical Note No. 36 <https://iers-conventions.obspm.fr/content/tn36.pdf>`_
+        `IERS Technical Note No. 36
+        <https://iers-conventions.obspm.fr/content/tn36.pdf>`_
     """
     # tilde-expansion of input file
-    input_file = os.path.expanduser(input_file)
+    input_file = pathlib.Path(input_file).expanduser().absolute()
     # check that IERS finals file is accessible
-    if not os.access(input_file, os.F_OK):
+    if not input_file.exists():
         raise FileNotFoundError(input_file)
     # read data file splitting at line breaks
-    with open(input_file, mode='r', encoding='utf8') as f:
+    with input_file.open(mode='r', encoding='utf8') as f:
         file_contents = f.read().splitlines()
     # number of data lines
     n_lines = len(file_contents)
     dinput = {}
     dinput['MJD'] = np.zeros((n_lines))
     dinput['x'] = np.zeros((n_lines))
     dinput['y'] = np.zeros((n_lines))
@@ -436,7 +454,52 @@
         counter += 1
     # reduce to data values
     dinput['MJD'] = dinput['MJD'][:counter]
     dinput['x'] = dinput['x'][:counter]
     dinput['y'] = dinput['y'][:counter]
     # return the date, flag and polar motion values
     return dinput
+
+def iers_polar_motion(
+        MJD: float | np.ndarray,
+        file: str | pathlib.Path = _finals_file,
+        **kwargs
+    ):
+    """
+    Interpolates daily earth orientation parameters (EOP) file from IERS
+
+    Parameters
+    ----------
+    MJD: np.ndarray
+        Modified Julian Date for interpolated measurements
+    file: str or Pathlib.Path
+        default path to IERS EOP "finals" file
+    k: int
+        Degree of the spline fit
+    s: int or float
+        Positive smoothing factor for the spline fit
+
+    Returns
+    -------
+    px: np.ndarray
+        Angular coordinate x [arcsec]
+    py: np.ndarray
+        Angular coordinate y [arcsec]
+
+    References
+    ----------
+    .. [1] G. Petit and B. Luzum (eds.), *IERS Conventions (2010)*,
+        International Earth Rotation and Reference Systems Service (IERS),
+        `IERS Technical Note No. 36
+        <https://iers-conventions.obspm.fr/content/tn36.pdf>`_
+    """
+    # set default parameters
+    kwargs.setdefault('k', 3)
+    kwargs.setdefault('s', 0)
+    # read IERS daily polar motion values
+    EOP = pyTMD.eop.iers_daily_EOP(file)
+    # interpolate daily polar motion values to MJD using cubic splines
+    xSPL = scipy.interpolate.UnivariateSpline(EOP['MJD'], EOP['x'], **kwargs)
+    ySPL = scipy.interpolate.UnivariateSpline(EOP['MJD'], EOP['y'], **kwargs)
+    px = xSPL(MJD)
+    py = ySPL(MJD)
+    return (px, py)
```

### Comparing `pyTMD-2.0.3/pyTMD/interpolate.py` & `pyTMD-2.0.4/pyTMD/interpolate.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.3/pyTMD/io/ATLAS.py` & `pyTMD-2.0.4/pyTMD/io/ATLAS.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 ATLAS.py
-Written by Tyler Sutterley (03/2023)
+Written by Tyler Sutterley (04/2023)
 
 Reads files for a tidal model and makes initial calculations to run tide program
 Includes functions to extract tidal harmonic constants from OTIS tide models for
     given locations
 netCDF4 files can be been compressed using gzip
 
 Reads netCDF4 ATLAS tidal solutions provided by Ohio State University and ESR
@@ -51,14 +51,15 @@
     netCDF4: Python interface to the netCDF C library
          https://unidata.github.io/netcdf4-python/netCDF4/index.html
 
 PROGRAM DEPENDENCIES:
     interpolate.py: interpolation routines for spatial data
 
 UPDATE HISTORY:
+    Updated 04/2023: using pathlib to define and expand tide model paths
     Updated 03/2023: add basic variable typing to function inputs
     Updated 12/2022: refactor tide read programs under io
         new functions to read and interpolate from constituents class
         new functions to output ATLAS formatted netCDF4 files
         refactored interpolation routines into new module
     Updated 11/2022: place some imports within try/except statements
         use f-strings for formatting verbose or ascii output
@@ -86,19 +87,19 @@
     Updated 07/2020: added function docstrings. separate bilinear interpolation
         changed TYPE variable to keyword argument. update griddata interpolation
     Updated 06/2020: use argmin and argmax in bilinear interpolation
     Written 09/2019
 """
 from __future__ import division, annotations
 
-import os
 import copy
 import gzip
 import uuid
 import logging
+import pathlib
 import datetime
 import warnings
 import numpy as np
 import pyTMD.version
 import pyTMD.io.constituents
 import pyTMD.interpolate
 
@@ -110,16 +111,16 @@
     warnings.warn("netCDF4 not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: extract harmonic constants from tide models at coordinates
 def extract_constants(
         ilon: np.ndarray, ilat: np.ndarray,
-        grid_file: str | None = None,
-        model_files: str | list | None = None,
+        grid_file: str | pathlib.Path | None = None,
+        model_files: str | list | pathlib.Path | None = None,
         **kwargs
     ):
     """
     Reads files for ATLAS netCDF4 tidal models
 
     Makes initial calculations to run the tide program
 
@@ -127,17 +128,17 @@
 
     Parameters
     ----------
     ilon: np.ndarray
         longitude to interpolate
     ilat: np.ndarray
         latitude to interpolate
-    grid_file: str or NoneType, default None
+    grid_file: str, pathlib.Path or NoneType, default None
         grid file for model
-    model_files: list or NoneType, default None
+    model_files: str, list, pathlib.Path or NoneType, default None
         list of model files for each constituent
     type: str, default 'z'
         Tidal variable to read
 
             - ``'z'``: heights
             - ``'u'``: horizontal transport velocities
             - ``'U'``: horizontal depth-averaged transport
@@ -185,22 +186,23 @@
     for old,new in deprecated_keywords.items():
         if old in kwargs.keys():
             warnings.warn(f"""Deprecated keyword argument {old}.
                 Changed to '{new}'""", DeprecationWarning)
             # set renamed argument to not break workflows
             kwargs[new] = copy.copy(kwargs[old])
 
-    # raise warning if model files are entered as a string
-    if isinstance(model_files, str):
+    # raise warning if model files are entered as a string or path
+    if isinstance(model_files, (str, pathlib.Path)):
         warnings.warn("Tide model is entered as a string")
         model_files = [model_files]
 
     # check that grid file is accessible
-    if not os.access(os.path.expanduser(grid_file), os.F_OK):
-        raise FileNotFoundError(os.path.expanduser(grid_file))
+    grid_file = pathlib.Path(grid_file).expanduser()
+    if not grid_file.exists():
+        raise FileNotFoundError(str(grid_file))
 
     # read the tide grid file for bathymetry and spatial coordinates
     lon, lat, bathymetry = read_netcdf_grid(grid_file, kwargs['type'],
         compressed=kwargs['compressed'])
 
     # adjust dimensions of input coordinates to be iterable
     ilon = np.atleast_1d(np.copy(ilon))
@@ -269,16 +271,17 @@
     ampl = np.ma.zeros((npts, nc))
     ampl.mask = np.zeros((npts, nc), dtype=bool)
     ph = np.ma.zeros((npts, nc))
     ph.mask = np.zeros((npts, nc), dtype=bool)
     # read and interpolate each constituent
     for i, model_file in enumerate(model_files):
         # check that model file is accessible
-        if not os.access(os.path.expanduser(model_file), os.F_OK):
-            raise FileNotFoundError(os.path.expanduser(model_file))
+        model_file = pathlib.Path(model_file).expanduser()
+        if not model_file.exists():
+            raise FileNotFoundError(str(model_file))
         if (kwargs['type'] == 'z'):
             # read constituent from elevation file
             hc, cons = read_netcdf_elevation(model_file,
                 compressed=kwargs['compressed'])
         elif kwargs['type'] in ('U','u','V','v'):
             # read constituent from transport file
             hc, cons = read_netcdf_transport(model_file, kwargs['type'],
@@ -344,26 +347,26 @@
     phase = ph*180.0/np.pi
     phase[phase < 0] += 360.0
     # return the interpolated values
     return (amplitude, phase, D, constituents)
 
 # PURPOSE: read harmonic constants from tide models
 def read_constants(
-        grid_file: str | None = None,
-        model_files: str | list | None = None,
+        grid_file: str | pathlib.Path | None = None,
+        model_files: str | list | pathlib.Path | None = None,
         **kwargs
     ):
     """
     Reads files for ATLAS netCDF4 tidal models
 
     Parameters
     ----------
-    grid_file: str or NoneType, default None
+    grid_file: str, pathlib.Path or NoneType, default None
         grid file for model
-    model_files: list or NoneType, default None
+    model_files: str, list, pathlib.Path or NoneType, default None
         list of model files for each constituent
     type: str, default 'z'
         Tidal variable to read
 
             - ``'z'``: heights
             - ``'u'``: horizontal transport velocities
             - ``'U'``: horizontal depth-averaged transport
@@ -377,22 +380,23 @@
     constituents: obj
         complex form of tide model constituents
     """
     # set default keyword arguments
     kwargs.setdefault('type', 'z')
     kwargs.setdefault('compressed', True)
 
-    # raise warning if model files are entered as a string
-    if isinstance(model_files, str):
+    # raise warning if model files are entered as a string or path
+    if isinstance(model_files, (str, pathlib.Path)):
         warnings.warn("Tide model is entered as a string")
         model_files = [model_files]
 
     # check that grid file is accessible
-    if not os.access(os.path.expanduser(grid_file), os.F_OK):
-        raise FileNotFoundError(os.path.expanduser(grid_file))
+    grid_file = pathlib.Path(grid_file).expanduser()
+    if not grid_file.exists():
+        raise FileNotFoundError(str(grid_file))
 
     # read the tide grid file for bathymetry and spatial coordinates
     lon, lat, bathymetry = read_netcdf_grid(grid_file, kwargs['type'],
         compressed=kwargs['compressed'])
 
     # grid step size of tide model
     dlon = lon[1] - lon[0]
@@ -406,16 +410,17 @@
         bathymetry=bathymetry.data,
         mask=bathymetry.mask
         )
 
     # read each model constituent
     for i, model_file in enumerate(model_files):
         # check that model file is accessible
-        if not os.access(os.path.expanduser(model_file), os.F_OK):
-            raise FileNotFoundError(os.path.expanduser(model_file))
+        model_file = pathlib.Path(model_file).expanduser()
+        if not model_file.exists():
+            raise FileNotFoundError(str(model_file))
         if (kwargs['type'] == 'z'):
             # read constituent from elevation file
             hc, cons = read_netcdf_elevation(model_file,
                 compressed=kwargs['compressed'])
         elif kwargs['type'] in ('U','u','V','v'):
             # read constituent from transport file
             hc, cons = read_netcdf_transport(model_file, kwargs['type'],
@@ -663,24 +668,24 @@
     temp[:,0] = input_matrix[:,-1]
     temp[:,1:-1] = input_matrix[:,:]
     temp[:,-1] = input_matrix[:,0]
     return temp
 
 # PURPOSE: read grid file
 def read_netcdf_grid(
-        input_file: str,
+        input_file: str | pathlib.Path,
         variable: str,
         **kwargs
     ):
     """
     Read grid file to extract model coordinates and bathymetry
 
     Parameters
     ----------
-    input_file: str
+    input_file: str or pathlib.Path
         input grid file
     variable: str
         Tidal variable to read
 
             - ``'z'``: heights
             - ``'u'``: horizontal transport velocities
             - ``'U'``: horizontal depth-averaged transport
@@ -698,21 +703,22 @@
         latitudinal coordinates of input grid
     bathymetry: np.ndarray
         model bathymetry
     """
     # set default keyword arguments
     kwargs.setdefault('compressed', False)
     # read the netcdf format tide grid file
+    input_file = pathlib.Path(input_file).expanduser()
     # reading a combined global solution with localized solutions
     if kwargs['compressed']:
         # read gzipped netCDF4 file
-        f = gzip.open(os.path.expanduser(input_file), 'rb')
+        f = gzip.open(input_file, 'rb')
         fileID = netCDF4.Dataset(uuid.uuid4().hex, 'r', memory=f.read())
     else:
-        fileID = netCDF4.Dataset(os.path.expanduser(input_file), 'r')
+        fileID = netCDF4.Dataset(input_file, 'r')
     # variable dimensions
     nx = fileID.dimensions['nx'].size
     ny = fileID.dimensions['ny'].size
     # allocate numpy masked array for bathymetry
     bathymetry = np.ma.zeros((ny,nx))
     # read bathymetry and coordinates for variable type
     if (variable == 'z'):
@@ -739,44 +745,45 @@
     fileID.close()
     f.close() if kwargs['compressed'] else None
     return (lon, lat, bathymetry)
 
 # PURPOSE: read elevation file to extract real and imaginary components for
 # constituent
 def read_netcdf_elevation(
-        input_file: str,
+        input_file: str | pathlib.Path,
         **kwargs
     ):
     """
     Read elevation file to extract real and imaginary components for constituent
 
     Parameters
     ----------
-    input_file: str
+    input_file: str or pathlib.Path
         input elevation file
     compressed: bool, default False
         Input file is gzip compressed
 
     Returns
     -------
     h: np.ndarray
         tidal elevation
     con: str
         tidal constituent ID
     """
     # set default keyword arguments
     kwargs.setdefault('compressed', False)
     # read the netcdf format tide elevation file
+    input_file = pathlib.Path(input_file).expanduser()
     # reading a combined global solution with localized solutions
     if kwargs['compressed']:
         # read gzipped netCDF4 file
-        f = gzip.open(os.path.expanduser(input_file), 'rb')
+        f = gzip.open(input_file, 'rb')
         fileID = netCDF4.Dataset(uuid.uuid4().hex, 'r', memory=f.read())
     else:
-        fileID = netCDF4.Dataset(os.path.expanduser(input_file), 'r')
+        fileID = netCDF4.Dataset(input_file, 'r')
     # constituent name
     con = fileID.variables['con'][:].tobytes().decode('utf8')
     # variable dimensions
     nx = fileID.dimensions['nx'].size
     ny = fileID.dimensions['ny'].size
     # real and imaginary components of elevation
     h = np.ma.zeros((ny,nx), dtype=np.complex64)
@@ -788,24 +795,24 @@
     f.close() if kwargs['compressed'] else None
     # return the elevation and constituent
     return (h, con.strip())
 
 # PURPOSE: read transport file to extract real and imaginary components for
 # constituent
 def read_netcdf_transport(
-        input_file: str,
+        input_file: str | pathlib.Path,
         variable: str,
         **kwargs
     ):
     """
     Read transport file to extract real and imaginary components for constituent
 
     Parameters
     ----------
-    input_file: str
+    input_file: str or pathlib.Path
         input transport file
     variable: str
         Tidal variable to read
 
             - ``'u'``: horizontal transport velocities
             - ``'U'``: horizontal depth-averaged transport
             - ``'v'``: vertical transport velocities
@@ -820,21 +827,22 @@
         tidal transport
     con: str
         tidal constituent ID
     """
     # set default keyword arguments
     kwargs.setdefault('compressed', False)
     # read the netcdf format tide transport file
+    input_file = pathlib.Path(input_file).expanduser()
     # reading a combined global solution with localized solutions
     if kwargs['compressed']:
         # read gzipped netCDF4 file
-        f = gzip.open(os.path.expanduser(input_file), 'rb')
+        f = gzip.open(input_file, 'rb')
         fileID = netCDF4.Dataset(uuid.uuid4().hex, 'r', memory=f.read())
     else:
-        fileID = netCDF4.Dataset(os.path.expanduser(input_file), 'r')
+        fileID = netCDF4.Dataset(input_file, 'r')
     # constituent name
     con = fileID.variables['con'][:].tobytes().decode('utf8')
     # variable dimensions
     nx = fileID.dimensions['nx'].size
     ny = fileID.dimensions['ny'].size
     # real and imaginary components of transport
     tr = np.ma.zeros((ny,nx), dtype=np.complex64)
@@ -849,15 +857,15 @@
     fileID.close()
     f.close() if kwargs['compressed'] else None
     # return the transport components and constituent
     return (tr, con.strip())
 
 # PURPOSE: output grid file in ATLAS netCDF format
 def output_netcdf_grid(
-        FILE: str,
+        FILE: str | pathlib.Path,
         hz: np.ndarray,
         hu: np.ndarray,
         hv: np.ndarray,
         lon_z: np.ndarray,
         lat_z: np.ndarray,
         lon_u: np.ndarray,
         lat_u: np.ndarray,
@@ -865,15 +873,15 @@
         lat_v: np.ndarray
     ):
     """
     Writes grid files in ATLAS netCDF format
 
     Parameters
     ----------
-    FILE: str
+    FILE: str or pathlib.Path
         output ATLAS grid file name
     hz: np.ndarray
         model bathymetry at z-nodes
     hu: np.ndarray
         model bathymetry at u-nodes
     hv: np.ndarray
         model bathymetry at v-nodes
@@ -886,16 +894,18 @@
     lat_u: np.ndarray
         latitude coordinates at u-nodes
     lon_v: np.ndarray
         longitude coordinates at v-nodes
     lat_v: np.ndarray
         latitude coordinates at v-nodes
     """
+    # tilde-expand output file
+    FILE = pathlib.Path(FILE).expanduser()
     # opening NetCDF file for writing
-    fileID = netCDF4.Dataset(os.path.expanduser(FILE), 'w', format="NETCDF4")
+    fileID = netCDF4.Dataset(FILE, 'w', format="NETCDF4")
     # define the NetCDF dimensions
     ny, nx = np.shape(hz)
     fileID.createDimension('nx', nx)
     fileID.createDimension('ny', ny)
     # defining the NetCDF variables
     nc = {}
     nc['lon_z'] = fileID.createVariable('lon_z', lon_z.dtype, ('nx',))
@@ -939,45 +949,47 @@
     fileID.type = "OTIS grid file"
     # add attribute for date created
     fileID.date_created = datetime.datetime.now().isoformat()
     # add attributes for software information
     fileID.software_reference = pyTMD.version.project_name
     fileID.software_version = pyTMD.version.full_version
     # Output NetCDF structure information
-    logging.info(FILE)
+    logging.info(str(FILE))
     logging.info(list(fileID.variables.keys()))
     # Closing the NetCDF file
     fileID.close()
 
 # PURPOSE: output elevation file in ATLAS netCDF format
 def output_netcdf_elevation(
-        FILE: str,
+        FILE: str | pathlib.Path,
         h: np.ndarray,
         lon_z: np.ndarray,
         lat_z: np.ndarray,
         constituent: str
     ):
     """
     Writes elevation files in ATLAS netCDF format
 
     Parameters
     ----------
-    FILE: str
+    FILE: str or pathlib.Path
         output ATLAS elevation file name
     h: np.ndarray
         Eulerian form of tidal elevation oscillation
     lon_z: np.ndarray
         longitude coordinates at z-nodes
     lat_z: np.ndarray
         latitude coordinates at z-nodes
     constituent: str
         tidal constituent ID
     """
+    # tilde-expand output file
+    FILE = pathlib.Path(FILE).expanduser()
     # opening NetCDF file for writing
-    fileID = netCDF4.Dataset(os.path.expanduser(FILE), 'w', format="NETCDF4")
+    fileID = netCDF4.Dataset(FILE, 'w', format="NETCDF4")
     # define the NetCDF dimensions
     ny, nx = np.shape(h)
     fileID.createDimension('nx', nx)
     fileID.createDimension('ny', ny)
     fileID.createDimension('nct', 4)
     # defining the NetCDF variables
     nc = {}
@@ -1021,36 +1033,36 @@
     fileID.type = "OTIS elevation file"
     # add attribute for date created
     fileID.date_created = datetime.datetime.now().isoformat()
     # add attributes for software information
     fileID.software_reference = pyTMD.version.project_name
     fileID.software_version = pyTMD.version.full_version
     # Output NetCDF structure information
-    logging.info(FILE)
+    logging.info(str(FILE))
     logging.info(list(fileID.variables.keys()))
     # Closing the NetCDF file
     fileID.close()
 
 # PURPOSE: output transport file in ATLAS netCDF format
 def output_netcdf_transport(
-        FILE: str,
+        FILE: str | pathlib.Path,
         u: np.ndarray,
         v: np.ndarray,
         lon_u: np.ndarray,
         lat_u: np.ndarray,
         lon_v: np.ndarray,
         lat_v: np.ndarray,
         constituent: str
     ):
     """
     Writes transport files in ATLAS netCDF format
 
     Parameters
     ----------
-    FILE: str
+    FILE: str or pathlib.Path
         output ATLAS transport file name
     u: np.ndarray
         Eulerian form of tidal zonal transport oscillation
     v: np.ndarray
         Eulerian form of tidal meridional transport oscillation
     lon_u: np.ndarray
         longitude coordinates at u-nodes
@@ -1059,16 +1071,18 @@
     lon_v: np.ndarray
         longitude coordinates at v-nodes
     lat_v: np.ndarray
         latitude coordinates at v-nodes
     constituents: str
         tidal constituent ID
     """
+    # tilde-expand output file
+    FILE = pathlib.Path(FILE).expanduser()
     # opening NetCDF file for writing
-    fileID = netCDF4.Dataset(os.path.expanduser(FILE), 'w', format="NETCDF4")
+    fileID = netCDF4.Dataset(FILE, 'w', format="NETCDF4")
     # define the NetCDF dimensions
     ny, nx = np.shape(u)
     fileID.createDimension('nx', nx)
     fileID.createDimension('ny', ny)
     fileID.createDimension('nct', 4)
     # defining the NetCDF variables
     nc = {}
@@ -1127,11 +1141,11 @@
     fileID.type = "OTIS transport file"
     # add attribute for date created
     fileID.date_created = datetime.datetime.now().isoformat()
     # add attributes for software information
     fileID.software_reference = pyTMD.version.project_name
     fileID.software_version = pyTMD.version.full_version
     # Output NetCDF structure information
-    logging.info(FILE)
+    logging.info(str(FILE))
     logging.info(list(fileID.variables.keys()))
     # Closing the NetCDF file
     fileID.close()
```

### Comparing `pyTMD-2.0.3/pyTMD/io/FES.py` & `pyTMD-2.0.4/pyTMD/io/FES.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,14 +53,15 @@
          https://unidata.github.io/netcdf4-python/netCDF4/index.html
 
 PROGRAM DEPENDENCIES:
     interpolate.py: interpolation routines for spatial data
 
 UPDATE HISTORY:
     Updated 04/2023: added global HAMTIDE11 model
+        using pathlib to define and expand tide model paths
     Updated 03/2023: add basic variable typing to function inputs
     Updated 12/2022: refactor tide read programs under io
         new functions to read and interpolate from constituents class
         new functions to output FES formatted netCDF4 files
         refactored interpolation routines into new module
     Updated 11/2022: place some imports within try/except statements
         use f-strings for formatting verbose or ascii output
@@ -85,19 +86,19 @@
     Updated 09/2020: set bounds error to false for regular grid interpolations
         adjust dimensions of input coordinates to be iterable
     Updated 08/2020: replaced griddata with scipy regular grid interpolators
     Written 07/2020
 """
 from __future__ import division, annotations
 
-import os
 import copy
 import gzip
 import uuid
 import logging
+import pathlib
 import datetime
 import warnings
 import numpy as np
 import pyTMD.version
 import pyTMD.interpolate
 import pyTMD.io.constituents
 
@@ -110,15 +111,15 @@
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: extract harmonic constants from tide models at coordinates
 def extract_constants(
         ilon: np.ndarray,
         ilat: np.ndarray,
-        model_files: str | list | None = None,
+        model_files: str | list | pathlib.Path | None = None,
         **kwargs
     ):
     """
     Reads files for a FES ascii or netCDF4 tidal model
 
     Makes initial calculations to run the tide program
 
@@ -126,15 +127,15 @@
 
     Parameters
     ----------
     ilon: np.ndarray
         longitude to interpolate
     ilat: np.ndarray
         latitude to interpolate
-    model_files: list or NoneType, default None
+    model_files: str, list, pathlib.Path or NoneType, default None
         list of model files for each constituent
     type: str, default 'z'
         Tidal variable to read
 
             - ``'z'``: heights
             - ``'u'``: horizontal transport velocities
             - ``'v'``: vertical transport velocities
@@ -186,16 +187,16 @@
     for old,new in deprecated_keywords.items():
         if old in kwargs.keys():
             warnings.warn(f"""Deprecated keyword argument {old}.
                 Changed to '{new}'""", DeprecationWarning)
             # set renamed argument to not break workflows
             kwargs[new] = copy.copy(kwargs[old])
 
-    # raise warning if model files are entered as a string
-    if isinstance(model_files, str):
+    # raise warning if model files are entered as a string or path
+    if isinstance(model_files, (str, pathlib.Path)):
         warnings.warn("Tide model is entered as a string")
         model_files = [model_files]
 
     # adjust dimensions of input coordinates to be iterable
     ilon = np.atleast_1d(np.copy(ilon))
     ilat = np.atleast_1d(np.copy(ilat))
     # number of points
@@ -205,25 +206,26 @@
 
     # amplitude and phase
     amplitude = np.ma.zeros((npts,nc))
     amplitude.mask = np.zeros((npts,nc),dtype=bool)
     ph = np.ma.zeros((npts,nc))
     ph.mask = np.zeros((npts,nc),dtype=bool)
     # read and interpolate each constituent
-    for i, fi in enumerate(model_files):
+    for i, model_file in enumerate(model_files):
         # check that model file is accessible
-        if not os.access(os.path.expanduser(fi), os.F_OK):
-            raise FileNotFoundError(os.path.expanduser(fi))
+        model_file = pathlib.Path(model_file).expanduser()
+        if not model_file.exists():
+            raise FileNotFoundError(str(model_file))
         # read constituent from elevation file
         if kwargs['version'] in ('FES1999','FES2004'):
             # FES ascii constituent files
-            hc,lon,lat = read_ascii_file(os.path.expanduser(fi), **kwargs)
+            hc, lon, lat = read_ascii_file(model_file, **kwargs)
         elif kwargs['version'] in ('FES2012','FES2014','EOT20','HAMTIDE11'):
             # FES netCDF4 constituent files
-            hc,lon,lat = read_netcdf_file(os.path.expanduser(fi), **kwargs)
+            hc, lon, lat = read_netcdf_file(model_file, **kwargs)
         # adjust longitudinal convention of input latitude and longitude
         # to fit tide model convention
         if (np.min(ilon) < 0.0) & (np.max(lon) > 180.0):
             # input points convention (-180:180)
             # tide model convention (0:360)
             ilon[ilon<0.0] += 360.0
         elif (np.max(ilon) > 180.0) & (np.min(lon) < 0.0):
@@ -298,23 +300,23 @@
     amplitude.data[amplitude.mask] = amplitude.fill_value
     phase.data[phase.mask] = phase.fill_value
     # return the interpolated values
     return (amplitude, phase)
 
 # PURPOSE: read harmonic constants from tide models
 def read_constants(
-        model_files: str | list | None = None,
+        model_files: str | list | pathlib.Path | None = None,
         **kwargs
     ):
     """
     Reads files for a FES ascii or netCDF4 tidal model
 
     Parameters
     ----------
-    model_files: list or NoneType, default None
+    model_files: str, list, pathlib.Path or NoneType, default None
         list of model files for each constituent
     type: str, default 'z'
         Tidal variable to read
 
             - ``'z'``: heights
             - ``'u'``: horizontal transport velocities
             - ``'v'``: vertical transport velocities
@@ -336,33 +338,34 @@
         complex form of tide model constituents
     """
     # set default keyword arguments
     kwargs.setdefault('type', 'z')
     kwargs.setdefault('version', None)
     kwargs.setdefault('compressed', False)
 
-    # raise warning if model files are entered as a string
-    if isinstance(model_files, str):
+    # raise warning if model files are entered as a string or path
+    if isinstance(model_files, (str, pathlib.Path)):
         warnings.warn("Tide model is entered as a string")
         model_files = [model_files]
 
     # save output constituents
     constituents = pyTMD.io.constituents()
     # read each model constituent
-    for i, fi in enumerate(model_files):
+    for i, model_file in enumerate(model_files):
         # check that model file is accessible
-        if not os.access(os.path.expanduser(fi), os.F_OK):
-            raise FileNotFoundError(os.path.expanduser(fi))
+        model_file = pathlib.Path(model_file).expanduser()
+        if not model_file.exists():
+            raise FileNotFoundError(str(model_file))
         # read constituent from elevation file
         if kwargs['version'] in ('FES1999','FES2004'):
             # FES ascii constituent files
-            hc,lon,lat = read_ascii_file(os.path.expanduser(fi), **kwargs)
+            hc, lon, lat = read_ascii_file(model_file, **kwargs)
         elif kwargs['version'] in ('FES2012','FES2014','EOT20','HAMTIDE11'):
             # FES netCDF4 constituent files
-            hc,lon,lat = read_netcdf_file(os.path.expanduser(fi), **kwargs)
+            hc, lon, lat = read_netcdf_file(model_file, **kwargs)
         # grid step size of tide model
         dlon = lon[1] - lon[0]
         # replace original values with extend arrays/matrices
         if np.isclose(lon[-1] - lon[0], 360.0 - dlon):
             lon = extend_array(lon, dlon)
             hc = extend_matrix(hc)
         # append extended constituent
@@ -569,21 +572,24 @@
     temp = np.ma.zeros((ny,nx+2), dtype=input_matrix.dtype)
     temp[:,0] = input_matrix[:,-1]
     temp[:,1:-1] = input_matrix[:,:]
     temp[:,-1] = input_matrix[:,0]
     return temp
 
 # PURPOSE: read FES ascii tide model grid files
-def read_ascii_file(input_file: str, **kwargs):
+def read_ascii_file(
+        input_file: str | pathlib.Path,
+        **kwargs
+    ):
     """
     Read FES (Finite Element Solution) tide model file
 
     Parameters
     ----------
-    input_file: str
+    input_file: str or pathlib.Path
         model file
     compressed: bool, default False
         Input file is gzip compressed
 
     Returns
     -------
     hc: np.ndarray
@@ -592,15 +598,15 @@
         longitude of tidal model
     lat: np.ndarray
         latitude of tidal model
     """
     # set default keyword arguments
     kwargs.setdefault('compressed', False)
     # tilde-expand input file
-    input_file = os.path.expanduser(input_file)
+    input_file = pathlib.Path(input_file).expanduser()
     # read input tide model file
     if kwargs['compressed']:
         # read gzipped ascii file
         with gzip.open(input_file, 'rb') as f:
             file_contents = f.read(input_file).splitlines()
     else:
         with open(input_file, mode="r", encoding='utf8') as f:
@@ -649,23 +655,23 @@
     hc = np.ma.array(amp*np.exp(-1j*ph*np.pi/180.0), mask=mask,
         fill_value=np.ma.default_fill_value(np.dtype(complex)))
     # return output variables
     return (hc, lon, lat)
 
 # PURPOSE: read FES netCDF4 tide model files
 def read_netcdf_file(
-        input_file: str,
+        input_file: str | pathlib.Path,
         **kwargs
     ):
     """
     Read FES (Finite Element Solution) tide model netCDF4 file
 
     Parameters
     ----------
-    input_file: str
+    input_file: str or pathlib.Path
         model file
     type: str or NoneType, default None
         Tidal variable to read
 
             - ``'z'``: heights
             - ``'u'``: horizontal transport velocities
             - ``'v'``: vertical transport velocities
@@ -688,21 +694,23 @@
     lat: np.ndarray
         latitude of tidal model
     """
     # set default keyword arguments
     kwargs.setdefault('type', None)
     kwargs.setdefault('version', None)
     kwargs.setdefault('compressed', False)
+    # tilde-expand input file
+    input_file = pathlib.Path(input_file).expanduser()
     # read the netcdf format tide elevation file
     if kwargs['compressed']:
         # read gzipped netCDF4 file
-        f = gzip.open(os.path.expanduser(input_file),'rb')
+        f = gzip.open(input_file, 'rb')
         fileID = netCDF4.Dataset(uuid.uuid4().hex, 'r', memory=f.read())
     else:
-        fileID = netCDF4.Dataset(os.path.expanduser(input_file), 'r')
+        fileID = netCDF4.Dataset(input_file, 'r')
     # variable dimensions for each model
     # amplitude and phase components for each type
     if kwargs['version'] in ('FES2012',):
         lon = fileID.variables['longitude'][:]
         lat = fileID.variables['latitude'][:]
         amp_key = dict(z='amplitude', u='Ua', v='Va')[kwargs['type']]
         phase_key = dict(z='phase', u='Ug', v='Vg')[kwargs['type']]
@@ -729,15 +737,15 @@
     hc = np.ma.array(amp*np.exp(-1j*ph*np.pi/180.0), mask=mask,
         fill_value=np.ma.default_fill_value(np.dtype(complex)))
     # return output variables
     return (hc, lon, lat)
 
 # PURPOSE: output tidal constituent file in FES2014 format
 def output_netcdf_file(
-        FILE: str,
+        FILE: str | pathlib.Path,
         hc: np.ndarray,
         lon: np.ndarray,
         lat: np.ndarray,
         constituent: str,
         **kwargs
     ):
     """
@@ -760,16 +768,18 @@
 
             - ``'z'``: heights
             - ``'u'``: horizontal transport velocities
             - ``'v'``: vertical transport velocities
     """
     # set default keyword arguments
     kwargs.setdefault('type', None)
+    # tilde-expand output file
+    FILE = pathlib.Path(FILE).expanduser()
     # opening NetCDF file for writing
-    fileID = netCDF4.Dataset(os.path.expanduser(FILE), 'w', format="NETCDF4")
+    fileID = netCDF4.Dataset(FILE, 'w', format="NETCDF4")
     # define the NetCDF dimensions
     fileID.createDimension('lon', len(lon))
     fileID.createDimension('lat', len(lat))
     fileID.createDimension('nct', 4)
     # calculate amplitude and phase
     amp = np.abs(hc)
     ph = 180.0*np.arctan2(-np.imag(hc), np.real(hc))/np.pi
@@ -828,11 +838,11 @@
     fileID.title = "FES tide file"
     # add attribute for date created
     fileID.date_created = datetime.datetime.now().isoformat()
     # add attributes for software information
     fileID.software_reference = pyTMD.version.project_name
     fileID.software_version = pyTMD.version.full_version
     # Output NetCDF structure information
-    logging.info(FILE)
+    logging.info(str(FILE))
     logging.info(list(fileID.variables.keys()))
     # Closing the NetCDF file
     fileID.close()
```

### Comparing `pyTMD-2.0.3/pyTMD/io/GOT.py` & `pyTMD-2.0.4/pyTMD/io/GOT.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
          https://unidata.github.io/netcdf4-python/netCDF4/index.html
 
 PROGRAM DEPENDENCIES:
     interpolate.py: interpolation routines for spatial data
 
 UPDATE HISTORY:
     Updated 04/2023: fix repeated longitudinal convention adjustment
+        using pathlib to define and expand tide model paths
     Updated 03/2023: add basic variable typing to function inputs
     Updated 12/2022: refactor tide read programs under io
         new functions to read and interpolate from constituents class
         new functions to read and write GOT netCDF4 files
         refactored interpolation routines into new module
     Updated 11/2022: use f-strings for formatting verbose or ascii output
     Updated 05/2022: reformat arguments to extract_GOT_constants definition
@@ -76,20 +77,20 @@
     Updated 12/2018: python3 compatibility updates for division and zip
     Updated 10/2018: added scale as load tides are in mm and ocean are in cm
     Updated 08/2018: added multivariate spline interpolation option
     Written 07/2018
 """
 from __future__ import division, annotations
 
-import os
 import re
 import copy
 import gzip
 import uuid
 import logging
+import pathlib
 import datetime
 import warnings
 import numpy as np
 import pyTMD.version
 import pyTMD.interpolate
 import pyTMD.io.constituents
 
@@ -102,15 +103,15 @@
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: extract harmonic constants from tide models at coordinates
 def extract_constants(
         ilon: np.ndarray,
         ilat: np.ndarray,
-        model_files: str | list | None = None,
+        model_files: str | pathlib.Path | list | None = None,
         **kwargs
     ):
     """
     Reads files for Richard Ray's Global Ocean Tide (GOT) models
 
     Makes initial calculations to run the tide program
 
@@ -118,15 +119,15 @@
 
     Parameters
     ----------
     ilon: np.ndarray
         longitude to interpolate
     ilat: np.ndarray
         latitude to interpolate
-    model_files: list or NoneType, default None
+    model_files: str, list, pathlib.Path or NoneType, default None
         list of model files for each constituent
     method: str, default 'spline'
         Interpolation method
 
             - ``'bilinear'``: quick bilinear interpolation
             - ``'spline'``: scipy bivariate spline interpolation
             - ``'linear'``, ``'nearest'``: scipy regular grid interpolations
@@ -169,16 +170,16 @@
     for old,new in deprecated_keywords.items():
         if old in kwargs.keys():
             warnings.warn(f"""Deprecated keyword argument {old}.
                 Changed to '{new}'""", DeprecationWarning)
             # set renamed argument to not break workflows
             kwargs[new] = copy.copy(kwargs[old])
 
-    # raise warning if model files are entered as a string
-    if isinstance(model_files,str):
+    # raise warning if model files are entered as a string or path
+    if isinstance(model_files, (str, pathlib.Path)):
         warnings.warn("Tide model is entered as a string")
         model_files = [model_files]
 
     # adjust dimensions of input coordinates to be iterable
     ilon = np.atleast_1d(np.copy(ilon))
     ilat = np.atleast_1d(np.copy(ilat))
     # number of points
@@ -192,24 +193,23 @@
     amplitude = np.ma.zeros((npts,nc))
     amplitude.mask = np.zeros((npts,nc),dtype=bool)
     ph = np.ma.zeros((npts,nc))
     ph.mask = np.zeros((npts,nc),dtype=bool)
     # read and interpolate each constituent
     for i,model_file in enumerate(model_files):
         # check that model file is accessible
-        if not os.access(os.path.expanduser(model_file), os.F_OK):
-            raise FileNotFoundError(os.path.expanduser(model_file))
+        model_file = pathlib.Path(model_file).expanduser()
+        if not model_file.exists():
+            raise FileNotFoundError(str(model_file))
         # read constituent from elevation file
         if (kwargs['grid'] == 'ascii'):
-            hc, lon, lat, cons = read_ascii_file(
-                os.path.expanduser(model_file),
+            hc, lon, lat, cons = read_ascii_file(model_file,
                 compressed=kwargs['compressed'])
         elif (kwargs['grid'] == 'netcdf'):
-            hc, lon, lat, cons = read_netcdf_file(
-                os.path.expanduser(model_file),
+            hc, lon, lat, cons = read_netcdf_file(model_file,
                 compressed=kwargs['compressed'])
         # append to the list of constituents
         constituents.append(cons)
         # adjust longitudinal convention of input latitude and longitude
         # to fit tide model convention
         if (np.min(ilon) < 0.0) & (np.max(lon) > 180.0):
             # input points convention (-180:180)
@@ -274,23 +274,23 @@
     amplitude.data[amplitude.mask] = amplitude.fill_value
     phase.data[phase.mask] = phase.fill_value
     # return the interpolated values
     return (amplitude, phase, constituents)
 
 # PURPOSE: read harmonic constants from tide models
 def read_constants(
-        model_files: str | list | None = None,
+        model_files: str | pathlib.Path | list | None = None,
         **kwargs
     ):
     """
     Reads files for Richard Ray's Global Ocean Tide (GOT) models
 
     Parameters
     ----------
-    model_files: list or NoneType, default None
+    model_files: str, list, pathlib.path or NoneType, default None
         list of model files for each constituent
     grid: str, default 'ascii'
         Tide model file type to read
 
             - ``'ascii'``: traditional GOT ascii format
             - ``'netcdf'``: GOT netCDF4 format
     compressed: bool, default False
@@ -302,33 +302,32 @@
         complex form of tide model constituents
     """
     # set default keyword arguments
     kwargs.setdefault('grid', 'ascii')
     kwargs.setdefault('compressed', False)
 
     # raise warning if model files are entered as a string
-    if isinstance(model_files,str):
+    if isinstance(model_files, (str, pathlib.Path)):
         warnings.warn("Tide model is entered as a string")
         model_files = [model_files]
 
     # save output constituents
     constituents = pyTMD.io.constituents()
     # read each model constituent
     for i, model_file in enumerate(model_files):
         # check that model file is accessible
-        if not os.access(os.path.expanduser(model_file), os.F_OK):
-            raise FileNotFoundError(os.path.expanduser(model_file))
+        model_file = pathlib.Path(model_file).expanduser()
+        if not model_file.exists():
+            raise FileNotFoundError(str(model_file))
         # read constituent from elevation file
         if (kwargs['grid'] == 'ascii'):
-            hc, lon, lat, cons = read_ascii_file(
-                os.path.expanduser(model_file),
+            hc, lon, lat, cons = read_ascii_file(model_file,
                 compressed=kwargs['compressed'])
         elif (kwargs['grid'] == 'netcdf'):
-            hc, lon, lat, cons = read_netcdf_file(
-                os.path.expanduser(model_file),
+            hc, lon, lat, cons = read_netcdf_file(model_file,
                 compressed=kwargs['compressed'])
         # grid step size of tide model
         dlon = np.abs(lon[1] - lon[0])
         # replace original values with extend matrices
         lon = extend_array(lon, dlon)
         hc = extend_matrix(hc)
         # append extended constituent
@@ -533,23 +532,23 @@
     temp[:,1:-2] = input_matrix[:,:]
     temp[:,-2] = input_matrix[:,0]
     temp[:,-1] = input_matrix[:,1]
     return temp
 
 # PURPOSE: read GOT model grid files
 def read_ascii_file(
-        input_file: str,
+        input_file: str | pathlib.Path,
         **kwargs
     ):
     """
     Read Richard Ray's Global Ocean Tide (GOT) model file
 
     Parameters
     ----------
-    input_file: str
+    input_file: str or pathlib.Path
         Model file
     compressed: bool, default False
         Input file is gzip compressed
 
     Returns
     -------
     hc: np.ndarray
@@ -560,15 +559,15 @@
         latitude of tidal model
     cons: str
         tidal constituent ID
     """
     # set default keyword arguments
     kwargs.setdefault('compressed', False)
     # tilde-expand input file
-    input_file = os.path.expanduser(input_file)
+    input_file = pathlib.Path(input_file).expanduser()
     # read input tide model file
     if kwargs['compressed']:
         # read gzipped ascii file
         with gzip.open(input_file, 'rb') as f:
             file_contents = f.read().decode('utf8').splitlines()
     else:
         with open(input_file, mode="r", encoding='utf8') as f:
@@ -614,23 +613,23 @@
     # set masks
     hc.mask = (amp.data == amp.fill_value) | (ph.data == ph.fill_value)
     # return output variables
     return (hc, lon, lat, cons)
 
 # PURPOSE: read GOT netCDF4 tide model files
 def read_netcdf_file(
-        input_file: str,
+        input_file: str | pathlib.Path,
         **kwargs
     ):
     """
     Read Richard Ray's Global Ocean Tide (GOT) netCDF4 model file
 
     Parameters
     ----------
-    input_file: str
+    input_file: str or pathlib.Path
         model file
     compressed: bool, default False
         Input file is gzip compressed
 
     Returns
     -------
     hc: np.ndarray
@@ -640,21 +639,23 @@
     lat: np.ndarray
         latitude of tidal model
     cons: str
         tidal constituent ID
     """
     # set default keyword arguments
     kwargs.setdefault('compressed', False)
+    # tilde-expand input file
+    input_file = pathlib.Path(input_file).expanduser()
     # read the netcdf format tide elevation file
     if kwargs['compressed']:
         # read gzipped netCDF4 file
-        f = gzip.open(os.path.expanduser(input_file),'rb')
+        f = gzip.open(input_file, 'rb')
         fileID = netCDF4.Dataset(uuid.uuid4().hex, 'r', memory=f.read())
     else:
-        fileID = netCDF4.Dataset(os.path.expanduser(input_file), 'r')
+        fileID = netCDF4.Dataset(input_file, 'r')
     # variable dimensions
     lon = fileID.variables['longitude'][:]
     lat = fileID.variables['latitude'][:]
     # get amplitude and phase components
     amp = fileID.variables['amplitude'][:]
     ph = fileID.variables['phase'][:]
     # extract constituent from attribute
@@ -667,40 +668,42 @@
         (ph.data == ph.fill_value) | \
         np.isnan(amp.data) | np.isnan(ph.data)
     hc = np.ma.array(amp*np.exp(-1j*ph*np.pi/180.0), mask=mask,
         fill_value=np.ma.default_fill_value(np.dtype(complex)))
     # return output variables
     return (hc, lon, lat, cons)
 
-# PURPOSE: output tidal constituent file in GOT format
+# PURPOSE: output tidal constituent file in GOT netCDF format
 def output_netcdf_file(
-        FILE: str,
+        FILE: str | pathlib.Path,
         hc: np.ndarray,
         lon: np.ndarray,
         lat: np.ndarray,
         constituent: str
     ):
     """
     Writes tidal constituent files in GOT netCDF format
 
     Parameters
     ----------
-    FILE: str
+    FILE: str or pathlib.Path
         output GOT model file name
     hc: np.ndarray
         Eulerian form of tidal constituent
     lon: np.ndarray
         longitude coordinates
     lat: np.ndarray
         latitude coordinates
     constituent: str
         tidal constituent ID
     """
+    # tilde-expand output file
+    FILE = pathlib.Path(FILE).expanduser()
     # opening NetCDF file for writing
-    fileID = netCDF4.Dataset(os.path.expanduser(FILE), 'w', format="NETCDF4")
+    fileID = netCDF4.Dataset(FILE, 'w', format="NETCDF4")
     # define the NetCDF dimensions
     fileID.createDimension('longitude', len(lon))
     fileID.createDimension('latitude', len(lat))
     # calculate amplitude and phase
     amp = np.abs(hc)
     ph = 180.0*np.arctan2(-np.imag(hc), np.real(hc))/np.pi
     ph.data[ph.data < 0] += 360.0
@@ -742,11 +745,11 @@
     fileID.Constituent = constituent.upper()
     # add attribute for date created
     fileID.date_created = datetime.datetime.now().isoformat()
     # add attributes for software information
     fileID.software_reference = pyTMD.version.project_name
     fileID.software_version = pyTMD.version.full_version
     # Output NetCDF structure information
-    logging.info(FILE)
+    logging.info(str(FILE))
     logging.info(list(fileID.variables.keys()))
     # Closing the NetCDF file
     fileID.close()
```

### Comparing `pyTMD-2.0.3/pyTMD/io/OTIS.py` & `pyTMD-2.0.4/pyTMD/io/OTIS.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 OTIS.py
-Written by Tyler Sutterley (03/2023)
+Written by Tyler Sutterley (04/2023)
 
 Reads files for a tidal model and makes initial calculations to run tide program
 Includes functions to extract tidal harmonic constants from OTIS tide models for
     given locations
 
 Reads OTIS format tidal solutions provided by Ohio State University and ESR
     http://volkov.oce.orst.edu/tides/region.html
@@ -55,14 +55,15 @@
          https://unidata.github.io/netcdf4-python/netCDF4/index.html
 
 PROGRAM DEPENDENCIES:
     convert_crs.py: converts lat/lon points to and from projected coordinates
     interpolate.py: interpolation routines for spatial data
 
 UPDATE HISTORY:
+    Updated 04/2023: using pathlib to define and expand tide model paths
     Updated 03/2023: add basic variable typing to function inputs
         new function name for converting coordinate reference systems
     Updated 12/2022: refactor tide read programs under io
         new functions to read and interpolate from constituents class
         refactored interpolation routines into new module
     Updated 11/2022: place some imports within try/except statements
         fix variable reads for ATLAS compact data formats
@@ -105,17 +106,17 @@
         combine both global and localized tidal solutions
         added multivariate spline interpolation option
     Updated 07/2018: added different interpolation methods
     Updated 09/2017: Adapted for Python
 """
 from __future__ import division, annotations
 
-import os
 import copy
 import struct
+import pathlib
 import warnings
 import numpy as np
 import scipy.interpolate
 import pyTMD.interpolate
 import pyTMD.io.constituents
 from pyTMD.convert_crs import convert_crs
 
@@ -128,16 +129,16 @@
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: extract harmonic constants from tide models at coordinates
 def extract_constants(
         ilon: np.ndarray,
         ilat: np.ndarray,
-        grid_file: str | None = None,
-        model_file: str | list | None = None,
+        grid_file: str | pathlib.Path | None = None,
+        model_file: str | pathlib.Path | list | None = None,
         EPSG: str | int | None = None,
         **kwargs
     ):
     """
     Reads files from tide models in OTIS and ATLAS-compact formats
 
     Makes initial calculations to run the tide program
@@ -146,17 +147,17 @@
 
     Parameters
     ----------
     ilon: np.ndarray
         longitude to interpolate
     ilat: np.ndarray
         latitude to interpolate
-    grid_file: str or NoneType, default None
+    grid_file: str, pathlib.Path or NoneType, default None
         grid file for model
-    model_file: str, list or NoneType, default None
+    model_file: str, pathlib.Path, list or NoneType, default None
         model file containing each constituent
     EPSG: str or NoneType, default None,
         projection of tide model data
     type: str, default 'z'
         Tidal variable to read
 
             - ``'z'``: heights
@@ -210,16 +211,18 @@
         if old in kwargs.keys():
             warnings.warn(f"""Deprecated keyword argument {old}.
                 Changed to '{new}'""", DeprecationWarning)
             # set renamed argument to not break workflows
             kwargs[new] = copy.copy(kwargs[old])
 
     # check that grid file is accessible
-    if not os.access(os.path.expanduser(grid_file), os.F_OK):
-        raise FileNotFoundError(os.path.expanduser(grid_file))
+    grid_file = pathlib.Path(grid_file).expanduser()
+    if not grid_file.exists():
+        raise FileNotFoundError(str(grid_file))
+
     # read the OTIS-format tide grid file
     if (kwargs['grid'] == 'ATLAS'):
         # if reading a global solution with localized solutions
         x0,y0,hz0,mz0,iob,dt,pmask,local = read_atlas_grid(grid_file)
         xi,yi,hz = combine_atlas_model(x0,y0,hz0,pmask,local,variable='depth')
         mz = create_atlas_mask(x0,y0,mz0,local,variable='depth')
     elif (kwargs['grid'] == 'ESR'):
@@ -451,27 +454,27 @@
     amplitude.data[amplitude.mask] = amplitude.fill_value
     phase.data[phase.mask] = phase.fill_value
     # return the interpolated values
     return (amplitude, phase, D, constituents)
 
 # PURPOSE: read harmonic constants from tide models
 def read_constants(
-        grid_file: str | None = None,
-        model_file: str | list | None = None,
+        grid_file: str | pathlib.Path | None = None,
+        model_file: str | pathlib.Path | list | None = None,
         EPSG: str | int | None = None,
         **kwargs
     ):
     """
     Reads files from tide models in OTIS and ATLAS-compact formats
 
     Parameters
     ----------
-    grid_file: str or NoneType, default None
+    grid_file: str, pathlib.Path or NoneType, default None
         grid file for model
-    model_file: str, list or NoneType, default None
+    model_file: str, pathlib.Path, list or NoneType, default None
         model file containing each constituent
     EPSG: str or NoneType, default None,
         projection of tide model data
     type: str, default 'z'
         Tidal variable to read
 
             - ``'z'``: heights
@@ -495,16 +498,18 @@
     """
     # set default keyword arguments
     kwargs.setdefault('type', 'z')
     kwargs.setdefault('grid', 'OTIS')
     kwargs.setdefault('apply_flexure', False)
 
     # check that grid file is accessible
-    if not os.access(os.path.expanduser(grid_file), os.F_OK):
-        raise FileNotFoundError(os.path.expanduser(grid_file))
+    grid_file = pathlib.Path(grid_file).expanduser()
+    if not grid_file.exists():
+        raise FileNotFoundError(str(grid_file))
+
     # read the OTIS-format tide grid file
     if (kwargs['grid'] == 'ATLAS'):
         # if reading a global solution with localized solutions
         x0,y0,hz0,mz0,iob,dt,pmask,local = read_atlas_grid(grid_file)
         xi,yi,hz = combine_atlas_model(x0,y0,hz0,pmask,local,variable='depth')
         mz = create_atlas_mask(x0,y0,mz0,local,variable='depth')
     elif (kwargs['grid'] == 'ESR'):
@@ -868,21 +873,21 @@
     temp = np.ma.zeros((ny, nx+2), dtype=input_matrix.dtype)
     temp[:,0] = input_matrix[:,-1]
     temp[:,1:-1] = input_matrix[:,:]
     temp[:,-1] = input_matrix[:,0]
     return temp
 
 # PURPOSE: read tide grid file
-def read_otis_grid(input_file: str):
+def read_otis_grid(input_file: str | pathlib.Path):
     """
     Read grid file to extract model coordinates, bathymetry, masks and indices
 
     Parameters
     ----------
-    input_file: str
+    input_file: str or pathlib.Path
         input grid file
 
     Returns
     -------
     x: np.ndarray
         x-coordinates of input grid
     y: np.ndarray
@@ -892,16 +897,17 @@
     mz: np.ndarray
         land/water mask
     iob: np.ndarray
         open boundary index
     dt: np.ndarray
         time step
     """
-    # open the file
-    fid = open(os.path.expanduser(input_file),'rb')
+    # open the input file
+    input_file = pathlib.Path(input_file).expanduser()
+    fid = input_file.open(mode='rb')
     fid.seek(4,0)
     # read data as big endian
     # get model dimensions and limits
     nx, = np.fromfile(fid, dtype=np.dtype('>i4'), count=1)
     ny, = np.fromfile(fid, dtype=np.dtype('>i4'), count=1)
     # extract x and y limits (these could be latitude and longitude)
     ylim = np.fromfile(fid, dtype=np.dtype('>f4'), count=2)
@@ -931,22 +937,22 @@
     mz = np.fromfile(fid, dtype=np.dtype('>i4'), count=nx*ny).reshape(ny, nx)
     # close the file
     fid.close()
     # return values
     return (x, y, hz, mz, iob, dt)
 
 # PURPOSE: read tide grid file with localized solutions
-def read_atlas_grid(input_file: str):
+def read_atlas_grid(input_file: str | pathlib.Path):
     """
     Read ATLAS grid file to extract model coordinates, bathymetry, masks and
     indices for both global and local solutions
 
     Parameters
     ----------
-    input_file: str
+    input_file: str or pathlib.Path
         input ATLAS grid file
 
     Returns
     -------
     x: np.ndarray
         x-coordinates of input ATLAS grid
     y: np.ndarray
@@ -962,18 +968,18 @@
     pmask: np.ndarray
         global mask
     local: dict
         dictionary of local tidal solutions for grid variables
 
             - ``'depth'``: model bathymetry
     """
-    # read the input file to get file information
-    fd = os.open(os.path.expanduser(input_file), os.O_RDONLY)
-    file_info = os.fstat(fd)
-    fid = os.fdopen(fd, 'rb')
+    # open the input file and get file information
+    input_file = pathlib.Path(input_file).expanduser()
+    file_info = input_file.stat()
+    fid = input_file.open(mode='rb')
     fid.seek(4,0)
     # read data as big endian
     # get model dimensions and limits
     nx, = np.fromfile(fid, dtype=np.dtype('>i4'), count=1)
     ny, = np.fromfile(fid, dtype=np.dtype('>i4'), count=1)
     # extract latitude and longitude limits
     lats = np.fromfile(fid, dtype=np.dtype('>f4'), count=2)
@@ -1032,22 +1038,22 @@
         local[name] = dict(lon=ln1, lat=lt1, depth=depth)
     # close the file
     fid.close()
     # return values
     return (x, y, hz, mz, iob, dt, pmask, local)
 
 # PURPOSE: read grid file
-def read_netcdf_grid(input_file: str):
+def read_netcdf_grid(input_file: str | pathlib.Path):
     """
     Read netCDF4 grid file to extract model coordinates, bathymetry,
     masks and flexure scaling factors
 
     Parameters
     ----------
-    input_file: str
+    input_file: str or pathlib.Path
         input grid file
 
     Returns
     -------
     x: np.ndarray
         x-coordinates of input grid
     y: np.ndarray
@@ -1055,16 +1061,18 @@
     hz: np.ndarray
         model bathymetry
     mz: np.ndarray
         land/water mask
     sf: np.ndarray
         scaling factor for applying ice flexure
     """
-    # read the netcdf format tide grid file
-    fileID = netCDF4.Dataset(os.path.expanduser(input_file),'r')
+    # tilde-expand input file
+    input_file = pathlib.Path(input_file).expanduser()
+    # read the netCDF format tide grid file
+    fileID = netCDF4.Dataset(input_file, 'r')
     # read coordinates and flip y orientation
     x = fileID.variables['x'][:].copy()
     y = fileID.variables['y'][::-1].copy()
     # read water column thickness and flip y orientation
     hz = fileID.variables['wct'][::-1,:].copy()
     # read mask and flip y orientation
     mz = fileID.variables['mask'][::-1,:].copy()
@@ -1076,23 +1084,23 @@
     # close the grid file
     fileID.close()
     # return values
     return (x, y, hz, mz, sf)
 
 # PURPOSE: read list of constituents from an elevation or transport file
 def read_constituents(
-        input_file: str,
+        input_file: str | pathlib.Path,
         grid: str = 'OTIS'
     ):
     """
     Read the list of constituents from an elevation or transport file
 
     Parameters
     ----------
-    input_file: str
+    input_file: str or pathlib.Path
         input tidal file
     grid: str, default 'OTIS'
         Tide model file type to read
 
             - ``'ATLAS'``: reading a global solution with localized solutions
             - ``'ESR'``: combined global or local netCDF4 solution
             - ``'OTIS'``: combined global or local solution
@@ -1100,56 +1108,60 @@
     Returns
     -------
     constituents: list
         list of tidal constituent IDs
     nc: int
         number of constituents
     """
+    # tilde-expand input file
+    input_file = pathlib.Path(input_file).expanduser()
     # check that model file is accessible
-    if not os.access(os.path.expanduser(input_file), os.F_OK):
-        raise FileNotFoundError(os.path.expanduser(input_file))
+    if not input_file.exists():
+        raise FileNotFoundError(str(input_file))
+    # get the constituents from the input file
     if (grid == 'ESR'):
         # open the netCDF4 file
-        fid = netCDF4.Dataset(os.path.expanduser(input_file),'r')
+        fid = netCDF4.Dataset(input_file, 'r')
         constituents = fid.variables['constituents'].constituent_order.split()
         nc = len(constituents)
         fid.close()
     else:
         # open the file
-        fid = open(os.path.expanduser(input_file),'rb')
+        fid = input_file.open(mode='rb')
         ll, = np.fromfile(fid, dtype=np.dtype('>i4'), count=1)
         nx,ny,nc = np.fromfile(fid, dtype=np.dtype('>i4'), count=3)
         fid.seek(16,1)
         constituents = [c.decode("utf8").rstrip() for c in fid.read(nc*4).split()]
         fid.close()
     return (constituents, nc)
 
 # PURPOSE: read elevation file to extract real and imaginary components for
 # constituent
 def read_otis_elevation(
-        input_file: str,
+        input_file: str | pathlib.Path,
         ic: int
     ):
     """
     Read elevation file to extract real and imaginary components for constituent
 
     Parameters
     ----------
-    input_file: str
+    input_file: str or pathlib.Path
         input elevation file
     ic: int
         index of consituent
 
     Returns
     -------
     h: np.ndarray
         tidal elevation
     """
-    # open the file
-    fid = open(os.path.expanduser(input_file),'rb')
+    # open the input file
+    input_file = pathlib.Path(input_file).expanduser()
+    fid = input_file.open(mode='rb')
     ll, = np.fromfile(fid, dtype=np.dtype('>i4'), count=1)
     nx,ny,nc = np.fromfile(fid, dtype=np.dtype('>i4'), count=3)
     # extract x and y limits
     ylim = np.fromfile(fid, dtype=np.dtype('>f4'), count=2)
     xlim = np.fromfile(fid, dtype=np.dtype('>f4'), count=2)
     # skip records to constituent
     nskip = ic*(nx*ny*8+8) + 8 + ll - 28
@@ -1169,25 +1181,25 @@
     fid.close()
     # return the elevation
     return h
 
 # PURPOSE: read elevation file with localized solutions to extract real and
 # imaginary components for constituent
 def read_atlas_elevation(
-        input_file: str,
+        input_file: str | pathlib.Path,
         ic: int,
         constituent: str
     ):
     """
     Read elevation file with localized solutions to extract real and imaginary
     components for constituent
 
     Parameters
     ----------
-    input_file: str
+    input_file: str or pathlib.Path
         input ATLAS elevation file
     ic: int
         index of consituent
     constituent: str
         tidal constituent ID
 
     Returns
@@ -1195,18 +1207,18 @@
     h: float
         global tidal elevation
     local: dict
         dictionary of local tidal solutions for elevation variables
 
             - ``'z'``: tidal elevation
     """
-    # read the input file to get file information
-    fd = os.open(os.path.expanduser(input_file), os.O_RDONLY)
-    file_info = os.fstat(fd)
-    fid = os.fdopen(fd, 'rb')
+    # open the input file and get file information
+    input_file = pathlib.Path(input_file).expanduser()
+    file_info = input_file.stat()
+    fid = input_file.open(mode='rb')
     ll, = np.fromfile(fid, dtype=np.dtype('>i4'), count=1)
     nx,ny,nc = np.fromfile(fid, dtype=np.dtype('>i4'), count=3)
     # extract x and y limits
     ylim = np.fromfile(fid, dtype=np.dtype('>f4'), count=2)
     xlim = np.fromfile(fid, dtype=np.dtype('>f4'), count=2)
     # skip records to constituent
     nskip = 8 + nc*4 + ic*(nx*ny*8 + 8)
@@ -1270,36 +1282,37 @@
     fid.close()
     # return the elevation
     return (h, local)
 
 # PURPOSE: read transport file to extract real and imaginary components for
 # constituent
 def read_otis_transport(
-        input_file: str,
+        input_file: str | pathlib.Path,
         ic: int
     ):
     """
     Read transport file to extract real and imaginary components for constituent
 
     Parameters
     ----------
-    input_file: str
+    input_file: str or pathlib.Path
         input transport file
     ic: int
         index of consituent
 
     Returns
     -------
     u: float
         zonal tidal transport
     v: float
         meridional zonal transport
     """
-    # open the file
-    fid = open(os.path.expanduser(input_file),'rb')
+    # open the input file
+    input_file = pathlib.Path(input_file).expanduser()
+    fid = input_file.open(mode='rb')
     ll, = np.fromfile(fid, dtype=np.dtype('>i4'), count=1)
     nx,ny,nc = np.fromfile(fid, dtype=np.dtype('>i4'), count=3)
     # extract x and y limits
     ylim = np.fromfile(fid, dtype=np.dtype('>f4'), count=2)
     xlim = np.fromfile(fid, dtype=np.dtype('>f4'), count=2)
     # skip records to constituent
     nskip = ic*(nx*ny*16+8) + 8 + ll - 28
@@ -1325,25 +1338,25 @@
     fid.close()
     # return the transport components
     return (u, v)
 
 # PURPOSE: read transport file with localized solutions to extract real and
 # imaginary components for constituent
 def read_atlas_transport(
-        input_file: str,
+        input_file: str | pathlib.Path,
         ic: int,
         constituent: str
     ):
     """
     Read transport file with localized solutions to extract real and imaginary
     components for constituent
 
     Parameters
     ----------
-    input_file: str
+    input_file: str or pathlib.Path
         input ATLAS transport file
     ic: int
         index of consituent
     constituent: str
         tidal constituent ID
 
     Returns
@@ -1354,18 +1367,18 @@
         global meridional zonal transport
     local: dict
         dictionary of local tidal solutions for transport variables
 
             - ``'u'``: zonal tidal transport
             - ``'v'``: meridional zonal transport
     """
-    # read the input file to get file information
-    fd = os.open(os.path.expanduser(input_file), os.O_RDONLY)
-    file_info = os.fstat(fd)
-    fid = os.fdopen(fd, 'rb')
+    # open the input file and get file information
+    input_file = pathlib.Path(input_file).expanduser()
+    file_info = input_file.stat()
+    fid = input_file.open(mode='rb')
     ll, = np.fromfile(fid, dtype=np.dtype('>i4'), count=1)
     nx,ny,nc = np.fromfile(fid, dtype=np.dtype('>i4'), count=3)
     # extract x and y limits
     ylim = np.fromfile(fid, dtype=np.dtype('>f4'), count=2)
     xlim = np.fromfile(fid, dtype=np.dtype('>f4'), count=2)
     # skip records to constituent
     nskip = 8 + nc*4 + ic*(nx*ny*16 + 8)
@@ -1638,24 +1651,24 @@
         z30.data[jj,ii] = val[variable][validy,validx]
     # return 2 arc-minute solution and coordinates
     return (x30, y30, z30)
 
 # PURPOSE: read netCDF4 file to extract real and imaginary components for
 # constituent
 def read_netcdf_file(
-        input_file: str,
+        input_file: str | pathlib.Path,
         ic: int,
         variable: str | None = None
     ):
     """
     Read netCDF4 file to extract real and imaginary components for constituent
 
     Parameters
     ----------
-    input_file: str
+    input_file: str or pathlib.Path
         input transport file
     ic: int
         index of consituent
     variable: str or NoneType, default None
         Tidal variable to read
 
             - ``'z'``: heights
@@ -1665,16 +1678,18 @@
             - ``'V'``: vertical depth-averaged transport
 
     Returns
     -------
     hc: complex
         complex form of tidal constituent oscillation
     """
+    # tilde-expand input file
+    input_file = pathlib.Path(input_file).expanduser()
     # read the netcdf format tide grid file
-    fileID = netCDF4.Dataset(os.path.expanduser(input_file), 'r')
+    fileID = netCDF4.Dataset(input_file, 'r')
     # variable dimensions
     nx = fileID.dimensions['x'].size
     ny = fileID.dimensions['y'].size
     # real and imaginary components of tidal constituent
     hc = np.ma.zeros((ny, nx), dtype=np.complex64)
     hc.mask = np.zeros((ny, nx), dtype=bool)
     # extract constituent and flip y orientation
@@ -1690,44 +1705,46 @@
     # close the file
     fileID.close()
     # return output variables
     return hc
 
 # PURPOSE: output grid file in OTIS format
 def output_otis_grid(
-        FILE: str,
+        FILE: str | pathlib.Path,
         xlim: np.ndarray | list,
         ylim: np.ndarray | list,
         hz: np.ndarray,
         mz: np.ndarray,
         iob: np.ndarray,
         dt: float
     ):
     """
     Writes OTIS-format grid files
 
     Parameters
     ----------
-    FILE: str
+    FILE: str or pathlib.Path
         output OTIS grid file name
     xlim: np.ndarray
         x-coordinate grid-cell edges of output grid
     ylim: np.ndarray
         y-coordinate grid-cell edges of output grid
     hz: np.ndarray
         bathymetry
     mz: np.ndarray
         land/water mask
     iob: np.ndarray
         open boundary index
     dt: float
         time step
     """
-    # open this way for files
-    fid = open(os.path.expanduser(FILE), 'wb')
+    # tilde-expand output file
+    FILE = pathlib.Path(FILE).expanduser()
+    # open output file
+    fid = FILE.open(mode='wb')
     nob = len(iob)
     ny, nx = np.shape(hz)
     reclen = 32
     fid.write(struct.pack('>i',reclen))
     fid.write(struct.pack('>i',nx))
     fid.write(struct.pack('>i',ny))
     ylim.tofile(fid,format='>f4')
@@ -1756,37 +1773,40 @@
         mz[m,:].tofile(fid,format='>i4')
     fid.write(struct.pack('>i',reclen))
     # close the output OTIS file
     fid.close()
 
 # PURPOSE: output elevation file in OTIS format
 def output_otis_elevation(
-        FILE: str,
+        FILE: str | pathlib.Path,
         h: np.ndarray,
         xlim: np.ndarray | list,
         ylim: np.ndarray | list,
         constituents: list
     ):
     """
     Writes OTIS-format elevation files
 
     Parameters
     ----------
-    FILE: str
+    FILE: str or pathlib.Path
         output OTIS elevation file name
     h: np.ndarray
         Eulerian form of tidal height oscillation
     xlim: np.ndarray
         x-coordinate grid-cell edges of output grid
     ylim: np.ndarray
         y-coordinate grid-cell edges of output grid
     constituents: list
         tidal constituent IDs
     """
-    fid = open(os.path.expanduser(FILE), 'wb')
+    # tilde-expand output file
+    FILE = pathlib.Path(FILE).expanduser()
+    # open output file
+    fid = FILE.open(mode='wb')
     ny, nx, nc = np.shape(h)
     # length of header: allow for 4 character >i c_id strings
     header_length = 4*(7 + nc)
     fid.write(struct.pack('>i',header_length))
     fid.write(struct.pack('>i',nx))
     fid.write(struct.pack('>i',ny))
     fid.write(struct.pack('>i',nc))
@@ -1806,40 +1826,43 @@
             temp.tofile(fid,format='>f4')
         fid.write(struct.pack('>i',constituent_header))
     # close the output OTIS file
     fid.close()
 
 # PURPOSE: output transport file in OTIS format
 def output_otis_transport(
-        FILE: str,
+        FILE: str | pathlib.Path,
         u: np.ndarray,
         v: np.ndarray,
         xlim: np.ndarray | list,
         ylim: np.ndarray | list,
         constituents: list
     ):
     """
     Writes OTIS-format transport files
 
     Parameters
     ----------
-    FILE: str
+    FILE: str or pathlib.Path
         output OTIS transport file name
     u: complex
         Eulerian form of tidal zonal transport oscillation
     v: complex
         Eulerian form of tidal meridional transport oscillation
     xlim: float
         x-coordinate grid-cell edges of output grid
     ylim: float
         y-coordinate grid-cell edges of output grid
     constituents: list
         tidal constituent IDs
     """
-    fid = open(os.path.expanduser(FILE), 'wb')
+    # tilde-expand output file
+    FILE = pathlib.Path(FILE).expanduser()
+    # open output file
+    fid = FILE.open(mode='wb')
     ny, nx, nc = np.shape(u)
     # length of header: allow for 4 character >i c_id strings
     header_length = 4*(7 + nc)
     fid.write(struct.pack('>i',header_length))
     fid.write(struct.pack('>i',nx))
     fid.write(struct.pack('>i',ny))
     fid.write(struct.pack('>i',nc))
```

### Comparing `pyTMD-2.0.3/pyTMD/io/constituents.py` & `pyTMD-2.0.4/pyTMD/io/constituents.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.3/pyTMD/io/ocean_pole_tide.py` & `pyTMD-2.0.4/pyTMD/io/ocean_pole_tide.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 ocean_pole_tide.py
-Written by Tyler Sutterley (03/2023)
+Written by Tyler Sutterley (05/2023)
 
 Reads ocean pole load tide coefficients provided by IERS
 http://maia.usno.navy.mil/conventions/2010/2010_official/chapter7/tn36_c7.pdf
 http://maia.usno.navy.mil/conventions/2010/2010_update/chapter7/icc7.pdf
 
 IERS 0.5x0.5 map of ocean pole tide coefficients:
 ftp://maia.usno.navy.mil/conventions/2010/2010_update/chapter7/additional_info/
@@ -20,41 +20,47 @@
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
 
 REFERENCES:
-    S Desai, "Observing the pole tide with satellite altimetry", Journal of
+    S. Desai, "Observing the pole tide with satellite altimetry", Journal of
         Geophysical Research: Oceans, 107(C11), 2002. doi: 10.1029/2001JC001224
-    S Desai, J Wahr and B Beckley "Revisiting the pole tide for and from
+    S. Desai, J. Wahr and B. Beckley "Revisiting the pole tide for and from
         satellite altimetry", Journal of Geodesy, 89(12), p1233-1243, 2015.
         doi: 10.1007/s00190-015-0848-7
 
 UPDATE HISTORY:
+    Updated 05/2023: add default for ocean pole tide file
+    Updated 04/2023: using pathlib to define and expand paths
     Updated 03/2023: add basic variable typing to function inputs
     Updated 12/2022: refactor ocean pole tide read programs under io
     Updated 04/2022: updated docstrings to numpy documentation format
         use longcomplex data format to be windows compliant
     Updated 07/2021: added check that ocean pole tide file is accessible
     Updated 03/2021: replaced numpy bool/int to prevent deprecation warnings
     Updated 08/2020: output north load and east load deformation components
     Updated 07/2020: added function docstrings
     Updated 12/2018: Compatibility updates for Python3
     Written 09/2017
 """
 from __future__ import annotations
 
-import os
 import re
 import gzip
+import pathlib
 import numpy as np
+from pyTMD.utilities import get_data_path
+
+# ocean pole tide file from Desai (2002) and IERS conventions
+_ocean_pole_tide_file = get_data_path(['data','opoleloadcoefcmcor.txt.gz'])
 
 # PURPOSE: read real and imaginary ocean pole tide coefficients
-def ocean_pole_tide(input_file: str):
+def ocean_pole_tide(input_file: str | pathlib.Path = _ocean_pole_tide_file):
     """
     Read real and imaginary ocean pole tide coefficients
 
     Parameters
     ----------
     input_file: str
         IERS map of ocean pole tide coefficients
@@ -70,27 +76,29 @@
     glon: np.ndarray
         ocean grid longitude
     glat: np.ndarray
         ocean grid latitude
 
     References
     ----------
-    .. [1] S Desai, "Observing the pole tide with satellite altimetry", *Journal of
+    .. [1] S. Desai, "Observing the pole tide with satellite altimetry", *Journal of
         Geophysical Research: Oceans*, 107(C11), (2002).
         `doi: 10.1029/2001JC001224 <https://doi.org/10.1029/2001JC001224>`_
-    .. [2] S Desai, J Wahr and B Beckley "Revisiting the pole tide for and from
+    .. [2] S. Desai, J. Wahr and B. Beckley "Revisiting the pole tide for and from
         satellite altimetry", *Journal of Geodesy*, 89(12), p1233-1243, (2015).
         `doi: 10.1007/s00190-015-0848-7 <https://doi.org/10.1007/s00190-015-0848-7>`_
     """
+    # convert input file to tilde-expanded pathlib object
+    input_file = pathlib.Path(input_file).expanduser()
     # check that ocean pole tide file is accessible
-    if not os.access(os.path.expanduser(input_file), os.F_OK):
-        raise FileNotFoundError(os.path.expanduser(input_file))
+    if not input_file.exists():
+        raise FileNotFoundError(str(input_file))
 
     # read GZIP ocean pole tide file
-    with gzip.open(os.path.expanduser(input_file),'rb') as f:
+    with gzip.open(input_file, 'rb') as f:
         file_contents = f.read().splitlines()
 
     # counts the number of lines in the header
     count = 0
     # Reading over header text
     HEADER = True
     while HEADER:
```

### Comparing `pyTMD-2.0.3/pyTMD/load_constituent.py` & `pyTMD-2.0.4/pyTMD/load_constituent.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,17 +52,17 @@
     alpha: float
         load love number of tidal constituent
     species: float
         spherical harmonic dependence of quadrupole potential
 
     References
     ----------
-    .. [1] Egbert and Erofeeva, "Efficient Inverse Modeling of Barotropic
-        Ocean Tides," *Journal of Atmospheric and Oceanic Technology*,
-        19(2), 183--204, (2002).
+    .. [1] G. D. Egbert and S. Y. Erofeeva, "Efficient Inverse Modeling of
+        Barotropic Ocean Tides," *Journal of Atmospheric and Oceanic
+        Technology*, 19(2), 183--204, (2002).
         `doi: 10.1175/1520-0426(2002)019<0183:EIMOBO>2.0.CO;2`__
 
     .. __: https://doi.org/10.1175/1520-0426(2002)019<0183:EIMOBO>2.0.CO;2
     """
     # constituents array that are included in tidal program
     cindex = ['m2','s2','k1','o1','n2','p1','k2','q1','2n2','mu2','nu2','l2',
         't2','j1','m1','oo1','rho1','mf','mm','ssa','m4','ms4','mn4','m6','m8',
```

### Comparing `pyTMD-2.0.3/pyTMD/load_nodal_corrections.py` & `pyTMD-2.0.4/pyTMD/arguments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python
 u"""
-load_nodal_corrections.py
+arguments.py
 Written by Tyler Sutterley (04/2023)
 Calculates the nodal corrections for tidal constituents
 Modification of ARGUMENTS fortran subroutine by Richard Ray 03/1999
 
 CALLING SEQUENCE:
-    pu,pf,G = load_nodal_corrections(MJD, constituents)
+    pu,pf,G = arguments(MJD, constituents)
 
 INPUTS:
     MJD: Modified Julian Day of input date
     constituents: tidal constituent IDs
 
 OUTPUTS:
     pu,pf: nodal corrections for the constituents
@@ -35,14 +35,15 @@
     M. G. G. Foreman and R. F. Henry, "The harmonic analysis of tidal model
         time series", Advances in Water Resources, 12, (1989).
     G. D. Egbert and S. Erofeeva, "Efficient Inverse Modeling of Barotropic
         Ocean Tides", Journal of Atmospheric and Oceanic Technology, (2002).
 
 UPDATE HISTORY:
     Updated 04/2023: using renamed astro mean_longitudes function
+        function renamed from original load_nodal_corrections
     Updated 03/2023: add basic variable typing to function inputs
     Updated 11/2022: use f-strings for formatting verbose or ascii output
     Updated 05/2022: added ESR netCDF4 formats to list of model types
         changed keyword arguments to camel case
     Updated 04/2022: updated docstrings to numpy documentation format
     Updated 12/2020: fix k1 for FES models
     Updated 08/2020: change time variable names to not overwrite functions
@@ -53,26 +54,24 @@
     Updated 07/2018: added option to use GSFC GOT nodal corrections
     Updated 09/2017: Rewritten in Python
     Rewritten in Matlab by Lana Erofeeva 01/2003
     Written by Richard Ray 03/1999
 """
 from __future__ import annotations
 
-import copy
-import warnings
 import numpy as np
 import pyTMD.astro
 
-def load_nodal_corrections(
+def arguments(
         MJD: np.ndarray,
         constituents: list | np.ndarray,
         **kwargs
     ):
     """
-    Calculates the nodal corrections for tidal constituents
+    Calculates the nodal corrections for tidal constituents [1]_ [2]_ [3]_
 
     Parameters
     ----------
     MJD: np.ndarray
         modified julian day of input date
     constituents: list
         tidal constituent IDs
@@ -88,63 +87,58 @@
     pf: np.ndarray
         nodal correction for the constituent phase
     G: np.ndarray
         phase correction in degrees
 
     References
     ----------
-    .. [1] Doodson and Warburg, "Admiralty Manual of Tides", HMSO, (1941).
-    .. [2] Schureman, "Manual of Harmonic Analysis and Prediction of Tides,"
+    .. [1] A. T. Doodson and H. D. Warburg, "Admiralty Manual of Tides",
+        HMSO, London, (1941).
+    .. [2] P. Schureman, "Manual of Harmonic Analysis and Prediction of Tides,"
         *US Coast and Geodetic Survey*, Special Publication, 98, (1958).
-    .. [3] Foreman and Henry, "The harmonic analysis of tidal model time
-        series," *Advances in Water Resources*, 12(3), 109--120, (1989).
-        `doi: 10.1016/0309-1708(89)90017-1
+    .. [3] M. G. G. Foreman and R. F. Henry, "The harmonic analysis of tidal
+        model time series," *Advances in Water Resources*, 12(3), 109--120,
+        (1989). `doi: 10.1016/0309-1708(89)90017-1
         <https://doi.org/10.1016/0309-1708(89)90017-1>`_
-    .. [4] Egbert and Erofeeva, "Efficient Inverse Modeling of Barotropic
-        Ocean Tides," *Journal of Atmospheric and Oceanic Technology*,
-        19(2), 183--204, (2002).
+    .. [4] G. D. Egbert and S. Y. Erofeeva, "Efficient Inverse Modeling of
+        Barotropic Ocean Tides," *Journal of Atmospheric and Oceanic
+        Technology*, 19(2), 183--204, (2002).
         `doi: 10.1175/1520-0426(2002)019<0183:EIMOBO>2.0.CO;2`__
 
     .. __: https://doi.org/10.1175/1520-0426(2002)019<0183:EIMOBO>2.0.CO;2
     """
     # set default keyword arguments
     kwargs.setdefault('deltat', 0.0)
     kwargs.setdefault('corrections', 'OTIS')
-    # raise warnings for deprecated keyword arguments
-    deprecated_keywords = dict(DELTAT='deltat',CORRECTIONS='corrections')
-    for old,new in deprecated_keywords.items():
-        if old in kwargs.keys():
-            warnings.warn(f"""Deprecated keyword argument {old}.
-                Changed to '{new}'""", DeprecationWarning)
-            # set renamed argument to not break workflows
-            kwargs[new] = copy.copy(kwargs[old])
 
     # constituents array (not all are included in tidal program)
     cindex = ['sa','ssa','mm','msf','mf','mt','alpha1','2q1','sigma1','q1',
         'rho1','o1','tau1','m1','chi1','pi1','p1','s1','k1','psi1','phi1',
         'theta1','j1','oo1','2n2','mu2','n2','nu2','m2a','m2','m2b','lambda2',
         'l2','t2','s2','r2','k2','eta2','mns2','2sm2','m3','mk3','s3','mn4',
         'm4','ms4','mk4','s4','s5','m6','s6','s7','s8','m8','mks2','msqm','mtm',
         'n4','eps2','z0']
 
-    # degrees to radians
-    dtr = np.pi/180.0
-
     # set function for astronomical longitudes
     ASTRO5 = True if kwargs['corrections'] in ('GOT','FES') else False
     # convert from Modified Julian Dates into Ephemeris Time
-    s,h,p,omega,pp = pyTMD.astro.mean_longitudes(MJD + kwargs['deltat'],
+    s, h, p, omega, pp = pyTMD.astro.mean_longitudes(MJD + kwargs['deltat'],
         ASTRO5=ASTRO5)
-    hour = (MJD % 1)*24.0
+    # number of temporal values
+    nt = len(np.atleast_1d(MJD))
+    # initial time conversions
+    hour = 24.0*np.mod(MJD, 1)
     t1 = 15.0*hour
     t2 = 30.0*hour
-    nt = len(np.atleast_1d(MJD))
+
+    # degrees to radians
+    dtr = np.pi/180.0
 
     # Determine equilibrium arguments
-    arg = np.zeros((nt,60))
+    arg = np.zeros((nt, 60))
     arg[:,0] = h - pp # Sa
     arg[:,1] = 2.0*h # Ssa
     arg[:,2] = s - p # Mm
     arg[:,3] = 2.0*s - 2.0*h # MSf
     arg[:,4] = 2.0*s # Mf
     arg[:,5] = 3.0*s - p # Mt
     arg[:,6] = t1 - 5.0*s + 3.0*h + p - 90.0 # alpha1
@@ -211,16 +205,16 @@
     sinn = np.sin(omega*dtr)
     cosn = np.cos(omega*dtr)
     sin2n = np.sin(2.0*omega*dtr)
     cos2n = np.cos(2.0*omega*dtr)
     sin3n = np.sin(3.0*omega*dtr)
 
     # set nodal corrections
-    f = np.zeros((nt,60))
-    u = np.zeros((nt,60))
+    f = np.zeros((nt, 60))
+    u = np.zeros((nt, 60))
     # determine nodal corrections f and u for each model type
     if kwargs['corrections'] in ('OTIS','ATLAS','ESR','netcdf'):
         f[:,0] = 1.0 # Sa
         f[:,1] = 1.0 # Ssa
         f[:,2] = 1.0 - 0.130*cosn # Mm
         f[:,3] = 1.0 # MSf
         f[:,4] = 1.043 + 0.414*cosn # Mf
@@ -545,8 +539,8 @@
         # map between given constituents and supported in tidal program
         j, = [j for j,val in enumerate(cindex) if (val == c)]
         pu[:,i] = u[:,j]*dtr
         pf[:,i] = f[:,j]
         G[:,i] = arg[:,j]
 
     # return values as tuple
-    return (pu,pf,G)
+    return (pu, pf, G)
```

### Comparing `pyTMD-2.0.3/pyTMD/predict.py` & `pyTMD-2.0.4/pyTMD/predict.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 #!/usr/bin/env python
 u"""
-predict.py (04/2023)
-Predict tide values using harmonic constants
+predict.py
+Written by Tyler Sutterley (04/2023)
+Prediction routines for ocean, load, equilibrium and solid earth tides
 
 REFERENCES:
     G. D. Egbert and S. Erofeeva, "Efficient Inverse Modeling of Barotropic
         Ocean Tides", Journal of Atmospheric and Oceanic Technology, (2002).
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
 
 PROGRAM DEPENDENCIES:
+    arguments.py: loads nodal corrections for tidal constituents
     astro.py: computes the basic astronomical mean longitudes
     constants.py: calculate reference parameters for common ellipsoids
     load_constituent.py: loads parameters for a given tidal constituent
-    load_nodal_corrections.py: loads nodal corrections for tidal constituents
     spatial.py: utilities for working with geospatial data
 
 UPDATE HISTORY:
     Updated 04/2023: using renamed astro mean_longitudes function
+        using renamed arguments function for nodal corrections
         adding prediction routine for solid earth tides
+        output solid earth tide corrections as combined XYZ components
     Updated 03/2023: add basic variable typing to function inputs
     Updated 12/2022: merged prediction functions into a single module
     Updated 05/2022: added ESR netCDF4 formats to list of model types
     Updated 04/2022: updated docstrings to numpy documentation format
     Updated 02/2021: replaced numpy bool to prevent deprecation warning
     Updated 09/2020: append output mask over each constituent
     Updated 08/2020: change time variable names to not overwrite functions
@@ -36,17 +39,17 @@
     Updated 07/2018: added option to use GSFC GOT nodal corrections
     Updated 09/2017: Rewritten in Python
 """
 from __future__ import annotations
 
 import numpy as np
 import pyTMD.astro
+from pyTMD.arguments import arguments
 from pyTMD.constants import constants
 from pyTMD.load_constituent import load_constituent
-from pyTMD.load_nodal_corrections import load_nodal_corrections
 
 # PURPOSE: Predict tides at single times
 def map(t: float | np.ndarray,
         hc: np.ndarray,
         constituents: list | np.ndarray,
         deltat: float | np.ndarray = 0.0,
         corrections: str = 'OTIS'
@@ -70,26 +73,26 @@
     Returns
     -------
     ht: np.ndarray
         tide values reconstructed using the nodal corrections
 
     References
     ----------
-    .. [1] Egbert and Erofeeva, "Efficient Inverse Modeling of Barotropic
-        Ocean Tides," *Journal of Atmospheric and Oceanic Technology*,
-        19(2), 183--204, (2002).
+    .. [1] G. D. Egbert and S. Y. Erofeeva, "Efficient Inverse Modeling of
+        Barotropic Ocean Tides," *Journal of Atmospheric and Oceanic
+        Technology*, 19(2), 183--204, (2002).
         `doi: 10.1175/1520-0426(2002)019<0183:EIMOBO>2.0.CO;2`__
 
     .. __: https://doi.org/10.1175/1520-0426(2002)019<0183:EIMOBO>2.0.CO;2
     """
     # number of points and number of constituents
     npts,nc = np.shape(hc)
     # load the nodal corrections
     # convert time to Modified Julian Days (MJD)
-    pu,pf,G = load_nodal_corrections(t + 48622.0, constituents,
+    pu,pf,G = arguments(t + 48622.0, constituents,
         deltat=deltat, corrections=corrections)
     # allocate for output tidal elevation
     ht = np.ma.zeros((npts))
     ht.mask = np.zeros((npts),dtype=bool)
     # for each constituent
     for k,c in enumerate(constituents):
         if corrections in ('OTIS','ATLAS','ESR','netcdf'):
@@ -133,25 +136,25 @@
     Returns
     -------
     ht: np.ndarray
         tidal time series reconstructed using the nodal corrections
 
     References
     ----------
-    .. [1] Egbert and Erofeeva, "Efficient Inverse Modeling of Barotropic
-        Ocean Tides," *Journal of Atmospheric and Oceanic Technology*,
-        19(2), 183--204, (2002).
+    .. [1] G. D. Egbert and S. Y. Erofeeva, "Efficient Inverse Modeling of
+        Barotropic Ocean Tides," *Journal of Atmospheric and Oceanic
+        Technology*, 19(2), 183--204, (2002).
         `doi: 10.1175/1520-0426(2002)019<0183:EIMOBO>2.0.CO;2`__
 
     .. __: https://doi.org/10.1175/1520-0426(2002)019<0183:EIMOBO>2.0.CO;2
     """
     nt = len(t)
     # load the nodal corrections
     # convert time to Modified Julian Days (MJD)
-    pu,pf,G = load_nodal_corrections(t + 48622.0, constituents,
+    pu,pf,G = arguments(t + 48622.0, constituents,
         deltat=deltat, corrections=corrections)
     # allocate for output time series
     ht = np.ma.zeros((nt))
     ht.mask = np.zeros((nt),dtype=bool)
     # for each constituent
     for k,c in enumerate(constituents):
         if corrections in ('OTIS','ATLAS','ESR','netcdf'):
@@ -195,25 +198,25 @@
     Returns
     -------
     ht: np.ndarray
         tidal time series reconstructed using the nodal corrections
 
     References
     ----------
-    .. [1] Egbert and Erofeeva, "Efficient Inverse Modeling of Barotropic
-        Ocean Tides," *Journal of Atmospheric and Oceanic Technology*,
-        19(2), 183--204, (2002).
+    .. [1] G. D. Egbert and S. Y. Erofeeva, "Efficient Inverse Modeling of
+        Barotropic Ocean Tides," *Journal of Atmospheric and Oceanic
+        Technology*, 19(2), 183--204, (2002).
         `doi: 10.1175/1520-0426(2002)019<0183:EIMOBO>2.0.CO;2`__
 
     .. __: https://doi.org/10.1175/1520-0426(2002)019<0183:EIMOBO>2.0.CO;2
     """
     nt = len(t)
     # load the nodal corrections
     # convert time to Modified Julian Days (MJD)
-    pu,pf,G = load_nodal_corrections(t + 48622.0, constituents,
+    pu,pf,G = arguments(t + 48622.0, constituents,
         deltat=deltat, corrections=corrections)
     # allocate for output time series
     ht = np.ma.zeros((nt))
     ht.mask = np.zeros((nt),dtype=bool)
     # for each constituent
     for k,c in enumerate(constituents):
         if corrections in ('OTIS','ATLAS','ESR','netcdf'):
@@ -235,15 +238,15 @@
         t: float | np.ndarray,
         zmajor: np.ndarray,
         constituents: list | np.ndarray,
         **kwargs
     ):
     """
     Calculate the tidal corrections for minor constituents inferred using
-    major constituents
+    major constituents [1]_ [2]_ [3]_ [4]_
 
     Parameters
     ----------
     t: float or np.ndarray
         days relative to 1992-01-01T00:00:00
     zmajor: np.ndarray
         Complex HC for given constituents/points
@@ -257,21 +260,28 @@
     Returns
     -------
     dh: np.ndarray
         Height from minor constituents
 
     References
     ----------
-    .. [1] A. T. Doodson and H. Warburg, "Admiralty Manual of Tides", HMSO, (1941).
+    .. [1] A. T. Doodson and H. D. Warburg, "Admiralty Manual of Tides",
+        HMSO, London, (1941).
     .. [2] P. Schureman, "Manual of Harmonic Analysis and Prediction of Tides,"
         *US Coast and Geodetic Survey*, Special Publication, 98, (1958).
-    .. [3] Foreman and Henry, "The harmonic analysis of tidal model time
-        series," *Advances in Water Resources*, 12(3), 109--120, (1989).
-        `doi: 10.1016/0309-1708(89)90017-1
+    .. [3] M. G. G. Foreman and R. F. Henry, "The harmonic analysis of tidal
+        model time series," *Advances in Water Resources*, 12(3), 109--120,
+        (1989). `doi: 10.1016/0309-1708(89)90017-1
         <https://doi.org/10.1016/0309-1708(89)90017-1>`_
+    .. [4] G. D. Egbert and S. Y. Erofeeva, "Efficient Inverse Modeling of
+        Barotropic Ocean Tides," *Journal of Atmospheric and Oceanic
+        Technology*, 19(2), 183--204, (2002).
+        `doi: 10.1175/1520-0426(2002)019<0183:EIMOBO>2.0.CO;2`__
+
+    .. __: https://doi.org/10.1175/1520-0426(2002)019<0183:EIMOBO>2.0.CO;2
     """
     # set default keyword arguments
     kwargs.setdefault('deltat', 0.0)
     kwargs.setdefault('corrections', 'OTIS')
 
     # degrees to radians
     dtr = np.pi/180.0
@@ -549,15 +559,16 @@
 # PURPOSE: estimate solid Earth tides due to gravitational attraction
 def solid_earth_tide(
         t: np.ndarray,
         XYZ: np.ndarray,
         SXYZ: np.ndarray,
         LXYZ: np.ndarray,
         a_axis: float = _iers.a_axis,
-        tide_system: str = 'tide_free'
+        tide_system: str = 'tide_free',
+        **kwargs
     ):
     """
     Compute the solid Earth tides due to the gravitational attraction
     of the moon and sun [1]_ [2]_ [3]_ [4]_
 
     Parameters
     ----------
@@ -576,15 +587,15 @@
 
             - ``'tide_free'``: no permanent direct and indirect tidal potentials
             - ``'mean_tide'``: permanent tidal potentials (direct and indirect)
 
     Returns
     -------
     dxt: np.ndarray
-        Solid Earth tide in meters
+        Solid Earth tide in meters in Cartesian coordinates
 
     References
     ----------
     .. [1] P. M. Mathews, B. A. Buffett, T. A. Herring and I. I Shapiro,
         "Forced nutations of the Earth: Influence of inner core dynamics:
         1. Theory", *Journal of Geophysical Research: Solid Earth*,
         96(B5), 8219--8242, (1991). `doi: 10.1029/90JB01955
@@ -600,94 +611,106 @@
         <https://doi.org/10.1029/92GL00259>`_
     .. [4] J. M. Wahr, "Body tides on an elliptical, rotating, elastic
         and oceanless Earth", *Geophysical Journal of the Royal
         Astronomical Society*, 64(3), 677--703, (1981).
         `doi: 10.1111/j.1365-246X.1981.tb02690.x
         <https://doi.org/10.1111/j.1365-246X.1981.tb02690.x>`_
     """
+    # set default keyword arguments
+    # nominal Love and Shida numbers
+    kwargs.setdefault('h2', 0.6078)
+    kwargs.setdefault('l2', 0.0847)
+    kwargs.setdefault('h3', 0.292)
+    kwargs.setdefault('l3', 0.015)
+    # mass ratios between earth and sun/moon
+    kwargs.setdefault('mass_ratio_solar', 332946.0482)
+    kwargs.setdefault('mass_ratio_lunar', 0.0123000371)
     # validate output tide system
     assert tide_system in ('tide_free', 'mean_tide')
     # number of input coordinates
     nt = len(np.atleast_1d(t))
-    # nominal Love and Shida numbers
-    h20 = 0.6078
-    l20 = 0.0847
-    h3 = 0.292
-    l3 = 0.015
-    # mass ratios between earth and sun/moon
-    mass_ratio_solar = 332946.0482
-    mass_ratio_lunar = 0.0123000371
     # convert time to Modified Julian Days (MJD)
     MJD = t + 48622.0
     # scalar product of input coordinates with sun/moon vectors
     radius = np.sqrt(XYZ[:,0]**2 + XYZ[:,1]**2 + XYZ[:,2]**2)
     solar_radius = np.sqrt(SXYZ[:,0]**2 + SXYZ[:,1]**2 + SXYZ[:,2]**2)
     lunar_radius = np.sqrt(LXYZ[:,0]**2 + LXYZ[:,1]**2 + LXYZ[:,2]**2)
     solar_scalar = (XYZ[:,0]*SXYZ[:,0] + XYZ[:,1]*SXYZ[:,1] +
         XYZ[:,2]*SXYZ[:,2])/(radius*solar_radius)
     lunar_scalar = (XYZ[:,0]*LXYZ[:,0] + XYZ[:,1]*LXYZ[:,1] +
         XYZ[:,2]*LXYZ[:,2])/(radius*lunar_radius)
     # compute new h2 and l2 (Mathews et al., 1997)
     cosphi = np.sqrt(XYZ[:,0]**2 + XYZ[:,1]**2)/radius
-    h2 = h20 - 0.0006*(1.0 - 3.0/2.0*cosphi**2)
-    l2 = l20 + 0.0002*(1.0 - 3.0/2.0*cosphi**2)
+    h2 = kwargs['h2'] - 0.0006*(1.0 - 3.0/2.0*cosphi**2)
+    l2 = kwargs['l2'] + 0.0002*(1.0 - 3.0/2.0*cosphi**2)
     # compute P2 terms
     P2_solar = 3.0*(h2/2.0 - l2)*solar_scalar**2 - h2/2.0
     P2_lunar = 3.0*(h2/2.0 - l2)*lunar_scalar**2 - h2/2.0
     # compute P3 terms
-    P3_solar = 5.0/2.0*(h3 - 3.0*l3)*solar_scalar**3 + \
-        3.0/2.0*(l3 - h3)*solar_scalar
-    P3_lunar = 5.0/2.0*(h3 - 3.0*l3)*lunar_scalar**3 + \
-        3.0/2.0*(l3 - h3)*lunar_scalar
+    P3_solar = 5.0/2.0*(kwargs['h3'] - 3.0*kwargs['l3'])*solar_scalar**3 + \
+        3.0/2.0*(kwargs['l3'] - kwargs['h3'])*solar_scalar
+    P3_lunar = 5.0/2.0*(kwargs['h3'] - 3.0*kwargs['l3'])*lunar_scalar**3 + \
+        3.0/2.0*(kwargs['l3'] - kwargs['h3'])*lunar_scalar
     # compute terms in direction of sun/moon vectors
     X2_solar = 3.0*l2*solar_scalar
     X2_lunar = 3.0*l2*lunar_scalar
-    X3_solar = 3.0*l3/2.0*(5.0*solar_scalar**2 - 1.0)
-    X3_lunar = 3.0*l3/2.0*(5.0*lunar_scalar**2 - 1.0)
+    X3_solar = 3.0*kwargs['l3']/2.0*(5.0*solar_scalar**2 - 1.0)
+    X3_lunar = 3.0*kwargs['l3']/2.0*(5.0*lunar_scalar**2 - 1.0)
     # factors for sun and moon using IAU estimates of mass ratios
-    F2_solar = mass_ratio_solar*a_axis*(a_axis/solar_radius)**3
-    F2_lunar = mass_ratio_lunar*a_axis*(a_axis/lunar_radius)**3
-    F3_solar = mass_ratio_lunar*a_axis*(a_axis/solar_radius)**4
-    F3_lunar = mass_ratio_lunar*a_axis*(a_axis/lunar_radius)**4
+    F2_solar = kwargs['mass_ratio_solar']*a_axis*(a_axis/solar_radius)**3
+    F2_lunar = kwargs['mass_ratio_lunar']*a_axis*(a_axis/lunar_radius)**3
+    F3_solar = kwargs['mass_ratio_solar']*a_axis*(a_axis/solar_radius)**4
+    F3_lunar = kwargs['mass_ratio_lunar']*a_axis*(a_axis/lunar_radius)**4
     # compute total displacement (Mathews et al. 1997)
     dxt = np.zeros((nt, 3))
     for i in range(3):
         S2 = F2_solar*(X2_solar*SXYZ[:,i]/solar_radius+P2_solar*XYZ[:,i]/radius)
         L2 = F2_lunar*(X2_lunar*LXYZ[:,i]/lunar_radius+P2_lunar*XYZ[:,i]/radius)
         S3 = F3_solar*(X3_solar*SXYZ[:,i]/solar_radius+P3_solar*XYZ[:,i]/radius)
         L3 = F3_lunar*(X3_lunar*LXYZ[:,i]/lunar_radius+P3_lunar*XYZ[:,i]/radius)
         dxt[:,i] = S2 + L2 + S3 + L3
-    # corrections for out-of-phase portions of the love numbers
-    DDX, DDY, DDZ = _out_of_phase_diurnal(XYZ, SXYZ, LXYZ, F2_solar, F2_lunar)
-    DSX, DSY, DSZ = _out_of_phase_semidiurnal(XYZ, SXYZ, LXYZ, F2_solar, F2_lunar)
+    # corrections for out-of-phase portions of the Love and Shida numbers
+    dxt += _out_of_phase_diurnal(XYZ, SXYZ, LXYZ, F2_solar, F2_lunar)
+    dxt += _out_of_phase_semidiurnal(XYZ, SXYZ, LXYZ, F2_solar, F2_lunar)
     # corrections for the latitudinal dependence
-    DLX, DLY, DLZ = _latitude_dependence(XYZ, SXYZ, LXYZ, F2_solar, F2_lunar)
+    dxt += _latitude_dependence(XYZ, SXYZ, LXYZ, F2_solar, F2_lunar)
     # corrections for the frequency dependence
-    DFDX, DFDY, DFDZ = _frequency_dependence_diurnal(XYZ, MJD)
-    DFLX, DFLY, DFLZ = _frequency_dependence_long_period(XYZ, MJD)
-    # add the corrections to the total displacement
-    dxt += np.c_[DDX, DDY, DDZ]
-    dxt += np.c_[DSX, DSY, DSZ]
-    dxt += np.c_[DLX, DLY, DLZ]
-    dxt += np.c_[DFDX, DFDY, DFDZ]
-    dxt += np.c_[DFLX, DFLY, DFLZ]
+    dxt += _frequency_dependence_diurnal(XYZ, MJD)
+    dxt += _frequency_dependence_long_period(XYZ, MJD)
     # convert the permanent tide system if specified
     if (tide_system.lower() == 'mean_tide'):
-        DPTX, DPTY, DPTZ = _free_to_mean(XYZ, h2, l2)
-        dxt += np.c_[DPTX, DPTY, DPTZ]
+        dxt += _free_to_mean(XYZ, h2, l2)
     # return the solid earth tide
     return dxt
 
-def _out_of_phase_diurnal(XYZ: np.ndarray, SXYZ: np.ndarray,
-    LXYZ: np.ndarray, F2_solar: np.ndarray, F2_lunar: np.ndarray):
+def _out_of_phase_diurnal(
+        XYZ: np.ndarray,
+        SXYZ: np.ndarray,
+        LXYZ: np.ndarray,
+        F2_solar: np.ndarray,
+        F2_lunar: np.ndarray
+    ):
     """
     Computes the out-of-phase corrections induced by mantle
     anelasticity in the diurnal band
+
+    Parameters
+    ----------
+    XYZ: np.ndarray
+        Cartesian coordinates of the station (meters)
+    SXYZ: np.ndarray
+        Earth-centered Earth-fixed coordinates of the sun (meters)
+    LXYZ: np.ndarray
+        Earth-centered Earth-fixed coordinates of the moon (meters)
+    F2_solar: np.ndarray
+        Factors for the sun
+    F2_lunar: np.ndarray
+        Factors for the moon
     """
-    # love number corrections
+    # Love and Shida number corrections
     dhi = -0.0025
     dli = -0.0007
     # Compute the normalized position vector of coordinates
     radius = np.sqrt(np.sum(XYZ**2, axis=1))
     sinphi = XYZ[:,2]/radius
     cosphi = np.sqrt(XYZ[:,0]**2 + XYZ[:,1]**2)/radius
     cos2phi = cosphi**2 - sinphi**2
@@ -710,27 +733,45 @@
     de_lunar = -3.0*dli*sinphi*F2_lunar*LXYZ[:,2]* \
         (LXYZ[:,0]*cosla+LXYZ[:,1]*sinla)/lunar_radius**2
     # add solar and lunar offsets
     DR = dr_solar + dr_lunar
     DN = dn_solar + dn_lunar
     DE = de_solar + de_lunar
     # compute corrections
-    DX = DR*cosla*cosphi - DE*sinla - DN*sinphi*cosla
-    DY = DR*sinla*cosphi + DE*cosla - DN*sinphi*sinla
+    DX = DR*cosla*cosphi - DE*sinla - DN*cosla*sinphi
+    DY = DR*sinla*cosphi + DE*cosla - DN*sinla*sinphi
     DZ = DR*sinphi + DN*cosphi
     # return the corrections
-    return (DX, DY, DZ)
+    return np.c_[DX, DY, DZ]
 
-def _out_of_phase_semidiurnal(XYZ: np.ndarray, SXYZ: np.ndarray,
-    LXYZ: np.ndarray, F2_solar: np.ndarray, F2_lunar: np.ndarray):
+def _out_of_phase_semidiurnal(
+        XYZ: np.ndarray,
+        SXYZ: np.ndarray,
+        LXYZ: np.ndarray,
+        F2_solar: np.ndarray,
+        F2_lunar: np.ndarray
+    ):
     """
     Computes the out-of-phase corrections induced by mantle
     anelasticity in the semi-diurnal band
+
+    Parameters
+    ----------
+    XYZ: np.ndarray
+        Cartesian coordinates of the station (meters)
+    SXYZ: np.ndarray
+        Earth-centered Earth-fixed coordinates of the sun (meters)
+    LXYZ: np.ndarray
+        Earth-centered Earth-fixed coordinates of the moon (meters)
+    F2_solar: np.ndarray
+        Factors for the sun
+    F2_lunar: np.ndarray
+        Factors for the moon
     """
-    # love number corrections
+    # Love and Shida number corrections
     dhi = -0.0022
     dli = -0.0007
     # Compute the normalized position vector of coordinates
     radius = np.sqrt(np.sum(XYZ**2, axis=1))
     sinphi = XYZ[:,2]/radius
     cosphi = np.sqrt(XYZ[:,0]**2 + XYZ[:,1]**2)/radius
     sinla = XYZ[:,1]/cosphi/radius
@@ -760,27 +801,45 @@
         ((LXYZ[:,0]**2-LXYZ[:,1]**2)*cos2la+2.0*LXYZ[:,0]*LXYZ[:,1]*sin2la) / \
         lunar_radius**2
     # add solar and lunar offsets
     DR = dr_solar + dr_lunar
     DN = dn_solar + dn_lunar
     DE = de_solar + de_lunar
     # compute corrections
-    DX = DR*cosla*cosphi - DE*sinla - DN*sinphi*cosla
-    DY = DR*sinla*cosphi + DE*cosla - DN*sinphi*sinla
+    DX = DR*cosla*cosphi - DE*sinla - DN*cosla*sinphi
+    DY = DR*sinla*cosphi + DE*cosla - DN*sinla*sinphi
     DZ = DR*sinphi + DN*cosphi
     # return the corrections
-    return (DX, DY, DZ)
+    return np.c_[DX, DY, DZ]
 
-def _latitude_dependence(XYZ: np.ndarray, SXYZ: np.ndarray,
-    LXYZ: np.ndarray, F2_solar, F2_lunar):
+def _latitude_dependence(
+        XYZ: np.ndarray,
+        SXYZ: np.ndarray,
+        LXYZ: np.ndarray,
+        F2_solar: np.ndarray,
+        F2_lunar: np.ndarray
+    ):
     """
     Computes the corrections induced by the latitude of the
     dependence given by L\ :sup:`1`
+
+    Parameters
+    ----------
+    XYZ: np.ndarray
+        Cartesian coordinates of the station (meters)
+    SXYZ: np.ndarray
+        Earth-centered Earth-fixed coordinates of the sun (meters)
+    LXYZ: np.ndarray
+        Earth-centered Earth-fixed coordinates of the moon (meters)
+    F2_solar: np.ndarray
+        Factors for the sun
+    F2_lunar: np.ndarray
+        Factors for the moon
     """
-    # love number corrections (diurnal and semi-diurnal)
+    # Love/Shida number corrections (diurnal and semi-diurnal)
     l1d = 0.0012
     l1sd = 0.0024
     # Compute the normalized position vector of coordinates
     radius = np.sqrt(np.sum(XYZ**2, axis=1))
     sinphi = XYZ[:,2]/radius
     cosphi = np.sqrt(XYZ[:,0]**2 + XYZ[:,1]**2)/radius
     sinla = XYZ[:,1]/cosphi/radius
@@ -812,29 +871,39 @@
     de_s_lunar =-l1sd/2.0*sinphi**2*cosphi*F2_lunar * \
         ((LXYZ[:,0]**2-LXYZ[:,1]**2)*sin2la-2.0*LXYZ[:,0]*LXYZ[:,1]*cos2la) / \
         lunar_radius**2
     # add solar and lunar offsets (diurnal and semi-diurnal)
     DN = 3.0*(dn_d_solar + dn_d_lunar + dn_s_solar + dn_s_lunar)
     DE = 3.0*(de_d_solar + de_d_lunar + de_s_solar + de_s_lunar)
     # compute combined diurnal and semi-diurnal corrections
-    DX = -DE*sinla - DN*sinphi*cosla
-    DY = DE*cosla - DN*sinphi*sinla
+    DX = -DE*sinla - DN*cosla*sinphi
+    DY = DE*cosla - DN*sinla*sinphi
     DZ = DN*cosphi
     # return the corrections
-    return (DX, DY, DZ)
+    return np.c_[DX, DY, DZ]
 
-def _frequency_dependence_diurnal(XYZ: np.ndarray, MJD: np.ndarray):
+def _frequency_dependence_diurnal(
+        XYZ: np.ndarray,
+        MJD: np.ndarray
+    ):
     """
     Computes the in-phase and out-of-phase corrections induced by mantle
     anelasticity in the diurnal band
+
+    Parameters
+    ----------
+    XYZ: np.ndarray
+        Cartesian coordinates of the station (meters)
+    MJD: np.ndarray
+        Modified Julian Day (MJD)
     """
     # number of time steps
     nt = len(np.atleast_1d(MJD))
     # Corrections to Diurnal Tides for Frequency Dependence
-    # of Love Number Parameters
+    # of Love and Shida Number Parameters
     # table 7.3a of IERS conventions
     table = np.array([
         [-3.0, 0.0, 2.0, 0.0, 0.0, -0.01, 0.0, 0.0, 0.0],
         [-3.0, 2.0, 0.0, 0.0, 0.0, -0.01, 0.0, 0.0, 0.0],
         [-2.0, 0.0, 1.0, -1.0, 0.0, -0.02, 0.0, 0.0, 0.0],
         [-2.0, 0.0, 1.0, 0.0, 0.0, -0.08, 0.0, -0.01, 0.01],
         [-2.0, 2.0, -1.0, 0.0, 0.0, -0.02, 0.0, 0.0, 0.0],
@@ -884,29 +953,39 @@
             ZNS*row[3] + PS*row[4]
         dr = 2.0*row[5]*sinphi*cosphi*np.sin(thetaf + zla) + \
             2.0*row[6]*sinphi*cosphi*np.cos(thetaf + zla)
         dn = row[7]*(cosphi**2 - sinphi**2)*np.sin(thetaf + zla) + \
             row[8]*(cosphi**2 - sinphi**2)*np.cos(thetaf + zla)
         de = row[7]*sinphi*np.cos(thetaf + zla) - \
             row[8]*sinphi*np.sin(thetaf + zla)
-        DX += 1e-3*(dr*cosla*cosphi - de*sinla - dn*sinphi*cosla)
-        DY += 1e-3*(dr*sinla*cosphi + de*cosla - dn*sinphi*sinla)
+        DX += 1e-3*(dr*cosla*cosphi - de*sinla - dn*cosla*sinphi)
+        DY += 1e-3*(dr*sinla*cosphi + de*cosla - dn*sinla*sinphi)
         DZ += 1e-3*(dr*sinphi + dn*cosphi)
     # return the corrections
-    return (DX, DY, DZ)
+    return np.c_[DX, DY, DZ]
 
-def _frequency_dependence_long_period(XYZ: np.ndarray, MJD: np.ndarray):
+def _frequency_dependence_long_period(
+        XYZ: np.ndarray,
+        MJD: np.ndarray
+    ):
     """
     Computes the in-phase and out-of-phase corrections induced by mantle
     anelasticity in the long-period band
+
+    Parameters
+    ----------
+    XYZ: np.ndarray
+        Cartesian coordinates of the station (meters)
+    MJD: np.ndarray
+        Modified Julian Day (MJD)
     """
     # number of time steps
     nt = len(np.atleast_1d(MJD))
     # Corrections to Long-Peroid Tides for Frequency Dependence
-    # of Love Number Parameters
+    # of Love and Shida Number Parameters
     # table 7.3b of IERS conventions
     table = np.array([
         [0.0, 0.0, 0.0, 1.0, 0.0, 0.47, 0.23, 0.16, 0.07],
         [0.0, 2.0, 0.0, 0.0, 0.0, -0.20, -0.12, -0.11, -0.05],
         [1.0, 0.0, -1.0, 0.0, 0.0, -0.11, -0.08, -0.09, -0.04],
         [2.0, 0.0, 0.0, 0.0, 0.0, -0.13, -0.11, -0.15, -0.07],
         [2.0, 0.0, 0.0, 1.0, 0.0, -0.05, -0.05, -0.06, -0.03]
@@ -927,33 +1006,52 @@
     for i, row in enumerate(table):
         thetaf = S*row[0] + H*row[1] + P*row[2] + ZNS*row[3] + PS*row[4]
         dr = row[5]*(3.0*sinphi**2 - 1.0)*np.cos(thetaf)/2.0 + \
             row[7]*(3.0*sinphi**2 - 1.0)*np.sin(thetaf)/2.0
         dn = row[6]*(2.0*cosphi*sinphi)*np.cos(thetaf) + \
             row[8]*(2.0*cosphi*sinphi)*np.sin(thetaf)
         de = 0.0
-        DX += 1e-3*(dr*cosla*cosphi - de*sinla - dn*sinphi*cosla)
-        DY += 1e-3*(dr*sinla*cosphi + de*cosla - dn*sinphi*sinla)
+        DX += 1e-3*(dr*cosla*cosphi - de*sinla - dn*cosla*sinphi)
+        DY += 1e-3*(dr*sinla*cosphi + de*cosla - dn*sinla*sinphi)
         DZ += 1e-3*(dr*sinphi + dn*cosphi)
     # return the corrections
-    return (DX, DY, DZ)
+    return np.c_[DX, DY, DZ]
 
-def _free_to_mean(XYZ: np.ndarray, h2: float | np.ndarray,
-    l2: float | np.ndarray):
+def _free_to_mean(
+        XYZ: np.ndarray,
+        h2: float | np.ndarray,
+        l2: float | np.ndarray
+    ):
     """
     Calculate offsets for converting the permanent tide from
     a tide-free to a mean-tide state
+
+    Parameters
+    ----------
+    XYZ: np.ndarray
+        Cartesian coordinates of the station (meters)
+    h2: float or np.ndarray
+        Degree-2 Love number of vertical displacement
+    l2: float or np.ndarray
+        Degree-2 Love (Shida) number of horizontal displacement
     """
     # Compute the normalized position vector of coordinates
     radius = np.sqrt(np.sum(XYZ**2, axis=1))
     sinphi = XYZ[:,2]/radius
     cosphi = np.sqrt(XYZ[:,0]**2 + XYZ[:,1]**2)/radius
     sinla = XYZ[:,1]/cosphi/radius
     cosla = XYZ[:,0]/cosphi/radius
-    dr = -np.sqrt(5.0/(4.0*np.pi))*h2*0.31460*(3.0/2.0*sinphi**2 - 0.5)
-    dn = -np.sqrt(5.0/(4.0*np.pi))*l2*0.31460*3.0*cosphi*sinphi
-    # compute as an additive correction
-    DX = -dr*cosla*cosphi + dn*cosla*sinphi
-    DY = -dr*sinla*cosphi + dn*sinla*sinphi
-    DZ = -dr*sinphi - dn*cosphi
+    # time-independent constituent of amplitude (Mathews et al. 1997)
+    H0 = -0.31460
+    # in Mathews et al. (1997): dR0=-0.1196 m with h2=0.6026
+    dR0 = np.sqrt(5.0/(4.0*np.pi))*h2*H0
+    # in Mathews et al. (1997): dN0=-0.0247 m with l2=0.0831
+    dN0 = np.sqrt(45.0/(16.0*np.pi))*l2*H0
+    # use double angle formula for sin(2*phi)
+    dr = dR0*(3.0/2.0*sinphi**2 - 1.0/2.0)
+    dn = 2.0*dN0*cosphi*sinphi
+    # compute as an additive correction (Mathews et al. 1997)
+    DX = dr*cosla*cosphi - dn*cosla*sinphi
+    DY = dr*sinla*cosphi - dn*sinla*sinphi
+    DZ = dr*sinphi + dn*cosphi
     # return the corrections
-    return (DX, DY, DZ)
+    return np.c_[DX, DY, DZ]
```

### Comparing `pyTMD-2.0.3/pyTMD/spatial.py` & `pyTMD-2.0.4/pyTMD/spatial.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,14 +19,17 @@
         https://github.com/yaml/pyyaml
 
 PROGRAM DEPENDENCIES:
     constants.py: calculate reference parameters for common ellipsoids
 
 UPDATE HISTORY:
     Updated 04/2023: copy inputs in cartesian to not modify original arrays
+        added iterative methods for converting from cartesian to geodetic
+        allow netCDF4 and HDF5 outputs to be appended to existing files
+        using pathlib to define and expand paths
     Updated 03/2023: add basic variable typing to function inputs
     Updated 02/2023: use outputs from constants class for WGS84 parameters
         include more possible dimension names for gridded and drift outputs
     Updated 01/2023: added default field mapping for reading from netCDF4/HDF5
         split netCDF4 output into separate functions for grid and drift types
     Updated 12/2022: add software information to output HDF5 and netCDF4
     Updated 11/2022: place some imports within try/except statements
@@ -56,22 +59,22 @@
     Updated 12/2020: added module for converting ellipsoids
     Updated 11/2020: output data as masked arrays if containing fill values
         add functions to read from and write to geotiff image formats
     Written 09/2020
 """
 from __future__ import annotations
 
-import os
 import re
 import io
 import copy
 import gzip
 import uuid
 import yaml
 import logging
+import pathlib
 import datetime
 import warnings
 import numpy as np
 import dateutil.parser
 from pyTMD.constants import constants
 import pyTMD.version
 # attempt imports
@@ -89,33 +92,35 @@
     import netCDF4
 except (ImportError, ModuleNotFoundError) as exc:
     warnings.filterwarnings("module")
     warnings.warn("netCDF4 not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
-def case_insensitive_filename(filename: str) -> str:
+def case_insensitive_filename(filename: str | pathlib.Path):
     """
     Searches a directory for a filename without case dependence
 
     Parameters
     ----------
     filename: str
         input filename
     """
     # check if file presently exists with input case
-    if not os.access(os.path.expanduser(filename),os.F_OK):
+    filename = pathlib.Path(filename).expanduser().absolute()
+    if not filename.exists():
         # search for filename without case dependence
-        basename = os.path.basename(filename)
-        directory = os.path.dirname(os.path.expanduser(filename))
-        f = [f for f in os.listdir(directory) if re.match(basename,f,re.I)]
+        f = [f.name for f in filename.parent.iterdir() if
+             re.match(filename.name, f.name, re.I)]
+        # raise error if no file found
         if not f:
-            raise FileNotFoundError(f'{filename} not found in file system')
-        filename = os.path.join(directory,f.pop())
-    return os.path.expanduser(filename)
+            raise FileNotFoundError(str(filename))
+        filename = filename.with_name(f.pop())
+    # return the matched filename
+    return filename
 
 def data_type(x: np.ndarray, y: np.ndarray, t: np.ndarray) -> str:
     """
     Determines input data type based on variable dimensions
 
     Parameters
     ----------
@@ -180,31 +185,31 @@
 
     Parameters
     ----------
     filename: str
         full path of input ascii file
     compression: str or NoneType, default None
         file compression type
-    columns: list, default ['time','y','x','data']
+    columns: list, default ['time', 'y', 'x', 'data']
         column names of ascii file
-    delimiter: str,
+    delimiter: str, default ','
         Delimiter for csv or ascii files
     header: int, default 0
         header lines to skip from start of file
     parse_dates: bool, default False
         Try parsing the time column
     """
     # set default keyword arguments
-    kwargs.setdefault('compression',None)
-    kwargs.setdefault('columns',['time','y','x','data'])
-    kwargs.setdefault('delimiter',',')
-    kwargs.setdefault('header',0)
-    kwargs.setdefault('parse_dates',False)
+    kwargs.setdefault('compression', None)
+    kwargs.setdefault('columns', ['time', 'y', 'x', 'data'])
+    kwargs.setdefault('delimiter', ',')
+    kwargs.setdefault('header', 0)
+    kwargs.setdefault('parse_dates', False)
     # print filename
-    logging.info(filename)
+    logging.info(str(filename))
     # get column names
     columns = copy.copy(kwargs['columns'])
     # open the ascii file and extract contents
     if (kwargs['compression'] == 'gzip'):
         # read input ascii data from gzip compressed file and split lines
         filename = case_insensitive_filename(filename)
         with gzip.open(filename, 'r') as f:
@@ -229,52 +234,54 @@
         YAML = False
         count = 0
         # Reading over header text
         while (YAML is False) & (count < file_lines):
             # file line at count
             line = file_contents[count]
             # if End of YAML Header is found: set YAML flag
-            YAML = bool(re.search(r"\# End of YAML header",line))
+            YAML = bool(re.search(r"\# End of YAML header", line))
             # add 1 to counter
             count += 1
         # parse the YAML header (specifying yaml loader)
         YAML_HEADER = yaml.load('\n'.join(file_contents[:count]),
            Loader=yaml.BaseLoader)
         # output spatial data and attributes
         dinput = {}
         # copy global attributes
         dinput['attributes'] = YAML_HEADER['header']['global_attributes']
         # allocate for each variable and copy variable attributes
         for c in columns:
             if (c == 'time') and kwargs['parse_dates']:
-                dinput[c] = np.zeros((file_lines-count),dtype='datetime64[ms]')
+                dinput[c] = np.zeros((file_lines-count), dtype='datetime64[ms]')
             else:
                 dinput[c] = np.zeros((file_lines-count))
             dinput['attributes'][c] = YAML_HEADER['header']['variables'][c]
         # update number of file lines to skip for reading data
         header = int(count)
     else:
         # allocate for each variable and variable attributes
         dinput = {}
         header = int(kwargs['header'])
         for c in columns:
             if (c == 'time') and kwargs['parse_dates']:
-                dinput[c] = np.zeros((file_lines-header),dtype='datetime64[ms]')
+                dinput[c] = np.zeros((file_lines-header), dtype='datetime64[ms]')
             else:
                 dinput[c] = np.zeros((file_lines-header))
         dinput['attributes'] = {c:dict() for c in columns}
     # extract spatial data array
     # for each line in the file
-    for i,line in enumerate(file_contents[header:]):
+    for i, line in enumerate(file_contents[header:]):
         # extract columns of interest and assign to dict
         # convert fortran exponentials if applicable
         if kwargs['delimiter']:
-            column = {c:l.replace('D','E') for c,l in zip(columns,line.split(kwargs['delimiter']))}
+            column = {c:l.replace('D', 'E') for c, l in
+                zip(columns, line.split(kwargs['delimiter']))}
         else:
-            column = {c:r.replace('D','E') for c,r in zip(columns,rx.findall(line))}
+            column = {c:r.replace('D', 'E') for c, r in
+                zip(columns, rx.findall(line))}
         # copy variables from column dict to output dictionary
         for c in columns:
             if (c == 'time') and kwargs['parse_dates']:
                 dinput[c][i] = dateutil.parser.parse(column[c])
             else:
                 dinput[c][i] = np.float64(column[c])
     # convert to masked array if fill values
@@ -303,71 +310,71 @@
         name for y-dimension variable
     varname: str, default 'data'
         name for data variable
     field_mapping: dict, default {}
         mapping between output variables and input netCDF4
     """
     # set default keyword arguments
-    kwargs.setdefault('compression',None)
-    kwargs.setdefault('timename','time')
-    kwargs.setdefault('xname','lon')
-    kwargs.setdefault('yname','lat')
-    kwargs.setdefault('varname','data')
-    kwargs.setdefault('field_mapping',{})
+    kwargs.setdefault('compression', None)
+    kwargs.setdefault('timename', 'time')
+    kwargs.setdefault('xname', 'lon')
+    kwargs.setdefault('yname', 'lat')
+    kwargs.setdefault('varname', 'data')
+    kwargs.setdefault('field_mapping', {})
     # read data from netCDF4 file
     # Open the NetCDF4 file for reading
     if (kwargs['compression'] == 'gzip'):
         # read as in-memory (diskless) netCDF4 dataset
-        with gzip.open(case_insensitive_filename(filename),'r') as f:
-            fileID = netCDF4.Dataset(uuid.uuid4().hex,memory=f.read())
+        with gzip.open(case_insensitive_filename(filename), 'r') as f:
+            fileID = netCDF4.Dataset(uuid.uuid4().hex, memory=f.read())
     elif (kwargs['compression'] == 'bytes'):
         # read as in-memory (diskless) netCDF4 dataset
-        fileID = netCDF4.Dataset(uuid.uuid4().hex,memory=filename.read())
+        fileID = netCDF4.Dataset(uuid.uuid4().hex, memory=filename.read())
     else:
         # read netCDF4 dataset
         fileID = netCDF4.Dataset(case_insensitive_filename(filename), 'r')
     # Output NetCDF file information
     logging.info(fileID.filepath())
     logging.info(list(fileID.variables.keys()))
     # create python dictionary for output variables and attributes
     dinput = {}
     dinput['attributes'] = {}
     # get attributes for the file
-    for attr in ['title','description','projection']:
+    for attr in ['title', 'description', 'projection']:
         # try getting the attribute
         try:
-            ncattr, = [s for s in fileID.ncattrs() if re.match(attr,s,re.I)]
+            ncattr, = [s for s in fileID.ncattrs() if re.match(attr, s, re.I)]
             dinput['attributes'][attr] = fileID.getncattr(ncattr)
-        except (ValueError,AttributeError):
+        except (ValueError, AttributeError):
             pass
     # list of attributes to attempt to retrieve from included variables
-    attributes_list = ['description','units','long_name','calendar',
-        'standard_name','grid_mapping','_FillValue']
+    attributes_list = ['description', 'units', 'long_name', 'calendar',
+        'standard_name', 'grid_mapping', '_FillValue']
     # mapping between netCDF4 variable names and output names
     if not kwargs['field_mapping']:
         kwargs['field_mapping']['x'] = copy.copy(kwargs['xname'])
         kwargs['field_mapping']['y'] = copy.copy(kwargs['yname'])
         if kwargs['varname'] is not None:
             kwargs['field_mapping']['data'] = copy.copy(kwargs['varname'])
         if kwargs['timename'] is not None:
             kwargs['field_mapping']['time'] = copy.copy(kwargs['timename'])
     # for each variable
-    for key,nc in kwargs['field_mapping'].items():
+    for key, nc in kwargs['field_mapping'].items():
         # Getting the data from each NetCDF variable
         dinput[key] = fileID.variables[nc][:]
         # get attributes for the included variables
         dinput['attributes'][key] = {}
         for attr in attributes_list:
             # try getting the attribute
             try:
                 ncattr, = [s for s in fileID.variables[nc].ncattrs()
-                    if re.match(attr,s,re.I)]
+                    if re.match(attr, s, re.I)]
                 dinput['attributes'][key][attr] = \
                     fileID.variables[nc].getncattr(ncattr)
-            except (ValueError,AttributeError):
+            except (ValueError, AttributeError):
                 pass
     # get projection information if there is a grid_mapping attribute
     if 'data' in dinput.keys() and 'grid_mapping' in dinput['attributes']['data'].keys():
         # try getting the attribute
         grid_mapping = dinput['attributes']['data']['grid_mapping']
         # get coordinate reference system attributes
         dinput['attributes']['crs'] = {}
@@ -385,15 +392,15 @@
         dinput['data'].fill_value = dinput['attributes']['data']['_FillValue']
         dinput['data'].mask = (dinput['data'].data == dinput['data'].fill_value)
     # Closing the NetCDF file
     fileID.close()
     # return the spatial variables
     return dinput
 
-def from_HDF5(filename: str, **kwargs):
+def from_HDF5(filename: str | pathlib.Path, **kwargs):
     """
     Read data from a HDF5 file
 
     Parameters
     ----------
     filename: str
         full path of input HDF5 file
@@ -407,28 +414,28 @@
         name for y-dimension variable
     varname: str, default 'data'
         name for data variable
     field_mapping: dict, default {}
         mapping between output variables and input HDF5
     """
     # set default keyword arguments
-    kwargs.setdefault('compression',None)
-    kwargs.setdefault('timename','time')
-    kwargs.setdefault('xname','lon')
-    kwargs.setdefault('yname','lat')
-    kwargs.setdefault('varname','data')
-    kwargs.setdefault('field_mapping',{})
+    kwargs.setdefault('compression', None)
+    kwargs.setdefault('timename', 'time')
+    kwargs.setdefault('xname', 'lon')
+    kwargs.setdefault('yname', 'lat')
+    kwargs.setdefault('varname', 'data')
+    kwargs.setdefault('field_mapping', {})
     # read data from HDF5 file
     # Open the HDF5 file for reading
     if (kwargs['compression'] == 'gzip'):
         # read gzip compressed file and extract into in-memory file object
-        with gzip.open(case_insensitive_filename(filename),'r') as f:
+        with gzip.open(case_insensitive_filename(filename), 'r') as f:
             fid = io.BytesIO(f.read())
         # set filename of BytesIO object
-        fid.filename = os.path.basename(filename)
+        fid.filename = filename.name
         # rewind to start of file
         fid.seek(0)
         # read as in-memory (diskless) HDF5 dataset from BytesIO object
         fileID = h5py.File(fid, 'r')
     elif (kwargs['compression'] == 'bytes'):
         # read as in-memory (diskless) HDF5 dataset
         fileID = h5py.File(filename, 'r')
@@ -438,50 +445,50 @@
     # Output HDF5 file information
     logging.info(fileID.filename)
     logging.info(list(fileID.keys()))
     # create python dictionary for output variables and attributes
     dinput = {}
     dinput['attributes'] = {}
     # get attributes for the file
-    for attr in ['title','description','projection']:
+    for attr in ['title', 'description', 'projection']:
         # try getting the attribute
         try:
             dinput['attributes'][attr] = fileID.attrs[attr]
-        except (KeyError,AttributeError):
+        except (KeyError, AttributeError):
             pass
     # list of attributes to attempt to retrieve from included variables
-    attributes_list = ['description','units','long_name','calendar',
-        'standard_name','grid_mapping','_FillValue']
+    attributes_list = ['description', 'units', 'long_name', 'calendar',
+        'standard_name', 'grid_mapping', '_FillValue']
     # mapping between HDF5 variable names and output names
     if not kwargs['field_mapping']:
         kwargs['field_mapping']['x'] = copy.copy(kwargs['xname'])
         kwargs['field_mapping']['y'] = copy.copy(kwargs['yname'])
         if kwargs['varname'] is not None:
             kwargs['field_mapping']['data'] = copy.copy(kwargs['varname'])
         if kwargs['timename'] is not None:
             kwargs['field_mapping']['time'] = copy.copy(kwargs['timename'])
     # for each variable
-    for key,h5 in kwargs['field_mapping'].items():
+    for key, h5 in kwargs['field_mapping'].items():
         # Getting the data from each HDF5 variable
         dinput[key] = np.copy(fileID[h5][:])
         # get attributes for the included variables
         dinput['attributes'][key] = {}
         for attr in attributes_list:
             # try getting the attribute
             try:
                 dinput['attributes'][key][attr] = fileID[h5].attrs[attr]
-            except (KeyError,AttributeError):
+            except (KeyError, AttributeError):
                 pass
     # get projection information if there is a grid_mapping attribute
     if 'data' in dinput.keys() and 'grid_mapping' in dinput['attributes']['data'].keys():
         # try getting the attribute
         grid_mapping = dinput['attributes']['data']['grid_mapping']
         # get coordinate reference system attributes
         dinput['attributes']['crs'] = {}
-        for att_name,att_val in fileID[grid_mapping].attrs.items():
+        for att_name, att_val in fileID[grid_mapping].attrs.items():
             dinput['attributes']['crs'][att_name] = att_val
         # get the spatial projection reference information from wkt
         # and overwrite the file-level projection attribute (if existing)
         srs = osgeo.osr.SpatialReference()
         srs.ImportFromWkt(dinput['attributes']['crs']['crs_wkt'])
         dinput['attributes']['projection'] = srs.ExportToProj4()
     # convert to masked array if fill values
@@ -504,59 +511,59 @@
         full path of input geotiff file
     compression: str or NoneType, default None
         file compression type
     bounds: list or NoneType, default bounds
         extent of the file to read: ``[xmin, xmax, ymin, ymax]``
     """
     # set default keyword arguments
-    kwargs.setdefault('compression',None)
-    kwargs.setdefault('bounds',None)
+    kwargs.setdefault('compression', None)
+    kwargs.setdefault('bounds', None)
     # Open the geotiff file for reading
     if (kwargs['compression'] == 'gzip'):
         # read as GDAL gzip virtual geotiff dataset
-        mmap_name = f"/vsigzip/{case_insensitive_filename(filename)}"
+        mmap_name = f"/vsigzip/{str(case_insensitive_filename(filename))}"
         ds = osgeo.gdal.Open(mmap_name)
     elif (kwargs['compression'] == 'bytes'):
         # read as GDAL memory-mapped (diskless) geotiff dataset
         mmap_name = f"/vsimem/{uuid.uuid4().hex}"
         osgeo.gdal.FileFromMemBuffer(mmap_name, filename.read())
         ds = osgeo.gdal.Open(mmap_name)
     else:
         # read geotiff dataset
-        ds = osgeo.gdal.Open(case_insensitive_filename(filename),
+        ds = osgeo.gdal.Open(str(case_insensitive_filename(filename)),
             osgeo.gdalconst.GA_ReadOnly)
     # print geotiff file if verbose
-    logging.info(filename)
+    logging.info(str(filename))
     # create python dictionary for output variables and attributes
     dinput = {}
-    dinput['attributes'] = {c:dict() for c in ['x','y','data']}
+    dinput['attributes'] = {c:dict() for c in ['x', 'y', 'data']}
     # get the spatial projection reference information
     srs = ds.GetSpatialRef()
     dinput['attributes']['projection'] = srs.ExportToProj4()
     dinput['attributes']['wkt'] = srs.ExportToWkt()
     # get dimensions
     xsize = ds.RasterXSize
     ysize = ds.RasterYSize
     bsize = ds.RasterCount
     # get geotiff info
     info_geotiff = ds.GetGeoTransform()
-    dinput['attributes']['spacing'] = (info_geotiff[1],info_geotiff[5])
+    dinput['attributes']['spacing'] = (info_geotiff[1], info_geotiff[5])
     # calculate image extents
     xmin = info_geotiff[0]
     ymax = info_geotiff[3]
     xmax = xmin + (xsize-1)*info_geotiff[1]
     ymin = ymax + (ysize-1)*info_geotiff[5]
     # x and y pixel center coordinates (converted from upper left)
     x = xmin + info_geotiff[1]/2.0 + np.arange(xsize)*info_geotiff[1]
     y = ymax + info_geotiff[5]/2.0 + np.arange(ysize)*info_geotiff[5]
     # if reducing to specified bounds
     if kwargs['bounds'] is not None:
         # reduced x and y limits
-        xlimits = (kwargs['bounds'][0],kwargs['bounds'][1])
-        ylimits = (kwargs['bounds'][2],kwargs['bounds'][3])
+        xlimits = (kwargs['bounds'][0], kwargs['bounds'][1])
+        ylimits = (kwargs['bounds'][2], kwargs['bounds'][3])
         # Specify offset and rows and columns to read
         xoffset = int((xlimits[0] - xmin)/info_geotiff[1])
         yoffset = int((ymax - ylimits[1])/np.abs(info_geotiff[5]))
         xcount = int((xlimits[1] - xlimits[0])/info_geotiff[1]) + 1
         ycount = int((ylimits[1] - ylimits[0])/np.abs(info_geotiff[5])) + 1
         # reduced x and y pixel center coordinates
         dinput['x'] = x[slice(xoffset, xoffset + xcount, None)]
@@ -577,15 +584,15 @@
         dinput['data'] = ds.ReadAsArray()
     # image extent
     dinput['attributes']['extent'] = (xmin, xmax, ymin, ymax)
     # set default time to zero for each band
     dinput.setdefault('time', np.zeros((bsize)))
     # check if image has fill values
     dinput['data'] = np.ma.asarray(dinput['data'])
-    dinput['data'].mask = np.zeros_like(dinput['data'],dtype=bool)
+    dinput['data'].mask = np.zeros_like(dinput['data'], dtype=bool)
     if ds.GetRasterBand(1).GetNoDataValue():
         # mask invalid values
         dinput['data'].fill_value = ds.GetRasterBand(1).GetNoDataValue()
         # create mask array for bad values
         dinput['data'].mask[:] = (dinput['data'].data == dinput['data'].fill_value)
         # set attribute for fill value
         dinput['attributes']['data']['_FillValue'] = dinput['data'].fill_value
@@ -604,68 +611,73 @@
         python dictionary of output data
     attributes: dict
         python dictionary of output attributes
     filename: str
         full path of output ascii file
     delimiter: str, default ','
         delimiter for output spatial file
-    columns: list, default ['time','y','x','data']
+    columns: list, default ['time', 'y', 'x', 'data']
         column names of ascii file
     header: bool, default False
         create a YAML header with data attributes
     """
     # set default keyword arguments
-    kwargs.setdefault('delimiter',',')
-    kwargs.setdefault('columns',['time','lat','lon','tide'])
-    kwargs.setdefault('header',False)
+    kwargs.setdefault('delimiter', ',')
+    kwargs.setdefault('columns', ['time', 'lat', 'lon', 'tide'])
+    kwargs.setdefault('header', False)
     # get column names
     columns = copy.copy(kwargs['columns'])
     # output filename
-    filename = os.path.expanduser(filename)
-    logging.info(filename)
+    filename = pathlib.Path(filename).expanduser().absolute()
+    logging.info(str(filename))
     # open the output file
-    fid = open(filename, mode='w', encoding='utf8')
+    fid = filename.open(mode='w', encoding='utf8')
     # create a column stack arranging data in column order
     data_stack = np.c_[[output[col] for col in columns]]
-    ncol,nrow = np.shape(data_stack)
+    ncol, nrow = np.shape(data_stack)
     # print YAML header to top of file
     if kwargs['header']:
         fid.write('{0}:\n'.format('header'))
         # data dimensions
         fid.write('\n  {0}:\n'.format('dimensions'))
-        fid.write('    {0:22}: {1:d}\n'.format('time',nrow))
+        fid.write('    {0:22}: {1:d}\n'.format('time', nrow))
         # non-standard attributes
         fid.write('  {0}:\n'.format('non-standard_attributes'))
         # data format
-        fid.write('    {0:22}: ({1:d}f0.8)\n'.format('formatting_string',ncol))
+        fid.write('    {0:22}: ({1:d}f0.8)\n'.format('formatting_string', ncol))
         fid.write('\n')
         # global attributes
         fid.write('\n  {0}:\n'.format('global_attributes'))
         today = datetime.datetime.now().isoformat()
         fid.write('    {0:22}: {1}\n'.format('date_created', today))
         # print variable descriptions to YAML header
         fid.write('\n  {0}:\n'.format('variables'))
         # print YAML header with variable attributes
-        for i,v in enumerate(columns):
+        for i, v in enumerate(columns):
             fid.write('    {0:22}:\n'.format(v))
-            for atn,atv in attributes[v].items():
-                fid.write('      {0:20}: {1}\n'.format(atn,atv))
+            for atn, atv in attributes[v].items():
+                fid.write('      {0:20}: {1}\n'.format(atn, atv))
             # add precision and column attributes for ascii yaml header
             fid.write('      {0:20}: double_precision\n'.format('precision'))
-            fid.write('      {0:20}: column {1:d}\n'.format('comment',i+1))
+            fid.write('      {0:20}: column {1:d}\n'.format('comment', i+1))
         # end of header
         fid.write('\n\n# End of YAML header\n')
     # write to file for each data point
     for line in range(nrow):
-        line_contents = [f'{d:0.8f}' for d in data_stack[:,line]]
+        line_contents = [f'{d:0.8f}' for d in data_stack[:, line]]
         print(kwargs['delimiter'].join(line_contents), file=fid)
     # close the output file
     fid.close()
 
-def to_netCDF4(output: dict, attributes: dict, filename: str, **kwargs):
+def to_netCDF4(
+        output: dict,
+        attributes: dict,
+        filename: str | pathlib.Path,
+        **kwargs
+    ):
     """
     Wrapper function for writing data to a netCDF4 file
 
     Parameters
     ----------
     output: dict
         python dictionary of output data
@@ -677,17 +689,19 @@
         Input data type
 
             - ``'time series'``
             - ``'drift'``
             - ``'grid'``
     """
     # default arguments
+    kwargs.setdefault('mode', 'w')
     kwargs.setdefault('data_type', 'drift')
     # opening NetCDF file for writing
-    fileID = netCDF4.Dataset(os.path.expanduser(filename),'w',format="NETCDF4")
+    filename = pathlib.Path(filename).expanduser().absolute()
+    fileID = netCDF4.Dataset(filename, kwargs['mode'], format="NETCDF4")
     if kwargs['data_type'] in ('drift',):
         kwargs.pop('data_type')
         _drift_netCDF4(fileID, output, attributes, **kwargs)
     elif kwargs['data_type'] in ('grid',):
         kwargs.pop('data_type')
         _grid_netCDF4(fileID, output, attributes, **kwargs)
     elif  kwargs['data_type'] in ('time series',):
@@ -697,18 +711,18 @@
     fileID.date_created = datetime.datetime.now().isoformat()
     # add attributes for software information
     fileID.software_reference = pyTMD.version.project_name
     fileID.software_version = pyTMD.version.full_version
     # add file-level attributes if applicable
     if 'ROOT' in attributes.keys():
         # Defining attributes for file
-        for att_name,att_val in attributes['ROOT'].items():
-            fileID.setncattr(att_name,att_val)
+        for att_name, att_val in attributes['ROOT'].items():
+            fileID.setncattr(att_name, att_val)
     # Output NetCDF structure information
-    logging.info(filename)
+    logging.info(str(filename))
     logging.info(list(fileID.variables.keys()))
     # Closing the NetCDF file
     fileID.close()
 
 def _drift_netCDF4(fileID, output: dict, attributes: dict, **kwargs):
     """
     Write drift data variables to a netCDF4 file object
@@ -723,28 +737,30 @@
         python dictionary of output attributes
     """
 
     # Defining the NetCDF dimensions
     fileID.createDimension('time', len(np.atleast_1d(output['time'])))
     # defining the NetCDF variables
     nc = {}
-    for key,val in output.items():
-        if '_FillValue' in attributes[key].keys():
+    for key, val in output.items():
+        if key in fileID.variables:
+            nc[key] = fileID.variables[key]
+        elif '_FillValue' in attributes[key].keys():
             nc[key] = fileID.createVariable(key, val.dtype, ('time',),
                 fill_value=attributes[key]['_FillValue'], zlib=True)
             attributes[key].pop('_FillValue')
         elif val.shape:
             nc[key] = fileID.createVariable(key, val.dtype, ('time',))
         else:
             nc[key] = fileID.createVariable(key, val.dtype, ())
         # filling NetCDF variables
         nc[key][:] = val
         # Defining attributes for variable
-        for att_name,att_val in attributes[key].items():
-            nc[key].setncattr(att_name,att_val)
+        for att_name, att_val in attributes[key].items():
+            nc[key].setncattr(att_name, att_val)
 
 def _grid_netCDF4(fileID, output: dict, attributes: dict, **kwargs):
     """
     Write gridded data variables to a netCDF4 file object
 
     Parameters
     ----------
@@ -752,45 +768,47 @@
         open netCDF4 file object
     output: dict
         python dictionary of output data
     attributes: dict
         python dictionary of output attributes
     """
     # input data fields
-    dimensions = ['time','lon','lat','t','x','y']
+    dimensions = ['time', 'lon', 'lat', 't', 'x', 'y']
     fields = sorted(set(output.keys()) - set(dimensions))
     # Defining the NetCDF dimensions
-    ny,nx,nt = output[fields[0]].shape
+    ny, nx, nt = output[fields[0]].shape
     fileID.createDimension('y', ny)
     fileID.createDimension('x', nx)
     fileID.createDimension('time', nt)
     # defining the NetCDF variables
     nc = {}
-    for key,val in output.items():
-        if '_FillValue' in attributes[key].keys():
-            nc[key] = fileID.createVariable(key, val.dtype, ('y','x','time'),
+    for key, val in output.items():
+        if key in fileID.variables:
+            nc[key] = fileID.variables[key]
+        elif '_FillValue' in attributes[key].keys():
+            nc[key] = fileID.createVariable(key, val.dtype, ('y', 'x', 'time'),
                 fill_value=attributes[key]['_FillValue'], zlib=True)
             attributes[key].pop('_FillValue')
         elif (val.ndim == 3):
-            nc[key] = fileID.createVariable(key, val.dtype, ('y','x','time'))
+            nc[key] = fileID.createVariable(key, val.dtype, ('y', 'x', 'time'))
         elif (val.ndim == 2):
-            nc[key] = fileID.createVariable(key, val.dtype, ('y','x'))
+            nc[key] = fileID.createVariable(key, val.dtype, ('y', 'x'))
         elif val.shape and (len(val) == ny):
             nc[key] = fileID.createVariable(key, val.dtype, ('y',))
         elif val.shape and (len(val) == nx):
             nc[key] = fileID.createVariable(key, val.dtype, ('x',))
         elif val.shape and (len(val) == nt):
             nc[key] = fileID.createVariable(key, val.dtype, ('time',))
         else:
             nc[key] = fileID.createVariable(key, val.dtype, ())
         # filling NetCDF variables
         nc[key][:] = val
         # Defining attributes for variable
-        for att_name,att_val in attributes[key].items():
-            nc[key].setncattr(att_name,att_val)
+        for att_name, att_val in attributes[key].items():
+            nc[key].setncattr(att_name, att_val)
 
 def _time_series_netCDF4(fileID, output: dict, attributes: dict, **kwargs):
     """
     Write time series data variables to a netCDF4 file object
 
     Parameters
     ----------
@@ -798,90 +816,107 @@
         open netCDF4 file object
     output: dict
         python dictionary of output data
     attributes: dict
         python dictionary of output attributes
     """
     # input data fields
-    dimensions = ['time','lon','lat','t','x','y']
+    dimensions = ['time', 'lon', 'lat', 't', 'x', 'y']
     fields = sorted(set(output.keys()) - set(dimensions))
     # Defining the NetCDF dimensions
-    nstation,nt = output[fields[0]].shape
+    nstation, nt = output[fields[0]].shape
     fileID.createDimension('station', nstation)
     fileID.createDimension('time', nt)
     # defining the NetCDF variables
     nc = {}
-    for key,val in output.items():
-        if '_FillValue' in attributes[key].keys():
-            nc[key] = fileID.createVariable(key, val.dtype, ('station','time'),
+    for key, val in output.items():
+        if key in fileID.variables:
+            nc[key] = fileID.variables[key]
+        elif '_FillValue' in attributes[key].keys():
+            nc[key] = fileID.createVariable(key, val.dtype, ('station', 'time'),
                 fill_value=attributes[key]['_FillValue'], zlib=True)
             attributes[key].pop('_FillValue')
         elif (val.ndim == 2):
-            nc[key] = fileID.createVariable(key, val.dtype, ('station','time'))
+            nc[key] = fileID.createVariable(key, val.dtype, ('station', 'time'))
         elif val.shape and (len(val) == nt):
             nc[key] = fileID.createVariable(key, val.dtype, ('time',))
         elif val.shape and (len(val) == nstation):
             nc[key] = fileID.createVariable(key, val.dtype, ('station',))
         else:
             nc[key] = fileID.createVariable(key, val.dtype, ())
         # filling NetCDF variables
         nc[key][:] = val
         # Defining attributes for variable
-        for att_name,att_val in attributes[key].items():
-            nc[key].setncattr(att_name,att_val)
+        for att_name, att_val in attributes[key].items():
+            nc[key].setncattr(att_name, att_val)
 
-def to_HDF5(output: dict, attributes: dict, filename: str, **kwargs):
+def to_HDF5(
+        output: dict,
+        attributes: dict,
+        filename: str,
+        **kwargs
+    ):
     """
     Write data to a HDF5 file
 
     Parameters
     ----------
     output: dict
         python dictionary of output data
     attributes: dict
         python dictionary of output attributes
     filename: str
         full path of output HDF5 file
     """
+    # set default keyword arguments
+    kwargs.setdefault('mode', 'w')
     # opening HDF5 file for writing
-    fileID = h5py.File(filename, 'w')
+    filename = pathlib.Path(filename).expanduser().absolute()
+    fileID = h5py.File(filename, mode=kwargs['mode'])
     # Defining the HDF5 dataset variables
     h5 = {}
-    for key,val in output.items():
-        if '_FillValue' in attributes[key].keys():
+    for key, val in output.items():
+        if key in fileID:
+            fileID[key][...] = val[:]
+        elif '_FillValue' in attributes[key].keys():
             h5[key] = fileID.create_dataset(key, val.shape, data=val,
                 dtype=val.dtype, fillvalue=attributes[key]['_FillValue'],
                 compression='gzip')
             attributes[key].pop('_FillValue')
         elif val.shape:
             h5[key] = fileID.create_dataset(key, val.shape, data=val,
                 dtype=val.dtype, compression='gzip')
         else:
             h5[key] = fileID.create_dataset(key, val.shape,
                 dtype=val.dtype)
         # Defining attributes for variable
-        for att_name,att_val in attributes[key].items():
+        for att_name, att_val in attributes[key].items():
             h5[key].attrs[att_name] = att_val
     # add attribute for date created
     fileID.attrs['date_created'] = datetime.datetime.now().isoformat()
     # add attributes for software information
     fileID.attrs['software_reference'] = pyTMD.version.project_name
     fileID.attrs['software_version'] = pyTMD.version.full_version
     # add file-level attributes if applicable
     if 'ROOT' in attributes.keys():
         # Defining attributes for file
-        for att_name,att_val in attributes['ROOT'].items():
+        for att_name, att_val in attributes['ROOT'].items():
             fileID.attrs[att_name] = att_val
     # Output HDF5 structure information
-    logging.info(filename)
+    logging.info(str(filename))
     logging.info(list(fileID.keys()))
     # Closing the HDF5 file
     fileID.close()
 
-def to_geotiff(output: dict, attributes: dict, filename: str, **kwargs):
+def to_geotiff(
+        output: dict,
+        attributes: dict,
+        filename: str,
+        **kwargs
+    ):
     """
     Write data to a geotiff file
 
     Parameters
     ----------
     output: dict
         python dictionary of output data
@@ -898,48 +933,49 @@
             - ``'cog'``: Cloud Optimized GeoTIFF
     dtype: obj, default osgeo.gdal.GDT_Float64
         GDAL data type
     options: list, default ['COMPRESS=LZW']
         GDAL driver creation options
     """
     # set default keyword arguments
-    kwargs.setdefault('varname','data')
-    kwargs.setdefault('driver','cog')
-    kwargs.setdefault('dtype',osgeo.gdal.GDT_Float64)
-    kwargs.setdefault('options',['COMPRESS=LZW'])
+    kwargs.setdefault('varname', 'data')
+    kwargs.setdefault('driver', 'cog')
+    kwargs.setdefault('dtype', osgeo.gdal.GDT_Float64)
+    kwargs.setdefault('options', ['COMPRESS=LZW'])
     varname = copy.copy(kwargs['varname'])
     # verify grid dimensions to be iterable
     output = expand_dims(output, varname=varname)
     # grid shape
-    ny,nx,nband = np.shape(output[varname])
+    ny, nx, nband = np.shape(output[varname])
     # output as geotiff or specified driver
     driver = osgeo.gdal.GetDriverByName(kwargs['driver'])
     # set up the dataset with creation options
-    ds = driver.Create(filename, nx, ny, nband,
+    filename = pathlib.Path(filename).expanduser().absolute()
+    ds = driver.Create(str(filename), nx, ny, nband,
         kwargs['dtype'], kwargs['options'])
     # top left x, w-e pixel resolution, rotation
     # top left y, rotation, n-s pixel resolution
-    xmin,xmax,ymin,ymax = attributes['extent']
-    dx,dy = attributes['spacing']
-    ds.SetGeoTransform([xmin,dx,0,ymax,0,dy])
+    xmin, xmax, ymin, ymax = attributes['extent']
+    dx, dy = attributes['spacing']
+    ds.SetGeoTransform([xmin, dx, 0, ymax, 0, dy])
     # set the spatial projection reference information
     srs = osgeo.osr.SpatialReference()
     srs.ImportFromWkt(attributes['wkt'])
     # export
     ds.SetProjection( srs.ExportToWkt() )
     # for each band
     for band in range(nband):
         # set fill value for band
         if '_FillValue' in attributes[varname].keys():
             fill_value = attributes[varname]['_FillValue']
             ds.GetRasterBand(band+1).SetNoDataValue(fill_value)
         # write band to geotiff array
-        ds.GetRasterBand(band+1).WriteArray(output[varname][:,:,band])
+        ds.GetRasterBand(band+1).WriteArray(output[varname][:, :, band])
     # print filename if verbose
-    logging.info(filename)
+    logging.info(str(filename))
     # close dataset
     ds.FlushCache()
 
 def expand_dims(obj: dict, varname: str = 'data'):
     """
     Add a singleton dimension to a spatial dictionary if non-existent
 
@@ -952,18 +988,18 @@
     """
     # change time dimensions to be iterableinformation
     try:
         obj['time'] = np.atleast_1d(obj['time'])
     except:
         pass
     # output spatial with a third dimension
-    if isinstance(varname,list):
+    if isinstance(varname, list):
         for v in varname:
             obj[v] = np.atleast_3d(obj[v])
-    elif isinstance(varname,str):
+    elif isinstance(varname, str):
         obj[varname] = np.atleast_3d(obj[varname])
     # return reformed spatial dictionary
     return obj
 
 def default_field_mapping(variables: list | np.ndarray):
     """
     Builds field mappings from a variable list
@@ -982,15 +1018,15 @@
     Returns
     -------
     field_mapping: dict
         Field mappings for netCDF4/HDF5 read functions
     """
     # get each variable name and add to field mapping dictionary
     field_mapping = {}
-    for i,var in enumerate(['time','y','x','data']):
+    for i, var in enumerate(['time', 'y', 'x', 'data']):
         try:
             field_mapping[var] = copy.copy(variables[i])
         except IndexError as exc:
             pass
     # return the field mapping
     return field_mapping
 
@@ -1032,15 +1068,15 @@
     phi2: np.ndarray
         latitude of output ellipsoid in degrees
     h2: np.ndarray
         height above output ellipsoid in meters
 
     References
     ----------
-    .. [1] J Meeus, *Astronomical Algorithms*, pp. 77--82, (1991).
+    .. [1] J. Meeus, *Astronomical Algorithms*, 2nd edition, 477 pp., (1998).
     """
     if (len(phi1) != len(h1)):
         raise ValueError('phi and h have incompatable dimensions')
     # semiminor axis of input and output ellipsoid
     b1 = (1.0 - f1)*a1
     b2 = (1.0 - f2)*a2
     # initialize output arrays
@@ -1275,15 +1311,15 @@
     x = np.atleast_1d(np.copy(x))
     y = np.atleast_1d(np.copy(y))
     z = np.atleast_1d(np.copy(z))
     # calculate radius
     rad = np.sqrt(x**2.0 + y**2.0 + z**2.0)
     # calculate angular coordinates
     # phi: azimuthal angle
-    phi = np.arctan2(y,x)
+    phi = np.arctan2(y, x)
     # th: polar angle
     th = np.arccos(z/rad)
     # convert to degrees and fix to 0:360
     lon = 180.0*phi/np.pi
     if np.any(lon < 0):
         lt0 = np.nonzero(lon < 0)
         lon[lt0] += 360.0
@@ -1294,19 +1330,218 @@
     return (lon, lat, rad)
 
 def to_geodetic(
         x: np.ndarray,
         y: np.ndarray,
         z: np.ndarray,
         a_axis: float = _wgs84.a_axis,
-        flat: float = _wgs84.flat
+        flat: float = _wgs84.flat,
+        method: str = 'bowring',
+        eps: float = np.finfo(np.float64).eps,
+        iterations: int = 10
+    ):
+    """
+    Convert from cartesian coordinates to geodetic coordinates
+    using either iterative or closed-form methods
+
+    Parameters
+    ----------
+    x, float
+        cartesian x-coordinates
+    y, float
+        cartesian y-coordinates
+    z, float
+        cartesian z-coordinates
+    a_axis: float, default 6378137.0
+        semimajor axis of the ellipsoid
+    flat: float, default 1.0/298.257223563
+        ellipsoidal flattening
+    method: str, default 'bowring'
+        method to use for conversion
+
+            - ``'moritz'``: iterative solution
+            - ``'bowring'``: iterative solution
+            - ``'zhu'``: closed-form solution
+    eps: float, default np.finfo(np.float64).eps
+        tolerance for iterative methods
+    iterations: int, default 10
+        maximum number of iterations
+    """
+    # verify axes and copy to not modify inputs
+    x = np.atleast_1d(np.copy(x))
+    y = np.atleast_1d(np.copy(y))
+    z = np.atleast_1d(np.copy(z))
+    # calculate the geodetic coordinates using the specified method
+    if (method.lower() == 'moritz'):
+        return _moritz_iterative(x, y, z, a_axis=a_axis, flat=flat,
+            eps=eps, iterations=iterations)
+    elif (method.lower() == 'bowring'):
+        return _bowring_iterative(x, y, z, a_axis=a_axis, flat=flat,
+            eps=eps, iterations=iterations)
+    elif (method.lower() == 'zhu'):
+        return _zhu_closed_form(x, y, z, a_axis=a_axis, flat=flat)
+    else:
+        raise ValueError(f'Unknown conversion method: {method}')
+
+def _moritz_iterative(
+        x: np.ndarray,
+        y: np.ndarray,
+        z: np.ndarray,
+        a_axis: float = _wgs84.a_axis,
+        flat: float = _wgs84.flat,
+        eps: float = np.finfo(np.float64).eps,
+        iterations: int = 10
+    ):
+    """
+    Convert from cartesian coordinates to geodetic coordinates
+    using the iterative solution of [1]_
+
+    Parameters
+    ----------
+    x, float
+        cartesian x-coordinates
+    y, float
+        cartesian y-coordinates
+    z, float
+        cartesian z-coordinates
+    a_axis: float, default 6378137.0
+        semimajor axis of the ellipsoid
+    flat: float, default 1.0/298.257223563
+        ellipsoidal flattening
+    eps: float, default np.finfo(np.float64).eps
+        tolerance for iterative method
+    iterations: int, default 10
+        maximum number of iterations
+
+    References
+    ----------
+    .. [1] B. Hofmann-Wellenhof and H. Moritz,
+        *Physical Geodesy*, 2nd Edition, 403 pp., (2006).
+        `doi: 10.1007/978-3-211-33545-1
+        <https://doi.org/10.1007/978-3-211-33545-1>`_
+    """
+    # Linear eccentricity and first numerical eccentricity
+    lin_ecc = np.sqrt((2.0*flat - flat**2)*a_axis**2)
+    ecc1 = lin_ecc/a_axis
+    # degrees to radians
+    dtr = np.pi/180.0
+    # calculate longitude
+    lon = np.arctan2(y, x)/dtr
+    # set initial estimate of height to 0
+    h = np.zeros_like(lon)
+    h0 = np.inf*np.ones_like(lon)
+    # calculate radius of parallel
+    p = np.sqrt(x**2 + y**2)
+    # initial estimated value for phi using h=0
+    phi = np.arctan(z/(p*(1.0 - ecc1**2)))
+    # iterate to tolerance or to maximum number of iterations
+    i = 0
+    while np.any(np.abs(h - h0) > eps) and (i <= iterations):
+        # copy previous iteration of height
+        h0 = np.copy(h)
+        # calculate radius of curvature
+        N = a_axis/np.sqrt(1.0 - ecc1**2 * np.sin(phi)**2)
+        # estimate new value of height
+        h = p/np.cos(phi) - N
+        # estimate new value for latitude using heights
+        phi = np.arctan(z/(p*(1.0 - ecc1**2*N/(N + h))))
+        # add to iterator
+        i += 1
+    # return latitude, longitude and height
+    return (lon, phi/dtr, h)
+
+def _bowring_iterative(
+        x: np.ndarray,
+        y: np.ndarray,
+        z: np.ndarray,
+        a_axis: float = _wgs84.a_axis,
+        flat: float = _wgs84.flat,
+        eps: float = np.finfo(np.float64).eps,
+        iterations: int = 10
+    ):
+    """
+    Convert from cartesian coordinates to geodetic coordinates
+    using the iterative solution of [1]_ [2]_
+
+    Parameters
+    ----------
+    x, float
+        cartesian x-coordinates
+    y, float
+        cartesian y-coordinates
+    z, float
+        cartesian z-coordinates
+    a_axis: float, default 6378137.0
+        semimajor axis of the ellipsoid
+    flat: float, default 1.0/298.257223563
+        ellipsoidal flattening
+    eps: float, default np.finfo(np.float64).eps
+        tolerance for iterative method
+    iterations: int, default 10
+        maximum number of iterations
+
+    References
+    ----------
+    .. [1] B. R. Bowring, "Transformation from spatial
+        to geodetic coordinates," *Survey Review*, 23(181),
+        323--327, (1976). `doi: 10.1179/sre.1976.23.181.323
+        <https://doi.org/10.1179/sre.1976.23.181.323>`_
+    .. [2] B. R. Bowring, "The Accuracy Of Geodetic
+        Latitude and Height Equations," *Survey Review*, 28(218),
+        202--206, (1985). `doi: 10.1179/sre.1985.28.218.202
+        <https://doi.org/10.1179/sre.1985.28.218.202>`_
+    """
+    # semiminor axis of the WGS84 ellipsoid [m]
+    b_axis = (1.0 - flat)*a_axis
+    # Linear eccentricity
+    lin_ecc = np.sqrt((2.0*flat - flat**2)*a_axis**2)
+    # square of first and second numerical eccentricity
+    e12 = lin_ecc**2/a_axis**2
+    e22 = lin_ecc**2/b_axis**2
+    # degrees to radians
+    dtr = np.pi/180.0
+    # calculate longitude
+    lon = np.arctan2(y, x)/dtr
+    # calculate radius of parallel
+    p = np.sqrt(x**2 + y**2)
+    # initial estimated value for reduced parametric latitude
+    u = np.arctan(a_axis*z/(b_axis*p))
+    # initial estimated value for latitude
+    phi = np.arctan((z + e22*b_axis*np.sin(u)**3) /
+        (p - e12*a_axis*np.cos(u)**3))
+    phi0 = np.inf*np.ones_like(lon)
+    # iterate to tolerance or to maximum number of iterations
+    i = 0
+    while np.any(np.abs(phi - phi0) > eps) and (i <= iterations):
+        # copy previous iteration of phi
+        phi0 = np.copy(phi)
+        # calculate reduced parametric latitude
+        u = np.arctan(b_axis*np.tan(phi)/a_axis)
+        # estimate new value of latitude
+        phi = np.arctan((z + e22*b_axis*np.sin(u)**3) /
+            (p - e12*a_axis*np.cos(u)**3))
+        # add to iterator
+        i += 1
+    # calculate final radius of curvature
+    N = a_axis/np.sqrt(1.0 - e12 * np.sin(phi)**2)
+    # estimate final height (Bowring, 1985)
+    h = p*np.cos(phi) + z*np.sin(phi) - a_axis**2/N
+    # return latitude, longitude and height
+    return (lon, phi/dtr, h)
+
+def _zhu_closed_form(
+        x: np.ndarray,
+        y: np.ndarray,
+        z: np.ndarray,
+        a_axis: float = _wgs84.a_axis,
+        flat: float = _wgs84.flat,
     ):
     """
     Convert from cartesian coordinates to geodetic coordinates
-    using a closed form solution
+    using the closed-form solution of [1]_
 
     Parameters
     ----------
     x, float
         cartesian x-coordinates
     y, float
         cartesian y-coordinates
@@ -1315,37 +1550,33 @@
     a_axis: float, default 6378137.0
         semimajor axis of the ellipsoid
     flat: float, default 1.0/298.257223563
         ellipsoidal flattening
 
     References
     ----------
-    .. [1] J Zhu "Exact conversion of Earth-centered, Earth-fixed
-        coordinates to geodetic coordinates,"
+    .. [1] J. Zhu, "Exact conversion of Earth-centered,
+        Earth-fixed coordinates to geodetic coordinates,"
         *Journal of Guidance, Control, and Dynamics*,
         16(2), 389--391, (1993). `doi: 10.2514/3.21016
         <https://arc.aiaa.org/doi/abs/10.2514/3.21016>`_
     """
-    # verify axes and copy to not modify inputs
-    x = np.atleast_1d(np.copy(x))
-    y = np.atleast_1d(np.copy(y))
-    z = np.atleast_1d(np.copy(z))
     # semiminor axis of the WGS84 ellipsoid [m]
     b_axis = (1.0 - flat)*a_axis
-    # Linear eccentricity and first numerical eccentricity
+    # Linear eccentricity
     lin_ecc = np.sqrt((2.0*flat - flat**2)*a_axis**2)
-    ecc1 = lin_ecc/a_axis
     # square of first numerical eccentricity
-    e12 = ecc1**2
+    e12 = lin_ecc**2/a_axis**2
     # degrees to radians
     dtr = np.pi/180.0
-    # calculate distance
-    w = np.sqrt(x**2 + y**2)
     # calculate longitude
-    lon = np.arctan2(y,x)/dtr
+    lon = np.arctan2(y, x)/dtr
+    # calculate radius of parallel
+    w = np.sqrt(x**2 + y**2)
+    # allocate for output latitude and height
     lat = np.zeros_like(lon)
     h = np.zeros_like(lon)
     if np.any(w == 0):
         # special case where w == 0 (exact polar solution)
         ind, = np.nonzero(w == 0)
         h[ind] = np.sign(z[ind])*z[ind] - b_axis
         lat[ind] = 90.0*np.sign(z[ind])
@@ -1373,15 +1604,15 @@
 def scale_areas(
         lat: np.ndarray,
         flat: float=_wgs84.flat,
         ref: float=70.0
     ):
     """
     Calculates area scaling factors for a polar stereographic projection
-    including special case of at the exact pole
+    including special case of at the exact pole [1]_ [2]_
 
     Parameters
     ----------
     lat: np.ndarray
         latitude (degrees north)
     flat: float, default 1.0/298.257223563
         ellipsoidal flattening
@@ -1391,15 +1622,15 @@
     Returns
     -------
     scale: np.ndarray
         area scaling factors at input latitudes
 
     References
     ----------
-    .. [1] J P Snyder, *Map Projections used by the U.S. Geological Survey*,
+    .. [1] J. P. Snyder, *Map Projections used by the U.S. Geological Survey*,
         Geological Survey Bulletin 1532, U.S. Government Printing Office, (1982).
     .. [2] JPL Technical Memorandum 3349-85-101
     """
     # convert latitude from degrees to positive radians
     theta = np.abs(lat)*np.pi/180.0
     # convert reference latitude from degrees to positive radians
     theta_ref = np.abs(ref)*np.pi/180.0
@@ -1416,9 +1647,9 @@
     mref = np.cos(theta_ref)/np.sqrt(1.0 - ecc2*np.sin(theta_ref)**2)
     tref = np.tan(np.pi/4.0 - theta_ref/2.0)/((1.0 - ecc*np.sin(theta_ref)) / \
         (1.0 + ecc*np.sin(theta_ref)))**(ecc/2.0)
     # distance scaling
     k = (mref/m)*(t/tref)
     kp = 0.5*mref*np.sqrt(((1.0+ecc)**(1.0+ecc))*((1.0-ecc)**(1.0-ecc)))/tref
     # area scaling
-    scale = np.where(np.isclose(theta,np.pi/2.0),1.0/(kp**2),1.0/(k**2))
+    scale = np.where(np.isclose(theta, np.pi/2.0), 1.0/(kp**2), 1.0/(k**2))
     return scale
```

### Comparing `pyTMD-2.0.3/pyTMD/tidal_ellipse.py` & `pyTMD-2.0.4/pyTMD/tidal_ellipse.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from __future__ import annotations
 
 import numpy as np
 
 def tidal_ellipse(u: np.ndarray, v: np.ndarray):
     """
     Expresses the amplitudes and phases for the u and v components in terms of
-    four ellipse parameters using Foreman's formula
+    four ellipse parameters using Foreman's formula [1]_
 
     Parameters
     ----------
     u: np.ndarray
         zonal current (EW)
     v: np.ndarray
         meridional current (NS)
@@ -54,17 +54,17 @@
         angle of inclination of the northern semimajor semi-axis
     uphase: float
         phase lag of the maximum current behind the maximum tidal potential
         of the individual constituent
 
     References
     ----------
-    .. [1] Foreman and Henry, "The harmonic analysis of tidal model time
-        series", *Advances in Water Resources*, 12(3), 109-120, (1989).
-        `doi: 10.1016/0309-1708(89)90017-1
+    .. [1] M. G. G. Foreman and R. F. Henry, "The harmonic analysis of tidal
+        model time series," *Advances in Water Resources*, 12(3), 109--120,
+        (1989). `doi: 10.1016/0309-1708(89)90017-1
         <https://doi.org/10.1016/0309-1708(89)90017-1>`_
     """
     # change to polar coordinates
     t1p = u.real - v.imag
     t2p = v.real + u.imag
     t1m = u.real + v.imag
     t2m = v.real - u.imag
```

### Comparing `pyTMD-2.0.3/pyTMD/tools.py` & `pyTMD-2.0.4/pyTMD/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 tools.py
-Written by Tyler Sutterley (01/2023)
+Written by Tyler Sutterley (04/2023)
 Jupyter notebook, user interface and plotting tools
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
     ipywidgets: interactive HTML widgets for Jupyter notebooks and IPython
@@ -13,27 +13,28 @@
     ipyleaflet: Jupyter / Leaflet bridge enabling interactive maps
         https://github.com/jupyter-widgets/ipyleaflet
     matplotlib: Python 2D plotting library
         http://matplotlib.org/
         https://github.com/matplotlib/matplotlib
 
 UPDATE HISTORY:
+    Updated 04/2023: using pathlib to define and expand paths
     Updated 01/2023: use debug level logging instead of import warnings
     Updated 11/2022: place more imports within try/except statements
     Updated 08/2022: place some imports behind try/except statements
     Updated 05/2022: include world copy jump in webmercator maps
     Updated 03/2022: add marker relocation routines from notebooks
     Updated 02/2022: add leaflet map projections
     Written 09/2021
 """
 import io
-import os
 import copy
 import base64
 import logging
+import pathlib
 import datetime
 import numpy as np
 import matplotlib
 matplotlib.rcParams['axes.linewidth'] = 2.0
 matplotlib.rcParams["animation.html"] = "jshtml"
 import matplotlib.cm as cm
 import matplotlib.colorbar
@@ -65,15 +66,15 @@
         # set default keyword options
         kwargs.setdefault('style', {})
         # set style
         self.style = copy.copy(kwargs['style'])
 
         # set the directory with tide models
         self.directory = ipywidgets.Text(
-            value=os.getcwd(),
+            value=pathlib.Path.cwd(),
             description='Directory:',
             disabled=False
         )
 
         # dropdown menu for setting tide model
         model_list = sorted(pyTMD.io.model.ocean_elevation() +
             pyTMD.io.model.load_elevation())
```

### Comparing `pyTMD-2.0.3/pyTMD/utilities.py` & `pyTMD-2.0.4/pyTMD/utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 #!/usr/bin/env python
 u"""
 utilities.py
-Written by Tyler Sutterley (03/2023)
+Written by Tyler Sutterley (05/2023)
 Download and management utilities for syncing time and auxiliary files
 
 PYTHON DEPENDENCIES:
     lxml: processing XML and HTML in Python
         https://pypi.python.org/pypi/lxml
 
 UPDATE HISTORY:
+    Updated 05/2023: add reify decorator for evaluation of properties
+    Updated 04/2023: using pathlib to define and expand paths
+        added function to download ephemeride files from JPL SSD server
     Updated 03/2023: add basic variable typing to function inputs
     Updated 01/2023: updated SSL context to fix some deprecation warnings
     Updated 11/2022: added list program for IERS Bulletin-A https server
         use f-strings for formatting verbose or ascii output
     Updated 04/2022: updated docstrings to numpy documentation format
     Updated 10/2021: build python logging instance for handling verbose output
     Updated 09/2021: added generic list from Apache http server
@@ -30,26 +33,26 @@
         generalize build opener function for different Earthdata instances
     Updated 08/2020: add GSFC CDDIS opener, login and download functions
     Written 08/2020
 """
 from __future__ import print_function, division, annotations
 
 import sys
-import os
 import re
 import io
 import ssl
 import netrc
 import ftplib
 import shutil
 import base64
 import socket
 import inspect
 import hashlib
 import logging
+import pathlib
 import warnings
 import posixpath
 import subprocess
 import lxml.etree
 import calendar, time
 import dateutil.parser
 if sys.version_info[0] == 2:
@@ -58,48 +61,64 @@
     import urllib2
 else:
     from urllib.parse import quote_plus
     from http.cookiejar import CookieJar
     import urllib.request as urllib2
 
 # PURPOSE: get absolute path within a package from a relative path
-def get_data_path(relpath: list | str):
+def get_data_path(relpath: list | str | pathlib.Path):
     """
     Get the absolute path within a package from a relative path
 
     Parameters
     ----------
     relpath: list or str
         relative path
     """
     # current file path
     filename = inspect.getframeinfo(inspect.currentframe()).filename
-    filepath = os.path.dirname(os.path.abspath(filename))
+    filepath = pathlib.Path(filename).absolute().parent
     if isinstance(relpath, list):
         # use *splat operator to extract from list
-        return os.path.join(filepath,*relpath)
+        return filepath.joinpath(*relpath)
     elif isinstance(relpath, str):
-        return os.path.join(filepath,relpath)
+        return filepath.joinpath(relpath)
+
+class reify(object):
+    """Class decorator that puts the result of the method it
+    decorates into the instance"""
+    def __init__(self, wrapped):
+        self.wrapped = wrapped
+        self.__name__ = wrapped.__name__
+        self.__doc__ = wrapped.__doc__
+
+    def __get__(self, inst, objtype=None):
+        if inst is None:
+            return self
+        val = self.wrapped(inst)
+        setattr(inst, self.wrapped.__name__, val)
+        return val
 
 # PURPOSE: platform independent file opener
-def file_opener(filename: str):
+def file_opener(filename: str | pathlib.Path):
     """
     Platform independent file opener
 
     Parameters
     ----------
     filename: str
         path to file
     """
+    filename = pathlib.Path(filename).expanduser()
     if (sys.platform == "win32"):
-        os.startfile(os.path.expanduser(filename), "explore")
+        pathlib.os.startfile(filename, "explore")
     elif (sys.platform == "darwin"):
-        subprocess.call(["open", os.path.expanduser(filename)])
+        subprocess.call(["open", filename])
     else:
-        subprocess.call(["xdg-open", os.path.expanduser(filename)])
+        subprocess.call(["xdg-open", filename])
 
 # PURPOSE: get the hash value of a file
 def get_hash(
         local: str | io.IOBase,
         algorithm: str = 'MD5'
     ):
     """
@@ -117,18 +136,22 @@
     """
     # check if open file object or if local file exists
     if isinstance(local, io.IOBase):
         if (algorithm == 'MD5'):
             return hashlib.md5(local.getvalue()).hexdigest()
         elif (algorithm == 'sha1'):
             return hashlib.sha1(local.getvalue()).hexdigest()
-    elif os.access(os.path.expanduser(local),os.F_OK):
+    elif isinstance(local, (str, pathlib.Path)):
         # generate checksum hash for local file
+        local = pathlib.Path(local).expanduser()
+        # if file currently doesn't exist, return empty string
+        if not local.exists():
+            return ''
         # open the local_file in binary read mode
-        with open(os.path.expanduser(local), 'rb') as local_buffer:
+        with local.open(mode='rb') as local_buffer:
             # generate checksum hash for a given type
             if (algorithm == 'MD5'):
                 return hashlib.md5(local_buffer.read()).hexdigest()
             elif (algorithm == 'sha1'):
                 return hashlib.sha1(local_buffer.read()).hexdigest()
     else:
         return ''
@@ -146,32 +169,32 @@
     refname: str, default HEAD
         Symbolic reference name
     short: bool, default False
         Return the shorted hash value
     """
     # get path to .git directory from current file path
     filename = inspect.getframeinfo(inspect.currentframe()).filename
-    basepath = os.path.dirname(os.path.dirname(os.path.abspath(filename)))
-    gitpath = os.path.join(basepath,'.git')
+    basepath = pathlib.Path(filename).absolute().parent.parent
+    gitpath = basepath.joinpath('.git')
     # build command
     cmd = ['git', f'--git-dir={gitpath}', 'rev-parse']
     cmd.append('--short') if short else None
     cmd.append(refname)
     # get output
     with warnings.catch_warnings():
         return str(subprocess.check_output(cmd), encoding='utf8').strip()
 
 # PURPOSE: get the current git status
 def get_git_status():
     """Get the status of a ``git`` repository as a boolean value
     """
     # get path to .git directory from current file path
     filename = inspect.getframeinfo(inspect.currentframe()).filename
-    basepath = os.path.dirname(os.path.dirname(os.path.abspath(filename)))
-    gitpath = os.path.join(basepath,'.git')
+    basepath = pathlib.Path(filename).absolute().parent.parent
+    gitpath = basepath.joinpath('.git')
     # build command
     cmd = ['git', f'--git-dir={gitpath}', 'status', '--porcelain']
     with warnings.catch_warnings():
         return bool(subprocess.check_output(cmd))
 
 # PURPOSE: recursively split a url path
 def url_split(s: str):
@@ -353,22 +376,23 @@
     source: str
         source file
     destination: str
         copied destination file
     move: bool, default False
         remove the source file
     """
-    source = os.path.abspath(os.path.expanduser(source))
-    destination = os.path.abspath(os.path.expanduser(destination))
+    source = pathlib.Path(source).expanduser().absolute()
+    destination = pathlib.Path(destination).expanduser().absolute()
     # log source and destination
-    logging.info(f'{source} -->\n\t{destination}')
+    logging.info(f'{str(source)} -->\n\t{str(destination)}')
     shutil.copyfile(source, destination)
     shutil.copystat(source, destination)
+    # remove the original file if moving
     if move:
-        os.remove(source)
+        source.unlink()
 
 # PURPOSE: check ftp connection
 def check_ftp_connection(
         HOST: str,
         username: str | None = None,
         password: str | None = None
     ):
@@ -480,15 +504,15 @@
 
 # PURPOSE: download a file from a ftp host
 def from_ftp(
         HOST: str,
         username: str | None = None,
         password: str | None = None,
         timeout: int | None = None,
-        local: str | None = None,
+        local: str | pathlib.Path | None = None,
         hash: str = '',
         chunk: int = 8192,
         verbose: bool = False,
         fid=sys.stdout,
         mode: oct = 0o775
     ):
     """
@@ -500,15 +524,15 @@
         remote ftp host path
     username: str or NoneType
         ftp username
     password: str or NoneType
         ftp password
     timeout: int or NoneType, default None
         timeout in seconds for blocking operations
-    local: str or NoneType, default None
+    local: str, pathlib.Path or NoneType, default None
         path to local file
     hash: str, default ''
         MD5 hash of local file
     chunk: int, default 8192
         chunk size for transfer encoding
     verbose: bool, default False
         print file transfer information
@@ -549,29 +573,28 @@
         remote_hash = hashlib.md5(remote_buffer.getvalue()).hexdigest()
         # get last modified date of remote file and convert into unix time
         mdtm = ftp.sendcmd(f'MDTM {ftp_remote_path}')
         remote_mtime = get_unix_time(mdtm[4:], format="%Y%m%d%H%M%S")
         # compare checksums
         if local and (hash != remote_hash):
             # convert to absolute path
-            local = os.path.abspath(local)
+            local = pathlib.Path(local).expanduser().absolute()
             # create directory if non-existent
-            if not os.access(os.path.dirname(local), os.F_OK):
-                os.makedirs(os.path.dirname(local), mode)
+            local.parent.mkdir(mode=mode, parents=True, exist_ok=True)
             # print file information
-            args = (posixpath.join(*HOST),local)
+            args = (posixpath.join(*HOST), str(local))
             logging.info('{0} -->\n\t{1}'.format(*args))
             # store bytes to file using chunked transfer encoding
             remote_buffer.seek(0)
-            with open(os.path.expanduser(local), 'wb') as f:
+            with local.open(mode='wb') as f:
                 shutil.copyfileobj(remote_buffer, f, chunk)
             # change the permissions mode
-            os.chmod(local,mode)
+            local.chmod(mode)
             # keep remote modification time of file and local access time
-            os.utime(local, (os.stat(local).st_atime, remote_mtime))
+            pathlib.os.utime(local, (local.stat().st_atime, remote_mtime))
         # close the ftp connection
         ftp.close()
         # return the bytesIO object
         remote_buffer.seek(0)
         return remote_buffer
 
 # default ssl context
@@ -667,15 +690,15 @@
         return (colnames, collastmod)
 
 # PURPOSE: download a file from a http host
 def from_http(
         HOST: str,
         timeout: int | None = None,
         context = _default_ssl_context,
-        local: str | None = None,
+        local: str | pathlib.path | None = None,
         hash: str = '',
         chunk: int = 16384,
         verbose: bool = False,
         fid = sys.stdout,
         mode: oct = 0o775
     ):
     """
@@ -685,15 +708,15 @@
     ----------
     HOST: str or list
         remote http host path split as list
     timeout: int or NoneType, default None
         timeout in seconds for blocking operations
     context: obj, default ssl.SSLContext(ssl.PROTOCOL_TLS)
         SSL context for ``urllib`` opener object
-    local: str or NoneType, default None
+    local: str, pathlib.Path or NoneType, default None
         path to local file
     hash: str, default ''
         MD5 hash of local file
     chunk: int, default 16384
         chunk size for transfer encoding
     verbose: bool, default False
         print file transfer information
@@ -728,27 +751,26 @@
         # save file basename with bytesIO object
         remote_buffer.filename = HOST[-1]
         # generate checksum hash for remote file
         remote_hash = hashlib.md5(remote_buffer.getvalue()).hexdigest()
         # compare checksums
         if local and (hash != remote_hash):
             # convert to absolute path
-            local = os.path.abspath(local)
+            local = pathlib.Path(local).expanduser().absolute()
             # create directory if non-existent
-            if not os.access(os.path.dirname(local), os.F_OK):
-                os.makedirs(os.path.dirname(local), mode)
+            local.parent.mkdir(mode=mode, parents=True, exist_ok=True)
             # print file information
-            args = (posixpath.join(*HOST),local)
+            args = (posixpath.join(*HOST), str(local))
             logging.info('{0} -->\n\t{1}'.format(*args))
             # store bytes to file using chunked transfer encoding
             remote_buffer.seek(0)
-            with open(os.path.expanduser(local), 'wb') as f:
+            with local.open(mode='wb') as f:
                 shutil.copyfileobj(remote_buffer, f, chunk)
             # change the permissions mode
-            os.chmod(local,mode)
+            local.chmod(mode)
         # return the bytesIO object
         remote_buffer.seek(0)
         return remote_buffer
 
 # PURPOSE: "login" to NASA Earthdata with supplied credentials
 def build_opener(
         username: str,
@@ -804,15 +826,15 @@
         handler.append(urllib2.HTTPRedirectHandler())
     # create "opener" (OpenerDirector instance)
     opener = urllib2.build_opener(*handler)
     # Encode username/password for request authorization headers
     # add Authorization header to opener
     if authorization_header:
         b64 = base64.b64encode(f'{username}:{password}'.encode())
-        opener.addheaders = [("Authorization","Basic {0}".format(b64.decode()))]
+        opener.addheaders = [("Authorization", f"Basic {b64.decode()}")]
     # Now all calls to urllib2.urlopen use our opener.
     urllib2.install_opener(opener)
     # All calls to urllib2.urlopen will now use handler
     # Make sure not to include the protocol in with the URL, or
     # HTTPPasswordMgrWithDefaultRealm will be confused.
     return opener
 
@@ -882,16 +904,16 @@
         build_opener(username, password)
         # check credentials
         check_credentials()
     # verify inputs for remote https host
     if isinstance(HOST, str):
         HOST = url_split(HOST)
     # Encode username/password for request authorization headers
-    base64_string = base64.b64encode(f'{username}:{password}'.encode())
-    authorization_header = "Basic {0}".format(base64_string.decode())
+    b64 = base64.b64encode(f'{username}:{password}'.encode())
+    authorization_header = f"Basic {b64.decode()}"
     # try listing from https
     try:
         # Create and submit request.
         request = urllib2.Request(posixpath.join(*HOST))
         request.add_header("Authorization", authorization_header)
         tree = lxml.etree.parse(urllib2.urlopen(request, timeout=timeout), parser)
     except:
@@ -924,15 +946,15 @@
 # PURPOSE: download a file from a GSFC CDDIS https server
 def from_cddis(
         HOST: str,
         username: str | None = None,
         password: str | None = None,
         build: bool = True,
         timeout: int | None = None,
-        local: str | None = None,
+        local: str | pathlib.Path | None = None,
         hash: str = '',
         chunk: int = 16384,
         verbose: bool = False,
         fid=sys.stdout,
         mode: oct = 0o775
     ):
     """
@@ -946,15 +968,15 @@
         NASA Earthdata username
     password: str or NoneType, default None
         NASA Earthdata password
     build: bool, default True
         Build opener and check Earthdata credentials
     timeout: int or NoneType, default None
         timeout in seconds for blocking operations
-    local: str or NoneType, default None
+    local: str, pathlib.Path or NoneType, default None
         path to local file
     hash: str, default ''
         MD5 hash of local file
     chunk: int, default 16384
         chunk size for transfer encoding
     verbose: bool, default False
         print file transfer information
@@ -981,16 +1003,16 @@
         build_opener(username, password)
         # check credentials
         check_credentials()
     # verify inputs for remote https host
     if isinstance(HOST, str):
         HOST = url_split(HOST)
     # Encode username/password for request authorization headers
-    base64_string = base64.b64encode(f'{username}:{password}'.encode())
-    authorization_header = "Basic {0}".format(base64_string.decode())
+    b64 = base64.b64encode(f'{username}:{password}'.encode())
+    authorization_header = f"Basic {b64.decode()}"
     # try downloading from https
     try:
         # Create and submit request.
         request = urllib2.Request(posixpath.join(*HOST))
         request.add_header("Authorization", authorization_header)
         response = urllib2.urlopen(request, timeout=timeout)
     except:
@@ -1003,27 +1025,26 @@
         # save file basename with bytesIO object
         remote_buffer.filename = HOST[-1]
         # generate checksum hash for remote file
         remote_hash = hashlib.md5(remote_buffer.getvalue()).hexdigest()
         # compare checksums
         if local and (hash != remote_hash):
             # convert to absolute path
-            local = os.path.abspath(local)
+            local = pathlib.Path(local).expanduser().absolute()
             # create directory if non-existent
-            if not os.access(os.path.dirname(local), os.F_OK):
-                os.makedirs(os.path.dirname(local), mode)
+            local.parent.mkdir(mode=mode, parents=True, exist_ok=True)
             # print file information
-            args = (posixpath.join(*HOST),local)
+            args = (posixpath.join(*HOST), str(local))
             logging.info('{0} -->\n\t{1}'.format(*args))
             # store bytes to file using chunked transfer encoding
             remote_buffer.seek(0)
-            with open(os.path.expanduser(local), 'wb') as f:
+            with local.open(mode='wb') as f:
                 shutil.copyfileobj(remote_buffer, f, chunk)
             # change the permissions mode
-            os.chmod(local,mode)
+            local.chmod(mode)
         # return the bytesIO object
         remote_buffer.seek(0)
         return remote_buffer
 
 # PURPOSE: list a directory on IERS https Server
 def iers_list(
         HOST: str,
@@ -1068,7 +1089,47 @@
         colnames = tree.xpath('//tr/td[@class="$tdclass"][4]//a/@href')
         # get the Unix timestamp value for a modification time
         collastmod = [get_unix_time(i,format='%Y-%m-%d')
             for i in tree.xpath('//tr/td[@class="$tdclass"][2]/span/text()')]
         # sort list of column names and last modified times in reverse order
         # return the list of column names and last modified times
         return (colnames[::-1], collastmod[::-1])
+
+def from_jpl_ssd(
+        kernel='de440s.bsp',
+        timeout: int | None = None,
+        context = _default_ssl_context,
+        hash: str = '',
+        chunk: int = 16384,
+        verbose: bool = False,
+        mode: oct = 0o775
+    ):
+    """
+    Download `planetary ephemeride kernels`__ from the JPL Solar
+    System Dynamics server
+
+    .. __: https://ssd.jpl.nasa.gov/planets/eph_export.html
+
+    Parameters
+    ----------
+    kernel: str
+        JPL kernel file to download
+    timeout: int or NoneType, default None
+        timeout in seconds for blocking operations
+    context: obj, default ssl.SSLContext(ssl.PROTOCOL_TLS)
+        SSL context for ``urllib`` opener object
+    hash: str, default ''
+        MD5 hash of local file
+    chunk: int, default 16384
+        chunk size for transfer encoding
+    verbose: bool, default False
+        print file transfer information
+    mode: oct, default 0o775
+        permissions mode of output local file
+    """
+    # local path to kernel file
+    local = get_data_path(['data',kernel])
+    # remote host path to kernel file
+    HOST = ['https://ssd.jpl.nasa.gov','ftp','eph','planets','bsp',kernel]
+    # get kernel file from remote host
+    from_http(HOST, timeout=timeout, context=context, local=local,
+        hash=hash, chunk=chunk, verbose=verbose, mode=mode)
```

### Comparing `pyTMD-2.0.3/pyTMD.egg-info/PKG-INFO` & `pyTMD-2.0.4/pyTMD.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTMD
-Version: 2.0.3
+Version: 2.0.4
 Summary: Tide Model Driver to read OTIS, GOT and FES formatted tidal solutions and make tidal predictions
 Home-page: https://github.com/tsutterley/pyTMD
 Author: Tyler Sutterley
 Author-email: tsutterl@uw.edu
 License: MIT
 Keywords: Ocean Tides,Load Tides,Pole Tides,Tidal Prediction,OTIS,GOT,FES
 Classifier: Development Status :: 3 - Alpha
@@ -26,16 +26,14 @@
 
 |Language|
 |License|
 |PyPI Version|
 |Anaconda-Server|
 |Documentation Status|
 |codecov|
-|Binder|
-|Pangeo|
 |zenodo|
 
 .. |Language| image:: https://img.shields.io/pypi/pyversions/pyTMD?color=green
    :target: https://www.python.org/
 
 .. |License| image:: https://img.shields.io/github/license/tsutterley/pyTMD
    :target: https://github.com/tsutterley/pyTMD/blob/main/LICENSE
@@ -48,23 +46,16 @@
 
 .. |Documentation Status| image:: https://readthedocs.org/projects/pytmd/badge/?version=latest
    :target: https://pytmd.readthedocs.io/en/latest/?badge=latest
 
 .. |codecov| image:: https://codecov.io/gh/tsutterley/pyTMD/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/tsutterley/pyTMD
 
-.. |Binder| image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/tsutterley/pyTMD/main
-
-.. |Pangeo| image:: https://img.shields.io/static/v1.svg?logo=Jupyter&label=PangeoBinderAWS&message=us-west-2&color=orange
-   :target: https://aws-uswest2-binder.pangeo.io/v2/gh/tsutterley/pyTMD/main?urlpath=lab
-
-.. |zenodo| image:: https://zenodo.org/badge/107997403.svg
-   :target: https://zenodo.org/badge/latestdoi/107997403
-
+.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5555395.svg
+   :target: https://doi.org/10.5281/zenodo.5555395
 
 Python-based tidal prediction software for estimating ocean, load, solid Earth and pole tides
 
 Ocean and load tidal predictions using OTIS, GOT and FES formatted tidal solutions
 
 - `OSU Tidal Prediction Software (OTPS) <https://www.tpxo.net/otps>`_
 - `ESR Tide Model Driver (TMD) Matlab Toolbox <https://www.esr.org/research/polar-tide-models/tmd-software/>`_
@@ -83,39 +74,32 @@
 - `IERS Daily Earth Orientation Parameters (EOP) from USNO <http://www.usno.navy.mil/USNO/earth-orientation/eo-products/weekly>`_
 - `IERS Daily Earth Orientation Parameters (EOP) from NASA CDDIS <ftp://cddis.nasa.gov/products/iers/finals.all>`_
 - `IERS Ocean Pole Load Tide Coefficients Map <http://maia.usno.navy.mil/conventions/2010/2010_update/chapter7/additional_info/opoleloadcoefcmcor.txt.gz>`_
 
 Dependencies
 ############
 
-- `cartopy: Python package designed for geospatial data processing <https://scitools.org.uk/cartopy/docs/latest/>`_
 - `dateutil: powerful extensions to datetime <https://dateutil.readthedocs.io/en/stable/>`_
-- `gdal: Pythonic interface to the Geospatial Data Abstraction Library (GDAL) <https://pypi.python.org/pypi/GDAL>`_
-- `h5py: Python interface for Hierarchal Data Format 5 (HDF5) <https://www.h5py.org/>`_
-- `ipyleaflet: Jupyter / Leaflet bridge enabling interactive maps <https://github.com/jupyter-widgets/ipyleaflet>`_
-- `ipywidgets: interactive HTML widgets for Jupyter notebooks and IPython <https://ipywidgets.readthedocs.io/en/latest/>`_
 - `lxml: processing XML and HTML in Python <https://pypi.python.org/pypi/lxml>`_
-- `matplotlib: Python 2D plotting library <https://matplotlib.org/>`_
 - `netCDF4: Python interface to the netCDF C library <https://unidata.github.io/netcdf4-python/>`_
 - `numpy: Scientific Computing Tools For Python <https://www.numpy.org>`_
 - `pyproj: Python interface to PROJ library <https://pypi.org/project/pyproj/>`_
-- `PyYAML: YAML parser and emitter for Python <https://github.com/yaml/pyyaml>`_
 - `scipy: Scientific Tools for Python <https://www.scipy.org/>`_
 - `setuptools_scm: manager for python package versions using scm metadata <https://pypi.org/project/setuptools-scm/1.9.0/>`_
 
 References
 ##########
 
     T. C. Sutterley, T. Markus, T. A. Neumann, M. R. van den Broeke, J. M. van Wessem, and S. R. M. Ligtenberg,
     "Antarctic ice shelf thickness change from multimission lidar mapping", *The Cryosphere*,
-    13, 1801-1817, (2019). `doi:tc-13-1801-2019 <https://doi.org/10.5194/tc-13-1801-2019>`_
+    13, 1801-1817, (2019). `doi: 10.5194/tc-13-1801-2019 <https://doi.org/10.5194/tc-13-1801-2019>`_
 
     L. Padman, M. R. Siegfried, H. A. Fricker,
     "Ocean Tide Influences on the Antarctic and Greenland Ice Sheets", *Reviews of Geophysics*,
-    56, 142-184, (2018). `doi:10.1002/2016RG000546 <https://doi.org/10.1002/2016RG000546>`_
+    56, 142-184, (2018). `doi: 10.1002/2016RG000546 <https://doi.org/10.1002/2016RG000546>`_
 
 Download
 ########
 
 | The program homepage is:
 | https://github.com/tsutterley/pyTMD
 | A zip archive of the latest version is available directly at:
```

### Comparing `pyTMD-2.0.3/pyTMD.egg-info/SOURCES.txt` & `pyTMD-2.0.4/pyTMD.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 .dockerignore
 .gitignore
+CODE_OF_CONDUCT.rst
 CONTRIBUTORS.rst
 LICENSE
 MANIFEST.in
 README.rst
 postBuild
 requirements-dev.txt
 requirements.txt
 setup.py
 version.txt
 pyTMD/__init__.py
+pyTMD/arguments.py
 pyTMD/astro.py
 pyTMD/calc_astrol_longitudes.py
 pyTMD/check_tide_points.py
 pyTMD/compute_tide_corrections.py
 pyTMD/constants.py
 pyTMD/convert_crs.py
 pyTMD/convert_ll_xy.py
@@ -38,14 +40,17 @@
 pyTMD/data/historic_deltat.data
 pyTMD/data/iers_deltat.data
 pyTMD/data/leap-seconds.list
 pyTMD/data/mean-pole.tab
 pyTMD/data/merged_deltat.data
 pyTMD/data/opoleloadcoefcmcor.txt.gz
 pyTMD/data/ser7.dat
+pyTMD/data/tab5.2e.txt
+pyTMD/data/tab5.3a.txt
+pyTMD/data/tab5.3b.txt
 pyTMD/io/ATLAS.py
 pyTMD/io/FES.py
 pyTMD/io/GOT.py
 pyTMD/io/OTIS.py
 pyTMD/io/__init__.py
 pyTMD/io/constituents.py
 pyTMD/io/model.py
```

### Comparing `pyTMD-2.0.3/scripts/arcticdata_tides.py` & `pyTMD-2.0.4/scripts/arcticdata_tides.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 arcticdata_tides.py
-Written by Tyler Sutterley (11/2022)
+Written by Tyler Sutterley (04/2023)
 Download Arctic Ocean Tide Models from the NSF ArcticData archive
 
 AODTM-5: https://arcticdata.io/catalog/view/doi:10.18739/A2901ZG3N
 AOTIM-5: https://arcticdata.io/catalog/view/doi:10.18739/A2S17SS80
 AOTIM-5-2018: https://arcticdata.io/catalog/view/doi:10.18739/A21R6N14K
 Arc2kmTM: https://arcticdata.io/catalog/view/doi:10.18739/A2D21RK6K
 Gr1kmTM: https://arcticdata.io/catalog/view/doi:10.18739/A2B853K18
@@ -28,34 +28,37 @@
     future: Compatibility layer between Python 2 and Python 3
         https://python-future.org/
 
 PROGRAM DEPENDENCIES:
     utilities.py: download and management utilities for syncing files
 
 UPDATE HISTORY:
+    Updated 04/2023: using pathlib to define and expand paths
     Updated 11/2022: use f-strings for formatting verbose or ascii output
     Updated 06/2022: added Greenland 1km model (Gr1kmTM) to list of models
     Updated 04/2022: use argparse descriptions within documentation
     Updated 10/2021: using python logging for handling verbose output
     Updated 07/2021: can use prefix files to define command line arguments
     Updated 10/2020: using argparse to set command line parameters
     Written 08/2020
 """
-from __future__ import print_function
+from __future__ import print_function, annotations
 
-import os
 import re
 import logging
+import pathlib
 import zipfile
 import argparse
 import posixpath
 import pyTMD.utilities
 
 # PURPOSE: Download Arctic Ocean Tide Models from the NSF ArcticData archive
-def arcticdata_tides(MODEL, DIRECTORY=None, MODE=0o775):
+def arcticdata_tides(MODEL: str,
+    DIRECTORY: str | pathlib.Path | None = None,
+    MODE: oct = 0o775):
 
     # create logger for verbosity level
     logger = pyTMD.utilities.build_logger(__name__,level=logging.INFO)
 
     # digital object identifier (doi) for each Arctic tide model
     DOI = {}
     DOI['AODTM-5'] = '10.18739/A2901ZG3N'
@@ -68,38 +71,39 @@
     LOCAL['AODTM-5'] = 'aodtm5_tmd'
     LOCAL['AOTIM-5'] = 'aotim5_tmd'
     LOCAL['AOTIM-5-2018'] = 'Arc5km2018'
     LOCAL['Arc2kmTM'] = 'Arc2kmTM'
     LOCAL['Gr1kmTM'] = 'Gr1kmTM'
 
     # recursively create directories if non-existent
-    if not os.access(os.path.join(DIRECTORY,LOCAL[MODEL]), os.F_OK):
-        os.makedirs(os.path.join(DIRECTORY,LOCAL[MODEL]), MODE)
+    DIRECTORY = pathlib.Path(DIRECTORY).expanduser().absolute()
+    local_dir = DIRECTORY.joinpath(LOCAL[MODEL])
+    local_dir.mkdir(MODE, parents=True, exist_ok=True)
 
     # build host url for model
     resource_map_doi = f'resource_map_doi:{DOI[MODEL]}'
     HOST = ['https://arcticdata.io','metacat','d1','mn','v2','packages',
         pyTMD.utilities.quote_plus(posixpath.join('application','bagit-097')),
         pyTMD.utilities.quote_plus(resource_map_doi)]
     # download zipfile from host
-    logger.info('{0} -->\n'.format(posixpath.join(*HOST)))
+    logger.info(f'{posixpath.join(*HOST)} -->\n')
     zfile = zipfile.ZipFile(pyTMD.utilities.from_http(HOST))
     # find model files within zip file
-    rx = re.compile('(grid|h[0]?|UV[0]?|Model|xy)_(.*?)',re.VERBOSE)
+    rx = re.compile(r'(grid|h[0]?|UV[0]?|Model|xy)_(.*?)',re.VERBOSE)
     members = [m for m in zfile.filelist if rx.search(m.filename)]
     # extract each member
     for m in members:
         # strip directories from member filename
         m.filename = posixpath.basename(m.filename)
-        local_file = os.path.join(DIRECTORY,LOCAL[MODEL],m.filename)
-        logger.info(local_file)
+        local_file = local_dir.joinpath(m.filename)
+        logger.info(str(local_file))
         # extract file
-        zfile.extract(m, path=os.path.join(DIRECTORY,LOCAL[MODEL]))
+        zfile.extract(m, path=local_dir)
         # change permissions mode
-        os.chmod(local_file, MODE)
+        local_file.chmod(MODE)
     # close the zipfile object
     zfile.close()
 
 # PURPOSE: create argument parser
 def arguments():
     parser = argparse.ArgumentParser(
         description="""Download Arctic Ocean Tide Models from the NSF ArcticData
@@ -107,16 +111,15 @@
             """,
         fromfile_prefix_chars="@"
     )
     parser.convert_arg_line_to_args = pyTMD.utilities.convert_arg_line_to_args
     # command line parameters
     # working data directory for location of tide models
     parser.add_argument('--directory','-D',
-        type=lambda p: os.path.abspath(os.path.expanduser(p)),
-        default=os.getcwd(),
+        type=pathlib.Path, default=pathlib.Path.cwd(),
         help='Working data directory')
     # Arctic Ocean tide model to download
     parser.add_argument('--tide','-T',
         metavar='TIDE', type=str, nargs='+', default=['Gr1kmTM'],
         choices=('AODTM-5','AOTIM-5','AOTIM-5-2018','Arc2kmTM','Gr1kmTM'),
         help='Arctic Ocean tide model to download')
     # permissions mode of the local directories and files (number in octal)
```

### Comparing `pyTMD-2.0.3/scripts/aviso_fes_tides.py` & `pyTMD-2.0.4/scripts/aviso_fes_tides.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/env python
 u"""
 aviso_fes_tides.py
-Written by Tyler Sutterley (11/2022)
+Written by Tyler Sutterley (04/2023)
 Downloads the FES (Finite Element Solution) global tide model from AVISO
 Decompresses the model tar files into the constituent files and auxiliary files
     https://www.aviso.altimetry.fr/data/products/auxiliary-products/
         global-tide-fes.html
     https://www.aviso.altimetry.fr/en/data/data-access.html
 
 CALLING SEQUENCE:
     python aviso_fes_tides.py --user <username> --tide FES2014
     where <username> is your AVISO data dissemination server username
 
 COMMAND LINE OPTIONS:
     --help: list the command line options
     --directory X: working data directory
-    --user X: username for AVISO FTP servers (email)
+    -U X, --user: username for AVISO FTP servers (email)
+    -P X, --password: password for AVISO FTP servers
     -N X, --netrc X: path to .netrc file for authentication
     --tide X: FES tide model to download
         FES1999
         FES2004
         FES2012
         FES2014
     --load: download load tide model outputs (fes2014)
@@ -31,14 +32,16 @@
     future: Compatibility layer between Python 2 and Python 3
         https://python-future.org/
 
 PROGRAM DEPENDENCIES:
     utilities.py: download and management utilities for syncing files
 
 UPDATE HISTORY:
+    Updated 04/2023: using pathlib to define and expand paths
+        added option to include AVISO FTP password as argument
     Updated 11/2022: added encoding for writing ascii files
         use f-strings for formatting verbose or ascii output
     Updated 04/2022: use argparse descriptions within documentation
     Updated 10/2021: using python logging for handling verbose output
     Updated 07/2021: can use prefix files to define command line arguments
     Updated 05/2021: use try/except for retrieving netrc credentials
     Updated 04/2021: set a default netrc file and check access
@@ -55,14 +58,15 @@
 import io
 import gzip
 import netrc
 import shutil
 import logging
 import tarfile
 import getpass
+import pathlib
 import argparse
 import builtins
 import posixpath
 import calendar, time
 import ftplib
 import pyTMD.utilities
 
@@ -70,23 +74,23 @@
 def aviso_fes_tides(MODEL, DIRECTORY=None, USER='', PASSWORD='', LOAD=False,
     CURRENTS=False, GZIP=False, LOG=False, MODE=None):
 
     # connect and login to AVISO ftp server
     f = ftplib.FTP('ftp-access.aviso.altimetry.fr',timeout=1000)
     f.login(USER, PASSWORD)
     # check if local directory exists and recursively create if not
-    localpath = os.path.join(DIRECTORY,MODEL.lower())
-    os.makedirs(localpath,MODE) if not os.path.exists(localpath) else None
+    localpath = pathlib.Path(DIRECTORY).joinpath(MODEL.lower()).expanduser()
+    localpath.mkdir(MODE, parents=True, exist_ok=True)
 
     # create log file with list of downloaded files (or print to terminal)
     if LOG:
         # format: AVISO_FES_tides_2002-04-01.log
         today = time.strftime('%Y-%m-%d',time.localtime())
-        LOGFILE = f'AVISO_FES_tides_{today}.log'
-        fid = open(os.path.join(DIRECTORY,LOGFILE), mode='w', encoding='utf8')
+        LOGFILE = localpath.joinpath(f'AVISO_FES_tides_{today}.log')
+        fid = LOGFILE.open(mode='w', encoding='utf8')
         logger = pyTMD.utilities.build_logger(__name__,stream=fid,
             level=logging.INFO)
         logger.info(f'AVISO FES Sync Log ({today})')
         logger.info(f'\tMODEL: {MODEL}')
     else:
         # standard output (terminal output)
         logger = pyTMD.utilities.build_logger(__name__,level=logging.INFO)
@@ -154,15 +158,15 @@
     for remotepath,tarmode,flatten in zip(FES[MODEL],TAR[MODEL],FLATTEN[MODEL]):
         # download file from ftp and decompress tar files
         ftp_download_file(logger,f,remotepath,localpath,tarmode,flatten,GZIP,MODE)
     # close the ftp connection
     f.quit()
     # close log file and set permissions level to MODE
     if LOG:
-        os.chmod(os.path.join(DIRECTORY,LOGFILE), MODE)
+        LOGFILE.chmod(MODE)
 
 # PURPOSE: pull file from a remote ftp server and decompress if tar file
 def ftp_download_file(logger,ftp,remote_path,local_dir,tarmode,flatten,GZIP,MODE):
     # remote and local directory for data product
     remote_file = posixpath.join('auxiliary','tide_model',*remote_path)
 
     # Printing files transferred
@@ -175,76 +179,74 @@
         fileobj.seek(0)
         # open the AOD1B monthly tar file
         tar = tarfile.open(name=remote_path[-1], fileobj=fileobj, mode=tarmode)
         # read tar file and extract all files
         member_files = [m for m in tar.getmembers() if tarfile.TarInfo.isfile(m)]
         for m in member_files:
             member = posixpath.basename(m.name) if flatten else m.name
-            fileBasename,fileExtension = posixpath.splitext(m.name)
+            fileBasename, fileExtension = posixpath.splitext(m.name)
             # extract file contents to new file
             if fileExtension in ('.asc','.nc') and GZIP:
-                local_file = os.path.join(local_dir,
-                    *posixpath.split(f'{member}.gz'))
-                logger.info(f'\t{local_file}')
+                local_file = local_dir.joinpath(*posixpath.split(f'{member}.gz'))
+                logger.info(f'\t{str(local_file)}')
                 # recursively create output directory if non-existent
-                if not os.access(os.path.dirname(local_file),os.F_OK):
-                    os.makedirs(os.path.dirname(local_file),MODE)
+                local_file.parent.mkdir(mode=MODE, parents=True, exist_ok=True)
                 # extract file to compressed gzip format in local directory
                 with tar.extractfile(m) as fi,gzip.open(local_file, 'wb') as fo:
                     shutil.copyfileobj(fi, fo)
             else:
-                local_file = os.path.join(local_dir,*posixpath.split(member))
-                logger.info(f'\t{local_file}')
+                local_file = local_dir.joinpath(*posixpath.split(member))
+                logger.info(f'\t{str(local_file)}')
                 # recursively create output directory if non-existent
-                if not os.access(os.path.dirname(local_file),os.F_OK):
-                    os.makedirs(os.path.dirname(local_file),MODE)
+                local_file.parent.mkdir(mode=MODE, parents=True, exist_ok=True)
                 # extract file to local directory
                 with tar.extractfile(m) as fi,open(local_file, 'wb') as fo:
                     shutil.copyfileobj(fi, fo)
             # get last modified date of remote file within tar file
             # keep remote modification time of file and local access time
-            os.utime(local_file, (os.stat(local_file).st_atime, m.mtime))
-            os.chmod(local_file, MODE)
+            pathlib.os.utime(local_file, (local_file.stat().st_atime, m.mtime))
+            local_file.chmod(MODE)
     else:
         # copy readme and uncompressed files directly
-        local_file = os.path.join(local_dir,remote_path[-1])
-        logger.info(f'\t{local_file}\n')
+        local_file = local_dir.joinpath(local_dir,remote_path[-1])
+        logger.info(f'\t{str(local_file)}\n')
         # copy remote file contents to local file
-        with open(local_file, 'wb') as f:
+        with local_file.open('wb') as f:
             ftp.retrbinary(f'RETR {remote_file}', f.write)
         # get last modified date of remote file and convert into unix time
         mdtm = ftp.sendcmd(f'MDTM {remote_file}')
         remote_mtime = calendar.timegm(time.strptime(mdtm[4:],"%Y%m%d%H%M%S"))
         # keep remote modification time of file and local access time
-        os.utime(local_file, (os.stat(local_file).st_atime, remote_mtime))
-        os.chmod(local_file, MODE)
+        pathlib.os.utime(local_file, (local_file.stat().st_atime, remote_mtime))
+        local_file.chmod(MODE)
 
 # PURPOSE: create argument parser
 def arguments():
     parser = argparse.ArgumentParser(
         description="""Downloads the FES (Finite Element Solution) global tide
             model from AVISO.  Decompresses the model tar files into the
             constituent files and auxiliary files.
             """,
         fromfile_prefix_chars="@"
     )
     parser.convert_arg_line_to_args = pyTMD.utilities.convert_arg_line_to_args
     # command line parameters
     # AVISO FTP credentials
     parser.add_argument('--user','-U',
-        type=str, default='',
-        help='Username for AVISO FTP servers')
+        type=str, default=os.environ.get('AVISO_USERNAME'),
+        help='Username for AVISO Login')
+    parser.add_argument('--password','-W',
+        type=str, default=os.environ.get('AVISO_PASSWORD'),
+        help='Password for AVISO Login')
     parser.add_argument('--netrc','-N',
-        type=lambda p: os.path.abspath(os.path.expanduser(p)),
-        default=os.path.join(os.path.expanduser('~'),'.netrc'),
+        type=pathlib.Path, default=pathlib.Path().home().joinpath('.netrc'),
         help='Path to .netrc file for authentication')
     # working data directory
     parser.add_argument('--directory','-D',
-        type=lambda p: os.path.abspath(os.path.expanduser(p)),
-        default=os.getcwd(),
+        type=pathlib.Path, default=pathlib.Path.cwd(),
         help='Working data directory')
     # FES tide models
     parser.add_argument('--tide','-T',
         metavar='TIDE', type=str, nargs='+',
         default=['FES2014'], choices=['FES1999','FES2004','FES2012','FES2014'],
         help='FES tide model to download')
     # download FES load tides
@@ -275,29 +277,35 @@
 def main():
     # Read the system arguments listed after the program
     parser = arguments()
     args,_ = parser.parse_known_args()
 
     # AVISO FTP Server hostname
     HOST = 'ftp-access.aviso.altimetry.fr'
-    # get AVISO FTP Server credentials
-    try:
-        args.user,_,PASSWORD = netrc.netrc(args.netrc).authenticators(HOST)
-    except:
-        # check that AVISO FTP Server credentials were entered
-        if not args.user:
-            prompt = f'Username for {HOST}: '
-            args.user = builtins.input(prompt)
+    # get authentication
+    if not args.user and not args.netrc.exists():
+        # check that AVISO credentials were entered
+        args.user = builtins.input(f'Username for {HOST}: ')
         # enter password securely from command-line
-        prompt = f'Password for {args.user}@{HOST}: '
-        PASSWORD = getpass.getpass(prompt)
+        args.password = getpass.getpass(f'Password for {args.user}@{HOST}: ')
+    elif args.netrc.exists():
+        args.user,_,args.password = netrc.netrc(args.netrc).authenticators(HOST)
+    elif args.user and not args.password:
+        # enter password securely from command-line
+        args.password = getpass.getpass(f'Password for {args.user}@{HOST}: ')
 
     # check internet connection before attempting to run program
-    if pyTMD.utilities.check_ftp_connection(HOST,args.user,PASSWORD):
+    if pyTMD.utilities.check_ftp_connection(HOST,args.user,args.password):
         for m in args.tide:
-            aviso_fes_tides(m, DIRECTORY=args.directory, USER=args.user,
-                PASSWORD=PASSWORD, LOAD=args.load, CURRENTS=args.currents,
-                GZIP=args.gzip, LOG=args.log, MODE=args.mode)
+            aviso_fes_tides(m,
+                DIRECTORY=args.directory,
+                USER=args.user,
+                PASSWORD=args.password,
+                LOAD=args.load,
+                CURRENTS=args.currents,
+                GZIP=args.gzip,
+                LOG=args.log,
+                MODE=args.mode)
 
 # run main program
 if __name__ == '__main__':
     main()
```

### Comparing `pyTMD-2.0.3/scripts/compute_LPET_elevations.py` & `pyTMD-2.0.4/scripts/compute_LPET_elevations.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,15 +60,17 @@
 PROGRAM DEPENDENCIES:
     time.py: utilities for calculating time operations
     spatial.py: utilities for reading and writing spatial data
     utilities.py: download and management utilities for syncing files
     predict.py: calculates long-period equilibrium ocean tides
 
 UPDATE HISTORY:
+    Updated 05/2023: use timescale class for time conversion operations
     Updated 04/2023: check if datetime before converting to seconds
+        using pathlib to define and expand paths
     Updated 02/2023: added functionality for time series type
     Updated 01/2023: added default field mapping for reading from netCDF4/HDF5
         added data type keyword for netCDF4 output
     Updated 12/2022: single implicit import of pyTMD tools
     Updated 11/2022: place some imports within try/except statements
         use f-strings for formatting verbose or ascii output
     Updated 10/2022: added delimiter option and datetime parsing for ascii files
@@ -80,16 +82,16 @@
     Updated 11/2020: added options to read from and write to geotiff image files
     Updated 10/2020: using argparse to set command line parameters
     Written 09/2020
 """
 from __future__ import print_function
 
 import sys
-import os
 import logging
+import pathlib
 import warnings
 import argparse
 import numpy as np
 import pyTMD
 
 # attempt imports
 try:
@@ -210,110 +212,75 @@
 
     # extract time units from netCDF4 and HDF5 attributes or from TIME_UNITS
     try:
         time_string = dinput['attributes']['time']['units']
         epoch1, to_secs = pyTMD.time.parse_date_string(time_string)
     except (TypeError, KeyError, ValueError):
         epoch1, to_secs = pyTMD.time.parse_date_string(TIME_UNITS)
-    # convert time to seconds
-    if (TIME_STANDARD.lower() != 'datetime'):
-        delta_time = to_secs*dinput['time'].flatten()
-
-    # calculate leap seconds if specified
-    if (TIME_STANDARD.upper() == 'GPS'):
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    elif (TIME_STANDARD.upper() == 'LORAN'):
-        # LORAN time is ahead of GPS time by 9 seconds
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(-9.0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time-9.0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    elif (TIME_STANDARD.upper() == 'TAI'):
-        # TAI time is ahead of GPS time by 19 seconds
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(-19.0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time-19.0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    else:
-        leap_seconds = 0.0
 
+    # convert delta times or datetimes objects to timescale
     if (TIME_STANDARD.lower() == 'datetime'):
-        # convert delta time array from datetime object
-        # to days relative to 1992-01-01T00:00:00
-        tide_time = pyTMD.time.convert_datetime(dinput['time'].flatten(),
-            epoch=pyTMD.time._tide_epoch)/86400.0
+        timescale = pyTMD.time.timescale().from_datetime(
+            dinput['time'].flatten())
     else:
-        # convert time from units to days since 1992-01-01T00:00:00 (UTC)
-        tide_time = pyTMD.time.convert_delta_time(delta_time-leap_seconds,
-            epoch1=epoch1, epoch2=pyTMD.time._tide_epoch, scale=1.0/86400.0)
-
-    # interpolate delta times from calendar dates to tide time
-    delta_file = pyTMD.utilities.get_data_path(['data','merged_deltat.data'])
-    deltat = pyTMD.time.interpolate_delta_time(delta_file, tide_time)
+        # convert time to seconds
+        delta_time = to_secs*dinput['time'].flatten()
+        timescale = pyTMD.time.timescale().from_deltatime(delta_time,
+            epoch=epoch1, standard=TIME_STANDARD)
     # number of time points
-    nt = len(tide_time)
+    nt = len(timescale)
+    # convert tide times to dynamical time
+    tide_time = timescale.tide + timescale.tt_ut1
 
     # predict long-period equilibrium tides at time
     if (TYPE == 'grid'):
         tide_lpe = np.zeros((ny,nx,nt))
         for i in range(nt):
-            lpet = pyTMD.predict.equilibrium_tide(tide_time[i] + deltat[i], phi)
+            lpet = pyTMD.predict.equilibrium_tide(tide_time[i], phi)
             tide_lpe[:,:,i] = np.reshape(lpet,(ny,nx))
     elif (TYPE == 'drift'):
-        tide_lpe = pyTMD.predict.equilibrium_tide(tide_time + deltat, phi)
+        tide_lpe = pyTMD.predict.equilibrium_tide(tide_time, phi)
     elif (TYPE == 'time series'):
         tide_lpe = np.zeros((nstation,nt))
         for s in range(nstation):
-            lpet = pyTMD.predict.equilibrium_tide(tide_time + deltat, phi[s])
+            lpet = pyTMD.predict.equilibrium_tide(tide_time, phi[s])
             tide_lpe[s,:] = np.copy(lpet)
 
     # output to file
-    output = dict(time=tide_time, lon=lon, lat=lat, tide_lpe=tide_lpe)
+    output = dict(time=timescale.tide, lon=lon, lat=lat, tide_lpe=tide_lpe)
     if (FORMAT == 'csv'):
         pyTMD.spatial.to_ascii(output, attrib, output_file,
             delimiter=DELIMITER, header=False,
             columns=['time','lat','lon','tide_lpe'])
     elif (FORMAT == 'netCDF4'):
         pyTMD.spatial.to_netCDF4(output, attrib, output_file, data_type=TYPE)
     elif (FORMAT == 'HDF5'):
         pyTMD.spatial.to_HDF5(output, attrib, output_file)
     elif (FORMAT == 'geotiff'):
         pyTMD.spatial.to_geotiff(output, attrib, output_file,
             varname='tide_lpe')
     # change the permissions level to MODE
-    os.chmod(output_file, MODE)
+    output_file.chmod(MODE)
 
 # PURPOSE: create argument parser
 def arguments():
     parser = argparse.ArgumentParser(
         description="""Calculates long-period equilibrium tidal elevations for
             an input file
             """,
         fromfile_prefix_chars="@"
     )
     parser.convert_arg_line_to_args = pyTMD.utilities.convert_arg_line_to_args
     # command line options
     # input and output file
     parser.add_argument('infile',
-        type=lambda p: os.path.abspath(os.path.expanduser(p)), nargs='?',
+        type=pathlib.Path, nargs='?',
         help='Input file to run')
     parser.add_argument('outfile',
-        type=lambda p: os.path.abspath(os.path.expanduser(p)), nargs='?',
+        type=pathlib.Path, nargs='?',
         help='Computed output file')
     # input and output data format
     parser.add_argument('--format','-F',
         type=str, default='csv', choices=('csv','netCDF4','HDF5','geotiff'),
         help='Input and output data format')
     # variable names (for csv names of columns)
     parser.add_argument('--variables','-v',
@@ -368,16 +335,15 @@
 def main():
     # Read the system arguments listed after the program
     parser = arguments()
     args,_ = parser.parse_known_args()
 
     # set output file from input filename if not entered
     if not args.outfile:
-        fileBasename,fileExtension = os.path.splitext(args.infile)
-        vars = (fileBasename,'lpe_tide',fileExtension)
+        vars = (args.infile.stem,'lpe_tide',args.infile.suffix)
         args.outfile = '{0}_{1}{2}'.format(*vars)
 
     # run long period equilibrium tide program for input file
     compute_LPET_elevations(args.infile, args.outfile,
         FORMAT=args.format,
         VARIABLES=args.variables,
         HEADER=args.header,
```

### Comparing `pyTMD-2.0.3/scripts/compute_LPT_displacements.py` & `pyTMD-2.0.4/scripts/compute_LPT_displacements.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 compute_LPT_displacements.py
-Written by Tyler Sutterley (04/2023)
+Written by Tyler Sutterley (05/2023)
 Calculates radial load pole tide displacements for an input file
     following IERS Convention (2010) guidelines
     https://iers-conventions.obspm.fr/chapter7.php
 
 INPUTS:
     csv file with columns for spatial and temporal coordinates
     HDF5 file with variables for spatial and temporal coordinates
@@ -69,15 +69,18 @@
     constants.py: gravitational and ellipsoidal parameters
     eop.py: utilities for calculating Earth Orientation Parameters (EOP)
     spatial: utilities for reading, writing and operating on spatial data
     time.py: utilities for calculating time operations
     utilities.py: download and management utilities for syncing files
 
 UPDATE HISTORY:
+    Updated 05/2023: use timescale class for time conversion operations
+        use defaults from eop module for pole tide and EOP files
     Updated 04/2023: check if datetime before converting to seconds
+        using pathlib to define and expand paths
     Updated 03/2023: added option for changing the IERS mean pole convention
     Updated 02/2023: added functionality for time series type
     Updated 01/2023: added default field mapping for reading from netCDF4/HDF5
         added data type keyword for netCDF4 output
     Updated 12/2022: single implicit import of pyTMD tools
         use constants class for ellipsoidal parameters
     Updated 11/2022: place some imports within try/except statements
@@ -97,20 +100,19 @@
     Updated 09/2020: can use HDF5 and netCDF4 as inputs and outputs
     Updated 10/2017: use mean pole coordinates from calc_mean_iers_pole.py
     Written 10/2017 for public release
 """
 from __future__ import print_function
 
 import sys
-import os
 import logging
+import pathlib
 import warnings
 import argparse
 import numpy as np
-import scipy.interpolate
 import pyTMD
 
 # attempt imports
 try:
     import pyproj
 except (ImportError, ModuleNotFoundError) as exc:
     warnings.filterwarnings("module")
@@ -232,59 +234,29 @@
 
     # extract time units from netCDF4 and HDF5 attributes or from TIME_UNITS
     try:
         time_string = dinput['attributes']['time']['units']
         epoch1, to_secs = pyTMD.time.parse_date_string(time_string)
     except (TypeError, KeyError, ValueError):
         epoch1, to_secs = pyTMD.time.parse_date_string(TIME_UNITS)
-    # convert time to seconds
-    if (TIME_STANDARD.lower() != 'datetime'):
-        delta_time = to_secs*dinput['time'].flatten()
-
-    # calculate leap seconds if specified
-    if (TIME_STANDARD.upper() == 'GPS'):
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    elif (TIME_STANDARD.upper() == 'LORAN'):
-        # LORAN time is ahead of GPS time by 9 seconds
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(-9.0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time-9.0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    elif (TIME_STANDARD.upper() == 'TAI'):
-        # TAI time is ahead of GPS time by 19 seconds
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(-19.0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time-19.0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    else:
-        leap_seconds = 0.0
 
+    # convert delta times or datetimes objects to timescale
     if (TIME_STANDARD.lower() == 'datetime'):
-        # convert delta time array from datetime object
-        # to Modified Julian days (days since 1858-11-17T00:00:00)
-        MJD = pyTMD.time.convert_datetime(dinput['time'].flatten(),
-            epoch=pyTMD.time._mjd_epoch)/86400.0
+        timescale = pyTMD.time.timescale().from_datetime(
+            dinput['time'].flatten())
     else:
-        # convert dates to Modified Julian days (days since 1858-11-17T00:00:00)
-        MJD = pyTMD.time.convert_delta_time(delta_time-leap_seconds,
-            epoch1=epoch1, epoch2=pyTMD.time._mjd_epoch, scale=1.0/86400.0)
-    # add offset to convert to Julian days and then convert to calendar dates
-    Y,M,D,h,m,s = pyTMD.time.convert_julian(2400000.5 + MJD, format='tuple')
+        # convert time to seconds
+        delta_time = to_secs*dinput['time'].flatten()
+        timescale = pyTMD.time.timescale().from_deltatime(delta_time,
+            epoch=epoch1, standard=TIME_STANDARD)
+
+    # convert dynamic time to Modified Julian Days (MJD)
+    MJD = timescale.tt - 2400000.5
+    # convert Julian days to calendar dates
+    Y,M,D,h,m,s = pyTMD.time.convert_julian(timescale.tt, format='tuple')
     # calculate time in year-decimal format
     time_decimal = pyTMD.time.convert_calendar_decimal(Y,M,day=D,
         hour=h,minute=m,second=s)
     # number of time points
     nt = len(time_decimal)
 
     # degrees and arcseconds to radians
@@ -309,27 +281,18 @@
     phi = dtr*lon.flatten()
 
     # compute normal gravity at spatial location and elevation of points.
     # Normal gravity at height h. p. 82, Eqn.(2-215)
     gamma_h = units.gamma_h(theta, h)
     dfactor = -hb2*atr*(units.omega**2*rr**2)/(2.0*gamma_h)
 
-    # pole tide files (mean and daily)
-    mean_pole_file = pyTMD.utilities.get_data_path(['data','mean-pole.tab'])
-    pole_tide_file = pyTMD.utilities.get_data_path(['data','finals.all'])
     # calculate angular coordinates of mean/secular pole at time
-    mpx, mpy, fl = pyTMD.eop.iers_mean_pole(mean_pole_file, time_decimal,
-        CONVENTION)
-    # read IERS daily polar motion values
-    EOP = pyTMD.eop.iers_daily_EOP(pole_tide_file)
-    # interpolate daily polar motion values to MJD using cubic splines
-    xSPL = scipy.interpolate.UnivariateSpline(EOP['MJD'],EOP['x'],k=3,s=0)
-    ySPL = scipy.interpolate.UnivariateSpline(EOP['MJD'],EOP['y'],k=3,s=0)
-    px = xSPL(MJD)
-    py = ySPL(MJD)
+    mpx, mpy, fl = pyTMD.eop.iers_mean_pole(time_decimal, convention=CONVENTION)
+    # read and interpolate IERS daily polar motion values
+    px, py = pyTMD.eop.iers_polar_motion(MJD, k=3, s=0)
     # calculate differentials from mean/secular pole positions
     mx = px - mpx
     my = -(py - mpy)
 
     # calculate radial displacement at time
     if (TYPE == 'grid'):
         Srad = np.ma.zeros((ny,nx,nt),fill_value=fill_value)
@@ -350,45 +313,45 @@
             SRAD = dfactor[s]*np.sin(2.0*theta[s])*(mx*np.cos(phi[s])+my*np.sin(phi[s]))
             Srad.data[s,:] = np.copy(SRAD)
             Srad.mask[s,:] = np.isnan(Srad.data[s,:])
     # replace invalid data with fill values
     Srad.data[Srad.mask] = Srad.fill_value
 
     # output to file
-    output = dict(time=MJD, lon=lon, lat=lat, tide_pole=Srad)
+    output = dict(time=timescale.MJD, lon=lon, lat=lat, tide_pole=Srad)
     if (FORMAT == 'csv'):
         pyTMD.spatial.to_ascii(output, attrib, output_file,
             delimiter=DELIMITER, header=False,
             columns=['time','lat','lon','tide_pole'])
     elif (FORMAT == 'netCDF4'):
         pyTMD.spatial.to_netCDF4(output, attrib, output_file, data_type=TYPE)
     elif (FORMAT == 'HDF5'):
         pyTMD.spatial.to_HDF5(output, attrib, output_file)
     elif (FORMAT == 'geotiff'):
         pyTMD.spatial.to_geotiff(output, attrib, output_file,
             varname='tide_pole')
     # change the permissions level to MODE
-    os.chmod(output_file, MODE)
+    output_file.chmod(MODE)
 
 # PURPOSE: create argument parser
 def arguments():
     parser = argparse.ArgumentParser(
         description="""Calculates radial pole load tide displacements for
             an input file following IERS Convention (2010) guidelines
             """,
         fromfile_prefix_chars="@"
     )
     parser.convert_arg_line_to_args = pyTMD.utilities.convert_arg_line_to_args
     # command line options
     # input and output file
     parser.add_argument('infile',
-        type=lambda p: os.path.abspath(os.path.expanduser(p)), nargs='?',
+        type=pathlib.Path, nargs='?',
         help='Input file to run')
     parser.add_argument('outfile',
-        type=lambda p: os.path.abspath(os.path.expanduser(p)), nargs='?',
+        type=pathlib.Path, nargs='?',
         help='Computed output file')
     # input and output data format
     parser.add_argument('--format','-F',
         type=str, default='csv', choices=('csv','netCDF4','HDF5','geotiff'),
         help='Input and output data format')
     # variable names (for csv names of columns)
     parser.add_argument('--variables','-v',
@@ -451,16 +414,15 @@
 def main():
     # Read the system arguments listed after the program
     parser = arguments()
     args,_ = parser.parse_known_args()
 
     # set output file from input filename if not entered
     if not args.outfile:
-        fileBasename,fileExtension = os.path.splitext(args.infile)
-        vars = (fileBasename,'pole_tide',fileExtension)
+        vars = (args.infile.stem,'pole_tide',args.infile.suffix)
         args.outfile = '{0}_{1}{2}'.format(*vars)
 
     # run load pole tide program for input file
     compute_LPT_displacements(args.infile, args.outfile,
         FORMAT=args.format,
         VARIABLES=args.variables,
         HEADER=args.header,
```

### Comparing `pyTMD-2.0.3/scripts/compute_OPT_displacements.py` & `pyTMD-2.0.4/scripts/compute_OPT_displacements.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 compute_OPT_displacements.py
-Written by Tyler Sutterley (04/2023)
+Written by Tyler Sutterley (05/2023)
 Calculates radial ocean pole load tide displacements for an input file
     following IERS Convention (2010) guidelines
     https://iers-conventions.obspm.fr/chapter7.php
 
 INPUTS:
     csv file with columns for spatial and temporal coordinates
     HDF5 file with variables for spatial and temporal coordinates
@@ -73,22 +73,25 @@
     time.py: utilities for calculating time operations
     spatial.py: utilities for reading and writing spatial data
     utilities.py: download and management utilities for syncing files
     eop.py: utilities for calculating Earth Orientation Parameters (EOP)
     io/ocean_pole_tide.py: read ocean pole load tide map from IERS
 
 REFERENCES:
-    S Desai, "Observing the pole tide with satellite altimetry", Journal of
+    S. Desai, "Observing the pole tide with satellite altimetry", Journal of
         Geophysical Research: Oceans, 107(C11), 2002. doi: 10.1029/2001JC001224
-    S Desai, J Wahr and B Beckley "Revisiting the pole tide for and from
+    S. Desai, J. Wahr and B. Beckley "Revisiting the pole tide for and from
         satellite altimetry", Journal of Geodesy, 89(12), p1233-1243, 2015.
         doi: 10.1007/s00190-015-0848-7
 
 UPDATE HISTORY:
+    Updated 05/2023: use timescale class for time conversion operations
+        use defaults from eop module for pole tide and EOP files
     Updated 04/2023: check if datetime before converting to seconds
+        using pathlib to define and expand paths
     Updated 03/2023: added option for changing the IERS mean pole convention
     Updated 02/2023: added functionality for time series type
     Updated 01/2023: added default field mapping for reading from netCDF4/HDF5
         added data type keyword for netCDF4 output
     Updated 12/2022: single implicit import of pyTMD tools
         use constants class for ellipsoidal parameters
     Updated 11/2022: place some imports within try/except statements
@@ -113,16 +116,16 @@
     Updated 08/2020: replaced griddata with scipy regular grid interpolators
     Updated 10/2017: use mean pole coordinates from calc_mean_iers_pole.py
     Written 10/2017 for public release
 """
 from __future__ import print_function
 
 import sys
-import os
 import logging
+import pathlib
 import warnings
 import argparse
 import numpy as np
 import scipy.interpolate
 import pyTMD
 
 # attempt imports
@@ -249,59 +252,29 @@
 
     # extract time units from netCDF4 and HDF5 attributes or from TIME_UNITS
     try:
         time_string = dinput['attributes']['time']['units']
         epoch1, to_secs = pyTMD.time.parse_date_string(time_string)
     except (TypeError, KeyError, ValueError):
         epoch1, to_secs = pyTMD.time.parse_date_string(TIME_UNITS)
-    # convert time to seconds
-    if (TIME_STANDARD.lower() != 'datetime'):
-        delta_time = to_secs*dinput['time'].flatten()
-
-    # calculate leap seconds if specified
-    if (TIME_STANDARD.upper() == 'GPS'):
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    elif (TIME_STANDARD.upper() == 'LORAN'):
-        # LORAN time is ahead of GPS time by 9 seconds
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(-9.0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time-9.0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    elif (TIME_STANDARD.upper() == 'TAI'):
-        # TAI time is ahead of GPS time by 19 seconds
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(-19.0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time-19.0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    else:
-        leap_seconds = 0.0
 
+    # convert delta times or datetimes objects to timescale
     if (TIME_STANDARD.lower() == 'datetime'):
-        # convert delta time array from datetime object
-        # to Modified Julian days (days since 1858-11-17T00:00:00)
-        MJD = pyTMD.time.convert_datetime(dinput['time'].flatten(),
-            epoch=pyTMD.time._mjd_epoch)/86400.0
+        timescale = pyTMD.time.timescale().from_datetime(
+            dinput['time'].flatten())
     else:
-        # convert dates to Modified Julian days (days since 1858-11-17T00:00:00)
-        MJD = pyTMD.time.convert_delta_time(delta_time-leap_seconds,
-            epoch1=epoch1, epoch2=pyTMD.time._mjd_epoch, scale=1.0/86400.0)
-    # add offset to convert to Julian days and then convert to calendar dates
-    Y,M,D,h,m,s = pyTMD.time.convert_julian(2400000.5 + MJD, format='tuple')
+        # convert time to seconds
+        delta_time = to_secs*dinput['time'].flatten()
+        timescale = pyTMD.time.timescale().from_deltatime(delta_time,
+            epoch=epoch1, standard=TIME_STANDARD)
+
+    # convert dynamic time to Modified Julian Days (MJD)
+    MJD = timescale.tt - 2400000.5
+    # convert Julian days to calendar dates
+    Y,M,D,h,m,s = pyTMD.time.convert_julian(timescale.tt, format='tuple')
     # calculate time in year-decimal format
     time_decimal = pyTMD.time.convert_calendar_decimal(Y,M,day=D,
         hour=h,minute=m,second=s)
     # number of time points
     nt = len(time_decimal)
 
     # degrees and arcseconds to radians
@@ -326,48 +299,37 @@
     latitude_geocentric = np.arctan(Z / np.sqrt(X**2.0 + Y**2.0))/dtr
 
     # pole tide displacement scale factor
     Hp = np.sqrt(8.0*np.pi/15.0)*(units.omega**2*units.a_axis**4)/units.GM
     K = 4.0*np.pi*units.G*rho_w*Hp*units.a_axis/(3.0*ge)
     K1 = 4.0*np.pi*units.G*rho_w*Hp*units.a_axis**3/(3.0*units.GM)
 
-    # pole tide files (mean and daily)
-    mean_pole_file = pyTMD.utilities.get_data_path(['data','mean-pole.tab'])
-    pole_tide_file = pyTMD.utilities.get_data_path(['data','finals.all'])
     # calculate angular coordinates of mean/secular pole at time
-    mpx, mpy, fl = pyTMD.eop.iers_mean_pole(mean_pole_file, time_decimal,
-        CONVENTION)
-    # read IERS daily polar motion values
-    EOP = pyTMD.eop.iers_daily_EOP(pole_tide_file)
-    # interpolate daily polar motion values to t1 using cubic splines
-    xSPL = scipy.interpolate.UnivariateSpline(EOP['MJD'],EOP['x'],k=3,s=0)
-    ySPL = scipy.interpolate.UnivariateSpline(EOP['MJD'],EOP['y'],k=3,s=0)
-    px = xSPL(MJD)
-    py = ySPL(MJD)
+    mpx, mpy, fl = pyTMD.eop.iers_mean_pole(time_decimal, convention=CONVENTION)
+    # read and interpolate IERS daily polar motion values
+    px, py = pyTMD.eop.iers_polar_motion(MJD, k=3, s=0)
     # calculate differentials from mean/secular pole positions
     mx = px - mpx
     my = -(py - mpy)
 
     # read ocean pole tide map from Desai (2002)
-    ocean_pole_tide_file = pyTMD.utilities.get_data_path(['data',
-        'opoleloadcoefcmcor.txt.gz'])
-    iur,iun,iue,ilon,ilat = pyTMD.io.ocean_pole_tide(ocean_pole_tide_file)
+    iur, iun, iue, ilon, ilat = pyTMD.io.ocean_pole_tide()
     # interpolate ocean pole tide map from Desai (2002)
     if (METHOD == 'spline'):
         # use scipy bivariate splines to interpolate to output points
         f1 = scipy.interpolate.RectBivariateSpline(ilon, ilat[::-1],
             iur[:,::-1].real, kx=1, ky=1)
         f2 = scipy.interpolate.RectBivariateSpline(ilon, ilat[::-1],
             iur[:,::-1].imag, kx=1, ky=1)
         UR = np.zeros((len(latitude_geocentric)),dtype=np.longcomplex)
         UR.real = f1.ev(lon.flatten(), latitude_geocentric)
         UR.imag = f2.ev(lon.flatten(), latitude_geocentric)
     else:
         # use scipy regular grid to interpolate values for a given method
-        r1 = scipy.interpolate.RegularGridInterpolator((ilon,ilat[::-1]),
+        r1 = scipy.interpolate.RegularGridInterpolator((ilon, ilat[::-1]),
             iur[:,::-1], method=METHOD)
         UR = r1.__call__(np.c_[lon.flatten(), latitude_geocentric])
 
     # calculate radial displacement at time
     if (TYPE == 'grid'):
         Urad = np.ma.zeros((ny,nx,nt),fill_value=fill_value)
         Urad.mask = np.zeros((ny,nx,nt),dtype=bool)
@@ -390,45 +352,45 @@
                 (my*gamma.real - mx*gamma.imag)*UR.imag[s])
             Urad.data[s,:] = np.copy(URAD)
             Urad.mask[s,:] = np.isnan(Urad.data[s,:])
     # replace invalid data with fill values
     Urad.data[Urad.mask] = Urad.fill_value
 
     # output to file
-    output = dict(time=MJD, lon=lon, lat=lat, tide_oc_pole=Urad)
+    output = dict(time=timescale.MJD, lon=lon, lat=lat, tide_oc_pole=Urad)
     if (FORMAT == 'csv'):
         pyTMD.spatial.to_ascii(output, attrib, output_file,
             delimiter=DELIMITER, header=False,
             columns=['time','lat','lon','tide_oc_pole'])
     elif (FORMAT == 'netCDF4'):
         pyTMD.spatial.to_netCDF4(output, attrib, output_file, data_type=TYPE)
     elif (FORMAT == 'HDF5'):
         pyTMD.spatial.to_HDF5(output, attrib, output_file)
     elif (FORMAT == 'geotiff'):
         pyTMD.spatial.to_geotiff(output, attrib, output_file,
             varname='tide_oc_pole')
     # change the permissions level to MODE
-    os.chmod(output_file, MODE)
+    output_file.chmod(MODE)
 
 # PURPOSE: create argument parser
 def arguments():
     parser = argparse.ArgumentParser(
         description="""Calculates radial ocean pole load tide displacements for
             an input file following IERS Convention (2010) guidelines
             """,
         fromfile_prefix_chars="@"
     )
     parser.convert_arg_line_to_args = pyTMD.utilities.convert_arg_line_to_args
     # command line options
     # input and output file
     parser.add_argument('infile',
-        type=lambda p: os.path.abspath(os.path.expanduser(p)), nargs='?',
+        type=pathlib.Path, nargs='?',
         help='Input file to run')
     parser.add_argument('outfile',
-        type=lambda p: os.path.abspath(os.path.expanduser(p)), nargs='?',
+        type=pathlib.Path, nargs='?',
         help='Computed output file')
     # input and output data format
     parser.add_argument('--format','-F',
         type=str, default='csv', choices=('csv','netCDF4','HDF5','geotiff'),
         help='Input and output data format')
     # variable names (for csv names of columns)
     parser.add_argument('--variables','-v',
@@ -496,16 +458,15 @@
 def main():
     # Read the system arguments listed after the program
     parser = arguments()
     args,_ = parser.parse_known_args()
 
     # set output file from input filename if not entered
     if not args.outfile:
-        fileBasename,fileExtension = os.path.splitext(args.infile)
-        vars = (fileBasename,'ocean_pole_tide',fileExtension)
+        vars = (args.infile.stem,'ocean_pole_tide',args.infile.suffix)
         args.outfile = '{0}_{1}{2}'.format(*vars)
 
     # run ocean pole tide program for input file
     compute_OPT_displacements(args.infile, args.outfile,
         FORMAT=args.format,
         VARIABLES=args.variables,
         HEADER=args.header,
```

### Comparing `pyTMD-2.0.3/scripts/compute_SET_displacements.py` & `pyTMD-2.0.4/scripts/compute_SET_displacements.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 compute_SET_displacements.py
-Written by Tyler Sutterley (04/2023)
+Written by Tyler Sutterley (05/2023)
 Calculates radial solid earth tide displacements for an input file
     following IERS Convention (2010) guidelines
     https://iers-conventions.obspm.fr/chapter7.php
 
 INPUTS:
     csv file with columns for spatial and temporal coordinates
     HDF5 file with variables for spatial and temporal coordinates
@@ -39,14 +39,17 @@
         datetime: formatted datetime string in UTC
     -P X, --projection X: spatial projection as EPSG code or PROJ4 string
         4326: latitude and longitude coordinates on WGS84 reference ellipsoid
     -E X, --ellipsoid X: Ellipsoid for calculating astronomical parameters
     -p X, --tide-system X: Permanent tide system for output values
         tide_free: no permanent direct and indirect tidal potentials
         mean_tide: permanent tidal potentials (direct and indirect)
+    -c X, --ephemerides X: method for calculating lunisolar ephemerides
+        approximate: low-resolution ephemerides (default)
+        JPL: computed solar and lunar ephemerides from JPL kernels
     -V, --verbose: Verbose output of processing run
     -M X, --mode X: Permission mode of output file
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
@@ -84,21 +87,24 @@
         19(6), 529--531, (1992). doi: 10.1029/92GL00259
     J. M. Wahr, "Body tides on an elliptical, rotating, elastic
         and oceanless Earth", Geophysical Journal of the Royal
         Astronomical Society, 64(3), 677--703, (1981).
         doi: 10.1111/j.1365-246X.1981.tb02690.x
 
 UPDATE HISTORY:
+    Updated 05/2023: use timescale class for time conversion operations
+        add option for using higher resolution ephemerides from JPL
+    Updated 04/2023: using pathlib to define and expand paths
     Written 04/2023
 """
 from __future__ import print_function
 
 import sys
-import os
 import logging
+import pathlib
 import warnings
 import argparse
 import numpy as np
 import pyTMD
 
 # attempt imports
 try:
@@ -145,14 +151,15 @@
     TYPE='drift',
     TIME_UNITS='days since 1858-11-17T00:00:00',
     TIME=None,
     TIME_STANDARD='UTC',
     PROJECTION='4326',
     ELLIPSOID='WGS84',
     TIDE_SYSTEM='tide_free',
+    EPHEMERIDES='approximate',
     VERBOSE=False,
     MODE=0o775):
 
     # create logger for verbosity level
     loglevel = logging.INFO if VERBOSE else logging.CRITICAL
     logging.basicConfig(level=loglevel)
 
@@ -221,168 +228,137 @@
 
     # extract time units from netCDF4 and HDF5 attributes or from TIME_UNITS
     try:
         time_string = dinput['attributes']['time']['units']
         epoch1, to_secs = pyTMD.time.parse_date_string(time_string)
     except (TypeError, KeyError, ValueError):
         epoch1, to_secs = pyTMD.time.parse_date_string(TIME_UNITS)
-    # convert time to seconds
-    if (TIME_STANDARD.lower() != 'datetime'):
-        delta_time = to_secs*dinput['time'].flatten()
-
-    # calculate leap seconds if specified
-    if (TIME_STANDARD.upper() == 'GPS'):
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    elif (TIME_STANDARD.upper() == 'LORAN'):
-        # LORAN time is ahead of GPS time by 9 seconds
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(-9.0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time-9.0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    elif (TIME_STANDARD.upper() == 'TAI'):
-        # TAI time is ahead of GPS time by 19 seconds
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(-19.0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time-19.0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    else:
-        leap_seconds = 0.0
 
+    # convert delta times or datetimes objects to timescale
     if (TIME_STANDARD.lower() == 'datetime'):
-        # convert delta time array from datetime object
-        # to days relative to 1992-01-01T00:00:00
-        tide_time = pyTMD.time.convert_datetime(dinput['time'].flatten(),
-            epoch=pyTMD.time._tide_epoch)/86400.0
+        timescale = pyTMD.time.timescale().from_datetime(
+            dinput['time'].flatten())
     else:
-        # convert time from units to days since 1992-01-01T00:00:00
-        tide_time = pyTMD.time.convert_delta_time(delta_time-leap_seconds,
-            epoch1=epoch1, epoch2=pyTMD.time._tide_epoch, scale=1.0/86400.0)
-
-    # interpolate delta times from calendar dates to tide time
-    delta_file = pyTMD.utilities.get_data_path(['data','merged_deltat.data'])
-    deltat = pyTMD.time.interpolate_delta_time(delta_file, tide_time)
+        # convert time to seconds
+        delta_time = to_secs*dinput['time'].flatten()
+        timescale = pyTMD.time.timescale().from_deltatime(delta_time,
+            epoch=epoch1, standard=TIME_STANDARD)
+    # convert tide times to dynamical time
+    tide_time = timescale.tide + timescale.tt_ut1
     # number of time points
-    nt = len(tide_time)
+    nt = len(timescale)
 
     # earth and physical parameters for ellipsoid
     units = pyTMD.constants(ELLIPSOID)
 
     # flatten heights
     h = dinput['data'].flatten() if ('data' in dinput.keys()) else 0.0
     # convert input coordinates to cartesian
     X, Y, Z = pyTMD.spatial.to_cartesian(lon, lat, h=h,
         a_axis=units.a_axis, flat=units.flat)
-    # convert time to Modified Julian Days (MJD) for ephemerides
-    MJD = tide_time + deltat + 48622.0
-    # get low-resolution solar and lunar ephemerides
-    SX, SY, SZ = pyTMD.astro.solar_ecef(MJD)
-    LX, LY, LZ = pyTMD.astro.lunar_ecef(MJD)
+    # compute ephemerides for lunisolar coordinates
+    if (EPHEMERIDES.lower() == 'approximate'):
+        # get low-resolution solar and lunar ephemerides
+        SX, SY, SZ = pyTMD.astro.solar_ecef(timescale.MJD)
+        LX, LY, LZ = pyTMD.astro.lunar_ecef(timescale.MJD)
+    elif (EPHEMERIDES.upper() == 'JPL'):
+        # compute solar and lunar ephemerides from JPL kernel
+        SX, SY, SZ = pyTMD.astro.solar_ephemerides(timescale.MJD)
+        LX, LY, LZ = pyTMD.astro.lunar_ephemerides(timescale.MJD)
 
     # calculate radial displacement at time
     if (TYPE == 'grid'):
         tide_se = np.zeros((ny,nx,nt))
         # convert coordinates to column arrays
         XYZ = np.c_[X, Y, Z]
         for i in range(nt):
             # reshape time to match spatial
-            t = tide_time[i] + deltat[i] + np.ones((ny*nx))
+            t = tide_time[i] + np.ones((ny*nx))
             # convert coordinates to column arrays
             SXYZ = np.repeat(np.c_[SX[i], SY[i], SZ[i]], ny*nx, axis=0)
             LXYZ = np.repeat(np.c_[LX[i], LY[i], LZ[i]], ny*nx, axis=0)
             # predict solid earth tides (cartesian)
             dxi = pyTMD.predict.solid_earth_tide(t,
                 XYZ, SXYZ, LXYZ, a_axis=units.a_axis,
                 tide_system=TIDE_SYSTEM)
             # calculate radial component of solid earth tides
-            dln,dlt,drad = pyTMD.spatial.to_geodetic(
+            dln, dlt, drad = pyTMD.spatial.to_geodetic(
                 X + dxi[:,0], Y + dxi[:,1], Z + dxi[:,2],
                 a_axis=units.a_axis, flat=units.flat)
             # remove effects of original topography
             # (if added when computing cartesian coordinates)
             tide_se[:,:,i] = np.reshape(drad - h, (ny,nx))
     elif (TYPE == 'drift'):
         # convert coordinates to column arrays
         XYZ = np.c_[X, Y, Z]
         SXYZ = np.c_[SX, SY, SZ]
         LXYZ = np.c_[LX, LY, LZ]
         # predict solid earth tides (cartesian)
-        dxi = pyTMD.predict.solid_earth_tide(tide_time + deltat,
+        dxi = pyTMD.predict.solid_earth_tide(tide_time,
             XYZ, SXYZ, LXYZ, a_axis=units.a_axis,
             tide_system=TIDE_SYSTEM)
         # calculate radial component of solid earth tides
-        dln,dlt,drad = pyTMD.spatial.to_geodetic(
+        dln, dlt, drad = pyTMD.spatial.to_geodetic(
             X + dxi[:,0], Y + dxi[:,1], Z + dxi[:,2],
             a_axis=units.a_axis, flat=units.flat)
         # remove effects of original topography
         # (if added when computing cartesian coordinates)
         tide_se = drad - h
     elif (TYPE == 'time series'):
         tide_se = np.zeros((nstation,nt))
         # convert coordinates to column arrays
         SXYZ = np.c_[SX, SY, SZ]
         LXYZ = np.c_[LX, LY, LZ]
         for s in range(nstation):
             # convert coordinates to column arrays
             XYZ = np.repeat(np.c_[X[s], Y[s], Z[s]], nt, axis=0)
             # predict solid earth tides (cartesian)
-            dxi = pyTMD.predict.solid_earth_tide(tide_time + deltat,
+            dxi = pyTMD.predict.solid_earth_tide(tide_time,
                 XYZ, SXYZ, LXYZ, a_axis=units.a_axis,
                 tide_system=TIDE_SYSTEM)
             # calculate radial component of solid earth tides
-            dln,dlt,drad = pyTMD.spatial.to_geodetic(
+            dln, dlt, drad = pyTMD.spatial.to_geodetic(
                 X + dxi[:,0], Y + dxi[:,1], Z + dxi[:,2],
                 a_axis=units.a_axis, flat=units.flat)
             # remove effects of original topography
             # (if added when computing cartesian coordinates)
             tide_se[s,:] = drad - h
 
     # output to file
-    output = dict(time=tide_time, lon=lon, lat=lat, tide_se=tide_se)
+    output = dict(time=timescale.tide, lon=lon, lat=lat, tide_se=tide_se)
     if (FORMAT == 'csv'):
         pyTMD.spatial.to_ascii(output, attrib, output_file,
             delimiter=DELIMITER, header=False,
             columns=['time','lat','lon','tide_se'])
     elif (FORMAT == 'netCDF4'):
         pyTMD.spatial.to_netCDF4(output, attrib, output_file, data_type=TYPE)
     elif (FORMAT == 'HDF5'):
         pyTMD.spatial.to_HDF5(output, attrib, output_file)
     elif (FORMAT == 'geotiff'):
         pyTMD.spatial.to_geotiff(output, attrib, output_file,
             varname='tide_se')
     # change the permissions level to MODE
-    os.chmod(output_file, MODE)
+    output_file.chmod(MODE)
 
 # PURPOSE: create argument parser
 def arguments():
     parser = argparse.ArgumentParser(
         description="""Calculates solid earth load tide displacements for
             an input file following IERS Convention (2010) guidelines
             """,
         fromfile_prefix_chars="@"
     )
     parser.convert_arg_line_to_args = pyTMD.utilities.convert_arg_line_to_args
     # command line options
     # input and output file
     parser.add_argument('infile',
-        type=lambda p: os.path.abspath(os.path.expanduser(p)), nargs='?',
+        type=pathlib.Path, nargs='?',
         help='Input file to run')
     parser.add_argument('outfile',
-        type=lambda p: os.path.abspath(os.path.expanduser(p)), nargs='?',
+        type=pathlib.Path, nargs='?',
         help='Computed output file')
     # input and output data format
     parser.add_argument('--format','-F',
         type=str, default='csv', choices=('csv','netCDF4','HDF5','geotiff'),
         help='Input and output data format')
     # variable names (for csv names of columns)
     parser.add_argument('--variables','-v',
@@ -425,14 +401,18 @@
     parser.add_argument('--ellipsoid','-E',
         type=str, choices=pyTMD._ellipsoids, default='WGS84',
         help='Ellipsoid for calculating astronomical parameters')
     # permanent tide system for output values
     parser.add_argument('--tide-system','-p',
         type=str, choices=('tide_free','mean_tide'), default='tide_free',
         help='Permanent tide system for output values')
+    # method for calculating lunisolar ephemerides
+    parser.add_argument('--ephemerides','-c',
+        type=str, choices=('approximate','JPL'), default='approximate',
+        help='Method for calculating lunisolar ephemerides')
     # verbose output of processing run
     # print information about each input and output file
     parser.add_argument('--verbose','-V',
         default=False, action='store_true',
         help='Verbose output of run')
     # permissions mode of the local files (number in octal)
     parser.add_argument('--mode','-M',
@@ -445,16 +425,15 @@
 def main():
     # Read the system arguments listed after the program
     parser = arguments()
     args,_ = parser.parse_known_args()
 
     # set output file from input filename if not entered
     if not args.outfile:
-        fileBasename,fileExtension = os.path.splitext(args.infile)
-        vars = (fileBasename,'solid_earth_tide',fileExtension)
+        vars = (args.infile.stem,'solid_earth_tide',args.infile.suffix)
         args.outfile = '{0}_{1}{2}'.format(*vars)
 
     # run solid earth tide program for input file
     compute_SET_displacements(args.infile, args.outfile,
         FORMAT=args.format,
         VARIABLES=args.variables,
         HEADER=args.header,
@@ -462,13 +441,14 @@
         TYPE=args.type,
         TIME_UNITS=args.epoch,
         TIME=args.deltatime,
         TIME_STANDARD=args.standard,
         PROJECTION=args.projection,
         ELLIPSOID=args.ellipsoid,
         TIDE_SYSTEM=args.tide_system,
+        EPHEMERIDES=args.ephemerides,
         VERBOSE=args.verbose,
         MODE=args.mode)
 
 # run main program
 if __name__ == '__main__':
     main()
```

### Comparing `pyTMD-2.0.3/scripts/compute_tidal_currents.py` & `pyTMD-2.0.4/scripts/compute_tidal_currents.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 compute_tidal_currents.py
-Written by Tyler Sutterley (02/2023)
+Written by Tyler Sutterley (05/2023)
 Calculates zonal and meridional tidal currents for an input file
 
 Uses OTIS format tidal solutions provided by Ohio State University and ESR
     http://volkov.oce.orst.edu/tides/region.html
     https://www.esr.org/research/polar-tide-models/list-of-polar-tide-models/
     ftp://ftp.esr.org/pub/datasets/tmd/
 or Finite Element Solution (FES) models provided by AVISO
@@ -75,26 +75,29 @@
     pyproj: Python interface to PROJ library
         https://pypi.org/project/pyproj/
 
 PROGRAM DEPENDENCIES:
     time.py: utilities for calculating time operations
     spatial: utilities for reading, writing and operating on spatial data
     utilities.py: download and management utilities for syncing files
+    arguments.py: load the nodal corrections for tidal constituents
     astro.py: computes the basic astronomical mean longitudes
     convert_crs.py: convert points to and from Coordinates Reference Systems
     load_constituent.py: loads parameters for a given tidal constituent
-    load_nodal_corrections.py: load the nodal corrections for tidal constituents
     io/model.py: retrieves tide model parameters for named tide models
     io/OTIS.py: extract tidal harmonic constants from OTIS tide models
     io/ATLAS.py: extract tidal harmonic constants from netcdf models
     io/FES.py: extract tidal harmonic constants from FES tide models
     interpolate.py: interpolation routines for spatial data
     predict.py: predict tidal values using harmonic constants
 
 UPDATE HISTORY:
+    Updated 05/2023: use timescale class for time conversion operations
+    Updated 04/2023: using pathlib to define and expand paths
+        using long_name and description attributes from model class
     Updated 02/2023: added functionality for time series type
     Updated 01/2023: added default field mapping for reading from netCDF4/HDF5
         added data type keyword for netCDF4 output
     Updated 12/2022: single implicit import of pyTMD tools
     Updated 11/2022: place some imports within try/except statements
         use f-strings for formatting verbose or ascii output
     Updated 10/2022: added delimiter option and datetime parsing for ascii files
@@ -128,16 +131,16 @@
     Updated 09/2019: added TPXO9_atlas reading from netcdf4 tide files
     Updated 07/2018: added GSFC Global Ocean Tides (GOT) models
     Written 10/2017 for public release
 """
 from __future__ import print_function
 
 import sys
-import os
 import logging
+import pathlib
 import warnings
 import argparse
 import numpy as np
 import pyTMD
 
 # attempt imports
 try:
@@ -218,29 +221,27 @@
     attrib['lat']['units'] = 'Degrees_North'
     # longitude
     attrib['lon'] = {}
     attrib['lon']['long_name'] = 'Longitude'
     attrib['lon']['units'] = 'Degrees_East'
     # zonal tidal currents
     attrib['u'] = {}
-    attrib['u']['description'] = ('depth_averaged_tidal_zonal_current_'
-        'from_harmonic_constants')
+    attrib['u']['description'] = model.description['u']
     attrib['u']['reference'] = model.reference
     attrib['u']['model'] = model.name
     attrib['u']['units'] = 'cm/s'
-    attrib['u']['long_name'] = 'zonal_tidal_current'
+    attrib['u']['long_name'] = model.long_name['u']
     attrib['u']['_FillValue'] = fill_value
     # meridional tidal currents
     attrib['v'] = {}
-    attrib['v']['description'] = ('depth_averaged_tidal_meridional_current_'
-        'from_harmonic_constants')
+    attrib['v']['description'] = model.description['v']
     attrib['v']['reference'] =  model.reference
     attrib['v']['model'] = model.name
     attrib['v']['units'] = 'cm/s'
-    attrib['v']['long_name'] = 'meridional_tidal_current'
+    attrib['v']['long_name'] = model.long_name['v']
     attrib['v']['_FillValue'] = fill_value
     # time
     attrib['time'] = {}
     attrib['time']['long_name'] = 'Time'
     attrib['time']['units'] = 'days since 1992-01-01T00:00:00'
     attrib['time']['calendar'] = 'standard'
 
@@ -282,65 +283,29 @@
 
     # extract time units from netCDF4 and HDF5 attributes or from TIME_UNITS
     try:
         time_string = dinput['attributes']['time']['units']
         epoch1, to_secs = pyTMD.time.parse_date_string(time_string)
     except (TypeError, KeyError, ValueError):
         epoch1, to_secs = pyTMD.time.parse_date_string(TIME_UNITS)
-    # convert time to seconds
-    if (TIME_STANDARD.lower() != 'datetime'):
-        delta_time = to_secs*dinput['time'].flatten()
-
-    # calculate leap seconds if specified
-    if (TIME_STANDARD.upper() == 'GPS'):
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    elif (TIME_STANDARD.upper() == 'LORAN'):
-        # LORAN time is ahead of GPS time by 9 seconds
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(-9.0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time-9.0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    elif (TIME_STANDARD.upper() == 'TAI'):
-        # TAI time is ahead of GPS time by 19 seconds
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(-19.0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time-19.0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    else:
-        leap_seconds = 0.0
 
-    # convert delta times or datetimes objects
+    # convert delta times or datetimes objects to timescale
     if (TIME_STANDARD.lower() == 'datetime'):
-        # convert delta time array from datetime object
-        # to days relative to 1992-01-01T00:00:00
-        tide_time = pyTMD.time.convert_datetime(dinput['time'].flatten(),
-            epoch=pyTMD.time._tide_epoch)/86400.0
+        timescale = pyTMD.time.timescale().from_datetime(
+            dinput['time'].flatten())
     else:
-        # convert time from units to days since 1992-01-01T00:00:00
-        tide_time = pyTMD.time.convert_delta_time(delta_time-leap_seconds,
-            epoch1=epoch1, epoch2=pyTMD.time._tide_epoch, scale=1.0/86400.0)
+        # convert time to seconds
+        delta_time = to_secs*dinput['time'].flatten()
+        timescale = pyTMD.time.timescale().from_deltatime(delta_time,
+            epoch=epoch1, standard=TIME_STANDARD)
     # number of time points
-    nt = len(tide_time)
-    # delta time (TT - UT1) file
-    delta_file = pyTMD.utilities.get_data_path(['data','merged_deltat.data'])
+    nt = len(timescale)
 
     # python dictionary with output data
-    output = {'time':tide_time, 'lon':lon, 'lat':lat}
+    output = {'time':timescale.tide, 'lon':lon, 'lat':lat}
     # iterate over u and v currents
     for t in model.type:
         # read tidal constants and interpolate to grid points
         if model.format in ('OTIS','ATLAS','ESR'):
             amp,ph,D,c = pyTMD.io.OTIS.extract_constants(lon.flatten(), lat.flatten(),
                 model.grid_file, model.model_file['u'], model.projection,
                 type=t, method=METHOD, extrapolate=EXTRAPOLATE, cutoff=CUTOFF,
@@ -355,51 +320,51 @@
         elif (model.format == 'FES'):
             amp,ph = pyTMD.io.FES.extract_constants(lon.flatten(), lat.flatten(),
                 model.model_file[t], type=t, version=model.version,
                 method=METHOD, extrapolate=EXTRAPOLATE, cutoff=CUTOFF,
                 scale=model.scale, compressed=model.compressed)
             # available model constituents
             c = model.constituents
-            # interpolate delta times from calendar dates to tide time
-            deltat = pyTMD.time.interpolate_delta_time(delta_file, tide_time)
+            # delta time (TT - UT1)
+            deltat = timescale.tt_ut1
 
         # calculate complex phase in radians for Euler's
         cph = -1j*ph*np.pi/180.0
         # calculate constituent oscillation
         hc = amp*np.exp(cph)
 
         # predict tidal currents at time and infer minor corrections
         if (TYPE == 'grid'):
             output[t] = np.ma.zeros((ny,nx,nt),fill_value=fill_value)
             output[t].mask = np.zeros((ny,nx,nt),dtype=bool)
             for i in range(nt):
-                TIDE = pyTMD.predict.map(tide_time[i], hc, c,
+                TIDE = pyTMD.predict.map(timescale.tide[i], hc, c,
                     deltat=deltat[i], corrections=model.format)
-                MINOR = pyTMD.predict.infer_minor(tide_time[i], hc, c,
+                MINOR = pyTMD.predict.infer_minor(timescale.tide[i], hc, c,
                     deltat=deltat[i], corrections=model.format)
                 # add major and minor components and reform grid
                 output[t][:,:,i] = np.reshape((TIDE+MINOR), (ny,nx))
                 output[t].mask[:,:,i] = np.reshape((TIDE.mask | MINOR.mask),
                     (ny,nx))
         elif (TYPE == 'drift'):
             output[t] = np.ma.zeros((nt), fill_value=fill_value)
             output[t].mask = np.any(hc.mask,axis=1)
-            output[t].data[:] = pyTMD.predict.drift(tide_time, hc, c,
+            output[t].data[:] = pyTMD.predict.drift(timescale.tide, hc, c,
                 deltat=deltat, corrections=model.format)
-            minor = pyTMD.predict.infer_minor(tide_time, hc, c,
+            minor = pyTMD.predict.infer_minor(timescale.tide, hc, c,
                 deltat=deltat, corrections=model.format)
             output[t].data[:] += minor.data[:]
         elif (TYPE == 'time series'):
             output[t] = np.ma.zeros((nstation,nt),fill_value=fill_value)
             output[t].mask = np.zeros((nstation,nt),dtype=bool)
             for s in range(nstation):
                 # calculate constituent oscillation for station
-                TIDE = pyTMD.predict.time_series(tide_time, hc[s,None,:], c,
+                TIDE = pyTMD.predict.time_series(timescale.tide, hc[s,None,:], c,
                     deltat=deltat, corrections=model.format)
-                MINOR = pyTMD.predict.infer_minor(tide_time, hc[s,None,:], c,
+                MINOR = pyTMD.predict.infer_minor(timescale.tide, hc[s,None,:], c,
                     deltat=deltat, corrections=model.format)
                 output[t].data[s,:] = TIDE.data[:] + MINOR.data[:]
                 output[t].mask[s,:] = (TIDE.mask | MINOR.mask)
         # replace invalid values with fill value
         output[t].data[output[t].mask] = output[t].fill_value
 
     # output to file
@@ -414,54 +379,53 @@
     elif (FORMAT == 'geotiff'):
         # merge current variables into a single variable
         output['data'] = np.concatenate((output['u'],output['v']),axis=-1)
         attrib['data'] = {'_FillValue':fill_value}
         pyTMD.spatial.to_geotiff(output, attrib, output_file,
             varname='data')
     # change the permissions level to MODE
-    os.chmod(output_file, MODE)
+    output_file.chmod(MODE)
 
 # PURPOSE: create argument parser
 def arguments():
     parser = argparse.ArgumentParser(
         description="""Calculates zonal and meridional tidal currents for
             an input file
             """,
         fromfile_prefix_chars="@"
     )
     parser.convert_arg_line_to_args = pyTMD.utilities.convert_arg_line_to_args
-    # command line options
     group = parser.add_mutually_exclusive_group(required=True)
+    # command line options
     # input and output file
     parser.add_argument('infile',
-        type=lambda p: os.path.abspath(os.path.expanduser(p)), nargs='?',
+        type=pathlib.Path, nargs='?',
         help='Input file to run')
     parser.add_argument('outfile',
-        type=lambda p: os.path.abspath(os.path.expanduser(p)), nargs='?',
+        type=pathlib.Path, nargs='?',
         help='Computed output file')
     # set data directory containing the tidal data
     parser.add_argument('--directory','-D',
-        type=lambda p: os.path.abspath(os.path.expanduser(p)),
-        default=os.getcwd(),
+        type=pathlib.Path,
         help='Working data directory')
     # tide model to use
     choices = sorted(pyTMD.io.model.ocean_current())
     group.add_argument('--tide','-T',
         type=str, choices=choices,
         help='Tide model to use in calculating currents')
     parser.add_argument('--atlas-format',
         type=str, choices=('OTIS','netcdf'), default='netcdf',
         help='ATLAS tide model format')
     parser.add_argument('--gzip','-G',
         default=False, action='store_true',
         help='Tide model files are gzip compressed')
     # tide model definition file to set an undefined model
     group.add_argument('--definition-file',
-        type=lambda p: os.path.abspath(os.path.expanduser(p)),
-        help='Tide model definition file for use in calculating currents')
+        type=pathlib.Path,
+        help='Tide model definition file')
     # input and output data format
     parser.add_argument('--format','-F',
         type=str, default='csv', choices=('csv','netCDF4','HDF5','geotiff'),
         help='Input and output data format')
     # variable names (for csv names of columns)
     parser.add_argument('--variables','-v',
         type=str, nargs='+', default=['time','lat','lon','data'],
@@ -529,16 +493,15 @@
 def main():
     # Read the system arguments listed after the program
     parser = arguments()
     args,_ = parser.parse_known_args()
 
     # set output file from input filename if not entered
     if not args.outfile:
-        fileBasename,fileExtension = os.path.splitext(args.infile)
-        vars = (fileBasename,args.tide,'_currents',fileExtension)
+        vars = (args.infile.stem,args.tide,'_currents',args.infile.suffix)
         args.outfile = '{0}_{1}{2}{3}'.format(*vars)
 
     # run tidal current program for input file
     compute_tidal_currents(args.directory, args.infile, args.outfile,
         TIDE_MODEL=args.tide,
         ATLAS_FORMAT=args.atlas_format,
         GZIP=args.gzip,
```

### Comparing `pyTMD-2.0.3/scripts/compute_tidal_elevations.py` & `pyTMD-2.0.4/scripts/compute_tidal_elevations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 compute_tidal_elevations.py
-Written by Tyler Sutterley (04/2023)
+Written by Tyler Sutterley (05/2023)
 Calculates tidal elevations for an input file
 
 Uses OTIS format tidal solutions provided by Ohio State University and ESR
     http://volkov.oce.orst.edu/tides/region.html
     https://www.esr.org/research/polar-tide-models/list-of-polar-tide-models/
     ftp://ftp.esr.org/pub/datasets/tmd/
 Global Tide Model (GOT) solutions provided by Richard Ray at GSFC
@@ -78,27 +78,29 @@
     pyproj: Python interface to PROJ library
         https://pypi.org/project/pyproj/
 
 PROGRAM DEPENDENCIES:
     time.py: utilities for calculating time operations
     spatial: utilities for reading, writing and operating on spatial data
     utilities.py: download and management utilities for syncing files
+    arguments.py: load the nodal corrections for tidal constituents
     astro.py: computes the basic astronomical mean longitudes
     convert_crs.py: convert points to and from Coordinates Reference Systems
     load_constituent.py: loads parameters for a given tidal constituent
-    load_nodal_corrections.py: load the nodal corrections for tidal constituents
     io/model.py: retrieves tide model parameters for named tide models
     io/OTIS.py: extract tidal harmonic constants from OTIS tide models
     io/ATLAS.py: extract tidal harmonic constants from netcdf models
     io/FES.py: extract tidal harmonic constants from FES tide models
     interpolate.py: interpolation routines for spatial data
     predict.py: predict tidal values using harmonic constants
 
 UPDATE HISTORY:
+    Updated 05/2023: use timescale class for time conversion operations
     Updated 04/2023: check if datetime before converting to seconds
+        using pathlib to define and expand paths
     Updated 02/2023: added functionality for time series type
     Updated 01/2023: added default field mapping for reading from netCDF4/HDF5
         added data type keyword for netCDF4 output
     Updated 12/2022: single implicit import of pyTMD tools
     Updated 11/2022: place some imports within try/except statements
         use f-strings for formatting verbose or ascii output
     Updated 10/2022: added delimiter option and datetime parsing for ascii files
@@ -134,16 +136,16 @@
     Updated 09/2019: added TPXO9_atlas reading from netcdf4 tide files
     Updated 07/2018: added GSFC Global Ocean Tides (GOT) models
     Written 10/2017 for public release
 """
 from __future__ import print_function
 
 import sys
-import os
 import logging
+import pathlib
 import warnings
 import argparse
 import numpy as np
 import pyTMD
 
 # attempt imports
 try:
@@ -208,15 +210,14 @@
 
     # get parameters for tide model
     if DEFINITION_FILE is not None:
         model = pyTMD.io.model(tide_dir).from_file(DEFINITION_FILE)
     else:
         model = pyTMD.io.model(tide_dir, format=ATLAS_FORMAT,
             compressed=GZIP).elevation(TIDE_MODEL)
-    output_variable = model.variable
 
     # invalid value
     fill_value = -9999.0
     # output netCDF4 and HDF5 file attributes
     # will be added to YAML header in csv files
     attrib = {}
     # latitude
@@ -224,14 +225,15 @@
     attrib['lat']['long_name'] = 'Latitude'
     attrib['lat']['units'] = 'Degrees_North'
     # longitude
     attrib['lon'] = {}
     attrib['lon']['long_name'] = 'Longitude'
     attrib['lon']['units'] = 'Degrees_East'
     # tides
+    output_variable = model.variable
     attrib[output_variable] = {}
     attrib[output_variable]['description'] = model.description
     attrib[output_variable]['reference'] = model.reference
     attrib[output_variable]['model'] = model.name
     attrib[output_variable]['units'] = 'meters'
     attrib[output_variable]['long_name'] = model.long_name
     attrib[output_variable]['_FillValue'] = fill_value
@@ -279,61 +281,26 @@
 
     # extract time units from netCDF4 and HDF5 attributes or from TIME_UNITS
     try:
         time_string = dinput['attributes']['time']['units']
         epoch1, to_secs = pyTMD.time.parse_date_string(time_string)
     except (TypeError, KeyError, ValueError):
         epoch1, to_secs = pyTMD.time.parse_date_string(TIME_UNITS)
-    # convert time to seconds
-    if (TIME_STANDARD.lower() != 'datetime'):
-        delta_time = to_secs*dinput['time'].flatten()
-
-    # calculate leap seconds if specified
-    if (TIME_STANDARD.upper() == 'GPS'):
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    elif (TIME_STANDARD.upper() == 'LORAN'):
-        # LORAN time is ahead of GPS time by 9 seconds
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(-9.0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time-9.0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    elif (TIME_STANDARD.upper() == 'TAI'):
-        # TAI time is ahead of GPS time by 19 seconds
-        GPS_Epoch_Time = pyTMD.time.convert_delta_time(-19.0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        GPS_Time = pyTMD.time.convert_delta_time(delta_time-19.0, epoch1=epoch1,
-            epoch2=pyTMD.time._gps_epoch, scale=1.0)
-        # calculate difference in leap seconds from start of epoch
-        leap_seconds = pyTMD.time.count_leap_seconds(GPS_Time) - \
-            pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
-    else:
-        leap_seconds = 0.0
 
+    # convert delta times or datetimes objects to timescale
     if (TIME_STANDARD.lower() == 'datetime'):
-        # convert delta time array from datetime object
-        # to days relative to 1992-01-01T00:00:00
-        tide_time = pyTMD.time.convert_datetime(dinput['time'].flatten(),
-            epoch=pyTMD.time._tide_epoch)/86400.0
+        timescale = pyTMD.time.timescale().from_datetime(
+            dinput['time'].flatten())
     else:
-        # convert time from units to days since 1992-01-01T00:00:00
-        tide_time = pyTMD.time.convert_delta_time(delta_time-leap_seconds,
-            epoch1=epoch1, epoch2=pyTMD.time._tide_epoch, scale=1.0/86400.0)
+        # convert time to seconds
+        delta_time = to_secs*dinput['time'].flatten()
+        timescale = pyTMD.time.timescale().from_deltatime(delta_time,
+            epoch=epoch1, standard=TIME_STANDARD)
     # number of time points
-    nt = len(tide_time)
-    # delta time (TT - UT1) file
-    delta_file = pyTMD.utilities.get_data_path(['data','merged_deltat.data'])
+    nt = len(timescale)
 
     # read tidal constants and interpolate to grid points
     if model.format in ('OTIS','ATLAS','ESR'):
         amp,ph,D,c = pyTMD.io.OTIS.extract_constants(lon.flatten(), lat.flatten(),
             model.grid_file, model.model_file, model.projection,
             type=model.type, method=METHOD, extrapolate=EXTRAPOLATE,
             cutoff=CUTOFF, grid=model.format, apply_flexure=APPLY_FLEXURE)
@@ -344,102 +311,101 @@
             method=METHOD, extrapolate=EXTRAPOLATE, cutoff=CUTOFF,
             scale=model.scale, compressed=model.compressed)
         deltat = np.zeros((nt))
     elif (model.format == 'GOT'):
         amp,ph,c = pyTMD.io.GOT.extract_constants(lon.flatten(), lat.flatten(),
             model.model_file, method=METHOD, extrapolate=EXTRAPOLATE,
             cutoff=CUTOFF, scale=model.scale, compressed=model.compressed)
-        # interpolate delta times from calendar dates to tide time
-        deltat = pyTMD.time.interpolate_delta_time(delta_file, tide_time)
+        # delta time (TT - UT1)
+        deltat = timescale.tt_ut1
     elif (model.format == 'FES'):
         amp,ph = pyTMD.io.FES.extract_constants(lon.flatten(), lat.flatten(),
             model.model_file, type=model.type, version=model.version,
             method=METHOD, extrapolate=EXTRAPOLATE, cutoff=CUTOFF,
             scale=model.scale, compressed=model.compressed)
         # available model constituents
         c = model.constituents
-        # interpolate delta times from calendar dates to tide time
-        deltat = pyTMD.time.interpolate_delta_time(delta_file, tide_time)
+        # delta time (TT - UT1)
+        deltat = timescale.tt_ut1
 
     # calculate complex phase in radians for Euler's
     cph = -1j*ph*np.pi/180.0
     # calculate constituent oscillation
     hc = amp*np.exp(cph)
 
     # predict tidal elevations at time and infer minor corrections
     if (TYPE == 'grid'):
         tide = np.ma.zeros((ny,nx,nt),fill_value=fill_value)
         tide.mask = np.zeros((ny,nx,nt),dtype=bool)
         for i in range(nt):
-            TIDE = pyTMD.predict.map(tide_time[i], hc, c,
+            TIDE = pyTMD.predict.map(timescale.tide[i], hc, c,
                 deltat=deltat[i], corrections=model.format)
-            MINOR = pyTMD.predict.infer_minor(tide_time[i], hc, c,
+            MINOR = pyTMD.predict.infer_minor(timescale.tide[i], hc, c,
                 deltat=deltat[i], corrections=model.format)
             # add major and minor components and reform grid
             tide[:,:,i] = np.reshape((TIDE+MINOR), (ny,nx))
             tide.mask[:,:,i] = np.reshape((TIDE.mask | MINOR.mask), (ny,nx))
     elif (TYPE == 'drift'):
         tide = np.ma.zeros((nt), fill_value=fill_value)
         tide.mask = np.any(hc.mask,axis=1)
-        tide.data[:] = pyTMD.predict.drift(tide_time, hc, c,
+        tide.data[:] = pyTMD.predict.drift(timescale.tide, hc, c,
             deltat=deltat, corrections=model.format)
-        minor = pyTMD.predict.infer_minor(tide_time, hc, c,
+        minor = pyTMD.predict.infer_minor(timescale.tide, hc, c,
             deltat=deltat, corrections=model.format)
         tide.data[:] += minor.data[:]
     elif (TYPE == 'time series'):
         tide = np.ma.zeros((nstation,nt),fill_value=fill_value)
         tide.mask = np.zeros((nstation,nt),dtype=bool)
         for s in range(nstation):
             # calculate constituent oscillation for station
-            TIDE = pyTMD.predict.time_series(tide_time, hc[s,None,:], c,
+            TIDE = pyTMD.predict.time_series(timescale.tide, hc[s,None,:], c,
                 deltat=deltat, corrections=model.format)
-            MINOR = pyTMD.predict.infer_minor(tide_time, hc[s,None,:], c,
+            MINOR = pyTMD.predict.infer_minor(timescale.tide, hc[s,None,:], c,
                 deltat=deltat, corrections=model.format)
             tide.data[s,:] = TIDE.data[:] + MINOR.data[:]
             tide.mask[s,:] = (TIDE.mask | MINOR.mask)
     # replace invalid values with fill value
     tide.data[tide.mask] = tide.fill_value
 
     # output to file
-    output = {'time':tide_time, 'lon':lon, 'lat':lat, output_variable:tide}
+    output = {'time':timescale.tide, 'lon':lon, 'lat':lat, output_variable:tide}
     if (FORMAT == 'csv'):
         pyTMD.spatial.to_ascii(output, attrib, output_file,
             delimiter=DELIMITER, header=False,
             columns=['time','lat','lon',output_variable])
     elif (FORMAT == 'netCDF4'):
         pyTMD.spatial.to_netCDF4(output, attrib, output_file, data_type=TYPE)
     elif (FORMAT == 'HDF5'):
         pyTMD.spatial.to_HDF5(output, attrib, output_file)
     elif (FORMAT == 'geotiff'):
         pyTMD.spatial.to_geotiff(output, attrib, output_file,
             varname=output_variable)
     # change the permissions level to MODE
-    os.chmod(output_file, MODE)
+    output_file.chmod(MODE)
 
 # PURPOSE: create argument parser
 def arguments():
     parser = argparse.ArgumentParser(
         description="""Calculates tidal elevations for an input file
             """,
         fromfile_prefix_chars="@"
     )
     parser.convert_arg_line_to_args = pyTMD.utilities.convert_arg_line_to_args
-    # command line options
     group = parser.add_mutually_exclusive_group(required=True)
+    # command line options
     # input and output file
     parser.add_argument('infile',
-        type=lambda p: os.path.abspath(os.path.expanduser(p)), nargs='?',
+        type=pathlib.Path, nargs='?',
         help='Input file to run')
     parser.add_argument('outfile',
-        type=lambda p: os.path.abspath(os.path.expanduser(p)), nargs='?',
+        type=pathlib.Path, nargs='?',
         help='Computed output file')
     # set data directory containing the tidal data
     parser.add_argument('--directory','-D',
-        type=lambda p: os.path.abspath(os.path.expanduser(p)),
-        default=os.getcwd(),
+        type=pathlib.Path,
         help='Working data directory')
     # tide model to use
     choices = sorted(pyTMD.io.model.ocean_elevation() +
                      pyTMD.io.model.load_elevation())
     group.add_argument('--tide','-T',
         type=str, choices=choices,
         help='Tide model to use in correction')
@@ -447,16 +413,16 @@
         type=str, choices=('OTIS','netcdf'), default='netcdf',
         help='ATLAS tide model format')
     parser.add_argument('--gzip','-G',
         default=False, action='store_true',
         help='Tide model files are gzip compressed')
     # tide model definition file to set an undefined model
     group.add_argument('--definition-file',
-        type=lambda p: os.path.abspath(os.path.expanduser(p)),
-        help='Tide model definition file for use as correction')
+        type=pathlib.Path,
+        help='Tide model definition file')
     # input and output data format
     parser.add_argument('--format','-F',
         type=str, default='csv', choices=('csv','netCDF4','HDF5','geotiff'),
         help='Input and output data format')
     # variable names (for csv names of columns)
     parser.add_argument('--variables','-v',
         type=str, nargs='+', default=['time','lat','lon','data'],
@@ -528,17 +494,16 @@
 def main():
     # Read the system arguments listed after the program
     parser = arguments()
     args,_ = parser.parse_known_args()
 
     # set output file from input filename if not entered
     if not args.outfile:
-        fileBasename,fileExtension = os.path.splitext(args.infile)
         flexure_flag = '_FLEXURE' if args.apply_flexure else ''
-        vars = (fileBasename,args.tide,flexure_flag,fileExtension)
+        vars = (args.infile.stem,args.tide,flexure_flag,args.infile.suffix)
         args.outfile = '{0}_{1}{2}{3}'.format(*vars)
 
     # run tidal elevation program for input file
     compute_tidal_elevations(args.directory, args.infile, args.outfile,
         TIDE_MODEL=args.tide,
         ATLAS_FORMAT=args.atlas_format,
         GZIP=args.gzip,
```

### Comparing `pyTMD-2.0.3/scripts/reduce_OTIS_files.py` & `pyTMD-2.0.4/scripts/reduce_OTIS_files.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 reduce_OTIS_files.py
-Written by Tyler Sutterley (12/2022)
+Written by Tyler Sutterley (04/2023)
 Read OTIS-format tidal files and reduce to a regional subset
 
 COMMAND LINE OPTIONS:
     -D X, --directory X: working data directory
     -T X, --tide X: Tide model to use
     -B X, --bounds X: Grid Bounds (xmin,xmax,ymin,ymax)
     --projection X: spatial projection of bounds as EPSG code or PROJ4 string
@@ -24,14 +24,15 @@
 PROGRAM DEPENDENCIES:
     io/model.py: retrieves tide model parameters for named tide models
     io/OTIS.py: extract tidal harmonic constants from OTIS tide models
     utilities.py: download and management utilities for syncing files
     convert_crs.py: converts lat/lon points to and from projected coordinates
 
 UPDATE HISTORY:
+    Updated 04/2023: using pathlib to define and expand paths
     Updated 03/2023: new function name for coordinate reference systems
     Updated 12/2022: refactored OTIS model input and output
     Updated 11/2022: place some imports within try/except statements
         use f-strings for formatting verbose or ascii output
     Updated 05/2022: updated keyword arguments to read tide model programs
     Updated 04/2022: use argparse descriptions within documentation
     Updated 11/2021: add function for attempting to extract projection
@@ -45,15 +46,15 @@
         Program Data Center http://www.usap-dc.org/view/dataset/601235
     Updated 11/2019: added AOTIM-5-2018 tide model (2018 update to 2004 model)
     Written 08/2018
 """
 from __future__ import print_function
 
 import sys
-import os
+import pathlib
 import warnings
 import argparse
 import numpy as np
 import pyTMD.io
 import pyTMD.utilities
 from pyTMD.convert_crs import convert_crs
 
@@ -85,15 +86,15 @@
     # no projection can be made
     raise pyproj.exceptions.CRSError
 
 # PURPOSE: reads OTIS-format tidal files and reduces to a regional subset
 def make_regional_OTIS_files(tide_dir, TIDE_MODEL, BOUNDS=4*[None],
     PROJECTION='4326', MODE=0o775):
     # get parameters for tide model
-    model = pyTMD.io.model(directory=tide_dir).elevation(TIDE_MODEL)
+    model = pyTMD.io.model(directory=tide_dir).grid(TIDE_MODEL)
     # directionaries with input and output files
     model_file = {}
     new_model_file = {}
 
     # read the OTIS-format tide grid file
     if (model.format == 'ATLAS'):
         # if reading a global solution with localized solutions
@@ -134,21 +135,21 @@
     mz1 = np.zeros((ny,nx),dtype='>i4')
     hz1[:,:] = hz[indy,indx].reshape(ny,nx)
     mz1[:,:] = mz[indy,indx].reshape(ny,nx)
     # output reduced grid to file
     new_grid_file = create_unique_filename(model.grid_file)
     pyTMD.io.OTIS.output_otis_grid(new_grid_file,xlim,ylim,hz1,mz1,iob,dt)
     # change the permissions level to MODE
-    os.chmod(new_grid_file, MODE)
+    new_grid_file.chmod(MODE)
 
     # combine ATLAS sub-grids into single output grid
     # reduce elevation files to bounds
     try:
         # get parameters for tide model
-        model = pyTMD.io.model(tide_dir).elevation(TIDE_MODEL)
+        model = model.elevation(TIDE_MODEL)
     except Exception as exc:
         pass
     else:
         # read each constituent
         constituents,nc = pyTMD.io.OTIS.read_constituents(model_file['z'])
         z1 = np.zeros((ny,nx,nc),dtype=np.complex64)
         for i,c in enumerate(constituents):
@@ -163,21 +164,21 @@
             # reduce elevation to new bounds
             z1[:,:,i] = z[indy,indx].reshape(ny,nx)
         # output reduced elevation components
         new_model_file['z'] = create_unique_filename(model_file['z'])
         pyTMD.io.OTIS.output_otis_elevation(new_model_file['z'], z1,
             xlim, ylim, constituents)
         # change the permissions level to MODE
-        os.chmod(new_model_file['z'], MODE)
+        new_model_file['z'].chmod(MODE)
 
     # combine ATLAS sub-grids into single output grid
     # reduce transport files to bounds
     try:
         # get parameters for tide model
-        model = pyTMD.io.model(tide_dir).current(TIDE_MODEL)
+        model = model.current(TIDE_MODEL)
     except Exception as exc:
         pass
     else:
         # read each constituent
         constituents,nc = pyTMD.io.OTIS.read_constituents(model_file['u'])
         u1 = np.zeros((ny,nx,nc),dtype=np.complex64)
         v1 = np.zeros((ny,nx,nc),dtype=np.complex64)
@@ -196,54 +197,53 @@
             u1[:,:,i] = u[indy,indx].reshape(ny,nx)
             v1[:,:,i] = v[indy,indx].reshape(ny,nx)
         # output reduced transport components
         new_model_file['uv'] = create_unique_filename(model_file['u'])
         pyTMD.io.OTIS.output_otis_transport(new_model_file['u'], u1, v1,
             xlim, ylim, constituents)
         # change the permissions level to MODE
-        os.chmod(new_model_file['u'], MODE)
+        new_model_file['u'].chmod(MODE)
 
 # PURPOSE: create a unique filename adding a numerical instance if existing
 def create_unique_filename(filename):
-    # split filename into fileBasename and fileExtension
-    fileBasename, fileExtension = os.path.splitext(filename)
-    fileExtension = '' if (fileExtension in ('.out','.oce')) else fileExtension
+    # split filename into parts
+    filename = pathlib.Path(filename)
+    basename = filename.stem
+    suffix = '' if (filename.suffix in ('.out','.oce')) else filename.suffix
     # replace extension with reduced flag
-    filename = '{0}{1}{2}'.format(fileBasename, fileExtension, '.reduced')
+    filename = filename.with_name(f'{basename}{suffix}.reduced')
     # create counter to add to the end of the filename if existing
     counter = 1
     while counter:
         try:
             # open file descriptor only if the file doesn't exist
-            fd = os.open(filename, os.O_CREAT | os.O_EXCL | os.O_RDWR)
+            fd = filename.open(mode='xb')
         except OSError:
             pass
         else:
             # close the file descriptor and return the filename
-            os.close(fd)
+            fd.close()
             return filename
         # new filename adds counter
-        args = (fileBasename, fileExtension, '.reduced', counter)
-        filename = '{0}{1}{2}_{3:d}'.format(*args)
+        filename = filename.with_name(f'{basename}{suffix}.reduced_{counter:d}')
         counter += 1
 
 # PURPOSE: create argument parser
 def arguments():
     parser = argparse.ArgumentParser(
         description="""Read OTIS-format tidal files and reduce to a regional
             subset
             """,
         fromfile_prefix_chars="@"
     )
     parser.convert_arg_line_to_args = pyTMD.utilities.convert_arg_line_to_args
     # command line options
     # set data directory containing the tidal data
     parser.add_argument('--directory','-D',
-        type=lambda p: os.path.abspath(os.path.expanduser(p)),
-        default=os.getcwd(),
+        type=pathlib.Path, default=pathlib.Path.cwd(),
         help='Working data directory')
     # tide model to use
     model_choices = ('CATS0201','CATS2008','CATS2008_load','TPXO9-atlas',
         'TPXO9.1','TPXO8-atlas','TPXO7.2','TPXO7.2_load','AODTM-5','AOTIM-5',
         'AOTIM-5-2018')
     parser.add_argument('--tide','-T',
         metavar='TIDE', type=str, default='TPXO9.1',
```

### Comparing `pyTMD-2.0.3/scripts/usap_cats_tides.py` & `pyTMD-2.0.4/scripts/usap_cats_tides.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 usap_cats_tides.py
-Written by Tyler Sutterley (11/2022)
+Written by Tyler Sutterley (04/2023)
 Download Circum-Antarctic Tidal Simulations from the US Antarctic Program
 CATS2008: https://www.usap-dc.org/view/dataset/601235
 
 NOTE: USAP now requires a captcha to download datasets
 
 CALLING SEQUENCE:
     python usap_cats_tides.py --tide=CATS2008
@@ -21,29 +21,30 @@
     future: Compatibility layer between Python 2 and Python 3
         https://python-future.org/
 
 PROGRAM DEPENDENCIES:
     utilities.py: download and management utilities for syncing files
 
 UPDATE HISTORY:
+    Updated 04/2023: using pathlib to define and expand paths
     Updated 11/2022: use f-strings for formatting verbose or ascii output
     Updated 04/2022: use argparse descriptions within documentation
     Updated 10/2021: using python logging for handling verbose output
     Updated 08/2021: USAP now requires captchas for dataset downloads
     Updated 07/2021: can use prefix files to define command line arguments
     Updated 10/2020: using argparse to set command line parameters
     Written 08/2020
 """
 from __future__ import print_function
 
 import sys
-import os
 import re
 import time
 import logging
+import pathlib
 import zipfile
 import warnings
 import argparse
 import posixpath
 import webbrowser
 import pyTMD.utilities
 
@@ -57,41 +58,42 @@
     REMOTE = {}
     REMOTE['CATS2008'] = ['601235','2019-12-19T23:26:43.6Z',
         'CATS2008.zip?dataset_id=601235']
     # local subdirectory for each model
     LOCAL = {}
     LOCAL['CATS2008'] = 'CATS2008'
     # recursively create directories if non-existent
-    if not os.access(os.path.join(DIRECTORY,LOCAL[MODEL]), os.F_OK):
-        os.makedirs(os.path.join(DIRECTORY,LOCAL[MODEL]), MODE)
+    DIRECTORY = pathlib.Path(DIRECTORY).expanduser().absolute()
+    local_dir = DIRECTORY.joinpath(LOCAL[MODEL])
+    local_dir.mkdir(MODE, parents=True, exist_ok=True)
 
     # USAP now requires a captcha to download datasets
     # use a manual download until USAP allows some sort of verification
     DATASET = {}
     DATASET['CATS2008'] = ['https://www.usap-dc.org','view','dataset','601235']
     # open USAP url in a new browser window
     webbrowser.open_new_tab(posixpath.join(*DATASET[MODEL]))
-    pyTMD.utilities.file_opener(os.path.join(DIRECTORY,LOCAL[MODEL]))
+    pyTMD.utilities.file_opener(local_dir)
     return
 
     # download CATS2008 zip file and read as virtual file object
     HOST = ['https://www.usap-dc.org','dataset','usap-dc',*REMOTE[MODEL]]
     # download zipfile from host
     zfile = zipfile.ZipFile(pyTMD.utilities.from_http(HOST))
     logger.info('{0} -->\n'.format(posixpath.join(*HOST)))
     # extract each member
     for m in zfile.filelist:
         # strip directories from member filename
         m.filename = posixpath.basename(m.filename)
-        local_file = os.path.join(DIRECTORY,LOCAL[MODEL],m.filename)
-        logger.info(f'\t{local_file}\n')
+        local_file = local_dir.joinpath(m.filename)
+        logger.info(f'\t{str(local_file)}\n')
         # extract file
-        zfile.extract(m, path=os.path.join(DIRECTORY,LOCAL[MODEL]))
+        zfile.extract(m, path=local_dir)
         # change permissions mode
-        os.chmod(local_file, MODE)
+        local_file.chmod(MODE)
     # close the zipfile object
     zfile.close()
 
 # PURPOSE: create argument parser
 def arguments():
     parser = argparse.ArgumentParser(
         description="""Download Circum-Antarctic Tidal Simulations from the
@@ -99,16 +101,15 @@
             """,
         fromfile_prefix_chars="@"
     )
     parser.convert_arg_line_to_args = pyTMD.utilities.convert_arg_line_to_args
     # command line parameters
     # working data directory for location of tide models
     parser.add_argument('--directory','-D',
-        type=lambda p: os.path.abspath(os.path.expanduser(p)),
-        default=os.getcwd(),
+        type=pathlib.Path, default=pathlib.Path.cwd(),
         help='Working data directory')
     # Antarctic Ocean tide model to download
     parser.add_argument('--tide','-T',
         metavar='TIDE', type=str, nargs='+', default=['CATS2008'],
         choices=('CATS2008',),
         help='Circum-Antarctic tide model to download')
     # permissions mode of the local directories and files (number in octal)
@@ -127,12 +128,12 @@
     # warn user that USAP requires a reCAPTCHA check
     warnings.filterwarnings("module")
     warnings.warn("Deprecated. USAP now requires captcha", DeprecationWarning)
     warnings.filterwarnings("ignore")
     # check internet connection before attempting to run program
     if pyTMD.utilities.check_connection('https://www.usap-dc.org'):
         for m in args.tide:
-            usap_cats_tides(m,DIRECTORY=args.directory,MODE=args.mode)
+            usap_cats_tides(m, DIRECTORY=args.directory, MODE=args.mode)
 
 # run main program
 if __name__ == '__main__':
     main()
```

### Comparing `pyTMD-2.0.3/scripts/verify_box_tpxo.py` & `pyTMD-2.0.4/scripts/verify_box_tpxo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 verify_box_tpxo.py
-Written by Tyler Sutterley (01/2023)
+Written by Tyler Sutterley (04/2023)
 Verifies downloaded TPXO9-atlas global tide models from the box file
     sharing service
 
 CALLING SEQUENCE:
     python verify_box_tpxo.py --token <token> --tide TPXO9-atlas-v5
     where <username> is your box api access token
 
@@ -27,28 +27,29 @@
     future: Compatibility layer between Python 2 and Python 3
         https://python-future.org/
 
 REFERENCE:
     https://developer.box.com/guides/
 
 UPDATE HISTORY:
+    Updated 04/2023: using pathlib to define and expand paths
     Updated 01/2023: use default context from utilities module
     Updated 11/2022: use f-strings for formatting verbose or ascii output
     Updated 04/2022: use argparse descriptions within documentation
     Updated 12/2021: added TPXO9-atlas-v5 to list of available tide models
     Updated 10/2021: using python logging for handling verbose output
     Updated 07/2021: can use prefix files to define command line arguments
     Written 03/2021
 """
 from __future__ import print_function
 
-import os
 import re
 import json
 import logging
+import pathlib
 import argparse
 import posixpath
 import pyTMD.utilities
 
 # PURPOSE: create an opener for box with a supplied user access token
 def build_opener(token, context=pyTMD.utilities._default_ssl_context,
     redirect=True):
@@ -85,27 +86,29 @@
 def verify_box_tpxo(tide_dir, folder_id, TIDE_MODEL=None,
     CURRENTS=False, MODE=None):
 
     # create logger for verbosity level
     logger = pyTMD.utilities.build_logger(__name__, level=logging.INFO)
 
     # check if local directory exists and recursively create if not
+    tide_dir = pathlib.Path(tide_dir).expanduser().absolute()
     if (TIDE_MODEL == 'TPXO9-atlas'):
-        localpath = os.path.join(tide_dir,'TPXO9_atlas')
+        localpath = tide_dir.joinpath('TPXO9_atlas')
     elif (TIDE_MODEL == 'TPXO9-atlas-v2'):
-        localpath = os.path.join(tide_dir,'TPXO9_atlas_v2')
+        localpath = tide_dir.joinpath('TPXO9_atlas_v2')
     elif (TIDE_MODEL == 'TPXO9-atlas-v3'):
-        localpath = os.path.join(tide_dir,'TPXO9_atlas_v3')
+        localpath = tide_dir.joinpath('TPXO9_atlas_v3')
     elif (TIDE_MODEL == 'TPXO9-atlas-v4'):
-        localpath = os.path.join(tide_dir,'TPXO9_atlas_v4')
+        localpath = tide_dir.joinpath('TPXO9_atlas_v4')
     elif (TIDE_MODEL == 'TPXO9-atlas-v5'):
-        localpath = os.path.join(tide_dir,'TPXO9_atlas_v5')
+        localpath = tide_dir.joinpath('TPXO9_atlas_v5')
 
     # create output directory if non-existent
-    os.makedirs(localpath,MODE) if not os.path.exists(localpath) else None
+    localpath.mkdir(MODE, parents=True, exist_ok=True)
+
     # regular expression pattern for files of interest
     regex_patterns = []
     regex_patterns.append('grid')
     regex_patterns.append('h')
     if CURRENTS:
         regex_patterns.append('u')
     rx = re.compile(r'^({0})'.format(r'|'.join(regex_patterns)), re.VERBOSE)
@@ -130,41 +133,40 @@
         request = pyTMD.utilities.urllib2.Request(file_url)
         response = pyTMD.utilities.urllib2.urlopen(request)
         file_contents = json.loads(response.read())
         modified_at = file_contents['modified_at']
         remote_mtime = pyTMD.utilities.get_unix_time(modified_at,
             format='%Y-%m-%dT%H:%M:%S%z')
         # print file information
-        local = os.path.join(localpath,entry['name'])
-        logger.info(f'\t{local}')
+        local = localpath.joinpath(entry['name'])
+        logger.info(f'\t{str(local)}')
         # compare checksums to validate download
         sha1 = pyTMD.utilities.get_hash(local,algorithm='sha1')
         if sha1 != entry['sha1']:
             logger.critical(f'Remote checksum: {entry["sha1"]}')
             logger.critical(f'Local checksum: {sha1}')
             raise Exception('Checksum verification failed')
         # keep remote modification time of file and local access time
-        os.utime(local, (os.stat(local).st_atime, remote_mtime))
+        pathlib.os.utime(local, (local.stat().st_atime, remote_mtime))
         # change the permissions mode of the local file
-        os.chmod(local, MODE)
+        local.chmod(MODE)
 
 # PURPOSE: create argument parser
 def arguments():
     parser = argparse.ArgumentParser(
         description="""Verifies downloaded TPXO9-atlas global
             tide models from the box file sharing service
             """,
         fromfile_prefix_chars="@"
     )
     parser.convert_arg_line_to_args = pyTMD.utilities.convert_arg_line_to_args
     # command line parameters
     # working data directory
     parser.add_argument('--directory','-D',
-        type=lambda p: os.path.abspath(os.path.expanduser(p)),
-        default=os.getcwd(),
+        type=pathlib.Path, default=pathlib.Path.cwd(),
         help='Working data directory')
     # box user access token
     parser.add_argument('--token','-t',
         type=str, default='',
         help='User access token for box API')
     # box folder id
     parser.add_argument('--folder','-F',
```

### Comparing `pyTMD-2.0.3/setup.py` & `pyTMD-2.0.4/setup.py`

 * *Files identical despite different names*

