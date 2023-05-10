# Comparing `tmp/geofileops-0.8.0a3.tar.gz` & `tmp/geofileops-0.8.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geofileops-0.8.0a3.tar", last modified: Fri May  5 11:57:59 2023, max compression
+gzip compressed data, was "geofileops-0.8.0a4.tar", last modified: Wed May 10 09:08:33 2023, max compression
```

## Comparing `geofileops-0.8.0a3.tar` & `geofileops-0.8.0a4.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:59.370919 geofileops-0.8.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-05 11:57:59.370919 geofileops-0.8.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:59.354919 geofileops-0.8.0a3/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/benchmark/benchmark_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/benchmark/benchmark_geofileops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/benchmark/benchmarker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:59.354919 geofileops-0.8.0a3/benchmark/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/benchmark/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/benchmark/benchmarks/benchmarks_geofileops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/benchmark/benchmarks/testdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/benchmark/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:59.358919 geofileops-0.8.0a3/geofileops/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    84479 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/fileops.py
--rw-r--r--   0 runner    (1001) docker     (123)    90643 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/geoops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:59.358919 geofileops-0.8.0a3/geofileops/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/helpers/_parameter_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/helpers/layerstyles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:59.362919 geofileops-0.8.0a3/geofileops/util/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/_general_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    71319 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/_geoops_gpd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/_geoops_ogr.py
--rw-r--r--   0 runner    (1001) docker     (123)   101634 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/_geoops_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/_io_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/_ogr_sql_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    18218 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/_ogr_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/_processing_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    20519 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/_sqlite_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/geodataframe_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/geofiletype.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/geofiletypes.csv
--rw-r--r--   0 runner    (1001) docker     (123)    30107 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/geometry_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/geoseries_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/grid_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/util/test.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/geofileops/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:59.358919 geofileops-0.8.0a3/geofileops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-05 11:57:59.000000 geofileops-0.8.0a3/geofileops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-05 11:57:59.000000 geofileops-0.8.0a3/geofileops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:57:59.000000 geofileops-0.8.0a3/geofileops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-05 11:57:59.000000 geofileops-0.8.0a3/geofileops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-05 11:57:59.000000 geofileops-0.8.0a3/geofileops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 11:57:59.370919 geofileops-0.8.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:59.362919 geofileops-0.8.0a3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:59.370919 geofileops-0.8.0a3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   114688 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/BEFL-kbl.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/geofileops_testdata.qgz
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/linestring-row-trees.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)   765952 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/linestring-watercourse.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/linestrings_hedges.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)   106496 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/point.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)   139264 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/polygon-invalid.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/polygon-no-rows.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/polygon-overlappingcircles-all.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/polygon-overlappingcircles-one.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/polygon-overlappingcircles-two+three.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)   122880 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/polygon-parcel.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)   126976 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/polygon-simplify-onborder-testcase.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)   143360 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/polygon-twolayers.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/polygon-zone.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/polygonstyle.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/data/polygonstyle.sld
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_general_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    48459 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_geofile.py
--rw-r--r--   0 runner    (1001) docker     (123)    16948 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_geofileops_singlelayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    38479 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_geofileops_singlelayer_gpd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_geofileops_singlelayer_ogr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_geofileops_singlelayer_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)    38740 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_geofileops_twolayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_geofiletype.py
--rw-r--r--   0 runner    (1001) docker     (123)    25181 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_geometry_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11797 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_geoseries_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_grid_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_io_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_layerstyles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_ogr_sql_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_ogr_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_parameter_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_processing_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_spatialite.py
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_sqlite_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-05 11:57:46.000000 geofileops-0.8.0a3/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:33.961224 geofileops-0.8.0a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-10 09:08:33.961224 geofileops-0.8.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:33.945224 geofileops-0.8.0a4/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/benchmark/benchmark_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/benchmark/benchmark_geofileops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/benchmark/benchmarker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:33.945224 geofileops-0.8.0a4/benchmark/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/benchmark/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/benchmark/benchmarks/benchmarks_geofileops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/benchmark/benchmarks/testdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/benchmark/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:33.945224 geofileops-0.8.0a4/geofileops/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84479 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/fileops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91013 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/geoops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:33.949225 geofileops-0.8.0a4/geofileops/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/helpers/_parameter_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/helpers/layerstyles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:33.949225 geofileops-0.8.0a4/geofileops/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/_general_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71319 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/_geoops_gpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/_geoops_ogr.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101634 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/_geoops_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/_io_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/_ogr_sql_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18218 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/_ogr_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/_processing_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20519 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/_sqlite_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/geodataframe_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/geofiletype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/geofiletypes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    30024 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/geometry_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12178 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/geoseries_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/grid_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/test.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:33.945224 geofileops-0.8.0a4/geofileops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-10 09:08:33.000000 geofileops-0.8.0a4/geofileops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-10 09:08:33.000000 geofileops-0.8.0a4/geofileops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:08:33.000000 geofileops-0.8.0a4/geofileops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-10 09:08:33.000000 geofileops-0.8.0a4/geofileops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 09:08:33.000000 geofileops-0.8.0a4/geofileops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-10 09:08:33.961224 geofileops-0.8.0a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:33.953225 geofileops-0.8.0a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:33.961224 geofileops-0.8.0a4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   114688 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/BEFL-kbl.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/geofileops_testdata.qgz
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/linestring-row-trees.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)   765952 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/linestring-watercourse.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/linestrings_hedges.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)   106496 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/point.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)   139264 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/polygon-invalid.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/polygon-no-rows.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/polygon-overlappingcircles-all.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/polygon-overlappingcircles-one.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/polygon-overlappingcircles-two+three.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)   122880 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/polygon-parcel.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)   126976 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/polygon-simplify-onborder-testcase.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)   143360 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/polygon-twolayers.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/polygon-zone.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/polygonstyle.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/polygonstyle.sld
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_general_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48459 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_geofile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16948 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_geofileops_singlelayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38647 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_geofileops_singlelayer_gpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_geofileops_singlelayer_ogr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_geofileops_singlelayer_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38740 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_geofileops_twolayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_geofiletype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25181 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_geometry_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11797 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_geoseries_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_grid_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_io_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_layerstyles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_ogr_sql_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_ogr_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_parameter_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_processing_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_spatialite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_sqlite_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_version.py
```

### Comparing `geofileops-0.8.0a3/LICENSE.txt` & `geofileops-0.8.0a4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/PKG-INFO` & `geofileops-0.8.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geofileops
-Version: 0.8.0a3
+Version: 0.8.0a4
 Summary: Package to do spatial operations on large geo files.
 Home-page: https://github.com/geofileops/geofileops
 Author: Pieter Roggemans
 Author-email: pieter.roggemans@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `geofileops-0.8.0a3/README.md` & `geofileops-0.8.0a4/README.md`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/benchmark/benchmarker.py` & `geofileops-0.8.0a4/benchmark/benchmarker.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/benchmark/benchmarks/benchmarks_geofileops.py` & `geofileops-0.8.0a4/benchmark/benchmarks/benchmarks_geofileops.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/benchmark/benchmarks/testdata.py` & `geofileops-0.8.0a4/benchmark/benchmarks/testdata.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/benchmark/reporter.py` & `geofileops-0.8.0a4/benchmark/reporter.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/geofileops/fileops.py` & `geofileops-0.8.0a4/geofileops/fileops.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/geofileops/geoops.py` & `geofileops-0.8.0a4/geofileops/geoops.py`

 * *Files 0% similar despite different names*

```diff
@@ -469,17 +469,17 @@
             agg_columns={
                 "columns": [
                     {"column": "crop", "agg": "max", "as": "crop_max"},
                     {"column": "crop", "agg": "count", "as": "crop_count"},
                     {
                         "column": "crop",
                         "agg": "concat",
+                        "as": "crop_concat",
                         "distinct": True,
                         "sep": ";",
-                        "as": "crop_concat",
                     },
                     {"column": "area", "agg": "mean", "as": "area_mean"},
                 ]
             },
             explodecollections=False,
         )
 
@@ -530,26 +530,28 @@
                   be a list of dicts with the following keys:
 
                     - "column": column name (case insensitive) in the input file. In
                       addition to standard columns, it is also possible to specify
                       "fid", a unique index available in all input files.
                     - "agg": aggregation to use:
 
-                        - count: the number of items
-                        - sum:
-                        - mean
-                        - min
-                        - max
-                        - median
-                        - concat
+                        - count: the number of values in the group
+                        - sum: the sum of the values in the group
+                        - mean: the mean/average of the values in the group
+                        - min: the minimum value in the group
+                        - max: the maximum value in the group
+                        - median: the median value in the group
+                        - concat: all non-null values in the group concatenated (in
+                          arbitrary order)
 
                     - "as": column name in the output file. Note: using "fid" as alias
                       is not recommended: it can cause errors or odd behaviour.
                     - "distinct" (optional): True to distinct the values before
                       aggregation.
+                    - "sep" (optional): the separator to use for concat. Default: ",".
 
         tiles_path (PathLike, optional): a path to a geofile containing tiles.
             If specified, the output will be dissolved/unioned only within the
             tiles provided.
             Can be used to evade huge geometries being created if the input
             geometries are very interconnected.
             Defaults to None (= the output is not tiled).
```

### Comparing `geofileops-0.8.0a3/geofileops/helpers/_parameter_helper.py` & `geofileops-0.8.0a4/geofileops/helpers/_parameter_helper.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/geofileops/helpers/layerstyles.py` & `geofileops-0.8.0a4/geofileops/helpers/layerstyles.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pathlib import Path
+import sqlite3
 from typing import Optional
 
 from osgeo import gdal
 from osgeo import ogr
 import pandas as pd
 
 from geofileops import fileops
@@ -92,34 +93,35 @@
         styles_found = (
             layer_styles_df[["f_table_name", "styleName"]]
             .reset_index()
             .to_dict(orient="records")
         )
         raise ValueError(f"layer style exists already: {styles_found}")
 
+    # Insert style
+    conn = sqlite3.connect(path)
+    sql = """
+        INSERT INTO layer_styles (
+                id, f_table_catalog, f_table_schema, f_table_name,
+                f_geometry_column, styleName, styleQML, styleSLD, useAsDefault,
+                description, owner, ui
+            )
+            VALUES (NULL, '', '', ?, ?, ?, ?, ?, ?, ?, ?, ?)
+    """
     try:
-        datasource = gdal.OpenEx(str(path), nOpenFlags=gdal.OF_UPDATE)
-
-        sql = f"""
-            INSERT INTO layer_styles (
-                    id, f_table_catalog, f_table_schema, f_table_name,
-                    f_geometry_column, styleName, styleQML, styleSLD, useAsDefault,
-                    description, owner, ui
-                )
-                VALUES (
-                    NULL, '', '', '{layer}',
-                    'geom', '{name}', '{qml}', '{sld}', {use_as_default_str},
-                    '{description}', '{owner}', '{ui}'
-                )
-        """
-        result = datasource.ExecuteSQL(sql, dialect="SQLITE")
-        datasource.ReleaseResultSet(result)
-
+        conn.execute(
+            sql,
+            (layer, "geom", name, qml, sld, use_as_default_str, description, owner, ui),
+        )
+        conn.commit()
+    except Exception as ex:
+        conn.rollback()
+        raise Exception(f"Error {ex} executing {sql}") from ex
     finally:
-        datasource = None
+        conn.close()
 
 
 def remove_layerstyle(path: Path, id: int):
     """
     Remove a layer style.
 
     Only styles saved according to the QGIS Geopackage styling extension are removed:
```

### Comparing `geofileops-0.8.0a3/geofileops/util/_general_util.py` & `geofileops-0.8.0a4/geofileops/util/_general_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/geofileops/util/_geoops_gpd.py` & `geofileops-0.8.0a4/geofileops/util/_geoops_gpd.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/geofileops/util/_geoops_ogr.py` & `geofileops-0.8.0a4/geofileops/util/_geoops_ogr.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/geofileops/util/_geoops_sql.py` & `geofileops-0.8.0a4/geofileops/util/_geoops_sql.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/geofileops/util/_io_util.py` & `geofileops-0.8.0a4/geofileops/util/_io_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/geofileops/util/_ogr_sql_util.py` & `geofileops-0.8.0a4/geofileops/util/_ogr_sql_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/geofileops/util/_ogr_util.py` & `geofileops-0.8.0a4/geofileops/util/_ogr_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/geofileops/util/_processing_util.py` & `geofileops-0.8.0a4/geofileops/util/_processing_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/geofileops/util/_sqlite_util.py` & `geofileops-0.8.0a4/geofileops/util/_sqlite_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/geofileops/util/geodataframe_util.py` & `geofileops-0.8.0a4/geofileops/util/geodataframe_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/geofileops/util/geofiletype.py` & `geofileops-0.8.0a4/geofileops/util/geofiletype.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/geofileops/util/geofiletypes.csv` & `geofileops-0.8.0a4/geofileops/util/geofiletypes.csv`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/geofileops/util/geometry_util.py` & `geofileops-0.8.0a4/geofileops/util/geometry_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,19 @@
 import enum
 import logging
 import math
 from typing import List, Optional, Union
 
 import geopandas as gpd
 import numpy as np
-import pygeos
 import pyproj
 import shapely.coords as sh_coords
-import shapely.wkb as sh_wkb
 import shapely.geometry as sh_geom
 import shapely.ops as sh_ops
+import shapely.validation
 
 
 #####################################################################
 # First define/init some general variables/constants
 #####################################################################
 
 
@@ -355,17 +354,15 @@
 
     Returns:
         Optional[sh_geom.base.BaseGeometry]: The fixed geometry.
     """
     if geometry is None:
         return None
     else:
-        return sh_wkb.loads(
-            pygeos.io.to_wkb(pygeos.make_valid(pygeos.io.from_shapely(geometry)))
-        )
+        return shapely.validation.make_valid(geometry)
 
 
 def numberpoints(geometry: Optional[sh_geom.base.BaseGeometry]) -> int:
     """
     Calculates the total number of points in a geometry.
 
     Args:
```

### Comparing `geofileops-0.8.0a3/geofileops/util/geoseries_util.py` & `geofileops-0.8.0a4/geofileops/util/geoseries_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,22 @@
 Module containing utilities regarding operations on geoseries.
 """
 
 import logging
 from typing import List, Optional
 
 import geopandas as gpd
+import geopandas._compat as gpd_compat
 import numpy as np
 import pandas as pd
-import pygeos
+
+if gpd_compat.USE_PYGEOS:
+    import pygeos as shapely2_or_pygeos
+else:
+    import shapely as shapely2_or_pygeos
 from shapely import geometry as sh_geom
 
 from . import geometry_util
 from .geometry_util import GeometryType, PrimitiveType, SimplifyAlgorithm
 
 #####################################################################
 # First define/init some general variables/constants
@@ -122,65 +127,66 @@
         # Too difficult to harmonize, so just return
         return geoseries
 
 
 def is_valid_reason(geoseries: gpd.GeoSeries) -> pd.Series:
     # Get result and keep geoseries indexes
     return pd.Series(
-        data=pygeos.is_valid_reason(geoseries.array.data),  # type: ignore
+        data=shapely2_or_pygeos.is_valid_reason(geoseries.array.data),  # type: ignore
         index=geoseries.index,
     )
 
 
 def _harmonize_to_multitype(
     geoseries: gpd.GeoSeries, dest_geometrytype: GeometryType
 ) -> gpd.GeoSeries:
-    # Copy geoseries to pygeos array
+    # Copy geoseries data to new array
     geometries_arr = geoseries.array.data.copy()  # type: ignore
 
     # Set empty geometries to None
-    empty_idxs = pygeos.is_empty(geometries_arr)
+    empty_idxs = shapely2_or_pygeos.is_empty(geometries_arr)
     if empty_idxs.sum():
         geometries_arr[empty_idxs] = None
 
     # Cast all geometries that are not of the correct multitype yet
     # Remark: all rows need to be retained, so the same indexers exist in the
     # returned geoseries
     if dest_geometrytype is GeometryType.MULTIPOLYGON:
         # Convert polygons to multipolygons
-        single_idxs = pygeos.get_type_id(geometries_arr) == 3
+        single_idxs = shapely2_or_pygeos.get_type_id(geometries_arr) == 3
         if single_idxs.sum():
             geometries_arr[single_idxs] = np.apply_along_axis(
-                pygeos.multipolygons,
+                shapely2_or_pygeos.multipolygons,
                 arr=(np.expand_dims(geometries_arr[single_idxs], 1)),
                 axis=1,
             )
     elif dest_geometrytype is GeometryType.MULTILINESTRING:
         # Convert linestrings to multilinestrings
-        single_idxs = pygeos.get_type_id(geometries_arr) == 1
+        single_idxs = shapely2_or_pygeos.get_type_id(geometries_arr) == 1
         if single_idxs.sum():
             geometries_arr[single_idxs] = np.apply_along_axis(
-                pygeos.multilinestrings,
+                shapely2_or_pygeos.multilinestrings,
                 arr=(np.expand_dims(geometries_arr[single_idxs], 1)),
                 axis=1,
             )
     elif dest_geometrytype is GeometryType.MULTIPOINT:
-        single_idxs = pygeos.get_type_id(geometries_arr) == 0
+        single_idxs = shapely2_or_pygeos.get_type_id(geometries_arr) == 0
         if single_idxs.sum():
             geometries_arr[single_idxs] = np.apply_along_axis(
-                pygeos.multipoints,
+                shapely2_or_pygeos.multipoints,
                 arr=(np.expand_dims(geometries_arr[single_idxs], 1)),
                 axis=1,
             )
     else:
         raise Exception(f"Unsupported destination GeometryType: {dest_geometrytype}")
 
     # Prepare result to return
-    geoseries_result = geoseries.copy()
-    geoseries_result.array.data = geometries_arr  # type: ignore
+    geoseries_result = gpd.GeoSeries(
+        geometries_arr, index=geoseries.index, crs=geoseries.crs
+    )  # type: ignore
     assert isinstance(geoseries_result, gpd.GeoSeries)
     return geoseries_result
 
 
 def polygons_to_lines(geoseries: gpd.GeoSeries) -> gpd.GeoSeries:
     polygons_lines = []
     for geom in geoseries:
@@ -263,24 +269,26 @@
                 or list(topoline_simpl[-1]) != topo.output["arcs"][index][-1]
             ):
                 # Start or end point of the simplified version is not the same anymore
                 continue
             else:
                 topo.output["arcs"][index] = list(topoline_simpl)
 
-    topo_simpl_geoseries = topo.to_gdf(crs=geoseries.crs).geometry
-    topo_simpl_geoseries.array.data = pygeos.make_valid(topo_simpl_geoseries.array.data)
+    topo_simpl_gdf = topo.to_gdf(crs=geoseries.crs)
+    topo_simpl_gdf.geometry = shapely2_or_pygeos.make_valid(
+        topo_simpl_gdf.geometry.array.data
+    )
     geometry_types_orig = geoseries.geom_type.unique()
-    geometry_types_simpl = topo_simpl_geoseries.geom_type.unique()
+    geometry_types_simpl = topo_simpl_gdf.geometry.geom_type.unique()
     if len(geometry_types_orig) == 1 and len(geometry_types_simpl) > 1:
-        topo_simpl_geoseries = geometry_collection_extract(
-            topo_simpl_geoseries,
+        topo_simpl_gdf.geometry = geometry_collection_extract(
+            topo_simpl_gdf.geometry,
             GeometryType(geometry_types_orig[0]).to_primitivetype,
         )
-    return topo_simpl_geoseries
+    return topo_simpl_gdf.geometry
 
 
 def simplify_ext(
     geoseries: gpd.GeoSeries,
     tolerance: float,
     algorithm: SimplifyAlgorithm = SimplifyAlgorithm.RAMER_DOUGLAS_PEUCKER,
     lookahead: int = 8,
```

### Comparing `geofileops-0.8.0a3/geofileops/util/grid_util.py` & `geofileops-0.8.0a4/geofileops/util/grid_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/geofileops/util/test.gpkg` & `geofileops-0.8.0a4/geofileops/util/test.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/geofileops.egg-info/PKG-INFO` & `geofileops-0.8.0a4/geofileops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geofileops
-Version: 0.8.0a3
+Version: 0.8.0a4
 Summary: Package to do spatial operations on large geo files.
 Home-page: https://github.com/geofileops/geofileops
 Author: Pieter Roggemans
 Author-email: pieter.roggemans@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `geofileops-0.8.0a3/geofileops.egg-info/SOURCES.txt` & `geofileops-0.8.0a4/geofileops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/setup.py` & `geofileops-0.8.0a4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,18 @@
     url="https://github.com/geofileops/geofileops",
     include_package_data=True,
     packages=setuptools.find_packages(),
     install_requires=[
         "cloudpickle",
         "fiona",
         "gdal",
-        "geopandas>=0.11,<1.0",
+        "geopandas>=0.11,<1",
         "numpy",
         "pandas",
         "psutil",
-        "pygeos",
         "pyogrio",
         "pyproj",
         "shapely",
         "topojson",
     ],
     extras_require={"full": ["simplification"]},
     classifiers=[
```

### Comparing `geofileops-0.8.0a3/tests/data/BEFL-kbl.gpkg` & `geofileops-0.8.0a4/tests/data/BEFL-kbl.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/data/geofileops_testdata.qgz` & `geofileops-0.8.0a4/tests/data/geofileops_testdata.qgz`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/data/linestring-row-trees.gpkg` & `geofileops-0.8.0a4/tests/data/linestring-row-trees.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/data/linestring-watercourse.gpkg` & `geofileops-0.8.0a4/tests/data/linestring-watercourse.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/data/linestrings_hedges.gpkg` & `geofileops-0.8.0a4/tests/data/linestrings_hedges.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/data/point.gpkg` & `geofileops-0.8.0a4/tests/data/point.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/data/polygon-invalid.gpkg` & `geofileops-0.8.0a4/tests/data/polygon-invalid.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/data/polygon-no-rows.gpkg` & `geofileops-0.8.0a4/tests/data/polygon-no-rows.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/data/polygon-overlappingcircles-all.gpkg` & `geofileops-0.8.0a4/tests/data/polygon-overlappingcircles-all.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/data/polygon-overlappingcircles-one.gpkg` & `geofileops-0.8.0a4/tests/data/polygon-overlappingcircles-one.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/data/polygon-overlappingcircles-two+three.gpkg` & `geofileops-0.8.0a4/tests/data/polygon-overlappingcircles-two+three.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/data/polygon-parcel.gpkg` & `geofileops-0.8.0a4/tests/data/polygon-parcel.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/data/polygon-simplify-onborder-testcase.gpkg` & `geofileops-0.8.0a4/tests/data/polygon-simplify-onborder-testcase.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/data/polygon-twolayers.gpkg` & `geofileops-0.8.0a4/tests/data/polygon-twolayers.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/data/polygon-zone.gpkg` & `geofileops-0.8.0a4/tests/data/polygon-zone.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/data/polygonstyle.qml` & `geofileops-0.8.0a4/tests/data/polygonstyle.qml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 3c21 444f 4354 5950 4520 7167 6973 2050  <!DOCTYPE qgis P
-00000010: 5542 4c49 4320 2268 7474 703a 2f2f 6d72  UBLIC "http://mr
-00000020: 6363 2e63 6f6d 2f71 6769 732e 6474 6422  cc.com/qgis.dtd"
-00000030: 2022 5359 5354 454d 223e 0a3c 7167 6973   "SYSTEM">.<qgis
+00000010: 5542 4c49 4320 2768 7474 703a 2f2f 6d72  UBLIC 'http://mr
+00000020: 6363 2e63 6f6d 2f71 6769 732e 6474 6427  cc.com/qgis.dtd'
+00000030: 2027 5359 5354 454d 273e 0a3c 7167 6973   'SYSTEM'>.<qgis
 00000040: 2073 696d 706c 6966 7944 7261 7769 6e67   simplifyDrawing
 00000050: 4869 6e74 733d 2231 2220 7265 6164 4f6e  Hints="1" readOn
 00000060: 6c79 3d22 3022 206c 6162 656c 7345 6e61  ly="0" labelsEna
 00000070: 626c 6564 3d22 3022 2073 696d 706c 6966  bled="0" simplif
 00000080: 794c 6f63 616c 3d22 3122 206d 6178 5363  yLocal="1" maxSc
 00000090: 616c 653d 2230 2220 6d69 6e53 6361 6c65  ale="0" minScale
 000000a0: 3d22 3130 3030 3030 3030 3022 2073 696d  ="100000000" sim
```

### Comparing `geofileops-0.8.0a3/tests/data/polygonstyle.sld` & `geofileops-0.8.0a4/tests/data/polygonstyle.sld`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text, with very long lines (358)*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
-00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
-00000020: 462d 3822 3f3e 0a3c 5374 796c 6564 4c61  F-8"?>.<StyledLa
+00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2731  <?xml version='1
+00000010: 2e30 2720 656e 636f 6469 6e67 3d27 5554  .0' encoding='UT
+00000020: 462d 3827 3f3e 0a3c 5374 796c 6564 4c61  F-8'?>.<StyledLa
 00000030: 7965 7244 6573 6372 6970 746f 7220 786d  yerDescriptor xm
 00000040: 6c6e 733d 2268 7474 703a 2f2f 7777 772e  lns="http://www.
 00000050: 6f70 656e 6769 732e 6e65 742f 736c 6422  opengis.net/sld"
 00000060: 2078 6d6c 6e73 3a6f 6763 3d22 6874 7470   xmlns:ogc="http
 00000070: 3a2f 2f77 7777 2e6f 7065 6e67 6973 2e6e  ://www.opengis.n
 00000080: 6574 2f6f 6763 2220 786d 6c6e 733a 786c  et/ogc" xmlns:xl
 00000090: 696e 6b3d 2268 7474 703a 2f2f 7777 772e  ink="http://www.
```

### Comparing `geofileops-0.8.0a3/tests/test_general_util.py` & `geofileops-0.8.0a4/tests/test_general_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/test_geofile.py` & `geofileops-0.8.0a4/tests/test_geofile.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/test_geofileops_singlelayer.py` & `geofileops-0.8.0a4/tests/test_geofileops_singlelayer.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/test_geofileops_singlelayer_gpd.py` & `geofileops-0.8.0a4/tests/test_geofileops_singlelayer_gpd.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,20 +331,20 @@
     output_gdf = gfo.read_file(output_path)
     assert input_gdf.crs == output_gdf.crs
     assert len(output_gdf) == output_layerinfo.featurecount
     assert output_gdf["geometry"][0] is not None
 
     # Some more default checks for NISCODE 12009
     niscode_idx = output_gdf[output_gdf["NIScode"] == "12009"].index.item()
+    fid_concat_result = sorted(output_gdf["fid_concat"][niscode_idx].split(","))
     if gfo.GeofileType(input_path).is_fid_zerobased:
-        assert output_gdf["fid_concat"][niscode_idx] == "38,42,44,54"
+        assert fid_concat_result == ["38", "42", "44", "54"]
     else:
-        assert output_gdf["fid_concat"][niscode_idx] == "39,43,45,55"
+        assert fid_concat_result == ["39", "43", "45", "55"]
     assert output_gdf["naam_MAX"][niscode_idx] == "Vosbergbeek"
-    # TODO: add more in depth check of result
 
 
 @pytest.mark.parametrize("agg_columns", [{"json": ["fid", "NaaM"]}, {"json": None}])
 def test_dissolve_linestrings_aggcolumns_json(tmp_path, agg_columns):
     # Prepare test data
     input_path = test_helper.get_testfile("linestring-watercourse")
     output_basepath = tmp_path / f"{input_path.stem}-output.gpkg"
@@ -386,22 +386,27 @@
     assert output_gdf["geometry"][0] is not None
 
     # Some more default checks for NISCODE 12009
     niscode_idx = output_gdf[output_gdf["NIScode"] == "12009"].index.item()
     json_value = json.loads(str(output_gdf["json"][niscode_idx]))
 
     # Check NAAM
-    naam_str = ",".join([value["NAAM"] for value in json_value])
-    exp = "Duffelse en Rumstse Scheibeek,Vosbergbeek,Maltaveldenloop,Grote Nete"
-    assert naam_str == exp
-    fid_str = ",".join([str(value["fid_orig"]) for value in json_value])
+    naam_result = sorted([value["NAAM"] for value in json_value])
+    exp = [
+        "Duffelse en Rumstse Scheibeek",
+        "Grote Nete",
+        "Maltaveldenloop",
+        "Vosbergbeek",
+    ]
+    assert naam_result == exp
+    fid_result = sorted([str(value["fid_orig"]) for value in json_value])
     if gfo.GeofileType(input_path).is_fid_zerobased:
-        assert fid_str == "38,42,44,54"
+        assert fid_result == ["38", "42", "44", "54"]
     else:
-        assert fid_str == "39,43,45,55"
+        assert fid_result == ["39", "43", "45", "55"]
 
     # Some specific tests depending on whether all columns asked or not
     if agg_columns["json"] is None:
         # fid_orig is added to json
         assert len(json_value[0]) == len(input_layerinfo.columns) + 1
     else:
         # fid_orig is added to json
@@ -834,18 +839,19 @@
     ].index.to_list()[0]
     assert output_gdf["lbl_count"][groenten_idx] == 5
     print(
         "groenten.lblhfdtlt_concat_distinct: "
         "f{output_gdf['lbl_conc_d'][groenten_idx]}"
     )
     assert output_gdf["lbl_cnt_d"][groenten_idx] == 4
+    fid_concat_result = sorted(output_gdf["fid_concat"][groenten_idx].split(","))
     if gfo.GeofileType(input_path).is_fid_zerobased:
-        assert output_gdf["fid_concat"][groenten_idx] == "41,42,43,44,45"
+        assert fid_concat_result == ["41", "42", "43", "44", "45"]
     else:
-        assert output_gdf["fid_concat"][groenten_idx] == "42,43,44,45,46"
+        assert fid_concat_result == ["42", "43", "44", "45", "46"]
 
 
 @pytest.mark.parametrize(
     "agg_columns", [{"json": ["lengte", "oppervl", "lblhfdtlt"]}, {"json": None}]
 )
 def test_dissolve_polygons_aggcolumns_json(tmp_path, agg_columns):
     # In shapefiles, the length of str columns is very limited, so the json
```

### Comparing `geofileops-0.8.0a3/tests/test_geofileops_singlelayer_ogr.py` & `geofileops-0.8.0a4/tests/test_geofileops_singlelayer_ogr.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/test_geofileops_singlelayer_sql.py` & `geofileops-0.8.0a4/tests/test_geofileops_singlelayer_sql.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/test_geofileops_twolayers.py` & `geofileops-0.8.0a4/tests/test_geofileops_twolayers.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/test_geofiletype.py` & `geofileops-0.8.0a4/tests/test_geofiletype.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/test_geometry_util.py` & `geofileops-0.8.0a4/tests/test_geometry_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/test_geoseries_util.py` & `geofileops-0.8.0a4/tests/test_geoseries_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/test_grid_util.py` & `geofileops-0.8.0a4/tests/test_grid_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/test_helper.py` & `geofileops-0.8.0a4/tests/test_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,21 @@
 
 from pathlib import Path
 import tempfile
 from typing import Optional, Union
 import sys
 
 import geopandas as gpd
+import geopandas._compat as gpd_compat
 import geopandas.testing as gpd_testing
-import pygeos
+
+if gpd_compat.USE_PYGEOS:
+    import pygeos as shapely2_or_pygeos
+else:
+    import shapely as shapely2_or_pygeos
 import shapely.geometry as sh_geom
 
 # Add path so the local geofileops packages are found
 sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
 import geofileops as gfo
 from geofileops.util import geodataframe_util
 from geofileops.util import geoseries_util
@@ -237,16 +242,20 @@
     """
     if sort_columns:
         left = left[sorted(left.columns)]
         right = right[sorted(right.columns)]
 
     if sort_values:
         if normalize:
-            left.geometry = gpd.GeoSeries(pygeos.normalize(left.geometry.array.data))
-            right.geometry = gpd.GeoSeries(pygeos.normalize(right.geometry.array.data))
+            left.geometry = gpd.GeoSeries(
+                shapely2_or_pygeos.normalize(left.geometry.array.data)
+            )
+            right.geometry = gpd.GeoSeries(
+                shapely2_or_pygeos.normalize(right.geometry.array.data)
+            )
         if promote_to_multi:
             left.geometry = geoseries_util.harmonize_geometrytypes(
                 left.geometry, force_multitype=True
             )
             right.geometry = geoseries_util.harmonize_geometrytypes(
                 right.geometry, force_multitype=True
             )
```

### Comparing `geofileops-0.8.0a3/tests/test_io_util.py` & `geofileops-0.8.0a4/tests/test_io_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/test_layerstyles.py` & `geofileops-0.8.0a4/tests/test_layerstyles.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/test_ogr_sql_util.py` & `geofileops-0.8.0a4/tests/test_ogr_sql_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/test_ogr_util.py` & `geofileops-0.8.0a4/tests/test_ogr_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/test_parameter_helper.py` & `geofileops-0.8.0a4/tests/test_parameter_helper.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/test_processing_util.py` & `geofileops-0.8.0a4/tests/test_processing_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/test_spatialite.py` & `geofileops-0.8.0a4/tests/test_spatialite.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a3/tests/test_sqlite_util.py` & `geofileops-0.8.0a4/tests/test_sqlite_util.py`

 * *Files identical despite different names*

